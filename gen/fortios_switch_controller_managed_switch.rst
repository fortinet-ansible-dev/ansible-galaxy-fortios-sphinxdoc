:source: fortios_switch_controller_managed_switch.py

:orphan:

.. fortios_switch_controller_managed_switch:

fortios_switch_controller_managed_switch -- Configure FortiSwitch devices that are managed by this FortiGate in Fortinet's FortiOS and FortiGate.
+++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++

.. versionadded:: 2.8

.. contents::
   :local:
   :depth: 1


Synopsis
--------
- This module is able to configure a FortiGate or FortiOS (FOS) device by allowing the user to set and modify switch_controller feature and managed_switch category. Examples include all parameters and values need to be adjusted to datasources before usage. Tested with FOS v6.4.0



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
    <li> <span class="li-head">switch_controller_managed_switch</span> - Configure FortiSwitch devices that are managed by this FortiGate. <span class="li-normal">type: dict</span></li>
        <ul class="ul-self">
        <li> <span class="li-head">state</span> - B(Deprecated) <span class="li-normal">type: str</span> <span class="li-required">required: False</span> <span class="li-normal">choices: present, absent</span></li>
        <li> <span class="li-head">settings_802_1X</span> - Configuration method to edit FortiSwitch 802.1X global settings. <span class="li-normal">type: dict</span></li>
            <ul class="ul-self">
            <li> <span class="li-head">link_down_auth</span> - Authentication state to set if a link is down. <span class="li-normal">type: str</span> <span class="li-normal">choices: set-unauth, no-action</span></li>
            <li> <span class="li-head">local_override</span> - Enable to override global 802.1X settings on individual FortiSwitches. <span class="li-normal">type: str</span> <span class="li-normal">choices: enable, disable</span></li>
            <li> <span class="li-head">max_reauth_attempt</span> - Maximum number of authentication attempts (0 - 15). <span class="li-normal">type: int</span></li>
            <li> <span class="li-head">reauth_period</span> - Reauthentication time interval (1 - 1440 min). <span class="li-normal">type: int</span></li>
            <li> <span class="li-head">tx_period</span> - 802.1X Tx period (seconds). <span class="li-normal">type: int</span></li>
            </ul>
        <li> <span class="li-head">access_profile</span> - FortiSwitch access profile. Source switch-controller.security-policy.local-access.name. <span class="li-normal">type: str</span></li>
        <li> <span class="li-head">custom_command</span> - Configuration method to edit FortiSwitch commands to be pushed to this FortiSwitch device upon rebooting the FortiGate switch controller or the FortiSwitch. <span class="li-normal">type: list</span></li>
            <ul class="ul-self">
            <li> <span class="li-head">command_entry</span> - List of FortiSwitch commands. <span class="li-normal">type: str</span></li>
            <li> <span class="li-head">command_name</span> - Names of commands to be pushed to this FortiSwitch device, as configured under config switch-controller custom-command. Source switch-controller.custom-command.command-name. <span class="li-normal">type: str</span></li>
            </ul>
        <li> <span class="li-head">delayed_restart_trigger</span> - Delayed restart triggered for this FortiSwitch. <span class="li-normal">type: int</span></li>
        <li> <span class="li-head">description</span> - Description. <span class="li-normal">type: str</span></li>
        <li> <span class="li-head">directly_connected</span> - Directly connected FortiSwitch. <span class="li-normal">type: int</span></li>
        <li> <span class="li-head">dynamic_capability</span> - List of features this FortiSwitch supports (not configurable) that is sent to the FortiGate device for subsequent configuration initiated by the FortiGate device. <span class="li-normal">type: int</span></li>
        <li> <span class="li-head">dynamically_discovered</span> - Dynamically discovered FortiSwitch. <span class="li-normal">type: int</span></li>
        <li> <span class="li-head">flow_identity</span> - Flow-tracking netflow ipfix switch identity in hex format(00000000-FFFFFFFF ). <span class="li-normal">type: str</span></li>
        <li> <span class="li-head">fsw_wan1_admin</span> - FortiSwitch WAN1 admin status; enable to authorize the FortiSwitch as a managed switch. <span class="li-normal">type: str</span> <span class="li-normal">choices: discovered, disable, enable</span></li>
        <li> <span class="li-head">fsw_wan1_peer</span> - Fortiswitch WAN1 peer port. <span class="li-normal">type: str</span></li>
        <li> <span class="li-head">igmp_snooping</span> - Configure FortiSwitch IGMP snooping global settings. <span class="li-normal">type: dict</span></li>
            <ul class="ul-self">
            <li> <span class="li-head">aging_time</span> - Maximum time to retain a multicast snooping entry for which no packets have been seen (15 - 3600 sec). <span class="li-normal">type: int</span></li>
            <li> <span class="li-head">flood_unknown_multicast</span> - Enable/disable unknown multicast flooding. <span class="li-normal">type: str</span> <span class="li-normal">choices: enable, disable</span></li>
            <li> <span class="li-head">local_override</span> - Enable/disable overriding the global IGMP snooping configuration. <span class="li-normal">type: str</span> <span class="li-normal">choices: enable, disable</span></li>
            </ul>
        <li> <span class="li-head">ip_source_guard</span> - IP source guard. <span class="li-normal">type: list</span></li>
            <ul class="ul-self">
            <li> <span class="li-head">binding_entry</span> - IP and MAC address configuration. <span class="li-normal">type: list</span></li>
                <ul class="ul-self">
                <li> <span class="li-head">entry_name</span> - Configure binding pair. <span class="li-normal">type: str</span></li>
                <li> <span class="li-head">ip</span> - Source IP for this rule. <span class="li-normal">type: str</span></li>
                <li> <span class="li-head">mac</span> - MAC address for this rule. <span class="li-normal">type: str</span></li>
                </ul>
            <li> <span class="li-head">description</span> - Description. <span class="li-normal">type: str</span></li>
            <li> <span class="li-head">port</span> - Ingress interface to which source guard is bound. <span class="li-normal">type: str</span> <span class="li-required">required: True</span></li>
            </ul>
        <li> <span class="li-head">l3_discovered</span> - Layer 3 management discovered. <span class="li-normal">type: int</span></li>
        <li> <span class="li-head">mclag_igmp_snooping_aware</span> - Enable/disable MCLAG IGMP-snooping awareness. <span class="li-normal">type: str</span> <span class="li-normal">choices: enable, disable</span></li>
        <li> <span class="li-head">mirror</span> - Configuration method to edit FortiSwitch packet mirror. <span class="li-normal">type: list</span></li>
            <ul class="ul-self">
            <li> <span class="li-head">dst</span> - Destination port. <span class="li-normal">type: str</span></li>
            <li> <span class="li-head">name</span> - Mirror name. <span class="li-normal">type: str</span> <span class="li-required">required: True</span></li>
            <li> <span class="li-head">src_egress</span> - Source egress interfaces. <span class="li-normal">type: list</span></li>
                <ul class="ul-self">
                <li> <span class="li-head">name</span> - Interface name. <span class="li-normal">type: str</span> <span class="li-required">required: True</span></li>
                </ul>
            <li> <span class="li-head">src_ingress</span> - Source ingress interfaces. <span class="li-normal">type: list</span></li>
                <ul class="ul-self">
                <li> <span class="li-head">name</span> - Interface name. <span class="li-normal">type: str</span> <span class="li-required">required: True</span></li>
                </ul>
            <li> <span class="li-head">status</span> - Active/inactive mirror configuration. <span class="li-normal">type: str</span> <span class="li-normal">choices: active, inactive</span></li>
            <li> <span class="li-head">switching_packet</span> - Enable/disable switching functionality when mirroring. <span class="li-normal">type: str</span> <span class="li-normal">choices: enable, disable</span></li>
            </ul>
        <li> <span class="li-head">name</span> - Managed-switch name. <span class="li-normal">type: str</span></li>
        <li> <span class="li-head">override_snmp_community</span> - Enable/disable overriding the global SNMP communities. <span class="li-normal">type: str</span> <span class="li-normal">choices: enable, disable</span></li>
        <li> <span class="li-head">override_snmp_sysinfo</span> - Enable/disable overriding the global SNMP system information. <span class="li-normal">type: str</span> <span class="li-normal">choices: disable, enable</span></li>
        <li> <span class="li-head">override_snmp_trap_threshold</span> - Enable/disable overriding the global SNMP trap threshold values. <span class="li-normal">type: str</span> <span class="li-normal">choices: enable, disable</span></li>
        <li> <span class="li-head">override_snmp_user</span> - Enable/disable overriding the global SNMP users. <span class="li-normal">type: str</span> <span class="li-normal">choices: enable, disable</span></li>
        <li> <span class="li-head">owner_vdom</span> - VDOM which owner of port belongs to. <span class="li-normal">type: str</span></li>
        <li> <span class="li-head">poe_detection_type</span> - PoE detection type for FortiSwitch. <span class="li-normal">type: int</span></li>
        <li> <span class="li-head">poe_pre_standard_detection</span> - Enable/disable PoE pre-standard detection. <span class="li-normal">type: str</span> <span class="li-normal">choices: enable, disable</span></li>
        <li> <span class="li-head">ports</span> - Managed-switch port list. <span class="li-normal">type: list</span></li>
            <ul class="ul-self">
            <li> <span class="li-head">access_mode</span> - Access mode of the port. <span class="li-normal">type: str</span> <span class="li-normal">choices: normal, nac</span></li>
            <li> <span class="li-head">allowed_vlans</span> - Configure switch port tagged vlans <span class="li-normal">type: list</span></li>
                <ul class="ul-self">
                <li> <span class="li-head">vlan_name</span> - VLAN name. Source system.interface.name. <span class="li-normal">type: str</span></li>
                </ul>
            <li> <span class="li-head">allowed_vlans_all</span> - Enable/disable all defined vlans on this port. <span class="li-normal">type: str</span> <span class="li-normal">choices: enable, disable</span></li>
            <li> <span class="li-head">arp_inspection_trust</span> - Trusted or untrusted dynamic ARP inspection. <span class="li-normal">type: str</span> <span class="li-normal">choices: untrusted, trusted</span></li>
            <li> <span class="li-head">bundle</span> - Enable/disable Link Aggregation Group (LAG) bundling for non-FortiLink interfaces. <span class="li-normal">type: str</span> <span class="li-normal">choices: enable, disable</span></li>
            <li> <span class="li-head">description</span> - Description for port. <span class="li-normal">type: str</span></li>
            <li> <span class="li-head">dhcp_snoop_option82_trust</span> - Enable/disable allowance of DHCP with option-82 on untrusted interface. <span class="li-normal">type: str</span> <span class="li-normal">choices: enable, disable</span></li>
            <li> <span class="li-head">dhcp_snooping</span> - Trusted or untrusted DHCP-snooping interface. <span class="li-normal">type: str</span> <span class="li-normal">choices: untrusted, trusted</span></li>
            <li> <span class="li-head">discard_mode</span> - Configure discard mode for port. <span class="li-normal">type: str</span> <span class="li-normal">choices: none, all-untagged, all-tagged</span></li>
            <li> <span class="li-head">edge_port</span> - Enable/disable this interface as an edge port, bridging connections between workstations and/or computers. <span class="li-normal">type: str</span> <span class="li-normal">choices: enable, disable</span></li>
            <li> <span class="li-head">export_tags</span> - Configure export tag(s) for FortiSwitch port when exported to a virtual port pool. <span class="li-normal">type: list</span></li>
                <ul class="ul-self">
                <li> <span class="li-head">tag_name</span> - FortiSwitch port tag name when exported to a virtual port pool. Source switch-controller.switch-interface-tag.name. <span class="li-normal">type: str</span></li>
                </ul>
            <li> <span class="li-head">export_to</span> - Export managed-switch port to a tenant VDOM. Source system.vdom.name. <span class="li-normal">type: str</span></li>
            <li> <span class="li-head">export_to_pool</span> - Switch controller export port to pool-list. Source switch-controller.virtual-port-pool.name. <span class="li-normal">type: str</span></li>
            <li> <span class="li-head">fgt_peer_device_name</span> - FGT peer device name. <span class="li-normal">type: str</span></li>
            <li> <span class="li-head">fgt_peer_port_name</span> - FGT peer port name. <span class="li-normal">type: str</span></li>
            <li> <span class="li-head">fiber_port</span> - Fiber-port. <span class="li-normal">type: int</span></li>
            <li> <span class="li-head">flags</span> - Port properties flags. <span class="li-normal">type: int</span></li>
            <li> <span class="li-head">fortilink_port</span> - FortiLink uplink port. <span class="li-normal">type: int</span></li>
            <li> <span class="li-head">igmps_flood_reports</span> - Enable/disable flooding of IGMP reports to this interface when igmp-snooping enabled. <span class="li-normal">type: str</span> <span class="li-normal">choices: enable, disable</span></li>
            <li> <span class="li-head">igmps_flood_traffic</span> - Enable/disable flooding of IGMP snooping traffic to this interface. <span class="li-normal">type: str</span> <span class="li-normal">choices: enable, disable</span></li>
            <li> <span class="li-head">ip_source_guard</span> - Enable/disable IP source guard. <span class="li-normal">type: str</span> <span class="li-normal">choices: disable, enable</span></li>
            <li> <span class="li-head">isl_local_trunk_name</span> - ISL local trunk name. <span class="li-normal">type: str</span></li>
            <li> <span class="li-head">isl_peer_device_name</span> - ISL peer device name. <span class="li-normal">type: str</span></li>
            <li> <span class="li-head">isl_peer_port_name</span> - ISL peer port name. <span class="li-normal">type: str</span></li>
            <li> <span class="li-head">lacp_speed</span> - end Link Aggregation Control Protocol (LACP) messages every 30 seconds (slow) or every second (fast). <span class="li-normal">type: str</span> <span class="li-normal">choices: slow, fast</span></li>
            <li> <span class="li-head">learning_limit</span> - Limit the number of dynamic MAC addresses on this Port (1 - 128, 0 = no limit, default). <span class="li-normal">type: int</span></li>
            <li> <span class="li-head">lldp_profile</span> - LLDP port TLV profile. Source switch-controller.lldp-profile.name. <span class="li-normal">type: str</span></li>
            <li> <span class="li-head">lldp_status</span> - LLDP transmit and receive status. <span class="li-normal">type: str</span> <span class="li-normal">choices: disable, rx-only, tx-only, tx-rx</span></li>
            <li> <span class="li-head">loop_guard</span> - Enable/disable loop-guard on this interface, an STP optimization used to prevent network loops. <span class="li-normal">type: str</span> <span class="li-normal">choices: enabled, disabled</span></li>
            <li> <span class="li-head">loop_guard_timeout</span> - Loop-guard timeout (0 - 120 min). <span class="li-normal">type: int</span></li>
            <li> <span class="li-head">mac_addr</span> - Port/Trunk MAC. <span class="li-normal">type: str</span></li>
            <li> <span class="li-head">max_bundle</span> - Maximum size of LAG bundle (1 - 24) <span class="li-normal">type: int</span></li>
            <li> <span class="li-head">mclag</span> - Enable/disable multi-chassis link aggregation (MCLAG). <span class="li-normal">type: str</span> <span class="li-normal">choices: enable, disable</span></li>
            <li> <span class="li-head">mclag_icl_port</span> - MCLAG-ICL port. <span class="li-normal">type: int</span></li>
            <li> <span class="li-head">member_withdrawal_behavior</span> - Port behavior after it withdraws because of loss of control packets. <span class="li-normal">type: str</span> <span class="li-normal">choices: forward, block</span></li>
            <li> <span class="li-head">members</span> - Aggregated LAG bundle interfaces. <span class="li-normal">type: list</span></li>
                <ul class="ul-self">
                <li> <span class="li-head">member_name</span> - Interface name from available options. <span class="li-normal">type: str</span></li>
                </ul>
            <li> <span class="li-head">min_bundle</span> - Minimum size of LAG bundle (1 - 24) <span class="li-normal">type: int</span></li>
            <li> <span class="li-head">mode</span> - LACP mode: ignore and do not send control messages, or negotiate 802.3ad aggregation passively or actively. <span class="li-normal">type: str</span> <span class="li-normal">choices: static, lacp-passive, lacp-active</span></li>
            <li> <span class="li-head">p2p_port</span> - General peer to peer tunnel port. <span class="li-normal">type: int</span></li>
            <li> <span class="li-head">packet_sample_rate</span> - Packet sampling rate (0 - 99999 p/sec). <span class="li-normal">type: int</span></li>
            <li> <span class="li-head">packet_sampler</span> - Enable/disable packet sampling on this interface. <span class="li-normal">type: str</span> <span class="li-normal">choices: enabled, disabled</span></li>
            <li> <span class="li-head">poe_capable</span> - PoE capable. <span class="li-normal">type: int</span></li>
            <li> <span class="li-head">poe_pre_standard_detection</span> - Enable/disable PoE pre-standard detection. <span class="li-normal">type: str</span> <span class="li-normal">choices: enable, disable</span></li>
            <li> <span class="li-head">poe_status</span> - Enable/disable PoE status. <span class="li-normal">type: str</span> <span class="li-normal">choices: enable, disable</span></li>
            <li> <span class="li-head">port_name</span> - Switch port name. <span class="li-normal">type: str</span></li>
            <li> <span class="li-head">port_number</span> - Port number. <span class="li-normal">type: int</span></li>
            <li> <span class="li-head">port_owner</span> - Switch port name. <span class="li-normal">type: str</span></li>
            <li> <span class="li-head">port_prefix_type</span> - Port prefix type. <span class="li-normal">type: int</span></li>
            <li> <span class="li-head">port_security_policy</span> - Switch controller authentication policy to apply to this managed switch from available options. Source switch-controller .security-policy.802-1X.name switch-controller.security-policy.captive-portal.name. <span class="li-normal">type: str</span></li>
            <li> <span class="li-head">port_selection_criteria</span> - Algorithm for aggregate port selection. <span class="li-normal">type: str</span> <span class="li-normal">choices: src-mac, dst-mac, src-dst-mac, src-ip, dst-ip, src-dst-ip</span></li>
            <li> <span class="li-head">qos_policy</span> - Switch controller QoS policy from available options. Source switch-controller.qos.qos-policy.name. <span class="li-normal">type: str</span></li>
            <li> <span class="li-head">sample_direction</span> - Packet sampling direction. <span class="li-normal">type: str</span> <span class="li-normal">choices: tx, rx, both</span></li>
            <li> <span class="li-head">sflow_counter_interval</span> - sFlow sampling counter polling interval (0 - 255 sec). <span class="li-normal">type: int</span></li>
            <li> <span class="li-head">speed</span> - Switch port speed; default and available settings depend on hardware. <span class="li-normal">type: str</span> <span class="li-normal">choices: 10half, 10full, 100half, 100full, 1000auto, 1000fiber, 1000full, 10000, 40000, auto, auto-module, 100FX-half, 100FX-full, 100000full, 2500auto, 25000full, 50000full, 10000cr, 10000sr, 100000sr4, 100000cr4, 25000cr4, 25000sr4, 5000full</span></li>
            <li> <span class="li-head">stacking_port</span> - Stacking port. <span class="li-normal">type: int</span></li>
            <li> <span class="li-head">status</span> - Switch port admin status: up or down. <span class="li-normal">type: str</span> <span class="li-normal">choices: up, down</span></li>
            <li> <span class="li-head">sticky_mac</span> - Enable or disable sticky-mac on the interface. <span class="li-normal">type: str</span> <span class="li-normal">choices: enable, disable</span></li>
            <li> <span class="li-head">storm_control_policy</span> - Switch controller storm control policy from available options. Source switch-controller.storm-control-policy.name. <span class="li-normal">type: str</span></li>
            <li> <span class="li-head">stp_bpdu_guard</span> - Enable/disable STP BPDU guard on this interface. <span class="li-normal">type: str</span> <span class="li-normal">choices: enabled, disabled</span></li>
            <li> <span class="li-head">stp_bpdu_guard_timeout</span> - BPDU Guard disabling protection (0 - 120 min). <span class="li-normal">type: int</span></li>
            <li> <span class="li-head">stp_root_guard</span> - Enable/disable STP root guard on this interface. <span class="li-normal">type: str</span> <span class="li-normal">choices: enabled, disabled</span></li>
            <li> <span class="li-head">stp_state</span> - Enable/disable Spanning Tree Protocol (STP) on this interface. <span class="li-normal">type: str</span> <span class="li-normal">choices: enabled, disabled</span></li>
            <li> <span class="li-head">switch_id</span> - Switch id. <span class="li-normal">type: str</span></li>
            <li> <span class="li-head">type</span> - Interface type: physical or trunk port. <span class="li-normal">type: str</span> <span class="li-normal">choices: physical, trunk</span></li>
            <li> <span class="li-head">untagged_vlans</span> - Configure switch port untagged vlans <span class="li-normal">type: list</span></li>
                <ul class="ul-self">
                <li> <span class="li-head">vlan_name</span> - VLAN name. Source system.interface.name. <span class="li-normal">type: str</span></li>
                </ul>
            <li> <span class="li-head">vlan</span> - Assign switch ports to a VLAN. Source system.interface.name. <span class="li-normal">type: str</span></li>
            </ul>
        <li> <span class="li-head">pre_provisioned</span> - Pre-provisioned managed switch. <span class="li-normal">type: int</span></li>
        <li> <span class="li-head">qos_drop_policy</span> - Set QoS drop-policy. <span class="li-normal">type: str</span> <span class="li-normal">choices: taildrop, random-early-detection</span></li>
        <li> <span class="li-head">qos_red_probability</span> - Set QoS RED/WRED drop probability. <span class="li-normal">type: int</span></li>
        <li> <span class="li-head">remote_log</span> - Configure logging by FortiSwitch device to a remote syslog server. <span class="li-normal">type: list</span></li>
            <ul class="ul-self">
            <li> <span class="li-head">csv</span> - Enable/disable comma-separated value (CSV) strings. <span class="li-normal">type: str</span> <span class="li-normal">choices: enable, disable</span></li>
            <li> <span class="li-head">facility</span> - Facility to log to remote syslog server. <span class="li-normal">type: str</span> <span class="li-normal">choices: kernel, user, mail, daemon, auth, syslog, lpr, news, uucp, cron, authpriv, ftp, ntp, audit, alert, clock, local0, local1, local2, local3, local4, local5, local6, local7</span></li>
            <li> <span class="li-head">name</span> - Remote log name. <span class="li-normal">type: str</span> <span class="li-required">required: True</span></li>
            <li> <span class="li-head">port</span> - Remote syslog server listening port. <span class="li-normal">type: int</span></li>
            <li> <span class="li-head">server</span> - IPv4 address of the remote syslog server. <span class="li-normal">type: str</span></li>
            <li> <span class="li-head">severity</span> - Severity of logs to be transferred to remote log server. <span class="li-normal">type: str</span> <span class="li-normal">choices: emergency, alert, critical, error, warning, notification, information, debug</span></li>
            <li> <span class="li-head">status</span> - Enable/disable logging by FortiSwitch device to a remote syslog server. <span class="li-normal">type: str</span> <span class="li-normal">choices: enable, disable</span></li>
            </ul>
        <li> <span class="li-head">snmp_community</span> - Configuration method to edit Simple Network Management Protocol (SNMP) communities. <span class="li-normal">type: list</span></li>
            <ul class="ul-self">
            <li> <span class="li-head">events</span> - SNMP notifications (traps) to send. <span class="li-normal">type: str</span> <span class="li-normal">choices: cpu-high, mem-low, log-full, intf-ip, ent-conf-change</span></li>
            <li> <span class="li-head">hosts</span> - Configure IPv4 SNMP managers (hosts). <span class="li-normal">type: list</span></li>
                <ul class="ul-self">
                <li> <span class="li-head">id</span> - Host entry ID. <span class="li-normal">type: int</span> <span class="li-required">required: True</span></li>
                <li> <span class="li-head">ip</span> - IPv4 address of the SNMP manager (host). <span class="li-normal">type: str</span></li>
                </ul>
            <li> <span class="li-head">id</span> - SNMP community ID. <span class="li-normal">type: int</span> <span class="li-required">required: True</span></li>
            <li> <span class="li-head">name</span> - SNMP community name. <span class="li-normal">type: str</span></li>
            <li> <span class="li-head">query_v1_port</span> - SNMP v1 query port . <span class="li-normal">type: int</span></li>
            <li> <span class="li-head">query_v1_status</span> - Enable/disable SNMP v1 queries. <span class="li-normal">type: str</span> <span class="li-normal">choices: disable, enable</span></li>
            <li> <span class="li-head">query_v2c_port</span> - SNMP v2c query port . <span class="li-normal">type: int</span></li>
            <li> <span class="li-head">query_v2c_status</span> - Enable/disable SNMP v2c queries. <span class="li-normal">type: str</span> <span class="li-normal">choices: disable, enable</span></li>
            <li> <span class="li-head">status</span> - Enable/disable this SNMP community. <span class="li-normal">type: str</span> <span class="li-normal">choices: disable, enable</span></li>
            <li> <span class="li-head">trap_v1_lport</span> - SNMP v2c trap local port . <span class="li-normal">type: int</span></li>
            <li> <span class="li-head">trap_v1_rport</span> - SNMP v2c trap remote port . <span class="li-normal">type: int</span></li>
            <li> <span class="li-head">trap_v1_status</span> - Enable/disable SNMP v1 traps. <span class="li-normal">type: str</span> <span class="li-normal">choices: disable, enable</span></li>
            <li> <span class="li-head">trap_v2c_lport</span> - SNMP v2c trap local port . <span class="li-normal">type: int</span></li>
            <li> <span class="li-head">trap_v2c_rport</span> - SNMP v2c trap remote port . <span class="li-normal">type: int</span></li>
            <li> <span class="li-head">trap_v2c_status</span> - Enable/disable SNMP v2c traps. <span class="li-normal">type: str</span> <span class="li-normal">choices: disable, enable</span></li>
            </ul>
        <li> <span class="li-head">snmp_sysinfo</span> - Configuration method to edit Simple Network Management Protocol (SNMP) system info. <span class="li-normal">type: dict</span></li>
            <ul class="ul-self">
            <li> <span class="li-head">contact_info</span> - Contact information. <span class="li-normal">type: str</span></li>
            <li> <span class="li-head">description</span> - System description. <span class="li-normal">type: str</span></li>
            <li> <span class="li-head">engine_id</span> - Local SNMP engine ID string (max 24 char). <span class="li-normal">type: str</span></li>
            <li> <span class="li-head">location</span> - System location. <span class="li-normal">type: str</span></li>
            <li> <span class="li-head">status</span> - Enable/disable SNMP. <span class="li-normal">type: str</span> <span class="li-normal">choices: disable, enable</span></li>
            </ul>
        <li> <span class="li-head">snmp_trap_threshold</span> - Configuration method to edit Simple Network Management Protocol (SNMP) trap threshold values. <span class="li-normal">type: dict</span></li>
            <ul class="ul-self">
            <li> <span class="li-head">trap_high_cpu_threshold</span> - CPU usage when trap is sent. <span class="li-normal">type: int</span></li>
            <li> <span class="li-head">trap_log_full_threshold</span> - Log disk usage when trap is sent. <span class="li-normal">type: int</span></li>
            <li> <span class="li-head">trap_low_memory_threshold</span> - Memory usage when trap is sent. <span class="li-normal">type: int</span></li>
            </ul>
        <li> <span class="li-head">snmp_user</span> - Configuration method to edit Simple Network Management Protocol (SNMP) users. <span class="li-normal">type: list</span></li>
            <ul class="ul-self">
            <li> <span class="li-head">auth_proto</span> - Authentication protocol. <span class="li-normal">type: str</span> <span class="li-normal">choices: md5, sha</span></li>
            <li> <span class="li-head">auth_pwd</span> - Password for authentication protocol. <span class="li-normal">type: str</span></li>
            <li> <span class="li-head">name</span> - SNMP user name. <span class="li-normal">type: str</span> <span class="li-required">required: True</span></li>
            <li> <span class="li-head">priv_proto</span> - Privacy (encryption) protocol. <span class="li-normal">type: str</span> <span class="li-normal">choices: aes, des</span></li>
            <li> <span class="li-head">priv_pwd</span> - Password for privacy (encryption) protocol. <span class="li-normal">type: str</span></li>
            <li> <span class="li-head">queries</span> - Enable/disable SNMP queries for this user. <span class="li-normal">type: str</span> <span class="li-normal">choices: disable, enable</span></li>
            <li> <span class="li-head">query_port</span> - SNMPv3 query port . <span class="li-normal">type: int</span></li>
            <li> <span class="li-head">security_level</span> - Security level for message authentication and encryption. <span class="li-normal">type: str</span> <span class="li-normal">choices: no-auth-no-priv, auth-no-priv, auth-priv</span></li>
            </ul>
        <li> <span class="li-head">staged_image_version</span> - Staged image version for FortiSwitch. <span class="li-normal">type: str</span></li>
        <li> <span class="li-head">static_mac</span> - Configuration method to edit FortiSwitch Static and Sticky MAC. <span class="li-normal">type: list</span></li>
            <ul class="ul-self">
            <li> <span class="li-head">description</span> - Description. <span class="li-normal">type: str</span></li>
            <li> <span class="li-head">id</span> - Id <span class="li-normal">type: int</span> <span class="li-required">required: True</span></li>
            <li> <span class="li-head">interface</span> - Interface name. <span class="li-normal">type: str</span></li>
            <li> <span class="li-head">mac</span> - MAC address. <span class="li-normal">type: str</span></li>
            <li> <span class="li-head">type</span> - Type. <span class="li-normal">type: str</span> <span class="li-normal">choices: static, sticky</span></li>
            <li> <span class="li-head">vlan</span> - Vlan. Source system.interface.name. <span class="li-normal">type: str</span></li>
            </ul>
        <li> <span class="li-head">storm_control</span> - Configuration method to edit FortiSwitch storm control for measuring traffic activity using data rates to prevent traffic disruption. <span class="li-normal">type: dict</span></li>
            <ul class="ul-self">
            <li> <span class="li-head">broadcast</span> - Enable/disable storm control to drop broadcast traffic. <span class="li-normal">type: str</span> <span class="li-normal">choices: enable, disable</span></li>
            <li> <span class="li-head">local_override</span> - Enable to override global FortiSwitch storm control settings for this FortiSwitch. <span class="li-normal">type: str</span> <span class="li-normal">choices: enable, disable</span></li>
            <li> <span class="li-head">rate</span> - Rate in packets per second at which storm traffic is controlled (1 - 10000000). Storm control drops excess traffic data rates beyond this threshold. <span class="li-normal">type: int</span></li>
            <li> <span class="li-head">unknown_multicast</span> - Enable/disable storm control to drop unknown multicast traffic. <span class="li-normal">type: str</span> <span class="li-normal">choices: enable, disable</span></li>
            <li> <span class="li-head">unknown_unicast</span> - Enable/disable storm control to drop unknown unicast traffic. <span class="li-normal">type: str</span> <span class="li-normal">choices: enable, disable</span></li>
            </ul>
        <li> <span class="li-head">stp_instance</span> - Configuration method to edit Spanning Tree Protocol (STP) instances. <span class="li-normal">type: list</span></li>
            <ul class="ul-self">
            <li> <span class="li-head">id</span> - Instance ID. <span class="li-normal">type: str</span> <span class="li-required">required: True</span></li>
            <li> <span class="li-head">priority</span> - Priority. <span class="li-normal">type: str</span> <span class="li-normal">choices: 0, 4096, 8192, 12288, 16384, 20480, 24576, 28672, 32768, 36864, 40960, 45056, 49152, 53248, 57344, 61440</span></li>
            </ul>
        <li> <span class="li-head">stp_settings</span> - Configuration method to edit Spanning Tree Protocol (STP) settings used to prevent bridge loops. <span class="li-normal">type: dict</span></li>
            <ul class="ul-self">
            <li> <span class="li-head">forward_time</span> - Period of time a port is in listening and learning state (4 - 30 sec). <span class="li-normal">type: int</span></li>
            <li> <span class="li-head">hello_time</span> - Period of time between successive STP frame Bridge Protocol Data Units (BPDUs) sent on a port (1 - 10 sec). <span class="li-normal">type: int</span></li>
            <li> <span class="li-head">local_override</span> - Enable to configure local STP settings that override global STP settings. <span class="li-normal">type: str</span> <span class="li-normal">choices: enable, disable</span></li>
            <li> <span class="li-head">max_age</span> - Maximum time before a bridge port saves its configuration BPDU information (6 - 40 sec). <span class="li-normal">type: int</span></li>
            <li> <span class="li-head">max_hops</span> - Maximum number of hops between the root bridge and the furthest bridge (1- 40). <span class="li-normal">type: int</span></li>
            <li> <span class="li-head">name</span> - Name of local STP settings configuration. <span class="li-normal">type: str</span></li>
            <li> <span class="li-head">pending_timer</span> - Pending time (1 - 15 sec). <span class="li-normal">type: int</span></li>
            <li> <span class="li-head">revision</span> - STP revision number (0 - 65535). <span class="li-normal">type: int</span></li>
            </ul>
        <li> <span class="li-head">switch_device_tag</span> - User definable label/tag. <span class="li-normal">type: str</span></li>
        <li> <span class="li-head">switch_dhcp_opt43_key</span> - DHCP option43 key. <span class="li-normal">type: str</span></li>
        <li> <span class="li-head">switch_id</span> - Managed-switch id. <span class="li-normal">type: str</span></li>
        <li> <span class="li-head">switch_log</span> - Configuration method to edit FortiSwitch logging settings (logs are transferred to and inserted into the FortiGate event log). <span class="li-normal">type: dict</span></li>
            <ul class="ul-self">
            <li> <span class="li-head">local_override</span> - Enable to configure local logging settings that override global logging settings. <span class="li-normal">type: str</span> <span class="li-normal">choices: enable, disable</span></li>
            <li> <span class="li-head">severity</span> - Severity of FortiSwitch logs that are added to the FortiGate event log. <span class="li-normal">type: str</span> <span class="li-normal">choices: emergency, alert, critical, error, warning, notification, information, debug</span></li>
            <li> <span class="li-head">status</span> - Enable/disable adding FortiSwitch logs to the FortiGate event log. <span class="li-normal">type: str</span> <span class="li-normal">choices: enable, disable</span></li>
            </ul>
        <li> <span class="li-head">switch_profile</span> - FortiSwitch profile. Source switch-controller.switch-profile.name. <span class="li-normal">type: str</span></li>
        <li> <span class="li-head">type</span> - Indication of switch type, physical or virtual. <span class="li-normal">type: str</span> <span class="li-normal">choices: virtual, physical</span></li>
        <li> <span class="li-head">version</span> - FortiSwitch version. <span class="li-normal">type: int</span></li>
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
      - name: Configure FortiSwitch devices that are managed by this FortiGate.
        fortios_switch_controller_managed_switch:
          vdom:  "{{ vdom }}"
          state: "present"
          access_token: "<your_own_value>"
          switch_controller_managed_switch:
            settings_802_1X:
                link_down_auth: "set-unauth"
                local_override: "enable"
                max_reauth_attempt: "6"
                reauth_period: "7"
                tx_period: "8"
            access_profile: "<your_own_value> (source switch-controller.security-policy.local-access.name)"
            custom_command:
             -
                command_entry: "<your_own_value>"
                command_name: "<your_own_value> (source switch-controller.custom-command.command-name)"
            delayed_restart_trigger: "13"
            description: "<your_own_value>"
            directly_connected: "15"
            dynamic_capability: "16"
            dynamically_discovered: "17"
            flow_identity: "<your_own_value>"
            fsw_wan1_admin: "discovered"
            fsw_wan1_peer: "<your_own_value>"
            igmp_snooping:
                aging_time: "22"
                flood_unknown_multicast: "enable"
                local_override: "enable"
            ip_source_guard:
             -
                binding_entry:
                 -
                    entry_name: "<your_own_value>"
                    ip: "<your_own_value>"
                    mac: "<your_own_value>"
                description: "<your_own_value>"
                port: "<your_own_value>"
            l3_discovered: "32"
            mclag_igmp_snooping_aware: "enable"
            mirror:
             -
                dst: "<your_own_value>"
                name: "default_name_36"
                src_egress:
                 -
                    name: "default_name_38"
                src_ingress:
                 -
                    name: "default_name_40"
                status: "active"
                switching_packet: "enable"
            name: "default_name_43"
            override_snmp_community: "enable"
            override_snmp_sysinfo: "disable"
            override_snmp_trap_threshold: "enable"
            override_snmp_user: "enable"
            owner_vdom: "<your_own_value>"
            poe_detection_type: "49"
            poe_pre_standard_detection: "enable"
            ports:
             -
                access_mode: "normal"
                allowed_vlans:
                 -
                    vlan_name: "<your_own_value> (source system.interface.name)"
                allowed_vlans_all: "enable"
                arp_inspection_trust: "untrusted"
                bundle: "enable"
                description: "<your_own_value>"
                dhcp_snoop_option82_trust: "enable"
                dhcp_snooping: "untrusted"
                discard_mode: "none"
                edge_port: "enable"
                export_tags:
                 -
                    tag_name: "<your_own_value> (source switch-controller.switch-interface-tag.name)"
                export_to: "<your_own_value> (source system.vdom.name)"
                export_to_pool: "<your_own_value> (source switch-controller.virtual-port-pool.name)"
                fgt_peer_device_name: "<your_own_value>"
                fgt_peer_port_name: "<your_own_value>"
                fiber_port: "69"
                flags: "70"
                fortilink_port: "71"
                igmps_flood_reports: "enable"
                igmps_flood_traffic: "enable"
                ip_source_guard: "disable"
                isl_local_trunk_name: "<your_own_value>"
                isl_peer_device_name: "<your_own_value>"
                isl_peer_port_name: "<your_own_value>"
                lacp_speed: "slow"
                learning_limit: "79"
                lldp_profile: "<your_own_value> (source switch-controller.lldp-profile.name)"
                lldp_status: "disable"
                loop_guard: "enabled"
                loop_guard_timeout: "83"
                mac_addr: "<your_own_value>"
                max_bundle: "85"
                mclag: "enable"
                mclag_icl_port: "87"
                member_withdrawal_behavior: "forward"
                members:
                 -
                    member_name: "<your_own_value>"
                min_bundle: "91"
                mode: "static"
                p2p_port: "93"
                packet_sample_rate: "94"
                packet_sampler: "enabled"
                poe_capable: "96"
                poe_pre_standard_detection: "enable"
                poe_status: "enable"
                port_name: "<your_own_value>"
                port_number: "100"
                port_owner: "<your_own_value>"
                port_prefix_type: "102"
                port_security_policy: "<your_own_value> (source switch-controller.security-policy.802-1X.name switch-controller.security-policy.captive-portal
                  .name)"
                port_selection_criteria: "src-mac"
                qos_policy: "<your_own_value> (source switch-controller.qos.qos-policy.name)"
                sample_direction: "tx"
                sflow_counter_interval: "107"
                speed: "10half"
                stacking_port: "109"
                status: "up"
                sticky_mac: "enable"
                storm_control_policy: "<your_own_value> (source switch-controller.storm-control-policy.name)"
                stp_bpdu_guard: "enabled"
                stp_bpdu_guard_timeout: "114"
                stp_root_guard: "enabled"
                stp_state: "enabled"
                switch_id: "<your_own_value>"
                type: "physical"
                untagged_vlans:
                 -
                    vlan_name: "<your_own_value> (source system.interface.name)"
                vlan: "<your_own_value> (source system.interface.name)"
            pre_provisioned: "122"
            qos_drop_policy: "taildrop"
            qos_red_probability: "124"
            remote_log:
             -
                csv: "enable"
                facility: "kernel"
                name: "default_name_128"
                port: "129"
                server: "192.168.100.40"
                severity: "emergency"
                status: "enable"
            snmp_community:
             -
                events: "cpu-high"
                hosts:
                 -
                    id:  "136"
                    ip: "<your_own_value>"
                id:  "138"
                name: "default_name_139"
                query_v1_port: "140"
                query_v1_status: "disable"
                query_v2c_port: "142"
                query_v2c_status: "disable"
                status: "disable"
                trap_v1_lport: "145"
                trap_v1_rport: "146"
                trap_v1_status: "disable"
                trap_v2c_lport: "148"
                trap_v2c_rport: "149"
                trap_v2c_status: "disable"
            snmp_sysinfo:
                contact_info: "<your_own_value>"
                description: "<your_own_value>"
                engine_id: "<your_own_value>"
                location: "<your_own_value>"
                status: "disable"
            snmp_trap_threshold:
                trap_high_cpu_threshold: "158"
                trap_log_full_threshold: "159"
                trap_low_memory_threshold: "160"
            snmp_user:
             -
                auth_proto: "md5"
                auth_pwd: "<your_own_value>"
                name: "default_name_164"
                priv_proto: "aes"
                priv_pwd: "<your_own_value>"
                queries: "disable"
                query_port: "168"
                security_level: "no-auth-no-priv"
            staged_image_version: "<your_own_value>"
            static_mac:
             -
                description: "<your_own_value>"
                id:  "173"
                interface: "<your_own_value>"
                mac: "<your_own_value>"
                type: "static"
                vlan: "<your_own_value> (source system.interface.name)"
            storm_control:
                broadcast: "enable"
                local_override: "enable"
                rate: "181"
                unknown_multicast: "enable"
                unknown_unicast: "enable"
            stp_instance:
             -
                id:  "185"
                priority: "0"
            stp_settings:
                forward_time: "188"
                hello_time: "189"
                local_override: "enable"
                max_age: "191"
                max_hops: "192"
                name: "default_name_193"
                pending_timer: "194"
                revision: "195"
            switch_device_tag: "<your_own_value>"
            switch_dhcp_opt43_key: "<your_own_value>"
            switch_id: "<your_own_value>"
            switch_log:
                local_override: "enable"
                severity: "emergency"
                status: "enable"
            switch_profile: "<your_own_value> (source switch-controller.switch-profile.name)"
            type: "virtual"
            version: "205"
    


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
