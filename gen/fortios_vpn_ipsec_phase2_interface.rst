:source: fortios_vpn_ipsec_phase2_interface.py

:orphan:

.. _fortios_vpn_ipsec_phase2_interface:

fortios_vpn_ipsec_phase2_interface -- Configure VPN autokey tunnel in Fortinet's FortiOS and FortiGate.
+++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++

.. versionadded:: 2.8

.. contents::
   :local:
   :depth: 1


Synopsis
--------
- This module is able to configure a FortiGate or FortiOS (FOS) device by allowing the user to set and modify vpn_ipsec feature and phase2_interface category. Examples include all parameters and values need to be adjusted to datasources before usage. Tested with FOS v6.0.5


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
    <li><span class="li-head">vpn_ipsec_phase2_interface</span> - Configure VPN autokey tunnel. <span class="li-normal">default: null</span> <span class="li-normal">type: dict</span></li>
            <ul class="ul-self">

            <li><span class="li-head">state</span> - B(Deprecated) Starting with Ansible 2.9 we recommend using the top-level 'state' parameter. HORIZONTALLINE Indicates whether to create or remove the object. <span class="li-normal">type: str</span> <span class="li-required">required: false</span> <span class="li-normal">choices: present,  absent</span></li>
            <li><span class="li-head">add_route</span> - Enable/disable automatic route addition. <span class="li-normal">type: str</span> <span class="li-normal">choices: phase1,  enable,  disable</span></li>
            <li><span class="li-head">auto_discovery_forwarder</span> - Enable/disable forwarding short-cut messages. <span class="li-normal">type: str</span> <span class="li-normal">choices: phase1,  enable,  disable</span></li>
            <li><span class="li-head">auto_discovery_sender</span> - Enable/disable sending short-cut messages. <span class="li-normal">type: str</span> <span class="li-normal">choices: phase1,  enable,  disable</span></li>
            <li><span class="li-head">auto_negotiate</span> - Enable/disable IPsec SA auto-negotiation. <span class="li-normal">type: str</span> <span class="li-normal">choices: enable,  disable</span></li>
            <li><span class="li-head">comments</span> - Comment. <span class="li-normal">type: str</span></li>
            <li><span class="li-head">dhcp_ipsec</span> - Enable/disable DHCP-IPsec. <span class="li-normal">type: str</span> <span class="li-normal">choices: enable,  disable</span></li>
            <li><span class="li-head">dhgrp</span> - Phase2 DH group. <span class="li-normal">type: str</span> <span class="li-normal">choices: 1,  2,  5,  14,  15,  16,  17,  18,  19,  20,  21,  27,  28,  29,  30,  31</span></li>
            <li><span class="li-head">dst_addr_type</span> - Remote proxy ID type. <span class="li-normal">type: str</span> <span class="li-normal">choices: subnet,  range,  ip,  name,  subnet6,  range6,  ip6,  name6</span></li>
            <li><span class="li-head">dst_end_ip</span> - Remote proxy ID IPv4 end. <span class="li-normal">type: str</span></li>
            <li><span class="li-head">dst_end_ip6</span> - Remote proxy ID IPv6 end. <span class="li-normal">type: str</span></li>
            <li><span class="li-head">dst_name</span> - Remote proxy ID name. Source firewall.address.name firewall.addrgrp.name. <span class="li-normal">type: str</span></li>
            <li><span class="li-head">dst_name6</span> - Remote proxy ID name. Source firewall.address6.name firewall.addrgrp6.name. <span class="li-normal">type: str</span></li>
            <li><span class="li-head">dst_port</span> - Quick mode destination port (1 - 65535 or 0 for all). <span class="li-normal">type: int</span></li>
            <li><span class="li-head">dst_start_ip</span> - Remote proxy ID IPv4 start. <span class="li-normal">type: str</span></li>
            <li><span class="li-head">dst_start_ip6</span> - Remote proxy ID IPv6 start. <span class="li-normal">type: str</span></li>
            <li><span class="li-head">dst_subnet</span> - Remote proxy ID IPv4 subnet. <span class="li-normal">type: str</span></li>
            <li><span class="li-head">dst_subnet6</span> - Remote proxy ID IPv6 subnet. <span class="li-normal">type: str</span></li>
            <li><span class="li-head">encapsulation</span> - ESP encapsulation mode. <span class="li-normal">type: str</span> <span class="li-normal">choices: tunnel-mode,  transport-mode</span></li>
            <li><span class="li-head">keepalive</span> - Enable/disable keep alive. <span class="li-normal">type: str</span> <span class="li-normal">choices: enable,  disable</span></li>
            <li><span class="li-head">keylife_type</span> - Keylife type. <span class="li-normal">type: str</span> <span class="li-normal">choices: seconds,  kbs,  both</span></li>
            <li><span class="li-head">keylifekbs</span> - Phase2 key life in number of bytes of traffic (5120 - 4294967295). <span class="li-normal">type: int</span></li>
            <li><span class="li-head">keylifeseconds</span> - Phase2 key life in time in seconds (120 - 172800). <span class="li-normal">type: int</span></li>
            <li><span class="li-head">l2tp</span> - Enable/disable L2TP over IPsec. <span class="li-normal">type: str</span> <span class="li-normal">choices: enable,  disable</span></li>
            <li><span class="li-head">name</span> - IPsec tunnel name. <span class="li-required">required</span> <span class="li-normal">type: str</span></li>
            <li><span class="li-head">pfs</span> - Enable/disable PFS feature. <span class="li-normal">type: str</span> <span class="li-normal">choices: enable,  disable</span></li>
            <li><span class="li-head">phase1name</span> - Phase 1 determines the options required for phase 2. Source vpn.ipsec.phase1-interface.name. <span class="li-normal">type: str</span></li>
            <li><span class="li-head">proposal</span> - Phase2 proposal. <span class="li-normal">type: str</span> <span class="li-normal">choices: null-md5,  null-sha1,  null-sha256,  null-sha384,  null-sha512,  des-null,  des-md5,  des-sha1,  des-sha256,  des-sha384,  des-sha512</span></li>
            <li><span class="li-head">protocol</span> - Quick mode protocol selector (1 - 255 or 0 for all). <span class="li-normal">type: int</span></li>
            <li><span class="li-head">replay</span> - Enable/disable replay detection. <span class="li-normal">type: str</span> <span class="li-normal">choices: enable,  disable</span></li>
            <li><span class="li-head">route_overlap</span> - Action for overlapping routes. <span class="li-normal">type: str</span> <span class="li-normal">choices: use-old,  use-new,  allow</span></li>
            <li><span class="li-head">single_source</span> - Enable/disable single source IP restriction. <span class="li-normal">type: str</span> <span class="li-normal">choices: enable,  disable</span></li>
            <li><span class="li-head">src_addr_type</span> - Local proxy ID type. <span class="li-normal">type: str</span> <span class="li-normal">choices: subnet,  range,  ip,  name,  subnet6,  range6,  ip6,  name6</span></li>
            <li><span class="li-head">src_end_ip</span> - Local proxy ID end. <span class="li-normal">type: str</span></li>
            <li><span class="li-head">src_end_ip6</span> - Local proxy ID IPv6 end. <span class="li-normal">type: str</span></li>
            <li><span class="li-head">src_name</span> - Local proxy ID name. Source firewall.address.name firewall.addrgrp.name. <span class="li-normal">type: str</span></li>
            <li><span class="li-head">src_name6</span> - Local proxy ID name. Source firewall.address6.name firewall.addrgrp6.name. <span class="li-normal">type: str</span></li>
            <li><span class="li-head">src_port</span> - Quick mode source port (1 - 65535 or 0 for all). <span class="li-normal">type: int</span></li>
            <li><span class="li-head">src_start_ip</span> - Local proxy ID start. <span class="li-normal">type: str</span></li>
            <li><span class="li-head">src_start_ip6</span> - Local proxy ID IPv6 start. <span class="li-normal">type: str</span></li>
            <li><span class="li-head">src_subnet</span> - Local proxy ID subnet. <span class="li-normal">type: str</span></li>
            <li><span class="li-head">src_subnet6</span> - Local proxy ID IPv6 subnet. <span class="li-normal">type: str</span>
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
      - name: Configure VPN autokey tunnel.
        fortios_vpn_ipsec_phase2_interface:
          host:  "{{ host }}"
          username: "{{ username }}"
          password: "{{ password }}"
          vdom:  "{{ vdom }}"
          https: "False"
          state: "present"
          vpn_ipsec_phase2_interface:
            add_route: "phase1"
            auto_discovery_forwarder: "phase1"
            auto_discovery_sender: "phase1"
            auto_negotiate: "enable"
            comments: "<your_own_value>"
            dhcp_ipsec: "enable"
            dhgrp: "1"
            dst_addr_type: "subnet"
            dst_end_ip: "<your_own_value>"
            dst_end_ip6: "<your_own_value>"
            dst_name: "<your_own_value> (source firewall.address.name firewall.addrgrp.name)"
            dst_name6: "<your_own_value> (source firewall.address6.name firewall.addrgrp6.name)"
            dst_port: "15"
            dst_start_ip: "<your_own_value>"
            dst_start_ip6: "<your_own_value>"
            dst_subnet: "<your_own_value>"
            dst_subnet6: "<your_own_value>"
            encapsulation: "tunnel-mode"
            keepalive: "enable"
            keylife_type: "seconds"
            keylifekbs: "23"
            keylifeseconds: "24"
            l2tp: "enable"
            name: "default_name_26"
            pfs: "enable"
            phase1name: "<your_own_value> (source vpn.ipsec.phase1-interface.name)"
            proposal: "null-md5"
            protocol: "30"
            replay: "enable"
            route_overlap: "use-old"
            single_source: "enable"
            src_addr_type: "subnet"
            src_end_ip: "<your_own_value>"
            src_end_ip6: "<your_own_value>"
            src_name: "<your_own_value> (source firewall.address.name firewall.addrgrp.name)"
            src_name6: "<your_own_value> (source firewall.address6.name firewall.addrgrp6.name)"
            src_port: "39"
            src_start_ip: "<your_own_value>"
            src_start_ip6: "<your_own_value>"
            src_subnet: "<your_own_value>"
            src_subnet6: "<your_own_value>"



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