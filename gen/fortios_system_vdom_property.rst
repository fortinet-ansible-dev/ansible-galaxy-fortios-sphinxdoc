:source: fortios_system_vdom_property.py

:orphan:

.. fortios_system_vdom_property:

fortios_system_vdom_property -- Configure VDOM property in Fortinet's FortiOS and FortiGate.
++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++

.. versionadded:: 2.0.0

.. contents::
   :local:
   :depth: 1


Synopsis
--------
- This module is able to configure a FortiGate or FortiOS (FOS) device by allowing the user to set and modify system feature and vdom_property category. Examples include all parameters and values need to be adjusted to datasources before usage. Tested with FOS v6.0.0



Requirements
------------
The below requirements are needed on the host that executes this module.

- ansible>=2.15


Tips
----
Using member operation to add an element to an existing object.

FortiOS Version Compatibility
-----------------------------
Supported Version Ranges: v6.0.0 -> 7.4.3



Parameters
----------


.. raw:: html

    <ul>
    <li> <span class="li-head">access_token</span> - Token-based authentication. Generated from GUI of Fortigate. <span class="li-normal">type: str</span> <span class="li-required">required: false</span> </li>
    <li> <span class="li-head">enable_log</span> - Enable/Disable logging for task. <span class="li-normal">type: bool</span> <span class="li-required">required: false</span> <span class="li-normal">default: False</span> </li>
    <li> <span class="li-head">vdom</span> - Virtual domain, among those defined previously. A vdom is a virtual instance of the FortiGate that can be configured and used as a different unit. <span class="li-normal">type: str</span> <span class="li-normal">default: root</span> </li>
    <li> <span class="li-head">member_path</span> - Member attribute path to operate on. <span class="li-normal">type: str</span> </li>
    <li> <span class="li-head">member_state</span> - Add or delete a member under specified attribute path. <span class="li-normal">type: str</span> <span class="li-normal">choices: present, absent</span> </li>
    <li> <span class="li-head">state</span> - Indicates whether to create or remove the object. <span class="li-normal">type: str</span> <span class="li-required">required: true</span> <span class="li-normal">choices: present, absent</span> </li>
    <li> <span class="li-head">system_vdom_property</span> - Configure VDOM property. <span class="li-normal">type: dict</span>
 <a id='label0' href="javascript:ContentClick('label1', 'label0');" onmouseover="ContentPreview('label1');" onmouseout="ContentUnpreview('label1');" title="click to collapse or expand..."> more... </a>
 <div id="label1" style="display:none">
 <table border="1">
 <tr>
 <td></td><td colspan="1">Supported Version Ranges</td>
 </tr>
 <tr>
 <td>system_vdom_property</td>
 <td><code class="docutils literal notranslate">v6.0.0 -> 7.4.3 </code></td>
 </tr>
 </table>
 </div>
 </li>
        <ul class="ul-self">
        <li> <span class="li-head">custom_service</span> - Maximum guaranteed number of firewall custom services. <span class="li-normal">type: list</span> </li>
        <li> <span class="li-head">description</span> - Description. <span class="li-normal">type: str</span>
 <a id='label2' href="javascript:ContentClick('label3', 'label2');" onmouseover="ContentPreview('label3');" onmouseout="ContentUnpreview('label3');" title="click to collapse or expand..."> more... </a>
 <div id="label3" style="display:none">
 <table border="1">
 <tr>
 <td></td>
 <td colspan="1">Supported Version Ranges</td>
 </tr>
 <tr>
 <td>description</td>
 <td><code class="docutils literal notranslate">v6.0.0 -> 7.4.3 </code></td>
 </tr>
 </table>
 </div>
 </li>
        <li> <span class="li-head">dialup_tunnel</span> - Maximum guaranteed number of dial-up tunnels. <span class="li-normal">type: list</span> </li>
        <li> <span class="li-head">firewall_address</span> - Maximum guaranteed number of firewall addresses (IPv4, IPv6, multicast). <span class="li-normal">type: list</span> </li>
        <li> <span class="li-head">firewall_addrgrp</span> - Maximum guaranteed number of firewall address groups (IPv4, IPv6). <span class="li-normal">type: list</span> </li>
        <li> <span class="li-head">firewall_policy</span> - Maximum guaranteed number of firewall policies (policy, DoS-policy4, DoS-policy6, multicast). <span class="li-normal">type: list</span> </li>
        <li> <span class="li-head">ipsec_phase1</span> - Maximum guaranteed number of VPN IPsec phase 1 tunnels. <span class="li-normal">type: list</span> </li>
        <li> <span class="li-head">ipsec_phase1_interface</span> - Maximum guaranteed number of VPN IPsec phase1 interface tunnels. <span class="li-normal">type: list</span> </li>
        <li> <span class="li-head">ipsec_phase2</span> - Maximum guaranteed number of VPN IPsec phase 2 tunnels. <span class="li-normal">type: list</span> </li>
        <li> <span class="li-head">ipsec_phase2_interface</span> - Maximum guaranteed number of VPN IPsec phase2 interface tunnels. <span class="li-normal">type: list</span> </li>
        <li> <span class="li-head">log_disk_quota</span> - Log disk quota in megabytes (MB). Range depends on how much disk space is available. <span class="li-normal">type: list</span> </li>
        <li> <span class="li-head">name</span> - VDOM name. Source system.vdom.name. <span class="li-normal">type: str</span> <span class="li-required">required: true</span>
 <a id='label4' href="javascript:ContentClick('label5', 'label4');" onmouseover="ContentPreview('label5');" onmouseout="ContentUnpreview('label5');" title="click to collapse or expand..."> more... </a>
 <div id="label5" style="display:none">
 <table border="1">
 <tr>
 <td></td>
 <td colspan="1">Supported Version Ranges</td>
 </tr>
 <tr>
 <td>name</td>
 <td><code class="docutils literal notranslate">v6.0.0 -> 7.4.3 </code></td>
 </tr>
 </table>
 </div>
 </li>
        <li> <span class="li-head">onetime_schedule</span> - Maximum guaranteed number of firewall one-time schedules. <span class="li-normal">type: list</span> </li>
        <li> <span class="li-head">proxy</span> - Maximum guaranteed number of concurrent proxy users. <span class="li-normal">type: list</span> </li>
        <li> <span class="li-head">recurring_schedule</span> - Maximum guaranteed number of firewall recurring schedules. <span class="li-normal">type: list</span> </li>
        <li> <span class="li-head">service_group</span> - Maximum guaranteed number of firewall service groups. <span class="li-normal">type: list</span> </li>
        <li> <span class="li-head">session</span> - Maximum guaranteed number of sessions. <span class="li-normal">type: list</span> </li>
        <li> <span class="li-head">snmp_index</span> - Permanent SNMP Index of the virtual domain (1 - 2147483647). <span class="li-normal">type: int</span>
 <a id='label6' href="javascript:ContentClick('label7', 'label6');" onmouseover="ContentPreview('label7');" onmouseout="ContentUnpreview('label7');" title="click to collapse or expand..."> more... </a>
 <div id="label7" style="display:none">
 <table border="1">
 <tr>
 <td></td>
 <td colspan="1">Supported Version Ranges</td>
 </tr>
 <tr>
 <td>snmp_index</td>
 <td><code class="docutils literal notranslate">v6.0.0 -> 7.4.3 </code></td>
 </tr>
 </table>
 </div>
 </li>
        <li> <span class="li-head">sslvpn</span> - Maximum guaranteed number of SSL-VPNs. <span class="li-normal">type: list</span> </li>
        <li> <span class="li-head">user</span> - Maximum guaranteed number of local users. <span class="li-normal">type: list</span> </li>
        <li> <span class="li-head">user_group</span> - Maximum guaranteed number of user groups. <span class="li-normal">type: list</span> </li>
        </ul>
    </ul>


Notes
-----

.. note::

   - Legacy fortiosapi has been deprecated, httpapi is the preferred way to run playbooks



Examples
--------

.. code-block:: yaml+jinja
    
    - name: Configure VDOM property.
      fortinet.fortios.fortios_system_vdom_property:
          vdom: "{{ vdom }}"
          state: "present"
          access_token: "<your_own_value>"
          system_vdom_property:
              custom_service: "<your_own_value>"
              description: "<your_own_value>"
              dialup_tunnel: "<your_own_value>"
              firewall_address: "<your_own_value>"
              firewall_addrgrp: "<your_own_value>"
              firewall_policy: "<your_own_value>"
              ipsec_phase1: "<your_own_value>"
              ipsec_phase1_interface: "<your_own_value>"
              ipsec_phase2: "<your_own_value>"
              ipsec_phase2_interface: "<your_own_value>"
              log_disk_quota: "<your_own_value>"
              name: "default_name_14 (source system.vdom.name)"
              onetime_schedule: "<your_own_value>"
              proxy: "<your_own_value>"
              recurring_schedule: "<your_own_value>"
              service_group: "<your_own_value>"
              session: "<your_own_value>"
              snmp_index: "0"
              sslvpn: "<your_own_value>"
              user: "<your_own_value>"
              user_group: "<your_own_value>"


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
