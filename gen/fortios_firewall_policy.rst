:source: fortios_firewall_policy.py

:orphan:

.. fortios_firewall_policy:

fortios_firewall_policy -- Configure IPv4 policies in Fortinet's FortiOS and FortiGate.
+++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++

.. versionadded:: 2.8

.. contents::
   :local:
   :depth: 1


Synopsis
--------
- This module is able to configure a FortiGate or FortiOS (FOS) device by allowing the user to set and modify firewall feature and policy category. Examples include all parameters and values need to be adjusted to datasources before usage. Tested with FOS v6.2.0



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
    <li> <span class="li-head">action</span> - the action indiactor to move an object in the list <span class="li-normal">type: str</span> <span class="li-normal">choices: move</span></li>
    <li> <span class="li-head">self</span> - mkey of self identifier <span class="li-normal">type: str</span></li>
    <li> <span class="li-head">after</span> - mkey of target identifier <span class="li-normal">type: str</span></li>
    <li> <span class="li-head">before</span> - mkey of target identifier <span class="li-normal">type: str</span></li>
    <li> <span class="li-head">state</span> - Indicates whether to create or remove the object. This attribute was present already in previous version in a deeper level. It has been moved out to this outer level. <span class="li-normal">type: str</span> <span class="li-required">required: False</span> <span class="li-normal">choices: present, absent</span></li>
    <li> <span class="li-head">firewall_policy</span> - Configure IPv4 policies. <span class="li-normal">type: dict</span></li>
        <ul class="ul-self">
        <li> <span class="li-head">state</span> - B(Deprecated) <span class="li-normal">type: str</span> <span class="li-required">required: False</span> <span class="li-normal">choices: present, absent</span></li>
        <li> <span class="li-head">action</span> - Policy action (allow/deny/ipsec). <span class="li-normal">type: str</span> <span class="li-normal">choices: accept, deny, ipsec</span></li>
        <li> <span class="li-head">anti_replay</span> - Enable/disable anti-replay check. <span class="li-normal">type: str</span> <span class="li-normal">choices: enable, disable</span></li>
        <li> <span class="li-head">app_category</span> - Application category ID list. <span class="li-normal">type: list</span></li>
            <ul class="ul-self">
            <li> <span class="li-head">id</span> - Category IDs. <span class="li-normal">type: int</span> <span class="li-required">required: True</span></li>
            </ul>
        <li> <span class="li-head">app_group</span> - Application group names. <span class="li-normal">type: list</span></li>
            <ul class="ul-self">
            <li> <span class="li-head">name</span> - Application group names. Source application.group.name. <span class="li-normal">type: str</span> <span class="li-required">required: True</span></li>
            </ul>
        <li> <span class="li-head">application</span> - Application ID list. <span class="li-normal">type: list</span></li>
            <ul class="ul-self">
            <li> <span class="li-head">id</span> - Application IDs. <span class="li-normal">type: int</span> <span class="li-required">required: True</span></li>
            </ul>
        <li> <span class="li-head">application_list</span> - Name of an existing Application list. Source application.list.name. <span class="li-normal">type: str</span></li>
        <li> <span class="li-head">auth_cert</span> - HTTPS server certificate for policy authentication. Source vpn.certificate.local.name. <span class="li-normal">type: str</span></li>
        <li> <span class="li-head">auth_path</span> - Enable/disable authentication-based routing. <span class="li-normal">type: str</span> <span class="li-normal">choices: enable, disable</span></li>
        <li> <span class="li-head">auth_redirect_addr</span> - HTTP-to-HTTPS redirect address for firewall authentication. <span class="li-normal">type: str</span></li>
        <li> <span class="li-head">av_profile</span> - Name of an existing Antivirus profile. Source antivirus.profile.name. <span class="li-normal">type: str</span></li>
        <li> <span class="li-head">block_notification</span> - Enable/disable block notification. <span class="li-normal">type: str</span> <span class="li-normal">choices: enable, disable</span></li>
        <li> <span class="li-head">captive_portal_exempt</span> - Enable to exempt some users from the captive portal. <span class="li-normal">type: str</span> <span class="li-normal">choices: enable, disable</span></li>
        <li> <span class="li-head">capture_packet</span> - Enable/disable capture packets. <span class="li-normal">type: str</span> <span class="li-normal">choices: enable, disable</span></li>
        <li> <span class="li-head">cifs_profile</span> - Name of an existing CIFS profile. Source cifs.profile.name. <span class="li-normal">type: str</span></li>
        <li> <span class="li-head">comments</span> - Comment. <span class="li-normal">type: str</span></li>
        <li> <span class="li-head">custom_log_fields</span> - Custom fields to append to log messages for this policy. <span class="li-normal">type: list</span></li>
            <ul class="ul-self">
            <li> <span class="li-head">field_id</span> - Custom log field. Source log.custom-field.id. <span class="li-normal">type: str</span></li>
            </ul>
        <li> <span class="li-head">delay_tcp_npu_session</span> - Enable TCP NPU session delay to guarantee packet order of 3-way handshake. <span class="li-normal">type: str</span> <span class="li-normal">choices: enable, disable</span></li>
        <li> <span class="li-head">devices</span> - Names of devices or device groups that can be matched by the policy. <span class="li-normal">type: list</span></li>
            <ul class="ul-self">
            <li> <span class="li-head">name</span> - Device or group name. <span class="li-normal">type: str</span> <span class="li-required">required: True</span></li>
            </ul>
        <li> <span class="li-head">diffserv_forward</span> - Enable to change packet"s DiffServ values to the specified diffservcode-forward value. <span class="li-normal">type: str</span> <span class="li-normal">choices: enable, disable</span></li>
        <li> <span class="li-head">diffserv_reverse</span> - Enable to change packet"s reverse (reply) DiffServ values to the specified diffservcode-rev value. <span class="li-normal">type: str</span> <span class="li-normal">choices: enable, disable</span></li>
        <li> <span class="li-head">diffservcode_forward</span> - Change packet"s DiffServ to this value. <span class="li-normal">type: str</span></li>
        <li> <span class="li-head">diffservcode_rev</span> - Change packet"s reverse (reply) DiffServ to this value. <span class="li-normal">type: str</span></li>
        <li> <span class="li-head">disclaimer</span> - Enable/disable user authentication disclaimer. <span class="li-normal">type: str</span> <span class="li-normal">choices: enable, disable</span></li>
        <li> <span class="li-head">dlp_sensor</span> - Name of an existing DLP sensor. Source dlp.sensor.name. <span class="li-normal">type: str</span></li>
        <li> <span class="li-head">dnsfilter_profile</span> - Name of an existing DNS filter profile. Source dnsfilter.profile.name. <span class="li-normal">type: str</span></li>
        <li> <span class="li-head">dsri</span> - Enable DSRI to ignore HTTP server responses. <span class="li-normal">type: str</span> <span class="li-normal">choices: enable, disable</span></li>
        <li> <span class="li-head">dstaddr</span> - Destination address and address group names. <span class="li-normal">type: list</span></li>
            <ul class="ul-self">
            <li> <span class="li-head">name</span> - Address name. Source firewall.address.name firewall.addrgrp.name firewall.vip.name firewall.vipgrp.name system.external-resource .name. <span class="li-normal">type: str</span> <span class="li-required">required: True</span></li>
            </ul>
        <li> <span class="li-head">dstaddr_negate</span> - When enabled dstaddr specifies what the destination address must NOT be. <span class="li-normal">type: str</span> <span class="li-normal">choices: enable, disable</span></li>
        <li> <span class="li-head">dstintf</span> - Outgoing (egress) interface. <span class="li-normal">type: list</span></li>
            <ul class="ul-self">
            <li> <span class="li-head">name</span> - Interface name. Source system.interface.name system.zone.name. <span class="li-normal">type: str</span> <span class="li-required">required: True</span></li>
            </ul>
        <li> <span class="li-head">email_collect</span> - Enable/disable email collection. <span class="li-normal">type: str</span> <span class="li-normal">choices: enable, disable</span></li>
        <li> <span class="li-head">emailfilter_profile</span> - Name of an existing email filter profile. Source emailfilter.profile.name. <span class="li-normal">type: str</span></li>
        <li> <span class="li-head">firewall_session_dirty</span> - How to handle sessions if the configuration of this firewall policy changes. <span class="li-normal">type: str</span> <span class="li-normal">choices: check-all, check-new</span></li>
        <li> <span class="li-head">fixedport</span> - Enable to prevent source NAT from changing a session"s source port. <span class="li-normal">type: str</span> <span class="li-normal">choices: enable, disable</span></li>
        <li> <span class="li-head">fsso</span> - Enable/disable Fortinet Single Sign-On. <span class="li-normal">type: str</span> <span class="li-normal">choices: enable, disable</span></li>
        <li> <span class="li-head">fsso_agent_for_ntlm</span> - FSSO agent to use for NTLM authentication. Source user.fsso.name. <span class="li-normal">type: str</span></li>
        <li> <span class="li-head">geoip_anycast</span> - Enable/disable recognition of anycast IP addresses using the geography IP database. <span class="li-normal">type: str</span> <span class="li-normal">choices: enable, disable</span></li>
        <li> <span class="li-head">global_label</span> - Label for the policy that appears when the GUI is in Global View mode. <span class="li-normal">type: str</span></li>
        <li> <span class="li-head">groups</span> - Names of user groups that can authenticate with this policy. <span class="li-normal">type: list</span></li>
            <ul class="ul-self">
            <li> <span class="li-head">name</span> - Group name. Source user.group.name. <span class="li-normal">type: str</span> <span class="li-required">required: True</span></li>
            </ul>
        <li> <span class="li-head">http_policy_redirect</span> - Redirect HTTP(S) traffic to matching transparent web proxy policy. <span class="li-normal">type: str</span> <span class="li-normal">choices: enable, disable</span></li>
        <li> <span class="li-head">icap_profile</span> - Name of an existing ICAP profile. Source icap.profile.name. <span class="li-normal">type: str</span></li>
        <li> <span class="li-head">identity_based_route</span> - Name of identity-based routing rule. Source firewall.identity-based-route.name. <span class="li-normal">type: str</span></li>
        <li> <span class="li-head">inbound</span> - Policy-based IPsec VPN: only traffic from the remote network can initiate a VPN. <span class="li-normal">type: str</span> <span class="li-normal">choices: enable, disable</span></li>
        <li> <span class="li-head">inspection_mode</span> - Inspection mode. <span class="li-normal">type: str</span> <span class="li-normal">choices: proxy, flow</span></li>
        <li> <span class="li-head">internet_service</span> - Enable/disable use of Internet Services for this policy. If enabled, destination address and service are not used. <span class="li-normal">type: str</span> <span class="li-normal">choices: enable, disable</span></li>
        <li> <span class="li-head">internet_service_custom</span> - Custom Internet Service name. <span class="li-normal">type: list</span></li>
            <ul class="ul-self">
            <li> <span class="li-head">name</span> - Custom Internet Service name. Source firewall.internet-service-custom.name. <span class="li-normal">type: str</span> <span class="li-required">required: True</span></li>
            </ul>
        <li> <span class="li-head">internet_service_custom_group</span> - Custom Internet Service group name. <span class="li-normal">type: list</span></li>
            <ul class="ul-self">
            <li> <span class="li-head">name</span> - Custom Internet Service group name. Source firewall.internet-service-custom-group.name. <span class="li-normal">type: str</span> <span class="li-required">required: True</span></li>
            </ul>
        <li> <span class="li-head">internet_service_group</span> - Internet Service group name. <span class="li-normal">type: list</span></li>
            <ul class="ul-self">
            <li> <span class="li-head">name</span> - Internet Service group name. Source firewall.internet-service-group.name. <span class="li-normal">type: str</span> <span class="li-required">required: True</span></li>
            </ul>
        <li> <span class="li-head">internet_service_id</span> - Internet Service ID. <span class="li-normal">type: list</span></li>
            <ul class="ul-self">
            <li> <span class="li-head">id</span> - Internet Service ID. Source firewall.internet-service.id. <span class="li-normal">type: int</span> <span class="li-required">required: True</span></li>
            </ul>
        <li> <span class="li-head">internet_service_negate</span> - When enabled internet-service specifies what the service must NOT be. <span class="li-normal">type: str</span> <span class="li-normal">choices: enable, disable</span></li>
        <li> <span class="li-head">internet_service_src</span> - Enable/disable use of Internet Services in source for this policy. If enabled, source address is not used. <span class="li-normal">type: str</span> <span class="li-normal">choices: enable, disable</span></li>
        <li> <span class="li-head">internet_service_src_custom</span> - Custom Internet Service source name. <span class="li-normal">type: list</span></li>
            <ul class="ul-self">
            <li> <span class="li-head">name</span> - Custom Internet Service name. Source firewall.internet-service-custom.name. <span class="li-normal">type: str</span> <span class="li-required">required: True</span></li>
            </ul>
        <li> <span class="li-head">internet_service_src_custom_group</span> - Custom Internet Service source group name. <span class="li-normal">type: list</span></li>
            <ul class="ul-self">
            <li> <span class="li-head">name</span> - Custom Internet Service group name. Source firewall.internet-service-custom-group.name. <span class="li-normal">type: str</span> <span class="li-required">required: True</span></li>
            </ul>
        <li> <span class="li-head">internet_service_src_group</span> - Internet Service source group name. <span class="li-normal">type: list</span></li>
            <ul class="ul-self">
            <li> <span class="li-head">name</span> - Internet Service group name. Source firewall.internet-service-group.name. <span class="li-normal">type: str</span> <span class="li-required">required: True</span></li>
            </ul>
        <li> <span class="li-head">internet_service_src_id</span> - Internet Service source ID. <span class="li-normal">type: list</span></li>
            <ul class="ul-self">
            <li> <span class="li-head">id</span> - Internet Service ID. Source firewall.internet-service.id. <span class="li-normal">type: int</span> <span class="li-required">required: True</span></li>
            </ul>
        <li> <span class="li-head">internet_service_src_negate</span> - When enabled internet-service-src specifies what the service must NOT be. <span class="li-normal">type: str</span> <span class="li-normal">choices: enable, disable</span></li>
        <li> <span class="li-head">ippool</span> - Enable to use IP Pools for source NAT. <span class="li-normal">type: str</span> <span class="li-normal">choices: enable, disable</span></li>
        <li> <span class="li-head">ips_sensor</span> - Name of an existing IPS sensor. Source ips.sensor.name. <span class="li-normal">type: str</span></li>
        <li> <span class="li-head">label</span> - Label for the policy that appears when the GUI is in Section View mode. <span class="li-normal">type: str</span></li>
        <li> <span class="li-head">logtraffic</span> - Enable or disable logging. Log all sessions or security profile sessions. <span class="li-normal">type: str</span> <span class="li-normal">choices: all, utm, disable</span></li>
        <li> <span class="li-head">logtraffic_start</span> - Record logs when a session starts. <span class="li-normal">type: str</span> <span class="li-normal">choices: enable, disable</span></li>
        <li> <span class="li-head">match_vip</span> - Enable to match packets that have had their destination addresses changed by a VIP. <span class="li-normal">type: str</span> <span class="li-normal">choices: enable, disable</span></li>
        <li> <span class="li-head">name</span> - Policy name. <span class="li-normal">type: str</span></li>
        <li> <span class="li-head">nat</span> - Enable/disable source NAT. <span class="li-normal">type: str</span> <span class="li-normal">choices: enable, disable</span></li>
        <li> <span class="li-head">natinbound</span> - Policy-based IPsec VPN: apply destination NAT to inbound traffic. <span class="li-normal">type: str</span> <span class="li-normal">choices: enable, disable</span></li>
        <li> <span class="li-head">natip</span> - Policy-based IPsec VPN: source NAT IP address for outgoing traffic. <span class="li-normal">type: str</span></li>
        <li> <span class="li-head">natoutbound</span> - Policy-based IPsec VPN: apply source NAT to outbound traffic. <span class="li-normal">type: str</span> <span class="li-normal">choices: enable, disable</span></li>
        <li> <span class="li-head">ntlm</span> - Enable/disable NTLM authentication. <span class="li-normal">type: str</span> <span class="li-normal">choices: enable, disable</span></li>
        <li> <span class="li-head">ntlm_enabled_browsers</span> - HTTP-User-Agent value of supported browsers. <span class="li-normal">type: list</span></li>
            <ul class="ul-self">
            <li> <span class="li-head">user_agent_string</span> - User agent string. <span class="li-normal">type: str</span></li>
            </ul>
        <li> <span class="li-head">ntlm_guest</span> - Enable/disable NTLM guest user access. <span class="li-normal">type: str</span> <span class="li-normal">choices: enable, disable</span></li>
        <li> <span class="li-head">outbound</span> - Policy-based IPsec VPN: only traffic from the internal network can initiate a VPN. <span class="li-normal">type: str</span> <span class="li-normal">choices: enable, disable</span></li>
        <li> <span class="li-head">per_ip_shaper</span> - Per-IP traffic shaper. Source firewall.shaper.per-ip-shaper.name. <span class="li-normal">type: str</span></li>
        <li> <span class="li-head">permit_any_host</span> - Accept UDP packets from any host. <span class="li-normal">type: str</span> <span class="li-normal">choices: enable, disable</span></li>
        <li> <span class="li-head">permit_stun_host</span> - Accept UDP packets from any Session Traversal Utilities for NAT (STUN) host. <span class="li-normal">type: str</span> <span class="li-normal">choices: enable, disable</span></li>
        <li> <span class="li-head">policyid</span> - Policy ID (0 - 4294967294). <span class="li-normal">type: int</span> <span class="li-required">required: True</span></li>
        <li> <span class="li-head">poolname</span> - IP Pool names. <span class="li-normal">type: list</span></li>
            <ul class="ul-self">
            <li> <span class="li-head">name</span> - IP pool name. Source firewall.ippool.name. <span class="li-normal">type: str</span> <span class="li-required">required: True</span></li>
            </ul>
        <li> <span class="li-head">profile_group</span> - Name of profile group. Source firewall.profile-group.name. <span class="li-normal">type: str</span></li>
        <li> <span class="li-head">profile_protocol_options</span> - Name of an existing Protocol options profile. Source firewall.profile-protocol-options.name. <span class="li-normal">type: str</span></li>
        <li> <span class="li-head">profile_type</span> - Determine whether the firewall policy allows security profile groups or single profiles only. <span class="li-normal">type: str</span> <span class="li-normal">choices: single, group</span></li>
        <li> <span class="li-head">radius_mac_auth_bypass</span> - Enable MAC authentication bypass. The bypassed MAC address must be received from RADIUS server. <span class="li-normal">type: str</span> <span class="li-normal">choices: enable, disable</span></li>
        <li> <span class="li-head">redirect_url</span> - URL users are directed to after seeing and accepting the disclaimer or authenticating. <span class="li-normal">type: str</span></li>
        <li> <span class="li-head">replacemsg_override_group</span> - Override the default replacement message group for this policy. Source system.replacemsg-group.name. <span class="li-normal">type: str</span></li>
        <li> <span class="li-head">reputation_direction</span> - Direction of the initial traffic for reputation to take effect. <span class="li-normal">type: str</span> <span class="li-normal">choices: source, destination</span></li>
        <li> <span class="li-head">reputation_minimum</span> - Minimum Reputation to take action. Source firewall.internet-service-reputation.id. <span class="li-normal">type: int</span></li>
        <li> <span class="li-head">rsso</span> - Enable/disable RADIUS single sign-on (RSSO). <span class="li-normal">type: str</span> <span class="li-normal">choices: enable, disable</span></li>
        <li> <span class="li-head">rtp_addr</span> - Address names if this is an RTP NAT policy. <span class="li-normal">type: list</span></li>
            <ul class="ul-self">
            <li> <span class="li-head">name</span> - Address name. Source firewall.internet-service-custom-group.name firewall.addrgrp.name. <span class="li-normal">type: str</span> <span class="li-required">required: True</span></li>
            </ul>
        <li> <span class="li-head">rtp_nat</span> - Enable Real Time Protocol (RTP) NAT. <span class="li-normal">type: str</span> <span class="li-normal">choices: disable, enable</span></li>
        <li> <span class="li-head">schedule</span> - Schedule name. Source firewall.schedule.onetime.name firewall.schedule.recurring.name firewall.schedule.group.name. <span class="li-normal">type: str</span></li>
        <li> <span class="li-head">schedule_timeout</span> - Enable to force current sessions to end when the schedule object times out. Disable allows them to end from inactivity. <span class="li-normal">type: str</span> <span class="li-normal">choices: enable, disable</span></li>
        <li> <span class="li-head">send_deny_packet</span> - Enable to send a reply when a session is denied or blocked by a firewall policy. <span class="li-normal">type: str</span> <span class="li-normal">choices: disable, enable</span></li>
        <li> <span class="li-head">service</span> - Service and service group names. <span class="li-normal">type: list</span></li>
            <ul class="ul-self">
            <li> <span class="li-head">name</span> - Service and service group names. Source firewall.service.custom.name firewall.service.group.name. <span class="li-normal">type: str</span> <span class="li-required">required: True</span></li>
            </ul>
        <li> <span class="li-head">service_negate</span> - When enabled service specifies what the service must NOT be. <span class="li-normal">type: str</span> <span class="li-normal">choices: enable, disable</span></li>
        <li> <span class="li-head">session_ttl</span> - TTL in seconds for sessions accepted by this policy (0 means use the system ). <span class="li-normal">type: int</span></li>
        <li> <span class="li-head">srcaddr</span> - Source address and address group names. <span class="li-normal">type: list</span></li>
            <ul class="ul-self">
            <li> <span class="li-head">name</span> - Address name. Source firewall.address.name firewall.addrgrp.name system.external-resource.name. <span class="li-normal">type: str</span> <span class="li-required">required: True</span></li>
            </ul>
        <li> <span class="li-head">srcaddr_negate</span> - When enabled srcaddr specifies what the source address must NOT be. <span class="li-normal">type: str</span> <span class="li-normal">choices: enable, disable</span></li>
        <li> <span class="li-head">srcintf</span> - Incoming (ingress) interface. <span class="li-normal">type: list</span></li>
            <ul class="ul-self">
            <li> <span class="li-head">name</span> - Interface name. Source system.interface.name system.zone.name. <span class="li-normal">type: str</span> <span class="li-required">required: True</span></li>
            </ul>
        <li> <span class="li-head">ssh_filter_profile</span> - Name of an existing SSH filter profile. Source ssh-filter.profile.name. <span class="li-normal">type: str</span></li>
        <li> <span class="li-head">ssh_policy_redirect</span> - Redirect SSH traffic to matching transparent proxy policy. <span class="li-normal">type: str</span> <span class="li-normal">choices: enable, disable</span></li>
        <li> <span class="li-head">ssl_mirror</span> - Enable to copy decrypted SSL traffic to a FortiGate interface (called SSL mirroring). <span class="li-normal">type: str</span> <span class="li-normal">choices: enable, disable</span></li>
        <li> <span class="li-head">ssl_mirror_intf</span> - SSL mirror interface name. <span class="li-normal">type: list</span></li>
            <ul class="ul-self">
            <li> <span class="li-head">name</span> - Mirror Interface name. Source system.interface.name system.zone.name. <span class="li-normal">type: str</span> <span class="li-required">required: True</span></li>
            </ul>
        <li> <span class="li-head">ssl_ssh_profile</span> - Name of an existing SSL SSH profile. Source firewall.ssl-ssh-profile.name. <span class="li-normal">type: str</span></li>
        <li> <span class="li-head">status</span> - Enable or disable this policy. <span class="li-normal">type: str</span> <span class="li-normal">choices: enable, disable</span></li>
        <li> <span class="li-head">tcp_mss_receiver</span> - Receiver TCP maximum segment size (MSS). <span class="li-normal">type: int</span></li>
        <li> <span class="li-head">tcp_mss_sender</span> - Sender TCP maximum segment size (MSS). <span class="li-normal">type: int</span></li>
        <li> <span class="li-head">tcp_session_without_syn</span> - Enable/disable creation of TCP session without SYN flag. <span class="li-normal">type: str</span> <span class="li-normal">choices: all, data-only, disable</span></li>
        <li> <span class="li-head">timeout_send_rst</span> - Enable/disable sending RST packets when TCP sessions expire. <span class="li-normal">type: str</span> <span class="li-normal">choices: enable, disable</span></li>
        <li> <span class="li-head">tos</span> - ToS (Type of Service) value used for comparison. <span class="li-normal">type: str</span></li>
        <li> <span class="li-head">tos_mask</span> - Non-zero bit positions are used for comparison while zero bit positions are ignored. <span class="li-normal">type: str</span></li>
        <li> <span class="li-head">tos_negate</span> - Enable negated TOS match. <span class="li-normal">type: str</span> <span class="li-normal">choices: enable, disable</span></li>
        <li> <span class="li-head">traffic_shaper</span> - Traffic shaper. Source firewall.shaper.traffic-shaper.name. <span class="li-normal">type: str</span></li>
        <li> <span class="li-head">traffic_shaper_reverse</span> - Reverse traffic shaper. Source firewall.shaper.traffic-shaper.name. <span class="li-normal">type: str</span></li>
        <li> <span class="li-head">url_category</span> - URL category ID list. <span class="li-normal">type: list</span></li>
            <ul class="ul-self">
            <li> <span class="li-head">id</span> - URL category ID. <span class="li-normal">type: int</span> <span class="li-required">required: True</span></li>
            </ul>
        <li> <span class="li-head">users</span> - Names of individual users that can authenticate with this policy. <span class="li-normal">type: list</span></li>
            <ul class="ul-self">
            <li> <span class="li-head">name</span> - Names of individual users that can authenticate with this policy. Source user.local.name. <span class="li-normal">type: str</span> <span class="li-required">required: True</span></li>
            </ul>
        <li> <span class="li-head">utm_status</span> - Enable to add one or more security profiles (AV, IPS, etc.) to the firewall policy. <span class="li-normal">type: str</span> <span class="li-normal">choices: enable, disable</span></li>
        <li> <span class="li-head">uuid</span> - Universally Unique Identifier (UUID; automatically assigned but can be manually reset). <span class="li-normal">type: str</span></li>
        <li> <span class="li-head">vlan_cos_fwd</span> - VLAN forward direction user priority: 255 passthrough, 0 lowest, 7 highest. <span class="li-normal">type: int</span></li>
        <li> <span class="li-head">vlan_cos_rev</span> - VLAN reverse direction user priority: 255 passthrough, 0 lowest, 7 highest. <span class="li-normal">type: int</span></li>
        <li> <span class="li-head">vlan_filter</span> - Set VLAN filters. <span class="li-normal">type: str</span></li>
        <li> <span class="li-head">voip_profile</span> - Name of an existing VoIP profile. Source voip.profile.name. <span class="li-normal">type: str</span></li>
        <li> <span class="li-head">vpntunnel</span> - Policy-based IPsec VPN: name of the IPsec VPN Phase 1. Source vpn.ipsec.phase1.name vpn.ipsec.manualkey.name. <span class="li-normal">type: str</span></li>
        <li> <span class="li-head">waf_profile</span> - Name of an existing Web application firewall profile. Source waf.profile.name. <span class="li-normal">type: str</span></li>
        <li> <span class="li-head">wanopt</span> - Enable/disable WAN optimization. <span class="li-normal">type: str</span> <span class="li-normal">choices: enable, disable</span></li>
        <li> <span class="li-head">wanopt_detection</span> - WAN optimization auto-detection mode. <span class="li-normal">type: str</span> <span class="li-normal">choices: active, passive, False</span></li>
        <li> <span class="li-head">wanopt_passive_opt</span> - WAN optimization passive mode options. This option decides what IP address will be used to connect server. <span class="li-normal">type: str</span> <span class="li-normal">choices: default, transparent, non-transparent</span></li>
        <li> <span class="li-head">wanopt_peer</span> - WAN optimization peer. Source wanopt.peer.peer-host-id. <span class="li-normal">type: str</span></li>
        <li> <span class="li-head">wanopt_profile</span> - WAN optimization profile. Source wanopt.profile.name. <span class="li-normal">type: str</span></li>
        <li> <span class="li-head">wccp</span> - Enable/disable forwarding traffic matching this policy to a configured WCCP server. <span class="li-normal">type: str</span> <span class="li-normal">choices: enable, disable</span></li>
        <li> <span class="li-head">webcache</span> - Enable/disable web cache. <span class="li-normal">type: str</span> <span class="li-normal">choices: enable, disable</span></li>
        <li> <span class="li-head">webcache_https</span> - Enable/disable web cache for HTTPS. <span class="li-normal">type: str</span> <span class="li-normal">choices: disable, enable</span></li>
        <li> <span class="li-head">webfilter_profile</span> - Name of an existing Web filter profile. Source webfilter.profile.name. <span class="li-normal">type: str</span></li>
        <li> <span class="li-head">webproxy_forward_server</span> - Web proxy forward server name. Source web-proxy.forward-server.name web-proxy.forward-server-group.name. <span class="li-normal">type: str</span></li>
        <li> <span class="li-head">webproxy_profile</span> - Webproxy profile name. Source web-proxy.profile.name. <span class="li-normal">type: str</span></li>
        <li> <span class="li-head">wsso</span> - Enable/disable WiFi Single Sign On (WSSO). <span class="li-normal">type: str</span> <span class="li-normal">choices: enable, disable</span></li>
        </ul>
    </ul>


Notes
-----

.. note::

   - Legacy fortiosapi has been deprecated, httpapi is the preferred way to run playbooks

   - Adjust object order by moving self after(before) another.

   - Only one of [after, before] must be specified when action is moving an object.



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
      - name: Configure IPv4 policies.
        fortios_firewall_policy:
          vdom:  "{{ vdom }}"
          state: "present"
          access_token: "<your_own_value>"
          firewall_policy:
            action: "accept"
            anti_replay: "enable"
            app_category:
             -
                id:  "6"
            app_group:
             -
                name: "default_name_8 (source application.group.name)"
            application:
             -
                id:  "10"
            application_list: "<your_own_value> (source application.list.name)"
            auth_cert: "<your_own_value> (source vpn.certificate.local.name)"
            auth_path: "enable"
            auth_redirect_addr: "<your_own_value>"
            av_profile: "<your_own_value> (source antivirus.profile.name)"
            block_notification: "enable"
            captive_portal_exempt: "enable"
            capture_packet: "enable"
            cifs_profile: "<your_own_value> (source cifs.profile.name)"
            comments: "<your_own_value>"
            custom_log_fields:
             -
                field_id: "<your_own_value> (source log.custom-field.id)"
            delay_tcp_npu_session: "enable"
            devices:
             -
                name: "default_name_25"
            diffserv_forward: "enable"
            diffserv_reverse: "enable"
            diffservcode_forward: "<your_own_value>"
            diffservcode_rev: "<your_own_value>"
            disclaimer: "enable"
            dlp_sensor: "<your_own_value> (source dlp.sensor.name)"
            dnsfilter_profile: "<your_own_value> (source dnsfilter.profile.name)"
            dsri: "enable"
            dstaddr:
             -
                name: "default_name_35 (source firewall.address.name firewall.addrgrp.name firewall.vip.name firewall.vipgrp.name system.external-resource.name)"
            dstaddr_negate: "enable"
            dstintf:
             -
                name: "default_name_38 (source system.interface.name system.zone.name)"
            email_collect: "enable"
            emailfilter_profile: "<your_own_value> (source emailfilter.profile.name)"
            firewall_session_dirty: "check-all"
            fixedport: "enable"
            fsso: "enable"
            fsso_agent_for_ntlm: "<your_own_value> (source user.fsso.name)"
            geoip_anycast: "enable"
            global_label: "<your_own_value>"
            groups:
             -
                name: "default_name_48 (source user.group.name)"
            http_policy_redirect: "enable"
            icap_profile: "<your_own_value> (source icap.profile.name)"
            identity_based_route: "<your_own_value> (source firewall.identity-based-route.name)"
            inbound: "enable"
            inspection_mode: "proxy"
            internet_service: "enable"
            internet_service_custom:
             -
                name: "default_name_56 (source firewall.internet-service-custom.name)"
            internet_service_custom_group:
             -
                name: "default_name_58 (source firewall.internet-service-custom-group.name)"
            internet_service_group:
             -
                name: "default_name_60 (source firewall.internet-service-group.name)"
            internet_service_id:
             -
                id:  "62 (source firewall.internet-service.id)"
            internet_service_negate: "enable"
            internet_service_src: "enable"
            internet_service_src_custom:
             -
                name: "default_name_66 (source firewall.internet-service-custom.name)"
            internet_service_src_custom_group:
             -
                name: "default_name_68 (source firewall.internet-service-custom-group.name)"
            internet_service_src_group:
             -
                name: "default_name_70 (source firewall.internet-service-group.name)"
            internet_service_src_id:
             -
                id:  "72 (source firewall.internet-service.id)"
            internet_service_src_negate: "enable"
            ippool: "enable"
            ips_sensor: "<your_own_value> (source ips.sensor.name)"
            label: "<your_own_value>"
            logtraffic: "all"
            logtraffic_start: "enable"
            match_vip: "enable"
            name: "default_name_80"
            nat: "enable"
            natinbound: "enable"
            natip: "<your_own_value>"
            natoutbound: "enable"
            ntlm: "enable"
            ntlm_enabled_browsers:
             -
                user_agent_string: "<your_own_value>"
            ntlm_guest: "enable"
            outbound: "enable"
            per_ip_shaper: "<your_own_value> (source firewall.shaper.per-ip-shaper.name)"
            permit_any_host: "enable"
            permit_stun_host: "enable"
            policyid: "93"
            poolname:
             -
                name: "default_name_95 (source firewall.ippool.name)"
            profile_group: "<your_own_value> (source firewall.profile-group.name)"
            profile_protocol_options: "<your_own_value> (source firewall.profile-protocol-options.name)"
            profile_type: "single"
            radius_mac_auth_bypass: "enable"
            redirect_url: "<your_own_value>"
            replacemsg_override_group: "<your_own_value> (source system.replacemsg-group.name)"
            reputation_direction: "source"
            reputation_minimum: "103 (source firewall.internet-service-reputation.id)"
            rsso: "enable"
            rtp_addr:
             -
                name: "default_name_106 (source firewall.internet-service-custom-group.name firewall.addrgrp.name)"
            rtp_nat: "disable"
            schedule: "<your_own_value> (source firewall.schedule.onetime.name firewall.schedule.recurring.name firewall.schedule.group.name)"
            schedule_timeout: "enable"
            send_deny_packet: "disable"
            service:
             -
                name: "default_name_112 (source firewall.service.custom.name firewall.service.group.name)"
            service_negate: "enable"
            session_ttl: "114"
            srcaddr:
             -
                name: "default_name_116 (source firewall.address.name firewall.addrgrp.name system.external-resource.name)"
            srcaddr_negate: "enable"
            srcintf:
             -
                name: "default_name_119 (source system.interface.name system.zone.name)"
            ssh_filter_profile: "<your_own_value> (source ssh-filter.profile.name)"
            ssh_policy_redirect: "enable"
            ssl_mirror: "enable"
            ssl_mirror_intf:
             -
                name: "default_name_124 (source system.interface.name system.zone.name)"
            ssl_ssh_profile: "<your_own_value> (source firewall.ssl-ssh-profile.name)"
            status: "enable"
            tcp_mss_receiver: "127"
            tcp_mss_sender: "128"
            tcp_session_without_syn: "all"
            timeout_send_rst: "enable"
            tos: "<your_own_value>"
            tos_mask: "<your_own_value>"
            tos_negate: "enable"
            traffic_shaper: "<your_own_value> (source firewall.shaper.traffic-shaper.name)"
            traffic_shaper_reverse: "<your_own_value> (source firewall.shaper.traffic-shaper.name)"
            url_category:
             -
                id:  "137"
            users:
             -
                name: "default_name_139 (source user.local.name)"
            utm_status: "enable"
            uuid: "<your_own_value>"
            vlan_cos_fwd: "142"
            vlan_cos_rev: "143"
            vlan_filter: "<your_own_value>"
            voip_profile: "<your_own_value> (source voip.profile.name)"
            vpntunnel: "<your_own_value> (source vpn.ipsec.phase1.name vpn.ipsec.manualkey.name)"
            waf_profile: "<your_own_value> (source waf.profile.name)"
            wanopt: "enable"
            wanopt_detection: "active"
            wanopt_passive_opt: "default"
            wanopt_peer: "<your_own_value> (source wanopt.peer.peer-host-id)"
            wanopt_profile: "<your_own_value> (source wanopt.profile.name)"
            wccp: "enable"
            webcache: "enable"
            webcache_https: "disable"
            webfilter_profile: "<your_own_value> (source webfilter.profile.name)"
            webproxy_forward_server: "<your_own_value> (source web-proxy.forward-server.name web-proxy.forward-server-group.name)"
            webproxy_profile: "<your_own_value> (source web-proxy.profile.name)"
            wsso: "enable"
    
      - name: move firewall.policy
        fortios_firewall_policy:
          vdom:  "root"
          action: "move"
          self: "<mkey of self identifier>"
          after: "<mkey of target identifier>"
         #before: "<mkey of target identifier>"
    


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
