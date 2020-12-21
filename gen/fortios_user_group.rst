:source: fortios_user_group.py

:orphan:

.. fortios_user_group:

fortios_user_group -- Configure user groups in Fortinet's FortiOS and FortiGate.
++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++

.. versionadded:: 2.9

.. contents::
   :local:
   :depth: 1


Synopsis
--------
- This module is able to configure a FortiGate or FortiOS (FOS) device by allowing the user to set and modify user feature and group category. Examples include all parameters and values need to be adjusted to datasources before usage. Tested with FOS v6.2.0



Requirements
------------
The below requirements are needed on the host that executes this module.

- ansible>=2.9.0


Parameters
----------


.. raw:: html

    <ul>
    <li> <span class="li-head">access_token</span> - Token-based authentication. Generated from GUI of Fortigate. <span class="li-normal">type: str</span> <span class="li-required">required: False</span></li>
    <li> <span class="li-head">vdom</span> - Virtual domain, among those defined previously. A vdom is a virtual instance of the FortiGate that can be configured and used as a different unit. <span class="li-normal">type: str</span> <span class="li-normal">default: root</span></li>
    <li> <span class="li-head">state</span> - Indicates whether to create or remove the object. <span class="li-normal">type: str</span> <span class="li-required">required: True</span> <span class="li-normal">choices: present, absent</span></li>
    <li> <span class="li-head">user_group</span> - Configure user groups. <span class="li-normal">type: dict</span></li>
        <ul class="ul-self">
        <li> <span class="li-head">auth_concurrent_override</span> - Enable/disable overriding the global number of concurrent authentication sessions for this user group. <span class="li-normal">type: str</span> <span class="li-normal">choices: enable, disable</span></li>
        <li> <span class="li-head">auth_concurrent_value</span> - Maximum number of concurrent authenticated connections per user (0 - 100). <span class="li-normal">type: int</span></li>
        <li> <span class="li-head">authtimeout</span> - Authentication timeout in minutes for this user group. 0 to use the global user setting auth-timeout. <span class="li-normal">type: int</span></li>
        <li> <span class="li-head">company</span> - Set the action for the company guest user field. <span class="li-normal">type: str</span> <span class="li-normal">choices: optional, mandatory, disabled</span></li>
        <li> <span class="li-head">email</span> - Enable/disable the guest user email address field. <span class="li-normal">type: str</span> <span class="li-normal">choices: disable, enable</span></li>
        <li> <span class="li-head">expire</span> - Time in seconds before guest user accounts expire. (1 - 31536000 sec) <span class="li-normal">type: int</span></li>
        <li> <span class="li-head">expire_type</span> - Determine when the expiration countdown begins. <span class="li-normal">type: str</span> <span class="li-normal">choices: immediately, first-successful-login</span></li>
        <li> <span class="li-head">group_type</span> - Set the group to be for firewall authentication, FSSO, RSSO, or guest users. <span class="li-normal">type: str</span> <span class="li-normal">choices: firewall, fsso-service, rsso, guest</span></li>
        <li> <span class="li-head">guest</span> - Guest User. <span class="li-normal">type: list</span></li>
            <ul class="ul-self">
            <li> <span class="li-head">comment</span> - Comment. <span class="li-normal">type: str</span></li>
            <li> <span class="li-head">company</span> - Set the action for the company guest user field. <span class="li-normal">type: str</span></li>
            <li> <span class="li-head">email</span> - Email. <span class="li-normal">type: str</span></li>
            <li> <span class="li-head">expiration</span> - Expire time. <span class="li-normal">type: str</span></li>
            <li> <span class="li-head">mobile_phone</span> - Mobile phone. <span class="li-normal">type: str</span></li>
            <li> <span class="li-head">name</span> - Guest name. <span class="li-normal">type: str</span></li>
            <li> <span class="li-head">password</span> - Guest password. <span class="li-normal">type: str</span></li>
            <li> <span class="li-head">sponsor</span> - Set the action for the sponsor guest user field. <span class="li-normal">type: str</span></li>
            <li> <span class="li-head">user_id</span> - Guest ID. <span class="li-normal">type: str</span></li>
            </ul>
        <li> <span class="li-head">http_digest_realm</span> - Realm attribute for MD5-digest authentication. <span class="li-normal">type: str</span></li>
        <li> <span class="li-head">id</span> - Group ID. <span class="li-normal">type: int</span></li>
        <li> <span class="li-head">match</span> - Group matches. <span class="li-normal">type: list</span></li>
            <ul class="ul-self">
            <li> <span class="li-head">group_name</span> - Name of matching user or group on remote authentication server. <span class="li-normal">type: str</span></li>
            <li> <span class="li-head">id</span> - ID. <span class="li-normal">type: int</span> <span class="li-required">required: True</span></li>
            <li> <span class="li-head">server_name</span> - Name of remote auth server. Source user.radius.name user.ldap.name user.tacacs+.name. <span class="li-normal">type: str</span></li>
            </ul>
        <li> <span class="li-head">max_accounts</span> - Maximum number of guest accounts that can be created for this group (0 means unlimited). <span class="li-normal">type: int</span></li>
        <li> <span class="li-head">member</span> - Names of users, peers, LDAP severs, or RADIUS servers to add to the user group. <span class="li-normal">type: list</span></li>
            <ul class="ul-self">
            <li> <span class="li-head">name</span> - Group member name. Source user.peer.name user.local.name user.radius.name user.tacacs+.name user.ldap.name user.adgrp.name user .pop3.name. <span class="li-normal">type: str</span> <span class="li-required">required: True</span></li>
            </ul>
        <li> <span class="li-head">mobile_phone</span> - Enable/disable the guest user mobile phone number field. <span class="li-normal">type: str</span> <span class="li-normal">choices: disable, enable</span></li>
        <li> <span class="li-head">multiple_guest_add</span> - Enable/disable addition of multiple guests. <span class="li-normal">type: str</span> <span class="li-normal">choices: disable, enable</span></li>
        <li> <span class="li-head">name</span> - Group name. <span class="li-normal">type: str</span> <span class="li-required">required: True</span></li>
        <li> <span class="li-head">password</span> - Guest user password type. <span class="li-normal">type: str</span> <span class="li-normal">choices: auto-generate, specify, disable</span></li>
        <li> <span class="li-head">sms_custom_server</span> - SMS server. Source system.sms-server.name. <span class="li-normal">type: str</span></li>
        <li> <span class="li-head">sms_server</span> - Send SMS through FortiGuard or other external server. <span class="li-normal">type: str</span> <span class="li-normal">choices: fortiguard, custom</span></li>
        <li> <span class="li-head">sponsor</span> - Set the action for the sponsor guest user field. <span class="li-normal">type: str</span> <span class="li-normal">choices: optional, mandatory, disabled</span></li>
        <li> <span class="li-head">sso_attribute_value</span> - Name of the RADIUS user group that this local user group represents. <span class="li-normal">type: str</span></li>
        <li> <span class="li-head">user_id</span> - Guest user ID type. <span class="li-normal">type: str</span> <span class="li-normal">choices: email, auto-generate, specify</span></li>
        <li> <span class="li-head">user_name</span> - Enable/disable the guest user name entry. <span class="li-normal">type: str</span> <span class="li-normal">choices: disable, enable</span></li>
        </ul>
    </ul>


Notes
-----

.. note::

   - Legacy fortiosapi has been deprecated, httpapi is the preferred way to run playbooks



Examples
--------

.. code-block:: yaml+jinja
    
    - hosts: fortigates
      collections:
        - fortinet.fortios
      connection: httpapi
      vars:
       vdom: "root"
       ansible_httpapi_use_ssl: yes
       ansible_httpapi_validate_certs: no
       ansible_httpapi_port: 443
      tasks:
      - name: Configure user groups.
        fortios_user_group:
          vdom:  "{{ vdom }}"
          state: "present"
          access_token: "<your_own_value>"
          user_group:
            auth_concurrent_override: "enable"
            auth_concurrent_value: "4"
            authtimeout: "5"
            company: "optional"
            email: "disable"
            expire: "8"
            expire_type: "immediately"
            group_type: "firewall"
            guest:
             -
                comment: "Comment."
                company: "<your_own_value>"
                email: "<your_own_value>"
                expiration: "<your_own_value>"
                mobile_phone: "<your_own_value>"
                name: "default_name_17"
                password: "<your_own_value>"
                sponsor: "<your_own_value>"
                user_id: "<your_own_value>"
            http_digest_realm: "<your_own_value>"
            id:  "22"
            match:
             -
                group_name: "<your_own_value>"
                id:  "25"
                server_name: "<your_own_value> (source user.radius.name user.ldap.name user.tacacs+.name)"
            max_accounts: "27"
            member:
             -
                name: "default_name_29 (source user.peer.name user.local.name user.radius.name user.tacacs+.name user.ldap.name user.adgrp.name user.pop3.name)"
            mobile_phone: "disable"
            multiple_guest_add: "disable"
            name: "default_name_32"
            password: "auto-generate"
            sms_custom_server: "<your_own_value> (source system.sms-server.name)"
            sms_server: "fortiguard"
            sponsor: "optional"
            sso_attribute_value: "<your_own_value>"
            user_id: "email"
            user_name: "disable"
    


Return Values
-------------
Common return values are documented: https://docs.ansible.com/ansible/latest/reference_appendices/common_return_values.html#common-return-values, the following are the fields unique to this module:

.. raw:: html

    <ul>

    <li> <span class="li-return">build</span> - Build number of the fortigate image <span class="li-normal">returned: always</span> <span class="li-normal">type: str</span> <span class="li-normal">sample: 1547</span></li>
    <li> <span class="li-return">http_method</span> - Last method used to provision the content into FortiGate <span class="li-normal">returned: always</span> <span class="li-normal">type: str</span> <span class="li-normal">sample: PUT</span></li>
    <li> <span class="li-return">http_status</span> - Last result given by FortiGate on last operation applied <span class="li-normal">returned: always</span> <span class="li-normal">type: str</span> <span class="li-normal">sample: 200</span></li>
    <li> <span class="li-return">mkey</span> - Master key (id) used in the last call to FortiGate <span class="li-normal">returned: success</span> <span class="li-normal">type: str</span> <span class="li-normal">sample: id</span></li>
    <li> <span class="li-return">name</span> - Name of the table used to fulfill the request <span class="li-normal">returned: always</span> <span class="li-normal">type: str</span> <span class="li-normal">sample: urlfilter</span></li>
    <li> <span class="li-return">path</span> - Path of the table used to fulfill the request <span class="li-normal">returned: always</span> <span class="li-normal">type: str</span> <span class="li-normal">sample: webfilter</span></li>
    <li> <span class="li-return">revision</span> - Internal revision number <span class="li-normal">returned: always</span> <span class="li-normal">type: str</span> <span class="li-normal">sample: 17.0.2.10658</span></li>
    <li> <span class="li-return">serial</span> - Serial number of the unit <span class="li-normal">returned: always</span> <span class="li-normal">type: str</span> <span class="li-normal">sample: FGVMEVYYQT3AB5352</span></li>
    <li> <span class="li-return">status</span> - Indication of the operation's result <span class="li-normal">returned: always</span> <span class="li-normal">type: str</span> <span class="li-normal">sample: success</span></li>
    <li> <span class="li-return">vdom</span> - Virtual domain used <span class="li-normal">returned: always</span> <span class="li-normal">type: str</span> <span class="li-normal">sample: root</span></li>
    <li> <span class="li-return">version</span> - Version of the FortiGate <span class="li-normal">returned: always</span> <span class="li-normal">type: str</span> <span class="li-normal">sample: v5.6.3</span></li>
    </ul>

Status
------

- This module is not guaranteed to have a backwards compatible interface.


Authors
-------

- Link Zheng (@chillancezen)
- Jie Xue (@JieX19)
- Hongbin Lu (@fgtdev-hblu)
- Frank Shen (@frankshen01)
- Miguel Angel Munoz (@mamunozgonzalez)
- Nicolas Thomas (@thomnico)


.. hint::
    If you notice any issues in this documentation, you can create a pull request to improve it.
