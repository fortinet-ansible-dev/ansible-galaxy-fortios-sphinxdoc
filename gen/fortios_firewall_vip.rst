:source: fortios_firewall_vip.py

:orphan:

.. fortios_firewall_vip:

fortios_firewall_vip -- Configure virtual IP for IPv4 in Fortinet's FortiOS and FortiGate.
++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++

.. versionadded:: 2.8

.. contents::
   :local:
   :depth: 1


Synopsis
--------
- This module is able to configure a FortiGate or FortiOS (FOS) device by allowing the user to set and modify firewall feature and vip category. Examples include all parameters and values need to be adjusted to datasources before usage. Tested with FOS v6.0.5



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
    <li> <span class="li-head">state</span> - Indicates whether to create or remove the object. This attribute was present already in previous version in a deeper level. It has been moved out to this outer level. <span class="li-normal">type: str</span> <span class="li-required">required: False</span> <span class="li-normal">choices: present, absent</span></li>
    <li> <span class="li-head">firewall_vip</span> - Configure virtual IP for IPv4. <span class="li-normal">type: dict</span></li>
        <ul class="ul-self">
        <li> <span class="li-head">state</span> - B(Deprecated) <span class="li-normal">type: str</span> <span class="li-required">required: False</span> <span class="li-normal">choices: present, absent</span></li>
        <li> <span class="li-head">arp_reply</span> - Enable to respond to ARP requests for this virtual IP address. Enabled by default. <span class="li-normal">type: str</span> <span class="li-normal">choices: disable, enable</span></li>
        <li> <span class="li-head">color</span> - Color of icon on the GUI. <span class="li-normal">type: int</span></li>
        <li> <span class="li-head">comment</span> - Comment. <span class="li-normal">type: str</span></li>
        <li> <span class="li-head">dns_mapping_ttl</span> - DNS mapping TTL (Set to zero to use TTL in DNS response). <span class="li-normal">type: int</span></li>
        <li> <span class="li-head">extaddr</span> - External FQDN address name. <span class="li-normal">type: list</span></li>
            <ul class="ul-self">
            <li> <span class="li-head">name</span> - Address name. Source firewall.address.name firewall.addrgrp.name. <span class="li-normal">type: str</span> <span class="li-required">required: True</span></li>
            </ul>
        <li> <span class="li-head">extintf</span> - Interface connected to the source network that receives the packets that will be forwarded to the destination network. Source system .interface.name. <span class="li-normal">type: str</span></li>
        <li> <span class="li-head">extip</span> - IP address or address range on the external interface that you want to map to an address or address range on the destination network. <span class="li-normal">type: str</span></li>
        <li> <span class="li-head">extport</span> - Incoming port number range that you want to map to a port number range on the destination network. <span class="li-normal">type: str</span></li>
        <li> <span class="li-head">gratuitous_arp_interval</span> - Enable to have the VIP send gratuitous ARPs. 0=disabled. Set from 5 up to 8640000 seconds to enable. <span class="li-normal">type: int</span></li>
        <li> <span class="li-head">http_cookie_age</span> - Time in minutes that client web browsers should keep a cookie. Default is 60 seconds. 0 = no time limit. <span class="li-normal">type: int</span></li>
        <li> <span class="li-head">http_cookie_domain</span> - Domain that HTTP cookie persistence should apply to. <span class="li-normal">type: str</span></li>
        <li> <span class="li-head">http_cookie_domain_from_host</span> - Enable/disable use of HTTP cookie domain from host field in HTTP. <span class="li-normal">type: str</span> <span class="li-normal">choices: disable, enable</span></li>
        <li> <span class="li-head">http_cookie_generation</span> - Generation of HTTP cookie to be accepted. Changing invalidates all existing cookies. <span class="li-normal">type: int</span></li>
        <li> <span class="li-head">http_cookie_path</span> - Limit HTTP cookie persistence to the specified path. <span class="li-normal">type: str</span></li>
        <li> <span class="li-head">http_cookie_share</span> - Control sharing of cookies across virtual servers. same-ip means a cookie from one virtual server can be used by another. Disable stops cookie sharing. <span class="li-normal">type: str</span> <span class="li-normal">choices: disable, same-ip</span></li>
        <li> <span class="li-head">http_ip_header</span> - For HTTP multiplexing, enable to add the original client IP address in the XForwarded-For HTTP header. <span class="li-normal">type: str</span> <span class="li-normal">choices: enable, disable</span></li>
        <li> <span class="li-head">http_ip_header_name</span> - For HTTP multiplexing, enter a custom HTTPS header name. The original client IP address is added to this header. If empty, X-Forwarded-For is used. <span class="li-normal">type: str</span></li>
        <li> <span class="li-head">http_multiplex</span> - Enable/disable HTTP multiplexing. <span class="li-normal">type: str</span> <span class="li-normal">choices: enable, disable</span></li>
        <li> <span class="li-head">https_cookie_secure</span> - Enable/disable verification that inserted HTTPS cookies are secure. <span class="li-normal">type: str</span> <span class="li-normal">choices: disable, enable</span></li>
        <li> <span class="li-head">id</span> - Custom defined ID. <span class="li-normal">type: int</span></li>
        <li> <span class="li-head">ldb_method</span> - Method used to distribute sessions to real servers. <span class="li-normal">type: str</span> <span class="li-normal">choices: static, round-robin, weighted, least-session, least-rtt, first-alive, http-host</span></li>
        <li> <span class="li-head">mapped_addr</span> - Mapped FQDN address name. Source firewall.address.name. <span class="li-normal">type: str</span></li>
        <li> <span class="li-head">mappedip</span> - IP address or address range on the destination network to which the external IP address is mapped. <span class="li-normal">type: list</span></li>
            <ul class="ul-self">
            <li> <span class="li-head">range</span> - Mapped IP range. <span class="li-normal">type: str</span> <span class="li-required">required: True</span></li>
            </ul>
        <li> <span class="li-head">mappedport</span> - Port number range on the destination network to which the external port number range is mapped. <span class="li-normal">type: str</span></li>
        <li> <span class="li-head">max_embryonic_connections</span> - Maximum number of incomplete connections. <span class="li-normal">type: int</span></li>
        <li> <span class="li-head">monitor</span> - Name of the health check monitor to use when polling to determine a virtual server"s connectivity status. <span class="li-normal">type: list</span></li>
            <ul class="ul-self">
            <li> <span class="li-head">name</span> - Health monitor name. Source firewall.ldb-monitor.name. <span class="li-normal">type: str</span> <span class="li-required">required: True</span></li>
            </ul>
        <li> <span class="li-head">name</span> - Virtual IP name. <span class="li-normal">type: str</span> <span class="li-required">required: True</span></li>
        <li> <span class="li-head">nat_source_vip</span> - Enable/disable forcing the source NAT mapped IP to the external IP for all traffic. <span class="li-normal">type: str</span> <span class="li-normal">choices: disable, enable</span></li>
        <li> <span class="li-head">outlook_web_access</span> - Enable to add the Front-End-Https header for Microsoft Outlook Web Access. <span class="li-normal">type: str</span> <span class="li-normal">choices: disable, enable</span></li>
        <li> <span class="li-head">persistence</span> - Configure how to make sure that clients connect to the same server every time they make a request that is part of the same session. <span class="li-normal">type: str</span> <span class="li-normal">choices: none, http-cookie, ssl-session-id</span></li>
        <li> <span class="li-head">portforward</span> - Enable/disable port forwarding. <span class="li-normal">type: str</span> <span class="li-normal">choices: disable, enable</span></li>
        <li> <span class="li-head">portmapping_type</span> - Port mapping type. <span class="li-normal">type: str</span> <span class="li-normal">choices: 1-to-1, m-to-n</span></li>
        <li> <span class="li-head">protocol</span> - Protocol to use when forwarding packets. <span class="li-normal">type: str</span> <span class="li-normal">choices: tcp, udp, sctp, icmp</span></li>
        <li> <span class="li-head">realservers</span> - Select the real servers that this server load balancing VIP will distribute traffic to. <span class="li-normal">type: list</span></li>
            <ul class="ul-self">
            <li> <span class="li-head">client_ip</span> - Only clients in this IP range can connect to this real server. <span class="li-normal">type: str</span></li>
            <li> <span class="li-head">healthcheck</span> - Enable to check the responsiveness of the real server before forwarding traffic. <span class="li-normal">type: str</span> <span class="li-normal">choices: disable, enable, vip</span></li>
            <li> <span class="li-head">holddown_interval</span> - Time in seconds that the health check monitor continues to monitor and unresponsive server that should be active. <span class="li-normal">type: int</span></li>
            <li> <span class="li-head">http_host</span> - HTTP server domain name in HTTP header. <span class="li-normal">type: str</span></li>
            <li> <span class="li-head">id</span> - Real server ID. <span class="li-normal">type: int</span> <span class="li-required">required: True</span></li>
            <li> <span class="li-head">ip</span> - IP address of the real server. <span class="li-normal">type: str</span></li>
            <li> <span class="li-head">max_connections</span> - Max number of active connections that can be directed to the real server. When reached, sessions are sent to other real servers. <span class="li-normal">type: int</span></li>
            <li> <span class="li-head">monitor</span> - Name of the health check monitor to use when polling to determine a virtual server"s connectivity status. Source firewall .ldb-monitor.name. <span class="li-normal">type: str</span></li>
            <li> <span class="li-head">port</span> - Port for communicating with the real server. Required if port forwarding is enabled. <span class="li-normal">type: int</span></li>
            <li> <span class="li-head">status</span> - Set the status of the real server to active so that it can accept traffic, or on standby or disabled so no traffic is sent. <span class="li-normal">type: str</span> <span class="li-normal">choices: active, standby, disable</span></li>
            <li> <span class="li-head">weight</span> - Weight of the real server. If weighted load balancing is enabled, the server with the highest weight gets more connections. <span class="li-normal">type: int</span></li>
            </ul>
        <li> <span class="li-head">server_type</span> - Protocol to be load balanced by the virtual server (also called the server load balance virtual IP). <span class="li-normal">type: str</span> <span class="li-normal">choices: http, https, imaps, pop3s, smtps, ssl, tcp, udp, ip</span></li>
        <li> <span class="li-head">service</span> - Service name. <span class="li-normal">type: list</span></li>
            <ul class="ul-self">
            <li> <span class="li-head">name</span> - Service name. Source firewall.service.custom.name firewall.service.group.name. <span class="li-normal">type: str</span> <span class="li-required">required: True</span></li>
            </ul>
        <li> <span class="li-head">src_filter</span> - Source address filter. Each address must be either an IP/subnet (x.x.x.x/n) or a range (x.x.x.x-y.y.y.y). Separate addresses with spaces. <span class="li-normal">type: list</span></li>
            <ul class="ul-self">
            <li> <span class="li-head">range</span> - Source-filter range. <span class="li-normal">type: str</span> <span class="li-required">required: True</span></li>
            </ul>
        <li> <span class="li-head">srcintf_filter</span> - Interfaces to which the VIP applies. Separate the names with spaces. <span class="li-normal">type: list</span></li>
            <ul class="ul-self">
            <li> <span class="li-head">interface_name</span> - Interface name. Source system.interface.name. <span class="li-normal">type: str</span></li>
            </ul>
        <li> <span class="li-head">ssl_algorithm</span> - Permitted encryption algorithms for SSL sessions according to encryption strength. <span class="li-normal">type: str</span> <span class="li-normal">choices: high, medium, low, custom</span></li>
        <li> <span class="li-head">ssl_certificate</span> - The name of the SSL certificate to use for SSL acceleration. Source vpn.certificate.local.name. <span class="li-normal">type: str</span></li>
        <li> <span class="li-head">ssl_cipher_suites</span> - SSL/TLS cipher suites acceptable from a client, ordered by priority. <span class="li-normal">type: list</span></li>
            <ul class="ul-self">
            <li> <span class="li-head">cipher</span> - Cipher suite name. <span class="li-normal">type: str</span> <span class="li-normal">choices: TLS-ECDHE-RSA-WITH-CHACHA20-POLY1305-SHA256, TLS-ECDHE-ECDSA-WITH-CHACHA20-POLY1305-SHA256, TLS-DHE-RSA-WITH-CHACHA20-POLY1305-SHA256, TLS-DHE-RSA-WITH-AES-128-CBC-SHA, TLS-DHE-RSA-WITH-AES-256-CBC-SHA, TLS-DHE-RSA-WITH-AES-128-CBC-SHA256, TLS-DHE-RSA-WITH-AES-128-GCM-SHA256, TLS-DHE-RSA-WITH-AES-256-CBC-SHA256, TLS-DHE-RSA-WITH-AES-256-GCM-SHA384, TLS-DHE-DSS-WITH-AES-128-CBC-SHA, TLS-DHE-DSS-WITH-AES-256-CBC-SHA, TLS-DHE-DSS-WITH-AES-128-CBC-SHA256, TLS-DHE-DSS-WITH-AES-128-GCM-SHA256, TLS-DHE-DSS-WITH-AES-256-CBC-SHA256, TLS-DHE-DSS-WITH-AES-256-GCM-SHA384, TLS-ECDHE-RSA-WITH-AES-128-CBC-SHA, TLS-ECDHE-RSA-WITH-AES-128-CBC-SHA256, TLS-ECDHE-RSA-WITH-AES-128-GCM-SHA256, TLS-ECDHE-RSA-WITH-AES-256-CBC-SHA, TLS-ECDHE-RSA-WITH-AES-256-CBC-SHA384, TLS-ECDHE-RSA-WITH-AES-256-GCM-SHA384, TLS-ECDHE-ECDSA-WITH-AES-128-CBC-SHA, TLS-ECDHE-ECDSA-WITH-AES-128-CBC-SHA256, TLS-ECDHE-ECDSA-WITH-AES-128-GCM-SHA256, TLS-ECDHE-ECDSA-WITH-AES-256-CBC-SHA384, TLS-ECDHE-ECDSA-WITH-AES-256-GCM-SHA384, TLS-RSA-WITH-AES-128-CBC-SHA, TLS-RSA-WITH-AES-256-CBC-SHA, TLS-RSA-WITH-AES-128-CBC-SHA256, TLS-RSA-WITH-AES-128-GCM-SHA256, TLS-RSA-WITH-AES-256-CBC-SHA256, TLS-RSA-WITH-AES-256-GCM-SHA384, TLS-RSA-WITH-CAMELLIA-128-CBC-SHA, TLS-RSA-WITH-CAMELLIA-256-CBC-SHA, TLS-RSA-WITH-CAMELLIA-128-CBC-SHA256, TLS-RSA-WITH-CAMELLIA-256-CBC-SHA256, TLS-DHE-RSA-WITH-3DES-EDE-CBC-SHA, TLS-DHE-RSA-WITH-CAMELLIA-128-CBC-SHA, TLS-DHE-DSS-WITH-CAMELLIA-128-CBC-SHA, TLS-DHE-RSA-WITH-CAMELLIA-256-CBC-SHA, TLS-DHE-DSS-WITH-CAMELLIA-256-CBC-SHA, TLS-DHE-RSA-WITH-CAMELLIA-128-CBC-SHA256, TLS-DHE-DSS-WITH-CAMELLIA-128-CBC-SHA256, TLS-DHE-RSA-WITH-CAMELLIA-256-CBC-SHA256, TLS-DHE-DSS-WITH-CAMELLIA-256-CBC-SHA256, TLS-DHE-RSA-WITH-SEED-CBC-SHA, TLS-DHE-DSS-WITH-SEED-CBC-SHA, TLS-DHE-RSA-WITH-ARIA-128-CBC-SHA256, TLS-DHE-RSA-WITH-ARIA-256-CBC-SHA384, TLS-DHE-DSS-WITH-ARIA-128-CBC-SHA256, TLS-DHE-DSS-WITH-ARIA-256-CBC-SHA384, TLS-RSA-WITH-SEED-CBC-SHA, TLS-RSA-WITH-ARIA-128-CBC-SHA256, TLS-RSA-WITH-ARIA-256-CBC-SHA384, TLS-ECDHE-RSA-WITH-ARIA-128-CBC-SHA256, TLS-ECDHE-RSA-WITH-ARIA-256-CBC-SHA384, TLS-ECDHE-ECDSA-WITH-ARIA-128-CBC-SHA256, TLS-ECDHE-ECDSA-WITH-ARIA-256-CBC-SHA384, TLS-ECDHE-RSA-WITH-RC4-128-SHA, TLS-ECDHE-RSA-WITH-3DES-EDE-CBC-SHA, TLS-DHE-DSS-WITH-3DES-EDE-CBC-SHA, TLS-RSA-WITH-3DES-EDE-CBC-SHA, TLS-RSA-WITH-RC4-128-MD5, TLS-RSA-WITH-RC4-128-SHA, TLS-DHE-RSA-WITH-DES-CBC-SHA, TLS-DHE-DSS-WITH-DES-CBC-SHA, TLS-RSA-WITH-DES-CBC-SHA</span></li>
            <li> <span class="li-head">priority</span> - SSL/TLS cipher suites priority. <span class="li-normal">type: int</span> <span class="li-required">required: True</span></li>
            <li> <span class="li-head">versions</span> - SSL/TLS versions that the cipher suite can be used with. <span class="li-normal">type: str</span> <span class="li-normal">choices: ssl-3.0, tls-1.0, tls-1.1, tls-1.2</span></li>
            </ul>
        <li> <span class="li-head">ssl_client_fallback</span> - Enable/disable support for preventing Downgrade Attacks on client connections (RFC 7507). <span class="li-normal">type: str</span> <span class="li-normal">choices: disable, enable</span></li>
        <li> <span class="li-head">ssl_client_renegotiation</span> - Allow, deny, or require secure renegotiation of client sessions to comply with RFC 5746. <span class="li-normal">type: str</span> <span class="li-normal">choices: allow, deny, secure</span></li>
        <li> <span class="li-head">ssl_client_session_state_max</span> - Maximum number of client to FortiGate SSL session states to keep. <span class="li-normal">type: int</span></li>
        <li> <span class="li-head">ssl_client_session_state_timeout</span> - Number of minutes to keep client to FortiGate SSL session state. <span class="li-normal">type: int</span></li>
        <li> <span class="li-head">ssl_client_session_state_type</span> - How to expire SSL sessions for the segment of the SSL connection between the client and the FortiGate. <span class="li-normal">type: str</span> <span class="li-normal">choices: disable, time, count, both</span></li>
        <li> <span class="li-head">ssl_dh_bits</span> - Number of bits to use in the Diffie-Hellman exchange for RSA encryption of SSL sessions. <span class="li-normal">type: str</span> <span class="li-normal">choices: 768, 1024, 1536, 2048, 3072, 4096</span></li>
        <li> <span class="li-head">ssl_hpkp</span> - Enable/disable including HPKP header in response. <span class="li-normal">type: str</span> <span class="li-normal">choices: disable, enable, report-only</span></li>
        <li> <span class="li-head">ssl_hpkp_age</span> - Number of seconds the client should honour the HPKP setting. <span class="li-normal">type: int</span></li>
        <li> <span class="li-head">ssl_hpkp_backup</span> - Certificate to generate backup HPKP pin from. Source vpn.certificate.local.name vpn.certificate.ca.name. <span class="li-normal">type: str</span></li>
        <li> <span class="li-head">ssl_hpkp_include_subdomains</span> - Indicate that HPKP header applies to all subdomains. <span class="li-normal">type: str</span> <span class="li-normal">choices: disable, enable</span></li>
        <li> <span class="li-head">ssl_hpkp_primary</span> - Certificate to generate primary HPKP pin from. Source vpn.certificate.local.name vpn.certificate.ca.name. <span class="li-normal">type: str</span></li>
        <li> <span class="li-head">ssl_hpkp_report_uri</span> - URL to report HPKP violations to. <span class="li-normal">type: str</span></li>
        <li> <span class="li-head">ssl_hsts</span> - Enable/disable including HSTS header in response. <span class="li-normal">type: str</span> <span class="li-normal">choices: disable, enable</span></li>
        <li> <span class="li-head">ssl_hsts_age</span> - Number of seconds the client should honour the HSTS setting. <span class="li-normal">type: int</span></li>
        <li> <span class="li-head">ssl_hsts_include_subdomains</span> - Indicate that HSTS header applies to all subdomains. <span class="li-normal">type: str</span> <span class="li-normal">choices: disable, enable</span></li>
        <li> <span class="li-head">ssl_http_location_conversion</span> - Enable to replace HTTP with HTTPS in the reply"s Location HTTP header field. <span class="li-normal">type: str</span> <span class="li-normal">choices: enable, disable</span></li>
        <li> <span class="li-head">ssl_http_match_host</span> - Enable/disable HTTP host matching for location conversion. <span class="li-normal">type: str</span> <span class="li-normal">choices: enable, disable</span></li>
        <li> <span class="li-head">ssl_max_version</span> - Highest SSL/TLS version acceptable from a client. <span class="li-normal">type: str</span> <span class="li-normal">choices: ssl-3.0, tls-1.0, tls-1.1, tls-1.2</span></li>
        <li> <span class="li-head">ssl_min_version</span> - Lowest SSL/TLS version acceptable from a client. <span class="li-normal">type: str</span> <span class="li-normal">choices: ssl-3.0, tls-1.0, tls-1.1, tls-1.2</span></li>
        <li> <span class="li-head">ssl_mode</span> - Apply SSL offloading between the client and the FortiGate (half) or from the client to the FortiGate and from the FortiGate to the server (full). <span class="li-normal">type: str</span> <span class="li-normal">choices: half, full</span></li>
        <li> <span class="li-head">ssl_pfs</span> - Select the cipher suites that can be used for SSL perfect forward secrecy (PFS). Applies to both client and server sessions. <span class="li-normal">type: str</span> <span class="li-normal">choices: require, deny, allow</span></li>
        <li> <span class="li-head">ssl_send_empty_frags</span> - Enable/disable sending empty fragments to avoid CBC IV attacks (SSL 3.0 & TLS 1.0 only). May need to be disabled for compatibility with older systems. <span class="li-normal">type: str</span> <span class="li-normal">choices: enable, disable</span></li>
        <li> <span class="li-head">ssl_server_algorithm</span> - Permitted encryption algorithms for the server side of SSL full mode sessions according to encryption strength. <span class="li-normal">type: str</span> <span class="li-normal">choices: high, medium, low, custom, client</span></li>
        <li> <span class="li-head">ssl_server_cipher_suites</span> - SSL/TLS cipher suites to offer to a server, ordered by priority. <span class="li-normal">type: list</span></li>
            <ul class="ul-self">
            <li> <span class="li-head">cipher</span> - Cipher suite name. <span class="li-normal">type: str</span> <span class="li-normal">choices: TLS-ECDHE-RSA-WITH-CHACHA20-POLY1305-SHA256, TLS-ECDHE-ECDSA-WITH-CHACHA20-POLY1305-SHA256, TLS-DHE-RSA-WITH-CHACHA20-POLY1305-SHA256, TLS-DHE-RSA-WITH-AES-128-CBC-SHA, TLS-DHE-RSA-WITH-AES-256-CBC-SHA, TLS-DHE-RSA-WITH-AES-128-CBC-SHA256, TLS-DHE-RSA-WITH-AES-128-GCM-SHA256, TLS-DHE-RSA-WITH-AES-256-CBC-SHA256, TLS-DHE-RSA-WITH-AES-256-GCM-SHA384, TLS-DHE-DSS-WITH-AES-128-CBC-SHA, TLS-DHE-DSS-WITH-AES-256-CBC-SHA, TLS-DHE-DSS-WITH-AES-128-CBC-SHA256, TLS-DHE-DSS-WITH-AES-128-GCM-SHA256, TLS-DHE-DSS-WITH-AES-256-CBC-SHA256, TLS-DHE-DSS-WITH-AES-256-GCM-SHA384, TLS-ECDHE-RSA-WITH-AES-128-CBC-SHA, TLS-ECDHE-RSA-WITH-AES-128-CBC-SHA256, TLS-ECDHE-RSA-WITH-AES-128-GCM-SHA256, TLS-ECDHE-RSA-WITH-AES-256-CBC-SHA, TLS-ECDHE-RSA-WITH-AES-256-CBC-SHA384, TLS-ECDHE-RSA-WITH-AES-256-GCM-SHA384, TLS-ECDHE-ECDSA-WITH-AES-128-CBC-SHA, TLS-ECDHE-ECDSA-WITH-AES-128-CBC-SHA256, TLS-ECDHE-ECDSA-WITH-AES-128-GCM-SHA256, TLS-ECDHE-ECDSA-WITH-AES-256-CBC-SHA384, TLS-ECDHE-ECDSA-WITH-AES-256-GCM-SHA384, TLS-RSA-WITH-AES-128-CBC-SHA, TLS-RSA-WITH-AES-256-CBC-SHA, TLS-RSA-WITH-AES-128-CBC-SHA256, TLS-RSA-WITH-AES-128-GCM-SHA256, TLS-RSA-WITH-AES-256-CBC-SHA256, TLS-RSA-WITH-AES-256-GCM-SHA384, TLS-RSA-WITH-CAMELLIA-128-CBC-SHA, TLS-RSA-WITH-CAMELLIA-256-CBC-SHA, TLS-RSA-WITH-CAMELLIA-128-CBC-SHA256, TLS-RSA-WITH-CAMELLIA-256-CBC-SHA256, TLS-DHE-RSA-WITH-3DES-EDE-CBC-SHA, TLS-DHE-RSA-WITH-CAMELLIA-128-CBC-SHA, TLS-DHE-DSS-WITH-CAMELLIA-128-CBC-SHA, TLS-DHE-RSA-WITH-CAMELLIA-256-CBC-SHA, TLS-DHE-DSS-WITH-CAMELLIA-256-CBC-SHA, TLS-DHE-RSA-WITH-CAMELLIA-128-CBC-SHA256, TLS-DHE-DSS-WITH-CAMELLIA-128-CBC-SHA256, TLS-DHE-RSA-WITH-CAMELLIA-256-CBC-SHA256, TLS-DHE-DSS-WITH-CAMELLIA-256-CBC-SHA256, TLS-DHE-RSA-WITH-SEED-CBC-SHA, TLS-DHE-DSS-WITH-SEED-CBC-SHA, TLS-DHE-RSA-WITH-ARIA-128-CBC-SHA256, TLS-DHE-RSA-WITH-ARIA-256-CBC-SHA384, TLS-DHE-DSS-WITH-ARIA-128-CBC-SHA256, TLS-DHE-DSS-WITH-ARIA-256-CBC-SHA384, TLS-RSA-WITH-SEED-CBC-SHA, TLS-RSA-WITH-ARIA-128-CBC-SHA256, TLS-RSA-WITH-ARIA-256-CBC-SHA384, TLS-ECDHE-RSA-WITH-ARIA-128-CBC-SHA256, TLS-ECDHE-RSA-WITH-ARIA-256-CBC-SHA384, TLS-ECDHE-ECDSA-WITH-ARIA-128-CBC-SHA256, TLS-ECDHE-ECDSA-WITH-ARIA-256-CBC-SHA384, TLS-ECDHE-RSA-WITH-RC4-128-SHA, TLS-ECDHE-RSA-WITH-3DES-EDE-CBC-SHA, TLS-DHE-DSS-WITH-3DES-EDE-CBC-SHA, TLS-RSA-WITH-3DES-EDE-CBC-SHA, TLS-RSA-WITH-RC4-128-MD5, TLS-RSA-WITH-RC4-128-SHA, TLS-DHE-RSA-WITH-DES-CBC-SHA, TLS-DHE-DSS-WITH-DES-CBC-SHA, TLS-RSA-WITH-DES-CBC-SHA</span></li>
            <li> <span class="li-head">priority</span> - SSL/TLS cipher suites priority. <span class="li-normal">type: int</span> <span class="li-required">required: True</span></li>
            <li> <span class="li-head">versions</span> - SSL/TLS versions that the cipher suite can be used with. <span class="li-normal">type: str</span> <span class="li-normal">choices: ssl-3.0, tls-1.0, tls-1.1, tls-1.2</span></li>
            </ul>
        <li> <span class="li-head">ssl_server_max_version</span> - Highest SSL/TLS version acceptable from a server. Use the client setting by default. <span class="li-normal">type: str</span> <span class="li-normal">choices: ssl-3.0, tls-1.0, tls-1.1, tls-1.2, client</span></li>
        <li> <span class="li-head">ssl_server_min_version</span> - Lowest SSL/TLS version acceptable from a server. Use the client setting by default. <span class="li-normal">type: str</span> <span class="li-normal">choices: ssl-3.0, tls-1.0, tls-1.1, tls-1.2, client</span></li>
        <li> <span class="li-head">ssl_server_session_state_max</span> - Maximum number of FortiGate to Server SSL session states to keep. <span class="li-normal">type: int</span></li>
        <li> <span class="li-head">ssl_server_session_state_timeout</span> - Number of minutes to keep FortiGate to Server SSL session state. <span class="li-normal">type: int</span></li>
        <li> <span class="li-head">ssl_server_session_state_type</span> - How to expire SSL sessions for the segment of the SSL connection between the server and the FortiGate. <span class="li-normal">type: str</span> <span class="li-normal">choices: disable, time, count, both</span></li>
        <li> <span class="li-head">type</span> - Configure a static NAT, load balance, server load balance, DNS translation, or FQDN VIP. <span class="li-normal">type: str</span> <span class="li-normal">choices: static-nat, load-balance, server-load-balance, dns-translation, fqdn</span></li>
        <li> <span class="li-head">uuid</span> - Universally Unique Identifier (UUID; automatically assigned but can be manually reset). <span class="li-normal">type: str</span></li>
        <li> <span class="li-head">weblogic_server</span> - Enable to add an HTTP header to indicate SSL offloading for a WebLogic server. <span class="li-normal">type: str</span> <span class="li-normal">choices: disable, enable</span></li>
        <li> <span class="li-head">websphere_server</span> - Enable to add an HTTP header to indicate SSL offloading for a WebSphere server. <span class="li-normal">type: str</span> <span class="li-normal">choices: disable, enable</span></li>
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
      - name: Configure virtual IP for IPv4.
        fortios_firewall_vip:
          vdom:  "{{ vdom }}"
          state: "present"
          firewall_vip:
            arp_reply: "disable"
            color: "4"
            comment: "Comment."
            dns_mapping_ttl: "6"
            extaddr:
             -
                name: "default_name_8 (source firewall.address.name firewall.addrgrp.name)"
            extintf: "<your_own_value> (source system.interface.name)"
            extip: "<your_own_value>"
            extport: "<your_own_value>"
            gratuitous_arp_interval: "12"
            http_cookie_age: "13"
            http_cookie_domain: "<your_own_value>"
            http_cookie_domain_from_host: "disable"
            http_cookie_generation: "16"
            http_cookie_path: "<your_own_value>"
            http_cookie_share: "disable"
            http_ip_header: "enable"
            http_ip_header_name: "<your_own_value>"
            http_multiplex: "enable"
            https_cookie_secure: "disable"
            id:  "23"
            ldb_method: "static"
            mapped_addr: "<your_own_value> (source firewall.address.name)"
            mappedip:
             -
                range: "<your_own_value>"
            mappedport: "<your_own_value>"
            max_embryonic_connections: "29"
            monitor:
             -
                name: "default_name_31 (source firewall.ldb-monitor.name)"
            name: "default_name_32"
            nat_source_vip: "disable"
            outlook_web_access: "disable"
            persistence: "none"
            portforward: "disable"
            portmapping_type: "1-to-1"
            protocol: "tcp"
            realservers:
             -
                client_ip: "<your_own_value>"
                healthcheck: "disable"
                holddown_interval: "42"
                http_host: "myhostname"
                id:  "44"
                ip: "<your_own_value>"
                max_connections: "46"
                monitor: "<your_own_value> (source firewall.ldb-monitor.name)"
                port: "48"
                status: "active"
                weight: "50"
            server_type: "http"
            service:
             -
                name: "default_name_53 (source firewall.service.custom.name firewall.service.group.name)"
            src_filter:
             -
                range: "<your_own_value>"
            srcintf_filter:
             -
                interface_name: "<your_own_value> (source system.interface.name)"
            ssl_algorithm: "high"
            ssl_certificate: "<your_own_value> (source vpn.certificate.local.name)"
            ssl_cipher_suites:
             -
                cipher: "TLS-ECDHE-RSA-WITH-CHACHA20-POLY1305-SHA256"
                priority: "62"
                versions: "ssl-3.0"
            ssl_client_fallback: "disable"
            ssl_client_renegotiation: "allow"
            ssl_client_session_state_max: "66"
            ssl_client_session_state_timeout: "67"
            ssl_client_session_state_type: "disable"
            ssl_dh_bits: "768"
            ssl_hpkp: "disable"
            ssl_hpkp_age: "71"
            ssl_hpkp_backup: "<your_own_value> (source vpn.certificate.local.name vpn.certificate.ca.name)"
            ssl_hpkp_include_subdomains: "disable"
            ssl_hpkp_primary: "<your_own_value> (source vpn.certificate.local.name vpn.certificate.ca.name)"
            ssl_hpkp_report_uri: "<your_own_value>"
            ssl_hsts: "disable"
            ssl_hsts_age: "77"
            ssl_hsts_include_subdomains: "disable"
            ssl_http_location_conversion: "enable"
            ssl_http_match_host: "enable"
            ssl_max_version: "ssl-3.0"
            ssl_min_version: "ssl-3.0"
            ssl_mode: "half"
            ssl_pfs: "require"
            ssl_send_empty_frags: "enable"
            ssl_server_algorithm: "high"
            ssl_server_cipher_suites:
             -
                cipher: "TLS-ECDHE-RSA-WITH-CHACHA20-POLY1305-SHA256"
                priority: "89"
                versions: "ssl-3.0"
            ssl_server_max_version: "ssl-3.0"
            ssl_server_min_version: "ssl-3.0"
            ssl_server_session_state_max: "93"
            ssl_server_session_state_timeout: "94"
            ssl_server_session_state_type: "disable"
            type: "static-nat"
            uuid: "<your_own_value>"
            weblogic_server: "disable"
            websphere_server: "disable"


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
