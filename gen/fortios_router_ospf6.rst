:source: fortios_router_ospf6.py

:orphan:

.. fortios_router_ospf6:

fortios_router_ospf6 -- Configure IPv6 OSPF in Fortinet's FortiOS and FortiGate.
++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++

.. versionadded:: 2.8

.. contents::
   :local:
   :depth: 1


Synopsis
--------
- This module is able to configure a FortiGate or FortiOS (FOS) device by allowing the user to set and modify router feature and ospf6 category. Examples include all parameters and values need to be adjusted to datasources before usage. Tested with FOS v6.0.0



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
    <li> <span class="li-head">router_ospf6</span> - Configure IPv6 OSPF. <span class="li-normal">type: dict</span></li>
        <ul class="ul-self">
        <li> <span class="li-head">abr_type</span> - Area border router type. <span class="li-normal">type: str</span> <span class="li-normal">choices: cisco, ibm, standard</span></li>
        <li> <span class="li-head">area</span> - OSPF6 area configuration. <span class="li-normal">type: list</span></li>
            <ul class="ul-self">
            <li> <span class="li-head">default_cost</span> - Summary default cost of stub or NSSA area. <span class="li-normal">type: int</span></li>
            <li> <span class="li-head">id</span> - Area entry IP address. <span class="li-normal">type: str</span> <span class="li-required">required: True</span></li>
            <li> <span class="li-head">nssa_default_information_originate</span> - Enable/disable originate type 7 default into NSSA area. <span class="li-normal">type: str</span> <span class="li-normal">choices: enable, disable</span></li>
            <li> <span class="li-head">nssa_default_information_originate_metric</span> - OSPFv3 default metric. <span class="li-normal">type: int</span></li>
            <li> <span class="li-head">nssa_default_information_originate_metric_type</span> - OSPFv3 metric type for default routes. <span class="li-normal">type: str</span> <span class="li-normal">choices: 1, 2</span></li>
            <li> <span class="li-head">nssa_redistribution</span> - Enable/disable redistribute into NSSA area. <span class="li-normal">type: str</span> <span class="li-normal">choices: enable, disable</span></li>
            <li> <span class="li-head">nssa_translator_role</span> - NSSA translator role type. <span class="li-normal">type: str</span> <span class="li-normal">choices: candidate, never, always</span></li>
            <li> <span class="li-head">range</span> - OSPF6 area range configuration. <span class="li-normal">type: list</span></li>
                <ul class="ul-self">
                <li> <span class="li-head">advertise</span> - Enable/disable advertise status. <span class="li-normal">type: str</span> <span class="li-normal">choices: disable, enable</span></li>
                <li> <span class="li-head">id</span> - Range entry ID. <span class="li-normal">type: int</span> <span class="li-required">required: True</span></li>
                <li> <span class="li-head">prefix6</span> - IPv6 prefix. <span class="li-normal">type: str</span></li>
                </ul>
            <li> <span class="li-head">stub_type</span> - Stub summary setting. <span class="li-normal">type: str</span> <span class="li-normal">choices: no-summary, summary</span></li>
            <li> <span class="li-head">type</span> - Area type setting. <span class="li-normal">type: str</span> <span class="li-normal">choices: regular, nssa, stub</span></li>
            <li> <span class="li-head">virtual_link</span> - OSPF6 virtual link configuration. <span class="li-normal">type: list</span></li>
                <ul class="ul-self">
                <li> <span class="li-head">dead_interval</span> - Dead interval. <span class="li-normal">type: int</span></li>
                <li> <span class="li-head">hello_interval</span> - Hello interval. <span class="li-normal">type: int</span></li>
                <li> <span class="li-head">name</span> - Virtual link entry name. <span class="li-normal">type: str</span> <span class="li-required">required: True</span></li>
                <li> <span class="li-head">peer</span> - A.B.C.D, peer router ID. <span class="li-normal">type: str</span></li>
                <li> <span class="li-head">retransmit_interval</span> - Retransmit interval. <span class="li-normal">type: int</span></li>
                <li> <span class="li-head">transmit_delay</span> - Transmit delay. <span class="li-normal">type: int</span></li>
                </ul>
            </ul>
        <li> <span class="li-head">auto_cost_ref_bandwidth</span> - Reference bandwidth in terms of megabits per second. <span class="li-normal">type: int</span></li>
        <li> <span class="li-head">bfd</span> - Enable/disable Bidirectional Forwarding Detection (BFD). <span class="li-normal">type: str</span> <span class="li-normal">choices: enable, disable</span></li>
        <li> <span class="li-head">default_information_metric</span> - Default information metric. <span class="li-normal">type: int</span></li>
        <li> <span class="li-head">default_information_metric_type</span> - Default information metric type. <span class="li-normal">type: str</span> <span class="li-normal">choices: 1, 2</span></li>
        <li> <span class="li-head">default_information_originate</span> - Enable/disable generation of default route. <span class="li-normal">type: str</span> <span class="li-normal">choices: enable, always, disable</span></li>
        <li> <span class="li-head">default_information_route_map</span> - Default information route map. Source router.route-map.name. <span class="li-normal">type: str</span></li>
        <li> <span class="li-head">default_metric</span> - Default metric of redistribute routes. <span class="li-normal">type: int</span></li>
        <li> <span class="li-head">log_neighbour_changes</span> - Enable logging of OSPFv3 neighbour"s changes <span class="li-normal">type: str</span> <span class="li-normal">choices: enable, disable</span></li>
        <li> <span class="li-head">ospf6_interface</span> - OSPF6 interface configuration. <span class="li-normal">type: list</span></li>
            <ul class="ul-self">
            <li> <span class="li-head">area_id</span> - A.B.C.D, in IPv4 address format. <span class="li-normal">type: str</span></li>
            <li> <span class="li-head">bfd</span> - Enable/disable Bidirectional Forwarding Detection (BFD). <span class="li-normal">type: str</span> <span class="li-normal">choices: global, enable, disable</span></li>
            <li> <span class="li-head">cost</span> - Cost of the interface, value range from 0 to 65535, 0 means auto-cost. <span class="li-normal">type: int</span></li>
            <li> <span class="li-head">dead_interval</span> - Dead interval. <span class="li-normal">type: int</span></li>
            <li> <span class="li-head">hello_interval</span> - Hello interval. <span class="li-normal">type: int</span></li>
            <li> <span class="li-head">interface</span> - Configuration interface name. Source system.interface.name. <span class="li-normal">type: str</span></li>
            <li> <span class="li-head">name</span> - Interface entry name. <span class="li-normal">type: str</span> <span class="li-required">required: True</span></li>
            <li> <span class="li-head">neighbor</span> - OSPFv3 neighbors are used when OSPFv3 runs on non-broadcast media <span class="li-normal">type: list</span></li>
                <ul class="ul-self">
                <li> <span class="li-head">cost</span> - Cost of the interface, value range from 0 to 65535, 0 means auto-cost. <span class="li-normal">type: int</span></li>
                <li> <span class="li-head">ip6</span> - IPv6 link local address of the neighbor. <span class="li-normal">type: str</span> <span class="li-required">required: True</span></li>
                <li> <span class="li-head">poll_interval</span> - Poll interval time in seconds. <span class="li-normal">type: int</span></li>
                <li> <span class="li-head">priority</span> - priority <span class="li-normal">type: int</span></li>
                </ul>
            <li> <span class="li-head">network_type</span> - Network type. <span class="li-normal">type: str</span> <span class="li-normal">choices: broadcast, point-to-point, non-broadcast, point-to-multipoint, point-to-multipoint-non-broadcast</span></li>
            <li> <span class="li-head">priority</span> - priority <span class="li-normal">type: int</span></li>
            <li> <span class="li-head">retransmit_interval</span> - Retransmit interval. <span class="li-normal">type: int</span></li>
            <li> <span class="li-head">status</span> - Enable/disable OSPF6 routing on this interface. <span class="li-normal">type: str</span> <span class="li-normal">choices: disable, enable</span></li>
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
            </ul>
        <li> <span class="li-head">router_id</span> - A.B.C.D, in IPv4 address format. <span class="li-normal">type: str</span></li>
        <li> <span class="li-head">spf_timers</span> - SPF calculation frequency. <span class="li-normal">type: str</span></li>
        <li> <span class="li-head">summary_address</span> - IPv6 address summary configuration. <span class="li-normal">type: list</span></li>
            <ul class="ul-self">
            <li> <span class="li-head">advertise</span> - Enable/disable advertise status. <span class="li-normal">type: str</span> <span class="li-normal">choices: disable, enable</span></li>
            <li> <span class="li-head">id</span> - Summary address entry ID. <span class="li-normal">type: int</span> <span class="li-required">required: True</span></li>
            <li> <span class="li-head">prefix6</span> - IPv6 prefix. <span class="li-normal">type: str</span></li>
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
      - name: Configure IPv6 OSPF.
        fortios_router_ospf6:
          vdom:  "{{ vdom }}"
          router_ospf6:
            abr_type: "cisco"
            area:
             -
                default_cost: "5"
                id:  "6"
                nssa_default_information_originate: "enable"
                nssa_default_information_originate_metric: "8"
                nssa_default_information_originate_metric_type: "1"
                nssa_redistribution: "enable"
                nssa_translator_role: "candidate"
                range:
                 -
                    advertise: "disable"
                    id:  "14"
                    prefix6: "<your_own_value>"
                stub_type: "no-summary"
                type: "regular"
                virtual_link:
                 -
                    dead_interval: "19"
                    hello_interval: "20"
                    name: "default_name_21"
                    peer: "<your_own_value>"
                    retransmit_interval: "23"
                    transmit_delay: "24"
            auto_cost_ref_bandwidth: "25"
            bfd: "enable"
            default_information_metric: "27"
            default_information_metric_type: "1"
            default_information_originate: "enable"
            default_information_route_map: "<your_own_value> (source router.route-map.name)"
            default_metric: "31"
            log_neighbour_changes: "enable"
            ospf6_interface:
             -
                area_id: "<your_own_value>"
                bfd: "global"
                cost: "36"
                dead_interval: "37"
                hello_interval: "38"
                interface: "<your_own_value> (source system.interface.name)"
                name: "default_name_40"
                neighbor:
                 -
                    cost: "42"
                    ip6: "<your_own_value>"
                    poll_interval: "44"
                    priority: "45"
                network_type: "broadcast"
                priority: "47"
                retransmit_interval: "48"
                status: "disable"
                transmit_delay: "50"
            passive_interface:
             -
                name: "default_name_52 (source system.interface.name)"
            redistribute:
             -
                metric: "54"
                metric_type: "1"
                name: "default_name_56"
                routemap: "<your_own_value> (source router.route-map.name)"
                status: "enable"
            router_id: "<your_own_value>"
            spf_timers: "<your_own_value>"
            summary_address:
             -
                advertise: "disable"
                id:  "63"
                prefix6: "<your_own_value>"
                tag: "65"


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
