:source: fortios_firewall_ssl_ssh_profile.py

:orphan:

.. fortios_firewall_ssl_ssh_profile:

fortios_firewall_ssl_ssh_profile -- Configure SSL/SSH protocol options in Fortinet's FortiOS and FortiGate.
+++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++

.. versionadded:: 2.8

.. contents::
   :local:
   :depth: 1


Synopsis
--------
- This module is able to configure a FortiGate or FortiOS (FOS) device by allowing the user to set and modify firewall feature and ssl_ssh_profile category. Examples include all parameters and values need to be adjusted to datasources before usage. Tested with FOS v6.0.0



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
    <li> <span class="li-head">firewall_ssl_ssh_profile</span> - Configure SSL/SSH protocol options. <span class="li-normal">type: dict</span></li>
        <ul class="ul-self">
        <li> <span class="li-head">state</span> - B(Deprecated) <span class="li-normal">type: str</span> <span class="li-required">required: False</span> <span class="li-normal">choices: present, absent</span></li>
        <li> <span class="li-head">caname</span> - CA certificate used by SSL Inspection. Source vpn.certificate.local.name. <span class="li-normal">type: str</span></li>
        <li> <span class="li-head">comment</span> - Optional comments. <span class="li-normal">type: str</span></li>
        <li> <span class="li-head">ftps</span> - Configure FTPS options. <span class="li-normal">type: dict</span></li>
            <ul class="ul-self">
            <li> <span class="li-head">allow_invalid_server_cert</span> - When enabled, allows SSL sessions whose server certificate validation failed. <span class="li-normal">type: str</span> <span class="li-normal">choices: enable, disable</span></li>
            <li> <span class="li-head">client_cert_request</span> - Action based on client certificate request failure. <span class="li-normal">type: str</span> <span class="li-normal">choices: bypass, inspect, block</span></li>
            <li> <span class="li-head">ports</span> - Ports to use for scanning (1 - 65535). <span class="li-normal">type: int</span></li>
            <li> <span class="li-head">status</span> - Configure protocol inspection status. <span class="li-normal">type: str</span> <span class="li-normal">choices: disable, deep-inspection</span></li>
            <li> <span class="li-head">unsupported_ssl</span> - Action based on the SSL encryption used being unsupported. <span class="li-normal">type: str</span> <span class="li-normal">choices: bypass, inspect, block</span></li>
            <li> <span class="li-head">untrusted_cert</span> - Allow, ignore, or block the untrusted SSL session server certificate. <span class="li-normal">type: str</span> <span class="li-normal">choices: allow, block, ignore</span></li>
            </ul>
        <li> <span class="li-head">https</span> - Configure HTTPS options. <span class="li-normal">type: dict</span></li>
            <ul class="ul-self">
            <li> <span class="li-head">allow_invalid_server_cert</span> - When enabled, allows SSL sessions whose server certificate validation failed. <span class="li-normal">type: str</span> <span class="li-normal">choices: enable, disable</span></li>
            <li> <span class="li-head">client_cert_request</span> - Action based on client certificate request failure. <span class="li-normal">type: str</span> <span class="li-normal">choices: bypass, inspect, block</span></li>
            <li> <span class="li-head">ports</span> - Ports to use for scanning (1 - 65535). <span class="li-normal">type: int</span></li>
            <li> <span class="li-head">status</span> - Configure protocol inspection status. <span class="li-normal">type: str</span> <span class="li-normal">choices: disable, certificate-inspection, deep-inspection</span></li>
            <li> <span class="li-head">unsupported_ssl</span> - Action based on the SSL encryption used being unsupported. <span class="li-normal">type: str</span> <span class="li-normal">choices: bypass, inspect, block</span></li>
            <li> <span class="li-head">untrusted_cert</span> - Allow, ignore, or block the untrusted SSL session server certificate. <span class="li-normal">type: str</span> <span class="li-normal">choices: allow, block, ignore</span></li>
            </ul>
        <li> <span class="li-head">imaps</span> - Configure IMAPS options. <span class="li-normal">type: dict</span></li>
            <ul class="ul-self">
            <li> <span class="li-head">allow_invalid_server_cert</span> - When enabled, allows SSL sessions whose server certificate validation failed. <span class="li-normal">type: str</span> <span class="li-normal">choices: enable, disable</span></li>
            <li> <span class="li-head">client_cert_request</span> - Action based on client certificate request failure. <span class="li-normal">type: str</span> <span class="li-normal">choices: bypass, inspect, block</span></li>
            <li> <span class="li-head">ports</span> - Ports to use for scanning (1 - 65535). <span class="li-normal">type: int</span></li>
            <li> <span class="li-head">status</span> - Configure protocol inspection status. <span class="li-normal">type: str</span> <span class="li-normal">choices: disable, deep-inspection</span></li>
            <li> <span class="li-head">unsupported_ssl</span> - Action based on the SSL encryption used being unsupported. <span class="li-normal">type: str</span> <span class="li-normal">choices: bypass, inspect, block</span></li>
            <li> <span class="li-head">untrusted_cert</span> - Allow, ignore, or block the untrusted SSL session server certificate. <span class="li-normal">type: str</span> <span class="li-normal">choices: allow, block, ignore</span></li>
            </ul>
        <li> <span class="li-head">mapi_over_https</span> - Enable/disable inspection of MAPI over HTTPS. <span class="li-normal">type: str</span> <span class="li-normal">choices: enable, disable</span></li>
        <li> <span class="li-head">name</span> - Name. <span class="li-normal">type: str</span> <span class="li-required">required: True</span></li>
        <li> <span class="li-head">pop3s</span> - Configure POP3S options. <span class="li-normal">type: dict</span></li>
            <ul class="ul-self">
            <li> <span class="li-head">allow_invalid_server_cert</span> - When enabled, allows SSL sessions whose server certificate validation failed. <span class="li-normal">type: str</span> <span class="li-normal">choices: enable, disable</span></li>
            <li> <span class="li-head">client_cert_request</span> - Action based on client certificate request failure. <span class="li-normal">type: str</span> <span class="li-normal">choices: bypass, inspect, block</span></li>
            <li> <span class="li-head">ports</span> - Ports to use for scanning (1 - 65535). <span class="li-normal">type: int</span></li>
            <li> <span class="li-head">status</span> - Configure protocol inspection status. <span class="li-normal">type: str</span> <span class="li-normal">choices: disable, deep-inspection</span></li>
            <li> <span class="li-head">unsupported_ssl</span> - Action based on the SSL encryption used being unsupported. <span class="li-normal">type: str</span> <span class="li-normal">choices: bypass, inspect, block</span></li>
            <li> <span class="li-head">untrusted_cert</span> - Allow, ignore, or block the untrusted SSL session server certificate. <span class="li-normal">type: str</span> <span class="li-normal">choices: allow, block, ignore</span></li>
            </ul>
        <li> <span class="li-head">rpc_over_https</span> - Enable/disable inspection of RPC over HTTPS. <span class="li-normal">type: str</span> <span class="li-normal">choices: enable, disable</span></li>
        <li> <span class="li-head">server_cert</span> - Certificate used by SSL Inspection to replace server certificate. Source vpn.certificate.local.name. <span class="li-normal">type: str</span></li>
        <li> <span class="li-head">server_cert_mode</span> - Re-sign or replace the server"s certificate. <span class="li-normal">type: str</span> <span class="li-normal">choices: re-sign, replace</span></li>
        <li> <span class="li-head">smtps</span> - Configure SMTPS options. <span class="li-normal">type: dict</span></li>
            <ul class="ul-self">
            <li> <span class="li-head">allow_invalid_server_cert</span> - When enabled, allows SSL sessions whose server certificate validation failed. <span class="li-normal">type: str</span> <span class="li-normal">choices: enable, disable</span></li>
            <li> <span class="li-head">client_cert_request</span> - Action based on client certificate request failure. <span class="li-normal">type: str</span> <span class="li-normal">choices: bypass, inspect, block</span></li>
            <li> <span class="li-head">ports</span> - Ports to use for scanning (1 - 65535). <span class="li-normal">type: int</span></li>
            <li> <span class="li-head">status</span> - Configure protocol inspection status. <span class="li-normal">type: str</span> <span class="li-normal">choices: disable, deep-inspection</span></li>
            <li> <span class="li-head">unsupported_ssl</span> - Action based on the SSL encryption used being unsupported. <span class="li-normal">type: str</span> <span class="li-normal">choices: bypass, inspect, block</span></li>
            <li> <span class="li-head">untrusted_cert</span> - Allow, ignore, or block the untrusted SSL session server certificate. <span class="li-normal">type: str</span> <span class="li-normal">choices: allow, block, ignore</span></li>
            </ul>
        <li> <span class="li-head">ssh</span> - Configure SSH options. <span class="li-normal">type: dict</span></li>
            <ul class="ul-self">
            <li> <span class="li-head">inspect_all</span> - Level of SSL inspection. <span class="li-normal">type: str</span> <span class="li-normal">choices: disable, deep-inspection</span></li>
            <li> <span class="li-head">ports</span> - Ports to use for scanning (1 - 65535). <span class="li-normal">type: int</span></li>
            <li> <span class="li-head">ssh_algorithm</span> - Relative strength of encryption algorithms accepted during negotiation. <span class="li-normal">type: str</span> <span class="li-normal">choices: compatible, high-encryption</span></li>
            <li> <span class="li-head">ssh_policy_check</span> - Enable/disable SSH policy check. <span class="li-normal">type: str</span> <span class="li-normal">choices: disable, enable</span></li>
            <li> <span class="li-head">ssh_tun_policy_check</span> - Enable/disable SSH tunnel policy check. <span class="li-normal">type: str</span> <span class="li-normal">choices: disable, enable</span></li>
            <li> <span class="li-head">status</span> - Configure protocol inspection status. <span class="li-normal">type: str</span> <span class="li-normal">choices: disable, deep-inspection</span></li>
            <li> <span class="li-head">unsupported_version</span> - Action based on SSH version being unsupported. <span class="li-normal">type: str</span> <span class="li-normal">choices: bypass, block</span></li>
            </ul>
        <li> <span class="li-head">ssl</span> - Configure SSL options. <span class="li-normal">type: dict</span></li>
            <ul class="ul-self">
            <li> <span class="li-head">allow_invalid_server_cert</span> - When enabled, allows SSL sessions whose server certificate validation failed. <span class="li-normal">type: str</span> <span class="li-normal">choices: enable, disable</span></li>
            <li> <span class="li-head">client_cert_request</span> - Action based on client certificate request failure. <span class="li-normal">type: str</span> <span class="li-normal">choices: bypass, inspect, block</span></li>
            <li> <span class="li-head">inspect_all</span> - Level of SSL inspection. <span class="li-normal">type: str</span> <span class="li-normal">choices: disable, certificate-inspection, deep-inspection</span></li>
            <li> <span class="li-head">unsupported_ssl</span> - Action based on the SSL encryption used being unsupported. <span class="li-normal">type: str</span> <span class="li-normal">choices: bypass, inspect, block</span></li>
            <li> <span class="li-head">untrusted_cert</span> - Allow, ignore, or block the untrusted SSL session server certificate. <span class="li-normal">type: str</span> <span class="li-normal">choices: allow, block, ignore</span></li>
            </ul>
        <li> <span class="li-head">ssl_anomalies_log</span> - Enable/disable logging SSL anomalies. <span class="li-normal">type: str</span> <span class="li-normal">choices: disable, enable</span></li>
        <li> <span class="li-head">ssl_exempt</span> - Servers to exempt from SSL inspection. <span class="li-normal">type: list</span></li>
            <ul class="ul-self">
            <li> <span class="li-head">address</span> - IPv4 address object. Source firewall.address.name firewall.addrgrp.name. <span class="li-normal">type: str</span></li>
            <li> <span class="li-head">address6</span> - IPv6 address object. Source firewall.address6.name firewall.addrgrp6.name. <span class="li-normal">type: str</span></li>
            <li> <span class="li-head">fortiguard_category</span> - FortiGuard category ID. <span class="li-normal">type: int</span></li>
            <li> <span class="li-head">id</span> - ID number. <span class="li-normal">type: int</span> <span class="li-required">required: True</span></li>
            <li> <span class="li-head">regex</span> - Exempt servers by regular expression. <span class="li-normal">type: str</span></li>
            <li> <span class="li-head">type</span> - Type of address object (IPv4 or IPv6) or FortiGuard category. <span class="li-normal">type: str</span> <span class="li-normal">choices: fortiguard-category, address, address6, wildcard-fqdn, regex</span></li>
            <li> <span class="li-head">wildcard_fqdn</span> - Exempt servers by wildcard FQDN. Source firewall.wildcard-fqdn.custom.name firewall.wildcard-fqdn.group.name. <span class="li-normal">type: str</span></li>
            </ul>
        <li> <span class="li-head">ssl_exemptions_log</span> - Enable/disable logging SSL exemptions. <span class="li-normal">type: str</span> <span class="li-normal">choices: disable, enable</span></li>
        <li> <span class="li-head">ssl_server</span> - SSL servers. <span class="li-normal">type: list</span></li>
            <ul class="ul-self">
            <li> <span class="li-head">ftps_client_cert_request</span> - Action based on client certificate request failure during the FTPS handshake. <span class="li-normal">type: str</span> <span class="li-normal">choices: bypass, inspect, block</span></li>
            <li> <span class="li-head">https_client_cert_request</span> - Action based on client certificate request failure during the HTTPS handshake. <span class="li-normal">type: str</span> <span class="li-normal">choices: bypass, inspect, block</span></li>
            <li> <span class="li-head">id</span> - SSL server ID. <span class="li-normal">type: int</span> <span class="li-required">required: True</span></li>
            <li> <span class="li-head">imaps_client_cert_request</span> - Action based on client certificate request failure during the IMAPS handshake. <span class="li-normal">type: str</span> <span class="li-normal">choices: bypass, inspect, block</span></li>
            <li> <span class="li-head">ip</span> - IPv4 address of the SSL server. <span class="li-normal">type: str</span></li>
            <li> <span class="li-head">pop3s_client_cert_request</span> - Action based on client certificate request failure during the POP3S handshake. <span class="li-normal">type: str</span> <span class="li-normal">choices: bypass, inspect, block</span></li>
            <li> <span class="li-head">smtps_client_cert_request</span> - Action based on client certificate request failure during the SMTPS handshake. <span class="li-normal">type: str</span> <span class="li-normal">choices: bypass, inspect, block</span></li>
            <li> <span class="li-head">ssl_other_client_cert_request</span> - Action based on client certificate request failure during an SSL protocol handshake. <span class="li-normal">type: str</span> <span class="li-normal">choices: bypass, inspect, block</span></li>
            </ul>
        <li> <span class="li-head">untrusted_caname</span> - Untrusted CA certificate used by SSL Inspection. Source vpn.certificate.local.name. <span class="li-normal">type: str</span></li>
        <li> <span class="li-head">use_ssl_server</span> - Enable/disable the use of SSL server table for SSL offloading. <span class="li-normal">type: str</span> <span class="li-normal">choices: disable, enable</span></li>
        <li> <span class="li-head">whitelist</span> - Enable/disable exempting servers by FortiGuard whitelist. <span class="li-normal">type: str</span> <span class="li-normal">choices: enable, disable</span></li>
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
      - name: Configure SSL/SSH protocol options.
        fortios_firewall_ssl_ssh_profile:
          vdom:  "{{ vdom }}"
          state: "present"
          access_token: "<your_own_value>"
          firewall_ssl_ssh_profile:
            caname: "<your_own_value> (source vpn.certificate.local.name)"
            comment: "Optional comments."
            ftps:
                allow_invalid_server_cert: "enable"
                client_cert_request: "bypass"
                ports: "8"
                status: "disable"
                unsupported_ssl: "bypass"
                untrusted_cert: "allow"
            https:
                allow_invalid_server_cert: "enable"
                client_cert_request: "bypass"
                ports: "15"
                status: "disable"
                unsupported_ssl: "bypass"
                untrusted_cert: "allow"
            imaps:
                allow_invalid_server_cert: "enable"
                client_cert_request: "bypass"
                ports: "22"
                status: "disable"
                unsupported_ssl: "bypass"
                untrusted_cert: "allow"
            mapi_over_https: "enable"
            name: "default_name_27"
            pop3s:
                allow_invalid_server_cert: "enable"
                client_cert_request: "bypass"
                ports: "31"
                status: "disable"
                unsupported_ssl: "bypass"
                untrusted_cert: "allow"
            rpc_over_https: "enable"
            server_cert: "<your_own_value> (source vpn.certificate.local.name)"
            server_cert_mode: "re-sign"
            smtps:
                allow_invalid_server_cert: "enable"
                client_cert_request: "bypass"
                ports: "41"
                status: "disable"
                unsupported_ssl: "bypass"
                untrusted_cert: "allow"
            ssh:
                inspect_all: "disable"
                ports: "47"
                ssh_algorithm: "compatible"
                ssh_policy_check: "disable"
                ssh_tun_policy_check: "disable"
                status: "disable"
                unsupported_version: "bypass"
            ssl:
                allow_invalid_server_cert: "enable"
                client_cert_request: "bypass"
                inspect_all: "disable"
                unsupported_ssl: "bypass"
                untrusted_cert: "allow"
            ssl_anomalies_log: "disable"
            ssl_exempt:
             -
                address: "<your_own_value> (source firewall.address.name firewall.addrgrp.name)"
                address6: "<your_own_value> (source firewall.address6.name firewall.addrgrp6.name)"
                fortiguard_category: "63"
                id:  "64"
                regex: "<your_own_value>"
                type: "fortiguard-category"
                wildcard_fqdn: "<your_own_value> (source firewall.wildcard-fqdn.custom.name firewall.wildcard-fqdn.group.name)"
            ssl_exemptions_log: "disable"
            ssl_server:
             -
                ftps_client_cert_request: "bypass"
                https_client_cert_request: "bypass"
                id:  "72"
                imaps_client_cert_request: "bypass"
                ip: "<your_own_value>"
                pop3s_client_cert_request: "bypass"
                smtps_client_cert_request: "bypass"
                ssl_other_client_cert_request: "bypass"
            untrusted_caname: "<your_own_value> (source vpn.certificate.local.name)"
            use_ssl_server: "disable"
            whitelist: "enable"
    


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
