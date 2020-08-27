:source: fortios_wireless_controller_wtp.py

:orphan:

.. fortios_wireless_controller_wtp:

fortios_wireless_controller_wtp -- Configure Wireless Termination Points (WTPs), that is, FortiAPs or APs to be managed by FortiGate in Fortinet's FortiOS and FortiGate.
+++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++

.. versionadded:: 2.8

.. contents::
   :local:
   :depth: 1


Synopsis
--------
- This module is able to configure a FortiGate or FortiOS (FOS) device by allowing the user to set and modify wireless_controller feature and wtp category. Examples include all parameters and values need to be adjusted to datasources before usage. Tested with FOS v6.0.0



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
    <li> <span class="li-head">wireless_controller_wtp</span> - Configure Wireless Termination Points (WTPs), that is, FortiAPs or APs to be managed by FortiGate. <span class="li-normal">type: dict</span></li>
        <ul class="ul-self">
        <li> <span class="li-head">state</span> - B(Deprecated) <span class="li-normal">type: str</span> <span class="li-required">required: False</span> <span class="li-normal">choices: present, absent</span></li>
        <li> <span class="li-head">admin</span> - Configure how the FortiGate operating as a wireless controller discovers and manages this WTP, AP or FortiAP. <span class="li-normal">type: str</span> <span class="li-normal">choices: discovered, disable, enable</span></li>
        <li> <span class="li-head">allowaccess</span> - Control management access to the managed WTP, FortiAP, or AP. Separate entries with a space. <span class="li-normal">type: str</span> <span class="li-normal">choices: telnet, http, https, ssh</span></li>
        <li> <span class="li-head">bonjour_profile</span> - Bonjour profile name. Source wireless-controller.bonjour-profile.name. <span class="li-normal">type: str</span></li>
        <li> <span class="li-head">coordinate_enable</span> - Enable/disable WTP coordinates (X,Y axis). <span class="li-normal">type: str</span> <span class="li-normal">choices: enable, disable</span></li>
        <li> <span class="li-head">coordinate_latitude</span> - WTP latitude coordinate. <span class="li-normal">type: str</span></li>
        <li> <span class="li-head">coordinate_longitude</span> - WTP longitude coordinate. <span class="li-normal">type: str</span></li>
        <li> <span class="li-head">coordinate_x</span> - X axis coordinate. <span class="li-normal">type: str</span></li>
        <li> <span class="li-head">coordinate_y</span> - Y axis coordinate. <span class="li-normal">type: str</span></li>
        <li> <span class="li-head">image_download</span> - Enable/disable WTP image download. <span class="li-normal">type: str</span> <span class="li-normal">choices: enable, disable</span></li>
        <li> <span class="li-head">index</span> - Index (0 - 4294967295). <span class="li-normal">type: int</span></li>
        <li> <span class="li-head">ip_fragment_preventing</span> - Method by which IP fragmentation is prevented for CAPWAP tunneled control and data packets . <span class="li-normal">type: str</span> <span class="li-normal">choices: tcp-mss-adjust, icmp-unreachable</span></li>
        <li> <span class="li-head">lan</span> - WTP LAN port mapping. <span class="li-normal">type: dict</span></li>
            <ul class="ul-self">
            <li> <span class="li-head">port_mode</span> - LAN port mode. <span class="li-normal">type: str</span> <span class="li-normal">choices: offline, nat-to-wan, bridge-to-wan, bridge-to-ssid</span></li>
            <li> <span class="li-head">port_ssid</span> - Bridge LAN port to SSID. Source wireless-controller.vap.name. <span class="li-normal">type: str</span></li>
            <li> <span class="li-head">port1_mode</span> - LAN port 1 mode. <span class="li-normal">type: str</span> <span class="li-normal">choices: offline, nat-to-wan, bridge-to-wan, bridge-to-ssid</span></li>
            <li> <span class="li-head">port1_ssid</span> - Bridge LAN port 1 to SSID. Source wireless-controller.vap.name. <span class="li-normal">type: str</span></li>
            <li> <span class="li-head">port2_mode</span> - LAN port 2 mode. <span class="li-normal">type: str</span> <span class="li-normal">choices: offline, nat-to-wan, bridge-to-wan, bridge-to-ssid</span></li>
            <li> <span class="li-head">port2_ssid</span> - Bridge LAN port 2 to SSID. Source wireless-controller.vap.name. <span class="li-normal">type: str</span></li>
            <li> <span class="li-head">port3_mode</span> - LAN port 3 mode. <span class="li-normal">type: str</span> <span class="li-normal">choices: offline, nat-to-wan, bridge-to-wan, bridge-to-ssid</span></li>
            <li> <span class="li-head">port3_ssid</span> - Bridge LAN port 3 to SSID. Source wireless-controller.vap.name. <span class="li-normal">type: str</span></li>
            <li> <span class="li-head">port4_mode</span> - LAN port 4 mode. <span class="li-normal">type: str</span> <span class="li-normal">choices: offline, nat-to-wan, bridge-to-wan, bridge-to-ssid</span></li>
            <li> <span class="li-head">port4_ssid</span> - Bridge LAN port 4 to SSID. Source wireless-controller.vap.name. <span class="li-normal">type: str</span></li>
            <li> <span class="li-head">port5_mode</span> - LAN port 5 mode. <span class="li-normal">type: str</span> <span class="li-normal">choices: offline, nat-to-wan, bridge-to-wan, bridge-to-ssid</span></li>
            <li> <span class="li-head">port5_ssid</span> - Bridge LAN port 5 to SSID. Source wireless-controller.vap.name. <span class="li-normal">type: str</span></li>
            <li> <span class="li-head">port6_mode</span> - LAN port 6 mode. <span class="li-normal">type: str</span> <span class="li-normal">choices: offline, nat-to-wan, bridge-to-wan, bridge-to-ssid</span></li>
            <li> <span class="li-head">port6_ssid</span> - Bridge LAN port 6 to SSID. Source wireless-controller.vap.name. <span class="li-normal">type: str</span></li>
            <li> <span class="li-head">port7_mode</span> - LAN port 7 mode. <span class="li-normal">type: str</span> <span class="li-normal">choices: offline, nat-to-wan, bridge-to-wan, bridge-to-ssid</span></li>
            <li> <span class="li-head">port7_ssid</span> - Bridge LAN port 7 to SSID. Source wireless-controller.vap.name. <span class="li-normal">type: str</span></li>
            <li> <span class="li-head">port8_mode</span> - LAN port 8 mode. <span class="li-normal">type: str</span> <span class="li-normal">choices: offline, nat-to-wan, bridge-to-wan, bridge-to-ssid</span></li>
            <li> <span class="li-head">port8_ssid</span> - Bridge LAN port 8 to SSID. Source wireless-controller.vap.name. <span class="li-normal">type: str</span></li>
            </ul>
        <li> <span class="li-head">led_state</span> - Enable to allow the FortiAPs LEDs to light. Disable to keep the LEDs off. You may want to keep the LEDs off so they are not distracting in low light areas etc. <span class="li-normal">type: str</span> <span class="li-normal">choices: enable, disable</span></li>
        <li> <span class="li-head">location</span> - Field for describing the physical location of the WTP, AP or FortiAP. <span class="li-normal">type: str</span></li>
        <li> <span class="li-head">login_passwd</span> - Set the managed WTP, FortiAP, or AP"s administrator password. <span class="li-normal">type: str</span></li>
        <li> <span class="li-head">login_passwd_change</span> - Change or reset the administrator password of a managed WTP, FortiAP or AP (yes, default, or no). <span class="li-normal">type: str</span> <span class="li-normal">choices: True, default, False</span></li>
        <li> <span class="li-head">mesh_bridge_enable</span> - Enable/disable mesh Ethernet bridge when WTP is configured as a mesh branch/leaf AP. <span class="li-normal">type: str</span> <span class="li-normal">choices: default, enable, disable</span></li>
        <li> <span class="li-head">name</span> - WTP, AP or FortiAP configuration name. <span class="li-normal">type: str</span></li>
        <li> <span class="li-head">override_allowaccess</span> - Enable to override the WTP profile management access configuration. <span class="li-normal">type: str</span> <span class="li-normal">choices: enable, disable</span></li>
        <li> <span class="li-head">override_ip_fragment</span> - Enable/disable overriding the WTP profile IP fragment prevention setting. <span class="li-normal">type: str</span> <span class="li-normal">choices: enable, disable</span></li>
        <li> <span class="li-head">override_lan</span> - Enable to override the WTP profile LAN port setting. <span class="li-normal">type: str</span> <span class="li-normal">choices: enable, disable</span></li>
        <li> <span class="li-head">override_led_state</span> - Enable to override the profile LED state setting for this FortiAP. You must enable this option to use the led-state command to turn off the FortiAP"s LEDs. <span class="li-normal">type: str</span> <span class="li-normal">choices: enable, disable</span></li>
        <li> <span class="li-head">override_login_passwd_change</span> - Enable to override the WTP profile login-password (administrator password) setting. <span class="li-normal">type: str</span> <span class="li-normal">choices: enable, disable</span></li>
        <li> <span class="li-head">override_split_tunnel</span> - Enable/disable overriding the WTP profile split tunneling setting. <span class="li-normal">type: str</span> <span class="li-normal">choices: enable, disable</span></li>
        <li> <span class="li-head">override_wan_port_mode</span> - Enable/disable overriding the wan-port-mode in the WTP profile. <span class="li-normal">type: str</span> <span class="li-normal">choices: enable, disable</span></li>
        <li> <span class="li-head">radio_1</span> - Configuration options for radio 1. <span class="li-normal">type: dict</span></li>
            <ul class="ul-self">
            <li> <span class="li-head">auto_power_high</span> - Automatic transmission power high limit in decibels (dB) of the measured power referenced to one milliwatt (mW), or dBm (10 - 17 dBm). <span class="li-normal">type: int</span></li>
            <li> <span class="li-head">auto_power_level</span> - Enable/disable automatic power-level adjustment to prevent co-channel interference . <span class="li-normal">type: str</span> <span class="li-normal">choices: enable, disable</span></li>
            <li> <span class="li-head">auto_power_low</span> - Automatic transmission power low limit in dBm (the actual range of transmit power depends on the AP platform type). <span class="li-normal">type: int</span></li>
            <li> <span class="li-head">band</span> - WiFi band that Radio 1 operates on. <span class="li-normal">type: str</span> <span class="li-normal">choices: 802.11a, 802.11b, 802.11g, 802.11n, 802.11n-5G, 802.11n,g-only, 802.11g-only, 802.11n-only, 802.11n-5G-only, 802.11ac, 802.11ac,n-only, 802.11ac-only</span></li>
            <li> <span class="li-head">channel</span> - Selected list of wireless radio channels. <span class="li-normal">type: list</span></li>
                <ul class="ul-self">
                <li> <span class="li-head">chan</span> - Channel number. <span class="li-normal">type: str</span> <span class="li-required">required: True</span></li>
                </ul>
            <li> <span class="li-head">override_analysis</span> - Enable to override the WTP profile spectrum analysis configuration. <span class="li-normal">type: str</span> <span class="li-normal">choices: enable, disable</span></li>
            <li> <span class="li-head">override_band</span> - Enable to override the WTP profile band setting. <span class="li-normal">type: str</span> <span class="li-normal">choices: enable, disable</span></li>
            <li> <span class="li-head">override_channel</span> - Enable to override WTP profile channel settings. <span class="li-normal">type: str</span> <span class="li-normal">choices: enable, disable</span></li>
            <li> <span class="li-head">override_txpower</span> - Enable to override the WTP profile power level configuration. <span class="li-normal">type: str</span> <span class="li-normal">choices: enable, disable</span></li>
            <li> <span class="li-head">override_vaps</span> - Enable to override WTP profile Virtual Access Point (VAP) settings. <span class="li-normal">type: str</span> <span class="li-normal">choices: enable, disable</span></li>
            <li> <span class="li-head">power_level</span> - Radio power level as a percentage of the maximum transmit power (0 - 100). <span class="li-normal">type: int</span></li>
            <li> <span class="li-head">radio_id</span> - radio-id <span class="li-normal">type: int</span></li>
            <li> <span class="li-head">spectrum_analysis</span> - Enable/disable spectrum analysis to find interference that would negatively impact wireless performance. <span class="li-normal">type: str</span> <span class="li-normal">choices: enable, disable</span></li>
            <li> <span class="li-head">vap_all</span> - Enable/disable the automatic inheritance of all Virtual Access Points (VAPs) . <span class="li-normal">type: str</span> <span class="li-normal">choices: enable, disable</span></li>
            <li> <span class="li-head">vaps</span> - Manually selected list of Virtual Access Points (VAPs). <span class="li-normal">type: list</span></li>
                <ul class="ul-self">
                <li> <span class="li-head">name</span> - Virtual Access Point (VAP) name. Source wireless-controller.vap-group.name wireless-controller.vap.name. <span class="li-normal">type: str</span> <span class="li-required">required: True</span></li>
                </ul>
            </ul>
        <li> <span class="li-head">radio_2</span> - Configuration options for radio 2. <span class="li-normal">type: dict</span></li>
            <ul class="ul-self">
            <li> <span class="li-head">auto_power_high</span> - Automatic transmission power high limit in decibels (dB) of the measured power referenced to one milliwatt (mW), or dBm (10 - 17 dBm). <span class="li-normal">type: int</span></li>
            <li> <span class="li-head">auto_power_level</span> - Enable/disable automatic power-level adjustment to prevent co-channel interference . <span class="li-normal">type: str</span> <span class="li-normal">choices: enable, disable</span></li>
            <li> <span class="li-head">auto_power_low</span> - Automatic transmission power low limit in dBm (the actual range of transmit power depends on the AP platform type). <span class="li-normal">type: int</span></li>
            <li> <span class="li-head">band</span> - WiFi band that Radio 1 operates on. <span class="li-normal">type: str</span> <span class="li-normal">choices: 802.11a, 802.11b, 802.11g, 802.11n, 802.11n-5G, 802.11n,g-only, 802.11g-only, 802.11n-only, 802.11n-5G-only, 802.11ac, 802.11ac,n-only, 802.11ac-only</span></li>
            <li> <span class="li-head">channel</span> - Selected list of wireless radio channels. <span class="li-normal">type: list</span></li>
                <ul class="ul-self">
                <li> <span class="li-head">chan</span> - Channel number. <span class="li-normal">type: str</span> <span class="li-required">required: True</span></li>
                </ul>
            <li> <span class="li-head">override_analysis</span> - Enable to override the WTP profile spectrum analysis configuration. <span class="li-normal">type: str</span> <span class="li-normal">choices: enable, disable</span></li>
            <li> <span class="li-head">override_band</span> - Enable to override the WTP profile band setting. <span class="li-normal">type: str</span> <span class="li-normal">choices: enable, disable</span></li>
            <li> <span class="li-head">override_channel</span> - Enable to override WTP profile channel settings. <span class="li-normal">type: str</span> <span class="li-normal">choices: enable, disable</span></li>
            <li> <span class="li-head">override_txpower</span> - Enable to override the WTP profile power level configuration. <span class="li-normal">type: str</span> <span class="li-normal">choices: enable, disable</span></li>
            <li> <span class="li-head">override_vaps</span> - Enable to override WTP profile Virtual Access Point (VAP) settings. <span class="li-normal">type: str</span> <span class="li-normal">choices: enable, disable</span></li>
            <li> <span class="li-head">power_level</span> - Radio power level as a percentage of the maximum transmit power (0 - 100). <span class="li-normal">type: int</span></li>
            <li> <span class="li-head">radio_id</span> - radio-id <span class="li-normal">type: int</span></li>
            <li> <span class="li-head">spectrum_analysis</span> - Enable/disable spectrum analysis to find interference that would negatively impact wireless performance. <span class="li-normal">type: str</span> <span class="li-normal">choices: enable, disable</span></li>
            <li> <span class="li-head">vap_all</span> - Enable/disable the automatic inheritance of all Virtual Access Points (VAPs) . <span class="li-normal">type: str</span> <span class="li-normal">choices: enable, disable</span></li>
            <li> <span class="li-head">vaps</span> - Manually selected list of Virtual Access Points (VAPs). <span class="li-normal">type: list</span></li>
                <ul class="ul-self">
                <li> <span class="li-head">name</span> - Virtual Access Point (VAP) name. Source wireless-controller.vap-group.name wireless-controller.vap.name. <span class="li-normal">type: str</span> <span class="li-required">required: True</span></li>
                </ul>
            </ul>
        <li> <span class="li-head">split_tunneling_acl</span> - Split tunneling ACL filter list. <span class="li-normal">type: list</span></li>
            <ul class="ul-self">
            <li> <span class="li-head">dest_ip</span> - Destination IP and mask for the split-tunneling subnet. <span class="li-normal">type: str</span></li>
            <li> <span class="li-head">id</span> - ID. <span class="li-normal">type: int</span> <span class="li-required">required: True</span></li>
            </ul>
        <li> <span class="li-head">split_tunneling_acl_local_ap_subnet</span> - Enable/disable automatically adding local subnetwork of FortiAP to split-tunneling ACL . <span class="li-normal">type: str</span> <span class="li-normal">choices: enable, disable</span></li>
        <li> <span class="li-head">split_tunneling_acl_path</span> - Split tunneling ACL path is local/tunnel. <span class="li-normal">type: str</span> <span class="li-normal">choices: tunnel, local</span></li>
        <li> <span class="li-head">tun_mtu_downlink</span> - Downlink tunnel MTU in octets. Set the value to either 0 (by default), 576, or 1500. <span class="li-normal">type: int</span></li>
        <li> <span class="li-head">tun_mtu_uplink</span> - Uplink tunnel maximum transmission unit (MTU) in octets (eight-bit bytes). Set the value to either 0 (by default), 576, or 1500. <span class="li-normal">type: int</span></li>
        <li> <span class="li-head">wan_port_mode</span> - Enable/disable using the FortiAP WAN port as a LAN port. <span class="li-normal">type: str</span> <span class="li-normal">choices: wan-lan, wan-only</span></li>
        <li> <span class="li-head">wtp_id</span> - WTP ID. <span class="li-normal">type: str</span></li>
        <li> <span class="li-head">wtp_mode</span> - WTP, AP, or FortiAP operating mode; normal (by default) or remote. A tunnel mode SSID can be assigned to an AP in normal mode but not remote mode, while a local-bridge mode SSID can be assigned to an AP in either normal mode or remote mode. <span class="li-normal">type: str</span> <span class="li-normal">choices: normal, remote</span></li>
        <li> <span class="li-head">wtp_profile</span> - WTP profile name to apply to this WTP, AP or FortiAP. Source wireless-controller.wtp-profile.name. <span class="li-normal">type: str</span></li>
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
      - name: Configure Wireless Termination Points (WTPs), that is, FortiAPs or APs to be managed by FortiGate.
        fortios_wireless_controller_wtp:
          vdom:  "{{ vdom }}"
          state: "present"
          wireless_controller_wtp:
            admin: "discovered"
            allowaccess: "telnet"
            bonjour_profile: "<your_own_value> (source wireless-controller.bonjour-profile.name)"
            coordinate_enable: "enable"
            coordinate_latitude: "<your_own_value>"
            coordinate_longitude: "<your_own_value>"
            coordinate_x: "<your_own_value>"
            coordinate_y: "<your_own_value>"
            image_download: "enable"
            index: "12"
            ip_fragment_preventing: "tcp-mss-adjust"
            lan:
                port_mode: "offline"
                port_ssid: "<your_own_value> (source wireless-controller.vap.name)"
                port1_mode: "offline"
                port1_ssid: "<your_own_value> (source wireless-controller.vap.name)"
                port2_mode: "offline"
                port2_ssid: "<your_own_value> (source wireless-controller.vap.name)"
                port3_mode: "offline"
                port3_ssid: "<your_own_value> (source wireless-controller.vap.name)"
                port4_mode: "offline"
                port4_ssid: "<your_own_value> (source wireless-controller.vap.name)"
                port5_mode: "offline"
                port5_ssid: "<your_own_value> (source wireless-controller.vap.name)"
                port6_mode: "offline"
                port6_ssid: "<your_own_value> (source wireless-controller.vap.name)"
                port7_mode: "offline"
                port7_ssid: "<your_own_value> (source wireless-controller.vap.name)"
                port8_mode: "offline"
                port8_ssid: "<your_own_value> (source wireless-controller.vap.name)"
            led_state: "enable"
            location: "<your_own_value>"
            login_passwd: "<your_own_value>"
            login_passwd_change: "yes"
            mesh_bridge_enable: "default"
            name: "default_name_38"
            override_allowaccess: "enable"
            override_ip_fragment: "enable"
            override_lan: "enable"
            override_led_state: "enable"
            override_login_passwd_change: "enable"
            override_split_tunnel: "enable"
            override_wan_port_mode: "enable"
            radio_1:
                auto_power_high: "47"
                auto_power_level: "enable"
                auto_power_low: "49"
                band: "802.11a"
                channel:
                 -
                    chan: "<your_own_value>"
                override_analysis: "enable"
                override_band: "enable"
                override_channel: "enable"
                override_txpower: "enable"
                override_vaps: "enable"
                power_level: "58"
                radio_id: "59"
                spectrum_analysis: "enable"
                vap_all: "enable"
                vaps:
                 -
                    name: "default_name_63 (source wireless-controller.vap-group.name wireless-controller.vap.name)"
            radio_2:
                auto_power_high: "65"
                auto_power_level: "enable"
                auto_power_low: "67"
                band: "802.11a"
                channel:
                 -
                    chan: "<your_own_value>"
                override_analysis: "enable"
                override_band: "enable"
                override_channel: "enable"
                override_txpower: "enable"
                override_vaps: "enable"
                power_level: "76"
                radio_id: "77"
                spectrum_analysis: "enable"
                vap_all: "enable"
                vaps:
                 -
                    name: "default_name_81 (source wireless-controller.vap-group.name wireless-controller.vap.name)"
            split_tunneling_acl:
             -
                dest_ip: "<your_own_value>"
                id:  "84"
            split_tunneling_acl_local_ap_subnet: "enable"
            split_tunneling_acl_path: "tunnel"
            tun_mtu_downlink: "87"
            tun_mtu_uplink: "88"
            wan_port_mode: "wan-lan"
            wtp_id: "<your_own_value>"
            wtp_mode: "normal"
            wtp_profile: "<your_own_value> (source wireless-controller.wtp-profile.name)"


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
