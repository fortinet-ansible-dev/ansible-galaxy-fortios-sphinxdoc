
Frequently Asked Questions (FAQ)
================================

|

**TABLE OF CONTENTS:**
 - `What's Access Token?`_
 - `How To Backup And Restore FOS?`_
 - `How To Import A License?`_
 - `How does Ansible work with login banner?`_
 - `How To Work With Raw FotiOS CLI?`_
 - `How to use the set_fact module in a task?`_
 - `How to use the member operation to add an element in an object?`_
 - `Set up FortiToken multi-factor authentication`_
 - `Avoid using the special placeholder 0 as the mkey in some modules`_
 - `Resolution for Ansible Always Sending GET/PUT Requests as POST Requests`_

What's Access Token?
~~~~~~~~~~~~~~~~~~~~

Access Token here is an API token which is used to authenticate an API request, an api token is associated with an API user once generated in FortiOS.
FortiOS Ansible supports api token based authentication, please see `Run Your Playbook`_ for how to use ``access_token`` in Ansible playbook.

Sometimes we also want to dynamically generate an API token via FortiOS ansible module, we have a demo to show how to generate an API token:

::

   # to customize privileges for the API user, we can also define an accprofile via module fortios_system_accprofile.
   - name: Create An API User if not present
     fortios_system_api_user:
        vdom: 'root'
        state: 'present'
        system_api_user:
            name: 'AnsibleAPIUser'
            accprofile: 'super_admin' # This is predefined privilege profile.
            vdom:
               - name: 'root'
            trusthost:
                - id: '1'
                  ipv4_trusthost: '192.168.190.0 255.255.255.0'

   # To reference the generated token, we can use notation "{{ tokeninfo.meta.results.access_token  }}" to keep it somewhere in disk.
   - name: Generate The API token
     fortios_monitor:
        vdom: 'root'
        selector: 'generate-key.system.api-user'
        params:
            api-user: 'AnsibleAPIUser'
     register: tokeninfo


How To Backup And Restore FOS?
~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~

Legacy module ``fortios_system_config_backup_restore`` is deprecated since 2.0.0, new modules are available for doing equivalent jobs.
New modules are desined to be very flexible, that requires us to combine modules to do complex task.

**Note: operation backup and restore needs administrative privilege, better not choose access token based authentication.**


Backup settings to local file.
...........................................

FortiOS Ansible collection doesn't provide any modules for local file operations, here we use builtin ``copy`` module to copy plain configuration text into a file.

::

   - name: Backup a virtual domain.
     fortios_monitor_fact:
        selector: 'system_config_backup'
        vdom: 'root'
        params:
            scope: 'global'
     register: backupinfo

   - name: Save the backup information.
     copy:
        content: '{{ backupinfo.meta.raw }}'
        dest: './local.backup'


Restore settings from local file.
..................................

FortiOS only accepts base64 encoded text, the configuration text must be encoded before being uploaded.


::

   - name: Restore from file.
     fortios_monitor:
        selector: 'restore.system.config'
        vdom: 'root'
        params:
            scope: 'global'
            source: 'upload'
            vdom: 'root'
            file_content: "{{ lookup( 'file', './local.backup') | string | b64encode }}"

Restore settings from other sources.
....................................

no matter what source is, just make sure content is encoded.

::

   - name: Backup a virtual domain.
     fortios_monitor_fact:
        selector: 'system_config_backup'
        vdom: 'root'
        params:
            scope: 'global'
     register: backupinfo

   - name: Restore from intermediate result.
     fortios_monitor:
        selector: 'restore.system.config'
        vdom: 'root'
        params:
            scope: 'global'
            source: 'upload'
            vdom: 'root'
            file_content: "{{ backupinfo.meta.raw | string | b64encode}}"



For more options to restore, see module ``fortios_monitor`` and its selector ``restore.system.config``,
for more options to backup, see module ``fortios_monitor_fact`` and its selector ``system_config_backup``.

How To Import A License?
~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~

Import a license for a newly installed FOS instance.
......................................................

Make sure the active management port allows access to http service by setting ``allowaccess``.

::

    FortiGate-VM64 # show system interface port1
    config system interface
    edit "port1"
        set vdom "root"
        set mode dhcp
        set allowaccess ping https ssh http fgfm
        set type physical
        set snmp-index 1
    next
    end

Then run the following playbook to upload licence for the first time:

::

   - hosts: fortigate_new
     connection: httpapi
     collections:
      - fortinet.fortios
     vars:
      vdom: "root"
      ansible_httpapi_use_ssl: true
      ansible_httpapi_validate_certs: false
      ansible_httpapi_port: 443
     tasks:

      - name: Upload the license to the newly installed FGT device
        fortios_monitor:
            vdom: "{{ vdom }}"
            selector: 'upload.system.vmlicense'
            params:
                file_content: "{{ lookup( 'file', './FGVM02TM20012347.lic') | string | b64encode }}"
        ignore_errors: True

In the example, we put license file ``FGVM02TM20012347.lic`` under current working directory.

Once FOS accepts a valid licence, it reboots immediately and the connection terminates suddenly, as a result, we must not regard connection timeout as errors, we'd better ignore connection timeout exception.
and the default connection timeout is 30 seconds, better make it smaller.

**Access token based authentication is not allowed in initial license import**

Renew a license for a licence-ready FOS instance.
......................................................

To renew the license for a running FOS instance, we don't have to use http service (by default, after license is activated, http service is redirected to https service, which causes problems for Ansible).
by setting ``ansible_httpapi_use_ssl`` to ``true`` and ``ansible_httpapi_port`` to ``443``, the task can normally upload the license.


**Renewing a license can use access token based authentication as long as associated API user has admin privilege to upload license.**

How does Ansible work with login banner?
~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~

what's login banner?
............................

FOS puts a barrier in login process if pre- and(or) post- login bannner are enabled, and ansible authentication is restricted: **only access token based authentication is allowed**.

How to safely generate access token?
........................................................

For Ansible FOS login banner usage, there could be a ``deadlock`` if one the of following cases apprears:

 - I don't have an API user or access token.
 - I have an access token but it has expired.

upon such deadlocks, there is no other way but to disable banners and (re)generate one.

To generate an access token in advance, please see `How To Generate Access Token Dynamically`_, and please do token generation with Ansible with all the login banners disabled(it's not necessay to disable banners if we generate access token from WEB UI).

::

    FGVM02TM20012347 # config system global
    FGVM02TM20012347 (global) # set post-login-banner disable
    FGVM02TM20012347 (global) # set pre-login-banner disable
    FGVM02TM20012347 (global) # end
    FGVM02TM20012347 #



where to keep generated access token?
..................................................

Normally if we generate an access token from WEB UI, we may put it in inventory file as below:

::

    [fortigates]
    fortigate01 enable_log=True ansible_host=YOUR_HOST_IP_ADDRESS

    [fortigates:vars]
    ansible_network_os=fortinet.fortios.fortios
    ansible_persistent_log_messages=True
    ansible_log_path=/tmp/ansible.network.log
    ansible_user=YOUR_USERNAME
    ansible_password=YOUR_PASSWORD
    ansible_httpapi_session_key={"access_token":"YOUR_OWN_TOKEN"}


we can encrypt the inventory file through ansible tool ``ansible-vault``, thus avoiding token leaks.

To automate token (re)generation, we might also want to keep it somewhere else in local storage. An example is given below to show how to save and re-use a token later:

::

   - name: Generate The API token
     fortios_monitor:
        vdom: 'root'
        selector: 'generate-key.system.api-user'
        params:
            api-user: 'AnsibleAPIUser'
     register: tokeninfo

   - name: Save the API token
     copy:
        content: "{{ tokeninfo.meta.results.access_token }}"
        dest: './access_token.save'


**Caveats: saved access token is not guarded by Ansible, once leaked, others may access the FOS illegally. one way to restrict illegal access is to limit source localtion in ipv4_trusthost during creating the API users.**

How To Work With Raw FotiOS CLI?
~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~

In FortiOS, some CLI commands are not exported as RestAPI, as a reasult, Ansible FortiOS collection has no identical module for those CLI commands.
And FortiOS default CLI shell is not a standard Unix shell, so Ansible builtin modules like ``shell`` and ``command`` are of no use.
To work this around in Ansible, we use a verbose but very efficient and flexible way to execute some FortiOS CLI commands from Ansible.


Below are two examples of the template:

**Append a firewall address member to a group using append command:**

::

 - hosts: localhost
   vars:
     # ======================== Below are crenditials to connect to Fortigate Device========
     fgt_host: '192.168.190.171'
     fgt_user: 'admin'
     fgt_pass: 'password'

     firewall_group_name: 'firwalladdressgroup0'
     firewall_address_name: 'firewalladdress0'
     # =====================================================================================
     script_path: '/tmp/fgt.shell.task'
   tasks:
    - name: Prepare The Shell Scrit Template.
      raw: |
             cat > {{script_path }} << EOF_OUTER
             # /bin/bash
             # Please make sure tool sshpass is installed. e.g. on Debian/Ubuntu, apt-get install sshpass.
             # Optionally you can pass some parameters.
             # The character `a` at second line below is to avoid post-login-banner barrier.
             sshpass -p '{{ fgt_pass }}' ssh -o StrictHostKeyChecking=no {{ fgt_user }}@{{ fgt_host }} <<EOF
             a
             # ====================== Edit Your Commands Below =============================================
             config firewall addrgrp
             edit '\$1'
             append member '\$2'
             end
             # ==============================================================================================
             EOF
             EOF_OUTER


    - name: Execute The Cli Commands.
      raw: |
             chmod +x {{ script_path }} && {{ script_path }} '{{ firewall_group_name }}' '{{ firewall_address_name }}'
      args:
        executable: /bin/bash

**Enable/Disable pre-/post- login banners**

::

 - hosts: localhost
   vars:
     # ======================== Below are crenditials to connect to Fortigate Device========
     fgt_host: '192.168.190.171'
     fgt_user: 'admin'
     fgt_pass: 'password'
     # =====================================================================================
     script_path: '/tmp/fgt.shell.task'
   tasks:
    - name: Prepare The Shell Scrit Template.
      raw: |
             cat > {{script_path }} << EOF_OUTER
             # /bin/bash
             # Please make sure tool sshpass is installed. e.g. on Debian/Ubuntu, apt-get install sshpass.
             # Optionally you can pass some parameters.
             # The character `a` at second line below is to avoid post-login-banner barrier.
             sshpass -p '{{ fgt_pass }}' ssh -o StrictHostKeyChecking=no {{ fgt_user }}@{{ fgt_host }} <<EOF
             a
             # ====================== Edit Your Commands Below =============================================
             config system global
             set pre-login-banner '\${1:-disbale}'
             set post-login-banner '\${2:-disable}'
             end
             # ==============================================================================================
             EOF
             EOF_OUTER


    - name: Execute The Cli Commands, e.g. enable pre- and post- login banner.
      raw: |
             chmod +x {{ script_path }} && {{ script_path }} enable enable
      args:
        executable: /bin/bash

How to use the set_fact module in a task?
~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~

In Ansible, there's an important module that works with variables and is used to get or set variable values, which is ``set_fact``.
This module is used to set new variables and these variables are available to subsequent plays in a playbook.
Using set_fact, we can store the value after preparing it on the fly using certain task.

The following example will show you how set_fact module can be used in a task to configure the firewall address group.

**Configuring the firewall address group with a string type of variable that contains all the grouped firewall addresses:**

::

  - hosts: fortigateslab
    connection: httpapi
    collections:
      - fortinet.fortios
    vars:
      vdom: 'root'
      ansible_httpapi_use_ssl: true
      ansible_httpapi_validate_certs: false
      ansible_httpapi_port: 443
      demo_input: 'login.microsoftonline.com, login.microsoft.com, login.windows.net'
      demo_members: []
    tasks:
      - name: Process input content
        set_fact:
          demo_members: "{{ demo_members + [{'name': item.strip(' ')}] }}"
        with_items:
          - "{{demo_input.split(',')}}"

      - debug:
          var: demo_members

      - name: Configure Firewall Schedule Recurring
        fortios_firewall_addrgrp:
          vdom:  '{{ vdom }}'
          state: 'present'
          enable_log: True
          firewall_addrgrp:
            name: 'group_1'
            comment: 'created via Ansible'
            visibility: 'enable'
            member: '{{ demo_members }}'

In the example, the first task is preprocessing the input content.
Specifically, it splits the input content with comma to get a list of the firewall addresses.
Then it appends the each address to the variable demo_members.
So the demo_members variable can be assigned to the variable members in the subsequent play.

How to use the member operation to add an element in an object?
~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~

Member operation is used to add an element to an existing object. The example below will show you how to use it.

::

  - hosts: fortigateslab
    connection: httpapi
    collections:
      - fortinet.fortios
    vars:
      ansible_httpapi_use_ssl: true
      ansible_httpapi_validate_certs: false
      ansible_httpapi_port: 443
    tasks:
    - name: Add an dns entry in the existing obj.
      fortios_system_dns_database:
        state: "present"
        member_state: "present"
        member_path: "dns_entry:id"
        system_dns_database:
          name: 1
          dns_entry:
            - id: 1
              hostname: xyz.com
              ip: 8.8.8.9
            - id: 2
              hostname: abc.com
              ip: 7.7.7.8

Set up FortiToken multi-factor authentication
~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~

It uses one of the two free mobile FortiTokens that is already installed on the FortiGate.

::

  tasks:
  - name: To configure MFA.
    fortios_user_local:
      enable_log: true
      vdom:  "{{ vdom }}"
      state: "present"
      user_local:
        auth_concurrent_override: "enable"
        auth_concurrent_value: "0"
        authtimeout: "0"
        email_to: "abc@gmail.com"
        fortitoken: "FTKMOB324C29689B"
        id:  "8"
        name: "test_user"
        status: "enable"
        two_factor: "fortitoken"
        two_factor_authentication: "fortitoken"
        two_factor_notification: "email"
        type: "password"
        username_case_sensitivity: "disable"
        username_sensitivity: "disable"

  - name: Activate the mobile token
    fortios_monitor:
      vdom: "root"
      selector: "send-activation.user.fortitoken"
      params:
        token: FTKMOB324C29689B
        method: email
        email: abc@gmail.com

Avoid using the special placeholder 0 as the mkey in some modules
~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~

While '0' is a special placeholder that allows the backend to assign the latest available number for the entity, it does have limitations, for example, when you create a new router_static entity that has the identical configurations with an existing one, if the 'seq_num' is '0' or seq_num is absent, there will be an error thrown out from the backend and complain "duplicate entry already exists". Also, it's required to provide the mkey when updating or deleting an entity. Therefore, using your own value for this purpose to avoid any potential issues in the future.

::

  tasks:
  - name: Configuring Static Routing 1
    fortios_router_static:
      enable_log: true
      state: present
      router_static:
        seq_num: 1
        dst: "180.0.1.11/32"
        gateway: "192.168.0.1"
        device: "port1"
        status: "enable"
        distance: 10

  - name: Update the distance parameter
    fortios_router_static:
      enable_log: true
      state: present
      router_static:
        seq_num: 1
        distance: 15

  - name: Delete the specific router static entity
    fortios_router_static:
      enable_log: true
      state: absent
      router_static:
        seq_num: 1

Resolution for Ansible Always Sending GET/PUT Requests as POST Requests
~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~

We have been inundated with complaints regarding older Ansible versions consistently sending GET/PUT requests as POST requests due to a bug in the ansible.netcommon module. To prevent such issues, please ensure that you have installed the latest Ansible version.

To upgrade to the latest version of ansible.netcommon, use the following command:
ansible-galaxy collection install ansible.netcommon --force

.. _Run Your Playbook: playbook.html
.. _How To Generate Access Token Dynamically: faq.html#what-s-access-token

