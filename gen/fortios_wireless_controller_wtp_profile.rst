:source: fortios_wireless_controller_wtp_profile.py

:orphan:

.. fortios_wireless_controller_wtp_profile:

fortios_wireless_controller_wtp_profile -- Configure WTP profiles or FortiAP profiles that define radio settings for manageable FortiAP platforms in Fortinet's FortiOS and FortiGate.
++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++

.. versionadded:: 2.8

.. contents::
   :local:
   :depth: 1


Synopsis
--------
- This module is able to configure a FortiGate or FortiOS (FOS) device by allowing the user to set and modify wireless_controller feature and wtp_profile category. Examples include all parameters and values need to be adjusted to datasources before usage. Tested with FOS v6.4.0



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
    <li> <span class="li-head">wireless_controller_wtp_profile</span> - Configure WTP profiles or FortiAP profiles that define radio settings for manageable FortiAP platforms. <span class="li-normal">type: dict</span></li>
        <ul class="ul-self">
        <li> <span class="li-head">state</span> - B(Deprecated) <span class="li-normal">type: str</span> <span class="li-required">required: False</span> <span class="li-normal">choices: present, absent</span></li>
        <li> <span class="li-head">allowaccess</span> - Control management access to the managed WTP, FortiAP, or AP. Separate entries with a space. <span class="li-normal">type: str</span> <span class="li-normal">choices: https, ssh, snmp</span></li>
        <li> <span class="li-head">ap_country</span> - Country in which this WTP, FortiAP or AP will operate . <span class="li-normal">type: str</span> <span class="li-normal">choices: NA, AL, DZ, AO, AR, AM, AU, AT, AZ, BS, BH, BD, BB, BY, BE, BZ, BO, BA, BR, BN, BG, KH, CF, CL, CN, CO, CR, HR, CY, CZ, DK, DO, EC, EG, SV, EE, FI, FR, GE, DE, GR, GL, GD, GU, GT, HT, HN, HK, HU, IS, IN, ID, IR, IE, IL, IT, JM, JO, KZ, KE, KP, KR, KW, LV, LB, LI, LT, LU, MO, MK, MY, MT, MX, MC, MA, MZ, MM, NP, NL, AN, AW, NZ, False, OM, PK, PA, PG, PY, PE, PH, PL, PT, PR, QA, RO, RU, RW, SA, RS, ME, SG, SK, SI, ZA, ES, LK, SE, SD, CH, SY, TW, TZ, TH, TT, TN, TR, AE, UA, GB, US, PS, UY, UZ, VE, VN, YE, ZB, ZW, JP, CA</span></li>
        <li> <span class="li-head">ap_handoff</span> - Enable/disable AP handoff of clients to other APs . <span class="li-normal">type: str</span> <span class="li-normal">choices: enable, disable</span></li>
        <li> <span class="li-head">apcfg_profile</span> - AP local configuration profile name. Source wireless-controller.apcfg-profile.name. <span class="li-normal">type: str</span></li>
        <li> <span class="li-head">ble_profile</span> - Bluetooth Low Energy profile name. Source wireless-controller.ble-profile.name. <span class="li-normal">type: str</span></li>
        <li> <span class="li-head">comment</span> - Comment. <span class="li-normal">type: str</span></li>
        <li> <span class="li-head">control_message_offload</span> - Enable/disable CAPWAP control message data channel offload. <span class="li-normal">type: str</span> <span class="li-normal">choices: ebp-frame, aeroscout-tag, ap-list, sta-list, sta-cap-list, stats, aeroscout-mu, sta-health, spectral-analysis</span></li>
        <li> <span class="li-head">deny_mac_list</span> - List of MAC addresses that are denied access to this WTP, FortiAP, or AP. <span class="li-normal">type: list</span></li>
            <ul class="ul-self">
            <li> <span class="li-head">id</span> - ID. <span class="li-normal">type: int</span> <span class="li-required">required: True</span></li>
            <li> <span class="li-head">mac</span> - A WiFi device with this MAC address is denied access to this WTP, FortiAP or AP. <span class="li-normal">type: str</span></li>
            </ul>
        <li> <span class="li-head">dtls_in_kernel</span> - Enable/disable data channel DTLS in kernel. <span class="li-normal">type: str</span> <span class="li-normal">choices: enable, disable</span></li>
        <li> <span class="li-head">dtls_policy</span> - WTP data channel DTLS policy . <span class="li-normal">type: str</span> <span class="li-normal">choices: clear-text, dtls-enabled, ipsec-vpn</span></li>
        <li> <span class="li-head">energy_efficient_ethernet</span> - Enable/disable use of energy efficient Ethernet on WTP. <span class="li-normal">type: str</span> <span class="li-normal">choices: enable, disable</span></li>
        <li> <span class="li-head">ext_info_enable</span> - Enable/disable station/VAP/radio extension information. <span class="li-normal">type: str</span> <span class="li-normal">choices: enable, disable</span></li>
        <li> <span class="li-head">frequency_handoff</span> - Enable/disable frequency handoff of clients to other channels . <span class="li-normal">type: str</span> <span class="li-normal">choices: enable, disable</span></li>
        <li> <span class="li-head">handoff_roaming</span> - Enable/disable client load balancing during roaming to avoid roaming delay . <span class="li-normal">type: str</span> <span class="li-normal">choices: enable, disable</span></li>
        <li> <span class="li-head">handoff_rssi</span> - Minimum received signal strength indicator (RSSI) value for handoff (20 - 30). <span class="li-normal">type: int</span></li>
        <li> <span class="li-head">handoff_sta_thresh</span> - Threshold value for AP handoff. <span class="li-normal">type: int</span></li>
        <li> <span class="li-head">ip_fragment_preventing</span> - Method(s) by which IP fragmentation is prevented for control and data packets through CAPWAP tunnel . <span class="li-normal">type: str</span> <span class="li-normal">choices: tcp-mss-adjust, icmp-unreachable</span></li>
        <li> <span class="li-head">lan</span> - WTP LAN port mapping. <span class="li-normal">type: dict</span></li>
            <ul class="ul-self">
            <li> <span class="li-head">port_mode</span> - LAN port mode. <span class="li-normal">type: str</span> <span class="li-normal">choices: offline, nat-to-wan, bridge-to-wan, bridge-to-ssid</span></li>
            <li> <span class="li-head">port_ssid</span> - Bridge LAN port to SSID. Source system.interface.name. <span class="li-normal">type: str</span></li>
            <li> <span class="li-head">port1_mode</span> - LAN port 1 mode. <span class="li-normal">type: str</span> <span class="li-normal">choices: offline, nat-to-wan, bridge-to-wan, bridge-to-ssid</span></li>
            <li> <span class="li-head">port1_ssid</span> - Bridge LAN port 1 to SSID. Source system.interface.name. <span class="li-normal">type: str</span></li>
            <li> <span class="li-head">port2_mode</span> - LAN port 2 mode. <span class="li-normal">type: str</span> <span class="li-normal">choices: offline, nat-to-wan, bridge-to-wan, bridge-to-ssid</span></li>
            <li> <span class="li-head">port2_ssid</span> - Bridge LAN port 2 to SSID. Source system.interface.name. <span class="li-normal">type: str</span></li>
            <li> <span class="li-head">port3_mode</span> - LAN port 3 mode. <span class="li-normal">type: str</span> <span class="li-normal">choices: offline, nat-to-wan, bridge-to-wan, bridge-to-ssid</span></li>
            <li> <span class="li-head">port3_ssid</span> - Bridge LAN port 3 to SSID. Source system.interface.name. <span class="li-normal">type: str</span></li>
            <li> <span class="li-head">port4_mode</span> - LAN port 4 mode. <span class="li-normal">type: str</span> <span class="li-normal">choices: offline, nat-to-wan, bridge-to-wan, bridge-to-ssid</span></li>
            <li> <span class="li-head">port4_ssid</span> - Bridge LAN port 4 to SSID. Source system.interface.name. <span class="li-normal">type: str</span></li>
            <li> <span class="li-head">port5_mode</span> - LAN port 5 mode. <span class="li-normal">type: str</span> <span class="li-normal">choices: offline, nat-to-wan, bridge-to-wan, bridge-to-ssid</span></li>
            <li> <span class="li-head">port5_ssid</span> - Bridge LAN port 5 to SSID. Source system.interface.name. <span class="li-normal">type: str</span></li>
            <li> <span class="li-head">port6_mode</span> - LAN port 6 mode. <span class="li-normal">type: str</span> <span class="li-normal">choices: offline, nat-to-wan, bridge-to-wan, bridge-to-ssid</span></li>
            <li> <span class="li-head">port6_ssid</span> - Bridge LAN port 6 to SSID. Source system.interface.name. <span class="li-normal">type: str</span></li>
            <li> <span class="li-head">port7_mode</span> - LAN port 7 mode. <span class="li-normal">type: str</span> <span class="li-normal">choices: offline, nat-to-wan, bridge-to-wan, bridge-to-ssid</span></li>
            <li> <span class="li-head">port7_ssid</span> - Bridge LAN port 7 to SSID. Source system.interface.name. <span class="li-normal">type: str</span></li>
            <li> <span class="li-head">port8_mode</span> - LAN port 8 mode. <span class="li-normal">type: str</span> <span class="li-normal">choices: offline, nat-to-wan, bridge-to-wan, bridge-to-ssid</span></li>
            <li> <span class="li-head">port8_ssid</span> - Bridge LAN port 8 to SSID. Source system.interface.name. <span class="li-normal">type: str</span></li>
            </ul>
        <li> <span class="li-head">lbs</span> - Set various location based service (LBS) options. <span class="li-normal">type: dict</span></li>
            <ul class="ul-self">
            <li> <span class="li-head">aeroscout</span> - Enable/disable AeroScout Real Time Location Service (RTLS) support . <span class="li-normal">type: str</span> <span class="li-normal">choices: enable, disable</span></li>
            <li> <span class="li-head">aeroscout_ap_mac</span> - Use BSSID or board MAC address as AP MAC address in AeroScout AP messages . <span class="li-normal">type: str</span> <span class="li-normal">choices: bssid, board-mac</span></li>
            <li> <span class="li-head">aeroscout_mmu_report</span> - Enable/disable compounded AeroScout tag and MU report . <span class="li-normal">type: str</span> <span class="li-normal">choices: enable, disable</span></li>
            <li> <span class="li-head">aeroscout_mu</span> - Enable/disable AeroScout Mobile Unit (MU) support . <span class="li-normal">type: str</span> <span class="li-normal">choices: enable, disable</span></li>
            <li> <span class="li-head">aeroscout_mu_factor</span> - AeroScout MU mode dilution factor . <span class="li-normal">type: int</span></li>
            <li> <span class="li-head">aeroscout_mu_timeout</span> - AeroScout MU mode timeout (0 - 65535 sec). <span class="li-normal">type: int</span></li>
            <li> <span class="li-head">aeroscout_server_ip</span> - IP address of AeroScout server. <span class="li-normal">type: str</span></li>
            <li> <span class="li-head">aeroscout_server_port</span> - AeroScout server UDP listening port. <span class="li-normal">type: int</span></li>
            <li> <span class="li-head">ekahau_blink_mode</span> - Enable/disable Ekahau blink mode (now known as AiRISTA Flow) to track and locate WiFi tags . <span class="li-normal">type: str</span> <span class="li-normal">choices: enable, disable</span></li>
            <li> <span class="li-head">ekahau_tag</span> - WiFi frame MAC address or WiFi Tag. <span class="li-normal">type: str</span></li>
            <li> <span class="li-head">erc_server_ip</span> - IP address of Ekahau RTLS Controller (ERC). <span class="li-normal">type: str</span></li>
            <li> <span class="li-head">erc_server_port</span> - Ekahau RTLS Controller (ERC) UDP listening port. <span class="li-normal">type: int</span></li>
            <li> <span class="li-head">fortipresence</span> - Enable/disable FortiPresence to monitor the location and activity of WiFi clients even if they don"t connect to this WiFi network . <span class="li-normal">type: str</span> <span class="li-normal">choices: foreign, both, disable</span></li>
            <li> <span class="li-head">fortipresence_ble</span> - Enable/disable FortiPresence finding and reporting BLE devices. <span class="li-normal">type: str</span> <span class="li-normal">choices: enable, disable</span></li>
            <li> <span class="li-head">fortipresence_frequency</span> - FortiPresence report transmit frequency (5 - 65535 sec). <span class="li-normal">type: int</span></li>
            <li> <span class="li-head">fortipresence_port</span> - FortiPresence server UDP listening port . <span class="li-normal">type: int</span></li>
            <li> <span class="li-head">fortipresence_project</span> - FortiPresence project name (max. 16 characters). <span class="li-normal">type: str</span></li>
            <li> <span class="li-head">fortipresence_rogue</span> - Enable/disable FortiPresence finding and reporting rogue APs. <span class="li-normal">type: str</span> <span class="li-normal">choices: enable, disable</span></li>
            <li> <span class="li-head">fortipresence_secret</span> - FortiPresence secret password (max. 16 characters). <span class="li-normal">type: str</span></li>
            <li> <span class="li-head">fortipresence_server</span> - FortiPresence server IP address. <span class="li-normal">type: str</span></li>
            <li> <span class="li-head">fortipresence_unassoc</span> - Enable/disable FortiPresence finding and reporting unassociated stations. <span class="li-normal">type: str</span> <span class="li-normal">choices: enable, disable</span></li>
            <li> <span class="li-head">station_locate</span> - Enable/disable client station locating services for all clients, whether associated or not . <span class="li-normal">type: str</span> <span class="li-normal">choices: enable, disable</span></li>
            </ul>
        <li> <span class="li-head">led_schedules</span> - Recurring firewall schedules for illuminating LEDs on the FortiAP. If led-state is enabled, LEDs will be visible when at least one of the schedules is valid. Separate multiple schedule names with a space. <span class="li-normal">type: list</span></li>
            <ul class="ul-self">
            <li> <span class="li-head">name</span> - Schedule name. Source firewall.schedule.group.name firewall.schedule.recurring.name firewall.schedule.onetime.name. <span class="li-normal">type: str</span> <span class="li-required">required: True</span></li>
            </ul>
        <li> <span class="li-head">led_state</span> - Enable/disable use of LEDs on WTP . <span class="li-normal">type: str</span> <span class="li-normal">choices: enable, disable</span></li>
        <li> <span class="li-head">lldp</span> - Enable/disable Link Layer Discovery Protocol (LLDP) for the WTP, FortiAP, or AP . <span class="li-normal">type: str</span> <span class="li-normal">choices: enable, disable</span></li>
        <li> <span class="li-head">login_passwd</span> - Set the managed WTP, FortiAP, or AP"s administrator password. <span class="li-normal">type: str</span></li>
        <li> <span class="li-head">login_passwd_change</span> - Change or reset the administrator password of a managed WTP, FortiAP or AP (yes, default, or no). <span class="li-normal">type: str</span> <span class="li-normal">choices: True, default, False</span></li>
        <li> <span class="li-head">max_clients</span> - Maximum number of stations (STAs) supported by the WTP . <span class="li-normal">type: int</span></li>
        <li> <span class="li-head">name</span> - WTP (or FortiAP or AP) profile name. <span class="li-normal">type: str</span> <span class="li-required">required: True</span></li>
        <li> <span class="li-head">platform</span> - WTP, FortiAP, or AP platform. <span class="li-normal">type: dict</span></li>
            <ul class="ul-self">
            <li> <span class="li-head">ddscan</span> - Enable/disable use of one radio for dedicated dual-band scanning to detect RF characterization and wireless threat management. <span class="li-normal">type: str</span> <span class="li-normal">choices: enable, disable</span></li>
            <li> <span class="li-head">mode</span> - Configure operation mode of 5G radios . <span class="li-normal">type: str</span> <span class="li-normal">choices: single-5G, dual-5G</span></li>
            <li> <span class="li-head">type</span> - WTP, FortiAP or AP platform type. There are built-in WTP profiles for all supported FortiAP models. You can select a built-in profile and customize it or create a new profile. <span class="li-normal">type: str</span> <span class="li-normal">choices: AP-11N, 220B, 210B, 222B, 112B, 320B, 11C, 14C, 223B, 28C, 320C, 221C, 25D, 222C, 224D, 214B, 21D, 24D, 112D, 223C, 321C, C220C, C225C, C23JD, C24JE, S321C, S322C, S323C, S311C, S313C, S321CR, S322CR, S323CR, S421E, S422E, S423E, 421E, 423E, 221E, 222E, 223E, 224E, 231E, S221E, S223E, 321E, 431F, 433F, U421E, U422EV, U423E, U221EV, U223EV, U24JEV, U321EV, U323EV, U431F, U433F</span></li>
            </ul>
        <li> <span class="li-head">poe_mode</span> - Set the WTP, FortiAP, or AP"s PoE mode. <span class="li-normal">type: str</span> <span class="li-normal">choices: auto, 8023af, 8023at, power-adapter</span></li>
        <li> <span class="li-head">radio_1</span> - Configuration options for radio 1. <span class="li-normal">type: dict</span></li>
            <ul class="ul-self">
            <li> <span class="li-head">airtime_fairness</span> - Enable/disable airtime fairness . <span class="li-normal">type: str</span> <span class="li-normal">choices: enable, disable</span></li>
            <li> <span class="li-head">amsdu</span> - Enable/disable 802.11n AMSDU support. AMSDU can improve performance if supported by your WiFi clients . <span class="li-normal">type: str</span> <span class="li-normal">choices: enable, disable</span></li>
            <li> <span class="li-head">ap_sniffer_addr</span> - MAC address to monitor. <span class="li-normal">type: str</span></li>
            <li> <span class="li-head">ap_sniffer_bufsize</span> - Sniffer buffer size (1 - 32 MB). <span class="li-normal">type: int</span></li>
            <li> <span class="li-head">ap_sniffer_chan</span> - Channel on which to operate the sniffer . <span class="li-normal">type: int</span></li>
            <li> <span class="li-head">ap_sniffer_ctl</span> - Enable/disable sniffer on WiFi control frame . <span class="li-normal">type: str</span> <span class="li-normal">choices: enable, disable</span></li>
            <li> <span class="li-head">ap_sniffer_data</span> - Enable/disable sniffer on WiFi data frame . <span class="li-normal">type: str</span> <span class="li-normal">choices: enable, disable</span></li>
            <li> <span class="li-head">ap_sniffer_mgmt_beacon</span> - Enable/disable sniffer on WiFi management Beacon frames . <span class="li-normal">type: str</span> <span class="li-normal">choices: enable, disable</span></li>
            <li> <span class="li-head">ap_sniffer_mgmt_other</span> - Enable/disable sniffer on WiFi management other frames  . <span class="li-normal">type: str</span> <span class="li-normal">choices: enable, disable</span></li>
            <li> <span class="li-head">ap_sniffer_mgmt_probe</span> - Enable/disable sniffer on WiFi management probe frames . <span class="li-normal">type: str</span> <span class="li-normal">choices: enable, disable</span></li>
            <li> <span class="li-head">auto_power_high</span> - The upper bound of automatic transmit power adjustment in dBm (the actual range of transmit power depends on the AP platform type). <span class="li-normal">type: int</span></li>
            <li> <span class="li-head">auto_power_level</span> - Enable/disable automatic power-level adjustment to prevent co-channel interference . <span class="li-normal">type: str</span> <span class="li-normal">choices: enable, disable</span></li>
            <li> <span class="li-head">auto_power_low</span> - The lower bound of automatic transmit power adjustment in dBm (the actual range of transmit power depends on the AP platform type). <span class="li-normal">type: int</span></li>
            <li> <span class="li-head">band</span> - WiFi band that Radio 1 operates on. <span class="li-normal">type: str</span> <span class="li-normal">choices: 802.11a, 802.11b, 802.11g, 802.11n, 802.11n-5G, 802.11ac, 802.11ax-5G, 802.11ax, 802.11n,g-only, 802.11g-only, 802.11n-only, 802.11n-5G-only, 802.11ac,n-only, 802.11ac-only, 802.11ax,ac-only, 802.11ax,ac,n-only, 802.11ax-5G-only, 802.11ax,n-only, 802.11ax,n,g-only, 802.11ax-only</span></li>
            <li> <span class="li-head">band_5g_type</span> - WiFi 5G band type. <span class="li-normal">type: str</span> <span class="li-normal">choices: 5g-full, 5g-high, 5g-low</span></li>
            <li> <span class="li-head">bandwidth_admission_control</span> - Enable/disable WiFi multimedia (WMM) bandwidth admission control to optimize WiFi bandwidth use. A request to join the wireless network is only allowed if the access point has enough bandwidth to support it. <span class="li-normal">type: str</span> <span class="li-normal">choices: enable, disable</span></li>
            <li> <span class="li-head">bandwidth_capacity</span> - Maximum bandwidth capacity allowed (1 - 600000 Kbps). <span class="li-normal">type: int</span></li>
            <li> <span class="li-head">beacon_interval</span> - Beacon interval. The time between beacon frames in msec (the actual range of beacon interval depends on the AP platform type). <span class="li-normal">type: int</span></li>
            <li> <span class="li-head">call_admission_control</span> - Enable/disable WiFi multimedia (WMM) call admission control to optimize WiFi bandwidth use for VoIP calls. New VoIP calls are only accepted if there is enough bandwidth available to support them. <span class="li-normal">type: str</span> <span class="li-normal">choices: enable, disable</span></li>
            <li> <span class="li-head">call_capacity</span> - Maximum number of Voice over WLAN (VoWLAN) phones supported by the radio (0 - 60). <span class="li-normal">type: int</span></li>
            <li> <span class="li-head">channel</span> - Selected list of wireless radio channels. <span class="li-normal">type: list</span></li>
                <ul class="ul-self">
                <li> <span class="li-head">chan</span> - Channel number. <span class="li-normal">type: str</span> <span class="li-required">required: True</span></li>
                </ul>
            <li> <span class="li-head">channel_bonding</span> - Channel bandwidth: 160,80, 40, or 20MHz. Channels may use both 20 and 40 by enabling coexistence. <span class="li-normal">type: str</span> <span class="li-normal">choices: 160MHz, 80MHz, 40MHz, 20MHz</span></li>
            <li> <span class="li-head">channel_utilization</span> - Enable/disable measuring channel utilization. <span class="li-normal">type: str</span> <span class="li-normal">choices: enable, disable</span></li>
            <li> <span class="li-head">coexistence</span> - Enable/disable allowing both HT20 and HT40 on the same radio . <span class="li-normal">type: str</span> <span class="li-normal">choices: enable, disable</span></li>
            <li> <span class="li-head">darrp</span> - Enable/disable Distributed Automatic Radio Resource Provisioning (DARRP) to make sure the radio is always using the most optimal channel . <span class="li-normal">type: str</span> <span class="li-normal">choices: enable, disable</span></li>
            <li> <span class="li-head">dtim</span> - Delivery Traffic Indication Map (DTIM) period (1 - 255). Set higher to save battery life of WiFi client in power-save mode. <span class="li-normal">type: int</span></li>
            <li> <span class="li-head">frag_threshold</span> - Maximum packet size that can be sent without fragmentation (800 - 2346 bytes). <span class="li-normal">type: int</span></li>
            <li> <span class="li-head">max_clients</span> - Maximum number of stations (STAs) or WiFi clients supported by the radio. Range depends on the hardware. <span class="li-normal">type: int</span></li>
            <li> <span class="li-head">max_distance</span> - Maximum expected distance between the AP and clients (0 - 54000 m). <span class="li-normal">type: int</span></li>
            <li> <span class="li-head">mode</span> - Mode of radio 1. Radio 1 can be disabled, configured as an access point, a rogue AP monitor, or a sniffer. <span class="li-normal">type: str</span> <span class="li-normal">choices: disabled, ap, monitor, sniffer</span></li>
            <li> <span class="li-head">power_level</span> - Radio power level as a percentage of the maximum transmit power (0 - 100). <span class="li-normal">type: int</span></li>
            <li> <span class="li-head">powersave_optimize</span> - Enable client power-saving features such as TIM, AC VO, and OBSS etc. <span class="li-normal">type: str</span> <span class="li-normal">choices: tim, ac-vo, no-obss-scan, no-11b-rate, client-rate-follow</span></li>
            <li> <span class="li-head">protection_mode</span> - Enable/disable 802.11g protection modes to support backwards compatibility with older clients (rtscts, ctsonly, disable). <span class="li-normal">type: str</span> <span class="li-normal">choices: rtscts, ctsonly, disable</span></li>
            <li> <span class="li-head">rts_threshold</span> - Maximum packet size for RTS transmissions, specifying the maximum size of a data packet before RTS/CTS (256 - 2346 bytes). <span class="li-normal">type: int</span></li>
            <li> <span class="li-head">short_guard_interval</span> - Use either the short guard interval (Short GI) of 400 ns or the long guard interval (Long GI) of 800 ns. <span class="li-normal">type: str</span> <span class="li-normal">choices: enable, disable</span></li>
            <li> <span class="li-head">spectrum_analysis</span> - Enable/disable spectrum analysis to find interference that would negatively impact wireless performance. <span class="li-normal">type: str</span> <span class="li-normal">choices: enable, scan-only, disable</span></li>
            <li> <span class="li-head">transmit_optimize</span> - Packet transmission optimization options including power saving, aggregation limiting, retry limiting, etc. All are enabled by default. <span class="li-normal">type: str</span> <span class="li-normal">choices: disable, power-save, aggr-limit, retry-limit, send-bar</span></li>
            <li> <span class="li-head">vap_all</span> - Enable/disable the automatic inheritance of all Virtual Access Points (VAPs) . <span class="li-normal">type: str</span> <span class="li-normal">choices: enable, disable</span></li>
            <li> <span class="li-head">vaps</span> - Manually selected list of Virtual Access Points (VAPs). <span class="li-normal">type: list</span></li>
                <ul class="ul-self">
                <li> <span class="li-head">name</span> - Virtual Access Point (VAP) name. Source wireless-controller.vap-group.name system.interface.name. <span class="li-normal">type: str</span> <span class="li-required">required: True</span></li>
                </ul>
            <li> <span class="li-head">wids_profile</span> - Wireless Intrusion Detection System (WIDS) profile name to assign to the radio. Source wireless-controller.wids-profile.name. <span class="li-normal">type: str</span></li>
            <li> <span class="li-head">zero_wait_dfs</span> - Enable/disable zero wait DFS on radio . <span class="li-normal">type: str</span> <span class="li-normal">choices: enable, disable</span></li>
            </ul>
        <li> <span class="li-head">radio_2</span> - Configuration options for radio 2. <span class="li-normal">type: dict</span></li>
            <ul class="ul-self">
            <li> <span class="li-head">airtime_fairness</span> - Enable/disable airtime fairness . <span class="li-normal">type: str</span> <span class="li-normal">choices: enable, disable</span></li>
            <li> <span class="li-head">amsdu</span> - Enable/disable 802.11n AMSDU support. AMSDU can improve performance if supported by your WiFi clients . <span class="li-normal">type: str</span> <span class="li-normal">choices: enable, disable</span></li>
            <li> <span class="li-head">ap_sniffer_addr</span> - MAC address to monitor. <span class="li-normal">type: str</span></li>
            <li> <span class="li-head">ap_sniffer_bufsize</span> - Sniffer buffer size (1 - 32 MB). <span class="li-normal">type: int</span></li>
            <li> <span class="li-head">ap_sniffer_chan</span> - Channel on which to operate the sniffer . <span class="li-normal">type: int</span></li>
            <li> <span class="li-head">ap_sniffer_ctl</span> - Enable/disable sniffer on WiFi control frame . <span class="li-normal">type: str</span> <span class="li-normal">choices: enable, disable</span></li>
            <li> <span class="li-head">ap_sniffer_data</span> - Enable/disable sniffer on WiFi data frame . <span class="li-normal">type: str</span> <span class="li-normal">choices: enable, disable</span></li>
            <li> <span class="li-head">ap_sniffer_mgmt_beacon</span> - Enable/disable sniffer on WiFi management Beacon frames . <span class="li-normal">type: str</span> <span class="li-normal">choices: enable, disable</span></li>
            <li> <span class="li-head">ap_sniffer_mgmt_other</span> - Enable/disable sniffer on WiFi management other frames  . <span class="li-normal">type: str</span> <span class="li-normal">choices: enable, disable</span></li>
            <li> <span class="li-head">ap_sniffer_mgmt_probe</span> - Enable/disable sniffer on WiFi management probe frames . <span class="li-normal">type: str</span> <span class="li-normal">choices: enable, disable</span></li>
            <li> <span class="li-head">auto_power_high</span> - The upper bound of automatic transmit power adjustment in dBm (the actual range of transmit power depends on the AP platform type). <span class="li-normal">type: int</span></li>
            <li> <span class="li-head">auto_power_level</span> - Enable/disable automatic power-level adjustment to prevent co-channel interference . <span class="li-normal">type: str</span> <span class="li-normal">choices: enable, disable</span></li>
            <li> <span class="li-head">auto_power_low</span> - The lower bound of automatic transmit power adjustment in dBm (the actual range of transmit power depends on the AP platform type). <span class="li-normal">type: int</span></li>
            <li> <span class="li-head">band</span> - WiFi band that Radio 2 operates on. <span class="li-normal">type: str</span> <span class="li-normal">choices: 802.11a, 802.11b, 802.11g, 802.11n, 802.11n-5G, 802.11ac, 802.11ax-5G, 802.11ax, 802.11n,g-only, 802.11g-only, 802.11n-only, 802.11n-5G-only, 802.11ac,n-only, 802.11ac-only, 802.11ax,ac-only, 802.11ax,ac,n-only, 802.11ax-5G-only, 802.11ax,n-only, 802.11ax,n,g-only, 802.11ax-only</span></li>
            <li> <span class="li-head">band_5g_type</span> - WiFi 5G band type. <span class="li-normal">type: str</span> <span class="li-normal">choices: 5g-full, 5g-high, 5g-low</span></li>
            <li> <span class="li-head">bandwidth_admission_control</span> - Enable/disable WiFi multimedia (WMM) bandwidth admission control to optimize WiFi bandwidth use. A request to join the wireless network is only allowed if the access point has enough bandwidth to support it. <span class="li-normal">type: str</span> <span class="li-normal">choices: enable, disable</span></li>
            <li> <span class="li-head">bandwidth_capacity</span> - Maximum bandwidth capacity allowed (1 - 600000 Kbps). <span class="li-normal">type: int</span></li>
            <li> <span class="li-head">beacon_interval</span> - Beacon interval. The time between beacon frames in msec (the actual range of beacon interval depends on the AP platform type). <span class="li-normal">type: int</span></li>
            <li> <span class="li-head">call_admission_control</span> - Enable/disable WiFi multimedia (WMM) call admission control to optimize WiFi bandwidth use for VoIP calls. New VoIP calls are only accepted if there is enough bandwidth available to support them. <span class="li-normal">type: str</span> <span class="li-normal">choices: enable, disable</span></li>
            <li> <span class="li-head">call_capacity</span> - Maximum number of Voice over WLAN (VoWLAN) phones supported by the radio (0 - 60). <span class="li-normal">type: int</span></li>
            <li> <span class="li-head">channel</span> - Selected list of wireless radio channels. <span class="li-normal">type: list</span></li>
                <ul class="ul-self">
                <li> <span class="li-head">chan</span> - Channel number. <span class="li-normal">type: str</span> <span class="li-required">required: True</span></li>
                </ul>
            <li> <span class="li-head">channel_bonding</span> - Channel bandwidth: 160,80, 40, or 20MHz. Channels may use both 20 and 40 by enabling coexistence. <span class="li-normal">type: str</span> <span class="li-normal">choices: 160MHz, 80MHz, 40MHz, 20MHz</span></li>
            <li> <span class="li-head">channel_utilization</span> - Enable/disable measuring channel utilization. <span class="li-normal">type: str</span> <span class="li-normal">choices: enable, disable</span></li>
            <li> <span class="li-head">coexistence</span> - Enable/disable allowing both HT20 and HT40 on the same radio . <span class="li-normal">type: str</span> <span class="li-normal">choices: enable, disable</span></li>
            <li> <span class="li-head">darrp</span> - Enable/disable Distributed Automatic Radio Resource Provisioning (DARRP) to make sure the radio is always using the most optimal channel . <span class="li-normal">type: str</span> <span class="li-normal">choices: enable, disable</span></li>
            <li> <span class="li-head">dtim</span> - Delivery Traffic Indication Map (DTIM) period (1 - 255). Set higher to save battery life of WiFi client in power-save mode. <span class="li-normal">type: int</span></li>
            <li> <span class="li-head">frag_threshold</span> - Maximum packet size that can be sent without fragmentation (800 - 2346 bytes). <span class="li-normal">type: int</span></li>
            <li> <span class="li-head">max_clients</span> - Maximum number of stations (STAs) or WiFi clients supported by the radio. Range depends on the hardware. <span class="li-normal">type: int</span></li>
            <li> <span class="li-head">max_distance</span> - Maximum expected distance between the AP and clients (0 - 54000 m). <span class="li-normal">type: int</span></li>
            <li> <span class="li-head">mode</span> - Mode of radio 2. Radio 2 can be disabled, configured as an access point, a rogue AP monitor, or a sniffer. <span class="li-normal">type: str</span> <span class="li-normal">choices: disabled, ap, monitor, sniffer</span></li>
            <li> <span class="li-head">power_level</span> - Radio power level as a percentage of the maximum transmit power (0 - 100). <span class="li-normal">type: int</span></li>
            <li> <span class="li-head">powersave_optimize</span> - Enable client power-saving features such as TIM, AC VO, and OBSS etc. <span class="li-normal">type: str</span> <span class="li-normal">choices: tim, ac-vo, no-obss-scan, no-11b-rate, client-rate-follow</span></li>
            <li> <span class="li-head">protection_mode</span> - Enable/disable 802.11g protection modes to support backwards compatibility with older clients (rtscts, ctsonly, disable). <span class="li-normal">type: str</span> <span class="li-normal">choices: rtscts, ctsonly, disable</span></li>
            <li> <span class="li-head">rts_threshold</span> - Maximum packet size for RTS transmissions, specifying the maximum size of a data packet before RTS/CTS (256 - 2346 bytes). <span class="li-normal">type: int</span></li>
            <li> <span class="li-head">short_guard_interval</span> - Use either the short guard interval (Short GI) of 400 ns or the long guard interval (Long GI) of 800 ns. <span class="li-normal">type: str</span> <span class="li-normal">choices: enable, disable</span></li>
            <li> <span class="li-head">spectrum_analysis</span> - Enable/disable spectrum analysis to find interference that would negatively impact wireless performance. <span class="li-normal">type: str</span> <span class="li-normal">choices: enable, scan-only, disable</span></li>
            <li> <span class="li-head">transmit_optimize</span> - Packet transmission optimization options including power saving, aggregation limiting, retry limiting, etc. All are enabled by default. <span class="li-normal">type: str</span> <span class="li-normal">choices: disable, power-save, aggr-limit, retry-limit, send-bar</span></li>
            <li> <span class="li-head">vap_all</span> - Enable/disable the automatic inheritance of all Virtual Access Points (VAPs) . <span class="li-normal">type: str</span> <span class="li-normal">choices: enable, disable</span></li>
            <li> <span class="li-head">vaps</span> - Manually selected list of Virtual Access Points (VAPs). <span class="li-normal">type: list</span></li>
                <ul class="ul-self">
                <li> <span class="li-head">name</span> - Virtual Access Point (VAP) name. Source wireless-controller.vap-group.name system.interface.name. <span class="li-normal">type: str</span> <span class="li-required">required: True</span></li>
                </ul>
            <li> <span class="li-head">wids_profile</span> - Wireless Intrusion Detection System (WIDS) profile name to assign to the radio. Source wireless-controller.wids-profile.name. <span class="li-normal">type: str</span></li>
            <li> <span class="li-head">zero_wait_dfs</span> - Enable/disable zero wait DFS on radio . <span class="li-normal">type: str</span> <span class="li-normal">choices: enable, disable</span></li>
            </ul>
        <li> <span class="li-head">radio_3</span> - Configuration options for radio 3. <span class="li-normal">type: dict</span></li>
            <ul class="ul-self">
            <li> <span class="li-head">airtime_fairness</span> - Enable/disable airtime fairness . <span class="li-normal">type: str</span> <span class="li-normal">choices: enable, disable</span></li>
            <li> <span class="li-head">amsdu</span> - Enable/disable 802.11n AMSDU support. AMSDU can improve performance if supported by your WiFi clients . <span class="li-normal">type: str</span> <span class="li-normal">choices: enable, disable</span></li>
            <li> <span class="li-head">ap_sniffer_addr</span> - MAC address to monitor. <span class="li-normal">type: str</span></li>
            <li> <span class="li-head">ap_sniffer_bufsize</span> - Sniffer buffer size (1 - 32 MB). <span class="li-normal">type: int</span></li>
            <li> <span class="li-head">ap_sniffer_chan</span> - Channel on which to operate the sniffer . <span class="li-normal">type: int</span></li>
            <li> <span class="li-head">ap_sniffer_ctl</span> - Enable/disable sniffer on WiFi control frame . <span class="li-normal">type: str</span> <span class="li-normal">choices: enable, disable</span></li>
            <li> <span class="li-head">ap_sniffer_data</span> - Enable/disable sniffer on WiFi data frame . <span class="li-normal">type: str</span> <span class="li-normal">choices: enable, disable</span></li>
            <li> <span class="li-head">ap_sniffer_mgmt_beacon</span> - Enable/disable sniffer on WiFi management Beacon frames . <span class="li-normal">type: str</span> <span class="li-normal">choices: enable, disable</span></li>
            <li> <span class="li-head">ap_sniffer_mgmt_other</span> - Enable/disable sniffer on WiFi management other frames  . <span class="li-normal">type: str</span> <span class="li-normal">choices: enable, disable</span></li>
            <li> <span class="li-head">ap_sniffer_mgmt_probe</span> - Enable/disable sniffer on WiFi management probe frames . <span class="li-normal">type: str</span> <span class="li-normal">choices: enable, disable</span></li>
            <li> <span class="li-head">auto_power_high</span> - The upper bound of automatic transmit power adjustment in dBm (the actual range of transmit power depends on the AP platform type). <span class="li-normal">type: int</span></li>
            <li> <span class="li-head">auto_power_level</span> - Enable/disable automatic power-level adjustment to prevent co-channel interference . <span class="li-normal">type: str</span> <span class="li-normal">choices: enable, disable</span></li>
            <li> <span class="li-head">auto_power_low</span> - The lower bound of automatic transmit power adjustment in dBm (the actual range of transmit power depends on the AP platform type). <span class="li-normal">type: int</span></li>
            <li> <span class="li-head">band</span> - WiFi band that Radio 3 operates on. <span class="li-normal">type: str</span> <span class="li-normal">choices: 802.11a, 802.11b, 802.11g, 802.11n, 802.11n-5G, 802.11ac, 802.11ax-5G, 802.11ax, 802.11n,g-only, 802.11g-only, 802.11n-only, 802.11n-5G-only, 802.11ac,n-only, 802.11ac-only, 802.11ax,ac-only, 802.11ax,ac,n-only, 802.11ax-5G-only, 802.11ax,n-only, 802.11ax,n,g-only, 802.11ax-only</span></li>
            <li> <span class="li-head">band_5g_type</span> - WiFi 5G band type. <span class="li-normal">type: str</span> <span class="li-normal">choices: 5g-full, 5g-high, 5g-low</span></li>
            <li> <span class="li-head">bandwidth_admission_control</span> - Enable/disable WiFi multimedia (WMM) bandwidth admission control to optimize WiFi bandwidth use. A request to join the wireless network is only allowed if the access point has enough bandwidth to support it. <span class="li-normal">type: str</span> <span class="li-normal">choices: enable, disable</span></li>
            <li> <span class="li-head">bandwidth_capacity</span> - Maximum bandwidth capacity allowed (1 - 600000 Kbps). <span class="li-normal">type: int</span></li>
            <li> <span class="li-head">beacon_interval</span> - Beacon interval. The time between beacon frames in msec (the actual range of beacon interval depends on the AP platform type). <span class="li-normal">type: int</span></li>
            <li> <span class="li-head">call_admission_control</span> - Enable/disable WiFi multimedia (WMM) call admission control to optimize WiFi bandwidth use for VoIP calls. New VoIP calls are only accepted if there is enough bandwidth available to support them. <span class="li-normal">type: str</span> <span class="li-normal">choices: enable, disable</span></li>
            <li> <span class="li-head">call_capacity</span> - Maximum number of Voice over WLAN (VoWLAN) phones supported by the radio (0 - 60). <span class="li-normal">type: int</span></li>
            <li> <span class="li-head">channel</span> - Selected list of wireless radio channels. <span class="li-normal">type: list</span></li>
                <ul class="ul-self">
                <li> <span class="li-head">chan</span> - Channel number. <span class="li-normal">type: str</span> <span class="li-required">required: True</span></li>
                </ul>
            <li> <span class="li-head">channel_bonding</span> - Channel bandwidth: 160,80, 40, or 20MHz. Channels may use both 20 and 40 by enabling coexistence. <span class="li-normal">type: str</span> <span class="li-normal">choices: 160MHz, 80MHz, 40MHz, 20MHz</span></li>
            <li> <span class="li-head">channel_utilization</span> - Enable/disable measuring channel utilization. <span class="li-normal">type: str</span> <span class="li-normal">choices: enable, disable</span></li>
            <li> <span class="li-head">coexistence</span> - Enable/disable allowing both HT20 and HT40 on the same radio . <span class="li-normal">type: str</span> <span class="li-normal">choices: enable, disable</span></li>
            <li> <span class="li-head">darrp</span> - Enable/disable Distributed Automatic Radio Resource Provisioning (DARRP) to make sure the radio is always using the most optimal channel . <span class="li-normal">type: str</span> <span class="li-normal">choices: enable, disable</span></li>
            <li> <span class="li-head">dtim</span> - Delivery Traffic Indication Map (DTIM) period (1 - 255). Set higher to save battery life of WiFi client in power-save mode. <span class="li-normal">type: int</span></li>
            <li> <span class="li-head">frag_threshold</span> - Maximum packet size that can be sent without fragmentation (800 - 2346 bytes). <span class="li-normal">type: int</span></li>
            <li> <span class="li-head">max_clients</span> - Maximum number of stations (STAs) or WiFi clients supported by the radio. Range depends on the hardware. <span class="li-normal">type: int</span></li>
            <li> <span class="li-head">max_distance</span> - Maximum expected distance between the AP and clients (0 - 54000 m). <span class="li-normal">type: int</span></li>
            <li> <span class="li-head">mode</span> - Mode of radio 3. Radio 3 can be disabled, configured as an access point, a rogue AP monitor, or a sniffer. <span class="li-normal">type: str</span> <span class="li-normal">choices: disabled, ap, monitor, sniffer</span></li>
            <li> <span class="li-head">power_level</span> - Radio power level as a percentage of the maximum transmit power (0 - 100). <span class="li-normal">type: int</span></li>
            <li> <span class="li-head">powersave_optimize</span> - Enable client power-saving features such as TIM, AC VO, and OBSS etc. <span class="li-normal">type: str</span> <span class="li-normal">choices: tim, ac-vo, no-obss-scan, no-11b-rate, client-rate-follow</span></li>
            <li> <span class="li-head">protection_mode</span> - Enable/disable 802.11g protection modes to support backwards compatibility with older clients (rtscts, ctsonly, disable). <span class="li-normal">type: str</span> <span class="li-normal">choices: rtscts, ctsonly, disable</span></li>
            <li> <span class="li-head">rts_threshold</span> - Maximum packet size for RTS transmissions, specifying the maximum size of a data packet before RTS/CTS (256 - 2346 bytes). <span class="li-normal">type: int</span></li>
            <li> <span class="li-head">short_guard_interval</span> - Use either the short guard interval (Short GI) of 400 ns or the long guard interval (Long GI) of 800 ns. <span class="li-normal">type: str</span> <span class="li-normal">choices: enable, disable</span></li>
            <li> <span class="li-head">spectrum_analysis</span> - Enable/disable spectrum analysis to find interference that would negatively impact wireless performance. <span class="li-normal">type: str</span> <span class="li-normal">choices: enable, scan-only, disable</span></li>
            <li> <span class="li-head">transmit_optimize</span> - Packet transmission optimization options including power saving, aggregation limiting, retry limiting, etc. All are enabled by default. <span class="li-normal">type: str</span> <span class="li-normal">choices: disable, power-save, aggr-limit, retry-limit, send-bar</span></li>
            <li> <span class="li-head">vap_all</span> - Enable/disable the automatic inheritance of all Virtual Access Points (VAPs) . <span class="li-normal">type: str</span> <span class="li-normal">choices: enable, disable</span></li>
            <li> <span class="li-head">vaps</span> - Manually selected list of Virtual Access Points (VAPs). <span class="li-normal">type: list</span></li>
                <ul class="ul-self">
                <li> <span class="li-head">name</span> - Virtual Access Point (VAP) name. Source wireless-controller.vap-group.name system.interface.name. <span class="li-normal">type: str</span> <span class="li-required">required: True</span></li>
                </ul>
            <li> <span class="li-head">wids_profile</span> - Wireless Intrusion Detection System (WIDS) profile name to assign to the radio. Source wireless-controller.wids-profile.name. <span class="li-normal">type: str</span></li>
            <li> <span class="li-head">zero_wait_dfs</span> - Enable/disable zero wait DFS on radio . <span class="li-normal">type: str</span> <span class="li-normal">choices: enable, disable</span></li>
            </ul>
        <li> <span class="li-head">radio_4</span> - Configuration options for radio 4. <span class="li-normal">type: dict</span></li>
            <ul class="ul-self">
            <li> <span class="li-head">airtime_fairness</span> - Enable/disable airtime fairness . <span class="li-normal">type: str</span> <span class="li-normal">choices: enable, disable</span></li>
            <li> <span class="li-head">amsdu</span> - Enable/disable 802.11n AMSDU support. AMSDU can improve performance if supported by your WiFi clients . <span class="li-normal">type: str</span> <span class="li-normal">choices: enable, disable</span></li>
            <li> <span class="li-head">ap_sniffer_addr</span> - MAC address to monitor. <span class="li-normal">type: str</span></li>
            <li> <span class="li-head">ap_sniffer_bufsize</span> - Sniffer buffer size (1 - 32 MB). <span class="li-normal">type: int</span></li>
            <li> <span class="li-head">ap_sniffer_chan</span> - Channel on which to operate the sniffer . <span class="li-normal">type: int</span></li>
            <li> <span class="li-head">ap_sniffer_ctl</span> - Enable/disable sniffer on WiFi control frame . <span class="li-normal">type: str</span> <span class="li-normal">choices: enable, disable</span></li>
            <li> <span class="li-head">ap_sniffer_data</span> - Enable/disable sniffer on WiFi data frame . <span class="li-normal">type: str</span> <span class="li-normal">choices: enable, disable</span></li>
            <li> <span class="li-head">ap_sniffer_mgmt_beacon</span> - Enable/disable sniffer on WiFi management Beacon frames . <span class="li-normal">type: str</span> <span class="li-normal">choices: enable, disable</span></li>
            <li> <span class="li-head">ap_sniffer_mgmt_other</span> - Enable/disable sniffer on WiFi management other frames  . <span class="li-normal">type: str</span> <span class="li-normal">choices: enable, disable</span></li>
            <li> <span class="li-head">ap_sniffer_mgmt_probe</span> - Enable/disable sniffer on WiFi management probe frames . <span class="li-normal">type: str</span> <span class="li-normal">choices: enable, disable</span></li>
            <li> <span class="li-head">auto_power_high</span> - The upper bound of automatic transmit power adjustment in dBm (the actual range of transmit power depends on the AP platform type). <span class="li-normal">type: int</span></li>
            <li> <span class="li-head">auto_power_level</span> - Enable/disable automatic power-level adjustment to prevent co-channel interference . <span class="li-normal">type: str</span> <span class="li-normal">choices: enable, disable</span></li>
            <li> <span class="li-head">auto_power_low</span> - The lower bound of automatic transmit power adjustment in dBm (the actual range of transmit power depends on the AP platform type). <span class="li-normal">type: int</span></li>
            <li> <span class="li-head">band</span> - WiFi band that Radio 3 operates on. <span class="li-normal">type: str</span> <span class="li-normal">choices: 802.11a, 802.11b, 802.11g, 802.11n, 802.11n-5G, 802.11ac, 802.11ax-5G, 802.11ax, 802.11n,g-only, 802.11g-only, 802.11n-only, 802.11n-5G-only, 802.11ac,n-only, 802.11ac-only, 802.11ax,ac-only, 802.11ax,ac,n-only, 802.11ax-5G-only, 802.11ax,n-only, 802.11ax,n,g-only, 802.11ax-only</span></li>
            <li> <span class="li-head">band_5g_type</span> - WiFi 5G band type. <span class="li-normal">type: str</span> <span class="li-normal">choices: 5g-full, 5g-high, 5g-low</span></li>
            <li> <span class="li-head">bandwidth_admission_control</span> - Enable/disable WiFi multimedia (WMM) bandwidth admission control to optimize WiFi bandwidth use. A request to join the wireless network is only allowed if the access point has enough bandwidth to support it. <span class="li-normal">type: str</span> <span class="li-normal">choices: enable, disable</span></li>
            <li> <span class="li-head">bandwidth_capacity</span> - Maximum bandwidth capacity allowed (1 - 600000 Kbps). <span class="li-normal">type: int</span></li>
            <li> <span class="li-head">beacon_interval</span> - Beacon interval. The time between beacon frames in msec (the actual range of beacon interval depends on the AP platform type). <span class="li-normal">type: int</span></li>
            <li> <span class="li-head">call_admission_control</span> - Enable/disable WiFi multimedia (WMM) call admission control to optimize WiFi bandwidth use for VoIP calls. New VoIP calls are only accepted if there is enough bandwidth available to support them. <span class="li-normal">type: str</span> <span class="li-normal">choices: enable, disable</span></li>
            <li> <span class="li-head">call_capacity</span> - Maximum number of Voice over WLAN (VoWLAN) phones supported by the radio (0 - 60). <span class="li-normal">type: int</span></li>
            <li> <span class="li-head">channel</span> - Selected list of wireless radio channels. <span class="li-normal">type: list</span></li>
                <ul class="ul-self">
                <li> <span class="li-head">chan</span> - Channel number. <span class="li-normal">type: str</span> <span class="li-required">required: True</span></li>
                </ul>
            <li> <span class="li-head">channel_bonding</span> - Channel bandwidth: 160,80, 40, or 20MHz. Channels may use both 20 and 40 by enabling coexistence. <span class="li-normal">type: str</span> <span class="li-normal">choices: 160MHz, 80MHz, 40MHz, 20MHz</span></li>
            <li> <span class="li-head">channel_utilization</span> - Enable/disable measuring channel utilization. <span class="li-normal">type: str</span> <span class="li-normal">choices: enable, disable</span></li>
            <li> <span class="li-head">coexistence</span> - Enable/disable allowing both HT20 and HT40 on the same radio . <span class="li-normal">type: str</span> <span class="li-normal">choices: enable, disable</span></li>
            <li> <span class="li-head">darrp</span> - Enable/disable Distributed Automatic Radio Resource Provisioning (DARRP) to make sure the radio is always using the most optimal channel . <span class="li-normal">type: str</span> <span class="li-normal">choices: enable, disable</span></li>
            <li> <span class="li-head">dtim</span> - Delivery Traffic Indication Map (DTIM) period (1 - 255). Set higher to save battery life of WiFi client in power-save mode. <span class="li-normal">type: int</span></li>
            <li> <span class="li-head">frag_threshold</span> - Maximum packet size that can be sent without fragmentation (800 - 2346 bytes). <span class="li-normal">type: int</span></li>
            <li> <span class="li-head">max_clients</span> - Maximum number of stations (STAs) or WiFi clients supported by the radio. Range depends on the hardware. <span class="li-normal">type: int</span></li>
            <li> <span class="li-head">max_distance</span> - Maximum expected distance between the AP and clients (0 - 54000 m). <span class="li-normal">type: int</span></li>
            <li> <span class="li-head">mode</span> - Mode of radio 3. Radio 3 can be disabled, configured as an access point, a rogue AP monitor, or a sniffer. <span class="li-normal">type: str</span> <span class="li-normal">choices: disabled, ap, monitor, sniffer</span></li>
            <li> <span class="li-head">power_level</span> - Radio power level as a percentage of the maximum transmit power (0 - 100). <span class="li-normal">type: int</span></li>
            <li> <span class="li-head">powersave_optimize</span> - Enable client power-saving features such as TIM, AC VO, and OBSS etc. <span class="li-normal">type: str</span> <span class="li-normal">choices: tim, ac-vo, no-obss-scan, no-11b-rate, client-rate-follow</span></li>
            <li> <span class="li-head">protection_mode</span> - Enable/disable 802.11g protection modes to support backwards compatibility with older clients (rtscts, ctsonly, disable). <span class="li-normal">type: str</span> <span class="li-normal">choices: rtscts, ctsonly, disable</span></li>
            <li> <span class="li-head">rts_threshold</span> - Maximum packet size for RTS transmissions, specifying the maximum size of a data packet before RTS/CTS (256 - 2346 bytes). <span class="li-normal">type: int</span></li>
            <li> <span class="li-head">short_guard_interval</span> - Use either the short guard interval (Short GI) of 400 ns or the long guard interval (Long GI) of 800 ns. <span class="li-normal">type: str</span> <span class="li-normal">choices: enable, disable</span></li>
            <li> <span class="li-head">spectrum_analysis</span> - Enable/disable spectrum analysis to find interference that would negatively impact wireless performance. <span class="li-normal">type: str</span> <span class="li-normal">choices: enable, scan-only, disable</span></li>
            <li> <span class="li-head">transmit_optimize</span> - Packet transmission optimization options including power saving, aggregation limiting, retry limiting, etc. All are enabled by default. <span class="li-normal">type: str</span> <span class="li-normal">choices: disable, power-save, aggr-limit, retry-limit, send-bar</span></li>
            <li> <span class="li-head">vap_all</span> - Enable/disable the automatic inheritance of all Virtual Access Points (VAPs) . <span class="li-normal">type: str</span> <span class="li-normal">choices: enable, disable</span></li>
            <li> <span class="li-head">vaps</span> - Manually selected list of Virtual Access Points (VAPs). <span class="li-normal">type: list</span></li>
                <ul class="ul-self">
                <li> <span class="li-head">name</span> - Virtual Access Point (VAP) name. Source wireless-controller.vap-group.name system.interface.name. <span class="li-normal">type: str</span> <span class="li-required">required: True</span></li>
                </ul>
            <li> <span class="li-head">wids_profile</span> - Wireless Intrusion Detection System (WIDS) profile name to assign to the radio. Source wireless-controller.wids-profile.name. <span class="li-normal">type: str</span></li>
            <li> <span class="li-head">zero_wait_dfs</span> - Enable/disable zero wait DFS on radio . <span class="li-normal">type: str</span> <span class="li-normal">choices: enable, disable</span></li>
            </ul>
        <li> <span class="li-head">split_tunneling_acl</span> - Split tunneling ACL filter list. <span class="li-normal">type: list</span></li>
            <ul class="ul-self">
            <li> <span class="li-head">dest_ip</span> - Destination IP and mask for the split-tunneling subnet. <span class="li-normal">type: str</span></li>
            <li> <span class="li-head">id</span> - ID. <span class="li-normal">type: int</span> <span class="li-required">required: True</span></li>
            </ul>
        <li> <span class="li-head">split_tunneling_acl_local_ap_subnet</span> - Enable/disable automatically adding local subnetwork of FortiAP to split-tunneling ACL . <span class="li-normal">type: str</span> <span class="li-normal">choices: enable, disable</span></li>
        <li> <span class="li-head">split_tunneling_acl_path</span> - Split tunneling ACL path is local/tunnel. <span class="li-normal">type: str</span> <span class="li-normal">choices: tunnel, local</span></li>
        <li> <span class="li-head">tun_mtu_downlink</span> - The MTU of downlink CAPWAP tunnel (576 - 1500 bytes or 0; 0 means the local MTU of FortiAP; ). <span class="li-normal">type: int</span></li>
        <li> <span class="li-head">tun_mtu_uplink</span> - The maximum transmission unit (MTU) of uplink CAPWAP tunnel (576 - 1500 bytes or 0; 0 means the local MTU of FortiAP; ). <span class="li-normal">type: int</span></li>
        <li> <span class="li-head">wan_port_mode</span> - Enable/disable using a WAN port as a LAN port. <span class="li-normal">type: str</span> <span class="li-normal">choices: wan-lan, wan-only</span></li>
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
      - name: Configure WTP profiles or FortiAP profiles that define radio settings for manageable FortiAP platforms.
        fortios_wireless_controller_wtp_profile:
          vdom:  "{{ vdom }}"
          state: "present"
          access_token: "<your_own_value>"
          wireless_controller_wtp_profile:
            allowaccess: "https"
            ap_country: "NA"
            ap_handoff: "enable"
            apcfg_profile: "<your_own_value> (source wireless-controller.apcfg-profile.name)"
            ble_profile: "<your_own_value> (source wireless-controller.ble-profile.name)"
            comment: "Comment."
            control_message_offload: "ebp-frame"
            deny_mac_list:
             -
                id:  "11"
                mac: "<your_own_value>"
            dtls_in_kernel: "enable"
            dtls_policy: "clear-text"
            energy_efficient_ethernet: "enable"
            ext_info_enable: "enable"
            frequency_handoff: "enable"
            handoff_roaming: "enable"
            handoff_rssi: "19"
            handoff_sta_thresh: "20"
            ip_fragment_preventing: "tcp-mss-adjust"
            lan:
                port_mode: "offline"
                port_ssid: "<your_own_value> (source system.interface.name)"
                port1_mode: "offline"
                port1_ssid: "<your_own_value> (source system.interface.name)"
                port2_mode: "offline"
                port2_ssid: "<your_own_value> (source system.interface.name)"
                port3_mode: "offline"
                port3_ssid: "<your_own_value> (source system.interface.name)"
                port4_mode: "offline"
                port4_ssid: "<your_own_value> (source system.interface.name)"
                port5_mode: "offline"
                port5_ssid: "<your_own_value> (source system.interface.name)"
                port6_mode: "offline"
                port6_ssid: "<your_own_value> (source system.interface.name)"
                port7_mode: "offline"
                port7_ssid: "<your_own_value> (source system.interface.name)"
                port8_mode: "offline"
                port8_ssid: "<your_own_value> (source system.interface.name)"
            lbs:
                aeroscout: "enable"
                aeroscout_ap_mac: "bssid"
                aeroscout_mmu_report: "enable"
                aeroscout_mu: "enable"
                aeroscout_mu_factor: "46"
                aeroscout_mu_timeout: "47"
                aeroscout_server_ip: "<your_own_value>"
                aeroscout_server_port: "49"
                ekahau_blink_mode: "enable"
                ekahau_tag: "<your_own_value>"
                erc_server_ip: "<your_own_value>"
                erc_server_port: "53"
                fortipresence: "foreign"
                fortipresence_ble: "enable"
                fortipresence_frequency: "56"
                fortipresence_port: "57"
                fortipresence_project: "<your_own_value>"
                fortipresence_rogue: "enable"
                fortipresence_secret: "<your_own_value>"
                fortipresence_server: "<your_own_value>"
                fortipresence_unassoc: "enable"
                station_locate: "enable"
            led_schedules:
             -
                name: "default_name_65 (source firewall.schedule.group.name firewall.schedule.recurring.name firewall.schedule.onetime.name)"
            led_state: "enable"
            lldp: "enable"
            login_passwd: "<your_own_value>"
            login_passwd_change: "yes"
            max_clients: "70"
            name: "default_name_71"
            platform:
                ddscan: "enable"
                mode: "single-5G"
                type: "AP-11N"
            poe_mode: "auto"
            radio_1:
                airtime_fairness: "enable"
                amsdu: "enable"
                ap_sniffer_addr: "<your_own_value>"
                ap_sniffer_bufsize: "81"
                ap_sniffer_chan: "82"
                ap_sniffer_ctl: "enable"
                ap_sniffer_data: "enable"
                ap_sniffer_mgmt_beacon: "enable"
                ap_sniffer_mgmt_other: "enable"
                ap_sniffer_mgmt_probe: "enable"
                auto_power_high: "88"
                auto_power_level: "enable"
                auto_power_low: "90"
                band: "802.11a"
                band_5g_type: "5g-full"
                bandwidth_admission_control: "enable"
                bandwidth_capacity: "94"
                beacon_interval: "95"
                call_admission_control: "enable"
                call_capacity: "97"
                channel:
                 -
                    chan: "<your_own_value>"
                channel_bonding: "160MHz"
                channel_utilization: "enable"
                coexistence: "enable"
                darrp: "enable"
                dtim: "104"
                frag_threshold: "105"
                max_clients: "106"
                max_distance: "107"
                mode: "disabled"
                power_level: "109"
                powersave_optimize: "tim"
                protection_mode: "rtscts"
                rts_threshold: "112"
                short_guard_interval: "enable"
                spectrum_analysis: "enable"
                transmit_optimize: "disable"
                vap_all: "enable"
                vaps:
                 -
                    name: "default_name_118 (source wireless-controller.vap-group.name system.interface.name)"
                wids_profile: "<your_own_value> (source wireless-controller.wids-profile.name)"
                zero_wait_dfs: "enable"
            radio_2:
                airtime_fairness: "enable"
                amsdu: "enable"
                ap_sniffer_addr: "<your_own_value>"
                ap_sniffer_bufsize: "125"
                ap_sniffer_chan: "126"
                ap_sniffer_ctl: "enable"
                ap_sniffer_data: "enable"
                ap_sniffer_mgmt_beacon: "enable"
                ap_sniffer_mgmt_other: "enable"
                ap_sniffer_mgmt_probe: "enable"
                auto_power_high: "132"
                auto_power_level: "enable"
                auto_power_low: "134"
                band: "802.11a"
                band_5g_type: "5g-full"
                bandwidth_admission_control: "enable"
                bandwidth_capacity: "138"
                beacon_interval: "139"
                call_admission_control: "enable"
                call_capacity: "141"
                channel:
                 -
                    chan: "<your_own_value>"
                channel_bonding: "160MHz"
                channel_utilization: "enable"
                coexistence: "enable"
                darrp: "enable"
                dtim: "148"
                frag_threshold: "149"
                max_clients: "150"
                max_distance: "151"
                mode: "disabled"
                power_level: "153"
                powersave_optimize: "tim"
                protection_mode: "rtscts"
                rts_threshold: "156"
                short_guard_interval: "enable"
                spectrum_analysis: "enable"
                transmit_optimize: "disable"
                vap_all: "enable"
                vaps:
                 -
                    name: "default_name_162 (source wireless-controller.vap-group.name system.interface.name)"
                wids_profile: "<your_own_value> (source wireless-controller.wids-profile.name)"
                zero_wait_dfs: "enable"
            radio_3:
                airtime_fairness: "enable"
                amsdu: "enable"
                ap_sniffer_addr: "<your_own_value>"
                ap_sniffer_bufsize: "169"
                ap_sniffer_chan: "170"
                ap_sniffer_ctl: "enable"
                ap_sniffer_data: "enable"
                ap_sniffer_mgmt_beacon: "enable"
                ap_sniffer_mgmt_other: "enable"
                ap_sniffer_mgmt_probe: "enable"
                auto_power_high: "176"
                auto_power_level: "enable"
                auto_power_low: "178"
                band: "802.11a"
                band_5g_type: "5g-full"
                bandwidth_admission_control: "enable"
                bandwidth_capacity: "182"
                beacon_interval: "183"
                call_admission_control: "enable"
                call_capacity: "185"
                channel:
                 -
                    chan: "<your_own_value>"
                channel_bonding: "160MHz"
                channel_utilization: "enable"
                coexistence: "enable"
                darrp: "enable"
                dtim: "192"
                frag_threshold: "193"
                max_clients: "194"
                max_distance: "195"
                mode: "disabled"
                power_level: "197"
                powersave_optimize: "tim"
                protection_mode: "rtscts"
                rts_threshold: "200"
                short_guard_interval: "enable"
                spectrum_analysis: "enable"
                transmit_optimize: "disable"
                vap_all: "enable"
                vaps:
                 -
                    name: "default_name_206 (source wireless-controller.vap-group.name system.interface.name)"
                wids_profile: "<your_own_value> (source wireless-controller.wids-profile.name)"
                zero_wait_dfs: "enable"
            radio_4:
                airtime_fairness: "enable"
                amsdu: "enable"
                ap_sniffer_addr: "<your_own_value>"
                ap_sniffer_bufsize: "213"
                ap_sniffer_chan: "214"
                ap_sniffer_ctl: "enable"
                ap_sniffer_data: "enable"
                ap_sniffer_mgmt_beacon: "enable"
                ap_sniffer_mgmt_other: "enable"
                ap_sniffer_mgmt_probe: "enable"
                auto_power_high: "220"
                auto_power_level: "enable"
                auto_power_low: "222"
                band: "802.11a"
                band_5g_type: "5g-full"
                bandwidth_admission_control: "enable"
                bandwidth_capacity: "226"
                beacon_interval: "227"
                call_admission_control: "enable"
                call_capacity: "229"
                channel:
                 -
                    chan: "<your_own_value>"
                channel_bonding: "160MHz"
                channel_utilization: "enable"
                coexistence: "enable"
                darrp: "enable"
                dtim: "236"
                frag_threshold: "237"
                max_clients: "238"
                max_distance: "239"
                mode: "disabled"
                power_level: "241"
                powersave_optimize: "tim"
                protection_mode: "rtscts"
                rts_threshold: "244"
                short_guard_interval: "enable"
                spectrum_analysis: "enable"
                transmit_optimize: "disable"
                vap_all: "enable"
                vaps:
                 -
                    name: "default_name_250 (source wireless-controller.vap-group.name system.interface.name)"
                wids_profile: "<your_own_value> (source wireless-controller.wids-profile.name)"
                zero_wait_dfs: "enable"
            split_tunneling_acl:
             -
                dest_ip: "<your_own_value>"
                id:  "255"
            split_tunneling_acl_local_ap_subnet: "enable"
            split_tunneling_acl_path: "tunnel"
            tun_mtu_downlink: "258"
            tun_mtu_uplink: "259"
            wan_port_mode: "wan-lan"
    


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
