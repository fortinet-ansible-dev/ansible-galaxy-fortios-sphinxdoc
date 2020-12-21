:source: fortios_firewall_ippool.py

:orphan:

.. fortios_firewall_ippool:

fortios_firewall_ippool -- Configure IPv4 IP pools in Fortinet's FortiOS and FortiGate.
+++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++

.. versionadded:: 2.8

.. contents::
   :local:
   :depth: 1


Synopsis
--------
- This module is able to configure a FortiGate or FortiOS (FOS) device by allowing the user to set and modify firewall feature and ippool category. Examples include all parameters and values need to be adjusted to datasources before usage. Tested with FOS v6.2.0



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
    <li> <span class="li-head">firewall_ippool</span> - Configure IPv4 IP pools. <span class="li-normal">type: dict</span></li>
        <ul class="ul-self">
        <li> <span class="li-head">state</span> - B(Deprecated) <span class="li-normal">type: str</span> <span class="li-required">required: False</span> <span class="li-normal">choices: present, absent</span></li>
        <li> <span class="li-head">arp_intf</span> - Select an interface from available options that will reply to ARP requests. (If blank, any is selected). Source system.interface.name. <span class="li-normal">type: str</span></li>
        <li> <span class="li-head">arp_reply</span> - Enable/disable replying to ARP requests when an IP Pool is added to a policy . <span class="li-normal">type: str</span> <span class="li-normal">choices: disable, enable</span></li>
        <li> <span class="li-head">associated_interface</span> - Associated interface name. Source system.interface.name. <span class="li-normal">type: str</span></li>
        <li> <span class="li-head">block_size</span> - Number of addresses in a block (64 to 4096). <span class="li-normal">type: int</span></li>
        <li> <span class="li-head">comments</span> - Comment. <span class="li-normal">type: str</span></li>
        <li> <span class="li-head">endip</span> - Final IPv4 address (inclusive) in the range for the address pool (format xxx.xxx.xxx.xxx). <span class="li-normal">type: str</span></li>
        <li> <span class="li-head">name</span> - IP pool name. <span class="li-normal">type: str</span> <span class="li-required">required: True</span></li>
        <li> <span class="li-head">num_blocks_per_user</span> - Number of addresses blocks that can be used by a user (1 to 128). <span class="li-normal">type: int</span></li>
        <li> <span class="li-head">pba_timeout</span> - Port block allocation timeout (seconds). <span class="li-normal">type: int</span></li>
        <li> <span class="li-head">permit_any_host</span> - Enable/disable full cone NAT. <span class="li-normal">type: str</span> <span class="li-normal">choices: disable, enable</span></li>
        <li> <span class="li-head">source_endip</span> - Final IPv4 address (inclusive) in the range of the source addresses to be translated (format xxx.xxx.xxx.xxx). <span class="li-normal">type: str</span></li>
        <li> <span class="li-head">source_startip</span> -  First IPv4 address (inclusive) in the range of the source addresses to be translated (format xxx.xxx.xxx.xxx). <span class="li-normal">type: str</span></li>
        <li> <span class="li-head">startip</span> - First IPv4 address (inclusive) in the range for the address pool (format xxx.xxx.xxx.xxx). <span class="li-normal">type: str</span></li>
        <li> <span class="li-head">type</span> - IP pool type (overload, one-to-one, fixed port range, or port block allocation). <span class="li-normal">type: str</span> <span class="li-normal">choices: overload, one-to-one, fixed-port-range, port-block-allocation</span></li>
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
      - name: Configure IPv4 IP pools.
        fortios_firewall_ippool:
          vdom:  "{{ vdom }}"
          state: "present"
          access_token: "<your_own_value>"
          firewall_ippool:
            arp_intf: "<your_own_value> (source system.interface.name)"
            arp_reply: "disable"
            associated_interface: "<your_own_value> (source system.interface.name)"
            block_size: "6"
            comments: "<your_own_value>"
            endip: "<your_own_value>"
            name: "default_name_9"
            num_blocks_per_user: "10"
            pba_timeout: "11"
            permit_any_host: "disable"
            source_endip: "<your_own_value>"
            source_startip: "<your_own_value>"
            startip: "<your_own_value>"
            type: "overload"
    


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
