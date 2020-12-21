:source: fortios_firewall_vip64.py

:orphan:

.. fortios_firewall_vip64:

fortios_firewall_vip64 -- Configure IPv6 to IPv4 virtual IPs in Fortinet's FortiOS and FortiGate.
+++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++

.. versionadded:: 2.8

.. contents::
   :local:
   :depth: 1


Synopsis
--------
- This module is able to configure a FortiGate or FortiOS (FOS) device by allowing the user to set and modify firewall feature and vip64 category. Examples include all parameters and values need to be adjusted to datasources before usage. Tested with FOS v6.0.0



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
    <li> <span class="li-head">state</span> - Indicates whether to create or remove the object. This attribute was present already in previous version in a deeper level. It has been moved out to this outer level. <span class="li-normal">type: str</span> <span class="li-required">required: False</span> <span class="li-normal">choices: present, absent</span></li>
    <li> <span class="li-head">firewall_vip64</span> - Configure IPv6 to IPv4 virtual IPs. <span class="li-normal">type: dict</span></li>
        <ul class="ul-self">
        <li> <span class="li-head">state</span> - B(Deprecated) <span class="li-normal">type: str</span> <span class="li-required">required: False</span> <span class="li-normal">choices: present, absent</span></li>
        <li> <span class="li-head">arp_reply</span> - Enable ARP reply. <span class="li-normal">type: str</span> <span class="li-normal">choices: disable, enable</span></li>
        <li> <span class="li-head">color</span> - Color of icon on the GUI. <span class="li-normal">type: int</span></li>
        <li> <span class="li-head">comment</span> - Comment. <span class="li-normal">type: str</span></li>
        <li> <span class="li-head">extip</span> - Start-external-IP [-end-external-IP]. <span class="li-normal">type: str</span></li>
        <li> <span class="li-head">extport</span> - External service port. <span class="li-normal">type: str</span></li>
        <li> <span class="li-head">id</span> - Custom defined id. <span class="li-normal">type: int</span></li>
        <li> <span class="li-head">ldb_method</span> - Load balance method. <span class="li-normal">type: str</span> <span class="li-normal">choices: static, round-robin, weighted, least-session, least-rtt, first-alive</span></li>
        <li> <span class="li-head">mappedip</span> - Start-mapped-IP [-end-mapped-IP]. <span class="li-normal">type: str</span></li>
        <li> <span class="li-head">mappedport</span> - Mapped service port. <span class="li-normal">type: str</span></li>
        <li> <span class="li-head">monitor</span> - Health monitors. <span class="li-normal">type: list</span></li>
            <ul class="ul-self">
            <li> <span class="li-head">name</span> - Health monitor name. Source firewall.ldb-monitor.name. <span class="li-normal">type: str</span> <span class="li-required">required: True</span></li>
            </ul>
        <li> <span class="li-head">name</span> - VIP64 name. <span class="li-normal">type: str</span> <span class="li-required">required: True</span></li>
        <li> <span class="li-head">portforward</span> - Enable port forwarding. <span class="li-normal">type: str</span> <span class="li-normal">choices: disable, enable</span></li>
        <li> <span class="li-head">protocol</span> - Mapped port protocol. <span class="li-normal">type: str</span> <span class="li-normal">choices: tcp, udp</span></li>
        <li> <span class="li-head">realservers</span> - Real servers. <span class="li-normal">type: list</span></li>
            <ul class="ul-self">
            <li> <span class="li-head">client_ip</span> - Restrict server to a client IP in this range. <span class="li-normal">type: str</span></li>
            <li> <span class="li-head">healthcheck</span> - Per server health check. <span class="li-normal">type: str</span> <span class="li-normal">choices: disable, enable, vip</span></li>
            <li> <span class="li-head">holddown_interval</span> - Hold down interval. <span class="li-normal">type: int</span></li>
            <li> <span class="li-head">id</span> - Real server ID. <span class="li-normal">type: int</span> <span class="li-required">required: True</span></li>
            <li> <span class="li-head">ip</span> - Mapped server IP. <span class="li-normal">type: str</span></li>
            <li> <span class="li-head">max_connections</span> - Maximum number of connections allowed to server. <span class="li-normal">type: int</span></li>
            <li> <span class="li-head">monitor</span> - Health monitors. Source firewall.ldb-monitor.name. <span class="li-normal">type: str</span></li>
            <li> <span class="li-head">port</span> - Mapped server port. <span class="li-normal">type: int</span></li>
            <li> <span class="li-head">status</span> - Server administrative status. <span class="li-normal">type: str</span> <span class="li-normal">choices: active, standby, disable</span></li>
            <li> <span class="li-head">weight</span> - weight <span class="li-normal">type: int</span></li>
            </ul>
        <li> <span class="li-head">server_type</span> - Server type. <span class="li-normal">type: str</span> <span class="li-normal">choices: http, tcp, udp, ip</span></li>
        <li> <span class="li-head">src_filter</span> - Source IP6 filter (x:x:x:x:x:x:x:x/x). <span class="li-normal">type: list</span></li>
            <ul class="ul-self">
            <li> <span class="li-head">range</span> - Src-filter range. <span class="li-normal">type: str</span> <span class="li-required">required: True</span></li>
            </ul>
        <li> <span class="li-head">type</span> - VIP type: static NAT or server load balance. <span class="li-normal">type: str</span> <span class="li-normal">choices: static-nat, server-load-balance</span></li>
        <li> <span class="li-head">uuid</span> - Universally Unique Identifier (UUID; automatically assigned but can be manually reset). <span class="li-normal">type: str</span></li>
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
      - name: Configure IPv6 to IPv4 virtual IPs.
        fortios_firewall_vip64:
          vdom:  "{{ vdom }}"
          state: "present"
          access_token: "<your_own_value>"
          firewall_vip64:
            arp_reply: "disable"
            color: "4"
            comment: "Comment."
            extip: "<your_own_value>"
            extport: "<your_own_value>"
            id:  "8"
            ldb_method: "static"
            mappedip: "<your_own_value>"
            mappedport: "<your_own_value>"
            monitor:
             -
                name: "default_name_13 (source firewall.ldb-monitor.name)"
            name: "default_name_14"
            portforward: "disable"
            protocol: "tcp"
            realservers:
             -
                client_ip: "<your_own_value>"
                healthcheck: "disable"
                holddown_interval: "20"
                id:  "21"
                ip: "<your_own_value>"
                max_connections: "23"
                monitor: "<your_own_value> (source firewall.ldb-monitor.name)"
                port: "25"
                status: "active"
                weight: "27"
            server_type: "http"
            src_filter:
             -
                range: "<your_own_value>"
            type: "static-nat"
            uuid: "<your_own_value>"
    


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
