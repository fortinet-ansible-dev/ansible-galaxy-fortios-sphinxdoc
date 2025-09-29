:source: fortios_extension_controller_extender_profile.py

:orphan:

.. fortios_extension_controller_extender_profile:

fortios_extension_controller_extender_profile -- FortiExtender extender profile configuration in Fortinet's FortiOS and FortiGate.
++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++

.. versionadded:: 2.0.0

.. contents::
   :local:
   :depth: 1


Synopsis
--------
- This module is able to configure a FortiGate or FortiOS (FOS) device by allowing the user to set and modify extension_controller feature and extender_profile category. Examples include all parameters and values need to be adjusted to datasources before usage. Tested with FOS v6.0.0



Requirements
------------
The below requirements are needed on the host that executes this module.

- ansible>=2.15


Tips
----
Using member operation to add an element to an existing object.

FortiOS Version Compatibility
-----------------------------
Supported Version Ranges: v7.2.1 -> v7.6.4


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
    <li> <span class="li-head">extension_controller_extender_profile</span> - FortiExtender extender profile configuration. <span class="li-normal">type: dict</span>
 <a id='label0' href="javascript:ContentClick('label1', 'label0');" onmouseover="ContentPreview('label1');" onmouseout="ContentUnpreview('label1');" title="click to collapse or expand..."> more... </a>
 <div id="label1" style="display:none">
 <table border="1">
 <tr>
 <td></td><td colspan="1">Supported Version Ranges</td>
 </tr>
 <tr>
 <td>extension_controller_extender_profile</td>
 <td><code class="docutils literal notranslate">v7.2.1 -> 7.6.4 </code></td>
 </tr>
 </table>
 </div>
 </li>
        <ul class="ul-self">
        <li> <span class="li-head">allowaccess</span> - Control management access to the managed extender. Separate entries with a space. <span class="li-normal">type: list</span> <span class="li-normal">choices: ping, telnet, http, https, ssh, snmp</span>
 <a id='label2' href="javascript:ContentClick('label3', 'label2');" onmouseover="ContentPreview('label3');" onmouseout="ContentUnpreview('label3');" title="click to collapse or expand..."> more... </a>
 <div id="label3" style="display:none">
 <table border="1">
 <tr>
 <td></td>
 <td colspan="1">Supported Version Ranges</td>
 </tr>
 <tr>
 <td>allowaccess</td>
 <td><code class="docutils literal notranslate">v7.2.1 -> 7.6.4 </code></td>
 </tr>
 <tr>
 <td>[ping]</td>
 <td><code class="docutils literal notranslate">v7.2.1 -> 7.6.4</code></td>
 <tr>
 <td>[telnet]</td>
 <td><code class="docutils literal notranslate">v7.2.1 -> 7.6.4</code></td>
 <tr>
 <td>[http]</td>
 <td><code class="docutils literal notranslate">v7.2.1 -> 7.6.4</code></td>
 <tr>
 <td>[https]</td>
 <td><code class="docutils literal notranslate">v7.2.1 -> 7.6.4</code></td>
 <tr>
 <td>[ssh]</td>
 <td><code class="docutils literal notranslate">v7.2.1 -> 7.6.4</code></td>
 <tr>
 <td>[snmp]</td>
 <td><code class="docutils literal notranslate">v7.2.1 -> 7.6.4</code></td>
 </table>
 </div>
 </li>
        <li> <span class="li-head">bandwidth_limit</span> - FortiExtender LAN extension bandwidth limit (Mbps). <span class="li-normal">type: int</span>
 <a id='label4' href="javascript:ContentClick('label5', 'label4');" onmouseover="ContentPreview('label5');" onmouseout="ContentUnpreview('label5');" title="click to collapse or expand..."> more... </a>
 <div id="label5" style="display:none">
 <table border="1">
 <tr>
 <td></td>
 <td colspan="1">Supported Version Ranges</td>
 </tr>
 <tr>
 <td>bandwidth_limit</td>
 <td><code class="docutils literal notranslate">v7.2.1 -> 7.6.4 </code></td>
 </tr>
 </table>
 </div>
 </li>
        <li> <span class="li-head">cellular</span> - FortiExtender cellular configuration. <span class="li-normal">type: dict</span>
 <a id='label6' href="javascript:ContentClick('label7', 'label6');" onmouseover="ContentPreview('label7');" onmouseout="ContentUnpreview('label7');" title="click to collapse or expand..."> more... </a>
 <div id="label7" style="display:none">
 <table border="1">
 <tr>
 <td></td><td colspan="1">Supported Version Ranges</td>
 </tr>
 <tr>
 <td>cellular</td>
 <td><code class="docutils literal notranslate">v7.2.1 -> 7.6.4 </code></td>
 </tr>
 </table>
 </div>
 </li>
            <ul class="ul-self">
            <li> <span class="li-head">controller_report</span> - FortiExtender controller report configuration. <span class="li-normal">type: dict</span>
 <a id='label8' href="javascript:ContentClick('label9', 'label8');" onmouseover="ContentPreview('label9');" onmouseout="ContentUnpreview('label9');" title="click to collapse or expand..."> more... </a>
 <div id="label9" style="display:none">
 <table border="1">
 <tr>
 <td></td><td colspan="1">Supported Version Ranges</td>
 </tr>
 <tr>
 <td>controller_report</td>
 <td><code class="docutils literal notranslate">v7.2.1 -> 7.6.4 </code></td>
 </tr>
 </table>
 </div>
 </li>
                <ul class="ul-self">
                <li> <span class="li-head">interval</span> - Controller report interval. <span class="li-normal">type: int</span>
 <a id='label10' href="javascript:ContentClick('label11', 'label10');" onmouseover="ContentPreview('label11');" onmouseout="ContentUnpreview('label11');" title="click to collapse or expand..."> more... </a>
 <div id="label11" style="display:none">
 <table border="1">
 <tr>
 <td></td>
 <td colspan="1">Supported Version Ranges</td>
 </tr>
 <tr>
 <td>interval</td>
 <td><code class="docutils literal notranslate">v7.2.1 -> 7.6.4 </code></td>
 </tr>
 </table>
 </div>
 </li>
                <li> <span class="li-head">signal_threshold</span> - Controller report signal threshold. <span class="li-normal">type: int</span>
 <a id='label12' href="javascript:ContentClick('label13', 'label12');" onmouseover="ContentPreview('label13');" onmouseout="ContentUnpreview('label13');" title="click to collapse or expand..."> more... </a>
 <div id="label13" style="display:none">
 <table border="1">
 <tr>
 <td></td>
 <td colspan="1">Supported Version Ranges</td>
 </tr>
 <tr>
 <td>signal_threshold</td>
 <td><code class="docutils literal notranslate">v7.2.1 -> 7.6.4 </code></td>
 </tr>
 </table>
 </div>
 </li>
                <li> <span class="li-head">status</span> - FortiExtender controller report status. <span class="li-normal">type: str</span> <span class="li-normal">choices: disable, enable</span>
 <a id='label14' href="javascript:ContentClick('label15', 'label14');" onmouseover="ContentPreview('label15');" onmouseout="ContentUnpreview('label15');" title="click to collapse or expand..."> more... </a>
 <div id="label15" style="display:none">
 <table border="1">
 <tr>
 <td></td>
 <td colspan="1">Supported Version Ranges</td>
 </tr>
 <tr>
 <td>status</td>
 <td><code class="docutils literal notranslate">v7.2.1 -> 7.6.4 </code></td>
 </tr>
 <tr>
 <td>[disable]</td>
 <td><code class="docutils literal notranslate">v7.2.1 -> 7.6.4</code></td>
 <tr>
 <td>[enable]</td>
 <td><code class="docutils literal notranslate">v7.2.1 -> 7.6.4</code></td>
 </table>
 </div>
 </li>
                </ul>
            <li> <span class="li-head">dataplan</span> - Dataplan names. <span class="li-normal">type: list</span> <span style="font-family:'Courier New'" class="li-required">member_path: cellular/dataplan:name</span>
 <a id='label16' href="javascript:ContentClick('label17', 'label16');" onmouseover="ContentPreview('label17');" onmouseout="ContentUnpreview('label17');" title="click to collapse or expand..."> more... </a>
 <div id="label17" style="display:none">
 <table border="1">
 <tr>
 <td></td><td colspan="1">Supported Version Ranges</td>
 </tr>
 <tr>
 <td>dataplan</td>
 <td><code class="docutils literal notranslate">v7.2.1 -> 7.6.4 </code></td>
 </tr>
 </table>
 </div>
 </li>
                <ul class="ul-self">
                <li> <span class="li-head">name</span> - Dataplan name. Source extension-controller.dataplan.name. <span class="li-normal">type: str</span> <span class="li-required">required: true</span>
 <a id='label18' href="javascript:ContentClick('label19', 'label18');" onmouseover="ContentPreview('label19');" onmouseout="ContentUnpreview('label19');" title="click to collapse or expand..."> more... </a>
 <div id="label19" style="display:none">
 <table border="1">
 <tr>
 <td></td>
 <td colspan="1">Supported Version Ranges</td>
 </tr>
 <tr>
 <td>name</td>
 <td><code class="docutils literal notranslate">v7.2.1 -> 7.6.4 </code></td>
 </tr>
 </table>
 </div>
 </li>
                </ul>
            <li> <span class="li-head">modem1</span> - Configuration options for modem 1. <span class="li-normal">type: dict</span>
 <a id='label20' href="javascript:ContentClick('label21', 'label20');" onmouseover="ContentPreview('label21');" onmouseout="ContentUnpreview('label21');" title="click to collapse or expand..."> more... </a>
 <div id="label21" style="display:none">
 <table border="1">
 <tr>
 <td></td><td colspan="1">Supported Version Ranges</td>
 </tr>
 <tr>
 <td>modem1</td>
 <td><code class="docutils literal notranslate">v7.2.1 -> 7.6.4 </code></td>
 </tr>
 </table>
 </div>
 </li>
                <ul class="ul-self">
                <li> <span class="li-head">auto_switch</span> - FortiExtender auto switch configuration. <span class="li-normal">type: dict</span>
 <a id='label22' href="javascript:ContentClick('label23', 'label22');" onmouseover="ContentPreview('label23');" onmouseout="ContentUnpreview('label23');" title="click to collapse or expand..."> more... </a>
 <div id="label23" style="display:none">
 <table border="1">
 <tr>
 <td></td><td colspan="1">Supported Version Ranges</td>
 </tr>
 <tr>
 <td>auto_switch</td>
 <td><code class="docutils literal notranslate">v7.2.1 -> 7.6.4 </code></td>
 </tr>
 </table>
 </div>
 </li>
                    <ul class="ul-self">
                    <li> <span class="li-head">dataplan</span> - Automatically switch based on data usage. <span class="li-normal">type: str</span> <span class="li-normal">choices: disable, enable</span>
 <a id='label24' href="javascript:ContentClick('label25', 'label24');" onmouseover="ContentPreview('label25');" onmouseout="ContentUnpreview('label25');" title="click to collapse or expand..."> more... </a>
 <div id="label25" style="display:none">
 <table border="1">
 <tr>
 <td></td>
 <td colspan="1">Supported Version Ranges</td>
 </tr>
 <tr>
 <td>dataplan</td>
 <td><code class="docutils literal notranslate">v7.2.1 -> 7.6.4 </code></td>
 </tr>
 <tr>
 <td>[disable]</td>
 <td><code class="docutils literal notranslate">v7.2.1 -> 7.6.4</code></td>
 <tr>
 <td>[enable]</td>
 <td><code class="docutils literal notranslate">v7.2.1 -> 7.6.4</code></td>
 </table>
 </div>
 </li>
                    <li> <span class="li-head">disconnect</span> - Auto switch by disconnect. <span class="li-normal">type: str</span> <span class="li-normal">choices: disable, enable</span>
 <a id='label26' href="javascript:ContentClick('label27', 'label26');" onmouseover="ContentPreview('label27');" onmouseout="ContentUnpreview('label27');" title="click to collapse or expand..."> more... </a>
 <div id="label27" style="display:none">
 <table border="1">
 <tr>
 <td></td>
 <td colspan="1">Supported Version Ranges</td>
 </tr>
 <tr>
 <td>disconnect</td>
 <td><code class="docutils literal notranslate">v7.2.1 -> 7.6.4 </code></td>
 </tr>
 <tr>
 <td>[disable]</td>
 <td><code class="docutils literal notranslate">v7.2.1 -> 7.6.4</code></td>
 <tr>
 <td>[enable]</td>
 <td><code class="docutils literal notranslate">v7.2.1 -> 7.6.4</code></td>
 </table>
 </div>
 </li>
                    <li> <span class="li-head">disconnect_period</span> - Automatically switch based on disconnect period. <span class="li-normal">type: int</span>
 <a id='label28' href="javascript:ContentClick('label29', 'label28');" onmouseover="ContentPreview('label29');" onmouseout="ContentUnpreview('label29');" title="click to collapse or expand..."> more... </a>
 <div id="label29" style="display:none">
 <table border="1">
 <tr>
 <td></td>
 <td colspan="1">Supported Version Ranges</td>
 </tr>
 <tr>
 <td>disconnect_period</td>
 <td><code class="docutils literal notranslate">v7.2.1 -> 7.6.4 </code></td>
 </tr>
 </table>
 </div>
 </li>
                    <li> <span class="li-head">disconnect_threshold</span> - Automatically switch based on disconnect threshold. <span class="li-normal">type: int</span>
 <a id='label30' href="javascript:ContentClick('label31', 'label30');" onmouseover="ContentPreview('label31');" onmouseout="ContentUnpreview('label31');" title="click to collapse or expand..."> more... </a>
 <div id="label31" style="display:none">
 <table border="1">
 <tr>
 <td></td>
 <td colspan="1">Supported Version Ranges</td>
 </tr>
 <tr>
 <td>disconnect_threshold</td>
 <td><code class="docutils literal notranslate">v7.2.1 -> 7.6.4 </code></td>
 </tr>
 </table>
 </div>
 </li>
                    <li> <span class="li-head">signal</span> - Automatically switch based on signal strength. <span class="li-normal">type: str</span> <span class="li-normal">choices: disable, enable</span>
 <a id='label32' href="javascript:ContentClick('label33', 'label32');" onmouseover="ContentPreview('label33');" onmouseout="ContentUnpreview('label33');" title="click to collapse or expand..."> more... </a>
 <div id="label33" style="display:none">
 <table border="1">
 <tr>
 <td></td>
 <td colspan="1">Supported Version Ranges</td>
 </tr>
 <tr>
 <td>signal</td>
 <td><code class="docutils literal notranslate">v7.2.1 -> 7.6.4 </code></td>
 </tr>
 <tr>
 <td>[disable]</td>
 <td><code class="docutils literal notranslate">v7.2.1 -> 7.6.4</code></td>
 <tr>
 <td>[enable]</td>
 <td><code class="docutils literal notranslate">v7.2.1 -> 7.6.4</code></td>
 </table>
 </div>
 </li>
                    <li> <span class="li-head">switch_back</span> - Auto switch with switch back multi-options. <span class="li-normal">type: list</span> <span class="li-normal">choices: time, timer</span>
 <a id='label34' href="javascript:ContentClick('label35', 'label34');" onmouseover="ContentPreview('label35');" onmouseout="ContentUnpreview('label35');" title="click to collapse or expand..."> more... </a>
 <div id="label35" style="display:none">
 <table border="1">
 <tr>
 <td></td>
 <td colspan="1">Supported Version Ranges</td>
 </tr>
 <tr>
 <td>switch_back</td>
 <td><code class="docutils literal notranslate">v7.2.1 -> 7.6.4 </code></td>
 </tr>
 <tr>
 <td>[time]</td>
 <td><code class="docutils literal notranslate">v7.2.1 -> 7.6.4</code></td>
 <tr>
 <td>[timer]</td>
 <td><code class="docutils literal notranslate">v7.2.1 -> 7.6.4</code></td>
 </table>
 </div>
 </li>
                    <li> <span class="li-head">switch_back_time</span> - Automatically switch over to preferred SIM/carrier at a specified time in UTC (HH:MM). <span class="li-normal">type: str</span>
 <a id='label36' href="javascript:ContentClick('label37', 'label36');" onmouseover="ContentPreview('label37');" onmouseout="ContentUnpreview('label37');" title="click to collapse or expand..."> more... </a>
 <div id="label37" style="display:none">
 <table border="1">
 <tr>
 <td></td>
 <td colspan="1">Supported Version Ranges</td>
 </tr>
 <tr>
 <td>switch_back_time</td>
 <td><code class="docutils literal notranslate">v7.2.1 -> 7.6.4 </code></td>
 </tr>
 </table>
 </div>
 </li>
                    <li> <span class="li-head">switch_back_timer</span> - Automatically switch over to preferred SIM/carrier after the given time (3600 - 2147483647 sec). <span class="li-normal">type: int</span>
 <a id='label38' href="javascript:ContentClick('label39', 'label38');" onmouseover="ContentPreview('label39');" onmouseout="ContentUnpreview('label39');" title="click to collapse or expand..."> more... </a>
 <div id="label39" style="display:none">
 <table border="1">
 <tr>
 <td></td>
 <td colspan="1">Supported Version Ranges</td>
 </tr>
 <tr>
 <td>switch_back_timer</td>
 <td><code class="docutils literal notranslate">v7.2.1 -> 7.6.4 </code></td>
 </tr>
 </table>
 </div>
 </li>
                    </ul>
                <li> <span class="li-head">default_sim</span> - Default SIM selection. <span class="li-normal">type: str</span> <span class="li-normal">choices: sim1, sim2, carrier, cost</span>
 <a id='label40' href="javascript:ContentClick('label41', 'label40');" onmouseover="ContentPreview('label41');" onmouseout="ContentUnpreview('label41');" title="click to collapse or expand..."> more... </a>
 <div id="label41" style="display:none">
 <table border="1">
 <tr>
 <td></td>
 <td colspan="1">Supported Version Ranges</td>
 </tr>
 <tr>
 <td>default_sim</td>
 <td><code class="docutils literal notranslate">v7.2.1 -> 7.6.4 </code></td>
 </tr>
 <tr>
 <td>[sim1]</td>
 <td><code class="docutils literal notranslate">v7.2.1 -> 7.6.4</code></td>
 <tr>
 <td>[sim2]</td>
 <td><code class="docutils literal notranslate">v7.2.1 -> 7.6.4</code></td>
 <tr>
 <td>[carrier]</td>
 <td><code class="docutils literal notranslate">v7.2.1 -> 7.6.4</code></td>
 <tr>
 <td>[cost]</td>
 <td><code class="docutils literal notranslate">v7.2.1 -> 7.6.4</code></td>
 </table>
 </div>
 </li>
                <li> <span class="li-head">gps</span> - FortiExtender GPS enable/disable. <span class="li-normal">type: str</span> <span class="li-normal">choices: disable, enable</span>
 <a id='label42' href="javascript:ContentClick('label43', 'label42');" onmouseover="ContentPreview('label43');" onmouseout="ContentUnpreview('label43');" title="click to collapse or expand..."> more... </a>
 <div id="label43" style="display:none">
 <table border="1">
 <tr>
 <td></td>
 <td colspan="1">Supported Version Ranges</td>
 </tr>
 <tr>
 <td>gps</td>
 <td><code class="docutils literal notranslate">v7.2.1 -> 7.6.4 </code></td>
 </tr>
 <tr>
 <td>[disable]</td>
 <td><code class="docutils literal notranslate">v7.2.1 -> 7.6.4</code></td>
 <tr>
 <td>[enable]</td>
 <td><code class="docutils literal notranslate">v7.2.1 -> 7.6.4</code></td>
 </table>
 </div>
 </li>
                <li> <span class="li-head">multiple_PDN</span> - Multiple-PDN enable/disable. <span class="li-normal">type: str</span> <span class="li-normal">choices: disable, enable</span>
 <a id='label44' href="javascript:ContentClick('label45', 'label44');" onmouseover="ContentPreview('label45');" onmouseout="ContentUnpreview('label45');" title="click to collapse or expand..."> more... </a>
 <div id="label45" style="display:none">
 <table border="1">
 <tr>
 <td></td>
 <td colspan="1">Supported Version Ranges</td>
 </tr>
 <tr>
 <td>multiple_PDN</td>
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
                <li> <span class="li-head">pdn1_dataplan</span> - PDN1-dataplan. Source extension-controller.dataplan.name. <span class="li-normal">type: str</span>
 <a id='label46' href="javascript:ContentClick('label47', 'label46');" onmouseover="ContentPreview('label47');" onmouseout="ContentUnpreview('label47');" title="click to collapse or expand..."> more... </a>
 <div id="label47" style="display:none">
 <table border="1">
 <tr>
 <td></td>
 <td colspan="1">Supported Version Ranges</td>
 </tr>
 <tr>
 <td>pdn1_dataplan</td>
 <td><code class="docutils literal notranslate">v7.6.1 -> 7.6.4 </code></td>
 </tr>
 </table>
 </div>
 </li>
                <li> <span class="li-head">pdn2_dataplan</span> - PDN2-dataplan. Source extension-controller.dataplan.name. <span class="li-normal">type: str</span>
 <a id='label48' href="javascript:ContentClick('label49', 'label48');" onmouseover="ContentPreview('label49');" onmouseout="ContentUnpreview('label49');" title="click to collapse or expand..."> more... </a>
 <div id="label49" style="display:none">
 <table border="1">
 <tr>
 <td></td>
 <td colspan="1">Supported Version Ranges</td>
 </tr>
 <tr>
 <td>pdn2_dataplan</td>
 <td><code class="docutils literal notranslate">v7.6.1 -> 7.6.4 </code></td>
 </tr>
 </table>
 </div>
 </li>
                <li> <span class="li-head">pdn3_dataplan</span> - PDN3-dataplan. Source extension-controller.dataplan.name. <span class="li-normal">type: str</span>
 <a id='label50' href="javascript:ContentClick('label51', 'label50');" onmouseover="ContentPreview('label51');" onmouseout="ContentUnpreview('label51');" title="click to collapse or expand..."> more... </a>
 <div id="label51" style="display:none">
 <table border="1">
 <tr>
 <td></td>
 <td colspan="1">Supported Version Ranges</td>
 </tr>
 <tr>
 <td>pdn3_dataplan</td>
 <td><code class="docutils literal notranslate">v7.6.1 -> 7.6.4 </code></td>
 </tr>
 </table>
 </div>
 </li>
                <li> <span class="li-head">pdn4_dataplan</span> - PDN4-dataplan. Source extension-controller.dataplan.name. <span class="li-normal">type: str</span>
 <a id='label52' href="javascript:ContentClick('label53', 'label52');" onmouseover="ContentPreview('label53');" onmouseout="ContentUnpreview('label53');" title="click to collapse or expand..."> more... </a>
 <div id="label53" style="display:none">
 <table border="1">
 <tr>
 <td></td>
 <td colspan="1">Supported Version Ranges</td>
 </tr>
 <tr>
 <td>pdn4_dataplan</td>
 <td><code class="docutils literal notranslate">v7.6.1 -> 7.6.4 </code></td>
 </tr>
 </table>
 </div>
 </li>
                <li> <span class="li-head">preferred_carrier</span> - Preferred carrier. <span class="li-normal">type: str</span>
 <a id='label54' href="javascript:ContentClick('label55', 'label54');" onmouseover="ContentPreview('label55');" onmouseout="ContentUnpreview('label55');" title="click to collapse or expand..."> more... </a>
 <div id="label55" style="display:none">
 <table border="1">
 <tr>
 <td></td>
 <td colspan="1">Supported Version Ranges</td>
 </tr>
 <tr>
 <td>preferred_carrier</td>
 <td><code class="docutils literal notranslate">v7.2.1 -> 7.6.4 </code></td>
 </tr>
 </table>
 </div>
 </li>
                <li> <span class="li-head">redundant_intf</span> - Redundant interface. <span class="li-normal">type: str</span>
 <a id='label56' href="javascript:ContentClick('label57', 'label56');" onmouseover="ContentPreview('label57');" onmouseout="ContentUnpreview('label57');" title="click to collapse or expand..."> more... </a>
 <div id="label57" style="display:none">
 <table border="1">
 <tr>
 <td></td>
 <td colspan="1">Supported Version Ranges</td>
 </tr>
 <tr>
 <td>redundant_intf</td>
 <td><code class="docutils literal notranslate">v7.2.1 -> 7.6.4 </code></td>
 </tr>
 </table>
 </div>
 </li>
                <li> <span class="li-head">redundant_mode</span> - FortiExtender mode. <span class="li-normal">type: str</span> <span class="li-normal">choices: disable, enable</span>
 <a id='label58' href="javascript:ContentClick('label59', 'label58');" onmouseover="ContentPreview('label59');" onmouseout="ContentUnpreview('label59');" title="click to collapse or expand..."> more... </a>
 <div id="label59" style="display:none">
 <table border="1">
 <tr>
 <td></td>
 <td colspan="1">Supported Version Ranges</td>
 </tr>
 <tr>
 <td>redundant_mode</td>
 <td><code class="docutils literal notranslate">v7.2.1 -> 7.6.4 </code></td>
 </tr>
 <tr>
 <td>[disable]</td>
 <td><code class="docutils literal notranslate">v7.2.1 -> 7.6.4</code></td>
 <tr>
 <td>[enable]</td>
 <td><code class="docutils literal notranslate">v7.2.1 -> 7.6.4</code></td>
 </table>
 </div>
 </li>
                <li> <span class="li-head">sim1_pin</span> - SIM <span class="li-normal">type: str</span> <span class="li-normal">choices: disable, enable</span>
 <a id='label60' href="javascript:ContentClick('label61', 'label60');" onmouseover="ContentPreview('label61');" onmouseout="ContentUnpreview('label61');" title="click to collapse or expand..."> more... </a>
 <div id="label61" style="display:none">
 <table border="1">
 <tr>
 <td></td>
 <td colspan="1">Supported Version Ranges</td>
 </tr>
 <tr>
 <td>sim1_pin</td>
 <td><code class="docutils literal notranslate">v7.2.1 -> 7.6.4 </code></td>
 </tr>
 <tr>
 <td>[disable]</td>
 <td><code class="docutils literal notranslate">v7.2.1 -> 7.6.4</code></td>
 <tr>
 <td>[enable]</td>
 <td><code class="docutils literal notranslate">v7.2.1 -> 7.6.4</code></td>
 </table>
 </div>
 </li>
                <li> <span class="li-head">sim1_pin_code</span> - SIM <span class="li-normal">type: str</span>
 <a id='label62' href="javascript:ContentClick('label63', 'label62');" onmouseover="ContentPreview('label63');" onmouseout="ContentUnpreview('label63');" title="click to collapse or expand..."> more... </a>
 <div id="label63" style="display:none">
 <table border="1">
 <tr>
 <td></td>
 <td colspan="1">Supported Version Ranges</td>
 </tr>
 <tr>
 <td>sim1_pin_code</td>
 <td><code class="docutils literal notranslate">v7.2.1 -> 7.6.4 </code></td>
 </tr>
 </table>
 </div>
 </li>
                <li> <span class="li-head">sim2_pin</span> - SIM <span class="li-normal">type: str</span> <span class="li-normal">choices: disable, enable</span>
 <a id='label64' href="javascript:ContentClick('label65', 'label64');" onmouseover="ContentPreview('label65');" onmouseout="ContentUnpreview('label65');" title="click to collapse or expand..."> more... </a>
 <div id="label65" style="display:none">
 <table border="1">
 <tr>
 <td></td>
 <td colspan="1">Supported Version Ranges</td>
 </tr>
 <tr>
 <td>sim2_pin</td>
 <td><code class="docutils literal notranslate">v7.2.1 -> 7.6.4 </code></td>
 </tr>
 <tr>
 <td>[disable]</td>
 <td><code class="docutils literal notranslate">v7.2.1 -> 7.6.4</code></td>
 <tr>
 <td>[enable]</td>
 <td><code class="docutils literal notranslate">v7.2.1 -> 7.6.4</code></td>
 </table>
 </div>
 </li>
                <li> <span class="li-head">sim2_pin_code</span> - SIM <span class="li-normal">type: str</span>
 <a id='label66' href="javascript:ContentClick('label67', 'label66');" onmouseover="ContentPreview('label67');" onmouseout="ContentUnpreview('label67');" title="click to collapse or expand..."> more... </a>
 <div id="label67" style="display:none">
 <table border="1">
 <tr>
 <td></td>
 <td colspan="1">Supported Version Ranges</td>
 </tr>
 <tr>
 <td>sim2_pin_code</td>
 <td><code class="docutils literal notranslate">v7.2.1 -> 7.6.4 </code></td>
 </tr>
 </table>
 </div>
 </li>
                </ul>
            <li> <span class="li-head">modem2</span> - Configuration options for modem 2. <span class="li-normal">type: dict</span>
 <a id='label68' href="javascript:ContentClick('label69', 'label68');" onmouseover="ContentPreview('label69');" onmouseout="ContentUnpreview('label69');" title="click to collapse or expand..."> more... </a>
 <div id="label69" style="display:none">
 <table border="1">
 <tr>
 <td></td><td colspan="1">Supported Version Ranges</td>
 </tr>
 <tr>
 <td>modem2</td>
 <td><code class="docutils literal notranslate">v7.2.1 -> 7.6.4 </code></td>
 </tr>
 </table>
 </div>
 </li>
                <ul class="ul-self">
                <li> <span class="li-head">auto_switch</span> - FortiExtender auto switch configuration. <span class="li-normal">type: dict</span>
 <a id='label70' href="javascript:ContentClick('label71', 'label70');" onmouseover="ContentPreview('label71');" onmouseout="ContentUnpreview('label71');" title="click to collapse or expand..."> more... </a>
 <div id="label71" style="display:none">
 <table border="1">
 <tr>
 <td></td><td colspan="1">Supported Version Ranges</td>
 </tr>
 <tr>
 <td>auto_switch</td>
 <td><code class="docutils literal notranslate">v7.2.1 -> 7.6.4 </code></td>
 </tr>
 </table>
 </div>
 </li>
                    <ul class="ul-self">
                    <li> <span class="li-head">dataplan</span> - Automatically switch based on data usage. <span class="li-normal">type: str</span> <span class="li-normal">choices: disable, enable</span>
 <a id='label72' href="javascript:ContentClick('label73', 'label72');" onmouseover="ContentPreview('label73');" onmouseout="ContentUnpreview('label73');" title="click to collapse or expand..."> more... </a>
 <div id="label73" style="display:none">
 <table border="1">
 <tr>
 <td></td>
 <td colspan="1">Supported Version Ranges</td>
 </tr>
 <tr>
 <td>dataplan</td>
 <td><code class="docutils literal notranslate">v7.2.1 -> 7.6.4 </code></td>
 </tr>
 <tr>
 <td>[disable]</td>
 <td><code class="docutils literal notranslate">v7.2.1 -> 7.6.4</code></td>
 <tr>
 <td>[enable]</td>
 <td><code class="docutils literal notranslate">v7.2.1 -> 7.6.4</code></td>
 </table>
 </div>
 </li>
                    <li> <span class="li-head">disconnect</span> - Auto switch by disconnect. <span class="li-normal">type: str</span> <span class="li-normal">choices: disable, enable</span>
 <a id='label74' href="javascript:ContentClick('label75', 'label74');" onmouseover="ContentPreview('label75');" onmouseout="ContentUnpreview('label75');" title="click to collapse or expand..."> more... </a>
 <div id="label75" style="display:none">
 <table border="1">
 <tr>
 <td></td>
 <td colspan="1">Supported Version Ranges</td>
 </tr>
 <tr>
 <td>disconnect</td>
 <td><code class="docutils literal notranslate">v7.2.1 -> 7.6.4 </code></td>
 </tr>
 <tr>
 <td>[disable]</td>
 <td><code class="docutils literal notranslate">v7.2.1 -> 7.6.4</code></td>
 <tr>
 <td>[enable]</td>
 <td><code class="docutils literal notranslate">v7.2.1 -> 7.6.4</code></td>
 </table>
 </div>
 </li>
                    <li> <span class="li-head">disconnect_period</span> - Automatically switch based on disconnect period. <span class="li-normal">type: int</span>
 <a id='label76' href="javascript:ContentClick('label77', 'label76');" onmouseover="ContentPreview('label77');" onmouseout="ContentUnpreview('label77');" title="click to collapse or expand..."> more... </a>
 <div id="label77" style="display:none">
 <table border="1">
 <tr>
 <td></td>
 <td colspan="1">Supported Version Ranges</td>
 </tr>
 <tr>
 <td>disconnect_period</td>
 <td><code class="docutils literal notranslate">v7.2.1 -> 7.6.4 </code></td>
 </tr>
 </table>
 </div>
 </li>
                    <li> <span class="li-head">disconnect_threshold</span> - Automatically switch based on disconnect threshold. <span class="li-normal">type: int</span>
 <a id='label78' href="javascript:ContentClick('label79', 'label78');" onmouseover="ContentPreview('label79');" onmouseout="ContentUnpreview('label79');" title="click to collapse or expand..."> more... </a>
 <div id="label79" style="display:none">
 <table border="1">
 <tr>
 <td></td>
 <td colspan="1">Supported Version Ranges</td>
 </tr>
 <tr>
 <td>disconnect_threshold</td>
 <td><code class="docutils literal notranslate">v7.2.1 -> 7.6.4 </code></td>
 </tr>
 </table>
 </div>
 </li>
                    <li> <span class="li-head">signal</span> - Automatically switch based on signal strength. <span class="li-normal">type: str</span> <span class="li-normal">choices: disable, enable</span>
 <a id='label80' href="javascript:ContentClick('label81', 'label80');" onmouseover="ContentPreview('label81');" onmouseout="ContentUnpreview('label81');" title="click to collapse or expand..."> more... </a>
 <div id="label81" style="display:none">
 <table border="1">
 <tr>
 <td></td>
 <td colspan="1">Supported Version Ranges</td>
 </tr>
 <tr>
 <td>signal</td>
 <td><code class="docutils literal notranslate">v7.2.1 -> 7.6.4 </code></td>
 </tr>
 <tr>
 <td>[disable]</td>
 <td><code class="docutils literal notranslate">v7.2.1 -> 7.6.4</code></td>
 <tr>
 <td>[enable]</td>
 <td><code class="docutils literal notranslate">v7.2.1 -> 7.6.4</code></td>
 </table>
 </div>
 </li>
                    <li> <span class="li-head">switch_back</span> - Auto switch with switch back multi-options. <span class="li-normal">type: list</span> <span class="li-normal">choices: time, timer</span>
 <a id='label82' href="javascript:ContentClick('label83', 'label82');" onmouseover="ContentPreview('label83');" onmouseout="ContentUnpreview('label83');" title="click to collapse or expand..."> more... </a>
 <div id="label83" style="display:none">
 <table border="1">
 <tr>
 <td></td>
 <td colspan="1">Supported Version Ranges</td>
 </tr>
 <tr>
 <td>switch_back</td>
 <td><code class="docutils literal notranslate">v7.2.1 -> 7.6.4 </code></td>
 </tr>
 <tr>
 <td>[time]</td>
 <td><code class="docutils literal notranslate">v7.2.1 -> 7.6.4</code></td>
 <tr>
 <td>[timer]</td>
 <td><code class="docutils literal notranslate">v7.2.1 -> 7.6.4</code></td>
 </table>
 </div>
 </li>
                    <li> <span class="li-head">switch_back_time</span> - Automatically switch over to preferred SIM/carrier at a specified time in UTC (HH:MM). <span class="li-normal">type: str</span>
 <a id='label84' href="javascript:ContentClick('label85', 'label84');" onmouseover="ContentPreview('label85');" onmouseout="ContentUnpreview('label85');" title="click to collapse or expand..."> more... </a>
 <div id="label85" style="display:none">
 <table border="1">
 <tr>
 <td></td>
 <td colspan="1">Supported Version Ranges</td>
 </tr>
 <tr>
 <td>switch_back_time</td>
 <td><code class="docutils literal notranslate">v7.2.1 -> 7.6.4 </code></td>
 </tr>
 </table>
 </div>
 </li>
                    <li> <span class="li-head">switch_back_timer</span> - Automatically switch over to preferred SIM/carrier after the given time (3600 - 2147483647 sec). <span class="li-normal">type: int</span>
 <a id='label86' href="javascript:ContentClick('label87', 'label86');" onmouseover="ContentPreview('label87');" onmouseout="ContentUnpreview('label87');" title="click to collapse or expand..."> more... </a>
 <div id="label87" style="display:none">
 <table border="1">
 <tr>
 <td></td>
 <td colspan="1">Supported Version Ranges</td>
 </tr>
 <tr>
 <td>switch_back_timer</td>
 <td><code class="docutils literal notranslate">v7.2.1 -> 7.6.4 </code></td>
 </tr>
 </table>
 </div>
 </li>
                    </ul>
                <li> <span class="li-head">default_sim</span> - Default SIM selection. <span class="li-normal">type: str</span> <span class="li-normal">choices: sim1, sim2, carrier, cost</span>
 <a id='label88' href="javascript:ContentClick('label89', 'label88');" onmouseover="ContentPreview('label89');" onmouseout="ContentUnpreview('label89');" title="click to collapse or expand..."> more... </a>
 <div id="label89" style="display:none">
 <table border="1">
 <tr>
 <td></td>
 <td colspan="1">Supported Version Ranges</td>
 </tr>
 <tr>
 <td>default_sim</td>
 <td><code class="docutils literal notranslate">v7.2.1 -> 7.6.4 </code></td>
 </tr>
 <tr>
 <td>[sim1]</td>
 <td><code class="docutils literal notranslate">v7.2.1 -> 7.6.4</code></td>
 <tr>
 <td>[sim2]</td>
 <td><code class="docutils literal notranslate">v7.2.1 -> 7.6.4</code></td>
 <tr>
 <td>[carrier]</td>
 <td><code class="docutils literal notranslate">v7.2.1 -> 7.6.4</code></td>
 <tr>
 <td>[cost]</td>
 <td><code class="docutils literal notranslate">v7.2.1 -> 7.6.4</code></td>
 </table>
 </div>
 </li>
                <li> <span class="li-head">gps</span> - FortiExtender GPS enable/disable. <span class="li-normal">type: str</span> <span class="li-normal">choices: disable, enable</span>
 <a id='label90' href="javascript:ContentClick('label91', 'label90');" onmouseover="ContentPreview('label91');" onmouseout="ContentUnpreview('label91');" title="click to collapse or expand..."> more... </a>
 <div id="label91" style="display:none">
 <table border="1">
 <tr>
 <td></td>
 <td colspan="1">Supported Version Ranges</td>
 </tr>
 <tr>
 <td>gps</td>
 <td><code class="docutils literal notranslate">v7.2.1 -> 7.6.4 </code></td>
 </tr>
 <tr>
 <td>[disable]</td>
 <td><code class="docutils literal notranslate">v7.2.1 -> 7.6.4</code></td>
 <tr>
 <td>[enable]</td>
 <td><code class="docutils literal notranslate">v7.2.1 -> 7.6.4</code></td>
 </table>
 </div>
 </li>
                <li> <span class="li-head">multiple_PDN</span> - Multiple-PDN enable/disable. <span class="li-normal">type: str</span> <span class="li-normal">choices: disable, enable</span>
 <a id='label92' href="javascript:ContentClick('label93', 'label92');" onmouseover="ContentPreview('label93');" onmouseout="ContentUnpreview('label93');" title="click to collapse or expand..."> more... </a>
 <div id="label93" style="display:none">
 <table border="1">
 <tr>
 <td></td>
 <td colspan="1">Supported Version Ranges</td>
 </tr>
 <tr>
 <td>multiple_PDN</td>
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
                <li> <span class="li-head">pdn1_dataplan</span> - PDN1-dataplan. Source extension-controller.dataplan.name. <span class="li-normal">type: str</span>
 <a id='label94' href="javascript:ContentClick('label95', 'label94');" onmouseover="ContentPreview('label95');" onmouseout="ContentUnpreview('label95');" title="click to collapse or expand..."> more... </a>
 <div id="label95" style="display:none">
 <table border="1">
 <tr>
 <td></td>
 <td colspan="1">Supported Version Ranges</td>
 </tr>
 <tr>
 <td>pdn1_dataplan</td>
 <td><code class="docutils literal notranslate">v7.6.1 -> 7.6.4 </code></td>
 </tr>
 </table>
 </div>
 </li>
                <li> <span class="li-head">pdn2_dataplan</span> - PDN2-dataplan. Source extension-controller.dataplan.name. <span class="li-normal">type: str</span>
 <a id='label96' href="javascript:ContentClick('label97', 'label96');" onmouseover="ContentPreview('label97');" onmouseout="ContentUnpreview('label97');" title="click to collapse or expand..."> more... </a>
 <div id="label97" style="display:none">
 <table border="1">
 <tr>
 <td></td>
 <td colspan="1">Supported Version Ranges</td>
 </tr>
 <tr>
 <td>pdn2_dataplan</td>
 <td><code class="docutils literal notranslate">v7.6.1 -> 7.6.4 </code></td>
 </tr>
 </table>
 </div>
 </li>
                <li> <span class="li-head">pdn3_dataplan</span> - PDN3-dataplan. Source extension-controller.dataplan.name. <span class="li-normal">type: str</span>
 <a id='label98' href="javascript:ContentClick('label99', 'label98');" onmouseover="ContentPreview('label99');" onmouseout="ContentUnpreview('label99');" title="click to collapse or expand..."> more... </a>
 <div id="label99" style="display:none">
 <table border="1">
 <tr>
 <td></td>
 <td colspan="1">Supported Version Ranges</td>
 </tr>
 <tr>
 <td>pdn3_dataplan</td>
 <td><code class="docutils literal notranslate">v7.6.1 -> 7.6.4 </code></td>
 </tr>
 </table>
 </div>
 </li>
                <li> <span class="li-head">pdn4_dataplan</span> - PDN4-dataplan. Source extension-controller.dataplan.name. <span class="li-normal">type: str</span>
 <a id='label100' href="javascript:ContentClick('label101', 'label100');" onmouseover="ContentPreview('label101');" onmouseout="ContentUnpreview('label101');" title="click to collapse or expand..."> more... </a>
 <div id="label101" style="display:none">
 <table border="1">
 <tr>
 <td></td>
 <td colspan="1">Supported Version Ranges</td>
 </tr>
 <tr>
 <td>pdn4_dataplan</td>
 <td><code class="docutils literal notranslate">v7.6.1 -> 7.6.4 </code></td>
 </tr>
 </table>
 </div>
 </li>
                <li> <span class="li-head">preferred_carrier</span> - Preferred carrier. <span class="li-normal">type: str</span>
 <a id='label102' href="javascript:ContentClick('label103', 'label102');" onmouseover="ContentPreview('label103');" onmouseout="ContentUnpreview('label103');" title="click to collapse or expand..."> more... </a>
 <div id="label103" style="display:none">
 <table border="1">
 <tr>
 <td></td>
 <td colspan="1">Supported Version Ranges</td>
 </tr>
 <tr>
 <td>preferred_carrier</td>
 <td><code class="docutils literal notranslate">v7.2.1 -> 7.6.4 </code></td>
 </tr>
 </table>
 </div>
 </li>
                <li> <span class="li-head">redundant_intf</span> - Redundant interface. <span class="li-normal">type: str</span>
 <a id='label104' href="javascript:ContentClick('label105', 'label104');" onmouseover="ContentPreview('label105');" onmouseout="ContentUnpreview('label105');" title="click to collapse or expand..."> more... </a>
 <div id="label105" style="display:none">
 <table border="1">
 <tr>
 <td></td>
 <td colspan="1">Supported Version Ranges</td>
 </tr>
 <tr>
 <td>redundant_intf</td>
 <td><code class="docutils literal notranslate">v7.2.1 -> 7.6.4 </code></td>
 </tr>
 </table>
 </div>
 </li>
                <li> <span class="li-head">redundant_mode</span> - FortiExtender mode. <span class="li-normal">type: str</span> <span class="li-normal">choices: disable, enable</span>
 <a id='label106' href="javascript:ContentClick('label107', 'label106');" onmouseover="ContentPreview('label107');" onmouseout="ContentUnpreview('label107');" title="click to collapse or expand..."> more... </a>
 <div id="label107" style="display:none">
 <table border="1">
 <tr>
 <td></td>
 <td colspan="1">Supported Version Ranges</td>
 </tr>
 <tr>
 <td>redundant_mode</td>
 <td><code class="docutils literal notranslate">v7.2.1 -> 7.6.4 </code></td>
 </tr>
 <tr>
 <td>[disable]</td>
 <td><code class="docutils literal notranslate">v7.2.1 -> 7.6.4</code></td>
 <tr>
 <td>[enable]</td>
 <td><code class="docutils literal notranslate">v7.2.1 -> 7.6.4</code></td>
 </table>
 </div>
 </li>
                <li> <span class="li-head">sim1_pin</span> - SIM <span class="li-normal">type: str</span> <span class="li-normal">choices: disable, enable</span>
 <a id='label108' href="javascript:ContentClick('label109', 'label108');" onmouseover="ContentPreview('label109');" onmouseout="ContentUnpreview('label109');" title="click to collapse or expand..."> more... </a>
 <div id="label109" style="display:none">
 <table border="1">
 <tr>
 <td></td>
 <td colspan="1">Supported Version Ranges</td>
 </tr>
 <tr>
 <td>sim1_pin</td>
 <td><code class="docutils literal notranslate">v7.2.1 -> 7.6.4 </code></td>
 </tr>
 <tr>
 <td>[disable]</td>
 <td><code class="docutils literal notranslate">v7.2.1 -> 7.6.4</code></td>
 <tr>
 <td>[enable]</td>
 <td><code class="docutils literal notranslate">v7.2.1 -> 7.6.4</code></td>
 </table>
 </div>
 </li>
                <li> <span class="li-head">sim1_pin_code</span> - SIM <span class="li-normal">type: str</span>
 <a id='label110' href="javascript:ContentClick('label111', 'label110');" onmouseover="ContentPreview('label111');" onmouseout="ContentUnpreview('label111');" title="click to collapse or expand..."> more... </a>
 <div id="label111" style="display:none">
 <table border="1">
 <tr>
 <td></td>
 <td colspan="1">Supported Version Ranges</td>
 </tr>
 <tr>
 <td>sim1_pin_code</td>
 <td><code class="docutils literal notranslate">v7.2.1 -> 7.6.4 </code></td>
 </tr>
 </table>
 </div>
 </li>
                <li> <span class="li-head">sim2_pin</span> - SIM <span class="li-normal">type: str</span> <span class="li-normal">choices: disable, enable</span>
 <a id='label112' href="javascript:ContentClick('label113', 'label112');" onmouseover="ContentPreview('label113');" onmouseout="ContentUnpreview('label113');" title="click to collapse or expand..."> more... </a>
 <div id="label113" style="display:none">
 <table border="1">
 <tr>
 <td></td>
 <td colspan="1">Supported Version Ranges</td>
 </tr>
 <tr>
 <td>sim2_pin</td>
 <td><code class="docutils literal notranslate">v7.2.1 -> 7.6.4 </code></td>
 </tr>
 <tr>
 <td>[disable]</td>
 <td><code class="docutils literal notranslate">v7.2.1 -> 7.6.4</code></td>
 <tr>
 <td>[enable]</td>
 <td><code class="docutils literal notranslate">v7.2.1 -> 7.6.4</code></td>
 </table>
 </div>
 </li>
                <li> <span class="li-head">sim2_pin_code</span> - SIM <span class="li-normal">type: str</span>
 <a id='label114' href="javascript:ContentClick('label115', 'label114');" onmouseover="ContentPreview('label115');" onmouseout="ContentUnpreview('label115');" title="click to collapse or expand..."> more... </a>
 <div id="label115" style="display:none">
 <table border="1">
 <tr>
 <td></td>
 <td colspan="1">Supported Version Ranges</td>
 </tr>
 <tr>
 <td>sim2_pin_code</td>
 <td><code class="docutils literal notranslate">v7.2.1 -> 7.6.4 </code></td>
 </tr>
 </table>
 </div>
 </li>
                </ul>
            <li> <span class="li-head">sms_notification</span> - FortiExtender cellular SMS notification configuration. <span class="li-normal">type: dict</span>
 <a id='label116' href="javascript:ContentClick('label117', 'label116');" onmouseover="ContentPreview('label117');" onmouseout="ContentUnpreview('label117');" title="click to collapse or expand..."> more... </a>
 <div id="label117" style="display:none">
 <table border="1">
 <tr>
 <td></td><td colspan="1">Supported Version Ranges</td>
 </tr>
 <tr>
 <td>sms_notification</td>
 <td><code class="docutils literal notranslate">v7.2.1 -> 7.6.4 </code></td>
 </tr>
 </table>
 </div>
 </li>
                <ul class="ul-self">
                <li> <span class="li-head">alert</span> - SMS alert list. <span class="li-normal">type: dict</span>
 <a id='label118' href="javascript:ContentClick('label119', 'label118');" onmouseover="ContentPreview('label119');" onmouseout="ContentUnpreview('label119');" title="click to collapse or expand..."> more... </a>
 <div id="label119" style="display:none">
 <table border="1">
 <tr>
 <td></td><td colspan="1">Supported Version Ranges</td>
 </tr>
 <tr>
 <td>alert</td>
 <td><code class="docutils literal notranslate">v7.2.1 -> 7.6.4 </code></td>
 </tr>
 </table>
 </div>
 </li>
                    <ul class="ul-self">
                    <li> <span class="li-head">data_exhausted</span> - Display string when data exhausted. <span class="li-normal">type: str</span>
 <a id='label120' href="javascript:ContentClick('label121', 'label120');" onmouseover="ContentPreview('label121');" onmouseout="ContentUnpreview('label121');" title="click to collapse or expand..."> more... </a>
 <div id="label121" style="display:none">
 <table border="1">
 <tr>
 <td></td>
 <td colspan="1">Supported Version Ranges</td>
 </tr>
 <tr>
 <td>data_exhausted</td>
 <td><code class="docutils literal notranslate">v7.2.1 -> 7.6.4 </code></td>
 </tr>
 </table>
 </div>
 </li>
                    <li> <span class="li-head">fgt_backup_mode_switch</span> - Display string when FortiGate backup mode switched. <span class="li-normal">type: str</span>
 <a id='label122' href="javascript:ContentClick('label123', 'label122');" onmouseover="ContentPreview('label123');" onmouseout="ContentUnpreview('label123');" title="click to collapse or expand..."> more... </a>
 <div id="label123" style="display:none">
 <table border="1">
 <tr>
 <td></td>
 <td colspan="1">Supported Version Ranges</td>
 </tr>
 <tr>
 <td>fgt_backup_mode_switch</td>
 <td><code class="docutils literal notranslate">v7.2.1 -> 7.6.4 </code></td>
 </tr>
 </table>
 </div>
 </li>
                    <li> <span class="li-head">low_signal_strength</span> - Display string when signal strength is low. <span class="li-normal">type: str</span>
 <a id='label124' href="javascript:ContentClick('label125', 'label124');" onmouseover="ContentPreview('label125');" onmouseout="ContentUnpreview('label125');" title="click to collapse or expand..."> more... </a>
 <div id="label125" style="display:none">
 <table border="1">
 <tr>
 <td></td>
 <td colspan="1">Supported Version Ranges</td>
 </tr>
 <tr>
 <td>low_signal_strength</td>
 <td><code class="docutils literal notranslate">v7.2.1 -> 7.6.4 </code></td>
 </tr>
 </table>
 </div>
 </li>
                    <li> <span class="li-head">mode_switch</span> - Display string when mode is switched. <span class="li-normal">type: str</span>
 <a id='label126' href="javascript:ContentClick('label127', 'label126');" onmouseover="ContentPreview('label127');" onmouseout="ContentUnpreview('label127');" title="click to collapse or expand..."> more... </a>
 <div id="label127" style="display:none">
 <table border="1">
 <tr>
 <td></td>
 <td colspan="1">Supported Version Ranges</td>
 </tr>
 <tr>
 <td>mode_switch</td>
 <td><code class="docutils literal notranslate">v7.2.1 -> 7.6.4 </code></td>
 </tr>
 </table>
 </div>
 </li>
                    <li> <span class="li-head">os_image_fallback</span> - Display string when falling back to a previous OS image. <span class="li-normal">type: str</span>
 <a id='label128' href="javascript:ContentClick('label129', 'label128');" onmouseover="ContentPreview('label129');" onmouseout="ContentUnpreview('label129');" title="click to collapse or expand..."> more... </a>
 <div id="label129" style="display:none">
 <table border="1">
 <tr>
 <td></td>
 <td colspan="1">Supported Version Ranges</td>
 </tr>
 <tr>
 <td>os_image_fallback</td>
 <td><code class="docutils literal notranslate">v7.2.1 -> 7.6.4 </code></td>
 </tr>
 </table>
 </div>
 </li>
                    <li> <span class="li-head">session_disconnect</span> - Display string when session disconnected. <span class="li-normal">type: str</span>
 <a id='label130' href="javascript:ContentClick('label131', 'label130');" onmouseover="ContentPreview('label131');" onmouseout="ContentUnpreview('label131');" title="click to collapse or expand..."> more... </a>
 <div id="label131" style="display:none">
 <table border="1">
 <tr>
 <td></td>
 <td colspan="1">Supported Version Ranges</td>
 </tr>
 <tr>
 <td>session_disconnect</td>
 <td><code class="docutils literal notranslate">v7.2.1 -> 7.6.4 </code></td>
 </tr>
 </table>
 </div>
 </li>
                    <li> <span class="li-head">system_reboot</span> - Display string when system rebooted. <span class="li-normal">type: str</span>
 <a id='label132' href="javascript:ContentClick('label133', 'label132');" onmouseover="ContentPreview('label133');" onmouseout="ContentUnpreview('label133');" title="click to collapse or expand..."> more... </a>
 <div id="label133" style="display:none">
 <table border="1">
 <tr>
 <td></td>
 <td colspan="1">Supported Version Ranges</td>
 </tr>
 <tr>
 <td>system_reboot</td>
 <td><code class="docutils literal notranslate">v7.2.1 -> 7.6.4 </code></td>
 </tr>
 </table>
 </div>
 </li>
                    </ul>
                <li> <span class="li-head">receiver</span> - SMS notification receiver list. <span class="li-normal">type: list</span> <span style="font-family:'Courier New'" class="li-required">member_path: cellular/sms_notification/receiver:name</span>
 <a id='label134' href="javascript:ContentClick('label135', 'label134');" onmouseover="ContentPreview('label135');" onmouseout="ContentUnpreview('label135');" title="click to collapse or expand..."> more... </a>
 <div id="label135" style="display:none">
 <table border="1">
 <tr>
 <td></td><td colspan="1">Supported Version Ranges</td>
 </tr>
 <tr>
 <td>receiver</td>
 <td><code class="docutils literal notranslate">v7.2.1 -> 7.6.4 </code></td>
 </tr>
 </table>
 </div>
 </li>
                    <ul class="ul-self">
                    <li> <span class="li-head">alert</span> - Alert multi-options. <span class="li-normal">type: list</span> <span class="li-normal">choices: system-reboot, data-exhausted, session-disconnect, low-signal-strength, mode-switch, os-image-fallback, fgt-backup-mode-switch</span>
 <a id='label136' href="javascript:ContentClick('label137', 'label136');" onmouseover="ContentPreview('label137');" onmouseout="ContentUnpreview('label137');" title="click to collapse or expand..."> more... </a>
 <div id="label137" style="display:none">
 <table border="1">
 <tr>
 <td></td>
 <td colspan="1">Supported Version Ranges</td>
 </tr>
 <tr>
 <td>alert</td>
 <td><code class="docutils literal notranslate">v7.2.1 -> 7.6.4 </code></td>
 </tr>
 <tr>
 <td>[system-reboot]</td>
 <td><code class="docutils literal notranslate">v7.2.1 -> 7.6.4</code></td>
 <tr>
 <td>[data-exhausted]</td>
 <td><code class="docutils literal notranslate">v7.2.1 -> 7.6.4</code></td>
 <tr>
 <td>[session-disconnect]</td>
 <td><code class="docutils literal notranslate">v7.2.1 -> 7.6.4</code></td>
 <tr>
 <td>[low-signal-strength]</td>
 <td><code class="docutils literal notranslate">v7.2.1 -> 7.6.4</code></td>
 <tr>
 <td>[mode-switch]</td>
 <td><code class="docutils literal notranslate">v7.2.1 -> 7.6.4</code></td>
 <tr>
 <td>[os-image-fallback]</td>
 <td><code class="docutils literal notranslate">v7.2.1 -> 7.6.4</code></td>
 <tr>
 <td>[fgt-backup-mode-switch]</td>
 <td><code class="docutils literal notranslate">v7.2.1 -> 7.6.4</code></td>
 </table>
 </div>
 </li>
                    <li> <span class="li-head">name</span> - FortiExtender SMS notification receiver name. <span class="li-normal">type: str</span> <span class="li-required">required: true</span>
 <a id='label138' href="javascript:ContentClick('label139', 'label138');" onmouseover="ContentPreview('label139');" onmouseout="ContentUnpreview('label139');" title="click to collapse or expand..."> more... </a>
 <div id="label139" style="display:none">
 <table border="1">
 <tr>
 <td></td>
 <td colspan="1">Supported Version Ranges</td>
 </tr>
 <tr>
 <td>name</td>
 <td><code class="docutils literal notranslate">v7.2.1 -> 7.6.4 </code></td>
 </tr>
 </table>
 </div>
 </li>
                    <li> <span class="li-head">phone_number</span> - Receiver phone number. Format: [+][country code][area code][local phone number]. For example, +16501234567. <span class="li-normal">type: str</span>
 <a id='label140' href="javascript:ContentClick('label141', 'label140');" onmouseover="ContentPreview('label141');" onmouseout="ContentUnpreview('label141');" title="click to collapse or expand..."> more... </a>
 <div id="label141" style="display:none">
 <table border="1">
 <tr>
 <td></td>
 <td colspan="1">Supported Version Ranges</td>
 </tr>
 <tr>
 <td>phone_number</td>
 <td><code class="docutils literal notranslate">v7.2.1 -> 7.6.4 </code></td>
 </tr>
 </table>
 </div>
 </li>
                    <li> <span class="li-head">status</span> - SMS notification receiver status. <span class="li-normal">type: str</span> <span class="li-normal">choices: disable, enable</span>
 <a id='label142' href="javascript:ContentClick('label143', 'label142');" onmouseover="ContentPreview('label143');" onmouseout="ContentUnpreview('label143');" title="click to collapse or expand..."> more... </a>
 <div id="label143" style="display:none">
 <table border="1">
 <tr>
 <td></td>
 <td colspan="1">Supported Version Ranges</td>
 </tr>
 <tr>
 <td>status</td>
 <td><code class="docutils literal notranslate">v7.2.1 -> 7.6.4 </code></td>
 </tr>
 <tr>
 <td>[disable]</td>
 <td><code class="docutils literal notranslate">v7.2.1 -> 7.6.4</code></td>
 <tr>
 <td>[enable]</td>
 <td><code class="docutils literal notranslate">v7.2.1 -> 7.6.4</code></td>
 </table>
 </div>
 </li>
                    </ul>
                <li> <span class="li-head">status</span> - FortiExtender SMS notification status. <span class="li-normal">type: str</span> <span class="li-normal">choices: disable, enable</span>
 <a id='label144' href="javascript:ContentClick('label145', 'label144');" onmouseover="ContentPreview('label145');" onmouseout="ContentUnpreview('label145');" title="click to collapse or expand..."> more... </a>
 <div id="label145" style="display:none">
 <table border="1">
 <tr>
 <td></td>
 <td colspan="1">Supported Version Ranges</td>
 </tr>
 <tr>
 <td>status</td>
 <td><code class="docutils literal notranslate">v7.2.1 -> 7.6.4 </code></td>
 </tr>
 <tr>
 <td>[disable]</td>
 <td><code class="docutils literal notranslate">v7.2.1 -> 7.6.4</code></td>
 <tr>
 <td>[enable]</td>
 <td><code class="docutils literal notranslate">v7.2.1 -> 7.6.4</code></td>
 </table>
 </div>
 </li>
                </ul>
            </ul>
        <li> <span class="li-head">enforce_bandwidth</span> - Enable/disable enforcement of bandwidth on LAN extension interface. <span class="li-normal">type: str</span> <span class="li-normal">choices: enable, disable</span>
 <a id='label146' href="javascript:ContentClick('label147', 'label146');" onmouseover="ContentPreview('label147');" onmouseout="ContentUnpreview('label147');" title="click to collapse or expand..."> more... </a>
 <div id="label147" style="display:none">
 <table border="1">
 <tr>
 <td></td>
 <td colspan="1">Supported Version Ranges</td>
 </tr>
 <tr>
 <td>enforce_bandwidth</td>
 <td><code class="docutils literal notranslate">v7.2.1 -> 7.6.4 </code></td>
 </tr>
 <tr>
 <td>[enable]</td>
 <td><code class="docutils literal notranslate">v7.2.1 -> 7.6.4</code></td>
 <tr>
 <td>[disable]</td>
 <td><code class="docutils literal notranslate">v7.2.1 -> 7.6.4</code></td>
 </table>
 </div>
 </li>
        <li> <span class="li-head">extension</span> - Extension option. <span class="li-normal">type: str</span> <span class="li-normal">choices: wan-extension, lan-extension</span>
 <a id='label148' href="javascript:ContentClick('label149', 'label148');" onmouseover="ContentPreview('label149');" onmouseout="ContentUnpreview('label149');" title="click to collapse or expand..."> more... </a>
 <div id="label149" style="display:none">
 <table border="1">
 <tr>
 <td></td>
 <td colspan="1">Supported Version Ranges</td>
 </tr>
 <tr>
 <td>extension</td>
 <td><code class="docutils literal notranslate">v7.2.1 -> 7.6.4 </code></td>
 </tr>
 <tr>
 <td>[wan-extension]</td>
 <td><code class="docutils literal notranslate">v7.2.1 -> 7.6.4</code></td>
 <tr>
 <td>[lan-extension]</td>
 <td><code class="docutils literal notranslate">v7.2.1 -> 7.6.4</code></td>
 </table>
 </div>
 </li>
        <li> <span class="li-head">id</span> - ID. <span class="li-normal">type: int</span>
 <a id='label150' href="javascript:ContentClick('label151', 'label150');" onmouseover="ContentPreview('label151');" onmouseout="ContentUnpreview('label151');" title="click to collapse or expand..."> more... </a>
 <div id="label151" style="display:none">
 <table border="1">
 <tr>
 <td></td>
 <td colspan="1">Supported Version Ranges</td>
 </tr>
 <tr>
 <td>id</td>
 <td><code class="docutils literal notranslate">v7.2.1 -> 7.6.4 </code></td>
 </tr>
 </table>
 </div>
 </li>
        <li> <span class="li-head">lan_extension</span> - FortiExtender LAN extension configuration. <span class="li-normal">type: dict</span>
 <a id='label152' href="javascript:ContentClick('label153', 'label152');" onmouseover="ContentPreview('label153');" onmouseout="ContentUnpreview('label153');" title="click to collapse or expand..."> more... </a>
 <div id="label153" style="display:none">
 <table border="1">
 <tr>
 <td></td><td colspan="1">Supported Version Ranges</td>
 </tr>
 <tr>
 <td>lan_extension</td>
 <td><code class="docutils literal notranslate">v7.2.1 -> 7.6.4 </code></td>
 </tr>
 </table>
 </div>
 </li>
            <ul class="ul-self">
            <li> <span class="li-head">backhaul</span> - LAN extension backhaul tunnel configuration. <span class="li-normal">type: list</span> <span style="font-family:'Courier New'" class="li-required">member_path: lan_extension/backhaul:name</span>
 <a id='label154' href="javascript:ContentClick('label155', 'label154');" onmouseover="ContentPreview('label155');" onmouseout="ContentUnpreview('label155');" title="click to collapse or expand..."> more... </a>
 <div id="label155" style="display:none">
 <table border="1">
 <tr>
 <td></td><td colspan="1">Supported Version Ranges</td>
 </tr>
 <tr>
 <td>backhaul</td>
 <td><code class="docutils literal notranslate">v7.2.1 -> 7.6.4 </code></td>
 </tr>
 </table>
 </div>
 </li>
                <ul class="ul-self">
                <li> <span class="li-head">name</span> - FortiExtender LAN extension backhaul name. <span class="li-normal">type: str</span> <span class="li-required">required: true</span>
 <a id='label156' href="javascript:ContentClick('label157', 'label156');" onmouseover="ContentPreview('label157');" onmouseout="ContentUnpreview('label157');" title="click to collapse or expand..."> more... </a>
 <div id="label157" style="display:none">
 <table border="1">
 <tr>
 <td></td>
 <td colspan="1">Supported Version Ranges</td>
 </tr>
 <tr>
 <td>name</td>
 <td><code class="docutils literal notranslate">v7.2.1 -> 7.6.4 </code></td>
 </tr>
 </table>
 </div>
 </li>
                <li> <span class="li-head">port</span> - FortiExtender uplink port. <span class="li-normal">type: str</span> <span class="li-normal">choices: wan, lte1, lte2, port1, port2, port3, port4, port5, sfp</span>
 <a id='label158' href="javascript:ContentClick('label159', 'label158');" onmouseover="ContentPreview('label159');" onmouseout="ContentUnpreview('label159');" title="click to collapse or expand..."> more... </a>
 <div id="label159" style="display:none">
 <table border="1">
 <tr>
 <td></td>
 <td colspan="1">Supported Version Ranges</td>
 </tr>
 <tr>
 <td>port</td>
 <td><code class="docutils literal notranslate">v7.2.1 -> 7.6.4 </code></td>
 </tr>
 <tr>
 <td>[wan]</td>
 <td><code class="docutils literal notranslate">v7.2.1 -> 7.6.4</code></td>
 <tr>
 <td>[lte1]</td>
 <td><code class="docutils literal notranslate">v7.2.1 -> 7.6.4</code></td>
 <tr>
 <td>[lte2]</td>
 <td><code class="docutils literal notranslate">v7.2.1 -> 7.6.4</code></td>
 <tr>
 <td>[port1]</td>
 <td><code class="docutils literal notranslate">v7.2.1 -> 7.6.4</code></td>
 <tr>
 <td>[port2]</td>
 <td><code class="docutils literal notranslate">v7.2.1 -> 7.6.4</code></td>
 <tr>
 <td>[port3]</td>
 <td><code class="docutils literal notranslate">v7.2.1 -> 7.6.4</code></td>
 <tr>
 <td>[port4]</td>
 <td><code class="docutils literal notranslate">v7.2.1 -> 7.6.4</code></td>
 <tr>
 <td>[port5]</td>
 <td><code class="docutils literal notranslate">v7.2.1 -> 7.6.4</code></td>
 <tr>
 <td>[sfp]</td>
 <td><code class="docutils literal notranslate">v7.2.1 -> 7.6.4</code></td>
 </table>
 </div>
 </li>
                <li> <span class="li-head">role</span> - FortiExtender uplink port. <span class="li-normal">type: str</span> <span class="li-normal">choices: primary, secondary</span>
 <a id='label160' href="javascript:ContentClick('label161', 'label160');" onmouseover="ContentPreview('label161');" onmouseout="ContentUnpreview('label161');" title="click to collapse or expand..."> more... </a>
 <div id="label161" style="display:none">
 <table border="1">
 <tr>
 <td></td>
 <td colspan="1">Supported Version Ranges</td>
 </tr>
 <tr>
 <td>role</td>
 <td><code class="docutils literal notranslate">v7.2.1 -> 7.6.4 </code></td>
 </tr>
 <tr>
 <td>[primary]</td>
 <td><code class="docutils literal notranslate">v7.2.1 -> 7.6.4</code></td>
 <tr>
 <td>[secondary]</td>
 <td><code class="docutils literal notranslate">v7.2.1 -> 7.6.4</code></td>
 </table>
 </div>
 </li>
                <li> <span class="li-head">weight</span> - WRR weight parameter. <span class="li-normal">type: int</span>
 <a id='label162' href="javascript:ContentClick('label163', 'label162');" onmouseover="ContentPreview('label163');" onmouseout="ContentUnpreview('label163');" title="click to collapse or expand..."> more... </a>
 <div id="label163" style="display:none">
 <table border="1">
 <tr>
 <td></td>
 <td colspan="1">Supported Version Ranges</td>
 </tr>
 <tr>
 <td>weight</td>
 <td><code class="docutils literal notranslate">v7.2.1 -> 7.6.4 </code></td>
 </tr>
 </table>
 </div>
 </li>
                </ul>
            <li> <span class="li-head">backhaul_interface</span> - IPsec phase1 interface. Source system.interface.name. <span class="li-normal">type: str</span>
 <a id='label164' href="javascript:ContentClick('label165', 'label164');" onmouseover="ContentPreview('label165');" onmouseout="ContentUnpreview('label165');" title="click to collapse or expand..."> more... </a>
 <div id="label165" style="display:none">
 <table border="1">
 <tr>
 <td></td>
 <td colspan="1">Supported Version Ranges</td>
 </tr>
 <tr>
 <td>backhaul_interface</td>
 <td><code class="docutils literal notranslate">v7.2.1 -> 7.6.4 </code></td>
 </tr>
 </table>
 </div>
 </li>
            <li> <span class="li-head">backhaul_ip</span> - IPsec phase1 IPv4/FQDN. Used to specify the external IP/FQDN when the FortiGate unit is behind a NAT device. <span class="li-normal">type: str</span>
 <a id='label166' href="javascript:ContentClick('label167', 'label166');" onmouseover="ContentPreview('label167');" onmouseout="ContentUnpreview('label167');" title="click to collapse or expand..."> more... </a>
 <div id="label167" style="display:none">
 <table border="1">
 <tr>
 <td></td>
 <td colspan="1">Supported Version Ranges</td>
 </tr>
 <tr>
 <td>backhaul_ip</td>
 <td><code class="docutils literal notranslate">v7.2.1 -> 7.6.4 </code></td>
 </tr>
 </table>
 </div>
 </li>
            <li> <span class="li-head">downlinks</span> - Config FortiExtender downlink interface for LAN extension. <span class="li-normal">type: list</span> <span style="font-family:'Courier New'" class="li-required">member_path: lan_extension/downlinks:name</span>
 <a id='label168' href="javascript:ContentClick('label169', 'label168');" onmouseover="ContentPreview('label169');" onmouseout="ContentUnpreview('label169');" title="click to collapse or expand..."> more... </a>
 <div id="label169" style="display:none">
 <table border="1">
 <tr>
 <td></td><td colspan="1">Supported Version Ranges</td>
 </tr>
 <tr>
 <td>downlinks</td>
 <td><code class="docutils literal notranslate">v7.6.0 -> 7.6.4 </code></td>
 </tr>
 </table>
 </div>
 </li>
                <ul class="ul-self">
                <li> <span class="li-head">name</span> - FortiExtender LAN extension downlink config entry name. <span class="li-normal">type: str</span> <span class="li-required">required: true</span>
 <a id='label170' href="javascript:ContentClick('label171', 'label170');" onmouseover="ContentPreview('label171');" onmouseout="ContentUnpreview('label171');" title="click to collapse or expand..."> more... </a>
 <div id="label171" style="display:none">
 <table border="1">
 <tr>
 <td></td>
 <td colspan="1">Supported Version Ranges</td>
 </tr>
 <tr>
 <td>name</td>
 <td><code class="docutils literal notranslate">v7.6.0 -> 7.6.4 </code></td>
 </tr>
 </table>
 </div>
 </li>
                <li> <span class="li-head">port</span> - FortiExtender LAN extension downlink port. <span class="li-normal">type: str</span> <span class="li-normal">choices: port1, port2, port3, port4, port5, lan1, lan2, lan</span>
 <a id='label172' href="javascript:ContentClick('label173', 'label172');" onmouseover="ContentPreview('label173');" onmouseout="ContentUnpreview('label173');" title="click to collapse or expand..."> more... </a>
 <div id="label173" style="display:none">
 <table border="1">
 <tr>
 <td></td>
 <td colspan="1">Supported Version Ranges</td>
 </tr>
 <tr>
 <td>port</td>
 <td><code class="docutils literal notranslate">v7.6.0 -> 7.6.4 </code></td>
 </tr>
 <tr>
 <td>[port1]</td>
 <td><code class="docutils literal notranslate">v7.6.0 -> 7.6.4</code></td>
 <tr>
 <td>[port2]</td>
 <td><code class="docutils literal notranslate">v7.6.0 -> 7.6.4</code></td>
 <tr>
 <td>[port3]</td>
 <td><code class="docutils literal notranslate">v7.6.0 -> 7.6.4</code></td>
 <tr>
 <td>[port4]</td>
 <td><code class="docutils literal notranslate">v7.6.0 -> 7.6.4</code></td>
 <tr>
 <td>[port5]</td>
 <td><code class="docutils literal notranslate">v7.6.0 -> 7.6.4</code></td>
 <tr>
 <td>[lan1]</td>
 <td><code class="docutils literal notranslate">v7.6.0 -> 7.6.4</code></td>
 <tr>
 <td>[lan2]</td>
 <td><code class="docutils literal notranslate">v7.6.0 -> 7.6.4</code></td>
 <tr>
 <td>[lan]</td>
 <td><code class="docutils literal notranslate">v7.6.4 -> 7.6.4</code></td>
 </tr>
 </table>
 </div>
 </li>
                <li> <span class="li-head">pvid</span> - FortiExtender LAN extension downlink PVID (1 - 4089). <span class="li-normal">type: int</span>
 <a id='label174' href="javascript:ContentClick('label175', 'label174');" onmouseover="ContentPreview('label175');" onmouseout="ContentUnpreview('label175');" title="click to collapse or expand..."> more... </a>
 <div id="label175" style="display:none">
 <table border="1">
 <tr>
 <td></td>
 <td colspan="1">Supported Version Ranges</td>
 </tr>
 <tr>
 <td>pvid</td>
 <td><code class="docutils literal notranslate">v7.6.0 -> 7.6.4 </code></td>
 </tr>
 </table>
 </div>
 </li>
                <li> <span class="li-head">type</span> - FortiExtender LAN extension downlink type [port/vap]. <span class="li-normal">type: str</span> <span class="li-normal">choices: port, vap</span>
 <a id='label176' href="javascript:ContentClick('label177', 'label176');" onmouseover="ContentPreview('label177');" onmouseout="ContentUnpreview('label177');" title="click to collapse or expand..."> more... </a>
 <div id="label177" style="display:none">
 <table border="1">
 <tr>
 <td></td>
 <td colspan="1">Supported Version Ranges</td>
 </tr>
 <tr>
 <td>type</td>
 <td><code class="docutils literal notranslate">v7.6.0 -> 7.6.4 </code></td>
 </tr>
 <tr>
 <td>[port]</td>
 <td><code class="docutils literal notranslate">v7.6.0 -> 7.6.4</code></td>
 <tr>
 <td>[vap]</td>
 <td><code class="docutils literal notranslate">v7.6.0 -> 7.6.4</code></td>
 </table>
 </div>
 </li>
                <li> <span class="li-head">vap</span> - FortiExtender LAN extension downlink vap. Source extension-controller.extender-vap.name. <span class="li-normal">type: str</span>
 <a id='label178' href="javascript:ContentClick('label179', 'label178');" onmouseover="ContentPreview('label179');" onmouseout="ContentUnpreview('label179');" title="click to collapse or expand..."> more... </a>
 <div id="label179" style="display:none">
 <table border="1">
 <tr>
 <td></td>
 <td colspan="1">Supported Version Ranges</td>
 </tr>
 <tr>
 <td>vap</td>
 <td><code class="docutils literal notranslate">v7.6.0 -> 7.6.4 </code></td>
 </tr>
 </table>
 </div>
 </li>
                <li> <span class="li-head">vids</span> - FortiExtender LAN extension downlink VIDs. <span class="li-normal">type: list</span> <span style="font-family:'Courier New'" class="li-required">member_path: lan_extension/downlinks:name/vids:vid</span>
 <a id='label180' href="javascript:ContentClick('label181', 'label180');" onmouseover="ContentPreview('label181');" onmouseout="ContentUnpreview('label181');" title="click to collapse or expand..."> more... </a>
 <div id="label181" style="display:none">
 <table border="1">
 <tr>
 <td></td><td colspan="1">Supported Version Ranges</td>
 </tr>
 <tr>
 <td>vids</td>
 <td><code class="docutils literal notranslate">v7.6.4 -> 7.6.4 </code></td>
 </tr>
 </table>
 </div>
 </li>
                    <ul class="ul-self">
                    <li> <span class="li-head">vid</span> - Please enter VID numbers (1 - 4089) with space separated. Up to 50 VIDs are accepted. see <a href='#notes'>Notes</a>. <span class="li-normal">type: int</span> <span class="li-required">required: true</span>
 <a id='label182' href="javascript:ContentClick('label183', 'label182');" onmouseover="ContentPreview('label183');" onmouseout="ContentUnpreview('label183');" title="click to collapse or expand..."> more... </a>
 <div id="label183" style="display:none">
 <table border="1">
 <tr>
 <td></td>
 <td colspan="1">Supported Version Ranges</td>
 </tr>
 <tr>
 <td>vid</td>
 <td><code class="docutils literal notranslate">v7.6.4 -> 7.6.4 </code></td>
 </tr>
 </table>
 </div>
 </li>
                    </ul>
                </ul>
            <li> <span class="li-head">ipsec_tunnel</span> - IPsec tunnel name. <span class="li-normal">type: str</span>
 <a id='label184' href="javascript:ContentClick('label185', 'label184');" onmouseover="ContentPreview('label185');" onmouseout="ContentUnpreview('label185');" title="click to collapse or expand..."> more... </a>
 <div id="label185" style="display:none">
 <table border="1">
 <tr>
 <td></td>
 <td colspan="1">Supported Version Ranges</td>
 </tr>
 <tr>
 <td>ipsec_tunnel</td>
 <td><code class="docutils literal notranslate">v7.2.1 -> 7.6.4 </code></td>
 </tr>
 </table>
 </div>
 </li>
            <li> <span class="li-head">link_loadbalance</span> - LAN extension link load balance strategy. <span class="li-normal">type: str</span> <span class="li-normal">choices: activebackup, loadbalance</span>
 <a id='label186' href="javascript:ContentClick('label187', 'label186');" onmouseover="ContentPreview('label187');" onmouseout="ContentUnpreview('label187');" title="click to collapse or expand..."> more... </a>
 <div id="label187" style="display:none">
 <table border="1">
 <tr>
 <td></td>
 <td colspan="1">Supported Version Ranges</td>
 </tr>
 <tr>
 <td>link_loadbalance</td>
 <td><code class="docutils literal notranslate">v7.2.1 -> 7.6.4 </code></td>
 </tr>
 <tr>
 <td>[activebackup]</td>
 <td><code class="docutils literal notranslate">v7.2.1 -> 7.6.4</code></td>
 <tr>
 <td>[loadbalance]</td>
 <td><code class="docutils literal notranslate">v7.2.1 -> 7.6.4</code></td>
 </table>
 </div>
 </li>
            <li> <span class="li-head">traffic_split_services</span> - Config FortiExtender traffic split interface for LAN extension. <span class="li-normal">type: list</span> <span style="font-family:'Courier New'" class="li-required">member_path: lan_extension/traffic_split_services:name</span>
 <a id='label188' href="javascript:ContentClick('label189', 'label188');" onmouseover="ContentPreview('label189');" onmouseout="ContentUnpreview('label189');" title="click to collapse or expand..."> more... </a>
 <div id="label189" style="display:none">
 <table border="1">
 <tr>
 <td></td><td colspan="1">Supported Version Ranges</td>
 </tr>
 <tr>
 <td>traffic_split_services</td>
 <td><code class="docutils literal notranslate">v7.6.1 -> 7.6.4 </code></td>
 </tr>
 </table>
 </div>
 </li>
                <ul class="ul-self">
                <li> <span class="li-head">address</span> - Address selection. Source firewall.address.name. <span class="li-normal">type: str</span>
 <a id='label190' href="javascript:ContentClick('label191', 'label190');" onmouseover="ContentPreview('label191');" onmouseout="ContentUnpreview('label191');" title="click to collapse or expand..."> more... </a>
 <div id="label191" style="display:none">
 <table border="1">
 <tr>
 <td></td>
 <td colspan="1">Supported Version Ranges</td>
 </tr>
 <tr>
 <td>address</td>
 <td><code class="docutils literal notranslate">v7.6.1 -> 7.6.4 </code></td>
 </tr>
 </table>
 </div>
 </li>
                <li> <span class="li-head">name</span> - FortiExtender LAN extension tunnel split entry name. <span class="li-normal">type: str</span> <span class="li-required">required: true</span>
 <a id='label192' href="javascript:ContentClick('label193', 'label192');" onmouseover="ContentPreview('label193');" onmouseout="ContentUnpreview('label193');" title="click to collapse or expand..."> more... </a>
 <div id="label193" style="display:none">
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
                <li> <span class="li-head">service</span> - Service selection. Source firewall.service.custom.name. <span class="li-normal">type: str</span>
 <a id='label194' href="javascript:ContentClick('label195', 'label194');" onmouseover="ContentPreview('label195');" onmouseout="ContentUnpreview('label195');" title="click to collapse or expand..."> more... </a>
 <div id="label195" style="display:none">
 <table border="1">
 <tr>
 <td></td>
 <td colspan="1">Supported Version Ranges</td>
 </tr>
 <tr>
 <td>service</td>
 <td><code class="docutils literal notranslate">v7.6.1 -> 7.6.4 </code></td>
 </tr>
 </table>
 </div>
 </li>
                <li> <span class="li-head">vsdb</span> - Set video streaming traffic goes through local WAN [enable/disable]. <span class="li-normal">type: str</span> <span class="li-normal">choices: disable, enable</span>
 <a id='label196' href="javascript:ContentClick('label197', 'label196');" onmouseover="ContentPreview('label197');" onmouseout="ContentUnpreview('label197');" title="click to collapse or expand..."> more... </a>
 <div id="label197" style="display:none">
 <table border="1">
 <tr>
 <td></td>
 <td colspan="1">Supported Version Ranges</td>
 </tr>
 <tr>
 <td>vsdb</td>
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
                </ul>
            </ul>
        <li> <span class="li-head">login_password</span> - Set the managed extender"s administrator password. <span class="li-normal">type: str</span>
 <a id='label198' href="javascript:ContentClick('label199', 'label198');" onmouseover="ContentPreview('label199');" onmouseout="ContentUnpreview('label199');" title="click to collapse or expand..."> more... </a>
 <div id="label199" style="display:none">
 <table border="1">
 <tr>
 <td></td>
 <td colspan="1">Supported Version Ranges</td>
 </tr>
 <tr>
 <td>login_password</td>
 <td><code class="docutils literal notranslate">v7.2.1 -> 7.6.4 </code></td>
 </tr>
 </table>
 </div>
 </li>
        <li> <span class="li-head">login_password_change</span> - Change or reset the administrator password of a managed extender (yes, default, or no). <span class="li-normal">type: str</span> <span class="li-normal">choices: yes, default, no</span>
 <a id='label200' href="javascript:ContentClick('label201', 'label200');" onmouseover="ContentPreview('label201');" onmouseout="ContentUnpreview('label201');" title="click to collapse or expand..."> more... </a>
 <div id="label201" style="display:none">
 <table border="1">
 <tr>
 <td></td>
 <td colspan="1">Supported Version Ranges</td>
 </tr>
 <tr>
 <td>login_password_change</td>
 <td><code class="docutils literal notranslate">v7.2.1 -> 7.6.4 </code></td>
 </tr>
 <tr>
 <td>[yes]</td>
 <td><code class="docutils literal notranslate">v7.2.1 -> 7.6.4</code></td>
 <tr>
 <td>[default]</td>
 <td><code class="docutils literal notranslate">v7.2.1 -> 7.6.4</code></td>
 <tr>
 <td>[no]</td>
 <td><code class="docutils literal notranslate">v7.2.1 -> 7.6.4</code></td>
 </table>
 </div>
 </li>
        <li> <span class="li-head">model</span> - Model. <span class="li-normal">type: str</span> <span class="li-normal">choices: FX201E, FX211E, FX200F, FXA11F, FXE11F, FXA21F, FXE21F, FXA22F, FXE22F, FX212F, FX311F, FX312F, FX511F, FXR51G, FXN51G, FXW51G, FVG21F, FVA21F, FVG22F, FVA22F, FX04DA, FG, BS10FW, BS20GW, BS20GN, FVG51G, FXE11G, FX211G</span>
 <a id='label202' href="javascript:ContentClick('label203', 'label202');" onmouseover="ContentPreview('label203');" onmouseout="ContentUnpreview('label203');" title="click to collapse or expand..."> more... </a>
 <div id="label203" style="display:none">
 <table border="1">
 <tr>
 <td></td>
 <td colspan="1">Supported Version Ranges</td>
 </tr>
 <tr>
 <td>model</td>
 <td><code class="docutils literal notranslate">v7.2.1 -> 7.6.4 </code></td>
 </tr>
 <tr>
 <td>[FX201E]</td>
 <td><code class="docutils literal notranslate">v7.2.1 -> 7.6.4</code></td>
 <tr>
 <td>[FX211E]</td>
 <td><code class="docutils literal notranslate">v7.2.1 -> 7.6.4</code></td>
 <tr>
 <td>[FX200F]</td>
 <td><code class="docutils literal notranslate">v7.2.1 -> 7.6.4</code></td>
 <tr>
 <td>[FXA11F]</td>
 <td><code class="docutils literal notranslate">v7.2.1 -> 7.6.4</code></td>
 <tr>
 <td>[FXE11F]</td>
 <td><code class="docutils literal notranslate">v7.2.1 -> 7.6.4</code></td>
 <tr>
 <td>[FXA21F]</td>
 <td><code class="docutils literal notranslate">v7.2.1 -> 7.6.4</code></td>
 <tr>
 <td>[FXE21F]</td>
 <td><code class="docutils literal notranslate">v7.2.1 -> 7.6.4</code></td>
 <tr>
 <td>[FXA22F]</td>
 <td><code class="docutils literal notranslate">v7.2.1 -> 7.6.4</code></td>
 <tr>
 <td>[FXE22F]</td>
 <td><code class="docutils literal notranslate">v7.2.1 -> 7.6.4</code></td>
 <tr>
 <td>[FX212F]</td>
 <td><code class="docutils literal notranslate">v7.2.1 -> 7.6.4</code></td>
 <tr>
 <td>[FX311F]</td>
 <td><code class="docutils literal notranslate">v7.2.1 -> 7.6.4</code></td>
 <tr>
 <td>[FX312F]</td>
 <td><code class="docutils literal notranslate">v7.2.1 -> 7.6.4</code></td>
 <tr>
 <td>[FX511F]</td>
 <td><code class="docutils literal notranslate">v7.2.1 -> 7.6.4</code></td>
 <tr>
 <td>[FXR51G]</td>
 <td><code class="docutils literal notranslate">v7.4.4 -> 7.6.4</code></td>
 </tr>
 <tr>
 <td>[FXN51G]</td>
 <td><code class="docutils literal notranslate">v7.6.0 -> 7.6.4</code></td>
 </tr>
 <tr>
 <td>[FXW51G]</td>
 <td><code class="docutils literal notranslate">v7.6.0 -> 7.6.4</code></td>
 </tr>
 <tr>
 <td>[FVG21F]</td>
 <td><code class="docutils literal notranslate">v7.2.1 -> 7.6.4</code></td>
 <tr>
 <td>[FVA21F]</td>
 <td><code class="docutils literal notranslate">v7.2.1 -> 7.6.4</code></td>
 <tr>
 <td>[FVG22F]</td>
 <td><code class="docutils literal notranslate">v7.2.1 -> 7.6.4</code></td>
 <tr>
 <td>[FVA22F]</td>
 <td><code class="docutils literal notranslate">v7.2.1 -> 7.6.4</code></td>
 <tr>
 <td>[FX04DA]</td>
 <td><code class="docutils literal notranslate">v7.2.1 -> 7.6.4</code></td>
 <tr>
 <td>[FG]</td>
 <td><code class="docutils literal notranslate">v7.4.4 -> 7.6.4</code></td>
 </tr>
 <tr>
 <td>[BS10FW]</td>
 <td><code class="docutils literal notranslate">v7.4.4 -> 7.6.4</code></td>
 </tr>
 <tr>
 <td>[BS20GW]</td>
 <td><code class="docutils literal notranslate">v7.4.4 -> 7.6.4</code></td>
 </tr>
 <tr>
 <td>[BS20GN]</td>
 <td><code class="docutils literal notranslate">v7.4.4 -> 7.6.4</code></td>
 </tr>
 <tr>
 <td>[FVG51G]</td>
 <td><code class="docutils literal notranslate">v7.6.1 -> 7.6.4</code></td>
 </tr>
 <tr>
 <td>[FXE11G]</td>
 <td><code class="docutils literal notranslate">v7.6.3 -> 7.6.4</code></td>
 </tr>
 <tr>
 <td>[FX211G]</td>
 <td><code class="docutils literal notranslate">v7.6.4 -> 7.6.4</code></td>
 </tr>
 </table>
 </div>
 </li>
        <li> <span class="li-head">name</span> - FortiExtender profile name. <span class="li-normal">type: str</span> <span class="li-required">required: true</span>
 <a id='label204' href="javascript:ContentClick('label205', 'label204');" onmouseover="ContentPreview('label205');" onmouseout="ContentUnpreview('label205');" title="click to collapse or expand..."> more... </a>
 <div id="label205" style="display:none">
 <table border="1">
 <tr>
 <td></td>
 <td colspan="1">Supported Version Ranges</td>
 </tr>
 <tr>
 <td>name</td>
 <td><code class="docutils literal notranslate">v7.2.1 -> 7.6.4 </code></td>
 </tr>
 </table>
 </div>
 </li>
        <li> <span class="li-head">wifi</span> - FortiExtender Wi-Fi configuration. <span class="li-normal">type: dict</span>
 <a id='label206' href="javascript:ContentClick('label207', 'label206');" onmouseover="ContentPreview('label207');" onmouseout="ContentUnpreview('label207');" title="click to collapse or expand..."> more... </a>
 <div id="label207" style="display:none">
 <table border="1">
 <tr>
 <td></td><td colspan="1">Supported Version Ranges</td>
 </tr>
 <tr>
 <td>wifi</td>
 <td><code class="docutils literal notranslate">v7.4.4 -> 7.6.4 </code></td>
 </tr>
 </table>
 </div>
 </li>
            <ul class="ul-self">
            <li> <span class="li-head">country</span> - Country in which this FEX will operate . <span class="li-normal">type: str</span> <span class="li-normal">choices: --, AF, AL, DZ, AS, AO, AR, AM, AU, AT, AZ, BS, BH, BD, BB, BY, BE, BZ, BJ, BM, BT, BO, BA, BW, BR, BN, BG, BF, KH, CM, KY, CF, TD, CL, CN, CX, CO, CG, CD, CR, HR, CY, CZ, DK, DJ, DM, DO, EC, EG, SV, ET, EE, GF, PF, FO, FJ, FI, FR, GA, GE, GM, DE, GH, GI, GR, GL, GD, GP, GU, GT, GY, HT, HN, HK, HU, IS, IN, ID, IQ, IE, IM, IL, IT, CI, JM, JO, KZ, KE, KR, KW, LA, LV, LB, LS, LR, LY, LI, LT, LU, MO, MK, MG, MW, MY, MV, ML, MT, MH, MQ, MR, MU, YT, MX, FM, MD, MC, MN, MA, MZ, MM, NA, NP, NL, AN, AW, NZ, NI, NE, NG, NO, MP, OM, PK, PW, PA, PG, PY, PE, PH, PL, PT, PR, QA, RE, RO, RU, RW, BL, KN, LC, MF, PM, VC, SA, SN, RS, ME, SL, SG, SK, SI, SO, ZA, ES, LK, SR, SZ, SE, CH, TW, TZ, TH, TL, TG, TT, TN, TR, TM, AE, TC, UG, UA, GB, US, PS, UY, UZ, VU, VE, VN, VI, WF, YE, ZM, ZW, JP, CA</span>
 <a id='label208' href="javascript:ContentClick('label209', 'label208');" onmouseover="ContentPreview('label209');" onmouseout="ContentUnpreview('label209');" title="click to collapse or expand..."> more... </a>
 <div id="label209" style="display:none">
 <table border="1">
 <tr>
 <td></td>
 <td colspan="1">Supported Version Ranges</td>
 </tr>
 <tr>
 <td>country</td>
 <td><code class="docutils literal notranslate">v7.4.4 -> 7.6.4 </code></td>
 </tr>
 <tr>
 <td>[--]</td>
 <td><code class="docutils literal notranslate">v7.4.4 -> 7.6.4</code></td>
 <tr>
 <td>[AF]</td>
 <td><code class="docutils literal notranslate">v7.4.4 -> 7.6.4</code></td>
 <tr>
 <td>[AL]</td>
 <td><code class="docutils literal notranslate">v7.4.4 -> 7.6.4</code></td>
 <tr>
 <td>[DZ]</td>
 <td><code class="docutils literal notranslate">v7.4.4 -> 7.6.4</code></td>
 <tr>
 <td>[AS]</td>
 <td><code class="docutils literal notranslate">v7.4.4 -> 7.6.4</code></td>
 <tr>
 <td>[AO]</td>
 <td><code class="docutils literal notranslate">v7.4.4 -> 7.6.4</code></td>
 <tr>
 <td>[AR]</td>
 <td><code class="docutils literal notranslate">v7.4.4 -> 7.6.4</code></td>
 <tr>
 <td>[AM]</td>
 <td><code class="docutils literal notranslate">v7.4.4 -> 7.6.4</code></td>
 <tr>
 <td>[AU]</td>
 <td><code class="docutils literal notranslate">v7.4.4 -> 7.6.4</code></td>
 <tr>
 <td>[AT]</td>
 <td><code class="docutils literal notranslate">v7.4.4 -> 7.6.4</code></td>
 <tr>
 <td>[AZ]</td>
 <td><code class="docutils literal notranslate">v7.4.4 -> 7.6.4</code></td>
 <tr>
 <td>[BS]</td>
 <td><code class="docutils literal notranslate">v7.4.4 -> 7.6.4</code></td>
 <tr>
 <td>[BH]</td>
 <td><code class="docutils literal notranslate">v7.4.4 -> 7.6.4</code></td>
 <tr>
 <td>[BD]</td>
 <td><code class="docutils literal notranslate">v7.4.4 -> 7.6.4</code></td>
 <tr>
 <td>[BB]</td>
 <td><code class="docutils literal notranslate">v7.4.4 -> 7.6.4</code></td>
 <tr>
 <td>[BY]</td>
 <td><code class="docutils literal notranslate">v7.4.4 -> 7.6.4</code></td>
 <tr>
 <td>[BE]</td>
 <td><code class="docutils literal notranslate">v7.4.4 -> 7.6.4</code></td>
 <tr>
 <td>[BZ]</td>
 <td><code class="docutils literal notranslate">v7.4.4 -> 7.6.4</code></td>
 <tr>
 <td>[BJ]</td>
 <td><code class="docutils literal notranslate">v7.4.4 -> 7.6.4</code></td>
 <tr>
 <td>[BM]</td>
 <td><code class="docutils literal notranslate">v7.4.4 -> 7.6.4</code></td>
 <tr>
 <td>[BT]</td>
 <td><code class="docutils literal notranslate">v7.4.4 -> 7.6.4</code></td>
 <tr>
 <td>[BO]</td>
 <td><code class="docutils literal notranslate">v7.4.4 -> 7.6.4</code></td>
 <tr>
 <td>[BA]</td>
 <td><code class="docutils literal notranslate">v7.4.4 -> 7.6.4</code></td>
 <tr>
 <td>[BW]</td>
 <td><code class="docutils literal notranslate">v7.4.4 -> 7.6.4</code></td>
 <tr>
 <td>[BR]</td>
 <td><code class="docutils literal notranslate">v7.4.4 -> 7.6.4</code></td>
 <tr>
 <td>[BN]</td>
 <td><code class="docutils literal notranslate">v7.4.4 -> 7.6.4</code></td>
 <tr>
 <td>[BG]</td>
 <td><code class="docutils literal notranslate">v7.4.4 -> 7.6.4</code></td>
 <tr>
 <td>[BF]</td>
 <td><code class="docutils literal notranslate">v7.4.4 -> 7.6.4</code></td>
 <tr>
 <td>[KH]</td>
 <td><code class="docutils literal notranslate">v7.4.4 -> 7.6.4</code></td>
 <tr>
 <td>[CM]</td>
 <td><code class="docutils literal notranslate">v7.4.4 -> 7.6.4</code></td>
 <tr>
 <td>[KY]</td>
 <td><code class="docutils literal notranslate">v7.4.4 -> 7.6.4</code></td>
 <tr>
 <td>[CF]</td>
 <td><code class="docutils literal notranslate">v7.4.4 -> 7.6.4</code></td>
 <tr>
 <td>[TD]</td>
 <td><code class="docutils literal notranslate">v7.4.4 -> 7.6.4</code></td>
 <tr>
 <td>[CL]</td>
 <td><code class="docutils literal notranslate">v7.4.4 -> 7.6.4</code></td>
 <tr>
 <td>[CN]</td>
 <td><code class="docutils literal notranslate">v7.4.4 -> 7.6.4</code></td>
 <tr>
 <td>[CX]</td>
 <td><code class="docutils literal notranslate">v7.4.4 -> 7.6.4</code></td>
 <tr>
 <td>[CO]</td>
 <td><code class="docutils literal notranslate">v7.4.4 -> 7.6.4</code></td>
 <tr>
 <td>[CG]</td>
 <td><code class="docutils literal notranslate">v7.4.4 -> 7.6.4</code></td>
 <tr>
 <td>[CD]</td>
 <td><code class="docutils literal notranslate">v7.4.4 -> 7.6.4</code></td>
 <tr>
 <td>[CR]</td>
 <td><code class="docutils literal notranslate">v7.4.4 -> 7.6.4</code></td>
 <tr>
 <td>[HR]</td>
 <td><code class="docutils literal notranslate">v7.4.4 -> 7.6.4</code></td>
 <tr>
 <td>[CY]</td>
 <td><code class="docutils literal notranslate">v7.4.4 -> 7.6.4</code></td>
 <tr>
 <td>[CZ]</td>
 <td><code class="docutils literal notranslate">v7.4.4 -> 7.6.4</code></td>
 <tr>
 <td>[DK]</td>
 <td><code class="docutils literal notranslate">v7.4.4 -> 7.6.4</code></td>
 <tr>
 <td>[DJ]</td>
 <td><code class="docutils literal notranslate">v7.4.4 -> 7.6.4</code></td>
 <tr>
 <td>[DM]</td>
 <td><code class="docutils literal notranslate">v7.4.4 -> 7.6.4</code></td>
 <tr>
 <td>[DO]</td>
 <td><code class="docutils literal notranslate">v7.4.4 -> 7.6.4</code></td>
 <tr>
 <td>[EC]</td>
 <td><code class="docutils literal notranslate">v7.4.4 -> 7.6.4</code></td>
 <tr>
 <td>[EG]</td>
 <td><code class="docutils literal notranslate">v7.4.4 -> 7.6.4</code></td>
 <tr>
 <td>[SV]</td>
 <td><code class="docutils literal notranslate">v7.4.4 -> 7.6.4</code></td>
 <tr>
 <td>[ET]</td>
 <td><code class="docutils literal notranslate">v7.4.4 -> 7.6.4</code></td>
 <tr>
 <td>[EE]</td>
 <td><code class="docutils literal notranslate">v7.4.4 -> 7.6.4</code></td>
 <tr>
 <td>[GF]</td>
 <td><code class="docutils literal notranslate">v7.4.4 -> 7.6.4</code></td>
 <tr>
 <td>[PF]</td>
 <td><code class="docutils literal notranslate">v7.4.4 -> 7.6.4</code></td>
 <tr>
 <td>[FO]</td>
 <td><code class="docutils literal notranslate">v7.4.4 -> 7.6.4</code></td>
 <tr>
 <td>[FJ]</td>
 <td><code class="docutils literal notranslate">v7.4.4 -> 7.6.4</code></td>
 <tr>
 <td>[FI]</td>
 <td><code class="docutils literal notranslate">v7.4.4 -> 7.6.4</code></td>
 <tr>
 <td>[FR]</td>
 <td><code class="docutils literal notranslate">v7.4.4 -> 7.6.4</code></td>
 <tr>
 <td>[GA]</td>
 <td><code class="docutils literal notranslate">v7.4.4 -> 7.6.4</code></td>
 <tr>
 <td>[GE]</td>
 <td><code class="docutils literal notranslate">v7.4.4 -> 7.6.4</code></td>
 <tr>
 <td>[GM]</td>
 <td><code class="docutils literal notranslate">v7.4.4 -> 7.6.4</code></td>
 <tr>
 <td>[DE]</td>
 <td><code class="docutils literal notranslate">v7.4.4 -> 7.6.4</code></td>
 <tr>
 <td>[GH]</td>
 <td><code class="docutils literal notranslate">v7.4.4 -> 7.6.4</code></td>
 <tr>
 <td>[GI]</td>
 <td><code class="docutils literal notranslate">v7.4.4 -> 7.6.4</code></td>
 <tr>
 <td>[GR]</td>
 <td><code class="docutils literal notranslate">v7.4.4 -> 7.6.4</code></td>
 <tr>
 <td>[GL]</td>
 <td><code class="docutils literal notranslate">v7.4.4 -> 7.6.4</code></td>
 <tr>
 <td>[GD]</td>
 <td><code class="docutils literal notranslate">v7.4.4 -> 7.6.4</code></td>
 <tr>
 <td>[GP]</td>
 <td><code class="docutils literal notranslate">v7.4.4 -> 7.6.4</code></td>
 <tr>
 <td>[GU]</td>
 <td><code class="docutils literal notranslate">v7.4.4 -> 7.6.4</code></td>
 <tr>
 <td>[GT]</td>
 <td><code class="docutils literal notranslate">v7.4.4 -> 7.6.4</code></td>
 <tr>
 <td>[GY]</td>
 <td><code class="docutils literal notranslate">v7.4.4 -> 7.6.4</code></td>
 <tr>
 <td>[HT]</td>
 <td><code class="docutils literal notranslate">v7.4.4 -> 7.6.4</code></td>
 <tr>
 <td>[HN]</td>
 <td><code class="docutils literal notranslate">v7.4.4 -> 7.6.4</code></td>
 <tr>
 <td>[HK]</td>
 <td><code class="docutils literal notranslate">v7.4.4 -> 7.6.4</code></td>
 <tr>
 <td>[HU]</td>
 <td><code class="docutils literal notranslate">v7.4.4 -> 7.6.4</code></td>
 <tr>
 <td>[IS]</td>
 <td><code class="docutils literal notranslate">v7.4.4 -> 7.6.4</code></td>
 <tr>
 <td>[IN]</td>
 <td><code class="docutils literal notranslate">v7.4.4 -> 7.6.4</code></td>
 <tr>
 <td>[ID]</td>
 <td><code class="docutils literal notranslate">v7.4.4 -> 7.6.4</code></td>
 <tr>
 <td>[IQ]</td>
 <td><code class="docutils literal notranslate">v7.4.4 -> 7.6.4</code></td>
 <tr>
 <td>[IE]</td>
 <td><code class="docutils literal notranslate">v7.4.4 -> 7.6.4</code></td>
 <tr>
 <td>[IM]</td>
 <td><code class="docutils literal notranslate">v7.4.4 -> 7.6.4</code></td>
 <tr>
 <td>[IL]</td>
 <td><code class="docutils literal notranslate">v7.4.4 -> 7.6.4</code></td>
 <tr>
 <td>[IT]</td>
 <td><code class="docutils literal notranslate">v7.4.4 -> 7.6.4</code></td>
 <tr>
 <td>[CI]</td>
 <td><code class="docutils literal notranslate">v7.4.4 -> 7.6.4</code></td>
 <tr>
 <td>[JM]</td>
 <td><code class="docutils literal notranslate">v7.4.4 -> 7.6.4</code></td>
 <tr>
 <td>[JO]</td>
 <td><code class="docutils literal notranslate">v7.4.4 -> 7.6.4</code></td>
 <tr>
 <td>[KZ]</td>
 <td><code class="docutils literal notranslate">v7.4.4 -> 7.6.4</code></td>
 <tr>
 <td>[KE]</td>
 <td><code class="docutils literal notranslate">v7.4.4 -> 7.6.4</code></td>
 <tr>
 <td>[KR]</td>
 <td><code class="docutils literal notranslate">v7.4.4 -> 7.6.4</code></td>
 <tr>
 <td>[KW]</td>
 <td><code class="docutils literal notranslate">v7.4.4 -> 7.6.4</code></td>
 <tr>
 <td>[LA]</td>
 <td><code class="docutils literal notranslate">v7.4.4 -> 7.6.4</code></td>
 <tr>
 <td>[LV]</td>
 <td><code class="docutils literal notranslate">v7.4.4 -> 7.6.4</code></td>
 <tr>
 <td>[LB]</td>
 <td><code class="docutils literal notranslate">v7.4.4 -> 7.6.4</code></td>
 <tr>
 <td>[LS]</td>
 <td><code class="docutils literal notranslate">v7.4.4 -> 7.6.4</code></td>
 <tr>
 <td>[LR]</td>
 <td><code class="docutils literal notranslate">v7.4.4 -> 7.6.4</code></td>
 <tr>
 <td>[LY]</td>
 <td><code class="docutils literal notranslate">v7.4.4 -> 7.6.4</code></td>
 <tr>
 <td>[LI]</td>
 <td><code class="docutils literal notranslate">v7.4.4 -> 7.6.4</code></td>
 <tr>
 <td>[LT]</td>
 <td><code class="docutils literal notranslate">v7.4.4 -> 7.6.4</code></td>
 <tr>
 <td>[LU]</td>
 <td><code class="docutils literal notranslate">v7.4.4 -> 7.6.4</code></td>
 <tr>
 <td>[MO]</td>
 <td><code class="docutils literal notranslate">v7.4.4 -> 7.6.4</code></td>
 <tr>
 <td>[MK]</td>
 <td><code class="docutils literal notranslate">v7.4.4 -> 7.6.4</code></td>
 <tr>
 <td>[MG]</td>
 <td><code class="docutils literal notranslate">v7.4.4 -> 7.6.4</code></td>
 <tr>
 <td>[MW]</td>
 <td><code class="docutils literal notranslate">v7.4.4 -> 7.6.4</code></td>
 <tr>
 <td>[MY]</td>
 <td><code class="docutils literal notranslate">v7.4.4 -> 7.6.4</code></td>
 <tr>
 <td>[MV]</td>
 <td><code class="docutils literal notranslate">v7.4.4 -> 7.6.4</code></td>
 <tr>
 <td>[ML]</td>
 <td><code class="docutils literal notranslate">v7.4.4 -> 7.6.4</code></td>
 <tr>
 <td>[MT]</td>
 <td><code class="docutils literal notranslate">v7.4.4 -> 7.6.4</code></td>
 <tr>
 <td>[MH]</td>
 <td><code class="docutils literal notranslate">v7.4.4 -> 7.6.4</code></td>
 <tr>
 <td>[MQ]</td>
 <td><code class="docutils literal notranslate">v7.4.4 -> 7.6.4</code></td>
 <tr>
 <td>[MR]</td>
 <td><code class="docutils literal notranslate">v7.4.4 -> 7.6.4</code></td>
 <tr>
 <td>[MU]</td>
 <td><code class="docutils literal notranslate">v7.4.4 -> 7.6.4</code></td>
 <tr>
 <td>[YT]</td>
 <td><code class="docutils literal notranslate">v7.4.4 -> 7.6.4</code></td>
 <tr>
 <td>[MX]</td>
 <td><code class="docutils literal notranslate">v7.4.4 -> 7.6.4</code></td>
 <tr>
 <td>[FM]</td>
 <td><code class="docutils literal notranslate">v7.4.4 -> 7.6.4</code></td>
 <tr>
 <td>[MD]</td>
 <td><code class="docutils literal notranslate">v7.4.4 -> 7.6.4</code></td>
 <tr>
 <td>[MC]</td>
 <td><code class="docutils literal notranslate">v7.4.4 -> 7.6.4</code></td>
 <tr>
 <td>[MN]</td>
 <td><code class="docutils literal notranslate">v7.4.4 -> 7.6.4</code></td>
 <tr>
 <td>[MA]</td>
 <td><code class="docutils literal notranslate">v7.4.4 -> 7.6.4</code></td>
 <tr>
 <td>[MZ]</td>
 <td><code class="docutils literal notranslate">v7.4.4 -> 7.6.4</code></td>
 <tr>
 <td>[MM]</td>
 <td><code class="docutils literal notranslate">v7.4.4 -> 7.6.4</code></td>
 <tr>
 <td>[NA]</td>
 <td><code class="docutils literal notranslate">v7.4.4 -> 7.6.4</code></td>
 <tr>
 <td>[NP]</td>
 <td><code class="docutils literal notranslate">v7.4.4 -> 7.6.4</code></td>
 <tr>
 <td>[NL]</td>
 <td><code class="docutils literal notranslate">v7.4.4 -> 7.6.4</code></td>
 <tr>
 <td>[AN]</td>
 <td><code class="docutils literal notranslate">v7.4.4 -> 7.6.4</code></td>
 <tr>
 <td>[AW]</td>
 <td><code class="docutils literal notranslate">v7.4.4 -> 7.6.4</code></td>
 <tr>
 <td>[NZ]</td>
 <td><code class="docutils literal notranslate">v7.4.4 -> 7.6.4</code></td>
 <tr>
 <td>[NI]</td>
 <td><code class="docutils literal notranslate">v7.4.4 -> 7.6.4</code></td>
 <tr>
 <td>[NE]</td>
 <td><code class="docutils literal notranslate">v7.4.4 -> 7.6.4</code></td>
 <tr>
 <td>[NG]</td>
 <td><code class="docutils literal notranslate">v7.4.4 -> 7.6.4</code></td>
 <tr>
 <td>[NO]</td>
 <td><code class="docutils literal notranslate">v7.4.4 -> 7.6.4</code></td>
 <tr>
 <td>[MP]</td>
 <td><code class="docutils literal notranslate">v7.4.4 -> 7.6.4</code></td>
 <tr>
 <td>[OM]</td>
 <td><code class="docutils literal notranslate">v7.4.4 -> 7.6.4</code></td>
 <tr>
 <td>[PK]</td>
 <td><code class="docutils literal notranslate">v7.4.4 -> 7.6.4</code></td>
 <tr>
 <td>[PW]</td>
 <td><code class="docutils literal notranslate">v7.4.4 -> 7.6.4</code></td>
 <tr>
 <td>[PA]</td>
 <td><code class="docutils literal notranslate">v7.4.4 -> 7.6.4</code></td>
 <tr>
 <td>[PG]</td>
 <td><code class="docutils literal notranslate">v7.4.4 -> 7.6.4</code></td>
 <tr>
 <td>[PY]</td>
 <td><code class="docutils literal notranslate">v7.4.4 -> 7.6.4</code></td>
 <tr>
 <td>[PE]</td>
 <td><code class="docutils literal notranslate">v7.4.4 -> 7.6.4</code></td>
 <tr>
 <td>[PH]</td>
 <td><code class="docutils literal notranslate">v7.4.4 -> 7.6.4</code></td>
 <tr>
 <td>[PL]</td>
 <td><code class="docutils literal notranslate">v7.4.4 -> 7.6.4</code></td>
 <tr>
 <td>[PT]</td>
 <td><code class="docutils literal notranslate">v7.4.4 -> 7.6.4</code></td>
 <tr>
 <td>[PR]</td>
 <td><code class="docutils literal notranslate">v7.4.4 -> 7.6.4</code></td>
 <tr>
 <td>[QA]</td>
 <td><code class="docutils literal notranslate">v7.4.4 -> 7.6.4</code></td>
 <tr>
 <td>[RE]</td>
 <td><code class="docutils literal notranslate">v7.4.4 -> 7.6.4</code></td>
 <tr>
 <td>[RO]</td>
 <td><code class="docutils literal notranslate">v7.4.4 -> 7.6.4</code></td>
 <tr>
 <td>[RU]</td>
 <td><code class="docutils literal notranslate">v7.4.4 -> 7.6.4</code></td>
 <tr>
 <td>[RW]</td>
 <td><code class="docutils literal notranslate">v7.4.4 -> 7.6.4</code></td>
 <tr>
 <td>[BL]</td>
 <td><code class="docutils literal notranslate">v7.4.4 -> 7.6.4</code></td>
 <tr>
 <td>[KN]</td>
 <td><code class="docutils literal notranslate">v7.4.4 -> 7.6.4</code></td>
 <tr>
 <td>[LC]</td>
 <td><code class="docutils literal notranslate">v7.4.4 -> 7.6.4</code></td>
 <tr>
 <td>[MF]</td>
 <td><code class="docutils literal notranslate">v7.4.4 -> 7.6.4</code></td>
 <tr>
 <td>[PM]</td>
 <td><code class="docutils literal notranslate">v7.4.4 -> 7.6.4</code></td>
 <tr>
 <td>[VC]</td>
 <td><code class="docutils literal notranslate">v7.4.4 -> 7.6.4</code></td>
 <tr>
 <td>[SA]</td>
 <td><code class="docutils literal notranslate">v7.4.4 -> 7.6.4</code></td>
 <tr>
 <td>[SN]</td>
 <td><code class="docutils literal notranslate">v7.4.4 -> 7.6.4</code></td>
 <tr>
 <td>[RS]</td>
 <td><code class="docutils literal notranslate">v7.4.4 -> 7.6.4</code></td>
 <tr>
 <td>[ME]</td>
 <td><code class="docutils literal notranslate">v7.4.4 -> 7.6.4</code></td>
 <tr>
 <td>[SL]</td>
 <td><code class="docutils literal notranslate">v7.4.4 -> 7.6.4</code></td>
 <tr>
 <td>[SG]</td>
 <td><code class="docutils literal notranslate">v7.4.4 -> 7.6.4</code></td>
 <tr>
 <td>[SK]</td>
 <td><code class="docutils literal notranslate">v7.4.4 -> 7.6.4</code></td>
 <tr>
 <td>[SI]</td>
 <td><code class="docutils literal notranslate">v7.4.4 -> 7.6.4</code></td>
 <tr>
 <td>[SO]</td>
 <td><code class="docutils literal notranslate">v7.4.4 -> 7.6.4</code></td>
 <tr>
 <td>[ZA]</td>
 <td><code class="docutils literal notranslate">v7.4.4 -> 7.6.4</code></td>
 <tr>
 <td>[ES]</td>
 <td><code class="docutils literal notranslate">v7.4.4 -> 7.6.4</code></td>
 <tr>
 <td>[LK]</td>
 <td><code class="docutils literal notranslate">v7.4.4 -> 7.6.4</code></td>
 <tr>
 <td>[SR]</td>
 <td><code class="docutils literal notranslate">v7.4.4 -> 7.6.4</code></td>
 <tr>
 <td>[SZ]</td>
 <td><code class="docutils literal notranslate">v7.4.4 -> 7.6.4</code></td>
 <tr>
 <td>[SE]</td>
 <td><code class="docutils literal notranslate">v7.4.4 -> 7.6.4</code></td>
 <tr>
 <td>[CH]</td>
 <td><code class="docutils literal notranslate">v7.4.4 -> 7.6.4</code></td>
 <tr>
 <td>[TW]</td>
 <td><code class="docutils literal notranslate">v7.4.4 -> 7.6.4</code></td>
 <tr>
 <td>[TZ]</td>
 <td><code class="docutils literal notranslate">v7.4.4 -> 7.6.4</code></td>
 <tr>
 <td>[TH]</td>
 <td><code class="docutils literal notranslate">v7.4.4 -> 7.6.4</code></td>
 <tr>
 <td>[TL]</td>
 <td><code class="docutils literal notranslate">v7.6.3 -> 7.6.4</code></td>
 </tr>
 <tr>
 <td>[TG]</td>
 <td><code class="docutils literal notranslate">v7.4.4 -> 7.6.4</code></td>
 <tr>
 <td>[TT]</td>
 <td><code class="docutils literal notranslate">v7.4.4 -> 7.6.4</code></td>
 <tr>
 <td>[TN]</td>
 <td><code class="docutils literal notranslate">v7.4.4 -> 7.6.4</code></td>
 <tr>
 <td>[TR]</td>
 <td><code class="docutils literal notranslate">v7.4.4 -> 7.6.4</code></td>
 <tr>
 <td>[TM]</td>
 <td><code class="docutils literal notranslate">v7.4.4 -> 7.6.4</code></td>
 <tr>
 <td>[AE]</td>
 <td><code class="docutils literal notranslate">v7.4.4 -> 7.6.4</code></td>
 <tr>
 <td>[TC]</td>
 <td><code class="docutils literal notranslate">v7.4.4 -> 7.6.4</code></td>
 <tr>
 <td>[UG]</td>
 <td><code class="docutils literal notranslate">v7.4.4 -> 7.6.4</code></td>
 <tr>
 <td>[UA]</td>
 <td><code class="docutils literal notranslate">v7.4.4 -> 7.6.4</code></td>
 <tr>
 <td>[GB]</td>
 <td><code class="docutils literal notranslate">v7.4.4 -> 7.6.4</code></td>
 <tr>
 <td>[US]</td>
 <td><code class="docutils literal notranslate">v7.4.4 -> 7.6.4</code></td>
 <tr>
 <td>[PS]</td>
 <td><code class="docutils literal notranslate">v7.4.4 -> 7.6.4</code></td>
 <tr>
 <td>[UY]</td>
 <td><code class="docutils literal notranslate">v7.4.4 -> 7.6.4</code></td>
 <tr>
 <td>[UZ]</td>
 <td><code class="docutils literal notranslate">v7.4.4 -> 7.6.4</code></td>
 <tr>
 <td>[VU]</td>
 <td><code class="docutils literal notranslate">v7.4.4 -> 7.6.4</code></td>
 <tr>
 <td>[VE]</td>
 <td><code class="docutils literal notranslate">v7.4.4 -> 7.6.4</code></td>
 <tr>
 <td>[VN]</td>
 <td><code class="docutils literal notranslate">v7.4.4 -> 7.6.4</code></td>
 <tr>
 <td>[VI]</td>
 <td><code class="docutils literal notranslate">v7.4.4 -> 7.6.4</code></td>
 <tr>
 <td>[WF]</td>
 <td><code class="docutils literal notranslate">v7.4.4 -> 7.6.4</code></td>
 <tr>
 <td>[YE]</td>
 <td><code class="docutils literal notranslate">v7.4.4 -> 7.6.4</code></td>
 <tr>
 <td>[ZM]</td>
 <td><code class="docutils literal notranslate">v7.4.4 -> 7.6.4</code></td>
 <tr>
 <td>[ZW]</td>
 <td><code class="docutils literal notranslate">v7.4.4 -> 7.6.4</code></td>
 <tr>
 <td>[JP]</td>
 <td><code class="docutils literal notranslate">v7.4.4 -> 7.6.4</code></td>
 <tr>
 <td>[CA]</td>
 <td><code class="docutils literal notranslate">v7.4.4 -> 7.6.4</code></td>
 </table>
 </div>
 </li>
            <li> <span class="li-head">radio_1</span> - Radio-1 config for Wi-Fi 2.4GHz <span class="li-normal">type: dict</span>
 <a id='label210' href="javascript:ContentClick('label211', 'label210');" onmouseover="ContentPreview('label211');" onmouseout="ContentUnpreview('label211');" title="click to collapse or expand..."> more... </a>
 <div id="label211" style="display:none">
 <table border="1">
 <tr>
 <td></td><td colspan="1">Supported Version Ranges</td>
 </tr>
 <tr>
 <td>radio_1</td>
 <td><code class="docutils literal notranslate">v7.4.4 -> 7.6.4 </code></td>
 </tr>
 </table>
 </div>
 </li>
                <ul class="ul-self">
                <li> <span class="li-head">band</span> - Wi-Fi band selection 2.4GHz / 5GHz. <span class="li-normal">type: str</span> <span class="li-normal">choices: 2.4GHz</span>
 <a id='label212' href="javascript:ContentClick('label213', 'label212');" onmouseover="ContentPreview('label213');" onmouseout="ContentUnpreview('label213');" title="click to collapse or expand..."> more... </a>
 <div id="label213" style="display:none">
 <table border="1">
 <tr>
 <td></td>
 <td colspan="1">Supported Version Ranges</td>
 </tr>
 <tr>
 <td>band</td>
 <td><code class="docutils literal notranslate">v7.4.4 -> 7.6.4 </code></td>
 </tr>
 <tr>
 <td>[2.4GHz]</td>
 <td><code class="docutils literal notranslate">v7.4.4 -> 7.6.4</code></td>
 </table>
 </div>
 </li>
                <li> <span class="li-head">bandwidth</span> - Wi-Fi channel bandwidth. <span class="li-normal">type: str</span> <span class="li-normal">choices: auto, 20MHz, 40MHz, 80MHz</span>
 <a id='label214' href="javascript:ContentClick('label215', 'label214');" onmouseover="ContentPreview('label215');" onmouseout="ContentUnpreview('label215');" title="click to collapse or expand..."> more... </a>
 <div id="label215" style="display:none">
 <table border="1">
 <tr>
 <td></td>
 <td colspan="1">Supported Version Ranges</td>
 </tr>
 <tr>
 <td>bandwidth</td>
 <td><code class="docutils literal notranslate">v7.4.4 -> 7.6.4 </code></td>
 </tr>
 <tr>
 <td>[auto]</td>
 <td><code class="docutils literal notranslate">v7.4.4 -> 7.6.4</code></td>
 <tr>
 <td>[20MHz]</td>
 <td><code class="docutils literal notranslate">v7.4.4 -> 7.6.4</code></td>
 <tr>
 <td>[40MHz]</td>
 <td><code class="docutils literal notranslate">v7.4.4 -> 7.6.4</code></td>
 <tr>
 <td>[80MHz]</td>
 <td><code class="docutils literal notranslate">v7.4.4 -> 7.6.4</code></td>
 </table>
 </div>
 </li>
                <li> <span class="li-head">beacon_interval</span> - Wi-Fi beacon interval in miliseconds (100 - 3500). <span class="li-normal">type: int</span>
 <a id='label216' href="javascript:ContentClick('label217', 'label216');" onmouseover="ContentPreview('label217');" onmouseout="ContentUnpreview('label217');" title="click to collapse or expand..."> more... </a>
 <div id="label217" style="display:none">
 <table border="1">
 <tr>
 <td></td>
 <td colspan="1">Supported Version Ranges</td>
 </tr>
 <tr>
 <td>beacon_interval</td>
 <td><code class="docutils literal notranslate">v7.4.4 -> 7.6.4 </code></td>
 </tr>
 </table>
 </div>
 </li>
                <li> <span class="li-head">bss_color</span> - Wi-Fi 802.11AX BSS color value (0 - 63, 0 = disable). <span class="li-normal">type: int</span>
 <a id='label218' href="javascript:ContentClick('label219', 'label218');" onmouseover="ContentPreview('label219');" onmouseout="ContentUnpreview('label219');" title="click to collapse or expand..."> more... </a>
 <div id="label219" style="display:none">
 <table border="1">
 <tr>
 <td></td>
 <td colspan="1">Supported Version Ranges</td>
 </tr>
 <tr>
 <td>bss_color</td>
 <td><code class="docutils literal notranslate">v7.4.4 -> 7.6.4 </code></td>
 </tr>
 </table>
 </div>
 </li>
                <li> <span class="li-head">bss_color_mode</span> - Wi-Fi 802.11AX BSS color mode. <span class="li-normal">type: str</span> <span class="li-normal">choices: auto, static</span>
 <a id='label220' href="javascript:ContentClick('label221', 'label220');" onmouseover="ContentPreview('label221');" onmouseout="ContentUnpreview('label221');" title="click to collapse or expand..."> more... </a>
 <div id="label221" style="display:none">
 <table border="1">
 <tr>
 <td></td>
 <td colspan="1">Supported Version Ranges</td>
 </tr>
 <tr>
 <td>bss_color_mode</td>
 <td><code class="docutils literal notranslate">v7.4.4 -> 7.6.4 </code></td>
 </tr>
 <tr>
 <td>[auto]</td>
 <td><code class="docutils literal notranslate">v7.4.4 -> 7.6.4</code></td>
 <tr>
 <td>[static]</td>
 <td><code class="docutils literal notranslate">v7.4.4 -> 7.6.4</code></td>
 </table>
 </div>
 </li>
                <li> <span class="li-head">channel</span> - Wi-Fi channels. <span class="li-normal">type: list</span> <span class="li-normal">choices: CH1, CH2, CH3, CH4, CH5, CH6, CH7, CH8, CH9, CH10, CH11</span>
 <a id='label222' href="javascript:ContentClick('label223', 'label222');" onmouseover="ContentPreview('label223');" onmouseout="ContentUnpreview('label223');" title="click to collapse or expand..."> more... </a>
 <div id="label223" style="display:none">
 <table border="1">
 <tr>
 <td></td>
 <td colspan="1">Supported Version Ranges</td>
 </tr>
 <tr>
 <td>channel</td>
 <td><code class="docutils literal notranslate">v7.4.4 -> 7.6.4 </code></td>
 </tr>
 <tr>
 <td>[CH1]</td>
 <td><code class="docutils literal notranslate">v7.4.4 -> 7.6.4</code></td>
 <tr>
 <td>[CH2]</td>
 <td><code class="docutils literal notranslate">v7.4.4 -> 7.6.4</code></td>
 <tr>
 <td>[CH3]</td>
 <td><code class="docutils literal notranslate">v7.4.4 -> 7.6.4</code></td>
 <tr>
 <td>[CH4]</td>
 <td><code class="docutils literal notranslate">v7.4.4 -> 7.6.4</code></td>
 <tr>
 <td>[CH5]</td>
 <td><code class="docutils literal notranslate">v7.4.4 -> 7.6.4</code></td>
 <tr>
 <td>[CH6]</td>
 <td><code class="docutils literal notranslate">v7.4.4 -> 7.6.4</code></td>
 <tr>
 <td>[CH7]</td>
 <td><code class="docutils literal notranslate">v7.4.4 -> 7.6.4</code></td>
 <tr>
 <td>[CH8]</td>
 <td><code class="docutils literal notranslate">v7.4.4 -> 7.6.4</code></td>
 <tr>
 <td>[CH9]</td>
 <td><code class="docutils literal notranslate">v7.4.4 -> 7.6.4</code></td>
 <tr>
 <td>[CH10]</td>
 <td><code class="docutils literal notranslate">v7.4.4 -> 7.6.4</code></td>
 <tr>
 <td>[CH11]</td>
 <td><code class="docutils literal notranslate">v7.4.4 -> 7.6.4</code></td>
 </table>
 </div>
 </li>
                <li> <span class="li-head">extension_channel</span> - Wi-Fi extension channel. <span class="li-normal">type: str</span> <span class="li-normal">choices: auto, higher, lower</span>
 <a id='label224' href="javascript:ContentClick('label225', 'label224');" onmouseover="ContentPreview('label225');" onmouseout="ContentUnpreview('label225');" title="click to collapse or expand..."> more... </a>
 <div id="label225" style="display:none">
 <table border="1">
 <tr>
 <td></td>
 <td colspan="1">Supported Version Ranges</td>
 </tr>
 <tr>
 <td>extension_channel</td>
 <td><code class="docutils literal notranslate">v7.4.4 -> 7.6.4 </code></td>
 </tr>
 <tr>
 <td>[auto]</td>
 <td><code class="docutils literal notranslate">v7.4.4 -> 7.6.4</code></td>
 <tr>
 <td>[higher]</td>
 <td><code class="docutils literal notranslate">v7.4.4 -> 7.6.4</code></td>
 <tr>
 <td>[lower]</td>
 <td><code class="docutils literal notranslate">v7.4.4 -> 7.6.4</code></td>
 </table>
 </div>
 </li>
                <li> <span class="li-head">guard_interval</span> - Wi-Fi guard interval. <span class="li-normal">type: str</span> <span class="li-normal">choices: auto, 400ns, 800ns</span>
 <a id='label226' href="javascript:ContentClick('label227', 'label226');" onmouseover="ContentPreview('label227');" onmouseout="ContentUnpreview('label227');" title="click to collapse or expand..."> more... </a>
 <div id="label227" style="display:none">
 <table border="1">
 <tr>
 <td></td>
 <td colspan="1">Supported Version Ranges</td>
 </tr>
 <tr>
 <td>guard_interval</td>
 <td><code class="docutils literal notranslate">v7.4.4 -> 7.6.4 </code></td>
 </tr>
 <tr>
 <td>[auto]</td>
 <td><code class="docutils literal notranslate">v7.4.4 -> 7.6.4</code></td>
 <tr>
 <td>[400ns]</td>
 <td><code class="docutils literal notranslate">v7.4.4 -> 7.6.4</code></td>
 <tr>
 <td>[800ns]</td>
 <td><code class="docutils literal notranslate">v7.4.4 -> 7.6.4</code></td>
 </table>
 </div>
 </li>
                <li> <span class="li-head">lan_ext_vap</span> - Wi-Fi LAN-Extention VAP. Select only one VAP. Source extension-controller.extender-vap.name. <span class="li-normal">type: str</span>
 <a id='label228' href="javascript:ContentClick('label229', 'label228');" onmouseover="ContentPreview('label229');" onmouseout="ContentUnpreview('label229');" title="click to collapse or expand..."> more... </a>
 <div id="label229" style="display:none">
 <table border="1">
 <tr>
 <td></td>
 <td colspan="1">Supported Version Ranges</td>
 </tr>
 <tr>
 <td>lan_ext_vap</td>
 <td><code class="docutils literal notranslate">v7.4.4 -> 7.6.4 </code></td>
 </tr>
 </table>
 </div>
 </li>
                <li> <span class="li-head">local_vaps</span> - Wi-Fi local VAP. Select up to three VAPs. <span class="li-normal">type: list</span> <span style="font-family:'Courier New'" class="li-required">member_path: wifi/radio_1/local_vaps:name</span>
 <a id='label230' href="javascript:ContentClick('label231', 'label230');" onmouseover="ContentPreview('label231');" onmouseout="ContentUnpreview('label231');" title="click to collapse or expand..."> more... </a>
 <div id="label231" style="display:none">
 <table border="1">
 <tr>
 <td></td><td colspan="1">Supported Version Ranges</td>
 </tr>
 <tr>
 <td>local_vaps</td>
 <td><code class="docutils literal notranslate">v7.4.4 -> 7.6.4 </code></td>
 </tr>
 </table>
 </div>
 </li>
                    <ul class="ul-self">
                    <li> <span class="li-head">name</span> - Wi-Fi local VAP name. Source extension-controller.extender-vap.name. <span class="li-normal">type: str</span> <span class="li-required">required: true</span>
 <a id='label232' href="javascript:ContentClick('label233', 'label232');" onmouseover="ContentPreview('label233');" onmouseout="ContentUnpreview('label233');" title="click to collapse or expand..."> more... </a>
 <div id="label233" style="display:none">
 <table border="1">
 <tr>
 <td></td>
 <td colspan="1">Supported Version Ranges</td>
 </tr>
 <tr>
 <td>name</td>
 <td><code class="docutils literal notranslate">v7.4.4 -> 7.6.4 </code></td>
 </tr>
 </table>
 </div>
 </li>
                    </ul>
                <li> <span class="li-head">max_clients</span> - Maximum number of Wi-Fi radio clients (0 - 512, 0 = unlimited). <span class="li-normal">type: int</span>
 <a id='label234' href="javascript:ContentClick('label235', 'label234');" onmouseover="ContentPreview('label235');" onmouseout="ContentUnpreview('label235');" title="click to collapse or expand..."> more... </a>
 <div id="label235" style="display:none">
 <table border="1">
 <tr>
 <td></td>
 <td colspan="1">Supported Version Ranges</td>
 </tr>
 <tr>
 <td>max_clients</td>
 <td><code class="docutils literal notranslate">v7.4.4 -> 7.6.4 </code></td>
 </tr>
 </table>
 </div>
 </li>
                <li> <span class="li-head">mode</span> - Wi-Fi radio mode AP(LAN mode) / Client(WAN mode). <span class="li-normal">type: str</span> <span class="li-normal">choices: AP, Client</span>
 <a id='label236' href="javascript:ContentClick('label237', 'label236');" onmouseover="ContentPreview('label237');" onmouseout="ContentUnpreview('label237');" title="click to collapse or expand..."> more... </a>
 <div id="label237" style="display:none">
 <table border="1">
 <tr>
 <td></td>
 <td colspan="1">Supported Version Ranges</td>
 </tr>
 <tr>
 <td>mode</td>
 <td><code class="docutils literal notranslate">v7.4.4 -> 7.6.4 </code></td>
 </tr>
 <tr>
 <td>[AP]</td>
 <td><code class="docutils literal notranslate">v7.4.4 -> 7.6.4</code></td>
 <tr>
 <td>[Client]</td>
 <td><code class="docutils literal notranslate">v7.4.4 -> 7.6.4</code></td>
 </table>
 </div>
 </li>
                <li> <span class="li-head">operating_standard</span> - Wi-Fi operating standard. <span class="li-normal">type: str</span> <span class="li-normal">choices: auto, 11A-N-AC-AX, 11A-N-AC, 11A-N, 11A, 11N-AC-AX, 11AC-AX, 11AC, 11N-AC, 11B-G-N-AX, 11B-G-N, 11B-G, 11B, 11G-N-AX, 11N-AX, 11AX, 11G-N, 11N, 11G</span>
 <a id='label238' href="javascript:ContentClick('label239', 'label238');" onmouseover="ContentPreview('label239');" onmouseout="ContentUnpreview('label239');" title="click to collapse or expand..."> more... </a>
 <div id="label239" style="display:none">
 <table border="1">
 <tr>
 <td></td>
 <td colspan="1">Supported Version Ranges</td>
 </tr>
 <tr>
 <td>operating_standard</td>
 <td><code class="docutils literal notranslate">v7.4.4 -> 7.6.4 </code></td>
 </tr>
 <tr>
 <td>[auto]</td>
 <td><code class="docutils literal notranslate">v7.4.4 -> 7.6.4</code></td>
 <tr>
 <td>[11A-N-AC-AX]</td>
 <td><code class="docutils literal notranslate">v7.4.4 -> 7.6.4</code></td>
 <tr>
 <td>[11A-N-AC]</td>
 <td><code class="docutils literal notranslate">v7.4.4 -> 7.6.4</code></td>
 <tr>
 <td>[11A-N]</td>
 <td><code class="docutils literal notranslate">v7.4.4 -> 7.6.4</code></td>
 <tr>
 <td>[11A]</td>
 <td><code class="docutils literal notranslate">v7.4.4 -> 7.6.4</code></td>
 <tr>
 <td>[11N-AC-AX]</td>
 <td><code class="docutils literal notranslate">v7.4.4 -> 7.6.4</code></td>
 <tr>
 <td>[11AC-AX]</td>
 <td><code class="docutils literal notranslate">v7.4.4 -> 7.6.4</code></td>
 <tr>
 <td>[11AC]</td>
 <td><code class="docutils literal notranslate">v7.4.4 -> 7.6.4</code></td>
 <tr>
 <td>[11N-AC]</td>
 <td><code class="docutils literal notranslate">v7.4.4 -> 7.6.4</code></td>
 <tr>
 <td>[11B-G-N-AX]</td>
 <td><code class="docutils literal notranslate">v7.4.4 -> 7.6.4</code></td>
 <tr>
 <td>[11B-G-N]</td>
 <td><code class="docutils literal notranslate">v7.4.4 -> 7.6.4</code></td>
 <tr>
 <td>[11B-G]</td>
 <td><code class="docutils literal notranslate">v7.4.4 -> 7.6.4</code></td>
 <tr>
 <td>[11B]</td>
 <td><code class="docutils literal notranslate">v7.4.4 -> 7.6.4</code></td>
 <tr>
 <td>[11G-N-AX]</td>
 <td><code class="docutils literal notranslate">v7.4.4 -> 7.6.4</code></td>
 <tr>
 <td>[11N-AX]</td>
 <td><code class="docutils literal notranslate">v7.4.4 -> 7.6.4</code></td>
 <tr>
 <td>[11AX]</td>
 <td><code class="docutils literal notranslate">v7.4.4 -> 7.6.4</code></td>
 <tr>
 <td>[11G-N]</td>
 <td><code class="docutils literal notranslate">v7.4.4 -> 7.6.4</code></td>
 <tr>
 <td>[11N]</td>
 <td><code class="docutils literal notranslate">v7.4.4 -> 7.6.4</code></td>
 <tr>
 <td>[11G]</td>
 <td><code class="docutils literal notranslate">v7.4.4 -> 7.6.4</code></td>
 </table>
 </div>
 </li>
                <li> <span class="li-head">power_level</span> - Wi-Fi power level in percent (0 - 100, 0 = auto). <span class="li-normal">type: int</span>
 <a id='label240' href="javascript:ContentClick('label241', 'label240');" onmouseover="ContentPreview('label241');" onmouseout="ContentUnpreview('label241');" title="click to collapse or expand..."> more... </a>
 <div id="label241" style="display:none">
 <table border="1">
 <tr>
 <td></td>
 <td colspan="1">Supported Version Ranges</td>
 </tr>
 <tr>
 <td>power_level</td>
 <td><code class="docutils literal notranslate">v7.4.4 -> 7.6.4 </code></td>
 </tr>
 </table>
 </div>
 </li>
                <li> <span class="li-head">set_80211d</span> - Enable/disable Wi-Fi 802.11d. <span class="li-normal">type: str</span> <span class="li-normal">choices: disable, enable</span>
 <a id='label242' href="javascript:ContentClick('label243', 'label242');" onmouseover="ContentPreview('label243');" onmouseout="ContentUnpreview('label243');" title="click to collapse or expand..."> more... </a>
 <div id="label243" style="display:none">
 <table border="1">
 <tr>
 <td></td>
 <td colspan="1">Supported Version Ranges</td>
 </tr>
 <tr>
 <td>set_80211d</td>
 <td><code class="docutils literal notranslate">v7.4.4 -> 7.6.4 </code></td>
 </tr>
 <tr>
 <td>[disable]</td>
 <td><code class="docutils literal notranslate">v7.4.4 -> 7.6.4</code></td>
 <tr>
 <td>[enable]</td>
 <td><code class="docutils literal notranslate">v7.4.4 -> 7.6.4</code></td>
 </table>
 </div>
 </li>
                <li> <span class="li-head">status</span> - Enable/disable Wi-Fi radio. <span class="li-normal">type: str</span> <span class="li-normal">choices: disable, enable</span>
 <a id='label244' href="javascript:ContentClick('label245', 'label244');" onmouseover="ContentPreview('label245');" onmouseout="ContentUnpreview('label245');" title="click to collapse or expand..."> more... </a>
 <div id="label245" style="display:none">
 <table border="1">
 <tr>
 <td></td>
 <td colspan="1">Supported Version Ranges</td>
 </tr>
 <tr>
 <td>status</td>
 <td><code class="docutils literal notranslate">v7.4.4 -> 7.6.4 </code></td>
 </tr>
 <tr>
 <td>[disable]</td>
 <td><code class="docutils literal notranslate">v7.4.4 -> 7.6.4</code></td>
 <tr>
 <td>[enable]</td>
 <td><code class="docutils literal notranslate">v7.4.4 -> 7.6.4</code></td>
 </table>
 </div>
 </li>
                </ul>
            <li> <span class="li-head">radio_2</span> - Radio-2 config for Wi-Fi 5GHz <span class="li-normal">type: dict</span>
 <a id='label246' href="javascript:ContentClick('label247', 'label246');" onmouseover="ContentPreview('label247');" onmouseout="ContentUnpreview('label247');" title="click to collapse or expand..."> more... </a>
 <div id="label247" style="display:none">
 <table border="1">
 <tr>
 <td></td><td colspan="1">Supported Version Ranges</td>
 </tr>
 <tr>
 <td>radio_2</td>
 <td><code class="docutils literal notranslate">v7.4.4 -> 7.6.4 </code></td>
 </tr>
 </table>
 </div>
 </li>
                <ul class="ul-self">
                <li> <span class="li-head">band</span> - Wi-Fi band selection 2.4GHz / 5GHz. <span class="li-normal">type: str</span> <span class="li-normal">choices: 5GHz</span>
 <a id='label248' href="javascript:ContentClick('label249', 'label248');" onmouseover="ContentPreview('label249');" onmouseout="ContentUnpreview('label249');" title="click to collapse or expand..."> more... </a>
 <div id="label249" style="display:none">
 <table border="1">
 <tr>
 <td></td>
 <td colspan="1">Supported Version Ranges</td>
 </tr>
 <tr>
 <td>band</td>
 <td><code class="docutils literal notranslate">v7.4.4 -> 7.6.4 </code></td>
 </tr>
 <tr>
 <td>[5GHz]</td>
 <td><code class="docutils literal notranslate">v7.4.4 -> 7.6.4</code></td>
 </table>
 </div>
 </li>
                <li> <span class="li-head">bandwidth</span> - Wi-Fi channel bandwidth. <span class="li-normal">type: str</span> <span class="li-normal">choices: auto, 20MHz, 40MHz, 80MHz</span>
 <a id='label250' href="javascript:ContentClick('label251', 'label250');" onmouseover="ContentPreview('label251');" onmouseout="ContentUnpreview('label251');" title="click to collapse or expand..."> more... </a>
 <div id="label251" style="display:none">
 <table border="1">
 <tr>
 <td></td>
 <td colspan="1">Supported Version Ranges</td>
 </tr>
 <tr>
 <td>bandwidth</td>
 <td><code class="docutils literal notranslate">v7.4.4 -> 7.6.4 </code></td>
 </tr>
 <tr>
 <td>[auto]</td>
 <td><code class="docutils literal notranslate">v7.4.4 -> 7.6.4</code></td>
 <tr>
 <td>[20MHz]</td>
 <td><code class="docutils literal notranslate">v7.4.4 -> 7.6.4</code></td>
 <tr>
 <td>[40MHz]</td>
 <td><code class="docutils literal notranslate">v7.4.4 -> 7.6.4</code></td>
 <tr>
 <td>[80MHz]</td>
 <td><code class="docutils literal notranslate">v7.4.4 -> 7.6.4</code></td>
 </table>
 </div>
 </li>
                <li> <span class="li-head">beacon_interval</span> - Wi-Fi beacon interval in miliseconds (100 - 3500). <span class="li-normal">type: int</span>
 <a id='label252' href="javascript:ContentClick('label253', 'label252');" onmouseover="ContentPreview('label253');" onmouseout="ContentUnpreview('label253');" title="click to collapse or expand..."> more... </a>
 <div id="label253" style="display:none">
 <table border="1">
 <tr>
 <td></td>
 <td colspan="1">Supported Version Ranges</td>
 </tr>
 <tr>
 <td>beacon_interval</td>
 <td><code class="docutils literal notranslate">v7.4.4 -> 7.6.4 </code></td>
 </tr>
 </table>
 </div>
 </li>
                <li> <span class="li-head">bss_color</span> - Wi-Fi 802.11AX BSS color value (0 - 63, 0 = disable). <span class="li-normal">type: int</span>
 <a id='label254' href="javascript:ContentClick('label255', 'label254');" onmouseover="ContentPreview('label255');" onmouseout="ContentUnpreview('label255');" title="click to collapse or expand..."> more... </a>
 <div id="label255" style="display:none">
 <table border="1">
 <tr>
 <td></td>
 <td colspan="1">Supported Version Ranges</td>
 </tr>
 <tr>
 <td>bss_color</td>
 <td><code class="docutils literal notranslate">v7.4.4 -> 7.6.4 </code></td>
 </tr>
 </table>
 </div>
 </li>
                <li> <span class="li-head">bss_color_mode</span> - Wi-Fi 802.11AX BSS color mode. <span class="li-normal">type: str</span> <span class="li-normal">choices: auto, static</span>
 <a id='label256' href="javascript:ContentClick('label257', 'label256');" onmouseover="ContentPreview('label257');" onmouseout="ContentUnpreview('label257');" title="click to collapse or expand..."> more... </a>
 <div id="label257" style="display:none">
 <table border="1">
 <tr>
 <td></td>
 <td colspan="1">Supported Version Ranges</td>
 </tr>
 <tr>
 <td>bss_color_mode</td>
 <td><code class="docutils literal notranslate">v7.4.4 -> 7.6.4 </code></td>
 </tr>
 <tr>
 <td>[auto]</td>
 <td><code class="docutils literal notranslate">v7.4.4 -> 7.6.4</code></td>
 <tr>
 <td>[static]</td>
 <td><code class="docutils literal notranslate">v7.4.4 -> 7.6.4</code></td>
 </table>
 </div>
 </li>
                <li> <span class="li-head">channel</span> - Wi-Fi channels. <span class="li-normal">type: list</span> <span class="li-normal">choices: CH36, CH40, CH44, CH48, CH52, CH56, CH60, CH64, CH100, CH104, CH108, CH112, CH116, CH120, CH124, CH128, CH132, CH136, CH140, CH144, CH149, CH153, CH157, CH161, CH165</span>
 <a id='label258' href="javascript:ContentClick('label259', 'label258');" onmouseover="ContentPreview('label259');" onmouseout="ContentUnpreview('label259');" title="click to collapse or expand..."> more... </a>
 <div id="label259" style="display:none">
 <table border="1">
 <tr>
 <td></td>
 <td colspan="1">Supported Version Ranges</td>
 </tr>
 <tr>
 <td>channel</td>
 <td><code class="docutils literal notranslate">v7.4.4 -> 7.6.4 </code></td>
 </tr>
 <tr>
 <td>[CH36]</td>
 <td><code class="docutils literal notranslate">v7.4.4 -> 7.6.4</code></td>
 <tr>
 <td>[CH40]</td>
 <td><code class="docutils literal notranslate">v7.4.4 -> 7.6.4</code></td>
 <tr>
 <td>[CH44]</td>
 <td><code class="docutils literal notranslate">v7.4.4 -> 7.6.4</code></td>
 <tr>
 <td>[CH48]</td>
 <td><code class="docutils literal notranslate">v7.4.4 -> 7.6.4</code></td>
 <tr>
 <td>[CH52]</td>
 <td><code class="docutils literal notranslate">v7.4.4 -> 7.6.4</code></td>
 <tr>
 <td>[CH56]</td>
 <td><code class="docutils literal notranslate">v7.4.4 -> 7.6.4</code></td>
 <tr>
 <td>[CH60]</td>
 <td><code class="docutils literal notranslate">v7.4.4 -> 7.6.4</code></td>
 <tr>
 <td>[CH64]</td>
 <td><code class="docutils literal notranslate">v7.4.4 -> 7.6.4</code></td>
 <tr>
 <td>[CH100]</td>
 <td><code class="docutils literal notranslate">v7.4.4 -> 7.6.4</code></td>
 <tr>
 <td>[CH104]</td>
 <td><code class="docutils literal notranslate">v7.4.4 -> 7.6.4</code></td>
 <tr>
 <td>[CH108]</td>
 <td><code class="docutils literal notranslate">v7.4.4 -> 7.6.4</code></td>
 <tr>
 <td>[CH112]</td>
 <td><code class="docutils literal notranslate">v7.4.4 -> 7.6.4</code></td>
 <tr>
 <td>[CH116]</td>
 <td><code class="docutils literal notranslate">v7.4.4 -> 7.6.4</code></td>
 <tr>
 <td>[CH120]</td>
 <td><code class="docutils literal notranslate">v7.4.4 -> 7.6.4</code></td>
 <tr>
 <td>[CH124]</td>
 <td><code class="docutils literal notranslate">v7.4.4 -> 7.6.4</code></td>
 <tr>
 <td>[CH128]</td>
 <td><code class="docutils literal notranslate">v7.4.4 -> 7.6.4</code></td>
 <tr>
 <td>[CH132]</td>
 <td><code class="docutils literal notranslate">v7.4.4 -> 7.6.4</code></td>
 <tr>
 <td>[CH136]</td>
 <td><code class="docutils literal notranslate">v7.4.4 -> 7.6.4</code></td>
 <tr>
 <td>[CH140]</td>
 <td><code class="docutils literal notranslate">v7.4.4 -> 7.6.4</code></td>
 <tr>
 <td>[CH144]</td>
 <td><code class="docutils literal notranslate">v7.4.4 -> 7.6.4</code></td>
 <tr>
 <td>[CH149]</td>
 <td><code class="docutils literal notranslate">v7.4.4 -> 7.6.4</code></td>
 <tr>
 <td>[CH153]</td>
 <td><code class="docutils literal notranslate">v7.4.4 -> 7.6.4</code></td>
 <tr>
 <td>[CH157]</td>
 <td><code class="docutils literal notranslate">v7.4.4 -> 7.6.4</code></td>
 <tr>
 <td>[CH161]</td>
 <td><code class="docutils literal notranslate">v7.4.4 -> 7.6.4</code></td>
 <tr>
 <td>[CH165]</td>
 <td><code class="docutils literal notranslate">v7.4.4 -> 7.6.4</code></td>
 </table>
 </div>
 </li>
                <li> <span class="li-head">extension_channel</span> - Wi-Fi extension channel. <span class="li-normal">type: str</span> <span class="li-normal">choices: auto, higher, lower</span>
 <a id='label260' href="javascript:ContentClick('label261', 'label260');" onmouseover="ContentPreview('label261');" onmouseout="ContentUnpreview('label261');" title="click to collapse or expand..."> more... </a>
 <div id="label261" style="display:none">
 <table border="1">
 <tr>
 <td></td>
 <td colspan="1">Supported Version Ranges</td>
 </tr>
 <tr>
 <td>extension_channel</td>
 <td><code class="docutils literal notranslate">v7.4.4 -> 7.6.4 </code></td>
 </tr>
 <tr>
 <td>[auto]</td>
 <td><code class="docutils literal notranslate">v7.4.4 -> 7.6.4</code></td>
 <tr>
 <td>[higher]</td>
 <td><code class="docutils literal notranslate">v7.4.4 -> 7.6.4</code></td>
 <tr>
 <td>[lower]</td>
 <td><code class="docutils literal notranslate">v7.4.4 -> 7.6.4</code></td>
 </table>
 </div>
 </li>
                <li> <span class="li-head">guard_interval</span> - Wi-Fi guard interval. <span class="li-normal">type: str</span> <span class="li-normal">choices: auto, 400ns, 800ns</span>
 <a id='label262' href="javascript:ContentClick('label263', 'label262');" onmouseover="ContentPreview('label263');" onmouseout="ContentUnpreview('label263');" title="click to collapse or expand..."> more... </a>
 <div id="label263" style="display:none">
 <table border="1">
 <tr>
 <td></td>
 <td colspan="1">Supported Version Ranges</td>
 </tr>
 <tr>
 <td>guard_interval</td>
 <td><code class="docutils literal notranslate">v7.4.4 -> 7.6.4 </code></td>
 </tr>
 <tr>
 <td>[auto]</td>
 <td><code class="docutils literal notranslate">v7.4.4 -> 7.6.4</code></td>
 <tr>
 <td>[400ns]</td>
 <td><code class="docutils literal notranslate">v7.4.4 -> 7.6.4</code></td>
 <tr>
 <td>[800ns]</td>
 <td><code class="docutils literal notranslate">v7.4.4 -> 7.6.4</code></td>
 </table>
 </div>
 </li>
                <li> <span class="li-head">lan_ext_vap</span> - Wi-Fi LAN-Extention VAP. Select only one VAP. Source extension-controller.extender-vap.name. <span class="li-normal">type: str</span>
 <a id='label264' href="javascript:ContentClick('label265', 'label264');" onmouseover="ContentPreview('label265');" onmouseout="ContentUnpreview('label265');" title="click to collapse or expand..."> more... </a>
 <div id="label265" style="display:none">
 <table border="1">
 <tr>
 <td></td>
 <td colspan="1">Supported Version Ranges</td>
 </tr>
 <tr>
 <td>lan_ext_vap</td>
 <td><code class="docutils literal notranslate">v7.4.4 -> 7.6.4 </code></td>
 </tr>
 </table>
 </div>
 </li>
                <li> <span class="li-head">local_vaps</span> - Wi-Fi local VAP. Select up to three VAPs. <span class="li-normal">type: list</span> <span style="font-family:'Courier New'" class="li-required">member_path: wifi/radio_2/local_vaps:name</span>
 <a id='label266' href="javascript:ContentClick('label267', 'label266');" onmouseover="ContentPreview('label267');" onmouseout="ContentUnpreview('label267');" title="click to collapse or expand..."> more... </a>
 <div id="label267" style="display:none">
 <table border="1">
 <tr>
 <td></td><td colspan="1">Supported Version Ranges</td>
 </tr>
 <tr>
 <td>local_vaps</td>
 <td><code class="docutils literal notranslate">v7.4.4 -> 7.6.4 </code></td>
 </tr>
 </table>
 </div>
 </li>
                    <ul class="ul-self">
                    <li> <span class="li-head">name</span> - Wi-Fi local VAP name. Source extension-controller.extender-vap.name. <span class="li-normal">type: str</span> <span class="li-required">required: true</span>
 <a id='label268' href="javascript:ContentClick('label269', 'label268');" onmouseover="ContentPreview('label269');" onmouseout="ContentUnpreview('label269');" title="click to collapse or expand..."> more... </a>
 <div id="label269" style="display:none">
 <table border="1">
 <tr>
 <td></td>
 <td colspan="1">Supported Version Ranges</td>
 </tr>
 <tr>
 <td>name</td>
 <td><code class="docutils literal notranslate">v7.4.4 -> 7.6.4 </code></td>
 </tr>
 </table>
 </div>
 </li>
                    </ul>
                <li> <span class="li-head">max_clients</span> - Maximum number of Wi-Fi radio clients (0 - 512, 0 = unlimited). <span class="li-normal">type: int</span>
 <a id='label270' href="javascript:ContentClick('label271', 'label270');" onmouseover="ContentPreview('label271');" onmouseout="ContentUnpreview('label271');" title="click to collapse or expand..."> more... </a>
 <div id="label271" style="display:none">
 <table border="1">
 <tr>
 <td></td>
 <td colspan="1">Supported Version Ranges</td>
 </tr>
 <tr>
 <td>max_clients</td>
 <td><code class="docutils literal notranslate">v7.4.4 -> 7.6.4 </code></td>
 </tr>
 </table>
 </div>
 </li>
                <li> <span class="li-head">mode</span> - Wi-Fi radio mode AP(LAN mode) / Client(WAN mode). <span class="li-normal">type: str</span> <span class="li-normal">choices: AP, Client</span>
 <a id='label272' href="javascript:ContentClick('label273', 'label272');" onmouseover="ContentPreview('label273');" onmouseout="ContentUnpreview('label273');" title="click to collapse or expand..."> more... </a>
 <div id="label273" style="display:none">
 <table border="1">
 <tr>
 <td></td>
 <td colspan="1">Supported Version Ranges</td>
 </tr>
 <tr>
 <td>mode</td>
 <td><code class="docutils literal notranslate">v7.4.4 -> 7.6.4 </code></td>
 </tr>
 <tr>
 <td>[AP]</td>
 <td><code class="docutils literal notranslate">v7.4.4 -> 7.6.4</code></td>
 <tr>
 <td>[Client]</td>
 <td><code class="docutils literal notranslate">v7.4.4 -> 7.6.4</code></td>
 </table>
 </div>
 </li>
                <li> <span class="li-head">operating_standard</span> - Wi-Fi operating standard. <span class="li-normal">type: str</span> <span class="li-normal">choices: auto, 11A-N-AC-AX, 11A-N-AC, 11A-N, 11A, 11N-AC-AX, 11AC-AX, 11AC, 11N-AC, 11B-G-N-AX, 11B-G-N, 11B-G, 11B, 11G-N-AX, 11N-AX, 11AX, 11G-N, 11N, 11G</span>
 <a id='label274' href="javascript:ContentClick('label275', 'label274');" onmouseover="ContentPreview('label275');" onmouseout="ContentUnpreview('label275');" title="click to collapse or expand..."> more... </a>
 <div id="label275" style="display:none">
 <table border="1">
 <tr>
 <td></td>
 <td colspan="1">Supported Version Ranges</td>
 </tr>
 <tr>
 <td>operating_standard</td>
 <td><code class="docutils literal notranslate">v7.4.4 -> 7.6.4 </code></td>
 </tr>
 <tr>
 <td>[auto]</td>
 <td><code class="docutils literal notranslate">v7.4.4 -> 7.6.4</code></td>
 <tr>
 <td>[11A-N-AC-AX]</td>
 <td><code class="docutils literal notranslate">v7.4.4 -> 7.6.4</code></td>
 <tr>
 <td>[11A-N-AC]</td>
 <td><code class="docutils literal notranslate">v7.4.4 -> 7.6.4</code></td>
 <tr>
 <td>[11A-N]</td>
 <td><code class="docutils literal notranslate">v7.4.4 -> 7.6.4</code></td>
 <tr>
 <td>[11A]</td>
 <td><code class="docutils literal notranslate">v7.4.4 -> 7.6.4</code></td>
 <tr>
 <td>[11N-AC-AX]</td>
 <td><code class="docutils literal notranslate">v7.4.4 -> 7.6.4</code></td>
 <tr>
 <td>[11AC-AX]</td>
 <td><code class="docutils literal notranslate">v7.4.4 -> 7.6.4</code></td>
 <tr>
 <td>[11AC]</td>
 <td><code class="docutils literal notranslate">v7.4.4 -> 7.6.4</code></td>
 <tr>
 <td>[11N-AC]</td>
 <td><code class="docutils literal notranslate">v7.4.4 -> 7.6.4</code></td>
 <tr>
 <td>[11B-G-N-AX]</td>
 <td><code class="docutils literal notranslate">v7.4.4 -> 7.6.4</code></td>
 <tr>
 <td>[11B-G-N]</td>
 <td><code class="docutils literal notranslate">v7.4.4 -> 7.6.4</code></td>
 <tr>
 <td>[11B-G]</td>
 <td><code class="docutils literal notranslate">v7.4.4 -> 7.6.4</code></td>
 <tr>
 <td>[11B]</td>
 <td><code class="docutils literal notranslate">v7.4.4 -> 7.6.4</code></td>
 <tr>
 <td>[11G-N-AX]</td>
 <td><code class="docutils literal notranslate">v7.4.4 -> 7.6.4</code></td>
 <tr>
 <td>[11N-AX]</td>
 <td><code class="docutils literal notranslate">v7.4.4 -> 7.6.4</code></td>
 <tr>
 <td>[11AX]</td>
 <td><code class="docutils literal notranslate">v7.4.4 -> 7.6.4</code></td>
 <tr>
 <td>[11G-N]</td>
 <td><code class="docutils literal notranslate">v7.4.4 -> 7.6.4</code></td>
 <tr>
 <td>[11N]</td>
 <td><code class="docutils literal notranslate">v7.4.4 -> 7.6.4</code></td>
 <tr>
 <td>[11G]</td>
 <td><code class="docutils literal notranslate">v7.4.4 -> 7.6.4</code></td>
 </table>
 </div>
 </li>
                <li> <span class="li-head">power_level</span> - Wi-Fi power level in percent (0 - 100, 0 = auto). <span class="li-normal">type: int</span>
 <a id='label276' href="javascript:ContentClick('label277', 'label276');" onmouseover="ContentPreview('label277');" onmouseout="ContentUnpreview('label277');" title="click to collapse or expand..."> more... </a>
 <div id="label277" style="display:none">
 <table border="1">
 <tr>
 <td></td>
 <td colspan="1">Supported Version Ranges</td>
 </tr>
 <tr>
 <td>power_level</td>
 <td><code class="docutils literal notranslate">v7.4.4 -> 7.6.4 </code></td>
 </tr>
 </table>
 </div>
 </li>
                <li> <span class="li-head">set_80211d</span> - Enable/disable Wi-Fi 802.11d. <span class="li-normal">type: str</span> <span class="li-normal">choices: disable, enable</span>
 <a id='label278' href="javascript:ContentClick('label279', 'label278');" onmouseover="ContentPreview('label279');" onmouseout="ContentUnpreview('label279');" title="click to collapse or expand..."> more... </a>
 <div id="label279" style="display:none">
 <table border="1">
 <tr>
 <td></td>
 <td colspan="1">Supported Version Ranges</td>
 </tr>
 <tr>
 <td>set_80211d</td>
 <td><code class="docutils literal notranslate">v7.4.4 -> 7.6.4 </code></td>
 </tr>
 <tr>
 <td>[disable]</td>
 <td><code class="docutils literal notranslate">v7.4.4 -> 7.6.4</code></td>
 <tr>
 <td>[enable]</td>
 <td><code class="docutils literal notranslate">v7.4.4 -> 7.6.4</code></td>
 </table>
 </div>
 </li>
                <li> <span class="li-head">status</span> - Enable/disable Wi-Fi radio. <span class="li-normal">type: str</span> <span class="li-normal">choices: disable, enable</span>
 <a id='label280' href="javascript:ContentClick('label281', 'label280');" onmouseover="ContentPreview('label281');" onmouseout="ContentUnpreview('label281');" title="click to collapse or expand..."> more... </a>
 <div id="label281" style="display:none">
 <table border="1">
 <tr>
 <td></td>
 <td colspan="1">Supported Version Ranges</td>
 </tr>
 <tr>
 <td>status</td>
 <td><code class="docutils literal notranslate">v7.4.4 -> 7.6.4 </code></td>
 </tr>
 <tr>
 <td>[disable]</td>
 <td><code class="docutils literal notranslate">v7.4.4 -> 7.6.4</code></td>
 <tr>
 <td>[enable]</td>
 <td><code class="docutils literal notranslate">v7.4.4 -> 7.6.4</code></td>
 </table>
 </div>
 </li>
                </ul>
            </ul>
        </ul>
    </ul>


Notes
-----

.. note::

   - Legacy fortiosapi has been deprecated, httpapi is the preferred way to run playbooks

   - The module supports check_mode.



Examples
--------

.. code-block:: yaml+jinja
    
    - name: FortiExtender extender profile configuration.
      fortinet.fortios.fortios_extension_controller_extender_profile:
          vdom: "{{ vdom }}"
          state: "present"
          access_token: "<your_own_value>"
          extension_controller_extender_profile:
              allowaccess: "ping"
              bandwidth_limit: "1024"
              cellular:
                  controller_report:
                      interval: "300"
                      signal_threshold: "10"
                      status: "disable"
                  dataplan:
                      -
                          name: "default_name_11 (source extension-controller.dataplan.name)"
                  modem1:
                      auto_switch:
                          dataplan: "disable"
                          disconnect: "disable"
                          disconnect_period: "600"
                          disconnect_threshold: "3"
                          signal: "disable"
                          switch_back: "time"
                          switch_back_time: "<your_own_value>"
                          switch_back_timer: "86400"
                      default_sim: "sim1"
                      gps: "disable"
                      multiple_PDN: "disable"
                      pdn1_dataplan: "<your_own_value> (source extension-controller.dataplan.name)"
                      pdn2_dataplan: "<your_own_value> (source extension-controller.dataplan.name)"
                      pdn3_dataplan: "<your_own_value> (source extension-controller.dataplan.name)"
                      pdn4_dataplan: "<your_own_value> (source extension-controller.dataplan.name)"
                      preferred_carrier: "<your_own_value>"
                      redundant_intf: "<your_own_value>"
                      redundant_mode: "disable"
                      sim1_pin: "disable"
                      sim1_pin_code: "<your_own_value>"
                      sim2_pin: "disable"
                      sim2_pin_code: "<your_own_value>"
                  modem2:
                      auto_switch:
                          dataplan: "disable"
                          disconnect: "disable"
                          disconnect_period: "600"
                          disconnect_threshold: "3"
                          signal: "disable"
                          switch_back: "time"
                          switch_back_time: "<your_own_value>"
                          switch_back_timer: "86400"
                      default_sim: "sim1"
                      gps: "disable"
                      multiple_PDN: "disable"
                      pdn1_dataplan: "<your_own_value> (source extension-controller.dataplan.name)"
                      pdn2_dataplan: "<your_own_value> (source extension-controller.dataplan.name)"
                      pdn3_dataplan: "<your_own_value> (source extension-controller.dataplan.name)"
                      pdn4_dataplan: "<your_own_value> (source extension-controller.dataplan.name)"
                      preferred_carrier: "<your_own_value>"
                      redundant_intf: "<your_own_value>"
                      redundant_mode: "disable"
                      sim1_pin: "disable"
                      sim1_pin_code: "<your_own_value>"
                      sim2_pin: "disable"
                      sim2_pin_code: "<your_own_value>"
                  sms_notification:
                      alert:
                          data_exhausted: "<your_own_value>"
                          fgt_backup_mode_switch: "<your_own_value>"
                          low_signal_strength: "<your_own_value>"
                          mode_switch: "<your_own_value>"
                          os_image_fallback: "<your_own_value>"
                          session_disconnect: "<your_own_value>"
                          system_reboot: "<your_own_value>"
                      receiver:
                          -
                              alert: "system-reboot"
                              name: "default_name_71"
                              phone_number: "<your_own_value>"
                              status: "disable"
                      status: "disable"
              enforce_bandwidth: "enable"
              extension: "wan-extension"
              id: "77"
              lan_extension:
                  backhaul:
                      -
                          name: "default_name_80"
                          port: "wan"
                          role: "primary"
                          weight: "1"
                  backhaul_interface: "<your_own_value> (source system.interface.name)"
                  backhaul_ip: "<your_own_value>"
                  downlinks:
                      -
                          name: "default_name_87"
                          port: "port1"
                          pvid: "1"
                          type: "port"
                          vap: "<your_own_value> (source extension-controller.extender-vap.name)"
                          vids:
                              -
                                  vid: "<you_own_value>"
                  ipsec_tunnel: "<your_own_value>"
                  link_loadbalance: "activebackup"
                  traffic_split_services:
                      -
                          address: "<your_own_value> (source firewall.address.name)"
                          name: "default_name_98"
                          service: "<your_own_value> (source firewall.service.custom.name)"
                          vsdb: "disable"
              login_password: "<your_own_value>"
              login_password_change: "yes"
              model: "FX201E"
              name: "default_name_104"
              wifi:
                  country: "--"
                  radio_1:
                      band: "2.4GHz"
                      bandwidth: "auto"
                      beacon_interval: "100"
                      bss_color: "0"
                      bss_color_mode: "auto"
                      channel: "CH1"
                      extension_channel: "auto"
                      guard_interval: "auto"
                      lan_ext_vap: "<your_own_value> (source extension-controller.extender-vap.name)"
                      local_vaps:
                          -
                              name: "default_name_118 (source extension-controller.extender-vap.name)"
                      max_clients: "0"
                      mode: "AP"
                      operating_standard: "auto"
                      power_level: "100"
                      set_80211d: "disable"
                      status: "disable"
                  radio_2:
                      band: "5GHz"
                      bandwidth: "auto"
                      beacon_interval: "100"
                      bss_color: "0"
                      bss_color_mode: "auto"
                      channel: "CH36"
                      extension_channel: "auto"
                      guard_interval: "auto"
                      lan_ext_vap: "<your_own_value> (source extension-controller.extender-vap.name)"
                      local_vaps:
                          -
                              name: "default_name_136 (source extension-controller.extender-vap.name)"
                      max_clients: "0"
                      mode: "AP"
                      operating_standard: "auto"
                      power_level: "100"
                      set_80211d: "disable"
                      status: "disable"


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
