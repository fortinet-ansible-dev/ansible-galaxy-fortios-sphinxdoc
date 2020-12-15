:source: fortios_system_dhcp6_server.py

:orphan:

.. fortios_system_dhcp6_server:

fortios_system_dhcp6_server -- Configure DHCPv6 servers in Fortinet's FortiOS and FortiGate.
++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++

.. versionadded:: 2.9

.. contents::
   :local:
   :depth: 1


Synopsis
--------
- This module is able to configure a FortiGate or FortiOS (FOS) device by allowing the user to set and modify system_dhcp6 feature and server category. Examples include all parameters and values need to be adjusted to datasources before usage. Tested with FOS v6.0.0



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
    <li> <span class="li-head">system_dhcp6_server</span> - Configure DHCPv6 servers. <span class="li-normal">type: dict</span></li>
        <ul class="ul-self">
        <li> <span class="li-head">dns_search_list</span> - DNS search list options. <span class="li-normal">type: str</span> <span class="li-normal">choices: delegated, specify</span></li>
        <li> <span class="li-head">dns_server1</span> - DNS server 1. <span class="li-normal">type: str</span></li>
        <li> <span class="li-head">dns_server2</span> - DNS server 2. <span class="li-normal">type: str</span></li>
        <li> <span class="li-head">dns_server3</span> - DNS server 3. <span class="li-normal">type: str</span></li>
        <li> <span class="li-head">dns_service</span> - Options for assigning DNS servers to DHCPv6 clients. <span class="li-normal">type: str</span> <span class="li-normal">choices: delegated, default, specify</span></li>
        <li> <span class="li-head">domain</span> - Domain name suffix for the IP addresses that the DHCP server assigns to clients. <span class="li-normal">type: str</span></li>
        <li> <span class="li-head">id</span> - ID. <span class="li-normal">type: int</span> <span class="li-required">required: True</span></li>
        <li> <span class="li-head">interface</span> - DHCP server can assign IP configurations to clients connected to this interface. Source system.interface.name. <span class="li-normal">type: str</span></li>
        <li> <span class="li-head">ip_mode</span> - Method used to assign client IP. <span class="li-normal">type: str</span> <span class="li-normal">choices: range, delegated</span></li>
        <li> <span class="li-head">ip_range</span> - DHCP IP range configuration. <span class="li-normal">type: list</span></li>
            <ul class="ul-self">
            <li> <span class="li-head">end_ip</span> - End of IP range. <span class="li-normal">type: str</span></li>
            <li> <span class="li-head">id</span> - ID. <span class="li-normal">type: int</span> <span class="li-required">required: True</span></li>
            <li> <span class="li-head">start_ip</span> - Start of IP range. <span class="li-normal">type: str</span></li>
            </ul>
        <li> <span class="li-head">lease_time</span> - Lease time in seconds, 0 means unlimited. <span class="li-normal">type: int</span></li>
        <li> <span class="li-head">option1</span> - Option 1. <span class="li-normal">type: str</span></li>
        <li> <span class="li-head">option2</span> - Option 2. <span class="li-normal">type: str</span></li>
        <li> <span class="li-head">option3</span> - Option 3. <span class="li-normal">type: str</span></li>
        <li> <span class="li-head">prefix_range</span> - DHCP prefix configuration. <span class="li-normal">type: list</span></li>
            <ul class="ul-self">
            <li> <span class="li-head">end_prefix</span> - End of prefix range. <span class="li-normal">type: str</span></li>
            <li> <span class="li-head">id</span> - ID. <span class="li-normal">type: int</span> <span class="li-required">required: True</span></li>
            <li> <span class="li-head">prefix_length</span> - Prefix length. <span class="li-normal">type: int</span></li>
            <li> <span class="li-head">start_prefix</span> - Start of prefix range. <span class="li-normal">type: str</span></li>
            </ul>
        <li> <span class="li-head">rapid_commit</span> - Enable/disable allow/disallow rapid commit. <span class="li-normal">type: str</span> <span class="li-normal">choices: disable, enable</span></li>
        <li> <span class="li-head">status</span> - Enable/disable this DHCPv6 configuration. <span class="li-normal">type: str</span> <span class="li-normal">choices: disable, enable</span></li>
        <li> <span class="li-head">subnet</span> - Subnet or subnet-id if the IP mode is delegated. <span class="li-normal">type: str</span></li>
        <li> <span class="li-head">upstream_interface</span> - Interface name from where delegated information is provided. Source system.interface.name. <span class="li-normal">type: str</span></li>
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
      - name: Configure DHCPv6 servers.
        fortios_system_dhcp6_server:
          vdom:  "{{ vdom }}"
          state: "present"
          access_token: "<your_own_value>"
          system_dhcp6_server:
            dns_search_list: "delegated"
            dns_server1: "<your_own_value>"
            dns_server2: "<your_own_value>"
            dns_server3: "<your_own_value>"
            dns_service: "delegated"
            domain: "<your_own_value>"
            id:  "9"
            interface: "<your_own_value> (source system.interface.name)"
            ip_mode: "range"
            ip_range:
             -
                end_ip: "<your_own_value>"
                id:  "14"
                start_ip: "<your_own_value>"
            lease_time: "16"
            option1: "<your_own_value>"
            option2: "<your_own_value>"
            option3: "<your_own_value>"
            prefix_range:
             -
                end_prefix: "<your_own_value>"
                id:  "22"
                prefix_length: "23"
                start_prefix: "<your_own_value>"
            rapid_commit: "disable"
            status: "disable"
            subnet: "<your_own_value>"
            upstream_interface: "<your_own_value> (source system.interface.name)"
    


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
