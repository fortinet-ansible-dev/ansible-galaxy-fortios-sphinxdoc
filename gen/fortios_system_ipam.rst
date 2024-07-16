:source: fortios_system_ipam.py

:orphan:

.. fortios_system_ipam:

fortios_system_ipam -- Configure IP address management services in Fortinet's FortiOS and FortiGate.
++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++

.. versionadded:: 2.0.0

.. contents::
   :local:
   :depth: 1


Synopsis
--------
- This module is able to configure a FortiGate or FortiOS (FOS) device by allowing the user to set and modify system feature and ipam category. Examples include all parameters and values need to be adjusted to datasources before usage. Tested with FOS v6.0.0



Requirements
------------
The below requirements are needed on the host that executes this module.

- ansible>=2.15


Tips
----
Using member operation to add an element to an existing object.

FortiOS Version Compatibility
-----------------------------
Supported Version Ranges: v7.0.2 -> v7.4.4


Parameters
----------


.. raw:: html

    <ul>
    <li> <span class="li-head">access_token</span> - Token-based authentication. Generated from GUI of Fortigate. <span class="li-normal">type: str</span> <span class="li-required">required: false</span> </li>
    <li> <span class="li-head">enable_log</span> - Enable/Disable logging for task. <span class="li-normal">type: bool</span> <span class="li-required">required: false</span> <span class="li-normal">default: False</span> </li>
    <li> <span class="li-head">vdom</span> - Virtual domain, among those defined previously. A vdom is a virtual instance of the FortiGate that can be configured and used as a different unit. <span class="li-normal">type: str</span> <span class="li-normal">default: root</span> </li>
    <li> <span class="li-head">member_path</span> - Member attribute path to operate on. <span class="li-normal">type: str</span> </li>
    <li> <span class="li-head">member_state</span> - Add or delete a member under specified attribute path. <span class="li-normal">type: str</span> <span class="li-normal">choices: present, absent</span> </li>
    <li> <span class="li-head">system_ipam</span> - Configure IP address management services. <span class="li-normal">type: dict</span>
 <a id='label0' href="javascript:ContentClick('label1', 'label0');" onmouseover="ContentPreview('label1');" onmouseout="ContentUnpreview('label1');" title="click to collapse or expand..."> more... </a>
 <div id="label1" style="display:none">
 <table border="1">
 <tr>
 <td></td><td colspan="1">Supported Version Ranges</td>
 </tr>
 <tr>
 <td>system_ipam</td>
 <td><code class="docutils literal notranslate">v7.0.2 -> 7.4.4 </code></td>
 </tr>
 </table>
 </div>
 </li>
        <ul class="ul-self">
        <li> <span class="li-head">automatic_conflict_resolution</span> - Enable/disable automatic conflict resolution. <span class="li-normal">type: str</span> <span class="li-normal">choices: disable, enable</span>
 <a id='label2' href="javascript:ContentClick('label3', 'label2');" onmouseover="ContentPreview('label3');" onmouseout="ContentUnpreview('label3');" title="click to collapse or expand..."> more... </a>
 <div id="label3" style="display:none">
 <table border="1">
 <tr>
 <td></td>
 <td colspan="1">Supported Version Ranges</td>
 </tr>
 <tr>
 <td>automatic_conflict_resolution</td>
 <td><code class="docutils literal notranslate">v7.4.0 -> 7.4.4 </code></td>
 </tr>
 <tr>
 <td>[disable]</td>
 <td><code class="docutils literal notranslate">v7.4.0 -> 7.4.4</code></td>
 <tr>
 <td>[enable]</td>
 <td><code class="docutils literal notranslate">v7.4.0 -> 7.4.4</code></td>
 </table>
 </div>
 </li>
        <li> <span class="li-head">manage_lan_addresses</span> - Enable/disable default management of LAN interface addresses. <span class="li-normal">type: str</span> <span class="li-normal">choices: disable, enable</span>
 <a id='label4' href="javascript:ContentClick('label5', 'label4');" onmouseover="ContentPreview('label5');" onmouseout="ContentUnpreview('label5');" title="click to collapse or expand..."> more... </a>
 <div id="label5" style="display:none">
 <table border="1">
 <tr>
 <td></td>
 <td colspan="1">Supported Version Ranges</td>
 </tr>
 <tr>
 <td>manage_lan_addresses</td>
 <td><code class="docutils literal notranslate">v7.4.0 -> 7.4.4 </code></td>
 </tr>
 <tr>
 <td>[disable]</td>
 <td><code class="docutils literal notranslate">v7.4.0 -> 7.4.4</code></td>
 <tr>
 <td>[enable]</td>
 <td><code class="docutils literal notranslate">v7.4.0 -> 7.4.4</code></td>
 </table>
 </div>
 </li>
        <li> <span class="li-head">manage_lan_extension_addresses</span> - Enable/disable default management of FortiExtender LAN extension interface addresses. <span class="li-normal">type: str</span> <span class="li-normal">choices: disable, enable</span>
 <a id='label6' href="javascript:ContentClick('label7', 'label6');" onmouseover="ContentPreview('label7');" onmouseout="ContentUnpreview('label7');" title="click to collapse or expand..."> more... </a>
 <div id="label7" style="display:none">
 <table border="1">
 <tr>
 <td></td>
 <td colspan="1">Supported Version Ranges</td>
 </tr>
 <tr>
 <td>manage_lan_extension_addresses</td>
 <td><code class="docutils literal notranslate">v7.4.0 -> 7.4.4 </code></td>
 </tr>
 <tr>
 <td>[disable]</td>
 <td><code class="docutils literal notranslate">v7.4.0 -> 7.4.4</code></td>
 <tr>
 <td>[enable]</td>
 <td><code class="docutils literal notranslate">v7.4.0 -> 7.4.4</code></td>
 </table>
 </div>
 </li>
        <li> <span class="li-head">manage_ssid_addresses</span> - Enable/disable default management of FortiAP SSID addresses. <span class="li-normal">type: str</span> <span class="li-normal">choices: disable, enable</span>
 <a id='label8' href="javascript:ContentClick('label9', 'label8');" onmouseover="ContentPreview('label9');" onmouseout="ContentUnpreview('label9');" title="click to collapse or expand..."> more... </a>
 <div id="label9" style="display:none">
 <table border="1">
 <tr>
 <td></td>
 <td colspan="1">Supported Version Ranges</td>
 </tr>
 <tr>
 <td>manage_ssid_addresses</td>
 <td><code class="docutils literal notranslate">v7.4.0 -> 7.4.4 </code></td>
 </tr>
 <tr>
 <td>[disable]</td>
 <td><code class="docutils literal notranslate">v7.4.0 -> 7.4.4</code></td>
 <tr>
 <td>[enable]</td>
 <td><code class="docutils literal notranslate">v7.4.0 -> 7.4.4</code></td>
 </table>
 </div>
 </li>
        <li> <span class="li-head">pool_subnet</span> - Configure IPAM pool subnet, Class A - Class B subnet. <span class="li-normal">type: str</span>
 <a id='label10' href="javascript:ContentClick('label11', 'label10');" onmouseover="ContentPreview('label11');" onmouseout="ContentUnpreview('label11');" title="click to collapse or expand..."> more... </a>
 <div id="label11" style="display:none">
 <table border="1">
 <tr>
 <td></td>
 <td colspan="1">Supported Version Ranges</td>
 </tr>
 <tr>
 <td>pool_subnet</td>
 <td><code class="docutils literal notranslate">v7.0.2 -> v7.2.0 </code></td>
 </tr>
 </table>
 </div>
 </li>
        <li> <span class="li-head">pools</span> - Configure IPAM pools. <span class="li-normal">type: list</span> <span style="font-family:'Courier New'" class="li-required">member_path: pools:name</span>
 <a id='label12' href="javascript:ContentClick('label13', 'label12');" onmouseover="ContentPreview('label13');" onmouseout="ContentUnpreview('label13');" title="click to collapse or expand..."> more... </a>
 <div id="label13" style="display:none">
 <table border="1">
 <tr>
 <td></td><td colspan="1">Supported Version Ranges</td>
 </tr>
 <tr>
 <td>pools</td>
 <td><code class="docutils literal notranslate">v7.2.1 -> 7.4.4 </code></td>
 </tr>
 </table>
 </div>
 </li>
            <ul class="ul-self">
            <li> <span class="li-head">description</span> - Description. <span class="li-normal">type: str</span>
 <a id='label14' href="javascript:ContentClick('label15', 'label14');" onmouseover="ContentPreview('label15');" onmouseout="ContentUnpreview('label15');" title="click to collapse or expand..."> more... </a>
 <div id="label15" style="display:none">
 <table border="1">
 <tr>
 <td></td>
 <td colspan="1">Supported Version Ranges</td>
 </tr>
 <tr>
 <td>description</td>
 <td><code class="docutils literal notranslate">v7.2.1 -> 7.4.4 </code></td>
 </tr>
 </table>
 </div>
 </li>
            <li> <span class="li-head">exclude</span> - Configure pool exclude subnets. <span class="li-normal">type: list</span> <span style="font-family:'Courier New'" class="li-required">member_path: pools:name/exclude:ID</span>
 <a id='label16' href="javascript:ContentClick('label17', 'label16');" onmouseover="ContentPreview('label17');" onmouseout="ContentUnpreview('label17');" title="click to collapse or expand..."> more... </a>
 <div id="label17" style="display:none">
 <table border="1">
 <tr>
 <td></td><td colspan="1">Supported Version Ranges</td>
 </tr>
 <tr>
 <td>exclude</td>
 <td><code class="docutils literal notranslate">v7.4.4 -> 7.4.4 </code></td>
 </tr>
 </table>
 </div>
 </li>
                <ul class="ul-self">
                <li> <span class="li-head">exclude_subnet</span> - Configure subnet to exclude from the IPAM pool. <span class="li-normal">type: str</span>
 <a id='label18' href="javascript:ContentClick('label19', 'label18');" onmouseover="ContentPreview('label19');" onmouseout="ContentUnpreview('label19');" title="click to collapse or expand..."> more... </a>
 <div id="label19" style="display:none">
 <table border="1">
 <tr>
 <td></td>
 <td colspan="1">Supported Version Ranges</td>
 </tr>
 <tr>
 <td>exclude_subnet</td>
 <td><code class="docutils literal notranslate">v7.4.4 -> 7.4.4 </code></td>
 </tr>
 </table>
 </div>
 </li>
                <li> <span class="li-head">ID</span> - Exclude ID. see <a href='#notes'>Notes</a>. <span class="li-normal">type: int</span> <span class="li-required">required: true</span>
 <a id='label20' href="javascript:ContentClick('label21', 'label20');" onmouseover="ContentPreview('label21');" onmouseout="ContentUnpreview('label21');" title="click to collapse or expand..."> more... </a>
 <div id="label21" style="display:none">
 <table border="1">
 <tr>
 <td></td>
 <td colspan="1">Supported Version Ranges</td>
 </tr>
 <tr>
 <td>ID</td>
 <td><code class="docutils literal notranslate">v7.4.4 -> 7.4.4 </code></td>
 </tr>
 </table>
 </div>
 </li>
                </ul>
            <li> <span class="li-head">name</span> - IPAM pool name. <span class="li-normal">type: str</span> <span class="li-required">required: true</span>
 <a id='label22' href="javascript:ContentClick('label23', 'label22');" onmouseover="ContentPreview('label23');" onmouseout="ContentUnpreview('label23');" title="click to collapse or expand..."> more... </a>
 <div id="label23" style="display:none">
 <table border="1">
 <tr>
 <td></td>
 <td colspan="1">Supported Version Ranges</td>
 </tr>
 <tr>
 <td>name</td>
 <td><code class="docutils literal notranslate">v7.2.1 -> 7.4.4 </code></td>
 </tr>
 </table>
 </div>
 </li>
            <li> <span class="li-head">subnet</span> - Configure IPAM pool subnet, Class A - Class B subnet. <span class="li-normal">type: str</span>
 <a id='label24' href="javascript:ContentClick('label25', 'label24');" onmouseover="ContentPreview('label25');" onmouseout="ContentUnpreview('label25');" title="click to collapse or expand..."> more... </a>
 <div id="label25" style="display:none">
 <table border="1">
 <tr>
 <td></td>
 <td colspan="1">Supported Version Ranges</td>
 </tr>
 <tr>
 <td>subnet</td>
 <td><code class="docutils literal notranslate">v7.2.1 -> 7.4.4 </code></td>
 </tr>
 </table>
 </div>
 </li>
            </ul>
        <li> <span class="li-head">require_subnet_size_match</span> - Enable/disable reassignment of subnets to make requested and actual sizes match. <span class="li-normal">type: str</span> <span class="li-normal">choices: disable, enable</span>
 <a id='label26' href="javascript:ContentClick('label27', 'label26');" onmouseover="ContentPreview('label27');" onmouseout="ContentUnpreview('label27');" title="click to collapse or expand..."> more... </a>
 <div id="label27" style="display:none">
 <table border="1">
 <tr>
 <td></td>
 <td colspan="1">Supported Version Ranges</td>
 </tr>
 <tr>
 <td>require_subnet_size_match</td>
 <td><code class="docutils literal notranslate">v7.4.2 -> 7.4.4 </code></td>
 </tr>
 <tr>
 <td>[disable]</td>
 <td><code class="docutils literal notranslate">v7.4.2 -> 7.4.4</code></td>
 <tr>
 <td>[enable]</td>
 <td><code class="docutils literal notranslate">v7.4.2 -> 7.4.4</code></td>
 </table>
 </div>
 </li>
        <li> <span class="li-head">rules</span> - Configure IPAM allocation rules. <span class="li-normal">type: list</span> <span style="font-family:'Courier New'" class="li-required">member_path: rules:name</span>
 <a id='label28' href="javascript:ContentClick('label29', 'label28');" onmouseover="ContentPreview('label29');" onmouseout="ContentUnpreview('label29');" title="click to collapse or expand..."> more... </a>
 <div id="label29" style="display:none">
 <table border="1">
 <tr>
 <td></td><td colspan="1">Supported Version Ranges</td>
 </tr>
 <tr>
 <td>rules</td>
 <td><code class="docutils literal notranslate">v7.2.1 -> 7.4.4 </code></td>
 </tr>
 </table>
 </div>
 </li>
            <ul class="ul-self">
            <li> <span class="li-head">description</span> - Description. <span class="li-normal">type: str</span>
 <a id='label30' href="javascript:ContentClick('label31', 'label30');" onmouseover="ContentPreview('label31');" onmouseout="ContentUnpreview('label31');" title="click to collapse or expand..."> more... </a>
 <div id="label31" style="display:none">
 <table border="1">
 <tr>
 <td></td>
 <td colspan="1">Supported Version Ranges</td>
 </tr>
 <tr>
 <td>description</td>
 <td><code class="docutils literal notranslate">v7.2.1 -> 7.4.4 </code></td>
 </tr>
 </table>
 </div>
 </li>
            <li> <span class="li-head">device</span> - Configure serial number or wildcard of FortiGate to match. <span class="li-normal">type: list</span> <span style="font-family:'Courier New'" class="li-required">member_path: rules:name/device:name</span>
 <a id='label32' href="javascript:ContentClick('label33', 'label32');" onmouseover="ContentPreview('label33');" onmouseout="ContentUnpreview('label33');" title="click to collapse or expand..."> more... </a>
 <div id="label33" style="display:none">
 <table border="1">
 <tr>
 <td></td><td colspan="1">Supported Version Ranges</td>
 </tr>
 <tr>
 <td>device</td>
 <td><code class="docutils literal notranslate">v7.2.1 -> 7.4.4 </code></td>
 </tr>
 </table>
 </div>
 </li>
                <ul class="ul-self">
                <li> <span class="li-head">name</span> - FortiGate serial number or wildcard. <span class="li-normal">type: str</span> <span class="li-required">required: true</span>
 <a id='label34' href="javascript:ContentClick('label35', 'label34');" onmouseover="ContentPreview('label35');" onmouseout="ContentUnpreview('label35');" title="click to collapse or expand..."> more... </a>
 <div id="label35" style="display:none">
 <table border="1">
 <tr>
 <td></td>
 <td colspan="1">Supported Version Ranges</td>
 </tr>
 <tr>
 <td>name</td>
 <td><code class="docutils literal notranslate">v7.2.1 -> 7.4.4 </code></td>
 </tr>
 </table>
 </div>
 </li>
                </ul>
            <li> <span class="li-head">dhcp</span> - Enable/disable DHCP server for matching IPAM interfaces. <span class="li-normal">type: str</span> <span class="li-normal">choices: enable, disable</span>
 <a id='label36' href="javascript:ContentClick('label37', 'label36');" onmouseover="ContentPreview('label37');" onmouseout="ContentUnpreview('label37');" title="click to collapse or expand..."> more... </a>
 <div id="label37" style="display:none">
 <table border="1">
 <tr>
 <td></td>
 <td colspan="1">Supported Version Ranges</td>
 </tr>
 <tr>
 <td>dhcp</td>
 <td><code class="docutils literal notranslate">v7.2.1 -> 7.4.4 </code></td>
 </tr>
 <tr>
 <td>[enable]</td>
 <td><code class="docutils literal notranslate">v7.2.1 -> 7.4.4</code></td>
 <tr>
 <td>[disable]</td>
 <td><code class="docutils literal notranslate">v7.2.1 -> 7.4.4</code></td>
 </table>
 </div>
 </li>
            <li> <span class="li-head">interface</span> - Configure name or wildcard of interface to match. <span class="li-normal">type: list</span> <span style="font-family:'Courier New'" class="li-required">member_path: rules:name/interface:name</span>
 <a id='label38' href="javascript:ContentClick('label39', 'label38');" onmouseover="ContentPreview('label39');" onmouseout="ContentUnpreview('label39');" title="click to collapse or expand..."> more... </a>
 <div id="label39" style="display:none">
 <table border="1">
 <tr>
 <td></td><td colspan="1">Supported Version Ranges</td>
 </tr>
 <tr>
 <td>interface</td>
 <td><code class="docutils literal notranslate">v7.2.1 -> 7.4.4 </code></td>
 </tr>
 </table>
 </div>
 </li>
                <ul class="ul-self">
                <li> <span class="li-head">name</span> - Interface name or wildcard. <span class="li-normal">type: str</span> <span class="li-required">required: true</span>
 <a id='label40' href="javascript:ContentClick('label41', 'label40');" onmouseover="ContentPreview('label41');" onmouseout="ContentUnpreview('label41');" title="click to collapse or expand..."> more... </a>
 <div id="label41" style="display:none">
 <table border="1">
 <tr>
 <td></td>
 <td colspan="1">Supported Version Ranges</td>
 </tr>
 <tr>
 <td>name</td>
 <td><code class="docutils literal notranslate">v7.2.1 -> 7.4.4 </code></td>
 </tr>
 </table>
 </div>
 </li>
                </ul>
            <li> <span class="li-head">name</span> - IPAM rule name. <span class="li-normal">type: str</span> <span class="li-required">required: true</span>
 <a id='label42' href="javascript:ContentClick('label43', 'label42');" onmouseover="ContentPreview('label43');" onmouseout="ContentUnpreview('label43');" title="click to collapse or expand..."> more... </a>
 <div id="label43" style="display:none">
 <table border="1">
 <tr>
 <td></td>
 <td colspan="1">Supported Version Ranges</td>
 </tr>
 <tr>
 <td>name</td>
 <td><code class="docutils literal notranslate">v7.2.1 -> 7.4.4 </code></td>
 </tr>
 </table>
 </div>
 </li>
            <li> <span class="li-head">pool</span> - Configure name of IPAM pool to use. <span class="li-normal">type: list</span> <span style="font-family:'Courier New'" class="li-required">member_path: rules:name/pool:name</span>
 <a id='label44' href="javascript:ContentClick('label45', 'label44');" onmouseover="ContentPreview('label45');" onmouseout="ContentUnpreview('label45');" title="click to collapse or expand..."> more... </a>
 <div id="label45" style="display:none">
 <table border="1">
 <tr>
 <td></td><td colspan="1">Supported Version Ranges</td>
 </tr>
 <tr>
 <td>pool</td>
 <td><code class="docutils literal notranslate">v7.2.1 -> 7.4.4 </code></td>
 </tr>
 </table>
 </div>
 </li>
                <ul class="ul-self">
                <li> <span class="li-head">name</span> - IPAM pool name. Source system.ipam.pools.name. <span class="li-normal">type: str</span> <span class="li-required">required: true</span>
 <a id='label46' href="javascript:ContentClick('label47', 'label46');" onmouseover="ContentPreview('label47');" onmouseout="ContentUnpreview('label47');" title="click to collapse or expand..."> more... </a>
 <div id="label47" style="display:none">
 <table border="1">
 <tr>
 <td></td>
 <td colspan="1">Supported Version Ranges</td>
 </tr>
 <tr>
 <td>name</td>
 <td><code class="docutils literal notranslate">v7.2.1 -> 7.4.4 </code></td>
 </tr>
 </table>
 </div>
 </li>
                </ul>
            <li> <span class="li-head">role</span> - Configure role of interface to match. <span class="li-normal">type: str</span> <span class="li-normal">choices: any, lan, wan, dmz, undefined</span>
 <a id='label48' href="javascript:ContentClick('label49', 'label48');" onmouseover="ContentPreview('label49');" onmouseout="ContentUnpreview('label49');" title="click to collapse or expand..."> more... </a>
 <div id="label49" style="display:none">
 <table border="1">
 <tr>
 <td></td>
 <td colspan="1">Supported Version Ranges</td>
 </tr>
 <tr>
 <td>role</td>
 <td><code class="docutils literal notranslate">v7.2.1 -> 7.4.4 </code></td>
 </tr>
 <tr>
 <td>[any]</td>
 <td><code class="docutils literal notranslate">v7.2.1 -> 7.4.4</code></td>
 <tr>
 <td>[lan]</td>
 <td><code class="docutils literal notranslate">v7.2.1 -> 7.4.4</code></td>
 <tr>
 <td>[wan]</td>
 <td><code class="docutils literal notranslate">v7.2.1 -> 7.4.4</code></td>
 <tr>
 <td>[dmz]</td>
 <td><code class="docutils literal notranslate">v7.2.1 -> 7.4.4</code></td>
 <tr>
 <td>[undefined]</td>
 <td><code class="docutils literal notranslate">v7.2.1 -> 7.4.4</code></td>
 </table>
 </div>
 </li>
            </ul>
        <li> <span class="li-head">server_type</span> - Configure the type of IPAM server to use. <span class="li-normal">type: str</span> <span class="li-normal">choices: fabric-root, cloud</span>
 <a id='label50' href="javascript:ContentClick('label51', 'label50');" onmouseover="ContentPreview('label51');" onmouseout="ContentUnpreview('label51');" title="click to collapse or expand..."> more... </a>
 <div id="label51" style="display:none">
 <table border="1">
 <tr>
 <td></td>
 <td colspan="1">Supported Version Ranges</td>
 </tr>
 <tr>
 <td>server_type</td>
 <td><code class="docutils literal notranslate">v7.0.2 -> 7.4.4 </code></td>
 </tr>
 <tr>
 <td>[fabric-root]</td>
 <td><code class="docutils literal notranslate">v7.0.2 -> 7.4.4</code></td>
 <tr>
 <td>[cloud]</td>
 <td><code class="docutils literal notranslate">v7.0.2 -> v7.2.4</code></td>
 </tr>
 </table>
 </div>
 </li>
        <li> <span class="li-head">status</span> - Enable/disable IP address management services. <span class="li-normal">type: str</span> <span class="li-normal">choices: enable, disable</span>
 <a id='label52' href="javascript:ContentClick('label53', 'label52');" onmouseover="ContentPreview('label53');" onmouseout="ContentUnpreview('label53');" title="click to collapse or expand..."> more... </a>
 <div id="label53" style="display:none">
 <table border="1">
 <tr>
 <td></td>
 <td colspan="1">Supported Version Ranges</td>
 </tr>
 <tr>
 <td>status</td>
 <td><code class="docutils literal notranslate">v7.0.2 -> 7.4.4 </code></td>
 </tr>
 <tr>
 <td>[enable]</td>
 <td><code class="docutils literal notranslate">v7.0.2 -> 7.4.4</code></td>
 <tr>
 <td>[disable]</td>
 <td><code class="docutils literal notranslate">v7.0.2 -> 7.4.4</code></td>
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
    
    - name: Configure IP address management services.
      fortinet.fortios.fortios_system_ipam:
          vdom: "{{ vdom }}"
          system_ipam:
              automatic_conflict_resolution: "disable"
              manage_lan_addresses: "disable"
              manage_lan_extension_addresses: "disable"
              manage_ssid_addresses: "disable"
              pool_subnet: "<your_own_value>"
              pools:
                  -
                      description: "<your_own_value>"
                      exclude:
                          -
                              exclude_subnet: "<your_own_value>"
                              ID: "<you_own_value>"
                      name: "default_name_13"
                      subnet: "<your_own_value>"
              require_subnet_size_match: "disable"
              rules:
                  -
                      description: "<your_own_value>"
                      device:
                          -
                              name: "default_name_19"
                      dhcp: "enable"
                      interface:
                          -
                              name: "default_name_22"
                      name: "default_name_23"
                      pool:
                          -
                              name: "default_name_25 (source system.ipam.pools.name)"
                      role: "any"
              server_type: "fabric-root"
              status: "enable"


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
