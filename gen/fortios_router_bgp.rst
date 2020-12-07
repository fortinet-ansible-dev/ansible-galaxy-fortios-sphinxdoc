:source: fortios_router_bgp.py

:orphan:

.. fortios_router_bgp:

fortios_router_bgp -- Configure BGP in Fortinet's FortiOS and FortiGate.
++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++

.. versionadded:: 2.8

.. contents::
   :local:
   :depth: 1


Synopsis
--------
- This module is able to configure a FortiGate or FortiOS (FOS) device by allowing the user to set and modify router feature and bgp category. Examples include all parameters and values need to be adjusted to datasources before usage. Tested with FOS v6.4.0



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
    <li> <span class="li-head">router_bgp</span> - Configure BGP. <span class="li-normal">type: dict</span></li>
        <ul class="ul-self">
        <li> <span class="li-head">additional_path</span> - Enable/disable selection of BGP IPv4 additional paths. <span class="li-normal">type: str</span> <span class="li-normal">choices: enable, disable</span></li>
        <li> <span class="li-head">additional_path_select</span> - Number of additional paths to be selected for each IPv4 NLRI. <span class="li-normal">type: int</span></li>
        <li> <span class="li-head">additional_path_select6</span> - Number of additional paths to be selected for each IPv6 NLRI. <span class="li-normal">type: int</span></li>
        <li> <span class="li-head">additional_path6</span> - Enable/disable selection of BGP IPv6 additional paths. <span class="li-normal">type: str</span> <span class="li-normal">choices: enable, disable</span></li>
        <li> <span class="li-head">admin_distance</span> - Administrative distance modifications. <span class="li-normal">type: list</span></li>
            <ul class="ul-self">
            <li> <span class="li-head">distance</span> - Administrative distance to apply (1 - 255). <span class="li-normal">type: int</span></li>
            <li> <span class="li-head">id</span> - ID. <span class="li-normal">type: int</span> <span class="li-required">required: True</span></li>
            <li> <span class="li-head">neighbour_prefix</span> - Neighbor address prefix. <span class="li-normal">type: str</span></li>
            <li> <span class="li-head">route_list</span> - Access list of routes to apply new distance to. Source router.access-list.name. <span class="li-normal">type: str</span></li>
            </ul>
        <li> <span class="li-head">aggregate_address</span> - BGP aggregate address table. <span class="li-normal">type: list</span></li>
            <ul class="ul-self">
            <li> <span class="li-head">as_set</span> - Enable/disable generate AS set path information. <span class="li-normal">type: str</span> <span class="li-normal">choices: enable, disable</span></li>
            <li> <span class="li-head">id</span> - ID. <span class="li-normal">type: int</span> <span class="li-required">required: True</span></li>
            <li> <span class="li-head">prefix</span> - Aggregate prefix. <span class="li-normal">type: str</span></li>
            <li> <span class="li-head">summary_only</span> - Enable/disable filter more specific routes from updates. <span class="li-normal">type: str</span> <span class="li-normal">choices: enable, disable</span></li>
            </ul>
        <li> <span class="li-head">aggregate_address6</span> - BGP IPv6 aggregate address table. <span class="li-normal">type: list</span></li>
            <ul class="ul-self">
            <li> <span class="li-head">as_set</span> - Enable/disable generate AS set path information. <span class="li-normal">type: str</span> <span class="li-normal">choices: enable, disable</span></li>
            <li> <span class="li-head">id</span> - ID. <span class="li-normal">type: int</span> <span class="li-required">required: True</span></li>
            <li> <span class="li-head">prefix6</span> - Aggregate IPv6 prefix. <span class="li-normal">type: str</span></li>
            <li> <span class="li-head">summary_only</span> - Enable/disable filter more specific routes from updates. <span class="li-normal">type: str</span> <span class="li-normal">choices: enable, disable</span></li>
            </ul>
        <li> <span class="li-head">always_compare_med</span> - Enable/disable always compare MED. <span class="li-normal">type: str</span> <span class="li-normal">choices: enable, disable</span></li>
        <li> <span class="li-head">as</span> - Router AS number, valid from 1 to 4294967295, 0 to disable BGP. <span class="li-normal">type: int</span></li>
        <li> <span class="li-head">bestpath_as_path_ignore</span> - Enable/disable ignore AS path. <span class="li-normal">type: str</span> <span class="li-normal">choices: enable, disable</span></li>
        <li> <span class="li-head">bestpath_cmp_confed_aspath</span> - Enable/disable compare federation AS path length. <span class="li-normal">type: str</span> <span class="li-normal">choices: enable, disable</span></li>
        <li> <span class="li-head">bestpath_cmp_routerid</span> - Enable/disable compare router ID for identical EBGP paths. <span class="li-normal">type: str</span> <span class="li-normal">choices: enable, disable</span></li>
        <li> <span class="li-head">bestpath_med_confed</span> - Enable/disable compare MED among confederation paths. <span class="li-normal">type: str</span> <span class="li-normal">choices: enable, disable</span></li>
        <li> <span class="li-head">bestpath_med_missing_as_worst</span> - Enable/disable treat missing MED as least preferred. <span class="li-normal">type: str</span> <span class="li-normal">choices: enable, disable</span></li>
        <li> <span class="li-head">client_to_client_reflection</span> - Enable/disable client-to-client route reflection. <span class="li-normal">type: str</span> <span class="li-normal">choices: enable, disable</span></li>
        <li> <span class="li-head">cluster_id</span> - Route reflector cluster ID. <span class="li-normal">type: str</span></li>
        <li> <span class="li-head">confederation_identifier</span> - Confederation identifier. <span class="li-normal">type: int</span></li>
        <li> <span class="li-head">confederation_peers</span> - Confederation peers. <span class="li-normal">type: list</span></li>
            <ul class="ul-self">
            <li> <span class="li-head">peer</span> - Peer ID. <span class="li-normal">type: str</span> <span class="li-required">required: True</span></li>
            </ul>
        <li> <span class="li-head">dampening</span> - Enable/disable route-flap dampening. <span class="li-normal">type: str</span> <span class="li-normal">choices: enable, disable</span></li>
        <li> <span class="li-head">dampening_max_suppress_time</span> - Maximum minutes a route can be suppressed. <span class="li-normal">type: int</span></li>
        <li> <span class="li-head">dampening_reachability_half_life</span> - Reachability half-life time for penalty (min). <span class="li-normal">type: int</span></li>
        <li> <span class="li-head">dampening_reuse</span> - Threshold to reuse routes. <span class="li-normal">type: int</span></li>
        <li> <span class="li-head">dampening_route_map</span> - Criteria for dampening. Source router.route-map.name. <span class="li-normal">type: str</span></li>
        <li> <span class="li-head">dampening_suppress</span> - Threshold to suppress routes. <span class="li-normal">type: int</span></li>
        <li> <span class="li-head">dampening_unreachability_half_life</span> - Unreachability half-life time for penalty (min). <span class="li-normal">type: int</span></li>
        <li> <span class="li-head">default_local_preference</span> - Default local preference. <span class="li-normal">type: int</span></li>
        <li> <span class="li-head">deterministic_med</span> - Enable/disable enforce deterministic comparison of MED. <span class="li-normal">type: str</span> <span class="li-normal">choices: enable, disable</span></li>
        <li> <span class="li-head">distance_external</span> - Distance for routes external to the AS. <span class="li-normal">type: int</span></li>
        <li> <span class="li-head">distance_internal</span> - Distance for routes internal to the AS. <span class="li-normal">type: int</span></li>
        <li> <span class="li-head">distance_local</span> - Distance for routes local to the AS. <span class="li-normal">type: int</span></li>
        <li> <span class="li-head">ebgp_multipath</span> - Enable/disable EBGP multi-path. <span class="li-normal">type: str</span> <span class="li-normal">choices: enable, disable</span></li>
        <li> <span class="li-head">enforce_first_as</span> - Enable/disable enforce first AS for EBGP routes. <span class="li-normal">type: str</span> <span class="li-normal">choices: enable, disable</span></li>
        <li> <span class="li-head">fast_external_failover</span> - Enable/disable reset peer BGP session if link goes down. <span class="li-normal">type: str</span> <span class="li-normal">choices: enable, disable</span></li>
        <li> <span class="li-head">graceful_end_on_timer</span> - Enable/disable to exit graceful restart on timer only. <span class="li-normal">type: str</span> <span class="li-normal">choices: enable, disable</span></li>
        <li> <span class="li-head">graceful_restart</span> - Enable/disable BGP graceful restart capabilities. <span class="li-normal">type: str</span> <span class="li-normal">choices: enable, disable</span></li>
        <li> <span class="li-head">graceful_restart_time</span> - Time needed for neighbors to restart (sec). <span class="li-normal">type: int</span></li>
        <li> <span class="li-head">graceful_stalepath_time</span> - Time to hold stale paths of restarting neighbor (sec). <span class="li-normal">type: int</span></li>
        <li> <span class="li-head">graceful_update_delay</span> - Route advertisement/selection delay after restart (sec). <span class="li-normal">type: int</span></li>
        <li> <span class="li-head">holdtime_timer</span> - Number of seconds to mark peer as dead. <span class="li-normal">type: int</span></li>
        <li> <span class="li-head">ibgp_multipath</span> - Enable/disable IBGP multi-path. <span class="li-normal">type: str</span> <span class="li-normal">choices: enable, disable</span></li>
        <li> <span class="li-head">ignore_optional_capability</span> - Don"t send unknown optional capability notification message <span class="li-normal">type: str</span> <span class="li-normal">choices: enable, disable</span></li>
        <li> <span class="li-head">keepalive_timer</span> - Frequency to send keep alive requests. <span class="li-normal">type: int</span></li>
        <li> <span class="li-head">log_neighbour_changes</span> - Enable logging of BGP neighbour"s changes <span class="li-normal">type: str</span> <span class="li-normal">choices: enable, disable</span></li>
        <li> <span class="li-head">neighbor</span> - BGP neighbor table. <span class="li-normal">type: list</span></li>
            <ul class="ul-self">
            <li> <span class="li-head">activate</span> - Enable/disable address family IPv4 for this neighbor. <span class="li-normal">type: str</span> <span class="li-normal">choices: enable, disable</span></li>
            <li> <span class="li-head">activate6</span> - Enable/disable address family IPv6 for this neighbor. <span class="li-normal">type: str</span> <span class="li-normal">choices: enable, disable</span></li>
            <li> <span class="li-head">additional_path</span> - Enable/disable IPv4 additional-path capability. <span class="li-normal">type: str</span> <span class="li-normal">choices: send, receive, both, disable</span></li>
            <li> <span class="li-head">additional_path6</span> - Enable/disable IPv6 additional-path capability. <span class="li-normal">type: str</span> <span class="li-normal">choices: send, receive, both, disable</span></li>
            <li> <span class="li-head">adv_additional_path</span> - Number of IPv4 additional paths that can be advertised to this neighbor. <span class="li-normal">type: int</span></li>
            <li> <span class="li-head">adv_additional_path6</span> - Number of IPv6 additional paths that can be advertised to this neighbor. <span class="li-normal">type: int</span></li>
            <li> <span class="li-head">advertisement_interval</span> - Minimum interval (sec) between sending updates. <span class="li-normal">type: int</span></li>
            <li> <span class="li-head">allowas_in</span> - IPv4 The maximum number of occurrence of my AS number allowed. <span class="li-normal">type: int</span></li>
            <li> <span class="li-head">allowas_in_enable</span> - Enable/disable IPv4 Enable to allow my AS in AS path. <span class="li-normal">type: str</span> <span class="li-normal">choices: enable, disable</span></li>
            <li> <span class="li-head">allowas_in_enable6</span> - Enable/disable IPv6 Enable to allow my AS in AS path. <span class="li-normal">type: str</span> <span class="li-normal">choices: enable, disable</span></li>
            <li> <span class="li-head">allowas_in6</span> - IPv6 The maximum number of occurrence of my AS number allowed. <span class="li-normal">type: int</span></li>
            <li> <span class="li-head">as_override</span> - Enable/disable replace peer AS with own AS for IPv4. <span class="li-normal">type: str</span> <span class="li-normal">choices: enable, disable</span></li>
            <li> <span class="li-head">as_override6</span> - Enable/disable replace peer AS with own AS for IPv6. <span class="li-normal">type: str</span> <span class="li-normal">choices: enable, disable</span></li>
            <li> <span class="li-head">attribute_unchanged</span> - IPv4 List of attributes that should be unchanged. <span class="li-normal">type: str</span> <span class="li-normal">choices: as-path, med, next-hop</span></li>
            <li> <span class="li-head">attribute_unchanged6</span> - IPv6 List of attributes that should be unchanged. <span class="li-normal">type: str</span> <span class="li-normal">choices: as-path, med, next-hop</span></li>
            <li> <span class="li-head">bfd</span> - Enable/disable BFD for this neighbor. <span class="li-normal">type: str</span> <span class="li-normal">choices: enable, disable</span></li>
            <li> <span class="li-head">capability_default_originate</span> - Enable/disable advertise default IPv4 route to this neighbor. <span class="li-normal">type: str</span> <span class="li-normal">choices: enable, disable</span></li>
            <li> <span class="li-head">capability_default_originate6</span> - Enable/disable advertise default IPv6 route to this neighbor. <span class="li-normal">type: str</span> <span class="li-normal">choices: enable, disable</span></li>
            <li> <span class="li-head">capability_dynamic</span> - Enable/disable advertise dynamic capability to this neighbor. <span class="li-normal">type: str</span> <span class="li-normal">choices: enable, disable</span></li>
            <li> <span class="li-head">capability_graceful_restart</span> - Enable/disable advertise IPv4 graceful restart capability to this neighbor. <span class="li-normal">type: str</span> <span class="li-normal">choices: enable, disable</span></li>
            <li> <span class="li-head">capability_graceful_restart6</span> - Enable/disable advertise IPv6 graceful restart capability to this neighbor. <span class="li-normal">type: str</span> <span class="li-normal">choices: enable, disable</span></li>
            <li> <span class="li-head">capability_orf</span> - Accept/Send IPv4 ORF lists to/from this neighbor. <span class="li-normal">type: str</span> <span class="li-normal">choices: none, receive, send, both</span></li>
            <li> <span class="li-head">capability_orf6</span> - Accept/Send IPv6 ORF lists to/from this neighbor. <span class="li-normal">type: str</span> <span class="li-normal">choices: none, receive, send, both</span></li>
            <li> <span class="li-head">capability_route_refresh</span> - Enable/disable advertise route refresh capability to this neighbor. <span class="li-normal">type: str</span> <span class="li-normal">choices: enable, disable</span></li>
            <li> <span class="li-head">conditional_advertise</span> - Conditional advertisement. <span class="li-normal">type: list</span></li>
                <ul class="ul-self">
                <li> <span class="li-head">advertise_routemap</span> - Name of advertising route map. Source router.route-map.name. <span class="li-normal">type: str</span></li>
                <li> <span class="li-head">condition_routemap</span> - Name of condition route map. Source router.route-map.name. <span class="li-normal">type: str</span></li>
                <li> <span class="li-head">condition_type</span> - Type of condition. <span class="li-normal">type: str</span> <span class="li-normal">choices: exist, non-exist</span></li>
                </ul>
            <li> <span class="li-head">connect_timer</span> - Interval (sec) for connect timer. <span class="li-normal">type: int</span></li>
            <li> <span class="li-head">default_originate_routemap</span> - Route map to specify criteria to originate IPv4 default. Source router.route-map.name. <span class="li-normal">type: str</span></li>
            <li> <span class="li-head">default_originate_routemap6</span> - Route map to specify criteria to originate IPv6 default. Source router.route-map.name. <span class="li-normal">type: str</span></li>
            <li> <span class="li-head">description</span> - Description. <span class="li-normal">type: str</span></li>
            <li> <span class="li-head">distribute_list_in</span> - Filter for IPv4 updates from this neighbor. Source router.access-list.name. <span class="li-normal">type: str</span></li>
            <li> <span class="li-head">distribute_list_in6</span> - Filter for IPv6 updates from this neighbor. Source router.access-list6.name. <span class="li-normal">type: str</span></li>
            <li> <span class="li-head">distribute_list_out</span> - Filter for IPv4 updates to this neighbor. Source router.access-list.name. <span class="li-normal">type: str</span></li>
            <li> <span class="li-head">distribute_list_out6</span> - Filter for IPv6 updates to this neighbor. Source router.access-list6.name. <span class="li-normal">type: str</span></li>
            <li> <span class="li-head">dont_capability_negotiate</span> - Don"t negotiate capabilities with this neighbor <span class="li-normal">type: str</span> <span class="li-normal">choices: enable, disable</span></li>
            <li> <span class="li-head">ebgp_enforce_multihop</span> - Enable/disable allow multi-hop EBGP neighbors. <span class="li-normal">type: str</span> <span class="li-normal">choices: enable, disable</span></li>
            <li> <span class="li-head">ebgp_multihop_ttl</span> - EBGP multihop TTL for this peer. <span class="li-normal">type: int</span></li>
            <li> <span class="li-head">filter_list_in</span> - BGP filter for IPv4 inbound routes. Source router.aspath-list.name. <span class="li-normal">type: str</span></li>
            <li> <span class="li-head">filter_list_in6</span> - BGP filter for IPv6 inbound routes. Source router.aspath-list.name. <span class="li-normal">type: str</span></li>
            <li> <span class="li-head">filter_list_out</span> - BGP filter for IPv4 outbound routes. Source router.aspath-list.name. <span class="li-normal">type: str</span></li>
            <li> <span class="li-head">filter_list_out6</span> - BGP filter for IPv6 outbound routes. Source router.aspath-list.name. <span class="li-normal">type: str</span></li>
            <li> <span class="li-head">holdtime_timer</span> - Interval (sec) before peer considered dead. <span class="li-normal">type: int</span></li>
            <li> <span class="li-head">interface</span> - Specify outgoing interface for peer connection. For IPv6 peer, the interface should have link-local address. Source system .interface.name. <span class="li-normal">type: str</span></li>
            <li> <span class="li-head">ip</span> - IP/IPv6 address of neighbor. <span class="li-normal">type: str</span> <span class="li-required">required: True</span></li>
            <li> <span class="li-head">keep_alive_timer</span> - Keep alive timer interval (sec). <span class="li-normal">type: int</span></li>
            <li> <span class="li-head">link_down_failover</span> - Enable/disable failover upon link down. <span class="li-normal">type: str</span> <span class="li-normal">choices: enable, disable</span></li>
            <li> <span class="li-head">local_as</span> - Local AS number of neighbor. <span class="li-normal">type: int</span></li>
            <li> <span class="li-head">local_as_no_prepend</span> - Do not prepend local-as to incoming updates. <span class="li-normal">type: str</span> <span class="li-normal">choices: enable, disable</span></li>
            <li> <span class="li-head">local_as_replace_as</span> - Replace real AS with local-as in outgoing updates. <span class="li-normal">type: str</span> <span class="li-normal">choices: enable, disable</span></li>
            <li> <span class="li-head">maximum_prefix</span> - Maximum number of IPv4 prefixes to accept from this peer. <span class="li-normal">type: int</span></li>
            <li> <span class="li-head">maximum_prefix_threshold</span> - Maximum IPv4 prefix threshold value (1 - 100 percent). <span class="li-normal">type: int</span></li>
            <li> <span class="li-head">maximum_prefix_threshold6</span> - Maximum IPv6 prefix threshold value (1 - 100 percent). <span class="li-normal">type: int</span></li>
            <li> <span class="li-head">maximum_prefix_warning_only</span> - Enable/disable IPv4 Only give warning message when limit is exceeded. <span class="li-normal">type: str</span> <span class="li-normal">choices: enable, disable</span></li>
            <li> <span class="li-head">maximum_prefix_warning_only6</span> - Enable/disable IPv6 Only give warning message when limit is exceeded. <span class="li-normal">type: str</span> <span class="li-normal">choices: enable, disable</span></li>
            <li> <span class="li-head">maximum_prefix6</span> - Maximum number of IPv6 prefixes to accept from this peer. <span class="li-normal">type: int</span></li>
            <li> <span class="li-head">next_hop_self</span> - Enable/disable IPv4 next-hop calculation for this neighbor. <span class="li-normal">type: str</span> <span class="li-normal">choices: enable, disable</span></li>
            <li> <span class="li-head">next_hop_self6</span> - Enable/disable IPv6 next-hop calculation for this neighbor. <span class="li-normal">type: str</span> <span class="li-normal">choices: enable, disable</span></li>
            <li> <span class="li-head">override_capability</span> - Enable/disable override result of capability negotiation. <span class="li-normal">type: str</span> <span class="li-normal">choices: enable, disable</span></li>
            <li> <span class="li-head">passive</span> - Enable/disable sending of open messages to this neighbor. <span class="li-normal">type: str</span> <span class="li-normal">choices: enable, disable</span></li>
            <li> <span class="li-head">password</span> - Password used in MD5 authentication. <span class="li-normal">type: str</span></li>
            <li> <span class="li-head">prefix_list_in</span> - IPv4 Inbound filter for updates from this neighbor. Source router.prefix-list.name. <span class="li-normal">type: str</span></li>
            <li> <span class="li-head">prefix_list_in6</span> - IPv6 Inbound filter for updates from this neighbor. Source router.prefix-list6.name. <span class="li-normal">type: str</span></li>
            <li> <span class="li-head">prefix_list_out</span> - IPv4 Outbound filter for updates to this neighbor. Source router.prefix-list.name. <span class="li-normal">type: str</span></li>
            <li> <span class="li-head">prefix_list_out6</span> - IPv6 Outbound filter for updates to this neighbor. Source router.prefix-list6.name. <span class="li-normal">type: str</span></li>
            <li> <span class="li-head">remote_as</span> - AS number of neighbor. <span class="li-normal">type: int</span></li>
            <li> <span class="li-head">remove_private_as</span> - Enable/disable remove private AS number from IPv4 outbound updates. <span class="li-normal">type: str</span> <span class="li-normal">choices: enable, disable</span></li>
            <li> <span class="li-head">remove_private_as6</span> - Enable/disable remove private AS number from IPv6 outbound updates. <span class="li-normal">type: str</span> <span class="li-normal">choices: enable, disable</span></li>
            <li> <span class="li-head">restart_time</span> - Graceful restart delay time (sec, 0 = global default). <span class="li-normal">type: int</span></li>
            <li> <span class="li-head">retain_stale_time</span> - Time to retain stale routes. <span class="li-normal">type: int</span></li>
            <li> <span class="li-head">route_map_in</span> - IPv4 Inbound route map filter. Source router.route-map.name. <span class="li-normal">type: str</span></li>
            <li> <span class="li-head">route_map_in6</span> - IPv6 Inbound route map filter. Source router.route-map.name. <span class="li-normal">type: str</span></li>
            <li> <span class="li-head">route_map_out</span> - IPv4 outbound route map filter. Source router.route-map.name. <span class="li-normal">type: str</span></li>
            <li> <span class="li-head">route_map_out_preferable</span> - IPv4 outbound route map filter if the peer is preferred. Source router.route-map.name. <span class="li-normal">type: str</span></li>
            <li> <span class="li-head">route_map_out6</span> - IPv6 Outbound route map filter. Source router.route-map.name. <span class="li-normal">type: str</span></li>
            <li> <span class="li-head">route_map_out6_preferable</span> - IPv6 outbound route map filter if the peer is preferred. Source router.route-map.name. <span class="li-normal">type: str</span></li>
            <li> <span class="li-head">route_reflector_client</span> - Enable/disable IPv4 AS route reflector client. <span class="li-normal">type: str</span> <span class="li-normal">choices: enable, disable</span></li>
            <li> <span class="li-head">route_reflector_client6</span> - Enable/disable IPv6 AS route reflector client. <span class="li-normal">type: str</span> <span class="li-normal">choices: enable, disable</span></li>
            <li> <span class="li-head">route_server_client</span> - Enable/disable IPv4 AS route server client. <span class="li-normal">type: str</span> <span class="li-normal">choices: enable, disable</span></li>
            <li> <span class="li-head">route_server_client6</span> - Enable/disable IPv6 AS route server client. <span class="li-normal">type: str</span> <span class="li-normal">choices: enable, disable</span></li>
            <li> <span class="li-head">send_community</span> - IPv4 Send community attribute to neighbor. <span class="li-normal">type: str</span> <span class="li-normal">choices: standard, extended, both, disable</span></li>
            <li> <span class="li-head">send_community6</span> - IPv6 Send community attribute to neighbor. <span class="li-normal">type: str</span> <span class="li-normal">choices: standard, extended, both, disable</span></li>
            <li> <span class="li-head">shutdown</span> - Enable/disable shutdown this neighbor. <span class="li-normal">type: str</span> <span class="li-normal">choices: enable, disable</span></li>
            <li> <span class="li-head">soft_reconfiguration</span> - Enable/disable allow IPv4 inbound soft reconfiguration. <span class="li-normal">type: str</span> <span class="li-normal">choices: enable, disable</span></li>
            <li> <span class="li-head">soft_reconfiguration6</span> - Enable/disable allow IPv6 inbound soft reconfiguration. <span class="li-normal">type: str</span> <span class="li-normal">choices: enable, disable</span></li>
            <li> <span class="li-head">stale_route</span> - Enable/disable stale route after neighbor down. <span class="li-normal">type: str</span> <span class="li-normal">choices: enable, disable</span></li>
            <li> <span class="li-head">strict_capability_match</span> - Enable/disable strict capability matching. <span class="li-normal">type: str</span> <span class="li-normal">choices: enable, disable</span></li>
            <li> <span class="li-head">unsuppress_map</span> - IPv4 Route map to selectively unsuppress suppressed routes. Source router.route-map.name. <span class="li-normal">type: str</span></li>
            <li> <span class="li-head">unsuppress_map6</span> - IPv6 Route map to selectively unsuppress suppressed routes. Source router.route-map.name. <span class="li-normal">type: str</span></li>
            <li> <span class="li-head">update_source</span> - Interface to use as source IP/IPv6 address of TCP connections. Source system.interface.name. <span class="li-normal">type: str</span></li>
            <li> <span class="li-head">weight</span> - Neighbor weight. <span class="li-normal">type: int</span></li>
            </ul>
        <li> <span class="li-head">neighbor_group</span> - BGP neighbor group table. <span class="li-normal">type: list</span></li>
            <ul class="ul-self">
            <li> <span class="li-head">activate</span> - Enable/disable address family IPv4 for this neighbor. <span class="li-normal">type: str</span> <span class="li-normal">choices: enable, disable</span></li>
            <li> <span class="li-head">activate6</span> - Enable/disable address family IPv6 for this neighbor. <span class="li-normal">type: str</span> <span class="li-normal">choices: enable, disable</span></li>
            <li> <span class="li-head">additional_path</span> - Enable/disable IPv4 additional-path capability. <span class="li-normal">type: str</span> <span class="li-normal">choices: send, receive, both, disable</span></li>
            <li> <span class="li-head">additional_path6</span> - Enable/disable IPv6 additional-path capability. <span class="li-normal">type: str</span> <span class="li-normal">choices: send, receive, both, disable</span></li>
            <li> <span class="li-head">adv_additional_path</span> - Number of IPv4 additional paths that can be advertised to this neighbor. <span class="li-normal">type: int</span></li>
            <li> <span class="li-head">adv_additional_path6</span> - Number of IPv6 additional paths that can be advertised to this neighbor. <span class="li-normal">type: int</span></li>
            <li> <span class="li-head">advertisement_interval</span> - Minimum interval (sec) between sending updates. <span class="li-normal">type: int</span></li>
            <li> <span class="li-head">allowas_in</span> - IPv4 The maximum number of occurrence of my AS number allowed. <span class="li-normal">type: int</span></li>
            <li> <span class="li-head">allowas_in_enable</span> - Enable/disable IPv4 Enable to allow my AS in AS path. <span class="li-normal">type: str</span> <span class="li-normal">choices: enable, disable</span></li>
            <li> <span class="li-head">allowas_in_enable6</span> - Enable/disable IPv6 Enable to allow my AS in AS path. <span class="li-normal">type: str</span> <span class="li-normal">choices: enable, disable</span></li>
            <li> <span class="li-head">allowas_in6</span> - IPv6 The maximum number of occurrence of my AS number allowed. <span class="li-normal">type: int</span></li>
            <li> <span class="li-head">as_override</span> - Enable/disable replace peer AS with own AS for IPv4. <span class="li-normal">type: str</span> <span class="li-normal">choices: enable, disable</span></li>
            <li> <span class="li-head">as_override6</span> - Enable/disable replace peer AS with own AS for IPv6. <span class="li-normal">type: str</span> <span class="li-normal">choices: enable, disable</span></li>
            <li> <span class="li-head">attribute_unchanged</span> - IPv4 List of attributes that should be unchanged. <span class="li-normal">type: str</span> <span class="li-normal">choices: as-path, med, next-hop</span></li>
            <li> <span class="li-head">attribute_unchanged6</span> - IPv6 List of attributes that should be unchanged. <span class="li-normal">type: str</span> <span class="li-normal">choices: as-path, med, next-hop</span></li>
            <li> <span class="li-head">bfd</span> - Enable/disable BFD for this neighbor. <span class="li-normal">type: str</span> <span class="li-normal">choices: enable, disable</span></li>
            <li> <span class="li-head">capability_default_originate</span> - Enable/disable advertise default IPv4 route to this neighbor. <span class="li-normal">type: str</span> <span class="li-normal">choices: enable, disable</span></li>
            <li> <span class="li-head">capability_default_originate6</span> - Enable/disable advertise default IPv6 route to this neighbor. <span class="li-normal">type: str</span> <span class="li-normal">choices: enable, disable</span></li>
            <li> <span class="li-head">capability_dynamic</span> - Enable/disable advertise dynamic capability to this neighbor. <span class="li-normal">type: str</span> <span class="li-normal">choices: enable, disable</span></li>
            <li> <span class="li-head">capability_graceful_restart</span> - Enable/disable advertise IPv4 graceful restart capability to this neighbor. <span class="li-normal">type: str</span> <span class="li-normal">choices: enable, disable</span></li>
            <li> <span class="li-head">capability_graceful_restart6</span> - Enable/disable advertise IPv6 graceful restart capability to this neighbor. <span class="li-normal">type: str</span> <span class="li-normal">choices: enable, disable</span></li>
            <li> <span class="li-head">capability_orf</span> - Accept/Send IPv4 ORF lists to/from this neighbor. <span class="li-normal">type: str</span> <span class="li-normal">choices: none, receive, send, both</span></li>
            <li> <span class="li-head">capability_orf6</span> - Accept/Send IPv6 ORF lists to/from this neighbor. <span class="li-normal">type: str</span> <span class="li-normal">choices: none, receive, send, both</span></li>
            <li> <span class="li-head">capability_route_refresh</span> - Enable/disable advertise route refresh capability to this neighbor. <span class="li-normal">type: str</span> <span class="li-normal">choices: enable, disable</span></li>
            <li> <span class="li-head">connect_timer</span> - Interval (sec) for connect timer. <span class="li-normal">type: int</span></li>
            <li> <span class="li-head">default_originate_routemap</span> - Route map to specify criteria to originate IPv4 default. Source router.route-map.name. <span class="li-normal">type: str</span></li>
            <li> <span class="li-head">default_originate_routemap6</span> - Route map to specify criteria to originate IPv6 default. Source router.route-map.name. <span class="li-normal">type: str</span></li>
            <li> <span class="li-head">description</span> - Description. <span class="li-normal">type: str</span></li>
            <li> <span class="li-head">distribute_list_in</span> - Filter for IPv4 updates from this neighbor. Source router.access-list.name. <span class="li-normal">type: str</span></li>
            <li> <span class="li-head">distribute_list_in6</span> - Filter for IPv6 updates from this neighbor. Source router.access-list6.name. <span class="li-normal">type: str</span></li>
            <li> <span class="li-head">distribute_list_out</span> - Filter for IPv4 updates to this neighbor. Source router.access-list.name. <span class="li-normal">type: str</span></li>
            <li> <span class="li-head">distribute_list_out6</span> - Filter for IPv6 updates to this neighbor. Source router.access-list6.name. <span class="li-normal">type: str</span></li>
            <li> <span class="li-head">dont_capability_negotiate</span> - Don"t negotiate capabilities with this neighbor <span class="li-normal">type: str</span> <span class="li-normal">choices: enable, disable</span></li>
            <li> <span class="li-head">ebgp_enforce_multihop</span> - Enable/disable allow multi-hop EBGP neighbors. <span class="li-normal">type: str</span> <span class="li-normal">choices: enable, disable</span></li>
            <li> <span class="li-head">ebgp_multihop_ttl</span> - EBGP multihop TTL for this peer. <span class="li-normal">type: int</span></li>
            <li> <span class="li-head">filter_list_in</span> - BGP filter for IPv4 inbound routes. Source router.aspath-list.name. <span class="li-normal">type: str</span></li>
            <li> <span class="li-head">filter_list_in6</span> - BGP filter for IPv6 inbound routes. Source router.aspath-list.name. <span class="li-normal">type: str</span></li>
            <li> <span class="li-head">filter_list_out</span> - BGP filter for IPv4 outbound routes. Source router.aspath-list.name. <span class="li-normal">type: str</span></li>
            <li> <span class="li-head">filter_list_out6</span> - BGP filter for IPv6 outbound routes. Source router.aspath-list.name. <span class="li-normal">type: str</span></li>
            <li> <span class="li-head">holdtime_timer</span> - Interval (sec) before peer considered dead. <span class="li-normal">type: int</span></li>
            <li> <span class="li-head">interface</span> - Specify outgoing interface for peer connection. For IPv6 peer, the interface should have link-local address. Source system .interface.name. <span class="li-normal">type: str</span></li>
            <li> <span class="li-head">keep_alive_timer</span> - Keep alive timer interval (sec). <span class="li-normal">type: int</span></li>
            <li> <span class="li-head">link_down_failover</span> - Enable/disable failover upon link down. <span class="li-normal">type: str</span> <span class="li-normal">choices: enable, disable</span></li>
            <li> <span class="li-head">local_as</span> - Local AS number of neighbor. <span class="li-normal">type: int</span></li>
            <li> <span class="li-head">local_as_no_prepend</span> - Do not prepend local-as to incoming updates. <span class="li-normal">type: str</span> <span class="li-normal">choices: enable, disable</span></li>
            <li> <span class="li-head">local_as_replace_as</span> - Replace real AS with local-as in outgoing updates. <span class="li-normal">type: str</span> <span class="li-normal">choices: enable, disable</span></li>
            <li> <span class="li-head">maximum_prefix</span> - Maximum number of IPv4 prefixes to accept from this peer. <span class="li-normal">type: int</span></li>
            <li> <span class="li-head">maximum_prefix_threshold</span> - Maximum IPv4 prefix threshold value (1 - 100 percent). <span class="li-normal">type: int</span></li>
            <li> <span class="li-head">maximum_prefix_threshold6</span> - Maximum IPv6 prefix threshold value (1 - 100 percent). <span class="li-normal">type: int</span></li>
            <li> <span class="li-head">maximum_prefix_warning_only</span> - Enable/disable IPv4 Only give warning message when limit is exceeded. <span class="li-normal">type: str</span> <span class="li-normal">choices: enable, disable</span></li>
            <li> <span class="li-head">maximum_prefix_warning_only6</span> - Enable/disable IPv6 Only give warning message when limit is exceeded. <span class="li-normal">type: str</span> <span class="li-normal">choices: enable, disable</span></li>
            <li> <span class="li-head">maximum_prefix6</span> - Maximum number of IPv6 prefixes to accept from this peer. <span class="li-normal">type: int</span></li>
            <li> <span class="li-head">name</span> - Neighbor group name. <span class="li-normal">type: str</span> <span class="li-required">required: True</span></li>
            <li> <span class="li-head">next_hop_self</span> - Enable/disable IPv4 next-hop calculation for this neighbor. <span class="li-normal">type: str</span> <span class="li-normal">choices: enable, disable</span></li>
            <li> <span class="li-head">next_hop_self6</span> - Enable/disable IPv6 next-hop calculation for this neighbor. <span class="li-normal">type: str</span> <span class="li-normal">choices: enable, disable</span></li>
            <li> <span class="li-head">override_capability</span> - Enable/disable override result of capability negotiation. <span class="li-normal">type: str</span> <span class="li-normal">choices: enable, disable</span></li>
            <li> <span class="li-head">passive</span> - Enable/disable sending of open messages to this neighbor. <span class="li-normal">type: str</span> <span class="li-normal">choices: enable, disable</span></li>
            <li> <span class="li-head">prefix_list_in</span> - IPv4 Inbound filter for updates from this neighbor. Source router.prefix-list.name. <span class="li-normal">type: str</span></li>
            <li> <span class="li-head">prefix_list_in6</span> - IPv6 Inbound filter for updates from this neighbor. Source router.prefix-list6.name. <span class="li-normal">type: str</span></li>
            <li> <span class="li-head">prefix_list_out</span> - IPv4 Outbound filter for updates to this neighbor. Source router.prefix-list.name. <span class="li-normal">type: str</span></li>
            <li> <span class="li-head">prefix_list_out6</span> - IPv6 Outbound filter for updates to this neighbor. Source router.prefix-list6.name. <span class="li-normal">type: str</span></li>
            <li> <span class="li-head">remote_as</span> - AS number of neighbor. <span class="li-normal">type: int</span></li>
            <li> <span class="li-head">remove_private_as</span> - Enable/disable remove private AS number from IPv4 outbound updates. <span class="li-normal">type: str</span> <span class="li-normal">choices: enable, disable</span></li>
            <li> <span class="li-head">remove_private_as6</span> - Enable/disable remove private AS number from IPv6 outbound updates. <span class="li-normal">type: str</span> <span class="li-normal">choices: enable, disable</span></li>
            <li> <span class="li-head">restart_time</span> - Graceful restart delay time (sec, 0 = global default). <span class="li-normal">type: int</span></li>
            <li> <span class="li-head">retain_stale_time</span> - Time to retain stale routes. <span class="li-normal">type: int</span></li>
            <li> <span class="li-head">route_map_in</span> - IPv4 Inbound route map filter. Source router.route-map.name. <span class="li-normal">type: str</span></li>
            <li> <span class="li-head">route_map_in6</span> - IPv6 Inbound route map filter. Source router.route-map.name. <span class="li-normal">type: str</span></li>
            <li> <span class="li-head">route_map_out</span> - IPv4 outbound route map filter. Source router.route-map.name. <span class="li-normal">type: str</span></li>
            <li> <span class="li-head">route_map_out_preferable</span> - IPv4 outbound route map filter if the peer is preferred. Source router.route-map.name. <span class="li-normal">type: str</span></li>
            <li> <span class="li-head">route_map_out6</span> - IPv6 Outbound route map filter. Source router.route-map.name. <span class="li-normal">type: str</span></li>
            <li> <span class="li-head">route_map_out6_preferable</span> - IPv6 outbound route map filter if the peer is preferred. Source router.route-map.name. <span class="li-normal">type: str</span></li>
            <li> <span class="li-head">route_reflector_client</span> - Enable/disable IPv4 AS route reflector client. <span class="li-normal">type: str</span> <span class="li-normal">choices: enable, disable</span></li>
            <li> <span class="li-head">route_reflector_client6</span> - Enable/disable IPv6 AS route reflector client. <span class="li-normal">type: str</span> <span class="li-normal">choices: enable, disable</span></li>
            <li> <span class="li-head">route_server_client</span> - Enable/disable IPv4 AS route server client. <span class="li-normal">type: str</span> <span class="li-normal">choices: enable, disable</span></li>
            <li> <span class="li-head">route_server_client6</span> - Enable/disable IPv6 AS route server client. <span class="li-normal">type: str</span> <span class="li-normal">choices: enable, disable</span></li>
            <li> <span class="li-head">send_community</span> - IPv4 Send community attribute to neighbor. <span class="li-normal">type: str</span> <span class="li-normal">choices: standard, extended, both, disable</span></li>
            <li> <span class="li-head">send_community6</span> - IPv6 Send community attribute to neighbor. <span class="li-normal">type: str</span> <span class="li-normal">choices: standard, extended, both, disable</span></li>
            <li> <span class="li-head">shutdown</span> - Enable/disable shutdown this neighbor. <span class="li-normal">type: str</span> <span class="li-normal">choices: enable, disable</span></li>
            <li> <span class="li-head">soft_reconfiguration</span> - Enable/disable allow IPv4 inbound soft reconfiguration. <span class="li-normal">type: str</span> <span class="li-normal">choices: enable, disable</span></li>
            <li> <span class="li-head">soft_reconfiguration6</span> - Enable/disable allow IPv6 inbound soft reconfiguration. <span class="li-normal">type: str</span> <span class="li-normal">choices: enable, disable</span></li>
            <li> <span class="li-head">stale_route</span> - Enable/disable stale route after neighbor down. <span class="li-normal">type: str</span> <span class="li-normal">choices: enable, disable</span></li>
            <li> <span class="li-head">strict_capability_match</span> - Enable/disable strict capability matching. <span class="li-normal">type: str</span> <span class="li-normal">choices: enable, disable</span></li>
            <li> <span class="li-head">unsuppress_map</span> - IPv4 Route map to selectively unsuppress suppressed routes. Source router.route-map.name. <span class="li-normal">type: str</span></li>
            <li> <span class="li-head">unsuppress_map6</span> - IPv6 Route map to selectively unsuppress suppressed routes. Source router.route-map.name. <span class="li-normal">type: str</span></li>
            <li> <span class="li-head">update_source</span> - Interface to use as source IP/IPv6 address of TCP connections. Source system.interface.name. <span class="li-normal">type: str</span></li>
            <li> <span class="li-head">weight</span> - Neighbor weight. <span class="li-normal">type: int</span></li>
            </ul>
        <li> <span class="li-head">neighbor_range</span> - BGP neighbor range table. <span class="li-normal">type: list</span></li>
            <ul class="ul-self">
            <li> <span class="li-head">id</span> - Neighbor range ID. <span class="li-normal">type: int</span> <span class="li-required">required: True</span></li>
            <li> <span class="li-head">max_neighbor_num</span> - Maximum number of neighbors. <span class="li-normal">type: int</span></li>
            <li> <span class="li-head">neighbor_group</span> - Neighbor group name. Source router.bgp.neighbor-group.name. <span class="li-normal">type: str</span></li>
            <li> <span class="li-head">prefix</span> - Neighbor range prefix. <span class="li-normal">type: str</span></li>
            </ul>
        <li> <span class="li-head">neighbor_range6</span> - BGP IPv6 neighbor range table. <span class="li-normal">type: list</span></li>
            <ul class="ul-self">
            <li> <span class="li-head">id</span> - IPv6 neighbor range ID. <span class="li-normal">type: int</span> <span class="li-required">required: True</span></li>
            <li> <span class="li-head">max_neighbor_num</span> - Maximum number of neighbors. <span class="li-normal">type: int</span></li>
            <li> <span class="li-head">neighbor_group</span> - Neighbor group name. Source router.bgp.neighbor-group.name. <span class="li-normal">type: str</span></li>
            <li> <span class="li-head">prefix6</span> - IPv6 prefix. <span class="li-normal">type: str</span></li>
            </ul>
        <li> <span class="li-head">network</span> - BGP network table. <span class="li-normal">type: list</span></li>
            <ul class="ul-self">
            <li> <span class="li-head">backdoor</span> - Enable/disable route as backdoor. <span class="li-normal">type: str</span> <span class="li-normal">choices: enable, disable</span></li>
            <li> <span class="li-head">id</span> - ID. <span class="li-normal">type: int</span> <span class="li-required">required: True</span></li>
            <li> <span class="li-head">prefix</span> - Network prefix. <span class="li-normal">type: str</span></li>
            <li> <span class="li-head">route_map</span> - Route map to modify generated route. Source router.route-map.name. <span class="li-normal">type: str</span></li>
            </ul>
        <li> <span class="li-head">network_import_check</span> - Enable/disable ensure BGP network route exists in IGP. <span class="li-normal">type: str</span> <span class="li-normal">choices: enable, disable</span></li>
        <li> <span class="li-head">network6</span> - BGP IPv6 network table. <span class="li-normal">type: list</span></li>
            <ul class="ul-self">
            <li> <span class="li-head">backdoor</span> - Enable/disable route as backdoor. <span class="li-normal">type: str</span> <span class="li-normal">choices: enable, disable</span></li>
            <li> <span class="li-head">id</span> - ID. <span class="li-normal">type: int</span> <span class="li-required">required: True</span></li>
            <li> <span class="li-head">prefix6</span> - Network IPv6 prefix. <span class="li-normal">type: str</span></li>
            <li> <span class="li-head">route_map</span> - Route map to modify generated route. Source router.route-map.name. <span class="li-normal">type: str</span></li>
            </ul>
        <li> <span class="li-head">redistribute</span> - BGP IPv4 redistribute table. <span class="li-normal">type: list</span></li>
            <ul class="ul-self">
            <li> <span class="li-head">name</span> - Distribute list entry name. <span class="li-normal">type: str</span> <span class="li-required">required: True</span></li>
            <li> <span class="li-head">route_map</span> - Route map name. Source router.route-map.name. <span class="li-normal">type: str</span></li>
            <li> <span class="li-head">status</span> - Status <span class="li-normal">type: str</span> <span class="li-normal">choices: enable, disable</span></li>
            </ul>
        <li> <span class="li-head">redistribute6</span> - BGP IPv6 redistribute table. <span class="li-normal">type: list</span></li>
            <ul class="ul-self">
            <li> <span class="li-head">name</span> - Distribute list entry name. <span class="li-normal">type: str</span> <span class="li-required">required: True</span></li>
            <li> <span class="li-head">route_map</span> - Route map name. Source router.route-map.name. <span class="li-normal">type: str</span></li>
            <li> <span class="li-head">status</span> - Status <span class="li-normal">type: str</span> <span class="li-normal">choices: enable, disable</span></li>
            </ul>
        <li> <span class="li-head">router_id</span> - Router ID. <span class="li-normal">type: str</span></li>
        <li> <span class="li-head">scan_time</span> - Background scanner interval (sec), 0 to disable it. <span class="li-normal">type: int</span></li>
        <li> <span class="li-head">synchronization</span> - Enable/disable only advertise routes from iBGP if routes present in an IGP. <span class="li-normal">type: str</span> <span class="li-normal">choices: enable, disable</span></li>
        <li> <span class="li-head">vrf_leak</span> - BGP VRF leaking table. <span class="li-normal">type: list</span></li>
            <ul class="ul-self">
            <li> <span class="li-head">target</span> - Target VRF table. <span class="li-normal">type: list</span></li>
                <ul class="ul-self">
                <li> <span class="li-head">interface</span> - Interface which is used to leak routes to target VRF. Source system.interface.name. <span class="li-normal">type: str</span></li>
                <li> <span class="li-head">route_map</span> - Route map of VRF leaking. Source router.route-map.name. <span class="li-normal">type: str</span></li>
                <li> <span class="li-head">vrf</span> - Target VRF ID <0 - 31>. <span class="li-normal">type: str</span> <span class="li-required">required: True</span></li>
                </ul>
            <li> <span class="li-head">vrf</span> - Origin VRF ID <0 - 31>. <span class="li-normal">type: str</span> <span class="li-required">required: True</span></li>
            </ul>
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
      - name: Configure BGP.
        fortios_router_bgp:
          vdom:  "{{ vdom }}"
          router_bgp:
            additional_path: "enable"
            additional_path_select: "4"
            additional_path_select6: "5"
            additional_path6: "enable"
            admin_distance:
             -
                distance: "8"
                id:  "9"
                neighbour_prefix: "<your_own_value>"
                route_list: "<your_own_value> (source router.access-list.name)"
            aggregate_address:
             -
                as_set: "enable"
                id:  "14"
                prefix: "<your_own_value>"
                summary_only: "enable"
            aggregate_address6:
             -
                as_set: "enable"
                id:  "19"
                prefix6: "<your_own_value>"
                summary_only: "enable"
            always_compare_med: "enable"
            as: "23"
            bestpath_as_path_ignore: "enable"
            bestpath_cmp_confed_aspath: "enable"
            bestpath_cmp_routerid: "enable"
            bestpath_med_confed: "enable"
            bestpath_med_missing_as_worst: "enable"
            client_to_client_reflection: "enable"
            cluster_id: "<your_own_value>"
            confederation_identifier: "31"
            confederation_peers:
             -
                peer: "<your_own_value>"
            dampening: "enable"
            dampening_max_suppress_time: "35"
            dampening_reachability_half_life: "36"
            dampening_reuse: "37"
            dampening_route_map: "<your_own_value> (source router.route-map.name)"
            dampening_suppress: "39"
            dampening_unreachability_half_life: "40"
            default_local_preference: "41"
            deterministic_med: "enable"
            distance_external: "43"
            distance_internal: "44"
            distance_local: "45"
            ebgp_multipath: "enable"
            enforce_first_as: "enable"
            fast_external_failover: "enable"
            graceful_end_on_timer: "enable"
            graceful_restart: "enable"
            graceful_restart_time: "51"
            graceful_stalepath_time: "52"
            graceful_update_delay: "53"
            holdtime_timer: "54"
            ibgp_multipath: "enable"
            ignore_optional_capability: "enable"
            keepalive_timer: "57"
            log_neighbour_changes: "enable"
            neighbor:
             -
                activate: "enable"
                activate6: "enable"
                additional_path: "send"
                additional_path6: "send"
                adv_additional_path: "64"
                adv_additional_path6: "65"
                advertisement_interval: "66"
                allowas_in: "67"
                allowas_in_enable: "enable"
                allowas_in_enable6: "enable"
                allowas_in6: "70"
                as_override: "enable"
                as_override6: "enable"
                attribute_unchanged: "as-path"
                attribute_unchanged6: "as-path"
                bfd: "enable"
                capability_default_originate: "enable"
                capability_default_originate6: "enable"
                capability_dynamic: "enable"
                capability_graceful_restart: "enable"
                capability_graceful_restart6: "enable"
                capability_orf: "none"
                capability_orf6: "none"
                capability_route_refresh: "enable"
                conditional_advertise:
                 -
                    advertise_routemap: "<your_own_value> (source router.route-map.name)"
                    condition_routemap: "<your_own_value> (source router.route-map.name)"
                    condition_type: "exist"
                connect_timer: "88"
                default_originate_routemap: "<your_own_value> (source router.route-map.name)"
                default_originate_routemap6: "<your_own_value> (source router.route-map.name)"
                description: "<your_own_value>"
                distribute_list_in: "<your_own_value> (source router.access-list.name)"
                distribute_list_in6: "<your_own_value> (source router.access-list6.name)"
                distribute_list_out: "<your_own_value> (source router.access-list.name)"
                distribute_list_out6: "<your_own_value> (source router.access-list6.name)"
                dont_capability_negotiate: "enable"
                ebgp_enforce_multihop: "enable"
                ebgp_multihop_ttl: "98"
                filter_list_in: "<your_own_value> (source router.aspath-list.name)"
                filter_list_in6: "<your_own_value> (source router.aspath-list.name)"
                filter_list_out: "<your_own_value> (source router.aspath-list.name)"
                filter_list_out6: "<your_own_value> (source router.aspath-list.name)"
                holdtime_timer: "103"
                interface: "<your_own_value> (source system.interface.name)"
                ip: "<your_own_value>"
                keep_alive_timer: "106"
                link_down_failover: "enable"
                local_as: "108"
                local_as_no_prepend: "enable"
                local_as_replace_as: "enable"
                maximum_prefix: "111"
                maximum_prefix_threshold: "112"
                maximum_prefix_threshold6: "113"
                maximum_prefix_warning_only: "enable"
                maximum_prefix_warning_only6: "enable"
                maximum_prefix6: "116"
                next_hop_self: "enable"
                next_hop_self6: "enable"
                override_capability: "enable"
                passive: "enable"
                password: "<your_own_value>"
                prefix_list_in: "<your_own_value> (source router.prefix-list.name)"
                prefix_list_in6: "<your_own_value> (source router.prefix-list6.name)"
                prefix_list_out: "<your_own_value> (source router.prefix-list.name)"
                prefix_list_out6: "<your_own_value> (source router.prefix-list6.name)"
                remote_as: "126"
                remove_private_as: "enable"
                remove_private_as6: "enable"
                restart_time: "129"
                retain_stale_time: "130"
                route_map_in: "<your_own_value> (source router.route-map.name)"
                route_map_in6: "<your_own_value> (source router.route-map.name)"
                route_map_out: "<your_own_value> (source router.route-map.name)"
                route_map_out_preferable: "<your_own_value> (source router.route-map.name)"
                route_map_out6: "<your_own_value> (source router.route-map.name)"
                route_map_out6_preferable: "<your_own_value> (source router.route-map.name)"
                route_reflector_client: "enable"
                route_reflector_client6: "enable"
                route_server_client: "enable"
                route_server_client6: "enable"
                send_community: "standard"
                send_community6: "standard"
                shutdown: "enable"
                soft_reconfiguration: "enable"
                soft_reconfiguration6: "enable"
                stale_route: "enable"
                strict_capability_match: "enable"
                unsuppress_map: "<your_own_value> (source router.route-map.name)"
                unsuppress_map6: "<your_own_value> (source router.route-map.name)"
                update_source: "<your_own_value> (source system.interface.name)"
                weight: "151"
            neighbor_group:
             -
                activate: "enable"
                activate6: "enable"
                additional_path: "send"
                additional_path6: "send"
                adv_additional_path: "157"
                adv_additional_path6: "158"
                advertisement_interval: "159"
                allowas_in: "160"
                allowas_in_enable: "enable"
                allowas_in_enable6: "enable"
                allowas_in6: "163"
                as_override: "enable"
                as_override6: "enable"
                attribute_unchanged: "as-path"
                attribute_unchanged6: "as-path"
                bfd: "enable"
                capability_default_originate: "enable"
                capability_default_originate6: "enable"
                capability_dynamic: "enable"
                capability_graceful_restart: "enable"
                capability_graceful_restart6: "enable"
                capability_orf: "none"
                capability_orf6: "none"
                capability_route_refresh: "enable"
                connect_timer: "177"
                default_originate_routemap: "<your_own_value> (source router.route-map.name)"
                default_originate_routemap6: "<your_own_value> (source router.route-map.name)"
                description: "<your_own_value>"
                distribute_list_in: "<your_own_value> (source router.access-list.name)"
                distribute_list_in6: "<your_own_value> (source router.access-list6.name)"
                distribute_list_out: "<your_own_value> (source router.access-list.name)"
                distribute_list_out6: "<your_own_value> (source router.access-list6.name)"
                dont_capability_negotiate: "enable"
                ebgp_enforce_multihop: "enable"
                ebgp_multihop_ttl: "187"
                filter_list_in: "<your_own_value> (source router.aspath-list.name)"
                filter_list_in6: "<your_own_value> (source router.aspath-list.name)"
                filter_list_out: "<your_own_value> (source router.aspath-list.name)"
                filter_list_out6: "<your_own_value> (source router.aspath-list.name)"
                holdtime_timer: "192"
                interface: "<your_own_value> (source system.interface.name)"
                keep_alive_timer: "194"
                link_down_failover: "enable"
                local_as: "196"
                local_as_no_prepend: "enable"
                local_as_replace_as: "enable"
                maximum_prefix: "199"
                maximum_prefix_threshold: "200"
                maximum_prefix_threshold6: "201"
                maximum_prefix_warning_only: "enable"
                maximum_prefix_warning_only6: "enable"
                maximum_prefix6: "204"
                name: "default_name_205"
                next_hop_self: "enable"
                next_hop_self6: "enable"
                override_capability: "enable"
                passive: "enable"
                prefix_list_in: "<your_own_value> (source router.prefix-list.name)"
                prefix_list_in6: "<your_own_value> (source router.prefix-list6.name)"
                prefix_list_out: "<your_own_value> (source router.prefix-list.name)"
                prefix_list_out6: "<your_own_value> (source router.prefix-list6.name)"
                remote_as: "214"
                remove_private_as: "enable"
                remove_private_as6: "enable"
                restart_time: "217"
                retain_stale_time: "218"
                route_map_in: "<your_own_value> (source router.route-map.name)"
                route_map_in6: "<your_own_value> (source router.route-map.name)"
                route_map_out: "<your_own_value> (source router.route-map.name)"
                route_map_out_preferable: "<your_own_value> (source router.route-map.name)"
                route_map_out6: "<your_own_value> (source router.route-map.name)"
                route_map_out6_preferable: "<your_own_value> (source router.route-map.name)"
                route_reflector_client: "enable"
                route_reflector_client6: "enable"
                route_server_client: "enable"
                route_server_client6: "enable"
                send_community: "standard"
                send_community6: "standard"
                shutdown: "enable"
                soft_reconfiguration: "enable"
                soft_reconfiguration6: "enable"
                stale_route: "enable"
                strict_capability_match: "enable"
                unsuppress_map: "<your_own_value> (source router.route-map.name)"
                unsuppress_map6: "<your_own_value> (source router.route-map.name)"
                update_source: "<your_own_value> (source system.interface.name)"
                weight: "239"
            neighbor_range:
             -
                id:  "241"
                max_neighbor_num: "242"
                neighbor_group: "<your_own_value> (source router.bgp.neighbor-group.name)"
                prefix: "<your_own_value>"
            neighbor_range6:
             -
                id:  "246"
                max_neighbor_num: "247"
                neighbor_group: "<your_own_value> (source router.bgp.neighbor-group.name)"
                prefix6: "<your_own_value>"
            network:
             -
                backdoor: "enable"
                id:  "252"
                prefix: "<your_own_value>"
                route_map: "<your_own_value> (source router.route-map.name)"
            network_import_check: "enable"
            network6:
             -
                backdoor: "enable"
                id:  "258"
                prefix6: "<your_own_value>"
                route_map: "<your_own_value> (source router.route-map.name)"
            redistribute:
             -
                name: "default_name_262"
                route_map: "<your_own_value> (source router.route-map.name)"
                status: "enable"
            redistribute6:
             -
                name: "default_name_266"
                route_map: "<your_own_value> (source router.route-map.name)"
                status: "enable"
            router_id: "<your_own_value>"
            scan_time: "270"
            synchronization: "enable"
            vrf_leak:
             -
                target:
                 -
                    interface: "<your_own_value> (source system.interface.name)"
                    route_map: "<your_own_value> (source router.route-map.name)"
                    vrf: "<your_own_value>"
                vrf: "<your_own_value>"
    


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
