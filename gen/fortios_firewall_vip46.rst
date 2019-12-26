:source: fortios_firewall_vip46.py

:orphan:

.. _fortios_firewall_vip46:

fortios_firewall_vip46 -- Configure IPv4 to IPv6 virtual IPs in Fortinet's FortiOS and FortiGate.
+++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++

.. versionadded:: 2.8

.. contents::
   :local:
   :depth: 1


Synopsis
--------
- This module is able to configure a FortiGate or FortiOS (FOS) device by allowing the user to set and modify firewall feature and vip46 category. Examples include all parameters and values need to be adjusted to datasources before usage. Tested with FOS v6.0.5


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
    <li><span class="li-head">state</span> - Indicates whether to create or remove the object. This attribute was present already in previous version in a deeper level. It has been moved out to this outer level. <span class="li-normal">type: str</span> <span class="li-required">required: false</span> <span class="li-normal">choices: present,  absent</span></li>
    <li><span class="li-head">firewall_vip46</span> - Configure IPv4 to IPv6 virtual IPs. <span class="li-normal">default: null</span> <span class="li-normal">type: dict</span></li>
            <ul class="ul-self">

            <li><span class="li-head">state</span> - B(Deprecated) Starting with Ansible 2.9 we recommend using the top-level 'state' parameter. HORIZONTALLINE Indicates whether to create or remove the object. <span class="li-normal">type: str</span> <span class="li-required">required: false</span> <span class="li-normal">choices: present,  absent</span></li>
            <li><span class="li-head">arp_reply</span> - Enable ARP reply. <span class="li-normal">type: str</span> <span class="li-normal">choices: disable,  enable</span></li>
            <li><span class="li-head">color</span> - Color of icon on the GUI. <span class="li-normal">type: int</span></li>
            <li><span class="li-head">comment</span> - Comment. <span class="li-normal">type: str</span></li>
            <li><span class="li-head">extip</span> - Start-external-IP [-end-external-IP]. <span class="li-normal">type: str</span></li>
            <li><span class="li-head">extport</span> - External service port. <span class="li-normal">type: str</span></li>
            <li><span class="li-head">id</span> - Custom defined id. <span class="li-normal">type: int</span></li>
            <li><span class="li-head">ldb_method</span> - Load balance method. <span class="li-normal">type: str</span> <span class="li-normal">choices: static,  round-robin,  weighted,  least-session,  least-rtt,  first-alive</span></li>
            <li><span class="li-head">mappedip</span> - Start-mapped-IP [-end mapped-IP]. <span class="li-normal">type: str</span></li>
            <li><span class="li-head">mappedport</span> - Mapped service port. <span class="li-normal">type: str</span></li>
            <li><span class="li-head">monitor</span> - Health monitors. <span class="li-normal">type: list</span></li>
                    <ul class="ul-self">

                    <li><span class="li-head">name</span> - Health monitor name. Source firewall.ldb-monitor.name. <span class="li-required">required</span> <span class="li-normal">type: str</span>
                    </ul>

            <li><span class="li-head">name</span> - VIP46 name. <span class="li-required">required</span> <span class="li-normal">type: str</span></li>
            <li><span class="li-head">portforward</span> - Enable port forwarding. <span class="li-normal">type: str</span> <span class="li-normal">choices: disable,  enable</span></li>
            <li><span class="li-head">protocol</span> - Mapped port protocol. <span class="li-normal">type: str</span> <span class="li-normal">choices: tcp,  udp</span></li>
            <li><span class="li-head">realservers</span> - Real servers. <span class="li-normal">type: list</span></li>
                    <ul class="ul-self">

                    <li><span class="li-head">client_ip</span> - Restrict server to a client IP in this range. <span class="li-normal">type: str</span></li>
                    <li><span class="li-head">healthcheck</span> - Per server health check. <span class="li-normal">type: str</span> <span class="li-normal">choices: disable,  enable,  vip</span></li>
                    <li><span class="li-head">holddown_interval</span> - Hold down interval. <span class="li-normal">type: int</span></li>
                    <li><span class="li-head">id</span> - Real server ID. <span class="li-required">required</span> <span class="li-normal">type: int</span></li>
                    <li><span class="li-head">ip</span> - Mapped server IPv6. <span class="li-normal">type: str</span></li>
                    <li><span class="li-head">max_connections</span> - Maximum number of connections allowed to server. <span class="li-normal">type: int</span></li>
                    <li><span class="li-head">monitor</span> - Health monitors. Source firewall.ldb-monitor.name. <span class="li-normal">type: str</span></li>
                    <li><span class="li-head">port</span> - Mapped server port. <span class="li-normal">type: int</span></li>
                    <li><span class="li-head">status</span> - Server administrative status. <span class="li-normal">type: str</span> <span class="li-normal">choices: active,  standby,  disable</span></li>
                    <li><span class="li-head">weight</span> - weight <span class="li-normal">type: int</span>
                    </ul>

            <li><span class="li-head">server_type</span> - Server type. <span class="li-normal">type: str</span> <span class="li-normal">choices: http,  tcp,  udp,  ip</span></li>
            <li><span class="li-head">src_filter</span> - Source IP filter (x.x.x.x/x). <span class="li-normal">type: list</span></li>
                    <ul class="ul-self">

                    <li><span class="li-head">range</span> - Src-filter range. <span class="li-required">required</span> <span class="li-normal">type: str</span>
                    </ul>

            <li><span class="li-head">type</span> - "VIP type: static NAT or server load balance." <span class="li-normal">type: str</span> <span class="li-normal">choices: static-nat,  server-load-balance</span></li>
            <li><span class="li-head">uuid</span> - Universally Unique Identifier (UUID; automatically assigned but can be manually reset). <span class="li-normal">type: str</span>
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
      - name: Configure IPv4 to IPv6 virtual IPs.
        fortios_firewall_vip46:
          host:  "{{ host }}"
          username: "{{ username }}"
          password: "{{ password }}"
          vdom:  "{{ vdom }}"
          https: "False"
          state: "present"
          firewall_vip46:
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