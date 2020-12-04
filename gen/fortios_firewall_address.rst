:source: fortios_firewall_address.py

:orphan:

.. fortios_firewall_address:

fortios_firewall_address -- Configure IPv4 addresses in Fortinet's FortiOS and FortiGate.
+++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++

.. versionadded:: 2.8

.. contents::
   :local:
   :depth: 1


Synopsis
--------
- This module is able to configure a FortiGate or FortiOS (FOS) device by allowing the user to set and modify firewall feature and address category. Examples include all parameters and values need to be adjusted to datasources before usage. Tested with FOS v6.4.0



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
    <li> <span class="li-head">firewall_address</span> - Configure IPv4 addresses. <span class="li-normal">type: dict</span></li>
        <ul class="ul-self">
        <li> <span class="li-head">state</span> - B(Deprecated) <span class="li-normal">type: str</span> <span class="li-required">required: False</span> <span class="li-normal">choices: present, absent</span></li>
        <li> <span class="li-head">allow_routing</span> - Enable/disable use of this address in the static route configuration. <span class="li-normal">type: str</span> <span class="li-normal">choices: enable, disable</span></li>
        <li> <span class="li-head">associated_interface</span> - Network interface associated with address. Source system.interface.name system.zone.name. <span class="li-normal">type: str</span></li>
        <li> <span class="li-head">cache_ttl</span> - Defines the minimal TTL of individual IP addresses in FQDN cache measured in seconds. <span class="li-normal">type: int</span></li>
        <li> <span class="li-head">clearpass_spt</span> - SPT (System Posture Token) value. <span class="li-normal">type: str</span> <span class="li-normal">choices: unknown, healthy, quarantine, checkup, transient, infected</span></li>
        <li> <span class="li-head">color</span> - Color of icon on the GUI. <span class="li-normal">type: int</span></li>
        <li> <span class="li-head">comment</span> - Comment. <span class="li-normal">type: str</span></li>
        <li> <span class="li-head">country</span> - IP addresses associated to a specific country. <span class="li-normal">type: str</span></li>
        <li> <span class="li-head">end_ip</span> - Final IP address (inclusive) in the range for the address. <span class="li-normal">type: str</span></li>
        <li> <span class="li-head">end_mac</span> - Last MAC address in the range. <span class="li-normal">type: str</span></li>
        <li> <span class="li-head">epg_name</span> - Endpoint group name. <span class="li-normal">type: str</span></li>
        <li> <span class="li-head">filter</span> - Match criteria filter. <span class="li-normal">type: str</span></li>
        <li> <span class="li-head">fqdn</span> - Fully Qualified Domain Name address. <span class="li-normal">type: str</span></li>
        <li> <span class="li-head">fsso_group</span> - FSSO group(s). <span class="li-normal">type: list</span></li>
            <ul class="ul-self">
            <li> <span class="li-head">name</span> - FSSO group name. Source user.adgrp.name. <span class="li-normal">type: str</span> <span class="li-required">required: True</span></li>
            </ul>
        <li> <span class="li-head">interface</span> - Name of interface whose IP address is to be used. Source system.interface.name. <span class="li-normal">type: str</span></li>
        <li> <span class="li-head">list</span> - IP address list. <span class="li-normal">type: list</span></li>
            <ul class="ul-self">
            <li> <span class="li-head">ip</span> - IP. <span class="li-normal">type: str</span> <span class="li-required">required: True</span></li>
            </ul>
        <li> <span class="li-head">name</span> - Address name. <span class="li-normal">type: str</span> <span class="li-required">required: True</span></li>
        <li> <span class="li-head">obj_id</span> - Object ID for NSX. <span class="li-normal">type: str</span></li>
        <li> <span class="li-head">organization</span> - Organization domain name (Syntax: organization/domain). <span class="li-normal">type: str</span></li>
        <li> <span class="li-head">policy_group</span> - Policy group name. <span class="li-normal">type: str</span></li>
        <li> <span class="li-head">sdn</span> - SDN. Source system.sdn-connector.name. <span class="li-normal">type: str</span></li>
        <li> <span class="li-head">sdn_addr_type</span> - Type of addresses to collect. <span class="li-normal">type: str</span> <span class="li-normal">choices: private, public, all</span></li>
        <li> <span class="li-head">sdn_tag</span> - SDN Tag. <span class="li-normal">type: str</span></li>
        <li> <span class="li-head">start_ip</span> - First IP address (inclusive) in the range for the address. <span class="li-normal">type: str</span></li>
        <li> <span class="li-head">start_mac</span> - First MAC address in the range. <span class="li-normal">type: str</span></li>
        <li> <span class="li-head">sub_type</span> - Sub-type of address. <span class="li-normal">type: str</span> <span class="li-normal">choices: sdn, clearpass-spt, fsso, ems-tag</span></li>
        <li> <span class="li-head">subnet</span> - IP address and subnet mask of address. <span class="li-normal">type: str</span></li>
        <li> <span class="li-head">subnet_name</span> - Subnet name. <span class="li-normal">type: str</span></li>
        <li> <span class="li-head">tagging</span> - Config object tagging. <span class="li-normal">type: list</span></li>
            <ul class="ul-self">
            <li> <span class="li-head">category</span> - Tag category. Source system.object-tagging.category. <span class="li-normal">type: str</span></li>
            <li> <span class="li-head">name</span> - Tagging entry name. <span class="li-normal">type: str</span> <span class="li-required">required: True</span></li>
            <li> <span class="li-head">tags</span> - Tags. <span class="li-normal">type: list</span></li>
                <ul class="ul-self">
                <li> <span class="li-head">name</span> - Tag name. Source system.object-tagging.tags.name. <span class="li-normal">type: str</span> <span class="li-required">required: True</span></li>
                </ul>
            </ul>
        <li> <span class="li-head">tenant</span> - Tenant. <span class="li-normal">type: str</span></li>
        <li> <span class="li-head">type</span> - Type of address. <span class="li-normal">type: str</span> <span class="li-normal">choices: ipmask, iprange, fqdn, geography, wildcard, dynamic, interface-subnet, mac</span></li>
        <li> <span class="li-head">uuid</span> - Universally Unique Identifier (UUID; automatically assigned but can be manually reset). <span class="li-normal">type: str</span></li>
        <li> <span class="li-head">wildcard</span> - IP address and wildcard netmask. <span class="li-normal">type: str</span></li>
        <li> <span class="li-head">wildcard_fqdn</span> - Fully Qualified Domain Name with wildcard characters. <span class="li-normal">type: str</span></li>
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
      - name: Configure IPv4 addresses.
        fortios_firewall_address:
          vdom:  "{{ vdom }}"
          state: "present"
          access_token: "<your_own_value>"
          firewall_address:
            allow_routing: "enable"
            associated_interface: "<your_own_value> (source system.interface.name system.zone.name)"
            cache_ttl: "5"
            clearpass_spt: "unknown"
            color: "7"
            comment: "Comment."
            country: "<your_own_value>"
            end_ip: "<your_own_value>"
            end_mac: "<your_own_value>"
            epg_name: "<your_own_value>"
            filter: "<your_own_value>"
            fqdn: "<your_own_value>"
            fsso_group:
             -
                name: "default_name_16 (source user.adgrp.name)"
            interface: "<your_own_value> (source system.interface.name)"
            list:
             -
                ip: "<your_own_value>"
            name: "default_name_20"
            obj_id: "<your_own_value>"
            organization: "<your_own_value>"
            policy_group: "<your_own_value>"
            sdn: "<your_own_value> (source system.sdn-connector.name)"
            sdn_addr_type: "private"
            sdn_tag: "<your_own_value>"
            start_ip: "<your_own_value>"
            start_mac: "<your_own_value>"
            sub_type: "sdn"
            subnet: "<your_own_value>"
            subnet_name: "<your_own_value>"
            tagging:
             -
                category: "<your_own_value> (source system.object-tagging.category)"
                name: "default_name_34"
                tags:
                 -
                    name: "default_name_36 (source system.object-tagging.tags.name)"
            tenant: "<your_own_value>"
            type: "ipmask"
            uuid: "<your_own_value>"
            wildcard: "<your_own_value>"
            wildcard_fqdn: "<your_own_value>"
    


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
