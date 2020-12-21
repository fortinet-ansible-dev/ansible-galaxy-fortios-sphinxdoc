:source: fortios_vpn_ssl_web_user_group_bookmark.py

:orphan:

.. fortios_vpn_ssl_web_user_group_bookmark:

fortios_vpn_ssl_web_user_group_bookmark -- Configure SSL VPN user group bookmark in Fortinet's FortiOS and FortiGate.
+++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++

.. versionadded:: 2.9

.. contents::
   :local:
   :depth: 1


Synopsis
--------
- This module is able to configure a FortiGate or FortiOS (FOS) device by allowing the user to set and modify vpn_ssl_web feature and user_group_bookmark category. Examples include all parameters and values need to be adjusted to datasources before usage. Tested with FOS v6.2.0



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
    <li> <span class="li-head">vpn_ssl_web_user_group_bookmark</span> - Configure SSL VPN user group bookmark. <span class="li-normal">type: dict</span></li>
        <ul class="ul-self">
        <li> <span class="li-head">bookmarks</span> - Bookmark table. <span class="li-normal">type: list</span></li>
            <ul class="ul-self">
            <li> <span class="li-head">additional_params</span> - Additional parameters. <span class="li-normal">type: str</span></li>
            <li> <span class="li-head">apptype</span> - Application type. <span class="li-normal">type: str</span> <span class="li-normal">choices: citrix, ftp, portforward, rdp, sftp, smb, ssh, telnet, vnc, web</span></li>
            <li> <span class="li-head">description</span> - Description. <span class="li-normal">type: str</span></li>
            <li> <span class="li-head">folder</span> - Network shared file folder parameter. <span class="li-normal">type: str</span></li>
            <li> <span class="li-head">form_data</span> - Form data. <span class="li-normal">type: list</span></li>
                <ul class="ul-self">
                <li> <span class="li-head">name</span> - Name. <span class="li-normal">type: str</span> <span class="li-required">required: True</span></li>
                <li> <span class="li-head">value</span> - Value. <span class="li-normal">type: str</span></li>
                </ul>
            <li> <span class="li-head">host</span> - Host name/IP parameter. <span class="li-normal">type: str</span></li>
            <li> <span class="li-head">listening_port</span> - Listening port (0 - 65535). <span class="li-normal">type: int</span></li>
            <li> <span class="li-head">load_balancing_info</span> - The load balancing information or cookie which should be provided to the connection broker. <span class="li-normal">type: str</span></li>
            <li> <span class="li-head">logon_password</span> - Logon password. <span class="li-normal">type: str</span></li>
            <li> <span class="li-head">logon_user</span> - Logon user. <span class="li-normal">type: str</span></li>
            <li> <span class="li-head">name</span> - Bookmark name. <span class="li-normal">type: str</span> <span class="li-required">required: True</span></li>
            <li> <span class="li-head">port</span> - Remote port. <span class="li-normal">type: int</span></li>
            <li> <span class="li-head">preconnection_blob</span> - An arbitrary string which identifies the RDP source. <span class="li-normal">type: str</span></li>
            <li> <span class="li-head">preconnection_id</span> - The numeric ID of the RDP source (0-2147483648). <span class="li-normal">type: int</span></li>
            <li> <span class="li-head">remote_port</span> - Remote port (0 - 65535). <span class="li-normal">type: int</span></li>
            <li> <span class="li-head">security</span> - Security mode for RDP connection. <span class="li-normal">type: str</span> <span class="li-normal">choices: rdp, nla, tls, any</span></li>
            <li> <span class="li-head">server_layout</span> - Server side keyboard layout. <span class="li-normal">type: str</span> <span class="li-normal">choices: de-de-qwertz, en-gb-qwerty, en-us-qwerty, es-es-qwerty, fr-fr-azerty, fr-ch-qwertz, it-it-qwerty, ja-jp-qwerty, pt-br-qwerty, sv-se-qwerty, tr-tr-qwerty, failsafe</span></li>
            <li> <span class="li-head">show_status_window</span> - Enable/disable showing of status window. <span class="li-normal">type: str</span> <span class="li-normal">choices: enable, disable</span></li>
            <li> <span class="li-head">sso</span> - Single Sign-On. <span class="li-normal">type: str</span> <span class="li-normal">choices: disable, static, auto</span></li>
            <li> <span class="li-head">sso_credential</span> - Single sign-on credentials. <span class="li-normal">type: str</span> <span class="li-normal">choices: sslvpn-login, alternative</span></li>
            <li> <span class="li-head">sso_credential_sent_once</span> - Single sign-on credentials are only sent once to remote server. <span class="li-normal">type: str</span> <span class="li-normal">choices: enable, disable</span></li>
            <li> <span class="li-head">sso_password</span> - SSO password. <span class="li-normal">type: str</span></li>
            <li> <span class="li-head">sso_username</span> - SSO user name. <span class="li-normal">type: str</span></li>
            <li> <span class="li-head">url</span> - URL parameter. <span class="li-normal">type: str</span></li>
            </ul>
        <li> <span class="li-head">name</span> - Group name. Source user.group.name. <span class="li-normal">type: str</span> <span class="li-required">required: True</span></li>
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
      - name: Configure SSL VPN user group bookmark.
        fortios_vpn_ssl_web_user_group_bookmark:
          vdom:  "{{ vdom }}"
          state: "present"
          access_token: "<your_own_value>"
          vpn_ssl_web_user_group_bookmark:
            bookmarks:
             -
                additional_params: "<your_own_value>"
                apptype: "citrix"
                description: "<your_own_value>"
                folder: "<your_own_value>"
                form_data:
                 -
                    name: "default_name_9"
                    value: "<your_own_value>"
                host: "<your_own_value>"
                listening_port: "12"
                load_balancing_info: "<your_own_value>"
                logon_password: "<your_own_value>"
                logon_user: "<your_own_value>"
                name: "default_name_16"
                port: "17"
                preconnection_blob: "<your_own_value>"
                preconnection_id: "19"
                remote_port: "20"
                security: "rdp"
                server_layout: "de-de-qwertz"
                show_status_window: "enable"
                sso: "disable"
                sso_credential: "sslvpn-login"
                sso_credential_sent_once: "enable"
                sso_password: "<your_own_value>"
                sso_username: "<your_own_value>"
                url: "myurl.com"
            name: "default_name_30 (source user.group.name)"
    


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
