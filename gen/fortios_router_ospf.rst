:source: fortios_router_ospf.py

:orphan:

.. fortios_router_ospf:

fortios_router_ospf -- Configure OSPF in Fortinet's FortiOS and FortiGate.
++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++

.. versionadded:: 2.8

.. contents::
   :local:
   :depth: 1


Synopsis
--------
- This module is able to configure a FortiGate or FortiOS (FOS) device by allowing the user to set and modify router feature and ospf category. Examples include all parameters and values need to be adjusted to datasources before usage. Tested with FOS v6.0.5



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
    <li> <span class="li-head">router_ospf</span> - Configure OSPF. <span class="li-normal">type: dict</span></li>
        <ul class="ul-self">
        <li> <span class="li-head">abr_type</span> - Area border router type. <span class="li-normal">type: str</span> <span class="li-normal">choices: cisco, ibm, shortcut, standard</span></li>
        <li> <span class="li-head">area</span> - OSPF area configuration. <span class="li-normal">type: list</span></li>
            <ul class="ul-self">
            <li> <span class="li-head">authentication</span> - Authentication type. <span class="li-normal">type: str</span> <span class="li-normal">choices: none, text, md5</span></li>
            <li> <span class="li-head">default_cost</span> - Summary default cost of stub or NSSA area. <span class="li-normal">type: int</span></li>
            <li> <span class="li-head">filter_list</span> - OSPF area filter-list configuration. <span class="li-normal">type: list</span></li>
                <ul class="ul-self">
                <li> <span class="li-head">direction</span> - Direction. <span class="li-normal">type: str</span> <span class="li-normal">choices: in, out</span></li>
                <li> <span class="li-head">id</span> - Filter list entry ID. <span class="li-normal">type: int</span> <span class="li-required">required: True</span></li>
                <li> <span class="li-head">list</span> - Access-list or prefix-list name. Source router.access-list.name router.prefix-list.name. <span class="li-normal">type: str</span></li>
                </ul>
            <li> <span class="li-head">id</span> - Area entry IP address. <span class="li-normal">type: str</span> <span class="li-required">required: True</span></li>
            <li> <span class="li-head">nssa_default_information_originate</span> - Redistribute, advertise, or do not originate Type-7 default route into NSSA area. <span class="li-normal">type: str</span> <span class="li-normal">choices: enable, always, disable</span></li>
            <li> <span class="li-head">nssa_default_information_originate_metric</span> - OSPF default metric. <span class="li-normal">type: int</span></li>
            <li> <span class="li-head">nssa_default_information_originate_metric_type</span> - OSPF metric type for default routes. <span class="li-normal">type: str</span> <span class="li-normal">choices: 1, 2</span></li>
            <li> <span class="li-head">nssa_redistribution</span> - Enable/disable redistribute into NSSA area. <span class="li-normal">type: str</span> <span class="li-normal">choices: enable, disable</span></li>
            <li> <span class="li-head">nssa_translator_role</span> - NSSA translator role type. <span class="li-normal">type: str</span> <span class="li-normal">choices: candidate, never, always</span></li>
            <li> <span class="li-head">range</span> - OSPF area range configuration. <span class="li-normal">type: list</span></li>
                <ul class="ul-self">
                <li> <span class="li-head">advertise</span> - Enable/disable advertise status. <span class="li-normal">type: str</span> <span class="li-normal">choices: disable, enable</span></li>
                <li> <span class="li-head">id</span> - Range entry ID. <span class="li-normal">type: int</span> <span class="li-required">required: True</span></li>
                <li> <span class="li-head">prefix</span> - Prefix. <span class="li-normal">type: str</span></li>
                <li> <span class="li-head">substitute</span> - Substitute prefix. <span class="li-normal">type: str</span></li>
                <li> <span class="li-head">substitute_status</span> - Enable/disable substitute status. <span class="li-normal">type: str</span> <span class="li-normal">choices: enable, disable</span></li>
                </ul>
            <li> <span class="li-head">shortcut</span> - Enable/disable shortcut option. <span class="li-normal">type: str</span> <span class="li-normal">choices: disable, enable, default</span></li>
            <li> <span class="li-head">stub_type</span> - Stub summary setting. <span class="li-normal">type: str</span> <span class="li-normal">choices: no-summary, summary</span></li>
            <li> <span class="li-head">type</span> - Area type setting. <span class="li-normal">type: str</span> <span class="li-normal">choices: regular, nssa, stub</span></li>
            <li> <span class="li-head">virtual_link</span> - OSPF virtual link configuration. <span class="li-normal">type: list</span></li>
                <ul class="ul-self">
                <li> <span class="li-head">authentication</span> - Authentication type. <span class="li-normal">type: str</span> <span class="li-normal">choices: none, text, md5</span></li>
                <li> <span class="li-head">authentication_key</span> - Authentication key. <span class="li-normal">type: str</span></li>
                <li> <span class="li-head">dead_interval</span> - Dead interval. <span class="li-normal">type: int</span></li>
                <li> <span class="li-head">hello_interval</span> - Hello interval. <span class="li-normal">type: int</span></li>
                <li> <span class="li-head">md5_key</span> - MD5 key. <span class="li-normal">type: str</span></li>
                <li> <span class="li-head">name</span> - Virtual link entry name. <span class="li-normal">type: str</span> <span class="li-required">required: True</span></li>
                <li> <span class="li-head">peer</span> - Peer IP. <span class="li-normal">type: str</span></li>
                <li> <span class="li-head">retransmit_interval</span> - Retransmit interval. <span class="li-normal">type: int</span></li>
                <li> <span class="li-head">transmit_delay</span> - Transmit delay. <span class="li-normal">type: int</span></li>
                </ul>
            </ul>
        <li> <span class="li-head">auto_cost_ref_bandwidth</span> - Reference bandwidth in terms of megabits per second. <span class="li-normal">type: int</span></li>
        <li> <span class="li-head">bfd</span> - Bidirectional Forwarding Detection (BFD). <span class="li-normal">type: str</span> <span class="li-normal">choices: enable, disable</span></li>
        <li> <span class="li-head">database_overflow</span> - Enable/disable database overflow. <span class="li-normal">type: str</span> <span class="li-normal">choices: enable, disable</span></li>
        <li> <span class="li-head">database_overflow_max_lsas</span> - Database overflow maximum LSAs. <span class="li-normal">type: int</span></li>
        <li> <span class="li-head">database_overflow_time_to_recover</span> - Database overflow time to recover (sec). <span class="li-normal">type: int</span></li>
        <li> <span class="li-head">default_information_metric</span> - Default information metric. <span class="li-normal">type: int</span></li>
        <li> <span class="li-head">default_information_metric_type</span> - Default information metric type. <span class="li-normal">type: str</span> <span class="li-normal">choices: 1, 2</span></li>
        <li> <span class="li-head">default_information_originate</span> - Enable/disable generation of default route. <span class="li-normal">type: str</span> <span class="li-normal">choices: enable, always, disable</span></li>
        <li> <span class="li-head">default_information_route_map</span> - Default information route map. Source router.route-map.name. <span class="li-normal">type: str</span></li>
        <li> <span class="li-head">default_metric</span> - Default metric of redistribute routes. <span class="li-normal">type: int</span></li>
        <li> <span class="li-head">distance</span> - Distance of the route. <span class="li-normal">type: int</span></li>
        <li> <span class="li-head">distance_external</span> - Administrative external distance. <span class="li-normal">type: int</span></li>
        <li> <span class="li-head">distance_inter_area</span> - Administrative inter-area distance. <span class="li-normal">type: int</span></li>
        <li> <span class="li-head">distance_intra_area</span> - Administrative intra-area distance. <span class="li-normal">type: int</span></li>
        <li> <span class="li-head">distribute_list</span> - Distribute list configuration. <span class="li-normal">type: list</span></li>
            <ul class="ul-self">
            <li> <span class="li-head">access_list</span> - Access list name. Source router.access-list.name. <span class="li-normal">type: str</span></li>
            <li> <span class="li-head">id</span> - Distribute list entry ID. <span class="li-normal">type: int</span> <span class="li-required">required: True</span></li>
            <li> <span class="li-head">protocol</span> - Protocol type. <span class="li-normal">type: str</span> <span class="li-normal">choices: connected, static, rip</span></li>
            </ul>
        <li> <span class="li-head">distribute_list_in</span> - Filter incoming routes. Source router.access-list.name router.prefix-list.name. <span class="li-normal">type: str</span></li>
        <li> <span class="li-head">distribute_route_map_in</span> - Filter incoming external routes by route-map. Source router.route-map.name. <span class="li-normal">type: str</span></li>
        <li> <span class="li-head">log_neighbour_changes</span> - Enable logging of OSPF neighbour"s changes <span class="li-normal">type: str</span> <span class="li-normal">choices: enable, disable</span></li>
        <li> <span class="li-head">neighbor</span> - OSPF neighbor configuration are used when OSPF runs on non-broadcast media <span class="li-normal">type: list</span></li>
            <ul class="ul-self">
            <li> <span class="li-head">cost</span> - Cost of the interface, value range from 0 to 65535, 0 means auto-cost. <span class="li-normal">type: int</span></li>
            <li> <span class="li-head">id</span> - Neighbor entry ID. <span class="li-normal">type: int</span> <span class="li-required">required: True</span></li>
            <li> <span class="li-head">ip</span> - Interface IP address of the neighbor. <span class="li-normal">type: str</span></li>
            <li> <span class="li-head">poll_interval</span> - Poll interval time in seconds. <span class="li-normal">type: int</span></li>
            <li> <span class="li-head">priority</span> - Priority. <span class="li-normal">type: int</span></li>
            </ul>
        <li> <span class="li-head">network</span> - OSPF network configuration. <span class="li-normal">type: list</span></li>
            <ul class="ul-self">
            <li> <span class="li-head">area</span> - Attach the network to area. <span class="li-normal">type: str</span></li>
            <li> <span class="li-head">id</span> - Network entry ID. <span class="li-normal">type: int</span> <span class="li-required">required: True</span></li>
            <li> <span class="li-head">prefix</span> - Prefix. <span class="li-normal">type: str</span></li>
            </ul>
        <li> <span class="li-head">ospf_interface</span> - OSPF interface configuration. <span class="li-normal">type: list</span></li>
            <ul class="ul-self">
            <li> <span class="li-head">authentication</span> - Authentication type. <span class="li-normal">type: str</span> <span class="li-normal">choices: none, text, md5</span></li>
            <li> <span class="li-head">authentication_key</span> - Authentication key. <span class="li-normal">type: str</span></li>
            <li> <span class="li-head">bfd</span> - Bidirectional Forwarding Detection (BFD). <span class="li-normal">type: str</span> <span class="li-normal">choices: global, enable, disable</span></li>
            <li> <span class="li-head">cost</span> - Cost of the interface, value range from 0 to 65535, 0 means auto-cost. <span class="li-normal">type: int</span></li>
            <li> <span class="li-head">database_filter_out</span> - Enable/disable control of flooding out LSAs. <span class="li-normal">type: str</span> <span class="li-normal">choices: enable, disable</span></li>
            <li> <span class="li-head">dead_interval</span> - Dead interval. <span class="li-normal">type: int</span></li>
            <li> <span class="li-head">hello_interval</span> - Hello interval. <span class="li-normal">type: int</span></li>
            <li> <span class="li-head">hello_multiplier</span> - Number of hello packets within dead interval. <span class="li-normal">type: int</span></li>
            <li> <span class="li-head">interface</span> - Configuration interface name. Source system.interface.name. <span class="li-normal">type: str</span></li>
            <li> <span class="li-head">ip</span> - IP address. <span class="li-normal">type: str</span></li>
            <li> <span class="li-head">md5_key</span> - MD5 key. <span class="li-normal">type: str</span></li>
            <li> <span class="li-head">mtu</span> - MTU for database description packets. <span class="li-normal">type: int</span></li>
            <li> <span class="li-head">mtu_ignore</span> - Enable/disable ignore MTU. <span class="li-normal">type: str</span> <span class="li-normal">choices: enable, disable</span></li>
            <li> <span class="li-head">name</span> - Interface entry name. <span class="li-normal">type: str</span> <span class="li-required">required: True</span></li>
            <li> <span class="li-head">network_type</span> - Network type. <span class="li-normal">type: str</span> <span class="li-normal">choices: broadcast, non-broadcast, point-to-point, point-to-multipoint, point-to-multipoint-non-broadcast</span></li>
            <li> <span class="li-head">prefix_length</span> - Prefix length. <span class="li-normal">type: int</span></li>
            <li> <span class="li-head">priority</span> - Priority. <span class="li-normal">type: int</span></li>
            <li> <span class="li-head">resync_timeout</span> - Graceful restart neighbor resynchronization timeout. <span class="li-normal">type: int</span></li>
            <li> <span class="li-head">retransmit_interval</span> - Retransmit interval. <span class="li-normal">type: int</span></li>
            <li> <span class="li-head">status</span> - Enable/disable status. <span class="li-normal">type: str</span> <span class="li-normal">choices: disable, enable</span></li>
            <li> <span class="li-head">transmit_delay</span> - Transmit delay. <span class="li-normal">type: int</span></li>
            </ul>
        <li> <span class="li-head">passive_interface</span> - Passive interface configuration. <span class="li-normal">type: list</span></li>
            <ul class="ul-self">
            <li> <span class="li-head">name</span> - Passive interface name. Source system.interface.name. <span class="li-normal">type: str</span> <span class="li-required">required: True</span></li>
            </ul>
        <li> <span class="li-head">redistribute</span> - Redistribute configuration. <span class="li-normal">type: list</span></li>
            <ul class="ul-self">
            <li> <span class="li-head">metric</span> - Redistribute metric setting. <span class="li-normal">type: int</span></li>
            <li> <span class="li-head">metric_type</span> - Metric type. <span class="li-normal">type: str</span> <span class="li-normal">choices: 1, 2</span></li>
            <li> <span class="li-head">name</span> - Redistribute name. <span class="li-normal">type: str</span> <span class="li-required">required: True</span></li>
            <li> <span class="li-head">routemap</span> - Route map name. Source router.route-map.name. <span class="li-normal">type: str</span></li>
            <li> <span class="li-head">status</span> - status <span class="li-normal">type: str</span> <span class="li-normal">choices: enable, disable</span></li>
            <li> <span class="li-head">tag</span> - Tag value. <span class="li-normal">type: int</span></li>
            </ul>
        <li> <span class="li-head">restart_mode</span> - OSPF restart mode (graceful or LLS). <span class="li-normal">type: str</span> <span class="li-normal">choices: none, lls, graceful-restart</span></li>
        <li> <span class="li-head">restart_period</span> - Graceful restart period. <span class="li-normal">type: int</span></li>
        <li> <span class="li-head">rfc1583_compatible</span> - Enable/disable RFC1583 compatibility. <span class="li-normal">type: str</span> <span class="li-normal">choices: enable, disable</span></li>
        <li> <span class="li-head">router_id</span> - Router ID. <span class="li-normal">type: str</span></li>
        <li> <span class="li-head">spf_timers</span> - SPF calculation frequency. <span class="li-normal">type: str</span></li>
        <li> <span class="li-head">summary_address</span> - IP address summary configuration. <span class="li-normal">type: list</span></li>
            <ul class="ul-self">
            <li> <span class="li-head">advertise</span> - Enable/disable advertise status. <span class="li-normal">type: str</span> <span class="li-normal">choices: disable, enable</span></li>
            <li> <span class="li-head">id</span> - Summary address entry ID. <span class="li-normal">type: int</span> <span class="li-required">required: True</span></li>
            <li> <span class="li-head">prefix</span> - Prefix. <span class="li-normal">type: str</span></li>
            <li> <span class="li-head">tag</span> - Tag value. <span class="li-normal">type: int</span></li>
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
      - name: Configure OSPF.
        fortios_router_ospf:
          vdom:  "{{ vdom }}"
          router_ospf:
            abr_type: "cisco"
            area:
             -
                authentication: "none"
                default_cost: "6"
                filter_list:
                 -
                    direction: "in"
                    id:  "9"
                    list: "<your_own_value> (source router.access-list.name router.prefix-list.name)"
                id:  "11"
                nssa_default_information_originate: "enable"
                nssa_default_information_originate_metric: "13"
                nssa_default_information_originate_metric_type: "1"
                nssa_redistribution: "enable"
                nssa_translator_role: "candidate"
                range:
                 -
                    advertise: "disable"
                    id:  "19"
                    prefix: "<your_own_value>"
                    substitute: "<your_own_value>"
                    substitute_status: "enable"
                shortcut: "disable"
                stub_type: "no-summary"
                type: "regular"
                virtual_link:
                 -
                    authentication: "none"
                    authentication_key: "<your_own_value>"
                    dead_interval: "29"
                    hello_interval: "30"
                    md5_key: "<your_own_value>"
                    name: "default_name_32"
                    peer: "<your_own_value>"
                    retransmit_interval: "34"
                    transmit_delay: "35"
            auto_cost_ref_bandwidth: "36"
            bfd: "enable"
            database_overflow: "enable"
            database_overflow_max_lsas: "39"
            database_overflow_time_to_recover: "40"
            default_information_metric: "41"
            default_information_metric_type: "1"
            default_information_originate: "enable"
            default_information_route_map: "<your_own_value> (source router.route-map.name)"
            default_metric: "45"
            distance: "46"
            distance_external: "47"
            distance_inter_area: "48"
            distance_intra_area: "49"
            distribute_list:
             -
                access_list: "<your_own_value> (source router.access-list.name)"
                id:  "52"
                protocol: "connected"
            distribute_list_in: "<your_own_value> (source router.access-list.name router.prefix-list.name)"
            distribute_route_map_in: "<your_own_value> (source router.route-map.name)"
            log_neighbour_changes: "enable"
            neighbor:
             -
                cost: "58"
                id:  "59"
                ip: "<your_own_value>"
                poll_interval: "61"
                priority: "62"
            network:
             -
                area: "<your_own_value>"
                id:  "65"
                prefix: "<your_own_value>"
            ospf_interface:
             -
                authentication: "none"
                authentication_key: "<your_own_value>"
                bfd: "global"
                cost: "71"
                database_filter_out: "enable"
                dead_interval: "73"
                hello_interval: "74"
                hello_multiplier: "75"
                interface: "<your_own_value> (source system.interface.name)"
                ip: "<your_own_value>"
                md5_key: "<your_own_value>"
                mtu: "79"
                mtu_ignore: "enable"
                name: "default_name_81"
                network_type: "broadcast"
                prefix_length: "83"
                priority: "84"
                resync_timeout: "85"
                retransmit_interval: "86"
                status: "disable"
                transmit_delay: "88"
            passive_interface:
             -
                name: "default_name_90 (source system.interface.name)"
            redistribute:
             -
                metric: "92"
                metric_type: "1"
                name: "default_name_94"
                routemap: "<your_own_value> (source router.route-map.name)"
                status: "enable"
                tag: "97"
            restart_mode: "none"
            restart_period: "99"
            rfc1583_compatible: "enable"
            router_id: "<your_own_value>"
            spf_timers: "<your_own_value>"
            summary_address:
             -
                advertise: "disable"
                id:  "105"
                prefix: "<your_own_value>"
                tag: "107"


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
