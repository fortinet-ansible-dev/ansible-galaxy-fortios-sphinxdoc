:source: fortios_system_virtual_wan_link.py

:orphan:

.. fortios_system_virtual_wan_link:

fortios_system_virtual_wan_link -- Configure redundant internet connections using SD-WAN (formerly virtual WAN link) in Fortinet's FortiOS and FortiGate.
+++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++

.. versionadded:: 2.8

.. contents::
   :local:
   :depth: 1


Synopsis
--------
- This module is able to configure a FortiGate or FortiOS (FOS) device by allowing the user to set and modify system feature and virtual_wan_link category. Examples include all parameters and values need to be adjusted to datasources before usage. Tested with FOS v6.2.0



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
    <li> <span class="li-head">system_virtual_wan_link</span> - Configure redundant internet connections using SD-WAN (formerly virtual WAN link). <span class="li-normal">type: dict</span></li>
        <ul class="ul-self">
        <li> <span class="li-head">fail_alert_interfaces</span> - Physical interfaces that will be alerted. <span class="li-normal">type: list</span></li>
            <ul class="ul-self">
            <li> <span class="li-head">name</span> - Physical interface name. Source system.interface.name. <span class="li-normal">type: str</span> <span class="li-required">required: True</span></li>
            </ul>
        <li> <span class="li-head">fail_detect</span> - Enable/disable SD-WAN Internet connection status checking (failure detection). <span class="li-normal">type: str</span> <span class="li-normal">choices: enable, disable</span></li>
        <li> <span class="li-head">health_check</span> - SD-WAN status checking or health checking. Identify a server on the Internet and determine how SD-WAN verifies that the FortiGate can communicate with it. <span class="li-normal">type: list</span></li>
            <ul class="ul-self">
            <li> <span class="li-head">addr_mode</span> - Address mode (IPv4 or IPv6). <span class="li-normal">type: str</span> <span class="li-normal">choices: ipv4, ipv6</span></li>
            <li> <span class="li-head">failtime</span> - Number of failures before server is considered lost (1 - 3600). <span class="li-normal">type: int</span></li>
            <li> <span class="li-head">http_agent</span> - String in the http-agent field in the HTTP header. <span class="li-normal">type: str</span></li>
            <li> <span class="li-head">http_get</span> - URL used to communicate with the server if the protocol if the protocol is HTTP. <span class="li-normal">type: str</span></li>
            <li> <span class="li-head">http_match</span> - Response string expected from the server if the protocol is HTTP. <span class="li-normal">type: str</span></li>
            <li> <span class="li-head">internet_service_id</span> - Internet service ID. Source firewall.internet-service.id. <span class="li-normal">type: int</span></li>
            <li> <span class="li-head">interval</span> - Status check interval in milliseconds, or the time between attempting to connect to the server (500 - 3600*1000 msec). <span class="li-normal">type: int</span></li>
            <li> <span class="li-head">members</span> - Member sequence number list. <span class="li-normal">type: list</span></li>
                <ul class="ul-self">
                <li> <span class="li-head">seq_num</span> - Member sequence number. Source system.virtual-wan-link.members.seq-num. <span class="li-normal">type: int</span></li>
                </ul>
            <li> <span class="li-head">name</span> - Status check or health check name. <span class="li-normal">type: str</span> <span class="li-required">required: True</span></li>
            <li> <span class="li-head">packet_size</span> - Packet size of a twamp test session, <span class="li-normal">type: int</span></li>
            <li> <span class="li-head">password</span> - Twamp controller password in authentication mode <span class="li-normal">type: str</span></li>
            <li> <span class="li-head">port</span> - Port number used to communicate with the server over the selected protocol. <span class="li-normal">type: int</span></li>
            <li> <span class="li-head">probe_packets</span> - Enable/disable transmission of probe packets. <span class="li-normal">type: str</span> <span class="li-normal">choices: disable, enable</span></li>
            <li> <span class="li-head">protocol</span> - Protocol used to determine if the FortiGate can communicate with the server. <span class="li-normal">type: str</span> <span class="li-normal">choices: ping, tcp-echo, udp-echo, http, twamp, ping6</span></li>
            <li> <span class="li-head">recoverytime</span> - Number of successful responses received before server is considered recovered (1 - 3600). <span class="li-normal">type: int</span></li>
            <li> <span class="li-head">security_mode</span> - Twamp controller security mode. <span class="li-normal">type: str</span> <span class="li-normal">choices: none, authentication</span></li>
            <li> <span class="li-head">server</span> - IP address or FQDN name of the server. <span class="li-normal">type: str</span></li>
            <li> <span class="li-head">sla</span> - Service level agreement (SLA). <span class="li-normal">type: list</span></li>
                <ul class="ul-self">
                <li> <span class="li-head">id</span> - SLA ID. <span class="li-normal">type: int</span> <span class="li-required">required: True</span></li>
                <li> <span class="li-head">jitter_threshold</span> - Jitter for SLA to make decision in milliseconds. (0 - 10000000). <span class="li-normal">type: int</span></li>
                <li> <span class="li-head">latency_threshold</span> - Latency for SLA to make decision in milliseconds. (0 - 10000000). <span class="li-normal">type: int</span></li>
                <li> <span class="li-head">link_cost_factor</span> - Criteria on which to base link selection. <span class="li-normal">type: str</span> <span class="li-normal">choices: latency, jitter, packet-loss</span></li>
                <li> <span class="li-head">packetloss_threshold</span> - Packet loss for SLA to make decision in percentage. (0 - 100). <span class="li-normal">type: int</span></li>
                </ul>
            <li> <span class="li-head">sla_fail_log_period</span> - Time interval in seconds that SLA fail log messages will be generated (0 - 3600). <span class="li-normal">type: int</span></li>
            <li> <span class="li-head">sla_pass_log_period</span> - Time interval in seconds that SLA pass log messages will be generated (0 - 3600). <span class="li-normal">type: int</span></li>
            <li> <span class="li-head">threshold_alert_jitter</span> - Alert threshold for jitter (ms). <span class="li-normal">type: int</span></li>
            <li> <span class="li-head">threshold_alert_latency</span> - Alert threshold for latency (ms). <span class="li-normal">type: int</span></li>
            <li> <span class="li-head">threshold_alert_packetloss</span> - Alert threshold for packet loss (percentage). <span class="li-normal">type: int</span></li>
            <li> <span class="li-head">threshold_warning_jitter</span> - Warning threshold for jitter (ms). <span class="li-normal">type: int</span></li>
            <li> <span class="li-head">threshold_warning_latency</span> - Warning threshold for latency (ms). <span class="li-normal">type: int</span></li>
            <li> <span class="li-head">threshold_warning_packetloss</span> - Warning threshold for packet loss (percentage). <span class="li-normal">type: int</span></li>
            <li> <span class="li-head">update_cascade_interface</span> - Enable/disable update cascade interface. <span class="li-normal">type: str</span> <span class="li-normal">choices: enable, disable</span></li>
            <li> <span class="li-head">update_static_route</span> - Enable/disable updating the static route. <span class="li-normal">type: str</span> <span class="li-normal">choices: enable, disable</span></li>
            </ul>
        <li> <span class="li-head">load_balance_mode</span> - Algorithm or mode to use for load balancing Internet traffic to SD-WAN members. <span class="li-normal">type: str</span> <span class="li-normal">choices: source-ip-based, weight-based, usage-based, source-dest-ip-based, measured-volume-based</span></li>
        <li> <span class="li-head">members</span> - FortiGate interfaces added to the virtual-wan-link. <span class="li-normal">type: list</span></li>
            <ul class="ul-self">
            <li> <span class="li-head">comment</span> - Comments. <span class="li-normal">type: str</span></li>
            <li> <span class="li-head">cost</span> - Cost of this interface for services in SLA mode (0 - 4294967295). <span class="li-normal">type: int</span></li>
            <li> <span class="li-head">gateway</span> - The default gateway for this interface. Usually the default gateway of the Internet service provider that this interface is connected to. <span class="li-normal">type: str</span></li>
            <li> <span class="li-head">gateway6</span> - IPv6 gateway. <span class="li-normal">type: str</span></li>
            <li> <span class="li-head">ingress_spillover_threshold</span> - Ingress spillover threshold for this interface (0 - 16776000 kbit/s). When this traffic volume threshold is reached, new sessions spill over to other interfaces in the SD-WAN. <span class="li-normal">type: int</span></li>
            <li> <span class="li-head">interface</span> - Interface name. Source system.interface.name. <span class="li-normal">type: str</span></li>
            <li> <span class="li-head">priority</span> - Priority of the interface (0 - 4294967295). Used for SD-WAN rules or priority rules. <span class="li-normal">type: int</span></li>
            <li> <span class="li-head">seq_num</span> - Sequence number(1-255). <span class="li-normal">type: int</span></li>
            <li> <span class="li-head">source</span> - Source IP address used in the health-check packet to the server. <span class="li-normal">type: str</span></li>
            <li> <span class="li-head">source6</span> - Source IPv6 address used in the health-check packet to the server. <span class="li-normal">type: str</span></li>
            <li> <span class="li-head">spillover_threshold</span> - Egress spillover threshold for this interface (0 - 16776000 kbit/s). When this traffic volume threshold is reached, new sessions spill over to other interfaces in the SD-WAN. <span class="li-normal">type: int</span></li>
            <li> <span class="li-head">status</span> - Enable/disable this interface in the SD-WAN. <span class="li-normal">type: str</span> <span class="li-normal">choices: disable, enable</span></li>
            <li> <span class="li-head">volume_ratio</span> - Measured volume ratio (this value / sum of all values = percentage of link volume, 0 - 255). <span class="li-normal">type: int</span></li>
            <li> <span class="li-head">weight</span> - Weight of this interface for weighted load balancing. (0 - 255) More traffic is directed to interfaces with higher weights. <span class="li-normal">type: int</span></li>
            </ul>
        <li> <span class="li-head">service</span> - Create SD-WAN rules (also called services) to control how sessions are distributed to interfaces in the SD-WAN. <span class="li-normal">type: list</span></li>
            <ul class="ul-self">
            <li> <span class="li-head">addr_mode</span> - Address mode (IPv4 or IPv6). <span class="li-normal">type: str</span> <span class="li-normal">choices: ipv4, ipv6</span></li>
            <li> <span class="li-head">bandwidth_weight</span> - Coefficient of reciprocal of available bidirectional bandwidth in the formula of custom-profile-1. <span class="li-normal">type: int</span></li>
            <li> <span class="li-head">default</span> - Enable/disable use of SD-WAN as default service. <span class="li-normal">type: str</span> <span class="li-normal">choices: enable, disable</span></li>
            <li> <span class="li-head">dscp_forward</span> - Enable/disable forward traffic DSCP tag. <span class="li-normal">type: str</span> <span class="li-normal">choices: enable, disable</span></li>
            <li> <span class="li-head">dscp_forward_tag</span> - Forward traffic DSCP tag. <span class="li-normal">type: str</span></li>
            <li> <span class="li-head">dscp_reverse</span> - Enable/disable reverse traffic DSCP tag. <span class="li-normal">type: str</span> <span class="li-normal">choices: enable, disable</span></li>
            <li> <span class="li-head">dscp_reverse_tag</span> - Reverse traffic DSCP tag. <span class="li-normal">type: str</span></li>
            <li> <span class="li-head">dst</span> - Destination address name. <span class="li-normal">type: list</span></li>
                <ul class="ul-self">
                <li> <span class="li-head">name</span> - Address or address group name. Source firewall.address.name firewall.addrgrp.name. <span class="li-normal">type: str</span> <span class="li-required">required: True</span></li>
                </ul>
            <li> <span class="li-head">dst_negate</span> - Enable/disable negation of destination address match. <span class="li-normal">type: str</span> <span class="li-normal">choices: enable, disable</span></li>
            <li> <span class="li-head">dst6</span> - Destination address6 name. <span class="li-normal">type: list</span></li>
                <ul class="ul-self">
                <li> <span class="li-head">name</span> - Address6 or address6 group name. Source firewall.address6.name firewall.addrgrp6.name. <span class="li-normal">type: str</span> <span class="li-required">required: True</span></li>
                </ul>
            <li> <span class="li-head">end_port</span> - End destination port number. <span class="li-normal">type: int</span></li>
            <li> <span class="li-head">gateway</span> - Enable/disable SD-WAN service gateway. <span class="li-normal">type: str</span> <span class="li-normal">choices: enable, disable</span></li>
            <li> <span class="li-head">groups</span> - User groups. <span class="li-normal">type: list</span></li>
                <ul class="ul-self">
                <li> <span class="li-head">name</span> - Group name. Source user.group.name. <span class="li-normal">type: str</span> <span class="li-required">required: True</span></li>
                </ul>
            <li> <span class="li-head">health_check</span> - Health check. Source system.virtual-wan-link.health-check.name. <span class="li-normal">type: str</span></li>
            <li> <span class="li-head">hold_down_time</span> - Waiting period in seconds when switching from the back-up member to the primary member (0 - 10000000). <span class="li-normal">type: int</span></li>
            <li> <span class="li-head">id</span> - Priority rule ID (1 - 4000). <span class="li-normal">type: int</span> <span class="li-required">required: True</span></li>
            <li> <span class="li-head">input_device</span> - Source interface name. <span class="li-normal">type: list</span></li>
                <ul class="ul-self">
                <li> <span class="li-head">name</span> - Interface name. Source system.interface.name. <span class="li-normal">type: str</span> <span class="li-required">required: True</span></li>
                </ul>
            <li> <span class="li-head">internet_service</span> - Enable/disable use of Internet service for application-based load balancing. <span class="li-normal">type: str</span> <span class="li-normal">choices: enable, disable</span></li>
            <li> <span class="li-head">internet_service_app_ctrl</span> - Application control based Internet Service ID list. <span class="li-normal">type: list</span></li>
                <ul class="ul-self">
                <li> <span class="li-head">id</span> - Application control based Internet Service ID. <span class="li-normal">type: int</span> <span class="li-required">required: True</span></li>
                </ul>
            <li> <span class="li-head">internet_service_app_ctrl_group</span> - Application control based Internet Service group list. <span class="li-normal">type: list</span></li>
                <ul class="ul-self">
                <li> <span class="li-head">name</span> - Application control based Internet Service group name. Source application.group.name. <span class="li-normal">type: str</span> <span class="li-required">required: True</span></li>
                </ul>
            <li> <span class="li-head">internet_service_custom</span> - Custom Internet service name list. <span class="li-normal">type: list</span></li>
                <ul class="ul-self">
                <li> <span class="li-head">name</span> - Custom Internet service name. Source firewall.internet-service-custom.name. <span class="li-normal">type: str</span> <span class="li-required">required: True</span></li>
                </ul>
            <li> <span class="li-head">internet_service_custom_group</span> - Custom Internet Service group list. <span class="li-normal">type: list</span></li>
                <ul class="ul-self">
                <li> <span class="li-head">name</span> - Custom Internet Service group name. Source firewall.internet-service-custom-group.name. <span class="li-normal">type: str</span> <span class="li-required">required: True</span></li>
                </ul>
            <li> <span class="li-head">internet_service_group</span> - Internet Service group list. <span class="li-normal">type: list</span></li>
                <ul class="ul-self">
                <li> <span class="li-head">name</span> - Internet Service group name. Source firewall.internet-service-group.name. <span class="li-normal">type: str</span> <span class="li-required">required: True</span></li>
                </ul>
            <li> <span class="li-head">internet_service_id</span> - Internet service ID list. <span class="li-normal">type: list</span></li>
                <ul class="ul-self">
                <li> <span class="li-head">id</span> - Internet service ID. Source firewall.internet-service.id. <span class="li-normal">type: int</span> <span class="li-required">required: True</span></li>
                </ul>
            <li> <span class="li-head">jitter_weight</span> - Coefficient of jitter in the formula of custom-profile-1. <span class="li-normal">type: int</span></li>
            <li> <span class="li-head">latency_weight</span> - Coefficient of latency in the formula of custom-profile-1. <span class="li-normal">type: int</span></li>
            <li> <span class="li-head">link_cost_factor</span> - Link cost factor. <span class="li-normal">type: str</span> <span class="li-normal">choices: latency, jitter, packet-loss, inbandwidth, outbandwidth, bibandwidth, custom-profile-1</span></li>
            <li> <span class="li-head">link_cost_threshold</span> - Percentage threshold change of link cost values that will result in policy route regeneration (0 - 10000000). <span class="li-normal">type: int</span></li>
            <li> <span class="li-head">member</span> - Member sequence number. Source system.virtual-wan-link.members.seq-num. <span class="li-normal">type: int</span></li>
            <li> <span class="li-head">mode</span> - Control how the priority rule sets the priority of interfaces in the SD-WAN. <span class="li-normal">type: str</span> <span class="li-normal">choices: auto, manual, priority, sla, load-balance</span></li>
            <li> <span class="li-head">name</span> - Priority rule name. <span class="li-normal">type: str</span></li>
            <li> <span class="li-head">packet_loss_weight</span> - Coefficient of packet-loss in the formula of custom-profile-1. <span class="li-normal">type: int</span></li>
            <li> <span class="li-head">priority_members</span> - Member sequence number list. <span class="li-normal">type: list</span></li>
                <ul class="ul-self">
                <li> <span class="li-head">seq_num</span> - Member sequence number. Source system.virtual-wan-link.members.seq-num. <span class="li-normal">type: int</span></li>
                </ul>
            <li> <span class="li-head">protocol</span> - Protocol number. <span class="li-normal">type: int</span></li>
            <li> <span class="li-head">quality_link</span> - Quality grade. <span class="li-normal">type: int</span></li>
            <li> <span class="li-head">route_tag</span> - IPv4 route map route-tag. <span class="li-normal">type: int</span></li>
            <li> <span class="li-head">sla</span> - Service level agreement (SLA). <span class="li-normal">type: list</span></li>
                <ul class="ul-self">
                <li> <span class="li-head">health_check</span> - Virtual WAN Link health-check. Source system.virtual-wan-link.health-check.name. <span class="li-normal">type: str</span></li>
                <li> <span class="li-head">id</span> - SLA ID. <span class="li-normal">type: int</span></li>
                </ul>
            <li> <span class="li-head">src</span> - Source address name. <span class="li-normal">type: list</span></li>
                <ul class="ul-self">
                <li> <span class="li-head">name</span> - Address or address group name. Source firewall.address.name firewall.addrgrp.name. <span class="li-normal">type: str</span> <span class="li-required">required: True</span></li>
                </ul>
            <li> <span class="li-head">src_negate</span> - Enable/disable negation of source address match. <span class="li-normal">type: str</span> <span class="li-normal">choices: enable, disable</span></li>
            <li> <span class="li-head">src6</span> - Source address6 name. <span class="li-normal">type: list</span></li>
                <ul class="ul-self">
                <li> <span class="li-head">name</span> - Address6 or address6 group name. Source firewall.address6.name firewall.addrgrp6.name. <span class="li-normal">type: str</span> <span class="li-required">required: True</span></li>
                </ul>
            <li> <span class="li-head">start_port</span> - Start destination port number. <span class="li-normal">type: int</span></li>
            <li> <span class="li-head">status</span> - Enable/disable SD-WAN service. <span class="li-normal">type: str</span> <span class="li-normal">choices: enable, disable</span></li>
            <li> <span class="li-head">tos</span> - Type of service bit pattern. <span class="li-normal">type: str</span></li>
            <li> <span class="li-head">tos_mask</span> - Type of service evaluated bits. <span class="li-normal">type: str</span></li>
            <li> <span class="li-head">users</span> - User name. <span class="li-normal">type: list</span></li>
                <ul class="ul-self">
                <li> <span class="li-head">name</span> - User name. Source user.local.name. <span class="li-normal">type: str</span> <span class="li-required">required: True</span></li>
                </ul>
            </ul>
        <li> <span class="li-head">status</span> - Enable/disable SD-WAN. <span class="li-normal">type: str</span> <span class="li-normal">choices: disable, enable</span></li>
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
      - name: Configure redundant internet connections using SD-WAN (formerly virtual WAN link).
        fortios_system_virtual_wan_link:
          vdom:  "{{ vdom }}"
          system_virtual_wan_link:
            fail_alert_interfaces:
             -
                name: "default_name_4 (source system.interface.name)"
            fail_detect: "enable"
            health_check:
             -
                addr_mode: "ipv4"
                failtime: "8"
                http_agent: "<your_own_value>"
                http_get: "<your_own_value>"
                http_match: "<your_own_value>"
                internet_service_id: "12 (source firewall.internet-service.id)"
                interval: "13"
                members:
                 -
                    seq_num: "15 (source system.virtual-wan-link.members.seq-num)"
                name: "default_name_16"
                packet_size: "17"
                password: "<your_own_value>"
                port: "19"
                probe_packets: "disable"
                protocol: "ping"
                recoverytime: "22"
                security_mode: "none"
                server: "192.168.100.40"
                sla:
                 -
                    id:  "26"
                    jitter_threshold: "27"
                    latency_threshold: "28"
                    link_cost_factor: "latency"
                    packetloss_threshold: "30"
                sla_fail_log_period: "31"
                sla_pass_log_period: "32"
                threshold_alert_jitter: "33"
                threshold_alert_latency: "34"
                threshold_alert_packetloss: "35"
                threshold_warning_jitter: "36"
                threshold_warning_latency: "37"
                threshold_warning_packetloss: "38"
                update_cascade_interface: "enable"
                update_static_route: "enable"
            load_balance_mode: "source-ip-based"
            members:
             -
                comment: "Comments."
                cost: "44"
                gateway: "<your_own_value>"
                gateway6: "<your_own_value>"
                ingress_spillover_threshold: "47"
                interface: "<your_own_value> (source system.interface.name)"
                priority: "49"
                seq_num: "50"
                source: "<your_own_value>"
                source6: "<your_own_value>"
                spillover_threshold: "53"
                status: "disable"
                volume_ratio: "55"
                weight: "56"
            service:
             -
                addr_mode: "ipv4"
                bandwidth_weight: "59"
                default: "enable"
                dscp_forward: "enable"
                dscp_forward_tag: "<your_own_value>"
                dscp_reverse: "enable"
                dscp_reverse_tag: "<your_own_value>"
                dst:
                 -
                    name: "default_name_66 (source firewall.address.name firewall.addrgrp.name)"
                dst_negate: "enable"
                dst6:
                 -
                    name: "default_name_69 (source firewall.address6.name firewall.addrgrp6.name)"
                end_port: "70"
                gateway: "enable"
                groups:
                 -
                    name: "default_name_73 (source user.group.name)"
                health_check: "<your_own_value> (source system.virtual-wan-link.health-check.name)"
                hold_down_time: "75"
                id:  "76"
                input_device:
                 -
                    name: "default_name_78 (source system.interface.name)"
                internet_service: "enable"
                internet_service_app_ctrl:
                 -
                    id:  "81"
                internet_service_app_ctrl_group:
                 -
                    name: "default_name_83 (source application.group.name)"
                internet_service_custom:
                 -
                    name: "default_name_85 (source firewall.internet-service-custom.name)"
                internet_service_custom_group:
                 -
                    name: "default_name_87 (source firewall.internet-service-custom-group.name)"
                internet_service_group:
                 -
                    name: "default_name_89 (source firewall.internet-service-group.name)"
                internet_service_id:
                 -
                    id:  "91 (source firewall.internet-service.id)"
                jitter_weight: "92"
                latency_weight: "93"
                link_cost_factor: "latency"
                link_cost_threshold: "95"
                member: "96 (source system.virtual-wan-link.members.seq-num)"
                mode: "auto"
                name: "default_name_98"
                packet_loss_weight: "99"
                priority_members:
                 -
                    seq_num: "101 (source system.virtual-wan-link.members.seq-num)"
                protocol: "102"
                quality_link: "103"
                route_tag: "104"
                sla:
                 -
                    health_check: "<your_own_value> (source system.virtual-wan-link.health-check.name)"
                    id:  "107"
                src:
                 -
                    name: "default_name_109 (source firewall.address.name firewall.addrgrp.name)"
                src_negate: "enable"
                src6:
                 -
                    name: "default_name_112 (source firewall.address6.name firewall.addrgrp6.name)"
                start_port: "113"
                status: "enable"
                tos: "<your_own_value>"
                tos_mask: "<your_own_value>"
                users:
                 -
                    name: "default_name_118 (source user.local.name)"
            status: "disable"
    


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
