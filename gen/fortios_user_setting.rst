:source: fortios_user_setting.py

:orphan:

.. fortios_user_setting:

fortios_user_setting -- Configure user authentication setting in Fortinet's FortiOS and FortiGate.
++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++

.. versionadded:: 2.9

.. contents::
   :local:
   :depth: 1


Synopsis
--------
- This module is able to configure a FortiGate or FortiOS (FOS) device by allowing the user to set and modify user feature and setting category. Examples include all parameters and values need to be adjusted to datasources before usage. Tested with FOS v6.4.0



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
    <li> <span class="li-head">user_setting</span> - Configure user authentication setting. <span class="li-normal">type: dict</span></li>
        <ul class="ul-self">
        <li> <span class="li-head">auth_blackout_time</span> - Time in seconds an IP address is denied access after failing to authenticate five times within one minute. <span class="li-normal">type: int</span></li>
        <li> <span class="li-head">auth_ca_cert</span> - HTTPS CA certificate for policy authentication. Source vpn.certificate.local.name. <span class="li-normal">type: str</span></li>
        <li> <span class="li-head">auth_cert</span> - HTTPS server certificate for policy authentication. Source vpn.certificate.local.name. <span class="li-normal">type: str</span></li>
        <li> <span class="li-head">auth_http_basic</span> - Enable/disable use of HTTP basic authentication for identity-based firewall policies. <span class="li-normal">type: str</span> <span class="li-normal">choices: enable, disable</span></li>
        <li> <span class="li-head">auth_invalid_max</span> - Maximum number of failed authentication attempts before the user is blocked. <span class="li-normal">type: int</span></li>
        <li> <span class="li-head">auth_lockout_duration</span> - Lockout period in seconds after too many login failures. <span class="li-normal">type: int</span></li>
        <li> <span class="li-head">auth_lockout_threshold</span> - Maximum number of failed login attempts before login lockout is triggered. <span class="li-normal">type: int</span></li>
        <li> <span class="li-head">auth_on_demand</span> - Always/implicitly trigger firewall authentication on demand. <span class="li-normal">type: str</span> <span class="li-normal">choices: always, implicitly</span></li>
        <li> <span class="li-head">auth_portal_timeout</span> - Time in minutes before captive portal user have to re-authenticate (1 - 30 min). <span class="li-normal">type: int</span></li>
        <li> <span class="li-head">auth_ports</span> - Set up non-standard ports for authentication with HTTP, HTTPS, FTP, and TELNET. <span class="li-normal">type: list</span></li>
            <ul class="ul-self">
            <li> <span class="li-head">id</span> - ID. <span class="li-normal">type: int</span> <span class="li-required">required: True</span></li>
            <li> <span class="li-head">port</span> - Non-standard port for firewall user authentication. <span class="li-normal">type: int</span></li>
            <li> <span class="li-head">type</span> - Service type. <span class="li-normal">type: str</span> <span class="li-normal">choices: http, https, ftp, telnet</span></li>
            </ul>
        <li> <span class="li-head">auth_secure_http</span> - Enable/disable redirecting HTTP user authentication to more secure HTTPS. <span class="li-normal">type: str</span> <span class="li-normal">choices: enable, disable</span></li>
        <li> <span class="li-head">auth_src_mac</span> - Enable/disable source MAC for user identity. <span class="li-normal">type: str</span> <span class="li-normal">choices: enable, disable</span></li>
        <li> <span class="li-head">auth_ssl_allow_renegotiation</span> - Allow/forbid SSL re-negotiation for HTTPS authentication. <span class="li-normal">type: str</span> <span class="li-normal">choices: enable, disable</span></li>
        <li> <span class="li-head">auth_ssl_min_proto_version</span> - Minimum supported protocol version for SSL/TLS connections . <span class="li-normal">type: str</span> <span class="li-normal">choices: default, SSLv3, TLSv1, TLSv1-1, TLSv1-2</span></li>
        <li> <span class="li-head">auth_timeout</span> - Time in minutes before the firewall user authentication timeout requires the user to re-authenticate. <span class="li-normal">type: int</span></li>
        <li> <span class="li-head">auth_timeout_type</span> - Control if authenticated users have to login again after a hard timeout, after an idle timeout, or after a session timeout. <span class="li-normal">type: str</span> <span class="li-normal">choices: idle-timeout, hard-timeout, new-session</span></li>
        <li> <span class="li-head">auth_type</span> - Supported firewall policy authentication protocols/methods. <span class="li-normal">type: str</span> <span class="li-normal">choices: http, https, ftp, telnet</span></li>
        <li> <span class="li-head">per_policy_disclaimer</span> - Enable/disable per policy disclaimer. <span class="li-normal">type: str</span> <span class="li-normal">choices: enable, disable</span></li>
        <li> <span class="li-head">radius_ses_timeout_act</span> - Set the RADIUS session timeout to a hard timeout or to ignore RADIUS server session timeouts. <span class="li-normal">type: str</span> <span class="li-normal">choices: hard-timeout, ignore-timeout</span></li>
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
      - name: Configure user authentication setting.
        fortios_user_setting:
          vdom:  "{{ vdom }}"
          user_setting:
            auth_blackout_time: "3"
            auth_ca_cert: "<your_own_value> (source vpn.certificate.local.name)"
            auth_cert: "<your_own_value> (source vpn.certificate.local.name)"
            auth_http_basic: "enable"
            auth_invalid_max: "7"
            auth_lockout_duration: "8"
            auth_lockout_threshold: "9"
            auth_on_demand: "always"
            auth_portal_timeout: "11"
            auth_ports:
             -
                id:  "13"
                port: "14"
                type: "http"
            auth_secure_http: "enable"
            auth_src_mac: "enable"
            auth_ssl_allow_renegotiation: "enable"
            auth_ssl_min_proto_version: "default"
            auth_timeout: "20"
            auth_timeout_type: "idle-timeout"
            auth_type: "http"
            per_policy_disclaimer: "enable"
            radius_ses_timeout_act: "hard-timeout"
    


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
