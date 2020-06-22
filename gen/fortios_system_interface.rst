:source: fortios_system_interface.py

:orphan:

.. fortios_system_interface:

fortios_system_interface -- Configure interfaces in Fortinet's FortiOS and FortiGate.
+++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++

.. versionadded:: 2.8

.. contents::
   :local:
   :depth: 1


Synopsis
--------
- This module is able to configure a FortiGate or FortiOS (FOS) device by allowing the user to set and modify system feature and interface category. Examples include all parameters and values need to be adjusted to datasources before usage. Tested with FOS v6.2.0



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
    <li> <span class="li-head">system_interface</span> - Configure interfaces. <span class="li-normal">type: dict</span></li>
        <ul class="ul-self">
        <li> <span class="li-head">state</span> - B(Deprecated) <span class="li-normal">type: str</span> <span class="li-required">required: False</span> <span class="li-normal">choices: present, absent</span></li>
        <li> <span class="li-head">ac_name</span> - PPPoE server name. <span class="li-normal">type: str</span></li>
        <li> <span class="li-head">aggregate</span> - Aggregate interface. <span class="li-normal">type: str</span></li>
        <li> <span class="li-head">algorithm</span> - Frame distribution algorithm. <span class="li-normal">type: str</span> <span class="li-normal">choices: L2, L3, L4</span></li>
        <li> <span class="li-head">alias</span> - Alias will be displayed with the interface name to make it easier to distinguish. <span class="li-normal">type: str</span></li>
        <li> <span class="li-head">allowaccess</span> - Permitted types of management access to this interface. <span class="li-normal">type: list</span> <span class="li-normal">choices: ping, https, ssh, snmp, http, telnet, fgfm, radius-acct, probe-response, capwap, ftm</span></li>
        <li> <span class="li-head">ap_discover</span> - Enable/disable automatic registration of unknown FortiAP devices. <span class="li-normal">type: str</span> <span class="li-normal">choices: enable, disable</span></li>
        <li> <span class="li-head">arpforward</span> - Enable/disable ARP forwarding. <span class="li-normal">type: str</span> <span class="li-normal">choices: enable, disable</span></li>
        <li> <span class="li-head">auth_type</span> - PPP authentication type to use. <span class="li-normal">type: str</span> <span class="li-normal">choices: auto, pap, chap, mschapv1, mschapv2</span></li>
        <li> <span class="li-head">auto_auth_extension_device</span> - Enable/disable automatic authorization of dedicated Fortinet extension device on this interface. <span class="li-normal">type: str</span> <span class="li-normal">choices: enable, disable</span></li>
        <li> <span class="li-head">bfd</span> - Bidirectional Forwarding Detection (BFD) settings. <span class="li-normal">type: str</span> <span class="li-normal">choices: global, enable, disable</span></li>
        <li> <span class="li-head">bfd_desired_min_tx</span> - BFD desired minimal transmit interval. <span class="li-normal">type: int</span></li>
        <li> <span class="li-head">bfd_detect_mult</span> - BFD detection multiplier. <span class="li-normal">type: int</span></li>
        <li> <span class="li-head">bfd_required_min_rx</span> - BFD required minimal receive interval. <span class="li-normal">type: int</span></li>
        <li> <span class="li-head">broadcast_forticlient_discovery</span> - Enable/disable broadcasting FortiClient discovery messages. <span class="li-normal">type: str</span> <span class="li-normal">choices: enable, disable</span></li>
        <li> <span class="li-head">broadcast_forward</span> - Enable/disable broadcast forwarding. <span class="li-normal">type: str</span> <span class="li-normal">choices: enable, disable</span></li>
        <li> <span class="li-head">captive_portal</span> - Enable/disable captive portal. <span class="li-normal">type: int</span></li>
        <li> <span class="li-head">cli_conn_status</span> - CLI connection status. <span class="li-normal">type: int</span></li>
        <li> <span class="li-head">color</span> - Color of icon on the GUI. <span class="li-normal">type: int</span></li>
        <li> <span class="li-head">dedicated_to</span> - Configure interface for single purpose. <span class="li-normal">type: str</span> <span class="li-normal">choices: none, management</span></li>
        <li> <span class="li-head">defaultgw</span> - Enable to get the gateway IP from the DHCP or PPPoE server. <span class="li-normal">type: str</span> <span class="li-normal">choices: enable, disable</span></li>
        <li> <span class="li-head">description</span> - Description. <span class="li-normal">type: str</span></li>
        <li> <span class="li-head">detected_peer_mtu</span> - MTU of detected peer (0 - 4294967295). <span class="li-normal">type: int</span></li>
        <li> <span class="li-head">detectprotocol</span> - Protocols used to detect the server. <span class="li-normal">type: str</span> <span class="li-normal">choices: ping, tcp-echo, udp-echo</span></li>
        <li> <span class="li-head">detectserver</span> - Gateway"s ping server for this IP. <span class="li-normal">type: str</span></li>
        <li> <span class="li-head">device_access_list</span> - Device access list. <span class="li-normal">type: str</span></li>
        <li> <span class="li-head">device_identification</span> - Enable/disable passively gathering of device identity information about the devices on the network connected to this interface. <span class="li-normal">type: str</span> <span class="li-normal">choices: enable, disable</span></li>
        <li> <span class="li-head">device_identification_active_scan</span> - Enable/disable active gathering of device identity information about the devices on the network connected to this interface. <span class="li-normal">type: str</span> <span class="li-normal">choices: enable, disable</span></li>
        <li> <span class="li-head">device_user_identification</span> - Enable/disable passive gathering of user identity information about users on this interface. <span class="li-normal">type: str</span> <span class="li-normal">choices: enable, disable</span></li>
        <li> <span class="li-head">devindex</span> - Device Index. <span class="li-normal">type: int</span></li>
        <li> <span class="li-head">dhcp_client_identifier</span> - DHCP client identifier. <span class="li-normal">type: str</span></li>
        <li> <span class="li-head">dhcp_relay_agent_option</span> - Enable/disable DHCP relay agent option. <span class="li-normal">type: str</span> <span class="li-normal">choices: enable, disable</span></li>
        <li> <span class="li-head">dhcp_relay_ip</span> - DHCP relay IP address. <span class="li-normal">type: str</span></li>
        <li> <span class="li-head">dhcp_relay_service</span> - Enable/disable allowing this interface to act as a DHCP relay. <span class="li-normal">type: str</span> <span class="li-normal">choices: disable, enable</span></li>
        <li> <span class="li-head">dhcp_relay_type</span> - DHCP relay type (regular or IPsec). <span class="li-normal">type: str</span> <span class="li-normal">choices: regular, ipsec</span></li>
        <li> <span class="li-head">dhcp_renew_time</span> - DHCP renew time in seconds (300-604800), 0 means use the renew time provided by the server. <span class="li-normal">type: int</span></li>
        <li> <span class="li-head">disc_retry_timeout</span> - Time in seconds to wait before retrying to start a PPPoE discovery, 0 means no timeout. <span class="li-normal">type: int</span></li>
        <li> <span class="li-head">disconnect_threshold</span> - Time in milliseconds to wait before sending a notification that this interface is down or disconnected. <span class="li-normal">type: int</span></li>
        <li> <span class="li-head">distance</span> - Distance for routes learned through PPPoE or DHCP, lower distance indicates preferred route. <span class="li-normal">type: int</span></li>
        <li> <span class="li-head">dns_server_override</span> - Enable/disable use DNS acquired by DHCP or PPPoE. <span class="li-normal">type: str</span> <span class="li-normal">choices: enable, disable</span></li>
        <li> <span class="li-head">drop_fragment</span> - Enable/disable drop fragment packets. <span class="li-normal">type: str</span> <span class="li-normal">choices: enable, disable</span></li>
        <li> <span class="li-head">drop_overlapped_fragment</span> - Enable/disable drop overlapped fragment packets. <span class="li-normal">type: str</span> <span class="li-normal">choices: enable, disable</span></li>
        <li> <span class="li-head">egress_shaping_profile</span> - Outgoing traffic shaping profile. Source firewall.shaping-profile.profile-name. <span class="li-normal">type: str</span></li>
        <li> <span class="li-head">estimated_downstream_bandwidth</span> - Estimated maximum downstream bandwidth (kbps). Used to estimate link utilization. <span class="li-normal">type: int</span></li>
        <li> <span class="li-head">estimated_upstream_bandwidth</span> - Estimated maximum upstream bandwidth (kbps). Used to estimate link utilization. <span class="li-normal">type: int</span></li>
        <li> <span class="li-head">explicit_ftp_proxy</span> - Enable/disable the explicit FTP proxy on this interface. <span class="li-normal">type: str</span> <span class="li-normal">choices: enable, disable</span></li>
        <li> <span class="li-head">explicit_web_proxy</span> - Enable/disable the explicit web proxy on this interface. <span class="li-normal">type: str</span> <span class="li-normal">choices: enable, disable</span></li>
        <li> <span class="li-head">external</span> - Enable/disable identifying the interface as an external interface (which usually means it"s connected to the Internet). <span class="li-normal">type: str</span> <span class="li-normal">choices: enable, disable</span></li>
        <li> <span class="li-head">fail_action_on_extender</span> - Action on extender when interface fail . <span class="li-normal">type: str</span> <span class="li-normal">choices: soft-restart, hard-restart, reboot</span></li>
        <li> <span class="li-head">fail_alert_interfaces</span> - Names of the FortiGate interfaces to which the link failure alert is sent. <span class="li-normal">type: list</span></li>
            <ul class="ul-self">
            <li> <span class="li-head">name</span> - Names of the non-virtual interface. Source system.interface.name. <span class="li-normal">type: str</span> <span class="li-required">required: True</span></li>
            </ul>
        <li> <span class="li-head">fail_alert_method</span> - Select link-failed-signal or link-down method to alert about a failed link. <span class="li-normal">type: str</span> <span class="li-normal">choices: link-failed-signal, link-down</span></li>
        <li> <span class="li-head">fail_detect</span> - Enable/disable fail detection features for this interface. <span class="li-normal">type: str</span> <span class="li-normal">choices: enable, disable</span></li>
        <li> <span class="li-head">fail_detect_option</span> - Options for detecting that this interface has failed. <span class="li-normal">type: str</span> <span class="li-normal">choices: detectserver, link-down</span></li>
        <li> <span class="li-head">fortiheartbeat</span> - Enable/disable FortiHeartBeat (FortiTelemetry on GUI). <span class="li-normal">type: str</span> <span class="li-normal">choices: enable, disable</span></li>
        <li> <span class="li-head">fortilink</span> - Enable FortiLink to dedicate this interface to manage other Fortinet devices. <span class="li-normal">type: str</span> <span class="li-normal">choices: enable, disable</span></li>
        <li> <span class="li-head">fortilink_backup_link</span> - fortilink split interface backup link. <span class="li-normal">type: int</span></li>
        <li> <span class="li-head">fortilink_split_interface</span> - Enable/disable FortiLink split interface to connect member link to different FortiSwitch in stack for uplink redundancy. <span class="li-normal">type: str</span> <span class="li-normal">choices: enable, disable</span></li>
        <li> <span class="li-head">fortilink_stacking</span> - Enable/disable FortiLink switch-stacking on this interface. <span class="li-normal">type: str</span> <span class="li-normal">choices: enable, disable</span></li>
        <li> <span class="li-head">forward_domain</span> - Transparent mode forward domain. <span class="li-normal">type: int</span></li>
        <li> <span class="li-head">gwdetect</span> - Enable/disable detect gateway alive for first. <span class="li-normal">type: str</span> <span class="li-normal">choices: enable, disable</span></li>
        <li> <span class="li-head">ha_priority</span> - HA election priority for the PING server. <span class="li-normal">type: int</span></li>
        <li> <span class="li-head">icmp_accept_redirect</span> - Enable/disable ICMP accept redirect. <span class="li-normal">type: str</span> <span class="li-normal">choices: enable, disable</span></li>
        <li> <span class="li-head">icmp_send_redirect</span> - Enable/disable ICMP send redirect. <span class="li-normal">type: str</span> <span class="li-normal">choices: enable, disable</span></li>
        <li> <span class="li-head">ident_accept</span> - Enable/disable authentication for this interface. <span class="li-normal">type: str</span> <span class="li-normal">choices: enable, disable</span></li>
        <li> <span class="li-head">idle_timeout</span> - PPPoE auto disconnect after idle timeout seconds, 0 means no timeout. <span class="li-normal">type: int</span></li>
        <li> <span class="li-head">inbandwidth</span> - Bandwidth limit for incoming traffic (0 - 16776000 kbps), 0 means unlimited. <span class="li-normal">type: int</span></li>
        <li> <span class="li-head">ingress_spillover_threshold</span> - Ingress Spillover threshold (0 - 16776000 kbps). <span class="li-normal">type: int</span></li>
        <li> <span class="li-head">interface</span> - Interface name. Source system.interface.name. <span class="li-normal">type: str</span></li>
        <li> <span class="li-head">internal</span> - Implicitly created. <span class="li-normal">type: int</span></li>
        <li> <span class="li-head">ip</span> - Interface IPv4 address and subnet mask, syntax: X.X.X.X/24. <span class="li-normal">type: str</span></li>
        <li> <span class="li-head">ipmac</span> - Enable/disable IP/MAC binding. <span class="li-normal">type: str</span> <span class="li-normal">choices: enable, disable</span></li>
        <li> <span class="li-head">ips_sniffer_mode</span> - Enable/disable the use of this interface as a one-armed sniffer. <span class="li-normal">type: str</span> <span class="li-normal">choices: enable, disable</span></li>
        <li> <span class="li-head">ipunnumbered</span> - Unnumbered IP used for PPPoE interfaces for which no unique local address is provided. <span class="li-normal">type: str</span></li>
        <li> <span class="li-head">ipv6</span> - IPv6 of interface. <span class="li-normal">type: dict</span></li>
            <ul class="ul-self">
            <li> <span class="li-head">autoconf</span> - Enable/disable address auto config. <span class="li-normal">type: str</span> <span class="li-normal">choices: enable, disable</span></li>
            <li> <span class="li-head">dhcp6_client_options</span> - DHCPv6 client options. <span class="li-normal">type: str</span> <span class="li-normal">choices: rapid, iapd, iana</span></li>
            <li> <span class="li-head">dhcp6_information_request</span> - Enable/disable DHCPv6 information request. <span class="li-normal">type: str</span> <span class="li-normal">choices: enable, disable</span></li>
            <li> <span class="li-head">dhcp6_prefix_delegation</span> - Enable/disable DHCPv6 prefix delegation. <span class="li-normal">type: str</span> <span class="li-normal">choices: enable, disable</span></li>
            <li> <span class="li-head">dhcp6_prefix_hint</span> - DHCPv6 prefix that will be used as a hint to the upstream DHCPv6 server. <span class="li-normal">type: str</span></li>
            <li> <span class="li-head">dhcp6_prefix_hint_plt</span> - DHCPv6 prefix hint preferred life time (sec), 0 means unlimited lease time. <span class="li-normal">type: int</span></li>
            <li> <span class="li-head">dhcp6_prefix_hint_vlt</span> - DHCPv6 prefix hint valid life time (sec). <span class="li-normal">type: int</span></li>
            <li> <span class="li-head">dhcp6_relay_ip</span> - DHCPv6 relay IP address. <span class="li-normal">type: str</span></li>
            <li> <span class="li-head">dhcp6_relay_service</span> - Enable/disable DHCPv6 relay. <span class="li-normal">type: str</span> <span class="li-normal">choices: disable, enable</span></li>
            <li> <span class="li-head">dhcp6_relay_type</span> - DHCPv6 relay type. <span class="li-normal">type: str</span> <span class="li-normal">choices: regular</span></li>
            <li> <span class="li-head">ip6_address</span> - Primary IPv6 address prefix, syntax: xxxx:xxxx:xxxx:xxxx:xxxx:xxxx:xxxx:xxxx/xxx <span class="li-normal">type: str</span></li>
            <li> <span class="li-head">ip6_allowaccess</span> - Allow management access to the interface. <span class="li-normal">type: list</span> <span class="li-normal">choices: ping, https, ssh, snmp, http, telnet, fgfm, capwap</span></li>
            <li> <span class="li-head">ip6_default_life</span> - Default life (sec). <span class="li-normal">type: int</span></li>
            <li> <span class="li-head">ip6_delegated_prefix_list</span> - Advertised IPv6 delegated prefix list. <span class="li-normal">type: list</span></li>
                <ul class="ul-self">
                <li> <span class="li-head">autonomous_flag</span> - Enable/disable the autonomous flag. <span class="li-normal">type: str</span> <span class="li-normal">choices: enable, disable</span></li>
                <li> <span class="li-head">onlink_flag</span> - Enable/disable the onlink flag. <span class="li-normal">type: str</span> <span class="li-normal">choices: enable, disable</span></li>
                <li> <span class="li-head">prefix_id</span> - Prefix ID. <span class="li-normal">type: int</span></li>
                <li> <span class="li-head">rdnss</span> - Recursive DNS server option. <span class="li-normal">type: str</span></li>
                <li> <span class="li-head">rdnss_service</span> - Recursive DNS service option. <span class="li-normal">type: str</span> <span class="li-normal">choices: delegated, default, specify</span></li>
                <li> <span class="li-head">subnet</span> - Add subnet ID to routing prefix. <span class="li-normal">type: str</span></li>
                <li> <span class="li-head">upstream_interface</span> - Name of the interface that provides delegated information. Source system.interface.name. <span class="li-normal">type: str</span></li>
                </ul>
            <li> <span class="li-head">ip6_dns_server_override</span> - Enable/disable using the DNS server acquired by DHCP. <span class="li-normal">type: str</span> <span class="li-normal">choices: enable, disable</span></li>
            <li> <span class="li-head">ip6_extra_addr</span> - Extra IPv6 address prefixes of interface. <span class="li-normal">type: list</span></li>
                <ul class="ul-self">
                <li> <span class="li-head">prefix</span> - IPv6 address prefix. <span class="li-normal">type: str</span> <span class="li-required">required: True</span></li>
                </ul>
            <li> <span class="li-head">ip6_hop_limit</span> - Hop limit (0 means unspecified). <span class="li-normal">type: int</span></li>
            <li> <span class="li-head">ip6_link_mtu</span> - IPv6 link MTU. <span class="li-normal">type: int</span></li>
            <li> <span class="li-head">ip6_manage_flag</span> - Enable/disable the managed flag. <span class="li-normal">type: str</span> <span class="li-normal">choices: enable, disable</span></li>
            <li> <span class="li-head">ip6_max_interval</span> - IPv6 maximum interval (4 to 1800 sec). <span class="li-normal">type: int</span></li>
            <li> <span class="li-head">ip6_min_interval</span> - IPv6 minimum interval (3 to 1350 sec). <span class="li-normal">type: int</span></li>
            <li> <span class="li-head">ip6_mode</span> - Addressing mode (static, DHCP, delegated). <span class="li-normal">type: str</span> <span class="li-normal">choices: static, dhcp, pppoe, delegated</span></li>
            <li> <span class="li-head">ip6_other_flag</span> - Enable/disable the other IPv6 flag. <span class="li-normal">type: str</span> <span class="li-normal">choices: enable, disable</span></li>
            <li> <span class="li-head">ip6_prefix_list</span> - Advertised prefix list. <span class="li-normal">type: list</span></li>
                <ul class="ul-self">
                <li> <span class="li-head">autonomous_flag</span> - Enable/disable the autonomous flag. <span class="li-normal">type: str</span> <span class="li-normal">choices: enable, disable</span></li>
                <li> <span class="li-head">dnssl</span> - DNS search list option. <span class="li-normal">type: list</span></li>
                    <ul class="ul-self">
                    <li> <span class="li-head">domain</span> - Domain name. <span class="li-normal">type: str</span> <span class="li-required">required: True</span></li>
                    </ul>
                <li> <span class="li-head">onlink_flag</span> - Enable/disable the onlink flag. <span class="li-normal">type: str</span> <span class="li-normal">choices: enable, disable</span></li>
                <li> <span class="li-head">preferred_life_time</span> - Preferred life time (sec). <span class="li-normal">type: int</span></li>
                <li> <span class="li-head">prefix</span> - IPv6 prefix. <span class="li-normal">type: str</span> <span class="li-required">required: True</span></li>
                <li> <span class="li-head">rdnss</span> - Recursive DNS server option. <span class="li-normal">type: str</span></li>
                <li> <span class="li-head">valid_life_time</span> - Valid life time (sec). <span class="li-normal">type: int</span></li>
                </ul>
            <li> <span class="li-head">ip6_reachable_time</span> - IPv6 reachable time (milliseconds; 0 means unspecified). <span class="li-normal">type: int</span></li>
            <li> <span class="li-head">ip6_retrans_time</span> - IPv6 retransmit time (milliseconds; 0 means unspecified). <span class="li-normal">type: int</span></li>
            <li> <span class="li-head">ip6_send_adv</span> - Enable/disable sending advertisements about the interface. <span class="li-normal">type: str</span> <span class="li-normal">choices: enable, disable</span></li>
            <li> <span class="li-head">ip6_subnet</span> -  Subnet to routing prefix, syntax: xxxx:xxxx:xxxx:xxxx:xxxx:xxxx:xxxx:xxxx/xxx <span class="li-normal">type: str</span></li>
            <li> <span class="li-head">ip6_upstream_interface</span> - Interface name providing delegated information. Source system.interface.name. <span class="li-normal">type: str</span></li>
            <li> <span class="li-head">nd_cert</span> - Neighbor discovery certificate. Source certificate.local.name. <span class="li-normal">type: str</span></li>
            <li> <span class="li-head">nd_cga_modifier</span> - Neighbor discovery CGA modifier. <span class="li-normal">type: str</span></li>
            <li> <span class="li-head">nd_mode</span> - Neighbor discovery mode. <span class="li-normal">type: str</span> <span class="li-normal">choices: basic, SEND-compatible</span></li>
            <li> <span class="li-head">nd_security_level</span> - Neighbor discovery security level (0 - 7; 0 = least secure). <span class="li-normal">type: int</span></li>
            <li> <span class="li-head">nd_timestamp_delta</span> - Neighbor discovery timestamp delta value (1 - 3600 sec; ). <span class="li-normal">type: int</span></li>
            <li> <span class="li-head">nd_timestamp_fuzz</span> - Neighbor discovery timestamp fuzz factor (1 - 60 sec; ). <span class="li-normal">type: int</span></li>
            <li> <span class="li-head">vrip6_link_local</span> - Link-local IPv6 address of virtual router. <span class="li-normal">type: str</span></li>
            <li> <span class="li-head">vrrp_virtual_mac6</span> - Enable/disable virtual MAC for VRRP. <span class="li-normal">type: str</span> <span class="li-normal">choices: enable, disable</span></li>
            <li> <span class="li-head">vrrp6</span> - IPv6 VRRP configuration. <span class="li-normal">type: list</span></li>
                <ul class="ul-self">
                <li> <span class="li-head">accept_mode</span> - Enable/disable accept mode. <span class="li-normal">type: str</span> <span class="li-normal">choices: enable, disable</span></li>
                <li> <span class="li-head">adv_interval</span> - Advertisement interval (1 - 255 seconds). <span class="li-normal">type: int</span></li>
                <li> <span class="li-head">preempt</span> - Enable/disable preempt mode. <span class="li-normal">type: str</span> <span class="li-normal">choices: enable, disable</span></li>
                <li> <span class="li-head">priority</span> - Priority of the virtual router (1 - 255). <span class="li-normal">type: int</span></li>
                <li> <span class="li-head">start_time</span> - Startup time (1 - 255 seconds). <span class="li-normal">type: int</span></li>
                <li> <span class="li-head">status</span> - Enable/disable VRRP. <span class="li-normal">type: str</span> <span class="li-normal">choices: enable, disable</span></li>
                <li> <span class="li-head">vrdst6</span> - Monitor the route to this destination. <span class="li-normal">type: str</span></li>
                <li> <span class="li-head">vrgrp</span> - VRRP group ID (1 - 65535). <span class="li-normal">type: int</span></li>
                <li> <span class="li-head">vrid</span> - Virtual router identifier (1 - 255). <span class="li-normal">type: int</span> <span class="li-required">required: True</span></li>
                <li> <span class="li-head">vrip6</span> - IPv6 address of the virtual router. <span class="li-normal">type: str</span></li>
                </ul>
            </ul>
        <li> <span class="li-head">l2forward</span> - Enable/disable l2 forwarding. <span class="li-normal">type: str</span> <span class="li-normal">choices: enable, disable</span></li>
        <li> <span class="li-head">lacp_ha_slave</span> - LACP HA slave. <span class="li-normal">type: str</span> <span class="li-normal">choices: enable, disable</span></li>
        <li> <span class="li-head">lacp_mode</span> - LACP mode. <span class="li-normal">type: str</span> <span class="li-normal">choices: static, passive, active</span></li>
        <li> <span class="li-head">lacp_speed</span> - How often the interface sends LACP messages. <span class="li-normal">type: str</span> <span class="li-normal">choices: slow, fast</span></li>
        <li> <span class="li-head">lcp_echo_interval</span> - Time in seconds between PPPoE Link Control Protocol (LCP) echo requests. <span class="li-normal">type: int</span></li>
        <li> <span class="li-head">lcp_max_echo_fails</span> - Maximum missed LCP echo messages before disconnect. <span class="li-normal">type: int</span></li>
        <li> <span class="li-head">link_up_delay</span> - Number of milliseconds to wait before considering a link is up. <span class="li-normal">type: int</span></li>
        <li> <span class="li-head">lldp_network_policy</span> - LLDP-MED network policy profile. Source system.lldp.network-policy.name. <span class="li-normal">type: str</span></li>
        <li> <span class="li-head">lldp_reception</span> - Enable/disable Link Layer Discovery Protocol (LLDP) reception. <span class="li-normal">type: str</span> <span class="li-normal">choices: enable, disable, vdom</span></li>
        <li> <span class="li-head">lldp_transmission</span> - Enable/disable Link Layer Discovery Protocol (LLDP) transmission. <span class="li-normal">type: str</span> <span class="li-normal">choices: enable, disable, vdom</span></li>
        <li> <span class="li-head">macaddr</span> - Change the interface"s MAC address. <span class="li-normal">type: str</span></li>
        <li> <span class="li-head">management_ip</span> - High Availability in-band management IP address of this interface. <span class="li-normal">type: str</span></li>
        <li> <span class="li-head">member</span> - Physical interfaces that belong to the aggregate or redundant interface. <span class="li-normal">type: list</span></li>
            <ul class="ul-self">
            <li> <span class="li-head">interface_name</span> - Physical interface name. Source system.interface.name. <span class="li-normal">type: str</span></li>
            </ul>
        <li> <span class="li-head">min_links</span> - Minimum number of aggregated ports that must be up. <span class="li-normal">type: int</span></li>
        <li> <span class="li-head">min_links_down</span> - Action to take when less than the configured minimum number of links are active. <span class="li-normal">type: str</span> <span class="li-normal">choices: operational, administrative</span></li>
        <li> <span class="li-head">mode</span> - Addressing mode (static, DHCP, PPPoE). <span class="li-normal">type: str</span> <span class="li-normal">choices: static, dhcp, pppoe</span></li>
        <li> <span class="li-head">mtu</span> - MTU value for this interface. <span class="li-normal">type: int</span></li>
        <li> <span class="li-head">mtu_override</span> - Enable to set a custom MTU for this interface. <span class="li-normal">type: str</span> <span class="li-normal">choices: enable, disable</span></li>
        <li> <span class="li-head">name</span> - Name. <span class="li-normal">type: str</span> <span class="li-required">required: True</span></li>
        <li> <span class="li-head">ndiscforward</span> - Enable/disable NDISC forwarding. <span class="li-normal">type: str</span> <span class="li-normal">choices: enable, disable</span></li>
        <li> <span class="li-head">netbios_forward</span> - Enable/disable NETBIOS forwarding. <span class="li-normal">type: str</span> <span class="li-normal">choices: disable, enable</span></li>
        <li> <span class="li-head">netflow_sampler</span> - Enable/disable NetFlow on this interface and set the data that NetFlow collects (rx, tx, or both). <span class="li-normal">type: str</span> <span class="li-normal">choices: disable, tx, rx, both</span></li>
        <li> <span class="li-head">outbandwidth</span> - Bandwidth limit for outgoing traffic (0 - 16776000 kbps). <span class="li-normal">type: int</span></li>
        <li> <span class="li-head">padt_retry_timeout</span> - PPPoE Active Discovery Terminate (PADT) used to terminate sessions after an idle time. <span class="li-normal">type: int</span></li>
        <li> <span class="li-head">password</span> - PPPoE account"s password. <span class="li-normal">type: str</span></li>
        <li> <span class="li-head">ping_serv_status</span> - PING server status. <span class="li-normal">type: int</span></li>
        <li> <span class="li-head">polling_interval</span> - sFlow polling interval (1 - 255 sec). <span class="li-normal">type: int</span></li>
        <li> <span class="li-head">pppoe_unnumbered_negotiate</span> - Enable/disable PPPoE unnumbered negotiation. <span class="li-normal">type: str</span> <span class="li-normal">choices: enable, disable</span></li>
        <li> <span class="li-head">pptp_auth_type</span> - PPTP authentication type. <span class="li-normal">type: str</span> <span class="li-normal">choices: auto, pap, chap, mschapv1, mschapv2</span></li>
        <li> <span class="li-head">pptp_client</span> - Enable/disable PPTP client. <span class="li-normal">type: str</span> <span class="li-normal">choices: enable, disable</span></li>
        <li> <span class="li-head">pptp_password</span> - PPTP password. <span class="li-normal">type: str</span></li>
        <li> <span class="li-head">pptp_server_ip</span> - PPTP server IP address. <span class="li-normal">type: str</span></li>
        <li> <span class="li-head">pptp_timeout</span> - Idle timer in minutes (0 for disabled). <span class="li-normal">type: int</span></li>
        <li> <span class="li-head">pptp_user</span> - PPTP user name. <span class="li-normal">type: str</span></li>
        <li> <span class="li-head">preserve_session_route</span> - Enable/disable preservation of session route when dirty. <span class="li-normal">type: str</span> <span class="li-normal">choices: enable, disable</span></li>
        <li> <span class="li-head">priority</span> - Priority of learned routes. <span class="li-normal">type: int</span></li>
        <li> <span class="li-head">priority_override</span> - Enable/disable fail back to higher priority port once recovered. <span class="li-normal">type: str</span> <span class="li-normal">choices: enable, disable</span></li>
        <li> <span class="li-head">proxy_captive_portal</span> - Enable/disable proxy captive portal on this interface. <span class="li-normal">type: str</span> <span class="li-normal">choices: enable, disable</span></li>
        <li> <span class="li-head">redundant_interface</span> - Redundant interface. <span class="li-normal">type: str</span></li>
        <li> <span class="li-head">remote_ip</span> - Remote IP address of tunnel. <span class="li-normal">type: str</span></li>
        <li> <span class="li-head">replacemsg_override_group</span> - Replacement message override group. <span class="li-normal">type: str</span></li>
        <li> <span class="li-head">role</span> - Interface role. <span class="li-normal">type: str</span> <span class="li-normal">choices: lan, wan, dmz, undefined</span></li>
        <li> <span class="li-head">sample_direction</span> - Data that NetFlow collects (rx, tx, or both). <span class="li-normal">type: str</span> <span class="li-normal">choices: tx, rx, both</span></li>
        <li> <span class="li-head">sample_rate</span> - sFlow sample rate (10 - 99999). <span class="li-normal">type: int</span></li>
        <li> <span class="li-head">secondary_IP</span> - Enable/disable adding a secondary IP to this interface. <span class="li-normal">type: str</span> <span class="li-normal">choices: enable, disable</span></li>
        <li> <span class="li-head">secondaryip</span> - Second IP address of interface. <span class="li-normal">type: list</span></li>
            <ul class="ul-self">
            <li> <span class="li-head">allowaccess</span> - Management access settings for the secondary IP address. <span class="li-normal">type: str</span> <span class="li-normal">choices: ping, https, ssh, snmp, http, telnet, fgfm, radius-acct, probe-response, capwap, ftm</span></li>
            <li> <span class="li-head">detectprotocol</span> - Protocols used to detect the server. <span class="li-normal">type: str</span> <span class="li-normal">choices: ping, tcp-echo, udp-echo</span></li>
            <li> <span class="li-head">detectserver</span> - Gateway"s ping server for this IP. <span class="li-normal">type: str</span></li>
            <li> <span class="li-head">gwdetect</span> - Enable/disable detect gateway alive for first. <span class="li-normal">type: str</span> <span class="li-normal">choices: enable, disable</span></li>
            <li> <span class="li-head">ha_priority</span> - HA election priority for the PING server. <span class="li-normal">type: int</span></li>
            <li> <span class="li-head">id</span> - ID. <span class="li-normal">type: int</span> <span class="li-required">required: True</span></li>
            <li> <span class="li-head">ip</span> - Secondary IP address of the interface. <span class="li-normal">type: str</span></li>
            <li> <span class="li-head">ping_serv_status</span> - PING server status. <span class="li-normal">type: int</span></li>
            </ul>
        <li> <span class="li-head">security_exempt_list</span> - Name of security-exempt-list. <span class="li-normal">type: str</span></li>
        <li> <span class="li-head">security_external_logout</span> - URL of external authentication logout server. <span class="li-normal">type: str</span></li>
        <li> <span class="li-head">security_external_web</span> - URL of external authentication web server. <span class="li-normal">type: str</span></li>
        <li> <span class="li-head">security_groups</span> - User groups that can authenticate with the captive portal. <span class="li-normal">type: list</span></li>
            <ul class="ul-self">
            <li> <span class="li-head">name</span> - Names of user groups that can authenticate with the captive portal. <span class="li-normal">type: str</span> <span class="li-required">required: True</span></li>
            </ul>
        <li> <span class="li-head">security_mac_auth_bypass</span> - Enable/disable MAC authentication bypass. <span class="li-normal">type: str</span> <span class="li-normal">choices: mac-auth-only, enable, disable</span></li>
        <li> <span class="li-head">security_mode</span> - Turn on captive portal authentication for this interface. <span class="li-normal">type: str</span> <span class="li-normal">choices: none, captive-portal, 802.1X</span></li>
        <li> <span class="li-head">security_redirect_url</span> - URL redirection after disclaimer/authentication. <span class="li-normal">type: str</span></li>
        <li> <span class="li-head">service_name</span> - PPPoE service name. <span class="li-normal">type: str</span></li>
        <li> <span class="li-head">sflow_sampler</span> - Enable/disable sFlow on this interface. <span class="li-normal">type: str</span> <span class="li-normal">choices: enable, disable</span></li>
        <li> <span class="li-head">snmp_index</span> - Permanent SNMP Index of the interface. <span class="li-normal">type: int</span></li>
        <li> <span class="li-head">speed</span> - Interface speed. The default setting and the options available depend on the interface hardware. <span class="li-normal">type: str</span> <span class="li-normal">choices: auto, 10full, 10half, 100full, 100half, 1000full, 1000half, 1000auto</span></li>
        <li> <span class="li-head">spillover_threshold</span> - Egress Spillover threshold (0 - 16776000 kbps), 0 means unlimited. <span class="li-normal">type: int</span></li>
        <li> <span class="li-head">src_check</span> - Enable/disable source IP check. <span class="li-normal">type: str</span> <span class="li-normal">choices: enable, disable</span></li>
        <li> <span class="li-head">status</span> - Bring the interface up or shut the interface down. <span class="li-normal">type: str</span> <span class="li-normal">choices: up, down</span></li>
        <li> <span class="li-head">stpforward</span> - Enable/disable STP forwarding. <span class="li-normal">type: str</span> <span class="li-normal">choices: enable, disable</span></li>
        <li> <span class="li-head">stpforward_mode</span> - Configure STP forwarding mode. <span class="li-normal">type: str</span> <span class="li-normal">choices: rpl-all-ext-id, rpl-bridge-ext-id, rpl-nothing</span></li>
        <li> <span class="li-head">subst</span> - Enable to always send packets from this interface to a destination MAC address. <span class="li-normal">type: str</span> <span class="li-normal">choices: enable, disable</span></li>
        <li> <span class="li-head">substitute_dst_mac</span> - Destination MAC address that all packets are sent to from this interface. <span class="li-normal">type: str</span></li>
        <li> <span class="li-head">switch</span> - Contained in switch. <span class="li-normal">type: str</span></li>
        <li> <span class="li-head">switch_controller_access_vlan</span> - Block FortiSwitch port-to-port traffic. <span class="li-normal">type: str</span> <span class="li-normal">choices: enable, disable</span></li>
        <li> <span class="li-head">switch_controller_arp_inspection</span> - Enable/disable FortiSwitch ARP inspection. <span class="li-normal">type: str</span> <span class="li-normal">choices: enable, disable</span></li>
        <li> <span class="li-head">switch_controller_dhcp_snooping</span> - Switch controller DHCP snooping. <span class="li-normal">type: str</span> <span class="li-normal">choices: enable, disable</span></li>
        <li> <span class="li-head">switch_controller_dhcp_snooping_option82</span> - Switch controller DHCP snooping option82. <span class="li-normal">type: str</span> <span class="li-normal">choices: enable, disable</span></li>
        <li> <span class="li-head">switch_controller_dhcp_snooping_verify_mac</span> - Switch controller DHCP snooping verify MAC. <span class="li-normal">type: str</span> <span class="li-normal">choices: enable, disable</span></li>
        <li> <span class="li-head">switch_controller_igmp_snooping</span> - Switch controller IGMP snooping. <span class="li-normal">type: str</span> <span class="li-normal">choices: enable, disable</span></li>
        <li> <span class="li-head">switch_controller_learning_limit</span> - Limit the number of dynamic MAC addresses on this VLAN (1 - 128, 0 = no limit, default). <span class="li-normal">type: int</span></li>
        <li> <span class="li-head">switch_controller_traffic_policy</span> - Switch controller traffic policy for the VLAN. Source switch-controller.traffic-policy.name. <span class="li-normal">type: str</span></li>
        <li> <span class="li-head">tagging</span> - Config object tagging. <span class="li-normal">type: list</span></li>
            <ul class="ul-self">
            <li> <span class="li-head">category</span> - Tag category. Source system.object-tagging.category. <span class="li-normal">type: str</span></li>
            <li> <span class="li-head">name</span> - Tagging entry name. <span class="li-normal">type: str</span> <span class="li-required">required: True</span></li>
            <li> <span class="li-head">tags</span> - Tags. <span class="li-normal">type: list</span></li>
                <ul class="ul-self">
                <li> <span class="li-head">name</span> - Tag name. Source system.object-tagging.tags.name. <span class="li-normal">type: str</span> <span class="li-required">required: True</span></li>
                </ul>
            </ul>
        <li> <span class="li-head">tcp_mss</span> - TCP maximum segment size. 0 means do not change segment size. <span class="li-normal">type: int</span></li>
        <li> <span class="li-head">trust_ip_1</span> - Trusted host for dedicated management traffic (0.0.0.0/24 for all hosts). <span class="li-normal">type: str</span></li>
        <li> <span class="li-head">trust_ip_2</span> - Trusted host for dedicated management traffic (0.0.0.0/24 for all hosts). <span class="li-normal">type: str</span></li>
        <li> <span class="li-head">trust_ip_3</span> - Trusted host for dedicated management traffic (0.0.0.0/24 for all hosts). <span class="li-normal">type: str</span></li>
        <li> <span class="li-head">trust_ip6_1</span> - Trusted IPv6 host for dedicated management traffic (::/0 for all hosts). <span class="li-normal">type: str</span></li>
        <li> <span class="li-head">trust_ip6_2</span> - Trusted IPv6 host for dedicated management traffic (::/0 for all hosts). <span class="li-normal">type: str</span></li>
        <li> <span class="li-head">trust_ip6_3</span> - Trusted IPv6 host for dedicated management traffic (::/0 for all hosts). <span class="li-normal">type: str</span></li>
        <li> <span class="li-head">type</span> - Interface type. <span class="li-normal">type: str</span> <span class="li-normal">choices: physical, vlan, aggregate, redundant, tunnel, vdom-link, loopback, switch, hard-switch, vap-switch, wl-mesh, fext-wan, vxlan, hdlc, switch-vlan</span></li>
        <li> <span class="li-head">username</span> - Username of the PPPoE account, provided by your ISP. <span class="li-normal">type: str</span></li>
        <li> <span class="li-head">vdom</span> - Interface is in this virtual domain (VDOM). Source system.vdom.name. <span class="li-normal">type: str</span></li>
        <li> <span class="li-head">vindex</span> - Switch control interface VLAN ID. <span class="li-normal">type: int</span></li>
        <li> <span class="li-head">vlanforward</span> - Enable/disable traffic forwarding between VLANs on this interface. <span class="li-normal">type: str</span> <span class="li-normal">choices: enable, disable</span></li>
        <li> <span class="li-head">vlanid</span> - VLAN ID (1 - 4094). <span class="li-normal">type: int</span></li>
        <li> <span class="li-head">vrf</span> - Virtual Routing Forwarding ID. <span class="li-normal">type: int</span></li>
        <li> <span class="li-head">vrrp</span> - VRRP configuration. <span class="li-normal">type: list</span></li>
            <ul class="ul-self">
            <li> <span class="li-head">accept_mode</span> - Enable/disable accept mode. <span class="li-normal">type: str</span> <span class="li-normal">choices: enable, disable</span></li>
            <li> <span class="li-head">adv_interval</span> - Advertisement interval (1 - 255 seconds). <span class="li-normal">type: int</span></li>
            <li> <span class="li-head">ignore_default_route</span> - Enable/disable ignoring of default route when checking destination. <span class="li-normal">type: str</span> <span class="li-normal">choices: enable, disable</span></li>
            <li> <span class="li-head">preempt</span> - Enable/disable preempt mode. <span class="li-normal">type: str</span> <span class="li-normal">choices: enable, disable</span></li>
            <li> <span class="li-head">priority</span> - Priority of the virtual router (1 - 255). <span class="li-normal">type: int</span></li>
            <li> <span class="li-head">proxy_arp</span> - VRRP Proxy ARP configuration. <span class="li-normal">type: list</span></li>
                <ul class="ul-self">
                <li> <span class="li-head">id</span> - ID. <span class="li-normal">type: int</span> <span class="li-required">required: True</span></li>
                <li> <span class="li-head">ip</span> - Set IP addresses of proxy ARP. <span class="li-normal">type: str</span></li>
                </ul>
            <li> <span class="li-head">start_time</span> - Startup time (1 - 255 seconds). <span class="li-normal">type: int</span></li>
            <li> <span class="li-head">status</span> - Enable/disable this VRRP configuration. <span class="li-normal">type: str</span> <span class="li-normal">choices: enable, disable</span></li>
            <li> <span class="li-head">version</span> - VRRP version. <span class="li-normal">type: str</span> <span class="li-normal">choices: 2, 3</span></li>
            <li> <span class="li-head">vrdst</span> - Monitor the route to this destination. <span class="li-normal">type: str</span></li>
            <li> <span class="li-head">vrdst_priority</span> - Priority of the virtual router when the virtual router destination becomes unreachable (0 - 254). <span class="li-normal">type: int</span></li>
            <li> <span class="li-head">vrgrp</span> - VRRP group ID (1 - 65535). <span class="li-normal">type: int</span></li>
            <li> <span class="li-head">vrid</span> - Virtual router identifier (1 - 255). <span class="li-normal">type: int</span> <span class="li-required">required: True</span></li>
            <li> <span class="li-head">vrip</span> - IP address of the virtual router. <span class="li-normal">type: str</span></li>
            </ul>
        <li> <span class="li-head">vrrp_virtual_mac</span> - Enable/disable use of virtual MAC for VRRP. <span class="li-normal">type: str</span> <span class="li-normal">choices: enable, disable</span></li>
        <li> <span class="li-head">wccp</span> - Enable/disable WCCP on this interface. Used for encapsulated WCCP communication between WCCP clients and servers. <span class="li-normal">type: str</span> <span class="li-normal">choices: enable, disable</span></li>
        <li> <span class="li-head">weight</span> - Default weight for static routes (if route has no weight configured). <span class="li-normal">type: int</span></li>
        <li> <span class="li-head">wins_ip</span> - WINS server IP. <span class="li-normal">type: str</span></li>
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
      - name: Configure interfaces.
        fortios_system_interface:
          vdom:  "{{ vdom }}"
          state: "present"
          system_interface:
            ac_name: "<your_own_value>"
            aggregate: "<your_own_value>"
            algorithm: "L2"
            alias: "<your_own_value>"
            allowaccess: "ping"
            ap_discover: "enable"
            arpforward: "enable"
            auth_type: "auto"
            auto_auth_extension_device: "enable"
            bfd: "global"
            bfd_desired_min_tx: "13"
            bfd_detect_mult: "14"
            bfd_required_min_rx: "15"
            broadcast_forticlient_discovery: "enable"
            broadcast_forward: "enable"
            captive_portal: "18"
            cli_conn_status: "19"
            color: "20"
            dedicated_to: "none"
            defaultgw: "enable"
            description: "<your_own_value>"
            detected_peer_mtu: "24"
            detectprotocol: "ping"
            detectserver: "<your_own_value>"
            device_access_list: "<your_own_value>"
            device_identification: "enable"
            device_identification_active_scan: "enable"
            device_user_identification: "enable"
            devindex: "31"
            dhcp_client_identifier:  "myId_32"
            dhcp_relay_agent_option: "enable"
            dhcp_relay_ip: "<your_own_value>"
            dhcp_relay_service: "disable"
            dhcp_relay_type: "regular"
            dhcp_renew_time: "37"
            disc_retry_timeout: "38"
            disconnect_threshold: "39"
            distance: "40"
            dns_server_override: "enable"
            drop_fragment: "enable"
            drop_overlapped_fragment: "enable"
            egress_shaping_profile: "<your_own_value> (source firewall.shaping-profile.profile-name)"
            estimated_downstream_bandwidth: "45"
            estimated_upstream_bandwidth: "46"
            explicit_ftp_proxy: "enable"
            explicit_web_proxy: "enable"
            external: "enable"
            fail_action_on_extender: "soft-restart"
            fail_alert_interfaces:
             -
                name: "default_name_52 (source system.interface.name)"
            fail_alert_method: "link-failed-signal"
            fail_detect: "enable"
            fail_detect_option: "detectserver"
            fortiheartbeat: "enable"
            fortilink: "enable"
            fortilink_backup_link: "58"
            fortilink_split_interface: "enable"
            fortilink_stacking: "enable"
            forward_domain: "61"
            gwdetect: "enable"
            ha_priority: "63"
            icmp_accept_redirect: "enable"
            icmp_send_redirect: "enable"
            ident_accept: "enable"
            idle_timeout: "67"
            inbandwidth: "68"
            ingress_spillover_threshold: "69"
            interface: "<your_own_value> (source system.interface.name)"
            internal: "71"
            ip: "<your_own_value>"
            ipmac: "enable"
            ips_sniffer_mode: "enable"
            ipunnumbered: "<your_own_value>"
            ipv6:
                autoconf: "enable"
                dhcp6_client_options: "rapid"
                dhcp6_information_request: "enable"
                dhcp6_prefix_delegation: "enable"
                dhcp6_prefix_hint: "<your_own_value>"
                dhcp6_prefix_hint_plt: "82"
                dhcp6_prefix_hint_vlt: "83"
                dhcp6_relay_ip: "<your_own_value>"
                dhcp6_relay_service: "disable"
                dhcp6_relay_type: "regular"
                ip6_address: "<your_own_value>"
                ip6_allowaccess: "ping"
                ip6_default_life: "89"
                ip6_delegated_prefix_list:
                 -
                    autonomous_flag: "enable"
                    onlink_flag: "enable"
                    prefix_id: "93"
                    rdnss: "<your_own_value>"
                    rdnss_service: "delegated"
                    subnet: "<your_own_value>"
                    upstream_interface: "<your_own_value> (source system.interface.name)"
                ip6_dns_server_override: "enable"
                ip6_extra_addr:
                 -
                    prefix: "<your_own_value>"
                ip6_hop_limit: "101"
                ip6_link_mtu: "102"
                ip6_manage_flag: "enable"
                ip6_max_interval: "104"
                ip6_min_interval: "105"
                ip6_mode: "static"
                ip6_other_flag: "enable"
                ip6_prefix_list:
                 -
                    autonomous_flag: "enable"
                    dnssl:
                     -
                        domain: "<your_own_value>"
                    onlink_flag: "enable"
                    preferred_life_time: "113"
                    prefix: "<your_own_value>"
                    rdnss: "<your_own_value>"
                    valid_life_time: "116"
                ip6_reachable_time: "117"
                ip6_retrans_time: "118"
                ip6_send_adv: "enable"
                ip6_subnet: "<your_own_value>"
                ip6_upstream_interface: "<your_own_value> (source system.interface.name)"
                nd_cert: "<your_own_value> (source certificate.local.name)"
                nd_cga_modifier: "<your_own_value>"
                nd_mode: "basic"
                nd_security_level: "125"
                nd_timestamp_delta: "126"
                nd_timestamp_fuzz: "127"
                vrip6_link_local: "<your_own_value>"
                vrrp_virtual_mac6: "enable"
                vrrp6:
                 -
                    accept_mode: "enable"
                    adv_interval: "132"
                    preempt: "enable"
                    priority: "134"
                    start_time: "135"
                    status: "enable"
                    vrdst6: "<your_own_value>"
                    vrgrp: "138"
                    vrid: "139"
                    vrip6: "<your_own_value>"
            l2forward: "enable"
            lacp_ha_slave: "enable"
            lacp_mode: "static"
            lacp_speed: "slow"
            lcp_echo_interval: "145"
            lcp_max_echo_fails: "146"
            link_up_delay: "147"
            lldp_network_policy: "<your_own_value> (source system.lldp.network-policy.name)"
            lldp_reception: "enable"
            lldp_transmission: "enable"
            macaddr: "<your_own_value>"
            management_ip: "<your_own_value>"
            member:
             -
                interface_name: "<your_own_value> (source system.interface.name)"
            min_links: "155"
            min_links_down: "operational"
            mode: "static"
            mtu: "158"
            mtu_override: "enable"
            name: "default_name_160"
            ndiscforward: "enable"
            netbios_forward: "disable"
            netflow_sampler: "disable"
            outbandwidth: "164"
            padt_retry_timeout: "165"
            password: "<your_own_value>"
            ping_serv_status: "167"
            polling_interval: "168"
            pppoe_unnumbered_negotiate: "enable"
            pptp_auth_type: "auto"
            pptp_client: "enable"
            pptp_password: "<your_own_value>"
            pptp_server_ip: "<your_own_value>"
            pptp_timeout: "174"
            pptp_user: "<your_own_value>"
            preserve_session_route: "enable"
            priority: "177"
            priority_override: "enable"
            proxy_captive_portal: "enable"
            redundant_interface: "<your_own_value>"
            remote_ip: "<your_own_value>"
            replacemsg_override_group: "<your_own_value>"
            role: "lan"
            sample_direction: "tx"
            sample_rate: "185"
            secondary_IP: "enable"
            secondaryip:
             -
                allowaccess: "ping"
                detectprotocol: "ping"
                detectserver: "<your_own_value>"
                gwdetect: "enable"
                ha_priority: "192"
                id:  "193"
                ip: "<your_own_value>"
                ping_serv_status: "195"
            security_exempt_list: "<your_own_value>"
            security_external_logout: "<your_own_value>"
            security_external_web: "<your_own_value>"
            security_groups:
             -
                name: "default_name_200"
            security_mac_auth_bypass: "mac-auth-only"
            security_mode: "none"
            security_redirect_url: "<your_own_value>"
            service_name: "<your_own_value>"
            sflow_sampler: "enable"
            snmp_index: "206"
            speed: "auto"
            spillover_threshold: "208"
            src_check: "enable"
            status: "up"
            stpforward: "enable"
            stpforward_mode: "rpl-all-ext-id"
            subst: "enable"
            substitute_dst_mac: "<your_own_value>"
            switch: "<your_own_value>"
            switch_controller_access_vlan: "enable"
            switch_controller_arp_inspection: "enable"
            switch_controller_dhcp_snooping: "enable"
            switch_controller_dhcp_snooping_option82: "enable"
            switch_controller_dhcp_snooping_verify_mac: "enable"
            switch_controller_igmp_snooping: "enable"
            switch_controller_learning_limit: "222"
            switch_controller_traffic_policy: "<your_own_value> (source switch-controller.traffic-policy.name)"
            tagging:
             -
                category: "<your_own_value> (source system.object-tagging.category)"
                name: "default_name_226"
                tags:
                 -
                    name: "default_name_228 (source system.object-tagging.tags.name)"
            tcp_mss: "229"
            trust_ip_1: "<your_own_value>"
            trust_ip_2: "<your_own_value>"
            trust_ip_3: "<your_own_value>"
            trust_ip6_1: "<your_own_value>"
            trust_ip6_2: "<your_own_value>"
            trust_ip6_3: "<your_own_value>"
            type: "physical"
            username: "<your_own_value>"
            vdom: "<your_own_value> (source system.vdom.name)"
            vindex: "239"
            vlanforward: "enable"
            vlanid: "241"
            vrf: "242"
            vrrp:
             -
                accept_mode: "enable"
                adv_interval: "245"
                ignore_default_route: "enable"
                preempt: "enable"
                priority: "248"
                proxy_arp:
                 -
                    id:  "250"
                    ip: "<your_own_value>"
                start_time: "252"
                status: "enable"
                version: "2"
                vrdst: "<your_own_value>"
                vrdst_priority: "256"
                vrgrp: "257"
                vrid: "258"
                vrip: "<your_own_value>"
            vrrp_virtual_mac: "enable"
            wccp: "enable"
            weight: "262"
            wins_ip: "<your_own_value>"


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
