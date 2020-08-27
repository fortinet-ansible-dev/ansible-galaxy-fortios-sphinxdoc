:source: fortios_system_link_monitor.py

:orphan:

.. fortios_system_link_monitor:

fortios_system_link_monitor -- Configure Link Health Monitor in Fortinet's FortiOS and FortiGate.
+++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++

.. versionadded:: 2.9

.. contents::
   :local:
   :depth: 1


Synopsis
--------
- This module is able to configure a FortiGate or FortiOS (FOS) device by allowing the user to set and modify system feature and link_monitor category. Examples include all parameters and values need to be adjusted to datasources before usage. Tested with FOS v6.0.0



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
    <li> <span class="li-head">state</span> - Indicates whether to create or remove the object. <span class="li-normal">type: str</span> <span class="li-required">required: True</span> <span class="li-normal">choices: present, absent</span></li>
    <li> <span class="li-head">system_link_monitor</span> - Configure Link Health Monitor. <span class="li-normal">type: dict</span></li>
        <ul class="ul-self">
        <li> <span class="li-head">addr_mode</span> - Address mode (IPv4 or IPv6). <span class="li-normal">type: str</span> <span class="li-normal">choices: ipv4, ipv6</span></li>
        <li> <span class="li-head">failtime</span> - Number of retry attempts before the server is considered down (1 - 10) <span class="li-normal">type: int</span></li>
        <li> <span class="li-head">gateway_ip</span> - Gateway IP address used to probe the server. <span class="li-normal">type: str</span></li>
        <li> <span class="li-head">gateway_ip6</span> - Gateway IPv6 address used to probe the server. <span class="li-normal">type: str</span></li>
        <li> <span class="li-head">ha_priority</span> - HA election priority (1 - 50). <span class="li-normal">type: int</span></li>
        <li> <span class="li-head">http_get</span> - If you are monitoring an HTML server you can send an HTTP-GET request with a custom string. Use this option to define the string. <span class="li-normal">type: str</span></li>
        <li> <span class="li-head">http_match</span> - String that you expect to see in the HTTP-GET requests of the traffic to be monitored. <span class="li-normal">type: str</span></li>
        <li> <span class="li-head">interval</span> - Detection interval (1 - 3600 sec). <span class="li-normal">type: int</span></li>
        <li> <span class="li-head">name</span> - Link monitor name. <span class="li-normal">type: str</span> <span class="li-required">required: True</span></li>
        <li> <span class="li-head">packet_size</span> - Packet size of a twamp test session, <span class="li-normal">type: int</span></li>
        <li> <span class="li-head">password</span> - Twamp controller password in authentication mode <span class="li-normal">type: str</span></li>
        <li> <span class="li-head">port</span> - Port number of the traffic to be used to monitor the server. <span class="li-normal">type: int</span></li>
        <li> <span class="li-head">protocol</span> - Protocols used to monitor the server. <span class="li-normal">type: str</span> <span class="li-normal">choices: ping, tcp-echo, udp-echo, http, twamp, ping6</span></li>
        <li> <span class="li-head">recoverytime</span> - Number of successful responses received before server is considered recovered (1 - 10). <span class="li-normal">type: int</span></li>
        <li> <span class="li-head">security_mode</span> - Twamp controller security mode. <span class="li-normal">type: str</span> <span class="li-normal">choices: none, authentication</span></li>
        <li> <span class="li-head">server</span> - IP address of the server(s) to be monitored. <span class="li-normal">type: list</span></li>
            <ul class="ul-self">
            <li> <span class="li-head">address</span> - Server address. <span class="li-normal">type: str</span> <span class="li-required">required: True</span></li>
            </ul>
        <li> <span class="li-head">source_ip</span> - Source IP address used in packet to the server. <span class="li-normal">type: str</span></li>
        <li> <span class="li-head">source_ip6</span> - Source IPv6 address used in packet to the server. <span class="li-normal">type: str</span></li>
        <li> <span class="li-head">srcintf</span> - Interface that receives the traffic to be monitored. Source system.interface.name. <span class="li-normal">type: str</span></li>
        <li> <span class="li-head">status</span> - Enable/disable this link monitor. <span class="li-normal">type: str</span> <span class="li-normal">choices: enable, disable</span></li>
        <li> <span class="li-head">update_cascade_interface</span> - Enable/disable update cascade interface. <span class="li-normal">type: str</span> <span class="li-normal">choices: enable, disable</span></li>
        <li> <span class="li-head">update_static_route</span> - Enable/disable updating the static route. <span class="li-normal">type: str</span> <span class="li-normal">choices: enable, disable</span></li>
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
      - name: Configure Link Health Monitor.
        fortios_system_link_monitor:
          vdom:  "{{ vdom }}"
          state: "present"
          system_link_monitor:
            addr_mode: "ipv4"
            failtime: "4"
            gateway_ip: "<your_own_value>"
            gateway_ip6: "<your_own_value>"
            ha_priority: "7"
            http_get: "<your_own_value>"
            http_match: "<your_own_value>"
            interval: "10"
            name: "default_name_11"
            packet_size: "12"
            password: "<your_own_value>"
            port: "14"
            protocol: "ping"
            recoverytime: "16"
            security_mode: "none"
            server:
             -
                address: "<your_own_value>"
            source_ip: "84.230.14.43"
            source_ip6: "<your_own_value>"
            srcintf: "<your_own_value> (source system.interface.name)"
            status: "enable"
            update_cascade_interface: "enable"
            update_static_route: "enable"


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
