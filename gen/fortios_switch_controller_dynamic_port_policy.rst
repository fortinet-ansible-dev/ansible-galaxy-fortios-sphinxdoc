:source: fortios_switch_controller_dynamic_port_policy.py

:orphan:

.. fortios_switch_controller_dynamic_port_policy:

fortios_switch_controller_dynamic_port_policy -- Configure Dynamic port policy to be applied on the managed FortiSwitch ports through DPP device in Fortinet's FortiOS and FortiGate.
+++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++

.. versionadded:: 2.0.0

.. contents::
   :local:
   :depth: 1


Synopsis
--------
- This module is able to configure a FortiGate or FortiOS (FOS) device by allowing the user to set and modify switch_controller feature and dynamic_port_policy category. Examples include all parameters and values need to be adjusted to datasources before usage. Tested with FOS v6.0.0



Requirements
------------
The below requirements are needed on the host that executes this module.

- ansible>=2.9


FortiOS Version Compatibility
-----------------------------


.. raw:: html

 <br>
 <table>
 <tr>
 <td></td>
 <td><code class="docutils literal notranslate">v7.0.0 </code></td>
 <td><code class="docutils literal notranslate">v7.0.1 </code></td>
 <td><code class="docutils literal notranslate">v7.0.2 </code></td>
 <td><code class="docutils literal notranslate">v7.0.3 </code></td>
 <td><code class="docutils literal notranslate">v7.0.4 </code></td>
 <td><code class="docutils literal notranslate">v7.0.5 </code></td>
 <td><code class="docutils literal notranslate">v7.0.6 </code></td>
 <td><code class="docutils literal notranslate">v7.0.7 </code></td>
 <td><code class="docutils literal notranslate">v7.0.8 </code></td>
 <td><code class="docutils literal notranslate">v7.2.0 </code></td>
 <td><code class="docutils literal notranslate">v7.2.1 </code></td>
 <td><code class="docutils literal notranslate">v7.2.2 </code></td>
 </tr>
 <tr>
 <td>fortios_switch_controller_dynamic_port_policy</td>
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
    <li> <span class="li-head">state</span> - Indicates whether to create or remove the object. <span class="li-normal">type: str</span> <span class="li-required">required: true</span> <span class="li-normal">choices: present, absent</span> </li>
    <li> <span class="li-head">switch_controller_dynamic_port_policy</span> - Configure Dynamic port policy to be applied on the managed FortiSwitch ports through DPP device. <span class="li-normal">type: dict</span>
 <a id='label0' href="javascript:ContentClick('label1', 'label0');" onmouseover="ContentPreview('label1');" onmouseout="ContentUnpreview('label1');" title="click to collapse or expand..."> more... </a>
 <div id="label1" style="display:none">
 <table border="1">
 <tr>
 <td></td>
 <td><code class="docutils literal notranslate">v7.0.0 </code></td>
 <td><code class="docutils literal notranslate">v7.0.1 </code></td>
 <td><code class="docutils literal notranslate">v7.0.2 </code></td>
 <td><code class="docutils literal notranslate">v7.0.3 </code></td>
 <td><code class="docutils literal notranslate">v7.0.4 </code></td>
 <td><code class="docutils literal notranslate">v7.0.5 </code></td>
 <td><code class="docutils literal notranslate">v7.0.6 </code></td>
 <td><code class="docutils literal notranslate">v7.0.7 </code></td>
 <td><code class="docutils literal notranslate">v7.0.8 </code></td>
 <td><code class="docutils literal notranslate">v7.2.0 </code></td>
 <td><code class="docutils literal notranslate">v7.2.1 </code></td>
 <td><code class="docutils literal notranslate">v7.2.2 </code></td>
 </tr>
 <tr>
 <td>switch_controller_dynamic_port_policy</td>
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
        <li> <span class="li-head">description</span> - Description for the Dynamic port policy. <span class="li-normal">type: str</span>
 <a id='label2' href="javascript:ContentClick('label3', 'label2');" onmouseover="ContentPreview('label3');" onmouseout="ContentUnpreview('label3');" title="click to collapse or expand..."> more... </a>
 <div id="label3" style="display:none">
 <table border="1">
 <tr>
 <td></td>
 <td><code class="docutils literal notranslate">v7.0.0 </code></td>
 <td><code class="docutils literal notranslate">v7.0.1 </code></td>
 <td><code class="docutils literal notranslate">v7.0.2 </code></td>
 <td><code class="docutils literal notranslate">v7.0.3 </code></td>
 <td><code class="docutils literal notranslate">v7.0.4 </code></td>
 <td><code class="docutils literal notranslate">v7.0.5 </code></td>
 <td><code class="docutils literal notranslate">v7.0.6 </code></td>
 <td><code class="docutils literal notranslate">v7.0.7 </code></td>
 <td><code class="docutils literal notranslate">v7.0.8 </code></td>
 <td><code class="docutils literal notranslate">v7.2.0 </code></td>
 <td><code class="docutils literal notranslate">v7.2.1 </code></td>
 <td><code class="docutils literal notranslate">v7.2.2 </code></td>
 </tr>
 <tr>
 <td>description</td>
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
        <li> <span class="li-head">fortilink</span> - FortiLink interface for which this Dynamic port policy belongs to. Source system.interface.name. <span class="li-normal">type: str</span>
 <a id='label4' href="javascript:ContentClick('label5', 'label4');" onmouseover="ContentPreview('label5');" onmouseout="ContentUnpreview('label5');" title="click to collapse or expand..."> more... </a>
 <div id="label5" style="display:none">
 <table border="1">
 <tr>
 <td></td>
 <td><code class="docutils literal notranslate">v7.0.0 </code></td>
 <td><code class="docutils literal notranslate">v7.0.1 </code></td>
 <td><code class="docutils literal notranslate">v7.0.2 </code></td>
 <td><code class="docutils literal notranslate">v7.0.3 </code></td>
 <td><code class="docutils literal notranslate">v7.0.4 </code></td>
 <td><code class="docutils literal notranslate">v7.0.5 </code></td>
 <td><code class="docutils literal notranslate">v7.0.6 </code></td>
 <td><code class="docutils literal notranslate">v7.0.7 </code></td>
 <td><code class="docutils literal notranslate">v7.0.8 </code></td>
 <td><code class="docutils literal notranslate">v7.2.0 </code></td>
 <td><code class="docutils literal notranslate">v7.2.1 </code></td>
 <td><code class="docutils literal notranslate">v7.2.2 </code></td>
 </tr>
 <tr>
 <td>fortilink</td>
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
        <li> <span class="li-head">name</span> - Dynamic port policy name. <span class="li-normal">type: str</span> <span class="li-required">required: true</span>
 <a id='label6' href="javascript:ContentClick('label7', 'label6');" onmouseover="ContentPreview('label7');" onmouseout="ContentUnpreview('label7');" title="click to collapse or expand..."> more... </a>
 <div id="label7" style="display:none">
 <table border="1">
 <tr>
 <td></td>
 <td><code class="docutils literal notranslate">v7.0.0 </code></td>
 <td><code class="docutils literal notranslate">v7.0.1 </code></td>
 <td><code class="docutils literal notranslate">v7.0.2 </code></td>
 <td><code class="docutils literal notranslate">v7.0.3 </code></td>
 <td><code class="docutils literal notranslate">v7.0.4 </code></td>
 <td><code class="docutils literal notranslate">v7.0.5 </code></td>
 <td><code class="docutils literal notranslate">v7.0.6 </code></td>
 <td><code class="docutils literal notranslate">v7.0.7 </code></td>
 <td><code class="docutils literal notranslate">v7.0.8 </code></td>
 <td><code class="docutils literal notranslate">v7.2.0 </code></td>
 <td><code class="docutils literal notranslate">v7.2.1 </code></td>
 <td><code class="docutils literal notranslate">v7.2.2 </code></td>
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
 </tr>
 </table>
 </div>
 </li>
        <li> <span class="li-head">policy</span> - Port policies with matching criteria and actions. <span class="li-normal">type: list</span>
 <a id='label8' href="javascript:ContentClick('label9', 'label8');" onmouseover="ContentPreview('label9');" onmouseout="ContentUnpreview('label9');" title="click to collapse or expand..."> more... </a>
 <div id="label9" style="display:none">
 <table border="1">
 <tr>
 <td></td>
 <td><code class="docutils literal notranslate">v7.0.0 </code></td>
 <td><code class="docutils literal notranslate">v7.0.1 </code></td>
 <td><code class="docutils literal notranslate">v7.0.2 </code></td>
 <td><code class="docutils literal notranslate">v7.0.3 </code></td>
 <td><code class="docutils literal notranslate">v7.0.4 </code></td>
 <td><code class="docutils literal notranslate">v7.0.5 </code></td>
 <td><code class="docutils literal notranslate">v7.0.6 </code></td>
 <td><code class="docutils literal notranslate">v7.0.7 </code></td>
 <td><code class="docutils literal notranslate">v7.0.8 </code></td>
 <td><code class="docutils literal notranslate">v7.2.0 </code></td>
 <td><code class="docutils literal notranslate">v7.2.1 </code></td>
 <td><code class="docutils literal notranslate">v7.2.2 </code></td>
 </tr>
 <tr>
 <td>policy</td>
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
            <li> <span class="li-head">802_1x</span> - 802.1x security policy to be applied when using this policy. Source switch-controller.security-policy.802-1X.name switch-controller.security-policy.captive-portal.name. <span class="li-normal">type: str</span>
 <a id='label10' href="javascript:ContentClick('label11', 'label10');" onmouseover="ContentPreview('label11');" onmouseout="ContentUnpreview('label11');" title="click to collapse or expand..."> more... </a>
 <div id="label11" style="display:none">
 <table border="1">
 <tr>
 <td></td>
 <td><code class="docutils literal notranslate">v7.0.0 </code></td>
 <td><code class="docutils literal notranslate">v7.0.1 </code></td>
 <td><code class="docutils literal notranslate">v7.0.2 </code></td>
 <td><code class="docutils literal notranslate">v7.0.3 </code></td>
 <td><code class="docutils literal notranslate">v7.0.4 </code></td>
 <td><code class="docutils literal notranslate">v7.0.5 </code></td>
 <td><code class="docutils literal notranslate">v7.0.6 </code></td>
 <td><code class="docutils literal notranslate">v7.0.7 </code></td>
 <td><code class="docutils literal notranslate">v7.0.8 </code></td>
 <td><code class="docutils literal notranslate">v7.2.0 </code></td>
 <td><code class="docutils literal notranslate">v7.2.1 </code></td>
 <td><code class="docutils literal notranslate">v7.2.2 </code></td>
 </tr>
 <tr>
 <td>802_1x</td>
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
            <li> <span class="li-head">bounce_port_link</span> - Enable/disable bouncing (administratively bring the link down, up) of a switch port where this policy is applied. Helps to clear and reassign VLAN from lldp-profile. <span class="li-normal">type: str</span> <span class="li-normal">choices: disable, enable</span>
 <a id='label12' href="javascript:ContentClick('label13', 'label12');" onmouseover="ContentPreview('label13');" onmouseout="ContentUnpreview('label13');" title="click to collapse or expand..."> more... </a>
 <div id="label13" style="display:none">
 <table border="1">
 <tr>
 <td></td>
 <td><code class="docutils literal notranslate">v7.0.0 </code></td>
 <td><code class="docutils literal notranslate">v7.0.1 </code></td>
 <td><code class="docutils literal notranslate">v7.0.2 </code></td>
 <td><code class="docutils literal notranslate">v7.0.3 </code></td>
 <td><code class="docutils literal notranslate">v7.0.4 </code></td>
 <td><code class="docutils literal notranslate">v7.0.5 </code></td>
 <td><code class="docutils literal notranslate">v7.0.6 </code></td>
 <td><code class="docutils literal notranslate">v7.0.7 </code></td>
 <td><code class="docutils literal notranslate">v7.0.8 </code></td>
 <td><code class="docutils literal notranslate">v7.2.0 </code></td>
 <td><code class="docutils literal notranslate">v7.2.1 </code></td>
 <td><code class="docutils literal notranslate">v7.2.2 </code></td>
 </tr>
 <tr>
 <td>bounce_port_link</td>
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
 </tr>
 </table>
 </div>
 </li>
            <li> <span class="li-head">category</span> - Category of Dynamic port policy. <span class="li-normal">type: str</span> <span class="li-normal">choices: device, interface-tag</span>
 <a id='label14' href="javascript:ContentClick('label15', 'label14');" onmouseover="ContentPreview('label15');" onmouseout="ContentUnpreview('label15');" title="click to collapse or expand..."> more... </a>
 <div id="label15" style="display:none">
 <table border="1">
 <tr>
 <td></td>
 <td><code class="docutils literal notranslate">v7.0.0 </code></td>
 <td><code class="docutils literal notranslate">v7.0.1 </code></td>
 <td><code class="docutils literal notranslate">v7.0.2 </code></td>
 <td><code class="docutils literal notranslate">v7.0.3 </code></td>
 <td><code class="docutils literal notranslate">v7.0.4 </code></td>
 <td><code class="docutils literal notranslate">v7.0.5 </code></td>
 <td><code class="docutils literal notranslate">v7.0.6 </code></td>
 <td><code class="docutils literal notranslate">v7.0.7 </code></td>
 <td><code class="docutils literal notranslate">v7.0.8 </code></td>
 <td><code class="docutils literal notranslate">v7.2.0 </code></td>
 <td><code class="docutils literal notranslate">v7.2.1 </code></td>
 <td><code class="docutils literal notranslate">v7.2.2 </code></td>
 </tr>
 <tr>
 <td>category</td>
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
 <td>[device]</td>
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
 <td>[interface-tag]</td>
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
            <li> <span class="li-head">description</span> - Description for the policy. <span class="li-normal">type: str</span>
 <a id='label16' href="javascript:ContentClick('label17', 'label16');" onmouseover="ContentPreview('label17');" onmouseout="ContentUnpreview('label17');" title="click to collapse or expand..."> more... </a>
 <div id="label17" style="display:none">
 <table border="1">
 <tr>
 <td></td>
 <td><code class="docutils literal notranslate">v7.0.0 </code></td>
 <td><code class="docutils literal notranslate">v7.0.1 </code></td>
 <td><code class="docutils literal notranslate">v7.0.2 </code></td>
 <td><code class="docutils literal notranslate">v7.0.3 </code></td>
 <td><code class="docutils literal notranslate">v7.0.4 </code></td>
 <td><code class="docutils literal notranslate">v7.0.5 </code></td>
 <td><code class="docutils literal notranslate">v7.0.6 </code></td>
 <td><code class="docutils literal notranslate">v7.0.7 </code></td>
 <td><code class="docutils literal notranslate">v7.0.8 </code></td>
 <td><code class="docutils literal notranslate">v7.2.0 </code></td>
 <td><code class="docutils literal notranslate">v7.2.1 </code></td>
 <td><code class="docutils literal notranslate">v7.2.2 </code></td>
 </tr>
 <tr>
 <td>description</td>
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
            <li> <span class="li-head">family</span> - Match policy based on family. <span class="li-normal">type: str</span>
 <a id='label18' href="javascript:ContentClick('label19', 'label18');" onmouseover="ContentPreview('label19');" onmouseout="ContentUnpreview('label19');" title="click to collapse or expand..."> more... </a>
 <div id="label19" style="display:none">
 <table border="1">
 <tr>
 <td></td>
 <td><code class="docutils literal notranslate">v7.0.0 </code></td>
 <td><code class="docutils literal notranslate">v7.0.1 </code></td>
 <td><code class="docutils literal notranslate">v7.0.2 </code></td>
 <td><code class="docutils literal notranslate">v7.0.3 </code></td>
 <td><code class="docutils literal notranslate">v7.0.4 </code></td>
 <td><code class="docutils literal notranslate">v7.0.5 </code></td>
 <td><code class="docutils literal notranslate">v7.0.6 </code></td>
 <td><code class="docutils literal notranslate">v7.0.7 </code></td>
 <td><code class="docutils literal notranslate">v7.0.8 </code></td>
 <td><code class="docutils literal notranslate">v7.2.0 </code></td>
 <td><code class="docutils literal notranslate">v7.2.1 </code></td>
 <td><code class="docutils literal notranslate">v7.2.2 </code></td>
 </tr>
 <tr>
 <td>family</td>
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
            <li> <span class="li-head">host</span> - Match policy based on host. <span class="li-normal">type: str</span>
 <a id='label20' href="javascript:ContentClick('label21', 'label20');" onmouseover="ContentPreview('label21');" onmouseout="ContentUnpreview('label21');" title="click to collapse or expand..."> more... </a>
 <div id="label21" style="display:none">
 <table border="1">
 <tr>
 <td></td>
 <td><code class="docutils literal notranslate">v7.0.0 </code></td>
 <td><code class="docutils literal notranslate">v7.0.1 </code></td>
 <td><code class="docutils literal notranslate">v7.0.2 </code></td>
 <td><code class="docutils literal notranslate">v7.0.3 </code></td>
 <td><code class="docutils literal notranslate">v7.0.4 </code></td>
 <td><code class="docutils literal notranslate">v7.0.5 </code></td>
 <td><code class="docutils literal notranslate">v7.0.6 </code></td>
 <td><code class="docutils literal notranslate">v7.0.7 </code></td>
 <td><code class="docutils literal notranslate">v7.0.8 </code></td>
 <td><code class="docutils literal notranslate">v7.2.0 </code></td>
 <td><code class="docutils literal notranslate">v7.2.1 </code></td>
 <td><code class="docutils literal notranslate">v7.2.2 </code></td>
 </tr>
 <tr>
 <td>host</td>
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
            <li> <span class="li-head">hw_vendor</span> - Match policy based on hardware vendor. <span class="li-normal">type: str</span>
 <a id='label22' href="javascript:ContentClick('label23', 'label22');" onmouseover="ContentPreview('label23');" onmouseout="ContentUnpreview('label23');" title="click to collapse or expand..."> more... </a>
 <div id="label23" style="display:none">
 <table border="1">
 <tr>
 <td></td>
 <td><code class="docutils literal notranslate">v7.0.0 </code></td>
 <td><code class="docutils literal notranslate">v7.0.1 </code></td>
 <td><code class="docutils literal notranslate">v7.0.2 </code></td>
 <td><code class="docutils literal notranslate">v7.0.3 </code></td>
 <td><code class="docutils literal notranslate">v7.0.4 </code></td>
 <td><code class="docutils literal notranslate">v7.0.5 </code></td>
 <td><code class="docutils literal notranslate">v7.0.6 </code></td>
 <td><code class="docutils literal notranslate">v7.0.7 </code></td>
 <td><code class="docutils literal notranslate">v7.0.8 </code></td>
 <td><code class="docutils literal notranslate">v7.2.0 </code></td>
 <td><code class="docutils literal notranslate">v7.2.1 </code></td>
 <td><code class="docutils literal notranslate">v7.2.2 </code></td>
 </tr>
 <tr>
 <td>hw_vendor</td>
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
 </tr>
 </table>
 </div>
 </li>
            <li> <span class="li-head">interface_tags</span> - Match policy based on the FortiSwitch interface object tags. <span class="li-normal">type: list</span>
 <a id='label24' href="javascript:ContentClick('label25', 'label24');" onmouseover="ContentPreview('label25');" onmouseout="ContentUnpreview('label25');" title="click to collapse or expand..."> more... </a>
 <div id="label25" style="display:none">
 <table border="1">
 <tr>
 <td></td>
 <td><code class="docutils literal notranslate">v7.0.0 </code></td>
 <td><code class="docutils literal notranslate">v7.0.1 </code></td>
 <td><code class="docutils literal notranslate">v7.0.2 </code></td>
 <td><code class="docutils literal notranslate">v7.0.3 </code></td>
 <td><code class="docutils literal notranslate">v7.0.4 </code></td>
 <td><code class="docutils literal notranslate">v7.0.5 </code></td>
 <td><code class="docutils literal notranslate">v7.0.6 </code></td>
 <td><code class="docutils literal notranslate">v7.0.7 </code></td>
 <td><code class="docutils literal notranslate">v7.0.8 </code></td>
 <td><code class="docutils literal notranslate">v7.2.0 </code></td>
 <td><code class="docutils literal notranslate">v7.2.1 </code></td>
 <td><code class="docutils literal notranslate">v7.2.2 </code></td>
 </tr>
 <tr>
 <td>interface_tags</td>
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
                <li> <span class="li-head">tag_name</span> - FortiSwitch port tag name. Source switch-controller.switch-interface-tag.name. <span class="li-normal">type: str</span>
 <a id='label26' href="javascript:ContentClick('label27', 'label26');" onmouseover="ContentPreview('label27');" onmouseout="ContentUnpreview('label27');" title="click to collapse or expand..."> more... </a>
 <div id="label27" style="display:none">
 <table border="1">
 <tr>
 <td></td>
 <td><code class="docutils literal notranslate">v7.0.0 </code></td>
 <td><code class="docutils literal notranslate">v7.0.1 </code></td>
 <td><code class="docutils literal notranslate">v7.0.2 </code></td>
 <td><code class="docutils literal notranslate">v7.0.3 </code></td>
 <td><code class="docutils literal notranslate">v7.0.4 </code></td>
 <td><code class="docutils literal notranslate">v7.0.5 </code></td>
 <td><code class="docutils literal notranslate">v7.0.6 </code></td>
 <td><code class="docutils literal notranslate">v7.0.7 </code></td>
 <td><code class="docutils literal notranslate">v7.0.8 </code></td>
 <td><code class="docutils literal notranslate">v7.2.0 </code></td>
 <td><code class="docutils literal notranslate">v7.2.1 </code></td>
 <td><code class="docutils literal notranslate">v7.2.2 </code></td>
 </tr>
 <tr>
 <td>tag_name</td>
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
            <li> <span class="li-head">lldp_profile</span> - LLDP profile to be applied when using this policy. Source switch-controller.lldp-profile.name. <span class="li-normal">type: str</span>
 <a id='label28' href="javascript:ContentClick('label29', 'label28');" onmouseover="ContentPreview('label29');" onmouseout="ContentUnpreview('label29');" title="click to collapse or expand..."> more... </a>
 <div id="label29" style="display:none">
 <table border="1">
 <tr>
 <td></td>
 <td><code class="docutils literal notranslate">v7.0.0 </code></td>
 <td><code class="docutils literal notranslate">v7.0.1 </code></td>
 <td><code class="docutils literal notranslate">v7.0.2 </code></td>
 <td><code class="docutils literal notranslate">v7.0.3 </code></td>
 <td><code class="docutils literal notranslate">v7.0.4 </code></td>
 <td><code class="docutils literal notranslate">v7.0.5 </code></td>
 <td><code class="docutils literal notranslate">v7.0.6 </code></td>
 <td><code class="docutils literal notranslate">v7.0.7 </code></td>
 <td><code class="docutils literal notranslate">v7.0.8 </code></td>
 <td><code class="docutils literal notranslate">v7.2.0 </code></td>
 <td><code class="docutils literal notranslate">v7.2.1 </code></td>
 <td><code class="docutils literal notranslate">v7.2.2 </code></td>
 </tr>
 <tr>
 <td>lldp_profile</td>
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
            <li> <span class="li-head">mac</span> - Match policy based on MAC address. <span class="li-normal">type: str</span>
 <a id='label30' href="javascript:ContentClick('label31', 'label30');" onmouseover="ContentPreview('label31');" onmouseout="ContentUnpreview('label31');" title="click to collapse or expand..."> more... </a>
 <div id="label31" style="display:none">
 <table border="1">
 <tr>
 <td></td>
 <td><code class="docutils literal notranslate">v7.0.0 </code></td>
 <td><code class="docutils literal notranslate">v7.0.1 </code></td>
 <td><code class="docutils literal notranslate">v7.0.2 </code></td>
 <td><code class="docutils literal notranslate">v7.0.3 </code></td>
 <td><code class="docutils literal notranslate">v7.0.4 </code></td>
 <td><code class="docutils literal notranslate">v7.0.5 </code></td>
 <td><code class="docutils literal notranslate">v7.0.6 </code></td>
 <td><code class="docutils literal notranslate">v7.0.7 </code></td>
 <td><code class="docutils literal notranslate">v7.0.8 </code></td>
 <td><code class="docutils literal notranslate">v7.2.0 </code></td>
 <td><code class="docutils literal notranslate">v7.2.1 </code></td>
 <td><code class="docutils literal notranslate">v7.2.2 </code></td>
 </tr>
 <tr>
 <td>mac</td>
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
            <li> <span class="li-head">name</span> - Policy name. <span class="li-normal">type: str</span>
 <a id='label32' href="javascript:ContentClick('label33', 'label32');" onmouseover="ContentPreview('label33');" onmouseout="ContentUnpreview('label33');" title="click to collapse or expand..."> more... </a>
 <div id="label33" style="display:none">
 <table border="1">
 <tr>
 <td></td>
 <td><code class="docutils literal notranslate">v7.0.0 </code></td>
 <td><code class="docutils literal notranslate">v7.0.1 </code></td>
 <td><code class="docutils literal notranslate">v7.0.2 </code></td>
 <td><code class="docutils literal notranslate">v7.0.3 </code></td>
 <td><code class="docutils literal notranslate">v7.0.4 </code></td>
 <td><code class="docutils literal notranslate">v7.0.5 </code></td>
 <td><code class="docutils literal notranslate">v7.0.6 </code></td>
 <td><code class="docutils literal notranslate">v7.0.7 </code></td>
 <td><code class="docutils literal notranslate">v7.0.8 </code></td>
 <td><code class="docutils literal notranslate">v7.2.0 </code></td>
 <td><code class="docutils literal notranslate">v7.2.1 </code></td>
 <td><code class="docutils literal notranslate">v7.2.2 </code></td>
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
 </tr>
 </table>
 </div>
 </li>
            <li> <span class="li-head">qos_policy</span> - QoS policy to be applied when using this policy. Source switch-controller.qos.qos-policy.name. <span class="li-normal">type: str</span>
 <a id='label34' href="javascript:ContentClick('label35', 'label34');" onmouseover="ContentPreview('label35');" onmouseout="ContentUnpreview('label35');" title="click to collapse or expand..."> more... </a>
 <div id="label35" style="display:none">
 <table border="1">
 <tr>
 <td></td>
 <td><code class="docutils literal notranslate">v7.0.0 </code></td>
 <td><code class="docutils literal notranslate">v7.0.1 </code></td>
 <td><code class="docutils literal notranslate">v7.0.2 </code></td>
 <td><code class="docutils literal notranslate">v7.0.3 </code></td>
 <td><code class="docutils literal notranslate">v7.0.4 </code></td>
 <td><code class="docutils literal notranslate">v7.0.5 </code></td>
 <td><code class="docutils literal notranslate">v7.0.6 </code></td>
 <td><code class="docutils literal notranslate">v7.0.7 </code></td>
 <td><code class="docutils literal notranslate">v7.0.8 </code></td>
 <td><code class="docutils literal notranslate">v7.2.0 </code></td>
 <td><code class="docutils literal notranslate">v7.2.1 </code></td>
 <td><code class="docutils literal notranslate">v7.2.2 </code></td>
 </tr>
 <tr>
 <td>qos_policy</td>
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
            <li> <span class="li-head">status</span> - Enable/disable policy. <span class="li-normal">type: str</span> <span class="li-normal">choices: enable, disable</span>
 <a id='label36' href="javascript:ContentClick('label37', 'label36');" onmouseover="ContentPreview('label37');" onmouseout="ContentUnpreview('label37');" title="click to collapse or expand..."> more... </a>
 <div id="label37" style="display:none">
 <table border="1">
 <tr>
 <td></td>
 <td><code class="docutils literal notranslate">v7.0.0 </code></td>
 <td><code class="docutils literal notranslate">v7.0.1 </code></td>
 <td><code class="docutils literal notranslate">v7.0.2 </code></td>
 <td><code class="docutils literal notranslate">v7.0.3 </code></td>
 <td><code class="docutils literal notranslate">v7.0.4 </code></td>
 <td><code class="docutils literal notranslate">v7.0.5 </code></td>
 <td><code class="docutils literal notranslate">v7.0.6 </code></td>
 <td><code class="docutils literal notranslate">v7.0.7 </code></td>
 <td><code class="docutils literal notranslate">v7.0.8 </code></td>
 <td><code class="docutils literal notranslate">v7.2.0 </code></td>
 <td><code class="docutils literal notranslate">v7.2.1 </code></td>
 <td><code class="docutils literal notranslate">v7.2.2 </code></td>
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
 </tr>
 </table>
 </div>
 </li>
            <li> <span class="li-head">type</span> - Match policy based on type. <span class="li-normal">type: str</span>
 <a id='label38' href="javascript:ContentClick('label39', 'label38');" onmouseover="ContentPreview('label39');" onmouseout="ContentUnpreview('label39');" title="click to collapse or expand..."> more... </a>
 <div id="label39" style="display:none">
 <table border="1">
 <tr>
 <td></td>
 <td><code class="docutils literal notranslate">v7.0.0 </code></td>
 <td><code class="docutils literal notranslate">v7.0.1 </code></td>
 <td><code class="docutils literal notranslate">v7.0.2 </code></td>
 <td><code class="docutils literal notranslate">v7.0.3 </code></td>
 <td><code class="docutils literal notranslate">v7.0.4 </code></td>
 <td><code class="docutils literal notranslate">v7.0.5 </code></td>
 <td><code class="docutils literal notranslate">v7.0.6 </code></td>
 <td><code class="docutils literal notranslate">v7.0.7 </code></td>
 <td><code class="docutils literal notranslate">v7.0.8 </code></td>
 <td><code class="docutils literal notranslate">v7.2.0 </code></td>
 <td><code class="docutils literal notranslate">v7.2.1 </code></td>
 <td><code class="docutils literal notranslate">v7.2.2 </code></td>
 </tr>
 <tr>
 <td>type</td>
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
            <li> <span class="li-head">vlan_policy</span> - VLAN policy to be applied when using this policy. Source switch-controller.vlan-policy.name. <span class="li-normal">type: str</span>
 <a id='label40' href="javascript:ContentClick('label41', 'label40');" onmouseover="ContentPreview('label41');" onmouseout="ContentUnpreview('label41');" title="click to collapse or expand..."> more... </a>
 <div id="label41" style="display:none">
 <table border="1">
 <tr>
 <td></td>
 <td><code class="docutils literal notranslate">v7.0.0 </code></td>
 <td><code class="docutils literal notranslate">v7.0.1 </code></td>
 <td><code class="docutils literal notranslate">v7.0.2 </code></td>
 <td><code class="docutils literal notranslate">v7.0.3 </code></td>
 <td><code class="docutils literal notranslate">v7.0.4 </code></td>
 <td><code class="docutils literal notranslate">v7.0.5 </code></td>
 <td><code class="docutils literal notranslate">v7.0.6 </code></td>
 <td><code class="docutils literal notranslate">v7.0.7 </code></td>
 <td><code class="docutils literal notranslate">v7.0.8 </code></td>
 <td><code class="docutils literal notranslate">v7.2.0 </code></td>
 <td><code class="docutils literal notranslate">v7.2.1 </code></td>
 <td><code class="docutils literal notranslate">v7.2.2 </code></td>
 </tr>
 <tr>
 <td>vlan_policy</td>
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
      - name: Configure Dynamic port policy to be applied on the managed FortiSwitch ports through DPP device.
        fortios_switch_controller_dynamic_port_policy:
          vdom:  "{{ vdom }}"
          state: "present"
          access_token: "<your_own_value>"
          switch_controller_dynamic_port_policy:
            description: "<your_own_value>"
            fortilink: "<your_own_value> (source system.interface.name)"
            name: "default_name_5"
            policy:
             -
                802_1x: "<your_own_value> (source switch-controller.security-policy.802-1X.name switch-controller.security-policy.captive-portal.name)"
                bounce_port_link: "disable"
                category: "device"
                description: "<your_own_value>"
                family: "<your_own_value>"
                host: "myhostname"
                hw_vendor: "<your_own_value>"
                interface_tags:
                 -
                    tag_name: "<your_own_value> (source switch-controller.switch-interface-tag.name)"
                lldp_profile: "<your_own_value> (source switch-controller.lldp-profile.name)"
                mac: "<your_own_value>"
                name: "default_name_18"
                qos_policy: "<your_own_value> (source switch-controller.qos.qos-policy.name)"
                status: "enable"
                type: "<your_own_value>"
                vlan_policy: "<your_own_value> (source switch-controller.vlan-policy.name)"
    


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
