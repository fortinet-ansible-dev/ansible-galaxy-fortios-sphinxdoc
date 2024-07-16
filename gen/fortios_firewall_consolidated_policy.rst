:source: fortios_firewall_consolidated_policy.py

:orphan:

.. fortios_firewall_consolidated_policy:

fortios_firewall_consolidated_policy -- Configure consolidated IPv4/IPv6 policies in Fortinet's FortiOS and FortiGate.
++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++

.. versionadded:: 2.0.0

.. contents::
   :local:
   :depth: 1


Synopsis
--------
- This module is able to configure a FortiGate or FortiOS (FOS) device by allowing the user to set and modify firewall_consolidated feature and policy category. Examples include all parameters and values need to be adjusted to datasources before usage. Tested with FOS v6.0.0



Requirements
------------
The below requirements are needed on the host that executes this module.

- ansible>=2.15


Tips
----
Using member operation to add an element to an existing object.

FortiOS Version Compatibility
-----------------------------
Supported Version Ranges: v6.2.0 -> v6.2.7


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
    <li> <span class="li-head">firewall_consolidated_policy</span> - Configure consolidated IPv4/IPv6 policies. <span class="li-normal">type: dict</span>
 <a id='label0' href="javascript:ContentClick('label1', 'label0');" onmouseover="ContentPreview('label1');" onmouseout="ContentUnpreview('label1');" title="click to collapse or expand..."> more... </a>
 <div id="label1" style="display:none">
 <table border="1">
 <tr>
 <td></td><td colspan="1">Supported Version Ranges</td>
 </tr>
 <tr>
 <td>firewall_consolidated_policy</td>
 <td><code class="docutils literal notranslate">v6.2.0 -> v6.2.7 </code></td>
 </tr>
 </table>
 </div>
 </li>
        <ul class="ul-self">
        <li> <span class="li-head">action</span> - Policy action (allow/deny/ipsec). <span class="li-normal">type: str</span> <span class="li-normal">choices: accept, deny, ipsec</span>
 <a id='label2' href="javascript:ContentClick('label3', 'label2');" onmouseover="ContentPreview('label3');" onmouseout="ContentUnpreview('label3');" title="click to collapse or expand..."> more... </a>
 <div id="label3" style="display:none">
 <table border="1">
 <tr>
 <td></td>
 <td colspan="1">Supported Version Ranges</td>
 </tr>
 <tr>
 <td>action</td>
 <td><code class="docutils literal notranslate">v6.2.0 -> v6.2.7 </code></td>
 </tr>
 <tr>
 <td>[accept]</td>
 <td><code class="docutils literal notranslate">v6.2.0 -> v6.2.7</code></td>
 <tr>
 <td>[deny]</td>
 <td><code class="docutils literal notranslate">v6.2.0 -> v6.2.7</code></td>
 <tr>
 <td>[ipsec]</td>
 <td><code class="docutils literal notranslate">v6.2.0 -> v6.2.7</code></td>
 </table>
 </div>
 </li>
        <li> <span class="li-head">application_list</span> - Name of an existing Application list. Source application.list.name. <span class="li-normal">type: str</span>
 <a id='label4' href="javascript:ContentClick('label5', 'label4');" onmouseover="ContentPreview('label5');" onmouseout="ContentUnpreview('label5');" title="click to collapse or expand..."> more... </a>
 <div id="label5" style="display:none">
 <table border="1">
 <tr>
 <td></td>
 <td colspan="1">Supported Version Ranges</td>
 </tr>
 <tr>
 <td>application_list</td>
 <td><code class="docutils literal notranslate">v6.2.0 -> v6.2.7 </code></td>
 </tr>
 </table>
 </div>
 </li>
        <li> <span class="li-head">auto_asic_offload</span> - Enable/disable policy traffic ASIC offloading. <span class="li-normal">type: str</span> <span class="li-normal">choices: enable, disable</span>
 <a id='label6' href="javascript:ContentClick('label7', 'label6');" onmouseover="ContentPreview('label7');" onmouseout="ContentUnpreview('label7');" title="click to collapse or expand..."> more... </a>
 <div id="label7" style="display:none">
 <table border="1">
 <tr>
 <td></td>
 <td colspan="1">Supported Version Ranges</td>
 </tr>
 <tr>
 <td>auto_asic_offload</td>
 <td><code class="docutils literal notranslate">v6.2.0 -> v6.2.7 </code></td>
 </tr>
 <tr>
 <td>[enable]</td>
 <td><code class="docutils literal notranslate">v6.2.0 -> v6.2.7</code></td>
 <tr>
 <td>[disable]</td>
 <td><code class="docutils literal notranslate">v6.2.0 -> v6.2.7</code></td>
 </table>
 </div>
 </li>
        <li> <span class="li-head">av_profile</span> - Name of an existing Antivirus profile. Source antivirus.profile.name. <span class="li-normal">type: str</span>
 <a id='label8' href="javascript:ContentClick('label9', 'label8');" onmouseover="ContentPreview('label9');" onmouseout="ContentUnpreview('label9');" title="click to collapse or expand..."> more... </a>
 <div id="label9" style="display:none">
 <table border="1">
 <tr>
 <td></td>
 <td colspan="1">Supported Version Ranges</td>
 </tr>
 <tr>
 <td>av_profile</td>
 <td><code class="docutils literal notranslate">v6.2.0 -> v6.2.7 </code></td>
 </tr>
 </table>
 </div>
 </li>
        <li> <span class="li-head">captive_portal_exempt</span> - Enable exemption of some users from the captive portal. <span class="li-normal">type: str</span> <span class="li-normal">choices: enable, disable</span>
 <a id='label10' href="javascript:ContentClick('label11', 'label10');" onmouseover="ContentPreview('label11');" onmouseout="ContentUnpreview('label11');" title="click to collapse or expand..."> more... </a>
 <div id="label11" style="display:none">
 <table border="1">
 <tr>
 <td></td>
 <td colspan="1">Supported Version Ranges</td>
 </tr>
 <tr>
 <td>captive_portal_exempt</td>
 <td><code class="docutils literal notranslate">v6.2.0 -> v6.2.7 </code></td>
 </tr>
 <tr>
 <td>[enable]</td>
 <td><code class="docutils literal notranslate">v6.2.0 -> v6.2.7</code></td>
 <tr>
 <td>[disable]</td>
 <td><code class="docutils literal notranslate">v6.2.0 -> v6.2.7</code></td>
 </table>
 </div>
 </li>
        <li> <span class="li-head">cifs_profile</span> - Name of an existing CIFS profile. Source cifs.profile.name. <span class="li-normal">type: str</span>
 <a id='label12' href="javascript:ContentClick('label13', 'label12');" onmouseover="ContentPreview('label13');" onmouseout="ContentUnpreview('label13');" title="click to collapse or expand..."> more... </a>
 <div id="label13" style="display:none">
 <table border="1">
 <tr>
 <td></td>
 <td colspan="1">Supported Version Ranges</td>
 </tr>
 <tr>
 <td>cifs_profile</td>
 <td><code class="docutils literal notranslate">v6.2.0 -> v6.2.7 </code></td>
 </tr>
 </table>
 </div>
 </li>
        <li> <span class="li-head">comments</span> - Comment. <span class="li-normal">type: str</span>
 <a id='label14' href="javascript:ContentClick('label15', 'label14');" onmouseover="ContentPreview('label15');" onmouseout="ContentUnpreview('label15');" title="click to collapse or expand..."> more... </a>
 <div id="label15" style="display:none">
 <table border="1">
 <tr>
 <td></td>
 <td colspan="1">Supported Version Ranges</td>
 </tr>
 <tr>
 <td>comments</td>
 <td><code class="docutils literal notranslate">v6.2.0 -> v6.2.7 </code></td>
 </tr>
 </table>
 </div>
 </li>
        <li> <span class="li-head">diffserv_forward</span> - Enable to change packet"s DiffServ values to the specified diffservcode-forward value. <span class="li-normal">type: str</span> <span class="li-normal">choices: enable, disable</span>
 <a id='label16' href="javascript:ContentClick('label17', 'label16');" onmouseover="ContentPreview('label17');" onmouseout="ContentUnpreview('label17');" title="click to collapse or expand..."> more... </a>
 <div id="label17" style="display:none">
 <table border="1">
 <tr>
 <td></td>
 <td colspan="1">Supported Version Ranges</td>
 </tr>
 <tr>
 <td>diffserv_forward</td>
 <td><code class="docutils literal notranslate">v6.2.0 -> v6.2.7 </code></td>
 </tr>
 <tr>
 <td>[enable]</td>
 <td><code class="docutils literal notranslate">v6.2.0 -> v6.2.7</code></td>
 <tr>
 <td>[disable]</td>
 <td><code class="docutils literal notranslate">v6.2.0 -> v6.2.7</code></td>
 </table>
 </div>
 </li>
        <li> <span class="li-head">diffserv_reverse</span> - Enable to change packet"s reverse (reply) DiffServ values to the specified diffservcode-rev value. <span class="li-normal">type: str</span> <span class="li-normal">choices: enable, disable</span>
 <a id='label18' href="javascript:ContentClick('label19', 'label18');" onmouseover="ContentPreview('label19');" onmouseout="ContentUnpreview('label19');" title="click to collapse or expand..."> more... </a>
 <div id="label19" style="display:none">
 <table border="1">
 <tr>
 <td></td>
 <td colspan="1">Supported Version Ranges</td>
 </tr>
 <tr>
 <td>diffserv_reverse</td>
 <td><code class="docutils literal notranslate">v6.2.0 -> v6.2.7 </code></td>
 </tr>
 <tr>
 <td>[enable]</td>
 <td><code class="docutils literal notranslate">v6.2.0 -> v6.2.7</code></td>
 <tr>
 <td>[disable]</td>
 <td><code class="docutils literal notranslate">v6.2.0 -> v6.2.7</code></td>
 </table>
 </div>
 </li>
        <li> <span class="li-head">diffservcode_forward</span> - Change packet"s DiffServ to this value. <span class="li-normal">type: str</span>
 <a id='label20' href="javascript:ContentClick('label21', 'label20');" onmouseover="ContentPreview('label21');" onmouseout="ContentUnpreview('label21');" title="click to collapse or expand..."> more... </a>
 <div id="label21" style="display:none">
 <table border="1">
 <tr>
 <td></td>
 <td colspan="1">Supported Version Ranges</td>
 </tr>
 <tr>
 <td>diffservcode_forward</td>
 <td><code class="docutils literal notranslate">v6.2.0 -> v6.2.7 </code></td>
 </tr>
 </table>
 </div>
 </li>
        <li> <span class="li-head">diffservcode_rev</span> - Change packet"s reverse (reply) DiffServ to this value. <span class="li-normal">type: str</span>
 <a id='label22' href="javascript:ContentClick('label23', 'label22');" onmouseover="ContentPreview('label23');" onmouseout="ContentUnpreview('label23');" title="click to collapse or expand..."> more... </a>
 <div id="label23" style="display:none">
 <table border="1">
 <tr>
 <td></td>
 <td colspan="1">Supported Version Ranges</td>
 </tr>
 <tr>
 <td>diffservcode_rev</td>
 <td><code class="docutils literal notranslate">v6.2.0 -> v6.2.7 </code></td>
 </tr>
 </table>
 </div>
 </li>
        <li> <span class="li-head">dlp_sensor</span> - Name of an existing DLP sensor. Source dlp.sensor.name. <span class="li-normal">type: str</span>
 <a id='label24' href="javascript:ContentClick('label25', 'label24');" onmouseover="ContentPreview('label25');" onmouseout="ContentUnpreview('label25');" title="click to collapse or expand..."> more... </a>
 <div id="label25" style="display:none">
 <table border="1">
 <tr>
 <td></td>
 <td colspan="1">Supported Version Ranges</td>
 </tr>
 <tr>
 <td>dlp_sensor</td>
 <td><code class="docutils literal notranslate">v6.2.0 -> v6.2.7 </code></td>
 </tr>
 </table>
 </div>
 </li>
        <li> <span class="li-head">dnsfilter_profile</span> - Name of an existing DNS filter profile. Source dnsfilter.profile.name. <span class="li-normal">type: str</span>
 <a id='label26' href="javascript:ContentClick('label27', 'label26');" onmouseover="ContentPreview('label27');" onmouseout="ContentUnpreview('label27');" title="click to collapse or expand..."> more... </a>
 <div id="label27" style="display:none">
 <table border="1">
 <tr>
 <td></td>
 <td colspan="1">Supported Version Ranges</td>
 </tr>
 <tr>
 <td>dnsfilter_profile</td>
 <td><code class="docutils literal notranslate">v6.2.0 -> v6.2.7 </code></td>
 </tr>
 </table>
 </div>
 </li>
        <li> <span class="li-head">dstaddr_negate</span> - When enabled dstaddr specifies what the destination address must NOT be. <span class="li-normal">type: str</span> <span class="li-normal">choices: enable, disable</span>
 <a id='label28' href="javascript:ContentClick('label29', 'label28');" onmouseover="ContentPreview('label29');" onmouseout="ContentUnpreview('label29');" title="click to collapse or expand..."> more... </a>
 <div id="label29" style="display:none">
 <table border="1">
 <tr>
 <td></td>
 <td colspan="1">Supported Version Ranges</td>
 </tr>
 <tr>
 <td>dstaddr_negate</td>
 <td><code class="docutils literal notranslate">v6.2.0 -> v6.2.7 </code></td>
 </tr>
 <tr>
 <td>[enable]</td>
 <td><code class="docutils literal notranslate">v6.2.0 -> v6.2.7</code></td>
 <tr>
 <td>[disable]</td>
 <td><code class="docutils literal notranslate">v6.2.0 -> v6.2.7</code></td>
 </table>
 </div>
 </li>
        <li> <span class="li-head">dstaddr4</span> - Destination IPv4 address name and address group names. <span class="li-normal">type: list</span> <span style="font-family:'Courier New'" class="li-required">member_path: dstaddr4:name</span>
 <a id='label30' href="javascript:ContentClick('label31', 'label30');" onmouseover="ContentPreview('label31');" onmouseout="ContentUnpreview('label31');" title="click to collapse or expand..."> more... </a>
 <div id="label31" style="display:none">
 <table border="1">
 <tr>
 <td></td><td colspan="1">Supported Version Ranges</td>
 </tr>
 <tr>
 <td>dstaddr4</td>
 <td><code class="docutils literal notranslate">v6.2.0 -> v6.2.7 </code></td>
 </tr>
 </table>
 </div>
 </li>
            <ul class="ul-self">
            <li> <span class="li-head">name</span> - Address name. Source firewall.address.name firewall.addrgrp.name firewall.vip.name firewall.vipgrp.name system.external-resource .name. <span class="li-normal">type: str</span> <span class="li-required">required: true</span>
 <a id='label32' href="javascript:ContentClick('label33', 'label32');" onmouseover="ContentPreview('label33');" onmouseout="ContentUnpreview('label33');" title="click to collapse or expand..."> more... </a>
 <div id="label33" style="display:none">
 <table border="1">
 <tr>
 <td></td>
 <td colspan="1">Supported Version Ranges</td>
 </tr>
 <tr>
 <td>name</td>
 <td><code class="docutils literal notranslate">v6.2.0 -> v6.2.7 </code></td>
 </tr>
 </table>
 </div>
 </li>
            </ul>
        <li> <span class="li-head">dstaddr6</span> - Destination IPv6 address name and address group names. <span class="li-normal">type: list</span> <span style="font-family:'Courier New'" class="li-required">member_path: dstaddr6:name</span>
 <a id='label34' href="javascript:ContentClick('label35', 'label34');" onmouseover="ContentPreview('label35');" onmouseout="ContentUnpreview('label35');" title="click to collapse or expand..."> more... </a>
 <div id="label35" style="display:none">
 <table border="1">
 <tr>
 <td></td><td colspan="1">Supported Version Ranges</td>
 </tr>
 <tr>
 <td>dstaddr6</td>
 <td><code class="docutils literal notranslate">v6.2.0 -> v6.2.7 </code></td>
 </tr>
 </table>
 </div>
 </li>
            <ul class="ul-self">
            <li> <span class="li-head">name</span> - Address name. Source firewall.address6.name firewall.addrgrp6.name firewall.vip6.name firewall.vipgrp6.name system .external-resource.name. <span class="li-normal">type: str</span> <span class="li-required">required: true</span>
 <a id='label36' href="javascript:ContentClick('label37', 'label36');" onmouseover="ContentPreview('label37');" onmouseout="ContentUnpreview('label37');" title="click to collapse or expand..."> more... </a>
 <div id="label37" style="display:none">
 <table border="1">
 <tr>
 <td></td>
 <td colspan="1">Supported Version Ranges</td>
 </tr>
 <tr>
 <td>name</td>
 <td><code class="docutils literal notranslate">v6.2.0 -> v6.2.7 </code></td>
 </tr>
 </table>
 </div>
 </li>
            </ul>
        <li> <span class="li-head">dstintf</span> - Outgoing (egress) interface. <span class="li-normal">type: list</span> <span style="font-family:'Courier New'" class="li-required">member_path: dstintf:name</span>
 <a id='label38' href="javascript:ContentClick('label39', 'label38');" onmouseover="ContentPreview('label39');" onmouseout="ContentUnpreview('label39');" title="click to collapse or expand..."> more... </a>
 <div id="label39" style="display:none">
 <table border="1">
 <tr>
 <td></td><td colspan="1">Supported Version Ranges</td>
 </tr>
 <tr>
 <td>dstintf</td>
 <td><code class="docutils literal notranslate">v6.2.0 -> v6.2.7 </code></td>
 </tr>
 </table>
 </div>
 </li>
            <ul class="ul-self">
            <li> <span class="li-head">name</span> - Interface name. Source system.interface.name system.zone.name. <span class="li-normal">type: str</span> <span class="li-required">required: true</span>
 <a id='label40' href="javascript:ContentClick('label41', 'label40');" onmouseover="ContentPreview('label41');" onmouseout="ContentUnpreview('label41');" title="click to collapse or expand..."> more... </a>
 <div id="label41" style="display:none">
 <table border="1">
 <tr>
 <td></td>
 <td colspan="1">Supported Version Ranges</td>
 </tr>
 <tr>
 <td>name</td>
 <td><code class="docutils literal notranslate">v6.2.0 -> v6.2.7 </code></td>
 </tr>
 </table>
 </div>
 </li>
            </ul>
        <li> <span class="li-head">emailfilter_profile</span> - Name of an existing email filter profile. Source emailfilter.profile.name. <span class="li-normal">type: str</span>
 <a id='label42' href="javascript:ContentClick('label43', 'label42');" onmouseover="ContentPreview('label43');" onmouseout="ContentUnpreview('label43');" title="click to collapse or expand..."> more... </a>
 <div id="label43" style="display:none">
 <table border="1">
 <tr>
 <td></td>
 <td colspan="1">Supported Version Ranges</td>
 </tr>
 <tr>
 <td>emailfilter_profile</td>
 <td><code class="docutils literal notranslate">v6.2.0 -> v6.2.7 </code></td>
 </tr>
 </table>
 </div>
 </li>
        <li> <span class="li-head">fixedport</span> - Enable to prevent source NAT from changing a session"s source port. <span class="li-normal">type: str</span> <span class="li-normal">choices: enable, disable</span>
 <a id='label44' href="javascript:ContentClick('label45', 'label44');" onmouseover="ContentPreview('label45');" onmouseout="ContentUnpreview('label45');" title="click to collapse or expand..."> more... </a>
 <div id="label45" style="display:none">
 <table border="1">
 <tr>
 <td></td>
 <td colspan="1">Supported Version Ranges</td>
 </tr>
 <tr>
 <td>fixedport</td>
 <td><code class="docutils literal notranslate">v6.2.0 -> v6.2.7 </code></td>
 </tr>
 <tr>
 <td>[enable]</td>
 <td><code class="docutils literal notranslate">v6.2.0 -> v6.2.7</code></td>
 <tr>
 <td>[disable]</td>
 <td><code class="docutils literal notranslate">v6.2.0 -> v6.2.7</code></td>
 </table>
 </div>
 </li>
        <li> <span class="li-head">fsso_groups</span> - Names of FSSO groups. <span class="li-normal">type: list</span> <span style="font-family:'Courier New'" class="li-required">member_path: fsso_groups:name</span>
 <a id='label46' href="javascript:ContentClick('label47', 'label46');" onmouseover="ContentPreview('label47');" onmouseout="ContentUnpreview('label47');" title="click to collapse or expand..."> more... </a>
 <div id="label47" style="display:none">
 <table border="1">
 <tr>
 <td></td><td colspan="1">Supported Version Ranges</td>
 </tr>
 <tr>
 <td>fsso_groups</td>
 <td><code class="docutils literal notranslate">v6.2.0 -> v6.2.7 </code></td>
 </tr>
 </table>
 </div>
 </li>
            <ul class="ul-self">
            <li> <span class="li-head">name</span> - Names of FSSO groups. Source user.adgrp.name. <span class="li-normal">type: str</span> <span class="li-required">required: true</span>
 <a id='label48' href="javascript:ContentClick('label49', 'label48');" onmouseover="ContentPreview('label49');" onmouseout="ContentUnpreview('label49');" title="click to collapse or expand..."> more... </a>
 <div id="label49" style="display:none">
 <table border="1">
 <tr>
 <td></td>
 <td colspan="1">Supported Version Ranges</td>
 </tr>
 <tr>
 <td>name</td>
 <td><code class="docutils literal notranslate">v6.2.0 -> v6.2.7 </code></td>
 </tr>
 </table>
 </div>
 </li>
            </ul>
        <li> <span class="li-head">global_label</span> - Label for the policy that appears when the GUI is in Global View mode. <span class="li-normal">type: str</span>
 <a id='label50' href="javascript:ContentClick('label51', 'label50');" onmouseover="ContentPreview('label51');" onmouseout="ContentUnpreview('label51');" title="click to collapse or expand..."> more... </a>
 <div id="label51" style="display:none">
 <table border="1">
 <tr>
 <td></td>
 <td colspan="1">Supported Version Ranges</td>
 </tr>
 <tr>
 <td>global_label</td>
 <td><code class="docutils literal notranslate">v6.2.3 -> v6.2.3 </code></td>
 </tr>
 </table>
 </div>
 </li>
        <li> <span class="li-head">groups</span> - Names of user groups that can authenticate with this policy. <span class="li-normal">type: list</span> <span style="font-family:'Courier New'" class="li-required">member_path: groups:name</span>
 <a id='label52' href="javascript:ContentClick('label53', 'label52');" onmouseover="ContentPreview('label53');" onmouseout="ContentUnpreview('label53');" title="click to collapse or expand..."> more... </a>
 <div id="label53" style="display:none">
 <table border="1">
 <tr>
 <td></td><td colspan="1">Supported Version Ranges</td>
 </tr>
 <tr>
 <td>groups</td>
 <td><code class="docutils literal notranslate">v6.2.0 -> v6.2.7 </code></td>
 </tr>
 </table>
 </div>
 </li>
            <ul class="ul-self">
            <li> <span class="li-head">name</span> - Group name. Source user.group.name. <span class="li-normal">type: str</span> <span class="li-required">required: true</span>
 <a id='label54' href="javascript:ContentClick('label55', 'label54');" onmouseover="ContentPreview('label55');" onmouseout="ContentUnpreview('label55');" title="click to collapse or expand..."> more... </a>
 <div id="label55" style="display:none">
 <table border="1">
 <tr>
 <td></td>
 <td colspan="1">Supported Version Ranges</td>
 </tr>
 <tr>
 <td>name</td>
 <td><code class="docutils literal notranslate">v6.2.0 -> v6.2.7 </code></td>
 </tr>
 </table>
 </div>
 </li>
            </ul>
        <li> <span class="li-head">http_policy_redirect</span> - Redirect HTTP(S) traffic to matching transparent web proxy policy. <span class="li-normal">type: str</span> <span class="li-normal">choices: enable, disable</span>
 <a id='label56' href="javascript:ContentClick('label57', 'label56');" onmouseover="ContentPreview('label57');" onmouseout="ContentUnpreview('label57');" title="click to collapse or expand..."> more... </a>
 <div id="label57" style="display:none">
 <table border="1">
 <tr>
 <td></td>
 <td colspan="1">Supported Version Ranges</td>
 </tr>
 <tr>
 <td>http_policy_redirect</td>
 <td><code class="docutils literal notranslate">v6.2.0 -> v6.2.7 </code></td>
 </tr>
 <tr>
 <td>[enable]</td>
 <td><code class="docutils literal notranslate">v6.2.0 -> v6.2.7</code></td>
 <tr>
 <td>[disable]</td>
 <td><code class="docutils literal notranslate">v6.2.0 -> v6.2.7</code></td>
 </table>
 </div>
 </li>
        <li> <span class="li-head">icap_profile</span> - Name of an existing ICAP profile. Source icap.profile.name. <span class="li-normal">type: str</span>
 <a id='label58' href="javascript:ContentClick('label59', 'label58');" onmouseover="ContentPreview('label59');" onmouseout="ContentUnpreview('label59');" title="click to collapse or expand..."> more... </a>
 <div id="label59" style="display:none">
 <table border="1">
 <tr>
 <td></td>
 <td colspan="1">Supported Version Ranges</td>
 </tr>
 <tr>
 <td>icap_profile</td>
 <td><code class="docutils literal notranslate">v6.2.0 -> v6.2.7 </code></td>
 </tr>
 </table>
 </div>
 </li>
        <li> <span class="li-head">inbound</span> - Policy-based IPsec VPN: only traffic from the remote network can initiate a VPN. <span class="li-normal">type: str</span> <span class="li-normal">choices: enable, disable</span>
 <a id='label60' href="javascript:ContentClick('label61', 'label60');" onmouseover="ContentPreview('label61');" onmouseout="ContentUnpreview('label61');" title="click to collapse or expand..."> more... </a>
 <div id="label61" style="display:none">
 <table border="1">
 <tr>
 <td></td>
 <td colspan="1">Supported Version Ranges</td>
 </tr>
 <tr>
 <td>inbound</td>
 <td><code class="docutils literal notranslate">v6.2.0 -> v6.2.7 </code></td>
 </tr>
 <tr>
 <td>[enable]</td>
 <td><code class="docutils literal notranslate">v6.2.0 -> v6.2.7</code></td>
 <tr>
 <td>[disable]</td>
 <td><code class="docutils literal notranslate">v6.2.0 -> v6.2.7</code></td>
 </table>
 </div>
 </li>
        <li> <span class="li-head">inspection_mode</span> - Policy inspection mode (Flow/proxy). Default is Flow mode. <span class="li-normal">type: str</span> <span class="li-normal">choices: proxy, flow</span>
 <a id='label62' href="javascript:ContentClick('label63', 'label62');" onmouseover="ContentPreview('label63');" onmouseout="ContentUnpreview('label63');" title="click to collapse or expand..."> more... </a>
 <div id="label63" style="display:none">
 <table border="1">
 <tr>
 <td></td>
 <td colspan="1">Supported Version Ranges</td>
 </tr>
 <tr>
 <td>inspection_mode</td>
 <td><code class="docutils literal notranslate">v6.2.0 -> v6.2.7 </code></td>
 </tr>
 <tr>
 <td>[proxy]</td>
 <td><code class="docutils literal notranslate">v6.2.0 -> v6.2.7</code></td>
 <tr>
 <td>[flow]</td>
 <td><code class="docutils literal notranslate">v6.2.0 -> v6.2.7</code></td>
 </table>
 </div>
 </li>
        <li> <span class="li-head">internet_service</span> - Enable/disable use of Internet Services for this policy. If enabled, destination address and service are not used. <span class="li-normal">type: str</span> <span class="li-normal">choices: enable, disable</span>
 <a id='label64' href="javascript:ContentClick('label65', 'label64');" onmouseover="ContentPreview('label65');" onmouseout="ContentUnpreview('label65');" title="click to collapse or expand..."> more... </a>
 <div id="label65" style="display:none">
 <table border="1">
 <tr>
 <td></td>
 <td colspan="1">Supported Version Ranges</td>
 </tr>
 <tr>
 <td>internet_service</td>
 <td><code class="docutils literal notranslate">v6.2.0 -> v6.2.7 </code></td>
 </tr>
 <tr>
 <td>[enable]</td>
 <td><code class="docutils literal notranslate">v6.2.0 -> v6.2.7</code></td>
 <tr>
 <td>[disable]</td>
 <td><code class="docutils literal notranslate">v6.2.0 -> v6.2.7</code></td>
 </table>
 </div>
 </li>
        <li> <span class="li-head">internet_service_custom</span> - Custom Internet Service name. <span class="li-normal">type: list</span> <span style="font-family:'Courier New'" class="li-required">member_path: internet_service_custom:name</span>
 <a id='label66' href="javascript:ContentClick('label67', 'label66');" onmouseover="ContentPreview('label67');" onmouseout="ContentUnpreview('label67');" title="click to collapse or expand..."> more... </a>
 <div id="label67" style="display:none">
 <table border="1">
 <tr>
 <td></td><td colspan="1">Supported Version Ranges</td>
 </tr>
 <tr>
 <td>internet_service_custom</td>
 <td><code class="docutils literal notranslate">v6.2.0 -> v6.2.7 </code></td>
 </tr>
 </table>
 </div>
 </li>
            <ul class="ul-self">
            <li> <span class="li-head">name</span> - Custom Internet Service name. Source firewall.internet-service-custom.name. <span class="li-normal">type: str</span> <span class="li-required">required: true</span>
 <a id='label68' href="javascript:ContentClick('label69', 'label68');" onmouseover="ContentPreview('label69');" onmouseout="ContentUnpreview('label69');" title="click to collapse or expand..."> more... </a>
 <div id="label69" style="display:none">
 <table border="1">
 <tr>
 <td></td>
 <td colspan="1">Supported Version Ranges</td>
 </tr>
 <tr>
 <td>name</td>
 <td><code class="docutils literal notranslate">v6.2.0 -> v6.2.7 </code></td>
 </tr>
 </table>
 </div>
 </li>
            </ul>
        <li> <span class="li-head">internet_service_custom_group</span> - Custom Internet Service group name. <span class="li-normal">type: list</span> <span style="font-family:'Courier New'" class="li-required">member_path: internet_service_custom_group:name</span>
 <a id='label70' href="javascript:ContentClick('label71', 'label70');" onmouseover="ContentPreview('label71');" onmouseout="ContentUnpreview('label71');" title="click to collapse or expand..."> more... </a>
 <div id="label71" style="display:none">
 <table border="1">
 <tr>
 <td></td><td colspan="1">Supported Version Ranges</td>
 </tr>
 <tr>
 <td>internet_service_custom_group</td>
 <td><code class="docutils literal notranslate">v6.2.0 -> v6.2.7 </code></td>
 </tr>
 </table>
 </div>
 </li>
            <ul class="ul-self">
            <li> <span class="li-head">name</span> - Custom Internet Service group name. Source firewall.internet-service-custom-group.name. <span class="li-normal">type: str</span> <span class="li-required">required: true</span>
 <a id='label72' href="javascript:ContentClick('label73', 'label72');" onmouseover="ContentPreview('label73');" onmouseout="ContentUnpreview('label73');" title="click to collapse or expand..."> more... </a>
 <div id="label73" style="display:none">
 <table border="1">
 <tr>
 <td></td>
 <td colspan="1">Supported Version Ranges</td>
 </tr>
 <tr>
 <td>name</td>
 <td><code class="docutils literal notranslate">v6.2.0 -> v6.2.7 </code></td>
 </tr>
 </table>
 </div>
 </li>
            </ul>
        <li> <span class="li-head">internet_service_group</span> - Internet Service group name. <span class="li-normal">type: list</span> <span style="font-family:'Courier New'" class="li-required">member_path: internet_service_group:name</span>
 <a id='label74' href="javascript:ContentClick('label75', 'label74');" onmouseover="ContentPreview('label75');" onmouseout="ContentUnpreview('label75');" title="click to collapse or expand..."> more... </a>
 <div id="label75" style="display:none">
 <table border="1">
 <tr>
 <td></td><td colspan="1">Supported Version Ranges</td>
 </tr>
 <tr>
 <td>internet_service_group</td>
 <td><code class="docutils literal notranslate">v6.2.0 -> v6.2.7 </code></td>
 </tr>
 </table>
 </div>
 </li>
            <ul class="ul-self">
            <li> <span class="li-head">name</span> - Internet Service group name. Source firewall.internet-service-group.name. <span class="li-normal">type: str</span> <span class="li-required">required: true</span>
 <a id='label76' href="javascript:ContentClick('label77', 'label76');" onmouseover="ContentPreview('label77');" onmouseout="ContentUnpreview('label77');" title="click to collapse or expand..."> more... </a>
 <div id="label77" style="display:none">
 <table border="1">
 <tr>
 <td></td>
 <td colspan="1">Supported Version Ranges</td>
 </tr>
 <tr>
 <td>name</td>
 <td><code class="docutils literal notranslate">v6.2.0 -> v6.2.7 </code></td>
 </tr>
 </table>
 </div>
 </li>
            </ul>
        <li> <span class="li-head">internet_service_id</span> - Internet Service ID. <span class="li-normal">type: list</span> <span style="font-family:'Courier New'" class="li-required">member_path: internet_service_id:id</span>
 <a id='label78' href="javascript:ContentClick('label79', 'label78');" onmouseover="ContentPreview('label79');" onmouseout="ContentUnpreview('label79');" title="click to collapse or expand..."> more... </a>
 <div id="label79" style="display:none">
 <table border="1">
 <tr>
 <td></td><td colspan="1">Supported Version Ranges</td>
 </tr>
 <tr>
 <td>internet_service_id</td>
 <td><code class="docutils literal notranslate">v6.2.0 -> v6.2.7 </code></td>
 </tr>
 </table>
 </div>
 </li>
            <ul class="ul-self">
            <li> <span class="li-head">id</span> - Internet Service ID. see <a href='#notes'>Notes</a>. Source firewall.internet-service.id. <span class="li-normal">type: int</span> <span class="li-required">required: true</span>
 <a id='label80' href="javascript:ContentClick('label81', 'label80');" onmouseover="ContentPreview('label81');" onmouseout="ContentUnpreview('label81');" title="click to collapse or expand..."> more... </a>
 <div id="label81" style="display:none">
 <table border="1">
 <tr>
 <td></td>
 <td colspan="1">Supported Version Ranges</td>
 </tr>
 <tr>
 <td>id</td>
 <td><code class="docutils literal notranslate">v6.2.0 -> v6.2.7 </code></td>
 </tr>
 </table>
 </div>
 </li>
            </ul>
        <li> <span class="li-head">internet_service_negate</span> - When enabled internet-service specifies what the service must NOT be. <span class="li-normal">type: str</span> <span class="li-normal">choices: enable, disable</span>
 <a id='label82' href="javascript:ContentClick('label83', 'label82');" onmouseover="ContentPreview('label83');" onmouseout="ContentUnpreview('label83');" title="click to collapse or expand..."> more... </a>
 <div id="label83" style="display:none">
 <table border="1">
 <tr>
 <td></td>
 <td colspan="1">Supported Version Ranges</td>
 </tr>
 <tr>
 <td>internet_service_negate</td>
 <td><code class="docutils literal notranslate">v6.2.0 -> v6.2.7 </code></td>
 </tr>
 <tr>
 <td>[enable]</td>
 <td><code class="docutils literal notranslate">v6.2.0 -> v6.2.7</code></td>
 <tr>
 <td>[disable]</td>
 <td><code class="docutils literal notranslate">v6.2.0 -> v6.2.7</code></td>
 </table>
 </div>
 </li>
        <li> <span class="li-head">internet_service_src</span> - Enable/disable use of Internet Services in source for this policy. If enabled, source address is not used. <span class="li-normal">type: str</span> <span class="li-normal">choices: enable, disable</span>
 <a id='label84' href="javascript:ContentClick('label85', 'label84');" onmouseover="ContentPreview('label85');" onmouseout="ContentUnpreview('label85');" title="click to collapse or expand..."> more... </a>
 <div id="label85" style="display:none">
 <table border="1">
 <tr>
 <td></td>
 <td colspan="1">Supported Version Ranges</td>
 </tr>
 <tr>
 <td>internet_service_src</td>
 <td><code class="docutils literal notranslate">v6.2.0 -> v6.2.7 </code></td>
 </tr>
 <tr>
 <td>[enable]</td>
 <td><code class="docutils literal notranslate">v6.2.0 -> v6.2.7</code></td>
 <tr>
 <td>[disable]</td>
 <td><code class="docutils literal notranslate">v6.2.0 -> v6.2.7</code></td>
 </table>
 </div>
 </li>
        <li> <span class="li-head">internet_service_src_custom</span> - Custom Internet Service source name. <span class="li-normal">type: list</span> <span style="font-family:'Courier New'" class="li-required">member_path: internet_service_src_custom:name</span>
 <a id='label86' href="javascript:ContentClick('label87', 'label86');" onmouseover="ContentPreview('label87');" onmouseout="ContentUnpreview('label87');" title="click to collapse or expand..."> more... </a>
 <div id="label87" style="display:none">
 <table border="1">
 <tr>
 <td></td><td colspan="1">Supported Version Ranges</td>
 </tr>
 <tr>
 <td>internet_service_src_custom</td>
 <td><code class="docutils literal notranslate">v6.2.0 -> v6.2.7 </code></td>
 </tr>
 </table>
 </div>
 </li>
            <ul class="ul-self">
            <li> <span class="li-head">name</span> - Custom Internet Service name. Source firewall.internet-service-custom.name. <span class="li-normal">type: str</span> <span class="li-required">required: true</span>
 <a id='label88' href="javascript:ContentClick('label89', 'label88');" onmouseover="ContentPreview('label89');" onmouseout="ContentUnpreview('label89');" title="click to collapse or expand..."> more... </a>
 <div id="label89" style="display:none">
 <table border="1">
 <tr>
 <td></td>
 <td colspan="1">Supported Version Ranges</td>
 </tr>
 <tr>
 <td>name</td>
 <td><code class="docutils literal notranslate">v6.2.0 -> v6.2.7 </code></td>
 </tr>
 </table>
 </div>
 </li>
            </ul>
        <li> <span class="li-head">internet_service_src_custom_group</span> - Custom Internet Service source group name. <span class="li-normal">type: list</span> <span style="font-family:'Courier New'" class="li-required">member_path: internet_service_src_custom_group:name</span>
 <a id='label90' href="javascript:ContentClick('label91', 'label90');" onmouseover="ContentPreview('label91');" onmouseout="ContentUnpreview('label91');" title="click to collapse or expand..."> more... </a>
 <div id="label91" style="display:none">
 <table border="1">
 <tr>
 <td></td><td colspan="1">Supported Version Ranges</td>
 </tr>
 <tr>
 <td>internet_service_src_custom_group</td>
 <td><code class="docutils literal notranslate">v6.2.0 -> v6.2.7 </code></td>
 </tr>
 </table>
 </div>
 </li>
            <ul class="ul-self">
            <li> <span class="li-head">name</span> - Custom Internet Service group name. Source firewall.internet-service-custom-group.name. <span class="li-normal">type: str</span> <span class="li-required">required: true</span>
 <a id='label92' href="javascript:ContentClick('label93', 'label92');" onmouseover="ContentPreview('label93');" onmouseout="ContentUnpreview('label93');" title="click to collapse or expand..."> more... </a>
 <div id="label93" style="display:none">
 <table border="1">
 <tr>
 <td></td>
 <td colspan="1">Supported Version Ranges</td>
 </tr>
 <tr>
 <td>name</td>
 <td><code class="docutils literal notranslate">v6.2.0 -> v6.2.7 </code></td>
 </tr>
 </table>
 </div>
 </li>
            </ul>
        <li> <span class="li-head">internet_service_src_group</span> - Internet Service source group name. <span class="li-normal">type: list</span> <span style="font-family:'Courier New'" class="li-required">member_path: internet_service_src_group:name</span>
 <a id='label94' href="javascript:ContentClick('label95', 'label94');" onmouseover="ContentPreview('label95');" onmouseout="ContentUnpreview('label95');" title="click to collapse or expand..."> more... </a>
 <div id="label95" style="display:none">
 <table border="1">
 <tr>
 <td></td><td colspan="1">Supported Version Ranges</td>
 </tr>
 <tr>
 <td>internet_service_src_group</td>
 <td><code class="docutils literal notranslate">v6.2.0 -> v6.2.7 </code></td>
 </tr>
 </table>
 </div>
 </li>
            <ul class="ul-self">
            <li> <span class="li-head">name</span> - Internet Service group name. Source firewall.internet-service-group.name. <span class="li-normal">type: str</span> <span class="li-required">required: true</span>
 <a id='label96' href="javascript:ContentClick('label97', 'label96');" onmouseover="ContentPreview('label97');" onmouseout="ContentUnpreview('label97');" title="click to collapse or expand..."> more... </a>
 <div id="label97" style="display:none">
 <table border="1">
 <tr>
 <td></td>
 <td colspan="1">Supported Version Ranges</td>
 </tr>
 <tr>
 <td>name</td>
 <td><code class="docutils literal notranslate">v6.2.0 -> v6.2.7 </code></td>
 </tr>
 </table>
 </div>
 </li>
            </ul>
        <li> <span class="li-head">internet_service_src_id</span> - Internet Service source ID. <span class="li-normal">type: list</span> <span style="font-family:'Courier New'" class="li-required">member_path: internet_service_src_id:id</span>
 <a id='label98' href="javascript:ContentClick('label99', 'label98');" onmouseover="ContentPreview('label99');" onmouseout="ContentUnpreview('label99');" title="click to collapse or expand..."> more... </a>
 <div id="label99" style="display:none">
 <table border="1">
 <tr>
 <td></td><td colspan="1">Supported Version Ranges</td>
 </tr>
 <tr>
 <td>internet_service_src_id</td>
 <td><code class="docutils literal notranslate">v6.2.0 -> v6.2.7 </code></td>
 </tr>
 </table>
 </div>
 </li>
            <ul class="ul-self">
            <li> <span class="li-head">id</span> - Internet Service ID. see <a href='#notes'>Notes</a>. Source firewall.internet-service.id. <span class="li-normal">type: int</span> <span class="li-required">required: true</span>
 <a id='label100' href="javascript:ContentClick('label101', 'label100');" onmouseover="ContentPreview('label101');" onmouseout="ContentUnpreview('label101');" title="click to collapse or expand..."> more... </a>
 <div id="label101" style="display:none">
 <table border="1">
 <tr>
 <td></td>
 <td colspan="1">Supported Version Ranges</td>
 </tr>
 <tr>
 <td>id</td>
 <td><code class="docutils literal notranslate">v6.2.0 -> v6.2.7 </code></td>
 </tr>
 </table>
 </div>
 </li>
            </ul>
        <li> <span class="li-head">internet_service_src_negate</span> - When enabled internet-service-src specifies what the service must NOT be. <span class="li-normal">type: str</span> <span class="li-normal">choices: enable, disable</span>
 <a id='label102' href="javascript:ContentClick('label103', 'label102');" onmouseover="ContentPreview('label103');" onmouseout="ContentUnpreview('label103');" title="click to collapse or expand..."> more... </a>
 <div id="label103" style="display:none">
 <table border="1">
 <tr>
 <td></td>
 <td colspan="1">Supported Version Ranges</td>
 </tr>
 <tr>
 <td>internet_service_src_negate</td>
 <td><code class="docutils literal notranslate">v6.2.0 -> v6.2.7 </code></td>
 </tr>
 <tr>
 <td>[enable]</td>
 <td><code class="docutils literal notranslate">v6.2.0 -> v6.2.7</code></td>
 <tr>
 <td>[disable]</td>
 <td><code class="docutils literal notranslate">v6.2.0 -> v6.2.7</code></td>
 </table>
 </div>
 </li>
        <li> <span class="li-head">ippool</span> - Enable to use IP Pools for source NAT. <span class="li-normal">type: str</span> <span class="li-normal">choices: enable, disable</span>
 <a id='label104' href="javascript:ContentClick('label105', 'label104');" onmouseover="ContentPreview('label105');" onmouseout="ContentUnpreview('label105');" title="click to collapse or expand..."> more... </a>
 <div id="label105" style="display:none">
 <table border="1">
 <tr>
 <td></td>
 <td colspan="1">Supported Version Ranges</td>
 </tr>
 <tr>
 <td>ippool</td>
 <td><code class="docutils literal notranslate">v6.2.0 -> v6.2.7 </code></td>
 </tr>
 <tr>
 <td>[enable]</td>
 <td><code class="docutils literal notranslate">v6.2.0 -> v6.2.7</code></td>
 <tr>
 <td>[disable]</td>
 <td><code class="docutils literal notranslate">v6.2.0 -> v6.2.7</code></td>
 </table>
 </div>
 </li>
        <li> <span class="li-head">ips_sensor</span> - Name of an existing IPS sensor. Source ips.sensor.name. <span class="li-normal">type: str</span>
 <a id='label106' href="javascript:ContentClick('label107', 'label106');" onmouseover="ContentPreview('label107');" onmouseout="ContentUnpreview('label107');" title="click to collapse or expand..."> more... </a>
 <div id="label107" style="display:none">
 <table border="1">
 <tr>
 <td></td>
 <td colspan="1">Supported Version Ranges</td>
 </tr>
 <tr>
 <td>ips_sensor</td>
 <td><code class="docutils literal notranslate">v6.2.0 -> v6.2.7 </code></td>
 </tr>
 </table>
 </div>
 </li>
        <li> <span class="li-head">logtraffic</span> - Enable or disable logging. Log all sessions or security profile sessions. <span class="li-normal">type: str</span> <span class="li-normal">choices: all, utm, disable</span>
 <a id='label108' href="javascript:ContentClick('label109', 'label108');" onmouseover="ContentPreview('label109');" onmouseout="ContentUnpreview('label109');" title="click to collapse or expand..."> more... </a>
 <div id="label109" style="display:none">
 <table border="1">
 <tr>
 <td></td>
 <td colspan="1">Supported Version Ranges</td>
 </tr>
 <tr>
 <td>logtraffic</td>
 <td><code class="docutils literal notranslate">v6.2.0 -> v6.2.7 </code></td>
 </tr>
 <tr>
 <td>[all]</td>
 <td><code class="docutils literal notranslate">v6.2.0 -> v6.2.7</code></td>
 <tr>
 <td>[utm]</td>
 <td><code class="docutils literal notranslate">v6.2.0 -> v6.2.7</code></td>
 <tr>
 <td>[disable]</td>
 <td><code class="docutils literal notranslate">v6.2.0 -> v6.2.7</code></td>
 </table>
 </div>
 </li>
        <li> <span class="li-head">logtraffic_start</span> - Record logs when a session starts. <span class="li-normal">type: str</span> <span class="li-normal">choices: enable, disable</span>
 <a id='label110' href="javascript:ContentClick('label111', 'label110');" onmouseover="ContentPreview('label111');" onmouseout="ContentUnpreview('label111');" title="click to collapse or expand..."> more... </a>
 <div id="label111" style="display:none">
 <table border="1">
 <tr>
 <td></td>
 <td colspan="1">Supported Version Ranges</td>
 </tr>
 <tr>
 <td>logtraffic_start</td>
 <td><code class="docutils literal notranslate">v6.2.0 -> v6.2.7 </code></td>
 </tr>
 <tr>
 <td>[enable]</td>
 <td><code class="docutils literal notranslate">v6.2.0 -> v6.2.7</code></td>
 <tr>
 <td>[disable]</td>
 <td><code class="docutils literal notranslate">v6.2.0 -> v6.2.7</code></td>
 </table>
 </div>
 </li>
        <li> <span class="li-head">mms_profile</span> - Name of an existing MMS profile. Source firewall.mms-profile.name. <span class="li-normal">type: str</span>
 <a id='label112' href="javascript:ContentClick('label113', 'label112');" onmouseover="ContentPreview('label113');" onmouseout="ContentUnpreview('label113');" title="click to collapse or expand..."> more... </a>
 <div id="label113" style="display:none">
 <table border="1">
 <tr>
 <td></td>
 <td colspan="1">Supported Version Ranges</td>
 </tr>
 <tr>
 <td>mms_profile</td>
 <td><code class="docutils literal notranslate">v6.2.0 -> v6.2.7 </code></td>
 </tr>
 </table>
 </div>
 </li>
        <li> <span class="li-head">name</span> - Policy name. <span class="li-normal">type: str</span>
 <a id='label114' href="javascript:ContentClick('label115', 'label114');" onmouseover="ContentPreview('label115');" onmouseout="ContentUnpreview('label115');" title="click to collapse or expand..."> more... </a>
 <div id="label115" style="display:none">
 <table border="1">
 <tr>
 <td></td>
 <td colspan="1">Supported Version Ranges</td>
 </tr>
 <tr>
 <td>name</td>
 <td><code class="docutils literal notranslate">v6.2.0 -> v6.2.7 </code></td>
 </tr>
 </table>
 </div>
 </li>
        <li> <span class="li-head">nat</span> - Enable/disable source NAT. <span class="li-normal">type: str</span> <span class="li-normal">choices: enable, disable</span>
 <a id='label116' href="javascript:ContentClick('label117', 'label116');" onmouseover="ContentPreview('label117');" onmouseout="ContentUnpreview('label117');" title="click to collapse or expand..."> more... </a>
 <div id="label117" style="display:none">
 <table border="1">
 <tr>
 <td></td>
 <td colspan="1">Supported Version Ranges</td>
 </tr>
 <tr>
 <td>nat</td>
 <td><code class="docutils literal notranslate">v6.2.0 -> v6.2.7 </code></td>
 </tr>
 <tr>
 <td>[enable]</td>
 <td><code class="docutils literal notranslate">v6.2.0 -> v6.2.7</code></td>
 <tr>
 <td>[disable]</td>
 <td><code class="docutils literal notranslate">v6.2.0 -> v6.2.7</code></td>
 </table>
 </div>
 </li>
        <li> <span class="li-head">outbound</span> - Policy-based IPsec VPN: only traffic from the internal network can initiate a VPN. <span class="li-normal">type: str</span> <span class="li-normal">choices: enable, disable</span>
 <a id='label118' href="javascript:ContentClick('label119', 'label118');" onmouseover="ContentPreview('label119');" onmouseout="ContentUnpreview('label119');" title="click to collapse or expand..."> more... </a>
 <div id="label119" style="display:none">
 <table border="1">
 <tr>
 <td></td>
 <td colspan="1">Supported Version Ranges</td>
 </tr>
 <tr>
 <td>outbound</td>
 <td><code class="docutils literal notranslate">v6.2.0 -> v6.2.7 </code></td>
 </tr>
 <tr>
 <td>[enable]</td>
 <td><code class="docutils literal notranslate">v6.2.0 -> v6.2.7</code></td>
 <tr>
 <td>[disable]</td>
 <td><code class="docutils literal notranslate">v6.2.0 -> v6.2.7</code></td>
 </table>
 </div>
 </li>
        <li> <span class="li-head">per_ip_shaper</span> - Per-IP traffic shaper. Source firewall.shaper.per-ip-shaper.name. <span class="li-normal">type: str</span>
 <a id='label120' href="javascript:ContentClick('label121', 'label120');" onmouseover="ContentPreview('label121');" onmouseout="ContentUnpreview('label121');" title="click to collapse or expand..."> more... </a>
 <div id="label121" style="display:none">
 <table border="1">
 <tr>
 <td></td>
 <td colspan="1">Supported Version Ranges</td>
 </tr>
 <tr>
 <td>per_ip_shaper</td>
 <td><code class="docutils literal notranslate">v6.2.0 -> v6.2.7 </code></td>
 </tr>
 </table>
 </div>
 </li>
        <li> <span class="li-head">policyid</span> - Policy ID (0 - 4294967294). see <a href='#notes'>Notes</a>. <span class="li-normal">type: int</span> <span class="li-required">required: true</span>
 <a id='label122' href="javascript:ContentClick('label123', 'label122');" onmouseover="ContentPreview('label123');" onmouseout="ContentUnpreview('label123');" title="click to collapse or expand..."> more... </a>
 <div id="label123" style="display:none">
 <table border="1">
 <tr>
 <td></td>
 <td colspan="1">Supported Version Ranges</td>
 </tr>
 <tr>
 <td>policyid</td>
 <td><code class="docutils literal notranslate">v6.2.0 -> v6.2.7 </code></td>
 </tr>
 </table>
 </div>
 </li>
        <li> <span class="li-head">poolname4</span> - IPv4 pool names. <span class="li-normal">type: list</span> <span style="font-family:'Courier New'" class="li-required">member_path: poolname4:name</span>
 <a id='label124' href="javascript:ContentClick('label125', 'label124');" onmouseover="ContentPreview('label125');" onmouseout="ContentUnpreview('label125');" title="click to collapse or expand..."> more... </a>
 <div id="label125" style="display:none">
 <table border="1">
 <tr>
 <td></td><td colspan="1">Supported Version Ranges</td>
 </tr>
 <tr>
 <td>poolname4</td>
 <td><code class="docutils literal notranslate">v6.2.0 -> v6.2.7 </code></td>
 </tr>
 </table>
 </div>
 </li>
            <ul class="ul-self">
            <li> <span class="li-head">name</span> - IPv4 pool name. Source firewall.ippool.name. <span class="li-normal">type: str</span> <span class="li-required">required: true</span>
 <a id='label126' href="javascript:ContentClick('label127', 'label126');" onmouseover="ContentPreview('label127');" onmouseout="ContentUnpreview('label127');" title="click to collapse or expand..."> more... </a>
 <div id="label127" style="display:none">
 <table border="1">
 <tr>
 <td></td>
 <td colspan="1">Supported Version Ranges</td>
 </tr>
 <tr>
 <td>name</td>
 <td><code class="docutils literal notranslate">v6.2.0 -> v6.2.7 </code></td>
 </tr>
 </table>
 </div>
 </li>
            </ul>
        <li> <span class="li-head">poolname6</span> - IPv6 pool names. <span class="li-normal">type: list</span> <span style="font-family:'Courier New'" class="li-required">member_path: poolname6:name</span>
 <a id='label128' href="javascript:ContentClick('label129', 'label128');" onmouseover="ContentPreview('label129');" onmouseout="ContentUnpreview('label129');" title="click to collapse or expand..."> more... </a>
 <div id="label129" style="display:none">
 <table border="1">
 <tr>
 <td></td><td colspan="1">Supported Version Ranges</td>
 </tr>
 <tr>
 <td>poolname6</td>
 <td><code class="docutils literal notranslate">v6.2.0 -> v6.2.7 </code></td>
 </tr>
 </table>
 </div>
 </li>
            <ul class="ul-self">
            <li> <span class="li-head">name</span> - IPv6 pool name. Source firewall.ippool6.name. <span class="li-normal">type: str</span> <span class="li-required">required: true</span>
 <a id='label130' href="javascript:ContentClick('label131', 'label130');" onmouseover="ContentPreview('label131');" onmouseout="ContentUnpreview('label131');" title="click to collapse or expand..."> more... </a>
 <div id="label131" style="display:none">
 <table border="1">
 <tr>
 <td></td>
 <td colspan="1">Supported Version Ranges</td>
 </tr>
 <tr>
 <td>name</td>
 <td><code class="docutils literal notranslate">v6.2.0 -> v6.2.7 </code></td>
 </tr>
 </table>
 </div>
 </li>
            </ul>
        <li> <span class="li-head">profile_group</span> - Name of profile group. Source firewall.profile-group.name. <span class="li-normal">type: str</span>
 <a id='label132' href="javascript:ContentClick('label133', 'label132');" onmouseover="ContentPreview('label133');" onmouseout="ContentUnpreview('label133');" title="click to collapse or expand..."> more... </a>
 <div id="label133" style="display:none">
 <table border="1">
 <tr>
 <td></td>
 <td colspan="1">Supported Version Ranges</td>
 </tr>
 <tr>
 <td>profile_group</td>
 <td><code class="docutils literal notranslate">v6.2.0 -> v6.2.7 </code></td>
 </tr>
 </table>
 </div>
 </li>
        <li> <span class="li-head">profile_protocol_options</span> - Name of an existing Protocol options profile. Source firewall.profile-protocol-options.name. <span class="li-normal">type: str</span>
 <a id='label134' href="javascript:ContentClick('label135', 'label134');" onmouseover="ContentPreview('label135');" onmouseout="ContentUnpreview('label135');" title="click to collapse or expand..."> more... </a>
 <div id="label135" style="display:none">
 <table border="1">
 <tr>
 <td></td>
 <td colspan="1">Supported Version Ranges</td>
 </tr>
 <tr>
 <td>profile_protocol_options</td>
 <td><code class="docutils literal notranslate">v6.2.0 -> v6.2.7 </code></td>
 </tr>
 </table>
 </div>
 </li>
        <li> <span class="li-head">profile_type</span> - Determine whether the firewall policy allows security profile groups or single profiles only. <span class="li-normal">type: str</span> <span class="li-normal">choices: single, group</span>
 <a id='label136' href="javascript:ContentClick('label137', 'label136');" onmouseover="ContentPreview('label137');" onmouseout="ContentUnpreview('label137');" title="click to collapse or expand..."> more... </a>
 <div id="label137" style="display:none">
 <table border="1">
 <tr>
 <td></td>
 <td colspan="1">Supported Version Ranges</td>
 </tr>
 <tr>
 <td>profile_type</td>
 <td><code class="docutils literal notranslate">v6.2.0 -> v6.2.7 </code></td>
 </tr>
 <tr>
 <td>[single]</td>
 <td><code class="docutils literal notranslate">v6.2.0 -> v6.2.7</code></td>
 <tr>
 <td>[group]</td>
 <td><code class="docutils literal notranslate">v6.2.0 -> v6.2.7</code></td>
 </table>
 </div>
 </li>
        <li> <span class="li-head">schedule</span> - Schedule name. Source firewall.schedule.onetime.name firewall.schedule.recurring.name firewall.schedule.group.name. <span class="li-normal">type: str</span>
 <a id='label138' href="javascript:ContentClick('label139', 'label138');" onmouseover="ContentPreview('label139');" onmouseout="ContentUnpreview('label139');" title="click to collapse or expand..."> more... </a>
 <div id="label139" style="display:none">
 <table border="1">
 <tr>
 <td></td>
 <td colspan="1">Supported Version Ranges</td>
 </tr>
 <tr>
 <td>schedule</td>
 <td><code class="docutils literal notranslate">v6.2.0 -> v6.2.7 </code></td>
 </tr>
 </table>
 </div>
 </li>
        <li> <span class="li-head">service</span> - Service and service group names. <span class="li-normal">type: list</span> <span style="font-family:'Courier New'" class="li-required">member_path: service:name</span>
 <a id='label140' href="javascript:ContentClick('label141', 'label140');" onmouseover="ContentPreview('label141');" onmouseout="ContentUnpreview('label141');" title="click to collapse or expand..."> more... </a>
 <div id="label141" style="display:none">
 <table border="1">
 <tr>
 <td></td><td colspan="1">Supported Version Ranges</td>
 </tr>
 <tr>
 <td>service</td>
 <td><code class="docutils literal notranslate">v6.2.0 -> v6.2.7 </code></td>
 </tr>
 </table>
 </div>
 </li>
            <ul class="ul-self">
            <li> <span class="li-head">name</span> - Service name. Source firewall.service.custom.name firewall.service.group.name. <span class="li-normal">type: str</span> <span class="li-required">required: true</span>
 <a id='label142' href="javascript:ContentClick('label143', 'label142');" onmouseover="ContentPreview('label143');" onmouseout="ContentUnpreview('label143');" title="click to collapse or expand..."> more... </a>
 <div id="label143" style="display:none">
 <table border="1">
 <tr>
 <td></td>
 <td colspan="1">Supported Version Ranges</td>
 </tr>
 <tr>
 <td>name</td>
 <td><code class="docutils literal notranslate">v6.2.0 -> v6.2.7 </code></td>
 </tr>
 </table>
 </div>
 </li>
            </ul>
        <li> <span class="li-head">service_negate</span> - When enabled service specifies what the service must NOT be. <span class="li-normal">type: str</span> <span class="li-normal">choices: enable, disable</span>
 <a id='label144' href="javascript:ContentClick('label145', 'label144');" onmouseover="ContentPreview('label145');" onmouseout="ContentUnpreview('label145');" title="click to collapse or expand..."> more... </a>
 <div id="label145" style="display:none">
 <table border="1">
 <tr>
 <td></td>
 <td colspan="1">Supported Version Ranges</td>
 </tr>
 <tr>
 <td>service_negate</td>
 <td><code class="docutils literal notranslate">v6.2.0 -> v6.2.7 </code></td>
 </tr>
 <tr>
 <td>[enable]</td>
 <td><code class="docutils literal notranslate">v6.2.0 -> v6.2.7</code></td>
 <tr>
 <td>[disable]</td>
 <td><code class="docutils literal notranslate">v6.2.0 -> v6.2.7</code></td>
 </table>
 </div>
 </li>
        <li> <span class="li-head">session_ttl</span> - TTL in seconds for sessions accepted by this policy (0 means use the system ). <span class="li-normal">type: int</span>
 <a id='label146' href="javascript:ContentClick('label147', 'label146');" onmouseover="ContentPreview('label147');" onmouseout="ContentUnpreview('label147');" title="click to collapse or expand..."> more... </a>
 <div id="label147" style="display:none">
 <table border="1">
 <tr>
 <td></td>
 <td colspan="1">Supported Version Ranges</td>
 </tr>
 <tr>
 <td>session_ttl</td>
 <td><code class="docutils literal notranslate">v6.2.0 -> v6.2.7 </code></td>
 </tr>
 </table>
 </div>
 </li>
        <li> <span class="li-head">srcaddr_negate</span> - When enabled srcaddr specifies what the source address must NOT be. <span class="li-normal">type: str</span> <span class="li-normal">choices: enable, disable</span>
 <a id='label148' href="javascript:ContentClick('label149', 'label148');" onmouseover="ContentPreview('label149');" onmouseout="ContentUnpreview('label149');" title="click to collapse or expand..."> more... </a>
 <div id="label149" style="display:none">
 <table border="1">
 <tr>
 <td></td>
 <td colspan="1">Supported Version Ranges</td>
 </tr>
 <tr>
 <td>srcaddr_negate</td>
 <td><code class="docutils literal notranslate">v6.2.0 -> v6.2.7 </code></td>
 </tr>
 <tr>
 <td>[enable]</td>
 <td><code class="docutils literal notranslate">v6.2.0 -> v6.2.7</code></td>
 <tr>
 <td>[disable]</td>
 <td><code class="docutils literal notranslate">v6.2.0 -> v6.2.7</code></td>
 </table>
 </div>
 </li>
        <li> <span class="li-head">srcaddr4</span> - Source IPv4 address name and address group names. <span class="li-normal">type: list</span> <span style="font-family:'Courier New'" class="li-required">member_path: srcaddr4:name</span>
 <a id='label150' href="javascript:ContentClick('label151', 'label150');" onmouseover="ContentPreview('label151');" onmouseout="ContentUnpreview('label151');" title="click to collapse or expand..."> more... </a>
 <div id="label151" style="display:none">
 <table border="1">
 <tr>
 <td></td><td colspan="1">Supported Version Ranges</td>
 </tr>
 <tr>
 <td>srcaddr4</td>
 <td><code class="docutils literal notranslate">v6.2.0 -> v6.2.7 </code></td>
 </tr>
 </table>
 </div>
 </li>
            <ul class="ul-self">
            <li> <span class="li-head">name</span> - Address name. Source firewall.address.name firewall.addrgrp.name system.external-resource.name. <span class="li-normal">type: str</span> <span class="li-required">required: true</span>
 <a id='label152' href="javascript:ContentClick('label153', 'label152');" onmouseover="ContentPreview('label153');" onmouseout="ContentUnpreview('label153');" title="click to collapse or expand..."> more... </a>
 <div id="label153" style="display:none">
 <table border="1">
 <tr>
 <td></td>
 <td colspan="1">Supported Version Ranges</td>
 </tr>
 <tr>
 <td>name</td>
 <td><code class="docutils literal notranslate">v6.2.0 -> v6.2.7 </code></td>
 </tr>
 </table>
 </div>
 </li>
            </ul>
        <li> <span class="li-head">srcaddr6</span> - Source IPv6 address name and address group names. <span class="li-normal">type: list</span> <span style="font-family:'Courier New'" class="li-required">member_path: srcaddr6:name</span>
 <a id='label154' href="javascript:ContentClick('label155', 'label154');" onmouseover="ContentPreview('label155');" onmouseout="ContentUnpreview('label155');" title="click to collapse or expand..."> more... </a>
 <div id="label155" style="display:none">
 <table border="1">
 <tr>
 <td></td><td colspan="1">Supported Version Ranges</td>
 </tr>
 <tr>
 <td>srcaddr6</td>
 <td><code class="docutils literal notranslate">v6.2.0 -> v6.2.7 </code></td>
 </tr>
 </table>
 </div>
 </li>
            <ul class="ul-self">
            <li> <span class="li-head">name</span> - Address name. Source firewall.address6.name firewall.addrgrp6.name system.external-resource.name. <span class="li-normal">type: str</span> <span class="li-required">required: true</span>
 <a id='label156' href="javascript:ContentClick('label157', 'label156');" onmouseover="ContentPreview('label157');" onmouseout="ContentUnpreview('label157');" title="click to collapse or expand..."> more... </a>
 <div id="label157" style="display:none">
 <table border="1">
 <tr>
 <td></td>
 <td colspan="1">Supported Version Ranges</td>
 </tr>
 <tr>
 <td>name</td>
 <td><code class="docutils literal notranslate">v6.2.0 -> v6.2.7 </code></td>
 </tr>
 </table>
 </div>
 </li>
            </ul>
        <li> <span class="li-head">srcintf</span> - Incoming (ingress) interface. <span class="li-normal">type: list</span> <span style="font-family:'Courier New'" class="li-required">member_path: srcintf:name</span>
 <a id='label158' href="javascript:ContentClick('label159', 'label158');" onmouseover="ContentPreview('label159');" onmouseout="ContentUnpreview('label159');" title="click to collapse or expand..."> more... </a>
 <div id="label159" style="display:none">
 <table border="1">
 <tr>
 <td></td><td colspan="1">Supported Version Ranges</td>
 </tr>
 <tr>
 <td>srcintf</td>
 <td><code class="docutils literal notranslate">v6.2.0 -> v6.2.7 </code></td>
 </tr>
 </table>
 </div>
 </li>
            <ul class="ul-self">
            <li> <span class="li-head">name</span> - Interface name. Source system.interface.name system.zone.name. <span class="li-normal">type: str</span> <span class="li-required">required: true</span>
 <a id='label160' href="javascript:ContentClick('label161', 'label160');" onmouseover="ContentPreview('label161');" onmouseout="ContentUnpreview('label161');" title="click to collapse or expand..."> more... </a>
 <div id="label161" style="display:none">
 <table border="1">
 <tr>
 <td></td>
 <td colspan="1">Supported Version Ranges</td>
 </tr>
 <tr>
 <td>name</td>
 <td><code class="docutils literal notranslate">v6.2.0 -> v6.2.7 </code></td>
 </tr>
 </table>
 </div>
 </li>
            </ul>
        <li> <span class="li-head">ssh_filter_profile</span> - Name of an existing SSH filter profile. Source ssh-filter.profile.name. <span class="li-normal">type: str</span>
 <a id='label162' href="javascript:ContentClick('label163', 'label162');" onmouseover="ContentPreview('label163');" onmouseout="ContentUnpreview('label163');" title="click to collapse or expand..."> more... </a>
 <div id="label163" style="display:none">
 <table border="1">
 <tr>
 <td></td>
 <td colspan="1">Supported Version Ranges</td>
 </tr>
 <tr>
 <td>ssh_filter_profile</td>
 <td><code class="docutils literal notranslate">v6.2.0 -> v6.2.7 </code></td>
 </tr>
 </table>
 </div>
 </li>
        <li> <span class="li-head">ssh_policy_redirect</span> - Redirect SSH traffic to matching transparent proxy policy. <span class="li-normal">type: str</span> <span class="li-normal">choices: enable, disable</span>
 <a id='label164' href="javascript:ContentClick('label165', 'label164');" onmouseover="ContentPreview('label165');" onmouseout="ContentUnpreview('label165');" title="click to collapse or expand..."> more... </a>
 <div id="label165" style="display:none">
 <table border="1">
 <tr>
 <td></td>
 <td colspan="1">Supported Version Ranges</td>
 </tr>
 <tr>
 <td>ssh_policy_redirect</td>
 <td><code class="docutils literal notranslate">v6.2.0 -> v6.2.7 </code></td>
 </tr>
 <tr>
 <td>[enable]</td>
 <td><code class="docutils literal notranslate">v6.2.0 -> v6.2.7</code></td>
 <tr>
 <td>[disable]</td>
 <td><code class="docutils literal notranslate">v6.2.0 -> v6.2.7</code></td>
 </table>
 </div>
 </li>
        <li> <span class="li-head">ssl_ssh_profile</span> - Name of an existing SSL SSH profile. Source firewall.ssl-ssh-profile.name. <span class="li-normal">type: str</span>
 <a id='label166' href="javascript:ContentClick('label167', 'label166');" onmouseover="ContentPreview('label167');" onmouseout="ContentUnpreview('label167');" title="click to collapse or expand..."> more... </a>
 <div id="label167" style="display:none">
 <table border="1">
 <tr>
 <td></td>
 <td colspan="1">Supported Version Ranges</td>
 </tr>
 <tr>
 <td>ssl_ssh_profile</td>
 <td><code class="docutils literal notranslate">v6.2.0 -> v6.2.7 </code></td>
 </tr>
 </table>
 </div>
 </li>
        <li> <span class="li-head">status</span> - Enable or disable this policy. <span class="li-normal">type: str</span> <span class="li-normal">choices: enable, disable</span>
 <a id='label168' href="javascript:ContentClick('label169', 'label168');" onmouseover="ContentPreview('label169');" onmouseout="ContentUnpreview('label169');" title="click to collapse or expand..."> more... </a>
 <div id="label169" style="display:none">
 <table border="1">
 <tr>
 <td></td>
 <td colspan="1">Supported Version Ranges</td>
 </tr>
 <tr>
 <td>status</td>
 <td><code class="docutils literal notranslate">v6.2.0 -> v6.2.7 </code></td>
 </tr>
 <tr>
 <td>[enable]</td>
 <td><code class="docutils literal notranslate">v6.2.0 -> v6.2.7</code></td>
 <tr>
 <td>[disable]</td>
 <td><code class="docutils literal notranslate">v6.2.0 -> v6.2.7</code></td>
 </table>
 </div>
 </li>
        <li> <span class="li-head">tcp_mss_receiver</span> - Receiver TCP maximum segment size (MSS). <span class="li-normal">type: int</span>
 <a id='label170' href="javascript:ContentClick('label171', 'label170');" onmouseover="ContentPreview('label171');" onmouseout="ContentUnpreview('label171');" title="click to collapse or expand..."> more... </a>
 <div id="label171" style="display:none">
 <table border="1">
 <tr>
 <td></td>
 <td colspan="1">Supported Version Ranges</td>
 </tr>
 <tr>
 <td>tcp_mss_receiver</td>
 <td><code class="docutils literal notranslate">v6.2.0 -> v6.2.7 </code></td>
 </tr>
 </table>
 </div>
 </li>
        <li> <span class="li-head">tcp_mss_sender</span> - Sender TCP maximum segment size (MSS). <span class="li-normal">type: int</span>
 <a id='label172' href="javascript:ContentClick('label173', 'label172');" onmouseover="ContentPreview('label173');" onmouseout="ContentUnpreview('label173');" title="click to collapse or expand..."> more... </a>
 <div id="label173" style="display:none">
 <table border="1">
 <tr>
 <td></td>
 <td colspan="1">Supported Version Ranges</td>
 </tr>
 <tr>
 <td>tcp_mss_sender</td>
 <td><code class="docutils literal notranslate">v6.2.0 -> v6.2.7 </code></td>
 </tr>
 </table>
 </div>
 </li>
        <li> <span class="li-head">traffic_shaper</span> - Traffic shaper. Source firewall.shaper.traffic-shaper.name. <span class="li-normal">type: str</span>
 <a id='label174' href="javascript:ContentClick('label175', 'label174');" onmouseover="ContentPreview('label175');" onmouseout="ContentUnpreview('label175');" title="click to collapse or expand..."> more... </a>
 <div id="label175" style="display:none">
 <table border="1">
 <tr>
 <td></td>
 <td colspan="1">Supported Version Ranges</td>
 </tr>
 <tr>
 <td>traffic_shaper</td>
 <td><code class="docutils literal notranslate">v6.2.0 -> v6.2.7 </code></td>
 </tr>
 </table>
 </div>
 </li>
        <li> <span class="li-head">traffic_shaper_reverse</span> - Reverse traffic shaper. Source firewall.shaper.traffic-shaper.name. <span class="li-normal">type: str</span>
 <a id='label176' href="javascript:ContentClick('label177', 'label176');" onmouseover="ContentPreview('label177');" onmouseout="ContentUnpreview('label177');" title="click to collapse or expand..."> more... </a>
 <div id="label177" style="display:none">
 <table border="1">
 <tr>
 <td></td>
 <td colspan="1">Supported Version Ranges</td>
 </tr>
 <tr>
 <td>traffic_shaper_reverse</td>
 <td><code class="docutils literal notranslate">v6.2.0 -> v6.2.7 </code></td>
 </tr>
 </table>
 </div>
 </li>
        <li> <span class="li-head">users</span> - Names of individual users that can authenticate with this policy. <span class="li-normal">type: list</span> <span style="font-family:'Courier New'" class="li-required">member_path: users:name</span>
 <a id='label178' href="javascript:ContentClick('label179', 'label178');" onmouseover="ContentPreview('label179');" onmouseout="ContentUnpreview('label179');" title="click to collapse or expand..."> more... </a>
 <div id="label179" style="display:none">
 <table border="1">
 <tr>
 <td></td><td colspan="1">Supported Version Ranges</td>
 </tr>
 <tr>
 <td>users</td>
 <td><code class="docutils literal notranslate">v6.2.0 -> v6.2.7 </code></td>
 </tr>
 </table>
 </div>
 </li>
            <ul class="ul-self">
            <li> <span class="li-head">name</span> - User name. Source user.local.name. <span class="li-normal">type: str</span> <span class="li-required">required: true</span>
 <a id='label180' href="javascript:ContentClick('label181', 'label180');" onmouseover="ContentPreview('label181');" onmouseout="ContentUnpreview('label181');" title="click to collapse or expand..."> more... </a>
 <div id="label181" style="display:none">
 <table border="1">
 <tr>
 <td></td>
 <td colspan="1">Supported Version Ranges</td>
 </tr>
 <tr>
 <td>name</td>
 <td><code class="docutils literal notranslate">v6.2.0 -> v6.2.7 </code></td>
 </tr>
 </table>
 </div>
 </li>
            </ul>
        <li> <span class="li-head">utm_status</span> - Enable to add one or more security profiles (AV, IPS, etc.) to the firewall policy. <span class="li-normal">type: str</span> <span class="li-normal">choices: enable, disable</span>
 <a id='label182' href="javascript:ContentClick('label183', 'label182');" onmouseover="ContentPreview('label183');" onmouseout="ContentUnpreview('label183');" title="click to collapse or expand..."> more... </a>
 <div id="label183" style="display:none">
 <table border="1">
 <tr>
 <td></td>
 <td colspan="1">Supported Version Ranges</td>
 </tr>
 <tr>
 <td>utm_status</td>
 <td><code class="docutils literal notranslate">v6.2.0 -> v6.2.7 </code></td>
 </tr>
 <tr>
 <td>[enable]</td>
 <td><code class="docutils literal notranslate">v6.2.0 -> v6.2.7</code></td>
 <tr>
 <td>[disable]</td>
 <td><code class="docutils literal notranslate">v6.2.0 -> v6.2.7</code></td>
 </table>
 </div>
 </li>
        <li> <span class="li-head">uuid</span> - Universally Unique Identifier (UUID; automatically assigned but can be manually reset). <span class="li-normal">type: str</span>
 <a id='label184' href="javascript:ContentClick('label185', 'label184');" onmouseover="ContentPreview('label185');" onmouseout="ContentUnpreview('label185');" title="click to collapse or expand..."> more... </a>
 <div id="label185" style="display:none">
 <table border="1">
 <tr>
 <td></td>
 <td colspan="1">Supported Version Ranges</td>
 </tr>
 <tr>
 <td>uuid</td>
 <td><code class="docutils literal notranslate">v6.2.0 -> v6.2.7 </code></td>
 </tr>
 </table>
 </div>
 </li>
        <li> <span class="li-head">voip_profile</span> - Name of an existing VoIP profile. Source voip.profile.name. <span class="li-normal">type: str</span>
 <a id='label186' href="javascript:ContentClick('label187', 'label186');" onmouseover="ContentPreview('label187');" onmouseout="ContentUnpreview('label187');" title="click to collapse or expand..."> more... </a>
 <div id="label187" style="display:none">
 <table border="1">
 <tr>
 <td></td>
 <td colspan="1">Supported Version Ranges</td>
 </tr>
 <tr>
 <td>voip_profile</td>
 <td><code class="docutils literal notranslate">v6.2.0 -> v6.2.7 </code></td>
 </tr>
 </table>
 </div>
 </li>
        <li> <span class="li-head">vpntunnel</span> - Policy-based IPsec VPN: name of the IPsec VPN Phase 1. Source vpn.ipsec.phase1.name vpn.ipsec.manualkey.name. <span class="li-normal">type: str</span>
 <a id='label188' href="javascript:ContentClick('label189', 'label188');" onmouseover="ContentPreview('label189');" onmouseout="ContentUnpreview('label189');" title="click to collapse or expand..."> more... </a>
 <div id="label189" style="display:none">
 <table border="1">
 <tr>
 <td></td>
 <td colspan="1">Supported Version Ranges</td>
 </tr>
 <tr>
 <td>vpntunnel</td>
 <td><code class="docutils literal notranslate">v6.2.0 -> v6.2.7 </code></td>
 </tr>
 </table>
 </div>
 </li>
        <li> <span class="li-head">waf_profile</span> - Name of an existing Web application firewall profile. Source waf.profile.name. <span class="li-normal">type: str</span>
 <a id='label190' href="javascript:ContentClick('label191', 'label190');" onmouseover="ContentPreview('label191');" onmouseout="ContentUnpreview('label191');" title="click to collapse or expand..."> more... </a>
 <div id="label191" style="display:none">
 <table border="1">
 <tr>
 <td></td>
 <td colspan="1">Supported Version Ranges</td>
 </tr>
 <tr>
 <td>waf_profile</td>
 <td><code class="docutils literal notranslate">v6.2.0 -> v6.2.7 </code></td>
 </tr>
 </table>
 </div>
 </li>
        <li> <span class="li-head">wanopt</span> - Enable/disable WAN optimization. <span class="li-normal">type: str</span> <span class="li-normal">choices: enable, disable</span>
 <a id='label192' href="javascript:ContentClick('label193', 'label192');" onmouseover="ContentPreview('label193');" onmouseout="ContentUnpreview('label193');" title="click to collapse or expand..."> more... </a>
 <div id="label193" style="display:none">
 <table border="1">
 <tr>
 <td></td>
 <td colspan="1">Supported Version Ranges</td>
 </tr>
 <tr>
 <td>wanopt</td>
 <td><code class="docutils literal notranslate">v6.2.0 -> v6.2.7 </code></td>
 </tr>
 <tr>
 <td>[enable]</td>
 <td><code class="docutils literal notranslate">v6.2.0 -> v6.2.7</code></td>
 <tr>
 <td>[disable]</td>
 <td><code class="docutils literal notranslate">v6.2.0 -> v6.2.7</code></td>
 </table>
 </div>
 </li>
        <li> <span class="li-head">wanopt_detection</span> - WAN optimization auto-detection mode. <span class="li-normal">type: str</span> <span class="li-normal">choices: active, passive, off</span>
 <a id='label194' href="javascript:ContentClick('label195', 'label194');" onmouseover="ContentPreview('label195');" onmouseout="ContentUnpreview('label195');" title="click to collapse or expand..."> more... </a>
 <div id="label195" style="display:none">
 <table border="1">
 <tr>
 <td></td>
 <td colspan="1">Supported Version Ranges</td>
 </tr>
 <tr>
 <td>wanopt_detection</td>
 <td><code class="docutils literal notranslate">v6.2.0 -> v6.2.7 </code></td>
 </tr>
 <tr>
 <td>[active]</td>
 <td><code class="docutils literal notranslate">v6.2.0 -> v6.2.7</code></td>
 <tr>
 <td>[passive]</td>
 <td><code class="docutils literal notranslate">v6.2.0 -> v6.2.7</code></td>
 <tr>
 <td>[off]</td>
 <td><code class="docutils literal notranslate">v6.2.0 -> v6.2.7</code></td>
 </table>
 </div>
 </li>
        <li> <span class="li-head">wanopt_passive_opt</span> - WAN optimization passive mode options. This option decides what IP address will be used to connect to server. <span class="li-normal">type: str</span> <span class="li-normal">choices: default, transparent, non-transparent</span>
 <a id='label196' href="javascript:ContentClick('label197', 'label196');" onmouseover="ContentPreview('label197');" onmouseout="ContentUnpreview('label197');" title="click to collapse or expand..."> more... </a>
 <div id="label197" style="display:none">
 <table border="1">
 <tr>
 <td></td>
 <td colspan="1">Supported Version Ranges</td>
 </tr>
 <tr>
 <td>wanopt_passive_opt</td>
 <td><code class="docutils literal notranslate">v6.2.0 -> v6.2.7 </code></td>
 </tr>
 <tr>
 <td>[default]</td>
 <td><code class="docutils literal notranslate">v6.2.0 -> v6.2.7</code></td>
 <tr>
 <td>[transparent]</td>
 <td><code class="docutils literal notranslate">v6.2.0 -> v6.2.7</code></td>
 <tr>
 <td>[non-transparent]</td>
 <td><code class="docutils literal notranslate">v6.2.0 -> v6.2.7</code></td>
 </table>
 </div>
 </li>
        <li> <span class="li-head">wanopt_peer</span> - WAN optimization peer. Source wanopt.peer.peer-host-id. <span class="li-normal">type: str</span>
 <a id='label198' href="javascript:ContentClick('label199', 'label198');" onmouseover="ContentPreview('label199');" onmouseout="ContentUnpreview('label199');" title="click to collapse or expand..."> more... </a>
 <div id="label199" style="display:none">
 <table border="1">
 <tr>
 <td></td>
 <td colspan="1">Supported Version Ranges</td>
 </tr>
 <tr>
 <td>wanopt_peer</td>
 <td><code class="docutils literal notranslate">v6.2.0 -> v6.2.7 </code></td>
 </tr>
 </table>
 </div>
 </li>
        <li> <span class="li-head">wanopt_profile</span> - WAN optimization profile. Source wanopt.profile.name. <span class="li-normal">type: str</span>
 <a id='label200' href="javascript:ContentClick('label201', 'label200');" onmouseover="ContentPreview('label201');" onmouseout="ContentUnpreview('label201');" title="click to collapse or expand..."> more... </a>
 <div id="label201" style="display:none">
 <table border="1">
 <tr>
 <td></td>
 <td colspan="1">Supported Version Ranges</td>
 </tr>
 <tr>
 <td>wanopt_profile</td>
 <td><code class="docutils literal notranslate">v6.2.0 -> v6.2.7 </code></td>
 </tr>
 </table>
 </div>
 </li>
        <li> <span class="li-head">webcache</span> - Enable/disable web cache. <span class="li-normal">type: str</span> <span class="li-normal">choices: enable, disable</span>
 <a id='label202' href="javascript:ContentClick('label203', 'label202');" onmouseover="ContentPreview('label203');" onmouseout="ContentUnpreview('label203');" title="click to collapse or expand..."> more... </a>
 <div id="label203" style="display:none">
 <table border="1">
 <tr>
 <td></td>
 <td colspan="1">Supported Version Ranges</td>
 </tr>
 <tr>
 <td>webcache</td>
 <td><code class="docutils literal notranslate">v6.2.0 -> v6.2.7 </code></td>
 </tr>
 <tr>
 <td>[enable]</td>
 <td><code class="docutils literal notranslate">v6.2.0 -> v6.2.7</code></td>
 <tr>
 <td>[disable]</td>
 <td><code class="docutils literal notranslate">v6.2.0 -> v6.2.7</code></td>
 </table>
 </div>
 </li>
        <li> <span class="li-head">webcache_https</span> - Enable/disable web cache for HTTPS. <span class="li-normal">type: str</span> <span class="li-normal">choices: disable, enable</span>
 <a id='label204' href="javascript:ContentClick('label205', 'label204');" onmouseover="ContentPreview('label205');" onmouseout="ContentUnpreview('label205');" title="click to collapse or expand..."> more... </a>
 <div id="label205" style="display:none">
 <table border="1">
 <tr>
 <td></td>
 <td colspan="1">Supported Version Ranges</td>
 </tr>
 <tr>
 <td>webcache_https</td>
 <td><code class="docutils literal notranslate">v6.2.0 -> v6.2.7 </code></td>
 </tr>
 <tr>
 <td>[disable]</td>
 <td><code class="docutils literal notranslate">v6.2.0 -> v6.2.7</code></td>
 <tr>
 <td>[enable]</td>
 <td><code class="docutils literal notranslate">v6.2.0 -> v6.2.7</code></td>
 </table>
 </div>
 </li>
        <li> <span class="li-head">webfilter_profile</span> - Name of an existing Web filter profile. Source webfilter.profile.name. <span class="li-normal">type: str</span>
 <a id='label206' href="javascript:ContentClick('label207', 'label206');" onmouseover="ContentPreview('label207');" onmouseout="ContentUnpreview('label207');" title="click to collapse or expand..."> more... </a>
 <div id="label207" style="display:none">
 <table border="1">
 <tr>
 <td></td>
 <td colspan="1">Supported Version Ranges</td>
 </tr>
 <tr>
 <td>webfilter_profile</td>
 <td><code class="docutils literal notranslate">v6.2.0 -> v6.2.7 </code></td>
 </tr>
 </table>
 </div>
 </li>
        <li> <span class="li-head">webproxy_forward_server</span> - Webproxy forward server name. Source web-proxy.forward-server.name web-proxy.forward-server-group.name. <span class="li-normal">type: str</span>
 <a id='label208' href="javascript:ContentClick('label209', 'label208');" onmouseover="ContentPreview('label209');" onmouseout="ContentUnpreview('label209');" title="click to collapse or expand..."> more... </a>
 <div id="label209" style="display:none">
 <table border="1">
 <tr>
 <td></td>
 <td colspan="1">Supported Version Ranges</td>
 </tr>
 <tr>
 <td>webproxy_forward_server</td>
 <td><code class="docutils literal notranslate">v6.2.0 -> v6.2.7 </code></td>
 </tr>
 </table>
 </div>
 </li>
        <li> <span class="li-head">webproxy_profile</span> - Webproxy profile name. Source web-proxy.profile.name. <span class="li-normal">type: str</span>
 <a id='label210' href="javascript:ContentClick('label211', 'label210');" onmouseover="ContentPreview('label211');" onmouseout="ContentUnpreview('label211');" title="click to collapse or expand..."> more... </a>
 <div id="label211" style="display:none">
 <table border="1">
 <tr>
 <td></td>
 <td colspan="1">Supported Version Ranges</td>
 </tr>
 <tr>
 <td>webproxy_profile</td>
 <td><code class="docutils literal notranslate">v6.2.0 -> v6.2.7 </code></td>
 </tr>
 </table>
 </div>
 </li>
        </ul>
    </ul>


Notes
-----

.. note::

   - We highly recommend using your own value as the policyid instead of 0, while '0' is a special placeholder that allows the backend to assign the latest available number for the object, it does have limitations. Please find more details in Q&A.

   - Legacy fortiosapi has been deprecated, httpapi is the preferred way to run playbooks

   - The module supports check_mode.



Examples
--------

.. code-block:: yaml+jinja
    
    - name: Configure consolidated IPv4/IPv6 policies.
      fortinet.fortios.fortios_firewall_consolidated_policy:
          vdom: "{{ vdom }}"
          state: "present"
          access_token: "<your_own_value>"
          firewall_consolidated_policy:
              action: "accept"
              application_list: "<your_own_value> (source application.list.name)"
              auto_asic_offload: "enable"
              av_profile: "<your_own_value> (source antivirus.profile.name)"
              captive_portal_exempt: "enable"
              cifs_profile: "<your_own_value> (source cifs.profile.name)"
              comments: "<your_own_value>"
              diffserv_forward: "enable"
              diffserv_reverse: "enable"
              diffservcode_forward: "<your_own_value>"
              diffservcode_rev: "<your_own_value>"
              dlp_sensor: "<your_own_value> (source dlp.sensor.name)"
              dnsfilter_profile: "<your_own_value> (source dnsfilter.profile.name)"
              dstaddr_negate: "enable"
              dstaddr4:
                  -
                      name: "default_name_18 (source firewall.address.name firewall.addrgrp.name firewall.vip.name firewall.vipgrp.name system.external-resource
                        .name)"
              dstaddr6:
                  -
                      name: "default_name_20 (source firewall.address6.name firewall.addrgrp6.name firewall.vip6.name firewall.vipgrp6.name system
                        .external-resource.name)"
              dstintf:
                  -
                      name: "default_name_22 (source system.interface.name system.zone.name)"
              emailfilter_profile: "<your_own_value> (source emailfilter.profile.name)"
              fixedport: "enable"
              fsso_groups:
                  -
                      name: "default_name_26 (source user.adgrp.name)"
              global_label: "<your_own_value>"
              groups:
                  -
                      name: "default_name_29 (source user.group.name)"
              http_policy_redirect: "enable"
              icap_profile: "<your_own_value> (source icap.profile.name)"
              inbound: "enable"
              inspection_mode: "proxy"
              internet_service: "enable"
              internet_service_custom:
                  -
                      name: "default_name_36 (source firewall.internet-service-custom.name)"
              internet_service_custom_group:
                  -
                      name: "default_name_38 (source firewall.internet-service-custom-group.name)"
              internet_service_group:
                  -
                      name: "default_name_40 (source firewall.internet-service-group.name)"
              internet_service_id:
                  -
                      id: "42 (source firewall.internet-service.id)"
              internet_service_negate: "enable"
              internet_service_src: "enable"
              internet_service_src_custom:
                  -
                      name: "default_name_46 (source firewall.internet-service-custom.name)"
              internet_service_src_custom_group:
                  -
                      name: "default_name_48 (source firewall.internet-service-custom-group.name)"
              internet_service_src_group:
                  -
                      name: "default_name_50 (source firewall.internet-service-group.name)"
              internet_service_src_id:
                  -
                      id: "52 (source firewall.internet-service.id)"
              internet_service_src_negate: "enable"
              ippool: "enable"
              ips_sensor: "<your_own_value> (source ips.sensor.name)"
              logtraffic: "all"
              logtraffic_start: "enable"
              mms_profile: "<your_own_value> (source firewall.mms-profile.name)"
              name: "default_name_59"
              nat: "enable"
              outbound: "enable"
              per_ip_shaper: "<your_own_value> (source firewall.shaper.per-ip-shaper.name)"
              policyid: "<you_own_value>"
              poolname4:
                  -
                      name: "default_name_65 (source firewall.ippool.name)"
              poolname6:
                  -
                      name: "default_name_67 (source firewall.ippool6.name)"
              profile_group: "<your_own_value> (source firewall.profile-group.name)"
              profile_protocol_options: "<your_own_value> (source firewall.profile-protocol-options.name)"
              profile_type: "single"
              schedule: "<your_own_value> (source firewall.schedule.onetime.name firewall.schedule.recurring.name firewall.schedule.group.name)"
              service:
                  -
                      name: "default_name_73 (source firewall.service.custom.name firewall.service.group.name)"
              service_negate: "enable"
              session_ttl: "1382400"
              srcaddr_negate: "enable"
              srcaddr4:
                  -
                      name: "default_name_78 (source firewall.address.name firewall.addrgrp.name system.external-resource.name)"
              srcaddr6:
                  -
                      name: "default_name_80 (source firewall.address6.name firewall.addrgrp6.name system.external-resource.name)"
              srcintf:
                  -
                      name: "default_name_82 (source system.interface.name system.zone.name)"
              ssh_filter_profile: "<your_own_value> (source ssh-filter.profile.name)"
              ssh_policy_redirect: "enable"
              ssl_ssh_profile: "<your_own_value> (source firewall.ssl-ssh-profile.name)"
              status: "enable"
              tcp_mss_receiver: "32767"
              tcp_mss_sender: "32767"
              traffic_shaper: "<your_own_value> (source firewall.shaper.traffic-shaper.name)"
              traffic_shaper_reverse: "<your_own_value> (source firewall.shaper.traffic-shaper.name)"
              users:
                  -
                      name: "default_name_92 (source user.local.name)"
              utm_status: "enable"
              uuid: "<your_own_value>"
              voip_profile: "<your_own_value> (source voip.profile.name)"
              vpntunnel: "<your_own_value> (source vpn.ipsec.phase1.name vpn.ipsec.manualkey.name)"
              waf_profile: "<your_own_value> (source waf.profile.name)"
              wanopt: "enable"
              wanopt_detection: "active"
              wanopt_passive_opt: "default"
              wanopt_peer: "<your_own_value> (source wanopt.peer.peer-host-id)"
              wanopt_profile: "<your_own_value> (source wanopt.profile.name)"
              webcache: "enable"
              webcache_https: "disable"
              webfilter_profile: "<your_own_value> (source webfilter.profile.name)"
              webproxy_forward_server: "<your_own_value> (source web-proxy.forward-server.name web-proxy.forward-server-group.name)"
              webproxy_profile: "<your_own_value> (source web-proxy.profile.name)"


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
