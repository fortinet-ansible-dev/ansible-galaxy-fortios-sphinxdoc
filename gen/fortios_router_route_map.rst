:source: fortios_router_route_map.py

:orphan:

.. fortios_router_route_map:

fortios_router_route_map -- Configure route maps in Fortinet's FortiOS and FortiGate.
+++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++

.. versionadded:: 2.9

.. contents::
   :local:
   :depth: 1


Synopsis
--------
- This module is able to configure a FortiGate or FortiOS (FOS) device by allowing the user to set and modify router feature and route_map category. Examples include all parameters and values need to be adjusted to datasources before usage. Tested with FOS v6.2.0



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
    <li> <span class="li-head">state</span> - Indicates whether to create or remove the object. <span class="li-normal">type: str</span> <span class="li-required">required: True</span> <span class="li-normal">choices: present, absent</span></li>
    <li> <span class="li-head">router_route_map</span> - Configure route maps. <span class="li-normal">type: dict</span></li>
        <ul class="ul-self">
        <li> <span class="li-head">comments</span> - Optional comments. <span class="li-normal">type: str</span></li>
        <li> <span class="li-head">name</span> - Name. <span class="li-normal">type: str</span> <span class="li-required">required: True</span></li>
        <li> <span class="li-head">rule</span> - Rule. <span class="li-normal">type: list</span></li>
            <ul class="ul-self">
            <li> <span class="li-head">action</span> - Action. <span class="li-normal">type: str</span> <span class="li-normal">choices: permit, deny</span></li>
            <li> <span class="li-head">id</span> - Rule ID. <span class="li-normal">type: int</span> <span class="li-required">required: True</span></li>
            <li> <span class="li-head">match_as_path</span> - Match BGP AS path list. Source router.aspath-list.name. <span class="li-normal">type: str</span></li>
            <li> <span class="li-head">match_community</span> - Match BGP community list. Source router.community-list.name. <span class="li-normal">type: str</span></li>
            <li> <span class="li-head">match_community_exact</span> - Enable/disable exact matching of communities. <span class="li-normal">type: str</span> <span class="li-normal">choices: enable, disable</span></li>
            <li> <span class="li-head">match_flags</span> - BGP flag value to match (0 - 65535) <span class="li-normal">type: int</span></li>
            <li> <span class="li-head">match_interface</span> - Match interface configuration. Source system.interface.name. <span class="li-normal">type: str</span></li>
            <li> <span class="li-head">match_ip_address</span> - Match IP address permitted by access-list or prefix-list. Source router.access-list.name router.prefix-list.name. <span class="li-normal">type: str</span></li>
            <li> <span class="li-head">match_ip_nexthop</span> - Match next hop IP address passed by access-list or prefix-list. Source router.access-list.name router.prefix-list.name. <span class="li-normal">type: str</span></li>
            <li> <span class="li-head">match_ip6_address</span> - Match IPv6 address permitted by access-list6 or prefix-list6. Source router.access-list6.name router.prefix-list6.name. <span class="li-normal">type: str</span></li>
            <li> <span class="li-head">match_ip6_nexthop</span> - Match next hop IPv6 address passed by access-list6 or prefix-list6. Source router.access-list6.name router.prefix-list6.name. <span class="li-normal">type: str</span></li>
            <li> <span class="li-head">match_metric</span> - Match metric for redistribute routes. <span class="li-normal">type: int</span></li>
            <li> <span class="li-head">match_origin</span> - Match BGP origin code. <span class="li-normal">type: str</span> <span class="li-normal">choices: none, egp, igp, incomplete</span></li>
            <li> <span class="li-head">match_route_type</span> - Match route type. <span class="li-normal">type: str</span> <span class="li-normal">choices: 1, 2, none</span></li>
            <li> <span class="li-head">match_tag</span> - Match tag. <span class="li-normal">type: int</span></li>
            <li> <span class="li-head">set_aggregator_as</span> - BGP aggregator AS. <span class="li-normal">type: int</span></li>
            <li> <span class="li-head">set_aggregator_ip</span> - BGP aggregator IP. <span class="li-normal">type: str</span></li>
            <li> <span class="li-head">set_aspath</span> - Prepend BGP AS path attribute. <span class="li-normal">type: list</span></li>
                <ul class="ul-self">
                <li> <span class="li-head">as</span> - AS number (0 - 42949672). NOTE: Use quotes for repeating numbers, e.g.: "1 1 2" <span class="li-normal">type: str</span> <span class="li-required">required: True</span></li>
                </ul>
            <li> <span class="li-head">set_aspath_action</span> - Specify preferred action of set-aspath. <span class="li-normal">type: str</span> <span class="li-normal">choices: prepend, replace</span></li>
            <li> <span class="li-head">set_atomic_aggregate</span> - Enable/disable BGP atomic aggregate attribute. <span class="li-normal">type: str</span> <span class="li-normal">choices: enable, disable</span></li>
            <li> <span class="li-head">set_community</span> - BGP community attribute. <span class="li-normal">type: list</span></li>
                <ul class="ul-self">
                <li> <span class="li-head">community</span> - Attribute: AA|AA:NN|internet|local-AS|no-advertise|no-export. <span class="li-normal">type: str</span> <span class="li-required">required: True</span></li>
                </ul>
            <li> <span class="li-head">set_community_additive</span> - Enable/disable adding set-community to existing community. <span class="li-normal">type: str</span> <span class="li-normal">choices: enable, disable</span></li>
            <li> <span class="li-head">set_community_delete</span> - Delete communities matching community list. Source router.community-list.name. <span class="li-normal">type: str</span></li>
            <li> <span class="li-head">set_dampening_max_suppress</span> - Maximum duration to suppress a route (1 - 255 min, 0 = unset). <span class="li-normal">type: int</span></li>
            <li> <span class="li-head">set_dampening_reachability_half_life</span> - Reachability half-life time for the penalty (1 - 45 min, 0 = unset). <span class="li-normal">type: int</span></li>
            <li> <span class="li-head">set_dampening_reuse</span> - Value to start reusing a route (1 - 20000, 0 = unset). <span class="li-normal">type: int</span></li>
            <li> <span class="li-head">set_dampening_suppress</span> - Value to start suppressing a route (1 - 20000, 0 = unset). <span class="li-normal">type: int</span></li>
            <li> <span class="li-head">set_dampening_unreachability_half_life</span> - Unreachability Half-life time for the penalty (1 - 45 min, 0 = unset) <span class="li-normal">type: int</span></li>
            <li> <span class="li-head">set_extcommunity_rt</span> - Route Target extended community. <span class="li-normal">type: list</span></li>
                <ul class="ul-self">
                <li> <span class="li-head">community</span> - AA:NN. <span class="li-normal">type: str</span> <span class="li-required">required: True</span></li>
                </ul>
            <li> <span class="li-head">set_extcommunity_soo</span> - Site-of-Origin extended community. <span class="li-normal">type: list</span></li>
                <ul class="ul-self">
                <li> <span class="li-head">community</span> - AA:NN <span class="li-normal">type: str</span> <span class="li-required">required: True</span></li>
                </ul>
            <li> <span class="li-head">set_flags</span> - BGP flags value (0 - 65535) <span class="li-normal">type: int</span></li>
            <li> <span class="li-head">set_ip_nexthop</span> - IP address of next hop. <span class="li-normal">type: str</span></li>
            <li> <span class="li-head">set_ip6_nexthop</span> - IPv6 global address of next hop. <span class="li-normal">type: str</span></li>
            <li> <span class="li-head">set_ip6_nexthop_local</span> - IPv6 local address of next hop. <span class="li-normal">type: str</span></li>
            <li> <span class="li-head">set_local_preference</span> - BGP local preference path attribute. <span class="li-normal">type: int</span></li>
            <li> <span class="li-head">set_metric</span> - Metric value. <span class="li-normal">type: int</span></li>
            <li> <span class="li-head">set_metric_type</span> - Metric type. <span class="li-normal">type: str</span> <span class="li-normal">choices: 1, 2, none</span></li>
            <li> <span class="li-head">set_origin</span> - BGP origin code. <span class="li-normal">type: str</span> <span class="li-normal">choices: none, egp, igp, incomplete</span></li>
            <li> <span class="li-head">set_originator_id</span> - BGP originator ID attribute. <span class="li-normal">type: str</span></li>
            <li> <span class="li-head">set_route_tag</span> - Route tag for routing table. <span class="li-normal">type: int</span></li>
            <li> <span class="li-head">set_tag</span> - Tag value. <span class="li-normal">type: int</span></li>
            <li> <span class="li-head">set_weight</span> - BGP weight for routing table. <span class="li-normal">type: int</span></li>
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
      - name: Configure route maps.
        fortios_router_route_map:
          vdom:  "{{ vdom }}"
          state: "present"
          access_token: "<your_own_value>"
          router_route_map:
            comments: "<your_own_value>"
            name: "default_name_4"
            rule:
             -
                action: "permit"
                id:  "7"
                match_as_path: "<your_own_value> (source router.aspath-list.name)"
                match_community: "<your_own_value> (source router.community-list.name)"
                match_community_exact: "enable"
                match_flags: "11"
                match_interface: "<your_own_value> (source system.interface.name)"
                match_ip_address: "<your_own_value> (source router.access-list.name router.prefix-list.name)"
                match_ip_nexthop: "<your_own_value> (source router.access-list.name router.prefix-list.name)"
                match_ip6_address: "<your_own_value> (source router.access-list6.name router.prefix-list6.name)"
                match_ip6_nexthop: "<your_own_value> (source router.access-list6.name router.prefix-list6.name)"
                match_metric: "17"
                match_origin: "none"
                match_route_type: "1"
                match_tag: "20"
                set_aggregator_as: "21"
                set_aggregator_ip: "<your_own_value>"
                set_aspath:
                 -
                    as: "<your_own_value>"
                set_aspath_action: "prepend"
                set_atomic_aggregate: "enable"
                set_community:
                 -
                    community: "<your_own_value>"
                set_community_additive: "enable"
                set_community_delete: "<your_own_value> (source router.community-list.name)"
                set_dampening_max_suppress: "31"
                set_dampening_reachability_half_life: "32"
                set_dampening_reuse: "33"
                set_dampening_suppress: "34"
                set_dampening_unreachability_half_life: "35"
                set_extcommunity_rt:
                 -
                    community: "<your_own_value>"
                set_extcommunity_soo:
                 -
                    community: "<your_own_value>"
                set_flags: "40"
                set_ip_nexthop: "<your_own_value>"
                set_ip6_nexthop: "<your_own_value>"
                set_ip6_nexthop_local: "<your_own_value>"
                set_local_preference: "44"
                set_metric: "45"
                set_metric_type: "1"
                set_origin: "none"
                set_originator_id: "<your_own_value>"
                set_route_tag: "49"
                set_tag: "50"
                set_weight: "51"
    


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
