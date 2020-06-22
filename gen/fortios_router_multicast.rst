:source: fortios_router_multicast.py

:orphan:

.. fortios_router_multicast:

fortios_router_multicast -- Configure router multicast in Fortinet's FortiOS and FortiGate.
+++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++

.. versionadded:: 2.8

.. contents::
   :local:
   :depth: 1


Synopsis
--------
- This module is able to configure a FortiGate or FortiOS (FOS) device by allowing the user to set and modify router feature and multicast category. Examples include all parameters and values need to be adjusted to datasources before usage. Tested with FOS v6.2.0



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
    <li> <span class="li-head">router_multicast</span> - Configure router multicast. <span class="li-normal">type: dict</span></li>
        <ul class="ul-self">
        <li> <span class="li-head">interface</span> - PIM interfaces. <span class="li-normal">type: list</span></li>
            <ul class="ul-self">
            <li> <span class="li-head">bfd</span> - Enable/disable Protocol Independent Multicast (PIM) Bidirectional Forwarding Detection (BFD). <span class="li-normal">type: str</span> <span class="li-normal">choices: enable, disable</span></li>
            <li> <span class="li-head">cisco_exclude_genid</span> - Exclude GenID from hello packets (compatibility with old Cisco IOS). <span class="li-normal">type: str</span> <span class="li-normal">choices: enable, disable</span></li>
            <li> <span class="li-head">dr_priority</span> - DR election priority. <span class="li-normal">type: int</span></li>
            <li> <span class="li-head">hello_holdtime</span> - Time before old neighbor information expires (0 - 65535 sec). <span class="li-normal">type: int</span></li>
            <li> <span class="li-head">hello_interval</span> - Interval between sending PIM hello messages (0 - 65535 sec). <span class="li-normal">type: int</span></li>
            <li> <span class="li-head">igmp</span> - IGMP configuration options. <span class="li-normal">type: dict</span></li>
                <ul class="ul-self">
                <li> <span class="li-head">access_group</span> - Groups IGMP hosts are allowed to join. Source router.access-list.name. <span class="li-normal">type: str</span></li>
                <li> <span class="li-head">immediate_leave_group</span> - Groups to drop membership for immediately after receiving IGMPv2 leave. Source router.access-list.name. <span class="li-normal">type: str</span></li>
                <li> <span class="li-head">last_member_query_count</span> - Number of group specific queries before removing group (2 - 7). <span class="li-normal">type: int</span></li>
                <li> <span class="li-head">last_member_query_interval</span> - Timeout between IGMPv2 leave and removing group (1 - 65535 msec). <span class="li-normal">type: int</span></li>
                <li> <span class="li-head">query_interval</span> - Interval between queries to IGMP hosts (1 - 65535 sec). <span class="li-normal">type: int</span></li>
                <li> <span class="li-head">query_max_response_time</span> - Maximum time to wait for a IGMP query response (1 - 25 sec). <span class="li-normal">type: int</span></li>
                <li> <span class="li-head">query_timeout</span> - Timeout between queries before becoming querier for network (60 - 900). <span class="li-normal">type: int</span></li>
                <li> <span class="li-head">router_alert_check</span> - Enable/disable require IGMP packets contain router alert option. <span class="li-normal">type: str</span> <span class="li-normal">choices: enable, disable</span></li>
                <li> <span class="li-head">version</span> - Maximum version of IGMP to support. <span class="li-normal">type: str</span> <span class="li-normal">choices: 3, 2, 1</span></li>
                </ul>
            <li> <span class="li-head">join_group</span> - Join multicast groups. <span class="li-normal">type: list</span></li>
                <ul class="ul-self">
                <li> <span class="li-head">address</span> - Multicast group IP address. <span class="li-normal">type: str</span> <span class="li-required">required: True</span></li>
                </ul>
            <li> <span class="li-head">multicast_flow</span> - Acceptable source for multicast group. Source router.multicast-flow.name. <span class="li-normal">type: str</span></li>
            <li> <span class="li-head">name</span> - Interface name. Source system.interface.name. <span class="li-normal">type: str</span> <span class="li-required">required: True</span></li>
            <li> <span class="li-head">neighbour_filter</span> - Routers acknowledged as neighbor routers. Source router.access-list.name. <span class="li-normal">type: str</span></li>
            <li> <span class="li-head">passive</span> - Enable/disable listening to IGMP but not participating in PIM. <span class="li-normal">type: str</span> <span class="li-normal">choices: enable, disable</span></li>
            <li> <span class="li-head">pim_mode</span> - PIM operation mode. <span class="li-normal">type: str</span> <span class="li-normal">choices: sparse-mode, dense-mode</span></li>
            <li> <span class="li-head">propagation_delay</span> - Delay flooding packets on this interface (100 - 5000 msec). <span class="li-normal">type: int</span></li>
            <li> <span class="li-head">rp_candidate</span> - Enable/disable compete to become RP in elections. <span class="li-normal">type: str</span> <span class="li-normal">choices: enable, disable</span></li>
            <li> <span class="li-head">rp_candidate_group</span> - Multicast groups managed by this RP. Source router.access-list.name. <span class="li-normal">type: str</span></li>
            <li> <span class="li-head">rp_candidate_interval</span> - RP candidate advertisement interval (1 - 16383 sec). <span class="li-normal">type: int</span></li>
            <li> <span class="li-head">rp_candidate_priority</span> - Router"s priority as RP. <span class="li-normal">type: int</span></li>
            <li> <span class="li-head">state_refresh_interval</span> - Interval between sending state-refresh packets (1 - 100 sec). <span class="li-normal">type: int</span></li>
            <li> <span class="li-head">static_group</span> - Statically set multicast groups to forward out. Source router.multicast-flow.name. <span class="li-normal">type: str</span></li>
            <li> <span class="li-head">ttl_threshold</span> - Minimum TTL of multicast packets that will be forwarded (applied only to new multicast routes) (1 - 255). <span class="li-normal">type: int</span></li>
            </ul>
        <li> <span class="li-head">multicast_routing</span> - Enable/disable IP multicast routing. <span class="li-normal">type: str</span> <span class="li-normal">choices: enable, disable</span></li>
        <li> <span class="li-head">pim_sm_global</span> - PIM sparse-mode global settings. <span class="li-normal">type: dict</span></li>
            <ul class="ul-self">
            <li> <span class="li-head">accept_register_list</span> - Sources allowed to register packets with this Rendezvous Point (RP). Source router.access-list.name. <span class="li-normal">type: str</span></li>
            <li> <span class="li-head">accept_source_list</span> - Sources allowed to send multicast traffic. Source router.access-list.name. <span class="li-normal">type: str</span></li>
            <li> <span class="li-head">bsr_allow_quick_refresh</span> - Enable/disable accept BSR quick refresh packets from neighbors. <span class="li-normal">type: str</span> <span class="li-normal">choices: enable, disable</span></li>
            <li> <span class="li-head">bsr_candidate</span> - Enable/disable allowing this router to become a bootstrap router (BSR). <span class="li-normal">type: str</span> <span class="li-normal">choices: enable, disable</span></li>
            <li> <span class="li-head">bsr_hash</span> - BSR hash length (0 - 32). <span class="li-normal">type: int</span></li>
            <li> <span class="li-head">bsr_interface</span> - Interface to advertise as candidate BSR. Source system.interface.name. <span class="li-normal">type: str</span></li>
            <li> <span class="li-head">bsr_priority</span> - BSR priority (0 - 255). <span class="li-normal">type: int</span></li>
            <li> <span class="li-head">cisco_crp_prefix</span> - Enable/disable making candidate RP compatible with old Cisco IOS. <span class="li-normal">type: str</span> <span class="li-normal">choices: enable, disable</span></li>
            <li> <span class="li-head">cisco_ignore_rp_set_priority</span> - Use only hash for RP selection (compatibility with old Cisco IOS). <span class="li-normal">type: str</span> <span class="li-normal">choices: enable, disable</span></li>
            <li> <span class="li-head">cisco_register_checksum</span> - Checksum entire register packet(for old Cisco IOS compatibility). <span class="li-normal">type: str</span> <span class="li-normal">choices: enable, disable</span></li>
            <li> <span class="li-head">cisco_register_checksum_group</span> - Cisco register checksum only these groups. Source router.access-list.name. <span class="li-normal">type: str</span></li>
            <li> <span class="li-head">join_prune_holdtime</span> - Join/prune holdtime (1 - 65535). <span class="li-normal">type: int</span></li>
            <li> <span class="li-head">message_interval</span> - Period of time between sending periodic PIM join/prune messages in seconds (1 - 65535). <span class="li-normal">type: int</span></li>
            <li> <span class="li-head">null_register_retries</span> - Maximum retries of null register (1 - 20). <span class="li-normal">type: int</span></li>
            <li> <span class="li-head">register_rate_limit</span> - Limit of packets/sec per source registered through this RP (0 - 65535). <span class="li-normal">type: int</span></li>
            <li> <span class="li-head">register_rp_reachability</span> - Enable/disable check RP is reachable before registering packets. <span class="li-normal">type: str</span> <span class="li-normal">choices: enable, disable</span></li>
            <li> <span class="li-head">register_source</span> - Override source address in register packets. <span class="li-normal">type: str</span> <span class="li-normal">choices: disable, interface, ip-address</span></li>
            <li> <span class="li-head">register_source_interface</span> - Override with primary interface address. Source system.interface.name. <span class="li-normal">type: str</span></li>
            <li> <span class="li-head">register_source_ip</span> - Override with local IP address. <span class="li-normal">type: str</span></li>
            <li> <span class="li-head">register_supression</span> - Period of time to honor register-stop message (1 - 65535 sec). <span class="li-normal">type: int</span></li>
            <li> <span class="li-head">rp_address</span> - Statically configure RP addresses. <span class="li-normal">type: list</span></li>
                <ul class="ul-self">
                <li> <span class="li-head">group</span> - Groups to use this RP. Source router.access-list.name. <span class="li-normal">type: str</span></li>
                <li> <span class="li-head">id</span> - ID. <span class="li-normal">type: int</span> <span class="li-required">required: True</span></li>
                <li> <span class="li-head">ip_address</span> - RP router address. <span class="li-normal">type: str</span></li>
                </ul>
            <li> <span class="li-head">rp_register_keepalive</span> - Timeout for RP receiving data on (S,G) tree (1 - 65535 sec). <span class="li-normal">type: int</span></li>
            <li> <span class="li-head">spt_threshold</span> - Enable/disable switching to source specific trees. <span class="li-normal">type: str</span> <span class="li-normal">choices: enable, disable</span></li>
            <li> <span class="li-head">spt_threshold_group</span> - Groups allowed to switch to source tree. Source router.access-list.name. <span class="li-normal">type: str</span></li>
            <li> <span class="li-head">ssm</span> - Enable/disable source specific multicast. <span class="li-normal">type: str</span> <span class="li-normal">choices: enable, disable</span></li>
            <li> <span class="li-head">ssm_range</span> - Groups allowed to source specific multicast. Source router.access-list.name. <span class="li-normal">type: str</span></li>
            </ul>
        <li> <span class="li-head">route_limit</span> - Maximum number of multicast routes. <span class="li-normal">type: int</span></li>
        <li> <span class="li-head">route_threshold</span> - Generate warnings when the number of multicast routes exceeds this number, must not be greater than route-limit. <span class="li-normal">type: int</span></li>
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
      - name: Configure router multicast.
        fortios_router_multicast:
          vdom:  "{{ vdom }}"
          router_multicast:
            interface:
             -
                bfd: "enable"
                cisco_exclude_genid: "enable"
                dr_priority: "6"
                hello_holdtime: "7"
                hello_interval: "8"
                igmp:
                    access_group: "<your_own_value> (source router.access-list.name)"
                    immediate_leave_group: "<your_own_value> (source router.access-list.name)"
                    last_member_query_count: "12"
                    last_member_query_interval: "13"
                    query_interval: "14"
                    query_max_response_time: "15"
                    query_timeout: "16"
                    router_alert_check: "enable"
                    version: "3"
                join_group:
                 -
                    address: "<your_own_value>"
                multicast_flow: "<your_own_value> (source router.multicast-flow.name)"
                name: "default_name_22 (source system.interface.name)"
                neighbour_filter: "<your_own_value> (source router.access-list.name)"
                passive: "enable"
                pim_mode: "sparse-mode"
                propagation_delay: "26"
                rp_candidate: "enable"
                rp_candidate_group: "<your_own_value> (source router.access-list.name)"
                rp_candidate_interval: "29"
                rp_candidate_priority: "30"
                state_refresh_interval: "31"
                static_group: "<your_own_value> (source router.multicast-flow.name)"
                ttl_threshold: "33"
            multicast_routing: "enable"
            pim_sm_global:
                accept_register_list: "<your_own_value> (source router.access-list.name)"
                accept_source_list: "<your_own_value> (source router.access-list.name)"
                bsr_allow_quick_refresh: "enable"
                bsr_candidate: "enable"
                bsr_hash: "40"
                bsr_interface: "<your_own_value> (source system.interface.name)"
                bsr_priority: "42"
                cisco_crp_prefix: "enable"
                cisco_ignore_rp_set_priority: "enable"
                cisco_register_checksum: "enable"
                cisco_register_checksum_group: "<your_own_value> (source router.access-list.name)"
                join_prune_holdtime: "47"
                message_interval: "48"
                null_register_retries: "49"
                register_rate_limit: "50"
                register_rp_reachability: "enable"
                register_source: "disable"
                register_source_interface: "<your_own_value> (source system.interface.name)"
                register_source_ip: "<your_own_value>"
                register_supression: "55"
                rp_address:
                 -
                    group: "<your_own_value> (source router.access-list.name)"
                    id:  "58"
                    ip_address: "<your_own_value>"
                rp_register_keepalive: "60"
                spt_threshold: "enable"
                spt_threshold_group: "<your_own_value> (source router.access-list.name)"
                ssm: "enable"
                ssm_range: "<your_own_value> (source router.access-list.name)"
            route_limit: "65"
            route_threshold: "66"


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
