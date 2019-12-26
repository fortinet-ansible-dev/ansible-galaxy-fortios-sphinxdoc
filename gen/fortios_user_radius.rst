:source: fortios_user_radius.py

:orphan:

.. _fortios_user_radius:

fortios_user_radius -- Configure RADIUS server entries in Fortinet's FortiOS and FortiGate.
+++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++

.. versionadded:: 2.8

.. contents::
   :local:
   :depth: 1


Synopsis
--------
- This module is able to configure a FortiGate or FortiOS (FOS) device by allowing the user to set and modify user feature and radius category. Examples include all parameters and values need to be adjusted to datasources before usage. Tested with FOS v6.0.5


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
    <li><span class="li-head">state</span> - Indicates whether to create or remove the object. This attribute was present already in previous version in a deeper level. It has been moved out to this outer level. <span class="li-normal">type: str</span> <span class="li-required">required: false</span> <span class="li-normal">choices: present,  absent</span></li>
    <li><span class="li-head">user_radius</span> - Configure RADIUS server entries. <span class="li-normal">default: null</span> <span class="li-normal">type: dict</span></li>
            <ul class="ul-self">

            <li><span class="li-head">state</span> - B(Deprecated) Starting with Ansible 2.9 we recommend using the top-level 'state' parameter. HORIZONTALLINE Indicates whether to create or remove the object. <span class="li-normal">type: str</span> <span class="li-required">required: false</span> <span class="li-normal">choices: present,  absent</span></li>
            <li><span class="li-head">accounting_server</span> - Additional accounting servers. <span class="li-normal">type: list</span></li>
                    <ul class="ul-self">

                    <li><span class="li-head">id</span> - ID (0 - 4294967295). <span class="li-required">required</span> <span class="li-normal">type: int</span></li>
                    <li><span class="li-head">port</span> - RADIUS accounting port number. <span class="li-normal">type: int</span></li>
                    <li><span class="li-head">secret</span> - Secret key. <span class="li-normal">type: str</span></li>
                    <li><span class="li-head">server</span> - name_str or ip_str Server CN domain name or IP. <span class="li-normal">type: str</span></li>
                    <li><span class="li-head">source_ip</span> - Source IP address for communications to the RADIUS server. <span class="li-normal">type: str</span></li>
                    <li><span class="li-head">status</span> - Status. <span class="li-normal">type: str</span> <span class="li-normal">choices: enable,  disable</span>
                    </ul>

            <li><span class="li-head">acct_all_servers</span> - Enable/disable sending of accounting messages to all configured servers. <span class="li-normal">type: str</span> <span class="li-normal">choices: enable,  disable</span></li>
            <li><span class="li-head">acct_interim_interval</span> - Time in seconds between each accounting interim update message. <span class="li-normal">type: int</span></li>
            <li><span class="li-head">all_usergroup</span> - Enable/disable automatically including this RADIUS server in all user groups. <span class="li-normal">type: str</span> <span class="li-normal">choices: disable,  enable</span></li>
            <li><span class="li-head">auth_type</span> - Authentication methods/protocols permitted for this RADIUS server. <span class="li-normal">type: str</span> <span class="li-normal">choices: auto,  ms_chap_v2,  ms_chap,  chap,  pap</span></li>
            <li><span class="li-head">class</span> - Class attribute name(s). <span class="li-normal">type: list</span></li>
                    <ul class="ul-self">

                    <li><span class="li-head">name</span> - Class name. <span class="li-required">required</span> <span class="li-normal">type: str</span>
                    </ul>

            <li><span class="li-head">h3c_compatibility</span> - Enable/disable compatibility with the H3C, a mechanism that performs security checking for authentication. <span class="li-normal">type: str</span> <span class="li-normal">choices: enable,  disable</span></li>
            <li><span class="li-head">name</span> - RADIUS server entry name. <span class="li-required">required</span> <span class="li-normal">type: str</span></li>
            <li><span class="li-head">nas_ip</span> - IP address used to communicate with the RADIUS server and used as NAS-IP-Address and Called-Station-ID attributes. <span class="li-normal">type: str</span></li>
            <li><span class="li-head">password_encoding</span> - Password encoding. <span class="li-normal">type: str</span> <span class="li-normal">choices: auto,  ISO-8859-1</span></li>
            <li><span class="li-head">password_renewal</span> - Enable/disable password renewal. <span class="li-normal">type: str</span> <span class="li-normal">choices: enable,  disable</span></li>
            <li><span class="li-head">radius_coa</span> - Enable to allow a mechanism to change the attributes of an authentication, authorization, and accounting session after it is authenticated. <span class="li-normal">type: str</span> <span class="li-normal">choices: enable,  disable</span></li>
            <li><span class="li-head">radius_port</span> - RADIUS service port number. <span class="li-normal">type: int</span></li>
            <li><span class="li-head">rsso</span> - Enable/disable RADIUS based single sign on feature. <span class="li-normal">type: str</span> <span class="li-normal">choices: enable,  disable</span></li>
            <li><span class="li-head">rsso_context_timeout</span> - Time in seconds before the logged out user is removed from the "user context list" of logged on users. <span class="li-normal">type: int</span></li>
            <li><span class="li-head">rsso_endpoint_attribute</span> - RADIUS attributes used to extract the user end point identifier from the RADIUS Start record. <span class="li-normal">type: str</span> <span class="li-normal">choices: User-Name,  NAS-IP-Address,  Framed-IP-Address,  Framed-IP-Netmask,  Filter-Id,  Login-IP-Host,  Reply-Message,  Callback-Number,  Callback-Id,  Framed-Route,  Framed-IPX-Network,  Class,  Called-Station-Id,  Calling-Station-Id,  NAS-Identifier,  Proxy-State,  Login-LAT-Service,  Login-LAT-Node,  Login-LAT-Group,  Framed-AppleTalk-Zone,  Acct-Session-Id,  Acct-Multi-Session-Id</span></li>
            <li><span class="li-head">rsso_endpoint_block_attribute</span> - RADIUS attributes used to block a user. <span class="li-normal">type: str</span> <span class="li-normal">choices: User-Name,  NAS-IP-Address,  Framed-IP-Address,  Framed-IP-Netmask,  Filter-Id,  Login-IP-Host,  Reply-Message,  Callback-Number,  Callback-Id,  Framed-Route,  Framed-IPX-Network,  Class,  Called-Station-Id,  Calling-Station-Id,  NAS-Identifier,  Proxy-State,  Login-LAT-Service,  Login-LAT-Node,  Login-LAT-Group,  Framed-AppleTalk-Zone,  Acct-Session-Id,  Acct-Multi-Session-Id</span></li>
            <li><span class="li-head">rsso_ep_one_ip_only</span> - Enable/disable the replacement of old IP addresses with new ones for the same endpoint on RADIUS accounting Start messages. <span class="li-normal">type: str</span> <span class="li-normal">choices: enable,  disable</span></li>
            <li><span class="li-head">rsso_flush_ip_session</span> - Enable/disable flushing user IP sessions on RADIUS accounting Stop messages. <span class="li-normal">type: str</span> <span class="li-normal">choices: enable,  disable</span></li>
            <li><span class="li-head">rsso_log_flags</span> - Events to log. <span class="li-normal">type: str</span> <span class="li-normal">choices: protocol-error,  profile-missing,  accounting-stop-missed,  accounting-event,  endpoint-block,  radiusd-other,  none</span></li>
            <li><span class="li-head">rsso_log_period</span> - Time interval in seconds that group event log messages will be generated for dynamic profile events. <span class="li-normal">type: int</span></li>
            <li><span class="li-head">rsso_radius_response</span> - Enable/disable sending RADIUS response packets after receiving Start and Stop records. <span class="li-normal">type: str</span> <span class="li-normal">choices: enable,  disable</span></li>
            <li><span class="li-head">rsso_radius_server_port</span> - UDP port to listen on for RADIUS Start and Stop records. <span class="li-normal">type: int</span></li>
            <li><span class="li-head">rsso_secret</span> - RADIUS secret used by the RADIUS accounting server. <span class="li-normal">type: str</span></li>
            <li><span class="li-head">rsso_validate_request_secret</span> - Enable/disable validating the RADIUS request shared secret in the Start or End record. <span class="li-normal">type: str</span> <span class="li-normal">choices: enable,  disable</span></li>
            <li><span class="li-head">secondary_secret</span> - Secret key to access the secondary server. <span class="li-normal">type: str</span></li>
            <li><span class="li-head">secondary_server</span> - name_str or ip_str secondary RADIUS CN domain name or IP. <span class="li-normal">type: str</span></li>
            <li><span class="li-head">secret</span> - Pre-shared secret key used to access the primary RADIUS server. <span class="li-normal">type: str</span></li>
            <li><span class="li-head">server</span> - Primary RADIUS server CN domain name or IP address. <span class="li-normal">type: str</span></li>
            <li><span class="li-head">source_ip</span> - Source IP address for communications to the RADIUS server. <span class="li-normal">type: str</span></li>
            <li><span class="li-head">sso_attribute</span> - RADIUS attribute that contains the profile group name to be extracted from the RADIUS Start record. <span class="li-normal">type: str</span> <span class="li-normal">choices: User-Name,  NAS-IP-Address,  Framed-IP-Address,  Framed-IP-Netmask,  Filter-Id,  Login-IP-Host,  Reply-Message,  Callback-Number,  Callback-Id,  Framed-Route,  Framed-IPX-Network,  Class,  Called-Station-Id,  Calling-Station-Id,  NAS-Identifier,  Proxy-State,  Login-LAT-Service,  Login-LAT-Node,  Login-LAT-Group,  Framed-AppleTalk-Zone,  Acct-Session-Id,  Acct-Multi-Session-Id</span></li>
            <li><span class="li-head">sso_attribute_key</span> - Key prefix for SSO group value in the SSO attribute. <span class="li-normal">type: str</span></li>
            <li><span class="li-head">sso_attribute_value_override</span> - Enable/disable override old attribute value with new value for the same endpoint. <span class="li-normal">type: str</span> <span class="li-normal">choices: enable,  disable</span></li>
            <li><span class="li-head">tertiary_secret</span> - Secret key to access the tertiary server. <span class="li-normal">type: str</span></li>
            <li><span class="li-head">tertiary_server</span> - name_str or ip_str tertiary RADIUS CN domain name or IP. <span class="li-normal">type: str</span></li>
            <li><span class="li-head">timeout</span> - Time in seconds between re-sending authentication requests. <span class="li-normal">type: int</span></li>
            <li><span class="li-head">use_management_vdom</span> - Enable/disable using management VDOM to send requests. <span class="li-normal">type: str</span> <span class="li-normal">choices: enable,  disable</span></li>
            <li><span class="li-head">username_case_sensitive</span> - Enable/disable case sensitive user names. <span class="li-normal">type: str</span> <span class="li-normal">choices: enable,  disable</span>
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
      - name: Configure RADIUS server entries.
        fortios_user_radius:
          host:  "{{ host }}"
          username: "{{ username }}"
          password: "{{ password }}"
          vdom:  "{{ vdom }}"
          https: "False"
          state: "present"
          user_radius:
            accounting_server:
             -
                id:  "4"
                port: "5"
                secret: "<your_own_value>"
                server: "192.168.100.40"
                source_ip: "84.230.14.43"
                status: "enable"
            acct_all_servers: "enable"
            acct_interim_interval: "11"
            all_usergroup: "disable"
            auth_type: "auto"
            class:
             -
                name: "default_name_15"
            h3c_compatibility: "enable"
            name: "default_name_17"
            nas_ip: "<your_own_value>"
            password_encoding: "auto"
            password_renewal: "enable"
            radius_coa: "enable"
            radius_port: "22"
            rsso: "enable"
            rsso_context_timeout: "24"
            rsso_endpoint_attribute: "User-Name"
            rsso_endpoint_block_attribute: "User-Name"
            rsso_ep_one_ip_only: "enable"
            rsso_flush_ip_session: "enable"
            rsso_log_flags: "protocol-error"
            rsso_log_period: "30"
            rsso_radius_response: "enable"
            rsso_radius_server_port: "32"
            rsso_secret: "<your_own_value>"
            rsso_validate_request_secret: "enable"
            secondary_secret: "<your_own_value>"
            secondary_server: "<your_own_value>"
            secret: "<your_own_value>"
            server: "192.168.100.40"
            source_ip: "84.230.14.43"
            sso_attribute: "User-Name"
            sso_attribute_key: "<your_own_value>"
            sso_attribute_value_override: "enable"
            tertiary_secret: "<your_own_value>"
            tertiary_server: "<your_own_value>"
            timeout: "45"
            use_management_vdom: "enable"
            username_case_sensitive: "enable"



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