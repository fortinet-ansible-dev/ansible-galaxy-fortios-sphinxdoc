:source: fortios_system_settings.py

:orphan:

.. fortios_system_settings:

fortios_system_settings -- Configure VDOM settings in Fortinet's FortiOS and FortiGate.
+++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++

.. versionadded:: 2.8

.. contents::
   :local:
   :depth: 1


Synopsis
--------
- This module is able to configure a FortiGate or FortiOS (FOS) device by allowing the user to set and modify system feature and settings category. Examples include all parameters and values need to be adjusted to datasources before usage. Tested with FOS v6.2.0



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
    <li> <span class="li-head">system_settings</span> - Configure VDOM settings. <span class="li-normal">type: dict</span></li>
        <ul class="ul-self">
        <li> <span class="li-head">allow_linkdown_path</span> - Enable/disable link down path. <span class="li-normal">type: str</span> <span class="li-normal">choices: enable, disable</span></li>
        <li> <span class="li-head">allow_subnet_overlap</span> - Enable/disable allowing interface subnets to use overlapping IP addresses. <span class="li-normal">type: str</span> <span class="li-normal">choices: enable, disable</span></li>
        <li> <span class="li-head">asymroute</span> - Enable/disable IPv4 asymmetric routing. <span class="li-normal">type: str</span> <span class="li-normal">choices: enable, disable</span></li>
        <li> <span class="li-head">asymroute_icmp</span> - Enable/disable ICMP asymmetric routing. <span class="li-normal">type: str</span> <span class="li-normal">choices: enable, disable</span></li>
        <li> <span class="li-head">asymroute6</span> - Enable/disable asymmetric IPv6 routing. <span class="li-normal">type: str</span> <span class="li-normal">choices: enable, disable</span></li>
        <li> <span class="li-head">asymroute6_icmp</span> - Enable/disable asymmetric ICMPv6 routing. <span class="li-normal">type: str</span> <span class="li-normal">choices: enable, disable</span></li>
        <li> <span class="li-head">bfd</span> - Enable/disable Bi-directional Forwarding Detection (BFD) on all interfaces. <span class="li-normal">type: str</span> <span class="li-normal">choices: enable, disable</span></li>
        <li> <span class="li-head">bfd_desired_min_tx</span> - BFD desired minimal transmit interval (1 - 100000 ms). <span class="li-normal">type: int</span></li>
        <li> <span class="li-head">bfd_detect_mult</span> - BFD detection multiplier (1 - 50). <span class="li-normal">type: int</span></li>
        <li> <span class="li-head">bfd_dont_enforce_src_port</span> - Enable to not enforce verifying the source port of BFD Packets. <span class="li-normal">type: str</span> <span class="li-normal">choices: enable, disable</span></li>
        <li> <span class="li-head">bfd_required_min_rx</span> - BFD required minimal receive interval (1 - 100000 ms). <span class="li-normal">type: int</span></li>
        <li> <span class="li-head">block_land_attack</span> - Enable/disable blocking of land attacks. <span class="li-normal">type: str</span> <span class="li-normal">choices: disable, enable</span></li>
        <li> <span class="li-head">central_nat</span> - Enable/disable central NAT. <span class="li-normal">type: str</span> <span class="li-normal">choices: enable, disable</span></li>
        <li> <span class="li-head">comments</span> - VDOM comments. <span class="li-normal">type: str</span></li>
        <li> <span class="li-head">compliance_check</span> - Enable/disable PCI DSS compliance checking. <span class="li-normal">type: str</span> <span class="li-normal">choices: enable, disable</span></li>
        <li> <span class="li-head">consolidated_firewall_mode</span> - Consolidated firewall mode. <span class="li-normal">type: str</span> <span class="li-normal">choices: enable, disable</span></li>
        <li> <span class="li-head">default_voip_alg_mode</span> - Configure how the FortiGate handles VoIP traffic when a policy that accepts the traffic doesn"t include a VoIP profile. <span class="li-normal">type: str</span> <span class="li-normal">choices: proxy-based, kernel-helper-based</span></li>
        <li> <span class="li-head">deny_tcp_with_icmp</span> - Enable/disable denying TCP by sending an ICMP communication prohibited packet. <span class="li-normal">type: str</span> <span class="li-normal">choices: enable, disable</span></li>
        <li> <span class="li-head">device</span> - Interface to use for management access for NAT mode. Source system.interface.name. <span class="li-normal">type: str</span></li>
        <li> <span class="li-head">dhcp_proxy</span> - Enable/disable the DHCP Proxy. <span class="li-normal">type: str</span> <span class="li-normal">choices: enable, disable</span></li>
        <li> <span class="li-head">dhcp_server_ip</span> - DHCP Server IPv4 address. <span class="li-normal">type: str</span></li>
        <li> <span class="li-head">dhcp6_server_ip</span> - DHCPv6 server IPv6 address. <span class="li-normal">type: str</span></li>
        <li> <span class="li-head">discovered_device_timeout</span> - Timeout for discovered devices (1 - 365 days). <span class="li-normal">type: int</span></li>
        <li> <span class="li-head">ecmp_max_paths</span> - Maximum number of Equal Cost Multi-Path (ECMP) next-hops. Set to 1 to disable ECMP routing (1 - 100). <span class="li-normal">type: int</span></li>
        <li> <span class="li-head">email_portal_check_dns</span> - Enable/disable using DNS to validate email addresses collected by a captive portal. <span class="li-normal">type: str</span> <span class="li-normal">choices: disable, enable</span></li>
        <li> <span class="li-head">firewall_session_dirty</span> - Select how to manage sessions affected by firewall policy configuration changes. <span class="li-normal">type: str</span> <span class="li-normal">choices: check-all, check-new, check-policy-option</span></li>
        <li> <span class="li-head">fw_session_hairpin</span> - Enable/disable checking for a matching policy each time hairpin traffic goes through the FortiGate. <span class="li-normal">type: str</span> <span class="li-normal">choices: enable, disable</span></li>
        <li> <span class="li-head">gateway</span> - Transparent mode IPv4 default gateway IP address. <span class="li-normal">type: str</span></li>
        <li> <span class="li-head">gateway6</span> - Transparent mode IPv4 default gateway IP address. <span class="li-normal">type: str</span></li>
        <li> <span class="li-head">gui_advanced_policy</span> - Enable/disable advanced policy configuration on the GUI. <span class="li-normal">type: str</span> <span class="li-normal">choices: enable, disable</span></li>
        <li> <span class="li-head">gui_allow_unnamed_policy</span> - Enable/disable the requirement for policy naming on the GUI. <span class="li-normal">type: str</span> <span class="li-normal">choices: enable, disable</span></li>
        <li> <span class="li-head">gui_antivirus</span> - Enable/disable AntiVirus on the GUI. <span class="li-normal">type: str</span> <span class="li-normal">choices: enable, disable</span></li>
        <li> <span class="li-head">gui_ap_profile</span> - Enable/disable FortiAP profiles on the GUI. <span class="li-normal">type: str</span> <span class="li-normal">choices: enable, disable</span></li>
        <li> <span class="li-head">gui_application_control</span> - Enable/disable application control on the GUI. <span class="li-normal">type: str</span> <span class="li-normal">choices: enable, disable</span></li>
        <li> <span class="li-head">gui_default_policy_columns</span> - Default columns to display for policy lists on GUI. <span class="li-normal">type: list</span></li>
            <ul class="ul-self">
            <li> <span class="li-head">name</span> - Select column name. <span class="li-normal">type: str</span> <span class="li-required">required: True</span></li>
            </ul>
        <li> <span class="li-head">gui_dhcp_advanced</span> - Enable/disable advanced DHCP options on the GUI. <span class="li-normal">type: str</span> <span class="li-normal">choices: enable, disable</span></li>
        <li> <span class="li-head">gui_dlp</span> - Enable/disable DLP on the GUI. <span class="li-normal">type: str</span> <span class="li-normal">choices: enable, disable</span></li>
        <li> <span class="li-head">gui_dns_database</span> - Enable/disable DNS database settings on the GUI. <span class="li-normal">type: str</span> <span class="li-normal">choices: enable, disable</span></li>
        <li> <span class="li-head">gui_dnsfilter</span> - Enable/disable DNS Filtering on the GUI. <span class="li-normal">type: str</span> <span class="li-normal">choices: enable, disable</span></li>
        <li> <span class="li-head">gui_domain_ip_reputation</span> - Enable/disable Domain and IP Reputation on the GUI. <span class="li-normal">type: str</span> <span class="li-normal">choices: enable, disable</span></li>
        <li> <span class="li-head">gui_dos_policy</span> - Enable/disable DoS policies on the GUI. <span class="li-normal">type: str</span> <span class="li-normal">choices: enable, disable</span></li>
        <li> <span class="li-head">gui_dynamic_profile_display</span> - Enable/disable RADIUS Single Sign On (RSSO) on the GUI. <span class="li-normal">type: str</span> <span class="li-normal">choices: enable, disable</span></li>
        <li> <span class="li-head">gui_dynamic_routing</span> - Enable/disable dynamic routing on the GUI. <span class="li-normal">type: str</span> <span class="li-normal">choices: enable, disable</span></li>
        <li> <span class="li-head">gui_email_collection</span> - Enable/disable email collection on the GUI. <span class="li-normal">type: str</span> <span class="li-normal">choices: enable, disable</span></li>
        <li> <span class="li-head">gui_endpoint_control</span> - Enable/disable endpoint control on the GUI. <span class="li-normal">type: str</span> <span class="li-normal">choices: enable, disable</span></li>
        <li> <span class="li-head">gui_endpoint_control_advanced</span> - Enable/disable advanced endpoint control options on the GUI. <span class="li-normal">type: str</span> <span class="li-normal">choices: enable, disable</span></li>
        <li> <span class="li-head">gui_explicit_proxy</span> - Enable/disable the explicit proxy on the GUI. <span class="li-normal">type: str</span> <span class="li-normal">choices: enable, disable</span></li>
        <li> <span class="li-head">gui_fortiap_split_tunneling</span> - Enable/disable FortiAP split tunneling on the GUI. <span class="li-normal">type: str</span> <span class="li-normal">choices: enable, disable</span></li>
        <li> <span class="li-head">gui_fortiextender_controller</span> - Enable/disable FortiExtender on the GUI. <span class="li-normal">type: str</span> <span class="li-normal">choices: enable, disable</span></li>
        <li> <span class="li-head">gui_icap</span> - Enable/disable ICAP on the GUI. <span class="li-normal">type: str</span> <span class="li-normal">choices: enable, disable</span></li>
        <li> <span class="li-head">gui_implicit_policy</span> - Enable/disable implicit firewall policies on the GUI. <span class="li-normal">type: str</span> <span class="li-normal">choices: enable, disable</span></li>
        <li> <span class="li-head">gui_ips</span> - Enable/disable IPS on the GUI. <span class="li-normal">type: str</span> <span class="li-normal">choices: enable, disable</span></li>
        <li> <span class="li-head">gui_load_balance</span> - Enable/disable server load balancing on the GUI. <span class="li-normal">type: str</span> <span class="li-normal">choices: enable, disable</span></li>
        <li> <span class="li-head">gui_local_in_policy</span> - Enable/disable Local-In policies on the GUI. <span class="li-normal">type: str</span> <span class="li-normal">choices: enable, disable</span></li>
        <li> <span class="li-head">gui_local_reports</span> - Enable/disable local reports on the GUI. <span class="li-normal">type: str</span> <span class="li-normal">choices: enable, disable</span></li>
        <li> <span class="li-head">gui_multicast_policy</span> - Enable/disable multicast firewall policies on the GUI. <span class="li-normal">type: str</span> <span class="li-normal">choices: enable, disable</span></li>
        <li> <span class="li-head">gui_multiple_interface_policy</span> - Enable/disable adding multiple interfaces to a policy on the GUI. <span class="li-normal">type: str</span> <span class="li-normal">choices: enable, disable</span></li>
        <li> <span class="li-head">gui_multiple_utm_profiles</span> - Enable/disable multiple UTM profiles on the GUI. <span class="li-normal">type: str</span> <span class="li-normal">choices: enable, disable</span></li>
        <li> <span class="li-head">gui_nat46_64</span> - Enable/disable NAT46 and NAT64 settings on the GUI. <span class="li-normal">type: str</span> <span class="li-normal">choices: enable, disable</span></li>
        <li> <span class="li-head">gui_object_colors</span> - Enable/disable object colors on the GUI. <span class="li-normal">type: str</span> <span class="li-normal">choices: enable, disable</span></li>
        <li> <span class="li-head">gui_policy_based_ipsec</span> - Enable/disable policy-based IPsec VPN on the GUI. <span class="li-normal">type: str</span> <span class="li-normal">choices: enable, disable</span></li>
        <li> <span class="li-head">gui_replacement_message_groups</span> - Enable/disable replacement message groups on the GUI. <span class="li-normal">type: str</span> <span class="li-normal">choices: enable, disable</span></li>
        <li> <span class="li-head">gui_spamfilter</span> - Enable/disable Antispam on the GUI. <span class="li-normal">type: str</span> <span class="li-normal">choices: enable, disable</span></li>
        <li> <span class="li-head">gui_sslvpn_personal_bookmarks</span> - Enable/disable SSL-VPN personal bookmark management on the GUI. <span class="li-normal">type: str</span> <span class="li-normal">choices: enable, disable</span></li>
        <li> <span class="li-head">gui_sslvpn_realms</span> - Enable/disable SSL-VPN realms on the GUI. <span class="li-normal">type: str</span> <span class="li-normal">choices: enable, disable</span></li>
        <li> <span class="li-head">gui_switch_controller</span> - Enable/disable the switch controller on the GUI. <span class="li-normal">type: str</span> <span class="li-normal">choices: enable, disable</span></li>
        <li> <span class="li-head">gui_threat_weight</span> - Enable/disable threat weight on the GUI. <span class="li-normal">type: str</span> <span class="li-normal">choices: enable, disable</span></li>
        <li> <span class="li-head">gui_traffic_shaping</span> - Enable/disable traffic shaping on the GUI. <span class="li-normal">type: str</span> <span class="li-normal">choices: enable, disable</span></li>
        <li> <span class="li-head">gui_voip_profile</span> - Enable/disable VoIP profiles on the GUI. <span class="li-normal">type: str</span> <span class="li-normal">choices: enable, disable</span></li>
        <li> <span class="li-head">gui_vpn</span> - Enable/disable VPN tunnels on the GUI. <span class="li-normal">type: str</span> <span class="li-normal">choices: enable, disable</span></li>
        <li> <span class="li-head">gui_waf_profile</span> - Enable/disable Web Application Firewall on the GUI. <span class="li-normal">type: str</span> <span class="li-normal">choices: enable, disable</span></li>
        <li> <span class="li-head">gui_wan_load_balancing</span> - Enable/disable SD-WAN on the GUI. <span class="li-normal">type: str</span> <span class="li-normal">choices: enable, disable</span></li>
        <li> <span class="li-head">gui_wanopt_cache</span> - Enable/disable WAN Optimization and Web Caching on the GUI. <span class="li-normal">type: str</span> <span class="li-normal">choices: enable, disable</span></li>
        <li> <span class="li-head">gui_webfilter</span> - Enable/disable Web filtering on the GUI. <span class="li-normal">type: str</span> <span class="li-normal">choices: enable, disable</span></li>
        <li> <span class="li-head">gui_webfilter_advanced</span> - Enable/disable advanced web filtering on the GUI. <span class="li-normal">type: str</span> <span class="li-normal">choices: enable, disable</span></li>
        <li> <span class="li-head">gui_wireless_controller</span> - Enable/disable the wireless controller on the GUI. <span class="li-normal">type: str</span> <span class="li-normal">choices: enable, disable</span></li>
        <li> <span class="li-head">http_external_dest</span> - Offload HTTP traffic to FortiWeb or FortiCache. <span class="li-normal">type: str</span> <span class="li-normal">choices: fortiweb, forticache</span></li>
        <li> <span class="li-head">ike_dn_format</span> - Configure IKE ASN.1 Distinguished Name format conventions. <span class="li-normal">type: str</span> <span class="li-normal">choices: with-space, no-space</span></li>
        <li> <span class="li-head">ike_quick_crash_detect</span> - Enable/disable IKE quick crash detection (RFC 6290). <span class="li-normal">type: str</span> <span class="li-normal">choices: enable, disable</span></li>
        <li> <span class="li-head">ike_session_resume</span> - Enable/disable IKEv2 session resumption (RFC 5723). <span class="li-normal">type: str</span> <span class="li-normal">choices: enable, disable</span></li>
        <li> <span class="li-head">implicit_allow_dns</span> - Enable/disable implicitly allowing DNS traffic. <span class="li-normal">type: str</span> <span class="li-normal">choices: enable, disable</span></li>
        <li> <span class="li-head">ip</span> - IP address and netmask. <span class="li-normal">type: str</span></li>
        <li> <span class="li-head">ip6</span> - IPv6 address prefix for NAT mode. <span class="li-normal">type: str</span></li>
        <li> <span class="li-head">link_down_access</span> - Enable/disable link down access traffic. <span class="li-normal">type: str</span> <span class="li-normal">choices: enable, disable</span></li>
        <li> <span class="li-head">lldp_reception</span> - Enable/disable Link Layer Discovery Protocol (LLDP) reception for this VDOM or apply global settings to this VDOM. <span class="li-normal">type: str</span> <span class="li-normal">choices: enable, disable, global</span></li>
        <li> <span class="li-head">lldp_transmission</span> - Enable/disable Link Layer Discovery Protocol (LLDP) transmission for this VDOM or apply global settings to this VDOM. <span class="li-normal">type: str</span> <span class="li-normal">choices: enable, disable, global</span></li>
        <li> <span class="li-head">mac_ttl</span> - Duration of MAC addresses in Transparent mode (300 - 8640000 sec). <span class="li-normal">type: int</span></li>
        <li> <span class="li-head">manageip</span> - Transparent mode IPv4 management IP address and netmask. <span class="li-normal">type: str</span></li>
        <li> <span class="li-head">manageip6</span> - Transparent mode IPv6 management IP address and netmask. <span class="li-normal">type: str</span></li>
        <li> <span class="li-head">multicast_forward</span> - Enable/disable multicast forwarding. <span class="li-normal">type: str</span> <span class="li-normal">choices: enable, disable</span></li>
        <li> <span class="li-head">multicast_skip_policy</span> - Enable/disable allowing multicast traffic through the FortiGate without a policy check. <span class="li-normal">type: str</span> <span class="li-normal">choices: enable, disable</span></li>
        <li> <span class="li-head">multicast_ttl_notchange</span> - Enable/disable preventing the FortiGate from changing the TTL for forwarded multicast packets. <span class="li-normal">type: str</span> <span class="li-normal">choices: enable, disable</span></li>
        <li> <span class="li-head">ngfw_mode</span> - Next Generation Firewall (NGFW) mode. <span class="li-normal">type: str</span> <span class="li-normal">choices: profile-based, policy-based</span></li>
        <li> <span class="li-head">opmode</span> - Firewall operation mode (NAT or Transparent). <span class="li-normal">type: str</span> <span class="li-normal">choices: nat, transparent</span></li>
        <li> <span class="li-head">prp_trailer_action</span> - Enable/disable action to take on PRP trailer. <span class="li-normal">type: str</span> <span class="li-normal">choices: enable, disable</span></li>
        <li> <span class="li-head">sccp_port</span> - TCP port the SCCP proxy monitors for SCCP traffic (0 - 65535). <span class="li-normal">type: int</span></li>
        <li> <span class="li-head">sctp_session_without_init</span> - Enable/disable SCTP session creation without SCTP INIT. <span class="li-normal">type: str</span> <span class="li-normal">choices: enable, disable</span></li>
        <li> <span class="li-head">ses_denied_traffic</span> - Enable/disable including denied session in the session table. <span class="li-normal">type: str</span> <span class="li-normal">choices: enable, disable</span></li>
        <li> <span class="li-head">sip_helper</span> - Enable/disable the SIP session helper to process SIP sessions unless SIP sessions are accepted by the SIP application layer gateway (ALG). <span class="li-normal">type: str</span> <span class="li-normal">choices: enable, disable</span></li>
        <li> <span class="li-head">sip_nat_trace</span> - Enable/disable recording the original SIP source IP address when NAT is used. <span class="li-normal">type: str</span> <span class="li-normal">choices: enable, disable</span></li>
        <li> <span class="li-head">sip_ssl_port</span> - TCP port the SIP proxy monitors for SIP SSL/TLS traffic (0 - 65535). <span class="li-normal">type: int</span></li>
        <li> <span class="li-head">sip_tcp_port</span> - TCP port the SIP proxy monitors for SIP traffic (0 - 65535). <span class="li-normal">type: int</span></li>
        <li> <span class="li-head">sip_udp_port</span> - UDP port the SIP proxy monitors for SIP traffic (0 - 65535). <span class="li-normal">type: int</span></li>
        <li> <span class="li-head">snat_hairpin_traffic</span> - Enable/disable source NAT (SNAT) for hairpin traffic. <span class="li-normal">type: str</span> <span class="li-normal">choices: enable, disable</span></li>
        <li> <span class="li-head">ssl_ssh_profile</span> - Profile for SSL/SSH inspection. Source firewall.ssl-ssh-profile.name. <span class="li-normal">type: str</span></li>
        <li> <span class="li-head">status</span> - Enable/disable this VDOM. <span class="li-normal">type: str</span> <span class="li-normal">choices: enable, disable</span></li>
        <li> <span class="li-head">strict_src_check</span> - Enable/disable strict source verification. <span class="li-normal">type: str</span> <span class="li-normal">choices: enable, disable</span></li>
        <li> <span class="li-head">tcp_session_without_syn</span> - Enable/disable allowing TCP session without SYN flags. <span class="li-normal">type: str</span> <span class="li-normal">choices: enable, disable</span></li>
        <li> <span class="li-head">utf8_spam_tagging</span> - Enable/disable converting antispam tags to UTF-8 for better non-ASCII character support. <span class="li-normal">type: str</span> <span class="li-normal">choices: enable, disable</span></li>
        <li> <span class="li-head">v4_ecmp_mode</span> - IPv4 Equal-cost multi-path (ECMP) routing and load balancing mode. <span class="li-normal">type: str</span> <span class="li-normal">choices: source-ip-based, weight-based, usage-based, source-dest-ip-based</span></li>
        <li> <span class="li-head">vpn_stats_log</span> - Enable/disable periodic VPN log statistics for one or more types of VPN. Separate names with a space. <span class="li-normal">type: str</span> <span class="li-normal">choices: ipsec, pptp, l2tp, ssl</span></li>
        <li> <span class="li-head">vpn_stats_period</span> - Period to send VPN log statistics (0 or 60 - 86400 sec). <span class="li-normal">type: int</span></li>
        <li> <span class="li-head">wccp_cache_engine</span> - Enable/disable WCCP cache engine. <span class="li-normal">type: str</span> <span class="li-normal">choices: enable, disable</span></li>
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
      - name: Configure VDOM settings.
        fortios_system_settings:
          vdom:  "{{ vdom }}"
          system_settings:
            allow_linkdown_path: "enable"
            allow_subnet_overlap: "enable"
            asymroute: "enable"
            asymroute_icmp: "enable"
            asymroute6: "enable"
            asymroute6_icmp: "enable"
            bfd: "enable"
            bfd_desired_min_tx: "10"
            bfd_detect_mult: "11"
            bfd_dont_enforce_src_port: "enable"
            bfd_required_min_rx: "13"
            block_land_attack: "disable"
            central_nat: "enable"
            comments: "<your_own_value>"
            compliance_check: "enable"
            consolidated_firewall_mode: "enable"
            default_voip_alg_mode: "proxy-based"
            deny_tcp_with_icmp: "enable"
            device: "<your_own_value> (source system.interface.name)"
            dhcp_proxy: "enable"
            dhcp_server_ip: "<your_own_value>"
            dhcp6_server_ip: "<your_own_value>"
            discovered_device_timeout: "25"
            ecmp_max_paths: "26"
            email_portal_check_dns: "disable"
            firewall_session_dirty: "check-all"
            fw_session_hairpin: "enable"
            gateway: "<your_own_value>"
            gateway6: "<your_own_value>"
            gui_advanced_policy: "enable"
            gui_allow_unnamed_policy: "enable"
            gui_antivirus: "enable"
            gui_ap_profile: "enable"
            gui_application_control: "enable"
            gui_default_policy_columns:
             -
                name: "default_name_38"
            gui_dhcp_advanced: "enable"
            gui_dlp: "enable"
            gui_dns_database: "enable"
            gui_dnsfilter: "enable"
            gui_domain_ip_reputation: "enable"
            gui_dos_policy: "enable"
            gui_dynamic_profile_display: "enable"
            gui_dynamic_routing: "enable"
            gui_email_collection: "enable"
            gui_endpoint_control: "enable"
            gui_endpoint_control_advanced: "enable"
            gui_explicit_proxy: "enable"
            gui_fortiap_split_tunneling: "enable"
            gui_fortiextender_controller: "enable"
            gui_icap: "enable"
            gui_implicit_policy: "enable"
            gui_ips: "enable"
            gui_load_balance: "enable"
            gui_local_in_policy: "enable"
            gui_local_reports: "enable"
            gui_multicast_policy: "enable"
            gui_multiple_interface_policy: "enable"
            gui_multiple_utm_profiles: "enable"
            gui_nat46_64: "enable"
            gui_object_colors: "enable"
            gui_policy_based_ipsec: "enable"
            gui_replacement_message_groups: "enable"
            gui_spamfilter: "enable"
            gui_sslvpn_personal_bookmarks: "enable"
            gui_sslvpn_realms: "enable"
            gui_switch_controller: "enable"
            gui_threat_weight: "enable"
            gui_traffic_shaping: "enable"
            gui_voip_profile: "enable"
            gui_vpn: "enable"
            gui_waf_profile: "enable"
            gui_wan_load_balancing: "enable"
            gui_wanopt_cache: "enable"
            gui_webfilter: "enable"
            gui_webfilter_advanced: "enable"
            gui_wireless_controller: "enable"
            http_external_dest: "fortiweb"
            ike_dn_format: "with-space"
            ike_quick_crash_detect: "enable"
            ike_session_resume: "enable"
            implicit_allow_dns: "enable"
            ip: "<your_own_value>"
            ip6: "<your_own_value>"
            link_down_access: "enable"
            lldp_reception: "enable"
            lldp_transmission: "enable"
            mac_ttl: "90"
            manageip: "<your_own_value>"
            manageip6: "<your_own_value>"
            multicast_forward: "enable"
            multicast_skip_policy: "enable"
            multicast_ttl_notchange: "enable"
            ngfw_mode: "profile-based"
            opmode: "nat"
            prp_trailer_action: "enable"
            sccp_port: "99"
            sctp_session_without_init: "enable"
            ses_denied_traffic: "enable"
            sip_helper: "enable"
            sip_nat_trace: "enable"
            sip_ssl_port: "104"
            sip_tcp_port: "105"
            sip_udp_port: "106"
            snat_hairpin_traffic: "enable"
            ssl_ssh_profile: "<your_own_value> (source firewall.ssl-ssh-profile.name)"
            status: "enable"
            strict_src_check: "enable"
            tcp_session_without_syn: "enable"
            utf8_spam_tagging: "enable"
            v4_ecmp_mode: "source-ip-based"
            vpn_stats_log: "ipsec"
            vpn_stats_period: "115"
            wccp_cache_engine: "enable"


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
