:source: fortios_system_sdn_vpn.py

:orphan:

.. fortios_system_sdn_vpn:

fortios_system_sdn_vpn -- Configure public cloud VPN service in Fortinet's FortiOS and FortiGate.
+++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++

.. versionadded:: 2.0.0

.. contents::
   :local:
   :depth: 1


Synopsis
--------
- This module is able to configure a FortiGate or FortiOS (FOS) device by allowing the user to set and modify system feature and sdn_vpn category. Examples include all parameters and values need to be adjusted to datasources before usage. Tested with FOS v6.0.0



Requirements
------------
The below requirements are needed on the host that executes this module.

- ansible>=2.15


Tips
----
Using member operation to add an element to an existing object.

FortiOS Version Compatibility
-----------------------------
Supported Version Ranges: v7.6.1 -> v7.6.4


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
    <li> <span class="li-head">system_sdn_vpn</span> - Configure public cloud VPN service. <span class="li-normal">type: dict</span>
 <a id='label0' href="javascript:ContentClick('label1', 'label0');" onmouseover="ContentPreview('label1');" onmouseout="ContentUnpreview('label1');" title="click to collapse or expand..."> more... </a>
 <div id="label1" style="display:none">
 <table border="1">
 <tr>
 <td></td><td colspan="1">Supported Version Ranges</td>
 </tr>
 <tr>
 <td>system_sdn_vpn</td>
 <td><code class="docutils literal notranslate">v7.6.1 -> 7.6.4 </code></td>
 </tr>
 </table>
 </div>
 </li>
        <ul class="ul-self">
        <li> <span class="li-head">bgp_as</span> - BGP Router AS number. <span class="li-normal">type: int</span>
 <a id='label2' href="javascript:ContentClick('label3', 'label2');" onmouseover="ContentPreview('label3');" onmouseout="ContentUnpreview('label3');" title="click to collapse or expand..."> more... </a>
 <div id="label3" style="display:none">
 <table border="1">
 <tr>
 <td></td>
 <td colspan="1">Supported Version Ranges</td>
 </tr>
 <tr>
 <td>bgp_as</td>
 <td><code class="docutils literal notranslate">v7.6.1 -> 7.6.4 </code></td>
 </tr>
 </table>
 </div>
 </li>
        <li> <span class="li-head">cgw_gateway</span> - Public IP address of the customer gateway. <span class="li-normal">type: str</span>
 <a id='label4' href="javascript:ContentClick('label5', 'label4');" onmouseover="ContentPreview('label5');" onmouseout="ContentUnpreview('label5');" title="click to collapse or expand..."> more... </a>
 <div id="label5" style="display:none">
 <table border="1">
 <tr>
 <td></td>
 <td colspan="1">Supported Version Ranges</td>
 </tr>
 <tr>
 <td>cgw_gateway</td>
 <td><code class="docutils literal notranslate">v7.6.1 -> 7.6.4 </code></td>
 </tr>
 </table>
 </div>
 </li>
        <li> <span class="li-head">cgw_name</span> - AWS customer gateway name to be created. <span class="li-normal">type: str</span>
 <a id='label6' href="javascript:ContentClick('label7', 'label6');" onmouseover="ContentPreview('label7');" onmouseout="ContentUnpreview('label7');" title="click to collapse or expand..."> more... </a>
 <div id="label7" style="display:none">
 <table border="1">
 <tr>
 <td></td>
 <td colspan="1">Supported Version Ranges</td>
 </tr>
 <tr>
 <td>cgw_name</td>
 <td><code class="docutils literal notranslate">v7.6.1 -> 7.6.4 </code></td>
 </tr>
 </table>
 </div>
 </li>
        <li> <span class="li-head">internal_interface</span> - Internal interface with local subnet. Source system.interface.name. <span class="li-normal">type: str</span>
 <a id='label8' href="javascript:ContentClick('label9', 'label8');" onmouseover="ContentPreview('label9');" onmouseout="ContentUnpreview('label9');" title="click to collapse or expand..."> more... </a>
 <div id="label9" style="display:none">
 <table border="1">
 <tr>
 <td></td>
 <td colspan="1">Supported Version Ranges</td>
 </tr>
 <tr>
 <td>internal_interface</td>
 <td><code class="docutils literal notranslate">v7.6.1 -> 7.6.4 </code></td>
 </tr>
 </table>
 </div>
 </li>
        <li> <span class="li-head">local_cidr</span> - Local subnet address and subnet mask. <span class="li-normal">type: str</span>
 <a id='label10' href="javascript:ContentClick('label11', 'label10');" onmouseover="ContentPreview('label11');" onmouseout="ContentUnpreview('label11');" title="click to collapse or expand..."> more... </a>
 <div id="label11" style="display:none">
 <table border="1">
 <tr>
 <td></td>
 <td colspan="1">Supported Version Ranges</td>
 </tr>
 <tr>
 <td>local_cidr</td>
 <td><code class="docutils literal notranslate">v7.6.1 -> 7.6.4 </code></td>
 </tr>
 </table>
 </div>
 </li>
        <li> <span class="li-head">name</span> - Public cloud VPN name. <span class="li-normal">type: str</span> <span class="li-required">required: true</span>
 <a id='label12' href="javascript:ContentClick('label13', 'label12');" onmouseover="ContentPreview('label13');" onmouseout="ContentUnpreview('label13');" title="click to collapse or expand..."> more... </a>
 <div id="label13" style="display:none">
 <table border="1">
 <tr>
 <td></td>
 <td colspan="1">Supported Version Ranges</td>
 </tr>
 <tr>
 <td>name</td>
 <td><code class="docutils literal notranslate">v7.6.1 -> 7.6.4 </code></td>
 </tr>
 </table>
 </div>
 </li>
        <li> <span class="li-head">nat_traversal</span> - Enable/disable use for NAT traversal. Please enable if your FortiGate device is behind a NAT/PAT device. <span class="li-normal">type: str</span> <span class="li-normal">choices: disable, enable</span>
 <a id='label14' href="javascript:ContentClick('label15', 'label14');" onmouseover="ContentPreview('label15');" onmouseout="ContentUnpreview('label15');" title="click to collapse or expand..."> more... </a>
 <div id="label15" style="display:none">
 <table border="1">
 <tr>
 <td></td>
 <td colspan="1">Supported Version Ranges</td>
 </tr>
 <tr>
 <td>nat_traversal</td>
 <td><code class="docutils literal notranslate">v7.6.1 -> 7.6.4 </code></td>
 </tr>
 <tr>
 <td>[disable]</td>
 <td><code class="docutils literal notranslate">v7.6.1 -> 7.6.4</code></td>
 <tr>
 <td>[enable]</td>
 <td><code class="docutils literal notranslate">v7.6.1 -> 7.6.4</code></td>
 </table>
 </div>
 </li>
        <li> <span class="li-head">psksecret</span> - Pre-shared secret for PSK authentication. Auto-generated if not specified <span class="li-normal">type: str</span>
 <a id='label16' href="javascript:ContentClick('label17', 'label16');" onmouseover="ContentPreview('label17');" onmouseout="ContentUnpreview('label17');" title="click to collapse or expand..."> more... </a>
 <div id="label17" style="display:none">
 <table border="1">
 <tr>
 <td></td>
 <td colspan="1">Supported Version Ranges</td>
 </tr>
 <tr>
 <td>psksecret</td>
 <td><code class="docutils literal notranslate">v7.6.1 -> 7.6.4 </code></td>
 </tr>
 </table>
 </div>
 </li>
        <li> <span class="li-head">remote_cidr</span> - Remote subnet address and subnet mask. <span class="li-normal">type: str</span>
 <a id='label18' href="javascript:ContentClick('label19', 'label18');" onmouseover="ContentPreview('label19');" onmouseout="ContentUnpreview('label19');" title="click to collapse or expand..."> more... </a>
 <div id="label19" style="display:none">
 <table border="1">
 <tr>
 <td></td>
 <td colspan="1">Supported Version Ranges</td>
 </tr>
 <tr>
 <td>remote_cidr</td>
 <td><code class="docutils literal notranslate">v7.6.1 -> 7.6.4 </code></td>
 </tr>
 </table>
 </div>
 </li>
        <li> <span class="li-head">remote_type</span> - Type of remote device. <span class="li-normal">type: str</span> <span class="li-normal">choices: vgw, tgw</span>
 <a id='label20' href="javascript:ContentClick('label21', 'label20');" onmouseover="ContentPreview('label21');" onmouseout="ContentUnpreview('label21');" title="click to collapse or expand..."> more... </a>
 <div id="label21" style="display:none">
 <table border="1">
 <tr>
 <td></td>
 <td colspan="1">Supported Version Ranges</td>
 </tr>
 <tr>
 <td>remote_type</td>
 <td><code class="docutils literal notranslate">v7.6.1 -> 7.6.4 </code></td>
 </tr>
 <tr>
 <td>[vgw]</td>
 <td><code class="docutils literal notranslate">v7.6.1 -> 7.6.4</code></td>
 <tr>
 <td>[tgw]</td>
 <td><code class="docutils literal notranslate">v7.6.1 -> 7.6.4</code></td>
 </table>
 </div>
 </li>
        <li> <span class="li-head">routing_type</span> - Type of routing. <span class="li-normal">type: str</span> <span class="li-normal">choices: static, dynamic</span>
 <a id='label22' href="javascript:ContentClick('label23', 'label22');" onmouseover="ContentPreview('label23');" onmouseout="ContentUnpreview('label23');" title="click to collapse or expand..."> more... </a>
 <div id="label23" style="display:none">
 <table border="1">
 <tr>
 <td></td>
 <td colspan="1">Supported Version Ranges</td>
 </tr>
 <tr>
 <td>routing_type</td>
 <td><code class="docutils literal notranslate">v7.6.1 -> 7.6.4 </code></td>
 </tr>
 <tr>
 <td>[static]</td>
 <td><code class="docutils literal notranslate">v7.6.1 -> 7.6.4</code></td>
 <tr>
 <td>[dynamic]</td>
 <td><code class="docutils literal notranslate">v7.6.1 -> 7.6.4</code></td>
 </table>
 </div>
 </li>
        <li> <span class="li-head">sdn</span> - SDN connector name. Source system.sdn-connector.name. <span class="li-normal">type: str</span>
 <a id='label24' href="javascript:ContentClick('label25', 'label24');" onmouseover="ContentPreview('label25');" onmouseout="ContentUnpreview('label25');" title="click to collapse or expand..."> more... </a>
 <div id="label25" style="display:none">
 <table border="1">
 <tr>
 <td></td>
 <td colspan="1">Supported Version Ranges</td>
 </tr>
 <tr>
 <td>sdn</td>
 <td><code class="docutils literal notranslate">v7.6.1 -> 7.6.4 </code></td>
 </tr>
 </table>
 </div>
 </li>
        <li> <span class="li-head">subnet_id</span> - AWS subnet id for TGW route propagation. <span class="li-normal">type: str</span>
 <a id='label26' href="javascript:ContentClick('label27', 'label26');" onmouseover="ContentPreview('label27');" onmouseout="ContentUnpreview('label27');" title="click to collapse or expand..."> more... </a>
 <div id="label27" style="display:none">
 <table border="1">
 <tr>
 <td></td>
 <td colspan="1">Supported Version Ranges</td>
 </tr>
 <tr>
 <td>subnet_id</td>
 <td><code class="docutils literal notranslate">v7.6.1 -> 7.6.4 </code></td>
 </tr>
 </table>
 </div>
 </li>
        <li> <span class="li-head">tgw_id</span> - Transit gateway id. <span class="li-normal">type: str</span>
 <a id='label28' href="javascript:ContentClick('label29', 'label28');" onmouseover="ContentPreview('label29');" onmouseout="ContentUnpreview('label29');" title="click to collapse or expand..."> more... </a>
 <div id="label29" style="display:none">
 <table border="1">
 <tr>
 <td></td>
 <td colspan="1">Supported Version Ranges</td>
 </tr>
 <tr>
 <td>tgw_id</td>
 <td><code class="docutils literal notranslate">v7.6.1 -> 7.6.4 </code></td>
 </tr>
 </table>
 </div>
 </li>
        <li> <span class="li-head">tunnel_interface</span> - Tunnel interface with public IP. Source system.interface.name. <span class="li-normal">type: str</span>
 <a id='label30' href="javascript:ContentClick('label31', 'label30');" onmouseover="ContentPreview('label31');" onmouseout="ContentUnpreview('label31');" title="click to collapse or expand..."> more... </a>
 <div id="label31" style="display:none">
 <table border="1">
 <tr>
 <td></td>
 <td colspan="1">Supported Version Ranges</td>
 </tr>
 <tr>
 <td>tunnel_interface</td>
 <td><code class="docutils literal notranslate">v7.6.1 -> 7.6.4 </code></td>
 </tr>
 </table>
 </div>
 </li>
        <li> <span class="li-head">vgw_id</span> - Virtual private gateway id. <span class="li-normal">type: str</span>
 <a id='label32' href="javascript:ContentClick('label33', 'label32');" onmouseover="ContentPreview('label33');" onmouseout="ContentUnpreview('label33');" title="click to collapse or expand..."> more... </a>
 <div id="label33" style="display:none">
 <table border="1">
 <tr>
 <td></td>
 <td colspan="1">Supported Version Ranges</td>
 </tr>
 <tr>
 <td>vgw_id</td>
 <td><code class="docutils literal notranslate">v7.6.1 -> 7.6.4 </code></td>
 </tr>
 </table>
 </div>
 </li>
        </ul>
    </ul>


Notes
-----

.. note::

   - Legacy fortiosapi has been deprecated, httpapi is the preferred way to run playbooks



Examples
--------

.. code-block:: yaml+jinja
    
    - name: Configure public cloud VPN service.
      fortinet.fortios.fortios_system_sdn_vpn:
          vdom: "{{ vdom }}"
          state: "present"
          access_token: "<your_own_value>"
          system_sdn_vpn:
              bgp_as: "65000"
              cgw_gateway: "<your_own_value>"
              cgw_name: "<your_own_value>"
              internal_interface: "<your_own_value> (source system.interface.name)"
              local_cidr: "<your_own_value>"
              name: "default_name_8"
              nat_traversal: "disable"
              psksecret: "<your_own_value>"
              remote_cidr: "<your_own_value>"
              remote_type: "vgw"
              routing_type: "static"
              sdn: "<your_own_value> (source system.sdn-connector.name)"
              subnet_id: "<your_own_value>"
              tgw_id: "<your_own_value>"
              tunnel_interface: "<your_own_value> (source system.interface.name)"
              vgw_id: "<your_own_value>"


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
