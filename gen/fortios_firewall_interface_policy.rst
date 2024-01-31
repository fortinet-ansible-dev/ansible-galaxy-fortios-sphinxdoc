:source: fortios_firewall_interface_policy.py

:orphan:

.. fortios_firewall_interface_policy:

fortios_firewall_interface_policy -- Configure IPv4 interface policies in Fortinet's FortiOS and FortiGate.
+++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++

.. versionadded:: 2.0.0

.. contents::
   :local:
   :depth: 1


Synopsis
--------
- This module is able to configure a FortiGate or FortiOS (FOS) device by allowing the user to set and modify firewall feature and interface_policy category. Examples include all parameters and values need to be adjusted to datasources before usage. Tested with FOS v6.0.0



Requirements
------------
The below requirements are needed on the host that executes this module.

- ansible>=2.14


Tips
----
Using member operation to add an element to an existing object.

FortiOS Version Compatibility
-----------------------------


.. raw:: html

 <br>
 <table border="1">
 <tr>
 <td></td><td colspan="1">Supported Version Ranges</td>
 </tr>
 <tr>
 <td>fortios_firewall_interface_policy</td>
 <td><code class="docutils literal notranslate">v6.0.0 -> latest </code></td>
 </tr>
 </table>
 <p>



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
    <li> <span class="li-head">firewall_interface_policy</span> - Configure IPv4 interface policies. <span class="li-normal">type: dict</span>
 <a id='label0' href="javascript:ContentClick('label1', 'label0');" onmouseover="ContentPreview('label1');" onmouseout="ContentUnpreview('label1');" title="click to collapse or expand..."> more... </a>
 <div id="label1" style="display:none">
 <table border="1">
 <tr>
 <td></td><td colspan="1">Supported Version Ranges</td>
 </tr>
 <tr>
 <td>firewall_interface_policy</td>
 <td><code class="docutils literal notranslate">v6.0.0 -> latest </code></td>
 </tr>
 </table>
 </div>
 </li>
        <ul class="ul-self">
        <li> <span class="li-head">address_type</span> - Policy address type (IPv4 or IPv6). <span class="li-normal">type: str</span> <span class="li-normal">choices: ipv4, ipv6</span>
 <a id='label2' href="javascript:ContentClick('label3', 'label2');" onmouseover="ContentPreview('label3');" onmouseout="ContentUnpreview('label3');" title="click to collapse or expand..."> more... </a>
 <div id="label3" style="display:none">
 <table border="1">
 <tr>
 <td></td>
 <td colspan="2">Supported Version Ranges</td>
 </tr>
 <tr>
 <td>address_type</td>
 <td><code class="docutils literal notranslate">v6.0.0 -> v6.0.11 </code></td>
 <td><code class="docutils literal notranslate">v6.2.3 -> v6.2.3 </code></td>
 </tr>
 <tr>
 <td>[ipv4]</td>
 <td><code class="docutils literal notranslate">v6.0.0 -> latest</code></td> <tr>
 <td>[ipv6]</td>
 <td><code class="docutils literal notranslate">v6.0.0 -> latest</code></td> </table>
 </div>
 </li>
        <li> <span class="li-head">application_list</span> - Application list name. Source application.list.name. <span class="li-normal">type: str</span>
 <a id='label4' href="javascript:ContentClick('label5', 'label4');" onmouseover="ContentPreview('label5');" onmouseout="ContentUnpreview('label5');" title="click to collapse or expand..."> more... </a>
 <div id="label5" style="display:none">
 <table border="1">
 <tr>
 <td></td>
 <td colspan="1">Supported Version Ranges</td>
 </tr>
 <tr>
 <td>application_list</td>
 <td><code class="docutils literal notranslate">v6.0.0 -> latest </code></td>
 </tr>
 </table>
 </div>
 </li>
        <li> <span class="li-head">application_list_status</span> - Enable/disable application control. <span class="li-normal">type: str</span> <span class="li-normal">choices: enable, disable</span>
 <a id='label6' href="javascript:ContentClick('label7', 'label6');" onmouseover="ContentPreview('label7');" onmouseout="ContentUnpreview('label7');" title="click to collapse or expand..."> more... </a>
 <div id="label7" style="display:none">
 <table border="1">
 <tr>
 <td></td>
 <td colspan="1">Supported Version Ranges</td>
 </tr>
 <tr>
 <td>application_list_status</td>
 <td><code class="docutils literal notranslate">v6.0.0 -> latest </code></td>
 </tr>
 <tr>
 <td>[enable]</td>
 <td><code class="docutils literal notranslate">v6.0.0 -> latest</code></td> <tr>
 <td>[disable]</td>
 <td><code class="docutils literal notranslate">v6.0.0 -> latest</code></td> </table>
 </div>
 </li>
        <li> <span class="li-head">av_profile</span> - Antivirus profile. Source antivirus.profile.name. <span class="li-normal">type: str</span>
 <a id='label8' href="javascript:ContentClick('label9', 'label8');" onmouseover="ContentPreview('label9');" onmouseout="ContentUnpreview('label9');" title="click to collapse or expand..."> more... </a>
 <div id="label9" style="display:none">
 <table border="1">
 <tr>
 <td></td>
 <td colspan="1">Supported Version Ranges</td>
 </tr>
 <tr>
 <td>av_profile</td>
 <td><code class="docutils literal notranslate">v6.0.0 -> latest </code></td>
 </tr>
 </table>
 </div>
 </li>
        <li> <span class="li-head">av_profile_status</span> - Enable/disable antivirus. <span class="li-normal">type: str</span> <span class="li-normal">choices: enable, disable</span>
 <a id='label10' href="javascript:ContentClick('label11', 'label10');" onmouseover="ContentPreview('label11');" onmouseout="ContentUnpreview('label11');" title="click to collapse or expand..."> more... </a>
 <div id="label11" style="display:none">
 <table border="1">
 <tr>
 <td></td>
 <td colspan="1">Supported Version Ranges</td>
 </tr>
 <tr>
 <td>av_profile_status</td>
 <td><code class="docutils literal notranslate">v6.0.0 -> latest </code></td>
 </tr>
 <tr>
 <td>[enable]</td>
 <td><code class="docutils literal notranslate">v6.0.0 -> latest</code></td> <tr>
 <td>[disable]</td>
 <td><code class="docutils literal notranslate">v6.0.0 -> latest</code></td> </table>
 </div>
 </li>
        <li> <span class="li-head">casb_profile</span> - CASB profile. Source casb.profile.name. <span class="li-normal">type: str</span>
 <a id='label12' href="javascript:ContentClick('label13', 'label12');" onmouseover="ContentPreview('label13');" onmouseout="ContentUnpreview('label13');" title="click to collapse or expand..."> more... </a>
 <div id="label13" style="display:none">
 <table border="1">
 <tr>
 <td></td>
 <td colspan="1">Supported Version Ranges</td>
 </tr>
 <tr>
 <td>casb_profile</td>
 <td><code class="docutils literal notranslate">v7.4.1 -> latest </code></td>
 </tr>
 </table>
 </div>
 </li>
        <li> <span class="li-head">casb_profile_status</span> - Enable/disable CASB. <span class="li-normal">type: str</span> <span class="li-normal">choices: enable, disable</span>
 <a id='label14' href="javascript:ContentClick('label15', 'label14');" onmouseover="ContentPreview('label15');" onmouseout="ContentUnpreview('label15');" title="click to collapse or expand..."> more... </a>
 <div id="label15" style="display:none">
 <table border="1">
 <tr>
 <td></td>
 <td colspan="1">Supported Version Ranges</td>
 </tr>
 <tr>
 <td>casb_profile_status</td>
 <td><code class="docutils literal notranslate">v7.4.1 -> latest </code></td>
 </tr>
 <tr>
 <td>[enable]</td>
 <td><code class="docutils literal notranslate">v6.0.0 -> latest</code></td> <tr>
 <td>[disable]</td>
 <td><code class="docutils literal notranslate">v6.0.0 -> latest</code></td> </table>
 </div>
 </li>
        <li> <span class="li-head">comments</span> - Comments. <span class="li-normal">type: str</span>
 <a id='label16' href="javascript:ContentClick('label17', 'label16');" onmouseover="ContentPreview('label17');" onmouseout="ContentUnpreview('label17');" title="click to collapse or expand..."> more... </a>
 <div id="label17" style="display:none">
 <table border="1">
 <tr>
 <td></td>
 <td colspan="1">Supported Version Ranges</td>
 </tr>
 <tr>
 <td>comments</td>
 <td><code class="docutils literal notranslate">v6.0.0 -> latest </code></td>
 </tr>
 </table>
 </div>
 </li>
        <li> <span class="li-head">dlp_profile</span> - DLP profile name. Source dlp.profile.name. <span class="li-normal">type: str</span>
 <a id='label18' href="javascript:ContentClick('label19', 'label18');" onmouseover="ContentPreview('label19');" onmouseout="ContentUnpreview('label19');" title="click to collapse or expand..."> more... </a>
 <div id="label19" style="display:none">
 <table border="1">
 <tr>
 <td></td>
 <td colspan="1">Supported Version Ranges</td>
 </tr>
 <tr>
 <td>dlp_profile</td>
 <td><code class="docutils literal notranslate">v7.2.0 -> latest </code></td>
 </tr>
 </table>
 </div>
 </li>
        <li> <span class="li-head">dlp_profile_status</span> - Enable/disable DLP. <span class="li-normal">type: str</span> <span class="li-normal">choices: enable, disable</span>
 <a id='label20' href="javascript:ContentClick('label21', 'label20');" onmouseover="ContentPreview('label21');" onmouseout="ContentUnpreview('label21');" title="click to collapse or expand..."> more... </a>
 <div id="label21" style="display:none">
 <table border="1">
 <tr>
 <td></td>
 <td colspan="1">Supported Version Ranges</td>
 </tr>
 <tr>
 <td>dlp_profile_status</td>
 <td><code class="docutils literal notranslate">v7.2.0 -> latest </code></td>
 </tr>
 <tr>
 <td>[enable]</td>
 <td><code class="docutils literal notranslate">v6.0.0 -> latest</code></td> <tr>
 <td>[disable]</td>
 <td><code class="docutils literal notranslate">v6.0.0 -> latest</code></td> </table>
 </div>
 </li>
        <li> <span class="li-head">dlp_sensor</span> - DLP sensor name. Source dlp.sensor.name. <span class="li-normal">type: str</span>
 <a id='label22' href="javascript:ContentClick('label23', 'label22');" onmouseover="ContentPreview('label23');" onmouseout="ContentUnpreview('label23');" title="click to collapse or expand..."> more... </a>
 <div id="label23" style="display:none">
 <table border="1">
 <tr>
 <td></td>
 <td colspan="1">Supported Version Ranges</td>
 </tr>
 <tr>
 <td>dlp_sensor</td>
 <td><code class="docutils literal notranslate">v6.0.0 -> v7.0.12 </code></td>
 </tr>
 </table>
 </div>
 </li>
        <li> <span class="li-head">dlp_sensor_status</span> - Enable/disable DLP. <span class="li-normal">type: str</span> <span class="li-normal">choices: enable, disable</span>
 <a id='label24' href="javascript:ContentClick('label25', 'label24');" onmouseover="ContentPreview('label25');" onmouseout="ContentUnpreview('label25');" title="click to collapse or expand..."> more... </a>
 <div id="label25" style="display:none">
 <table border="1">
 <tr>
 <td></td>
 <td colspan="1">Supported Version Ranges</td>
 </tr>
 <tr>
 <td>dlp_sensor_status</td>
 <td><code class="docutils literal notranslate">v6.0.0 -> v7.0.12 </code></td>
 </tr>
 <tr>
 <td>[enable]</td>
 <td><code class="docutils literal notranslate">v6.0.0 -> latest</code></td> <tr>
 <td>[disable]</td>
 <td><code class="docutils literal notranslate">v6.0.0 -> latest</code></td> </table>
 </div>
 </li>
        <li> <span class="li-head">dsri</span> - Enable/disable DSRI. <span class="li-normal">type: str</span> <span class="li-normal">choices: enable, disable</span>
 <a id='label26' href="javascript:ContentClick('label27', 'label26');" onmouseover="ContentPreview('label27');" onmouseout="ContentUnpreview('label27');" title="click to collapse or expand..."> more... </a>
 <div id="label27" style="display:none">
 <table border="1">
 <tr>
 <td></td>
 <td colspan="1">Supported Version Ranges</td>
 </tr>
 <tr>
 <td>dsri</td>
 <td><code class="docutils literal notranslate">v6.0.0 -> latest </code></td>
 </tr>
 <tr>
 <td>[enable]</td>
 <td><code class="docutils literal notranslate">v6.0.0 -> latest</code></td> <tr>
 <td>[disable]</td>
 <td><code class="docutils literal notranslate">v6.0.0 -> latest</code></td> </table>
 </div>
 </li>
        <li> <span class="li-head">dstaddr</span> - Address object to limit traffic monitoring to network traffic sent to the specified address or range. <span class="li-normal">type: list</span> <span style="font-family:'Courier New'" class="li-required">member_path: dstaddr:name</span>
 <a id='label28' href="javascript:ContentClick('label29', 'label28');" onmouseover="ContentPreview('label29');" onmouseout="ContentUnpreview('label29');" title="click to collapse or expand..."> more... </a>
 <div id="label29" style="display:none">
 <table border="1">
 <tr>
 <td></td><td colspan="1">Supported Version Ranges</td>
 </tr>
 <tr>
 <td>dstaddr</td>
 <td><code class="docutils literal notranslate">v6.0.0 -> latest </code></td>
 </tr>
 </table>
 </div>
 </li>
            <ul class="ul-self">
            <li> <span class="li-head">name</span> - Address name. Source firewall.address.name firewall.addrgrp.name. <span class="li-normal">type: str</span> <span class="li-required">required: true</span>
 <a id='label30' href="javascript:ContentClick('label31', 'label30');" onmouseover="ContentPreview('label31');" onmouseout="ContentUnpreview('label31');" title="click to collapse or expand..."> more... </a>
 <div id="label31" style="display:none">
 <table border="1">
 <tr>
 <td></td>
 <td colspan="1">Supported Version Ranges</td>
 </tr>
 <tr>
 <td>name</td>
 <td><code class="docutils literal notranslate">v6.0.0 -> latest </code></td>
 </tr>
 </table>
 </div>
 </li>
            </ul>
        <li> <span class="li-head">emailfilter_profile</span> - Email filter profile. Source emailfilter.profile.name. <span class="li-normal">type: str</span>
 <a id='label32' href="javascript:ContentClick('label33', 'label32');" onmouseover="ContentPreview('label33');" onmouseout="ContentUnpreview('label33');" title="click to collapse or expand..."> more... </a>
 <div id="label33" style="display:none">
 <table border="1">
 <tr>
 <td></td>
 <td colspan="1">Supported Version Ranges</td>
 </tr>
 <tr>
 <td>emailfilter_profile</td>
 <td><code class="docutils literal notranslate">v6.2.0 -> latest </code></td>
 </tr>
 </table>
 </div>
 </li>
        <li> <span class="li-head">emailfilter_profile_status</span> - Enable/disable email filter. <span class="li-normal">type: str</span> <span class="li-normal">choices: enable, disable</span>
 <a id='label34' href="javascript:ContentClick('label35', 'label34');" onmouseover="ContentPreview('label35');" onmouseout="ContentUnpreview('label35');" title="click to collapse or expand..."> more... </a>
 <div id="label35" style="display:none">
 <table border="1">
 <tr>
 <td></td>
 <td colspan="1">Supported Version Ranges</td>
 </tr>
 <tr>
 <td>emailfilter_profile_status</td>
 <td><code class="docutils literal notranslate">v6.2.0 -> latest </code></td>
 </tr>
 <tr>
 <td>[enable]</td>
 <td><code class="docutils literal notranslate">v6.0.0 -> latest</code></td> <tr>
 <td>[disable]</td>
 <td><code class="docutils literal notranslate">v6.0.0 -> latest</code></td> </table>
 </div>
 </li>
        <li> <span class="li-head">interface</span> - Monitored interface name from available interfaces. Source system.zone.name system.interface.name. <span class="li-normal">type: str</span>
 <a id='label36' href="javascript:ContentClick('label37', 'label36');" onmouseover="ContentPreview('label37');" onmouseout="ContentUnpreview('label37');" title="click to collapse or expand..."> more... </a>
 <div id="label37" style="display:none">
 <table border="1">
 <tr>
 <td></td>
 <td colspan="1">Supported Version Ranges</td>
 </tr>
 <tr>
 <td>interface</td>
 <td><code class="docutils literal notranslate">v6.0.0 -> latest </code></td>
 </tr>
 </table>
 </div>
 </li>
        <li> <span class="li-head">ips_sensor</span> - IPS sensor name. Source ips.sensor.name. <span class="li-normal">type: str</span>
 <a id='label38' href="javascript:ContentClick('label39', 'label38');" onmouseover="ContentPreview('label39');" onmouseout="ContentUnpreview('label39');" title="click to collapse or expand..."> more... </a>
 <div id="label39" style="display:none">
 <table border="1">
 <tr>
 <td></td>
 <td colspan="1">Supported Version Ranges</td>
 </tr>
 <tr>
 <td>ips_sensor</td>
 <td><code class="docutils literal notranslate">v6.0.0 -> latest </code></td>
 </tr>
 </table>
 </div>
 </li>
        <li> <span class="li-head">ips_sensor_status</span> - Enable/disable IPS. <span class="li-normal">type: str</span> <span class="li-normal">choices: enable, disable</span>
 <a id='label40' href="javascript:ContentClick('label41', 'label40');" onmouseover="ContentPreview('label41');" onmouseout="ContentUnpreview('label41');" title="click to collapse or expand..."> more... </a>
 <div id="label41" style="display:none">
 <table border="1">
 <tr>
 <td></td>
 <td colspan="1">Supported Version Ranges</td>
 </tr>
 <tr>
 <td>ips_sensor_status</td>
 <td><code class="docutils literal notranslate">v6.0.0 -> latest </code></td>
 </tr>
 <tr>
 <td>[enable]</td>
 <td><code class="docutils literal notranslate">v6.0.0 -> latest</code></td> <tr>
 <td>[disable]</td>
 <td><code class="docutils literal notranslate">v6.0.0 -> latest</code></td> </table>
 </div>
 </li>
        <li> <span class="li-head">label</span> - Label. <span class="li-normal">type: str</span>
 <a id='label42' href="javascript:ContentClick('label43', 'label42');" onmouseover="ContentPreview('label43');" onmouseout="ContentUnpreview('label43');" title="click to collapse or expand..."> more... </a>
 <div id="label43" style="display:none">
 <table border="1">
 <tr>
 <td></td>
 <td colspan="2">Supported Version Ranges</td>
 </tr>
 <tr>
 <td>label</td>
 <td><code class="docutils literal notranslate">v6.0.0 -> v6.0.11 </code></td>
 <td><code class="docutils literal notranslate">v6.2.3 -> v6.2.3 </code></td>
 </tr>
 </table>
 </div>
 </li>
        <li> <span class="li-head">logtraffic</span> - Logging type to be used in this policy (Options: all | utm | disable). <span class="li-normal">type: str</span> <span class="li-normal">choices: all, utm, disable</span>
 <a id='label44' href="javascript:ContentClick('label45', 'label44');" onmouseover="ContentPreview('label45');" onmouseout="ContentUnpreview('label45');" title="click to collapse or expand..."> more... </a>
 <div id="label45" style="display:none">
 <table border="1">
 <tr>
 <td></td>
 <td colspan="1">Supported Version Ranges</td>
 </tr>
 <tr>
 <td>logtraffic</td>
 <td><code class="docutils literal notranslate">v6.0.0 -> latest </code></td>
 </tr>
 <tr>
 <td>[all]</td>
 <td><code class="docutils literal notranslate">v6.0.0 -> latest</code></td> <tr>
 <td>[utm]</td>
 <td><code class="docutils literal notranslate">v6.0.0 -> latest</code></td> <tr>
 <td>[disable]</td>
 <td><code class="docutils literal notranslate">v6.0.0 -> latest</code></td> </table>
 </div>
 </li>
        <li> <span class="li-head">policyid</span> - Policy ID (0 - 4294967295). see <a href='#notes'>Notes</a>. <span class="li-normal">type: int</span> <span class="li-required">required: true</span>
 <a id='label46' href="javascript:ContentClick('label47', 'label46');" onmouseover="ContentPreview('label47');" onmouseout="ContentUnpreview('label47');" title="click to collapse or expand..."> more... </a>
 <div id="label47" style="display:none">
 <table border="1">
 <tr>
 <td></td>
 <td colspan="1">Supported Version Ranges</td>
 </tr>
 <tr>
 <td>policyid</td>
 <td><code class="docutils literal notranslate">v6.0.0 -> latest </code></td>
 </tr>
 </table>
 </div>
 </li>
        <li> <span class="li-head">scan_botnet_connections</span> - Enable/disable scanning for connections to Botnet servers. <span class="li-normal">type: str</span> <span class="li-normal">choices: disable, block, monitor</span>
 <a id='label48' href="javascript:ContentClick('label49', 'label48');" onmouseover="ContentPreview('label49');" onmouseout="ContentUnpreview('label49');" title="click to collapse or expand..."> more... </a>
 <div id="label49" style="display:none">
 <table border="1">
 <tr>
 <td></td>
 <td colspan="1">Supported Version Ranges</td>
 </tr>
 <tr>
 <td>scan_botnet_connections</td>
 <td><code class="docutils literal notranslate">v6.0.0 -> v6.0.11 </code></td>
 </tr>
 <tr>
 <td>[disable]</td>
 <td><code class="docutils literal notranslate">v6.0.0 -> latest</code></td> <tr>
 <td>[block]</td>
 <td><code class="docutils literal notranslate">v6.0.0 -> latest</code></td> <tr>
 <td>[monitor]</td>
 <td><code class="docutils literal notranslate">v6.0.0 -> latest</code></td> </table>
 </div>
 </li>
        <li> <span class="li-head">service</span> - Service object from available options. <span class="li-normal">type: list</span> <span style="font-family:'Courier New'" class="li-required">member_path: service:name</span>
 <a id='label50' href="javascript:ContentClick('label51', 'label50');" onmouseover="ContentPreview('label51');" onmouseout="ContentUnpreview('label51');" title="click to collapse or expand..."> more... </a>
 <div id="label51" style="display:none">
 <table border="1">
 <tr>
 <td></td><td colspan="1">Supported Version Ranges</td>
 </tr>
 <tr>
 <td>service</td>
 <td><code class="docutils literal notranslate">v6.0.0 -> latest </code></td>
 </tr>
 </table>
 </div>
 </li>
            <ul class="ul-self">
            <li> <span class="li-head">name</span> - Service name. Source firewall.service.custom.name firewall.service.group.name. <span class="li-normal">type: str</span> <span class="li-required">required: true</span>
 <a id='label52' href="javascript:ContentClick('label53', 'label52');" onmouseover="ContentPreview('label53');" onmouseout="ContentUnpreview('label53');" title="click to collapse or expand..."> more... </a>
 <div id="label53" style="display:none">
 <table border="1">
 <tr>
 <td></td>
 <td colspan="1">Supported Version Ranges</td>
 </tr>
 <tr>
 <td>name</td>
 <td><code class="docutils literal notranslate">v6.0.0 -> latest </code></td>
 </tr>
 </table>
 </div>
 </li>
            </ul>
        <li> <span class="li-head">spamfilter_profile</span> - Antispam profile. Source spamfilter.profile.name. <span class="li-normal">type: str</span>
 <a id='label54' href="javascript:ContentClick('label55', 'label54');" onmouseover="ContentPreview('label55');" onmouseout="ContentUnpreview('label55');" title="click to collapse or expand..."> more... </a>
 <div id="label55" style="display:none">
 <table border="1">
 <tr>
 <td></td>
 <td colspan="1">Supported Version Ranges</td>
 </tr>
 <tr>
 <td>spamfilter_profile</td>
 <td><code class="docutils literal notranslate">v6.0.0 -> v6.0.11 </code></td>
 </tr>
 </table>
 </div>
 </li>
        <li> <span class="li-head">spamfilter_profile_status</span> - Enable/disable antispam. <span class="li-normal">type: str</span> <span class="li-normal">choices: enable, disable</span>
 <a id='label56' href="javascript:ContentClick('label57', 'label56');" onmouseover="ContentPreview('label57');" onmouseout="ContentUnpreview('label57');" title="click to collapse or expand..."> more... </a>
 <div id="label57" style="display:none">
 <table border="1">
 <tr>
 <td></td>
 <td colspan="1">Supported Version Ranges</td>
 </tr>
 <tr>
 <td>spamfilter_profile_status</td>
 <td><code class="docutils literal notranslate">v6.0.0 -> v6.0.11 </code></td>
 </tr>
 <tr>
 <td>[enable]</td>
 <td><code class="docutils literal notranslate">v6.0.0 -> latest</code></td> <tr>
 <td>[disable]</td>
 <td><code class="docutils literal notranslate">v6.0.0 -> latest</code></td> </table>
 </div>
 </li>
        <li> <span class="li-head">srcaddr</span> - Address object to limit traffic monitoring to network traffic sent from the specified address or range. <span class="li-normal">type: list</span> <span style="font-family:'Courier New'" class="li-required">member_path: srcaddr:name</span>
 <a id='label58' href="javascript:ContentClick('label59', 'label58');" onmouseover="ContentPreview('label59');" onmouseout="ContentUnpreview('label59');" title="click to collapse or expand..."> more... </a>
 <div id="label59" style="display:none">
 <table border="1">
 <tr>
 <td></td><td colspan="1">Supported Version Ranges</td>
 </tr>
 <tr>
 <td>srcaddr</td>
 <td><code class="docutils literal notranslate">v6.0.0 -> latest </code></td>
 </tr>
 </table>
 </div>
 </li>
            <ul class="ul-self">
            <li> <span class="li-head">name</span> - Address name. Source firewall.address.name firewall.addrgrp.name. <span class="li-normal">type: str</span> <span class="li-required">required: true</span>
 <a id='label60' href="javascript:ContentClick('label61', 'label60');" onmouseover="ContentPreview('label61');" onmouseout="ContentUnpreview('label61');" title="click to collapse or expand..."> more... </a>
 <div id="label61" style="display:none">
 <table border="1">
 <tr>
 <td></td>
 <td colspan="1">Supported Version Ranges</td>
 </tr>
 <tr>
 <td>name</td>
 <td><code class="docutils literal notranslate">v6.0.0 -> latest </code></td>
 </tr>
 </table>
 </div>
 </li>
            </ul>
        <li> <span class="li-head">status</span> - Enable/disable this policy. <span class="li-normal">type: str</span> <span class="li-normal">choices: enable, disable</span>
 <a id='label62' href="javascript:ContentClick('label63', 'label62');" onmouseover="ContentPreview('label63');" onmouseout="ContentUnpreview('label63');" title="click to collapse or expand..."> more... </a>
 <div id="label63" style="display:none">
 <table border="1">
 <tr>
 <td></td>
 <td colspan="1">Supported Version Ranges</td>
 </tr>
 <tr>
 <td>status</td>
 <td><code class="docutils literal notranslate">v6.0.0 -> latest </code></td>
 </tr>
 <tr>
 <td>[enable]</td>
 <td><code class="docutils literal notranslate">v6.0.0 -> latest</code></td> <tr>
 <td>[disable]</td>
 <td><code class="docutils literal notranslate">v6.0.0 -> latest</code></td> </table>
 </div>
 </li>
        <li> <span class="li-head">webfilter_profile</span> - Web filter profile. Source webfilter.profile.name. <span class="li-normal">type: str</span>
 <a id='label64' href="javascript:ContentClick('label65', 'label64');" onmouseover="ContentPreview('label65');" onmouseout="ContentUnpreview('label65');" title="click to collapse or expand..."> more... </a>
 <div id="label65" style="display:none">
 <table border="1">
 <tr>
 <td></td>
 <td colspan="1">Supported Version Ranges</td>
 </tr>
 <tr>
 <td>webfilter_profile</td>
 <td><code class="docutils literal notranslate">v6.0.0 -> latest </code></td>
 </tr>
 </table>
 </div>
 </li>
        <li> <span class="li-head">webfilter_profile_status</span> - Enable/disable web filtering. <span class="li-normal">type: str</span> <span class="li-normal">choices: enable, disable</span>
 <a id='label66' href="javascript:ContentClick('label67', 'label66');" onmouseover="ContentPreview('label67');" onmouseout="ContentUnpreview('label67');" title="click to collapse or expand..."> more... </a>
 <div id="label67" style="display:none">
 <table border="1">
 <tr>
 <td></td>
 <td colspan="1">Supported Version Ranges</td>
 </tr>
 <tr>
 <td>webfilter_profile_status</td>
 <td><code class="docutils literal notranslate">v6.0.0 -> latest </code></td>
 </tr>
 <tr>
 <td>[enable]</td>
 <td><code class="docutils literal notranslate">v6.0.0 -> latest</code></td> <tr>
 <td>[disable]</td>
 <td><code class="docutils literal notranslate">v6.0.0 -> latest</code></td> </table>
 </div>
 </li>
        </ul>
    </ul>


Notes
-----

.. note::

   - We highly recommend using your own value as the policyid instead of 0, while '0' is a special placeholder that allows the backend to assign the latest available number for the object, it does have limitations. Please find more details in Q&A.

   - Legacy fortiosapi has been deprecated, httpapi is the preferred way to run playbooks



Examples
--------

.. code-block:: yaml+jinja
    
    - name: Configure IPv4 interface policies.
      fortinet.fortios.fortios_firewall_interface_policy:
          vdom: "{{ vdom }}"
          state: "present"
          access_token: "<your_own_value>"
          firewall_interface_policy:
              address_type: "ipv4"
              application_list: "<your_own_value> (source application.list.name)"
              application_list_status: "enable"
              av_profile: "<your_own_value> (source antivirus.profile.name)"
              av_profile_status: "enable"
              casb_profile: "<your_own_value> (source casb.profile.name)"
              casb_profile_status: "enable"
              comments: "<your_own_value>"
              dlp_profile: "<your_own_value> (source dlp.profile.name)"
              dlp_profile_status: "enable"
              dlp_sensor: "<your_own_value> (source dlp.sensor.name)"
              dlp_sensor_status: "enable"
              dsri: "enable"
              dstaddr:
                  -
                      name: "default_name_17 (source firewall.address.name firewall.addrgrp.name)"
              emailfilter_profile: "<your_own_value> (source emailfilter.profile.name)"
              emailfilter_profile_status: "enable"
              interface: "<your_own_value> (source system.zone.name system.interface.name)"
              ips_sensor: "<your_own_value> (source ips.sensor.name)"
              ips_sensor_status: "enable"
              label: "<your_own_value>"
              logtraffic: "all"
              policyid: "<you_own_value>"
              scan_botnet_connections: "disable"
              service:
                  -
                      name: "default_name_28 (source firewall.service.custom.name firewall.service.group.name)"
              spamfilter_profile: "<your_own_value> (source spamfilter.profile.name)"
              spamfilter_profile_status: "enable"
              srcaddr:
                  -
                      name: "default_name_32 (source firewall.address.name firewall.addrgrp.name)"
              status: "enable"
              webfilter_profile: "<your_own_value> (source webfilter.profile.name)"
              webfilter_profile_status: "enable"


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
