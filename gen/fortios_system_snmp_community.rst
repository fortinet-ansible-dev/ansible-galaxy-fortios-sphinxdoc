:source: fortios_system_snmp_community.py

:orphan:

.. fortios_system_snmp_community:

fortios_system_snmp_community -- SNMP community configuration in Fortinet's FortiOS and FortiGate.
++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++

.. versionadded:: 2.9

.. contents::
   :local:
   :depth: 1


Synopsis
--------
- This module is able to configure a FortiGate or FortiOS (FOS) device by allowing the user to set and modify system_snmp feature and community category. Examples include all parameters and values need to be adjusted to datasources before usage. Tested with FOS v6.4.0



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
    <li> <span class="li-head">system_snmp_community</span> - SNMP community configuration. <span class="li-normal">type: dict</span></li>
        <ul class="ul-self">
        <li> <span class="li-head">events</span> - SNMP trap events. <span class="li-normal">type: list</span> <span class="li-normal">choices: cpu-high, mem-low, log-full, intf-ip, vpn-tun-up, vpn-tun-down, ha-switch, ha-hb-failure, ips-signature, ips-anomaly, av-virus, av-oversize, av-pattern, av-fragmented, fm-if-change, fm-conf-change, bgp-established, bgp-backward-transition, ha-member-up, ha-member-down, ent-conf-change, av-conserve, av-bypass, av-oversize-passed, av-oversize-blocked, ips-pkg-update, ips-fail-open, faz-disconnect, wc-ap-up, wc-ap-down, fswctl-session-up, fswctl-session-down, load-balance-real-server-down, device-new, per-cpu-high, dhcp</span></li>
        <li> <span class="li-head">hosts</span> - Configure IPv4 SNMP managers (hosts). <span class="li-normal">type: list</span></li>
            <ul class="ul-self">
            <li> <span class="li-head">ha_direct</span> - Enable/disable direct management of HA cluster members. <span class="li-normal">type: str</span> <span class="li-normal">choices: enable, disable</span></li>
            <li> <span class="li-head">host_type</span> - Control whether the SNMP manager sends SNMP queries, receives SNMP traps, or both. <span class="li-normal">type: str</span> <span class="li-normal">choices: any, query, trap</span></li>
            <li> <span class="li-head">id</span> - Host entry ID. <span class="li-normal">type: int</span> <span class="li-required">required: True</span></li>
            <li> <span class="li-head">ip</span> - IPv4 address of the SNMP manager (host). <span class="li-normal">type: str</span></li>
            <li> <span class="li-head">source_ip</span> - Source IPv4 address for SNMP traps. <span class="li-normal">type: str</span></li>
            </ul>
        <li> <span class="li-head">hosts6</span> - Configure IPv6 SNMP managers. <span class="li-normal">type: list</span></li>
            <ul class="ul-self">
            <li> <span class="li-head">ha_direct</span> - Enable/disable direct management of HA cluster members. <span class="li-normal">type: str</span> <span class="li-normal">choices: enable, disable</span></li>
            <li> <span class="li-head">host_type</span> - Control whether the SNMP manager sends SNMP queries, receives SNMP traps, or both. <span class="li-normal">type: str</span> <span class="li-normal">choices: any, query, trap</span></li>
            <li> <span class="li-head">id</span> - Host6 entry ID. <span class="li-normal">type: int</span> <span class="li-required">required: True</span></li>
            <li> <span class="li-head">ipv6</span> - SNMP manager IPv6 address prefix. <span class="li-normal">type: str</span></li>
            <li> <span class="li-head">source_ipv6</span> - Source IPv6 address for SNMP traps. <span class="li-normal">type: str</span></li>
            </ul>
        <li> <span class="li-head">id</span> - Community ID. <span class="li-normal">type: int</span> <span class="li-required">required: True</span></li>
        <li> <span class="li-head">name</span> - Community name. <span class="li-normal">type: str</span></li>
        <li> <span class="li-head">query_v1_port</span> - SNMP v1 query port . <span class="li-normal">type: int</span></li>
        <li> <span class="li-head">query_v1_status</span> - Enable/disable SNMP v1 queries. <span class="li-normal">type: str</span> <span class="li-normal">choices: enable, disable</span></li>
        <li> <span class="li-head">query_v2c_port</span> - SNMP v2c query port . <span class="li-normal">type: int</span></li>
        <li> <span class="li-head">query_v2c_status</span> - Enable/disable SNMP v2c queries. <span class="li-normal">type: str</span> <span class="li-normal">choices: enable, disable</span></li>
        <li> <span class="li-head">status</span> - Enable/disable this SNMP community. <span class="li-normal">type: str</span> <span class="li-normal">choices: enable, disable</span></li>
        <li> <span class="li-head">trap_v1_lport</span> - SNMP v1 trap local port . <span class="li-normal">type: int</span></li>
        <li> <span class="li-head">trap_v1_rport</span> - SNMP v1 trap remote port . <span class="li-normal">type: int</span></li>
        <li> <span class="li-head">trap_v1_status</span> - Enable/disable SNMP v1 traps. <span class="li-normal">type: str</span> <span class="li-normal">choices: enable, disable</span></li>
        <li> <span class="li-head">trap_v2c_lport</span> - SNMP v2c trap local port . <span class="li-normal">type: int</span></li>
        <li> <span class="li-head">trap_v2c_rport</span> - SNMP v2c trap remote port . <span class="li-normal">type: int</span></li>
        <li> <span class="li-head">trap_v2c_status</span> - Enable/disable SNMP v2c traps. <span class="li-normal">type: str</span> <span class="li-normal">choices: enable, disable</span></li>
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
      - name: SNMP community configuration.
        fortios_system_snmp_community:
          vdom:  "{{ vdom }}"
          state: "present"
          access_token: "<your_own_value>"
          system_snmp_community:
            events: "cpu-high"
            hosts:
             -
                ha_direct: "enable"
                host_type: "any"
                id:  "7"
                ip: "<your_own_value>"
                source_ip: "84.230.14.43"
            hosts6:
             -
                ha_direct: "enable"
                host_type: "any"
                id:  "13"
                ipv6: "<your_own_value>"
                source_ipv6: "<your_own_value>"
            id:  "16"
            name: "default_name_17"
            query_v1_port: "18"
            query_v1_status: "enable"
            query_v2c_port: "20"
            query_v2c_status: "enable"
            status: "enable"
            trap_v1_lport: "23"
            trap_v1_rport: "24"
            trap_v1_status: "enable"
            trap_v2c_lport: "26"
            trap_v2c_rport: "27"
            trap_v2c_status: "enable"
    


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
