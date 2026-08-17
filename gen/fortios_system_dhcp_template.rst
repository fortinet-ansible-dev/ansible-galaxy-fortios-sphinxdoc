:source: fortios_system_dhcp_template.py

:orphan:

.. fortios_system_dhcp_template:

fortios_system_dhcp_template -- Configure DHCP server templates in Fortinet's FortiOS and FortiGate.
++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++

.. versionadded:: 2.0.0

.. contents::
   :local:
   :depth: 1


Synopsis
--------
- This module is able to configure a FortiGate or FortiOS (FOS) device by allowing the user to set and modify system_dhcp feature and template category. Examples include all parameters and values need to be adjusted to datasources before usage. Tested with FOS v6.0.0



Requirements
------------
The below requirements are needed on the host that executes this module.

- ansible>=2.16


Tips
----
Using member operation to add an element to an existing object.

FortiOS Version Compatibility
-----------------------------
Supported Version Ranges: v8.0.0


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
    <li> <span class="li-head">system_dhcp_template</span> - Configure DHCP server templates. <span class="li-normal">type: dict</span>
 <a id='label0' href="javascript:ContentClick('label1', 'label0');" onmouseover="ContentPreview('label1');" onmouseout="ContentUnpreview('label1');" title="click to collapse or expand..."> more... </a>
 <div id="label1" style="display:none">
 <table border="1">
 <tr>
 <td></td><td colspan="1">Supported Version Ranges</td>
 </tr>
 <tr>
 <td>system_dhcp_template</td>
 <td><code class="docutils literal notranslate">v8.0.0 -> 8.0.0 </code></td>
 </tr>
 </table>
 </div>
 </li>
        <ul class="ul-self">
        <li> <span class="li-head">auto_configuration</span> - Enable/disable auto configuration. <span class="li-normal">type: str</span> <span class="li-normal">choices: disable, enable</span>
 <a id='label2' href="javascript:ContentClick('label3', 'label2');" onmouseover="ContentPreview('label3');" onmouseout="ContentUnpreview('label3');" title="click to collapse or expand..."> more... </a>
 <div id="label3" style="display:none">
 <table border="1">
 <tr>
 <td></td>
 <td colspan="1">Supported Version Ranges</td>
 </tr>
 <tr>
 <td>auto_configuration</td>
 <td><code class="docutils literal notranslate">v8.0.0 -> 8.0.0 </code></td>
 </tr>
 <tr>
 <td>[disable]</td>
 <td><code class="docutils literal notranslate">v8.0.0 -> 8.0.0</code></td>
 <tr>
 <td>[enable]</td>
 <td><code class="docutils literal notranslate">v8.0.0 -> 8.0.0</code></td>
 </table>
 </div>
 </li>
        <li> <span class="li-head">conflicted_ip_timeout</span> - Time in seconds to wait after a conflicted IP address is removed from the DHCP range before it can be reused. <span class="li-normal">type: int</span>
 <a id='label4' href="javascript:ContentClick('label5', 'label4');" onmouseover="ContentPreview('label5');" onmouseout="ContentUnpreview('label5');" title="click to collapse or expand..."> more... </a>
 <div id="label5" style="display:none">
 <table border="1">
 <tr>
 <td></td>
 <td colspan="1">Supported Version Ranges</td>
 </tr>
 <tr>
 <td>conflicted_ip_timeout</td>
 <td><code class="docutils literal notranslate">v8.0.0 -> 8.0.0 </code></td>
 </tr>
 </table>
 </div>
 </li>
        <li> <span class="li-head">ddns_auth</span> - DDNS authentication mode. <span class="li-normal">type: str</span> <span class="li-normal">choices: disable, tsig</span>
 <a id='label6' href="javascript:ContentClick('label7', 'label6');" onmouseover="ContentPreview('label7');" onmouseout="ContentUnpreview('label7');" title="click to collapse or expand..."> more... </a>
 <div id="label7" style="display:none">
 <table border="1">
 <tr>
 <td></td>
 <td colspan="1">Supported Version Ranges</td>
 </tr>
 <tr>
 <td>ddns_auth</td>
 <td><code class="docutils literal notranslate">v8.0.0 -> 8.0.0 </code></td>
 </tr>
 <tr>
 <td>[disable]</td>
 <td><code class="docutils literal notranslate">v8.0.0 -> 8.0.0</code></td>
 <tr>
 <td>[tsig]</td>
 <td><code class="docutils literal notranslate">v8.0.0 -> 8.0.0</code></td>
 </table>
 </div>
 </li>
        <li> <span class="li-head">ddns_key</span> - DDNS update key (base 64 encoding). <span class="li-normal">type: str</span>
 <a id='label8' href="javascript:ContentClick('label9', 'label8');" onmouseover="ContentPreview('label9');" onmouseout="ContentUnpreview('label9');" title="click to collapse or expand..."> more... </a>
 <div id="label9" style="display:none">
 <table border="1">
 <tr>
 <td></td>
 <td colspan="1">Supported Version Ranges</td>
 </tr>
 <tr>
 <td>ddns_key</td>
 <td><code class="docutils literal notranslate">v8.0.0 -> 8.0.0 </code></td>
 </tr>
 </table>
 </div>
 </li>
        <li> <span class="li-head">ddns_keyname</span> - DDNS update key name. <span class="li-normal">type: str</span>
 <a id='label10' href="javascript:ContentClick('label11', 'label10');" onmouseover="ContentPreview('label11');" onmouseout="ContentUnpreview('label11');" title="click to collapse or expand..."> more... </a>
 <div id="label11" style="display:none">
 <table border="1">
 <tr>
 <td></td>
 <td colspan="1">Supported Version Ranges</td>
 </tr>
 <tr>
 <td>ddns_keyname</td>
 <td><code class="docutils literal notranslate">v8.0.0 -> 8.0.0 </code></td>
 </tr>
 </table>
 </div>
 </li>
        <li> <span class="li-head">ddns_server_ip</span> - DDNS server IP. <span class="li-normal">type: str</span>
 <a id='label12' href="javascript:ContentClick('label13', 'label12');" onmouseover="ContentPreview('label13');" onmouseout="ContentUnpreview('label13');" title="click to collapse or expand..."> more... </a>
 <div id="label13" style="display:none">
 <table border="1">
 <tr>
 <td></td>
 <td colspan="1">Supported Version Ranges</td>
 </tr>
 <tr>
 <td>ddns_server_ip</td>
 <td><code class="docutils literal notranslate">v8.0.0 -> 8.0.0 </code></td>
 </tr>
 </table>
 </div>
 </li>
        <li> <span class="li-head">ddns_ttl</span> - TTL. <span class="li-normal">type: int</span>
 <a id='label14' href="javascript:ContentClick('label15', 'label14');" onmouseover="ContentPreview('label15');" onmouseout="ContentUnpreview('label15');" title="click to collapse or expand..."> more... </a>
 <div id="label15" style="display:none">
 <table border="1">
 <tr>
 <td></td>
 <td colspan="1">Supported Version Ranges</td>
 </tr>
 <tr>
 <td>ddns_ttl</td>
 <td><code class="docutils literal notranslate">v8.0.0 -> 8.0.0 </code></td>
 </tr>
 </table>
 </div>
 </li>
        <li> <span class="li-head">ddns_update</span> - Enable/disable DDNS update for DHCP. <span class="li-normal">type: str</span> <span class="li-normal">choices: disable, enable</span>
 <a id='label16' href="javascript:ContentClick('label17', 'label16');" onmouseover="ContentPreview('label17');" onmouseout="ContentUnpreview('label17');" title="click to collapse or expand..."> more... </a>
 <div id="label17" style="display:none">
 <table border="1">
 <tr>
 <td></td>
 <td colspan="1">Supported Version Ranges</td>
 </tr>
 <tr>
 <td>ddns_update</td>
 <td><code class="docutils literal notranslate">v8.0.0 -> 8.0.0 </code></td>
 </tr>
 <tr>
 <td>[disable]</td>
 <td><code class="docutils literal notranslate">v8.0.0 -> 8.0.0</code></td>
 <tr>
 <td>[enable]</td>
 <td><code class="docutils literal notranslate">v8.0.0 -> 8.0.0</code></td>
 </table>
 </div>
 </li>
        <li> <span class="li-head">ddns_update_override</span> - Enable/disable DDNS update override for DHCP. <span class="li-normal">type: str</span> <span class="li-normal">choices: disable, enable</span>
 <a id='label18' href="javascript:ContentClick('label19', 'label18');" onmouseover="ContentPreview('label19');" onmouseout="ContentUnpreview('label19');" title="click to collapse or expand..."> more... </a>
 <div id="label19" style="display:none">
 <table border="1">
 <tr>
 <td></td>
 <td colspan="1">Supported Version Ranges</td>
 </tr>
 <tr>
 <td>ddns_update_override</td>
 <td><code class="docutils literal notranslate">v8.0.0 -> 8.0.0 </code></td>
 </tr>
 <tr>
 <td>[disable]</td>
 <td><code class="docutils literal notranslate">v8.0.0 -> 8.0.0</code></td>
 <tr>
 <td>[enable]</td>
 <td><code class="docutils literal notranslate">v8.0.0 -> 8.0.0</code></td>
 </table>
 </div>
 </li>
        <li> <span class="li-head">ddns_zone</span> - Zone of your domain name (ex. DDNS.com). <span class="li-normal">type: str</span>
 <a id='label20' href="javascript:ContentClick('label21', 'label20');" onmouseover="ContentPreview('label21');" onmouseout="ContentUnpreview('label21');" title="click to collapse or expand..."> more... </a>
 <div id="label21" style="display:none">
 <table border="1">
 <tr>
 <td></td>
 <td colspan="1">Supported Version Ranges</td>
 </tr>
 <tr>
 <td>ddns_zone</td>
 <td><code class="docutils literal notranslate">v8.0.0 -> 8.0.0 </code></td>
 </tr>
 </table>
 </div>
 </li>
        <li> <span class="li-head">dns_server1</span> - DNS server 1. <span class="li-normal">type: str</span>
 <a id='label22' href="javascript:ContentClick('label23', 'label22');" onmouseover="ContentPreview('label23');" onmouseout="ContentUnpreview('label23');" title="click to collapse or expand..."> more... </a>
 <div id="label23" style="display:none">
 <table border="1">
 <tr>
 <td></td>
 <td colspan="1">Supported Version Ranges</td>
 </tr>
 <tr>
 <td>dns_server1</td>
 <td><code class="docutils literal notranslate">v8.0.0 -> 8.0.0 </code></td>
 </tr>
 </table>
 </div>
 </li>
        <li> <span class="li-head">dns_server2</span> - DNS server 2. <span class="li-normal">type: str</span>
 <a id='label24' href="javascript:ContentClick('label25', 'label24');" onmouseover="ContentPreview('label25');" onmouseout="ContentUnpreview('label25');" title="click to collapse or expand..."> more... </a>
 <div id="label25" style="display:none">
 <table border="1">
 <tr>
 <td></td>
 <td colspan="1">Supported Version Ranges</td>
 </tr>
 <tr>
 <td>dns_server2</td>
 <td><code class="docutils literal notranslate">v8.0.0 -> 8.0.0 </code></td>
 </tr>
 </table>
 </div>
 </li>
        <li> <span class="li-head">dns_server3</span> - DNS server 3. <span class="li-normal">type: str</span>
 <a id='label26' href="javascript:ContentClick('label27', 'label26');" onmouseover="ContentPreview('label27');" onmouseout="ContentUnpreview('label27');" title="click to collapse or expand..."> more... </a>
 <div id="label27" style="display:none">
 <table border="1">
 <tr>
 <td></td>
 <td colspan="1">Supported Version Ranges</td>
 </tr>
 <tr>
 <td>dns_server3</td>
 <td><code class="docutils literal notranslate">v8.0.0 -> 8.0.0 </code></td>
 </tr>
 </table>
 </div>
 </li>
        <li> <span class="li-head">dns_server4</span> - DNS server 4. <span class="li-normal">type: str</span>
 <a id='label28' href="javascript:ContentClick('label29', 'label28');" onmouseover="ContentPreview('label29');" onmouseout="ContentUnpreview('label29');" title="click to collapse or expand..."> more... </a>
 <div id="label29" style="display:none">
 <table border="1">
 <tr>
 <td></td>
 <td colspan="1">Supported Version Ranges</td>
 </tr>
 <tr>
 <td>dns_server4</td>
 <td><code class="docutils literal notranslate">v8.0.0 -> 8.0.0 </code></td>
 </tr>
 </table>
 </div>
 </li>
        <li> <span class="li-head">dns_service</span> - Options for assigning DNS servers to DHCP clients. <span class="li-normal">type: str</span> <span class="li-normal">choices: local, default, specify</span>
 <a id='label30' href="javascript:ContentClick('label31', 'label30');" onmouseover="ContentPreview('label31');" onmouseout="ContentUnpreview('label31');" title="click to collapse or expand..."> more... </a>
 <div id="label31" style="display:none">
 <table border="1">
 <tr>
 <td></td>
 <td colspan="1">Supported Version Ranges</td>
 </tr>
 <tr>
 <td>dns_service</td>
 <td><code class="docutils literal notranslate">v8.0.0 -> 8.0.0 </code></td>
 </tr>
 <tr>
 <td>[local]</td>
 <td><code class="docutils literal notranslate">v8.0.0 -> 8.0.0</code></td>
 <tr>
 <td>[default]</td>
 <td><code class="docutils literal notranslate">v8.0.0 -> 8.0.0</code></td>
 <tr>
 <td>[specify]</td>
 <td><code class="docutils literal notranslate">v8.0.0 -> 8.0.0</code></td>
 </table>
 </div>
 </li>
        <li> <span class="li-head">domain</span> - Domain name suffix for the IP addresses that the DHCP server assigns to clients. <span class="li-normal">type: str</span>
 <a id='label32' href="javascript:ContentClick('label33', 'label32');" onmouseover="ContentPreview('label33');" onmouseout="ContentUnpreview('label33');" title="click to collapse or expand..."> more... </a>
 <div id="label33" style="display:none">
 <table border="1">
 <tr>
 <td></td>
 <td colspan="1">Supported Version Ranges</td>
 </tr>
 <tr>
 <td>domain</td>
 <td><code class="docutils literal notranslate">v8.0.0 -> 8.0.0 </code></td>
 </tr>
 </table>
 </div>
 </li>
        <li> <span class="li-head">exclude_range</span> - Exclude one or more ranges of IP addresses from being assigned to clients. <span class="li-normal">type: list</span> <span style="font-family:'Courier New'" class="li-required">member_path: exclude_range:id</span>
 <a id='label34' href="javascript:ContentClick('label35', 'label34');" onmouseover="ContentPreview('label35');" onmouseout="ContentUnpreview('label35');" title="click to collapse or expand..."> more... </a>
 <div id="label35" style="display:none">
 <table border="1">
 <tr>
 <td></td><td colspan="1">Supported Version Ranges</td>
 </tr>
 <tr>
 <td>exclude_range</td>
 <td><code class="docutils literal notranslate">v8.0.0 -> 8.0.0 </code></td>
 </tr>
 </table>
 </div>
 </li>
            <ul class="ul-self">
            <li> <span class="li-head">id</span> - ID. see <a href='#notes'>Notes</a>. <span class="li-normal">type: int</span> <span class="li-required">required: true</span>
 <a id='label36' href="javascript:ContentClick('label37', 'label36');" onmouseover="ContentPreview('label37');" onmouseout="ContentUnpreview('label37');" title="click to collapse or expand..."> more... </a>
 <div id="label37" style="display:none">
 <table border="1">
 <tr>
 <td></td>
 <td colspan="1">Supported Version Ranges</td>
 </tr>
 <tr>
 <td>id</td>
 <td><code class="docutils literal notranslate">v8.0.0 -> 8.0.0 </code></td>
 </tr>
 </table>
 </div>
 </li>
            <li> <span class="li-head">ip_count</span> - Number of IP addresses to include in the range. <span class="li-normal">type: int</span>
 <a id='label38' href="javascript:ContentClick('label39', 'label38');" onmouseover="ContentPreview('label39');" onmouseout="ContentUnpreview('label39');" title="click to collapse or expand..."> more... </a>
 <div id="label39" style="display:none">
 <table border="1">
 <tr>
 <td></td>
 <td colspan="1">Supported Version Ranges</td>
 </tr>
 <tr>
 <td>ip_count</td>
 <td><code class="docutils literal notranslate">v8.0.0 -> 8.0.0 </code></td>
 </tr>
 </table>
 </div>
 </li>
            <li> <span class="li-head">lease_time</span> - Lease time in seconds, 0 means default lease time. <span class="li-normal">type: int</span>
 <a id='label40' href="javascript:ContentClick('label41', 'label40');" onmouseover="ContentPreview('label41');" onmouseout="ContentUnpreview('label41');" title="click to collapse or expand..."> more... </a>
 <div id="label41" style="display:none">
 <table border="1">
 <tr>
 <td></td>
 <td colspan="1">Supported Version Ranges</td>
 </tr>
 <tr>
 <td>lease_time</td>
 <td><code class="docutils literal notranslate">v8.0.0 -> 8.0.0 </code></td>
 </tr>
 </table>
 </div>
 </li>
            <li> <span class="li-head">oui_match</span> - Enable/disable organizationally unique identifier (OUI) matching. When enabled only DHCP requests with a matching OUI are served with this range. <span class="li-normal">type: str</span> <span class="li-normal">choices: disable, enable</span>
 <a id='label42' href="javascript:ContentClick('label43', 'label42');" onmouseover="ContentPreview('label43');" onmouseout="ContentUnpreview('label43');" title="click to collapse or expand..."> more... </a>
 <div id="label43" style="display:none">
 <table border="1">
 <tr>
 <td></td>
 <td colspan="1">Supported Version Ranges</td>
 </tr>
 <tr>
 <td>oui_match</td>
 <td><code class="docutils literal notranslate">v8.0.0 -> 8.0.0 </code></td>
 </tr>
 <tr>
 <td>[disable]</td>
 <td><code class="docutils literal notranslate">v8.0.0 -> 8.0.0</code></td>
 <tr>
 <td>[enable]</td>
 <td><code class="docutils literal notranslate">v8.0.0 -> 8.0.0</code></td>
 </table>
 </div>
 </li>
            <li> <span class="li-head">oui_string</span> - One or more OUI strings in quotes separated by spaces (in format of xx:xx:xx). <span class="li-normal">type: list</span> <span style="font-family:'Courier New'" class="li-required">member_path: exclude_range:id/oui_string:oui_string</span>
 <a id='label44' href="javascript:ContentClick('label45', 'label44');" onmouseover="ContentPreview('label45');" onmouseout="ContentUnpreview('label45');" title="click to collapse or expand..."> more... </a>
 <div id="label45" style="display:none">
 <table border="1">
 <tr>
 <td></td><td colspan="1">Supported Version Ranges</td>
 </tr>
 <tr>
 <td>oui_string</td>
 <td><code class="docutils literal notranslate">v8.0.0 -> 8.0.0 </code></td>
 </tr>
 </table>
 </div>
 </li>
                <ul class="ul-self">
                <li> <span class="li-head">oui_string</span> - MAC OUI strings. <span class="li-normal">type: str</span> <span class="li-required">required: true</span>
 <a id='label46' href="javascript:ContentClick('label47', 'label46');" onmouseover="ContentPreview('label47');" onmouseout="ContentUnpreview('label47');" title="click to collapse or expand..."> more... </a>
 <div id="label47" style="display:none">
 <table border="1">
 <tr>
 <td></td>
 <td colspan="1">Supported Version Ranges</td>
 </tr>
 <tr>
 <td>oui_string</td>
 <td><code class="docutils literal notranslate">v8.0.0 -> 8.0.0 </code></td>
 </tr>
 </table>
 </div>
 </li>
                </ul>
            <li> <span class="li-head">start_ip_index</span> - Start of IP range. <span class="li-normal">type: int</span>
 <a id='label48' href="javascript:ContentClick('label49', 'label48');" onmouseover="ContentPreview('label49');" onmouseout="ContentUnpreview('label49');" title="click to collapse or expand..."> more... </a>
 <div id="label49" style="display:none">
 <table border="1">
 <tr>
 <td></td>
 <td colspan="1">Supported Version Ranges</td>
 </tr>
 <tr>
 <td>start_ip_index</td>
 <td><code class="docutils literal notranslate">v8.0.0 -> 8.0.0 </code></td>
 </tr>
 </table>
 </div>
 </li>
            <li> <span class="li-head">uci_match</span> - Enable/disable user class identifier (UCI) matching. When enabled only DHCP requests with a matching UCI are served with this range. <span class="li-normal">type: str</span> <span class="li-normal">choices: disable, enable</span>
 <a id='label50' href="javascript:ContentClick('label51', 'label50');" onmouseover="ContentPreview('label51');" onmouseout="ContentUnpreview('label51');" title="click to collapse or expand..."> more... </a>
 <div id="label51" style="display:none">
 <table border="1">
 <tr>
 <td></td>
 <td colspan="1">Supported Version Ranges</td>
 </tr>
 <tr>
 <td>uci_match</td>
 <td><code class="docutils literal notranslate">v8.0.0 -> 8.0.0 </code></td>
 </tr>
 <tr>
 <td>[disable]</td>
 <td><code class="docutils literal notranslate">v8.0.0 -> 8.0.0</code></td>
 <tr>
 <td>[enable]</td>
 <td><code class="docutils literal notranslate">v8.0.0 -> 8.0.0</code></td>
 </table>
 </div>
 </li>
            <li> <span class="li-head">uci_string</span> - One or more UCI strings in quotes separated by spaces. <span class="li-normal">type: list</span> <span style="font-family:'Courier New'" class="li-required">member_path: exclude_range:id/uci_string:uci_string</span>
 <a id='label52' href="javascript:ContentClick('label53', 'label52');" onmouseover="ContentPreview('label53');" onmouseout="ContentUnpreview('label53');" title="click to collapse or expand..."> more... </a>
 <div id="label53" style="display:none">
 <table border="1">
 <tr>
 <td></td><td colspan="1">Supported Version Ranges</td>
 </tr>
 <tr>
 <td>uci_string</td>
 <td><code class="docutils literal notranslate">v8.0.0 -> 8.0.0 </code></td>
 </tr>
 </table>
 </div>
 </li>
                <ul class="ul-self">
                <li> <span class="li-head">uci_string</span> - UCI strings. <span class="li-normal">type: str</span> <span class="li-required">required: true</span>
 <a id='label54' href="javascript:ContentClick('label55', 'label54');" onmouseover="ContentPreview('label55');" onmouseout="ContentUnpreview('label55');" title="click to collapse or expand..."> more... </a>
 <div id="label55" style="display:none">
 <table border="1">
 <tr>
 <td></td>
 <td colspan="1">Supported Version Ranges</td>
 </tr>
 <tr>
 <td>uci_string</td>
 <td><code class="docutils literal notranslate">v8.0.0 -> 8.0.0 </code></td>
 </tr>
 </table>
 </div>
 </li>
                </ul>
            <li> <span class="li-head">vci_match</span> - Enable/disable vendor class identifier (VCI) matching. When enabled only DHCP requests with a matching VCI are served with this range. <span class="li-normal">type: str</span> <span class="li-normal">choices: disable, enable</span>
 <a id='label56' href="javascript:ContentClick('label57', 'label56');" onmouseover="ContentPreview('label57');" onmouseout="ContentUnpreview('label57');" title="click to collapse or expand..."> more... </a>
 <div id="label57" style="display:none">
 <table border="1">
 <tr>
 <td></td>
 <td colspan="1">Supported Version Ranges</td>
 </tr>
 <tr>
 <td>vci_match</td>
 <td><code class="docutils literal notranslate">v8.0.0 -> 8.0.0 </code></td>
 </tr>
 <tr>
 <td>[disable]</td>
 <td><code class="docutils literal notranslate">v8.0.0 -> 8.0.0</code></td>
 <tr>
 <td>[enable]</td>
 <td><code class="docutils literal notranslate">v8.0.0 -> 8.0.0</code></td>
 </table>
 </div>
 </li>
            <li> <span class="li-head">vci_string</span> - One or more VCI strings in quotes separated by spaces. <span class="li-normal">type: list</span> <span style="font-family:'Courier New'" class="li-required">member_path: exclude_range:id/vci_string:vci_string</span>
 <a id='label58' href="javascript:ContentClick('label59', 'label58');" onmouseover="ContentPreview('label59');" onmouseout="ContentUnpreview('label59');" title="click to collapse or expand..."> more... </a>
 <div id="label59" style="display:none">
 <table border="1">
 <tr>
 <td></td><td colspan="1">Supported Version Ranges</td>
 </tr>
 <tr>
 <td>vci_string</td>
 <td><code class="docutils literal notranslate">v8.0.0 -> 8.0.0 </code></td>
 </tr>
 </table>
 </div>
 </li>
                <ul class="ul-self">
                <li> <span class="li-head">vci_string</span> - VCI strings. <span class="li-normal">type: str</span> <span class="li-required">required: true</span>
 <a id='label60' href="javascript:ContentClick('label61', 'label60');" onmouseover="ContentPreview('label61');" onmouseout="ContentUnpreview('label61');" title="click to collapse or expand..."> more... </a>
 <div id="label61" style="display:none">
 <table border="1">
 <tr>
 <td></td>
 <td colspan="1">Supported Version Ranges</td>
 </tr>
 <tr>
 <td>vci_string</td>
 <td><code class="docutils literal notranslate">v8.0.0 -> 8.0.0 </code></td>
 </tr>
 </table>
 </div>
 </li>
                </ul>
            <li> <span class="li-head">vendor</span> - Vendor this ip-range will be assigned to. <span class="li-normal">type: str</span>
 <a id='label62' href="javascript:ContentClick('label63', 'label62');" onmouseover="ContentPreview('label63');" onmouseout="ContentUnpreview('label63');" title="click to collapse or expand..."> more... </a>
 <div id="label63" style="display:none">
 <table border="1">
 <tr>
 <td></td>
 <td colspan="1">Supported Version Ranges</td>
 </tr>
 <tr>
 <td>vendor</td>
 <td><code class="docutils literal notranslate">v8.0.0 -> 8.0.0 </code></td>
 </tr>
 </table>
 </div>
 </li>
            </ul>
        <li> <span class="li-head">fabric_force_sync</span> - Enable/disable forced synchronization of configuration objects from the root FortiGate unit to the downstream devices.  Configuration conflict check is skipped. <span class="li-normal">type: str</span> <span class="li-normal">choices: enable, disable</span>
 <a id='label64' href="javascript:ContentClick('label65', 'label64');" onmouseover="ContentPreview('label65');" onmouseout="ContentUnpreview('label65');" title="click to collapse or expand..."> more... </a>
 <div id="label65" style="display:none">
 <table border="1">
 <tr>
 <td></td>
 <td colspan="1">Supported Version Ranges</td>
 </tr>
 <tr>
 <td>fabric_force_sync</td>
 <td><code class="docutils literal notranslate">v8.0.0 -> 8.0.0 </code></td>
 </tr>
 <tr>
 <td>[enable]</td>
 <td><code class="docutils literal notranslate">v8.0.0 -> 8.0.0</code></td>
 <tr>
 <td>[disable]</td>
 <td><code class="docutils literal notranslate">v8.0.0 -> 8.0.0</code></td>
 </table>
 </div>
 </li>
        <li> <span class="li-head">fabric_object</span> - Security Fabric global object setting. <span class="li-normal">type: str</span> <span class="li-normal">choices: enable, disable</span>
 <a id='label66' href="javascript:ContentClick('label67', 'label66');" onmouseover="ContentPreview('label67');" onmouseout="ContentUnpreview('label67');" title="click to collapse or expand..."> more... </a>
 <div id="label67" style="display:none">
 <table border="1">
 <tr>
 <td></td>
 <td colspan="1">Supported Version Ranges</td>
 </tr>
 <tr>
 <td>fabric_object</td>
 <td><code class="docutils literal notranslate">v8.0.0 -> 8.0.0 </code></td>
 </tr>
 <tr>
 <td>[enable]</td>
 <td><code class="docutils literal notranslate">v8.0.0 -> 8.0.0</code></td>
 <tr>
 <td>[disable]</td>
 <td><code class="docutils literal notranslate">v8.0.0 -> 8.0.0</code></td>
 </table>
 </div>
 </li>
        <li> <span class="li-head">fabric_object_source</span> - Source of truth for fabric object. <span class="li-normal">type: str</span> <span class="li-normal">choices: member, local, root</span>
 <a id='label68' href="javascript:ContentClick('label69', 'label68');" onmouseover="ContentPreview('label69');" onmouseout="ContentUnpreview('label69');" title="click to collapse or expand..."> more... </a>
 <div id="label69" style="display:none">
 <table border="1">
 <tr>
 <td></td>
 <td colspan="1">Supported Version Ranges</td>
 </tr>
 <tr>
 <td>fabric_object_source</td>
 <td><code class="docutils literal notranslate">v8.0.0 -> 8.0.0 </code></td>
 </tr>
 <tr>
 <td>[member]</td>
 <td><code class="docutils literal notranslate">v8.0.0 -> 8.0.0</code></td>
 <tr>
 <td>[local]</td>
 <td><code class="docutils literal notranslate">v8.0.0 -> 8.0.0</code></td>
 <tr>
 <td>[root]</td>
 <td><code class="docutils literal notranslate">v8.0.0 -> 8.0.0</code></td>
 </table>
 </div>
 </li>
        <li> <span class="li-head">filename</span> - Name of the boot file on the TFTP server. <span class="li-normal">type: str</span>
 <a id='label70' href="javascript:ContentClick('label71', 'label70');" onmouseover="ContentPreview('label71');" onmouseout="ContentUnpreview('label71');" title="click to collapse or expand..."> more... </a>
 <div id="label71" style="display:none">
 <table border="1">
 <tr>
 <td></td>
 <td colspan="1">Supported Version Ranges</td>
 </tr>
 <tr>
 <td>filename</td>
 <td><code class="docutils literal notranslate">v8.0.0 -> 8.0.0 </code></td>
 </tr>
 </table>
 </div>
 </li>
        <li> <span class="li-head">forticlient_on_net_status</span> - Enable/disable FortiClient-On-Net service for this DHCP server. <span class="li-normal">type: str</span> <span class="li-normal">choices: disable, enable</span>
 <a id='label72' href="javascript:ContentClick('label73', 'label72');" onmouseover="ContentPreview('label73');" onmouseout="ContentUnpreview('label73');" title="click to collapse or expand..."> more... </a>
 <div id="label73" style="display:none">
 <table border="1">
 <tr>
 <td></td>
 <td colspan="1">Supported Version Ranges</td>
 </tr>
 <tr>
 <td>forticlient_on_net_status</td>
 <td><code class="docutils literal notranslate">v8.0.0 -> 8.0.0 </code></td>
 </tr>
 <tr>
 <td>[disable]</td>
 <td><code class="docutils literal notranslate">v8.0.0 -> 8.0.0</code></td>
 <tr>
 <td>[enable]</td>
 <td><code class="docutils literal notranslate">v8.0.0 -> 8.0.0</code></td>
 </table>
 </div>
 </li>
        <li> <span class="li-head">ip_range</span> - DHCP IP range configuration. <span class="li-normal">type: list</span> <span style="font-family:'Courier New'" class="li-required">member_path: ip_range:id</span>
 <a id='label74' href="javascript:ContentClick('label75', 'label74');" onmouseover="ContentPreview('label75');" onmouseout="ContentUnpreview('label75');" title="click to collapse or expand..."> more... </a>
 <div id="label75" style="display:none">
 <table border="1">
 <tr>
 <td></td><td colspan="1">Supported Version Ranges</td>
 </tr>
 <tr>
 <td>ip_range</td>
 <td><code class="docutils literal notranslate">v8.0.0 -> 8.0.0 </code></td>
 </tr>
 </table>
 </div>
 </li>
            <ul class="ul-self">
            <li> <span class="li-head">id</span> - ID. see <a href='#notes'>Notes</a>. <span class="li-normal">type: int</span> <span class="li-required">required: true</span>
 <a id='label76' href="javascript:ContentClick('label77', 'label76');" onmouseover="ContentPreview('label77');" onmouseout="ContentUnpreview('label77');" title="click to collapse or expand..."> more... </a>
 <div id="label77" style="display:none">
 <table border="1">
 <tr>
 <td></td>
 <td colspan="1">Supported Version Ranges</td>
 </tr>
 <tr>
 <td>id</td>
 <td><code class="docutils literal notranslate">v8.0.0 -> 8.0.0 </code></td>
 </tr>
 </table>
 </div>
 </li>
            <li> <span class="li-head">ip_count</span> - Number of IP addresses to include in the range. <span class="li-normal">type: int</span>
 <a id='label78' href="javascript:ContentClick('label79', 'label78');" onmouseover="ContentPreview('label79');" onmouseout="ContentUnpreview('label79');" title="click to collapse or expand..."> more... </a>
 <div id="label79" style="display:none">
 <table border="1">
 <tr>
 <td></td>
 <td colspan="1">Supported Version Ranges</td>
 </tr>
 <tr>
 <td>ip_count</td>
 <td><code class="docutils literal notranslate">v8.0.0 -> 8.0.0 </code></td>
 </tr>
 </table>
 </div>
 </li>
            <li> <span class="li-head">lease_time</span> - Lease time in seconds, 0 means default lease time. <span class="li-normal">type: int</span>
 <a id='label80' href="javascript:ContentClick('label81', 'label80');" onmouseover="ContentPreview('label81');" onmouseout="ContentUnpreview('label81');" title="click to collapse or expand..."> more... </a>
 <div id="label81" style="display:none">
 <table border="1">
 <tr>
 <td></td>
 <td colspan="1">Supported Version Ranges</td>
 </tr>
 <tr>
 <td>lease_time</td>
 <td><code class="docutils literal notranslate">v8.0.0 -> 8.0.0 </code></td>
 </tr>
 </table>
 </div>
 </li>
            <li> <span class="li-head">oui_match</span> - Enable/disable organizationally unique identifier (OUI) matching. When enabled only DHCP requests with a matching OUI are served with this range. <span class="li-normal">type: str</span> <span class="li-normal">choices: disable, enable</span>
 <a id='label82' href="javascript:ContentClick('label83', 'label82');" onmouseover="ContentPreview('label83');" onmouseout="ContentUnpreview('label83');" title="click to collapse or expand..."> more... </a>
 <div id="label83" style="display:none">
 <table border="1">
 <tr>
 <td></td>
 <td colspan="1">Supported Version Ranges</td>
 </tr>
 <tr>
 <td>oui_match</td>
 <td><code class="docutils literal notranslate">v8.0.0 -> 8.0.0 </code></td>
 </tr>
 <tr>
 <td>[disable]</td>
 <td><code class="docutils literal notranslate">v8.0.0 -> 8.0.0</code></td>
 <tr>
 <td>[enable]</td>
 <td><code class="docutils literal notranslate">v8.0.0 -> 8.0.0</code></td>
 </table>
 </div>
 </li>
            <li> <span class="li-head">oui_string</span> - One or more OUI strings in quotes separated by spaces (in format of xx:xx:xx). <span class="li-normal">type: list</span> <span style="font-family:'Courier New'" class="li-required">member_path: ip_range:id/oui_string:oui_string</span>
 <a id='label84' href="javascript:ContentClick('label85', 'label84');" onmouseover="ContentPreview('label85');" onmouseout="ContentUnpreview('label85');" title="click to collapse or expand..."> more... </a>
 <div id="label85" style="display:none">
 <table border="1">
 <tr>
 <td></td><td colspan="1">Supported Version Ranges</td>
 </tr>
 <tr>
 <td>oui_string</td>
 <td><code class="docutils literal notranslate">v8.0.0 -> 8.0.0 </code></td>
 </tr>
 </table>
 </div>
 </li>
                <ul class="ul-self">
                <li> <span class="li-head">oui_string</span> - MAC OUI strings. <span class="li-normal">type: str</span> <span class="li-required">required: true</span>
 <a id='label86' href="javascript:ContentClick('label87', 'label86');" onmouseover="ContentPreview('label87');" onmouseout="ContentUnpreview('label87');" title="click to collapse or expand..."> more... </a>
 <div id="label87" style="display:none">
 <table border="1">
 <tr>
 <td></td>
 <td colspan="1">Supported Version Ranges</td>
 </tr>
 <tr>
 <td>oui_string</td>
 <td><code class="docutils literal notranslate">v8.0.0 -> 8.0.0 </code></td>
 </tr>
 </table>
 </div>
 </li>
                </ul>
            <li> <span class="li-head">reserve</span> - Enable/disable address reservation for use without DHCP. <span class="li-normal">type: str</span> <span class="li-normal">choices: disable, enable</span>
 <a id='label88' href="javascript:ContentClick('label89', 'label88');" onmouseover="ContentPreview('label89');" onmouseout="ContentUnpreview('label89');" title="click to collapse or expand..."> more... </a>
 <div id="label89" style="display:none">
 <table border="1">
 <tr>
 <td></td>
 <td colspan="1">Supported Version Ranges</td>
 </tr>
 <tr>
 <td>reserve</td>
 <td><code class="docutils literal notranslate">v8.0.0 -> 8.0.0 </code></td>
 </tr>
 <tr>
 <td>[disable]</td>
 <td><code class="docutils literal notranslate">v8.0.0 -> 8.0.0</code></td>
 <tr>
 <td>[enable]</td>
 <td><code class="docutils literal notranslate">v8.0.0 -> 8.0.0</code></td>
 </table>
 </div>
 </li>
            <li> <span class="li-head">uci_match</span> - Enable/disable user class identifier (UCI) matching. When enabled only DHCP requests with a matching UCI are served with this range. <span class="li-normal">type: str</span> <span class="li-normal">choices: disable, enable</span>
 <a id='label90' href="javascript:ContentClick('label91', 'label90');" onmouseover="ContentPreview('label91');" onmouseout="ContentUnpreview('label91');" title="click to collapse or expand..."> more... </a>
 <div id="label91" style="display:none">
 <table border="1">
 <tr>
 <td></td>
 <td colspan="1">Supported Version Ranges</td>
 </tr>
 <tr>
 <td>uci_match</td>
 <td><code class="docutils literal notranslate">v8.0.0 -> 8.0.0 </code></td>
 </tr>
 <tr>
 <td>[disable]</td>
 <td><code class="docutils literal notranslate">v8.0.0 -> 8.0.0</code></td>
 <tr>
 <td>[enable]</td>
 <td><code class="docutils literal notranslate">v8.0.0 -> 8.0.0</code></td>
 </table>
 </div>
 </li>
            <li> <span class="li-head">uci_string</span> - One or more UCI strings in quotes separated by spaces. <span class="li-normal">type: list</span> <span style="font-family:'Courier New'" class="li-required">member_path: ip_range:id/uci_string:uci_string</span>
 <a id='label92' href="javascript:ContentClick('label93', 'label92');" onmouseover="ContentPreview('label93');" onmouseout="ContentUnpreview('label93');" title="click to collapse or expand..."> more... </a>
 <div id="label93" style="display:none">
 <table border="1">
 <tr>
 <td></td><td colspan="1">Supported Version Ranges</td>
 </tr>
 <tr>
 <td>uci_string</td>
 <td><code class="docutils literal notranslate">v8.0.0 -> 8.0.0 </code></td>
 </tr>
 </table>
 </div>
 </li>
                <ul class="ul-self">
                <li> <span class="li-head">uci_string</span> - UCI strings. <span class="li-normal">type: str</span> <span class="li-required">required: true</span>
 <a id='label94' href="javascript:ContentClick('label95', 'label94');" onmouseover="ContentPreview('label95');" onmouseout="ContentUnpreview('label95');" title="click to collapse or expand..."> more... </a>
 <div id="label95" style="display:none">
 <table border="1">
 <tr>
 <td></td>
 <td colspan="1">Supported Version Ranges</td>
 </tr>
 <tr>
 <td>uci_string</td>
 <td><code class="docutils literal notranslate">v8.0.0 -> 8.0.0 </code></td>
 </tr>
 </table>
 </div>
 </li>
                </ul>
            <li> <span class="li-head">vci_match</span> - Enable/disable vendor class identifier (VCI) matching. When enabled only DHCP requests with a matching VCI are served with this range. <span class="li-normal">type: str</span> <span class="li-normal">choices: disable, enable</span>
 <a id='label96' href="javascript:ContentClick('label97', 'label96');" onmouseover="ContentPreview('label97');" onmouseout="ContentUnpreview('label97');" title="click to collapse or expand..."> more... </a>
 <div id="label97" style="display:none">
 <table border="1">
 <tr>
 <td></td>
 <td colspan="1">Supported Version Ranges</td>
 </tr>
 <tr>
 <td>vci_match</td>
 <td><code class="docutils literal notranslate">v8.0.0 -> 8.0.0 </code></td>
 </tr>
 <tr>
 <td>[disable]</td>
 <td><code class="docutils literal notranslate">v8.0.0 -> 8.0.0</code></td>
 <tr>
 <td>[enable]</td>
 <td><code class="docutils literal notranslate">v8.0.0 -> 8.0.0</code></td>
 </table>
 </div>
 </li>
            <li> <span class="li-head">vci_string</span> - One or more VCI strings in quotes separated by spaces. <span class="li-normal">type: list</span> <span style="font-family:'Courier New'" class="li-required">member_path: ip_range:id/vci_string:vci_string</span>
 <a id='label98' href="javascript:ContentClick('label99', 'label98');" onmouseover="ContentPreview('label99');" onmouseout="ContentUnpreview('label99');" title="click to collapse or expand..."> more... </a>
 <div id="label99" style="display:none">
 <table border="1">
 <tr>
 <td></td><td colspan="1">Supported Version Ranges</td>
 </tr>
 <tr>
 <td>vci_string</td>
 <td><code class="docutils literal notranslate">v8.0.0 -> 8.0.0 </code></td>
 </tr>
 </table>
 </div>
 </li>
                <ul class="ul-self">
                <li> <span class="li-head">vci_string</span> - VCI strings. <span class="li-normal">type: str</span> <span class="li-required">required: true</span>
 <a id='label100' href="javascript:ContentClick('label101', 'label100');" onmouseover="ContentPreview('label101');" onmouseout="ContentUnpreview('label101');" title="click to collapse or expand..."> more... </a>
 <div id="label101" style="display:none">
 <table border="1">
 <tr>
 <td></td>
 <td colspan="1">Supported Version Ranges</td>
 </tr>
 <tr>
 <td>vci_string</td>
 <td><code class="docutils literal notranslate">v8.0.0 -> 8.0.0 </code></td>
 </tr>
 </table>
 </div>
 </li>
                </ul>
            <li> <span class="li-head">vendor</span> - Vendor this ip-range will be assigned to. <span class="li-normal">type: str</span>
 <a id='label102' href="javascript:ContentClick('label103', 'label102');" onmouseover="ContentPreview('label103');" onmouseout="ContentUnpreview('label103');" title="click to collapse or expand..."> more... </a>
 <div id="label103" style="display:none">
 <table border="1">
 <tr>
 <td></td>
 <td colspan="1">Supported Version Ranges</td>
 </tr>
 <tr>
 <td>vendor</td>
 <td><code class="docutils literal notranslate">v8.0.0 -> 8.0.0 </code></td>
 </tr>
 </table>
 </div>
 </li>
            </ul>
        <li> <span class="li-head">ipsec_lease_hold</span> - DHCP over IPsec leases expire this many seconds after tunnel down (0 to disable forced-expiry). <span class="li-normal">type: int</span>
 <a id='label104' href="javascript:ContentClick('label105', 'label104');" onmouseover="ContentPreview('label105');" onmouseout="ContentUnpreview('label105');" title="click to collapse or expand..."> more... </a>
 <div id="label105" style="display:none">
 <table border="1">
 <tr>
 <td></td>
 <td colspan="1">Supported Version Ranges</td>
 </tr>
 <tr>
 <td>ipsec_lease_hold</td>
 <td><code class="docutils literal notranslate">v8.0.0 -> 8.0.0 </code></td>
 </tr>
 </table>
 </div>
 </li>
        <li> <span class="li-head">lease_time</span> - Lease time in seconds, 0 means unlimited. <span class="li-normal">type: int</span>
 <a id='label106' href="javascript:ContentClick('label107', 'label106');" onmouseover="ContentPreview('label107');" onmouseout="ContentUnpreview('label107');" title="click to collapse or expand..."> more... </a>
 <div id="label107" style="display:none">
 <table border="1">
 <tr>
 <td></td>
 <td colspan="1">Supported Version Ranges</td>
 </tr>
 <tr>
 <td>lease_time</td>
 <td><code class="docutils literal notranslate">v8.0.0 -> 8.0.0 </code></td>
 </tr>
 </table>
 </div>
 </li>
        <li> <span class="li-head">mac_acl_default_action</span> - MAC access control default action (allow or block assigning IP settings). <span class="li-normal">type: str</span> <span class="li-normal">choices: assign, block</span>
 <a id='label108' href="javascript:ContentClick('label109', 'label108');" onmouseover="ContentPreview('label109');" onmouseout="ContentUnpreview('label109');" title="click to collapse or expand..."> more... </a>
 <div id="label109" style="display:none">
 <table border="1">
 <tr>
 <td></td>
 <td colspan="1">Supported Version Ranges</td>
 </tr>
 <tr>
 <td>mac_acl_default_action</td>
 <td><code class="docutils literal notranslate">v8.0.0 -> 8.0.0 </code></td>
 </tr>
 <tr>
 <td>[assign]</td>
 <td><code class="docutils literal notranslate">v8.0.0 -> 8.0.0</code></td>
 <tr>
 <td>[block]</td>
 <td><code class="docutils literal notranslate">v8.0.0 -> 8.0.0</code></td>
 </table>
 </div>
 </li>
        <li> <span class="li-head">name</span> - DHCP server template name. <span class="li-normal">type: str</span> <span class="li-required">required: true</span>
 <a id='label110' href="javascript:ContentClick('label111', 'label110');" onmouseover="ContentPreview('label111');" onmouseout="ContentUnpreview('label111');" title="click to collapse or expand..."> more... </a>
 <div id="label111" style="display:none">
 <table border="1">
 <tr>
 <td></td>
 <td colspan="1">Supported Version Ranges</td>
 </tr>
 <tr>
 <td>name</td>
 <td><code class="docutils literal notranslate">v8.0.0 -> 8.0.0 </code></td>
 </tr>
 </table>
 </div>
 </li>
        <li> <span class="li-head">next_server</span> - IP address of a server, such as a TFTP server, from which DHCP clients can download a boot file. <span class="li-normal">type: str</span>
 <a id='label112' href="javascript:ContentClick('label113', 'label112');" onmouseover="ContentPreview('label113');" onmouseout="ContentUnpreview('label113');" title="click to collapse or expand..."> more... </a>
 <div id="label113" style="display:none">
 <table border="1">
 <tr>
 <td></td>
 <td colspan="1">Supported Version Ranges</td>
 </tr>
 <tr>
 <td>next_server</td>
 <td><code class="docutils literal notranslate">v8.0.0 -> 8.0.0 </code></td>
 </tr>
 </table>
 </div>
 </li>
        <li> <span class="li-head">ntp_server1</span> - NTP server 1. <span class="li-normal">type: str</span>
 <a id='label114' href="javascript:ContentClick('label115', 'label114');" onmouseover="ContentPreview('label115');" onmouseout="ContentUnpreview('label115');" title="click to collapse or expand..."> more... </a>
 <div id="label115" style="display:none">
 <table border="1">
 <tr>
 <td></td>
 <td colspan="1">Supported Version Ranges</td>
 </tr>
 <tr>
 <td>ntp_server1</td>
 <td><code class="docutils literal notranslate">v8.0.0 -> 8.0.0 </code></td>
 </tr>
 </table>
 </div>
 </li>
        <li> <span class="li-head">ntp_server2</span> - NTP server 2. <span class="li-normal">type: str</span>
 <a id='label116' href="javascript:ContentClick('label117', 'label116');" onmouseover="ContentPreview('label117');" onmouseout="ContentUnpreview('label117');" title="click to collapse or expand..."> more... </a>
 <div id="label117" style="display:none">
 <table border="1">
 <tr>
 <td></td>
 <td colspan="1">Supported Version Ranges</td>
 </tr>
 <tr>
 <td>ntp_server2</td>
 <td><code class="docutils literal notranslate">v8.0.0 -> 8.0.0 </code></td>
 </tr>
 </table>
 </div>
 </li>
        <li> <span class="li-head">ntp_server3</span> - NTP server 3. <span class="li-normal">type: str</span>
 <a id='label118' href="javascript:ContentClick('label119', 'label118');" onmouseover="ContentPreview('label119');" onmouseout="ContentUnpreview('label119');" title="click to collapse or expand..."> more... </a>
 <div id="label119" style="display:none">
 <table border="1">
 <tr>
 <td></td>
 <td colspan="1">Supported Version Ranges</td>
 </tr>
 <tr>
 <td>ntp_server3</td>
 <td><code class="docutils literal notranslate">v8.0.0 -> 8.0.0 </code></td>
 </tr>
 </table>
 </div>
 </li>
        <li> <span class="li-head">ntp_service</span> - Options for assigning Network Time Protocol (NTP) servers to DHCP clients. <span class="li-normal">type: str</span> <span class="li-normal">choices: local, default, specify</span>
 <a id='label120' href="javascript:ContentClick('label121', 'label120');" onmouseover="ContentPreview('label121');" onmouseout="ContentUnpreview('label121');" title="click to collapse or expand..."> more... </a>
 <div id="label121" style="display:none">
 <table border="1">
 <tr>
 <td></td>
 <td colspan="1">Supported Version Ranges</td>
 </tr>
 <tr>
 <td>ntp_service</td>
 <td><code class="docutils literal notranslate">v8.0.0 -> 8.0.0 </code></td>
 </tr>
 <tr>
 <td>[local]</td>
 <td><code class="docutils literal notranslate">v8.0.0 -> 8.0.0</code></td>
 <tr>
 <td>[default]</td>
 <td><code class="docutils literal notranslate">v8.0.0 -> 8.0.0</code></td>
 <tr>
 <td>[specify]</td>
 <td><code class="docutils literal notranslate">v8.0.0 -> 8.0.0</code></td>
 </table>
 </div>
 </li>
        <li> <span class="li-head">options</span> - DHCP options. <span class="li-normal">type: list</span> <span style="font-family:'Courier New'" class="li-required">member_path: options:id</span>
 <a id='label122' href="javascript:ContentClick('label123', 'label122');" onmouseover="ContentPreview('label123');" onmouseout="ContentUnpreview('label123');" title="click to collapse or expand..."> more... </a>
 <div id="label123" style="display:none">
 <table border="1">
 <tr>
 <td></td><td colspan="1">Supported Version Ranges</td>
 </tr>
 <tr>
 <td>options</td>
 <td><code class="docutils literal notranslate">v8.0.0 -> 8.0.0 </code></td>
 </tr>
 </table>
 </div>
 </li>
            <ul class="ul-self">
            <li> <span class="li-head">code</span> - DHCP option code. <span class="li-normal">type: int</span>
 <a id='label124' href="javascript:ContentClick('label125', 'label124');" onmouseover="ContentPreview('label125');" onmouseout="ContentUnpreview('label125');" title="click to collapse or expand..."> more... </a>
 <div id="label125" style="display:none">
 <table border="1">
 <tr>
 <td></td>
 <td colspan="1">Supported Version Ranges</td>
 </tr>
 <tr>
 <td>code</td>
 <td><code class="docutils literal notranslate">v8.0.0 -> 8.0.0 </code></td>
 </tr>
 </table>
 </div>
 </li>
            <li> <span class="li-head">id</span> - ID. see <a href='#notes'>Notes</a>. <span class="li-normal">type: int</span> <span class="li-required">required: true</span>
 <a id='label126' href="javascript:ContentClick('label127', 'label126');" onmouseover="ContentPreview('label127');" onmouseout="ContentUnpreview('label127');" title="click to collapse or expand..."> more... </a>
 <div id="label127" style="display:none">
 <table border="1">
 <tr>
 <td></td>
 <td colspan="1">Supported Version Ranges</td>
 </tr>
 <tr>
 <td>id</td>
 <td><code class="docutils literal notranslate">v8.0.0 -> 8.0.0 </code></td>
 </tr>
 </table>
 </div>
 </li>
            <li> <span class="li-head">ip</span> - DHCP option IPs. <span class="li-normal">type: list</span> </li>
            <li> <span class="li-head">type</span> - DHCP option type. <span class="li-normal">type: str</span> <span class="li-normal">choices: hex, string, ip, fqdn</span>
 <a id='label128' href="javascript:ContentClick('label129', 'label128');" onmouseover="ContentPreview('label129');" onmouseout="ContentUnpreview('label129');" title="click to collapse or expand..."> more... </a>
 <div id="label129" style="display:none">
 <table border="1">
 <tr>
 <td></td>
 <td colspan="1">Supported Version Ranges</td>
 </tr>
 <tr>
 <td>type</td>
 <td><code class="docutils literal notranslate">v8.0.0 -> 8.0.0 </code></td>
 </tr>
 <tr>
 <td>[hex]</td>
 <td><code class="docutils literal notranslate">v8.0.0 -> 8.0.0</code></td>
 <tr>
 <td>[string]</td>
 <td><code class="docutils literal notranslate">v8.0.0 -> 8.0.0</code></td>
 <tr>
 <td>[ip]</td>
 <td><code class="docutils literal notranslate">v8.0.0 -> 8.0.0</code></td>
 <tr>
 <td>[fqdn]</td>
 <td><code class="docutils literal notranslate">v8.0.0 -> 8.0.0</code></td>
 </table>
 </div>
 </li>
            <li> <span class="li-head">uci_match</span> - Enable/disable user class identifier (UCI) matching. When enabled only DHCP requests with a matching UCI are served with this option. <span class="li-normal">type: str</span> <span class="li-normal">choices: disable, enable</span>
 <a id='label130' href="javascript:ContentClick('label131', 'label130');" onmouseover="ContentPreview('label131');" onmouseout="ContentUnpreview('label131');" title="click to collapse or expand..."> more... </a>
 <div id="label131" style="display:none">
 <table border="1">
 <tr>
 <td></td>
 <td colspan="1">Supported Version Ranges</td>
 </tr>
 <tr>
 <td>uci_match</td>
 <td><code class="docutils literal notranslate">v8.0.0 -> 8.0.0 </code></td>
 </tr>
 <tr>
 <td>[disable]</td>
 <td><code class="docutils literal notranslate">v8.0.0 -> 8.0.0</code></td>
 <tr>
 <td>[enable]</td>
 <td><code class="docutils literal notranslate">v8.0.0 -> 8.0.0</code></td>
 </table>
 </div>
 </li>
            <li> <span class="li-head">uci_string</span> - One or more UCI strings in quotes separated by spaces. <span class="li-normal">type: list</span> <span style="font-family:'Courier New'" class="li-required">member_path: options:id/uci_string:uci_string</span>
 <a id='label132' href="javascript:ContentClick('label133', 'label132');" onmouseover="ContentPreview('label133');" onmouseout="ContentUnpreview('label133');" title="click to collapse or expand..."> more... </a>
 <div id="label133" style="display:none">
 <table border="1">
 <tr>
 <td></td><td colspan="1">Supported Version Ranges</td>
 </tr>
 <tr>
 <td>uci_string</td>
 <td><code class="docutils literal notranslate">v8.0.0 -> 8.0.0 </code></td>
 </tr>
 </table>
 </div>
 </li>
                <ul class="ul-self">
                <li> <span class="li-head">uci_string</span> - UCI strings. <span class="li-normal">type: str</span> <span class="li-required">required: true</span>
 <a id='label134' href="javascript:ContentClick('label135', 'label134');" onmouseover="ContentPreview('label135');" onmouseout="ContentUnpreview('label135');" title="click to collapse or expand..."> more... </a>
 <div id="label135" style="display:none">
 <table border="1">
 <tr>
 <td></td>
 <td colspan="1">Supported Version Ranges</td>
 </tr>
 <tr>
 <td>uci_string</td>
 <td><code class="docutils literal notranslate">v8.0.0 -> 8.0.0 </code></td>
 </tr>
 </table>
 </div>
 </li>
                </ul>
            <li> <span class="li-head">value</span> - DHCP option value. <span class="li-normal">type: str</span>
 <a id='label136' href="javascript:ContentClick('label137', 'label136');" onmouseover="ContentPreview('label137');" onmouseout="ContentUnpreview('label137');" title="click to collapse or expand..."> more... </a>
 <div id="label137" style="display:none">
 <table border="1">
 <tr>
 <td></td>
 <td colspan="1">Supported Version Ranges</td>
 </tr>
 <tr>
 <td>value</td>
 <td><code class="docutils literal notranslate">v8.0.0 -> 8.0.0 </code></td>
 </tr>
 </table>
 </div>
 </li>
            <li> <span class="li-head">vci_match</span> - Enable/disable vendor class identifier (VCI) matching. When enabled only DHCP requests with a matching VCI are served with this option. <span class="li-normal">type: str</span> <span class="li-normal">choices: disable, enable</span>
 <a id='label138' href="javascript:ContentClick('label139', 'label138');" onmouseover="ContentPreview('label139');" onmouseout="ContentUnpreview('label139');" title="click to collapse or expand..."> more... </a>
 <div id="label139" style="display:none">
 <table border="1">
 <tr>
 <td></td>
 <td colspan="1">Supported Version Ranges</td>
 </tr>
 <tr>
 <td>vci_match</td>
 <td><code class="docutils literal notranslate">v8.0.0 -> 8.0.0 </code></td>
 </tr>
 <tr>
 <td>[disable]</td>
 <td><code class="docutils literal notranslate">v8.0.0 -> 8.0.0</code></td>
 <tr>
 <td>[enable]</td>
 <td><code class="docutils literal notranslate">v8.0.0 -> 8.0.0</code></td>
 </table>
 </div>
 </li>
            <li> <span class="li-head">vci_string</span> - One or more VCI strings in quotes separated by spaces. <span class="li-normal">type: list</span> <span style="font-family:'Courier New'" class="li-required">member_path: options:id/vci_string:vci_string</span>
 <a id='label140' href="javascript:ContentClick('label141', 'label140');" onmouseover="ContentPreview('label141');" onmouseout="ContentUnpreview('label141');" title="click to collapse or expand..."> more... </a>
 <div id="label141" style="display:none">
 <table border="1">
 <tr>
 <td></td><td colspan="1">Supported Version Ranges</td>
 </tr>
 <tr>
 <td>vci_string</td>
 <td><code class="docutils literal notranslate">v8.0.0 -> 8.0.0 </code></td>
 </tr>
 </table>
 </div>
 </li>
                <ul class="ul-self">
                <li> <span class="li-head">vci_string</span> - VCI strings. <span class="li-normal">type: str</span> <span class="li-required">required: true</span>
 <a id='label142' href="javascript:ContentClick('label143', 'label142');" onmouseover="ContentPreview('label143');" onmouseout="ContentUnpreview('label143');" title="click to collapse or expand..."> more... </a>
 <div id="label143" style="display:none">
 <table border="1">
 <tr>
 <td></td>
 <td colspan="1">Supported Version Ranges</td>
 </tr>
 <tr>
 <td>vci_string</td>
 <td><code class="docutils literal notranslate">v8.0.0 -> 8.0.0 </code></td>
 </tr>
 </table>
 </div>
 </li>
                </ul>
            </ul>
        <li> <span class="li-head">relay_agent</span> - Relay agent IP. <span class="li-normal">type: str</span>
 <a id='label144' href="javascript:ContentClick('label145', 'label144');" onmouseover="ContentPreview('label145');" onmouseout="ContentUnpreview('label145');" title="click to collapse or expand..."> more... </a>
 <div id="label145" style="display:none">
 <table border="1">
 <tr>
 <td></td>
 <td colspan="1">Supported Version Ranges</td>
 </tr>
 <tr>
 <td>relay_agent</td>
 <td><code class="docutils literal notranslate">v8.0.0 -> 8.0.0 </code></td>
 </tr>
 </table>
 </div>
 </li>
        <li> <span class="li-head">reserve_extra_addresses</span> - Enable/disable reservation of the extra IP addresses in the subnet. <span class="li-normal">type: str</span> <span class="li-normal">choices: disable, enable</span>
 <a id='label146' href="javascript:ContentClick('label147', 'label146');" onmouseover="ContentPreview('label147');" onmouseout="ContentUnpreview('label147');" title="click to collapse or expand..."> more... </a>
 <div id="label147" style="display:none">
 <table border="1">
 <tr>
 <td></td>
 <td colspan="1">Supported Version Ranges</td>
 </tr>
 <tr>
 <td>reserve_extra_addresses</td>
 <td><code class="docutils literal notranslate">v8.0.0 -> 8.0.0 </code></td>
 </tr>
 <tr>
 <td>[disable]</td>
 <td><code class="docutils literal notranslate">v8.0.0 -> 8.0.0</code></td>
 <tr>
 <td>[enable]</td>
 <td><code class="docutils literal notranslate">v8.0.0 -> 8.0.0</code></td>
 </table>
 </div>
 </li>
        <li> <span class="li-head">reserved_address</span> - Options for the DHCP server to assign IP settings to specific MAC addresses. <span class="li-normal">type: list</span> <span style="font-family:'Courier New'" class="li-required">member_path: reserved_address:id</span>
 <a id='label148' href="javascript:ContentClick('label149', 'label148');" onmouseover="ContentPreview('label149');" onmouseout="ContentUnpreview('label149');" title="click to collapse or expand..."> more... </a>
 <div id="label149" style="display:none">
 <table border="1">
 <tr>
 <td></td><td colspan="1">Supported Version Ranges</td>
 </tr>
 <tr>
 <td>reserved_address</td>
 <td><code class="docutils literal notranslate">v8.0.0 -> 8.0.0 </code></td>
 </tr>
 </table>
 </div>
 </li>
            <ul class="ul-self">
            <li> <span class="li-head">action</span> - Options for the DHCP server to configure the client with the reserved MAC address. <span class="li-normal">type: str</span> <span class="li-normal">choices: assign, block, reserved</span>
 <a id='label150' href="javascript:ContentClick('label151', 'label150');" onmouseover="ContentPreview('label151');" onmouseout="ContentUnpreview('label151');" title="click to collapse or expand..."> more... </a>
 <div id="label151" style="display:none">
 <table border="1">
 <tr>
 <td></td>
 <td colspan="1">Supported Version Ranges</td>
 </tr>
 <tr>
 <td>action</td>
 <td><code class="docutils literal notranslate">v8.0.0 -> 8.0.0 </code></td>
 </tr>
 <tr>
 <td>[assign]</td>
 <td><code class="docutils literal notranslate">v8.0.0 -> 8.0.0</code></td>
 <tr>
 <td>[block]</td>
 <td><code class="docutils literal notranslate">v8.0.0 -> 8.0.0</code></td>
 <tr>
 <td>[reserved]</td>
 <td><code class="docutils literal notranslate">v8.0.0 -> 8.0.0</code></td>
 </table>
 </div>
 </li>
            <li> <span class="li-head">circuit_id</span> - Option 82 circuit-ID of the client that will get the reserved IP address. <span class="li-normal">type: str</span>
 <a id='label152' href="javascript:ContentClick('label153', 'label152');" onmouseover="ContentPreview('label153');" onmouseout="ContentUnpreview('label153');" title="click to collapse or expand..."> more... </a>
 <div id="label153" style="display:none">
 <table border="1">
 <tr>
 <td></td>
 <td colspan="1">Supported Version Ranges</td>
 </tr>
 <tr>
 <td>circuit_id</td>
 <td><code class="docutils literal notranslate">v8.0.0 -> 8.0.0 </code></td>
 </tr>
 </table>
 </div>
 </li>
            <li> <span class="li-head">circuit_id_type</span> - DHCP option type. <span class="li-normal">type: str</span> <span class="li-normal">choices: hex, string</span>
 <a id='label154' href="javascript:ContentClick('label155', 'label154');" onmouseover="ContentPreview('label155');" onmouseout="ContentUnpreview('label155');" title="click to collapse or expand..."> more... </a>
 <div id="label155" style="display:none">
 <table border="1">
 <tr>
 <td></td>
 <td colspan="1">Supported Version Ranges</td>
 </tr>
 <tr>
 <td>circuit_id_type</td>
 <td><code class="docutils literal notranslate">v8.0.0 -> 8.0.0 </code></td>
 </tr>
 <tr>
 <td>[hex]</td>
 <td><code class="docutils literal notranslate">v8.0.0 -> 8.0.0</code></td>
 <tr>
 <td>[string]</td>
 <td><code class="docutils literal notranslate">v8.0.0 -> 8.0.0</code></td>
 </table>
 </div>
 </li>
            <li> <span class="li-head">description</span> - Description. <span class="li-normal">type: str</span>
 <a id='label156' href="javascript:ContentClick('label157', 'label156');" onmouseover="ContentPreview('label157');" onmouseout="ContentUnpreview('label157');" title="click to collapse or expand..."> more... </a>
 <div id="label157" style="display:none">
 <table border="1">
 <tr>
 <td></td>
 <td colspan="1">Supported Version Ranges</td>
 </tr>
 <tr>
 <td>description</td>
 <td><code class="docutils literal notranslate">v8.0.0 -> 8.0.0 </code></td>
 </tr>
 </table>
 </div>
 </li>
            <li> <span class="li-head">id</span> - ID. see <a href='#notes'>Notes</a>. <span class="li-normal">type: int</span> <span class="li-required">required: true</span>
 <a id='label158' href="javascript:ContentClick('label159', 'label158');" onmouseover="ContentPreview('label159');" onmouseout="ContentUnpreview('label159');" title="click to collapse or expand..."> more... </a>
 <div id="label159" style="display:none">
 <table border="1">
 <tr>
 <td></td>
 <td colspan="1">Supported Version Ranges</td>
 </tr>
 <tr>
 <td>id</td>
 <td><code class="docutils literal notranslate">v8.0.0 -> 8.0.0 </code></td>
 </tr>
 </table>
 </div>
 </li>
            <li> <span class="li-head">ip_index</span> - Index of IP address to be reserved for the MAC address. <span class="li-normal">type: int</span>
 <a id='label160' href="javascript:ContentClick('label161', 'label160');" onmouseover="ContentPreview('label161');" onmouseout="ContentUnpreview('label161');" title="click to collapse or expand..."> more... </a>
 <div id="label161" style="display:none">
 <table border="1">
 <tr>
 <td></td>
 <td colspan="1">Supported Version Ranges</td>
 </tr>
 <tr>
 <td>ip_index</td>
 <td><code class="docutils literal notranslate">v8.0.0 -> 8.0.0 </code></td>
 </tr>
 </table>
 </div>
 </li>
            <li> <span class="li-head">mac</span> - MAC address of the client that will get the reserved IP address. <span class="li-normal">type: str</span>
 <a id='label162' href="javascript:ContentClick('label163', 'label162');" onmouseover="ContentPreview('label163');" onmouseout="ContentUnpreview('label163');" title="click to collapse or expand..."> more... </a>
 <div id="label163" style="display:none">
 <table border="1">
 <tr>
 <td></td>
 <td colspan="1">Supported Version Ranges</td>
 </tr>
 <tr>
 <td>mac</td>
 <td><code class="docutils literal notranslate">v8.0.0 -> 8.0.0 </code></td>
 </tr>
 </table>
 </div>
 </li>
            <li> <span class="li-head">remote_id</span> - Option 82 remote-ID of the client that will get the reserved IP address. <span class="li-normal">type: str</span>
 <a id='label164' href="javascript:ContentClick('label165', 'label164');" onmouseover="ContentPreview('label165');" onmouseout="ContentUnpreview('label165');" title="click to collapse or expand..."> more... </a>
 <div id="label165" style="display:none">
 <table border="1">
 <tr>
 <td></td>
 <td colspan="1">Supported Version Ranges</td>
 </tr>
 <tr>
 <td>remote_id</td>
 <td><code class="docutils literal notranslate">v8.0.0 -> 8.0.0 </code></td>
 </tr>
 </table>
 </div>
 </li>
            <li> <span class="li-head">remote_id_type</span> - DHCP option type. <span class="li-normal">type: str</span> <span class="li-normal">choices: hex, string</span>
 <a id='label166' href="javascript:ContentClick('label167', 'label166');" onmouseover="ContentPreview('label167');" onmouseout="ContentUnpreview('label167');" title="click to collapse or expand..."> more... </a>
 <div id="label167" style="display:none">
 <table border="1">
 <tr>
 <td></td>
 <td colspan="1">Supported Version Ranges</td>
 </tr>
 <tr>
 <td>remote_id_type</td>
 <td><code class="docutils literal notranslate">v8.0.0 -> 8.0.0 </code></td>
 </tr>
 <tr>
 <td>[hex]</td>
 <td><code class="docutils literal notranslate">v8.0.0 -> 8.0.0</code></td>
 <tr>
 <td>[string]</td>
 <td><code class="docutils literal notranslate">v8.0.0 -> 8.0.0</code></td>
 </table>
 </div>
 </li>
            <li> <span class="li-head">type</span> - DHCP reserved-address type. <span class="li-normal">type: str</span> <span class="li-normal">choices: mac, option82</span>
 <a id='label168' href="javascript:ContentClick('label169', 'label168');" onmouseover="ContentPreview('label169');" onmouseout="ContentUnpreview('label169');" title="click to collapse or expand..."> more... </a>
 <div id="label169" style="display:none">
 <table border="1">
 <tr>
 <td></td>
 <td colspan="1">Supported Version Ranges</td>
 </tr>
 <tr>
 <td>type</td>
 <td><code class="docutils literal notranslate">v8.0.0 -> 8.0.0 </code></td>
 </tr>
 <tr>
 <td>[mac]</td>
 <td><code class="docutils literal notranslate">v8.0.0 -> 8.0.0</code></td>
 <tr>
 <td>[option82]</td>
 <td><code class="docutils literal notranslate">v8.0.0 -> 8.0.0</code></td>
 </table>
 </div>
 </li>
            </ul>
        <li> <span class="li-head">server_type</span> - DHCP server can be a normal DHCP server or an IPsec DHCP server. <span class="li-normal">type: str</span> <span class="li-normal">choices: regular, ipsec</span>
 <a id='label170' href="javascript:ContentClick('label171', 'label170');" onmouseover="ContentPreview('label171');" onmouseout="ContentUnpreview('label171');" title="click to collapse or expand..."> more... </a>
 <div id="label171" style="display:none">
 <table border="1">
 <tr>
 <td></td>
 <td colspan="1">Supported Version Ranges</td>
 </tr>
 <tr>
 <td>server_type</td>
 <td><code class="docutils literal notranslate">v8.0.0 -> 8.0.0 </code></td>
 </tr>
 <tr>
 <td>[regular]</td>
 <td><code class="docutils literal notranslate">v8.0.0 -> 8.0.0</code></td>
 <tr>
 <td>[ipsec]</td>
 <td><code class="docutils literal notranslate">v8.0.0 -> 8.0.0</code></td>
 </table>
 </div>
 </li>
        <li> <span class="li-head">shared_subnet</span> - Enable/disable shared subnet. <span class="li-normal">type: str</span> <span class="li-normal">choices: disable, enable</span>
 <a id='label172' href="javascript:ContentClick('label173', 'label172');" onmouseover="ContentPreview('label173');" onmouseout="ContentUnpreview('label173');" title="click to collapse or expand..."> more... </a>
 <div id="label173" style="display:none">
 <table border="1">
 <tr>
 <td></td>
 <td colspan="1">Supported Version Ranges</td>
 </tr>
 <tr>
 <td>shared_subnet</td>
 <td><code class="docutils literal notranslate">v8.0.0 -> 8.0.0 </code></td>
 </tr>
 <tr>
 <td>[disable]</td>
 <td><code class="docutils literal notranslate">v8.0.0 -> 8.0.0</code></td>
 <tr>
 <td>[enable]</td>
 <td><code class="docutils literal notranslate">v8.0.0 -> 8.0.0</code></td>
 </table>
 </div>
 </li>
        <li> <span class="li-head">tftp_server</span> - One or more hostnames or IP addresses of the TFTP servers in quotes separated by spaces. <span class="li-normal">type: list</span> <span style="font-family:'Courier New'" class="li-required">member_path: tftp_server:tftp_server</span>
 <a id='label174' href="javascript:ContentClick('label175', 'label174');" onmouseover="ContentPreview('label175');" onmouseout="ContentUnpreview('label175');" title="click to collapse or expand..."> more... </a>
 <div id="label175" style="display:none">
 <table border="1">
 <tr>
 <td></td><td colspan="1">Supported Version Ranges</td>
 </tr>
 <tr>
 <td>tftp_server</td>
 <td><code class="docutils literal notranslate">v8.0.0 -> 8.0.0 </code></td>
 </tr>
 </table>
 </div>
 </li>
            <ul class="ul-self">
            <li> <span class="li-head">tftp_server</span> - TFTP server. <span class="li-normal">type: str</span> <span class="li-required">required: true</span>
 <a id='label176' href="javascript:ContentClick('label177', 'label176');" onmouseover="ContentPreview('label177');" onmouseout="ContentUnpreview('label177');" title="click to collapse or expand..."> more... </a>
 <div id="label177" style="display:none">
 <table border="1">
 <tr>
 <td></td>
 <td colspan="1">Supported Version Ranges</td>
 </tr>
 <tr>
 <td>tftp_server</td>
 <td><code class="docutils literal notranslate">v8.0.0 -> 8.0.0 </code></td>
 </tr>
 </table>
 </div>
 </li>
            </ul>
        <li> <span class="li-head">timezone</span> - Select the time zone to be assigned to DHCP clients. Source system.timezone.name. <span class="li-normal">type: str</span>
 <a id='label178' href="javascript:ContentClick('label179', 'label178');" onmouseover="ContentPreview('label179');" onmouseout="ContentUnpreview('label179');" title="click to collapse or expand..."> more... </a>
 <div id="label179" style="display:none">
 <table border="1">
 <tr>
 <td></td>
 <td colspan="1">Supported Version Ranges</td>
 </tr>
 <tr>
 <td>timezone</td>
 <td><code class="docutils literal notranslate">v8.0.0 -> 8.0.0 </code></td>
 </tr>
 </table>
 </div>
 </li>
        <li> <span class="li-head">timezone_option</span> - Options for the DHCP server to set the client"s time zone. <span class="li-normal">type: str</span> <span class="li-normal">choices: disable, default, specify</span>
 <a id='label180' href="javascript:ContentClick('label181', 'label180');" onmouseover="ContentPreview('label181');" onmouseout="ContentUnpreview('label181');" title="click to collapse or expand..."> more... </a>
 <div id="label181" style="display:none">
 <table border="1">
 <tr>
 <td></td>
 <td colspan="1">Supported Version Ranges</td>
 </tr>
 <tr>
 <td>timezone_option</td>
 <td><code class="docutils literal notranslate">v8.0.0 -> 8.0.0 </code></td>
 </tr>
 <tr>
 <td>[disable]</td>
 <td><code class="docutils literal notranslate">v8.0.0 -> 8.0.0</code></td>
 <tr>
 <td>[default]</td>
 <td><code class="docutils literal notranslate">v8.0.0 -> 8.0.0</code></td>
 <tr>
 <td>[specify]</td>
 <td><code class="docutils literal notranslate">v8.0.0 -> 8.0.0</code></td>
 </table>
 </div>
 </li>
        <li> <span class="li-head">uuid</span> - Universally Unique Identifier (UUID; automatically assigned but can be manually reset). <span class="li-normal">type: str</span>
 <a id='label182' href="javascript:ContentClick('label183', 'label182');" onmouseover="ContentPreview('label183');" onmouseout="ContentUnpreview('label183');" title="click to collapse or expand..."> more... </a>
 <div id="label183" style="display:none">
 <table border="1">
 <tr>
 <td></td>
 <td colspan="1">Supported Version Ranges</td>
 </tr>
 <tr>
 <td>uuid</td>
 <td><code class="docutils literal notranslate">v8.0.0 -> 8.0.0 </code></td>
 </tr>
 </table>
 </div>
 </li>
        <li> <span class="li-head">vci_match</span> - Enable/disable vendor class identifier (VCI) matching. When enabled only DHCP requests with a matching VCI are served. <span class="li-normal">type: str</span> <span class="li-normal">choices: disable, enable</span>
 <a id='label184' href="javascript:ContentClick('label185', 'label184');" onmouseover="ContentPreview('label185');" onmouseout="ContentUnpreview('label185');" title="click to collapse or expand..."> more... </a>
 <div id="label185" style="display:none">
 <table border="1">
 <tr>
 <td></td>
 <td colspan="1">Supported Version Ranges</td>
 </tr>
 <tr>
 <td>vci_match</td>
 <td><code class="docutils literal notranslate">v8.0.0 -> 8.0.0 </code></td>
 </tr>
 <tr>
 <td>[disable]</td>
 <td><code class="docutils literal notranslate">v8.0.0 -> 8.0.0</code></td>
 <tr>
 <td>[enable]</td>
 <td><code class="docutils literal notranslate">v8.0.0 -> 8.0.0</code></td>
 </table>
 </div>
 </li>
        <li> <span class="li-head">vci_string</span> - One or more VCI strings in quotes separated by spaces. <span class="li-normal">type: list</span> <span style="font-family:'Courier New'" class="li-required">member_path: vci_string:vci_string</span>
 <a id='label186' href="javascript:ContentClick('label187', 'label186');" onmouseover="ContentPreview('label187');" onmouseout="ContentUnpreview('label187');" title="click to collapse or expand..."> more... </a>
 <div id="label187" style="display:none">
 <table border="1">
 <tr>
 <td></td><td colspan="1">Supported Version Ranges</td>
 </tr>
 <tr>
 <td>vci_string</td>
 <td><code class="docutils literal notranslate">v8.0.0 -> 8.0.0 </code></td>
 </tr>
 </table>
 </div>
 </li>
            <ul class="ul-self">
            <li> <span class="li-head">vci_string</span> - VCI strings. <span class="li-normal">type: str</span> <span class="li-required">required: true</span>
 <a id='label188' href="javascript:ContentClick('label189', 'label188');" onmouseover="ContentPreview('label189');" onmouseout="ContentUnpreview('label189');" title="click to collapse or expand..."> more... </a>
 <div id="label189" style="display:none">
 <table border="1">
 <tr>
 <td></td>
 <td colspan="1">Supported Version Ranges</td>
 </tr>
 <tr>
 <td>vci_string</td>
 <td><code class="docutils literal notranslate">v8.0.0 -> 8.0.0 </code></td>
 </tr>
 </table>
 </div>
 </li>
            </ul>
        <li> <span class="li-head">wifi_ac_service</span> - Options for assigning WiFi access controllers to DHCP clients. <span class="li-normal">type: str</span> <span class="li-normal">choices: specify, local</span>
 <a id='label190' href="javascript:ContentClick('label191', 'label190');" onmouseover="ContentPreview('label191');" onmouseout="ContentUnpreview('label191');" title="click to collapse or expand..."> more... </a>
 <div id="label191" style="display:none">
 <table border="1">
 <tr>
 <td></td>
 <td colspan="1">Supported Version Ranges</td>
 </tr>
 <tr>
 <td>wifi_ac_service</td>
 <td><code class="docutils literal notranslate">v8.0.0 -> 8.0.0 </code></td>
 </tr>
 <tr>
 <td>[specify]</td>
 <td><code class="docutils literal notranslate">v8.0.0 -> 8.0.0</code></td>
 <tr>
 <td>[local]</td>
 <td><code class="docutils literal notranslate">v8.0.0 -> 8.0.0</code></td>
 </table>
 </div>
 </li>
        <li> <span class="li-head">wifi_ac1</span> - WiFi Access Controller 1 IP address (DHCP option 138, RFC 5417). <span class="li-normal">type: str</span>
 <a id='label192' href="javascript:ContentClick('label193', 'label192');" onmouseover="ContentPreview('label193');" onmouseout="ContentUnpreview('label193');" title="click to collapse or expand..."> more... </a>
 <div id="label193" style="display:none">
 <table border="1">
 <tr>
 <td></td>
 <td colspan="1">Supported Version Ranges</td>
 </tr>
 <tr>
 <td>wifi_ac1</td>
 <td><code class="docutils literal notranslate">v8.0.0 -> 8.0.0 </code></td>
 </tr>
 </table>
 </div>
 </li>
        <li> <span class="li-head">wifi_ac2</span> - WiFi Access Controller 2 IP address (DHCP option 138, RFC 5417). <span class="li-normal">type: str</span>
 <a id='label194' href="javascript:ContentClick('label195', 'label194');" onmouseover="ContentPreview('label195');" onmouseout="ContentUnpreview('label195');" title="click to collapse or expand..."> more... </a>
 <div id="label195" style="display:none">
 <table border="1">
 <tr>
 <td></td>
 <td colspan="1">Supported Version Ranges</td>
 </tr>
 <tr>
 <td>wifi_ac2</td>
 <td><code class="docutils literal notranslate">v8.0.0 -> 8.0.0 </code></td>
 </tr>
 </table>
 </div>
 </li>
        <li> <span class="li-head">wifi_ac3</span> - WiFi Access Controller 3 IP address (DHCP option 138, RFC 5417). <span class="li-normal">type: str</span>
 <a id='label196' href="javascript:ContentClick('label197', 'label196');" onmouseover="ContentPreview('label197');" onmouseout="ContentUnpreview('label197');" title="click to collapse or expand..."> more... </a>
 <div id="label197" style="display:none">
 <table border="1">
 <tr>
 <td></td>
 <td colspan="1">Supported Version Ranges</td>
 </tr>
 <tr>
 <td>wifi_ac3</td>
 <td><code class="docutils literal notranslate">v8.0.0 -> 8.0.0 </code></td>
 </tr>
 </table>
 </div>
 </li>
        <li> <span class="li-head">wins_server1</span> - WINS server 1. <span class="li-normal">type: str</span>
 <a id='label198' href="javascript:ContentClick('label199', 'label198');" onmouseover="ContentPreview('label199');" onmouseout="ContentUnpreview('label199');" title="click to collapse or expand..."> more... </a>
 <div id="label199" style="display:none">
 <table border="1">
 <tr>
 <td></td>
 <td colspan="1">Supported Version Ranges</td>
 </tr>
 <tr>
 <td>wins_server1</td>
 <td><code class="docutils literal notranslate">v8.0.0 -> 8.0.0 </code></td>
 </tr>
 </table>
 </div>
 </li>
        <li> <span class="li-head">wins_server2</span> - WINS server 2. <span class="li-normal">type: str</span>
 <a id='label200' href="javascript:ContentClick('label201', 'label200');" onmouseover="ContentPreview('label201');" onmouseout="ContentUnpreview('label201');" title="click to collapse or expand..."> more... </a>
 <div id="label201" style="display:none">
 <table border="1">
 <tr>
 <td></td>
 <td colspan="1">Supported Version Ranges</td>
 </tr>
 <tr>
 <td>wins_server2</td>
 <td><code class="docutils literal notranslate">v8.0.0 -> 8.0.0 </code></td>
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
    
    - name: Configure DHCP server templates.
      fortinet.fortios.fortios_system_dhcp_template:
          vdom: "{{ vdom }}"
          state: "present"
          access_token: "<your_own_value>"
          system_dhcp_template:
              auto_configuration: "disable"
              conflicted_ip_timeout: "1800"
              ddns_auth: "disable"
              ddns_key: "<your_own_value>"
              ddns_keyname: "<your_own_value>"
              ddns_server_ip: "<your_own_value>"
              ddns_ttl: "300"
              ddns_update: "disable"
              ddns_update_override: "disable"
              ddns_zone: "<your_own_value>"
              dns_server1: "<your_own_value>"
              dns_server2: "<your_own_value>"
              dns_server3: "<your_own_value>"
              dns_server4: "<your_own_value>"
              dns_service: "local"
              domain: "<your_own_value>"
              exclude_range:
                  -
                      id: "20"
                      ip_count: "0"
                      lease_time: "0"
                      oui_match: "disable"
                      oui_string:
                          -
                              oui_string: "<your_own_value>"
                      start_ip_index: "0"
                      uci_match: "disable"
                      uci_string:
                          -
                              uci_string: "<your_own_value>"
                      vci_match: "disable"
                      vci_string:
                          -
                              vci_string: "<your_own_value>"
                      vendor: "<your_own_value>"
              fabric_force_sync: "enable"
              fabric_object: "enable"
              fabric_object_source: "member"
              filename: "<your_own_value>"
              forticlient_on_net_status: "disable"
              ip_range:
                  -
                      id: "40"
                      ip_count: "0"
                      lease_time: "0"
                      oui_match: "disable"
                      oui_string:
                          -
                              oui_string: "<your_own_value>"
                      reserve: "disable"
                      uci_match: "disable"
                      uci_string:
                          -
                              uci_string: "<your_own_value>"
                      vci_match: "disable"
                      vci_string:
                          -
                              vci_string: "<your_own_value>"
                      vendor: "<your_own_value>"
              ipsec_lease_hold: "60"
              lease_time: "604800"
              mac_acl_default_action: "assign"
              name: "default_name_57"
              next_server: "<your_own_value>"
              ntp_server1: "<your_own_value>"
              ntp_server2: "<your_own_value>"
              ntp_server3: "<your_own_value>"
              ntp_service: "local"
              options:
                  -
                      code: "0"
                      id: "65"
                      ip: "<your_own_value>"
                      type: "hex"
                      uci_match: "disable"
                      uci_string:
                          -
                              uci_string: "<your_own_value>"
                      value: "<your_own_value>"
                      vci_match: "disable"
                      vci_string:
                          -
                              vci_string: "<your_own_value>"
              relay_agent: "<your_own_value>"
              reserve_extra_addresses: "disable"
              reserved_address:
                  -
                      action: "assign"
                      circuit_id: "<your_own_value>"
                      circuit_id_type: "hex"
                      description: "<your_own_value>"
                      id: "82"
                      ip_index: "0"
                      mac: "<your_own_value>"
                      remote_id: "<your_own_value>"
                      remote_id_type: "hex"
                      type: "mac"
              server_type: "regular"
              shared_subnet: "disable"
              tftp_server:
                  -
                      tftp_server: "<your_own_value>"
              timezone: "<your_own_value> (source system.timezone.name)"
              timezone_option: "disable"
              uuid: "<your_own_value>"
              vci_match: "disable"
              vci_string:
                  -
                      vci_string: "<your_own_value>"
              wifi_ac_service: "specify"
              wifi_ac1: "<your_own_value>"
              wifi_ac2: "<your_own_value>"
              wifi_ac3: "<your_own_value>"
              wins_server1: "<your_own_value>"
              wins_server2: "<your_own_value>"


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
