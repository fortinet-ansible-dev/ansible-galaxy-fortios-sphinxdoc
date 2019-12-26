:source: fortios_switch_controller_managed_switch.py

:orphan:

.. _fortios_switch_controller_managed_switch:

fortios_switch_controller_managed_switch -- Configure FortiSwitch devices that are managed by this FortiGate in Fortinet's FortiOS and FortiGate.
+++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++

.. versionadded:: 2.8

.. contents::
   :local:
   :depth: 1


Synopsis
--------
- This module is able to configure a FortiGate or FortiOS (FOS) device by allowing the user to set and modify switch_controller feature and managed_switch category. Examples include all parameters and values need to be adjusted to datasources before usage. Tested with FOS v6.0.5


Requirements
------------
The below requirements are needed on the host that executes this module.

- fortiosapi>=0.9.8


Parameters
----------

.. raw:: html

    <ul>

    <li><span class="li-head">host</span> - FortiOS or FortiGate IP address. <span class="li-normal">type: str</span> <span class="li-required">required: false</span></li>
    <li><span class="li-head">username</span> - FortiOS or FortiGate username. <span class="li-normal">type: str</span> <span class="li-required">required: false</span></li>
    <li><span class="li-head">password</span> - FortiOS or FortiGate password. <span class="li-normal">type: str</span> <span class="li-normal">default: ""</span></li>
    <li><span class="li-head">vdom</span> - Virtual domain, among those defined previously. A vdom is a virtual instance of the FortiGate that can be configured and used as a different unit. <span class="li-normal">type: str</span> <span class="li-normal">default: root</span></li>
    <li><span class="li-head">https</span> - Indicates if the requests towards FortiGate must use HTTPS protocol. <span class="li-normal">type: bool</span> <span class="li-normal">default: true</span></li>
    <li><span class="li-head">ssl_verify</span> - Ensures FortiGate certificate must be verified by a proper CA. <span class="li-normal">type: bool</span> <span class="li-normal">default: true</span></li>
    <li><span class="li-head">state</span> - Indicates whether to create or remove the object. This attribute was present already in previous version in a deeper level. It has been moved out to this outer level. <span class="li-normal">type: str</span> <span class="li-required">required: false</span> <span class="li-normal">choices: present,  absent</span></li>
    <li><span class="li-head">switch_controller_managed_switch</span> - Configure FortiSwitch devices that are managed by this FortiGate. <span class="li-normal">default: null</span> <span class="li-normal">type: dict</span></li>
            <ul class="ul-self">

            <li><span class="li-head">state</span> - B(Deprecated) Starting with Ansible 2.9 we recommend using the top-level 'state' parameter. HORIZONTALLINE Indicates whether to create or remove the object. <span class="li-normal">type: str</span> <span class="li-required">required: false</span> <span class="li-normal">choices: present,  absent</span></li>
            <li><span class="li-head">802_1X_settings</span> - Configuration method to edit FortiSwitch 802.1X global settings. <span class="li-normal">type: dict</span></li>
                    <ul class="ul-self">

                    <li><span class="li-head">link_down_auth</span> - Authentication state to set if a link is down. <span class="li-normal">type: str</span> <span class="li-normal">choices: set-unauth,  no-action</span></li>
                    <li><span class="li-head">local_override</span> - Enable to override global 802.1X settings on individual FortiSwitches. <span class="li-normal">type: str</span> <span class="li-normal">choices: enable,  disable</span></li>
                    <li><span class="li-head">max_reauth_attempt</span> - Maximum number of authentication attempts (0 - 15). <span class="li-normal">type: int</span></li>
                    <li><span class="li-head">reauth_period</span> - Reauthentication time interval (1 - 1440 min). <span class="li-normal">type: int</span>
                    </ul>

            <li><span class="li-head">custom_command</span> - Configuration method to edit FortiSwitch commands to be pushed to this FortiSwitch device upon rebooting the FortiGate switch controller or the FortiSwitch. <span class="li-normal">type: list</span></li>
                    <ul class="ul-self">

                    <li><span class="li-head">command_entry</span> - List of FortiSwitch commands. <span class="li-normal">type: str</span></li>
                    <li><span class="li-head">command_name</span> - Names of commands to be pushed to this FortiSwitch device, as configured under config switch-controller custom-command. Source switch-controller.custom-command.command-name. <span class="li-normal">type: str</span>
                    </ul>

            <li><span class="li-head">delayed_restart_trigger</span> - Delayed restart triggered for this FortiSwitch. <span class="li-normal">type: int</span> description: Description. <span class="li-normal">type: str</span></li>
            <li><span class="li-head">directly_connected</span> - Directly connected FortiSwitch. <span class="li-normal">type: int</span></li>
            <li><span class="li-head">dynamic_capability</span> - List of features this FortiSwitch supports (not configurable) that is sent to the FortiGate device for subsequent configuration initiated by the FortiGate device. <span class="li-normal">type: int</span></li>
            <li><span class="li-head">dynamically_discovered</span> - Dynamically discovered FortiSwitch. <span class="li-normal">type: int</span></li>
            <li><span class="li-head">fsw_wan1_admin</span> - FortiSwitch WAN1 admin status; enable to authorize the FortiSwitch as a managed switch. <span class="li-normal">type: str</span> <span class="li-normal">choices: discovered,  disable,  enable</span></li>
            <li><span class="li-head">fsw_wan1_peer</span> - Fortiswitch WAN1 peer port. <span class="li-normal">type: str</span></li>
            <li><span class="li-head">fsw_wan2_admin</span> - FortiSwitch WAN2 admin status; enable to authorize the FortiSwitch as a managed switch. <span class="li-normal">type: str</span> <span class="li-normal">choices: discovered,  disable,  enable</span></li>
            <li><span class="li-head">fsw_wan2_peer</span> - FortiSwitch WAN2 peer port. <span class="li-normal">type: str</span></li>
            <li><span class="li-head">igmp_snooping</span> - Configure FortiSwitch IGMP snooping global settings. <span class="li-normal">type: dict</span></li>
                    <ul class="ul-self">

                    <li><span class="li-head">aging_time</span> - Maximum time to retain a multicast snooping entry for which no packets have been seen (15 - 3600 sec). <span class="li-normal">type: int</span></li>
                    <li><span class="li-head">flood_unknown_multicast</span> - Enable/disable unknown multicast flooding. <span class="li-normal">type: str</span> <span class="li-normal">choices: enable,  disable</span></li>
                    <li><span class="li-head">local_override</span> - Enable/disable overriding the global IGMP snooping configuration. <span class="li-normal">type: str</span> <span class="li-normal">choices: enable,  disable</span>
                    </ul>

            <li><span class="li-head">max_allowed_trunk_members</span> - FortiSwitch maximum allowed trunk members. <span class="li-normal">type: int</span></li>
            <li><span class="li-head">mirror</span> - Configuration method to edit FortiSwitch packet mirror. <span class="li-normal">type: list</span></li>
                    <ul class="ul-self">

                    <li><span class="li-head">dst</span> - Destination port. <span class="li-normal">type: str</span></li>
                    <li><span class="li-head">name</span> - Mirror name. <span class="li-required">required</span> <span class="li-normal">type: str</span></li>
                    <li><span class="li-head">src_egress</span> - Source egress interfaces. <span class="li-normal">type: list</span></li>
                            <ul class="ul-self">

                            <li><span class="li-head">name</span> - Interface name. <span class="li-required">required</span> <span class="li-normal">type: str</span>
                            </ul>

                    <li><span class="li-head">src_ingress</span> - Source ingress interfaces. <span class="li-normal">type: list</span></li>
                            <ul class="ul-self">

                            <li><span class="li-head">name</span> - Interface name. <span class="li-required">required</span> <span class="li-normal">type: str</span>
                            </ul>

                    <li><span class="li-head">status</span> - Active/inactive mirror configuration. <span class="li-normal">type: str</span> <span class="li-normal">choices: active,  inactive</span></li>
                    <li><span class="li-head">switching_packet</span> - Enable/disable switching functionality when mirroring. <span class="li-normal">type: str</span> <span class="li-normal">choices: enable,  disable</span>
                    </ul>

            <li><span class="li-head">name</span> - Managed-switch name. <span class="li-normal">type: str</span></li>
            <li><span class="li-head">owner_vdom</span> - VDOM which owner of port belongs to. <span class="li-normal">type: str</span></li>
            <li><span class="li-head">poe_detection_type</span> - PoE detection type for FortiSwitch. <span class="li-normal">type: int</span></li>
            <li><span class="li-head">poe_pre_standard_detection</span> - Enable/disable PoE pre-standard detection. <span class="li-normal">type: str</span> <span class="li-normal">choices: enable,  disable</span></li>
            <li><span class="li-head">ports</span> - Managed-switch port list. <span class="li-normal">type: list</span></li>
                    <ul class="ul-self">

                    <li><span class="li-head">allowed_vlans</span> - Configure switch port tagged vlans <span class="li-normal">type: list</span></li>
                            <ul class="ul-self">

                            <li><span class="li-head">vlan_name</span> - VLAN name. Source system.interface.name. <span class="li-normal">type: str</span>
                            </ul>

                    <li><span class="li-head">allowed_vlans_all</span> - Enable/disable all defined vlans on this port. <span class="li-normal">type: str</span> <span class="li-normal">choices: enable,  disable</span></li>
                    <li><span class="li-head">arp_inspection_trust</span> - Trusted or untrusted dynamic ARP inspection. <span class="li-normal">type: str</span> <span class="li-normal">choices: untrusted,  trusted</span></li>
                    <li><span class="li-head">bundle</span> - Enable/disable Link Aggregation Group (LAG) bundling for non-FortiLink interfaces. <span class="li-normal">type: str</span> <span class="li-normal">choices: enable,  disable</span> description: Description for port. <span class="li-normal">type: str</span></li>
                    <li><span class="li-head">dhcp_snoop_option82_trust</span> - Enable/disable allowance of DHCP with option-82 on untrusted interface. <span class="li-normal">type: str</span> <span class="li-normal">choices: enable,  disable</span></li>
                    <li><span class="li-head">dhcp_snooping</span> - Trusted or untrusted DHCP-snooping interface. <span class="li-normal">type: str</span> <span class="li-normal">choices: untrusted,  trusted</span></li>
                    <li><span class="li-head">discard_mode</span> - Configure discard mode for port. <span class="li-normal">type: str</span> <span class="li-normal">choices: none,  all-untagged,  all-tagged</span></li>
                    <li><span class="li-head">edge_port</span> - Enable/disable this interface as an edge port, bridging connections between workstations and/or computers. <span class="li-normal">type: str</span> <span class="li-normal">choices: enable,  disable</span></li>
                    <li><span class="li-head">export_tags</span> - Switch controller export tag name. <span class="li-normal">type: list</span></li>
                            <ul class="ul-self">

                            <li><span class="li-head">tag_name</span> - Switch tag name. Source switch-controller.switch-interface-tag.name. <span class="li-normal">type: str</span>
                            </ul>

                    <li><span class="li-head">export_to</span> - Export managed-switch port to a tenant VDOM. Source system.vdom.name. <span class="li-normal">type: str</span></li>
                    <li><span class="li-head">export_to_pool</span> - Switch controller export port to pool-list. Source switch-controller.virtual-port-pool.name. <span class="li-normal">type: str</span></li>
                    <li><span class="li-head">export_to_pool_flag</span> - Switch controller export port to pool-list. <span class="li-normal">type: int</span></li>
                    <li><span class="li-head">fgt_peer_device_name</span> - FGT peer device name. <span class="li-normal">type: str</span></li>
                    <li><span class="li-head">fgt_peer_port_name</span> - FGT peer port name. <span class="li-normal">type: str</span></li>
                    <li><span class="li-head">fiber_port</span> - Fiber-port. <span class="li-normal">type: int</span></li>
                    <li><span class="li-head">flags</span> - Port properties flags. <span class="li-normal">type: int</span></li>
                    <li><span class="li-head">fortilink_port</span> - FortiLink uplink port. <span class="li-normal">type: int</span></li>
                    <li><span class="li-head">igmp_snooping</span> - Set IGMP snooping mode for the physical port interface. <span class="li-normal">type: str</span> <span class="li-normal">choices: enable,  disable</span></li>
                    <li><span class="li-head">igmps_flood_reports</span> - Enable/disable flooding of IGMP reports to this interface when igmp-snooping enabled. <span class="li-normal">type: str</span> <span class="li-normal">choices: enable,  disable</span></li>
                    <li><span class="li-head">igmps_flood_traffic</span> - Enable/disable flooding of IGMP snooping traffic to this interface. <span class="li-normal">type: str</span> <span class="li-normal">choices: enable,  disable</span></li>
                    <li><span class="li-head">isl_local_trunk_name</span> - ISL local trunk name. <span class="li-normal">type: str</span></li>
                    <li><span class="li-head">isl_peer_device_name</span> - ISL peer device name. <span class="li-normal">type: str</span></li>
                    <li><span class="li-head">isl_peer_port_name</span> - ISL peer port name. <span class="li-normal">type: str</span></li>
                    <li><span class="li-head">lacp_speed</span> - end Link Aggregation Control Protocol (LACP) messages every 30 seconds (slow) or every second (fast). <span class="li-normal">type: str</span> <span class="li-normal">choices: slow,  fast</span></li>
                    <li><span class="li-head">learning_limit</span> - Limit the number of dynamic MAC addresses on this Port (1 - 128, 0 = no limit, default). <span class="li-normal">type: int</span></li>
                    <li><span class="li-head">lldp_profile</span> - LLDP port TLV profile. Source switch-controller.lldp-profile.name. <span class="li-normal">type: str</span></li>
                    <li><span class="li-head">lldp_status</span> - LLDP transmit and receive status. <span class="li-normal">type: str</span> <span class="li-normal">choices: disable,  rx-only,  tx-only,  tx-rx</span></li>
                    <li><span class="li-head">loop_guard</span> - Enable/disable loop-guard on this interface, an STP optimization used to prevent network loops. <span class="li-normal">type: str</span> <span class="li-normal">choices: enabled,  disabled</span></li>
                    <li><span class="li-head">loop_guard_timeout</span> - Loop-guard timeout (0 - 120 min). <span class="li-normal">type: int</span></li>
                    <li><span class="li-head">max_bundle</span> - Maximum size of LAG bundle (1 - 24) <span class="li-normal">type: int</span></li>
                    <li><span class="li-head">mclag</span> - Enable/disable multi-chassis link aggregation (MCLAG). <span class="li-normal">type: str</span> <span class="li-normal">choices: enable,  disable</span></li>
                    <li><span class="li-head">member_withdrawal_behavior</span> - Port behavior after it withdraws because of loss of control packets. <span class="li-normal">type: str</span> <span class="li-normal">choices: forward,  block</span></li>
                    <li><span class="li-head">members</span> - Aggregated LAG bundle interfaces. <span class="li-normal">type: list</span></li>
                            <ul class="ul-self">

                            <li><span class="li-head">member_name</span> - Interface name from available options. <span class="li-normal">type: str</span>
                            </ul>

                    <li><span class="li-head">min_bundle</span> - Minimum size of LAG bundle (1 - 24) <span class="li-normal">type: int</span></li>
                    <li><span class="li-head">mode</span> - "LACP mode: ignore and do not send control messages, or negotiate 802.3ad aggregation passively or actively." <span class="li-normal">type: str</span> <span class="li-normal">choices: static,  lacp-passive,  lacp-active</span></li>
                    <li><span class="li-head">poe_capable</span> - PoE capable. <span class="li-normal">type: int</span></li>
                    <li><span class="li-head">poe_pre_standard_detection</span> - Enable/disable PoE pre-standard detection. <span class="li-normal">type: str</span> <span class="li-normal">choices: enable,  disable</span></li>
                    <li><span class="li-head">poe_status</span> - Enable/disable PoE status. <span class="li-normal">type: str</span> <span class="li-normal">choices: enable,  disable</span></li>
                    <li><span class="li-head">port_name</span> - Switch port name. <span class="li-normal">type: str</span></li>
                    <li><span class="li-head">port_number</span> - Port number. <span class="li-normal">type: int</span></li>
                    <li><span class="li-head">port_owner</span> - Switch port name. <span class="li-normal">type: str</span></li>
                    <li><span class="li-head">port_prefix_type</span> - Port prefix type. <span class="li-normal">type: int</span></li>
                    <li><span class="li-head">port_security_policy</span> - Switch controller authentication policy to apply to this managed switch from available options. Source switch-controller .security-policy.802-1X.name switch-controller.security-policy.captive-portal.name. <span class="li-normal">type: str</span></li>
                    <li><span class="li-head">port_selection_criteria</span> - Algorithm for aggregate port selection. <span class="li-normal">type: str</span> <span class="li-normal">choices: src-mac,  dst-mac,  src-dst-mac,  src-ip,  dst-ip,  src-dst-ip</span></li>
                    <li><span class="li-head">qos_policy</span> - Switch controller QoS policy from available options. Source switch-controller.qos.qos-policy.name. <span class="li-normal">type: str</span></li>
                    <li><span class="li-head">sample_direction</span> - sFlow sample direction. <span class="li-normal">type: str</span> <span class="li-normal">choices: tx,  rx,  both</span></li>
                    <li><span class="li-head">sflow_counter_interval</span> - sFlow sampler counter polling interval (1 - 255 sec). <span class="li-normal">type: int</span></li>
                    <li><span class="li-head">sflow_sample_rate</span> - sFlow sampler sample rate (0 - 99999 p/sec). <span class="li-normal">type: int</span></li>
                    <li><span class="li-head">sflow_sampler</span> - Enable/disable sFlow protocol on this interface. <span class="li-normal">type: str</span> <span class="li-normal">choices: enabled,  disabled</span></li>
                    <li><span class="li-head">speed</span> - Switch port speed; default and available settings depend on hardware. <span class="li-normal">type: str</span> <span class="li-normal">choices: 10half,  10full,  100half,  100full,  1000auto,  1000fiber,  1000full,  10000,  40000,  auto,  auto-module,  100FX-half,  100FX-full,  100000full,  2500full,  25000full,  50000full</span></li>
                    <li><span class="li-head">speed_mask</span> - Switch port speed mask. <span class="li-normal">type: int</span></li>
                    <li><span class="li-head">stacking_port</span> - Stacking port. <span class="li-normal">type: int</span></li>
                    <li><span class="li-head">status</span> - "Switch port admin status: up or down." <span class="li-normal">type: str</span> <span class="li-normal">choices: up,  down</span></li>
                    <li><span class="li-head">stp_bpdu_guard</span> - Enable/disable STP BPDU guard on this interface. <span class="li-normal">type: str</span> <span class="li-normal">choices: enabled,  disabled</span></li>
                    <li><span class="li-head">stp_bpdu_guard_timeout</span> - BPDU Guard disabling protection (0 - 120 min). <span class="li-normal">type: int</span></li>
                    <li><span class="li-head">stp_root_guard</span> - Enable/disable STP root guard on this interface. <span class="li-normal">type: str</span> <span class="li-normal">choices: enabled,  disabled</span></li>
                    <li><span class="li-head">stp_state</span> - Enable/disable Spanning Tree Protocol (STP) on this interface. <span class="li-normal">type: str</span> <span class="li-normal">choices: enabled,  disabled</span></li>
                    <li><span class="li-head">switch_id</span> - Switch id. <span class="li-normal">type: str</span> <span class="li-normal">type:</span> "Interface type: physical or trunk port." <span class="li-normal">type: str</span> <span class="li-normal">choices: physical,  trunk</span></li>
                    <li><span class="li-head">untagged_vlans</span> - Configure switch port untagged vlans <span class="li-normal">type: list</span></li>
                            <ul class="ul-self">

                            <li><span class="li-head">vlan_name</span> - VLAN name. Source system.interface.name. <span class="li-normal">type: str</span>
                            </ul>

                    <li><span class="li-head">virtual_port</span> - Virtualized switch port. <span class="li-normal">type: int</span></li>
                    <li><span class="li-head">vlan</span> - Assign switch ports to a VLAN. Source system.interface.name. <span class="li-normal">type: str</span>
                    </ul>

            <li><span class="li-head">pre_provisioned</span> - Pre-provisioned managed switch. <span class="li-normal">type: int</span></li>
            <li><span class="li-head">staged_image_version</span> - Staged image version for FortiSwitch. <span class="li-normal">type: str</span></li>
            <li><span class="li-head">storm_control</span> - Configuration method to edit FortiSwitch storm control for measuring traffic activity using data rates to prevent traffic disruption. <span class="li-normal">type: dict</span></li>
                    <ul class="ul-self">

                    <li><span class="li-head">broadcast</span> - Enable/disable storm control to drop broadcast traffic. <span class="li-normal">type: str</span> <span class="li-normal">choices: enable,  disable</span></li>
                    <li><span class="li-head">local_override</span> - Enable to override global FortiSwitch storm control settings for this FortiSwitch. <span class="li-normal">type: str</span> <span class="li-normal">choices: enable,  disable</span></li>
                    <li><span class="li-head">rate</span> - Rate in packets per second at which storm traffic is controlled (1 - 10000000). Storm control drops excess traffic data rates beyond this threshold. <span class="li-normal">type: int</span></li>
                    <li><span class="li-head">unknown_multicast</span> - Enable/disable storm control to drop unknown multicast traffic. <span class="li-normal">type: str</span> <span class="li-normal">choices: enable,  disable</span></li>
                    <li><span class="li-head">unknown_unicast</span> - Enable/disable storm control to drop unknown unicast traffic. <span class="li-normal">type: str</span> <span class="li-normal">choices: enable,  disable</span>
                    </ul>

            <li><span class="li-head">stp_settings</span> - Configuration method to edit Spanning Tree Protocol (STP) settings used to prevent bridge loops. <span class="li-normal">type: dict</span></li>
                    <ul class="ul-self">

                    <li><span class="li-head">forward_time</span> - Period of time a port is in listening and learning state (4 - 30 sec). <span class="li-normal">type: int</span></li>
                    <li><span class="li-head">hello_time</span> - Period of time between successive STP frame Bridge Protocol Data Units (BPDUs) sent on a port (1 - 10 sec). <span class="li-normal">type: int</span></li>
                    <li><span class="li-head">local_override</span> - Enable to configure local STP settings that override global STP settings. <span class="li-normal">type: str</span> <span class="li-normal">choices: enable,  disable</span></li>
                    <li><span class="li-head">max_age</span> - Maximum time before a bridge port saves its configuration BPDU information (6 - 40 sec). <span class="li-normal">type: int</span></li>
                    <li><span class="li-head">max_hops</span> - Maximum number of hops between the root bridge and the furthest bridge (1- 40). <span class="li-normal">type: int</span></li>
                    <li><span class="li-head">name</span> - Name of local STP settings configuration. <span class="li-normal">type: str</span></li>
                    <li><span class="li-head">pending_timer</span> - Pending time (1 - 15 sec). <span class="li-normal">type: int</span></li>
                    <li><span class="li-head">revision</span> - STP revision number (0 - 65535). <span class="li-normal">type: int</span></li>
                    <li><span class="li-head">status</span> - Enable/disable STP. <span class="li-normal">type: str</span> <span class="li-normal">choices: enable,  disable</span>
                    </ul>

            <li><span class="li-head">switch_device_tag</span> - User definable label/tag. <span class="li-normal">type: str</span></li>
            <li><span class="li-head">switch_id</span> - Managed-switch id. <span class="li-normal">type: str</span></li>
            <li><span class="li-head">switch_log</span> - Configuration method to edit FortiSwitch logging settings (logs are transferred to and inserted into the FortiGate event log). <span class="li-normal">type: dict</span></li>
                    <ul class="ul-self">

                    <li><span class="li-head">local_override</span> - Enable to configure local logging settings that override global logging settings. <span class="li-normal">type: str</span> <span class="li-normal">choices: enable,  disable</span></li>
                    <li><span class="li-head">severity</span> - Severity of FortiSwitch logs that are added to the FortiGate event log. <span class="li-normal">type: str</span> <span class="li-normal">choices: emergency,  alert,  critical,  error,  warning,  notification,  information,  debug</span></li>
                    <li><span class="li-head">status</span> - Enable/disable adding FortiSwitch logs to the FortiGate event log. <span class="li-normal">type: str</span> <span class="li-normal">choices: enable,  disable</span>
                    </ul>

            <li><span class="li-head">switch_profile</span> - FortiSwitch profile. Source switch-controller.switch-profile.name. <span class="li-normal">type: str</span></li>
            <li><span class="li-head">switch_stp_settings</span> - Configure spanning tree protocol (STP). <span class="li-normal">type: dict</span></li>
                    <ul class="ul-self">

                    <li><span class="li-head">status</span> - Enable/disable STP. <span class="li-normal">type: str</span> <span class="li-normal">choices: enable,  disable</span>
                    </ul>

            <li><span class="li-head">type</span> - Indication of switch type, physical or virtual. <span class="li-normal">type: str</span> <span class="li-normal">choices: virtual,  physical</span></li>
            <li><span class="li-head">version</span> - FortiSwitch version. <span class="li-normal">type: int</span>
            </ul>

    </ul>




Notes
-----

.. note::


   - Requires fortiosapi library developed by Fortinet

   - Run as a local_action in your playbook



Examples
--------

.. code-block:: yaml+jinja

    - hosts: localhost
      vars:
       host: "192.168.122.40"
       username: "admin"
       password: ""
       vdom: "root"
       ssl_verify: "False"
      tasks:
      - name: Configure FortiSwitch devices that are managed by this FortiGate.
        fortios_switch_controller_managed_switch:
          host:  "{{ host }}"
          username: "{{ username }}"
          password: "{{ password }}"
          vdom:  "{{ vdom }}"
          https: "False"
          state: "present"
          switch_controller_managed_switch:
            802_1X_settings:
                link_down_auth: "set-unauth"
                local_override: "enable"
                max_reauth_attempt: "6"
                reauth_period: "7"
            custom_command:
             -
                command_entry: "<your_own_value>"
                command_name: "<your_own_value> (source switch-controller.custom-command.command-name)"
            delayed_restart_trigger: "11"
            description: "<your_own_value>"
            directly_connected: "13"
            dynamic_capability: "14"
            dynamically_discovered: "15"
            fsw_wan1_admin: "discovered"
            fsw_wan1_peer: "<your_own_value>"
            fsw_wan2_admin: "discovered"
            fsw_wan2_peer: "<your_own_value>"
            igmp_snooping:
                aging_time: "21"
                flood_unknown_multicast: "enable"
                local_override: "enable"
            max_allowed_trunk_members: "24"
            mirror:
             -
                dst: "<your_own_value>"
                name: "default_name_27"
                src_egress:
                 -
                    name: "default_name_29"
                src_ingress:
                 -
                    name: "default_name_31"
                status: "active"
                switching_packet: "enable"
            name: "default_name_34"
            owner_vdom: "<your_own_value>"
            poe_detection_type: "36"
            poe_pre_standard_detection: "enable"
            ports:
             -
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
                export_to_pool_flag: "53"
                fgt_peer_device_name: "<your_own_value>"
                fgt_peer_port_name: "<your_own_value>"
                fiber_port: "56"
                flags: "57"
                fortilink_port: "58"
                igmp_snooping: "enable"
                igmps_flood_reports: "enable"
                igmps_flood_traffic: "enable"
                isl_local_trunk_name: "<your_own_value>"
                isl_peer_device_name: "<your_own_value>"
                isl_peer_port_name: "<your_own_value>"
                lacp_speed: "slow"
                learning_limit: "66"
                lldp_profile: "<your_own_value> (source switch-controller.lldp-profile.name)"
                lldp_status: "disable"
                loop_guard: "enabled"
                loop_guard_timeout: "70"
                max_bundle: "71"
                mclag: "enable"
                member_withdrawal_behavior: "forward"
                members:
                 -
                    member_name: "<your_own_value>"
                min_bundle: "76"
                mode: "static"
                poe_capable: "78"
                poe_pre_standard_detection: "enable"
                poe_status: "enable"
                port_name: "<your_own_value>"
                port_number: "82"
                port_owner: "<your_own_value>"
                port_prefix_type: "84"
                port_security_policy: "<your_own_value> (source switch-controller.security-policy.802-1X.name switch-controller.security-policy.captive-portal
                  .name)"
                port_selection_criteria: "src-mac"
                qos_policy: "<your_own_value> (source switch-controller.qos.qos-policy.name)"
                sample_direction: "tx"
                sflow_counter_interval: "89"
                sflow_sample_rate: "90"
                sflow_sampler: "enabled"
                speed: "10half"
                speed_mask: "93"
                stacking_port: "94"
                status: "up"
                stp_bpdu_guard: "enabled"
                stp_bpdu_guard_timeout: "97"
                stp_root_guard: "enabled"
                stp_state: "enabled"
                switch_id: "<your_own_value>"
                type: "physical"
                untagged_vlans:
                 -
                    vlan_name: "<your_own_value> (source system.interface.name)"
                virtual_port: "104"
                vlan: "<your_own_value> (source system.interface.name)"
            pre_provisioned: "106"
            staged_image_version: "<your_own_value>"
            storm_control:
                broadcast: "enable"
                local_override: "enable"
                rate: "111"
                unknown_multicast: "enable"
                unknown_unicast: "enable"
            stp_settings:
                forward_time: "115"
                hello_time: "116"
                local_override: "enable"
                max_age: "118"
                max_hops: "119"
                name: "default_name_120"
                pending_timer: "121"
                revision: "122"
                status: "enable"
            switch_device_tag: "<your_own_value>"
            switch_id: "<your_own_value>"
            switch_log:
                local_override: "enable"
                severity: "emergency"
                status: "enable"
            switch_profile: "<your_own_value> (source switch-controller.switch-profile.name)"
            switch_stp_settings:
                status: "enable"
            type: "virtual"
            version: "134"



Return Values
-------------
Common return values are documented: https://docs.ansible.com/ansible/latest/reference_appendices/common_return_values.html#common-return-values, the following are the fields unique to this module:

.. raw:: html

    <ul>

    <li><span class="li-return">build</span> - Build number of the fortigate image <span class="li-normal">returned: always</span> <span class="li-normal">type: str</span> <span class="li-normal">sample: '1547'</span></li>
    <li><span class="li-return">http_method</span> - Last method used to provision the content into FortiGate <span class="li-normal">returned: always</span> <span class="li-normal">type: str</span> <span class="li-normal">sample: 'PUT'</span></li>
    <li><span class="li-return">http_status</span> - Last result given by FortiGate on last operation applied <span class="li-normal">returned: always</span> <span class="li-normal">type: str</span> <span class="li-normal">sample: 200</span></li>
    <li><span class="li-return">mkey</span> - Master key (id) used in the last call to FortiGate <span class="li-normal">returned: success</span> <span class="li-normal">type: str</span> <span class="li-normal">sample: id</span></li>
    <li><span class="li-return">name</span> - Name of the table used to fulfill the request <span class="li-normal">returned: always</span> <span class="li-normal">type: str</span> <span class="li-normal">sample: urlfilter</span></li>
    <li><span class="li-return">path</span> - Path of the table used to fulfill the request <span class="li-normal">returned: always</span> <span class="li-normal">type: str</span> <span class="li-normal">sample: webfilter</span></li>
    <li><span class="li-return">revision</span> - Internal revision number <span class="li-normal">returned: always</span> <span class="li-normal">type: str</span> <span class="li-normal">sample: 17.0.2.10658</span></li>
    <li><span class="li-return">serial</span> - Serial number of the unit <span class="li-normal">returned: always</span> <span class="li-normal">type: str</span> <span class="li-normal">sample: FGVMEVYYQT3AB5352</span></li>
    <li><span class="li-return">status</span> - Indication of the operation's result <span class="li-normal">returned: always</span> <span class="li-normal">type: str</span> <span class="li-normal">sample: success</span></li>
    <li><span class="li-return">vdom</span> - Virtual domain used <span class="li-normal">returned: always</span> <span class="li-normal">type: str</span> <span class="li-normal">sample: root</span></li>
    <li><span class="li-return">version</span> - Version of the FortiGate <span class="li-normal">returned: always</span> <span class="li-normal">type: str</span> <span class="li-normal">sample: v5.6.3</span></li>
    </ul>



Status
------

- This module is not guaranteed to have a backwards compatible interface.



Authors
-------

- Miguel Angel Munoz (@mamunozgonzalez)
- Nicolas Thomas (@thomnico)



.. hint::
    If you notice any issues in this documentation, you can create a pull request to improve it.