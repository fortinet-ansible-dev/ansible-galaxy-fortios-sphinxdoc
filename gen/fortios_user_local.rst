:source: fortios_user_local.py

:orphan:

.. _fortios_user_local:

fortios_user_local -- Configure local users in Fortinet's FortiOS and FortiGate.
++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++

.. versionadded:: 2.9

.. contents::
   :local:
   :depth: 1


Synopsis
--------
- This module is able to configure a FortiGate or FortiOS (FOS) device by allowing the user to set and modify user feature and local category. Examples include all parameters and values need to be adjusted to datasources before usage. Tested with FOS v6.0.5


Requirements
------------
The below requirements are needed on the host that executes this module.

- fortiosapi>=0.9.8


Parameters
----------

.. raw:: html

    <ul>

    <li><span class="li-head">host</span> - FortiOS or FortiGate IP address. <span class="li-normal">type: str</span> <span class="li-required">required: false</span></li>
    <li><span class="li-head">username</span> - FortiOS or FortiGate username. <span class="li-normal">type: str</span> <span class="li-required">required: false</span></li>
    <li><span class="li-head">password</span> - FortiOS or FortiGate password. <span class="li-normal">type: str</span> <span class="li-normal">default: ""</span></li>
    <li><span class="li-head">vdom</span> - Virtual domain, among those defined previously. A vdom is a virtual instance of the FortiGate that can be configured and used as a different unit. <span class="li-normal">type: str</span> <span class="li-normal">default: root</span></li>
    <li><span class="li-head">https</span> - Indicates if the requests towards FortiGate must use HTTPS protocol. <span class="li-normal">type: bool</span> <span class="li-normal">default: true</span></li>
    <li><span class="li-head">ssl_verify</span> - Ensures FortiGate certificate must be verified by a proper CA. <span class="li-normal">type: bool</span> <span class="li-normal">default: true</span></li>
    <li><span class="li-head">state</span> - Indicates whether to create or remove the object. <span class="li-normal">type: str</span> <span class="li-required">required</span> <span class="li-normal">choices: present,  absent</span></li>
    <li><span class="li-head">user_local</span> - Configure local users. <span class="li-normal">default: null</span> <span class="li-normal">type: dict</span></li>
            <ul class="ul-self">

            <li><span class="li-head">auth_concurrent_override</span> - Enable/disable overriding the policy-auth-concurrent under config system global. <span class="li-normal">type: str</span> <span class="li-normal">choices: enable,  disable</span></li>
            <li><span class="li-head">auth_concurrent_value</span> - Maximum number of concurrent logins permitted from the same user. <span class="li-normal">type: int</span></li>
            <li><span class="li-head">authtimeout</span> - Time in minutes before the authentication timeout for a user is reached. <span class="li-normal">type: int</span></li>
            <li><span class="li-head">email_to</span> - Two-factor recipient's email address. <span class="li-normal">type: str</span></li>
            <li><span class="li-head">fortitoken</span> - Two-factor recipient's FortiToken serial number. Source user.fortitoken.serial-number. <span class="li-normal">type: str</span></li>
            <li><span class="li-head">id</span> - User ID. <span class="li-normal">type: int</span></li>
            <li><span class="li-head">ldap_server</span> - Name of LDAP server with which the user must authenticate. Source user.ldap.name. <span class="li-normal">type: str</span></li>
            <li><span class="li-head">name</span> - User name. <span class="li-required">required</span> <span class="li-normal">type: str</span></li>
            <li><span class="li-head">passwd</span> - User's password. <span class="li-normal">type: str</span></li>
            <li><span class="li-head">passwd_policy</span> - Password policy to apply to this user, as defined in config user password-policy. Source user.password-policy.name. <span class="li-normal">type: str</span></li>
            <li><span class="li-head">passwd_time</span> - Time of the last password update. <span class="li-normal">type: str</span></li>
            <li><span class="li-head">ppk_identity</span> - IKEv2 Postquantum Preshared Key Identity. <span class="li-normal">type: str</span></li>
            <li><span class="li-head">ppk_secret</span> - IKEv2 Postquantum Preshared Key (ASCII string or hexadecimal encoded with a leading 0x). <span class="li-normal">type: str</span></li>
            <li><span class="li-head">radius_server</span> - Name of RADIUS server with which the user must authenticate. Source user.radius.name. <span class="li-normal">type: str</span></li>
            <li><span class="li-head">sms_custom_server</span> - Two-factor recipient's SMS server. Source system.sms-server.name. <span class="li-normal">type: str</span></li>
            <li><span class="li-head">sms_phone</span> - Two-factor recipient's mobile phone number. <span class="li-normal">type: str</span></li>
            <li><span class="li-head">sms_server</span> - Send SMS through FortiGuard or other external server. <span class="li-normal">type: str</span> <span class="li-normal">choices: fortiguard,  custom</span></li>
            <li><span class="li-head">status</span> - Enable/disable allowing the local user to authenticate with the FortiGate unit. <span class="li-normal">type: str</span> <span class="li-normal">choices: enable,  disable</span></li>
            <li><span class="li-head">two_factor</span> - Enable/disable two-factor authentication. <span class="li-normal">type: str</span> <span class="li-normal">choices: disable,  fortitoken,  email,  sms</span> <span class="li-normal">type:</span> Authentication method. <span class="li-normal">type: str</span> <span class="li-normal">choices: password,  radius,  tacacs+,  ldap</span></li>
            <li><span class="li-head">workstation</span> - Name of the remote user workstation, if you want to limit the user to authenticate only from a particular workstation. <span class="li-normal">type: str</span>
            </ul>

    </ul>




Notes
-----

.. note::


   - Requires fortiosapi library developed by Fortinet

   - Run as a local_action in your playbook



Examples
--------

.. code-block:: yaml+jinja

    - hosts: localhost
      vars:
       host: "192.168.122.40"
       username: "admin"
       password: ""
       vdom: "root"
       ssl_verify: "False"
      tasks:
      - name: Configure local users.
        fortios_user_local:
          host:  "{{ host }}"
          username: "{{ username }}"
          password: "{{ password }}"
          vdom:  "{{ vdom }}"
          https: "False"
          state: "present"
          user_local:
            auth_concurrent_override: "enable"
            auth_concurrent_value: "4"
            authtimeout: "5"
            email_to: "<your_own_value>"
            fortitoken: "<your_own_value> (source user.fortitoken.serial-number)"
            id:  "8"
            ldap_server: "<your_own_value> (source user.ldap.name)"
            name: "default_name_10"
            passwd: "<your_own_value>"
            passwd_policy: "<your_own_value> (source user.password-policy.name)"
            passwd_time: "<your_own_value>"
            ppk_identity: "<your_own_value>"
            ppk_secret: "<your_own_value>"
            radius_server: "<your_own_value> (source user.radius.name)"
            sms_custom_server: "<your_own_value> (source system.sms-server.name)"
            sms_phone: "<your_own_value>"
            sms_server: "fortiguard"
            status: "enable"
            two_factor: "disable"
            type: "password"
            workstation: "<your_own_value>"



Return Values
-------------
Common return values are documented: https://docs.ansible.com/ansible/latest/reference_appendices/common_return_values.html#common-return-values, the following are the fields unique to this module:

.. raw:: html

    <ul>

    <li><span class="li-return">build</span> - Build number of the fortigate image <span class="li-normal">returned: always</span> <span class="li-normal">type: str</span> <span class="li-normal">sample: '1547'</span></li>
    <li><span class="li-return">http_method</span> - Last method used to provision the content into FortiGate <span class="li-normal">returned: always</span> <span class="li-normal">type: str</span> <span class="li-normal">sample: 'PUT'</span></li>
    <li><span class="li-return">http_status</span> - Last result given by FortiGate on last operation applied <span class="li-normal">returned: always</span> <span class="li-normal">type: str</span> <span class="li-normal">sample: 200</span></li>
    <li><span class="li-return">mkey</span> - Master key (id) used in the last call to FortiGate <span class="li-normal">returned: success</span> <span class="li-normal">type: str</span> <span class="li-normal">sample: id</span></li>
    <li><span class="li-return">name</span> - Name of the table used to fulfill the request <span class="li-normal">returned: always</span> <span class="li-normal">type: str</span> <span class="li-normal">sample: urlfilter</span></li>
    <li><span class="li-return">path</span> - Path of the table used to fulfill the request <span class="li-normal">returned: always</span> <span class="li-normal">type: str</span> <span class="li-normal">sample: webfilter</span></li>
    <li><span class="li-return">revision</span> - Internal revision number <span class="li-normal">returned: always</span> <span class="li-normal">type: str</span> <span class="li-normal">sample: 17.0.2.10658</span></li>
    <li><span class="li-return">serial</span> - Serial number of the unit <span class="li-normal">returned: always</span> <span class="li-normal">type: str</span> <span class="li-normal">sample: FGVMEVYYQT3AB5352</span></li>
    <li><span class="li-return">status</span> - Indication of the operation's result <span class="li-normal">returned: always</span> <span class="li-normal">type: str</span> <span class="li-normal">sample: success</span></li>
    <li><span class="li-return">vdom</span> - Virtual domain used <span class="li-normal">returned: always</span> <span class="li-normal">type: str</span> <span class="li-normal">sample: root</span></li>
    <li><span class="li-return">version</span> - Version of the FortiGate <span class="li-normal">returned: always</span> <span class="li-normal">type: str</span> <span class="li-normal">sample: v5.6.3</span></li>
    </ul>



Status
------

- This module is not guaranteed to have a backwards compatible interface.



Authors
-------

- Miguel Angel Munoz (@mamunozgonzalez)
- Nicolas Thomas (@thomnico)



.. hint::
    If you notice any issues in this documentation, you can create a pull request to improve it.