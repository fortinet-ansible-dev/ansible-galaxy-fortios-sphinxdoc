:source: fortios_router_ripng.py

:orphan:

.. _fortios_router_ripng:

fortios_router_ripng -- Configure RIPng in Fortinet's FortiOS and FortiGate.
++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++

.. versionadded:: 2.9

.. contents::
   :local:
   :depth: 1


Synopsis
--------
- This module is able to configure a FortiGate or FortiOS (FOS) device by allowing the user to set and modify router feature and ripng category. Examples include all parameters and values need to be adjusted to datasources before usage. Tested with FOS v6.0.5


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
    <li><span class="li-head">router_ripng</span> - Configure RIPng. <span class="li-normal">default: null</span> <span class="li-normal">type: dict</span></li>
            <ul class="ul-self">

            <li><span class="li-head">aggregate_address</span> - Aggregate address. <span class="li-normal">type: list</span></li>
                    <ul class="ul-self">

                    <li><span class="li-head">id</span> - Aggregate address entry ID. <span class="li-required">required</span> <span class="li-normal">type: int</span></li>
                    <li><span class="li-head">prefix6</span> - Aggregate address prefix. <span class="li-normal">type: str</span>
                    </ul>

            <li><span class="li-head">default_information_originate</span> - Enable/disable generation of default route. <span class="li-normal">type: str</span> <span class="li-normal">choices: enable,  disable</span></li>
            <li><span class="li-head">default_metric</span> - Metric that the FortiGate unit advertises to adjacent routers. <span class="li-normal">type: int</span></li>
            <li><span class="li-head">distance</span> - Administrative distance <span class="li-normal">type: list</span></li>
                    <ul class="ul-self">

                    <li><span class="li-head">access_list6</span> - Access list for route destination. Source router.access-list6.name. <span class="li-normal">type: str</span></li>
                    <li><span class="li-head">distance</span> - Distance (1 - 255). <span class="li-normal">type: int</span></li>
                    <li><span class="li-head">id</span> - Distance ID. <span class="li-required">required</span> <span class="li-normal">type: int</span></li>
                    <li><span class="li-head">prefix6</span> - Distance prefix6. <span class="li-normal">type: str</span>
                    </ul>

            <li><span class="li-head">distribute_list</span> - Use this to filter incoming or outgoing updates using an access list or a prefix list. <span class="li-normal">type: list</span></li>
                    <ul class="ul-self">

                    <li><span class="li-head">direction</span> - Distribute list direction. <span class="li-normal">type: str</span> <span class="li-normal">choices: in,  out</span></li>
                    <li><span class="li-head">id</span> - Distribute list ID. <span class="li-required">required</span> <span class="li-normal">type: int</span></li>
                    <li><span class="li-head">interface</span> - Distribute list interface name. Source system.interface.name. <span class="li-normal">type: str</span></li>
                    <li><span class="li-head">listname</span> - Distribute access/prefix list name. Source router.access-list6.name router.prefix-list6.name. <span class="li-normal">type: str</span></li>
                    <li><span class="li-head">status</span> - Use this to activate or deactivate <span class="li-normal">type: str</span> <span class="li-normal">choices: enable,  disable</span>
                    </ul>

            <li><span class="li-head">garbage_timer</span> - Time in seconds that must elapse after the timeout interval for a route expires,. <span class="li-normal">type: int</span></li>
            <li><span class="li-head">interface</span> - RIPng interface configuration. <span class="li-normal">type: list</span></li>
                    <ul class="ul-self">

                    <li><span class="li-head">flags</span> - Configuration flags of the interface. <span class="li-normal">type: int</span></li>
                    <li><span class="li-head">name</span> - Interface name. Source system.interface.name. <span class="li-required">required</span> <span class="li-normal">type: str</span></li>
                    <li><span class="li-head">split_horizon</span> - Configure RIP to use either regular or poisoned split horizon on this interface. <span class="li-normal">type: str</span> <span class="li-normal">choices: poisoned,  regular</span></li>
                    <li><span class="li-head">split_horizon_status</span> - Enable/disable split horizon. <span class="li-normal">type: str</span> <span class="li-normal">choices: enable,  disable</span>
                    </ul>

            <li><span class="li-head">max_out_metric</span> - Maximum metric allowed to output(0 means 'not set'). <span class="li-normal">type: int</span></li>
            <li><span class="li-head">neighbor</span> - List of neighbors. <span class="li-normal">type: list</span></li>
                    <ul class="ul-self">

                    <li><span class="li-head">id</span> - Neighbor entry ID. <span class="li-required">required</span> <span class="li-normal">type: int</span></li>
                    <li><span class="li-head">interface</span> - Interface name. Source system.interface.name. <span class="li-normal">type: str</span></li>
                    <li><span class="li-head">ip6</span> - IPv6 link-local address. <span class="li-normal">type: str</span>
                    </ul>

            <li><span class="li-head">network</span> - list of networks connected. <span class="li-normal">type: list</span></li>
                    <ul class="ul-self">

                    <li><span class="li-head">id</span> - Network entry ID. <span class="li-required">required</span> <span class="li-normal">type: int</span></li>
                    <li><span class="li-head">prefix</span> - Network IPv6 link-local prefix. <span class="li-normal">type: str</span>
                    </ul>

            <li><span class="li-head">offset_list</span> - Adds the specified offset to the metric (hop count) of a route. <span class="li-normal">type: list</span></li>
                    <ul class="ul-self">

                    <li><span class="li-head">access_list6</span> - IPv6 access list name. Source router.access-list6.name. <span class="li-normal">type: str</span></li>
                    <li><span class="li-head">direction</span> - Offset list direction. <span class="li-normal">type: str</span> <span class="li-normal">choices: in,  out</span></li>
                    <li><span class="li-head">id</span> - Offset-list ID. <span class="li-required">required</span> <span class="li-normal">type: int</span></li>
                    <li><span class="li-head">interface</span> - Interface name. Source system.interface.name. <span class="li-normal">type: str</span></li>
                    <li><span class="li-head">offset</span> - Offset range <span class="li-normal">type: int</span></li>
                    <li><span class="li-head">status</span> - Indicates if the offset is active or not <span class="li-normal">type: str</span> <span class="li-normal">choices: enable,  disable</span>
                    </ul>

            <li><span class="li-head">passive_interface</span> - Passive interface configuration. <span class="li-normal">type: list</span></li>
                    <ul class="ul-self">

                    <li><span class="li-head">name</span> - Passive interface name. Source system.interface.name. <span class="li-required">required</span> <span class="li-normal">type: str</span>
                    </ul>

            <li><span class="li-head">redistribute</span> - Redistribute configuration. <span class="li-normal">type: list</span></li>
                    <ul class="ul-self">

                    <li><span class="li-head">metric</span> - Redistribute metric setting. <span class="li-normal">type: int</span></li>
                    <li><span class="li-head">name</span> - Redistribute name. <span class="li-required">required</span> <span class="li-normal">type: str</span></li>
                    <li><span class="li-head">routemap</span> - Route map name. Source router.route-map.name. <span class="li-normal">type: str</span></li>
                    <li><span class="li-head">status</span> - Indicates if the redistribute is active or not <span class="li-normal">type: str</span> <span class="li-normal">choices: enable,  disable</span>
                    </ul>

            <li><span class="li-head">timeout_timer</span> - Time interval in seconds after which a route is declared unreachable. <span class="li-normal">type: int</span></li>
            <li><span class="li-head">update_timer</span> - The time interval in seconds between RIP updates. <span class="li-normal">type: int</span>
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
      - name: Configure RIPng.
        fortios_router_ripng:
          host:  "{{ host }}"
          username: "{{ username }}"
          password: "{{ password }}"
          vdom:  "{{ vdom }}"
          https: "False"
          router_ripng:
            aggregate_address:
             -
                id:  "4"
                prefix6: "<your_own_value>"
            default_information_originate: "enable"
            default_metric: "7"
            distance:
             -
                access_list6: "<your_own_value> (source router.access-list6.name)"
                distance: "10"
                id:  "11"
                prefix6: "<your_own_value>"
            distribute_list:
             -
                direction: "in"
                id:  "15"
                interface: "<your_own_value> (source system.interface.name)"
                listname: "<your_own_value> (source router.access-list6.name router.prefix-list6.name)"
                status: "enable"
            garbage_timer: "19"
            interface:
             -
                flags: "21"
                name: "default_name_22 (source system.interface.name)"
                split_horizon: "poisoned"
                split_horizon_status: "enable"
            max_out_metric: "25"
            neighbor:
             -
                id:  "27"
                interface: "<your_own_value> (source system.interface.name)"
                ip6: "<your_own_value>"
            network:
             -
                id:  "31"
                prefix: "<your_own_value>"
            offset_list:
             -
                access_list6: "<your_own_value> (source router.access-list6.name)"
                direction: "in"
                id:  "36"
                interface: "<your_own_value> (source system.interface.name)"
                offset: "38"
                status: "enable"
            passive_interface:
             -
                name: "default_name_41 (source system.interface.name)"
            redistribute:
             -
                metric: "43"
                name: "default_name_44"
                routemap: "<your_own_value> (source router.route-map.name)"
                status: "enable"
            timeout_timer: "47"
            update_timer: "48"



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