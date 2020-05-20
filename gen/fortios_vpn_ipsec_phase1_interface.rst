:source: fortios_vpn_ipsec_phase1_interface.py

:orphan:

.. fortios_vpn_ipsec_phase1_interface:

fortios_vpn_ipsec_phase1_interface -- Configure VPN remote gateway in Fortinet's FortiOS and FortiGate.
+++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++

.. versionadded:: 2.8

.. contents::
   :local:
   :depth: 1


Synopsis
--------
- This module is able to configure a FortiGate or FortiOS (FOS) device by allowing the user to set and modify vpn_ipsec feature and phase1_interface category. Examples include all parameters and values need to be adjusted to datasources before usage. Tested with FOS v6.0.5



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
    <li> <span class="li-head">vpn_ipsec_phase1_interface</span> - Configure VPN remote gateway. <span class="li-normal">type: dict</span></li>
        <ul class="ul-self">
        <li> <span class="li-head">state</span> - B(Deprecated) <span class="li-normal">type: str</span> <span class="li-required">required: False</span> <span class="li-normal">choices: present, absent</span></li>
        <li> <span class="li-head">acct_verify</span> - Enable/disable verification of RADIUS accounting record. <span class="li-normal">type: str</span> <span class="li-normal">choices: enable, disable</span></li>
        <li> <span class="li-head">add_gw_route</span> - Enable/disable automatically add a route to the remote gateway. <span class="li-normal">type: str</span> <span class="li-normal">choices: enable, disable</span></li>
        <li> <span class="li-head">add_route</span> - Enable/disable control addition of a route to peer destination selector. <span class="li-normal">type: str</span> <span class="li-normal">choices: disable, enable</span></li>
        <li> <span class="li-head">assign_ip</span> - Enable/disable assignment of IP to IPsec interface via configuration method. <span class="li-normal">type: str</span> <span class="li-normal">choices: disable, enable</span></li>
        <li> <span class="li-head">assign_ip_from</span> - Method by which the IP address will be assigned. <span class="li-normal">type: str</span> <span class="li-normal">choices: range, usrgrp, dhcp, name</span></li>
        <li> <span class="li-head">authmethod</span> - Authentication method. <span class="li-normal">type: str</span> <span class="li-normal">choices: psk, signature</span></li>
        <li> <span class="li-head">authmethod_remote</span> - Authentication method (remote side). <span class="li-normal">type: str</span> <span class="li-normal">choices: psk, signature</span></li>
        <li> <span class="li-head">authpasswd</span> - XAuth password (max 35 characters). <span class="li-normal">type: str</span></li>
        <li> <span class="li-head">authusr</span> - XAuth user name. <span class="li-normal">type: str</span></li>
        <li> <span class="li-head">authusrgrp</span> - Authentication user group. Source user.group.name. <span class="li-normal">type: str</span></li>
        <li> <span class="li-head">auto_discovery_forwarder</span> - Enable/disable forwarding auto-discovery short-cut messages. <span class="li-normal">type: str</span> <span class="li-normal">choices: enable, disable</span></li>
        <li> <span class="li-head">auto_discovery_psk</span> - Enable/disable use of pre-shared secrets for authentication of auto-discovery tunnels. <span class="li-normal">type: str</span> <span class="li-normal">choices: enable, disable</span></li>
        <li> <span class="li-head">auto_discovery_receiver</span> - Enable/disable accepting auto-discovery short-cut messages. <span class="li-normal">type: str</span> <span class="li-normal">choices: enable, disable</span></li>
        <li> <span class="li-head">auto_discovery_sender</span> - Enable/disable sending auto-discovery short-cut messages. <span class="li-normal">type: str</span> <span class="li-normal">choices: enable, disable</span></li>
        <li> <span class="li-head">auto_negotiate</span> - Enable/disable automatic initiation of IKE SA negotiation. <span class="li-normal">type: str</span> <span class="li-normal">choices: enable, disable</span></li>
        <li> <span class="li-head">backup_gateway</span> - Instruct unity clients about the backup gateway address(es). <span class="li-normal">type: list</span></li>
            <ul class="ul-self">
            <li> <span class="li-head">address</span> - Address of backup gateway. <span class="li-normal">type: str</span> <span class="li-required">required: True</span></li>
            </ul>
        <li> <span class="li-head">banner</span> - Message that unity client should display after connecting. <span class="li-normal">type: str</span></li>
        <li> <span class="li-head">cert_id_validation</span> - Enable/disable cross validation of peer ID and the identity in the peer"s certificate as specified in RFC 4945. <span class="li-normal">type: str</span> <span class="li-normal">choices: enable, disable</span></li>
        <li> <span class="li-head">certificate</span> - The names of up to 4 signed personal certificates. <span class="li-normal">type: list</span></li>
            <ul class="ul-self">
            <li> <span class="li-head">name</span> - Certificate name. Source vpn.certificate.local.name. <span class="li-normal">type: str</span> <span class="li-required">required: True</span></li>
            </ul>
        <li> <span class="li-head">childless_ike</span> - Enable/disable childless IKEv2 initiation (RFC 6023). <span class="li-normal">type: str</span> <span class="li-normal">choices: enable, disable</span></li>
        <li> <span class="li-head">client_auto_negotiate</span> - Enable/disable allowing the VPN client to bring up the tunnel when there is no traffic. <span class="li-normal">type: str</span> <span class="li-normal">choices: disable, enable</span></li>
        <li> <span class="li-head">client_keep_alive</span> - Enable/disable allowing the VPN client to keep the tunnel up when there is no traffic. <span class="li-normal">type: str</span> <span class="li-normal">choices: disable, enable</span></li>
        <li> <span class="li-head">comments</span> - Comment. <span class="li-normal">type: str</span></li>
        <li> <span class="li-head">default_gw</span> - IPv4 address of default route gateway to use for traffic exiting the interface. <span class="li-normal">type: str</span></li>
        <li> <span class="li-head">default_gw_priority</span> - Priority for default gateway route. A higher priority number signifies a less preferred route. <span class="li-normal">type: int</span></li>
        <li> <span class="li-head">dhgrp</span> - DH group. <span class="li-normal">type: str</span> <span class="li-normal">choices: 1, 2, 5, 14, 15, 16, 17, 18, 19, 20, 21, 27, 28, 29, 30, 31</span></li>
        <li> <span class="li-head">digital_signature_auth</span> - Enable/disable IKEv2 Digital Signature Authentication (RFC 7427). <span class="li-normal">type: str</span> <span class="li-normal">choices: enable, disable</span></li>
        <li> <span class="li-head">distance</span> - Distance for routes added by IKE (1 - 255). <span class="li-normal">type: int</span></li>
        <li> <span class="li-head">dns_mode</span> - DNS server mode. <span class="li-normal">type: str</span> <span class="li-normal">choices: manual, auto</span></li>
        <li> <span class="li-head">domain</span> - Instruct unity clients about the default DNS domain. <span class="li-normal">type: str</span></li>
        <li> <span class="li-head">dpd</span> - Dead Peer Detection mode. <span class="li-normal">type: str</span> <span class="li-normal">choices: disable, on-idle, on-demand</span></li>
        <li> <span class="li-head">dpd_retrycount</span> - Number of DPD retry attempts. <span class="li-normal">type: int</span></li>
        <li> <span class="li-head">dpd_retryinterval</span> - DPD retry interval. <span class="li-normal">type: str</span></li>
        <li> <span class="li-head">eap</span> - Enable/disable IKEv2 EAP authentication. <span class="li-normal">type: str</span> <span class="li-normal">choices: enable, disable</span></li>
        <li> <span class="li-head">eap_identity</span> - IKEv2 EAP peer identity type. <span class="li-normal">type: str</span> <span class="li-normal">choices: use-id-payload, send-request</span></li>
        <li> <span class="li-head">encap_local_gw4</span> - Local IPv4 address of GRE/VXLAN tunnel. <span class="li-normal">type: str</span></li>
        <li> <span class="li-head">encap_local_gw6</span> - Local IPv6 address of GRE/VXLAN tunnel. <span class="li-normal">type: str</span></li>
        <li> <span class="li-head">encap_remote_gw4</span> - Remote IPv4 address of GRE/VXLAN tunnel. <span class="li-normal">type: str</span></li>
        <li> <span class="li-head">encap_remote_gw6</span> - Remote IPv6 address of GRE/VXLAN tunnel. <span class="li-normal">type: str</span></li>
        <li> <span class="li-head">encapsulation</span> - Enable/disable GRE/VXLAN encapsulation. <span class="li-normal">type: str</span> <span class="li-normal">choices: none, gre, vxlan</span></li>
        <li> <span class="li-head">encapsulation_address</span> - Source for GRE/VXLAN tunnel address. <span class="li-normal">type: str</span> <span class="li-normal">choices: ike, ipv4, ipv6</span></li>
        <li> <span class="li-head">enforce_unique_id</span> - Enable/disable peer ID uniqueness check. <span class="li-normal">type: str</span> <span class="li-normal">choices: disable, keep-new, keep-old</span></li>
        <li> <span class="li-head">exchange_interface_ip</span> - Enable/disable exchange of IPsec interface IP address. <span class="li-normal">type: str</span> <span class="li-normal">choices: enable, disable</span></li>
        <li> <span class="li-head">exchange_ip_addr4</span> - IPv4 address to exchange with peers. <span class="li-normal">type: str</span></li>
        <li> <span class="li-head">exchange_ip_addr6</span> - IPv6 address to exchange with peers <span class="li-normal">type: str</span></li>
        <li> <span class="li-head">forticlient_enforcement</span> - Enable/disable FortiClient enforcement. <span class="li-normal">type: str</span> <span class="li-normal">choices: enable, disable</span></li>
        <li> <span class="li-head">fragmentation</span> - Enable/disable fragment IKE message on re-transmission. <span class="li-normal">type: str</span> <span class="li-normal">choices: enable, disable</span></li>
        <li> <span class="li-head">fragmentation_mtu</span> - IKE fragmentation MTU (500 - 16000). <span class="li-normal">type: int</span></li>
        <li> <span class="li-head">group_authentication</span> - Enable/disable IKEv2 IDi group authentication. <span class="li-normal">type: str</span> <span class="li-normal">choices: enable, disable</span></li>
        <li> <span class="li-head">group_authentication_secret</span> - Password for IKEv2 IDi group authentication.  (ASCII string or hexadecimal indicated by a leading 0x.) <span class="li-normal">type: str</span></li>
        <li> <span class="li-head">ha_sync_esp_seqno</span> - Enable/disable sequence number jump ahead for IPsec HA. <span class="li-normal">type: str</span> <span class="li-normal">choices: enable, disable</span></li>
        <li> <span class="li-head">idle_timeout</span> - Enable/disable IPsec tunnel idle timeout. <span class="li-normal">type: str</span> <span class="li-normal">choices: enable, disable</span></li>
        <li> <span class="li-head">idle_timeoutinterval</span> - IPsec tunnel idle timeout in minutes (5 - 43200). <span class="li-normal">type: int</span></li>
        <li> <span class="li-head">ike_version</span> - IKE protocol version. <span class="li-normal">type: str</span> <span class="li-normal">choices: 1, 2</span></li>
        <li> <span class="li-head">include_local_lan</span> - Enable/disable allow local LAN access on unity clients. <span class="li-normal">type: str</span> <span class="li-normal">choices: disable, enable</span></li>
        <li> <span class="li-head">interface</span> - Local physical, aggregate, or VLAN outgoing interface. Source system.interface.name. <span class="li-normal">type: str</span></li>
        <li> <span class="li-head">ip_version</span> - IP version to use for VPN interface. <span class="li-normal">type: str</span> <span class="li-normal">choices: 4, 6</span></li>
        <li> <span class="li-head">ipv4_dns_server1</span> - IPv4 DNS server 1. <span class="li-normal">type: str</span></li>
        <li> <span class="li-head">ipv4_dns_server2</span> - IPv4 DNS server 2. <span class="li-normal">type: str</span></li>
        <li> <span class="li-head">ipv4_dns_server3</span> - IPv4 DNS server 3. <span class="li-normal">type: str</span></li>
        <li> <span class="li-head">ipv4_end_ip</span> - End of IPv4 range. <span class="li-normal">type: str</span></li>
        <li> <span class="li-head">ipv4_exclude_range</span> - Configuration Method IPv4 exclude ranges. <span class="li-normal">type: list</span></li>
            <ul class="ul-self">
            <li> <span class="li-head">end_ip</span> - End of IPv4 exclusive range. <span class="li-normal">type: str</span></li>
            <li> <span class="li-head">id</span> - ID. <span class="li-normal">type: int</span> <span class="li-required">required: True</span></li>
            <li> <span class="li-head">start_ip</span> - Start of IPv4 exclusive range. <span class="li-normal">type: str</span></li>
            </ul>
        <li> <span class="li-head">ipv4_name</span> - IPv4 address name. Source firewall.address.name firewall.addrgrp.name. <span class="li-normal">type: str</span></li>
        <li> <span class="li-head">ipv4_netmask</span> - IPv4 Netmask. <span class="li-normal">type: str</span></li>
        <li> <span class="li-head">ipv4_split_exclude</span> - IPv4 subnets that should not be sent over the IPsec tunnel. Source firewall.address.name firewall.addrgrp.name. <span class="li-normal">type: str</span></li>
        <li> <span class="li-head">ipv4_split_include</span> - IPv4 split-include subnets. Source firewall.address.name firewall.addrgrp.name. <span class="li-normal">type: str</span></li>
        <li> <span class="li-head">ipv4_start_ip</span> - Start of IPv4 range. <span class="li-normal">type: str</span></li>
        <li> <span class="li-head">ipv4_wins_server1</span> - WINS server 1. <span class="li-normal">type: str</span></li>
        <li> <span class="li-head">ipv4_wins_server2</span> - WINS server 2. <span class="li-normal">type: str</span></li>
        <li> <span class="li-head">ipv6_dns_server1</span> - IPv6 DNS server 1. <span class="li-normal">type: str</span></li>
        <li> <span class="li-head">ipv6_dns_server2</span> - IPv6 DNS server 2. <span class="li-normal">type: str</span></li>
        <li> <span class="li-head">ipv6_dns_server3</span> - IPv6 DNS server 3. <span class="li-normal">type: str</span></li>
        <li> <span class="li-head">ipv6_end_ip</span> - End of IPv6 range. <span class="li-normal">type: str</span></li>
        <li> <span class="li-head">ipv6_exclude_range</span> - Configuration method IPv6 exclude ranges. <span class="li-normal">type: list</span></li>
            <ul class="ul-self">
            <li> <span class="li-head">end_ip</span> - End of IPv6 exclusive range. <span class="li-normal">type: str</span></li>
            <li> <span class="li-head">id</span> - ID. <span class="li-normal">type: int</span> <span class="li-required">required: True</span></li>
            <li> <span class="li-head">start_ip</span> - Start of IPv6 exclusive range. <span class="li-normal">type: str</span></li>
            </ul>
        <li> <span class="li-head">ipv6_name</span> - IPv6 address name. Source firewall.address6.name firewall.addrgrp6.name. <span class="li-normal">type: str</span></li>
        <li> <span class="li-head">ipv6_prefix</span> - IPv6 prefix. <span class="li-normal">type: int</span></li>
        <li> <span class="li-head">ipv6_split_exclude</span> - IPv6 subnets that should not be sent over the IPsec tunnel. Source firewall.address6.name firewall.addrgrp6.name. <span class="li-normal">type: str</span></li>
        <li> <span class="li-head">ipv6_split_include</span> - IPv6 split-include subnets. Source firewall.address6.name firewall.addrgrp6.name. <span class="li-normal">type: str</span></li>
        <li> <span class="li-head">ipv6_start_ip</span> - Start of IPv6 range. <span class="li-normal">type: str</span></li>
        <li> <span class="li-head">keepalive</span> - NAT-T keep alive interval. <span class="li-normal">type: int</span></li>
        <li> <span class="li-head">keylife</span> - Time to wait in seconds before phase 1 encryption key expires. <span class="li-normal">type: int</span></li>
        <li> <span class="li-head">local_gw</span> - IPv4 address of the local gateway"s external interface. <span class="li-normal">type: str</span></li>
        <li> <span class="li-head">local_gw6</span> - IPv6 address of the local gateway"s external interface. <span class="li-normal">type: str</span></li>
        <li> <span class="li-head">localid</span> - Local ID. <span class="li-normal">type: str</span></li>
        <li> <span class="li-head">localid_type</span> - Local ID type. <span class="li-normal">type: str</span> <span class="li-normal">choices: auto, fqdn, user-fqdn, keyid, address, asn1dn</span></li>
        <li> <span class="li-head">mesh_selector_type</span> - Add selectors containing subsets of the configuration depending on traffic. <span class="li-normal">type: str</span> <span class="li-normal">choices: disable, subnet, host</span></li>
        <li> <span class="li-head">mode</span> - The ID protection mode used to establish a secure channel. <span class="li-normal">type: str</span> <span class="li-normal">choices: aggressive, main</span></li>
        <li> <span class="li-head">mode_cfg</span> - Enable/disable configuration method. <span class="li-normal">type: str</span> <span class="li-normal">choices: disable, enable</span></li>
        <li> <span class="li-head">monitor</span> - IPsec interface as backup for primary interface. Source vpn.ipsec.phase1-interface.name. <span class="li-normal">type: str</span></li>
        <li> <span class="li-head">monitor_hold_down_delay</span> - Time to wait in seconds before recovery once primary re-establishes. <span class="li-normal">type: int</span></li>
        <li> <span class="li-head">monitor_hold_down_time</span> - Time of day at which to fail back to primary after it re-establishes. <span class="li-normal">type: str</span></li>
        <li> <span class="li-head">monitor_hold_down_type</span> - Recovery time method when primary interface re-establishes. <span class="li-normal">type: str</span> <span class="li-normal">choices: immediate, delay, time</span></li>
        <li> <span class="li-head">monitor_hold_down_weekday</span> - Day of the week to recover once primary re-establishes. <span class="li-normal">type: str</span> <span class="li-normal">choices: everyday, sunday, monday, tuesday, wednesday, thursday, friday, saturday</span></li>
        <li> <span class="li-head">name</span> - IPsec remote gateway name. <span class="li-normal">type: str</span> <span class="li-required">required: True</span></li>
        <li> <span class="li-head">nattraversal</span> - Enable/disable NAT traversal. <span class="li-normal">type: str</span> <span class="li-normal">choices: enable, disable, forced</span></li>
        <li> <span class="li-head">negotiate_timeout</span> - IKE SA negotiation timeout in seconds (1 - 300). <span class="li-normal">type: int</span></li>
        <li> <span class="li-head">net_device</span> - Enable/disable kernel device creation for dialup instances. <span class="li-normal">type: str</span> <span class="li-normal">choices: enable, disable</span></li>
        <li> <span class="li-head">passive_mode</span> - Enable/disable IPsec passive mode for static tunnels. <span class="li-normal">type: str</span> <span class="li-normal">choices: enable, disable</span></li>
        <li> <span class="li-head">peer</span> - Accept this peer certificate. Source user.peer.name. <span class="li-normal">type: str</span></li>
        <li> <span class="li-head">peergrp</span> - Accept this peer certificate group. Source user.peergrp.name. <span class="li-normal">type: str</span></li>
        <li> <span class="li-head">peerid</span> - Accept this peer identity. <span class="li-normal">type: str</span></li>
        <li> <span class="li-head">peertype</span> - Accept this peer type. <span class="li-normal">type: str</span> <span class="li-normal">choices: any, one, dialup, peer, peergrp</span></li>
        <li> <span class="li-head">ppk</span> - Enable/disable IKEv2 Postquantum Preshared Key (PPK). <span class="li-normal">type: str</span> <span class="li-normal">choices: disable, allow, require</span></li>
        <li> <span class="li-head">ppk_identity</span> - IKEv2 Postquantum Preshared Key Identity. <span class="li-normal">type: str</span></li>
        <li> <span class="li-head">ppk_secret</span> - IKEv2 Postquantum Preshared Key (ASCII string or hexadecimal encoded with a leading 0x). <span class="li-normal">type: str</span></li>
        <li> <span class="li-head">priority</span> - Priority for routes added by IKE (0 - 4294967295). <span class="li-normal">type: int</span></li>
        <li> <span class="li-head">proposal</span> - Phase1 proposal. <span class="li-normal">type: list</span> <span class="li-normal">choices: des-md5, des-sha1, des-sha256, des-sha384, des-sha512, 3des-md5, 3des-sha1, 3des-sha256, 3des-sha384, 3des-sha512, aes128-md5, aes128-sha1, aes128-sha256, aes128-sha384, aes128-sha512, aes128gcm-prfsha1, aes128gcm-prfsha256, aes128gcm-prfsha384, aes128gcm-prfsha512, aes192-md5, aes192-sha1, aes192-sha256, aes192-sha384, aes192-sha512, aes256-md5, aes256-sha1, aes256-sha256, aes256-sha384, aes256-sha512, aes256gcm-prfsha1, aes256gcm-prfsha256, aes256gcm-prfsha384, aes256gcm-prfsha512, chacha20poly1305-prfsha1, chacha20poly1305-prfsha256, chacha20poly1305-prfsha384, chacha20poly1305-prfsha512, aria128-md5, aria128-sha1, aria128-sha256, aria128-sha384, aria128-sha512, aria192-md5, aria192-sha1, aria192-sha256, aria192-sha384, aria192-sha512, aria256-md5, aria256-sha1, aria256-sha256, aria256-sha384, aria256-sha512, seed-md5, seed-sha1, seed-sha256, seed-sha384, seed-sha512</span></li>
        <li> <span class="li-head">psksecret</span> - Pre-shared secret for PSK authentication (ASCII string or hexadecimal encoded with a leading 0x). <span class="li-normal">type: str</span></li>
        <li> <span class="li-head">psksecret_remote</span> - Pre-shared secret for remote side PSK authentication (ASCII string or hexadecimal encoded with a leading 0x). <span class="li-normal">type: str</span></li>
        <li> <span class="li-head">reauth</span> - Enable/disable re-authentication upon IKE SA lifetime expiration. <span class="li-normal">type: str</span> <span class="li-normal">choices: disable, enable</span></li>
        <li> <span class="li-head">rekey</span> - Enable/disable phase1 rekey. <span class="li-normal">type: str</span> <span class="li-normal">choices: enable, disable</span></li>
        <li> <span class="li-head">remote_gw</span> - IPv4 address of the remote gateway"s external interface. <span class="li-normal">type: str</span></li>
        <li> <span class="li-head">remote_gw6</span> - IPv6 address of the remote gateway"s external interface. <span class="li-normal">type: str</span></li>
        <li> <span class="li-head">remotegw_ddns</span> - Domain name of remote gateway (eg. name.DDNS.com). <span class="li-normal">type: str</span></li>
        <li> <span class="li-head">rsa_signature_format</span> - Digital Signature Authentication RSA signature format. <span class="li-normal">type: str</span> <span class="li-normal">choices: pkcs1, pss</span></li>
        <li> <span class="li-head">save_password</span> - Enable/disable saving XAuth username and password on VPN clients. <span class="li-normal">type: str</span> <span class="li-normal">choices: disable, enable</span></li>
        <li> <span class="li-head">send_cert_chain</span> - Enable/disable sending certificate chain. <span class="li-normal">type: str</span> <span class="li-normal">choices: enable, disable</span></li>
        <li> <span class="li-head">signature_hash_alg</span> - Digital Signature Authentication hash algorithms. <span class="li-normal">type: str</span> <span class="li-normal">choices: sha1, sha2-256, sha2-384, sha2-512</span></li>
        <li> <span class="li-head">split_include_service</span> - Split-include services. Source firewall.service.group.name firewall.service.custom.name. <span class="li-normal">type: str</span></li>
        <li> <span class="li-head">suite_b</span> - Use Suite-B. <span class="li-normal">type: str</span> <span class="li-normal">choices: disable, suite-b-gcm-128, suite-b-gcm-256</span></li>
        <li> <span class="li-head">tunnel_search</span> - Tunnel search method for when the interface is shared. <span class="li-normal">type: str</span> <span class="li-normal">choices: selectors, nexthop</span></li>
        <li> <span class="li-head">type</span> - Remote gateway type. <span class="li-normal">type: str</span> <span class="li-normal">choices: static, dynamic, ddns</span></li>
        <li> <span class="li-head">unity_support</span> - Enable/disable support for Cisco UNITY Configuration Method extensions. <span class="li-normal">type: str</span> <span class="li-normal">choices: disable, enable</span></li>
        <li> <span class="li-head">usrgrp</span> - User group name for dialup peers. Source user.group.name. <span class="li-normal">type: str</span></li>
        <li> <span class="li-head">vni</span> - VNI of VXLAN tunnel. <span class="li-normal">type: int</span></li>
        <li> <span class="li-head">wizard_type</span> - GUI VPN Wizard Type. <span class="li-normal">type: str</span> <span class="li-normal">choices: custom, dialup-forticlient, dialup-ios, dialup-android, dialup-windows, dialup-cisco, static-fortigate, dialup-fortigate, static-cisco, dialup-cisco-fw</span></li>
        <li> <span class="li-head">xauthtype</span> - XAuth type. <span class="li-normal">type: str</span> <span class="li-normal">choices: disable, client, pap, chap, auto</span></li>
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
      - name: Configure VPN remote gateway.
        fortios_vpn_ipsec_phase1_interface:
          vdom:  "{{ vdom }}"
          state: "present"
          vpn_ipsec_phase1_interface:
            acct_verify: "enable"
            add_gw_route: "enable"
            add_route: "disable"
            assign_ip: "disable"
            assign_ip_from: "range"
            authmethod: "psk"
            authmethod_remote: "psk"
            authpasswd: "<your_own_value>"
            authusr: "<your_own_value>"
            authusrgrp: "<your_own_value> (source user.group.name)"
            auto_discovery_forwarder: "enable"
            auto_discovery_psk: "enable"
            auto_discovery_receiver: "enable"
            auto_discovery_sender: "enable"
            auto_negotiate: "enable"
            backup_gateway:
             -
                address: "<your_own_value>"
            banner: "<your_own_value>"
            cert_id_validation: "enable"
            certificate:
             -
                name: "default_name_23 (source vpn.certificate.local.name)"
            childless_ike: "enable"
            client_auto_negotiate: "disable"
            client_keep_alive: "disable"
            comments: "<your_own_value>"
            default_gw: "<your_own_value>"
            default_gw_priority: "29"
            dhgrp: "1"
            digital_signature_auth: "enable"
            distance: "32"
            dns_mode: "manual"
            domain: "<your_own_value>"
            dpd: "disable"
            dpd_retrycount: "36"
            dpd_retryinterval: "<your_own_value>"
            eap: "enable"
            eap_identity: "use-id-payload"
            encap_local_gw4: "<your_own_value>"
            encap_local_gw6: "<your_own_value>"
            encap_remote_gw4: "<your_own_value>"
            encap_remote_gw6: "<your_own_value>"
            encapsulation: "none"
            encapsulation_address: "ike"
            enforce_unique_id: "disable"
            exchange_interface_ip: "enable"
            exchange_ip_addr4: "<your_own_value>"
            exchange_ip_addr6: "<your_own_value>"
            forticlient_enforcement: "enable"
            fragmentation: "enable"
            fragmentation_mtu: "52"
            group_authentication: "enable"
            group_authentication_secret: "<your_own_value>"
            ha_sync_esp_seqno: "enable"
            idle_timeout: "enable"
            idle_timeoutinterval: "57"
            ike_version: "1"
            include_local_lan: "disable"
            interface: "<your_own_value> (source system.interface.name)"
            ip_version: "4"
            ipv4_dns_server1: "<your_own_value>"
            ipv4_dns_server2: "<your_own_value>"
            ipv4_dns_server3: "<your_own_value>"
            ipv4_end_ip: "<your_own_value>"
            ipv4_exclude_range:
             -
                end_ip: "<your_own_value>"
                id:  "68"
                start_ip: "<your_own_value>"
            ipv4_name: "<your_own_value> (source firewall.address.name firewall.addrgrp.name)"
            ipv4_netmask: "<your_own_value>"
            ipv4_split_exclude: "<your_own_value> (source firewall.address.name firewall.addrgrp.name)"
            ipv4_split_include: "<your_own_value> (source firewall.address.name firewall.addrgrp.name)"
            ipv4_start_ip: "<your_own_value>"
            ipv4_wins_server1: "<your_own_value>"
            ipv4_wins_server2: "<your_own_value>"
            ipv6_dns_server1: "<your_own_value>"
            ipv6_dns_server2: "<your_own_value>"
            ipv6_dns_server3: "<your_own_value>"
            ipv6_end_ip: "<your_own_value>"
            ipv6_exclude_range:
             -
                end_ip: "<your_own_value>"
                id:  "83"
                start_ip: "<your_own_value>"
            ipv6_name: "<your_own_value> (source firewall.address6.name firewall.addrgrp6.name)"
            ipv6_prefix: "86"
            ipv6_split_exclude: "<your_own_value> (source firewall.address6.name firewall.addrgrp6.name)"
            ipv6_split_include: "<your_own_value> (source firewall.address6.name firewall.addrgrp6.name)"
            ipv6_start_ip: "<your_own_value>"
            keepalive: "90"
            keylife: "91"
            local_gw: "<your_own_value>"
            local_gw6: "<your_own_value>"
            localid: "<your_own_value>"
            localid_type: "auto"
            mesh_selector_type: "disable"
            mode: "aggressive"
            mode_cfg: "disable"
            monitor: "<your_own_value> (source vpn.ipsec.phase1-interface.name)"
            monitor_hold_down_delay: "100"
            monitor_hold_down_time: "<your_own_value>"
            monitor_hold_down_type: "immediate"
            monitor_hold_down_weekday: "everyday"
            name: "default_name_104"
            nattraversal: "enable"
            negotiate_timeout: "106"
            net_device: "enable"
            passive_mode: "enable"
            peer: "<your_own_value> (source user.peer.name)"
            peergrp: "<your_own_value> (source user.peergrp.name)"
            peerid: "<your_own_value>"
            peertype: "any"
            ppk: "disable"
            ppk_identity: "<your_own_value>"
            ppk_secret: "<your_own_value>"
            priority: "116"
            proposal: "des-md5"
            psksecret: "<your_own_value>"
            psksecret_remote: "<your_own_value>"
            reauth: "disable"
            rekey: "enable"
            remote_gw: "<your_own_value>"
            remote_gw6: "<your_own_value>"
            remotegw_ddns: "<your_own_value>"
            rsa_signature_format: "pkcs1"
            save_password: "disable"
            send_cert_chain: "enable"
            signature_hash_alg: "sha1"
            split_include_service: "<your_own_value> (source firewall.service.group.name firewall.service.custom.name)"
            suite_b: "disable"
            tunnel_search: "selectors"
            type: "static"
            unity_support: "disable"
            usrgrp: "<your_own_value> (source user.group.name)"
            vni: "135"
            wizard_type: "custom"
            xauthtype: "disable"


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
