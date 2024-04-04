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
Supported Version Ranges: v7.2.1 -> 7.4.3



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
 <td><code class="docutils literal notranslate">v7.2.1 -> 7.4.3 </code></td>
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
 <td><code class="docutils literal notranslate">v7.2.1 -> 7.4.3 </code></td>
 </tr>
 <tr>
 <td>[ping]</td>
 <td><code class="docutils literal notranslate">v7.2.1 -> 7.4.3</code></td>
 <tr>
 <td>[telnet]</td>
 <td><code class="docutils literal notranslate">v7.2.1 -> 7.4.3</code></td>
 <tr>
 <td>[http]</td>
 <td><code class="docutils literal notranslate">v7.2.1 -> 7.4.3</code></td>
 <tr>
 <td>[https]</td>
 <td><code class="docutils literal notranslate">v7.2.1 -> 7.4.3</code></td>
 <tr>
 <td>[ssh]</td>
 <td><code class="docutils literal notranslate">v7.2.1 -> 7.4.3</code></td>
 <tr>
 <td>[snmp]</td>
 <td><code class="docutils literal notranslate">v7.2.1 -> 7.4.3</code></td>
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
 <td><code class="docutils literal notranslate">v7.2.1 -> 7.4.3 </code></td>
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
 <td><code class="docutils literal notranslate">v7.2.1 -> 7.4.3 </code></td>
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
 <td><code class="docutils literal notranslate">v7.2.1 -> 7.4.3 </code></td>
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
 <td><code class="docutils literal notranslate">v7.2.1 -> 7.4.3 </code></td>
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
 <td><code class="docutils literal notranslate">v7.2.1 -> 7.4.3 </code></td>
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
 <td><code class="docutils literal notranslate">v7.2.1 -> 7.4.3 </code></td>
 </tr>
 <tr>
 <td>[disable]</td>
 <td><code class="docutils literal notranslate">v7.2.1 -> 7.4.3</code></td>
 <tr>
 <td>[enable]</td>
 <td><code class="docutils literal notranslate">v7.2.1 -> 7.4.3</code></td>
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
 <td><code class="docutils literal notranslate">v7.2.1 -> 7.4.3 </code></td>
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
 <td><code class="docutils literal notranslate">v7.2.1 -> 7.4.3 </code></td>
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
 <td><code class="docutils literal notranslate">v7.2.1 -> 7.4.3 </code></td>
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
 <td><code class="docutils literal notranslate">v7.2.1 -> 7.4.3 </code></td>
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
 <td><code class="docutils literal notranslate">v7.2.1 -> 7.4.3 </code></td>
 </tr>
 <tr>
 <td>[disable]</td>
 <td><code class="docutils literal notranslate">v7.2.1 -> 7.4.3</code></td>
 <tr>
 <td>[enable]</td>
 <td><code class="docutils literal notranslate">v7.2.1 -> 7.4.3</code></td>
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
 <td><code class="docutils literal notranslate">v7.2.1 -> 7.4.3 </code></td>
 </tr>
 <tr>
 <td>[disable]</td>
 <td><code class="docutils literal notranslate">v7.2.1 -> 7.4.3</code></td>
 <tr>
 <td>[enable]</td>
 <td><code class="docutils literal notranslate">v7.2.1 -> 7.4.3</code></td>
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
 <td><code class="docutils literal notranslate">v7.2.1 -> 7.4.3 </code></td>
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
 <td><code class="docutils literal notranslate">v7.2.1 -> 7.4.3 </code></td>
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
 <td><code class="docutils literal notranslate">v7.2.1 -> 7.4.3 </code></td>
 </tr>
 <tr>
 <td>[disable]</td>
 <td><code class="docutils literal notranslate">v7.2.1 -> 7.4.3</code></td>
 <tr>
 <td>[enable]</td>
 <td><code class="docutils literal notranslate">v7.2.1 -> 7.4.3</code></td>
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
 <td><code class="docutils literal notranslate">v7.2.1 -> 7.4.3 </code></td>
 </tr>
 <tr>
 <td>[time]</td>
 <td><code class="docutils literal notranslate">v7.2.1 -> 7.4.3</code></td>
 <tr>
 <td>[timer]</td>
 <td><code class="docutils literal notranslate">v7.2.1 -> 7.4.3</code></td>
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
 <td><code class="docutils literal notranslate">v7.2.1 -> 7.4.3 </code></td>
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
 <td><code class="docutils literal notranslate">v7.2.1 -> 7.4.3 </code></td>
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
 <td><code class="docutils literal notranslate">v7.2.1 -> 7.4.3 </code></td>
 </tr>
 <tr>
 <td>[sim1]</td>
 <td><code class="docutils literal notranslate">v7.2.1 -> 7.4.3</code></td>
 <tr>
 <td>[sim2]</td>
 <td><code class="docutils literal notranslate">v7.2.1 -> 7.4.3</code></td>
 <tr>
 <td>[carrier]</td>
 <td><code class="docutils literal notranslate">v7.2.1 -> 7.4.3</code></td>
 <tr>
 <td>[cost]</td>
 <td><code class="docutils literal notranslate">v7.2.1 -> 7.4.3</code></td>
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
 <td><code class="docutils literal notranslate">v7.2.1 -> 7.4.3 </code></td>
 </tr>
 <tr>
 <td>[disable]</td>
 <td><code class="docutils literal notranslate">v7.2.1 -> 7.4.3</code></td>
 <tr>
 <td>[enable]</td>
 <td><code class="docutils literal notranslate">v7.2.1 -> 7.4.3</code></td>
 </table>
 </div>
 </li>
                <li> <span class="li-head">preferred_carrier</span> - Preferred carrier. <span class="li-normal">type: str</span>
 <a id='label44' href="javascript:ContentClick('label45', 'label44');" onmouseover="ContentPreview('label45');" onmouseout="ContentUnpreview('label45');" title="click to collapse or expand..."> more... </a>
 <div id="label45" style="display:none">
 <table border="1">
 <tr>
 <td></td>
 <td colspan="1">Supported Version Ranges</td>
 </tr>
 <tr>
 <td>preferred_carrier</td>
 <td><code class="docutils literal notranslate">v7.2.1 -> 7.4.3 </code></td>
 </tr>
 </table>
 </div>
 </li>
                <li> <span class="li-head">redundant_intf</span> - Redundant interface. <span class="li-normal">type: str</span>
 <a id='label46' href="javascript:ContentClick('label47', 'label46');" onmouseover="ContentPreview('label47');" onmouseout="ContentUnpreview('label47');" title="click to collapse or expand..."> more... </a>
 <div id="label47" style="display:none">
 <table border="1">
 <tr>
 <td></td>
 <td colspan="1">Supported Version Ranges</td>
 </tr>
 <tr>
 <td>redundant_intf</td>
 <td><code class="docutils literal notranslate">v7.2.1 -> 7.4.3 </code></td>
 </tr>
 </table>
 </div>
 </li>
                <li> <span class="li-head">redundant_mode</span> - FortiExtender mode. <span class="li-normal">type: str</span> <span class="li-normal">choices: disable, enable</span>
 <a id='label48' href="javascript:ContentClick('label49', 'label48');" onmouseover="ContentPreview('label49');" onmouseout="ContentUnpreview('label49');" title="click to collapse or expand..."> more... </a>
 <div id="label49" style="display:none">
 <table border="1">
 <tr>
 <td></td>
 <td colspan="1">Supported Version Ranges</td>
 </tr>
 <tr>
 <td>redundant_mode</td>
 <td><code class="docutils literal notranslate">v7.2.1 -> 7.4.3 </code></td>
 </tr>
 <tr>
 <td>[disable]</td>
 <td><code class="docutils literal notranslate">v7.2.1 -> 7.4.3</code></td>
 <tr>
 <td>[enable]</td>
 <td><code class="docutils literal notranslate">v7.2.1 -> 7.4.3</code></td>
 </table>
 </div>
 </li>
                <li> <span class="li-head">sim1_pin</span> - SIM <span class="li-normal">type: str</span> <span class="li-normal">choices: disable, enable</span>
 <a id='label50' href="javascript:ContentClick('label51', 'label50');" onmouseover="ContentPreview('label51');" onmouseout="ContentUnpreview('label51');" title="click to collapse or expand..."> more... </a>
 <div id="label51" style="display:none">
 <table border="1">
 <tr>
 <td></td>
 <td colspan="1">Supported Version Ranges</td>
 </tr>
 <tr>
 <td>sim1_pin</td>
 <td><code class="docutils literal notranslate">v7.2.1 -> 7.4.3 </code></td>
 </tr>
 <tr>
 <td>[disable]</td>
 <td><code class="docutils literal notranslate">v7.2.1 -> 7.4.3</code></td>
 <tr>
 <td>[enable]</td>
 <td><code class="docutils literal notranslate">v7.2.1 -> 7.4.3</code></td>
 </table>
 </div>
 </li>
                <li> <span class="li-head">sim1_pin_code</span> - SIM <span class="li-normal">type: str</span>
 <a id='label52' href="javascript:ContentClick('label53', 'label52');" onmouseover="ContentPreview('label53');" onmouseout="ContentUnpreview('label53');" title="click to collapse or expand..."> more... </a>
 <div id="label53" style="display:none">
 <table border="1">
 <tr>
 <td></td>
 <td colspan="1">Supported Version Ranges</td>
 </tr>
 <tr>
 <td>sim1_pin_code</td>
 <td><code class="docutils literal notranslate">v7.2.1 -> 7.4.3 </code></td>
 </tr>
 </table>
 </div>
 </li>
                <li> <span class="li-head">sim2_pin</span> - SIM <span class="li-normal">type: str</span> <span class="li-normal">choices: disable, enable</span>
 <a id='label54' href="javascript:ContentClick('label55', 'label54');" onmouseover="ContentPreview('label55');" onmouseout="ContentUnpreview('label55');" title="click to collapse or expand..."> more... </a>
 <div id="label55" style="display:none">
 <table border="1">
 <tr>
 <td></td>
 <td colspan="1">Supported Version Ranges</td>
 </tr>
 <tr>
 <td>sim2_pin</td>
 <td><code class="docutils literal notranslate">v7.2.1 -> 7.4.3 </code></td>
 </tr>
 <tr>
 <td>[disable]</td>
 <td><code class="docutils literal notranslate">v7.2.1 -> 7.4.3</code></td>
 <tr>
 <td>[enable]</td>
 <td><code class="docutils literal notranslate">v7.2.1 -> 7.4.3</code></td>
 </table>
 </div>
 </li>
                <li> <span class="li-head">sim2_pin_code</span> - SIM <span class="li-normal">type: str</span>
 <a id='label56' href="javascript:ContentClick('label57', 'label56');" onmouseover="ContentPreview('label57');" onmouseout="ContentUnpreview('label57');" title="click to collapse or expand..."> more... </a>
 <div id="label57" style="display:none">
 <table border="1">
 <tr>
 <td></td>
 <td colspan="1">Supported Version Ranges</td>
 </tr>
 <tr>
 <td>sim2_pin_code</td>
 <td><code class="docutils literal notranslate">v7.2.1 -> 7.4.3 </code></td>
 </tr>
 </table>
 </div>
 </li>
                </ul>
            <li> <span class="li-head">modem2</span> - Configuration options for modem 2. <span class="li-normal">type: dict</span>
 <a id='label58' href="javascript:ContentClick('label59', 'label58');" onmouseover="ContentPreview('label59');" onmouseout="ContentUnpreview('label59');" title="click to collapse or expand..."> more... </a>
 <div id="label59" style="display:none">
 <table border="1">
 <tr>
 <td></td><td colspan="1">Supported Version Ranges</td>
 </tr>
 <tr>
 <td>modem2</td>
 <td><code class="docutils literal notranslate">v7.2.1 -> 7.4.3 </code></td>
 </tr>
 </table>
 </div>
 </li>
                <ul class="ul-self">
                <li> <span class="li-head">auto_switch</span> - FortiExtender auto switch configuration. <span class="li-normal">type: dict</span>
 <a id='label60' href="javascript:ContentClick('label61', 'label60');" onmouseover="ContentPreview('label61');" onmouseout="ContentUnpreview('label61');" title="click to collapse or expand..."> more... </a>
 <div id="label61" style="display:none">
 <table border="1">
 <tr>
 <td></td><td colspan="1">Supported Version Ranges</td>
 </tr>
 <tr>
 <td>auto_switch</td>
 <td><code class="docutils literal notranslate">v7.2.1 -> 7.4.3 </code></td>
 </tr>
 </table>
 </div>
 </li>
                    <ul class="ul-self">
                    <li> <span class="li-head">dataplan</span> - Automatically switch based on data usage. <span class="li-normal">type: str</span> <span class="li-normal">choices: disable, enable</span>
 <a id='label62' href="javascript:ContentClick('label63', 'label62');" onmouseover="ContentPreview('label63');" onmouseout="ContentUnpreview('label63');" title="click to collapse or expand..."> more... </a>
 <div id="label63" style="display:none">
 <table border="1">
 <tr>
 <td></td>
 <td colspan="1">Supported Version Ranges</td>
 </tr>
 <tr>
 <td>dataplan</td>
 <td><code class="docutils literal notranslate">v7.2.1 -> 7.4.3 </code></td>
 </tr>
 <tr>
 <td>[disable]</td>
 <td><code class="docutils literal notranslate">v7.2.1 -> 7.4.3</code></td>
 <tr>
 <td>[enable]</td>
 <td><code class="docutils literal notranslate">v7.2.1 -> 7.4.3</code></td>
 </table>
 </div>
 </li>
                    <li> <span class="li-head">disconnect</span> - Auto switch by disconnect. <span class="li-normal">type: str</span> <span class="li-normal">choices: disable, enable</span>
 <a id='label64' href="javascript:ContentClick('label65', 'label64');" onmouseover="ContentPreview('label65');" onmouseout="ContentUnpreview('label65');" title="click to collapse or expand..."> more... </a>
 <div id="label65" style="display:none">
 <table border="1">
 <tr>
 <td></td>
 <td colspan="1">Supported Version Ranges</td>
 </tr>
 <tr>
 <td>disconnect</td>
 <td><code class="docutils literal notranslate">v7.2.1 -> 7.4.3 </code></td>
 </tr>
 <tr>
 <td>[disable]</td>
 <td><code class="docutils literal notranslate">v7.2.1 -> 7.4.3</code></td>
 <tr>
 <td>[enable]</td>
 <td><code class="docutils literal notranslate">v7.2.1 -> 7.4.3</code></td>
 </table>
 </div>
 </li>
                    <li> <span class="li-head">disconnect_period</span> - Automatically switch based on disconnect period. <span class="li-normal">type: int</span>
 <a id='label66' href="javascript:ContentClick('label67', 'label66');" onmouseover="ContentPreview('label67');" onmouseout="ContentUnpreview('label67');" title="click to collapse or expand..."> more... </a>
 <div id="label67" style="display:none">
 <table border="1">
 <tr>
 <td></td>
 <td colspan="1">Supported Version Ranges</td>
 </tr>
 <tr>
 <td>disconnect_period</td>
 <td><code class="docutils literal notranslate">v7.2.1 -> 7.4.3 </code></td>
 </tr>
 </table>
 </div>
 </li>
                    <li> <span class="li-head">disconnect_threshold</span> - Automatically switch based on disconnect threshold. <span class="li-normal">type: int</span>
 <a id='label68' href="javascript:ContentClick('label69', 'label68');" onmouseover="ContentPreview('label69');" onmouseout="ContentUnpreview('label69');" title="click to collapse or expand..."> more... </a>
 <div id="label69" style="display:none">
 <table border="1">
 <tr>
 <td></td>
 <td colspan="1">Supported Version Ranges</td>
 </tr>
 <tr>
 <td>disconnect_threshold</td>
 <td><code class="docutils literal notranslate">v7.2.1 -> 7.4.3 </code></td>
 </tr>
 </table>
 </div>
 </li>
                    <li> <span class="li-head">signal</span> - Automatically switch based on signal strength. <span class="li-normal">type: str</span> <span class="li-normal">choices: disable, enable</span>
 <a id='label70' href="javascript:ContentClick('label71', 'label70');" onmouseover="ContentPreview('label71');" onmouseout="ContentUnpreview('label71');" title="click to collapse or expand..."> more... </a>
 <div id="label71" style="display:none">
 <table border="1">
 <tr>
 <td></td>
 <td colspan="1">Supported Version Ranges</td>
 </tr>
 <tr>
 <td>signal</td>
 <td><code class="docutils literal notranslate">v7.2.1 -> 7.4.3 </code></td>
 </tr>
 <tr>
 <td>[disable]</td>
 <td><code class="docutils literal notranslate">v7.2.1 -> 7.4.3</code></td>
 <tr>
 <td>[enable]</td>
 <td><code class="docutils literal notranslate">v7.2.1 -> 7.4.3</code></td>
 </table>
 </div>
 </li>
                    <li> <span class="li-head">switch_back</span> - Auto switch with switch back multi-options. <span class="li-normal">type: list</span> <span class="li-normal">choices: time, timer</span>
 <a id='label72' href="javascript:ContentClick('label73', 'label72');" onmouseover="ContentPreview('label73');" onmouseout="ContentUnpreview('label73');" title="click to collapse or expand..."> more... </a>
 <div id="label73" style="display:none">
 <table border="1">
 <tr>
 <td></td>
 <td colspan="1">Supported Version Ranges</td>
 </tr>
 <tr>
 <td>switch_back</td>
 <td><code class="docutils literal notranslate">v7.2.1 -> 7.4.3 </code></td>
 </tr>
 <tr>
 <td>[time]</td>
 <td><code class="docutils literal notranslate">v7.2.1 -> 7.4.3</code></td>
 <tr>
 <td>[timer]</td>
 <td><code class="docutils literal notranslate">v7.2.1 -> 7.4.3</code></td>
 </table>
 </div>
 </li>
                    <li> <span class="li-head">switch_back_time</span> - Automatically switch over to preferred SIM/carrier at a specified time in UTC (HH:MM). <span class="li-normal">type: str</span>
 <a id='label74' href="javascript:ContentClick('label75', 'label74');" onmouseover="ContentPreview('label75');" onmouseout="ContentUnpreview('label75');" title="click to collapse or expand..."> more... </a>
 <div id="label75" style="display:none">
 <table border="1">
 <tr>
 <td></td>
 <td colspan="1">Supported Version Ranges</td>
 </tr>
 <tr>
 <td>switch_back_time</td>
 <td><code class="docutils literal notranslate">v7.2.1 -> 7.4.3 </code></td>
 </tr>
 </table>
 </div>
 </li>
                    <li> <span class="li-head">switch_back_timer</span> - Automatically switch over to preferred SIM/carrier after the given time (3600 - 2147483647 sec). <span class="li-normal">type: int</span>
 <a id='label76' href="javascript:ContentClick('label77', 'label76');" onmouseover="ContentPreview('label77');" onmouseout="ContentUnpreview('label77');" title="click to collapse or expand..."> more... </a>
 <div id="label77" style="display:none">
 <table border="1">
 <tr>
 <td></td>
 <td colspan="1">Supported Version Ranges</td>
 </tr>
 <tr>
 <td>switch_back_timer</td>
 <td><code class="docutils literal notranslate">v7.2.1 -> 7.4.3 </code></td>
 </tr>
 </table>
 </div>
 </li>
                    </ul>
                <li> <span class="li-head">default_sim</span> - Default SIM selection. <span class="li-normal">type: str</span> <span class="li-normal">choices: sim1, sim2, carrier, cost</span>
 <a id='label78' href="javascript:ContentClick('label79', 'label78');" onmouseover="ContentPreview('label79');" onmouseout="ContentUnpreview('label79');" title="click to collapse or expand..."> more... </a>
 <div id="label79" style="display:none">
 <table border="1">
 <tr>
 <td></td>
 <td colspan="1">Supported Version Ranges</td>
 </tr>
 <tr>
 <td>default_sim</td>
 <td><code class="docutils literal notranslate">v7.2.1 -> 7.4.3 </code></td>
 </tr>
 <tr>
 <td>[sim1]</td>
 <td><code class="docutils literal notranslate">v7.2.1 -> 7.4.3</code></td>
 <tr>
 <td>[sim2]</td>
 <td><code class="docutils literal notranslate">v7.2.1 -> 7.4.3</code></td>
 <tr>
 <td>[carrier]</td>
 <td><code class="docutils literal notranslate">v7.2.1 -> 7.4.3</code></td>
 <tr>
 <td>[cost]</td>
 <td><code class="docutils literal notranslate">v7.2.1 -> 7.4.3</code></td>
 </table>
 </div>
 </li>
                <li> <span class="li-head">gps</span> - FortiExtender GPS enable/disable. <span class="li-normal">type: str</span> <span class="li-normal">choices: disable, enable</span>
 <a id='label80' href="javascript:ContentClick('label81', 'label80');" onmouseover="ContentPreview('label81');" onmouseout="ContentUnpreview('label81');" title="click to collapse or expand..."> more... </a>
 <div id="label81" style="display:none">
 <table border="1">
 <tr>
 <td></td>
 <td colspan="1">Supported Version Ranges</td>
 </tr>
 <tr>
 <td>gps</td>
 <td><code class="docutils literal notranslate">v7.2.1 -> 7.4.3 </code></td>
 </tr>
 <tr>
 <td>[disable]</td>
 <td><code class="docutils literal notranslate">v7.2.1 -> 7.4.3</code></td>
 <tr>
 <td>[enable]</td>
 <td><code class="docutils literal notranslate">v7.2.1 -> 7.4.3</code></td>
 </table>
 </div>
 </li>
                <li> <span class="li-head">preferred_carrier</span> - Preferred carrier. <span class="li-normal">type: str</span>
 <a id='label82' href="javascript:ContentClick('label83', 'label82');" onmouseover="ContentPreview('label83');" onmouseout="ContentUnpreview('label83');" title="click to collapse or expand..."> more... </a>
 <div id="label83" style="display:none">
 <table border="1">
 <tr>
 <td></td>
 <td colspan="1">Supported Version Ranges</td>
 </tr>
 <tr>
 <td>preferred_carrier</td>
 <td><code class="docutils literal notranslate">v7.2.1 -> 7.4.3 </code></td>
 </tr>
 </table>
 </div>
 </li>
                <li> <span class="li-head">redundant_intf</span> - Redundant interface. <span class="li-normal">type: str</span>
 <a id='label84' href="javascript:ContentClick('label85', 'label84');" onmouseover="ContentPreview('label85');" onmouseout="ContentUnpreview('label85');" title="click to collapse or expand..."> more... </a>
 <div id="label85" style="display:none">
 <table border="1">
 <tr>
 <td></td>
 <td colspan="1">Supported Version Ranges</td>
 </tr>
 <tr>
 <td>redundant_intf</td>
 <td><code class="docutils literal notranslate">v7.2.1 -> 7.4.3 </code></td>
 </tr>
 </table>
 </div>
 </li>
                <li> <span class="li-head">redundant_mode</span> - FortiExtender mode. <span class="li-normal">type: str</span> <span class="li-normal">choices: disable, enable</span>
 <a id='label86' href="javascript:ContentClick('label87', 'label86');" onmouseover="ContentPreview('label87');" onmouseout="ContentUnpreview('label87');" title="click to collapse or expand..."> more... </a>
 <div id="label87" style="display:none">
 <table border="1">
 <tr>
 <td></td>
 <td colspan="1">Supported Version Ranges</td>
 </tr>
 <tr>
 <td>redundant_mode</td>
 <td><code class="docutils literal notranslate">v7.2.1 -> 7.4.3 </code></td>
 </tr>
 <tr>
 <td>[disable]</td>
 <td><code class="docutils literal notranslate">v7.2.1 -> 7.4.3</code></td>
 <tr>
 <td>[enable]</td>
 <td><code class="docutils literal notranslate">v7.2.1 -> 7.4.3</code></td>
 </table>
 </div>
 </li>
                <li> <span class="li-head">sim1_pin</span> - SIM <span class="li-normal">type: str</span> <span class="li-normal">choices: disable, enable</span>
 <a id='label88' href="javascript:ContentClick('label89', 'label88');" onmouseover="ContentPreview('label89');" onmouseout="ContentUnpreview('label89');" title="click to collapse or expand..."> more... </a>
 <div id="label89" style="display:none">
 <table border="1">
 <tr>
 <td></td>
 <td colspan="1">Supported Version Ranges</td>
 </tr>
 <tr>
 <td>sim1_pin</td>
 <td><code class="docutils literal notranslate">v7.2.1 -> 7.4.3 </code></td>
 </tr>
 <tr>
 <td>[disable]</td>
 <td><code class="docutils literal notranslate">v7.2.1 -> 7.4.3</code></td>
 <tr>
 <td>[enable]</td>
 <td><code class="docutils literal notranslate">v7.2.1 -> 7.4.3</code></td>
 </table>
 </div>
 </li>
                <li> <span class="li-head">sim1_pin_code</span> - SIM <span class="li-normal">type: str</span>
 <a id='label90' href="javascript:ContentClick('label91', 'label90');" onmouseover="ContentPreview('label91');" onmouseout="ContentUnpreview('label91');" title="click to collapse or expand..."> more... </a>
 <div id="label91" style="display:none">
 <table border="1">
 <tr>
 <td></td>
 <td colspan="1">Supported Version Ranges</td>
 </tr>
 <tr>
 <td>sim1_pin_code</td>
 <td><code class="docutils literal notranslate">v7.2.1 -> 7.4.3 </code></td>
 </tr>
 </table>
 </div>
 </li>
                <li> <span class="li-head">sim2_pin</span> - SIM <span class="li-normal">type: str</span> <span class="li-normal">choices: disable, enable</span>
 <a id='label92' href="javascript:ContentClick('label93', 'label92');" onmouseover="ContentPreview('label93');" onmouseout="ContentUnpreview('label93');" title="click to collapse or expand..."> more... </a>
 <div id="label93" style="display:none">
 <table border="1">
 <tr>
 <td></td>
 <td colspan="1">Supported Version Ranges</td>
 </tr>
 <tr>
 <td>sim2_pin</td>
 <td><code class="docutils literal notranslate">v7.2.1 -> 7.4.3 </code></td>
 </tr>
 <tr>
 <td>[disable]</td>
 <td><code class="docutils literal notranslate">v7.2.1 -> 7.4.3</code></td>
 <tr>
 <td>[enable]</td>
 <td><code class="docutils literal notranslate">v7.2.1 -> 7.4.3</code></td>
 </table>
 </div>
 </li>
                <li> <span class="li-head">sim2_pin_code</span> - SIM <span class="li-normal">type: str</span>
 <a id='label94' href="javascript:ContentClick('label95', 'label94');" onmouseover="ContentPreview('label95');" onmouseout="ContentUnpreview('label95');" title="click to collapse or expand..."> more... </a>
 <div id="label95" style="display:none">
 <table border="1">
 <tr>
 <td></td>
 <td colspan="1">Supported Version Ranges</td>
 </tr>
 <tr>
 <td>sim2_pin_code</td>
 <td><code class="docutils literal notranslate">v7.2.1 -> 7.4.3 </code></td>
 </tr>
 </table>
 </div>
 </li>
                </ul>
            <li> <span class="li-head">sms_notification</span> - FortiExtender cellular SMS notification configuration. <span class="li-normal">type: dict</span>
 <a id='label96' href="javascript:ContentClick('label97', 'label96');" onmouseover="ContentPreview('label97');" onmouseout="ContentUnpreview('label97');" title="click to collapse or expand..."> more... </a>
 <div id="label97" style="display:none">
 <table border="1">
 <tr>
 <td></td><td colspan="1">Supported Version Ranges</td>
 </tr>
 <tr>
 <td>sms_notification</td>
 <td><code class="docutils literal notranslate">v7.2.1 -> 7.4.3 </code></td>
 </tr>
 </table>
 </div>
 </li>
                <ul class="ul-self">
                <li> <span class="li-head">alert</span> - SMS alert list. <span class="li-normal">type: dict</span>
 <a id='label98' href="javascript:ContentClick('label99', 'label98');" onmouseover="ContentPreview('label99');" onmouseout="ContentUnpreview('label99');" title="click to collapse or expand..."> more... </a>
 <div id="label99" style="display:none">
 <table border="1">
 <tr>
 <td></td><td colspan="1">Supported Version Ranges</td>
 </tr>
 <tr>
 <td>alert</td>
 <td><code class="docutils literal notranslate">v7.2.1 -> 7.4.3 </code></td>
 </tr>
 </table>
 </div>
 </li>
                    <ul class="ul-self">
                    <li> <span class="li-head">data_exhausted</span> - Display string when data exhausted. <span class="li-normal">type: str</span>
 <a id='label100' href="javascript:ContentClick('label101', 'label100');" onmouseover="ContentPreview('label101');" onmouseout="ContentUnpreview('label101');" title="click to collapse or expand..."> more... </a>
 <div id="label101" style="display:none">
 <table border="1">
 <tr>
 <td></td>
 <td colspan="1">Supported Version Ranges</td>
 </tr>
 <tr>
 <td>data_exhausted</td>
 <td><code class="docutils literal notranslate">v7.2.1 -> 7.4.3 </code></td>
 </tr>
 </table>
 </div>
 </li>
                    <li> <span class="li-head">fgt_backup_mode_switch</span> - Display string when FortiGate backup mode switched. <span class="li-normal">type: str</span>
 <a id='label102' href="javascript:ContentClick('label103', 'label102');" onmouseover="ContentPreview('label103');" onmouseout="ContentUnpreview('label103');" title="click to collapse or expand..."> more... </a>
 <div id="label103" style="display:none">
 <table border="1">
 <tr>
 <td></td>
 <td colspan="1">Supported Version Ranges</td>
 </tr>
 <tr>
 <td>fgt_backup_mode_switch</td>
 <td><code class="docutils literal notranslate">v7.2.1 -> 7.4.3 </code></td>
 </tr>
 </table>
 </div>
 </li>
                    <li> <span class="li-head">low_signal_strength</span> - Display string when signal strength is low. <span class="li-normal">type: str</span>
 <a id='label104' href="javascript:ContentClick('label105', 'label104');" onmouseover="ContentPreview('label105');" onmouseout="ContentUnpreview('label105');" title="click to collapse or expand..."> more... </a>
 <div id="label105" style="display:none">
 <table border="1">
 <tr>
 <td></td>
 <td colspan="1">Supported Version Ranges</td>
 </tr>
 <tr>
 <td>low_signal_strength</td>
 <td><code class="docutils literal notranslate">v7.2.1 -> 7.4.3 </code></td>
 </tr>
 </table>
 </div>
 </li>
                    <li> <span class="li-head">mode_switch</span> - Display string when mode is switched. <span class="li-normal">type: str</span>
 <a id='label106' href="javascript:ContentClick('label107', 'label106');" onmouseover="ContentPreview('label107');" onmouseout="ContentUnpreview('label107');" title="click to collapse or expand..."> more... </a>
 <div id="label107" style="display:none">
 <table border="1">
 <tr>
 <td></td>
 <td colspan="1">Supported Version Ranges</td>
 </tr>
 <tr>
 <td>mode_switch</td>
 <td><code class="docutils literal notranslate">v7.2.1 -> 7.4.3 </code></td>
 </tr>
 </table>
 </div>
 </li>
                    <li> <span class="li-head">os_image_fallback</span> - Display string when falling back to a previous OS image. <span class="li-normal">type: str</span>
 <a id='label108' href="javascript:ContentClick('label109', 'label108');" onmouseover="ContentPreview('label109');" onmouseout="ContentUnpreview('label109');" title="click to collapse or expand..."> more... </a>
 <div id="label109" style="display:none">
 <table border="1">
 <tr>
 <td></td>
 <td colspan="1">Supported Version Ranges</td>
 </tr>
 <tr>
 <td>os_image_fallback</td>
 <td><code class="docutils literal notranslate">v7.2.1 -> 7.4.3 </code></td>
 </tr>
 </table>
 </div>
 </li>
                    <li> <span class="li-head">session_disconnect</span> - Display string when session disconnected. <span class="li-normal">type: str</span>
 <a id='label110' href="javascript:ContentClick('label111', 'label110');" onmouseover="ContentPreview('label111');" onmouseout="ContentUnpreview('label111');" title="click to collapse or expand..."> more... </a>
 <div id="label111" style="display:none">
 <table border="1">
 <tr>
 <td></td>
 <td colspan="1">Supported Version Ranges</td>
 </tr>
 <tr>
 <td>session_disconnect</td>
 <td><code class="docutils literal notranslate">v7.2.1 -> 7.4.3 </code></td>
 </tr>
 </table>
 </div>
 </li>
                    <li> <span class="li-head">system_reboot</span> - Display string when system rebooted. <span class="li-normal">type: str</span>
 <a id='label112' href="javascript:ContentClick('label113', 'label112');" onmouseover="ContentPreview('label113');" onmouseout="ContentUnpreview('label113');" title="click to collapse or expand..."> more... </a>
 <div id="label113" style="display:none">
 <table border="1">
 <tr>
 <td></td>
 <td colspan="1">Supported Version Ranges</td>
 </tr>
 <tr>
 <td>system_reboot</td>
 <td><code class="docutils literal notranslate">v7.2.1 -> 7.4.3 </code></td>
 </tr>
 </table>
 </div>
 </li>
                    </ul>
                <li> <span class="li-head">receiver</span> - SMS notification receiver list. <span class="li-normal">type: list</span> <span style="font-family:'Courier New'" class="li-required">member_path: cellular/sms_notification/receiver:name</span>
 <a id='label114' href="javascript:ContentClick('label115', 'label114');" onmouseover="ContentPreview('label115');" onmouseout="ContentUnpreview('label115');" title="click to collapse or expand..."> more... </a>
 <div id="label115" style="display:none">
 <table border="1">
 <tr>
 <td></td><td colspan="1">Supported Version Ranges</td>
 </tr>
 <tr>
 <td>receiver</td>
 <td><code class="docutils literal notranslate">v7.2.1 -> 7.4.3 </code></td>
 </tr>
 </table>
 </div>
 </li>
                    <ul class="ul-self">
                    <li> <span class="li-head">alert</span> - Alert multi-options. <span class="li-normal">type: list</span> <span class="li-normal">choices: system-reboot, data-exhausted, session-disconnect, low-signal-strength, mode-switch, os-image-fallback, fgt-backup-mode-switch</span>
 <a id='label116' href="javascript:ContentClick('label117', 'label116');" onmouseover="ContentPreview('label117');" onmouseout="ContentUnpreview('label117');" title="click to collapse or expand..."> more... </a>
 <div id="label117" style="display:none">
 <table border="1">
 <tr>
 <td></td>
 <td colspan="1">Supported Version Ranges</td>
 </tr>
 <tr>
 <td>alert</td>
 <td><code class="docutils literal notranslate">v7.2.1 -> 7.4.3 </code></td>
 </tr>
 <tr>
 <td>[system-reboot]</td>
 <td><code class="docutils literal notranslate">v7.2.1 -> 7.4.3</code></td>
 <tr>
 <td>[data-exhausted]</td>
 <td><code class="docutils literal notranslate">v7.2.1 -> 7.4.3</code></td>
 <tr>
 <td>[session-disconnect]</td>
 <td><code class="docutils literal notranslate">v7.2.1 -> 7.4.3</code></td>
 <tr>
 <td>[low-signal-strength]</td>
 <td><code class="docutils literal notranslate">v7.2.1 -> 7.4.3</code></td>
 <tr>
 <td>[mode-switch]</td>
 <td><code class="docutils literal notranslate">v7.2.1 -> 7.4.3</code></td>
 <tr>
 <td>[os-image-fallback]</td>
 <td><code class="docutils literal notranslate">v7.2.1 -> 7.4.3</code></td>
 <tr>
 <td>[fgt-backup-mode-switch]</td>
 <td><code class="docutils literal notranslate">v7.2.1 -> 7.4.3</code></td>
 </table>
 </div>
 </li>
                    <li> <span class="li-head">name</span> - FortiExtender SMS notification receiver name. <span class="li-normal">type: str</span> <span class="li-required">required: true</span>
 <a id='label118' href="javascript:ContentClick('label119', 'label118');" onmouseover="ContentPreview('label119');" onmouseout="ContentUnpreview('label119');" title="click to collapse or expand..."> more... </a>
 <div id="label119" style="display:none">
 <table border="1">
 <tr>
 <td></td>
 <td colspan="1">Supported Version Ranges</td>
 </tr>
 <tr>
 <td>name</td>
 <td><code class="docutils literal notranslate">v7.2.1 -> 7.4.3 </code></td>
 </tr>
 </table>
 </div>
 </li>
                    <li> <span class="li-head">phone_number</span> - Receiver phone number. Format: [+][country code][area code][local phone number]. For example, +16501234567. <span class="li-normal">type: str</span>
 <a id='label120' href="javascript:ContentClick('label121', 'label120');" onmouseover="ContentPreview('label121');" onmouseout="ContentUnpreview('label121');" title="click to collapse or expand..."> more... </a>
 <div id="label121" style="display:none">
 <table border="1">
 <tr>
 <td></td>
 <td colspan="1">Supported Version Ranges</td>
 </tr>
 <tr>
 <td>phone_number</td>
 <td><code class="docutils literal notranslate">v7.2.1 -> 7.4.3 </code></td>
 </tr>
 </table>
 </div>
 </li>
                    <li> <span class="li-head">status</span> - SMS notification receiver status. <span class="li-normal">type: str</span> <span class="li-normal">choices: disable, enable</span>
 <a id='label122' href="javascript:ContentClick('label123', 'label122');" onmouseover="ContentPreview('label123');" onmouseout="ContentUnpreview('label123');" title="click to collapse or expand..."> more... </a>
 <div id="label123" style="display:none">
 <table border="1">
 <tr>
 <td></td>
 <td colspan="1">Supported Version Ranges</td>
 </tr>
 <tr>
 <td>status</td>
 <td><code class="docutils literal notranslate">v7.2.1 -> 7.4.3 </code></td>
 </tr>
 <tr>
 <td>[disable]</td>
 <td><code class="docutils literal notranslate">v7.2.1 -> 7.4.3</code></td>
 <tr>
 <td>[enable]</td>
 <td><code class="docutils literal notranslate">v7.2.1 -> 7.4.3</code></td>
 </table>
 </div>
 </li>
                    </ul>
                <li> <span class="li-head">status</span> - FortiExtender SMS notification status. <span class="li-normal">type: str</span> <span class="li-normal">choices: disable, enable</span>
 <a id='label124' href="javascript:ContentClick('label125', 'label124');" onmouseover="ContentPreview('label125');" onmouseout="ContentUnpreview('label125');" title="click to collapse or expand..."> more... </a>
 <div id="label125" style="display:none">
 <table border="1">
 <tr>
 <td></td>
 <td colspan="1">Supported Version Ranges</td>
 </tr>
 <tr>
 <td>status</td>
 <td><code class="docutils literal notranslate">v7.2.1 -> 7.4.3 </code></td>
 </tr>
 <tr>
 <td>[disable]</td>
 <td><code class="docutils literal notranslate">v7.2.1 -> 7.4.3</code></td>
 <tr>
 <td>[enable]</td>
 <td><code class="docutils literal notranslate">v7.2.1 -> 7.4.3</code></td>
 </table>
 </div>
 </li>
                </ul>
            </ul>
        <li> <span class="li-head">enforce_bandwidth</span> - Enable/disable enforcement of bandwidth on LAN extension interface. <span class="li-normal">type: str</span> <span class="li-normal">choices: enable, disable</span>
 <a id='label126' href="javascript:ContentClick('label127', 'label126');" onmouseover="ContentPreview('label127');" onmouseout="ContentUnpreview('label127');" title="click to collapse or expand..."> more... </a>
 <div id="label127" style="display:none">
 <table border="1">
 <tr>
 <td></td>
 <td colspan="1">Supported Version Ranges</td>
 </tr>
 <tr>
 <td>enforce_bandwidth</td>
 <td><code class="docutils literal notranslate">v7.2.1 -> 7.4.3 </code></td>
 </tr>
 <tr>
 <td>[enable]</td>
 <td><code class="docutils literal notranslate">v7.2.1 -> 7.4.3</code></td>
 <tr>
 <td>[disable]</td>
 <td><code class="docutils literal notranslate">v7.2.1 -> 7.4.3</code></td>
 </table>
 </div>
 </li>
        <li> <span class="li-head">extension</span> - Extension option. <span class="li-normal">type: str</span> <span class="li-normal">choices: wan-extension, lan-extension</span>
 <a id='label128' href="javascript:ContentClick('label129', 'label128');" onmouseover="ContentPreview('label129');" onmouseout="ContentUnpreview('label129');" title="click to collapse or expand..."> more... </a>
 <div id="label129" style="display:none">
 <table border="1">
 <tr>
 <td></td>
 <td colspan="1">Supported Version Ranges</td>
 </tr>
 <tr>
 <td>extension</td>
 <td><code class="docutils literal notranslate">v7.2.1 -> 7.4.3 </code></td>
 </tr>
 <tr>
 <td>[wan-extension]</td>
 <td><code class="docutils literal notranslate">v7.2.1 -> 7.4.3</code></td>
 <tr>
 <td>[lan-extension]</td>
 <td><code class="docutils literal notranslate">v7.2.1 -> 7.4.3</code></td>
 </table>
 </div>
 </li>
        <li> <span class="li-head">id</span> - ID. <span class="li-normal">type: int</span>
 <a id='label130' href="javascript:ContentClick('label131', 'label130');" onmouseover="ContentPreview('label131');" onmouseout="ContentUnpreview('label131');" title="click to collapse or expand..."> more... </a>
 <div id="label131" style="display:none">
 <table border="1">
 <tr>
 <td></td>
 <td colspan="1">Supported Version Ranges</td>
 </tr>
 <tr>
 <td>id</td>
 <td><code class="docutils literal notranslate">v7.2.1 -> 7.4.3 </code></td>
 </tr>
 </table>
 </div>
 </li>
        <li> <span class="li-head">lan_extension</span> - FortiExtender lan extension configuration. <span class="li-normal">type: dict</span>
 <a id='label132' href="javascript:ContentClick('label133', 'label132');" onmouseover="ContentPreview('label133');" onmouseout="ContentUnpreview('label133');" title="click to collapse or expand..."> more... </a>
 <div id="label133" style="display:none">
 <table border="1">
 <tr>
 <td></td><td colspan="1">Supported Version Ranges</td>
 </tr>
 <tr>
 <td>lan_extension</td>
 <td><code class="docutils literal notranslate">v7.2.1 -> 7.4.3 </code></td>
 </tr>
 </table>
 </div>
 </li>
            <ul class="ul-self">
            <li> <span class="li-head">backhaul</span> - LAN extension backhaul tunnel configuration. <span class="li-normal">type: list</span> <span style="font-family:'Courier New'" class="li-required">member_path: lan_extension/backhaul:name</span>
 <a id='label134' href="javascript:ContentClick('label135', 'label134');" onmouseover="ContentPreview('label135');" onmouseout="ContentUnpreview('label135');" title="click to collapse or expand..."> more... </a>
 <div id="label135" style="display:none">
 <table border="1">
 <tr>
 <td></td><td colspan="1">Supported Version Ranges</td>
 </tr>
 <tr>
 <td>backhaul</td>
 <td><code class="docutils literal notranslate">v7.2.1 -> 7.4.3 </code></td>
 </tr>
 </table>
 </div>
 </li>
                <ul class="ul-self">
                <li> <span class="li-head">name</span> - FortiExtender LAN extension backhaul name. <span class="li-normal">type: str</span> <span class="li-required">required: true</span>
 <a id='label136' href="javascript:ContentClick('label137', 'label136');" onmouseover="ContentPreview('label137');" onmouseout="ContentUnpreview('label137');" title="click to collapse or expand..."> more... </a>
 <div id="label137" style="display:none">
 <table border="1">
 <tr>
 <td></td>
 <td colspan="1">Supported Version Ranges</td>
 </tr>
 <tr>
 <td>name</td>
 <td><code class="docutils literal notranslate">v7.2.1 -> 7.4.3 </code></td>
 </tr>
 </table>
 </div>
 </li>
                <li> <span class="li-head">port</span> - FortiExtender uplink port. <span class="li-normal">type: str</span> <span class="li-normal">choices: wan, lte1, lte2, port1, port2, port3, port4, port5, sfp</span>
 <a id='label138' href="javascript:ContentClick('label139', 'label138');" onmouseover="ContentPreview('label139');" onmouseout="ContentUnpreview('label139');" title="click to collapse or expand..."> more... </a>
 <div id="label139" style="display:none">
 <table border="1">
 <tr>
 <td></td>
 <td colspan="1">Supported Version Ranges</td>
 </tr>
 <tr>
 <td>port</td>
 <td><code class="docutils literal notranslate">v7.2.1 -> 7.4.3 </code></td>
 </tr>
 <tr>
 <td>[wan]</td>
 <td><code class="docutils literal notranslate">v7.2.1 -> 7.4.3</code></td>
 <tr>
 <td>[lte1]</td>
 <td><code class="docutils literal notranslate">v7.2.1 -> 7.4.3</code></td>
 <tr>
 <td>[lte2]</td>
 <td><code class="docutils literal notranslate">v7.2.1 -> 7.4.3</code></td>
 <tr>
 <td>[port1]</td>
 <td><code class="docutils literal notranslate">v7.2.1 -> 7.4.3</code></td>
 <tr>
 <td>[port2]</td>
 <td><code class="docutils literal notranslate">v7.2.1 -> 7.4.3</code></td>
 <tr>
 <td>[port3]</td>
 <td><code class="docutils literal notranslate">v7.2.1 -> 7.4.3</code></td>
 <tr>
 <td>[port4]</td>
 <td><code class="docutils literal notranslate">v7.2.1 -> 7.4.3</code></td>
 <tr>
 <td>[port5]</td>
 <td><code class="docutils literal notranslate">v7.2.1 -> 7.4.3</code></td>
 <tr>
 <td>[sfp]</td>
 <td><code class="docutils literal notranslate">v7.2.1 -> 7.4.3</code></td>
 </table>
 </div>
 </li>
                <li> <span class="li-head">role</span> - FortiExtender uplink port. <span class="li-normal">type: str</span> <span class="li-normal">choices: primary, secondary</span>
 <a id='label140' href="javascript:ContentClick('label141', 'label140');" onmouseover="ContentPreview('label141');" onmouseout="ContentUnpreview('label141');" title="click to collapse or expand..."> more... </a>
 <div id="label141" style="display:none">
 <table border="1">
 <tr>
 <td></td>
 <td colspan="1">Supported Version Ranges</td>
 </tr>
 <tr>
 <td>role</td>
 <td><code class="docutils literal notranslate">v7.2.1 -> 7.4.3 </code></td>
 </tr>
 <tr>
 <td>[primary]</td>
 <td><code class="docutils literal notranslate">v7.2.1 -> 7.4.3</code></td>
 <tr>
 <td>[secondary]</td>
 <td><code class="docutils literal notranslate">v7.2.1 -> 7.4.3</code></td>
 </table>
 </div>
 </li>
                <li> <span class="li-head">weight</span> - WRR weight parameter. <span class="li-normal">type: int</span>
 <a id='label142' href="javascript:ContentClick('label143', 'label142');" onmouseover="ContentPreview('label143');" onmouseout="ContentUnpreview('label143');" title="click to collapse or expand..."> more... </a>
 <div id="label143" style="display:none">
 <table border="1">
 <tr>
 <td></td>
 <td colspan="1">Supported Version Ranges</td>
 </tr>
 <tr>
 <td>weight</td>
 <td><code class="docutils literal notranslate">v7.2.1 -> 7.4.3 </code></td>
 </tr>
 </table>
 </div>
 </li>
                </ul>
            <li> <span class="li-head">backhaul_interface</span> - IPsec phase1 interface. Source system.interface.name. <span class="li-normal">type: str</span>
 <a id='label144' href="javascript:ContentClick('label145', 'label144');" onmouseover="ContentPreview('label145');" onmouseout="ContentUnpreview('label145');" title="click to collapse or expand..."> more... </a>
 <div id="label145" style="display:none">
 <table border="1">
 <tr>
 <td></td>
 <td colspan="1">Supported Version Ranges</td>
 </tr>
 <tr>
 <td>backhaul_interface</td>
 <td><code class="docutils literal notranslate">v7.2.1 -> 7.4.3 </code></td>
 </tr>
 </table>
 </div>
 </li>
            <li> <span class="li-head">backhaul_ip</span> - IPsec phase1 IPv4/FQDN. Used to specify the external IP/FQDN when the FortiGate unit is behind a NAT device. <span class="li-normal">type: str</span>
 <a id='label146' href="javascript:ContentClick('label147', 'label146');" onmouseover="ContentPreview('label147');" onmouseout="ContentUnpreview('label147');" title="click to collapse or expand..."> more... </a>
 <div id="label147" style="display:none">
 <table border="1">
 <tr>
 <td></td>
 <td colspan="1">Supported Version Ranges</td>
 </tr>
 <tr>
 <td>backhaul_ip</td>
 <td><code class="docutils literal notranslate">v7.2.1 -> 7.4.3 </code></td>
 </tr>
 </table>
 </div>
 </li>
            <li> <span class="li-head">ipsec_tunnel</span> - IPsec tunnel name. <span class="li-normal">type: str</span>
 <a id='label148' href="javascript:ContentClick('label149', 'label148');" onmouseover="ContentPreview('label149');" onmouseout="ContentUnpreview('label149');" title="click to collapse or expand..."> more... </a>
 <div id="label149" style="display:none">
 <table border="1">
 <tr>
 <td></td>
 <td colspan="1">Supported Version Ranges</td>
 </tr>
 <tr>
 <td>ipsec_tunnel</td>
 <td><code class="docutils literal notranslate">v7.2.1 -> 7.4.3 </code></td>
 </tr>
 </table>
 </div>
 </li>
            <li> <span class="li-head">link_loadbalance</span> - LAN extension link load balance strategy. <span class="li-normal">type: str</span> <span class="li-normal">choices: activebackup, loadbalance</span>
 <a id='label150' href="javascript:ContentClick('label151', 'label150');" onmouseover="ContentPreview('label151');" onmouseout="ContentUnpreview('label151');" title="click to collapse or expand..."> more... </a>
 <div id="label151" style="display:none">
 <table border="1">
 <tr>
 <td></td>
 <td colspan="1">Supported Version Ranges</td>
 </tr>
 <tr>
 <td>link_loadbalance</td>
 <td><code class="docutils literal notranslate">v7.2.1 -> 7.4.3 </code></td>
 </tr>
 <tr>
 <td>[activebackup]</td>
 <td><code class="docutils literal notranslate">v7.2.1 -> 7.4.3</code></td>
 <tr>
 <td>[loadbalance]</td>
 <td><code class="docutils literal notranslate">v7.2.1 -> 7.4.3</code></td>
 </table>
 </div>
 </li>
            </ul>
        <li> <span class="li-head">login_password</span> - Set the managed extender"s administrator password. <span class="li-normal">type: str</span>
 <a id='label152' href="javascript:ContentClick('label153', 'label152');" onmouseover="ContentPreview('label153');" onmouseout="ContentUnpreview('label153');" title="click to collapse or expand..."> more... </a>
 <div id="label153" style="display:none">
 <table border="1">
 <tr>
 <td></td>
 <td colspan="1">Supported Version Ranges</td>
 </tr>
 <tr>
 <td>login_password</td>
 <td><code class="docutils literal notranslate">v7.2.1 -> 7.4.3 </code></td>
 </tr>
 </table>
 </div>
 </li>
        <li> <span class="li-head">login_password_change</span> - Change or reset the administrator password of a managed extender (yes, default, or no). <span class="li-normal">type: str</span> <span class="li-normal">choices: yes, default, no</span>
 <a id='label154' href="javascript:ContentClick('label155', 'label154');" onmouseover="ContentPreview('label155');" onmouseout="ContentUnpreview('label155');" title="click to collapse or expand..."> more... </a>
 <div id="label155" style="display:none">
 <table border="1">
 <tr>
 <td></td>
 <td colspan="1">Supported Version Ranges</td>
 </tr>
 <tr>
 <td>login_password_change</td>
 <td><code class="docutils literal notranslate">v7.2.1 -> 7.4.3 </code></td>
 </tr>
 <tr>
 <td>[yes]</td>
 <td><code class="docutils literal notranslate">v7.2.1 -> 7.4.3</code></td>
 <tr>
 <td>[default]</td>
 <td><code class="docutils literal notranslate">v7.2.1 -> 7.4.3</code></td>
 <tr>
 <td>[no]</td>
 <td><code class="docutils literal notranslate">v7.2.1 -> 7.4.3</code></td>
 </table>
 </div>
 </li>
        <li> <span class="li-head">model</span> - Model. <span class="li-normal">type: str</span> <span class="li-normal">choices: FX201E, FX211E, FX200F, FXA11F, FXE11F, FXA21F, FXE21F, FXA22F, FXE22F, FX212F, FX311F, FX312F, FX511F, FVG21F, FVA21F, FVG22F, FVA22F, FX04DA</span>
 <a id='label156' href="javascript:ContentClick('label157', 'label156');" onmouseover="ContentPreview('label157');" onmouseout="ContentUnpreview('label157');" title="click to collapse or expand..."> more... </a>
 <div id="label157" style="display:none">
 <table border="1">
 <tr>
 <td></td>
 <td colspan="1">Supported Version Ranges</td>
 </tr>
 <tr>
 <td>model</td>
 <td><code class="docutils literal notranslate">v7.2.1 -> 7.4.3 </code></td>
 </tr>
 <tr>
 <td>[FX201E]</td>
 <td><code class="docutils literal notranslate">v7.2.1 -> 7.4.3</code></td>
 <tr>
 <td>[FX211E]</td>
 <td><code class="docutils literal notranslate">v7.2.1 -> 7.4.3</code></td>
 <tr>
 <td>[FX200F]</td>
 <td><code class="docutils literal notranslate">v7.2.1 -> 7.4.3</code></td>
 <tr>
 <td>[FXA11F]</td>
 <td><code class="docutils literal notranslate">v7.2.1 -> 7.4.3</code></td>
 <tr>
 <td>[FXE11F]</td>
 <td><code class="docutils literal notranslate">v7.2.1 -> 7.4.3</code></td>
 <tr>
 <td>[FXA21F]</td>
 <td><code class="docutils literal notranslate">v7.2.1 -> 7.4.3</code></td>
 <tr>
 <td>[FXE21F]</td>
 <td><code class="docutils literal notranslate">v7.2.1 -> 7.4.3</code></td>
 <tr>
 <td>[FXA22F]</td>
 <td><code class="docutils literal notranslate">v7.2.1 -> 7.4.3</code></td>
 <tr>
 <td>[FXE22F]</td>
 <td><code class="docutils literal notranslate">v7.2.1 -> 7.4.3</code></td>
 <tr>
 <td>[FX212F]</td>
 <td><code class="docutils literal notranslate">v7.2.1 -> 7.4.3</code></td>
 <tr>
 <td>[FX311F]</td>
 <td><code class="docutils literal notranslate">v7.2.1 -> 7.4.3</code></td>
 <tr>
 <td>[FX312F]</td>
 <td><code class="docutils literal notranslate">v7.2.1 -> 7.4.3</code></td>
 <tr>
 <td>[FX511F]</td>
 <td><code class="docutils literal notranslate">v7.2.1 -> 7.4.3</code></td>
 <tr>
 <td>[FVG21F]</td>
 <td><code class="docutils literal notranslate">v7.2.1 -> 7.4.3</code></td>
 <tr>
 <td>[FVA21F]</td>
 <td><code class="docutils literal notranslate">v7.2.1 -> 7.4.3</code></td>
 <tr>
 <td>[FVG22F]</td>
 <td><code class="docutils literal notranslate">v7.2.1 -> 7.4.3</code></td>
 <tr>
 <td>[FVA22F]</td>
 <td><code class="docutils literal notranslate">v7.2.1 -> 7.4.3</code></td>
 <tr>
 <td>[FX04DA]</td>
 <td><code class="docutils literal notranslate">v7.2.1 -> 7.4.3</code></td>
 </table>
 </div>
 </li>
        <li> <span class="li-head">name</span> - FortiExtender profile name. <span class="li-normal">type: str</span> <span class="li-required">required: true</span>
 <a id='label158' href="javascript:ContentClick('label159', 'label158');" onmouseover="ContentPreview('label159');" onmouseout="ContentUnpreview('label159');" title="click to collapse or expand..."> more... </a>
 <div id="label159" style="display:none">
 <table border="1">
 <tr>
 <td></td>
 <td colspan="1">Supported Version Ranges</td>
 </tr>
 <tr>
 <td>name</td>
 <td><code class="docutils literal notranslate">v7.2.1 -> 7.4.3 </code></td>
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
                              name: "default_name_61"
                              phone_number: "<your_own_value>"
                              status: "disable"
                      status: "disable"
              enforce_bandwidth: "enable"
              extension: "wan-extension"
              id: "67"
              lan_extension:
                  backhaul:
                      -
                          name: "default_name_70"
                          port: "wan"
                          role: "primary"
                          weight: "1"
                  backhaul_interface: "<your_own_value> (source system.interface.name)"
                  backhaul_ip: "<your_own_value>"
                  ipsec_tunnel: "<your_own_value>"
                  link_loadbalance: "activebackup"
              login_password: "<your_own_value>"
              login_password_change: "yes"
              model: "FX201E"
              name: "default_name_81"


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
