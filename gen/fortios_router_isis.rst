:source: fortios_router_isis.py

:orphan:

.. fortios_router_isis:

fortios_router_isis -- Configure IS-IS in Fortinet's FortiOS and FortiGate.
+++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++

.. versionadded:: 2.9

.. contents::
   :local:
   :depth: 1


Synopsis
--------
- This module is able to configure a FortiGate or FortiOS (FOS) device by allowing the user to set and modify router feature and isis category. Examples include all parameters and values need to be adjusted to datasources before usage. Tested with FOS v6.0.0



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
    <li> <span class="li-head">router_isis</span> - Configure IS-IS. <span class="li-normal">type: dict</span></li>
        <ul class="ul-self">
        <li> <span class="li-head">adjacency_check</span> - Enable/disable adjacency check. <span class="li-normal">type: str</span> <span class="li-normal">choices: enable, disable</span></li>
        <li> <span class="li-head">adjacency_check6</span> - Enable/disable IPv6 adjacency check. <span class="li-normal">type: str</span> <span class="li-normal">choices: enable, disable</span></li>
        <li> <span class="li-head">adv_passive_only</span> - Enable/disable IS-IS advertisement of passive interfaces only. <span class="li-normal">type: str</span> <span class="li-normal">choices: enable, disable</span></li>
        <li> <span class="li-head">adv_passive_only6</span> - Enable/disable IPv6 IS-IS advertisement of passive interfaces only. <span class="li-normal">type: str</span> <span class="li-normal">choices: enable, disable</span></li>
        <li> <span class="li-head">auth_keychain_l1</span> - Authentication key-chain for level 1 PDUs. Source router.key-chain.name. <span class="li-normal">type: str</span></li>
        <li> <span class="li-head">auth_keychain_l2</span> - Authentication key-chain for level 2 PDUs. Source router.key-chain.name. <span class="li-normal">type: str</span></li>
        <li> <span class="li-head">auth_mode_l1</span> - Level 1 authentication mode. <span class="li-normal">type: str</span> <span class="li-normal">choices: password, md5</span></li>
        <li> <span class="li-head">auth_mode_l2</span> - Level 2 authentication mode. <span class="li-normal">type: str</span> <span class="li-normal">choices: password, md5</span></li>
        <li> <span class="li-head">auth_password_l1</span> - Authentication password for level 1 PDUs. <span class="li-normal">type: str</span></li>
        <li> <span class="li-head">auth_password_l2</span> - Authentication password for level 2 PDUs. <span class="li-normal">type: str</span></li>
        <li> <span class="li-head">auth_sendonly_l1</span> - Enable/disable level 1 authentication send-only. <span class="li-normal">type: str</span> <span class="li-normal">choices: enable, disable</span></li>
        <li> <span class="li-head">auth_sendonly_l2</span> - Enable/disable level 2 authentication send-only. <span class="li-normal">type: str</span> <span class="li-normal">choices: enable, disable</span></li>
        <li> <span class="li-head">default_originate</span> - Enable/disable distribution of default route information. <span class="li-normal">type: str</span> <span class="li-normal">choices: enable, disable</span></li>
        <li> <span class="li-head">default_originate6</span> - Enable/disable distribution of default IPv6 route information. <span class="li-normal">type: str</span> <span class="li-normal">choices: enable, disable</span></li>
        <li> <span class="li-head">dynamic_hostname</span> - Enable/disable dynamic hostname. <span class="li-normal">type: str</span> <span class="li-normal">choices: enable, disable</span></li>
        <li> <span class="li-head">ignore_lsp_errors</span> - Enable/disable ignoring of LSP errors with bad checksums. <span class="li-normal">type: str</span> <span class="li-normal">choices: enable, disable</span></li>
        <li> <span class="li-head">is_type</span> - IS type. <span class="li-normal">type: str</span> <span class="li-normal">choices: level-1-2, level-1, level-2-only</span></li>
        <li> <span class="li-head">isis_interface</span> - IS-IS interface configuration. <span class="li-normal">type: list</span></li>
            <ul class="ul-self">
            <li> <span class="li-head">auth_keychain_l1</span> - Authentication key-chain for level 1 PDUs. Source router.key-chain.name. <span class="li-normal">type: str</span></li>
            <li> <span class="li-head">auth_keychain_l2</span> - Authentication key-chain for level 2 PDUs. Source router.key-chain.name. <span class="li-normal">type: str</span></li>
            <li> <span class="li-head">auth_mode_l1</span> - Level 1 authentication mode. <span class="li-normal">type: str</span> <span class="li-normal">choices: md5, password</span></li>
            <li> <span class="li-head">auth_mode_l2</span> - Level 2 authentication mode. <span class="li-normal">type: str</span> <span class="li-normal">choices: md5, password</span></li>
            <li> <span class="li-head">auth_password_l1</span> - Authentication password for level 1 PDUs. <span class="li-normal">type: str</span></li>
            <li> <span class="li-head">auth_password_l2</span> - Authentication password for level 2 PDUs. <span class="li-normal">type: str</span></li>
            <li> <span class="li-head">auth_send_only_l1</span> - Enable/disable authentication send-only for level 1 PDUs. <span class="li-normal">type: str</span> <span class="li-normal">choices: enable, disable</span></li>
            <li> <span class="li-head">auth_send_only_l2</span> - Enable/disable authentication send-only for level 2 PDUs. <span class="li-normal">type: str</span> <span class="li-normal">choices: enable, disable</span></li>
            <li> <span class="li-head">circuit_type</span> - IS-IS interface"s circuit type <span class="li-normal">type: str</span> <span class="li-normal">choices: level-1-2, level-1, level-2</span></li>
            <li> <span class="li-head">csnp_interval_l1</span> - Level 1 CSNP interval. <span class="li-normal">type: int</span></li>
            <li> <span class="li-head">csnp_interval_l2</span> - Level 2 CSNP interval. <span class="li-normal">type: int</span></li>
            <li> <span class="li-head">hello_interval_l1</span> - Level 1 hello interval. <span class="li-normal">type: int</span></li>
            <li> <span class="li-head">hello_interval_l2</span> - Level 2 hello interval. <span class="li-normal">type: int</span></li>
            <li> <span class="li-head">hello_multiplier_l1</span> - Level 1 multiplier for Hello holding time. <span class="li-normal">type: int</span></li>
            <li> <span class="li-head">hello_multiplier_l2</span> - Level 2 multiplier for Hello holding time. <span class="li-normal">type: int</span></li>
            <li> <span class="li-head">hello_padding</span> - Enable/disable padding to IS-IS hello packets. <span class="li-normal">type: str</span> <span class="li-normal">choices: enable, disable</span></li>
            <li> <span class="li-head">lsp_interval</span> - LSP transmission interval (milliseconds). <span class="li-normal">type: int</span></li>
            <li> <span class="li-head">lsp_retransmit_interval</span> - LSP retransmission interval (sec). <span class="li-normal">type: int</span></li>
            <li> <span class="li-head">mesh_group</span> - Enable/disable IS-IS mesh group. <span class="li-normal">type: str</span> <span class="li-normal">choices: enable, disable</span></li>
            <li> <span class="li-head">mesh_group_id</span> - Mesh group ID <0-4294967295>, 0: mesh-group blocked. <span class="li-normal">type: int</span></li>
            <li> <span class="li-head">metric_l1</span> - Level 1 metric for interface. <span class="li-normal">type: int</span></li>
            <li> <span class="li-head">metric_l2</span> - Level 2 metric for interface. <span class="li-normal">type: int</span></li>
            <li> <span class="li-head">name</span> - IS-IS interface name. Source system.interface.name. <span class="li-normal">type: str</span> <span class="li-required">required: True</span></li>
            <li> <span class="li-head">network_type</span> - IS-IS interface"s network type <span class="li-normal">type: str</span> <span class="li-normal">choices: broadcast, point-to-point, loopback</span></li>
            <li> <span class="li-head">priority_l1</span> - Level 1 priority. <span class="li-normal">type: int</span></li>
            <li> <span class="li-head">priority_l2</span> - Level 2 priority. <span class="li-normal">type: int</span></li>
            <li> <span class="li-head">status</span> - Enable/disable interface for IS-IS. <span class="li-normal">type: str</span> <span class="li-normal">choices: enable, disable</span></li>
            <li> <span class="li-head">status6</span> - Enable/disable IPv6 interface for IS-IS. <span class="li-normal">type: str</span> <span class="li-normal">choices: enable, disable</span></li>
            <li> <span class="li-head">wide_metric_l1</span> - Level 1 wide metric for interface. <span class="li-normal">type: int</span></li>
            <li> <span class="li-head">wide_metric_l2</span> - Level 2 wide metric for interface. <span class="li-normal">type: int</span></li>
            </ul>
        <li> <span class="li-head">isis_net</span> - IS-IS net configuration. <span class="li-normal">type: list</span></li>
            <ul class="ul-self">
            <li> <span class="li-head">id</span> - isis-net ID. <span class="li-normal">type: int</span> <span class="li-required">required: True</span></li>
            <li> <span class="li-head">net</span> - IS-IS net xx.xxxx. ... .xxxx.xx. <span class="li-normal">type: str</span></li>
            </ul>
        <li> <span class="li-head">lsp_gen_interval_l1</span> - Minimum interval for level 1 LSP regenerating. <span class="li-normal">type: int</span></li>
        <li> <span class="li-head">lsp_gen_interval_l2</span> - Minimum interval for level 2 LSP regenerating. <span class="li-normal">type: int</span></li>
        <li> <span class="li-head">lsp_refresh_interval</span> - LSP refresh time in seconds. <span class="li-normal">type: int</span></li>
        <li> <span class="li-head">max_lsp_lifetime</span> - Maximum LSP lifetime in seconds. <span class="li-normal">type: int</span></li>
        <li> <span class="li-head">metric_style</span> - Use old-style (ISO 10589) or new-style packet formats <span class="li-normal">type: str</span> <span class="li-normal">choices: narrow, wide, transition, narrow-transition, narrow-transition-l1, narrow-transition-l2, wide-l1, wide-l2, wide-transition, wide-transition-l1, wide-transition-l2, transition-l1, transition-l2</span></li>
        <li> <span class="li-head">overload_bit</span> - Enable/disable signal other routers not to use us in SPF. <span class="li-normal">type: str</span> <span class="li-normal">choices: enable, disable</span></li>
        <li> <span class="li-head">overload_bit_on_startup</span> - Overload-bit only temporarily after reboot. <span class="li-normal">type: int</span></li>
        <li> <span class="li-head">overload_bit_suppress</span> - Suppress overload-bit for the specific prefixes. <span class="li-normal">type: str</span> <span class="li-normal">choices: external, interlevel</span></li>
        <li> <span class="li-head">redistribute</span> - IS-IS redistribute protocols. <span class="li-normal">type: list</span></li>
            <ul class="ul-self">
            <li> <span class="li-head">level</span> - Level. <span class="li-normal">type: str</span> <span class="li-normal">choices: level-1-2, level-1, level-2</span></li>
            <li> <span class="li-head">metric</span> - Metric. <span class="li-normal">type: int</span></li>
            <li> <span class="li-head">metric_type</span> - Metric type. <span class="li-normal">type: str</span> <span class="li-normal">choices: external, internal</span></li>
            <li> <span class="li-head">protocol</span> - Protocol name. <span class="li-normal">type: str</span> <span class="li-required">required: True</span></li>
            <li> <span class="li-head">routemap</span> - Route map name. Source router.route-map.name. <span class="li-normal">type: str</span></li>
            <li> <span class="li-head">status</span> - Status. <span class="li-normal">type: str</span> <span class="li-normal">choices: enable, disable</span></li>
            </ul>
        <li> <span class="li-head">redistribute_l1</span> - Enable/disable redistribution of level 1 routes into level 2. <span class="li-normal">type: str</span> <span class="li-normal">choices: enable, disable</span></li>
        <li> <span class="li-head">redistribute_l1_list</span> - Access-list for route redistribution from l1 to l2. Source router.access-list.name. <span class="li-normal">type: str</span></li>
        <li> <span class="li-head">redistribute_l2</span> - Enable/disable redistribution of level 2 routes into level 1. <span class="li-normal">type: str</span> <span class="li-normal">choices: enable, disable</span></li>
        <li> <span class="li-head">redistribute_l2_list</span> - Access-list for route redistribution from l2 to l1. Source router.access-list.name. <span class="li-normal">type: str</span></li>
        <li> <span class="li-head">redistribute6</span> - IS-IS IPv6 redistribution for routing protocols. <span class="li-normal">type: list</span></li>
            <ul class="ul-self">
            <li> <span class="li-head">level</span> - Level. <span class="li-normal">type: str</span> <span class="li-normal">choices: level-1-2, level-1, level-2</span></li>
            <li> <span class="li-head">metric</span> - Metric. <span class="li-normal">type: int</span></li>
            <li> <span class="li-head">metric_type</span> - Metric type. <span class="li-normal">type: str</span> <span class="li-normal">choices: external, internal</span></li>
            <li> <span class="li-head">protocol</span> - Protocol name. <span class="li-normal">type: str</span> <span class="li-required">required: True</span></li>
            <li> <span class="li-head">routemap</span> - Route map name. Source router.route-map.name. <span class="li-normal">type: str</span></li>
            <li> <span class="li-head">status</span> - Enable/disable redistribution. <span class="li-normal">type: str</span> <span class="li-normal">choices: enable, disable</span></li>
            </ul>
        <li> <span class="li-head">redistribute6_l1</span> - Enable/disable redistribution of level 1 IPv6 routes into level 2. <span class="li-normal">type: str</span> <span class="li-normal">choices: enable, disable</span></li>
        <li> <span class="li-head">redistribute6_l1_list</span> - Access-list for IPv6 route redistribution from l1 to l2. Source router.access-list6.name. <span class="li-normal">type: str</span></li>
        <li> <span class="li-head">redistribute6_l2</span> - Enable/disable redistribution of level 2 IPv6 routes into level 1. <span class="li-normal">type: str</span> <span class="li-normal">choices: enable, disable</span></li>
        <li> <span class="li-head">redistribute6_l2_list</span> - Access-list for IPv6 route redistribution from l2 to l1. Source router.access-list6.name. <span class="li-normal">type: str</span></li>
        <li> <span class="li-head">spf_interval_exp_l1</span> - Level 1 SPF calculation delay. <span class="li-normal">type: str</span></li>
        <li> <span class="li-head">spf_interval_exp_l2</span> - Level 2 SPF calculation delay. <span class="li-normal">type: str</span></li>
        <li> <span class="li-head">summary_address</span> - IS-IS summary addresses. <span class="li-normal">type: list</span></li>
            <ul class="ul-self">
            <li> <span class="li-head">id</span> - Summary address entry ID. <span class="li-normal">type: int</span> <span class="li-required">required: True</span></li>
            <li> <span class="li-head">level</span> - Level. <span class="li-normal">type: str</span> <span class="li-normal">choices: level-1-2, level-1, level-2</span></li>
            <li> <span class="li-head">prefix</span> - Prefix. <span class="li-normal">type: str</span></li>
            </ul>
        <li> <span class="li-head">summary_address6</span> - IS-IS IPv6 summary address. <span class="li-normal">type: list</span></li>
            <ul class="ul-self">
            <li> <span class="li-head">id</span> - Prefix entry ID. <span class="li-normal">type: int</span> <span class="li-required">required: True</span></li>
            <li> <span class="li-head">level</span> - Level. <span class="li-normal">type: str</span> <span class="li-normal">choices: level-1-2, level-1, level-2</span></li>
            <li> <span class="li-head">prefix6</span> - IPv6 prefix. <span class="li-normal">type: str</span></li>
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
      - name: Configure IS-IS.
        fortios_router_isis:
          vdom:  "{{ vdom }}"
          router_isis:
            adjacency_check: "enable"
            adjacency_check6: "enable"
            adv_passive_only: "enable"
            adv_passive_only6: "enable"
            auth_keychain_l1: "<your_own_value> (source router.key-chain.name)"
            auth_keychain_l2: "<your_own_value> (source router.key-chain.name)"
            auth_mode_l1: "password"
            auth_mode_l2: "password"
            auth_password_l1: "<your_own_value>"
            auth_password_l2: "<your_own_value>"
            auth_sendonly_l1: "enable"
            auth_sendonly_l2: "enable"
            default_originate: "enable"
            default_originate6: "enable"
            dynamic_hostname: "enable"
            ignore_lsp_errors: "enable"
            is_type: "level-1-2"
            isis_interface:
             -
                auth_keychain_l1: "<your_own_value> (source router.key-chain.name)"
                auth_keychain_l2: "<your_own_value> (source router.key-chain.name)"
                auth_mode_l1: "md5"
                auth_mode_l2: "md5"
                auth_password_l1: "<your_own_value>"
                auth_password_l2: "<your_own_value>"
                auth_send_only_l1: "enable"
                auth_send_only_l2: "enable"
                circuit_type: "level-1-2"
                csnp_interval_l1: "30"
                csnp_interval_l2: "31"
                hello_interval_l1: "32"
                hello_interval_l2: "33"
                hello_multiplier_l1: "34"
                hello_multiplier_l2: "35"
                hello_padding: "enable"
                lsp_interval: "37"
                lsp_retransmit_interval: "38"
                mesh_group: "enable"
                mesh_group_id: "40"
                metric_l1: "41"
                metric_l2: "42"
                name: "default_name_43 (source system.interface.name)"
                network_type: "broadcast"
                priority_l1: "45"
                priority_l2: "46"
                status: "enable"
                status6: "enable"
                wide_metric_l1: "49"
                wide_metric_l2: "50"
            isis_net:
             -
                id:  "52"
                net: "<your_own_value>"
            lsp_gen_interval_l1: "54"
            lsp_gen_interval_l2: "55"
            lsp_refresh_interval: "56"
            max_lsp_lifetime: "57"
            metric_style: "narrow"
            overload_bit: "enable"
            overload_bit_on_startup: "60"
            overload_bit_suppress: "external"
            redistribute:
             -
                level: "level-1-2"
                metric: "64"
                metric_type: "external"
                protocol: "<your_own_value>"
                routemap: "<your_own_value> (source router.route-map.name)"
                status: "enable"
            redistribute_l1: "enable"
            redistribute_l1_list: "<your_own_value> (source router.access-list.name)"
            redistribute_l2: "enable"
            redistribute_l2_list: "<your_own_value> (source router.access-list.name)"
            redistribute6:
             -
                level: "level-1-2"
                metric: "75"
                metric_type: "external"
                protocol: "<your_own_value>"
                routemap: "<your_own_value> (source router.route-map.name)"
                status: "enable"
            redistribute6_l1: "enable"
            redistribute6_l1_list: "<your_own_value> (source router.access-list6.name)"
            redistribute6_l2: "enable"
            redistribute6_l2_list: "<your_own_value> (source router.access-list6.name)"
            spf_interval_exp_l1: "<your_own_value>"
            spf_interval_exp_l2: "<your_own_value>"
            summary_address:
             -
                id:  "87"
                level: "level-1-2"
                prefix: "<your_own_value>"
            summary_address6:
             -
                id:  "91"
                level: "level-1-2"
                prefix6: "<your_own_value>"


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
