
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

|

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

   # To reference the generated token, we can use notation "{{ tokeninfo.meta.results.access_token  }}"in further tasks or keep it somewhere in disk.
   - name: Generate The API token
     fortios_monitor:
        vdom: 'root'
        selector: 'generate-key.system.api-user'
        params:
            api-user: 'AnsibleAPIUser'
     register: tokeninfo

   - name: do another api request with newly generated access_token
     fortios_configuration_fact:
        access_token: "{{ tokeninfo.meta.results.access_token  }}"
        vdom: 'root'
        selector: 'system_status'



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
      ansible_httpapi_use_ssl: no
      ansible_httpapi_validate_certs: no
      ansible_httpapi_port: 80
      ansible_command_timeout: 5
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
by setting ``ansible_httpapi_use_ssl`` to ``True`` and ``ansible_httpapi_port`` to ``443``, the task can normally upload the license.


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

Normally if we generate an access token from WEB UI, we may put it in inventory file as a variable ``fortios_access_token``:

::

    [fortigates]
    fortigate01 ansible_host=<the address of the host> fortios_access_token=<the access token>


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

then in subsequent tasks, we read the token directly from saved file:

::

   vars:
    vdom: "root"
    ansible_httpapi_use_ssl: yes
    ansible_httpapi_validate_certs: no
    ansible_httpapi_port: 443
    saved_access_token: "{{ lookup( 'file', './access_token.save') | string }}"

   tasks:
    - name: do another api request with saved access_token
      fortios_configuration_fact:
        access_token: "{{ saved_access_token }}"
        vdom: 'root'
        selector: 'system_status'

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
      ansible_httpapi_use_ssl: yes
      ansible_httpapi_validate_certs: no
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
          access_token: '{{ fortios_access_token }}'
          firewall_addrgrp:
            name: 'group_1'
            comment: 'created via Ansible'
            visibility: 'enable'
            member: '{{ demo_members }}'

In the example, the first task is preprocessing the input content.
Specifically, it splits the input content with comma to get a list of the firewall addresses.
Then it appends the each address to the variable demo_members.
So the demo_members variable can be assigned to the variable members in the subsequent play.


.. _Run Your Playbook: playbook.html
.. _How To Generate Access Token Dynamically: faq.html#what-s-access-token

