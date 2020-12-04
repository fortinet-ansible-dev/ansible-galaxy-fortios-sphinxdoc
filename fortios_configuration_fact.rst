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
        <li><span class="li-normal">diagnose__tree__.vpn_l2tp</span> </li>
        <li><span class="li-normal">execute__tree__.fortiguard-log_try</span> </li>
        <li><span class="li-normal">execute__tree__.batch_end</span> </li>
        <li><span class="li-normal">execute__tree__.restore.vmlicense_ftp</span> </li>
        <li><span class="li-normal">execute__tree__.set.system.session.filter.negate_sport</span> </li>
        <li><span class="li-normal">execute__tree__.ping6-options_source</span> </li>
        <li><span class="li-normal">diagnose__tree__.ips_urlfilter</span> </li>
        <li><span class="li-normal">log.fortianalyzer_override-setting</span> </li>
        <li><span class="li-normal">execute__tree__.backup.config-with-forticlient-info_usb</span> </li>
        <li><span class="li-normal">execute__tree__.log_list</span> </li>
        <li><span class="li-normal">firewall.ssl_setting</span> </li>
        <li><span class="li-normal">vpn.ipsec_phase2-interface</span>  <span class="li-required">param: name</span>  <span class="li-required">type: str</span></li>
        <li><span class="li-normal">router_key-chain</span>  <span class="li-required">param: name</span>  <span class="li-required">type: str</span></li>
        <li><span class="li-normal">system_ddns</span>  <span class="li-required">param: ddnsid</span>  <span class="li-required">type: int</span></li>
        <li><span class="li-normal">system_replacemsg-group</span>  <span class="li-required">param: name</span>  <span class="li-required">type: str</span></li>
        <li><span class="li-normal">execute__tree__.set.system.session.filter.negate_duration</span> </li>
        <li><span class="li-normal">system_ftm-push</span> </li>
        <li><span class="li-normal">system_sms-server</span>  <span class="li-required">param: name</span>  <span class="li-required">type: str</span></li>
        <li><span class="li-normal">firewall_central-snat-map</span>  <span class="li-required">param: policyid</span>  <span class="li-required">type: int</span></li>
        <li><span class="li-normal">firewall_multicast-address6</span>  <span class="li-required">param: name</span>  <span class="li-required">type: str</span></li>
        <li><span class="li-normal">execute__tree___factoryreset2</span> </li>
        <li><span class="li-normal">execute__tree___update-list</span> </li>
        <li><span class="li-normal">execute__tree__.wireless-controller_led-blink</span> </li>
        <li><span class="li-normal">execute__tree__.revision.list_config</span> </li>
        <li><span class="li-normal">system.replacemsg_sslvpn</span>  <span class="li-required">param: msg_type</span>  <span class="li-required">type: str</span></li>
        <li><span class="li-normal">diagnose__tree__.ips.av_stats</span> </li>
        <li><span class="li-normal">system_pppoe-interface</span>  <span class="li-required">param: name</span>  <span class="li-required">type: str</span></li>
        <li><span class="li-normal">execute__tree__.wireless-controller.upload-wtp-image_ftp</span> </li>
        <li><span class="li-normal">diagnose__tree___wireless-controller</span> </li>
        <li><span class="li-normal">execute__tree___update-geo-ip</span> </li>
        <li><span class="li-normal">diagnose__tree___lldptx</span> </li>
        <li><span class="li-normal">firewall_addrgrp6</span>  <span class="li-required">param: name</span>  <span class="li-required">type: str</span></li>
        <li><span class="li-normal">log.disk_filter</span> </li>
        <li><span class="li-normal">system_affinity-packet-redistribution</span>  <span class="li-required">param: id</span>  <span class="li-required">type: int</span></li>
        <li><span class="li-normal">diagnose__tree__.ip_tcp</span> </li>
        <li><span class="li-normal">firewall_proxy-address</span>  <span class="li-required">param: name</span>  <span class="li-required">type: str</span></li>
        <li><span class="li-normal">execute__tree__.restore.config.management-station_normal</span> </li>
        <li><span class="li-normal">execute__tree__.dhcp6_lease-list</span> </li>
        <li><span class="li-normal">authentication_rule</span>  <span class="li-required">param: name</span>  <span class="li-required">type: str</span></li>
        <li><span class="li-normal">execute__tree__.wireless-controller.hs20-icon_list-hs-icon</span> </li>
        <li><span class="li-normal">execute__tree__.switch-controller_set-standalone</span> </li>
        <li><span class="li-normal">execute__tree___ping</span> </li>
        <li><span class="li-normal">execute__tree___set-next-reboot</span> </li>
        <li><span class="li-normal">execute__tree__.backup.memory.log_ftp</span> </li>
        <li><span class="li-normal">execute__tree__.ping6-options_interval</span> </li>
        <li><span class="li-normal">execute__tree__.firewall.ssh.generate_local-key</span> </li>
        <li><span class="li-normal">router_bfd</span> </li>
        <li><span class="li-normal">execute__tree__.restore.image_tftp</span> </li>
        <li><span class="li-normal">execute__tree__.upload.image_tftp</span> </li>
        <li><span class="li-normal">execute__tree__.backup.disk.log_tftp</span> </li>
        <li><span class="li-normal">execute__tree__.fortitoken.import_usb</span> </li>
        <li><span class="li-normal">switch-controller_custom-command</span>  <span class="li-required">param: command_name</span>  <span class="li-required">type: str</span></li>
        <li><span class="li-normal">system_resource-limits</span> </li>
        <li><span class="li-normal">execute__tree__.report_flush-cache</span> </li>
        <li><span class="li-normal">system.replacemsg_auth</span>  <span class="li-required">param: msg_type</span>  <span class="li-required">type: str</span></li>
        <li><span class="li-normal">system.autoupdate_schedule</span> </li>
        <li><span class="li-normal">execute__tree__.restore.secondary-image_usb</span> </li>
        <li><span class="li-normal">execute__tree__.central-mgmt_register-device</span> </li>
        <li><span class="li-normal">execute__tree__.backup.config_usb</span> </li>
        <li><span class="li-normal">execute__tree__.restore.script_tftp</span> </li>
        <li><span class="li-normal">waf_sub-class</span>  <span class="li-required">param: id</span>  <span class="li-required">type: int</span></li>
        <li><span class="li-normal">firewall_local-in-policy6</span>  <span class="li-required">param: policyid</span>  <span class="li-required">type: int</span></li>
        <li><span class="li-normal">diagnose__tree__.ips_raw</span> </li>
        <li><span class="li-normal">log.fortianalyzer_override-filter</span> </li>
        <li><span class="li-normal">system.replacemsg_icap</span>  <span class="li-required">param: msg_type</span>  <span class="li-required">type: str</span></li>
        <li><span class="li-normal">system_object-tagging</span>  <span class="li-required">param: category</span>  <span class="li-required">type: str</span></li>
        <li><span class="li-normal">spamfilter_profile</span>  <span class="li-required">param: name</span>  <span class="li-required">type: str</span></li>
        <li><span class="li-normal">execute__tree___update-now</span> </li>
        <li><span class="li-normal">execute__tree__.ping-options_tos</span> </li>
        <li><span class="li-normal">diagnose__tree___vmware</span> </li>
        <li><span class="li-normal">spamfilter_bwl</span>  <span class="li-required">param: id</span>  <span class="li-required">type: int</span></li>
        <li><span class="li-normal">execute__tree__.extender_delete-fortiextender-image</span> </li>
        <li><span class="li-normal">execute__tree__.webcache.delete_simple-string</span> </li>
        <li><span class="li-normal">execute__tree__.set.system.session.filter.negate_proto</span> </li>
        <li><span class="li-normal">web-proxy_profile</span>  <span class="li-required">param: name</span>  <span class="li-required">type: str</span></li>
        <li><span class="li-normal">diagnose__tree__.webfilter_fortiguard</span> </li>
        <li><span class="li-normal">execute__tree__.auto-script_delete</span> </li>
        <li><span class="li-normal">diagnose__tree___cp</span> </li>
        <li><span class="li-normal">diagnose__tree__.ipv6_devconf</span> </li>
        <li><span class="li-normal">spamfilter_mheader</span>  <span class="li-required">param: id</span>  <span class="li-required">type: int</span></li>
        <li><span class="li-normal">router_route-map</span>  <span class="li-required">param: name</span>  <span class="li-required">type: str</span></li>
        <li><span class="li-normal">diagnose__tree__.ip_ipip-tunnel</span> </li>
        <li><span class="li-normal">user_adgrp</span>  <span class="li-required">param: name</span>  <span class="li-required">type: str</span></li>
        <li><span class="li-normal">system_auto-script</span>  <span class="li-required">param: name</span>  <span class="li-required">type: str</span></li>
        <li><span class="li-normal">switch-controller_quarantine</span> </li>
        <li><span class="li-normal">firewall.service_category</span>  <span class="li-required">param: name</span>  <span class="li-required">type: str</span></li>
        <li><span class="li-normal">execute__tree__.router.clear.ospf6_process</span> </li>
        <li><span class="li-normal">execute__tree__.switch-controller.get-physical-conn_dot</span> </li>
        <li><span class="li-normal">system_link-monitor</span>  <span class="li-required">param: name</span>  <span class="li-required">type: str</span></li>
        <li><span class="li-normal">switch-controller_stp-settings</span> </li>
        <li><span class="li-normal">user_security-exempt-list</span>  <span class="li-required">param: name</span>  <span class="li-required">type: str</span></li>
        <li><span class="li-normal">execute__tree__.mrouter.clear_igmp-interface</span> </li>
        <li><span class="li-normal">diagnose__tree___antivirus</span> </li>
        <li><span class="li-normal">execute__tree__.log.filter_dump</span> </li>
        <li><span class="li-normal">firewall_sniffer</span>  <span class="li-required">param: id</span>  <span class="li-required">type: int</span></li>
        <li><span class="li-normal">execute__tree__.vpn.certificate.ca.export_tftp</span> </li>
        <li><span class="li-normal">execute__tree__.vpn.sslvpn_del-all</span> </li>
        <li><span class="li-normal">execute__tree__.restore.config_flash</span> </li>
        <li><span class="li-normal">log.fortiguard_override-setting</span> </li>
        <li><span class="li-normal">execute__tree__.mrouter.clear_multicast-routes</span> </li>
        <li><span class="li-normal">firewall_internet-service</span>  <span class="li-required">param: id</span>  <span class="li-required">type: int</span></li>
        <li><span class="li-normal">execute__tree__.interface_dhcpclient-renew</span> </li>
        <li><span class="li-normal">execute__tree__.tac_report</span> </li>
        <li><span class="li-normal">firewall_vipgrp46</span>  <span class="li-required">param: name</span>  <span class="li-required">type: str</span></li>
        <li><span class="li-normal">log.webtrends_filter</span> </li>
        <li><span class="li-normal">webfilter_ips-urlfilter-setting6</span> </li>
        <li><span class="li-normal">router_prefix-list6</span>  <span class="li-required">param: name</span>  <span class="li-required">type: str</span></li>
        <li><span class="li-normal">execute__tree__.extender_list-fortiextender-image</span> </li>
        <li><span class="li-normal">log_setting</span> </li>
        <li><span class="li-normal">firewall_address6-template</span>  <span class="li-required">param: name</span>  <span class="li-required">type: str</span></li>
        <li><span class="li-normal">wireless-controller.hotspot20_h2qp-wan-metric</span>  <span class="li-required">param: name</span>  <span class="li-required">type: str</span></li>
        <li><span class="li-normal">system_automation-action</span>  <span class="li-required">param: name</span>  <span class="li-required">type: str</span></li>
        <li><span class="li-normal">system.autoupdate_tunneling</span> </li>
        <li><span class="li-normal">diagnose__tree__.ip.router_isis</span> </li>
        <li><span class="li-normal">execute__tree__.nsx.group_delete</span> </li>
        <li><span class="li-normal">webfilter_ips-urlfilter-setting</span> </li>
        <li><span class="li-normal">execute__tree__.wireless-controller.hs20-icon.upload-icon_ftp</span> </li>
        <li><span class="li-normal">execute__tree__.restore.config_usb-mode</span> </li>
        <li><span class="li-normal">execute__tree__.vpn.sslvpn_del-tunnel</span> </li>
        <li><span class="li-normal">switch-controller_network-monitor-settings</span> </li>
        <li><span class="li-normal">system_alias</span>  <span class="li-required">param: name</span>  <span class="li-required">type: str</span></li>
        <li><span class="li-normal">diagnose__tree___endpoint</span> </li>
        <li><span class="li-normal">switch-controller_mac-sync-settings</span> </li>
        <li><span class="li-normal">web-proxy_forward-server-group</span>  <span class="li-required">param: name</span>  <span class="li-required">type: str</span></li>
        <li><span class="li-normal">execute__tree__.upload.report-img_ftp</span> </li>
        <li><span class="li-normal">execute__tree__.switch-controller.restart-swtp-delayed_all</span> </li>
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
        <li><span class="li-normal">execute__tree__.ping-options_adaptive-ping</span> </li>
        <li><span class="li-normal">diagnose__tree__.ip_udp</span> </li>
        <li><span class="li-normal">diagnose__tree__.vpn_ipsec</span> </li>
        <li><span class="li-normal">execute__tree__.backup.disk.log_ftp</span> </li>
        <li><span class="li-normal">firewall.service_group</span>  <span class="li-required">param: name</span>  <span class="li-required">type: str</span></li>
        <li><span class="li-normal">system.autoupdate_push-update</span> </li>
        <li><span class="li-normal">firewall_address6</span>  <span class="li-required">param: name</span>  <span class="li-required">type: str</span></li>
        <li><span class="li-normal">endpoint-control_profile</span>  <span class="li-required">param: profile_name</span>  <span class="li-required">type: str</span></li>
        <li><span class="li-normal">execute__tree__.usb-disk_eject</span> </li>
        <li><span class="li-normal">execute__tree__.interface_dhcp6client-renew</span> </li>
        <li><span class="li-normal">diagnose__tree___traffictest</span> </li>
        <li><span class="li-normal">wireless-controller_wids-profile</span>  <span class="li-required">param: name</span>  <span class="li-required">type: str</span></li>
        <li><span class="li-normal">execute__tree__.vpn.certificate.local.generate_default-ssl-ca</span> </li>
        <li><span class="li-normal">log.fortiguard_filter</span> </li>
        <li><span class="li-normal">firewall_ipv6-eh-filter</span> </li>
        <li><span class="li-normal">execute__tree___sync-session</span> </li>
        <li><span class="li-normal">execute__tree__.mrouter.clear_igmp-group</span> </li>
        <li><span class="li-normal">user_device-category</span>  <span class="li-required">param: name</span>  <span class="li-required">type: str</span></li>
        <li><span class="li-normal">diagnose__tree___wacs</span> </li>
        <li><span class="li-normal">execute__tree__.restore.image_ftp</span> </li>
        <li><span class="li-normal">firewall_identity-based-route</span>  <span class="li-required">param: name</span>  <span class="li-required">type: str</span></li>
        <li><span class="li-normal">execute__tree__.switch-controller_push-swtp-image</span> </li>
        <li><span class="li-normal">system_console</span> </li>
        <li><span class="li-normal">diagnose__tree__.vpn_concentrator</span> </li>
        <li><span class="li-normal">system_ntp</span> </li>
        <li><span class="li-normal">router_bgp</span> </li>
        <li><span class="li-normal">system_nat64</span> </li>
        <li><span class="li-normal">execute__tree__.ping-options_reset</span> </li>
        <li><span class="li-normal">execute__tree__.set.system.session.filter.clear_sport</span> </li>
        <li><span class="li-normal">system.3g-modem_custom</span>  <span class="li-required">param: id</span>  <span class="li-required">type: int</span></li>
        <li><span class="li-normal">report_layout</span>  <span class="li-required">param: name</span>  <span class="li-required">type: str</span></li>
        <li><span class="li-normal">wireless-controller_timers</span> </li>
        <li><span class="li-normal">diagnose__tree___src-vis</span> </li>
        <li><span class="li-normal">execute__tree__.set.system.session.filter_expire</span> </li>
        <li><span class="li-normal">execute__tree__.vpn.certificate.local.generate_rsa</span> </li>
        <li><span class="li-normal">execute__tree__.router_restart</span> </li>
        <li><span class="li-normal">diagnose__tree___wad</span> </li>
        <li><span class="li-normal">wireless-controller.hotspot20_icon</span>  <span class="li-required">param: name</span>  <span class="li-required">type: str</span></li>
        <li><span class="li-normal">diagnose__tree___waf</span> </li>
        <li><span class="li-normal">execute__tree__.wireless-controller_delete-wtp-image</span> </li>
        <li><span class="li-normal">execute__tree__.log_flush-cache</span> </li>
        <li><span class="li-normal">execute__tree__.backup.config_management-station</span> </li>
        <li><span class="li-normal">log.memory_global-setting</span> </li>
        <li><span class="li-normal">router_multicast-flow</span>  <span class="li-required">param: name</span>  <span class="li-required">type: str</span></li>
        <li><span class="li-normal">ssh-filter_profile</span>  <span class="li-required">param: name</span>  <span class="li-required">type: str</span></li>
        <li><span class="li-normal">system_fortisandbox</span> </li>
        <li><span class="li-normal">execute__tree__.modem_hangup</span> </li>
        <li><span class="li-normal">system_virtual-wan-link</span> </li>
        <li><span class="li-normal">ips_sensor</span>  <span class="li-required">param: name</span>  <span class="li-required">type: str</span></li>
        <li><span class="li-normal">firewall.wildcard-fqdn_custom</span>  <span class="li-required">param: name</span>  <span class="li-required">type: str</span></li>
        <li><span class="li-normal">router_static</span>  <span class="li-required">param: seq_num</span>  <span class="li-required">type: int</span></li>
        <li><span class="li-normal">execute__tree___disconnect-admin-session</span> </li>
        <li><span class="li-normal">execute__tree__.switch-controller_custom-command</span> </li>
        <li><span class="li-normal">alertemail_setting</span> </li>
        <li><span class="li-normal">diagnose__tree__.ip.router_command</span> </li>
        <li><span class="li-normal">diagnose__tree___alertconsole</span> </li>
        <li><span class="li-normal">diagnose__tree___forticare</span> </li>
        <li><span class="li-normal">execute__tree__.fortitoken.import_ftp</span> </li>
        <li><span class="li-normal">router_policy</span>  <span class="li-required">param: seq_num</span>  <span class="li-required">type: int</span></li>
        <li><span class="li-normal">user_fortitoken</span>  <span class="li-required">param: serial_number</span>  <span class="li-required">type: str</span></li>
        <li><span class="li-normal">execute__tree__.replace-device_fortiap</span> </li>
        <li><span class="li-normal">web-proxy_debug-url</span>  <span class="li-required">param: name</span>  <span class="li-required">type: str</span></li>
        <li><span class="li-normal">execute__tree__.switch-controller.restart-swtp-delayed_switch-group</span> </li>
        <li><span class="li-normal">execute__tree__.switch-controller_get-conn-status</span> </li>
        <li><span class="li-normal">execute__tree__.vpn.sslvpn_rdel-tunnel</span> </li>
        <li><span class="li-normal">execute__tree__.vpn.certificate.local.generate_default-ssl-serv-key</span> </li>
        <li><span class="li-normal">diagnose__tree___fdsm</span> </li>
        <li><span class="li-normal">webfilter_override</span>  <span class="li-required">param: id</span>  <span class="li-required">type: int</span></li>
        <li><span class="li-normal">diagnose__tree__.ipv6_ipv6-tunnel</span> </li>
        <li><span class="li-normal">execute__tree__.vpn.certificate.local_verify</span> </li>
        <li><span class="li-normal">execute__tree__.log.filter_start-line</span> </li>
        <li><span class="li-normal">execute__tree__.ping6-options_view-settings</span> </li>
        <li><span class="li-normal">system_fsso-polling</span> </li>
        <li><span class="li-normal">user_peer</span>  <span class="li-required">param: name</span>  <span class="li-required">type: str</span></li>
        <li><span class="li-normal">vpn.ssl.web_host-check-software</span>  <span class="li-required">param: name</span>  <span class="li-required">type: str</span></li>
        <li><span class="li-normal">execute__tree___forticarrier-license</span> </li>
        <li><span class="li-normal">switch-controller_lldp-profile</span>  <span class="li-required">param: name</span>  <span class="li-required">type: str</span></li>
        <li><span class="li-normal">execute__tree__.policy-packet-capture_delete-all</span> </li>
        <li><span class="li-normal">execute__tree__.switch-controller_trigger-config-sync</span> </li>
        <li><span class="li-normal">execute__tree__.backup.config_tftp</span> </li>
        <li><span class="li-normal">vpn.ssl.web_realm</span>  <span class="li-required">param: url_path</span>  <span class="li-required">type: str</span></li>
        <li><span class="li-normal">system_stp</span> </li>
        <li><span class="li-normal">execute__tree__.ha_synchronize</span> </li>
        <li><span class="li-normal">execute__tree__.upload.report-img_tftp</span> </li>
        <li><span class="li-normal">execute__tree__.ping-options_df-bit</span> </li>
        <li><span class="li-normal">execute__tree__.set.system.session.filter.clear_proto</span> </li>
        <li><span class="li-normal">execute__tree__.webcache.delete_regular-expression</span> </li>
        <li><span class="li-normal">switch-controller.security-policy_captive-portal</span>  <span class="li-required">param: name</span>  <span class="li-required">type: str</span></li>
        <li><span class="li-normal">firewall_shaping-policy</span>  <span class="li-required">param: id</span>  <span class="li-required">type: int</span></li>
        <li><span class="li-normal">execute__tree__.fortiguard-message_add</span> </li>
        <li><span class="li-normal">log_custom-field</span>  <span class="li-required">param: id</span>  <span class="li-required">type: str</span></li>
        <li><span class="li-normal">execute__tree__.ping6-options_ttl</span> </li>
        <li><span class="li-normal">firewall_address</span>  <span class="li-required">param: name</span>  <span class="li-required">type: str</span></li>
        <li><span class="li-normal">certificate_crl</span>  <span class="li-required">param: name</span>  <span class="li-required">type: str</span></li>
        <li><span class="li-normal">execute__tree__.restore.config.management-station_template</span> </li>
        <li><span class="li-normal">execute__tree__.backup.disk.alllogs_tftp</span> </li>
        <li><span class="li-normal">execute__tree__.set.system.session.filter.clear_dst</span> </li>
        <li><span class="li-normal">firewall.ssh_setting</span> </li>
        <li><span class="li-normal">execute__tree__.wireless-controller.upload-wtp-image_tftp</span> </li>
        <li><span class="li-normal">diagnose__tree__.ip.router_igmp</span> </li>
        <li><span class="li-normal">router_access-list</span>  <span class="li-required">param: name</span>  <span class="li-required">type: str</span></li>
        <li><span class="li-normal">log.memory_setting</span> </li>
        <li><span class="li-normal">system_alarm</span> </li>
        <li><span class="li-normal">diagnose__tree__.vpn_ike</span> </li>
        <li><span class="li-normal">system_ipv6-neighbor-cache</span>  <span class="li-required">param: id</span>  <span class="li-required">type: int</span></li>
        <li><span class="li-normal">diagnose__tree__.test_application</span> </li>
        <li><span class="li-normal">execute__tree__.interface_pppoe-reconnect</span> </li>
        <li><span class="li-normal">execute__tree__.fortiguard-log_login</span> </li>
        <li><span class="li-normal">diagnose__tree__.webfilter_bword</span> </li>
        <li><span class="li-normal">execute__tree__.switch-controller_clear-igmp-snoop</span> </li>
        <li><span class="li-normal">system_cluster-sync</span>  <span class="li-required">param: sync_id</span>  <span class="li-required">type: int</span></li>
        <li><span class="li-normal">wanopt_settings</span> </li>
        <li><span class="li-normal">endpoint-control_registered-forticlient</span>  <span class="li-required">param: uid</span>  <span class="li-required">type: str</span></li>
        <li><span class="li-normal">system_dedicated-mgmt</span> </li>
        <li><span class="li-normal">diagnose__tree___disktest</span> </li>
        <li><span class="li-normal">execute__tree__.wireless-controller_list-wtp-image</span> </li>
        <li><span class="li-normal">execute__tree__.vpn.certificate.ca.import_tftp</span> </li>
        <li><span class="li-normal">execute__tree__.usb-disk_list</span> </li>
        <li><span class="li-normal">diagnose__tree__.ip_multicast</span> </li>
        <li><span class="li-normal">diagnose__tree__.ips.av_timeout</span> </li>
        <li><span class="li-normal">firewall_policy46</span>  <span class="li-required">param: policyid</span>  <span class="li-required">type: int</span></li>
        <li><span class="li-normal">execute__tree__.vpn.sslvpn_rdel-web</span> </li>
        <li><span class="li-normal">execute__tree__.vpn.certificate.local.import_tftp</span> </li>
        <li><span class="li-normal">diagnose__tree__.ipv6_route</span> </li>
        <li><span class="li-normal">execute__tree__.router.clear.bgp_flap-statistics</span> </li>
        <li><span class="li-normal">execute__tree__.fortiguard-log_join</span> </li>
        <li><span class="li-normal">antivirus_settings</span> </li>
        <li><span class="li-normal">execute__tree__.wireless-controller_restart-acd</span> </li>
        <li><span class="li-normal">switch-controller_802-1X-settings</span> </li>
        <li><span class="li-normal">execute__tree__.switch-controller_restart-swtpd</span> </li>
        <li><span class="li-normal">execute__tree__.backup.memory.alllogs_ftp</span> </li>
        <li><span class="li-normal">execute__tree__.fortitoken_import-sn-file</span> </li>
        <li><span class="li-normal">system_session-ttl</span> </li>
        <li><span class="li-normal">execute__tree__.extender.upload-fortiextender-image_tftp</span> </li>
        <li><span class="li-normal">diagnose__tree___central-mgmt</span> </li>
        <li><span class="li-normal">system_storage</span>  <span class="li-required">param: name</span>  <span class="li-required">type: str</span></li>
        <li><span class="li-normal">execute__tree__.fortiguard-log_create-account</span> </li>
        <li><span class="li-normal">execute__tree__.fortiguard-message_update</span> </li>
        <li><span class="li-normal">log.memory_filter</span> </li>
        <li><span class="li-normal">firewall_auth-portal</span> </li>
        <li><span class="li-normal">system_sflow</span> </li>
        <li><span class="li-normal">user_ldap</span>  <span class="li-required">param: name</span>  <span class="li-required">type: str</span></li>
        <li><span class="li-normal">diagnose__tree___rsso</span> </li>
        <li><span class="li-normal">ips_global</span> </li>
        <li><span class="li-normal">wanopt_remote-storage</span> </li>
        <li><span class="li-normal">execute__tree__.vpn.certificate.local.generate_default-ssl-key-certs</span> </li>
        <li><span class="li-normal">wireless-controller.hotspot20_qos-map</span>  <span class="li-required">param: name</span>  <span class="li-required">type: str</span></li>
        <li><span class="li-normal">vpn_l2tp</span> </li>
        <li><span class="li-normal">diagnose__tree___fortiview</span> </li>
        <li><span class="li-normal">diagnose__tree__.ip_rtcache</span> </li>
        <li><span class="li-normal">firewall_vip46</span>  <span class="li-required">param: name</span>  <span class="li-required">type: str</span></li>
        <li><span class="li-normal">execute__tree__.usb-disk_delete</span> </li>
        <li><span class="li-normal">execute__tree__.wireless-controller.hs20-icon.backup-icon_tftp</span> </li>
        <li><span class="li-normal">execute__tree__.wireless-controller.hs20-icon_delete-hs-icon</span> </li>
        <li><span class="li-normal">execute__tree__.usb-disk_format</span> </li>
        <li><span class="li-normal">authentication_setting</span> </li>
        <li><span class="li-normal">vpn.certificate_ocsp-server</span>  <span class="li-required">param: name</span>  <span class="li-required">type: str</span></li>
        <li><span class="li-normal">diagnose__tree___spamfilter</span> </li>
        <li><span class="li-normal">execute__tree__.traceroute-options_source</span> </li>
        <li><span class="li-normal">antivirus_heuristic</span> </li>
        <li><span class="li-normal">spamfilter_bword</span>  <span class="li-required">param: id</span>  <span class="li-required">type: int</span></li>
        <li><span class="li-normal">system_custom-language</span>  <span class="li-required">param: name</span>  <span class="li-required">type: str</span></li>
        <li><span class="li-normal">web-proxy_explicit</span> </li>
        <li><span class="li-normal">execute__tree__.disk_format</span> </li>
        <li><span class="li-normal">execute__tree__.log_display</span> </li>
        <li><span class="li-normal">execute__tree___factory-license</span> </li>
        <li><span class="li-normal">wireless-controller_wtp-group</span>  <span class="li-required">param: name</span>  <span class="li-required">type: str</span></li>
        <li><span class="li-normal">execute__tree__.backup.disk.ipsarchives_usb</span> </li>
        <li><span class="li-normal">execute__tree__.report_recreate-db</span> </li>
        <li><span class="li-normal">execute__tree__.set.system.session.filter.clear_dport</span> </li>
        <li><span class="li-normal">system_vdom-sflow</span> </li>
        <li><span class="li-normal">switch-controller_igmp-snooping</span> </li>
        <li><span class="li-normal">waf_signature</span>  <span class="li-required">param: id</span>  <span class="li-required">type: int</span></li>
        <li><span class="li-normal">execute__tree__.fortitoken-mobile_import</span> </li>
        <li><span class="li-normal">log.null-device_setting</span> </li>
        <li><span class="li-normal">ips_rule-settings</span>  <span class="li-required">param: id</span>  <span class="li-required">type: int</span></li>
        <li><span class="li-normal">log.syslogd_setting</span> </li>
        <li><span class="li-normal">execute__tree__.backup.memory.alllogs_tftp</span> </li>
        <li><span class="li-normal">diagnose__tree__.ipv6.router_rip</span> </li>
        <li><span class="li-normal">switch-controller.security-policy_802-1X</span>  <span class="li-required">param: name</span>  <span class="li-required">type: str</span></li>
        <li><span class="li-normal">report_setting</span> </li>
        <li><span class="li-normal">execute__tree__.set.system.session.filter_policy</span> </li>
        <li><span class="li-normal">execute__tree__.set.system.session.filter.negate_expire</span> </li>
        <li><span class="li-normal">user_setting</span> </li>
        <li><span class="li-normal">diagnose__tree__.test_update</span> </li>
        <li><span class="li-normal">icap_profile</span>  <span class="li-required">param: name</span>  <span class="li-required">type: str</span></li>
        <li><span class="li-normal">system_geoip-override</span>  <span class="li-required">param: name</span>  <span class="li-required">type: str</span></li>
        <li><span class="li-normal">vpn.ipsec_phase1</span>  <span class="li-required">param: name</span>  <span class="li-required">type: str</span></li>
        <li><span class="li-normal">vpn.ipsec_phase2</span>  <span class="li-required">param: name</span>  <span class="li-required">type: str</span></li>
        <li><span class="li-normal">wireless-controller.hotspot20_anqp-network-auth-type</span>  <span class="li-required">param: name</span>  <span class="li-required">type: str</span></li>
        <li><span class="li-normal">execute__tree__.ping-options_data-size</span> </li>
        <li><span class="li-normal">webfilter_ips-urlfilter-cache-setting</span> </li>
        <li><span class="li-normal">firewall.ipmacbinding_setting</span> </li>
        <li><span class="li-normal">diagnose__tree___autoupdate</span> </li>
        <li><span class="li-normal">diagnose__tree__.ipv6_gre-tunnel</span> </li>
        <li><span class="li-normal">log.fortianalyzer2_filter</span> </li>
        <li><span class="li-normal">diagnose__tree__.netlink_device</span> </li>
        <li><span class="li-normal">application_rule-settings</span>  <span class="li-required">param: id</span>  <span class="li-required">type: int</span></li>
        <li><span class="li-normal">execute__tree__.system.custom-language_import</span> </li>
        <li><span class="li-normal">diagnose__tree__.ips_share</span> </li>
        <li><span class="li-normal">log.syslogd4_filter</span> </li>
        <li><span class="li-normal">execute__tree__.mrouter.clear_sparse-mode-bsr</span> </li>
        <li><span class="li-normal">execute__tree__.set.system.session.filter_list</span> </li>
        <li><span class="li-normal">execute__tree__.restore.script_scp</span> </li>
        <li><span class="li-normal">system_proxy-arp</span>  <span class="li-required">param: id</span>  <span class="li-required">type: int</span></li>
        <li><span class="li-normal">webfilter_ftgd-local-rating</span>  <span class="li-required">param: url</span>  <span class="li-required">type: str</span></li>
        <li><span class="li-normal">execute__tree__.extender.upload-fortiextender-image_ftp</span> </li>
        <li><span class="li-normal">diagnose__tree___switch-controller</span> </li>
        <li><span class="li-normal">execute__tree__.switch-controller.virtual-port-pool_show</span> </li>
        <li><span class="li-normal">diagnose__tree__.ips.global_rule</span> </li>
        <li><span class="li-normal">ips_custom</span>  <span class="li-required">param: tag</span>  <span class="li-required">type: str</span></li>
        <li><span class="li-normal">vpn_ocvpn</span> </li>
        <li><span class="li-normal">execute__tree__.switch-controller.get-sync-status_group </span> </li>
        <li><span class="li-normal">execute__tree__.ping6-options_interface</span> </li>
        <li><span class="li-normal">execute__tree__.switch-controller_restart-acd</span> </li>
        <li><span class="li-normal">switch-controller_switch-interface-tag</span>  <span class="li-required">param: name</span>  <span class="li-required">type: str</span></li>
        <li><span class="li-normal">router_policy6</span>  <span class="li-required">param: seq_num</span>  <span class="li-required">type: int</span></li>
        <li><span class="li-normal">execute__tree__.restore.other-objects_ftp</span> </li>
        <li><span class="li-normal">execute__tree__.system.fortisandbox_test-connectivity</span> </li>
        <li><span class="li-normal">switch-controller.qos_ip-dscp-map</span>  <span class="li-required">param: name</span>  <span class="li-required">type: str</span></li>
        <li><span class="li-normal">execute__tree__.upload.config_usb</span> </li>
        <li><span class="li-normal">diagnose__tree__.netlink_qlen</span> </li>
        <li><span class="li-normal">execute__tree__.backup.config_flash</span> </li>
        <li><span class="li-normal">log_eventfilter</span> </li>
        <li><span class="li-normal">firewall_internet-service-custom</span>  <span class="li-required">param: name</span>  <span class="li-required">type: str</span></li>
        <li><span class="li-normal">diagnose__tree__.ips_packet</span> </li>
        <li><span class="li-normal">execute__tree__.restore.av_ftp</span> </li>
        <li><span class="li-normal">diagnose__tree__.ip.router_imi</span> </li>
        <li><span class="li-normal">router_auth-path</span>  <span class="li-required">param: name</span>  <span class="li-required">type: str</span></li>
        <li><span class="li-normal">diagnose__tree__.ip.router_bgp</span> </li>
        <li><span class="li-normal">diagnose__tree___radiusd</span> </li>
        <li><span class="li-normal">system_external-resource</span>  <span class="li-required">param: name</span>  <span class="li-required">type: str</span></li>
        <li><span class="li-normal">execute__tree__.log_backup</span> </li>
        <li><span class="li-normal">execute__tree__.set.system.session.filter_sport</span> </li>
        <li><span class="li-normal">execute__tree__.ping6-options_reset</span> </li>
        <li><span class="li-normal">diagnose__tree__.ip.router_rip</span> </li>
        <li><span class="li-normal">diagnose__tree__.vpn_ssl</span> </li>
        <li><span class="li-normal">execute__tree__.restore.ipsuserdefsig_ftp</span> </li>
        <li><span class="li-normal">execute__tree__.set.system.session.filter.clear_expire</span> </li>
        <li><span class="li-normal">system_ips-urlfilter-dns6</span>  <span class="li-required">param: address6</span>  <span class="li-required">type: str</span></li>
        <li><span class="li-normal">execute__tree__.extender_restart-fortiextender-daemon</span> </li>
        <li><span class="li-normal">diagnose__tree___geoip</span> </li>
        <li><span class="li-normal">execute__tree__.vpn.certificate.remote.import_tftp</span> </li>
        <li><span class="li-normal">execute__tree__.restore.config_dhcp</span> </li>
        <li><span class="li-normal">report_style</span>  <span class="li-required">param: name</span>  <span class="li-required">type: str</span></li>
        <li><span class="li-normal">wireless-controller_wtp</span>  <span class="li-required">param: wtp_id</span>  <span class="li-required">type: str</span></li>
        <li><span class="li-normal">execute__tree__.log_upload-progress</span> </li>
        <li><span class="li-normal">execute__tree__.switch-controller.get-physical-conn_standard</span> </li>
        <li><span class="li-normal">diagnose__tree__.ips_session</span> </li>
        <li><span class="li-normal">execute__tree___shutdown</span> </li>
        <li><span class="li-normal">system_ipip-tunnel</span>  <span class="li-required">param: name</span>  <span class="li-required">type: str</span></li>
        <li><span class="li-normal">system.dhcp6_server</span>  <span class="li-required">param: id</span>  <span class="li-required">type: int</span></li>
        <li><span class="li-normal">execute__tree__.restore.script_lastlog</span> </li>
        <li><span class="li-normal">execute__tree__.webcache.delete_status</span> </li>
        <li><span class="li-normal">execute__tree__.revision.delete_config</span> </li>
        <li><span class="li-normal">execute__tree__.switch-controller.get-sync-status_name </span> </li>
        <li><span class="li-normal">firewall_multicast-policy</span>  <span class="li-required">param: id</span>  <span class="li-required">type: int</span></li>
        <li><span class="li-normal">execute__tree__.vpn.certificate.local.generate_default-ssl-ca-untrusted</span> </li>
        <li><span class="li-normal">system_modem</span> </li>
        <li><span class="li-normal">router_rip</span> </li>
        <li><span class="li-normal">execute__tree__.vpn.sslvpn_rlist</span> </li>
        <li><span class="li-normal">diagnose__tree__.ips_ssl</span> </li>
        <li><span class="li-normal">diagnose__tree___fortiguard</span> </li>
        <li><span class="li-normal">execute__tree__.set.system.session.filter.negate_dst</span> </li>
        <li><span class="li-normal">execute__tree__.vpn.sslvpn_list</span> </li>
        <li><span class="li-normal">system_password-policy</span> </li>
        <li><span class="li-normal">diagnose__tree___settings</span> </li>
        <li><span class="li-normal">switch-controller_virtual-port-pool</span>  <span class="li-required">param: name</span>  <span class="li-required">type: str</span></li>
        <li><span class="li-normal">wireless-controller_setting</span> </li>
        <li><span class="li-normal">router_static6</span>  <span class="li-required">param: seq_num</span>  <span class="li-required">type: int</span></li>
        <li><span class="li-normal">wireless-controller.hotspot20_anqp-ip-address-type</span>  <span class="li-required">param: name</span>  <span class="li-required">type: str</span></li>
        <li><span class="li-normal">firewall_vipgrp</span>  <span class="li-required">param: name</span>  <span class="li-required">type: str</span></li>
        <li><span class="li-normal">switch-controller_switch-profile</span>  <span class="li-required">param: name</span>  <span class="li-required">type: str</span></li>
        <li><span class="li-normal">execute__tree___formatlogdisk</span> </li>
        <li><span class="li-normal">system_switch-interface</span>  <span class="li-required">param: name</span>  <span class="li-required">type: str</span></li>
        <li><span class="li-normal">router_isis</span> </li>
        <li><span class="li-normal">firewall_policy</span>  <span class="li-required">param: policyid</span>  <span class="li-required">type: int</span></li>
        <li><span class="li-normal">log.syslogd_override-setting</span> </li>
        <li><span class="li-normal">execute__tree__.set.system.session.filter_src</span> </li>
        <li><span class="li-normal">system_lte-modem</span> </li>
        <li><span class="li-normal">execute__tree__.ping6-options_pattern</span> </li>
        <li><span class="li-normal">execute__tree___reboot</span> </li>
        <li><span class="li-normal">webfilter_content</span>  <span class="li-required">param: id</span>  <span class="li-required">type: int</span></li>
        <li><span class="li-normal">firewall_vipgrp6</span>  <span class="li-required">param: name</span>  <span class="li-required">type: str</span></li>
        <li><span class="li-normal">execute__tree__.switch-controller.virtual-port-pool_show-by-pool</span> </li>
        <li><span class="li-normal">diagnose__tree__.netlink_aggregate</span> </li>
        <li><span class="li-normal">execute__tree___telnet</span> </li>
        <li><span class="li-normal">execute__tree__.modem_dial</span> </li>
        <li><span class="li-normal">firewall.schedule_onetime</span>  <span class="li-required">param: name</span>  <span class="li-required">type: str</span></li>
        <li><span class="li-normal">antivirus_profile</span>  <span class="li-required">param: name</span>  <span class="li-required">type: str</span></li>
        <li><span class="li-normal">log.fortianalyzer_setting</span> </li>
        <li><span class="li-normal">execute__tree__.restore.other-objects_tftp</span> </li>
        <li><span class="li-normal">execute__tree__.backup.full-config_tftp</span> </li>
        <li><span class="li-normal">firewall_ippool6</span>  <span class="li-required">param: name</span>  <span class="li-required">type: str</span></li>
        <li><span class="li-normal">execute__tree__.ping-options_interface</span> </li>
        <li><span class="li-normal">execute__tree__.backup.config-with-forticlient-info_tftp</span> </li>
        <li><span class="li-normal">system_central-management</span> </li>
        <li><span class="li-normal">execute__tree__.cfg_save</span> </li>
        <li><span class="li-normal">system.replacemsg_http</span>  <span class="li-required">param: msg_type</span>  <span class="li-required">type: str</span></li>
        <li><span class="li-normal">execute__tree__.ping6-options_repeat-count</span> </li>
        <li><span class="li-normal">diagnose__tree__.ips.debug_disable</span> </li>
        <li><span class="li-normal">diagnose__tree__.ips_memory</span> </li>
        <li><span class="li-normal">diagnose__tree__.ips.debug_enable</span> </li>
        <li><span class="li-normal">system_zone</span>  <span class="li-required">param: name</span>  <span class="li-required">type: str</span></li>
        <li><span class="li-normal">system_vdom-dns</span> </li>
        <li><span class="li-normal">execute__tree__.fortiguard-log_domain</span> </li>
        <li><span class="li-normal">execute__tree__.batch_start</span> </li>
        <li><span class="li-normal">firewall_multicast-address</span>  <span class="li-required">param: name</span>  <span class="li-required">type: str</span></li>
        <li><span class="li-normal">wireless-controller_wtp-profile</span>  <span class="li-required">param: name</span>  <span class="li-required">type: str</span></li>
        <li><span class="li-normal">execute__tree__.vpn.sslvpn_rdel-all-tunnel</span> </li>
        <li><span class="li-normal">execute__tree__.log.filter_reset</span> </li>
        <li><span class="li-normal">vpn.ssl_settings</span> </li>
        <li><span class="li-normal">router_ospf</span> </li>
        <li><span class="li-normal">switch-controller.qos_queue-policy</span>  <span class="li-required">param: name</span>  <span class="li-required">type: str</span></li>
        <li><span class="li-normal">execute__tree__.set.system.session.filter.negate_vd</span> </li>
        <li><span class="li-normal">execute__tree__.log_detail</span> </li>
        <li><span class="li-normal">execute__tree__.restore.config_usb</span> </li>
        <li><span class="li-normal">execute__tree__.auto-script_start</span> </li>
        <li><span class="li-normal">execute__tree___ping6</span> </li>
        <li><span class="li-normal">execute__tree___update-ips</span> </li>
        <li><span class="li-normal">execute__tree__.vpn.sslvpn_del-web</span> </li>
        <li><span class="li-normal">diagnose__tree__.netlink_redundant</span> </li>
        <li><span class="li-normal">diagnose__tree__.vpn_tunnel</span> </li>
        <li><span class="li-normal">ftp-proxy_explicit</span> </li>
        <li><span class="li-normal">execute__tree__.router.clear.bgp_dampening</span> </li>
        <li><span class="li-normal">user_device-group</span>  <span class="li-required">param: name</span>  <span class="li-required">type: str</span></li>
        <li><span class="li-normal">execute__tree__.backup.disk.alllogs_ftp</span> </li>
        <li><span class="li-normal">execute__tree__.report_run</span> </li>
        <li><span class="li-normal">execute__tree__.set.system.session.filter_vd</span> </li>
        <li><span class="li-normal">execute__tree__.extender_push-fortiextender-image</span> </li>
        <li><span class="li-normal">vpn.certificate_crl</span>  <span class="li-required">param: name</span>  <span class="li-required">type: str</span></li>
        <li><span class="li-normal">execute__tree__.switch-controller.virtual-port-pool_return</span> </li>
        <li><span class="li-normal">execute__tree__.cli_status-msg-only</span> </li>
        <li><span class="li-normal">user_local</span>  <span class="li-required">param: name</span>  <span class="li-required">type: str</span></li>
        <li><span class="li-normal">execute__tree__.set.system.session.filter_dport</span> </li>
        <li><span class="li-normal">webfilter_profile</span>  <span class="li-required">param: name</span>  <span class="li-required">type: str</span></li>
        <li><span class="li-normal">switch-controller_storm-control</span> </li>
        <li><span class="li-normal">execute__tree__.log.filter_ha-member</span> </li>
        <li><span class="li-normal">firewall_ssl-ssh-profile</span>  <span class="li-required">param: name</span>  <span class="li-required">type: str</span></li>
        <li><span class="li-normal">execute__tree__.dhcp6_lease-clear</span> </li>
        <li><span class="li-normal">execute__tree__.central-mgmt_unregister-device</span> </li>
        <li><span class="li-normal">execute__tree__.mrouter.clear_statistics</span> </li>
        <li><span class="li-normal">execute__tree__.switch-controller.get-sync-status_all</span> </li>
        <li><span class="li-normal">execute__tree__.cfg_reload</span> </li>
        <li><span class="li-normal">log.disk_setting</span> </li>
        <li><span class="li-normal">dlp_filepattern</span>  <span class="li-required">param: id</span>  <span class="li-required">type: int</span></li>
        <li><span class="li-normal">execute__tree__.ping-options_view-settings</span> </li>
        <li><span class="li-normal">firewall_ippool</span>  <span class="li-required">param: name</span>  <span class="li-required">type: str</span></li>
        <li><span class="li-normal">web-proxy_url-match</span>  <span class="li-required">param: name</span>  <span class="li-required">type: str</span></li>
        <li><span class="li-normal">execute__tree__.restore.secondary-image_tftp</span> </li>
        <li><span class="li-normal">dlp_fp-sensitivity</span>  <span class="li-required">param: name</span>  <span class="li-required">type: str</span></li>
        <li><span class="li-normal">execute__tree__.fortitoken.import_tftp</span> </li>
        <li><span class="li-normal">system_interface</span>  <span class="li-required">param: name</span>  <span class="li-required">type: str</span></li>
        <li><span class="li-normal">diagnose__tree___log</span> </li>
        <li><span class="li-normal">execute__tree__.cli_check-template-status</span> </li>
        <li><span class="li-normal">system_virtual-wire-pair</span>  <span class="li-required">param: name</span>  <span class="li-required">type: str</span></li>
        <li><span class="li-normal">execute__tree___factoryreset</span> </li>
        <li><span class="li-normal">diagnose__tree__.ips.av_cache</span> </li>
        <li><span class="li-normal">system.replacemsg_webproxy</span>  <span class="li-required">param: msg_type</span>  <span class="li-required">type: str</span></li>
        <li><span class="li-normal">execute__tree__.restore.ips_ftp</span> </li>
        <li><span class="li-normal">diagnose__tree___debug</span> </li>
        <li><span class="li-normal">execute__tree__.ping-options_validate-reply</span> </li>
        <li><span class="li-normal">execute__tree__.ping-options_timeout</span> </li>
        <li><span class="li-normal">user_password-policy</span>  <span class="li-required">param: name</span>  <span class="li-required">type: str</span></li>
        <li><span class="li-normal">switch-controller.qos_qos-policy</span>  <span class="li-required">param: name</span>  <span class="li-required">type: str</span></li>
        <li><span class="li-normal">execute__tree__.extender_dial</span> </li>
        <li><span class="li-normal">diagnose__tree__.ips.debug_status</span> </li>
        <li><span class="li-normal">wireless-controller_inter-controller</span> </li>
        <li><span class="li-normal">execute__tree__.set.system.session.filter.negate_dport</span> </li>
        <li><span class="li-normal">diagnose__tree__.vpn_ocvpn</span> </li>
        <li><span class="li-normal">execute__tree__.switch-controller.stage-tiered-swtp-image_sn</span> </li>
        <li><span class="li-normal">execute__tree__.log_delete</span> </li>
        <li><span class="li-normal">log.syslogd4_setting</span> </li>
        <li><span class="li-normal">execute__tree__.backup.config_ftp</span> </li>
        <li><span class="li-normal">execute__tree__.switch-controller_factory-reset</span> </li>
        <li><span class="li-normal">switch-controller_switch-group</span>  <span class="li-required">param: name</span>  <span class="li-required">type: str</span></li>
        <li><span class="li-normal">execute__tree__.log.filter_max-checklines</span> </li>
        <li><span class="li-normal">user_fsso</span>  <span class="li-required">param: name</span>  <span class="li-required">type: str</span></li>
        <li><span class="li-normal">diagnose__tree__.ips_dissector</span> </li>
        <li><span class="li-normal">firewall_vipgrp64</span>  <span class="li-required">param: name</span>  <span class="li-required">type: str</span></li>
        <li><span class="li-normal">execute__tree__.restore.config.management-station_script</span> </li>
        <li><span class="li-normal">user_quarantine</span> </li>
        <li><span class="li-normal">system_ips-urlfilter-dns</span>  <span class="li-required">param: address</span>  <span class="li-required">type: str</span></li>
        <li><span class="li-normal">execute__tree__.restore.image_usb</span> </li>
        <li><span class="li-normal">system_fm</span> </li>
        <li><span class="li-normal">execute__tree__.firewall.ssh.generate_local-ca</span> </li>
        <li><span class="li-normal">system_global</span> </li>
        <li><span class="li-normal">wireless-controller.hotspot20_anqp-nai-realm</span>  <span class="li-required">param: name</span>  <span class="li-required">type: str</span></li>
        <li><span class="li-normal">diagnose__tree___extender</span> </li>
        <li><span class="li-normal">execute__tree__.auto-script_result</span> </li>
        <li><span class="li-normal">execute__tree__.switch-controller_loop-guard-reset</span> </li>
        <li><span class="li-normal">system_physical-switch</span>  <span class="li-required">param: name</span>  <span class="li-required">type: str</span></li>
        <li><span class="li-normal">execute__tree__.restore.script_ftp</span> </li>
        <li><span class="li-normal">execute__tree__.ping-options_pattern</span> </li>
        <li><span class="li-normal">execute__tree__.backup.ipsuserdefsig_tftp</span> </li>
        <li><span class="li-normal">execute__tree__.switch-controller_clear-802-1X-interface</span> </li>
        <li><span class="li-normal">execute__tree__.log_delete-all</span> </li>
        <li><span class="li-normal">log.fortianalyzer3_setting</span> </li>
        <li><span class="li-normal">execute__tree__.nsx.group_import</span> </li>
        <li><span class="li-normal">firewall_vip</span>  <span class="li-required">param: name</span>  <span class="li-required">type: str</span></li>
        <li><span class="li-normal">system_virtual-switch</span>  <span class="li-required">param: name</span>  <span class="li-required">type: str</span></li>
        <li><span class="li-normal">execute__tree___traceroute</span> </li>
        <li><span class="li-normal">diagnose__tree__.ip.router_bfd</span> </li>
        <li><span class="li-normal">diagnose__tree__.snmp_ip</span> </li>
        <li><span class="li-normal">execute__tree__.router.clear.bgp_ipv6</span> </li>
        <li><span class="li-normal">execute__tree__.wireless-controller.hs20-icon.upload-icon_tftp</span> </li>
        <li><span class="li-normal">execute__tree__.set.system.session.filter.clear_all</span> </li>
        <li><span class="li-normal">wanopt_auth-group</span>  <span class="li-required">param: name</span>  <span class="li-required">type: str</span></li>
        <li><span class="li-normal">wanopt_webcache</span> </li>
        <li><span class="li-normal">system.snmp_user</span>  <span class="li-required">param: name</span>  <span class="li-required">type: str</span></li>
        <li><span class="li-normal">firewall_ip-translation</span>  <span class="li-required">param: transid</span>  <span class="li-required">type: int</span></li>
        <li><span class="li-normal">system_settings</span> </li>
        <li><span class="li-normal">log.fortianalyzer2_setting</span> </li>
        <li><span class="li-normal">execute__tree__.batch_lastlog</span> </li>
        <li><span class="li-normal">wireless-controller_vap</span>  <span class="li-required">param: name</span>  <span class="li-required">type: str</span></li>
        <li><span class="li-normal">execute__tree__.router.clear.bfd_session</span> </li>
        <li><span class="li-normal">execute__tree__.webfilter_quota-reset</span> </li>
        <li><span class="li-normal">diagnose__tree__.ips.config_disable</span> </li>
        <li><span class="li-normal">diagnose__tree__.netlink_dstmac</span> </li>
        <li><span class="li-normal">wanopt_cache-service</span> </li>
        <li><span class="li-normal">execute__tree__.upload.config_tftp</span> </li>
        <li><span class="li-normal">execute__tree__.usb-device_disconnect</span> </li>
        <li><span class="li-normal">switch-controller_switch-log</span> </li>
        <li><span class="li-normal">execute__tree__.vpn.certificate.ca.import_bundle</span> </li>
        <li><span class="li-normal">firewall_internet-service-group</span>  <span class="li-required">param: name</span>  <span class="li-required">type: str</span></li>
        <li><span class="li-normal">system.replacemsg_mail</span>  <span class="li-required">param: msg_type</span>  <span class="li-required">type: str</span></li>
        <li><span class="li-normal">execute__tree__.set.system.session.filter.negate_policy</span> </li>
        <li><span class="li-normal">system_replacemsg-image</span>  <span class="li-required">param: name</span>  <span class="li-required">type: str</span></li>
        <li><span class="li-normal">execute__tree__.set.system.session.filter.clear_src</span> </li>
        <li><span class="li-normal">diagnose__tree__.ips_dac</span> </li>
        <li><span class="li-normal">diagnose__tree___sys</span> </li>
        <li><span class="li-normal">diagnose__tree___npu</span> </li>
        <li><span class="li-normal">execute__tree__.router.clear.bgp_external</span> </li>
        <li><span class="li-normal">execute__tree__.upload.image_ftp</span> </li>
        <li><span class="li-normal">antivirus_quarantine</span> </li>
        <li><span class="li-normal">diagnose__tree___security-rating</span> </li>
        <li><span class="li-normal">execute__tree__.fortitoken-mobile_provision</span> </li>
        <li><span class="li-normal">vpn.certificate_ca</span>  <span class="li-required">param: name</span>  <span class="li-required">type: str</span></li>
        <li><span class="li-normal">endpoint-control_forticlient-registration-sync</span>  <span class="li-required">param: peer_name</span>  <span class="li-required">type: str</span></li>
        <li><span class="li-normal">system_sdn-connector</span>  <span class="li-required">param: name</span>  <span class="li-required">type: str</span></li>
        <li><span class="li-normal">vpn.ssl.web_user-group-bookmark</span>  <span class="li-required">param: name</span>  <span class="li-required">type: str</span></li>
        <li><span class="li-normal">endpoint-control_settings</span> </li>
        <li><span class="li-normal">log.null-device_filter</span> </li>
        <li><span class="li-normal">dlp_settings</span> </li>
        <li><span class="li-normal">execute__tree__.fortiguard-log_agreement</span> </li>
        <li><span class="li-normal">wireless-controller_utm-profile</span>  <span class="li-required">param: name</span>  <span class="li-required">type: str</span></li>
        <li><span class="li-normal">execute__tree__.vpn.certificate.ca.import_auto</span> </li>
        <li><span class="li-normal">router_aspath-list</span>  <span class="li-required">param: name</span>  <span class="li-required">type: str</span></li>
        <li><span class="li-normal">firewall.schedule_group</span>  <span class="li-required">param: name</span>  <span class="li-required">type: str</span></li>
        <li><span class="li-normal">execute__tree__.modem_trigger</span> </li>
        <li><span class="li-normal">diagnose__tree__.netlink_backlog</span> </li>
        <li><span class="li-normal">system_dscp-based-priority</span>  <span class="li-required">param: id</span>  <span class="li-required">type: int</span></li>
        <li><span class="li-normal">icap_server</span>  <span class="li-required">param: name</span>  <span class="li-required">type: str</span></li>
        <li><span class="li-normal">vpn.ipsec_phase1-interface</span>  <span class="li-required">param: name</span>  <span class="li-required">type: str</span></li>
        <li><span class="li-normal">authentication_scheme</span>  <span class="li-required">param: name</span>  <span class="li-required">type: str</span></li>
        <li><span class="li-normal">execute__tree__.fsso_refresh</span> </li>
        <li><span class="li-normal">execute__tree__.clear.system.arp_table</span> </li>
        <li><span class="li-normal">diagnose__tree__.ip_route</span> </li>
        <li><span class="li-normal">log.fortianalyzer3_filter</span> </li>
        <li><span class="li-normal">system_email-server</span> </li>
        <li><span class="li-normal">diagnose__tree__.test_authserver</span> </li>
        <li><span class="li-normal">wireless-controller_ap-status</span>  <span class="li-required">param: id</span>  <span class="li-required">type: int</span></li>
        <li><span class="li-normal">application_list</span>  <span class="li-required">param: name</span>  <span class="li-required">type: str</span></li>
        <li><span class="li-normal">execute__tree__.switch-controller.stage-tiered-swtp-image_switch-group</span> </li>
        <li><span class="li-normal">execute__tree__.restore.src-vis_ftp</span> </li>
        <li><span class="li-normal">diagnose__tree__.ip_framed-ip</span> </li>
        <li><span class="li-normal">diagnose__tree___wadbd</span> </li>
        <li><span class="li-normal">vpn.ssl.web_user-bookmark</span>  <span class="li-required">param: name</span>  <span class="li-required">type: str</span></li>
        <li><span class="li-normal">execute__tree__.log_flush-cache-all</span> </li>
        <li><span class="li-normal">execute__tree__.set.system.session.filter.negate_src</span> </li>
        <li><span class="li-normal">execute__tree___ssh</span> </li>
        <li><span class="li-normal">firewall.shaper_traffic-shaper</span>  <span class="li-required">param: name</span>  <span class="li-required">type: str</span></li>
        <li><span class="li-normal">system_management-tunnel</span> </li>
        <li><span class="li-normal">system_csf</span> </li>
        <li><span class="li-normal">execute__tree__.fortiguard-log_certificate-activation</span> </li>
        <li><span class="li-normal">execute__tree__.auto-script.backup_tftp</span> </li>
        <li><span class="li-normal">execute__tree__.log_roll</span> </li>
        <li><span class="li-normal">firewall.shaper_per-ip-shaper</span>  <span class="li-required">param: name</span>  <span class="li-required">type: str</span></li>
        <li><span class="li-normal">execute__tree__.backup.disk.ipsarchives_tftp</span> </li>
        <li><span class="li-normal">execute__tree__.usb-disk_rename</span> </li>
        <li><span class="li-normal">execute__tree__.disk_scan</span> </li>
        <li><span class="li-normal">execute__tree__.report-config_reset</span> </li>
        <li><span class="li-normal">dnsfilter_profile</span>  <span class="li-required">param: name</span>  <span class="li-required">type: str</span></li>
        <li><span class="li-normal">execute__tree__.set.system.session.filter_dst</span> </li>
        <li><span class="li-normal">execute__tree__.backup.disk.log_usb</span> </li>
        <li><span class="li-normal">user_device-access-list</span>  <span class="li-required">param: name</span>  <span class="li-required">type: str</span></li>
        <li><span class="li-normal">system_ha-monitor</span> </li>
        <li><span class="li-normal">execute__tree__.fortitoken-mobile_poll</span> </li>
        <li><span class="li-normal">execute__tree__.restore.secondary-image_ftp</span> </li>
        <li><span class="li-normal">wireless-controller.hotspot20_anqp-venue-name</span>  <span class="li-required">param: name</span>  <span class="li-required">type: str</span></li>
        <li><span class="li-normal">system.snmp_sysinfo</span> </li>
        <li><span class="li-normal">diagnose__tree__.netlink_brctl</span> </li>
        <li><span class="li-normal">execute__tree__.traceroute-options_view-settings</span> </li>
        <li><span class="li-normal">execute__tree__.restore.av_tftp</span> </li>
        <li><span class="li-normal">diagnose__tree___fortitoken</span> </li>
        <li><span class="li-normal">application_custom</span>  <span class="li-required">param: tag</span>  <span class="li-required">type: str</span></li>
        <li><span class="li-normal">execute__tree__.wireless-controller_reset-wtp</span> </li>
        <li><span class="li-normal">system_api-user</span>  <span class="li-required">param: name</span>  <span class="li-required">type: str</span></li>
        <li><span class="li-normal">ips_rule</span>  <span class="li-required">param: name</span>  <span class="li-required">type: str</span></li>
        <li><span class="li-normal">spamfilter_fortishield</span> </li>
        <li><span class="li-normal">system_npu</span> </li>
        <li><span class="li-normal">execute__tree__.switch-controller.restart-swtp-delayed_sn</span> </li>
        <li><span class="li-normal">system_netflow</span> </li>
        <li><span class="li-normal">execute__tree__.set.system.session.filter_duration</span> </li>
        <li><span class="li-normal">vpn.ipsec_forticlient</span>  <span class="li-required">param: realm</span>  <span class="li-required">type: str</span></li>
        <li><span class="li-normal">system_automation-trigger</span>  <span class="li-required">param: name</span>  <span class="li-required">type: str</span></li>
        <li><span class="li-normal">firewall_policy64</span>  <span class="li-required">param: policyid</span>  <span class="li-required">type: int</span></li>
        <li><span class="li-normal">wireless-controller.hotspot20_h2qp-osu-provider</span>  <span class="li-required">param: name</span>  <span class="li-required">type: str</span></li>
        <li><span class="li-normal">application_name</span>  <span class="li-required">param: name</span>  <span class="li-required">type: str</span></li>
        <li><span class="li-normal">diagnose__tree__.ip_gre-tunnel</span> </li>
        <li><span class="li-normal">execute__tree__.restore.ipsuserdefsig_tftp</span> </li>
        <li><span class="li-normal">firewall.service_custom</span>  <span class="li-required">param: name</span>  <span class="li-required">type: str</span></li>
        <li><span class="li-normal">spamfilter_iptrust</span>  <span class="li-required">param: id</span>  <span class="li-required">type: int</span></li>
        <li><span class="li-normal">system_mobile-tunnel</span>  <span class="li-required">param: name</span>  <span class="li-required">type: str</span></li>
        <li><span class="li-normal">firewall_ttl-policy</span>  <span class="li-required">param: id</span>  <span class="li-required">type: int</span></li>
        <li><span class="li-normal">execute__tree__.central-mgmt_set-mgmt-id</span> </li>
        <li><span class="li-normal">system.replacemsg_utm</span>  <span class="li-required">param: msg_type</span>  <span class="li-required">type: str</span></li>
        <li><span class="li-normal">execute__tree__.log.filter_view-lines</span> </li>
        <li><span class="li-normal">vpn_pptp</span> </li>
        <li><span class="li-normal">execute__tree__.traceroute-options_device</span> </li>
        <li><span class="li-normal">diagnose__tree__.ip_address</span> </li>
        <li><span class="li-normal">wireless-controller.hotspot20_hs-profile</span>  <span class="li-required">param: name</span>  <span class="li-required">type: str</span></li>
        <li><span class="li-normal">log.webtrends_setting</span> </li>
        <li><span class="li-normal">execute__tree__.switch-controller_stage-swtp-image</span> </li>
        <li><span class="li-normal">firewall_local-in-policy</span>  <span class="li-required">param: policyid</span>  <span class="li-required">type: int</span></li>
        <li><span class="li-normal">execute__tree__.vpn.sslvpn_rdel-all</span> </li>
        <li><span class="li-normal">execute__tree__.restore.image_management-station</span> </li>
        <li><span class="li-normal">diagnose__tree__.netlink_interface</span> </li>
        <li><span class="li-normal">execute__tree___upd-vd-license</span> </li>
        <li><span class="li-normal">switch-controller.qos_dot1p-map</span>  <span class="li-required">param: name</span>  <span class="li-required">type: str</span></li>
        <li><span class="li-normal">firewall_multicast-policy6</span>  <span class="li-required">param: id</span>  <span class="li-required">type: int</span></li>
        <li><span class="li-normal">execute__tree__.switch-controller.upload-swtp-image_tftp</span> </li>
        <li><span class="li-normal">execute__tree__.restore.src-vis_tftp</span> </li>
        <li><span class="li-normal">execute__tree__.switch-controller.virtual-port-pool_show-by-property</span> </li>
        <li><span class="li-normal">diagnose__tree___firewall</span> </li>
        <li><span class="li-normal">wanopt_content-delivery-network-rule</span>  <span class="li-required">param: name</span>  <span class="li-required">type: str</span></li>
        <li><span class="li-normal">execute__tree__.log.filter_category</span> </li>
        <li><span class="li-normal">execute__tree__.switch-controller.virtual-port-pool_show-by-tag</span> </li>
        <li><span class="li-normal">system_dns-database</span>  <span class="li-required">param: name</span>  <span class="li-required">type: str</span></li>
        <li><span class="li-normal">diagnose__tree__.ip_arp</span> </li>
        <li><span class="li-normal">execute__tree__.log.filter_show-utm-ref</span> </li>
        <li><span class="li-normal">waf_main-class</span>  <span class="li-required">param: id</span>  <span class="li-required">type: int</span></li>
        <li><span class="li-normal">execute__tree__.switch-controller.restart-swtp_sn</span> </li>
        <li><span class="li-normal">system.replacemsg_nac-quar</span>  <span class="li-required">param: msg_type</span>  <span class="li-required">type: str</span></li>
        <li><span class="li-normal">system_vdom-radius-server</span>  <span class="li-required">param: name</span>  <span class="li-required">type: str</span></li>
        <li><span class="li-normal">system_vdom</span>  <span class="li-required">param: name</span>  <span class="li-required">type: str</span></li>
        <li><span class="li-normal">execute__tree__.ping-options_ttl</span> </li>
        <li><span class="li-normal">execute__tree__.traceroute-options_queries</span> </li>
        <li><span class="li-normal">execute__tree__.auto-script_status</span> </li>
        <li><span class="li-normal">user_tacacs+</span>  <span class="li-required">param: name</span>  <span class="li-required">type: str</span></li>
        <li><span class="li-normal">wanopt_peer</span>  <span class="li-required">param: peer_host_id</span>  <span class="li-required">type: str</span></li>
        <li><span class="li-normal">log.syslogd3_setting</span> </li>
        <li><span class="li-normal">execute__tree__.extender_hangup</span> </li>
        <li><span class="li-normal">diagnose__tree___web-ui</span> </li>
        <li><span class="li-normal">report_dataset</span>  <span class="li-required">param: name</span>  <span class="li-required">type: str</span></li>
        <li><span class="li-normal">execute__tree__.fortitoken-mobile_renew</span> </li>
        <li><span class="li-normal">webfilter_ftgd-local-cat</span>  <span class="li-required">param: desc</span>  <span class="li-required">type: str</span></li>
        <li><span class="li-normal">router_multicast6</span> </li>
        <li><span class="li-normal">vpn.certificate_remote</span>  <span class="li-required">param: name</span>  <span class="li-required">type: str</span></li>
        <li><span class="li-normal">execute__tree__.backup.config-with-forticlient-info_ftp</span> </li>
        <li><span class="li-normal">execute__tree__.vpn.ipsec.tunnel_up</span> </li>
        <li><span class="li-normal">diagnose__tree__.ip.router_ospf</span> </li>
        <li><span class="li-normal">execute__tree___send-fds-statistics</span> </li>
        <li><span class="li-normal">diagnose__tree__.vpn_pptp</span> </li>
        <li><span class="li-normal">system_fips-cc</span> </li>
        <li><span class="li-normal">execute__tree__.restore.image_flash</span> </li>
        <li><span class="li-normal">execute__tree__.log.filter_device</span> </li>
        <li><span class="li-normal">system_ha</span> </li>
        <li><span class="li-normal">log.syslogd3_filter</span> </li>
        <li><span class="li-normal">diagnose__tree___internet-service</span> </li>
        <li><span class="li-normal">user_radius</span>  <span class="li-required">param: name</span>  <span class="li-required">type: str</span></li>
        <li><span class="li-normal">execute__tree__.log.fortiguard_test-connectivity</span> </li>
        <li><span class="li-normal">firewall_DoS-policy6</span>  <span class="li-required">param: policyid</span>  <span class="li-required">type: int</span></li>
        <li><span class="li-normal">execute__tree___date</span> </li>
        <li><span class="li-normal">execute__tree__.restore.ips_tftp</span> </li>
        <li><span class="li-normal">execute__tree__.dhcp_lease-list</span> </li>
        <li><span class="li-normal">system_tos-based-priority</span>  <span class="li-required">param: id</span>  <span class="li-required">type: int</span></li>
        <li><span class="li-normal">execute__tree__.api-user_generate-key</span> </li>
        <li><span class="li-normal">diagnose__tree__.ipv6_address</span> </li>
        <li><span class="li-normal">vpn.certificate_local</span>  <span class="li-required">param: name</span>  <span class="li-required">type: str</span></li>
        <li><span class="li-normal">system_accprofile</span>  <span class="li-required">param: name</span>  <span class="li-required">type: str</span></li>
        <li><span class="li-normal">execute__tree___erase-disk</span> </li>
        <li><span class="li-normal">wireless-controller_global</span> </li>
        <li><span class="li-normal">log.syslogd_filter</span> </li>
        <li><span class="li-normal">execute__tree__.mrouter.clear_sparse-routes</span> </li>
        <li><span class="li-normal">execute__tree__.switch-controller.virtual-port-pool_request</span> </li>
        <li><span class="li-normal">execute__tree__.ping-options_repeat-count</span> </li>
        <li><span class="li-normal">dlp_sensor</span>  <span class="li-required">param: name</span>  <span class="li-required">type: str</span></li>
        <li><span class="li-normal">execute__tree__.fortiguard-log_update</span> </li>
        <li><span class="li-normal">log.syslogd2_filter</span> </li>
        <li><span class="li-normal">wireless-controller_ble-profile</span>  <span class="li-required">param: name</span>  <span class="li-required">type: str</span></li>
        <li><span class="li-normal">system_password-policy-guest-admin</span> </li>
        <li><span class="li-normal">diagnose__tree__.ipv6.router_ospf</span> </li>
        <li><span class="li-normal">execute__tree__.vpn.certificate.local.generate_cmp</span> </li>
        <li><span class="li-normal">execute__tree__.switch-controller_delete-swtp-image</span> </li>
        <li><span class="li-normal">user_pop3</span>  <span class="li-required">param: name</span>  <span class="li-required">type: str</span></li>
        <li><span class="li-normal">execute__tree__.fortitoken_sync</span> </li>
        <li><span class="li-normal">execute__tree__.backup.disk.ipsarchives_ftp</span> </li>
        <li><span class="li-normal">execute__tree__.ha_disconnect</span> </li>
        <li><span class="li-normal">execute__tree__.switch-controller.restart-swtp_switch-group</span> </li>
        <li><span class="li-normal">execute__tree___update-av</span> </li>
        <li><span class="li-normal">switch-controller_system</span> </li>
        <li><span class="li-normal">execute__tree__.ha_manage</span> </li>
        <li><span class="li-normal">voip_profile</span>  <span class="li-required">param: name</span>  <span class="li-required">type: str</span></li>
        <li><span class="li-normal">vpn.ipsec_manualkey-interface</span>  <span class="li-required">param: name</span>  <span class="li-required">type: str</span></li>
        <li><span class="li-normal">execute__tree__.auto-script_stopall</span> </li>
        <li><span class="li-normal">diagnose__tree__.ips_filter</span> </li>
        <li><span class="li-normal">execute__tree__.batch_status</span> </li>
        <li><span class="li-normal">system_vdom-netflow</span> </li>
        <li><span class="li-normal">execute__tree__.set.system.session.filter.clear_duration</span> </li>
        <li><span class="li-normal">firewall.ipmacbinding_table</span>  <span class="li-required">param: seq_num</span>  <span class="li-required">type: int</span></li>
        <li><span class="li-normal">execute__tree__.usb-device_list</span> </li>
        <li><span class="li-normal">system_automation-destination</span>  <span class="li-required">param: name</span>  <span class="li-required">type: str</span></li>
        <li><span class="li-normal">dlp_fp-doc-source</span>  <span class="li-required">param: name</span>  <span class="li-required">type: str</span></li>
        <li><span class="li-normal">execute__tree__.router.clear.bgp_as</span> </li>
        <li><span class="li-normal">firewall_ldb-monitor</span>  <span class="li-required">param: name</span>  <span class="li-required">type: str</span></li>
        <li><span class="li-normal">firewall.ssh_host-key</span>  <span class="li-required">param: name</span>  <span class="li-required">type: str</span></li>
        <li><span class="li-normal">system_vdom-link</span>  <span class="li-required">param: name</span>  <span class="li-required">type: str</span></li>
        <li><span class="li-normal">system_admin</span>  <span class="li-required">param: name</span>  <span class="li-required">type: str</span></li>
        <li><span class="li-normal">execute__tree__.vpn.sslvpn_guirlist</span> </li>
        <li><span class="li-normal">router_ospf6</span> </li>
        <li><span class="li-normal">user_device</span>  <span class="li-required">param: alias</span>  <span class="li-required">type: str</span></li>
        <li><span class="li-normal">log.fortiguard_setting</span> </li>
        <li><span class="li-normal">execute__tree__.switch-controller_list-swtp-image</span> </li>
        <li><span class="li-normal">system.snmp_community</span>  <span class="li-required">param: id</span>  <span class="li-required">type: int</span></li>
        <li><span class="li-normal">execute__tree__.log.fortianalyzer_test-connectivity</span> </li>
        <li><span class="li-normal">execute__tree__.set.system.session.filter.clear_policy</span> </li>
        <li><span class="li-normal">ips_settings</span> </li>
        <li><span class="li-normal">log.syslogd_override-filter</span> </li>
        <li><span class="li-normal">diagnose__tree__.ipv6_multicast</span> </li>
        <li><span class="li-normal">system_vdom-exception</span>  <span class="li-required">param: id</span>  <span class="li-required">type: int</span></li>
        <li><span class="li-normal">system_wccp</span>  <span class="li-required">param: service_id</span>  <span class="li-required">type: str</span></li>
        <li><span class="li-normal">system_automation-stitch</span>  <span class="li-required">param: name</span>  <span class="li-required">type: str</span></li>
        <li><span class="li-normal">execute__tree__.log.filter_field</span> </li>
        <li><span class="li-normal">firewall_profile-protocol-options</span>  <span class="li-required">param: name</span>  <span class="li-required">type: str</span></li>
        <li><span class="li-normal">report_theme</span>  <span class="li-required">param: name</span>  <span class="li-required">type: str</span></li>
        <li><span class="li-normal">execute__tree__.backup.config-with-forticlient-info_usb-mode</span> </li>
        <li><span class="li-normal">diagnose__tree__.ipv6_sit-tunnel</span> </li>
        <li><span class="li-normal">firewall.ssh_local-key</span>  <span class="li-required">param: name</span>  <span class="li-required">type: str</span></li>
        <li><span class="li-normal">firewall_vip64</span>  <span class="li-required">param: name</span>  <span class="li-required">type: str</span></li>
        <li><span class="li-normal">web-proxy_wisp</span>  <span class="li-required">param: name</span>  <span class="li-required">type: str</span></li>
        <li><span class="li-normal">spamfilter_options</span> </li>
        <li><span class="li-normal">execute__tree__.forticlient_list</span> </li>
        <li><span class="li-normal">endpoint-control_forticlient-ems</span>  <span class="li-required">param: name</span>  <span class="li-required">type: str</span></li>
        <li><span class="li-normal">system_dns-server</span>  <span class="li-required">param: name</span>  <span class="li-required">type: str</span></li>
        <li><span class="li-normal">system.replacemsg_alertmail</span>  <span class="li-required">param: msg_type</span>  <span class="li-required">type: str</span></li>
        <li><span class="li-normal">log.fortiguard_override-filter</span> </li>
        <li><span class="li-normal">endpoint-control_client</span>  <span class="li-required">param: id</span>  <span class="li-required">type: int</span></li>
        <li><span class="li-normal">router_access-list6</span>  <span class="li-required">param: name</span>  <span class="li-required">type: str</span></li>
        <li><span class="li-normal">system_fortiguard</span> </li>
        <li><span class="li-normal">web-proxy_global</span> </li>
        <li><span class="li-normal">diagnose__tree__.ip.router_pim-dm</span> </li>
        <li><span class="li-normal">diagnose__tree__.test_guest</span> </li>
        <li><span class="li-normal">wanopt_profile</span>  <span class="li-required">param: name</span>  <span class="li-required">type: str</span></li>
        <li><span class="li-normal">execute__tree__.switch-controller_poe-reset</span> </li>
        <li><span class="li-normal">wireless-controller.hotspot20_anqp-3gpp-cellular</span>  <span class="li-required">param: name</span>  <span class="li-required">type: str</span></li>
        <li><span class="li-normal">execute__tree__.auto-script.backup_ftp</span> </li>
        <li><span class="li-normal">system.replacemsg_ec</span>  <span class="li-required">param: msg_type</span>  <span class="li-required">type: str</span></li>
        <li><span class="li-normal">switch-controller_vlan</span>  <span class="li-required">param: name</span>  <span class="li-required">type: str</span></li>
        <li><span class="li-normal">system_vxlan</span>  <span class="li-required">param: name</span>  <span class="li-required">type: str</span></li>
        <li><span class="li-normal">webfilter_search-engine</span>  <span class="li-required">param: name</span>  <span class="li-required">type: str</span></li>
        <li><span class="li-normal">system_ipv6-tunnel</span>  <span class="li-required">param: name</span>  <span class="li-required">type: str</span></li>
        <li><span class="li-normal">certificate_local</span>  <span class="li-required">param: name</span>  <span class="li-required">type: str</span></li>
        <li><span class="li-normal">diagnose__tree__.test_analytics-report</span> </li>
        <li><span class="li-normal">execute__tree__.ping6-options_tos</span> </li>
        <li><span class="li-normal">execute__tree__.backup.full-config_usb-mode</span> </li>
        <li><span class="li-normal">execute__tree___update-src-vis</span> </li>
        <li><span class="li-normal">execute__tree__.backup.disk.alllogs_usb</span> </li>
        <li><span class="li-normal">execute__tree___enter</span> </li>
        <li><span class="li-normal">user_fsso-polling</span>  <span class="li-required">param: id</span>  <span class="li-required">type: int</span></li>
        <li><span class="li-normal">system.dhcp_server</span>  <span class="li-required">param: id</span>  <span class="li-required">type: int</span></li>
        <li><span class="li-normal">report_chart</span>  <span class="li-required">param: name</span>  <span class="li-required">type: str</span></li>
        <li><span class="li-normal">vpn.certificate_setting</span> </li>
        <li><span class="li-normal">router_bfd6</span> </li>
        <li><span class="li-normal">execute__tree__.restore.vmlicense_tftp</span> </li>
        <li><span class="li-normal">system.replacemsg_nntp</span>  <span class="li-required">param: msg_type</span>  <span class="li-required">type: str</span></li>
        <li><span class="li-normal">execute__tree__.backup.full-config_ftp</span> </li>
        <li><span class="li-normal">execute__tree__.router.clear.bgp_all</span> </li>
        <li><span class="li-normal">firewall_proxy-policy</span>  <span class="li-required">param: policyid</span>  <span class="li-required">type: int</span></li>
        <li><span class="li-normal">diagnose__tree__.snmp_trap</span> </li>
        <li><span class="li-normal">system_dns</span> </li>
        <li><span class="li-normal">user_peergrp</span>  <span class="li-required">param: name</span>  <span class="li-required">type: str</span></li>
        <li><span class="li-normal">execute__tree__.upload.image_usb</span> </li>
        <li><span class="li-normal">execute__tree__.router.clear.bgp_ip</span> </li>
        <li><span class="li-normal">execute__tree__.set.system.session.filter.clear_vd</span> </li>
        <li><span class="li-normal">execute__tree__.ping-options_source</span> </li>
        <li><span class="li-normal">vpn.ipsec_concentrator</span>  <span class="li-required">param: name</span>  <span class="li-required">type: str</span></li>
        <li><span class="li-normal">execute__tree__.fortitoken_activate</span> </li>
        <li><span class="li-normal">ips_decoder</span>  <span class="li-required">param: name</span>  <span class="li-required">type: str</span></li>
        <li><span class="li-normal">dnsfilter_domain-filter</span>  <span class="li-required">param: id</span>  <span class="li-required">type: int</span></li>
        <li><span class="li-normal">execute__tree__.auto-script_stop</span> </li>
        <li><span class="li-normal">wireless-controller_vap-group</span>  <span class="li-required">param: name</span>  <span class="li-required">type: str</span></li>
        <li><span class="li-normal">execute__tree__.forticlient_info</span> </li>
        <li><span class="li-normal">diagnose__tree__.ip.router_pim-sm</span> </li>
        <li><span class="li-normal">system_affinity-interrupt</span>  <span class="li-required">param: id</span>  <span class="li-required">type: int</span></li>
        <li><span class="li-normal">firewall_shaping-profile</span>  <span class="li-required">param: profile_name</span>  <span class="li-required">type: str</span></li>
        <li><span class="li-normal">firewall_interface-policy6</span>  <span class="li-required">param: policyid</span>  <span class="li-required">type: int</span></li>
        <li><span class="li-normal">execute__tree__.switch-controller.stage-tiered-swtp-image_all</span> </li>
        <li><span class="li-normal">execute__tree__.revision.list_image</span> </li>
        <li><span class="li-normal">execute__tree__.vpn.certificate.local.generate_ec</span> </li>
        <li><span class="li-normal">vpn.ipsec_manualkey</span>  <span class="li-required">param: name</span>  <span class="li-required">type: str</span></li>
        <li><span class="li-normal">execute__tree__.upload.config_ftp</span> </li>
        <li><span class="li-normal">switch-controller_global</span> </li>
        <li><span class="li-normal">execute__tree___dsscc</span> </li>
        <li><span class="li-normal">router_setting</span> </li>
        <li><span class="li-normal">diagnose__tree___sniffer</span> </li>
        <li><span class="li-normal">system.replacemsg_admin</span>  <span class="li-required">param: msg_type</span>  <span class="li-required">type: str</span></li>
        <li><span class="li-normal">firewall.schedule_recurring</span>  <span class="li-required">param: name</span>  <span class="li-required">type: str</span></li>
        <li><span class="li-normal">execute__tree__.webcache.delete_wildcard</span> </li>
        <li><span class="li-normal">system_sit-tunnel</span>  <span class="li-required">param: name</span>  <span class="li-required">type: str</span></li>
        <li><span class="li-normal">system_arp-table</span>  <span class="li-required">param: id</span>  <span class="li-required">type: int</span></li>
        <li><span class="li-normal">switch-controller_lldp-settings</span> </li>
        <li><span class="li-normal">webfilter_content-header</span>  <span class="li-required">param: id</span>  <span class="li-required">type: int</span></li>
        <li><span class="li-normal">system_auto-install</span> </li>
        <li><span class="li-normal">execute__tree__.replace-device_fortiswitch</span> </li>
        <li><span class="li-normal">user_domain-controller</span>  <span class="li-required">param: name</span>  <span class="li-required">type: str</span></li>
        <li><span class="li-normal">router_multicast</span> </li>
        <li><span class="li-normal">firewall_ssl-server</span>  <span class="li-required">param: name</span>  <span class="li-required">type: str</span></li>
        <li><span class="li-normal">execute__tree__.ping6-options_adaptive-ping</span> </li>
        <li><span class="li-normal">system.replacemsg_traffic-quota</span>  <span class="li-required">param: msg_type</span>  <span class="li-required">type: str</span></li>
        <li><span class="li-normal">system_fortimanager</span> </li>
        <li><span class="li-normal">execute__tree__.restore.config_ftp</span> </li>
        <li><span class="li-normal">system_mac-address-table</span>  <span class="li-required">param: mac</span>  <span class="li-required">type: str</span></li>
        <li><span class="li-normal">log.fortianalyzer_filter</span> </li>
        <li><span class="li-normal">system_network-visibility</span> </li>
        <li><span class="li-normal">diagnose__tree__.ips_anomaly6</span> </li>
        <li><span class="li-normal">diagnose__tree__.ips_test</span> </li>
        <li><span class="li-normal">execute__tree__.router.clear.ospf_process</span> </li>
        <li><span class="li-normal">execute__tree__.backup.ipsuserdefsig_ftp</span> </li>
        <li><span class="li-normal">execute__tree__.ha_set-priority</span> </li>
        <li><span class="li-normal">execute__tree__.ping-options_interval</span> </li>
        <li><span class="li-normal">firewall_interface-policy</span>  <span class="li-required">param: policyid</span>  <span class="li-required">type: int</span></li>
        <li><span class="li-normal">execute__tree__.vpn.certificate.local.export_tftp</span> </li>
        <li><span class="li-normal">system.replacemsg_fortiguard-wf</span>  <span class="li-required">param: msg_type</span>  <span class="li-required">type: str</span></li>
        <li><span class="li-normal">execute__tree___time</span> </li>
        <li><span class="li-normal">wireless-controller_bonjour-profile</span>  <span class="li-required">param: name</span>  <span class="li-required">type: str</span></li>
        <li><span class="li-normal">execute__tree__.wireless-controller.hs20-icon.backup-icon_ftp</span> </li>
        <li><span class="li-normal">webfilter_urlfilter</span>  <span class="li-required">param: id</span>  <span class="li-required">type: int</span></li>
        <li><span class="li-normal">execute__tree__.revision.delete_image</span> </li>
        <li><span class="li-normal">execute__tree__.backup.memory.log_tftp</span> </li>
        <li><span class="li-normal">execute__tree__.switch-controller_bpdu-guard-reset</span> </li>
        <li><span class="li-normal">execute__tree__.ping6-options_timeout</span> </li>
        <li><span class="li-normal">diagnose__tree___report</span> </li>
        <li><span class="li-normal">system_probe-response</span> </li>
        <li><span class="li-normal">execute__tree__.nsx.group_list</span> </li>
        <li><span class="li-normal">wireless-controller.hotspot20_h2qp-operator-name</span>  <span class="li-required">param: name</span>  <span class="li-required">type: str</span></li>
        <li><span class="li-normal">diagnose__tree___user</span> </li>
        <li><span class="li-normal">switch-controller_sflow</span> </li>
        <li><span class="li-normal">execute__tree__.vpn.ipsec.tunnel_down</span> </li>
        <li><span class="li-normal">execute__tree__.backup.config_usb-mode</span> </li>
        <li><span class="li-normal">webfilter_fortiguard</span> </li>
        <li><span class="li-normal">wireless-controller.hotspot20_anqp-roaming-consortium</span>  <span class="li-required">param: name</span>  <span class="li-required">type: str</span></li>
        <li><span class="li-normal">diagnose__tree__.ips.config_enable</span> </li>
        <li><span class="li-normal">firewall_DoS-policy</span>  <span class="li-required">param: policyid</span>  <span class="li-required">type: int</span></li>
        <li><span class="li-normal">firewall_proxy-addrgrp</span>  <span class="li-required">param: name</span>  <span class="li-required">type: str</span></li>
        <li><span class="li-normal">firewall_addrgrp</span>  <span class="li-required">param: name</span>  <span class="li-required">type: str</span></li>
        <li><span class="li-normal">firewall_policy6</span>  <span class="li-required">param: policyid</span>  <span class="li-required">type: int</span></li>
        <li><span class="li-normal">router_ripng</span> </li>
        <li><span class="li-normal">firewall_vip6</span>  <span class="li-required">param: name</span>  <span class="li-required">type: str</span></li>
        <li><span class="li-normal">execute__tree__.restore.config_tftp</span> </li>
        <li><span class="li-normal">web-proxy_forward-server</span>  <span class="li-required">param: name</span>  <span class="li-required">type: str</span></li>
        <li><span class="li-normal">system.replacemsg_spam</span>  <span class="li-required">param: msg_type</span>  <span class="li-required">type: str</span></li>
        <li><span class="li-normal">certificate_ca</span>  <span class="li-required">param: name</span>  <span class="li-required">type: str</span></li>
        <li><span class="li-normal">execute__tree__.mrouter.clear_dense-routes</span> </li>
        <li><span class="li-normal">execute__tree___tracert6</span> </li>
        <li><span class="li-normal">firewall.ssh_local-ca</span>  <span class="li-required">param: name</span>  <span class="li-required">type: str</span></li>
        <li><span class="li-normal">execute__tree__.switch-controller.upload-swtp-image_ftp</span> </li>
        <li><span class="li-normal">diagnose__tree___forticlient</span> </li>
        <li><span class="li-normal">spamfilter_dnsbl</span>  <span class="li-required">param: id</span>  <span class="li-required">type: int</span></li>
        <li><span class="li-normal">execute__tree__.disk_list</span> </li>
        <li><span class="li-normal">execute__tree__.ping6-options_data-size</span> </li>
        <li><span class="li-normal">execute__tree__.switch-controller.restart-swtp_all</span> </li>
        <li><span class="li-normal">execute__tree__.backup.full-config_usb</span> </li>
        <li><span class="li-normal">execute__tree__.fortiguard-message_info</span> </li>
        <li><span class="li-normal">waf_profile</span>  <span class="li-required">param: name</span>  <span class="li-required">type: str</span></li>
        <li><span class="li-normal">firewall.wildcard-fqdn_group</span>  <span class="li-required">param: name</span>  <span class="li-required">type: str</span></li>
        <li><span class="li-normal">switch-controller_managed-switch</span>  <span class="li-required">param: switch_id</span>  <span class="li-required">type: str</span></li>
        <li><span class="li-normal">execute__tree__.extender_reset-fortiextender</span> </li>
        <li><span class="li-normal">user_group</span>  <span class="li-required">param: name</span>  <span class="li-required">type: str</span></li>
        <li><span class="li-normal">diagnose__tree___hardware</span> </li>
        <li><span class="li-normal">execute__tree__.dhcp_lease-clear</span> </li>
        <li><span class="li-normal">user_krb-keytab</span>  <span class="li-required">param: name</span>  <span class="li-required">type: str</span></li>
        <li><span class="li-normal">diagnose__tree__.ipv6_neighbor-cache</span> </li>
        <li><span class="li-normal">execute__tree__.log_upload</span> </li>
        <li><span class="li-normal">execute__tree__.ping6-options_validate-reply</span> </li>
        <li><span class="li-normal">execute__tree__.switch-controller.get-sync-status_switch-id</span> </li>
        <li><span class="li-normal">diagnose__tree__.ips_signature</span> </li>
        <li><span class="li-normal">execute__tree__.vpn.certificate.remote.export_tftp</span> </li>
        <li><span class="li-normal">application_group</span>  <span class="li-required">param: name</span>  <span class="li-required">type: str</span></li>
        <li><span class="li-normal">system.replacemsg_ftp</span>  <span class="li-required">param: msg_type</span>  <span class="li-required">type: str</span></li>
        <li><span class="li-normal">execute__tree__.vpn.certificate.crl.import_auto</span> </li>
        <li><span class="li-normal">diagnose__tree__.ips_anomaly</span> </li>
        <li><span class="li-normal">log_threat-weight</span> </li>
        <li><span class="li-normal">extender-controller_extender</span>  <span class="li-required">param: id</span>  <span class="li-required">type: str</span></li>
        <li><span class="li-normal">execute__tree__.set.system.session.filter_proto</span> </li>
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