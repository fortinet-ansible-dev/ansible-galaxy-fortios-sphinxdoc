:source: fortios_system_admin.py

:orphan:

.. fortios_system_admin:

fortios_system_admin -- Configure admin users in Fortinet's FortiOS and FortiGate.
++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++

.. versionadded:: 2.8

.. contents::
   :local:
   :depth: 1


Synopsis
--------
- This module is able to configure a FortiGate or FortiOS (FOS) device by allowing the user to set and modify system feature and admin category. Examples include all parameters and values need to be adjusted to datasources before usage. Tested with FOS v6.2.0



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
    <li> <span class="li-head">state</span> - Indicates whether to create or remove the object. This attribute was present already in previous version in a deeper level. It has been moved out to this outer level. <span class="li-normal">type: str</span> <span class="li-required">required: False</span> <span class="li-normal">choices: present, absent</span></li>
    <li> <span class="li-head">system_admin</span> - Configure admin users. <span class="li-normal">type: dict</span></li>
        <ul class="ul-self">
        <li> <span class="li-head">state</span> - B(Deprecated) <span class="li-normal">type: str</span> <span class="li-required">required: False</span> <span class="li-normal">choices: present, absent</span></li>
        <li> <span class="li-head">accprofile</span> - Access profile for this administrator. Access profiles control administrator access to FortiGate features. Source system.accprofile.name. <span class="li-normal">type: str</span></li>
        <li> <span class="li-head">accprofile_override</span> - Enable to use the name of an access profile provided by the remote authentication server to control the FortiGate features that this administrator can access. <span class="li-normal">type: str</span> <span class="li-normal">choices: enable, disable</span></li>
        <li> <span class="li-head">allow_remove_admin_session</span> - Enable/disable allow admin session to be removed by privileged admin users. <span class="li-normal">type: str</span> <span class="li-normal">choices: enable, disable</span></li>
        <li> <span class="li-head">comments</span> - Comment. <span class="li-normal">type: str</span></li>
        <li> <span class="li-head">email_to</span> - This administrator"s email address. <span class="li-normal">type: str</span></li>
        <li> <span class="li-head">force_password_change</span> - Enable/disable force password change on next login. <span class="li-normal">type: str</span> <span class="li-normal">choices: enable, disable</span></li>
        <li> <span class="li-head">fortitoken</span> - This administrator"s FortiToken serial number. <span class="li-normal">type: str</span></li>
        <li> <span class="li-head">guest_auth</span> - Enable/disable guest authentication. <span class="li-normal">type: str</span> <span class="li-normal">choices: disable, enable</span></li>
        <li> <span class="li-head">guest_lang</span> - Guest management portal language. Source system.custom-language.name. <span class="li-normal">type: str</span></li>
        <li> <span class="li-head">guest_usergroups</span> - Select guest user groups. <span class="li-normal">type: list</span></li>
            <ul class="ul-self">
            <li> <span class="li-head">name</span> - Select guest user groups. <span class="li-normal">type: str</span> <span class="li-required">required: True</span></li>
            </ul>
        <li> <span class="li-head">gui_dashboard</span> - GUI dashboards. <span class="li-normal">type: list</span></li>
            <ul class="ul-self">
            <li> <span class="li-head">columns</span> - Number of columns. <span class="li-normal">type: int</span></li>
            <li> <span class="li-head">id</span> - Dashboard ID. <span class="li-normal">type: int</span> <span class="li-required">required: True</span></li>
            <li> <span class="li-head">layout_type</span> - Layout type. <span class="li-normal">type: str</span> <span class="li-normal">choices: responsive, fixed</span></li>
            <li> <span class="li-head">name</span> - Dashboard name. <span class="li-normal">type: str</span></li>
            <li> <span class="li-head">permanent</span> - Permanent dashboard (can"t be removed via the GUI). <span class="li-normal">type: str</span> <span class="li-normal">choices: disable, enable</span></li>
            <li> <span class="li-head">vdom</span> - Virtual domain. Source system.vdom.name. <span class="li-normal">type: str</span></li>
            <li> <span class="li-head">widget</span> - Dashboard widgets. <span class="li-normal">type: list</span></li>
                <ul class="ul-self">
                <li> <span class="li-head">fabric_device</span> - Fabric device to monitor. <span class="li-normal">type: str</span></li>
                <li> <span class="li-head">fabric_device_widget_name</span> - Fabric device widget name. <span class="li-normal">type: str</span></li>
                <li> <span class="li-head">fabric_device_widget_visualization_type</span> - Visualization type for fabric device widget. <span class="li-normal">type: str</span></li>
                <li> <span class="li-head">fortiview_device</span> - FortiView device. <span class="li-normal">type: str</span></li>
                <li> <span class="li-head">fortiview_filters</span> - FortiView filters. <span class="li-normal">type: list</span></li>
                    <ul class="ul-self">
                    <li> <span class="li-head">id</span> - FortiView Filter ID. <span class="li-normal">type: int</span> <span class="li-required">required: True</span></li>
                    <li> <span class="li-head">key</span> - Filter key. <span class="li-normal">type: str</span></li>
                    <li> <span class="li-head">value</span> - Filter value. <span class="li-normal">type: str</span></li>
                    </ul>
                <li> <span class="li-head">fortiview_sort_by</span> - FortiView sort by. <span class="li-normal">type: str</span></li>
                <li> <span class="li-head">fortiview_timeframe</span> - FortiView timeframe. <span class="li-normal">type: str</span></li>
                <li> <span class="li-head">fortiview_type</span> - FortiView type. <span class="li-normal">type: str</span></li>
                <li> <span class="li-head">fortiview_visualization</span> - FortiView visualization. <span class="li-normal">type: str</span></li>
                <li> <span class="li-head">height</span> - Height. <span class="li-normal">type: int</span></li>
                <li> <span class="li-head">id</span> - Widget ID. <span class="li-normal">type: int</span> <span class="li-required">required: True</span></li>
                <li> <span class="li-head">industry</span> - Security Audit Rating industry. <span class="li-normal">type: str</span> <span class="li-normal">choices: default, custom</span></li>
                <li> <span class="li-head">interface</span> - Interface to monitor. Source system.interface.name. <span class="li-normal">type: str</span></li>
                <li> <span class="li-head">region</span> - Security Audit Rating region. <span class="li-normal">type: str</span> <span class="li-normal">choices: default, custom</span></li>
                <li> <span class="li-head">title</span> - Widget title. <span class="li-normal">type: str</span></li>
                <li> <span class="li-head">type</span> - Widget type. <span class="li-normal">type: str</span> <span class="li-normal">choices: sysinfo, licinfo, vminfo, forticloud, cpu-usage, memory-usage, disk-usage, log-rate, sessions, session-rate, tr-history, analytics, usb-modem, admins, security-fabric, security-fabric-ranking, ha-status, vulnerability-summary, host-scan-summary, fortiview, botnet-activity, fabric-device</span></li>
                <li> <span class="li-head">width</span> - Width. <span class="li-normal">type: int</span></li>
                <li> <span class="li-head">x_pos</span> - X position. <span class="li-normal">type: int</span></li>
                <li> <span class="li-head">y_pos</span> - Y position. <span class="li-normal">type: int</span></li>
                </ul>
            </ul>
        <li> <span class="li-head">gui_global_menu_favorites</span> - Favorite GUI menu IDs for the global VDOM. <span class="li-normal">type: list</span></li>
            <ul class="ul-self">
            <li> <span class="li-head">id</span> - Select menu ID. <span class="li-normal">type: str</span> <span class="li-required">required: True</span></li>
            </ul>
        <li> <span class="li-head">gui_new_feature_acknowledge</span> - Acknowledgement of new features. <span class="li-normal">type: list</span></li>
            <ul class="ul-self">
            <li> <span class="li-head">id</span> - Select menu ID. <span class="li-normal">type: str</span> <span class="li-required">required: True</span></li>
            </ul>
        <li> <span class="li-head">gui_vdom_menu_favorites</span> - Favorite GUI menu IDs for VDOMs. <span class="li-normal">type: list</span></li>
            <ul class="ul-self">
            <li> <span class="li-head">id</span> - Select menu ID. <span class="li-normal">type: str</span> <span class="li-required">required: True</span></li>
            </ul>
        <li> <span class="li-head">hidden</span> - Admin user hidden attribute. <span class="li-normal">type: int</span></li>
        <li> <span class="li-head">history0</span> - history0 <span class="li-normal">type: str</span></li>
        <li> <span class="li-head">history1</span> - history1 <span class="li-normal">type: str</span></li>
        <li> <span class="li-head">ip6_trusthost1</span> - Any IPv6 address from which the administrator can connect to the FortiGate unit. Default allows access from any IPv6 address. <span class="li-normal">type: str</span></li>
        <li> <span class="li-head">ip6_trusthost10</span> - Any IPv6 address from which the administrator can connect to the FortiGate unit. Default allows access from any IPv6 address. <span class="li-normal">type: str</span></li>
        <li> <span class="li-head">ip6_trusthost2</span> - Any IPv6 address from which the administrator can connect to the FortiGate unit. Default allows access from any IPv6 address. <span class="li-normal">type: str</span></li>
        <li> <span class="li-head">ip6_trusthost3</span> - Any IPv6 address from which the administrator can connect to the FortiGate unit. Default allows access from any IPv6 address. <span class="li-normal">type: str</span></li>
        <li> <span class="li-head">ip6_trusthost4</span> - Any IPv6 address from which the administrator can connect to the FortiGate unit. Default allows access from any IPv6 address. <span class="li-normal">type: str</span></li>
        <li> <span class="li-head">ip6_trusthost5</span> - Any IPv6 address from which the administrator can connect to the FortiGate unit. Default allows access from any IPv6 address. <span class="li-normal">type: str</span></li>
        <li> <span class="li-head">ip6_trusthost6</span> - Any IPv6 address from which the administrator can connect to the FortiGate unit. Default allows access from any IPv6 address. <span class="li-normal">type: str</span></li>
        <li> <span class="li-head">ip6_trusthost7</span> - Any IPv6 address from which the administrator can connect to the FortiGate unit. Default allows access from any IPv6 address. <span class="li-normal">type: str</span></li>
        <li> <span class="li-head">ip6_trusthost8</span> - Any IPv6 address from which the administrator can connect to the FortiGate unit. Default allows access from any IPv6 address. <span class="li-normal">type: str</span></li>
        <li> <span class="li-head">ip6_trusthost9</span> - Any IPv6 address from which the administrator can connect to the FortiGate unit. Default allows access from any IPv6 address. <span class="li-normal">type: str</span></li>
        <li> <span class="li-head">login_time</span> - Record user login time. <span class="li-normal">type: list</span></li>
            <ul class="ul-self">
            <li> <span class="li-head">last_failed_login</span> - Last failed login time. <span class="li-normal">type: str</span></li>
            <li> <span class="li-head">last_login</span> - Last successful login time. <span class="li-normal">type: str</span></li>
            <li> <span class="li-head">usr_name</span> - User name. <span class="li-normal">type: str</span></li>
            </ul>
        <li> <span class="li-head">name</span> - User name. <span class="li-normal">type: str</span> <span class="li-required">required: True</span></li>
        <li> <span class="li-head">password</span> - Admin user password. <span class="li-normal">type: str</span></li>
        <li> <span class="li-head">password_expire</span> - Password expire time. <span class="li-normal">type: str</span></li>
        <li> <span class="li-head">peer_auth</span> - Set to enable peer certificate authentication (for HTTPS admin access). <span class="li-normal">type: str</span> <span class="li-normal">choices: enable, disable</span></li>
        <li> <span class="li-head">peer_group</span> - Name of peer group defined under config user group which has PKI members. Used for peer certificate authentication (for HTTPS admin access). <span class="li-normal">type: str</span></li>
        <li> <span class="li-head">radius_vdom_override</span> - Enable to use the names of VDOMs provided by the remote authentication server to control the VDOMs that this administrator can access. <span class="li-normal">type: str</span> <span class="li-normal">choices: enable, disable</span></li>
        <li> <span class="li-head">remote_auth</span> - Enable/disable authentication using a remote RADIUS, LDAP, or TACACS+ server. <span class="li-normal">type: str</span> <span class="li-normal">choices: enable, disable</span></li>
        <li> <span class="li-head">remote_group</span> - User group name used for remote auth. <span class="li-normal">type: str</span></li>
        <li> <span class="li-head">schedule</span> - Firewall schedule used to restrict when the administrator can log in. No schedule means no restrictions. <span class="li-normal">type: str</span></li>
        <li> <span class="li-head">sms_custom_server</span> - Custom SMS server to send SMS messages to. Source system.sms-server.name. <span class="li-normal">type: str</span></li>
        <li> <span class="li-head">sms_phone</span> - Phone number on which the administrator receives SMS messages. <span class="li-normal">type: str</span></li>
        <li> <span class="li-head">sms_server</span> - Send SMS messages using the FortiGuard SMS server or a custom server. <span class="li-normal">type: str</span> <span class="li-normal">choices: fortiguard, custom</span></li>
        <li> <span class="li-head">ssh_certificate</span> - Select the certificate to be used by the FortiGate for authentication with an SSH client. Source certificate.local.name. <span class="li-normal">type: str</span></li>
        <li> <span class="li-head">ssh_public_key1</span> - Public key of an SSH client. The client is authenticated without being asked for credentials. Create the public-private key pair in the SSH client application. <span class="li-normal">type: str</span></li>
        <li> <span class="li-head">ssh_public_key2</span> - Public key of an SSH client. The client is authenticated without being asked for credentials. Create the public-private key pair in the SSH client application. <span class="li-normal">type: str</span></li>
        <li> <span class="li-head">ssh_public_key3</span> - Public key of an SSH client. The client is authenticated without being asked for credentials. Create the public-private key pair in the SSH client application. <span class="li-normal">type: str</span></li>
        <li> <span class="li-head">trusthost1</span> - Any IPv4 address or subnet address and netmask from which the administrator can connect to the FortiGate unit. Default allows access from any IPv4 address. <span class="li-normal">type: str</span></li>
        <li> <span class="li-head">trusthost10</span> - Any IPv4 address or subnet address and netmask from which the administrator can connect to the FortiGate unit. Default allows access from any IPv4 address. <span class="li-normal">type: str</span></li>
        <li> <span class="li-head">trusthost2</span> - Any IPv4 address or subnet address and netmask from which the administrator can connect to the FortiGate unit. Default allows access from any IPv4 address. <span class="li-normal">type: str</span></li>
        <li> <span class="li-head">trusthost3</span> - Any IPv4 address or subnet address and netmask from which the administrator can connect to the FortiGate unit. Default allows access from any IPv4 address. <span class="li-normal">type: str</span></li>
        <li> <span class="li-head">trusthost4</span> - Any IPv4 address or subnet address and netmask from which the administrator can connect to the FortiGate unit. Default allows access from any IPv4 address. <span class="li-normal">type: str</span></li>
        <li> <span class="li-head">trusthost5</span> - Any IPv4 address or subnet address and netmask from which the administrator can connect to the FortiGate unit. Default allows access from any IPv4 address. <span class="li-normal">type: str</span></li>
        <li> <span class="li-head">trusthost6</span> - Any IPv4 address or subnet address and netmask from which the administrator can connect to the FortiGate unit. Default allows access from any IPv4 address. <span class="li-normal">type: str</span></li>
        <li> <span class="li-head">trusthost7</span> - Any IPv4 address or subnet address and netmask from which the administrator can connect to the FortiGate unit. Default allows access from any IPv4 address. <span class="li-normal">type: str</span></li>
        <li> <span class="li-head">trusthost8</span> - Any IPv4 address or subnet address and netmask from which the administrator can connect to the FortiGate unit. Default allows access from any IPv4 address. <span class="li-normal">type: str</span></li>
        <li> <span class="li-head">trusthost9</span> - Any IPv4 address or subnet address and netmask from which the administrator can connect to the FortiGate unit. Default allows access from any IPv4 address. <span class="li-normal">type: str</span></li>
        <li> <span class="li-head">two_factor</span> - Enable/disable two-factor authentication. <span class="li-normal">type: str</span> <span class="li-normal">choices: disable, fortitoken, email, sms, fortitoken-cloud</span></li>
        <li> <span class="li-head">vdom</span> - Virtual domain(s) that the administrator can access. <span class="li-normal">type: list</span></li>
            <ul class="ul-self">
            <li> <span class="li-head">name</span> - Virtual domain name. Source system.vdom.name. <span class="li-normal">type: str</span> <span class="li-required">required: True</span></li>
            </ul>
        <li> <span class="li-head">wildcard</span> - Enable/disable wildcard RADIUS authentication. <span class="li-normal">type: str</span> <span class="li-normal">choices: enable, disable</span></li>
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
      - name: Configure admin users.
        fortios_system_admin:
          vdom:  "{{ vdom }}"
          state: "present"
          access_token: "<your_own_value>"
          system_admin:
            accprofile: "<your_own_value> (source system.accprofile.name)"
            accprofile_override: "enable"
            allow_remove_admin_session: "enable"
            comments: "<your_own_value>"
            email_to: "<your_own_value>"
            force_password_change: "enable"
            fortitoken: "<your_own_value>"
            guest_auth: "disable"
            guest_lang: "<your_own_value> (source system.custom-language.name)"
            guest_usergroups:
             -
                name: "default_name_13"
            gui_dashboard:
             -
                columns: "15"
                id:  "16"
                layout_type: "responsive"
                name: "default_name_18"
                permanent: "disable"
                vdom: "<your_own_value> (source system.vdom.name)"
                widget:
                 -
                    fabric_device: "<your_own_value>"
                    fabric_device_widget_name: "<your_own_value>"
                    fabric_device_widget_visualization_type: "<your_own_value>"
                    fortiview_device: "<your_own_value>"
                    fortiview_filters:
                     -
                        id:  "27"
                        key: "<your_own_value>"
                        value: "<your_own_value>"
                    fortiview_sort_by: "<your_own_value>"
                    fortiview_timeframe: "<your_own_value>"
                    fortiview_type: "<your_own_value>"
                    fortiview_visualization: "<your_own_value>"
                    height: "34"
                    id:  "35"
                    industry: "default"
                    interface: "<your_own_value> (source system.interface.name)"
                    region: "default"
                    title: "<your_own_value>"
                    type: "sysinfo"
                    width: "41"
                    x_pos: "42"
                    y_pos: "43"
            gui_global_menu_favorites:
             -
                id:  "45"
            gui_new_feature_acknowledge:
             -
                id:  "47"
            gui_vdom_menu_favorites:
             -
                id:  "49"
            hidden: "50"
            history0: "<your_own_value>"
            history1: "<your_own_value>"
            ip6_trusthost1: "<your_own_value>"
            ip6_trusthost10: "<your_own_value>"
            ip6_trusthost2: "<your_own_value>"
            ip6_trusthost3: "<your_own_value>"
            ip6_trusthost4: "<your_own_value>"
            ip6_trusthost5: "<your_own_value>"
            ip6_trusthost6: "<your_own_value>"
            ip6_trusthost7: "<your_own_value>"
            ip6_trusthost8: "<your_own_value>"
            ip6_trusthost9: "<your_own_value>"
            login_time:
             -
                last_failed_login: "<your_own_value>"
                last_login: "<your_own_value>"
                usr_name: "<your_own_value>"
            name: "default_name_67"
            password: "<your_own_value>"
            password_expire: "<your_own_value>"
            peer_auth: "enable"
            peer_group: "<your_own_value>"
            radius_vdom_override: "enable"
            remote_auth: "enable"
            remote_group: "<your_own_value>"
            schedule: "<your_own_value>"
            sms_custom_server: "<your_own_value> (source system.sms-server.name)"
            sms_phone: "<your_own_value>"
            sms_server: "fortiguard"
            ssh_certificate: "<your_own_value> (source certificate.local.name)"
            ssh_public_key1: "<your_own_value>"
            ssh_public_key2: "<your_own_value>"
            ssh_public_key3: "<your_own_value>"
            trusthost1: "<your_own_value>"
            trusthost10: "<your_own_value>"
            trusthost2: "<your_own_value>"
            trusthost3: "<your_own_value>"
            trusthost4: "<your_own_value>"
            trusthost5: "<your_own_value>"
            trusthost6: "<your_own_value>"
            trusthost7: "<your_own_value>"
            trusthost8: "<your_own_value>"
            trusthost9: "<your_own_value>"
            two_factor: "disable"
            vdom:
             -
                name: "default_name_95 (source system.vdom.name)"
            wildcard: "enable"
    


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
