:source: fortios_system_vxlan.py

:orphan:

.. fortios_system_vxlan:

fortios_system_vxlan -- Configure VXLAN devices in Fortinet's FortiOS and FortiGate.
++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++

.. versionadded:: 2.9

.. contents::
   :local:
   :depth: 1


Synopsis
--------
- This module is able to configure a FortiGate or FortiOS (FOS) device by allowing the user to set and modify system feature and vxlan category. Examples include all parameters and values need to be adjusted to datasources before usage. Tested with FOS v6.0.0



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
    <li> <span class="li-head">system_vxlan</span> - Configure VXLAN devices. <span class="li-normal">type: dict</span></li>
        <ul class="ul-self">
        <li> <span class="li-head">dstport</span> - VXLAN destination port (1 - 65535). <span class="li-normal">type: int</span></li>
        <li> <span class="li-head">interface</span> - Outgoing interface for VXLAN encapsulated traffic. Source system.interface.name. <span class="li-normal">type: str</span></li>
        <li> <span class="li-head">ip_version</span> - IP version to use for the VXLAN interface and so for communication over the VXLAN. IPv4 or IPv6 unicast or multicast. <span class="li-normal">type: str</span> <span class="li-normal">choices: ipv4-unicast, ipv6-unicast, ipv4-multicast, ipv6-multicast</span></li>
        <li> <span class="li-head">multicast_ttl</span> - VXLAN multicast TTL (1-255). <span class="li-normal">type: int</span></li>
        <li> <span class="li-head">name</span> - VXLAN device or interface name. Must be a unique interface name. <span class="li-normal">type: str</span> <span class="li-required">required: True</span></li>
        <li> <span class="li-head">remote_ip</span> - IPv4 address of the VXLAN interface on the device at the remote end of the VXLAN. <span class="li-normal">type: list</span></li>
            <ul class="ul-self">
            <li> <span class="li-head">ip</span> - IPv4 address. <span class="li-normal">type: str</span> <span class="li-required">required: True</span></li>
            </ul>
        <li> <span class="li-head">remote_ip6</span> - IPv6 IP address of the VXLAN interface on the device at the remote end of the VXLAN. <span class="li-normal">type: list</span></li>
            <ul class="ul-self">
            <li> <span class="li-head">ip6</span> - IPv6 address. <span class="li-normal">type: str</span> <span class="li-required">required: True</span></li>
            </ul>
        <li> <span class="li-head">vni</span> - VXLAN network ID. <span class="li-normal">type: int</span></li>
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
      - name: Configure VXLAN devices.
        fortios_system_vxlan:
          vdom:  "{{ vdom }}"
          state: "present"
          access_token: "<your_own_value>"
          system_vxlan:
            dstport: "3"
            interface: "<your_own_value> (source system.interface.name)"
            ip_version: "ipv4-unicast"
            multicast_ttl: "6"
            name: "default_name_7"
            remote_ip:
             -
                ip: "<your_own_value>"
            remote_ip6:
             -
                ip6: "<your_own_value>"
            vni: "12"
    


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
