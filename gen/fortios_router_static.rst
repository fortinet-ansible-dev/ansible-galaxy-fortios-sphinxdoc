:source: fortios_router_static.py

:orphan:

.. fortios_router_static:

fortios_router_static -- Configure IPv4 static routing tables in Fortinet's FortiOS and FortiGate.
++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++

.. versionadded:: 2.8

.. contents::
   :local:
   :depth: 1


Synopsis
--------
- This module is able to configure a FortiGate or FortiOS (FOS) device by allowing the user to set and modify router feature and static category. Examples include all parameters and values need to be adjusted to datasources before usage. Tested with FOS v6.0.0



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
    <li> <span class="li-head">router_static</span> - Configure IPv4 static routing tables. <span class="li-normal">type: dict</span></li>
        <ul class="ul-self">
        <li> <span class="li-head">state</span> - B(Deprecated) <span class="li-normal">type: str</span> <span class="li-required">required: False</span> <span class="li-normal">choices: present, absent</span></li>
        <li> <span class="li-head">bfd</span> - Enable/disable Bidirectional Forwarding Detection (BFD). <span class="li-normal">type: str</span> <span class="li-normal">choices: enable, disable</span></li>
        <li> <span class="li-head">blackhole</span> - Enable/disable black hole. <span class="li-normal">type: str</span> <span class="li-normal">choices: enable, disable</span></li>
        <li> <span class="li-head">comment</span> - Optional comments. <span class="li-normal">type: str</span></li>
        <li> <span class="li-head">device</span> - Gateway out interface or tunnel. Source system.interface.name. <span class="li-normal">type: str</span></li>
        <li> <span class="li-head">distance</span> - Administrative distance (1 - 255). <span class="li-normal">type: int</span></li>
        <li> <span class="li-head">dst</span> - Destination IP and mask for this route. <span class="li-normal">type: str</span></li>
        <li> <span class="li-head">dstaddr</span> - Name of firewall address or address group. Source firewall.address.name firewall.addrgrp.name. <span class="li-normal">type: str</span></li>
        <li> <span class="li-head">dynamic_gateway</span> - Enable use of dynamic gateway retrieved from a DHCP or PPP server. <span class="li-normal">type: str</span> <span class="li-normal">choices: enable, disable</span></li>
        <li> <span class="li-head">gateway</span> - Gateway IP for this route. <span class="li-normal">type: str</span></li>
        <li> <span class="li-head">internet_service</span> - Application ID in the Internet service database. Source firewall.internet-service.id. <span class="li-normal">type: int</span></li>
        <li> <span class="li-head">internet_service_custom</span> - Application name in the Internet service custom database. Source firewall.internet-service-custom.name. <span class="li-normal">type: str</span></li>
        <li> <span class="li-head">link_monitor_exempt</span> - Enable/disable withdrawing this route when link monitor or health check is down. <span class="li-normal">type: str</span> <span class="li-normal">choices: enable, disable</span></li>
        <li> <span class="li-head">priority</span> - Administrative priority (0 - 4294967295). <span class="li-normal">type: int</span></li>
        <li> <span class="li-head">seq_num</span> - Sequence number. <span class="li-normal">type: int</span></li>
        <li> <span class="li-head">src</span> - Source prefix for this route. <span class="li-normal">type: str</span></li>
        <li> <span class="li-head">status</span> - Enable/disable this static route. <span class="li-normal">type: str</span> <span class="li-normal">choices: enable, disable</span></li>
        <li> <span class="li-head">virtual_wan_link</span> - Enable/disable egress through the virtual-wan-link. <span class="li-normal">type: str</span> <span class="li-normal">choices: enable, disable</span></li>
        <li> <span class="li-head">vrf</span> - Virtual Routing Forwarding ID. <span class="li-normal">type: int</span></li>
        <li> <span class="li-head">weight</span> - Administrative weight (0 - 255). <span class="li-normal">type: int</span></li>
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
      - name: Configure IPv4 static routing tables.
        fortios_router_static:
          vdom:  "{{ vdom }}"
          state: "present"
          access_token: "<your_own_value>"
          router_static:
            bfd: "enable"
            blackhole: "enable"
            comment: "Optional comments."
            device: "<your_own_value> (source system.interface.name)"
            distance: "7"
            dst: "<your_own_value>"
            dstaddr: "<your_own_value> (source firewall.address.name firewall.addrgrp.name)"
            dynamic_gateway: "enable"
            gateway: "<your_own_value>"
            internet_service: "12 (source firewall.internet-service.id)"
            internet_service_custom: "<your_own_value> (source firewall.internet-service-custom.name)"
            link_monitor_exempt: "enable"
            priority: "15"
            seq_num: "16"
            src: "<your_own_value>"
            status: "enable"
            virtual_wan_link: "enable"
            vrf: "20"
            weight: "21"
    


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
