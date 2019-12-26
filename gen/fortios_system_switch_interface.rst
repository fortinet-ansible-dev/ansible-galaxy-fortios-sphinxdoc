:source: fortios_system_switch_interface.py

:orphan:

.. _fortios_system_switch_interface:

fortios_system_switch_interface -- Configure software switch interfaces by grouping physical and WiFi interfaces in Fortinet's FortiOS and FortiGate.
+++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++

.. versionadded:: 2.9

.. contents::
   :local:
   :depth: 1


Synopsis
--------
- This module is able to configure a FortiGate or FortiOS (FOS) device by allowing the user to set and modify system feature and switch_interface category. Examples include all parameters and values need to be adjusted to datasources before usage. Tested with FOS v6.0.5


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
    <li><span class="li-head">state</span> - Indicates whether to create or remove the object. <span class="li-normal">type: str</span> <span class="li-required">required</span> <span class="li-normal">choices: present,  absent</span></li>
    <li><span class="li-head">system_switch_interface</span> - Configure software switch interfaces by grouping physical and WiFi interfaces. <span class="li-normal">default: null</span> <span class="li-normal">type: dict</span></li>
            <ul class="ul-self">

            <li><span class="li-head">intra_switch_policy</span> - Allow any traffic between switch interfaces or require firewall policies to allow traffic between switch interfaces. <span class="li-normal">type: str</span> <span class="li-normal">choices: implicit,  explicit</span></li>
            <li><span class="li-head">member</span> - Names of the interfaces that belong to the virtual switch. <span class="li-normal">type: list</span></li>
                    <ul class="ul-self">

                    <li><span class="li-head">interface_name</span> - Physical interface name. Source system.interface.name. <span class="li-normal">type: str</span>
                    </ul>

            <li><span class="li-head">name</span> - Interface name (name cannot be in use by any other interfaces, VLANs, or inter-VDOM links). <span class="li-required">required</span> <span class="li-normal">type: str</span></li>
            <li><span class="li-head">span</span> - Enable/disable port spanning. Port spanning echoes traffic received by the software switch to the span destination port. <span class="li-normal">type: str</span> <span class="li-normal">choices: disable,  enable</span></li>
            <li><span class="li-head">span_dest_port</span> - SPAN destination port name. All traffic on the SPAN source ports is echoed to the SPAN destination port. Source system.interface.name. <span class="li-normal">type: str</span></li>
            <li><span class="li-head">span_direction</span> - "The direction in which the SPAN port operates, either: rx, tx, or both." <span class="li-normal">type: str</span> <span class="li-normal">choices: rx,  tx,  both</span></li>
            <li><span class="li-head">span_source_port</span> - Physical interface name. Port spanning echoes all traffic on the SPAN source ports to the SPAN destination port. <span class="li-normal">type: list</span></li>
                    <ul class="ul-self">

                    <li><span class="li-head">interface_name</span> - Physical interface name. Source system.interface.name. <span class="li-normal">type: str</span>
                    </ul>

            <li><span class="li-head">type</span> - "Type of switch based on functionality: switch for normal functionality, or hub to duplicate packets to all port members." <span class="li-normal">type: str</span> <span class="li-normal">choices: switch,  hub</span></li>
            <li><span class="li-head">vdom</span> - VDOM that the software switch belongs to. Source system.vdom.name. <span class="li-normal">type: str</span>
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
      - name: Configure software switch interfaces by grouping physical and WiFi interfaces.
        fortios_system_switch_interface:
          host:  "{{ host }}"
          username: "{{ username }}"
          password: "{{ password }}"
          vdom:  "{{ vdom }}"
          https: "False"
          state: "present"
          system_switch_interface:
            intra_switch_policy: "implicit"
            member:
             -
                interface_name: "<your_own_value> (source system.interface.name)"
            name: "default_name_6"
            span: "disable"
            span_dest_port: "<your_own_value> (source system.interface.name)"
            span_direction: "rx"
            span_source_port:
             -
                interface_name: "<your_own_value> (source system.interface.name)"
            type: "switch"
            vdom: "<your_own_value> (source system.vdom.name)"



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