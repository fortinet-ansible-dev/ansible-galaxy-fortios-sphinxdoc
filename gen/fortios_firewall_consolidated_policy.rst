:source: fortios_firewall_consolidated_policy.py

:orphan:

.. fortios_firewall_consolidated_policy:

fortios_firewall_consolidated_policy -- Configure consolidated IPv4/IPv6 policies in Fortinet's FortiOS and FortiGate.
++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++

.. versionadded:: 2.9

.. contents::
   :local:
   :depth: 1


Synopsis
--------
- This module is able to configure a FortiGate or FortiOS (FOS) device by allowing the user to set and modify firewall_consolidated feature and policy category. Examples include all parameters and values need to be adjusted to datasources before usage. Tested with FOS v6.4.0



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
    <li> <span class="li-head">state</span> - Indicates whether to create or remove the object. <span class="li-normal">type: str</span> <span class="li-required">required: True</span> <span class="li-normal">choices: present, absent</span></li>
    <li> <span class="li-head">firewall_consolidated_policy</span> - Configure consolidated IPv4/IPv6 policies. <span class="li-normal">type: dict</span></li>
        <ul class="ul-self">
        <li> <span class="li-head">action</span> - Policy action (allow/deny/ipsec). <span class="li-normal">type: str</span> <span class="li-normal">choices: accept, deny, ipsec</span></li>
        <li> <span class="li-head">application_list</span> - Name of an existing Application list. Source application.list.name. <span class="li-normal">type: str</span></li>
        <li> <span class="li-head">auto_asic_offload</span> - Enable/disable policy traffic ASIC offloading. <span class="li-normal">type: str</span> <span class="li-normal">choices: enable, disable</span></li>
        <li> <span class="li-head">av_profile</span> - Name of an existing Antivirus profile. Source antivirus.profile.name. <span class="li-normal">type: str</span></li>
        <li> <span class="li-head">captive_portal_exempt</span> - Enable exemption of some users from the captive portal. <span class="li-normal">type: str</span> <span class="li-normal">choices: enable, disable</span></li>
        <li> <span class="li-head">cifs_profile</span> - Name of an existing CIFS profile. Source cifs.profile.name. <span class="li-normal">type: str</span></li>
        <li> <span class="li-head">comments</span> - Comment. <span class="li-normal">type: str</span></li>
        <li> <span class="li-head">diffserv_forward</span> - Enable to change packet"s DiffServ values to the specified diffservcode-forward value. <span class="li-normal">type: str</span> <span class="li-normal">choices: enable, disable</span></li>
        <li> <span class="li-head">diffserv_reverse</span> - Enable to change packet"s reverse (reply) DiffServ values to the specified diffservcode-rev value. <span class="li-normal">type: str</span> <span class="li-normal">choices: enable, disable</span></li>
        <li> <span class="li-head">diffservcode_forward</span> - Change packet"s DiffServ to this value. <span class="li-normal">type: str</span></li>
        <li> <span class="li-head">diffservcode_rev</span> - Change packet"s reverse (reply) DiffServ to this value. <span class="li-normal">type: str</span></li>
        <li> <span class="li-head">dlp_sensor</span> - Name of an existing DLP sensor. Source dlp.sensor.name. <span class="li-normal">type: str</span></li>
        <li> <span class="li-head">dnsfilter_profile</span> - Name of an existing DNS filter profile. Source dnsfilter.profile.name. <span class="li-normal">type: str</span></li>
        <li> <span class="li-head">dstaddr_negate</span> - When enabled dstaddr specifies what the destination address must NOT be. <span class="li-normal">type: str</span> <span class="li-normal">choices: enable, disable</span></li>
        <li> <span class="li-head">dstaddr4</span> - Destination IPv4 address name and address group names. <span class="li-normal">type: list</span></li>
            <ul class="ul-self">
            <li> <span class="li-head">name</span> - Address name. Source firewall.address.name firewall.addrgrp.name firewall.vip.name firewall.vipgrp.name system.external-resource .name. <span class="li-normal">type: str</span> <span class="li-required">required: True</span></li>
            </ul>
        <li> <span class="li-head">dstaddr6</span> - Destination IPv6 address name and address group names. <span class="li-normal">type: list</span></li>
            <ul class="ul-self">
            <li> <span class="li-head">name</span> - Address name. Source firewall.address6.name firewall.addrgrp6.name firewall.vip6.name firewall.vipgrp6.name system .external-resource.name. <span class="li-normal">type: str</span> <span class="li-required">required: True</span></li>
            </ul>
        <li> <span class="li-head">dstintf</span> - Outgoing (egress) interface. <span class="li-normal">type: list</span></li>
            <ul class="ul-self">
            <li> <span class="li-head">name</span> - Interface name. Source system.interface.name system.zone.name. <span class="li-normal">type: str</span> <span class="li-required">required: True</span></li>
            </ul>
        <li> <span class="li-head">emailfilter_profile</span> - Name of an existing email filter profile. Source emailfilter.profile.name. <span class="li-normal">type: str</span></li>
        <li> <span class="li-head">fixedport</span> - Enable to prevent source NAT from changing a session"s source port. <span class="li-normal">type: str</span> <span class="li-normal">choices: enable, disable</span></li>
        <li> <span class="li-head">fsso_groups</span> - Names of FSSO groups. <span class="li-normal">type: list</span></li>
            <ul class="ul-self">
            <li> <span class="li-head">name</span> - Names of FSSO groups. Source user.adgrp.name. <span class="li-normal">type: str</span> <span class="li-required">required: True</span></li>
            </ul>
        <li> <span class="li-head">groups</span> - Names of user groups that can authenticate with this policy. <span class="li-normal">type: list</span></li>
            <ul class="ul-self">
            <li> <span class="li-head">name</span> - Group name. Source user.group.name. <span class="li-normal">type: str</span> <span class="li-required">required: True</span></li>
            </ul>
        <li> <span class="li-head">http_policy_redirect</span> - Redirect HTTP(S) traffic to matching transparent web proxy policy. <span class="li-normal">type: str</span> <span class="li-normal">choices: enable, disable</span></li>
        <li> <span class="li-head">icap_profile</span> - Name of an existing ICAP profile. Source icap.profile.name. <span class="li-normal">type: str</span></li>
        <li> <span class="li-head">inbound</span> - Policy-based IPsec VPN: only traffic from the remote network can initiate a VPN. <span class="li-normal">type: str</span> <span class="li-normal">choices: enable, disable</span></li>
        <li> <span class="li-head">inspection_mode</span> - Policy inspection mode (Flow/proxy). Default is Flow mode. <span class="li-normal">type: str</span> <span class="li-normal">choices: proxy, flow</span></li>
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
        <li> <span class="li-head">internet_service_name</span> - Internet Service name. <span class="li-normal">type: list</span></li>
            <ul class="ul-self">
            <li> <span class="li-head">name</span> - Internet Service name. Source firewall.internet-service-name.name. <span class="li-normal">type: str</span> <span class="li-required">required: True</span></li>
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
        <li> <span class="li-head">internet_service_src_name</span> - Internet Service source name. <span class="li-normal">type: list</span></li>
            <ul class="ul-self">
            <li> <span class="li-head">name</span> - Internet Service name. Source firewall.internet-service-name.name. <span class="li-normal">type: str</span> <span class="li-required">required: True</span></li>
            </ul>
        <li> <span class="li-head">internet_service_src_negate</span> - When enabled internet-service-src specifies what the service must NOT be. <span class="li-normal">type: str</span> <span class="li-normal">choices: enable, disable</span></li>
        <li> <span class="li-head">ippool</span> - Enable to use IP Pools for source NAT. <span class="li-normal">type: str</span> <span class="li-normal">choices: enable, disable</span></li>
        <li> <span class="li-head">ips_sensor</span> - Name of an existing IPS sensor. Source ips.sensor.name. <span class="li-normal">type: str</span></li>
        <li> <span class="li-head">logtraffic</span> - Enable or disable logging. Log all sessions or security profile sessions. <span class="li-normal">type: str</span> <span class="li-normal">choices: all, utm, disable</span></li>
        <li> <span class="li-head">logtraffic_start</span> - Record logs when a session starts. <span class="li-normal">type: str</span> <span class="li-normal">choices: enable, disable</span></li>
        <li> <span class="li-head">name</span> - Policy name. <span class="li-normal">type: str</span></li>
        <li> <span class="li-head">nat</span> - Enable/disable source NAT. <span class="li-normal">type: str</span> <span class="li-normal">choices: enable, disable</span></li>
        <li> <span class="li-head">outbound</span> - Policy-based IPsec VPN: only traffic from the internal network can initiate a VPN. <span class="li-normal">type: str</span> <span class="li-normal">choices: enable, disable</span></li>
        <li> <span class="li-head">per_ip_shaper</span> - Per-IP traffic shaper. Source firewall.shaper.per-ip-shaper.name. <span class="li-normal">type: str</span></li>
        <li> <span class="li-head">policyid</span> - Policy ID (0 - 4294967294). <span class="li-normal">type: int</span> <span class="li-required">required: True</span></li>
        <li> <span class="li-head">poolname4</span> - IPv4 pool names. <span class="li-normal">type: list</span></li>
            <ul class="ul-self">
            <li> <span class="li-head">name</span> - IPv4 pool name. Source firewall.ippool.name. <span class="li-normal">type: str</span> <span class="li-required">required: True</span></li>
            </ul>
        <li> <span class="li-head">poolname6</span> - IPv6 pool names. <span class="li-normal">type: list</span></li>
            <ul class="ul-self">
            <li> <span class="li-head">name</span> - IPv6 pool name. Source firewall.ippool6.name. <span class="li-normal">type: str</span> <span class="li-required">required: True</span></li>
            </ul>
        <li> <span class="li-head">profile_group</span> - Name of profile group. Source firewall.profile-group.name. <span class="li-normal">type: str</span></li>
        <li> <span class="li-head">profile_protocol_options</span> - Name of an existing Protocol options profile. Source firewall.profile-protocol-options.name. <span class="li-normal">type: str</span></li>
        <li> <span class="li-head">profile_type</span> - Determine whether the firewall policy allows security profile groups or single profiles only. <span class="li-normal">type: str</span> <span class="li-normal">choices: single, group</span></li>
        <li> <span class="li-head">schedule</span> - Schedule name. Source firewall.schedule.onetime.name firewall.schedule.recurring.name firewall.schedule.group.name. <span class="li-normal">type: str</span></li>
        <li> <span class="li-head">service</span> - Service and service group names. <span class="li-normal">type: list</span></li>
            <ul class="ul-self">
            <li> <span class="li-head">name</span> - Service name. Source firewall.service.custom.name firewall.service.group.name. <span class="li-normal">type: str</span> <span class="li-required">required: True</span></li>
            </ul>
        <li> <span class="li-head">service_negate</span> - When enabled service specifies what the service must NOT be. <span class="li-normal">type: str</span> <span class="li-normal">choices: enable, disable</span></li>
        <li> <span class="li-head">session_ttl</span> - TTL in seconds for sessions accepted by this policy (0 means use the system ). <span class="li-normal">type: int</span></li>
        <li> <span class="li-head">srcaddr_negate</span> - When enabled srcaddr specifies what the source address must NOT be. <span class="li-normal">type: str</span> <span class="li-normal">choices: enable, disable</span></li>
        <li> <span class="li-head">srcaddr4</span> - Source IPv4 address name and address group names. <span class="li-normal">type: list</span></li>
            <ul class="ul-self">
            <li> <span class="li-head">name</span> - Address name. Source firewall.address.name firewall.addrgrp.name system.external-resource.name. <span class="li-normal">type: str</span> <span class="li-required">required: True</span></li>
            </ul>
        <li> <span class="li-head">srcaddr6</span> - Source IPv6 address name and address group names. <span class="li-normal">type: list</span></li>
            <ul class="ul-self">
            <li> <span class="li-head">name</span> - Address name. Source firewall.address6.name firewall.addrgrp6.name system.external-resource.name. <span class="li-normal">type: str</span> <span class="li-required">required: True</span></li>
            </ul>
        <li> <span class="li-head">srcintf</span> - Incoming (ingress) interface. <span class="li-normal">type: list</span></li>
            <ul class="ul-self">
            <li> <span class="li-head">name</span> - Interface name. Source system.interface.name system.zone.name. <span class="li-normal">type: str</span> <span class="li-required">required: True</span></li>
            </ul>
        <li> <span class="li-head">ssh_filter_profile</span> - Name of an existing SSH filter profile. Source ssh-filter.profile.name. <span class="li-normal">type: str</span></li>
        <li> <span class="li-head">ssh_policy_redirect</span> - Redirect SSH traffic to matching transparent proxy policy. <span class="li-normal">type: str</span> <span class="li-normal">choices: enable, disable</span></li>
        <li> <span class="li-head">ssl_ssh_profile</span> - Name of an existing SSL SSH profile. Source firewall.ssl-ssh-profile.name. <span class="li-normal">type: str</span></li>
        <li> <span class="li-head">status</span> - Enable or disable this policy. <span class="li-normal">type: str</span> <span class="li-normal">choices: enable, disable</span></li>
        <li> <span class="li-head">tcp_mss_receiver</span> - Receiver TCP maximum segment size (MSS). <span class="li-normal">type: int</span></li>
        <li> <span class="li-head">tcp_mss_sender</span> - Sender TCP maximum segment size (MSS). <span class="li-normal">type: int</span></li>
        <li> <span class="li-head">traffic_shaper</span> - Traffic shaper. Source firewall.shaper.traffic-shaper.name. <span class="li-normal">type: str</span></li>
        <li> <span class="li-head">traffic_shaper_reverse</span> - Reverse traffic shaper. Source firewall.shaper.traffic-shaper.name. <span class="li-normal">type: str</span></li>
        <li> <span class="li-head">users</span> - Names of individual users that can authenticate with this policy. <span class="li-normal">type: list</span></li>
            <ul class="ul-self">
            <li> <span class="li-head">name</span> - User name. Source user.local.name. <span class="li-normal">type: str</span> <span class="li-required">required: True</span></li>
            </ul>
        <li> <span class="li-head">utm_status</span> - Enable to add one or more security profiles (AV, IPS, etc.) to the firewall policy. <span class="li-normal">type: str</span> <span class="li-normal">choices: enable, disable</span></li>
        <li> <span class="li-head">uuid</span> - Universally Unique Identifier (UUID; automatically assigned but can be manually reset). <span class="li-normal">type: str</span></li>
        <li> <span class="li-head">voip_profile</span> - Name of an existing VoIP profile. Source voip.profile.name. <span class="li-normal">type: str</span></li>
        <li> <span class="li-head">vpntunnel</span> - Policy-based IPsec VPN: name of the IPsec VPN Phase 1. Source vpn.ipsec.phase1.name vpn.ipsec.manualkey.name. <span class="li-normal">type: str</span></li>
        <li> <span class="li-head">waf_profile</span> - Name of an existing Web application firewall profile. Source waf.profile.name. <span class="li-normal">type: str</span></li>
        <li> <span class="li-head">wanopt</span> - Enable/disable WAN optimization. <span class="li-normal">type: str</span> <span class="li-normal">choices: enable, disable</span></li>
        <li> <span class="li-head">wanopt_detection</span> - WAN optimization auto-detection mode. <span class="li-normal">type: str</span> <span class="li-normal">choices: active, passive, False</span></li>
        <li> <span class="li-head">wanopt_passive_opt</span> - WAN optimization passive mode options. This option decides what IP address will be used to connect to server. <span class="li-normal">type: str</span> <span class="li-normal">choices: default, transparent, non-transparent</span></li>
        <li> <span class="li-head">wanopt_peer</span> - WAN optimization peer. Source wanopt.peer.peer-host-id. <span class="li-normal">type: str</span></li>
        <li> <span class="li-head">wanopt_profile</span> - WAN optimization profile. Source wanopt.profile.name. <span class="li-normal">type: str</span></li>
        <li> <span class="li-head">webcache</span> - Enable/disable web cache. <span class="li-normal">type: str</span> <span class="li-normal">choices: enable, disable</span></li>
        <li> <span class="li-head">webcache_https</span> - Enable/disable web cache for HTTPS. <span class="li-normal">type: str</span> <span class="li-normal">choices: disable, enable</span></li>
        <li> <span class="li-head">webfilter_profile</span> - Name of an existing Web filter profile. Source webfilter.profile.name. <span class="li-normal">type: str</span></li>
        <li> <span class="li-head">webproxy_forward_server</span> - Webproxy forward server name. Source web-proxy.forward-server.name web-proxy.forward-server-group.name. <span class="li-normal">type: str</span></li>
        <li> <span class="li-head">webproxy_profile</span> - Webproxy profile name. Source web-proxy.profile.name. <span class="li-normal">type: str</span></li>
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
      - name: Configure consolidated IPv4/IPv6 policies.
        fortios_firewall_consolidated_policy:
          vdom:  "{{ vdom }}"
          state: "present"
          firewall_consolidated_policy:
            action: "accept"
            application_list: "<your_own_value> (source application.list.name)"
            auto_asic_offload: "enable"
            av_profile: "<your_own_value> (source antivirus.profile.name)"
            captive_portal_exempt: "enable"
            cifs_profile: "<your_own_value> (source cifs.profile.name)"
            comments: "<your_own_value>"
            diffserv_forward: "enable"
            diffserv_reverse: "enable"
            diffservcode_forward: "<your_own_value>"
            diffservcode_rev: "<your_own_value>"
            dlp_sensor: "<your_own_value> (source dlp.sensor.name)"
            dnsfilter_profile: "<your_own_value> (source dnsfilter.profile.name)"
            dstaddr_negate: "enable"
            dstaddr4:
             -
                name: "default_name_18 (source firewall.address.name firewall.addrgrp.name firewall.vip.name firewall.vipgrp.name system.external-resource.name)"
            dstaddr6:
             -
                name: "default_name_20 (source firewall.address6.name firewall.addrgrp6.name firewall.vip6.name firewall.vipgrp6.name system.external-resource
                  .name)"
            dstintf:
             -
                name: "default_name_22 (source system.interface.name system.zone.name)"
            emailfilter_profile: "<your_own_value> (source emailfilter.profile.name)"
            fixedport: "enable"
            fsso_groups:
             -
                name: "default_name_26 (source user.adgrp.name)"
            groups:
             -
                name: "default_name_28 (source user.group.name)"
            http_policy_redirect: "enable"
            icap_profile: "<your_own_value> (source icap.profile.name)"
            inbound: "enable"
            inspection_mode: "proxy"
            internet_service: "enable"
            internet_service_custom:
             -
                name: "default_name_35 (source firewall.internet-service-custom.name)"
            internet_service_custom_group:
             -
                name: "default_name_37 (source firewall.internet-service-custom-group.name)"
            internet_service_group:
             -
                name: "default_name_39 (source firewall.internet-service-group.name)"
            internet_service_name:
             -
                name: "default_name_41 (source firewall.internet-service-name.name)"
            internet_service_negate: "enable"
            internet_service_src: "enable"
            internet_service_src_custom:
             -
                name: "default_name_45 (source firewall.internet-service-custom.name)"
            internet_service_src_custom_group:
             -
                name: "default_name_47 (source firewall.internet-service-custom-group.name)"
            internet_service_src_group:
             -
                name: "default_name_49 (source firewall.internet-service-group.name)"
            internet_service_src_name:
             -
                name: "default_name_51 (source firewall.internet-service-name.name)"
            internet_service_src_negate: "enable"
            ippool: "enable"
            ips_sensor: "<your_own_value> (source ips.sensor.name)"
            logtraffic: "all"
            logtraffic_start: "enable"
            name: "default_name_57"
            nat: "enable"
            outbound: "enable"
            per_ip_shaper: "<your_own_value> (source firewall.shaper.per-ip-shaper.name)"
            policyid: "61"
            poolname4:
             -
                name: "default_name_63 (source firewall.ippool.name)"
            poolname6:
             -
                name: "default_name_65 (source firewall.ippool6.name)"
            profile_group: "<your_own_value> (source firewall.profile-group.name)"
            profile_protocol_options: "<your_own_value> (source firewall.profile-protocol-options.name)"
            profile_type: "single"
            schedule: "<your_own_value> (source firewall.schedule.onetime.name firewall.schedule.recurring.name firewall.schedule.group.name)"
            service:
             -
                name: "default_name_71 (source firewall.service.custom.name firewall.service.group.name)"
            service_negate: "enable"
            session_ttl: "73"
            srcaddr_negate: "enable"
            srcaddr4:
             -
                name: "default_name_76 (source firewall.address.name firewall.addrgrp.name system.external-resource.name)"
            srcaddr6:
             -
                name: "default_name_78 (source firewall.address6.name firewall.addrgrp6.name system.external-resource.name)"
            srcintf:
             -
                name: "default_name_80 (source system.interface.name system.zone.name)"
            ssh_filter_profile: "<your_own_value> (source ssh-filter.profile.name)"
            ssh_policy_redirect: "enable"
            ssl_ssh_profile: "<your_own_value> (source firewall.ssl-ssh-profile.name)"
            status: "enable"
            tcp_mss_receiver: "85"
            tcp_mss_sender: "86"
            traffic_shaper: "<your_own_value> (source firewall.shaper.traffic-shaper.name)"
            traffic_shaper_reverse: "<your_own_value> (source firewall.shaper.traffic-shaper.name)"
            users:
             -
                name: "default_name_90 (source user.local.name)"
            utm_status: "enable"
            uuid: "<your_own_value>"
            voip_profile: "<your_own_value> (source voip.profile.name)"
            vpntunnel: "<your_own_value> (source vpn.ipsec.phase1.name vpn.ipsec.manualkey.name)"
            waf_profile: "<your_own_value> (source waf.profile.name)"
            wanopt: "enable"
            wanopt_detection: "active"
            wanopt_passive_opt: "default"
            wanopt_peer: "<your_own_value> (source wanopt.peer.peer-host-id)"
            wanopt_profile: "<your_own_value> (source wanopt.profile.name)"
            webcache: "enable"
            webcache_https: "disable"
            webfilter_profile: "<your_own_value> (source webfilter.profile.name)"
            webproxy_forward_server: "<your_own_value> (source web-proxy.forward-server.name web-proxy.forward-server-group.name)"
            webproxy_profile: "<your_own_value> (source web-proxy.profile.name)"


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
