:source: fortios_switch_controller_flow_tracking.py

:orphan:

.. fortios_switch_controller_flow_tracking:

fortios_switch_controller_flow_tracking -- Configure FortiSwitch flow tracking and export via ipfix/netflow in Fortinet's FortiOS and FortiGate.
++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++

.. versionadded:: 2.9

.. contents::
   :local:
   :depth: 1


Synopsis
--------
- This module is able to configure a FortiGate or FortiOS (FOS) device by allowing the user to set and modify switch_controller feature and flow_tracking category. Examples include all parameters and values need to be adjusted to datasources before usage. Tested with FOS v6.4.0



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
    <li> <span class="li-head">switch_controller_flow_tracking</span> - Configure FortiSwitch flow tracking and export via ipfix/netflow. <span class="li-normal">type: dict</span></li>
        <ul class="ul-self">
        <li> <span class="li-head">aggregates</span> - Configure aggregates in which all traffic sessions matching the IP Address will be grouped into the same flow. <span class="li-normal">type: list</span></li>
            <ul class="ul-self">
            <li> <span class="li-head">id</span> - Aggregate id. <span class="li-normal">type: int</span> <span class="li-required">required: True</span></li>
            <li> <span class="li-head">ip</span> - IP address to group all matching traffic sessions to a flow. <span class="li-normal">type: str</span></li>
            </ul>
        <li> <span class="li-head">collector_ip</span> - Configure collector ip address. <span class="li-normal">type: str</span></li>
        <li> <span class="li-head">collector_port</span> - Configure collector port number(0-65535). <span class="li-normal">type: int</span></li>
        <li> <span class="li-head">format</span> - Configure flow tracking protocol. <span class="li-normal">type: str</span> <span class="li-normal">choices: netflow1, netflow5, netflow9, ipfix</span></li>
        <li> <span class="li-head">level</span> - Configure flow tracking level. <span class="li-normal">type: str</span> <span class="li-normal">choices: vlan, ip, port, proto, mac</span></li>
        <li> <span class="li-head">max_export_pkt_size</span> - Configure flow max export packet size (512-9216). <span class="li-normal">type: int</span></li>
        <li> <span class="li-head">sample_mode</span> - Configure sample mode for the flow tracking. <span class="li-normal">type: str</span> <span class="li-normal">choices: local, perimeter, device-ingress</span></li>
        <li> <span class="li-head">sample_rate</span> - Configure sample rate for the perimeter and device-ingress sampling(0 - 99999). <span class="li-normal">type: int</span></li>
        <li> <span class="li-head">timeout_general</span> - Configure flow session general timeout (60-604800). <span class="li-normal">type: int</span></li>
        <li> <span class="li-head">timeout_icmp</span> - Configure flow session ICMP timeout (60-604800). <span class="li-normal">type: int</span></li>
        <li> <span class="li-head">timeout_max</span> - Configure flow session max timeout (60-604800). <span class="li-normal">type: int</span></li>
        <li> <span class="li-head">timeout_tcp</span> - Configure flow session TCP timeout (60-604800). <span class="li-normal">type: int</span></li>
        <li> <span class="li-head">timeout_tcp_fin</span> - Configure flow session TCP FIN timeout (60-604800). <span class="li-normal">type: int</span></li>
        <li> <span class="li-head">timeout_tcp_rst</span> - Configure flow session TCP RST timeout (60-604800). <span class="li-normal">type: int</span></li>
        <li> <span class="li-head">timeout_udp</span> - Configure flow session UDP timeout (60-604800). <span class="li-normal">type: int</span></li>
        <li> <span class="li-head">transport</span> - Configure L4 transport protocol for exporting packets. <span class="li-normal">type: str</span> <span class="li-normal">choices: udp, tcp, sctp</span></li>
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
      - name: Configure FortiSwitch flow tracking and export via ipfix/netflow.
        fortios_switch_controller_flow_tracking:
          vdom:  "{{ vdom }}"
          switch_controller_flow_tracking:
            aggregates:
             -
                id:  "4"
                ip: "<your_own_value>"
            collector_ip: "<your_own_value>"
            collector_port: "7"
            format: "netflow1"
            level: "vlan"
            max_export_pkt_size: "10"
            sample_mode: "local"
            sample_rate: "12"
            timeout_general: "13"
            timeout_icmp: "14"
            timeout_max: "15"
            timeout_tcp: "16"
            timeout_tcp_fin: "17"
            timeout_tcp_rst: "18"
            timeout_udp: "19"
            transport: "udp"


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
