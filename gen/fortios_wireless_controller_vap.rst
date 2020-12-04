:source: fortios_wireless_controller_vap.py

:orphan:

.. fortios_wireless_controller_vap:

fortios_wireless_controller_vap -- Configure Virtual Access Points (VAPs) in Fortinet's FortiOS and FortiGate.
++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++

.. versionadded:: 2.8

.. contents::
   :local:
   :depth: 1


Synopsis
--------
- This module is able to configure a FortiGate or FortiOS (FOS) device by allowing the user to set and modify wireless_controller feature and vap category. Examples include all parameters and values need to be adjusted to datasources before usage. Tested with FOS v6.2.0



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
    <li> <span class="li-head">wireless_controller_vap</span> - Configure Virtual Access Points (VAPs). <span class="li-normal">type: dict</span></li>
        <ul class="ul-self">
        <li> <span class="li-head">state</span> - B(Deprecated) <span class="li-normal">type: str</span> <span class="li-required">required: False</span> <span class="li-normal">choices: present, absent</span></li>
        <li> <span class="li-head">acct_interim_interval</span> - WiFi RADIUS accounting interim interval (60 - 86400 sec). <span class="li-normal">type: int</span></li>
        <li> <span class="li-head">address_group</span> - Address group ID. Source wireless-controller.addrgrp.id. <span class="li-normal">type: str</span></li>
        <li> <span class="li-head">alias</span> - Alias. <span class="li-normal">type: str</span></li>
        <li> <span class="li-head">atf_weight</span> - Airtime weight in percentage . <span class="li-normal">type: int</span></li>
        <li> <span class="li-head">auth</span> - Authentication protocol. <span class="li-normal">type: str</span> <span class="li-normal">choices: psk, radius, usergroup</span></li>
        <li> <span class="li-head">broadcast_ssid</span> - Enable/disable broadcasting the SSID . <span class="li-normal">type: str</span> <span class="li-normal">choices: enable, disable</span></li>
        <li> <span class="li-head">broadcast_suppression</span> - Optional suppression of broadcast messages. For example, you can keep DHCP messages, ARP broadcasts, and so on off of the wireless network. <span class="li-normal">type: str</span> <span class="li-normal">choices: dhcp-up, dhcp-down, dhcp-starvation, dhcp-ucast, arp-known, arp-unknown, arp-reply, arp-poison, arp-proxy, netbios-ns, netbios-ds, ipv6, all-other-mc, all-other-bc</span></li>
        <li> <span class="li-head">captive_portal_ac_name</span> - Local-bridging captive portal ac-name. <span class="li-normal">type: str</span></li>
        <li> <span class="li-head">captive_portal_macauth_radius_secret</span> - Secret key to access the macauth RADIUS server. <span class="li-normal">type: str</span></li>
        <li> <span class="li-head">captive_portal_macauth_radius_server</span> - Captive portal external RADIUS server domain name or IP address. <span class="li-normal">type: str</span></li>
        <li> <span class="li-head">captive_portal_radius_secret</span> - Secret key to access the RADIUS server. <span class="li-normal">type: str</span></li>
        <li> <span class="li-head">captive_portal_radius_server</span> - Captive portal RADIUS server domain name or IP address. <span class="li-normal">type: str</span></li>
        <li> <span class="li-head">captive_portal_session_timeout_interval</span> - Session timeout interval (0 - 864000 sec). <span class="li-normal">type: int</span></li>
        <li> <span class="li-head">dhcp_lease_time</span> - DHCP lease time in seconds for NAT IP address. <span class="li-normal">type: int</span></li>
        <li> <span class="li-head">dhcp_option82_circuit_id_insertion</span> - Enable/disable DHCP option 82 circuit-id insert . <span class="li-normal">type: str</span> <span class="li-normal">choices: style-1, style-2, disable</span></li>
        <li> <span class="li-head">dhcp_option82_insertion</span> - Enable/disable DHCP option 82 insert . <span class="li-normal">type: str</span> <span class="li-normal">choices: enable, disable</span></li>
        <li> <span class="li-head">dhcp_option82_remote_id_insertion</span> - Enable/disable DHCP option 82 remote-id insert . <span class="li-normal">type: str</span> <span class="li-normal">choices: style-1, disable</span></li>
        <li> <span class="li-head">dynamic_vlan</span> - Enable/disable dynamic VLAN assignment. <span class="li-normal">type: str</span> <span class="li-normal">choices: enable, disable</span></li>
        <li> <span class="li-head">eap_reauth</span> - Enable/disable EAP re-authentication for WPA-Enterprise security. <span class="li-normal">type: str</span> <span class="li-normal">choices: enable, disable</span></li>
        <li> <span class="li-head">eap_reauth_intv</span> - EAP re-authentication interval (1800 - 864000 sec). <span class="li-normal">type: int</span></li>
        <li> <span class="li-head">eapol_key_retries</span> - Enable/disable retransmission of EAPOL-Key frames (message 3/4 and group message 1/2) . <span class="li-normal">type: str</span> <span class="li-normal">choices: disable, enable</span></li>
        <li> <span class="li-head">encrypt</span> - Encryption protocol to use (only available when security is set to a WPA type). <span class="li-normal">type: str</span> <span class="li-normal">choices: TKIP, AES, TKIP-AES</span></li>
        <li> <span class="li-head">external_fast_roaming</span> - Enable/disable fast roaming or pre-authentication with external APs not managed by the FortiGate . <span class="li-normal">type: str</span> <span class="li-normal">choices: enable, disable</span></li>
        <li> <span class="li-head">external_logout</span> - URL of external authentication logout server. <span class="li-normal">type: str</span></li>
        <li> <span class="li-head">external_web</span> - URL of external authentication web server. <span class="li-normal">type: str</span></li>
        <li> <span class="li-head">fast_bss_transition</span> - Enable/disable 802.11r Fast BSS Transition (FT) . <span class="li-normal">type: str</span> <span class="li-normal">choices: disable, enable</span></li>
        <li> <span class="li-head">fast_roaming</span> - Enable/disable fast-roaming, or pre-authentication, where supported by clients . <span class="li-normal">type: str</span> <span class="li-normal">choices: enable, disable</span></li>
        <li> <span class="li-head">ft_mobility_domain</span> - Mobility domain identifier in FT (1 - 65535). <span class="li-normal">type: int</span></li>
        <li> <span class="li-head">ft_over_ds</span> - Enable/disable FT over the Distribution System (DS). <span class="li-normal">type: str</span> <span class="li-normal">choices: disable, enable</span></li>
        <li> <span class="li-head">ft_r0_key_lifetime</span> - Lifetime of the PMK-R0 key in FT, 1-65535 minutes. <span class="li-normal">type: int</span></li>
        <li> <span class="li-head">gtk_rekey</span> - Enable/disable GTK rekey for WPA security. <span class="li-normal">type: str</span> <span class="li-normal">choices: enable, disable</span></li>
        <li> <span class="li-head">gtk_rekey_intv</span> - GTK rekey interval (1800 - 864000 sec). <span class="li-normal">type: int</span></li>
        <li> <span class="li-head">hotspot20_profile</span> - Hotspot 2.0 profile name. Source wireless-controller.hotspot20.hs-profile.name. <span class="li-normal">type: str</span></li>
        <li> <span class="li-head">intra_vap_privacy</span> - Enable/disable blocking communication between clients on the same SSID (called intra-SSID privacy) . <span class="li-normal">type: str</span> <span class="li-normal">choices: enable, disable</span></li>
        <li> <span class="li-head">ip</span> - IP address and subnet mask for the local standalone NAT subnet. <span class="li-normal">type: str</span></li>
        <li> <span class="li-head">key</span> - WEP Key. <span class="li-normal">type: str</span></li>
        <li> <span class="li-head">keyindex</span> - WEP key index (1 - 4). <span class="li-normal">type: int</span></li>
        <li> <span class="li-head">ldpc</span> - VAP low-density parity-check (LDPC) coding configuration. <span class="li-normal">type: str</span> <span class="li-normal">choices: disable, rx, tx, rxtx</span></li>
        <li> <span class="li-head">local_authentication</span> - Enable/disable AP local authentication. <span class="li-normal">type: str</span> <span class="li-normal">choices: enable, disable</span></li>
        <li> <span class="li-head">local_bridging</span> - Enable/disable bridging of wireless and Ethernet interfaces on the FortiAP . <span class="li-normal">type: str</span> <span class="li-normal">choices: enable, disable</span></li>
        <li> <span class="li-head">local_lan</span> - Allow/deny traffic destined for a Class A, B, or C private IP address . <span class="li-normal">type: str</span> <span class="li-normal">choices: allow, deny</span></li>
        <li> <span class="li-head">local_standalone</span> - Enable/disable AP local standalone . <span class="li-normal">type: str</span> <span class="li-normal">choices: enable, disable</span></li>
        <li> <span class="li-head">local_standalone_nat</span> - Enable/disable AP local standalone NAT mode. <span class="li-normal">type: str</span> <span class="li-normal">choices: enable, disable</span></li>
        <li> <span class="li-head">mac_auth_bypass</span> - Enable/disable MAC authentication bypass. <span class="li-normal">type: str</span> <span class="li-normal">choices: enable, disable</span></li>
        <li> <span class="li-head">mac_filter</span> - Enable/disable MAC filtering to block wireless clients by mac address. <span class="li-normal">type: str</span> <span class="li-normal">choices: enable, disable</span></li>
        <li> <span class="li-head">mac_filter_list</span> - Create a list of MAC addresses for MAC address filtering. <span class="li-normal">type: list</span></li>
            <ul class="ul-self">
            <li> <span class="li-head">id</span> - ID. <span class="li-normal">type: int</span> <span class="li-required">required: True</span></li>
            <li> <span class="li-head">mac</span> - MAC address. <span class="li-normal">type: str</span></li>
            <li> <span class="li-head">mac_filter_policy</span> - Deny or allow the client with this MAC address. <span class="li-normal">type: str</span> <span class="li-normal">choices: allow, deny</span></li>
            </ul>
        <li> <span class="li-head">mac_filter_policy_other</span> - Allow or block clients with MAC addresses that are not in the filter list. <span class="li-normal">type: str</span> <span class="li-normal">choices: allow, deny</span></li>
        <li> <span class="li-head">max_clients</span> - Maximum number of clients that can connect simultaneously to the VAP . <span class="li-normal">type: int</span></li>
        <li> <span class="li-head">max_clients_ap</span> - Maximum number of clients that can connect simultaneously to the VAP per AP radio . <span class="li-normal">type: int</span></li>
        <li> <span class="li-head">me_disable_thresh</span> - Disable multicast enhancement when this many clients are receiving multicast traffic. <span class="li-normal">type: int</span></li>
        <li> <span class="li-head">mesh_backhaul</span> - Enable/disable using this VAP as a WiFi mesh backhaul . This entry is only available when security is set to a WPA type or open. <span class="li-normal">type: str</span> <span class="li-normal">choices: enable, disable</span></li>
        <li> <span class="li-head">mpsk</span> - Enable/disable multiple pre-shared keys (PSKs.) <span class="li-normal">type: str</span> <span class="li-normal">choices: enable, disable</span></li>
        <li> <span class="li-head">mpsk_concurrent_clients</span> - Number of pre-shared keys (PSKs) to allow if multiple pre-shared keys are enabled. <span class="li-normal">type: int</span></li>
        <li> <span class="li-head">mpsk_key</span> - Pre-shared keys that can be used to connect to this virtual access point. <span class="li-normal">type: list</span></li>
            <ul class="ul-self">
            <li> <span class="li-head">comment</span> - Comment. <span class="li-normal">type: str</span></li>
            <li> <span class="li-head">concurrent_clients</span> - Number of clients that can connect using this pre-shared key. <span class="li-normal">type: str</span></li>
            <li> <span class="li-head">key_name</span> - Pre-shared key name. <span class="li-normal">type: str</span></li>
            <li> <span class="li-head">passphrase</span> - WPA Pre-shared key. <span class="li-normal">type: str</span></li>
            </ul>
        <li> <span class="li-head">multicast_enhance</span> - Enable/disable converting multicast to unicast to improve performance . <span class="li-normal">type: str</span> <span class="li-normal">choices: enable, disable</span></li>
        <li> <span class="li-head">multicast_rate</span> - Multicast rate (0, 6000, 12000, or 24000 kbps). <span class="li-normal">type: str</span> <span class="li-normal">choices: 0, 6000, 12000, 24000</span></li>
        <li> <span class="li-head">name</span> - Virtual AP name. <span class="li-normal">type: str</span> <span class="li-required">required: True</span></li>
        <li> <span class="li-head">okc</span> - Enable/disable Opportunistic Key Caching (OKC) . <span class="li-normal">type: str</span> <span class="li-normal">choices: disable, enable</span></li>
        <li> <span class="li-head">owe_groups</span> - OWE-Groups. <span class="li-normal">type: str</span> <span class="li-normal">choices: 19, 20, 21</span></li>
        <li> <span class="li-head">owe_transition</span> - Enable/disable OWE transition mode support. <span class="li-normal">type: str</span> <span class="li-normal">choices: disable, enable</span></li>
        <li> <span class="li-head">owe_transition_ssid</span> - OWE transition mode peer SSID. <span class="li-normal">type: str</span></li>
        <li> <span class="li-head">passphrase</span> - WPA pre-shard key (PSK) to be used to authenticate WiFi users. <span class="li-normal">type: str</span></li>
        <li> <span class="li-head">pmf</span> - Protected Management Frames (PMF) support . <span class="li-normal">type: str</span> <span class="li-normal">choices: disable, enable, optional</span></li>
        <li> <span class="li-head">pmf_assoc_comeback_timeout</span> - Protected Management Frames (PMF) comeback maximum timeout (1-20 sec). <span class="li-normal">type: int</span></li>
        <li> <span class="li-head">pmf_sa_query_retry_timeout</span> - Protected Management Frames (PMF) SA query retry timeout interval (1 - 5 100s of msec). <span class="li-normal">type: int</span></li>
        <li> <span class="li-head">portal_message_override_group</span> - Replacement message group for this VAP (only available when security is set to a captive portal type). Source system.replacemsg-group .name. <span class="li-normal">type: str</span></li>
        <li> <span class="li-head">portal_message_overrides</span> - Individual message overrides. <span class="li-normal">type: dict</span></li>
            <ul class="ul-self">
            <li> <span class="li-head">auth_disclaimer_page</span> - Override auth-disclaimer-page message with message from portal-message-overrides group. <span class="li-normal">type: str</span></li>
            <li> <span class="li-head">auth_login_failed_page</span> - Override auth-login-failed-page message with message from portal-message-overrides group. <span class="li-normal">type: str</span></li>
            <li> <span class="li-head">auth_login_page</span> - Override auth-login-page message with message from portal-message-overrides group. <span class="li-normal">type: str</span></li>
            <li> <span class="li-head">auth_reject_page</span> - Override auth-reject-page message with message from portal-message-overrides group. <span class="li-normal">type: str</span></li>
            </ul>
        <li> <span class="li-head">portal_type</span> - Captive portal functionality. Configure how the captive portal authenticates users and whether it includes a disclaimer. <span class="li-normal">type: str</span> <span class="li-normal">choices: auth, auth+disclaimer, disclaimer, email-collect, cmcc, cmcc-macauth, auth-mac</span></li>
        <li> <span class="li-head">probe_resp_suppression</span> - Enable/disable probe response suppression (to ignore weak signals) . <span class="li-normal">type: str</span> <span class="li-normal">choices: enable, disable</span></li>
        <li> <span class="li-head">probe_resp_threshold</span> - Minimum signal level/threshold in dBm required for the AP response to probe requests (-95 to -20). <span class="li-normal">type: str</span></li>
        <li> <span class="li-head">ptk_rekey</span> - Enable/disable PTK rekey for WPA-Enterprise security. <span class="li-normal">type: str</span> <span class="li-normal">choices: enable, disable</span></li>
        <li> <span class="li-head">ptk_rekey_intv</span> - PTK rekey interval (1800 - 864000 sec). <span class="li-normal">type: int</span></li>
        <li> <span class="li-head">qos_profile</span> - Quality of service profile name. Source wireless-controller.qos-profile.name. <span class="li-normal">type: str</span></li>
        <li> <span class="li-head">quarantine</span> - Enable/disable station quarantine . <span class="li-normal">type: str</span> <span class="li-normal">choices: enable, disable</span></li>
        <li> <span class="li-head">radio_2g_threshold</span> - Minimum signal level/threshold in dBm required for the AP response to receive a packet in 2.4G band (-95 to -20). <span class="li-normal">type: str</span></li>
        <li> <span class="li-head">radio_5g_threshold</span> - Minimum signal level/threshold in dBm required for the AP response to receive a packet in 5G band(-95 to -20). <span class="li-normal">type: str</span></li>
        <li> <span class="li-head">radio_sensitivity</span> - Enable/disable software radio sensitivity (to ignore weak signals) . <span class="li-normal">type: str</span> <span class="li-normal">choices: enable, disable</span></li>
        <li> <span class="li-head">radius_mac_auth</span> - Enable/disable RADIUS-based MAC authentication of clients . <span class="li-normal">type: str</span> <span class="li-normal">choices: enable, disable</span></li>
        <li> <span class="li-head">radius_mac_auth_server</span> - RADIUS-based MAC authentication server. Source user.radius.name. <span class="li-normal">type: str</span></li>
        <li> <span class="li-head">radius_mac_auth_usergroups</span> - Selective user groups that are permitted for RADIUS mac authentication. <span class="li-normal">type: list</span></li>
            <ul class="ul-self">
            <li> <span class="li-head">name</span> - User group name. <span class="li-normal">type: str</span> <span class="li-required">required: True</span></li>
            </ul>
        <li> <span class="li-head">radius_server</span> - RADIUS server to be used to authenticate WiFi users. Source user.radius.name. <span class="li-normal">type: str</span></li>
        <li> <span class="li-head">rates_11a</span> - Allowed data rates for 802.11a. <span class="li-normal">type: str</span> <span class="li-normal">choices: 1, 1-basic, 2, 2-basic, 5.5, 5.5-basic, 11, 11-basic, 6, 6-basic, 9, 9-basic, 12, 12-basic, 18, 18-basic, 24, 24-basic, 36, 36-basic, 48, 48-basic, 54, 54-basic</span></li>
        <li> <span class="li-head">rates_11ac_ss12</span> - Allowed data rates for 802.11ac with 1 or 2 spatial streams. <span class="li-normal">type: str</span> <span class="li-normal">choices: mcs0/1, mcs1/1, mcs2/1, mcs3/1, mcs4/1, mcs5/1, mcs6/1, mcs7/1, mcs8/1, mcs9/1, mcs10/1, mcs11/1, mcs0/2, mcs1/2, mcs2/2, mcs3/2, mcs4/2, mcs5/2, mcs6/2, mcs7/2, mcs8/2, mcs9/2, mcs10/2, mcs11/2</span></li>
        <li> <span class="li-head">rates_11ac_ss34</span> - Allowed data rates for 802.11ac with 3 or 4 spatial streams. <span class="li-normal">type: str</span> <span class="li-normal">choices: mcs0/3, mcs1/3, mcs2/3, mcs3/3, mcs4/3, mcs5/3, mcs6/3, mcs7/3, mcs8/3, mcs9/3, mcs10/3, mcs11/3, mcs0/4, mcs1/4, mcs2/4, mcs3/4, mcs4/4, mcs5/4, mcs6/4, mcs7/4, mcs8/4, mcs9/4, mcs10/4, mcs11/4</span></li>
        <li> <span class="li-head">rates_11bg</span> - Allowed data rates for 802.11b/g. <span class="li-normal">type: str</span> <span class="li-normal">choices: 1, 1-basic, 2, 2-basic, 5.5, 5.5-basic, 11, 11-basic, 6, 6-basic, 9, 9-basic, 12, 12-basic, 18, 18-basic, 24, 24-basic, 36, 36-basic, 48, 48-basic, 54, 54-basic</span></li>
        <li> <span class="li-head">rates_11n_ss12</span> - Allowed data rates for 802.11n with 1 or 2 spatial streams. <span class="li-normal">type: str</span> <span class="li-normal">choices: mcs0/1, mcs1/1, mcs2/1, mcs3/1, mcs4/1, mcs5/1, mcs6/1, mcs7/1, mcs8/2, mcs9/2, mcs10/2, mcs11/2, mcs12/2, mcs13/2, mcs14/2, mcs15/2</span></li>
        <li> <span class="li-head">rates_11n_ss34</span> - Allowed data rates for 802.11n with 3 or 4 spatial streams. <span class="li-normal">type: str</span> <span class="li-normal">choices: mcs16/3, mcs17/3, mcs18/3, mcs19/3, mcs20/3, mcs21/3, mcs22/3, mcs23/3, mcs24/4, mcs25/4, mcs26/4, mcs27/4, mcs28/4, mcs29/4, mcs30/4, mcs31/4</span></li>
        <li> <span class="li-head">sae_groups</span> - SAE-Groups. <span class="li-normal">type: str</span> <span class="li-normal">choices: 1, 2, 5, 14, 15, 16, 17, 18, 19, 20, 21, 27, 28, 29, 30, 31</span></li>
        <li> <span class="li-head">sae_password</span> - WPA3 SAE password to be used to authenticate WiFi users. <span class="li-normal">type: str</span></li>
        <li> <span class="li-head">schedule</span> - VAP schedule name. Source firewall.schedule.recurring.name. <span class="li-normal">type: str</span></li>
        <li> <span class="li-head">security</span> - Security mode for the wireless interface . <span class="li-normal">type: str</span> <span class="li-normal">choices: open, captive-portal, wep64, wep128, wpa-personal, wpa-personal+captive-portal, wpa-enterprise, wpa-only-personal, wpa-only-personal+captive-portal, wpa-only-enterprise, wpa2-only-personal, wpa2-only-personal+captive-portal, wpa2-only-enterprise, wpa3-enterprise, wpa3-sae, wpa3-sae-transition, owe, osen</span></li>
        <li> <span class="li-head">security_exempt_list</span> - Optional security exempt list for captive portal authentication. Source user.security-exempt-list.name. <span class="li-normal">type: str</span></li>
        <li> <span class="li-head">security_obsolete_option</span> - Enable/disable obsolete security options. <span class="li-normal">type: str</span> <span class="li-normal">choices: enable, disable</span></li>
        <li> <span class="li-head">security_redirect_url</span> - Optional URL for redirecting users after they pass captive portal authentication. <span class="li-normal">type: str</span></li>
        <li> <span class="li-head">selected_usergroups</span> - Selective user groups that are permitted to authenticate. <span class="li-normal">type: list</span></li>
            <ul class="ul-self">
            <li> <span class="li-head">name</span> - User group name. Source user.group.name. <span class="li-normal">type: str</span> <span class="li-required">required: True</span></li>
            </ul>
        <li> <span class="li-head">split_tunneling</span> - Enable/disable split tunneling . <span class="li-normal">type: str</span> <span class="li-normal">choices: enable, disable</span></li>
        <li> <span class="li-head">ssid</span> - IEEE 802.11 service set identifier (SSID) for the wireless interface. Users who wish to use the wireless network must configure their computers to access this SSID name. <span class="li-normal">type: str</span></li>
        <li> <span class="li-head">tkip_counter_measure</span> - Enable/disable TKIP counter measure. <span class="li-normal">type: str</span> <span class="li-normal">choices: enable, disable</span></li>
        <li> <span class="li-head">usergroup</span> - Firewall user group to be used to authenticate WiFi users. <span class="li-normal">type: list</span></li>
            <ul class="ul-self">
            <li> <span class="li-head">name</span> - User group name. Source user.group.name. <span class="li-normal">type: str</span> <span class="li-required">required: True</span></li>
            </ul>
        <li> <span class="li-head">utm_profile</span> - UTM profile name. Source wireless-controller.utm-profile.name. <span class="li-normal">type: str</span></li>
        <li> <span class="li-head">vlan_auto</span> - Enable/disable automatic management of SSID VLAN interface. <span class="li-normal">type: str</span> <span class="li-normal">choices: enable, disable</span></li>
        <li> <span class="li-head">vlan_pool</span> - VLAN pool. <span class="li-normal">type: list</span></li>
            <ul class="ul-self">
            <li> <span class="li-head">id</span> - ID. <span class="li-normal">type: int</span> <span class="li-required">required: True</span></li>
            <li> <span class="li-head">wtp_group</span> - WTP group name. Source wireless-controller.wtp-group.name. <span class="li-normal">type: str</span></li>
            </ul>
        <li> <span class="li-head">vlan_pooling</span> - Enable/disable VLAN pooling, to allow grouping of multiple wireless controller VLANs into VLAN pools . When set to wtp-group, VLAN pooling occurs with VLAN assignment by wtp-group. <span class="li-normal">type: str</span> <span class="li-normal">choices: wtp-group, round-robin, hash, disable</span></li>
        <li> <span class="li-head">vlanid</span> - Optional VLAN ID. <span class="li-normal">type: int</span></li>
        <li> <span class="li-head">voice_enterprise</span> - Enable/disable 802.11k and 802.11v assisted Voice-Enterprise roaming . <span class="li-normal">type: str</span> <span class="li-normal">choices: disable, enable</span></li>
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
      - name: Configure Virtual Access Points (VAPs).
        fortios_wireless_controller_vap:
          vdom:  "{{ vdom }}"
          state: "present"
          access_token: "<your_own_value>"
          wireless_controller_vap:
            acct_interim_interval: "3"
            address_group: "<your_own_value> (source wireless-controller.addrgrp.id)"
            alias: "<your_own_value>"
            atf_weight: "6"
            auth: "psk"
            broadcast_ssid: "enable"
            broadcast_suppression: "dhcp-up"
            captive_portal_ac_name: "<your_own_value>"
            captive_portal_macauth_radius_secret: "<your_own_value>"
            captive_portal_macauth_radius_server: "<your_own_value>"
            captive_portal_radius_secret: "<your_own_value>"
            captive_portal_radius_server: "<your_own_value>"
            captive_portal_session_timeout_interval: "15"
            dhcp_lease_time: "16"
            dhcp_option82_circuit_id_insertion: "style-1"
            dhcp_option82_insertion: "enable"
            dhcp_option82_remote_id_insertion: "style-1"
            dynamic_vlan: "enable"
            eap_reauth: "enable"
            eap_reauth_intv: "22"
            eapol_key_retries: "disable"
            encrypt: "TKIP"
            external_fast_roaming: "enable"
            external_logout: "<your_own_value>"
            external_web: "<your_own_value>"
            fast_bss_transition: "disable"
            fast_roaming: "enable"
            ft_mobility_domain: "30"
            ft_over_ds: "disable"
            ft_r0_key_lifetime: "32"
            gtk_rekey: "enable"
            gtk_rekey_intv: "34"
            hotspot20_profile: "<your_own_value> (source wireless-controller.hotspot20.hs-profile.name)"
            intra_vap_privacy: "enable"
            ip: "<your_own_value>"
            key: "<your_own_value>"
            keyindex: "39"
            ldpc: "disable"
            local_authentication: "enable"
            local_bridging: "enable"
            local_lan: "allow"
            local_standalone: "enable"
            local_standalone_nat: "enable"
            mac_auth_bypass: "enable"
            mac_filter: "enable"
            mac_filter_list:
             -
                id:  "49"
                mac: "<your_own_value>"
                mac_filter_policy: "allow"
            mac_filter_policy_other: "allow"
            max_clients: "53"
            max_clients_ap: "54"
            me_disable_thresh: "55"
            mesh_backhaul: "enable"
            mpsk: "enable"
            mpsk_concurrent_clients: "58"
            mpsk_key:
             -
                comment: "Comment."
                concurrent_clients: "<your_own_value>"
                key_name: "<your_own_value>"
                passphrase: "<your_own_value>"
            multicast_enhance: "enable"
            multicast_rate: "0"
            name: "default_name_66"
            okc: "disable"
            owe_groups: "19"
            owe_transition: "disable"
            owe_transition_ssid: "<your_own_value>"
            passphrase: "<your_own_value>"
            pmf: "disable"
            pmf_assoc_comeback_timeout: "73"
            pmf_sa_query_retry_timeout: "74"
            portal_message_override_group: "<your_own_value> (source system.replacemsg-group.name)"
            portal_message_overrides:
                auth_disclaimer_page: "<your_own_value>"
                auth_login_failed_page: "<your_own_value>"
                auth_login_page: "<your_own_value>"
                auth_reject_page: "<your_own_value>"
            portal_type: "auth"
            probe_resp_suppression: "enable"
            probe_resp_threshold: "<your_own_value>"
            ptk_rekey: "enable"
            ptk_rekey_intv: "85"
            qos_profile: "<your_own_value> (source wireless-controller.qos-profile.name)"
            quarantine: "enable"
            radio_2g_threshold: "<your_own_value>"
            radio_5g_threshold: "<your_own_value>"
            radio_sensitivity: "enable"
            radius_mac_auth: "enable"
            radius_mac_auth_server: "<your_own_value> (source user.radius.name)"
            radius_mac_auth_usergroups:
             -
                name: "default_name_94"
            radius_server: "<your_own_value> (source user.radius.name)"
            rates_11a: "1"
            rates_11ac_ss12: "mcs0/1"
            rates_11ac_ss34: "mcs0/3"
            rates_11bg: "1"
            rates_11n_ss12: "mcs0/1"
            rates_11n_ss34: "mcs16/3"
            sae_groups: "1"
            sae_password: "<your_own_value>"
            schedule: "<your_own_value> (source firewall.schedule.recurring.name)"
            security: "open"
            security_exempt_list: "<your_own_value> (source user.security-exempt-list.name)"
            security_obsolete_option: "enable"
            security_redirect_url: "<your_own_value>"
            selected_usergroups:
             -
                name: "default_name_110 (source user.group.name)"
            split_tunneling: "enable"
            ssid: "<your_own_value>"
            tkip_counter_measure: "enable"
            usergroup:
             -
                name: "default_name_115 (source user.group.name)"
            utm_profile: "<your_own_value> (source wireless-controller.utm-profile.name)"
            vlan_auto: "enable"
            vlan_pool:
             -
                id:  "119"
                wtp_group: "<your_own_value> (source wireless-controller.wtp-group.name)"
            vlan_pooling: "wtp-group"
            vlanid: "122"
            voice_enterprise: "disable"
    


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
