:source: fortios_vpn_ssl_settings.py

:orphan:

.. fortios_vpn_ssl_settings:

fortios_vpn_ssl_settings -- Configure SSL VPN in Fortinet's FortiOS and FortiGate.
++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++

.. versionadded:: 2.8

.. contents::
   :local:
   :depth: 1


Synopsis
--------
- This module is able to configure a FortiGate or FortiOS (FOS) device by allowing the user to set and modify vpn_ssl feature and settings category. Examples include all parameters and values need to be adjusted to datasources before usage. Tested with FOS v6.0.5



Requirements
------------
The below requirements are needed on the host that executes this module.

- ansible>=2.9.0


Parameters
----------


.. raw:: html

    <ul>
    <li> <span class="li-head">host</span> - FortiOS or FortiGate IP address. <span class="li-normal">type: str</span> <span class="li-required">required: False</span></li>
    <li> <span class="li-head">username</span> - FortiOS or FortiGate username. <span class="li-normal">type: str</span> <span class="li-required">required: False</span></li>
    <li> <span class="li-head">password</span> - FortiOS or FortiGate password. <span class="li-normal">type: str</span> <span class="li-normal">default: </span></li>
    <li> <span class="li-head">vdom</span> - Virtual domain, among those defined previously. A vdom is a virtual instance of the FortiGate that can be configured and used as a different unit. <span class="li-normal">type: str</span> <span class="li-normal">default: root</span></li>
    <li> <span class="li-head">https</span> - Indicates if the requests towards FortiGate must use HTTPS protocol. <span class="li-normal">type: bool</span> <span class="li-normal">default: True</span></li>
    <li> <span class="li-head">ssl_verify</span> - Ensures FortiGate certificate must be verified by a proper CA. <span class="li-normal">type: bool</span> <span class="li-normal">default: True</span></li>
    <li> <span class="li-head">vpn_ssl_settings</span> - Configure SSL VPN. <span class="li-normal">type: dict</span></li>
        <ul class="ul-self">
        <li> <span class="li-head">algorithm</span> - Force the SSL-VPN security level. High allows only high. Medium allows medium and high. Low allows any. <span class="li-normal">type: str</span> <span class="li-normal">choices: high, medium, default, low</span></li>
        <li> <span class="li-head">auth_timeout</span> - SSL-VPN authentication timeout (1 - 259200 sec (3 days), 0 for no timeout). <span class="li-normal">type: int</span></li>
        <li> <span class="li-head">authentication_rule</span> - Authentication rule for SSL VPN. <span class="li-normal">type: list</span></li>
            <ul class="ul-self">
            <li> <span class="li-head">auth</span> - SSL VPN authentication method restriction. <span class="li-normal">type: str</span> <span class="li-normal">choices: any, local, radius, tacacs+, ldap</span></li>
            <li> <span class="li-head">cipher</span> - SSL VPN cipher strength. <span class="li-normal">type: str</span> <span class="li-normal">choices: any, high, medium</span></li>
            <li> <span class="li-head">client_cert</span> - Enable/disable SSL VPN client certificate restrictive. <span class="li-normal">type: str</span> <span class="li-normal">choices: enable, disable</span></li>
            <li> <span class="li-head">groups</span> - User groups. <span class="li-normal">type: list</span></li>
                <ul class="ul-self">
                <li> <span class="li-head">name</span> - Group name. Source user.group.name. <span class="li-normal">type: str</span> <span class="li-required">required: True</span></li>
                </ul>
            <li> <span class="li-head">id</span> - ID (0 - 4294967295). <span class="li-normal">type: int</span> <span class="li-required">required: True</span></li>
            <li> <span class="li-head">portal</span> - SSL VPN portal. Source vpn.ssl.web.portal.name. <span class="li-normal">type: str</span></li>
            <li> <span class="li-head">realm</span> - SSL VPN realm. Source vpn.ssl.web.realm.url-path. <span class="li-normal">type: str</span></li>
            <li> <span class="li-head">source_address</span> - Source address of incoming traffic. <span class="li-normal">type: list</span></li>
                <ul class="ul-self">
                <li> <span class="li-head">name</span> - Address name. Source firewall.address.name firewall.addrgrp.name. <span class="li-normal">type: str</span> <span class="li-required">required: True</span></li>
                </ul>
            <li> <span class="li-head">source_address_negate</span> - Enable/disable negated source address match. <span class="li-normal">type: str</span> <span class="li-normal">choices: enable, disable</span></li>
            <li> <span class="li-head">source_address6</span> - IPv6 source address of incoming traffic. <span class="li-normal">type: list</span></li>
                <ul class="ul-self">
                <li> <span class="li-head">name</span> - IPv6 address name. Source firewall.address6.name firewall.addrgrp6.name. <span class="li-normal">type: str</span> <span class="li-required">required: True</span></li>
                </ul>
            <li> <span class="li-head">source_address6_negate</span> - Enable/disable negated source IPv6 address match. <span class="li-normal">type: str</span> <span class="li-normal">choices: enable, disable</span></li>
            <li> <span class="li-head">source_interface</span> - SSL VPN source interface of incoming traffic. <span class="li-normal">type: list</span></li>
                <ul class="ul-self">
                <li> <span class="li-head">name</span> - Interface name. Source system.interface.name system.zone.name. <span class="li-normal">type: str</span> <span class="li-required">required: True</span></li>
                </ul>
            <li> <span class="li-head">users</span> - User name. <span class="li-normal">type: list</span></li>
                <ul class="ul-self">
                <li> <span class="li-head">name</span> - User name. Source user.local.name. <span class="li-normal">type: str</span> <span class="li-required">required: True</span></li>
                </ul>
            </ul>
        <li> <span class="li-head">auto_tunnel_static_route</span> - Enable to auto-create static routes for the SSL-VPN tunnel IP addresses. <span class="li-normal">type: str</span> <span class="li-normal">choices: enable, disable</span></li>
        <li> <span class="li-head">banned_cipher</span> - Select one or more cipher technologies that cannot be used in SSL-VPN negotiations. <span class="li-normal">type: list</span> <span class="li-normal">choices: RSA, DH, DHE, ECDH, ECDHE, DSS, ECDSA, AES, AESGCM, CAMELLIA, 3DES, SHA1, SHA256, SHA384, STATIC</span></li>
        <li> <span class="li-head">check_referer</span> - Enable/disable verification of referer field in HTTP request header. <span class="li-normal">type: str</span> <span class="li-normal">choices: enable, disable</span></li>
        <li> <span class="li-head">default_portal</span> - Default SSL VPN portal. Source vpn.ssl.web.portal.name. <span class="li-normal">type: str</span></li>
        <li> <span class="li-head">deflate_compression_level</span> - Compression level (0~9). <span class="li-normal">type: int</span></li>
        <li> <span class="li-head">deflate_min_data_size</span> - Minimum amount of data that triggers compression (200 - 65535 bytes). <span class="li-normal">type: int</span></li>
        <li> <span class="li-head">dns_server1</span> - DNS server 1. <span class="li-normal">type: str</span></li>
        <li> <span class="li-head">dns_server2</span> - DNS server 2. <span class="li-normal">type: str</span></li>
        <li> <span class="li-head">dns_suffix</span> - DNS suffix used for SSL-VPN clients. <span class="li-normal">type: str</span></li>
        <li> <span class="li-head">dtls_hello_timeout</span> - SSLVPN maximum DTLS hello timeout (10 - 60 sec). <span class="li-normal">type: int</span></li>
        <li> <span class="li-head">dtls_tunnel</span> - Enable DTLS to prevent eavesdropping, tampering, or message forgery. <span class="li-normal">type: str</span> <span class="li-normal">choices: enable, disable</span></li>
        <li> <span class="li-head">force_two_factor_auth</span> - Enable to force two-factor authentication for all SSL-VPNs. <span class="li-normal">type: str</span> <span class="li-normal">choices: enable, disable</span></li>
        <li> <span class="li-head">header_x_forwarded_for</span> - Forward the same, add, or remove HTTP header. <span class="li-normal">type: str</span> <span class="li-normal">choices: pass, add, remove</span></li>
        <li> <span class="li-head">http_compression</span> - Enable to allow HTTP compression over SSL-VPN tunnels. <span class="li-normal">type: str</span> <span class="li-normal">choices: enable, disable</span></li>
        <li> <span class="li-head">http_only_cookie</span> - Enable/disable SSL-VPN support for HttpOnly cookies. <span class="li-normal">type: str</span> <span class="li-normal">choices: enable, disable</span></li>
        <li> <span class="li-head">http_request_body_timeout</span> - SSL-VPN session is disconnected if an HTTP request body is not received within this time (1 - 60 sec). <span class="li-normal">type: int</span></li>
        <li> <span class="li-head">http_request_header_timeout</span> - SSL-VPN session is disconnected if an HTTP request header is not received within this time (1 - 60 sec). <span class="li-normal">type: int</span></li>
        <li> <span class="li-head">https_redirect</span> - Enable/disable redirect of port 80 to SSL-VPN port. <span class="li-normal">type: str</span> <span class="li-normal">choices: enable, disable</span></li>
        <li> <span class="li-head">idle_timeout</span> - SSL VPN disconnects if idle for specified time in seconds. <span class="li-normal">type: int</span></li>
        <li> <span class="li-head">ipv6_dns_server1</span> - IPv6 DNS server 1. <span class="li-normal">type: str</span></li>
        <li> <span class="li-head">ipv6_dns_server2</span> - IPv6 DNS server 2. <span class="li-normal">type: str</span></li>
        <li> <span class="li-head">ipv6_wins_server1</span> - IPv6 WINS server 1. <span class="li-normal">type: str</span></li>
        <li> <span class="li-head">ipv6_wins_server2</span> - IPv6 WINS server 2. <span class="li-normal">type: str</span></li>
        <li> <span class="li-head">login_attempt_limit</span> - SSL VPN maximum login attempt times before block (0 - 10). <span class="li-normal">type: int</span></li>
        <li> <span class="li-head">login_block_time</span> - Time for which a user is blocked from logging in after too many failed login attempts (0 - 86400 sec). <span class="li-normal">type: int</span></li>
        <li> <span class="li-head">login_timeout</span> - SSLVPN maximum login timeout (10 - 180 sec). <span class="li-normal">type: int</span></li>
        <li> <span class="li-head">port</span> - SSL-VPN access port (1 - 65535). <span class="li-normal">type: int</span></li>
        <li> <span class="li-head">port_precedence</span> - Enable means that if SSL-VPN connections are allowed on an interface admin GUI connections are blocked on that interface. <span class="li-normal">type: str</span> <span class="li-normal">choices: enable, disable</span></li>
        <li> <span class="li-head">reqclientcert</span> - Enable to require client certificates for all SSL-VPN users. <span class="li-normal">type: str</span> <span class="li-normal">choices: enable, disable</span></li>
        <li> <span class="li-head">route_source_interface</span> - Enable to allow SSL-VPN sessions to bypass routing and bind to the incoming interface. <span class="li-normal">type: str</span> <span class="li-normal">choices: enable, disable</span></li>
        <li> <span class="li-head">servercert</span> - Name of the server certificate to be used for SSL-VPNs. Source vpn.certificate.local.name. <span class="li-normal">type: str</span></li>
        <li> <span class="li-head">source_address</span> - Source address of incoming traffic. <span class="li-normal">type: list</span></li>
            <ul class="ul-self">
            <li> <span class="li-head">name</span> - Address name. Source firewall.address.name firewall.addrgrp.name. <span class="li-normal">type: str</span> <span class="li-required">required: True</span></li>
            </ul>
        <li> <span class="li-head">source_address_negate</span> - Enable/disable negated source address match. <span class="li-normal">type: str</span> <span class="li-normal">choices: enable, disable</span></li>
        <li> <span class="li-head">source_address6</span> - IPv6 source address of incoming traffic. <span class="li-normal">type: list</span></li>
            <ul class="ul-self">
            <li> <span class="li-head">name</span> - IPv6 address name. Source firewall.address6.name firewall.addrgrp6.name. <span class="li-normal">type: str</span> <span class="li-required">required: True</span></li>
            </ul>
        <li> <span class="li-head">source_address6_negate</span> - Enable/disable negated source IPv6 address match. <span class="li-normal">type: str</span> <span class="li-normal">choices: enable, disable</span></li>
        <li> <span class="li-head">source_interface</span> - SSL VPN source interface of incoming traffic. <span class="li-normal">type: list</span></li>
            <ul class="ul-self">
            <li> <span class="li-head">name</span> - Interface name. Source system.interface.name system.zone.name. <span class="li-normal">type: str</span> <span class="li-required">required: True</span></li>
            </ul>
        <li> <span class="li-head">ssl_client_renegotiation</span> - Enable to allow client renegotiation by the server if the tunnel goes down. <span class="li-normal">type: str</span> <span class="li-normal">choices: disable, enable</span></li>
        <li> <span class="li-head">ssl_insert_empty_fragment</span> - Enable/disable insertion of empty fragment. <span class="li-normal">type: str</span> <span class="li-normal">choices: enable, disable</span></li>
        <li> <span class="li-head">tlsv1_0</span> - Enable/disable TLSv1.0. <span class="li-normal">type: str</span> <span class="li-normal">choices: enable, disable</span></li>
        <li> <span class="li-head">tlsv1_1</span> - Enable/disable TLSv1.1. <span class="li-normal">type: str</span> <span class="li-normal">choices: enable, disable</span></li>
        <li> <span class="li-head">tlsv1_2</span> - Enable/disable TLSv1.2. <span class="li-normal">type: str</span> <span class="li-normal">choices: enable, disable</span></li>
        <li> <span class="li-head">tunnel_ip_pools</span> - Names of the IPv4 IP Pool firewall objects that define the IP addresses reserved for remote clients. <span class="li-normal">type: list</span></li>
            <ul class="ul-self">
            <li> <span class="li-head">name</span> - Address name. Source firewall.address.name firewall.addrgrp.name. <span class="li-normal">type: str</span> <span class="li-required">required: True</span></li>
            </ul>
        <li> <span class="li-head">tunnel_ipv6_pools</span> - Names of the IPv6 IP Pool firewall objects that define the IP addresses reserved for remote clients. <span class="li-normal">type: list</span></li>
            <ul class="ul-self">
            <li> <span class="li-head">name</span> - Address name. Source firewall.address6.name firewall.addrgrp6.name. <span class="li-normal">type: str</span> <span class="li-required">required: True</span></li>
            </ul>
        <li> <span class="li-head">unsafe_legacy_renegotiation</span> - Enable/disable unsafe legacy re-negotiation. <span class="li-normal">type: str</span> <span class="li-normal">choices: enable, disable</span></li>
        <li> <span class="li-head">url_obscuration</span> - Enable to obscure the host name of the URL of the web browser display. <span class="li-normal">type: str</span> <span class="li-normal">choices: enable, disable</span></li>
        <li> <span class="li-head">wins_server1</span> - WINS server 1. <span class="li-normal">type: str</span></li>
        <li> <span class="li-head">wins_server2</span> - WINS server 2. <span class="li-normal">type: str</span></li>
        <li> <span class="li-head">x_content_type_options</span> - Add HTTP X-Content-Type-Options header. <span class="li-normal">type: str</span> <span class="li-normal">choices: enable, disable</span></li>
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
      - name: Configure SSL VPN.
        fortios_vpn_ssl_settings:
          vdom:  "{{ vdom }}"
          vpn_ssl_settings:
            algorithm: "high"
            auth_timeout: "4"
            authentication_rule:
             -
                auth: "any"
                cipher: "any"
                client_cert: "enable"
                groups:
                 -
                    name: "default_name_10 (source user.group.name)"
                id:  "11"
                portal: "<your_own_value> (source vpn.ssl.web.portal.name)"
                realm: "<your_own_value> (source vpn.ssl.web.realm.url-path)"
                source_address:
                 -
                    name: "default_name_15 (source firewall.address.name firewall.addrgrp.name)"
                source_address_negate: "enable"
                source_address6:
                 -
                    name: "default_name_18 (source firewall.address6.name firewall.addrgrp6.name)"
                source_address6_negate: "enable"
                source_interface:
                 -
                    name: "default_name_21 (source system.interface.name system.zone.name)"
                users:
                 -
                    name: "default_name_23 (source user.local.name)"
            auto_tunnel_static_route: "enable"
            banned_cipher: "RSA"
            check_referer: "enable"
            default_portal: "<your_own_value> (source vpn.ssl.web.portal.name)"
            deflate_compression_level: "28"
            deflate_min_data_size: "29"
            dns_server1: "<your_own_value>"
            dns_server2: "<your_own_value>"
            dns_suffix: "<your_own_value>"
            dtls_hello_timeout: "33"
            dtls_tunnel: "enable"
            force_two_factor_auth: "enable"
            header_x_forwarded_for: "pass"
            http_compression: "enable"
            http_only_cookie: "enable"
            http_request_body_timeout: "39"
            http_request_header_timeout: "40"
            https_redirect: "enable"
            idle_timeout: "42"
            ipv6_dns_server1: "<your_own_value>"
            ipv6_dns_server2: "<your_own_value>"
            ipv6_wins_server1: "<your_own_value>"
            ipv6_wins_server2: "<your_own_value>"
            login_attempt_limit: "47"
            login_block_time: "48"
            login_timeout: "49"
            port: "50"
            port_precedence: "enable"
            reqclientcert: "enable"
            route_source_interface: "enable"
            servercert: "<your_own_value> (source vpn.certificate.local.name)"
            source_address:
             -
                name: "default_name_56 (source firewall.address.name firewall.addrgrp.name)"
            source_address_negate: "enable"
            source_address6:
             -
                name: "default_name_59 (source firewall.address6.name firewall.addrgrp6.name)"
            source_address6_negate: "enable"
            source_interface:
             -
                name: "default_name_62 (source system.interface.name system.zone.name)"
            ssl_client_renegotiation: "disable"
            ssl_insert_empty_fragment: "enable"
            tlsv1_0: "enable"
            tlsv1_1: "enable"
            tlsv1_2: "enable"
            tunnel_ip_pools:
             -
                name: "default_name_69 (source firewall.address.name firewall.addrgrp.name)"
            tunnel_ipv6_pools:
             -
                name: "default_name_71 (source firewall.address6.name firewall.addrgrp6.name)"
            unsafe_legacy_renegotiation: "enable"
            url_obscuration: "enable"
            wins_server1: "<your_own_value>"
            wins_server2: "<your_own_value>"
            x_content_type_options: "enable"


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
- Hongbin Lu (@fgtdev-hblu)
- Frank Shen (@frankshen01)
- Jie Xue (@JieX19)
- Miguel Angel Munoz (@mamunozgonzalez)
- Nicolas Thomas (@thomnico)


.. hint::
    If you notice any issues in this documentation, you can create a pull request to improve it.
