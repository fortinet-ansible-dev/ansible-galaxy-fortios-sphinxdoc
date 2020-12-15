:source: fortios_configuration_fact.py

:orphan:

.. :

fortios_configuration_fact -- Retrieve Facts of FortiOS Configurable Objects.
++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++

.. versionadded:: 2.10

.. contents::
   :local:
   :depth: 1


Synopsis
--------
- Collects facts from network devices running the fortios operating system. This module places the facts gathered in the fact tree keyed by the respective resource name.  This facts module will only collect those facts which user specified in playbook.



Requirements
------------
The below requirements are needed on the host that executes this module.

- install galaxy collection fortinet.fortios 


Parameters
----------


.. raw:: html

    <ul>
    <li> <span class="li-head">vdom</span> - Virtual domain, among those defined previously. A vdom is a virtual instance of the FortiGate that can be configured and used as a different unit. <span class="li-normal">type: str</span> <span class="li-required">required: False</span> <span class="li-normal">default: root</span></li>
    <li> <span class="li-head">access_token</span> - Token-based authentication. Generated from GUI of Fortigate. <span class="li-normal">type: str</span> <span class="li-required">required: False</span> </li>
    <li><span class="li-head">selector</span> - selector of the retrieved fortimanager facts <span class="li-normal">type: str</span> <span class="li-required">choices:</span></li>
        <li style="list-style: none;"><section class="accordion">
        <input type="checkbox" name="collapse" id="handle2">
        <h2 class="handle">
            <label for="handle2"><u>Show full selector list...</u></label>
        </h2>
        <div class="content">
        <ul class="ul-self">
        
            <li><span class="li-normal">log_gui-display</span> </li>
          
            <li><span class="li-normal">log.fortianalyzer_override-setting</span> </li>
          
            <li><span class="li-normal">firewall.ssl_setting</span> </li>
          
            <li><span class="li-normal">vpn.ipsec_phase2-interface</span>  <span class="li-required">param: name</span>  <span class="li-required">type: str</span></li>
          
            <li><span class="li-normal">router_key-chain</span>  <span class="li-required">param: name</span>  <span class="li-required">type: str</span></li>
          
            <li><span class="li-normal">system_ddns</span>  <span class="li-required">param: ddnsid</span>  <span class="li-required">type: int</span></li>
          
            <li><span class="li-normal">system_replacemsg-group</span>  <span class="li-required">param: name</span>  <span class="li-required">type: str</span></li>
          
            <li><span class="li-normal">system_ftm-push</span> </li>
          
            <li><span class="li-normal">system_sms-server</span>  <span class="li-required">param: name</span>  <span class="li-required">type: str</span></li>
          
            <li><span class="li-normal">firewall_central-snat-map</span>  <span class="li-required">param: policyid</span>  <span class="li-required">type: int</span></li>
          
            <li><span class="li-normal">firewall_multicast-address6</span>  <span class="li-required">param: name</span>  <span class="li-required">type: str</span></li>
          
            <li><span class="li-normal">system.replacemsg_sslvpn</span>  <span class="li-required">param: msg_type</span>  <span class="li-required">type: str</span></li>
          
            <li><span class="li-normal">system_pppoe-interface</span>  <span class="li-required">param: name</span>  <span class="li-required">type: str</span></li>
          
            <li><span class="li-normal">firewall_addrgrp6</span>  <span class="li-required">param: name</span>  <span class="li-required">type: str</span></li>
          
            <li><span class="li-normal">log.disk_filter</span> </li>
          
            <li><span class="li-normal">system_affinity-packet-redistribution</span>  <span class="li-required">param: id</span>  <span class="li-required">type: int</span></li>
          
            <li><span class="li-normal">firewall_proxy-address</span>  <span class="li-required">param: name</span>  <span class="li-required">type: str</span></li>
          
            <li><span class="li-normal">authentication_rule</span>  <span class="li-required">param: name</span>  <span class="li-required">type: str</span></li>
          
            <li><span class="li-normal">router_bfd</span> </li>
          
            <li><span class="li-normal">switch-controller_custom-command</span>  <span class="li-required">param: command_name</span>  <span class="li-required">type: str</span></li>
          
            <li><span class="li-normal">system_resource-limits</span> </li>
          
            <li><span class="li-normal">system.replacemsg_auth</span>  <span class="li-required">param: msg_type</span>  <span class="li-required">type: str</span></li>
          
            <li><span class="li-normal">system.autoupdate_schedule</span> </li>
          
            <li><span class="li-normal">waf_sub-class</span>  <span class="li-required">param: id</span>  <span class="li-required">type: int</span></li>
          
            <li><span class="li-normal">firewall_local-in-policy6</span>  <span class="li-required">param: policyid</span>  <span class="li-required">type: int</span></li>
          
            <li><span class="li-normal">log.fortianalyzer_override-filter</span> </li>
          
            <li><span class="li-normal">system.replacemsg_icap</span>  <span class="li-required">param: msg_type</span>  <span class="li-required">type: str</span></li>
          
            <li><span class="li-normal">system_object-tagging</span>  <span class="li-required">param: category</span>  <span class="li-required">type: str</span></li>
          
            <li><span class="li-normal">spamfilter_profile</span>  <span class="li-required">param: name</span>  <span class="li-required">type: str</span></li>
          
            <li><span class="li-normal">spamfilter_bwl</span>  <span class="li-required">param: id</span>  <span class="li-required">type: int</span></li>
          
            <li><span class="li-normal">web-proxy_profile</span>  <span class="li-required">param: name</span>  <span class="li-required">type: str</span></li>
          
            <li><span class="li-normal">spamfilter_mheader</span>  <span class="li-required">param: id</span>  <span class="li-required">type: int</span></li>
          
            <li><span class="li-normal">router_route-map</span>  <span class="li-required">param: name</span>  <span class="li-required">type: str</span></li>
          
            <li><span class="li-normal">user_adgrp</span>  <span class="li-required">param: name</span>  <span class="li-required">type: str</span></li>
          
            <li><span class="li-normal">system_auto-script</span>  <span class="li-required">param: name</span>  <span class="li-required">type: str</span></li>
          
            <li><span class="li-normal">switch-controller_quarantine</span> </li>
          
            <li><span class="li-normal">firewall.service_category</span>  <span class="li-required">param: name</span>  <span class="li-required">type: str</span></li>
          
            <li><span class="li-normal">system_link-monitor</span>  <span class="li-required">param: name</span>  <span class="li-required">type: str</span></li>
          
            <li><span class="li-normal">switch-controller_stp-settings</span> </li>
          
            <li><span class="li-normal">user_security-exempt-list</span>  <span class="li-required">param: name</span>  <span class="li-required">type: str</span></li>
          
            <li><span class="li-normal">firewall_sniffer</span>  <span class="li-required">param: id</span>  <span class="li-required">type: int</span></li>
          
            <li><span class="li-normal">log.fortiguard_override-setting</span> </li>
          
            <li><span class="li-normal">firewall_internet-service</span>  <span class="li-required">param: id</span>  <span class="li-required">type: int</span></li>
          
            <li><span class="li-normal">firewall_vipgrp46</span>  <span class="li-required">param: name</span>  <span class="li-required">type: str</span></li>
          
            <li><span class="li-normal">log.webtrends_filter</span> </li>
          
            <li><span class="li-normal">webfilter_ips-urlfilter-setting6</span> </li>
          
            <li><span class="li-normal">router_prefix-list6</span>  <span class="li-required">param: name</span>  <span class="li-required">type: str</span></li>
          
            <li><span class="li-normal">log_setting</span> </li>
          
            <li><span class="li-normal">firewall_address6-template</span>  <span class="li-required">param: name</span>  <span class="li-required">type: str</span></li>
          
            <li><span class="li-normal">wireless-controller.hotspot20_h2qp-wan-metric</span>  <span class="li-required">param: name</span>  <span class="li-required">type: str</span></li>
          
            <li><span class="li-normal">system_automation-action</span>  <span class="li-required">param: name</span>  <span class="li-required">type: str</span></li>
          
            <li><span class="li-normal">system.autoupdate_tunneling</span> </li>
          
            <li><span class="li-normal">webfilter_ips-urlfilter-setting</span> </li>
          
            <li><span class="li-normal">switch-controller_network-monitor-settings</span> </li>
          
            <li><span class="li-normal">system_alias</span>  <span class="li-required">param: name</span>  <span class="li-required">type: str</span></li>
          
            <li><span class="li-normal">switch-controller_mac-sync-settings</span> </li>
          
            <li><span class="li-normal">web-proxy_forward-server-group</span>  <span class="li-required">param: name</span>  <span class="li-required">type: str</span></li>
          
            <li><span class="li-normal">system_session-helper</span>  <span class="li-required">param: id</span>  <span class="li-required">type: int</span></li>
          
            <li><span class="li-normal">router_community-list</span>  <span class="li-required">param: name</span>  <span class="li-required">type: str</span></li>
          
            <li><span class="li-normal">wireless-controller_qos-profile</span>  <span class="li-required">param: name</span>  <span class="li-required">type: str</span></li>
          
            <li><span class="li-normal">firewall_dnstranslation</span>  <span class="li-required">param: id</span>  <span class="li-required">type: int</span></li>
          
            <li><span class="li-normal">vpn.ssl.web_portal</span>  <span class="li-required">param: name</span>  <span class="li-required">type: str</span></li>
          
            <li><span class="li-normal">system_vdom-property</span>  <span class="li-required">param: name</span>  <span class="li-required">type: str</span></li>
          
            <li><span class="li-normal">system.replacemsg_device-detection-portal</span>  <span class="li-required">param: msg_type</span>  <span class="li-required">type: str</span></li>
          
            <li><span class="li-normal">log.syslogd2_setting</span> </li>
          
            <li><span class="li-normal">firewall_internet-service-custom-group</span>  <span class="li-required">param: name</span>  <span class="li-required">type: str</span></li>
          
            <li><span class="li-normal">firewall_profile-group</span>  <span class="li-required">param: name</span>  <span class="li-required">type: str</span></li>
          
            <li><span class="li-normal">firewall.service_group</span>  <span class="li-required">param: name</span>  <span class="li-required">type: str</span></li>
          
            <li><span class="li-normal">system.autoupdate_push-update</span> </li>
          
            <li><span class="li-normal">firewall_address6</span>  <span class="li-required">param: name</span>  <span class="li-required">type: str</span></li>
          
            <li><span class="li-normal">endpoint-control_profile</span>  <span class="li-required">param: profile_name</span>  <span class="li-required">type: str</span></li>
          
            <li><span class="li-normal">wireless-controller_wids-profile</span>  <span class="li-required">param: name</span>  <span class="li-required">type: str</span></li>
          
            <li><span class="li-normal">log.fortiguard_filter</span> </li>
          
            <li><span class="li-normal">firewall_ipv6-eh-filter</span> </li>
          
            <li><span class="li-normal">user_device-category</span>  <span class="li-required">param: name</span>  <span class="li-required">type: str</span></li>
          
            <li><span class="li-normal">firewall_identity-based-route</span>  <span class="li-required">param: name</span>  <span class="li-required">type: str</span></li>
          
            <li><span class="li-normal">system_console</span> </li>
          
            <li><span class="li-normal">system_ntp</span> </li>
          
            <li><span class="li-normal">router_bgp</span> </li>
          
            <li><span class="li-normal">system_nat64</span> </li>
          
            <li><span class="li-normal">system.3g-modem_custom</span>  <span class="li-required">param: id</span>  <span class="li-required">type: int</span></li>
          
            <li><span class="li-normal">report_layout</span>  <span class="li-required">param: name</span>  <span class="li-required">type: str</span></li>
          
            <li><span class="li-normal">wireless-controller_timers</span> </li>
          
            <li><span class="li-normal">wireless-controller.hotspot20_icon</span>  <span class="li-required">param: name</span>  <span class="li-required">type: str</span></li>
          
            <li><span class="li-normal">log.memory_global-setting</span> </li>
          
            <li><span class="li-normal">router_multicast-flow</span>  <span class="li-required">param: name</span>  <span class="li-required">type: str</span></li>
          
            <li><span class="li-normal">ssh-filter_profile</span>  <span class="li-required">param: name</span>  <span class="li-required">type: str</span></li>
          
            <li><span class="li-normal">system_fortisandbox</span> </li>
          
            <li><span class="li-normal">system_virtual-wan-link</span> </li>
          
            <li><span class="li-normal">ips_sensor</span>  <span class="li-required">param: name</span>  <span class="li-required">type: str</span></li>
          
            <li><span class="li-normal">firewall.wildcard-fqdn_custom</span>  <span class="li-required">param: name</span>  <span class="li-required">type: str</span></li>
          
            <li><span class="li-normal">router_static</span>  <span class="li-required">param: seq_num</span>  <span class="li-required">type: int</span></li>
          
            <li><span class="li-normal">alertemail_setting</span> </li>
          
            <li><span class="li-normal">router_policy</span>  <span class="li-required">param: seq_num</span>  <span class="li-required">type: int</span></li>
          
            <li><span class="li-normal">user_fortitoken</span>  <span class="li-required">param: serial_number</span>  <span class="li-required">type: str</span></li>
          
            <li><span class="li-normal">web-proxy_debug-url</span>  <span class="li-required">param: name</span>  <span class="li-required">type: str</span></li>
          
            <li><span class="li-normal">webfilter_override</span>  <span class="li-required">param: id</span>  <span class="li-required">type: int</span></li>
          
            <li><span class="li-normal">system_fsso-polling</span> </li>
          
            <li><span class="li-normal">user_peer</span>  <span class="li-required">param: name</span>  <span class="li-required">type: str</span></li>
          
            <li><span class="li-normal">vpn.ssl.web_host-check-software</span>  <span class="li-required">param: name</span>  <span class="li-required">type: str</span></li>
          
            <li><span class="li-normal">switch-controller_lldp-profile</span>  <span class="li-required">param: name</span>  <span class="li-required">type: str</span></li>
          
            <li><span class="li-normal">vpn.ssl.web_realm</span>  <span class="li-required">param: url_path</span>  <span class="li-required">type: str</span></li>
          
            <li><span class="li-normal">system_stp</span> </li>
          
            <li><span class="li-normal">switch-controller.security-policy_captive-portal</span>  <span class="li-required">param: name</span>  <span class="li-required">type: str</span></li>
          
            <li><span class="li-normal">firewall_shaping-policy</span>  <span class="li-required">param: id</span>  <span class="li-required">type: int</span></li>
          
            <li><span class="li-normal">log_custom-field</span>  <span class="li-required">param: id</span>  <span class="li-required">type: str</span></li>
          
            <li><span class="li-normal">firewall_address</span>  <span class="li-required">param: name</span>  <span class="li-required">type: str</span></li>
          
            <li><span class="li-normal">certificate_crl</span>  <span class="li-required">param: name</span>  <span class="li-required">type: str</span></li>
          
            <li><span class="li-normal">firewall.ssh_setting</span> </li>
          
            <li><span class="li-normal">router_access-list</span>  <span class="li-required">param: name</span>  <span class="li-required">type: str</span></li>
          
            <li><span class="li-normal">log.memory_setting</span> </li>
          
            <li><span class="li-normal">system_alarm</span> </li>
          
            <li><span class="li-normal">system_ipv6-neighbor-cache</span>  <span class="li-required">param: id</span>  <span class="li-required">type: int</span></li>
          
            <li><span class="li-normal">system_cluster-sync</span>  <span class="li-required">param: sync_id</span>  <span class="li-required">type: int</span></li>
          
            <li><span class="li-normal">wanopt_settings</span> </li>
          
            <li><span class="li-normal">endpoint-control_registered-forticlient</span>  <span class="li-required">param: uid</span>  <span class="li-required">type: str</span></li>
          
            <li><span class="li-normal">system_dedicated-mgmt</span> </li>
          
            <li><span class="li-normal">firewall_policy46</span>  <span class="li-required">param: policyid</span>  <span class="li-required">type: int</span></li>
          
            <li><span class="li-normal">antivirus_settings</span> </li>
          
            <li><span class="li-normal">switch-controller_802-1X-settings</span> </li>
          
            <li><span class="li-normal">system_session-ttl</span> </li>
          
            <li><span class="li-normal">system_storage</span>  <span class="li-required">param: name</span>  <span class="li-required">type: str</span></li>
          
            <li><span class="li-normal">log.memory_filter</span> </li>
          
            <li><span class="li-normal">firewall_auth-portal</span> </li>
          
            <li><span class="li-normal">system_sflow</span> </li>
          
            <li><span class="li-normal">user_ldap</span>  <span class="li-required">param: name</span>  <span class="li-required">type: str</span></li>
          
            <li><span class="li-normal">ips_global</span> </li>
          
            <li><span class="li-normal">wanopt_remote-storage</span> </li>
          
            <li><span class="li-normal">wireless-controller.hotspot20_qos-map</span>  <span class="li-required">param: name</span>  <span class="li-required">type: str</span></li>
          
            <li><span class="li-normal">vpn_l2tp</span> </li>
          
            <li><span class="li-normal">firewall_vip46</span>  <span class="li-required">param: name</span>  <span class="li-required">type: str</span></li>
          
            <li><span class="li-normal">authentication_setting</span> </li>
          
            <li><span class="li-normal">vpn.certificate_ocsp-server</span>  <span class="li-required">param: name</span>  <span class="li-required">type: str</span></li>
          
            <li><span class="li-normal">antivirus_heuristic</span> </li>
          
            <li><span class="li-normal">spamfilter_bword</span>  <span class="li-required">param: id</span>  <span class="li-required">type: int</span></li>
          
            <li><span class="li-normal">system_custom-language</span>  <span class="li-required">param: name</span>  <span class="li-required">type: str</span></li>
          
            <li><span class="li-normal">web-proxy_explicit</span> </li>
          
            <li><span class="li-normal">wireless-controller_wtp-group</span>  <span class="li-required">param: name</span>  <span class="li-required">type: str</span></li>
          
            <li><span class="li-normal">system_vdom-sflow</span> </li>
          
            <li><span class="li-normal">switch-controller_igmp-snooping</span> </li>
          
            <li><span class="li-normal">waf_signature</span>  <span class="li-required">param: id</span>  <span class="li-required">type: int</span></li>
          
            <li><span class="li-normal">log.null-device_setting</span> </li>
          
            <li><span class="li-normal">ips_rule-settings</span>  <span class="li-required">param: id</span>  <span class="li-required">type: int</span></li>
          
            <li><span class="li-normal">log.syslogd_setting</span> </li>
          
            <li><span class="li-normal">switch-controller.security-policy_802-1X</span>  <span class="li-required">param: name</span>  <span class="li-required">type: str</span></li>
          
            <li><span class="li-normal">report_setting</span> </li>
          
            <li><span class="li-normal">user_setting</span> </li>
          
            <li><span class="li-normal">icap_profile</span>  <span class="li-required">param: name</span>  <span class="li-required">type: str</span></li>
          
            <li><span class="li-normal">system_geoip-override</span>  <span class="li-required">param: name</span>  <span class="li-required">type: str</span></li>
          
            <li><span class="li-normal">vpn.ipsec_phase1</span>  <span class="li-required">param: name</span>  <span class="li-required">type: str</span></li>
          
            <li><span class="li-normal">vpn.ipsec_phase2</span>  <span class="li-required">param: name</span>  <span class="li-required">type: str</span></li>
          
            <li><span class="li-normal">wireless-controller.hotspot20_anqp-network-auth-type</span>  <span class="li-required">param: name</span>  <span class="li-required">type: str</span></li>
          
            <li><span class="li-normal">webfilter_ips-urlfilter-cache-setting</span> </li>
          
            <li><span class="li-normal">firewall.ipmacbinding_setting</span> </li>
          
            <li><span class="li-normal">log.fortianalyzer2_filter</span> </li>
          
            <li><span class="li-normal">application_rule-settings</span>  <span class="li-required">param: id</span>  <span class="li-required">type: int</span></li>
          
            <li><span class="li-normal">log.syslogd4_filter</span> </li>
          
            <li><span class="li-normal">system_proxy-arp</span>  <span class="li-required">param: id</span>  <span class="li-required">type: int</span></li>
          
            <li><span class="li-normal">webfilter_ftgd-local-rating</span>  <span class="li-required">param: url</span>  <span class="li-required">type: str</span></li>
          
            <li><span class="li-normal">ips_custom</span>  <span class="li-required">param: tag</span>  <span class="li-required">type: str</span></li>
          
            <li><span class="li-normal">vpn_ocvpn</span> </li>
          
            <li><span class="li-normal">switch-controller_switch-interface-tag</span>  <span class="li-required">param: name</span>  <span class="li-required">type: str</span></li>
          
            <li><span class="li-normal">router_policy6</span>  <span class="li-required">param: seq_num</span>  <span class="li-required">type: int</span></li>
          
            <li><span class="li-normal">switch-controller.qos_ip-dscp-map</span>  <span class="li-required">param: name</span>  <span class="li-required">type: str</span></li>
          
            <li><span class="li-normal">log_eventfilter</span> </li>
          
            <li><span class="li-normal">firewall_internet-service-custom</span>  <span class="li-required">param: name</span>  <span class="li-required">type: str</span></li>
          
            <li><span class="li-normal">router_auth-path</span>  <span class="li-required">param: name</span>  <span class="li-required">type: str</span></li>
          
            <li><span class="li-normal">system_external-resource</span>  <span class="li-required">param: name</span>  <span class="li-required">type: str</span></li>
          
            <li><span class="li-normal">system_ips-urlfilter-dns6</span>  <span class="li-required">param: address6</span>  <span class="li-required">type: str</span></li>
          
            <li><span class="li-normal">report_style</span>  <span class="li-required">param: name</span>  <span class="li-required">type: str</span></li>
          
            <li><span class="li-normal">wireless-controller_wtp</span>  <span class="li-required">param: wtp_id</span>  <span class="li-required">type: str</span></li>
          
            <li><span class="li-normal">system_ipip-tunnel</span>  <span class="li-required">param: name</span>  <span class="li-required">type: str</span></li>
          
            <li><span class="li-normal">system.dhcp6_server</span>  <span class="li-required">param: id</span>  <span class="li-required">type: int</span></li>
          
            <li><span class="li-normal">firewall_multicast-policy</span>  <span class="li-required">param: id</span>  <span class="li-required">type: int</span></li>
          
            <li><span class="li-normal">system_modem</span> </li>
          
            <li><span class="li-normal">router_rip</span> </li>
          
            <li><span class="li-normal">system_password-policy</span> </li>
          
            <li><span class="li-normal">switch-controller_virtual-port-pool</span>  <span class="li-required">param: name</span>  <span class="li-required">type: str</span></li>
          
            <li><span class="li-normal">wireless-controller_setting</span> </li>
          
            <li><span class="li-normal">router_static6</span>  <span class="li-required">param: seq_num</span>  <span class="li-required">type: int</span></li>
          
            <li><span class="li-normal">wireless-controller.hotspot20_anqp-ip-address-type</span>  <span class="li-required">param: name</span>  <span class="li-required">type: str</span></li>
          
            <li><span class="li-normal">firewall_vipgrp</span>  <span class="li-required">param: name</span>  <span class="li-required">type: str</span></li>
          
            <li><span class="li-normal">switch-controller_switch-profile</span>  <span class="li-required">param: name</span>  <span class="li-required">type: str</span></li>
          
            <li><span class="li-normal">system_switch-interface</span>  <span class="li-required">param: name</span>  <span class="li-required">type: str</span></li>
          
            <li><span class="li-normal">router_isis</span> </li>
          
            <li><span class="li-normal">firewall_policy</span>  <span class="li-required">param: policyid</span>  <span class="li-required">type: int</span></li>
          
            <li><span class="li-normal">log.syslogd_override-setting</span> </li>
          
            <li><span class="li-normal">system_lte-modem</span> </li>
          
            <li><span class="li-normal">webfilter_content</span>  <span class="li-required">param: id</span>  <span class="li-required">type: int</span></li>
          
            <li><span class="li-normal">firewall_vipgrp6</span>  <span class="li-required">param: name</span>  <span class="li-required">type: str</span></li>
          
            <li><span class="li-normal">firewall.schedule_onetime</span>  <span class="li-required">param: name</span>  <span class="li-required">type: str</span></li>
          
            <li><span class="li-normal">antivirus_profile</span>  <span class="li-required">param: name</span>  <span class="li-required">type: str</span></li>
          
            <li><span class="li-normal">log.fortianalyzer_setting</span> </li>
          
            <li><span class="li-normal">firewall_ippool6</span>  <span class="li-required">param: name</span>  <span class="li-required">type: str</span></li>
          
            <li><span class="li-normal">system_central-management</span> </li>
          
            <li><span class="li-normal">system.replacemsg_http</span>  <span class="li-required">param: msg_type</span>  <span class="li-required">type: str</span></li>
          
            <li><span class="li-normal">system_zone</span>  <span class="li-required">param: name</span>  <span class="li-required">type: str</span></li>
          
            <li><span class="li-normal">system_vdom-dns</span> </li>
          
            <li><span class="li-normal">firewall_multicast-address</span>  <span class="li-required">param: name</span>  <span class="li-required">type: str</span></li>
          
            <li><span class="li-normal">wireless-controller_wtp-profile</span>  <span class="li-required">param: name</span>  <span class="li-required">type: str</span></li>
          
            <li><span class="li-normal">vpn.ssl_settings</span> </li>
          
            <li><span class="li-normal">router_ospf</span> </li>
          
            <li><span class="li-normal">switch-controller.qos_queue-policy</span>  <span class="li-required">param: name</span>  <span class="li-required">type: str</span></li>
          
            <li><span class="li-normal">ftp-proxy_explicit</span> </li>
          
            <li><span class="li-normal">user_device-group</span>  <span class="li-required">param: name</span>  <span class="li-required">type: str</span></li>
          
            <li><span class="li-normal">vpn.certificate_crl</span>  <span class="li-required">param: name</span>  <span class="li-required">type: str</span></li>
          
            <li><span class="li-normal">user_local</span>  <span class="li-required">param: name</span>  <span class="li-required">type: str</span></li>
          
            <li><span class="li-normal">webfilter_profile</span>  <span class="li-required">param: name</span>  <span class="li-required">type: str</span></li>
          
            <li><span class="li-normal">switch-controller_storm-control</span> </li>
          
            <li><span class="li-normal">firewall_ssl-ssh-profile</span>  <span class="li-required">param: name</span>  <span class="li-required">type: str</span></li>
          
            <li><span class="li-normal">log.disk_setting</span> </li>
          
            <li><span class="li-normal">dlp_filepattern</span>  <span class="li-required">param: id</span>  <span class="li-required">type: int</span></li>
          
            <li><span class="li-normal">firewall_ippool</span>  <span class="li-required">param: name</span>  <span class="li-required">type: str</span></li>
          
            <li><span class="li-normal">web-proxy_url-match</span>  <span class="li-required">param: name</span>  <span class="li-required">type: str</span></li>
          
            <li><span class="li-normal">dlp_fp-sensitivity</span>  <span class="li-required">param: name</span>  <span class="li-required">type: str</span></li>
          
            <li><span class="li-normal">system_interface</span>  <span class="li-required">param: name</span>  <span class="li-required">type: str</span></li>
          
            <li><span class="li-normal">system_virtual-wire-pair</span>  <span class="li-required">param: name</span>  <span class="li-required">type: str</span></li>
          
            <li><span class="li-normal">system.replacemsg_webproxy</span>  <span class="li-required">param: msg_type</span>  <span class="li-required">type: str</span></li>
          
            <li><span class="li-normal">user_password-policy</span>  <span class="li-required">param: name</span>  <span class="li-required">type: str</span></li>
          
            <li><span class="li-normal">switch-controller.qos_qos-policy</span>  <span class="li-required">param: name</span>  <span class="li-required">type: str</span></li>
          
            <li><span class="li-normal">wireless-controller_inter-controller</span> </li>
          
            <li><span class="li-normal">log.syslogd4_setting</span> </li>
          
            <li><span class="li-normal">switch-controller_switch-group</span>  <span class="li-required">param: name</span>  <span class="li-required">type: str</span></li>
          
            <li><span class="li-normal">user_fsso</span>  <span class="li-required">param: name</span>  <span class="li-required">type: str</span></li>
          
            <li><span class="li-normal">firewall_vipgrp64</span>  <span class="li-required">param: name</span>  <span class="li-required">type: str</span></li>
          
            <li><span class="li-normal">user_quarantine</span> </li>
          
            <li><span class="li-normal">system_ips-urlfilter-dns</span>  <span class="li-required">param: address</span>  <span class="li-required">type: str</span></li>
          
            <li><span class="li-normal">system_fm</span> </li>
          
            <li><span class="li-normal">system_global</span> </li>
          
            <li><span class="li-normal">wireless-controller.hotspot20_anqp-nai-realm</span>  <span class="li-required">param: name</span>  <span class="li-required">type: str</span></li>
          
            <li><span class="li-normal">system_physical-switch</span>  <span class="li-required">param: name</span>  <span class="li-required">type: str</span></li>
          
            <li><span class="li-normal">log.fortianalyzer3_setting</span> </li>
          
            <li><span class="li-normal">firewall_vip</span>  <span class="li-required">param: name</span>  <span class="li-required">type: str</span></li>
          
            <li><span class="li-normal">system_virtual-switch</span>  <span class="li-required">param: name</span>  <span class="li-required">type: str</span></li>
          
            <li><span class="li-normal">wanopt_auth-group</span>  <span class="li-required">param: name</span>  <span class="li-required">type: str</span></li>
          
            <li><span class="li-normal">wanopt_webcache</span> </li>
          
            <li><span class="li-normal">system.snmp_user</span>  <span class="li-required">param: name</span>  <span class="li-required">type: str</span></li>
          
            <li><span class="li-normal">firewall_ip-translation</span>  <span class="li-required">param: transid</span>  <span class="li-required">type: int</span></li>
          
            <li><span class="li-normal">system_settings</span> </li>
          
            <li><span class="li-normal">log.fortianalyzer2_setting</span> </li>
          
            <li><span class="li-normal">wireless-controller_vap</span>  <span class="li-required">param: name</span>  <span class="li-required">type: str</span></li>
          
            <li><span class="li-normal">wanopt_cache-service</span> </li>
          
            <li><span class="li-normal">switch-controller_switch-log</span> </li>
          
            <li><span class="li-normal">firewall_internet-service-group</span>  <span class="li-required">param: name</span>  <span class="li-required">type: str</span></li>
          
            <li><span class="li-normal">system.replacemsg_mail</span>  <span class="li-required">param: msg_type</span>  <span class="li-required">type: str</span></li>
          
            <li><span class="li-normal">system_replacemsg-image</span>  <span class="li-required">param: name</span>  <span class="li-required">type: str</span></li>
          
            <li><span class="li-normal">antivirus_quarantine</span> </li>
          
            <li><span class="li-normal">vpn.certificate_ca</span>  <span class="li-required">param: name</span>  <span class="li-required">type: str</span></li>
          
            <li><span class="li-normal">endpoint-control_forticlient-registration-sync</span>  <span class="li-required">param: peer_name</span>  <span class="li-required">type: str</span></li>
          
            <li><span class="li-normal">system_sdn-connector</span>  <span class="li-required">param: name</span>  <span class="li-required">type: str</span></li>
          
            <li><span class="li-normal">vpn.ssl.web_user-group-bookmark</span>  <span class="li-required">param: name</span>  <span class="li-required">type: str</span></li>
          
            <li><span class="li-normal">endpoint-control_settings</span> </li>
          
            <li><span class="li-normal">log.null-device_filter</span> </li>
          
            <li><span class="li-normal">dlp_settings</span> </li>
          
            <li><span class="li-normal">wireless-controller_utm-profile</span>  <span class="li-required">param: name</span>  <span class="li-required">type: str</span></li>
          
            <li><span class="li-normal">router_aspath-list</span>  <span class="li-required">param: name</span>  <span class="li-required">type: str</span></li>
          
            <li><span class="li-normal">firewall.schedule_group</span>  <span class="li-required">param: name</span>  <span class="li-required">type: str</span></li>
          
            <li><span class="li-normal">system_dscp-based-priority</span>  <span class="li-required">param: id</span>  <span class="li-required">type: int</span></li>
          
            <li><span class="li-normal">icap_server</span>  <span class="li-required">param: name</span>  <span class="li-required">type: str</span></li>
          
            <li><span class="li-normal">vpn.ipsec_phase1-interface</span>  <span class="li-required">param: name</span>  <span class="li-required">type: str</span></li>
          
            <li><span class="li-normal">authentication_scheme</span>  <span class="li-required">param: name</span>  <span class="li-required">type: str</span></li>
          
            <li><span class="li-normal">log.fortianalyzer3_filter</span> </li>
          
            <li><span class="li-normal">system_email-server</span> </li>
          
            <li><span class="li-normal">wireless-controller_ap-status</span>  <span class="li-required">param: id</span>  <span class="li-required">type: int</span></li>
          
            <li><span class="li-normal">application_list</span>  <span class="li-required">param: name</span>  <span class="li-required">type: str</span></li>
          
            <li><span class="li-normal">vpn.ssl.web_user-bookmark</span>  <span class="li-required">param: name</span>  <span class="li-required">type: str</span></li>
          
            <li><span class="li-normal">firewall.shaper_traffic-shaper</span>  <span class="li-required">param: name</span>  <span class="li-required">type: str</span></li>
          
            <li><span class="li-normal">system_management-tunnel</span> </li>
          
            <li><span class="li-normal">system_csf</span> </li>
          
            <li><span class="li-normal">firewall.shaper_per-ip-shaper</span>  <span class="li-required">param: name</span>  <span class="li-required">type: str</span></li>
          
            <li><span class="li-normal">dnsfilter_profile</span>  <span class="li-required">param: name</span>  <span class="li-required">type: str</span></li>
          
            <li><span class="li-normal">user_device-access-list</span>  <span class="li-required">param: name</span>  <span class="li-required">type: str</span></li>
          
            <li><span class="li-normal">system_ha-monitor</span> </li>
          
            <li><span class="li-normal">wireless-controller.hotspot20_anqp-venue-name</span>  <span class="li-required">param: name</span>  <span class="li-required">type: str</span></li>
          
            <li><span class="li-normal">system.snmp_sysinfo</span> </li>
          
            <li><span class="li-normal">application_custom</span>  <span class="li-required">param: tag</span>  <span class="li-required">type: str</span></li>
          
            <li><span class="li-normal">system_api-user</span>  <span class="li-required">param: name</span>  <span class="li-required">type: str</span></li>
          
            <li><span class="li-normal">ips_rule</span>  <span class="li-required">param: name</span>  <span class="li-required">type: str</span></li>
          
            <li><span class="li-normal">spamfilter_fortishield</span> </li>
          
            <li><span class="li-normal">system_npu</span> </li>
          
            <li><span class="li-normal">system_netflow</span> </li>
          
            <li><span class="li-normal">vpn.ipsec_forticlient</span>  <span class="li-required">param: realm</span>  <span class="li-required">type: str</span></li>
          
            <li><span class="li-normal">system_automation-trigger</span>  <span class="li-required">param: name</span>  <span class="li-required">type: str</span></li>
          
            <li><span class="li-normal">firewall_policy64</span>  <span class="li-required">param: policyid</span>  <span class="li-required">type: int</span></li>
          
            <li><span class="li-normal">wireless-controller.hotspot20_h2qp-osu-provider</span>  <span class="li-required">param: name</span>  <span class="li-required">type: str</span></li>
          
            <li><span class="li-normal">application_name</span>  <span class="li-required">param: name</span>  <span class="li-required">type: str</span></li>
          
            <li><span class="li-normal">firewall.service_custom</span>  <span class="li-required">param: name</span>  <span class="li-required">type: str</span></li>
          
            <li><span class="li-normal">spamfilter_iptrust</span>  <span class="li-required">param: id</span>  <span class="li-required">type: int</span></li>
          
            <li><span class="li-normal">system_mobile-tunnel</span>  <span class="li-required">param: name</span>  <span class="li-required">type: str</span></li>
          
            <li><span class="li-normal">firewall_ttl-policy</span>  <span class="li-required">param: id</span>  <span class="li-required">type: int</span></li>
          
            <li><span class="li-normal">system.replacemsg_utm</span>  <span class="li-required">param: msg_type</span>  <span class="li-required">type: str</span></li>
          
            <li><span class="li-normal">vpn_pptp</span> </li>
          
            <li><span class="li-normal">wireless-controller.hotspot20_hs-profile</span>  <span class="li-required">param: name</span>  <span class="li-required">type: str</span></li>
          
            <li><span class="li-normal">log.webtrends_setting</span> </li>
          
            <li><span class="li-normal">firewall_local-in-policy</span>  <span class="li-required">param: policyid</span>  <span class="li-required">type: int</span></li>
          
            <li><span class="li-normal">switch-controller.qos_dot1p-map</span>  <span class="li-required">param: name</span>  <span class="li-required">type: str</span></li>
          
            <li><span class="li-normal">firewall_multicast-policy6</span>  <span class="li-required">param: id</span>  <span class="li-required">type: int</span></li>
          
            <li><span class="li-normal">wanopt_content-delivery-network-rule</span>  <span class="li-required">param: name</span>  <span class="li-required">type: str</span></li>
          
            <li><span class="li-normal">system_dns-database</span>  <span class="li-required">param: name</span>  <span class="li-required">type: str</span></li>
          
            <li><span class="li-normal">waf_main-class</span>  <span class="li-required">param: id</span>  <span class="li-required">type: int</span></li>
          
            <li><span class="li-normal">system.replacemsg_nac-quar</span>  <span class="li-required">param: msg_type</span>  <span class="li-required">type: str</span></li>
          
            <li><span class="li-normal">system_vdom-radius-server</span>  <span class="li-required">param: name</span>  <span class="li-required">type: str</span></li>
          
            <li><span class="li-normal">system_vdom</span>  <span class="li-required">param: name</span>  <span class="li-required">type: str</span></li>
          
            <li><span class="li-normal">user_tacacs+</span>  <span class="li-required">param: name</span>  <span class="li-required">type: str</span></li>
          
            <li><span class="li-normal">wanopt_peer</span>  <span class="li-required">param: peer_host_id</span>  <span class="li-required">type: str</span></li>
          
            <li><span class="li-normal">log.syslogd3_setting</span> </li>
          
            <li><span class="li-normal">report_dataset</span>  <span class="li-required">param: name</span>  <span class="li-required">type: str</span></li>
          
            <li><span class="li-normal">webfilter_ftgd-local-cat</span>  <span class="li-required">param: desc</span>  <span class="li-required">type: str</span></li>
          
            <li><span class="li-normal">router_multicast6</span> </li>
          
            <li><span class="li-normal">vpn.certificate_remote</span>  <span class="li-required">param: name</span>  <span class="li-required">type: str</span></li>
          
            <li><span class="li-normal">system_fips-cc</span> </li>
          
            <li><span class="li-normal">system_ha</span> </li>
          
            <li><span class="li-normal">log.syslogd3_filter</span> </li>
          
            <li><span class="li-normal">user_radius</span>  <span class="li-required">param: name</span>  <span class="li-required">type: str</span></li>
          
            <li><span class="li-normal">firewall_DoS-policy6</span>  <span class="li-required">param: policyid</span>  <span class="li-required">type: int</span></li>
          
            <li><span class="li-normal">system_tos-based-priority</span>  <span class="li-required">param: id</span>  <span class="li-required">type: int</span></li>
          
            <li><span class="li-normal">vpn.certificate_local</span>  <span class="li-required">param: name</span>  <span class="li-required">type: str</span></li>
          
            <li><span class="li-normal">system_accprofile</span>  <span class="li-required">param: name</span>  <span class="li-required">type: str</span></li>
          
            <li><span class="li-normal">wireless-controller_global</span> </li>
          
            <li><span class="li-normal">log.syslogd_filter</span> </li>
          
            <li><span class="li-normal">dlp_sensor</span>  <span class="li-required">param: name</span>  <span class="li-required">type: str</span></li>
          
            <li><span class="li-normal">log.syslogd2_filter</span> </li>
          
            <li><span class="li-normal">wireless-controller_ble-profile</span>  <span class="li-required">param: name</span>  <span class="li-required">type: str</span></li>
          
            <li><span class="li-normal">system_password-policy-guest-admin</span> </li>
          
            <li><span class="li-normal">user_pop3</span>  <span class="li-required">param: name</span>  <span class="li-required">type: str</span></li>
          
            <li><span class="li-normal">switch-controller_system</span> </li>
          
            <li><span class="li-normal">voip_profile</span>  <span class="li-required">param: name</span>  <span class="li-required">type: str</span></li>
          
            <li><span class="li-normal">vpn.ipsec_manualkey-interface</span>  <span class="li-required">param: name</span>  <span class="li-required">type: str</span></li>
          
            <li><span class="li-normal">system_vdom-netflow</span> </li>
          
            <li><span class="li-normal">firewall.ipmacbinding_table</span>  <span class="li-required">param: seq_num</span>  <span class="li-required">type: int</span></li>
          
            <li><span class="li-normal">system_automation-destination</span>  <span class="li-required">param: name</span>  <span class="li-required">type: str</span></li>
          
            <li><span class="li-normal">dlp_fp-doc-source</span>  <span class="li-required">param: name</span>  <span class="li-required">type: str</span></li>
          
            <li><span class="li-normal">firewall_ldb-monitor</span>  <span class="li-required">param: name</span>  <span class="li-required">type: str</span></li>
          
            <li><span class="li-normal">firewall.ssh_host-key</span>  <span class="li-required">param: name</span>  <span class="li-required">type: str</span></li>
          
            <li><span class="li-normal">system_vdom-link</span>  <span class="li-required">param: name</span>  <span class="li-required">type: str</span></li>
          
            <li><span class="li-normal">system_admin</span>  <span class="li-required">param: name</span>  <span class="li-required">type: str</span></li>
          
            <li><span class="li-normal">router_ospf6</span> </li>
          
            <li><span class="li-normal">user_device</span>  <span class="li-required">param: alias</span>  <span class="li-required">type: str</span></li>
          
            <li><span class="li-normal">log.fortiguard_setting</span> </li>
          
            <li><span class="li-normal">system.snmp_community</span>  <span class="li-required">param: id</span>  <span class="li-required">type: int</span></li>
          
            <li><span class="li-normal">ips_settings</span> </li>
          
            <li><span class="li-normal">log.syslogd_override-filter</span> </li>
          
            <li><span class="li-normal">system_vdom-exception</span>  <span class="li-required">param: id</span>  <span class="li-required">type: int</span></li>
          
            <li><span class="li-normal">system_wccp</span>  <span class="li-required">param: service_id</span>  <span class="li-required">type: str</span></li>
          
            <li><span class="li-normal">system_automation-stitch</span>  <span class="li-required">param: name</span>  <span class="li-required">type: str</span></li>
          
            <li><span class="li-normal">firewall_profile-protocol-options</span>  <span class="li-required">param: name</span>  <span class="li-required">type: str</span></li>
          
            <li><span class="li-normal">report_theme</span>  <span class="li-required">param: name</span>  <span class="li-required">type: str</span></li>
          
            <li><span class="li-normal">firewall.ssh_local-key</span>  <span class="li-required">param: name</span>  <span class="li-required">type: str</span></li>
          
            <li><span class="li-normal">firewall_vip64</span>  <span class="li-required">param: name</span>  <span class="li-required">type: str</span></li>
          
            <li><span class="li-normal">web-proxy_wisp</span>  <span class="li-required">param: name</span>  <span class="li-required">type: str</span></li>
          
            <li><span class="li-normal">spamfilter_options</span> </li>
          
            <li><span class="li-normal">endpoint-control_forticlient-ems</span>  <span class="li-required">param: name</span>  <span class="li-required">type: str</span></li>
          
            <li><span class="li-normal">system_dns-server</span>  <span class="li-required">param: name</span>  <span class="li-required">type: str</span></li>
          
            <li><span class="li-normal">system.replacemsg_alertmail</span>  <span class="li-required">param: msg_type</span>  <span class="li-required">type: str</span></li>
          
            <li><span class="li-normal">log.fortiguard_override-filter</span> </li>
          
            <li><span class="li-normal">endpoint-control_client</span>  <span class="li-required">param: id</span>  <span class="li-required">type: int</span></li>
          
            <li><span class="li-normal">router_access-list6</span>  <span class="li-required">param: name</span>  <span class="li-required">type: str</span></li>
          
            <li><span class="li-normal">system_fortiguard</span> </li>
          
            <li><span class="li-normal">web-proxy_global</span> </li>
          
            <li><span class="li-normal">wanopt_profile</span>  <span class="li-required">param: name</span>  <span class="li-required">type: str</span></li>
          
            <li><span class="li-normal">wireless-controller.hotspot20_anqp-3gpp-cellular</span>  <span class="li-required">param: name</span>  <span class="li-required">type: str</span></li>
          
            <li><span class="li-normal">system.replacemsg_ec</span>  <span class="li-required">param: msg_type</span>  <span class="li-required">type: str</span></li>
          
            <li><span class="li-normal">switch-controller_vlan</span>  <span class="li-required">param: name</span>  <span class="li-required">type: str</span></li>
          
            <li><span class="li-normal">system_vxlan</span>  <span class="li-required">param: name</span>  <span class="li-required">type: str</span></li>
          
            <li><span class="li-normal">webfilter_search-engine</span>  <span class="li-required">param: name</span>  <span class="li-required">type: str</span></li>
          
            <li><span class="li-normal">system_ipv6-tunnel</span>  <span class="li-required">param: name</span>  <span class="li-required">type: str</span></li>
          
            <li><span class="li-normal">certificate_local</span>  <span class="li-required">param: name</span>  <span class="li-required">type: str</span></li>
          
            <li><span class="li-normal">user_fsso-polling</span>  <span class="li-required">param: id</span>  <span class="li-required">type: int</span></li>
          
            <li><span class="li-normal">system.dhcp_server</span>  <span class="li-required">param: id</span>  <span class="li-required">type: int</span></li>
          
            <li><span class="li-normal">report_chart</span>  <span class="li-required">param: name</span>  <span class="li-required">type: str</span></li>
          
            <li><span class="li-normal">vpn.certificate_setting</span> </li>
          
            <li><span class="li-normal">router_bfd6</span> </li>
          
            <li><span class="li-normal">system.replacemsg_nntp</span>  <span class="li-required">param: msg_type</span>  <span class="li-required">type: str</span></li>
          
            <li><span class="li-normal">firewall_proxy-policy</span>  <span class="li-required">param: policyid</span>  <span class="li-required">type: int</span></li>
          
            <li><span class="li-normal">system_dns</span> </li>
          
            <li><span class="li-normal">user_peergrp</span>  <span class="li-required">param: name</span>  <span class="li-required">type: str</span></li>
          
            <li><span class="li-normal">vpn.ipsec_concentrator</span>  <span class="li-required">param: name</span>  <span class="li-required">type: str</span></li>
          
            <li><span class="li-normal">ips_decoder</span>  <span class="li-required">param: name</span>  <span class="li-required">type: str</span></li>
          
            <li><span class="li-normal">dnsfilter_domain-filter</span>  <span class="li-required">param: id</span>  <span class="li-required">type: int</span></li>
          
            <li><span class="li-normal">wireless-controller_vap-group</span>  <span class="li-required">param: name</span>  <span class="li-required">type: str</span></li>
          
            <li><span class="li-normal">system_affinity-interrupt</span>  <span class="li-required">param: id</span>  <span class="li-required">type: int</span></li>
          
            <li><span class="li-normal">firewall_shaping-profile</span>  <span class="li-required">param: profile_name</span>  <span class="li-required">type: str</span></li>
          
            <li><span class="li-normal">firewall_interface-policy6</span>  <span class="li-required">param: policyid</span>  <span class="li-required">type: int</span></li>
          
            <li><span class="li-normal">vpn.ipsec_manualkey</span>  <span class="li-required">param: name</span>  <span class="li-required">type: str</span></li>
          
            <li><span class="li-normal">switch-controller_global</span> </li>
          
            <li><span class="li-normal">router_setting</span> </li>
          
            <li><span class="li-normal">system.replacemsg_admin</span>  <span class="li-required">param: msg_type</span>  <span class="li-required">type: str</span></li>
          
            <li><span class="li-normal">firewall.schedule_recurring</span>  <span class="li-required">param: name</span>  <span class="li-required">type: str</span></li>
          
            <li><span class="li-normal">system_sit-tunnel</span>  <span class="li-required">param: name</span>  <span class="li-required">type: str</span></li>
          
            <li><span class="li-normal">system_arp-table</span>  <span class="li-required">param: id</span>  <span class="li-required">type: int</span></li>
          
            <li><span class="li-normal">switch-controller_lldp-settings</span> </li>
          
            <li><span class="li-normal">webfilter_content-header</span>  <span class="li-required">param: id</span>  <span class="li-required">type: int</span></li>
          
            <li><span class="li-normal">system_auto-install</span> </li>
          
            <li><span class="li-normal">user_domain-controller</span>  <span class="li-required">param: name</span>  <span class="li-required">type: str</span></li>
          
            <li><span class="li-normal">router_multicast</span> </li>
          
            <li><span class="li-normal">firewall_ssl-server</span>  <span class="li-required">param: name</span>  <span class="li-required">type: str</span></li>
          
            <li><span class="li-normal">system.replacemsg_traffic-quota</span>  <span class="li-required">param: msg_type</span>  <span class="li-required">type: str</span></li>
          
            <li><span class="li-normal">system_fortimanager</span> </li>
          
            <li><span class="li-normal">system_mac-address-table</span>  <span class="li-required">param: mac</span>  <span class="li-required">type: str</span></li>
          
            <li><span class="li-normal">log.fortianalyzer_filter</span> </li>
          
            <li><span class="li-normal">system_network-visibility</span> </li>
          
            <li><span class="li-normal">firewall_interface-policy</span>  <span class="li-required">param: policyid</span>  <span class="li-required">type: int</span></li>
          
            <li><span class="li-normal">system.replacemsg_fortiguard-wf</span>  <span class="li-required">param: msg_type</span>  <span class="li-required">type: str</span></li>
          
            <li><span class="li-normal">wireless-controller_bonjour-profile</span>  <span class="li-required">param: name</span>  <span class="li-required">type: str</span></li>
          
            <li><span class="li-normal">webfilter_urlfilter</span>  <span class="li-required">param: id</span>  <span class="li-required">type: int</span></li>
          
            <li><span class="li-normal">system_probe-response</span> </li>
          
            <li><span class="li-normal">wireless-controller.hotspot20_h2qp-operator-name</span>  <span class="li-required">param: name</span>  <span class="li-required">type: str</span></li>
          
            <li><span class="li-normal">switch-controller_sflow</span> </li>
          
            <li><span class="li-normal">webfilter_fortiguard</span> </li>
          
            <li><span class="li-normal">wireless-controller.hotspot20_anqp-roaming-consortium</span>  <span class="li-required">param: name</span>  <span class="li-required">type: str</span></li>
          
            <li><span class="li-normal">firewall_DoS-policy</span>  <span class="li-required">param: policyid</span>  <span class="li-required">type: int</span></li>
          
            <li><span class="li-normal">firewall_proxy-addrgrp</span>  <span class="li-required">param: name</span>  <span class="li-required">type: str</span></li>
          
            <li><span class="li-normal">firewall_addrgrp</span>  <span class="li-required">param: name</span>  <span class="li-required">type: str</span></li>
          
            <li><span class="li-normal">firewall_policy6</span>  <span class="li-required">param: policyid</span>  <span class="li-required">type: int</span></li>
          
            <li><span class="li-normal">router_ripng</span> </li>
          
            <li><span class="li-normal">firewall_vip6</span>  <span class="li-required">param: name</span>  <span class="li-required">type: str</span></li>
          
            <li><span class="li-normal">web-proxy_forward-server</span>  <span class="li-required">param: name</span>  <span class="li-required">type: str</span></li>
          
            <li><span class="li-normal">system.replacemsg_spam</span>  <span class="li-required">param: msg_type</span>  <span class="li-required">type: str</span></li>
          
            <li><span class="li-normal">certificate_ca</span>  <span class="li-required">param: name</span>  <span class="li-required">type: str</span></li>
          
            <li><span class="li-normal">firewall.ssh_local-ca</span>  <span class="li-required">param: name</span>  <span class="li-required">type: str</span></li>
          
            <li><span class="li-normal">spamfilter_dnsbl</span>  <span class="li-required">param: id</span>  <span class="li-required">type: int</span></li>
          
            <li><span class="li-normal">waf_profile</span>  <span class="li-required">param: name</span>  <span class="li-required">type: str</span></li>
          
            <li><span class="li-normal">firewall.wildcard-fqdn_group</span>  <span class="li-required">param: name</span>  <span class="li-required">type: str</span></li>
          
            <li><span class="li-normal">switch-controller_managed-switch</span>  <span class="li-required">param: switch_id</span>  <span class="li-required">type: str</span></li>
          
            <li><span class="li-normal">user_group</span>  <span class="li-required">param: name</span>  <span class="li-required">type: str</span></li>
          
            <li><span class="li-normal">user_krb-keytab</span>  <span class="li-required">param: name</span>  <span class="li-required">type: str</span></li>
          
            <li><span class="li-normal">application_group</span>  <span class="li-required">param: name</span>  <span class="li-required">type: str</span></li>
          
            <li><span class="li-normal">system.replacemsg_ftp</span>  <span class="li-required">param: msg_type</span>  <span class="li-required">type: str</span></li>
          
            <li><span class="li-normal">log_threat-weight</span> </li>
          
            <li><span class="li-normal">extender-controller_extender</span>  <span class="li-required">param: id</span>  <span class="li-required">type: str</span></li>
          
            <li><span class="li-normal">wireless-controller.hotspot20_h2qp-conn-capability</span>  <span class="li-required">param: name</span>  <span class="li-required">type: str</span></li>
          
            <li><span class="li-normal">router_prefix-list</span>  <span class="li-required">param: name</span>  <span class="li-required">type: str</span></li>
          
            <li><span class="li-normal">system_gre-tunnel</span>  <span class="li-required">param: name</span>  <span class="li-required">type: str</span></li>
          </ul>
        </div>
        </section>
    <li><span class="li-head">params</span> - the parameter for each selector, see definition in above list.<span class="li-normal">type: dict</span></li>


Notes
-----

.. note::

   - Different ``selector`` may have different parameters, users are expected to look up them for a specific selector.

   - For some selectors, the objects are global, no ``params`` are allowed to appear.

   - If ``params`` is empty a non-unique object, the whole object list is returned.

   - This module has support for all configuration API, excluding any monitor API.

   - The result of API request is stored in ``results`` as a list.


Examples
--------

.. code-block:: yaml+jinja
    
    - hosts: fortigateslab
      connection: httpapi
      collections:
        - fortinet.fortios
      vars:
        ansible_httpapi_use_ssl: yes
        ansible_httpapi_validate_certs: no
        ansible_httpapi_port: 443
        vdom: "root"
      tasks:
      - name: get all
        fortios_configuration_fact:
          vdom: ""
          access_token: ""
          selector: log_custom-field

      - name: get single
        fortios_configuration_fact:
          vdom: ""
          access_token: ""
          selector: log_custom-field
          #optionally list or single get
          params:
            id: "3"

      - name: fetch one firewall address
        fortios_configuration_fact:
          selector: firewall_address
          params:
            name: "login.microsoft.com"

      - name: fetch all firewall addresses
        fortios_configuration_fact:
          selector: firewall_address


Return Values
-------------
Common return values are documented: https://docs.ansible.com/ansible/latest/reference_appendices/common_return_values.html#common-return-values, the following are the fields unique to this module:

.. raw:: html

    <ul>

    <li> <span class="li-return">build</span> - Build number of the fortigate image <span class="li-normal">returned: always</span> <span class="li-normal">type: str</span> <span class="li-normal">sample: 1547</span></li>
    <li> <span class="li-return">http_method</span> - Last method used to provision the content into FortiGate <span class="li-normal">returned: always</span> <span class="li-normal">type: str</span> <span class="li-normal">sample: GET</span></li>
    <li> <span class="li-return">name</span> - Name of the table used to fulfill the request <span class="li-normal">returned: always</span> <span class="li-normal">type: str</span> <span class="li-normal">sample: firmware</span></li>
    <li> <span class="li-return">path</span> - Path of the table used to fulfill the request <span class="li-normal">returned: always</span> <span class="li-normal">type: str</span> <span class="li-normal">sample: system</span></li>
    <li> <span class="li-return">results</span> - Object list retrieved from device. <span class="li-normal">returned: always</span> <span class="li-normal">type: list</span></li>
    <li> <span class="li-return">revision</span> - Internal revision number <span class="li-normal">returned: always</span> <span class="li-normal">type: str</span> <span class="li-normal">sample: 17.0.2.10658</span></li>
    <li> <span class="li-return">serial</span> - Serial number of the unit <span class="li-normal">returned: always</span> <span class="li-normal">type: str</span> <span class="li-normal">sample: FGVMEVYYQT3AB5352</span></li>
    <li> <span class="li-return">status</span> - Indication of the operation's result <span class="li-normal">returned: always</span> <span class="li-normal">type: str</span> <span class="li-normal">sample: success</span></li>
    <li> <span class="li-return">vdom</span> - Virtual domain used <span class="li-normal">returned: always</span> <span class="li-normal">type: str</span> <span class="li-normal">sample: root</span></li>
    <li> <span class="li-return">version</span> - Version of the FortiGate <span class="li-normal">returned: always</span> <span class="li-normal">type: str</span> <span class="li-normal">sample: v5.6.3</span></li>
    <li> <span class="li-return">ansible_facts</span> - The list of fact subsets collected from the device <span class="li-normal">returned: always</span> <span class="li-normal">type: dict</span></li>
    </ul>

Status
------

- This module is not guaranteed to have a backwards compatible interface.


Authors
-------

- Link Zheng (@chillancezen)
- Jie Xue (@JieX19)
- Hongbin Lu (@fgtdev-hblu)
- Frank Shen (@fshen01)


.. hint::
    If you notice any issues in this documentation, you can create a pull request to improve it.