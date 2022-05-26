:source: fortios_firewall_central_snat_map.py

:orphan:

.. fortios_firewall_central_snat_map:

fortios_firewall_central_snat_map -- Configure IPv4 and IPv6 central SNAT policies in Fortinet's FortiOS and FortiGate.
+++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++

.. versionadded:: 2.0.0

.. contents::
   :local:
   :depth: 1


Synopsis
--------
- This module is able to configure a FortiGate or FortiOS (FOS) device by allowing the user to set and modify firewall feature and central_snat_map category. Examples include all parameters and values need to be adjusted to datasources before usage. Tested with FOS v6.0.0



Requirements
------------
The below requirements are needed on the host that executes this module.

- ansible>=2.9.0


FortiOS Version Compatibility
-----------------------------


.. raw:: html

 <br>
 <table>
 <tr>
 <td></td>
 <td><code class="docutils literal notranslate">v6.0.0 </code></td>
 <td><code class="docutils literal notranslate">v6.0.5 </code></td>
 <td><code class="docutils literal notranslate">v6.0.11 </code></td>
 <td><code class="docutils literal notranslate">v6.2.0 </code></td>
 <td><code class="docutils literal notranslate">v6.2.3 </code></td>
 <td><code class="docutils literal notranslate">v6.2.5 </code></td>
 <td><code class="docutils literal notranslate">v6.2.7 </code></td>
 <td><code class="docutils literal notranslate">v6.4.0 </code></td>
 <td><code class="docutils literal notranslate">v6.4.1 </code></td>
 <td><code class="docutils literal notranslate">v6.4.4 </code></td>
 <td><code class="docutils literal notranslate">v7.0.0 </code></td>
 <td><code class="docutils literal notranslate">v7.0.1 </code></td>
 <td><code class="docutils literal notranslate">v7.0.2 </code></td>
 <td><code class="docutils literal notranslate">v7.0.3 </code></td>
 <td><code class="docutils literal notranslate">v7.0.4 </code></td>
 <td><code class="docutils literal notranslate">v7.0.5 </code></td>
 </tr>
 <tr>
 <td>fortios_firewall_central_snat_map</td>
 <td>yes</td>
 <td>yes</td>
 <td>yes</td>
 <td>yes</td>
 <td>yes</td>
 <td>yes</td>
 <td>yes</td>
 <td>yes</td>
 <td>yes</td>
 <td>yes</td>
 <td>yes</td>
 <td>yes</td>
 <td>yes</td>
 <td>yes</td>
 <td>yes</td>
 <td>yes</td>
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
    <li> <span class="li-head">action</span> - the action indiactor to move an object in the list <span class="li-normal">type: str</span> <span class="li-normal">choices: move</span> </li>
    <li> <span class="li-head">self</span> - mkey of self identifier <span class="li-normal">type: str</span> </li>
    <li> <span class="li-head">after</span> - mkey of target identifier <span class="li-normal">type: str</span> </li>
    <li> <span class="li-head">before</span> - mkey of target identifier <span class="li-normal">type: str</span> </li>
    <li> <span class="li-head">state</span> - Indicates whether to create or remove the object. <span class="li-normal">type: str</span> <span class="li-required">required: true</span> <span class="li-normal">choices: present, absent</span> </li>
    <li> <span class="li-head">firewall_central_snat_map</span> - Configure IPv4 and IPv6 central SNAT policies. <span class="li-normal">type: dict</span>
 <a id='label0' href="javascript:ContentClick('label1', 'label0');" onmouseover="ContentPreview('label1');" onmouseout="ContentUnpreview('label1');" title="click to collapse or expand..."> more... </a>
 <div id="label1" style="display:none">
 <table border="1">
 <tr>
 <td></td>
 <td><code class="docutils literal notranslate">v6.0.0 </code></td>
 <td><code class="docutils literal notranslate">v6.0.5 </code></td>
 <td><code class="docutils literal notranslate">v6.0.11 </code></td>
 <td><code class="docutils literal notranslate">v6.2.0 </code></td>
 <td><code class="docutils literal notranslate">v6.2.3 </code></td>
 <td><code class="docutils literal notranslate">v6.2.5 </code></td>
 <td><code class="docutils literal notranslate">v6.2.7 </code></td>
 <td><code class="docutils literal notranslate">v6.4.0 </code></td>
 <td><code class="docutils literal notranslate">v6.4.1 </code></td>
 <td><code class="docutils literal notranslate">v6.4.4 </code></td>
 <td><code class="docutils literal notranslate">v7.0.0 </code></td>
 <td><code class="docutils literal notranslate">v7.0.1 </code></td>
 <td><code class="docutils literal notranslate">v7.0.2 </code></td>
 <td><code class="docutils literal notranslate">v7.0.3 </code></td>
 <td><code class="docutils literal notranslate">v7.0.4 </code></td>
 <td><code class="docutils literal notranslate">v7.0.5 </code></td>
 </tr>
 <tr>
 <td>firewall_central_snat_map</td>
 <td>yes</td>
 <td>yes</td>
 <td>yes</td>
 <td>yes</td>
 <td>yes</td>
 <td>yes</td>
 <td>yes</td>
 <td>yes</td>
 <td>yes</td>
 <td>yes</td>
 <td>yes</td>
 <td>yes</td>
 <td>yes</td>
 <td>yes</td>
 <td>yes</td>
 <td>yes</td>
 </tr>
 </table>
 </div>
 </li>
        <ul class="ul-self">
        <li> <span class="li-head">comments</span> - Comment. <span class="li-normal">type: str</span>
 <a id='label2' href="javascript:ContentClick('label3', 'label2');" onmouseover="ContentPreview('label3');" onmouseout="ContentUnpreview('label3');" title="click to collapse or expand..."> more... </a>
 <div id="label3" style="display:none">
 <table border="1">
 <tr>
 <td></td>
 <td><code class="docutils literal notranslate">v6.0.0 </code></td>
 <td><code class="docutils literal notranslate">v6.0.5 </code></td>
 <td><code class="docutils literal notranslate">v6.0.11 </code></td>
 <td><code class="docutils literal notranslate">v6.2.0 </code></td>
 <td><code class="docutils literal notranslate">v6.2.3 </code></td>
 <td><code class="docutils literal notranslate">v6.2.5 </code></td>
 <td><code class="docutils literal notranslate">v6.2.7 </code></td>
 <td><code class="docutils literal notranslate">v6.4.0 </code></td>
 <td><code class="docutils literal notranslate">v6.4.1 </code></td>
 <td><code class="docutils literal notranslate">v6.4.4 </code></td>
 <td><code class="docutils literal notranslate">v7.0.0 </code></td>
 <td><code class="docutils literal notranslate">v7.0.1 </code></td>
 <td><code class="docutils literal notranslate">v7.0.2 </code></td>
 <td><code class="docutils literal notranslate">v7.0.3 </code></td>
 <td><code class="docutils literal notranslate">v7.0.4 </code></td>
 <td><code class="docutils literal notranslate">v7.0.5 </code></td>
 </tr>
 <tr>
 <td>comments</td>
 <td>yes</td>
 <td>yes</td>
 <td>yes</td>
 <td>yes</td>
 <td>yes</td>
 <td>yes</td>
 <td>yes</td>
 <td>yes</td>
 <td>yes</td>
 <td>yes</td>
 <td>yes</td>
 <td>yes</td>
 <td>yes</td>
 <td>yes</td>
 <td>yes</td>
 <td>yes</td>
 </tr>
 </table>
 </div>
 </li>
        <li> <span class="li-head">dst_addr</span> - IPv4 Destination address. <span class="li-normal">type: list</span> <span style="font-family:'Courier New'" class="li-required">member_path: dst_addr:name</span>
 <a id='label4' href="javascript:ContentClick('label5', 'label4');" onmouseover="ContentPreview('label5');" onmouseout="ContentUnpreview('label5');" title="click to collapse or expand..."> more... </a>
 <div id="label5" style="display:none">
 <table border="1">
 <tr>
 <td></td>
 <td><code class="docutils literal notranslate">v6.0.0 </code></td>
 <td><code class="docutils literal notranslate">v6.0.5 </code></td>
 <td><code class="docutils literal notranslate">v6.0.11 </code></td>
 <td><code class="docutils literal notranslate">v6.2.0 </code></td>
 <td><code class="docutils literal notranslate">v6.2.3 </code></td>
 <td><code class="docutils literal notranslate">v6.2.5 </code></td>
 <td><code class="docutils literal notranslate">v6.2.7 </code></td>
 <td><code class="docutils literal notranslate">v6.4.0 </code></td>
 <td><code class="docutils literal notranslate">v6.4.1 </code></td>
 <td><code class="docutils literal notranslate">v6.4.4 </code></td>
 <td><code class="docutils literal notranslate">v7.0.0 </code></td>
 <td><code class="docutils literal notranslate">v7.0.1 </code></td>
 <td><code class="docutils literal notranslate">v7.0.2 </code></td>
 <td><code class="docutils literal notranslate">v7.0.3 </code></td>
 <td><code class="docutils literal notranslate">v7.0.4 </code></td>
 <td><code class="docutils literal notranslate">v7.0.5 </code></td>
 </tr>
 <tr>
 <td>dst_addr</td>
 <td>yes</td>
 <td>yes</td>
 <td>yes</td>
 <td>yes</td>
 <td>yes</td>
 <td>yes</td>
 <td>yes</td>
 <td>yes</td>
 <td>yes</td>
 <td>yes</td>
 <td>yes</td>
 <td>yes</td>
 <td>yes</td>
 <td>yes</td>
 <td>yes</td>
 <td>yes</td>
 </tr>
 </table>
 </div>
 </li>
            <ul class="ul-self">
            <li> <span class="li-head">name</span> - Address name. Source firewall.address.name firewall.addrgrp.name. <span class="li-normal">type: str</span> <span class="li-required">required: true</span>
 <a id='label6' href="javascript:ContentClick('label7', 'label6');" onmouseover="ContentPreview('label7');" onmouseout="ContentUnpreview('label7');" title="click to collapse or expand..."> more... </a>
 <div id="label7" style="display:none">
 <table border="1">
 <tr>
 <td></td>
 <td><code class="docutils literal notranslate">v6.0.0 </code></td>
 <td><code class="docutils literal notranslate">v6.0.5 </code></td>
 <td><code class="docutils literal notranslate">v6.0.11 </code></td>
 <td><code class="docutils literal notranslate">v6.2.0 </code></td>
 <td><code class="docutils literal notranslate">v6.2.3 </code></td>
 <td><code class="docutils literal notranslate">v6.2.5 </code></td>
 <td><code class="docutils literal notranslate">v6.2.7 </code></td>
 <td><code class="docutils literal notranslate">v6.4.0 </code></td>
 <td><code class="docutils literal notranslate">v6.4.1 </code></td>
 <td><code class="docutils literal notranslate">v6.4.4 </code></td>
 <td><code class="docutils literal notranslate">v7.0.0 </code></td>
 <td><code class="docutils literal notranslate">v7.0.1 </code></td>
 <td><code class="docutils literal notranslate">v7.0.2 </code></td>
 <td><code class="docutils literal notranslate">v7.0.3 </code></td>
 <td><code class="docutils literal notranslate">v7.0.4 </code></td>
 <td><code class="docutils literal notranslate">v7.0.5 </code></td>
 </tr>
 <tr>
 <td>name</td>
 <td>yes</td>
 <td>yes</td>
 <td>yes</td>
 <td>yes</td>
 <td>yes</td>
 <td>yes</td>
 <td>yes</td>
 <td>yes</td>
 <td>yes</td>
 <td>yes</td>
 <td>yes</td>
 <td>yes</td>
 <td>yes</td>
 <td>yes</td>
 <td>yes</td>
 <td>yes</td>
 </tr>
 </table>
 </div>
 </li>
            </ul>
        <li> <span class="li-head">dst_addr6</span> - IPv6 Destination address. <span class="li-normal">type: list</span> <span style="font-family:'Courier New'" class="li-required">member_path: dst_addr6:name</span>
 <a id='label8' href="javascript:ContentClick('label9', 'label8');" onmouseover="ContentPreview('label9');" onmouseout="ContentUnpreview('label9');" title="click to collapse or expand..."> more... </a>
 <div id="label9" style="display:none">
 <table border="1">
 <tr>
 <td></td>
 <td><code class="docutils literal notranslate">v6.0.0 </code></td>
 <td><code class="docutils literal notranslate">v6.0.5 </code></td>
 <td><code class="docutils literal notranslate">v6.0.11 </code></td>
 <td><code class="docutils literal notranslate">v6.2.0 </code></td>
 <td><code class="docutils literal notranslate">v6.2.3 </code></td>
 <td><code class="docutils literal notranslate">v6.2.5 </code></td>
 <td><code class="docutils literal notranslate">v6.2.7 </code></td>
 <td><code class="docutils literal notranslate">v6.4.0 </code></td>
 <td><code class="docutils literal notranslate">v6.4.1 </code></td>
 <td><code class="docutils literal notranslate">v6.4.4 </code></td>
 <td><code class="docutils literal notranslate">v7.0.0 </code></td>
 <td><code class="docutils literal notranslate">v7.0.1 </code></td>
 <td><code class="docutils literal notranslate">v7.0.2 </code></td>
 <td><code class="docutils literal notranslate">v7.0.3 </code></td>
 <td><code class="docutils literal notranslate">v7.0.4 </code></td>
 <td><code class="docutils literal notranslate">v7.0.5 </code></td>
 </tr>
 <tr>
 <td>dst_addr6</td>
 <td>no</td>
 <td>no</td>
 <td>no</td>
 <td>no</td>
 <td>no</td>
 <td>no</td>
 <td>no</td>
 <td>yes</td>
 <td>yes</td>
 <td>yes</td>
 <td>yes</td>
 <td>yes</td>
 <td>yes</td>
 <td>yes</td>
 <td>yes</td>
 <td>yes</td>
 </tr>
 </table>
 </div>
 </li>
            <ul class="ul-self">
            <li> <span class="li-head">name</span> - Address name. Source firewall.address6.name firewall.addrgrp6.name. <span class="li-normal">type: str</span> <span class="li-required">required: true</span>
 <a id='label10' href="javascript:ContentClick('label11', 'label10');" onmouseover="ContentPreview('label11');" onmouseout="ContentUnpreview('label11');" title="click to collapse or expand..."> more... </a>
 <div id="label11" style="display:none">
 <table border="1">
 <tr>
 <td></td>
 <td><code class="docutils literal notranslate">v6.4.0 </code></td>
 <td><code class="docutils literal notranslate">v6.4.1 </code></td>
 <td><code class="docutils literal notranslate">v6.4.4 </code></td>
 <td><code class="docutils literal notranslate">v7.0.0 </code></td>
 <td><code class="docutils literal notranslate">v7.0.1 </code></td>
 <td><code class="docutils literal notranslate">v7.0.2 </code></td>
 <td><code class="docutils literal notranslate">v7.0.3 </code></td>
 <td><code class="docutils literal notranslate">v7.0.4 </code></td>
 <td><code class="docutils literal notranslate">v7.0.5 </code></td>
 </tr>
 <tr>
 <td>name</td>
 <td>yes</td>
 <td>yes</td>
 <td>yes</td>
 <td>yes</td>
 <td>yes</td>
 <td>yes</td>
 <td>yes</td>
 <td>yes</td>
 <td>yes</td>
 </tr>
 </table>
 </div>
 </li>
            </ul>
        <li> <span class="li-head">dstintf</span> - Destination interface name from available interfaces. <span class="li-normal">type: list</span> <span style="font-family:'Courier New'" class="li-required">member_path: dstintf:name</span>
 <a id='label12' href="javascript:ContentClick('label13', 'label12');" onmouseover="ContentPreview('label13');" onmouseout="ContentUnpreview('label13');" title="click to collapse or expand..."> more... </a>
 <div id="label13" style="display:none">
 <table border="1">
 <tr>
 <td></td>
 <td><code class="docutils literal notranslate">v6.0.0 </code></td>
 <td><code class="docutils literal notranslate">v6.0.5 </code></td>
 <td><code class="docutils literal notranslate">v6.0.11 </code></td>
 <td><code class="docutils literal notranslate">v6.2.0 </code></td>
 <td><code class="docutils literal notranslate">v6.2.3 </code></td>
 <td><code class="docutils literal notranslate">v6.2.5 </code></td>
 <td><code class="docutils literal notranslate">v6.2.7 </code></td>
 <td><code class="docutils literal notranslate">v6.4.0 </code></td>
 <td><code class="docutils literal notranslate">v6.4.1 </code></td>
 <td><code class="docutils literal notranslate">v6.4.4 </code></td>
 <td><code class="docutils literal notranslate">v7.0.0 </code></td>
 <td><code class="docutils literal notranslate">v7.0.1 </code></td>
 <td><code class="docutils literal notranslate">v7.0.2 </code></td>
 <td><code class="docutils literal notranslate">v7.0.3 </code></td>
 <td><code class="docutils literal notranslate">v7.0.4 </code></td>
 <td><code class="docutils literal notranslate">v7.0.5 </code></td>
 </tr>
 <tr>
 <td>dstintf</td>
 <td>yes</td>
 <td>yes</td>
 <td>yes</td>
 <td>yes</td>
 <td>yes</td>
 <td>yes</td>
 <td>yes</td>
 <td>yes</td>
 <td>yes</td>
 <td>yes</td>
 <td>yes</td>
 <td>yes</td>
 <td>yes</td>
 <td>yes</td>
 <td>yes</td>
 <td>yes</td>
 </tr>
 </table>
 </div>
 </li>
            <ul class="ul-self">
            <li> <span class="li-head">name</span> - Interface name. Source system.interface.name system.zone.name. <span class="li-normal">type: str</span> <span class="li-required">required: true</span>
 <a id='label14' href="javascript:ContentClick('label15', 'label14');" onmouseover="ContentPreview('label15');" onmouseout="ContentUnpreview('label15');" title="click to collapse or expand..."> more... </a>
 <div id="label15" style="display:none">
 <table border="1">
 <tr>
 <td></td>
 <td><code class="docutils literal notranslate">v6.0.0 </code></td>
 <td><code class="docutils literal notranslate">v6.0.5 </code></td>
 <td><code class="docutils literal notranslate">v6.0.11 </code></td>
 <td><code class="docutils literal notranslate">v6.2.0 </code></td>
 <td><code class="docutils literal notranslate">v6.2.3 </code></td>
 <td><code class="docutils literal notranslate">v6.2.5 </code></td>
 <td><code class="docutils literal notranslate">v6.2.7 </code></td>
 <td><code class="docutils literal notranslate">v6.4.0 </code></td>
 <td><code class="docutils literal notranslate">v6.4.1 </code></td>
 <td><code class="docutils literal notranslate">v6.4.4 </code></td>
 <td><code class="docutils literal notranslate">v7.0.0 </code></td>
 <td><code class="docutils literal notranslate">v7.0.1 </code></td>
 <td><code class="docutils literal notranslate">v7.0.2 </code></td>
 <td><code class="docutils literal notranslate">v7.0.3 </code></td>
 <td><code class="docutils literal notranslate">v7.0.4 </code></td>
 <td><code class="docutils literal notranslate">v7.0.5 </code></td>
 </tr>
 <tr>
 <td>name</td>
 <td>yes</td>
 <td>yes</td>
 <td>yes</td>
 <td>yes</td>
 <td>yes</td>
 <td>yes</td>
 <td>yes</td>
 <td>yes</td>
 <td>yes</td>
 <td>yes</td>
 <td>yes</td>
 <td>yes</td>
 <td>yes</td>
 <td>yes</td>
 <td>yes</td>
 <td>yes</td>
 </tr>
 </table>
 </div>
 </li>
            </ul>
        <li> <span class="li-head">nat</span> - Enable/disable source NAT. <span class="li-normal">type: str</span> <span class="li-normal">choices: disable, enable</span>
 <a id='label16' href="javascript:ContentClick('label17', 'label16');" onmouseover="ContentPreview('label17');" onmouseout="ContentUnpreview('label17');" title="click to collapse or expand..."> more... </a>
 <div id="label17" style="display:none">
 <table border="1">
 <tr>
 <td></td>
 <td><code class="docutils literal notranslate">v6.0.0 </code></td>
 <td><code class="docutils literal notranslate">v6.0.5 </code></td>
 <td><code class="docutils literal notranslate">v6.0.11 </code></td>
 <td><code class="docutils literal notranslate">v6.2.0 </code></td>
 <td><code class="docutils literal notranslate">v6.2.3 </code></td>
 <td><code class="docutils literal notranslate">v6.2.5 </code></td>
 <td><code class="docutils literal notranslate">v6.2.7 </code></td>
 <td><code class="docutils literal notranslate">v6.4.0 </code></td>
 <td><code class="docutils literal notranslate">v6.4.1 </code></td>
 <td><code class="docutils literal notranslate">v6.4.4 </code></td>
 <td><code class="docutils literal notranslate">v7.0.0 </code></td>
 <td><code class="docutils literal notranslate">v7.0.1 </code></td>
 <td><code class="docutils literal notranslate">v7.0.2 </code></td>
 <td><code class="docutils literal notranslate">v7.0.3 </code></td>
 <td><code class="docutils literal notranslate">v7.0.4 </code></td>
 <td><code class="docutils literal notranslate">v7.0.5 </code></td>
 </tr>
 <tr>
 <td>nat</td>
 <td>yes</td>
 <td>yes</td>
 <td>yes</td>
 <td>yes</td>
 <td>yes</td>
 <td>yes</td>
 <td>yes</td>
 <td>yes</td>
 <td>yes</td>
 <td>yes</td>
 <td>yes</td>
 <td>yes</td>
 <td>yes</td>
 <td>yes</td>
 <td>yes</td>
 <td>yes</td>
 </tr>
 <tr>
 <td>[disable]</td>
 <td>yes</td>
 <td>yes</td>
 <td>yes</td>
 <td>yes</td>
 <td>yes</td>
 <td>yes</td>
 <td>yes</td>
 <td>yes</td>
 <td>yes</td>
 <td>yes</td>
 <td>yes</td>
 <td>yes</td>
 <td>yes</td>
 <td>yes</td>
 <td>yes</td>
 <td>yes</td>
 </tr>
 <tr>
 <td>[enable]</td>
 <td>yes</td>
 <td>yes</td>
 <td>yes</td>
 <td>yes</td>
 <td>yes</td>
 <td>yes</td>
 <td>yes</td>
 <td>yes</td>
 <td>yes</td>
 <td>yes</td>
 <td>yes</td>
 <td>yes</td>
 <td>yes</td>
 <td>yes</td>
 <td>yes</td>
 <td>yes</td>
 </tr>
 </table>
 </div>
 </li>
        <li> <span class="li-head">nat_ippool</span> - Name of the IP pools to be used to translate addresses from available IP Pools. <span class="li-normal">type: list</span> <span style="font-family:'Courier New'" class="li-required">member_path: nat_ippool:name</span>
 <a id='label18' href="javascript:ContentClick('label19', 'label18');" onmouseover="ContentPreview('label19');" onmouseout="ContentUnpreview('label19');" title="click to collapse or expand..."> more... </a>
 <div id="label19" style="display:none">
 <table border="1">
 <tr>
 <td></td>
 <td><code class="docutils literal notranslate">v6.0.0 </code></td>
 <td><code class="docutils literal notranslate">v6.0.5 </code></td>
 <td><code class="docutils literal notranslate">v6.0.11 </code></td>
 <td><code class="docutils literal notranslate">v6.2.0 </code></td>
 <td><code class="docutils literal notranslate">v6.2.3 </code></td>
 <td><code class="docutils literal notranslate">v6.2.5 </code></td>
 <td><code class="docutils literal notranslate">v6.2.7 </code></td>
 <td><code class="docutils literal notranslate">v6.4.0 </code></td>
 <td><code class="docutils literal notranslate">v6.4.1 </code></td>
 <td><code class="docutils literal notranslate">v6.4.4 </code></td>
 <td><code class="docutils literal notranslate">v7.0.0 </code></td>
 <td><code class="docutils literal notranslate">v7.0.1 </code></td>
 <td><code class="docutils literal notranslate">v7.0.2 </code></td>
 <td><code class="docutils literal notranslate">v7.0.3 </code></td>
 <td><code class="docutils literal notranslate">v7.0.4 </code></td>
 <td><code class="docutils literal notranslate">v7.0.5 </code></td>
 </tr>
 <tr>
 <td>nat_ippool</td>
 <td>yes</td>
 <td>yes</td>
 <td>yes</td>
 <td>yes</td>
 <td>yes</td>
 <td>yes</td>
 <td>yes</td>
 <td>yes</td>
 <td>yes</td>
 <td>yes</td>
 <td>yes</td>
 <td>yes</td>
 <td>yes</td>
 <td>yes</td>
 <td>yes</td>
 <td>yes</td>
 </tr>
 </table>
 </div>
 </li>
            <ul class="ul-self">
            <li> <span class="li-head">name</span> - IP pool name. Source firewall.ippool.name. <span class="li-normal">type: str</span> <span class="li-required">required: true</span>
 <a id='label20' href="javascript:ContentClick('label21', 'label20');" onmouseover="ContentPreview('label21');" onmouseout="ContentUnpreview('label21');" title="click to collapse or expand..."> more... </a>
 <div id="label21" style="display:none">
 <table border="1">
 <tr>
 <td></td>
 <td><code class="docutils literal notranslate">v6.0.0 </code></td>
 <td><code class="docutils literal notranslate">v6.0.5 </code></td>
 <td><code class="docutils literal notranslate">v6.0.11 </code></td>
 <td><code class="docutils literal notranslate">v6.2.0 </code></td>
 <td><code class="docutils literal notranslate">v6.2.3 </code></td>
 <td><code class="docutils literal notranslate">v6.2.5 </code></td>
 <td><code class="docutils literal notranslate">v6.2.7 </code></td>
 <td><code class="docutils literal notranslate">v6.4.0 </code></td>
 <td><code class="docutils literal notranslate">v6.4.1 </code></td>
 <td><code class="docutils literal notranslate">v6.4.4 </code></td>
 <td><code class="docutils literal notranslate">v7.0.0 </code></td>
 <td><code class="docutils literal notranslate">v7.0.1 </code></td>
 <td><code class="docutils literal notranslate">v7.0.2 </code></td>
 <td><code class="docutils literal notranslate">v7.0.3 </code></td>
 <td><code class="docutils literal notranslate">v7.0.4 </code></td>
 <td><code class="docutils literal notranslate">v7.0.5 </code></td>
 </tr>
 <tr>
 <td>name</td>
 <td>yes</td>
 <td>yes</td>
 <td>yes</td>
 <td>yes</td>
 <td>yes</td>
 <td>yes</td>
 <td>yes</td>
 <td>yes</td>
 <td>yes</td>
 <td>yes</td>
 <td>yes</td>
 <td>yes</td>
 <td>yes</td>
 <td>yes</td>
 <td>yes</td>
 <td>yes</td>
 </tr>
 </table>
 </div>
 </li>
            </ul>
        <li> <span class="li-head">nat_ippool6</span> - IPv6 pools to be used for source NAT. <span class="li-normal">type: list</span> <span style="font-family:'Courier New'" class="li-required">member_path: nat_ippool6:name</span>
 <a id='label22' href="javascript:ContentClick('label23', 'label22');" onmouseover="ContentPreview('label23');" onmouseout="ContentUnpreview('label23');" title="click to collapse or expand..."> more... </a>
 <div id="label23" style="display:none">
 <table border="1">
 <tr>
 <td></td>
 <td><code class="docutils literal notranslate">v6.0.0 </code></td>
 <td><code class="docutils literal notranslate">v6.0.5 </code></td>
 <td><code class="docutils literal notranslate">v6.0.11 </code></td>
 <td><code class="docutils literal notranslate">v6.2.0 </code></td>
 <td><code class="docutils literal notranslate">v6.2.3 </code></td>
 <td><code class="docutils literal notranslate">v6.2.5 </code></td>
 <td><code class="docutils literal notranslate">v6.2.7 </code></td>
 <td><code class="docutils literal notranslate">v6.4.0 </code></td>
 <td><code class="docutils literal notranslate">v6.4.1 </code></td>
 <td><code class="docutils literal notranslate">v6.4.4 </code></td>
 <td><code class="docutils literal notranslate">v7.0.0 </code></td>
 <td><code class="docutils literal notranslate">v7.0.1 </code></td>
 <td><code class="docutils literal notranslate">v7.0.2 </code></td>
 <td><code class="docutils literal notranslate">v7.0.3 </code></td>
 <td><code class="docutils literal notranslate">v7.0.4 </code></td>
 <td><code class="docutils literal notranslate">v7.0.5 </code></td>
 </tr>
 <tr>
 <td>nat_ippool6</td>
 <td>no</td>
 <td>no</td>
 <td>no</td>
 <td>no</td>
 <td>no</td>
 <td>no</td>
 <td>no</td>
 <td>yes</td>
 <td>yes</td>
 <td>yes</td>
 <td>yes</td>
 <td>yes</td>
 <td>yes</td>
 <td>yes</td>
 <td>yes</td>
 <td>yes</td>
 </tr>
 </table>
 </div>
 </li>
            <ul class="ul-self">
            <li> <span class="li-head">name</span> - IPv6 pool name. Source firewall.ippool6.name. <span class="li-normal">type: str</span> <span class="li-required">required: true</span>
 <a id='label24' href="javascript:ContentClick('label25', 'label24');" onmouseover="ContentPreview('label25');" onmouseout="ContentUnpreview('label25');" title="click to collapse or expand..."> more... </a>
 <div id="label25" style="display:none">
 <table border="1">
 <tr>
 <td></td>
 <td><code class="docutils literal notranslate">v6.4.0 </code></td>
 <td><code class="docutils literal notranslate">v6.4.1 </code></td>
 <td><code class="docutils literal notranslate">v6.4.4 </code></td>
 <td><code class="docutils literal notranslate">v7.0.0 </code></td>
 <td><code class="docutils literal notranslate">v7.0.1 </code></td>
 <td><code class="docutils literal notranslate">v7.0.2 </code></td>
 <td><code class="docutils literal notranslate">v7.0.3 </code></td>
 <td><code class="docutils literal notranslate">v7.0.4 </code></td>
 <td><code class="docutils literal notranslate">v7.0.5 </code></td>
 </tr>
 <tr>
 <td>name</td>
 <td>yes</td>
 <td>yes</td>
 <td>yes</td>
 <td>yes</td>
 <td>yes</td>
 <td>yes</td>
 <td>yes</td>
 <td>yes</td>
 <td>yes</td>
 </tr>
 </table>
 </div>
 </li>
            </ul>
        <li> <span class="li-head">nat_port</span> - Translated port or port range (1 to 65535, 0 means any port). <span class="li-normal">type: str</span>
 <a id='label26' href="javascript:ContentClick('label27', 'label26');" onmouseover="ContentPreview('label27');" onmouseout="ContentUnpreview('label27');" title="click to collapse or expand..."> more... </a>
 <div id="label27" style="display:none">
 <table border="1">
 <tr>
 <td></td>
 <td><code class="docutils literal notranslate">v6.0.0 </code></td>
 <td><code class="docutils literal notranslate">v6.0.5 </code></td>
 <td><code class="docutils literal notranslate">v6.0.11 </code></td>
 <td><code class="docutils literal notranslate">v6.2.0 </code></td>
 <td><code class="docutils literal notranslate">v6.2.3 </code></td>
 <td><code class="docutils literal notranslate">v6.2.5 </code></td>
 <td><code class="docutils literal notranslate">v6.2.7 </code></td>
 <td><code class="docutils literal notranslate">v6.4.0 </code></td>
 <td><code class="docutils literal notranslate">v6.4.1 </code></td>
 <td><code class="docutils literal notranslate">v6.4.4 </code></td>
 <td><code class="docutils literal notranslate">v7.0.0 </code></td>
 <td><code class="docutils literal notranslate">v7.0.1 </code></td>
 <td><code class="docutils literal notranslate">v7.0.2 </code></td>
 <td><code class="docutils literal notranslate">v7.0.3 </code></td>
 <td><code class="docutils literal notranslate">v7.0.4 </code></td>
 <td><code class="docutils literal notranslate">v7.0.5 </code></td>
 </tr>
 <tr>
 <td>nat_port</td>
 <td>yes</td>
 <td>yes</td>
 <td>yes</td>
 <td>yes</td>
 <td>yes</td>
 <td>yes</td>
 <td>yes</td>
 <td>yes</td>
 <td>yes</td>
 <td>yes</td>
 <td>yes</td>
 <td>yes</td>
 <td>yes</td>
 <td>yes</td>
 <td>yes</td>
 <td>yes</td>
 </tr>
 </table>
 </div>
 </li>
        <li> <span class="li-head">nat46</span> - Enable/disable NAT46. <span class="li-normal">type: str</span> <span class="li-normal">choices: enable, disable</span>
 <a id='label28' href="javascript:ContentClick('label29', 'label28');" onmouseover="ContentPreview('label29');" onmouseout="ContentUnpreview('label29');" title="click to collapse or expand..."> more... </a>
 <div id="label29" style="display:none">
 <table border="1">
 <tr>
 <td></td>
 <td><code class="docutils literal notranslate">v6.0.0 </code></td>
 <td><code class="docutils literal notranslate">v6.0.5 </code></td>
 <td><code class="docutils literal notranslate">v6.0.11 </code></td>
 <td><code class="docutils literal notranslate">v6.2.0 </code></td>
 <td><code class="docutils literal notranslate">v6.2.3 </code></td>
 <td><code class="docutils literal notranslate">v6.2.5 </code></td>
 <td><code class="docutils literal notranslate">v6.2.7 </code></td>
 <td><code class="docutils literal notranslate">v6.4.0 </code></td>
 <td><code class="docutils literal notranslate">v6.4.1 </code></td>
 <td><code class="docutils literal notranslate">v6.4.4 </code></td>
 <td><code class="docutils literal notranslate">v7.0.0 </code></td>
 <td><code class="docutils literal notranslate">v7.0.1 </code></td>
 <td><code class="docutils literal notranslate">v7.0.2 </code></td>
 <td><code class="docutils literal notranslate">v7.0.3 </code></td>
 <td><code class="docutils literal notranslate">v7.0.4 </code></td>
 <td><code class="docutils literal notranslate">v7.0.5 </code></td>
 </tr>
 <tr>
 <td>nat46</td>
 <td>no</td>
 <td>no</td>
 <td>no</td>
 <td>no</td>
 <td>no</td>
 <td>no</td>
 <td>no</td>
 <td>no</td>
 <td>no</td>
 <td>no</td>
 <td>no</td>
 <td>yes</td>
 <td>yes</td>
 <td>yes</td>
 <td>yes</td>
 <td>yes</td>
 </tr>
 <tr>
 <td>[enable]</td>
 <td>n/a</td>
 <td>n/a</td>
 <td>n/a</td>
 <td>n/a</td>
 <td>n/a</td>
 <td>n/a</td>
 <td>n/a</td>
 <td>n/a</td>
 <td>n/a</td>
 <td>n/a</td>
 <td>n/a</td>
 <td>yes</td>
 <td>yes</td>
 <td>yes</td>
 <td>yes</td>
 <td>yes</td>
 </tr>
 <tr>
 <td>[disable]</td>
 <td>n/a</td>
 <td>n/a</td>
 <td>n/a</td>
 <td>n/a</td>
 <td>n/a</td>
 <td>n/a</td>
 <td>n/a</td>
 <td>n/a</td>
 <td>n/a</td>
 <td>n/a</td>
 <td>n/a</td>
 <td>yes</td>
 <td>yes</td>
 <td>yes</td>
 <td>yes</td>
 <td>yes</td>
 </tr>
 </table>
 </div>
 </li>
        <li> <span class="li-head">nat64</span> - Enable/disable NAT64. <span class="li-normal">type: str</span> <span class="li-normal">choices: enable, disable</span>
 <a id='label30' href="javascript:ContentClick('label31', 'label30');" onmouseover="ContentPreview('label31');" onmouseout="ContentUnpreview('label31');" title="click to collapse or expand..."> more... </a>
 <div id="label31" style="display:none">
 <table border="1">
 <tr>
 <td></td>
 <td><code class="docutils literal notranslate">v6.0.0 </code></td>
 <td><code class="docutils literal notranslate">v6.0.5 </code></td>
 <td><code class="docutils literal notranslate">v6.0.11 </code></td>
 <td><code class="docutils literal notranslate">v6.2.0 </code></td>
 <td><code class="docutils literal notranslate">v6.2.3 </code></td>
 <td><code class="docutils literal notranslate">v6.2.5 </code></td>
 <td><code class="docutils literal notranslate">v6.2.7 </code></td>
 <td><code class="docutils literal notranslate">v6.4.0 </code></td>
 <td><code class="docutils literal notranslate">v6.4.1 </code></td>
 <td><code class="docutils literal notranslate">v6.4.4 </code></td>
 <td><code class="docutils literal notranslate">v7.0.0 </code></td>
 <td><code class="docutils literal notranslate">v7.0.1 </code></td>
 <td><code class="docutils literal notranslate">v7.0.2 </code></td>
 <td><code class="docutils literal notranslate">v7.0.3 </code></td>
 <td><code class="docutils literal notranslate">v7.0.4 </code></td>
 <td><code class="docutils literal notranslate">v7.0.5 </code></td>
 </tr>
 <tr>
 <td>nat64</td>
 <td>no</td>
 <td>no</td>
 <td>no</td>
 <td>no</td>
 <td>no</td>
 <td>no</td>
 <td>no</td>
 <td>no</td>
 <td>no</td>
 <td>no</td>
 <td>no</td>
 <td>yes</td>
 <td>yes</td>
 <td>yes</td>
 <td>yes</td>
 <td>yes</td>
 </tr>
 <tr>
 <td>[enable]</td>
 <td>n/a</td>
 <td>n/a</td>
 <td>n/a</td>
 <td>n/a</td>
 <td>n/a</td>
 <td>n/a</td>
 <td>n/a</td>
 <td>n/a</td>
 <td>n/a</td>
 <td>n/a</td>
 <td>n/a</td>
 <td>yes</td>
 <td>yes</td>
 <td>yes</td>
 <td>yes</td>
 <td>yes</td>
 </tr>
 <tr>
 <td>[disable]</td>
 <td>n/a</td>
 <td>n/a</td>
 <td>n/a</td>
 <td>n/a</td>
 <td>n/a</td>
 <td>n/a</td>
 <td>n/a</td>
 <td>n/a</td>
 <td>n/a</td>
 <td>n/a</td>
 <td>n/a</td>
 <td>yes</td>
 <td>yes</td>
 <td>yes</td>
 <td>yes</td>
 <td>yes</td>
 </tr>
 </table>
 </div>
 </li>
        <li> <span class="li-head">orig_addr</span> - IPv4 Original address. <span class="li-normal">type: list</span> <span style="font-family:'Courier New'" class="li-required">member_path: orig_addr:name</span>
 <a id='label32' href="javascript:ContentClick('label33', 'label32');" onmouseover="ContentPreview('label33');" onmouseout="ContentUnpreview('label33');" title="click to collapse or expand..."> more... </a>
 <div id="label33" style="display:none">
 <table border="1">
 <tr>
 <td></td>
 <td><code class="docutils literal notranslate">v6.0.0 </code></td>
 <td><code class="docutils literal notranslate">v6.0.5 </code></td>
 <td><code class="docutils literal notranslate">v6.0.11 </code></td>
 <td><code class="docutils literal notranslate">v6.2.0 </code></td>
 <td><code class="docutils literal notranslate">v6.2.3 </code></td>
 <td><code class="docutils literal notranslate">v6.2.5 </code></td>
 <td><code class="docutils literal notranslate">v6.2.7 </code></td>
 <td><code class="docutils literal notranslate">v6.4.0 </code></td>
 <td><code class="docutils literal notranslate">v6.4.1 </code></td>
 <td><code class="docutils literal notranslate">v6.4.4 </code></td>
 <td><code class="docutils literal notranslate">v7.0.0 </code></td>
 <td><code class="docutils literal notranslate">v7.0.1 </code></td>
 <td><code class="docutils literal notranslate">v7.0.2 </code></td>
 <td><code class="docutils literal notranslate">v7.0.3 </code></td>
 <td><code class="docutils literal notranslate">v7.0.4 </code></td>
 <td><code class="docutils literal notranslate">v7.0.5 </code></td>
 </tr>
 <tr>
 <td>orig_addr</td>
 <td>yes</td>
 <td>yes</td>
 <td>yes</td>
 <td>yes</td>
 <td>yes</td>
 <td>yes</td>
 <td>yes</td>
 <td>yes</td>
 <td>yes</td>
 <td>yes</td>
 <td>yes</td>
 <td>yes</td>
 <td>yes</td>
 <td>yes</td>
 <td>yes</td>
 <td>yes</td>
 </tr>
 </table>
 </div>
 </li>
            <ul class="ul-self">
            <li> <span class="li-head">name</span> - Address name. Source firewall.address.name firewall.addrgrp.name. <span class="li-normal">type: str</span> <span class="li-required">required: true</span>
 <a id='label34' href="javascript:ContentClick('label35', 'label34');" onmouseover="ContentPreview('label35');" onmouseout="ContentUnpreview('label35');" title="click to collapse or expand..."> more... </a>
 <div id="label35" style="display:none">
 <table border="1">
 <tr>
 <td></td>
 <td><code class="docutils literal notranslate">v6.0.0 </code></td>
 <td><code class="docutils literal notranslate">v6.0.5 </code></td>
 <td><code class="docutils literal notranslate">v6.0.11 </code></td>
 <td><code class="docutils literal notranslate">v6.2.0 </code></td>
 <td><code class="docutils literal notranslate">v6.2.3 </code></td>
 <td><code class="docutils literal notranslate">v6.2.5 </code></td>
 <td><code class="docutils literal notranslate">v6.2.7 </code></td>
 <td><code class="docutils literal notranslate">v6.4.0 </code></td>
 <td><code class="docutils literal notranslate">v6.4.1 </code></td>
 <td><code class="docutils literal notranslate">v6.4.4 </code></td>
 <td><code class="docutils literal notranslate">v7.0.0 </code></td>
 <td><code class="docutils literal notranslate">v7.0.1 </code></td>
 <td><code class="docutils literal notranslate">v7.0.2 </code></td>
 <td><code class="docutils literal notranslate">v7.0.3 </code></td>
 <td><code class="docutils literal notranslate">v7.0.4 </code></td>
 <td><code class="docutils literal notranslate">v7.0.5 </code></td>
 </tr>
 <tr>
 <td>name</td>
 <td>yes</td>
 <td>yes</td>
 <td>yes</td>
 <td>yes</td>
 <td>yes</td>
 <td>yes</td>
 <td>yes</td>
 <td>yes</td>
 <td>yes</td>
 <td>yes</td>
 <td>yes</td>
 <td>yes</td>
 <td>yes</td>
 <td>yes</td>
 <td>yes</td>
 <td>yes</td>
 </tr>
 </table>
 </div>
 </li>
            </ul>
        <li> <span class="li-head">orig_addr6</span> - IPv6 Original address. <span class="li-normal">type: list</span> <span style="font-family:'Courier New'" class="li-required">member_path: orig_addr6:name</span>
 <a id='label36' href="javascript:ContentClick('label37', 'label36');" onmouseover="ContentPreview('label37');" onmouseout="ContentUnpreview('label37');" title="click to collapse or expand..."> more... </a>
 <div id="label37" style="display:none">
 <table border="1">
 <tr>
 <td></td>
 <td><code class="docutils literal notranslate">v6.0.0 </code></td>
 <td><code class="docutils literal notranslate">v6.0.5 </code></td>
 <td><code class="docutils literal notranslate">v6.0.11 </code></td>
 <td><code class="docutils literal notranslate">v6.2.0 </code></td>
 <td><code class="docutils literal notranslate">v6.2.3 </code></td>
 <td><code class="docutils literal notranslate">v6.2.5 </code></td>
 <td><code class="docutils literal notranslate">v6.2.7 </code></td>
 <td><code class="docutils literal notranslate">v6.4.0 </code></td>
 <td><code class="docutils literal notranslate">v6.4.1 </code></td>
 <td><code class="docutils literal notranslate">v6.4.4 </code></td>
 <td><code class="docutils literal notranslate">v7.0.0 </code></td>
 <td><code class="docutils literal notranslate">v7.0.1 </code></td>
 <td><code class="docutils literal notranslate">v7.0.2 </code></td>
 <td><code class="docutils literal notranslate">v7.0.3 </code></td>
 <td><code class="docutils literal notranslate">v7.0.4 </code></td>
 <td><code class="docutils literal notranslate">v7.0.5 </code></td>
 </tr>
 <tr>
 <td>orig_addr6</td>
 <td>no</td>
 <td>no</td>
 <td>no</td>
 <td>no</td>
 <td>no</td>
 <td>no</td>
 <td>no</td>
 <td>yes</td>
 <td>yes</td>
 <td>yes</td>
 <td>yes</td>
 <td>yes</td>
 <td>yes</td>
 <td>yes</td>
 <td>yes</td>
 <td>yes</td>
 </tr>
 </table>
 </div>
 </li>
            <ul class="ul-self">
            <li> <span class="li-head">name</span> - Address name. Source firewall.address6.name firewall.addrgrp6.name. <span class="li-normal">type: str</span> <span class="li-required">required: true</span>
 <a id='label38' href="javascript:ContentClick('label39', 'label38');" onmouseover="ContentPreview('label39');" onmouseout="ContentUnpreview('label39');" title="click to collapse or expand..."> more... </a>
 <div id="label39" style="display:none">
 <table border="1">
 <tr>
 <td></td>
 <td><code class="docutils literal notranslate">v6.4.0 </code></td>
 <td><code class="docutils literal notranslate">v6.4.1 </code></td>
 <td><code class="docutils literal notranslate">v6.4.4 </code></td>
 <td><code class="docutils literal notranslate">v7.0.0 </code></td>
 <td><code class="docutils literal notranslate">v7.0.1 </code></td>
 <td><code class="docutils literal notranslate">v7.0.2 </code></td>
 <td><code class="docutils literal notranslate">v7.0.3 </code></td>
 <td><code class="docutils literal notranslate">v7.0.4 </code></td>
 <td><code class="docutils literal notranslate">v7.0.5 </code></td>
 </tr>
 <tr>
 <td>name</td>
 <td>yes</td>
 <td>yes</td>
 <td>yes</td>
 <td>yes</td>
 <td>yes</td>
 <td>yes</td>
 <td>yes</td>
 <td>yes</td>
 <td>yes</td>
 </tr>
 </table>
 </div>
 </li>
            </ul>
        <li> <span class="li-head">orig_port</span> - Original TCP port (1 to 65535, 0 means any port). <span class="li-normal">type: str</span>
 <a id='label40' href="javascript:ContentClick('label41', 'label40');" onmouseover="ContentPreview('label41');" onmouseout="ContentUnpreview('label41');" title="click to collapse or expand..."> more... </a>
 <div id="label41" style="display:none">
 <table border="1">
 <tr>
 <td></td>
 <td><code class="docutils literal notranslate">v6.0.0 </code></td>
 <td><code class="docutils literal notranslate">v6.0.5 </code></td>
 <td><code class="docutils literal notranslate">v6.0.11 </code></td>
 <td><code class="docutils literal notranslate">v6.2.0 </code></td>
 <td><code class="docutils literal notranslate">v6.2.3 </code></td>
 <td><code class="docutils literal notranslate">v6.2.5 </code></td>
 <td><code class="docutils literal notranslate">v6.2.7 </code></td>
 <td><code class="docutils literal notranslate">v6.4.0 </code></td>
 <td><code class="docutils literal notranslate">v6.4.1 </code></td>
 <td><code class="docutils literal notranslate">v6.4.4 </code></td>
 <td><code class="docutils literal notranslate">v7.0.0 </code></td>
 <td><code class="docutils literal notranslate">v7.0.1 </code></td>
 <td><code class="docutils literal notranslate">v7.0.2 </code></td>
 <td><code class="docutils literal notranslate">v7.0.3 </code></td>
 <td><code class="docutils literal notranslate">v7.0.4 </code></td>
 <td><code class="docutils literal notranslate">v7.0.5 </code></td>
 </tr>
 <tr>
 <td>orig_port</td>
 <td>yes</td>
 <td>yes</td>
 <td>yes</td>
 <td>yes</td>
 <td>yes</td>
 <td>yes</td>
 <td>yes</td>
 <td>yes</td>
 <td>yes</td>
 <td>yes</td>
 <td>yes</td>
 <td>yes</td>
 <td>yes</td>
 <td>yes</td>
 <td>yes</td>
 <td>yes</td>
 </tr>
 </table>
 </div>
 </li>
        <li> <span class="li-head">policyid</span> - Policy ID. <span class="li-normal">type: int</span> <span class="li-required">required: true</span>
 <a id='label42' href="javascript:ContentClick('label43', 'label42');" onmouseover="ContentPreview('label43');" onmouseout="ContentUnpreview('label43');" title="click to collapse or expand..."> more... </a>
 <div id="label43" style="display:none">
 <table border="1">
 <tr>
 <td></td>
 <td><code class="docutils literal notranslate">v6.0.0 </code></td>
 <td><code class="docutils literal notranslate">v6.0.5 </code></td>
 <td><code class="docutils literal notranslate">v6.0.11 </code></td>
 <td><code class="docutils literal notranslate">v6.2.0 </code></td>
 <td><code class="docutils literal notranslate">v6.2.3 </code></td>
 <td><code class="docutils literal notranslate">v6.2.5 </code></td>
 <td><code class="docutils literal notranslate">v6.2.7 </code></td>
 <td><code class="docutils literal notranslate">v6.4.0 </code></td>
 <td><code class="docutils literal notranslate">v6.4.1 </code></td>
 <td><code class="docutils literal notranslate">v6.4.4 </code></td>
 <td><code class="docutils literal notranslate">v7.0.0 </code></td>
 <td><code class="docutils literal notranslate">v7.0.1 </code></td>
 <td><code class="docutils literal notranslate">v7.0.2 </code></td>
 <td><code class="docutils literal notranslate">v7.0.3 </code></td>
 <td><code class="docutils literal notranslate">v7.0.4 </code></td>
 <td><code class="docutils literal notranslate">v7.0.5 </code></td>
 </tr>
 <tr>
 <td>policyid</td>
 <td>yes</td>
 <td>yes</td>
 <td>yes</td>
 <td>yes</td>
 <td>yes</td>
 <td>yes</td>
 <td>yes</td>
 <td>yes</td>
 <td>yes</td>
 <td>yes</td>
 <td>yes</td>
 <td>yes</td>
 <td>yes</td>
 <td>yes</td>
 <td>yes</td>
 <td>yes</td>
 </tr>
 </table>
 </div>
 </li>
        <li> <span class="li-head">protocol</span> - Integer value for the protocol type (0 - 255). <span class="li-normal">type: int</span>
 <a id='label44' href="javascript:ContentClick('label45', 'label44');" onmouseover="ContentPreview('label45');" onmouseout="ContentUnpreview('label45');" title="click to collapse or expand..."> more... </a>
 <div id="label45" style="display:none">
 <table border="1">
 <tr>
 <td></td>
 <td><code class="docutils literal notranslate">v6.0.0 </code></td>
 <td><code class="docutils literal notranslate">v6.0.5 </code></td>
 <td><code class="docutils literal notranslate">v6.0.11 </code></td>
 <td><code class="docutils literal notranslate">v6.2.0 </code></td>
 <td><code class="docutils literal notranslate">v6.2.3 </code></td>
 <td><code class="docutils literal notranslate">v6.2.5 </code></td>
 <td><code class="docutils literal notranslate">v6.2.7 </code></td>
 <td><code class="docutils literal notranslate">v6.4.0 </code></td>
 <td><code class="docutils literal notranslate">v6.4.1 </code></td>
 <td><code class="docutils literal notranslate">v6.4.4 </code></td>
 <td><code class="docutils literal notranslate">v7.0.0 </code></td>
 <td><code class="docutils literal notranslate">v7.0.1 </code></td>
 <td><code class="docutils literal notranslate">v7.0.2 </code></td>
 <td><code class="docutils literal notranslate">v7.0.3 </code></td>
 <td><code class="docutils literal notranslate">v7.0.4 </code></td>
 <td><code class="docutils literal notranslate">v7.0.5 </code></td>
 </tr>
 <tr>
 <td>protocol</td>
 <td>yes</td>
 <td>yes</td>
 <td>yes</td>
 <td>yes</td>
 <td>yes</td>
 <td>yes</td>
 <td>yes</td>
 <td>yes</td>
 <td>yes</td>
 <td>yes</td>
 <td>yes</td>
 <td>yes</td>
 <td>yes</td>
 <td>yes</td>
 <td>yes</td>
 <td>yes</td>
 </tr>
 </table>
 </div>
 </li>
        <li> <span class="li-head">srcintf</span> - Source interface name from available interfaces. <span class="li-normal">type: list</span> <span style="font-family:'Courier New'" class="li-required">member_path: srcintf:name</span>
 <a id='label46' href="javascript:ContentClick('label47', 'label46');" onmouseover="ContentPreview('label47');" onmouseout="ContentUnpreview('label47');" title="click to collapse or expand..."> more... </a>
 <div id="label47" style="display:none">
 <table border="1">
 <tr>
 <td></td>
 <td><code class="docutils literal notranslate">v6.0.0 </code></td>
 <td><code class="docutils literal notranslate">v6.0.5 </code></td>
 <td><code class="docutils literal notranslate">v6.0.11 </code></td>
 <td><code class="docutils literal notranslate">v6.2.0 </code></td>
 <td><code class="docutils literal notranslate">v6.2.3 </code></td>
 <td><code class="docutils literal notranslate">v6.2.5 </code></td>
 <td><code class="docutils literal notranslate">v6.2.7 </code></td>
 <td><code class="docutils literal notranslate">v6.4.0 </code></td>
 <td><code class="docutils literal notranslate">v6.4.1 </code></td>
 <td><code class="docutils literal notranslate">v6.4.4 </code></td>
 <td><code class="docutils literal notranslate">v7.0.0 </code></td>
 <td><code class="docutils literal notranslate">v7.0.1 </code></td>
 <td><code class="docutils literal notranslate">v7.0.2 </code></td>
 <td><code class="docutils literal notranslate">v7.0.3 </code></td>
 <td><code class="docutils literal notranslate">v7.0.4 </code></td>
 <td><code class="docutils literal notranslate">v7.0.5 </code></td>
 </tr>
 <tr>
 <td>srcintf</td>
 <td>yes</td>
 <td>yes</td>
 <td>yes</td>
 <td>yes</td>
 <td>yes</td>
 <td>yes</td>
 <td>yes</td>
 <td>yes</td>
 <td>yes</td>
 <td>yes</td>
 <td>yes</td>
 <td>yes</td>
 <td>yes</td>
 <td>yes</td>
 <td>yes</td>
 <td>yes</td>
 </tr>
 </table>
 </div>
 </li>
            <ul class="ul-self">
            <li> <span class="li-head">name</span> - Interface name. Source system.interface.name system.zone.name. <span class="li-normal">type: str</span> <span class="li-required">required: true</span>
 <a id='label48' href="javascript:ContentClick('label49', 'label48');" onmouseover="ContentPreview('label49');" onmouseout="ContentUnpreview('label49');" title="click to collapse or expand..."> more... </a>
 <div id="label49" style="display:none">
 <table border="1">
 <tr>
 <td></td>
 <td><code class="docutils literal notranslate">v6.0.0 </code></td>
 <td><code class="docutils literal notranslate">v6.0.5 </code></td>
 <td><code class="docutils literal notranslate">v6.0.11 </code></td>
 <td><code class="docutils literal notranslate">v6.2.0 </code></td>
 <td><code class="docutils literal notranslate">v6.2.3 </code></td>
 <td><code class="docutils literal notranslate">v6.2.5 </code></td>
 <td><code class="docutils literal notranslate">v6.2.7 </code></td>
 <td><code class="docutils literal notranslate">v6.4.0 </code></td>
 <td><code class="docutils literal notranslate">v6.4.1 </code></td>
 <td><code class="docutils literal notranslate">v6.4.4 </code></td>
 <td><code class="docutils literal notranslate">v7.0.0 </code></td>
 <td><code class="docutils literal notranslate">v7.0.1 </code></td>
 <td><code class="docutils literal notranslate">v7.0.2 </code></td>
 <td><code class="docutils literal notranslate">v7.0.3 </code></td>
 <td><code class="docutils literal notranslate">v7.0.4 </code></td>
 <td><code class="docutils literal notranslate">v7.0.5 </code></td>
 </tr>
 <tr>
 <td>name</td>
 <td>yes</td>
 <td>yes</td>
 <td>yes</td>
 <td>yes</td>
 <td>yes</td>
 <td>yes</td>
 <td>yes</td>
 <td>yes</td>
 <td>yes</td>
 <td>yes</td>
 <td>yes</td>
 <td>yes</td>
 <td>yes</td>
 <td>yes</td>
 <td>yes</td>
 <td>yes</td>
 </tr>
 </table>
 </div>
 </li>
            </ul>
        <li> <span class="li-head">status</span> - Enable/disable the active status of this policy. <span class="li-normal">type: str</span> <span class="li-normal">choices: enable, disable</span>
 <a id='label50' href="javascript:ContentClick('label51', 'label50');" onmouseover="ContentPreview('label51');" onmouseout="ContentUnpreview('label51');" title="click to collapse or expand..."> more... </a>
 <div id="label51" style="display:none">
 <table border="1">
 <tr>
 <td></td>
 <td><code class="docutils literal notranslate">v6.0.0 </code></td>
 <td><code class="docutils literal notranslate">v6.0.5 </code></td>
 <td><code class="docutils literal notranslate">v6.0.11 </code></td>
 <td><code class="docutils literal notranslate">v6.2.0 </code></td>
 <td><code class="docutils literal notranslate">v6.2.3 </code></td>
 <td><code class="docutils literal notranslate">v6.2.5 </code></td>
 <td><code class="docutils literal notranslate">v6.2.7 </code></td>
 <td><code class="docutils literal notranslate">v6.4.0 </code></td>
 <td><code class="docutils literal notranslate">v6.4.1 </code></td>
 <td><code class="docutils literal notranslate">v6.4.4 </code></td>
 <td><code class="docutils literal notranslate">v7.0.0 </code></td>
 <td><code class="docutils literal notranslate">v7.0.1 </code></td>
 <td><code class="docutils literal notranslate">v7.0.2 </code></td>
 <td><code class="docutils literal notranslate">v7.0.3 </code></td>
 <td><code class="docutils literal notranslate">v7.0.4 </code></td>
 <td><code class="docutils literal notranslate">v7.0.5 </code></td>
 </tr>
 <tr>
 <td>status</td>
 <td>yes</td>
 <td>yes</td>
 <td>yes</td>
 <td>yes</td>
 <td>yes</td>
 <td>yes</td>
 <td>yes</td>
 <td>yes</td>
 <td>yes</td>
 <td>yes</td>
 <td>yes</td>
 <td>yes</td>
 <td>yes</td>
 <td>yes</td>
 <td>yes</td>
 <td>yes</td>
 </tr>
 <tr>
 <td>[enable]</td>
 <td>yes</td>
 <td>yes</td>
 <td>yes</td>
 <td>yes</td>
 <td>yes</td>
 <td>yes</td>
 <td>yes</td>
 <td>yes</td>
 <td>yes</td>
 <td>yes</td>
 <td>yes</td>
 <td>yes</td>
 <td>yes</td>
 <td>yes</td>
 <td>yes</td>
 <td>yes</td>
 </tr>
 <tr>
 <td>[disable]</td>
 <td>yes</td>
 <td>yes</td>
 <td>yes</td>
 <td>yes</td>
 <td>yes</td>
 <td>yes</td>
 <td>yes</td>
 <td>yes</td>
 <td>yes</td>
 <td>yes</td>
 <td>yes</td>
 <td>yes</td>
 <td>yes</td>
 <td>yes</td>
 <td>yes</td>
 <td>yes</td>
 </tr>
 </table>
 </div>
 </li>
        <li> <span class="li-head">type</span> - IPv4/IPv6 source NAT. <span class="li-normal">type: str</span> <span class="li-normal">choices: ipv4, ipv6</span>
 <a id='label52' href="javascript:ContentClick('label53', 'label52');" onmouseover="ContentPreview('label53');" onmouseout="ContentUnpreview('label53');" title="click to collapse or expand..."> more... </a>
 <div id="label53" style="display:none">
 <table border="1">
 <tr>
 <td></td>
 <td><code class="docutils literal notranslate">v6.0.0 </code></td>
 <td><code class="docutils literal notranslate">v6.0.5 </code></td>
 <td><code class="docutils literal notranslate">v6.0.11 </code></td>
 <td><code class="docutils literal notranslate">v6.2.0 </code></td>
 <td><code class="docutils literal notranslate">v6.2.3 </code></td>
 <td><code class="docutils literal notranslate">v6.2.5 </code></td>
 <td><code class="docutils literal notranslate">v6.2.7 </code></td>
 <td><code class="docutils literal notranslate">v6.4.0 </code></td>
 <td><code class="docutils literal notranslate">v6.4.1 </code></td>
 <td><code class="docutils literal notranslate">v6.4.4 </code></td>
 <td><code class="docutils literal notranslate">v7.0.0 </code></td>
 <td><code class="docutils literal notranslate">v7.0.1 </code></td>
 <td><code class="docutils literal notranslate">v7.0.2 </code></td>
 <td><code class="docutils literal notranslate">v7.0.3 </code></td>
 <td><code class="docutils literal notranslate">v7.0.4 </code></td>
 <td><code class="docutils literal notranslate">v7.0.5 </code></td>
 </tr>
 <tr>
 <td>type</td>
 <td>no</td>
 <td>no</td>
 <td>no</td>
 <td>no</td>
 <td>no</td>
 <td>no</td>
 <td>no</td>
 <td>yes</td>
 <td>yes</td>
 <td>yes</td>
 <td>yes</td>
 <td>yes</td>
 <td>yes</td>
 <td>yes</td>
 <td>yes</td>
 <td>yes</td>
 </tr>
 <tr>
 <td>[ipv4]</td>
 <td>n/a</td>
 <td>n/a</td>
 <td>n/a</td>
 <td>n/a</td>
 <td>n/a</td>
 <td>n/a</td>
 <td>n/a</td>
 <td>yes</td>
 <td>yes</td>
 <td>yes</td>
 <td>yes</td>
 <td>yes</td>
 <td>yes</td>
 <td>yes</td>
 <td>yes</td>
 <td>yes</td>
 </tr>
 <tr>
 <td>[ipv6]</td>
 <td>n/a</td>
 <td>n/a</td>
 <td>n/a</td>
 <td>n/a</td>
 <td>n/a</td>
 <td>n/a</td>
 <td>n/a</td>
 <td>yes</td>
 <td>yes</td>
 <td>yes</td>
 <td>yes</td>
 <td>yes</td>
 <td>yes</td>
 <td>yes</td>
 <td>yes</td>
 <td>yes</td>
 </tr>
 </table>
 </div>
 </li>
        <li> <span class="li-head">uuid</span> - Universally Unique Identifier (UUID; automatically assigned but can be manually reset). <span class="li-normal">type: str</span>
 <a id='label54' href="javascript:ContentClick('label55', 'label54');" onmouseover="ContentPreview('label55');" onmouseout="ContentUnpreview('label55');" title="click to collapse or expand..."> more... </a>
 <div id="label55" style="display:none">
 <table border="1">
 <tr>
 <td></td>
 <td><code class="docutils literal notranslate">v6.0.0 </code></td>
 <td><code class="docutils literal notranslate">v6.0.5 </code></td>
 <td><code class="docutils literal notranslate">v6.0.11 </code></td>
 <td><code class="docutils literal notranslate">v6.2.0 </code></td>
 <td><code class="docutils literal notranslate">v6.2.3 </code></td>
 <td><code class="docutils literal notranslate">v6.2.5 </code></td>
 <td><code class="docutils literal notranslate">v6.2.7 </code></td>
 <td><code class="docutils literal notranslate">v6.4.0 </code></td>
 <td><code class="docutils literal notranslate">v6.4.1 </code></td>
 <td><code class="docutils literal notranslate">v6.4.4 </code></td>
 <td><code class="docutils literal notranslate">v7.0.0 </code></td>
 <td><code class="docutils literal notranslate">v7.0.1 </code></td>
 <td><code class="docutils literal notranslate">v7.0.2 </code></td>
 <td><code class="docutils literal notranslate">v7.0.3 </code></td>
 <td><code class="docutils literal notranslate">v7.0.4 </code></td>
 <td><code class="docutils literal notranslate">v7.0.5 </code></td>
 </tr>
 <tr>
 <td>uuid</td>
 <td>no</td>
 <td>no</td>
 <td>no</td>
 <td>no</td>
 <td>no</td>
 <td>no</td>
 <td>no</td>
 <td>yes</td>
 <td>yes</td>
 <td>yes</td>
 <td>yes</td>
 <td>yes</td>
 <td>yes</td>
 <td>yes</td>
 <td>yes</td>
 <td>yes</td>
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

   - Adjust object order by moving self after(before) another.

   - Only one of [after, before] must be specified when action is moving an object.



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
      - name: Configure IPv4 and IPv6 central SNAT policies.
        fortios_firewall_central_snat_map:
          vdom:  "{{ vdom }}"
          state: "present"
          access_token: "<your_own_value>"
          firewall_central_snat_map:
            comments: "<your_own_value>"
            dst_addr:
             -
                name: "default_name_5 (source firewall.address.name firewall.addrgrp.name)"
            dst_addr6:
             -
                name: "default_name_7 (source firewall.address6.name firewall.addrgrp6.name)"
            dstintf:
             -
                name: "default_name_9 (source system.interface.name system.zone.name)"
            nat: "disable"
            nat_ippool:
             -
                name: "default_name_12 (source firewall.ippool.name)"
            nat_ippool6:
             -
                name: "default_name_14 (source firewall.ippool6.name)"
            nat_port: "<your_own_value>"
            nat46: "enable"
            nat64: "enable"
            orig_addr:
             -
                name: "default_name_19 (source firewall.address.name firewall.addrgrp.name)"
            orig_addr6:
             -
                name: "default_name_21 (source firewall.address6.name firewall.addrgrp6.name)"
            orig_port: "<your_own_value>"
            policyid: "23"
            protocol: "24"
            srcintf:
             -
                name: "default_name_26 (source system.interface.name system.zone.name)"
            status: "enable"
            type: "ipv4"
            uuid: "<your_own_value>"
    
      - name: move firewall.central_snat_map
        fortios_firewall_central_snat_map:
          vdom:  "root"
          action: "move"
          self: "<mkey of self identifier>"
          after: "<mkey of target identifier>"
         #before: "<mkey of target identifier>"
    


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
