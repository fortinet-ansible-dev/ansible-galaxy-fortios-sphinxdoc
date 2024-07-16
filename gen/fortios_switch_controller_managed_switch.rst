:source: fortios_switch_controller_managed_switch.py

:orphan:

.. fortios_switch_controller_managed_switch:

fortios_switch_controller_managed_switch -- Configure FortiSwitch devices that are managed by this FortiGate in Fortinet's FortiOS and FortiGate.
+++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++

.. versionadded:: 2.0.0

.. contents::
   :local:
   :depth: 1


Synopsis
--------
- This module is able to configure a FortiGate or FortiOS (FOS) device by allowing the user to set and modify switch_controller feature and managed_switch category. Examples include all parameters and values need to be adjusted to datasources before usage. Tested with FOS v6.0.0



Requirements
------------
The below requirements are needed on the host that executes this module.

- ansible>=2.15


Tips
----
Using member operation to add an element to an existing object.

FortiOS Version Compatibility
-----------------------------
Supported Version Ranges: v6.0.0 -> v7.4.4


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
    <li> <span class="li-head">switch_controller_managed_switch</span> - Configure FortiSwitch devices that are managed by this FortiGate. <span class="li-normal">type: dict</span>
 <a id='label0' href="javascript:ContentClick('label1', 'label0');" onmouseover="ContentPreview('label1');" onmouseout="ContentUnpreview('label1');" title="click to collapse or expand..."> more... </a>
 <div id="label1" style="display:none">
 <table border="1">
 <tr>
 <td></td><td colspan="1">Supported Version Ranges</td>
 </tr>
 <tr>
 <td>switch_controller_managed_switch</td>
 <td><code class="docutils literal notranslate">v6.0.0 -> 7.4.4 </code></td>
 </tr>
 </table>
 </div>
 </li>
        <ul class="ul-self">
        <li> <span class="li-head">settings_802_1X</span> - Configuration method to edit FortiSwitch 802.1X global settings. <span class="li-normal">type: dict</span>
 <a id='label2' href="javascript:ContentClick('label3', 'label2');" onmouseover="ContentPreview('label3');" onmouseout="ContentUnpreview('label3');" title="click to collapse or expand..."> more... </a>
 <div id="label3" style="display:none">
 <table border="1">
 <tr>
 <td></td><td colspan="1">Supported Version Ranges</td>
 </tr>
 <tr>
 <td>settings_802_1X</td>
 <td><code class="docutils literal notranslate">v6.0.0 -> 7.4.4 </code></td>
 </tr>
 </table>
 </div>
 </li>
            <ul class="ul-self">
            <li> <span class="li-head">link_down_auth</span> - Authentication state to set if a link is down. <span class="li-normal">type: str</span> <span class="li-normal">choices: set-unauth, no-action</span>
 <a id='label4' href="javascript:ContentClick('label5', 'label4');" onmouseover="ContentPreview('label5');" onmouseout="ContentUnpreview('label5');" title="click to collapse or expand..."> more... </a>
 <div id="label5" style="display:none">
 <table border="1">
 <tr>
 <td></td>
 <td colspan="1">Supported Version Ranges</td>
 </tr>
 <tr>
 <td>link_down_auth</td>
 <td><code class="docutils literal notranslate">v6.0.0 -> 7.4.4 </code></td>
 </tr>
 <tr>
 <td>[set-unauth]</td>
 <td><code class="docutils literal notranslate">v6.0.0 -> 7.4.4</code></td>
 <tr>
 <td>[no-action]</td>
 <td><code class="docutils literal notranslate">v6.0.0 -> 7.4.4</code></td>
 </table>
 </div>
 </li>
            <li> <span class="li-head">local_override</span> - Enable to override global 802.1X settings on individual FortiSwitches. <span class="li-normal">type: str</span> <span class="li-normal">choices: enable, disable</span>
 <a id='label6' href="javascript:ContentClick('label7', 'label6');" onmouseover="ContentPreview('label7');" onmouseout="ContentUnpreview('label7');" title="click to collapse or expand..."> more... </a>
 <div id="label7" style="display:none">
 <table border="1">
 <tr>
 <td></td>
 <td colspan="1">Supported Version Ranges</td>
 </tr>
 <tr>
 <td>local_override</td>
 <td><code class="docutils literal notranslate">v6.0.0 -> 7.4.4 </code></td>
 </tr>
 <tr>
 <td>[enable]</td>
 <td><code class="docutils literal notranslate">v6.0.0 -> 7.4.4</code></td>
 <tr>
 <td>[disable]</td>
 <td><code class="docutils literal notranslate">v6.0.0 -> 7.4.4</code></td>
 </table>
 </div>
 </li>
            <li> <span class="li-head">mab_reauth</span> - Enable or disable MAB reauthentication settings. <span class="li-normal">type: str</span> <span class="li-normal">choices: disable, enable</span>
 <a id='label8' href="javascript:ContentClick('label9', 'label8');" onmouseover="ContentPreview('label9');" onmouseout="ContentUnpreview('label9');" title="click to collapse or expand..."> more... </a>
 <div id="label9" style="display:none">
 <table border="1">
 <tr>
 <td></td>
 <td colspan="1">Supported Version Ranges</td>
 </tr>
 <tr>
 <td>mab_reauth</td>
 <td><code class="docutils literal notranslate">v7.2.0 -> 7.4.4 </code></td>
 </tr>
 <tr>
 <td>[disable]</td>
 <td><code class="docutils literal notranslate">v7.2.0 -> 7.4.4</code></td>
 <tr>
 <td>[enable]</td>
 <td><code class="docutils literal notranslate">v7.2.0 -> 7.4.4</code></td>
 </table>
 </div>
 </li>
            <li> <span class="li-head">mac_called_station_delimiter</span> - MAC called station delimiter . <span class="li-normal">type: str</span> <span class="li-normal">choices: colon, hyphen, none, single-hyphen</span>
 <a id='label10' href="javascript:ContentClick('label11', 'label10');" onmouseover="ContentPreview('label11');" onmouseout="ContentUnpreview('label11');" title="click to collapse or expand..."> more... </a>
 <div id="label11" style="display:none">
 <table border="1">
 <tr>
 <td></td>
 <td colspan="1">Supported Version Ranges</td>
 </tr>
 <tr>
 <td>mac_called_station_delimiter</td>
 <td><code class="docutils literal notranslate">v7.4.2 -> 7.4.4 </code></td>
 </tr>
 <tr>
 <td>[colon]</td>
 <td><code class="docutils literal notranslate">v7.4.2 -> 7.4.4</code></td>
 <tr>
 <td>[hyphen]</td>
 <td><code class="docutils literal notranslate">v7.4.2 -> 7.4.4</code></td>
 <tr>
 <td>[none]</td>
 <td><code class="docutils literal notranslate">v7.4.2 -> 7.4.4</code></td>
 <tr>
 <td>[single-hyphen]</td>
 <td><code class="docutils literal notranslate">v7.4.2 -> 7.4.4</code></td>
 </table>
 </div>
 </li>
            <li> <span class="li-head">mac_calling_station_delimiter</span> - MAC calling station delimiter . <span class="li-normal">type: str</span> <span class="li-normal">choices: colon, hyphen, none, single-hyphen</span>
 <a id='label12' href="javascript:ContentClick('label13', 'label12');" onmouseover="ContentPreview('label13');" onmouseout="ContentUnpreview('label13');" title="click to collapse or expand..."> more... </a>
 <div id="label13" style="display:none">
 <table border="1">
 <tr>
 <td></td>
 <td colspan="1">Supported Version Ranges</td>
 </tr>
 <tr>
 <td>mac_calling_station_delimiter</td>
 <td><code class="docutils literal notranslate">v7.4.2 -> 7.4.4 </code></td>
 </tr>
 <tr>
 <td>[colon]</td>
 <td><code class="docutils literal notranslate">v7.4.2 -> 7.4.4</code></td>
 <tr>
 <td>[hyphen]</td>
 <td><code class="docutils literal notranslate">v7.4.2 -> 7.4.4</code></td>
 <tr>
 <td>[none]</td>
 <td><code class="docutils literal notranslate">v7.4.2 -> 7.4.4</code></td>
 <tr>
 <td>[single-hyphen]</td>
 <td><code class="docutils literal notranslate">v7.4.2 -> 7.4.4</code></td>
 </table>
 </div>
 </li>
            <li> <span class="li-head">mac_case</span> - MAC case . <span class="li-normal">type: str</span> <span class="li-normal">choices: lowercase, uppercase</span>
 <a id='label14' href="javascript:ContentClick('label15', 'label14');" onmouseover="ContentPreview('label15');" onmouseout="ContentUnpreview('label15');" title="click to collapse or expand..."> more... </a>
 <div id="label15" style="display:none">
 <table border="1">
 <tr>
 <td></td>
 <td colspan="1">Supported Version Ranges</td>
 </tr>
 <tr>
 <td>mac_case</td>
 <td><code class="docutils literal notranslate">v7.4.2 -> 7.4.4 </code></td>
 </tr>
 <tr>
 <td>[lowercase]</td>
 <td><code class="docutils literal notranslate">v7.4.2 -> 7.4.4</code></td>
 <tr>
 <td>[uppercase]</td>
 <td><code class="docutils literal notranslate">v7.4.2 -> 7.4.4</code></td>
 </table>
 </div>
 </li>
            <li> <span class="li-head">mac_password_delimiter</span> - MAC authentication password delimiter . <span class="li-normal">type: str</span> <span class="li-normal">choices: colon, hyphen, none, single-hyphen</span>
 <a id='label16' href="javascript:ContentClick('label17', 'label16');" onmouseover="ContentPreview('label17');" onmouseout="ContentUnpreview('label17');" title="click to collapse or expand..."> more... </a>
 <div id="label17" style="display:none">
 <table border="1">
 <tr>
 <td></td>
 <td colspan="1">Supported Version Ranges</td>
 </tr>
 <tr>
 <td>mac_password_delimiter</td>
 <td><code class="docutils literal notranslate">v7.4.2 -> 7.4.4 </code></td>
 </tr>
 <tr>
 <td>[colon]</td>
 <td><code class="docutils literal notranslate">v7.4.2 -> 7.4.4</code></td>
 <tr>
 <td>[hyphen]</td>
 <td><code class="docutils literal notranslate">v7.4.2 -> 7.4.4</code></td>
 <tr>
 <td>[none]</td>
 <td><code class="docutils literal notranslate">v7.4.2 -> 7.4.4</code></td>
 <tr>
 <td>[single-hyphen]</td>
 <td><code class="docutils literal notranslate">v7.4.2 -> 7.4.4</code></td>
 </table>
 </div>
 </li>
            <li> <span class="li-head">mac_username_delimiter</span> - MAC authentication username delimiter . <span class="li-normal">type: str</span> <span class="li-normal">choices: colon, hyphen, none, single-hyphen</span>
 <a id='label18' href="javascript:ContentClick('label19', 'label18');" onmouseover="ContentPreview('label19');" onmouseout="ContentUnpreview('label19');" title="click to collapse or expand..."> more... </a>
 <div id="label19" style="display:none">
 <table border="1">
 <tr>
 <td></td>
 <td colspan="1">Supported Version Ranges</td>
 </tr>
 <tr>
 <td>mac_username_delimiter</td>
 <td><code class="docutils literal notranslate">v7.4.2 -> 7.4.4 </code></td>
 </tr>
 <tr>
 <td>[colon]</td>
 <td><code class="docutils literal notranslate">v7.4.2 -> 7.4.4</code></td>
 <tr>
 <td>[hyphen]</td>
 <td><code class="docutils literal notranslate">v7.4.2 -> 7.4.4</code></td>
 <tr>
 <td>[none]</td>
 <td><code class="docutils literal notranslate">v7.4.2 -> 7.4.4</code></td>
 <tr>
 <td>[single-hyphen]</td>
 <td><code class="docutils literal notranslate">v7.4.2 -> 7.4.4</code></td>
 </table>
 </div>
 </li>
            <li> <span class="li-head">max_reauth_attempt</span> - Maximum number of authentication attempts (0 - 15). <span class="li-normal">type: int</span>
 <a id='label20' href="javascript:ContentClick('label21', 'label20');" onmouseover="ContentPreview('label21');" onmouseout="ContentUnpreview('label21');" title="click to collapse or expand..."> more... </a>
 <div id="label21" style="display:none">
 <table border="1">
 <tr>
 <td></td>
 <td colspan="1">Supported Version Ranges</td>
 </tr>
 <tr>
 <td>max_reauth_attempt</td>
 <td><code class="docutils literal notranslate">v6.0.0 -> 7.4.4 </code></td>
 </tr>
 </table>
 </div>
 </li>
            <li> <span class="li-head">reauth_period</span> - Reauthentication time interval (1 - 1440 min). <span class="li-normal">type: int</span>
 <a id='label22' href="javascript:ContentClick('label23', 'label22');" onmouseover="ContentPreview('label23');" onmouseout="ContentUnpreview('label23');" title="click to collapse or expand..."> more... </a>
 <div id="label23" style="display:none">
 <table border="1">
 <tr>
 <td></td>
 <td colspan="1">Supported Version Ranges</td>
 </tr>
 <tr>
 <td>reauth_period</td>
 <td><code class="docutils literal notranslate">v6.0.0 -> 7.4.4 </code></td>
 </tr>
 </table>
 </div>
 </li>
            <li> <span class="li-head">tx_period</span> - 802.1X Tx period (seconds). <span class="li-normal">type: int</span>
 <a id='label24' href="javascript:ContentClick('label25', 'label24');" onmouseover="ContentPreview('label25');" onmouseout="ContentUnpreview('label25');" title="click to collapse or expand..."> more... </a>
 <div id="label25" style="display:none">
 <table border="1">
 <tr>
 <td></td>
 <td colspan="1">Supported Version Ranges</td>
 </tr>
 <tr>
 <td>tx_period</td>
 <td><code class="docutils literal notranslate">v6.4.0 -> 7.4.4 </code></td>
 </tr>
 </table>
 </div>
 </li>
            </ul>
        <li> <span class="li-head">access_profile</span> - FortiSwitch access profile. Source switch-controller.security-policy.local-access.name. <span class="li-normal">type: str</span>
 <a id='label26' href="javascript:ContentClick('label27', 'label26');" onmouseover="ContentPreview('label27');" onmouseout="ContentUnpreview('label27');" title="click to collapse or expand..."> more... </a>
 <div id="label27" style="display:none">
 <table border="1">
 <tr>
 <td></td>
 <td colspan="1">Supported Version Ranges</td>
 </tr>
 <tr>
 <td>access_profile</td>
 <td><code class="docutils literal notranslate">v6.2.0 -> 7.4.4 </code></td>
 </tr>
 </table>
 </div>
 </li>
        <li> <span class="li-head">custom_command</span> - Configuration method to edit FortiSwitch commands to be pushed to this FortiSwitch device upon rebooting the FortiGate switch controller or the FortiSwitch. <span class="li-normal">type: list</span> <span style="font-family:'Courier New'" class="li-required">member_path: custom_command:command_entry</span>
 <a id='label28' href="javascript:ContentClick('label29', 'label28');" onmouseover="ContentPreview('label29');" onmouseout="ContentUnpreview('label29');" title="click to collapse or expand..."> more... </a>
 <div id="label29" style="display:none">
 <table border="1">
 <tr>
 <td></td><td colspan="1">Supported Version Ranges</td>
 </tr>
 <tr>
 <td>custom_command</td>
 <td><code class="docutils literal notranslate">v6.0.0 -> 7.4.4 </code></td>
 </tr>
 </table>
 </div>
 </li>
            <ul class="ul-self">
            <li> <span class="li-head">command_entry</span> - List of FortiSwitch commands. <span class="li-normal">type: str</span> <span class="li-required">required: true</span>
 <a id='label30' href="javascript:ContentClick('label31', 'label30');" onmouseover="ContentPreview('label31');" onmouseout="ContentUnpreview('label31');" title="click to collapse or expand..."> more... </a>
 <div id="label31" style="display:none">
 <table border="1">
 <tr>
 <td></td>
 <td colspan="1">Supported Version Ranges</td>
 </tr>
 <tr>
 <td>command_entry</td>
 <td><code class="docutils literal notranslate">v6.0.0 -> 7.4.4 </code></td>
 </tr>
 </table>
 </div>
 </li>
            <li> <span class="li-head">command_name</span> - Names of commands to be pushed to this FortiSwitch device, as configured under config switch-controller custom-command. Source switch-controller.custom-command.command-name. <span class="li-normal">type: str</span>
 <a id='label32' href="javascript:ContentClick('label33', 'label32');" onmouseover="ContentPreview('label33');" onmouseout="ContentUnpreview('label33');" title="click to collapse or expand..."> more... </a>
 <div id="label33" style="display:none">
 <table border="1">
 <tr>
 <td></td>
 <td colspan="1">Supported Version Ranges</td>
 </tr>
 <tr>
 <td>command_name</td>
 <td><code class="docutils literal notranslate">v6.0.0 -> 7.4.4 </code></td>
 </tr>
 </table>
 </div>
 </li>
            </ul>
        <li> <span class="li-head">delayed_restart_trigger</span> - Delayed restart triggered for this FortiSwitch. <span class="li-normal">type: int</span>
 <a id='label34' href="javascript:ContentClick('label35', 'label34');" onmouseover="ContentPreview('label35');" onmouseout="ContentUnpreview('label35');" title="click to collapse or expand..."> more... </a>
 <div id="label35" style="display:none">
 <table border="1">
 <tr>
 <td></td>
 <td colspan="1">Supported Version Ranges</td>
 </tr>
 <tr>
 <td>delayed_restart_trigger</td>
 <td><code class="docutils literal notranslate">v6.0.0 -> 7.4.4 </code></td>
 </tr>
 </table>
 </div>
 </li>
        <li> <span class="li-head">description</span> - Description. <span class="li-normal">type: str</span>
 <a id='label36' href="javascript:ContentClick('label37', 'label36');" onmouseover="ContentPreview('label37');" onmouseout="ContentUnpreview('label37');" title="click to collapse or expand..."> more... </a>
 <div id="label37" style="display:none">
 <table border="1">
 <tr>
 <td></td>
 <td colspan="1">Supported Version Ranges</td>
 </tr>
 <tr>
 <td>description</td>
 <td><code class="docutils literal notranslate">v6.0.0 -> 7.4.4 </code></td>
 </tr>
 </table>
 </div>
 </li>
        <li> <span class="li-head">dhcp_server_access_list</span> - DHCP snooping server access list. <span class="li-normal">type: str</span> <span class="li-normal">choices: global, enable, disable</span>
 <a id='label38' href="javascript:ContentClick('label39', 'label38');" onmouseover="ContentPreview('label39');" onmouseout="ContentUnpreview('label39');" title="click to collapse or expand..."> more... </a>
 <div id="label39" style="display:none">
 <table border="1">
 <tr>
 <td></td>
 <td colspan="1">Supported Version Ranges</td>
 </tr>
 <tr>
 <td>dhcp_server_access_list</td>
 <td><code class="docutils literal notranslate">v7.0.1 -> 7.4.4 </code></td>
 </tr>
 <tr>
 <td>[global]</td>
 <td><code class="docutils literal notranslate">v7.0.1 -> 7.4.4</code></td>
 <tr>
 <td>[enable]</td>
 <td><code class="docutils literal notranslate">v7.0.1 -> 7.4.4</code></td>
 <tr>
 <td>[disable]</td>
 <td><code class="docutils literal notranslate">v7.0.1 -> 7.4.4</code></td>
 </table>
 </div>
 </li>
        <li> <span class="li-head">dhcp_snooping_static_client</span> - Configure FortiSwitch DHCP snooping static clients. <span class="li-normal">type: list</span> <span style="font-family:'Courier New'" class="li-required">member_path: dhcp_snooping_static_client:name</span>
 <a id='label40' href="javascript:ContentClick('label41', 'label40');" onmouseover="ContentPreview('label41');" onmouseout="ContentUnpreview('label41');" title="click to collapse or expand..."> more... </a>
 <div id="label41" style="display:none">
 <table border="1">
 <tr>
 <td></td><td colspan="1">Supported Version Ranges</td>
 </tr>
 <tr>
 <td>dhcp_snooping_static_client</td>
 <td><code class="docutils literal notranslate">v7.2.4 -> 7.4.4 </code></td>
 </tr>
 </table>
 </div>
 </li>
            <ul class="ul-self">
            <li> <span class="li-head">ip</span> - Client static IP address. <span class="li-normal">type: str</span>
 <a id='label42' href="javascript:ContentClick('label43', 'label42');" onmouseover="ContentPreview('label43');" onmouseout="ContentUnpreview('label43');" title="click to collapse or expand..."> more... </a>
 <div id="label43" style="display:none">
 <table border="1">
 <tr>
 <td></td>
 <td colspan="1">Supported Version Ranges</td>
 </tr>
 <tr>
 <td>ip</td>
 <td><code class="docutils literal notranslate">v7.2.4 -> 7.4.4 </code></td>
 </tr>
 </table>
 </div>
 </li>
            <li> <span class="li-head">mac</span> - Client MAC address. <span class="li-normal">type: str</span>
 <a id='label44' href="javascript:ContentClick('label45', 'label44');" onmouseover="ContentPreview('label45');" onmouseout="ContentUnpreview('label45');" title="click to collapse or expand..."> more... </a>
 <div id="label45" style="display:none">
 <table border="1">
 <tr>
 <td></td>
 <td colspan="1">Supported Version Ranges</td>
 </tr>
 <tr>
 <td>mac</td>
 <td><code class="docutils literal notranslate">v7.2.4 -> 7.4.4 </code></td>
 </tr>
 </table>
 </div>
 </li>
            <li> <span class="li-head">name</span> - Client name. <span class="li-normal">type: str</span> <span class="li-required">required: true</span>
 <a id='label46' href="javascript:ContentClick('label47', 'label46');" onmouseover="ContentPreview('label47');" onmouseout="ContentUnpreview('label47');" title="click to collapse or expand..."> more... </a>
 <div id="label47" style="display:none">
 <table border="1">
 <tr>
 <td></td>
 <td colspan="1">Supported Version Ranges</td>
 </tr>
 <tr>
 <td>name</td>
 <td><code class="docutils literal notranslate">v7.2.4 -> 7.4.4 </code></td>
 </tr>
 </table>
 </div>
 </li>
            <li> <span class="li-head">port</span> - Interface name. <span class="li-normal">type: str</span>
 <a id='label48' href="javascript:ContentClick('label49', 'label48');" onmouseover="ContentPreview('label49');" onmouseout="ContentUnpreview('label49');" title="click to collapse or expand..."> more... </a>
 <div id="label49" style="display:none">
 <table border="1">
 <tr>
 <td></td>
 <td colspan="1">Supported Version Ranges</td>
 </tr>
 <tr>
 <td>port</td>
 <td><code class="docutils literal notranslate">v7.2.4 -> 7.4.4 </code></td>
 </tr>
 </table>
 </div>
 </li>
            <li> <span class="li-head">vlan</span> - VLAN name. Source system.interface.name. <span class="li-normal">type: str</span>
 <a id='label50' href="javascript:ContentClick('label51', 'label50');" onmouseover="ContentPreview('label51');" onmouseout="ContentUnpreview('label51');" title="click to collapse or expand..."> more... </a>
 <div id="label51" style="display:none">
 <table border="1">
 <tr>
 <td></td>
 <td colspan="1">Supported Version Ranges</td>
 </tr>
 <tr>
 <td>vlan</td>
 <td><code class="docutils literal notranslate">v7.2.4 -> 7.4.4 </code></td>
 </tr>
 </table>
 </div>
 </li>
            </ul>
        <li> <span class="li-head">directly_connected</span> - Directly connected FortiSwitch. <span class="li-normal">type: int</span>
 <a id='label52' href="javascript:ContentClick('label53', 'label52');" onmouseover="ContentPreview('label53');" onmouseout="ContentUnpreview('label53');" title="click to collapse or expand..."> more... </a>
 <div id="label53" style="display:none">
 <table border="1">
 <tr>
 <td></td>
 <td colspan="2">Supported Version Ranges</td>
 </tr>
 <tr>
 <td>directly_connected</td>
 <td><code class="docutils literal notranslate">v6.0.0 -> v7.0.5 </code></td>
 <td><code class="docutils literal notranslate">v7.2.0 -> v7.2.0 </code></td>
 </tr>
 </table>
 </div>
 </li>
        <li> <span class="li-head">dynamic_capability</span> - List of features this FortiSwitch supports (not configurable) that is sent to the FortiGate device for subsequent configuration initiated by the FortiGate device. <span class="li-normal">type: str</span>
 <a id='label54' href="javascript:ContentClick('label55', 'label54');" onmouseover="ContentPreview('label55');" onmouseout="ContentUnpreview('label55');" title="click to collapse or expand..."> more... </a>
 <div id="label55" style="display:none">
 <table border="1">
 <tr>
 <td></td>
 <td colspan="1">Supported Version Ranges</td>
 </tr>
 <tr>
 <td>dynamic_capability</td>
 <td><code class="docutils literal notranslate">v6.0.0 -> 7.4.4 </code></td>
 </tr>
 </table>
 </div>
 </li>
        <li> <span class="li-head">dynamically_discovered</span> - Dynamically discovered FortiSwitch. <span class="li-normal">type: int</span>
 <a id='label56' href="javascript:ContentClick('label57', 'label56');" onmouseover="ContentPreview('label57');" onmouseout="ContentUnpreview('label57');" title="click to collapse or expand..."> more... </a>
 <div id="label57" style="display:none">
 <table border="1">
 <tr>
 <td></td>
 <td colspan="2">Supported Version Ranges</td>
 </tr>
 <tr>
 <td>dynamically_discovered</td>
 <td><code class="docutils literal notranslate">v6.0.0 -> v7.0.5 </code></td>
 <td><code class="docutils literal notranslate">v7.2.0 -> v7.2.0 </code></td>
 </tr>
 </table>
 </div>
 </li>
        <li> <span class="li-head">firmware_provision</span> - Enable/disable provisioning of firmware to FortiSwitches on join connection. <span class="li-normal">type: str</span> <span class="li-normal">choices: enable, disable</span>
 <a id='label58' href="javascript:ContentClick('label59', 'label58');" onmouseover="ContentPreview('label59');" onmouseout="ContentUnpreview('label59');" title="click to collapse or expand..."> more... </a>
 <div id="label59" style="display:none">
 <table border="1">
 <tr>
 <td></td>
 <td colspan="1">Supported Version Ranges</td>
 </tr>
 <tr>
 <td>firmware_provision</td>
 <td><code class="docutils literal notranslate">v7.0.0 -> 7.4.4 </code></td>
 </tr>
 <tr>
 <td>[enable]</td>
 <td><code class="docutils literal notranslate">v7.0.0 -> 7.4.4</code></td>
 <tr>
 <td>[disable]</td>
 <td><code class="docutils literal notranslate">v7.0.0 -> 7.4.4</code></td>
 </table>
 </div>
 </li>
        <li> <span class="li-head">firmware_provision_latest</span> - Enable/disable one-time automatic provisioning of the latest firmware version. <span class="li-normal">type: str</span> <span class="li-normal">choices: disable, once</span>
 <a id='label60' href="javascript:ContentClick('label61', 'label60');" onmouseover="ContentPreview('label61');" onmouseout="ContentUnpreview('label61');" title="click to collapse or expand..."> more... </a>
 <div id="label61" style="display:none">
 <table border="1">
 <tr>
 <td></td>
 <td colspan="1">Supported Version Ranges</td>
 </tr>
 <tr>
 <td>firmware_provision_latest</td>
 <td><code class="docutils literal notranslate">v7.0.4 -> 7.4.4 </code></td>
 </tr>
 <tr>
 <td>[disable]</td>
 <td><code class="docutils literal notranslate">v7.0.4 -> 7.4.4</code></td>
 <tr>
 <td>[once]</td>
 <td><code class="docutils literal notranslate">v7.0.4 -> 7.4.4</code></td>
 </table>
 </div>
 </li>
        <li> <span class="li-head">firmware_provision_version</span> - Firmware version to provision to this FortiSwitch on bootup (major.minor.build, i.e. 6.2.1234). <span class="li-normal">type: str</span>
 <a id='label62' href="javascript:ContentClick('label63', 'label62');" onmouseover="ContentPreview('label63');" onmouseout="ContentUnpreview('label63');" title="click to collapse or expand..."> more... </a>
 <div id="label63" style="display:none">
 <table border="1">
 <tr>
 <td></td>
 <td colspan="1">Supported Version Ranges</td>
 </tr>
 <tr>
 <td>firmware_provision_version</td>
 <td><code class="docutils literal notranslate">v7.0.0 -> 7.4.4 </code></td>
 </tr>
 </table>
 </div>
 </li>
        <li> <span class="li-head">flow_identity</span> - Flow-tracking netflow ipfix switch identity in hex format(00000000-FFFFFFFF ). <span class="li-normal">type: str</span>
 <a id='label64' href="javascript:ContentClick('label65', 'label64');" onmouseover="ContentPreview('label65');" onmouseout="ContentUnpreview('label65');" title="click to collapse or expand..."> more... </a>
 <div id="label65" style="display:none">
 <table border="1">
 <tr>
 <td></td>
 <td colspan="1">Supported Version Ranges</td>
 </tr>
 <tr>
 <td>flow_identity</td>
 <td><code class="docutils literal notranslate">v6.2.0 -> 7.4.4 </code></td>
 </tr>
 </table>
 </div>
 </li>
        <li> <span class="li-head">fsw_wan1_admin</span> - FortiSwitch WAN1 admin status; enable to authorize the FortiSwitch as a managed switch. <span class="li-normal">type: str</span> <span class="li-normal">choices: discovered, disable, enable</span>
 <a id='label66' href="javascript:ContentClick('label67', 'label66');" onmouseover="ContentPreview('label67');" onmouseout="ContentUnpreview('label67');" title="click to collapse or expand..."> more... </a>
 <div id="label67" style="display:none">
 <table border="1">
 <tr>
 <td></td>
 <td colspan="1">Supported Version Ranges</td>
 </tr>
 <tr>
 <td>fsw_wan1_admin</td>
 <td><code class="docutils literal notranslate">v6.0.0 -> 7.4.4 </code></td>
 </tr>
 <tr>
 <td>[discovered]</td>
 <td><code class="docutils literal notranslate">v6.0.0 -> 7.4.4</code></td>
 <tr>
 <td>[disable]</td>
 <td><code class="docutils literal notranslate">v6.0.0 -> 7.4.4</code></td>
 <tr>
 <td>[enable]</td>
 <td><code class="docutils literal notranslate">v6.0.0 -> 7.4.4</code></td>
 </table>
 </div>
 </li>
        <li> <span class="li-head">fsw_wan1_peer</span> - FortiSwitch WAN1 peer port. Source system.interface.name. <span class="li-normal">type: str</span>
 <a id='label68' href="javascript:ContentClick('label69', 'label68');" onmouseover="ContentPreview('label69');" onmouseout="ContentUnpreview('label69');" title="click to collapse or expand..."> more... </a>
 <div id="label69" style="display:none">
 <table border="1">
 <tr>
 <td></td>
 <td colspan="1">Supported Version Ranges</td>
 </tr>
 <tr>
 <td>fsw_wan1_peer</td>
 <td><code class="docutils literal notranslate">v6.0.0 -> 7.4.4 </code></td>
 </tr>
 </table>
 </div>
 </li>
        <li> <span class="li-head">fsw_wan2_admin</span> - FortiSwitch WAN2 admin status; enable to authorize the FortiSwitch as a managed switch. <span class="li-normal">type: str</span> <span class="li-normal">choices: discovered, disable, enable</span>
 <a id='label70' href="javascript:ContentClick('label71', 'label70');" onmouseover="ContentPreview('label71');" onmouseout="ContentUnpreview('label71');" title="click to collapse or expand..."> more... </a>
 <div id="label71" style="display:none">
 <table border="1">
 <tr>
 <td></td>
 <td colspan="2">Supported Version Ranges</td>
 </tr>
 <tr>
 <td>fsw_wan2_admin</td>
 <td><code class="docutils literal notranslate">v6.0.0 -> v6.0.11 </code></td>
 <td><code class="docutils literal notranslate">v6.2.3 -> v6.2.3 </code></td>
 </tr>
 <tr>
 <td>[discovered]</td>
 <td><code class="docutils literal notranslate">v6.0.0 -> v6.0.11</code></td>
 <tr>
 <td>[disable]</td>
 <td><code class="docutils literal notranslate">v6.0.0 -> v6.0.11</code></td>
 <tr>
 <td>[enable]</td>
 <td><code class="docutils literal notranslate">v6.0.0 -> v6.0.11</code></td>
 </table>
 </div>
 </li>
        <li> <span class="li-head">fsw_wan2_peer</span> - FortiSwitch WAN2 peer port. <span class="li-normal">type: str</span>
 <a id='label72' href="javascript:ContentClick('label73', 'label72');" onmouseover="ContentPreview('label73');" onmouseout="ContentUnpreview('label73');" title="click to collapse or expand..."> more... </a>
 <div id="label73" style="display:none">
 <table border="1">
 <tr>
 <td></td>
 <td colspan="2">Supported Version Ranges</td>
 </tr>
 <tr>
 <td>fsw_wan2_peer</td>
 <td><code class="docutils literal notranslate">v6.0.0 -> v6.0.11 </code></td>
 <td><code class="docutils literal notranslate">v6.2.3 -> v6.2.3 </code></td>
 </tr>
 </table>
 </div>
 </li>
        <li> <span class="li-head">igmp_snooping</span> - Configure FortiSwitch IGMP snooping global settings. <span class="li-normal">type: dict</span>
 <a id='label74' href="javascript:ContentClick('label75', 'label74');" onmouseover="ContentPreview('label75');" onmouseout="ContentUnpreview('label75');" title="click to collapse or expand..."> more... </a>
 <div id="label75" style="display:none">
 <table border="1">
 <tr>
 <td></td><td colspan="1">Supported Version Ranges</td>
 </tr>
 <tr>
 <td>igmp_snooping</td>
 <td><code class="docutils literal notranslate">v6.0.0 -> 7.4.4 </code></td>
 </tr>
 </table>
 </div>
 </li>
            <ul class="ul-self">
            <li> <span class="li-head">aging_time</span> - Maximum time to retain a multicast snooping entry for which no packets have been seen (15 - 3600 sec). <span class="li-normal">type: int</span>
 <a id='label76' href="javascript:ContentClick('label77', 'label76');" onmouseover="ContentPreview('label77');" onmouseout="ContentUnpreview('label77');" title="click to collapse or expand..."> more... </a>
 <div id="label77" style="display:none">
 <table border="1">
 <tr>
 <td></td>
 <td colspan="1">Supported Version Ranges</td>
 </tr>
 <tr>
 <td>aging_time</td>
 <td><code class="docutils literal notranslate">v6.0.0 -> 7.4.4 </code></td>
 </tr>
 </table>
 </div>
 </li>
            <li> <span class="li-head">flood_unknown_multicast</span> - Enable/disable unknown multicast flooding. <span class="li-normal">type: str</span> <span class="li-normal">choices: enable, disable</span>
 <a id='label78' href="javascript:ContentClick('label79', 'label78');" onmouseover="ContentPreview('label79');" onmouseout="ContentUnpreview('label79');" title="click to collapse or expand..."> more... </a>
 <div id="label79" style="display:none">
 <table border="1">
 <tr>
 <td></td>
 <td colspan="1">Supported Version Ranges</td>
 </tr>
 <tr>
 <td>flood_unknown_multicast</td>
 <td><code class="docutils literal notranslate">v6.0.0 -> 7.4.4 </code></td>
 </tr>
 <tr>
 <td>[enable]</td>
 <td><code class="docutils literal notranslate">v6.0.0 -> 7.4.4</code></td>
 <tr>
 <td>[disable]</td>
 <td><code class="docutils literal notranslate">v6.0.0 -> 7.4.4</code></td>
 </table>
 </div>
 </li>
            <li> <span class="li-head">local_override</span> - Enable/disable overriding the global IGMP snooping configuration. <span class="li-normal">type: str</span> <span class="li-normal">choices: enable, disable</span>
 <a id='label80' href="javascript:ContentClick('label81', 'label80');" onmouseover="ContentPreview('label81');" onmouseout="ContentUnpreview('label81');" title="click to collapse or expand..."> more... </a>
 <div id="label81" style="display:none">
 <table border="1">
 <tr>
 <td></td>
 <td colspan="1">Supported Version Ranges</td>
 </tr>
 <tr>
 <td>local_override</td>
 <td><code class="docutils literal notranslate">v6.0.0 -> 7.4.4 </code></td>
 </tr>
 <tr>
 <td>[enable]</td>
 <td><code class="docutils literal notranslate">v6.0.0 -> 7.4.4</code></td>
 <tr>
 <td>[disable]</td>
 <td><code class="docutils literal notranslate">v6.0.0 -> 7.4.4</code></td>
 </table>
 </div>
 </li>
            <li> <span class="li-head">vlans</span> - Configure IGMP snooping VLAN. <span class="li-normal">type: list</span> <span style="font-family:'Courier New'" class="li-required">member_path: igmp_snooping/vlans:vlan_name</span>
 <a id='label82' href="javascript:ContentClick('label83', 'label82');" onmouseover="ContentPreview('label83');" onmouseout="ContentUnpreview('label83');" title="click to collapse or expand..."> more... </a>
 <div id="label83" style="display:none">
 <table border="1">
 <tr>
 <td></td><td colspan="1">Supported Version Ranges</td>
 </tr>
 <tr>
 <td>vlans</td>
 <td><code class="docutils literal notranslate">v7.0.2 -> 7.4.4 </code></td>
 </tr>
 </table>
 </div>
 </li>
                <ul class="ul-self">
                <li> <span class="li-head">proxy</span> - IGMP snooping proxy for the VLAN interface. <span class="li-normal">type: str</span> <span class="li-normal">choices: disable, enable, global</span>
 <a id='label84' href="javascript:ContentClick('label85', 'label84');" onmouseover="ContentPreview('label85');" onmouseout="ContentUnpreview('label85');" title="click to collapse or expand..."> more... </a>
 <div id="label85" style="display:none">
 <table border="1">
 <tr>
 <td></td>
 <td colspan="1">Supported Version Ranges</td>
 </tr>
 <tr>
 <td>proxy</td>
 <td><code class="docutils literal notranslate">v7.0.2 -> 7.4.4 </code></td>
 </tr>
 <tr>
 <td>[disable]</td>
 <td><code class="docutils literal notranslate">v7.0.2 -> 7.4.4</code></td>
 <tr>
 <td>[enable]</td>
 <td><code class="docutils literal notranslate">v7.0.2 -> 7.4.4</code></td>
 <tr>
 <td>[global]</td>
 <td><code class="docutils literal notranslate">v7.0.2 -> 7.4.4</code></td>
 </table>
 </div>
 </li>
                <li> <span class="li-head">querier</span> - Enable/disable IGMP snooping querier for the VLAN interface. <span class="li-normal">type: str</span> <span class="li-normal">choices: disable, enable</span>
 <a id='label86' href="javascript:ContentClick('label87', 'label86');" onmouseover="ContentPreview('label87');" onmouseout="ContentUnpreview('label87');" title="click to collapse or expand..."> more... </a>
 <div id="label87" style="display:none">
 <table border="1">
 <tr>
 <td></td>
 <td colspan="1">Supported Version Ranges</td>
 </tr>
 <tr>
 <td>querier</td>
 <td><code class="docutils literal notranslate">v7.0.2 -> 7.4.4 </code></td>
 </tr>
 <tr>
 <td>[disable]</td>
 <td><code class="docutils literal notranslate">v7.0.2 -> 7.4.4</code></td>
 <tr>
 <td>[enable]</td>
 <td><code class="docutils literal notranslate">v7.0.2 -> 7.4.4</code></td>
 </table>
 </div>
 </li>
                <li> <span class="li-head">querier_addr</span> - IGMP snooping querier address. <span class="li-normal">type: str</span>
 <a id='label88' href="javascript:ContentClick('label89', 'label88');" onmouseover="ContentPreview('label89');" onmouseout="ContentUnpreview('label89');" title="click to collapse or expand..."> more... </a>
 <div id="label89" style="display:none">
 <table border="1">
 <tr>
 <td></td>
 <td colspan="1">Supported Version Ranges</td>
 </tr>
 <tr>
 <td>querier_addr</td>
 <td><code class="docutils literal notranslate">v7.0.2 -> 7.4.4 </code></td>
 </tr>
 </table>
 </div>
 </li>
                <li> <span class="li-head">version</span> - IGMP snooping querying version. <span class="li-normal">type: int</span>
 <a id='label90' href="javascript:ContentClick('label91', 'label90');" onmouseover="ContentPreview('label91');" onmouseout="ContentUnpreview('label91');" title="click to collapse or expand..."> more... </a>
 <div id="label91" style="display:none">
 <table border="1">
 <tr>
 <td></td>
 <td colspan="1">Supported Version Ranges</td>
 </tr>
 <tr>
 <td>version</td>
 <td><code class="docutils literal notranslate">v7.0.2 -> 7.4.4 </code></td>
 </tr>
 </table>
 </div>
 </li>
                <li> <span class="li-head">vlan_name</span> - List of FortiSwitch VLANs. Source system.interface.name. <span class="li-normal">type: str</span> <span class="li-required">required: true</span>
 <a id='label92' href="javascript:ContentClick('label93', 'label92');" onmouseover="ContentPreview('label93');" onmouseout="ContentUnpreview('label93');" title="click to collapse or expand..."> more... </a>
 <div id="label93" style="display:none">
 <table border="1">
 <tr>
 <td></td>
 <td colspan="1">Supported Version Ranges</td>
 </tr>
 <tr>
 <td>vlan_name</td>
 <td><code class="docutils literal notranslate">v7.0.2 -> 7.4.4 </code></td>
 </tr>
 </table>
 </div>
 </li>
                </ul>
            </ul>
        <li> <span class="li-head">ip_source_guard</span> - IP source guard. <span class="li-normal">type: list</span> <span style="font-family:'Courier New'" class="li-required">member_path: ip_source_guard:port</span>
 <a id='label94' href="javascript:ContentClick('label95', 'label94');" onmouseover="ContentPreview('label95');" onmouseout="ContentUnpreview('label95');" title="click to collapse or expand..."> more... </a>
 <div id="label95" style="display:none">
 <table border="1">
 <tr>
 <td></td><td colspan="1">Supported Version Ranges</td>
 </tr>
 <tr>
 <td>ip_source_guard</td>
 <td><code class="docutils literal notranslate">v6.4.0 -> 7.4.4 </code></td>
 </tr>
 </table>
 </div>
 </li>
            <ul class="ul-self">
            <li> <span class="li-head">binding_entry</span> - IP and MAC address configuration. <span class="li-normal">type: list</span> <span style="font-family:'Courier New'" class="li-required">member_path: ip_source_guard:port/binding_entry:entry_name</span>
 <a id='label96' href="javascript:ContentClick('label97', 'label96');" onmouseover="ContentPreview('label97');" onmouseout="ContentUnpreview('label97');" title="click to collapse or expand..."> more... </a>
 <div id="label97" style="display:none">
 <table border="1">
 <tr>
 <td></td><td colspan="1">Supported Version Ranges</td>
 </tr>
 <tr>
 <td>binding_entry</td>
 <td><code class="docutils literal notranslate">v6.4.0 -> 7.4.4 </code></td>
 </tr>
 </table>
 </div>
 </li>
                <ul class="ul-self">
                <li> <span class="li-head">entry_name</span> - Configure binding pair. <span class="li-normal">type: str</span> <span class="li-required">required: true</span>
 <a id='label98' href="javascript:ContentClick('label99', 'label98');" onmouseover="ContentPreview('label99');" onmouseout="ContentUnpreview('label99');" title="click to collapse or expand..."> more... </a>
 <div id="label99" style="display:none">
 <table border="1">
 <tr>
 <td></td>
 <td colspan="1">Supported Version Ranges</td>
 </tr>
 <tr>
 <td>entry_name</td>
 <td><code class="docutils literal notranslate">v6.4.0 -> 7.4.4 </code></td>
 </tr>
 </table>
 </div>
 </li>
                <li> <span class="li-head">ip</span> - Source IP for this rule. <span class="li-normal">type: str</span>
 <a id='label100' href="javascript:ContentClick('label101', 'label100');" onmouseover="ContentPreview('label101');" onmouseout="ContentUnpreview('label101');" title="click to collapse or expand..."> more... </a>
 <div id="label101" style="display:none">
 <table border="1">
 <tr>
 <td></td>
 <td colspan="1">Supported Version Ranges</td>
 </tr>
 <tr>
 <td>ip</td>
 <td><code class="docutils literal notranslate">v6.4.0 -> 7.4.4 </code></td>
 </tr>
 </table>
 </div>
 </li>
                <li> <span class="li-head">mac</span> - MAC address for this rule. <span class="li-normal">type: str</span>
 <a id='label102' href="javascript:ContentClick('label103', 'label102');" onmouseover="ContentPreview('label103');" onmouseout="ContentUnpreview('label103');" title="click to collapse or expand..."> more... </a>
 <div id="label103" style="display:none">
 <table border="1">
 <tr>
 <td></td>
 <td colspan="1">Supported Version Ranges</td>
 </tr>
 <tr>
 <td>mac</td>
 <td><code class="docutils literal notranslate">v6.4.0 -> 7.4.4 </code></td>
 </tr>
 </table>
 </div>
 </li>
                </ul>
            <li> <span class="li-head">description</span> - Description. <span class="li-normal">type: str</span>
 <a id='label104' href="javascript:ContentClick('label105', 'label104');" onmouseover="ContentPreview('label105');" onmouseout="ContentUnpreview('label105');" title="click to collapse or expand..."> more... </a>
 <div id="label105" style="display:none">
 <table border="1">
 <tr>
 <td></td>
 <td colspan="1">Supported Version Ranges</td>
 </tr>
 <tr>
 <td>description</td>
 <td><code class="docutils literal notranslate">v6.4.0 -> 7.4.4 </code></td>
 </tr>
 </table>
 </div>
 </li>
            <li> <span class="li-head">port</span> - Ingress interface to which source guard is bound. <span class="li-normal">type: str</span> <span class="li-required">required: true</span>
 <a id='label106' href="javascript:ContentClick('label107', 'label106');" onmouseover="ContentPreview('label107');" onmouseout="ContentUnpreview('label107');" title="click to collapse or expand..."> more... </a>
 <div id="label107" style="display:none">
 <table border="1">
 <tr>
 <td></td>
 <td colspan="1">Supported Version Ranges</td>
 </tr>
 <tr>
 <td>port</td>
 <td><code class="docutils literal notranslate">v6.4.0 -> 7.4.4 </code></td>
 </tr>
 </table>
 </div>
 </li>
            </ul>
        <li> <span class="li-head">l3_discovered</span> - Layer 3 management discovered. <span class="li-normal">type: int</span>
 <a id='label108' href="javascript:ContentClick('label109', 'label108');" onmouseover="ContentPreview('label109');" onmouseout="ContentUnpreview('label109');" title="click to collapse or expand..."> more... </a>
 <div id="label109" style="display:none">
 <table border="1">
 <tr>
 <td></td>
 <td colspan="2">Supported Version Ranges</td>
 </tr>
 <tr>
 <td>l3_discovered</td>
 <td><code class="docutils literal notranslate">v6.4.0 -> v7.0.5 </code></td>
 <td><code class="docutils literal notranslate">v7.2.0 -> v7.2.0 </code></td>
 </tr>
 </table>
 </div>
 </li>
        <li> <span class="li-head">max_allowed_trunk_members</span> - FortiSwitch maximum allowed trunk members. <span class="li-normal">type: int</span>
 <a id='label110' href="javascript:ContentClick('label111', 'label110');" onmouseover="ContentPreview('label111');" onmouseout="ContentUnpreview('label111');" title="click to collapse or expand..."> more... </a>
 <div id="label111" style="display:none">
 <table border="1">
 <tr>
 <td></td>
 <td colspan="4">Supported Version Ranges</td>
 </tr>
 <tr>
 <td>max_allowed_trunk_members</td>
 <td><code class="docutils literal notranslate">v6.0.0 -> v6.0.11 </code></td>
 <td><code class="docutils literal notranslate">v6.2.3 -> v6.2.3 </code></td>
 <td><code class="docutils literal notranslate">v6.4.0 -> v6.4.0 </code></td>
 <td><code class="docutils literal notranslate">v6.4.4 -> 7.4.4 </code></td>
 </tr>
 </table>
 </div>
 </li>
        <li> <span class="li-head">mclag_igmp_snooping_aware</span> - Enable/disable MCLAG IGMP-snooping awareness. <span class="li-normal">type: str</span> <span class="li-normal">choices: enable, disable</span>
 <a id='label112' href="javascript:ContentClick('label113', 'label112');" onmouseover="ContentPreview('label113');" onmouseout="ContentUnpreview('label113');" title="click to collapse or expand..."> more... </a>
 <div id="label113" style="display:none">
 <table border="1">
 <tr>
 <td></td>
 <td colspan="1">Supported Version Ranges</td>
 </tr>
 <tr>
 <td>mclag_igmp_snooping_aware</td>
 <td><code class="docutils literal notranslate">v6.2.0 -> 7.4.4 </code></td>
 </tr>
 <tr>
 <td>[enable]</td>
 <td><code class="docutils literal notranslate">v6.2.0 -> 7.4.4</code></td>
 <tr>
 <td>[disable]</td>
 <td><code class="docutils literal notranslate">v6.2.0 -> 7.4.4</code></td>
 </table>
 </div>
 </li>
        <li> <span class="li-head">mgmt_mode</span> - FortiLink management mode. <span class="li-normal">type: int</span>
 <a id='label114' href="javascript:ContentClick('label115', 'label114');" onmouseover="ContentPreview('label115');" onmouseout="ContentUnpreview('label115');" title="click to collapse or expand..."> more... </a>
 <div id="label115" style="display:none">
 <table border="1">
 <tr>
 <td></td>
 <td colspan="1">Supported Version Ranges</td>
 </tr>
 <tr>
 <td>mgmt_mode</td>
 <td><code class="docutils literal notranslate">v7.4.2 -> 7.4.4 </code></td>
 </tr>
 </table>
 </div>
 </li>
        <li> <span class="li-head">mirror</span> - Configuration method to edit FortiSwitch packet mirror. <span class="li-normal">type: list</span> <span style="font-family:'Courier New'" class="li-required">member_path: mirror:name</span>
 <a id='label116' href="javascript:ContentClick('label117', 'label116');" onmouseover="ContentPreview('label117');" onmouseout="ContentUnpreview('label117');" title="click to collapse or expand..."> more... </a>
 <div id="label117" style="display:none">
 <table border="1">
 <tr>
 <td></td><td colspan="1">Supported Version Ranges</td>
 </tr>
 <tr>
 <td>mirror</td>
 <td><code class="docutils literal notranslate">v6.0.0 -> 7.4.4 </code></td>
 </tr>
 </table>
 </div>
 </li>
            <ul class="ul-self">
            <li> <span class="li-head">dst</span> - Destination port. <span class="li-normal">type: str</span>
 <a id='label118' href="javascript:ContentClick('label119', 'label118');" onmouseover="ContentPreview('label119');" onmouseout="ContentUnpreview('label119');" title="click to collapse or expand..."> more... </a>
 <div id="label119" style="display:none">
 <table border="1">
 <tr>
 <td></td>
 <td colspan="1">Supported Version Ranges</td>
 </tr>
 <tr>
 <td>dst</td>
 <td><code class="docutils literal notranslate">v6.0.0 -> 7.4.4 </code></td>
 </tr>
 </table>
 </div>
 </li>
            <li> <span class="li-head">name</span> - Mirror name. <span class="li-normal">type: str</span> <span class="li-required">required: true</span>
 <a id='label120' href="javascript:ContentClick('label121', 'label120');" onmouseover="ContentPreview('label121');" onmouseout="ContentUnpreview('label121');" title="click to collapse or expand..."> more... </a>
 <div id="label121" style="display:none">
 <table border="1">
 <tr>
 <td></td>
 <td colspan="1">Supported Version Ranges</td>
 </tr>
 <tr>
 <td>name</td>
 <td><code class="docutils literal notranslate">v6.0.0 -> 7.4.4 </code></td>
 </tr>
 </table>
 </div>
 </li>
            <li> <span class="li-head">src_egress</span> - Source egress interfaces. <span class="li-normal">type: list</span> <span style="font-family:'Courier New'" class="li-required">member_path: mirror:name/src_egress:name</span>
 <a id='label122' href="javascript:ContentClick('label123', 'label122');" onmouseover="ContentPreview('label123');" onmouseout="ContentUnpreview('label123');" title="click to collapse or expand..."> more... </a>
 <div id="label123" style="display:none">
 <table border="1">
 <tr>
 <td></td><td colspan="1">Supported Version Ranges</td>
 </tr>
 <tr>
 <td>src_egress</td>
 <td><code class="docutils literal notranslate">v6.0.0 -> 7.4.4 </code></td>
 </tr>
 </table>
 </div>
 </li>
                <ul class="ul-self">
                <li> <span class="li-head">name</span> - Interface name. <span class="li-normal">type: str</span> <span class="li-required">required: true</span>
 <a id='label124' href="javascript:ContentClick('label125', 'label124');" onmouseover="ContentPreview('label125');" onmouseout="ContentUnpreview('label125');" title="click to collapse or expand..."> more... </a>
 <div id="label125" style="display:none">
 <table border="1">
 <tr>
 <td></td>
 <td colspan="1">Supported Version Ranges</td>
 </tr>
 <tr>
 <td>name</td>
 <td><code class="docutils literal notranslate">v6.0.0 -> 7.4.4 </code></td>
 </tr>
 </table>
 </div>
 </li>
                </ul>
            <li> <span class="li-head">src_ingress</span> - Source ingress interfaces. <span class="li-normal">type: list</span> <span style="font-family:'Courier New'" class="li-required">member_path: mirror:name/src_ingress:name</span>
 <a id='label126' href="javascript:ContentClick('label127', 'label126');" onmouseover="ContentPreview('label127');" onmouseout="ContentUnpreview('label127');" title="click to collapse or expand..."> more... </a>
 <div id="label127" style="display:none">
 <table border="1">
 <tr>
 <td></td><td colspan="1">Supported Version Ranges</td>
 </tr>
 <tr>
 <td>src_ingress</td>
 <td><code class="docutils literal notranslate">v6.0.0 -> 7.4.4 </code></td>
 </tr>
 </table>
 </div>
 </li>
                <ul class="ul-self">
                <li> <span class="li-head">name</span> - Interface name. <span class="li-normal">type: str</span> <span class="li-required">required: true</span>
 <a id='label128' href="javascript:ContentClick('label129', 'label128');" onmouseover="ContentPreview('label129');" onmouseout="ContentUnpreview('label129');" title="click to collapse or expand..."> more... </a>
 <div id="label129" style="display:none">
 <table border="1">
 <tr>
 <td></td>
 <td colspan="1">Supported Version Ranges</td>
 </tr>
 <tr>
 <td>name</td>
 <td><code class="docutils literal notranslate">v6.0.0 -> 7.4.4 </code></td>
 </tr>
 </table>
 </div>
 </li>
                </ul>
            <li> <span class="li-head">status</span> - Active/inactive mirror configuration. <span class="li-normal">type: str</span> <span class="li-normal">choices: active, inactive</span>
 <a id='label130' href="javascript:ContentClick('label131', 'label130');" onmouseover="ContentPreview('label131');" onmouseout="ContentUnpreview('label131');" title="click to collapse or expand..."> more... </a>
 <div id="label131" style="display:none">
 <table border="1">
 <tr>
 <td></td>
 <td colspan="1">Supported Version Ranges</td>
 </tr>
 <tr>
 <td>status</td>
 <td><code class="docutils literal notranslate">v6.0.0 -> 7.4.4 </code></td>
 </tr>
 <tr>
 <td>[active]</td>
 <td><code class="docutils literal notranslate">v6.0.0 -> 7.4.4</code></td>
 <tr>
 <td>[inactive]</td>
 <td><code class="docutils literal notranslate">v6.0.0 -> 7.4.4</code></td>
 </table>
 </div>
 </li>
            <li> <span class="li-head">switching_packet</span> - Enable/disable switching functionality when mirroring. <span class="li-normal">type: str</span> <span class="li-normal">choices: enable, disable</span>
 <a id='label132' href="javascript:ContentClick('label133', 'label132');" onmouseover="ContentPreview('label133');" onmouseout="ContentUnpreview('label133');" title="click to collapse or expand..."> more... </a>
 <div id="label133" style="display:none">
 <table border="1">
 <tr>
 <td></td>
 <td colspan="1">Supported Version Ranges</td>
 </tr>
 <tr>
 <td>switching_packet</td>
 <td><code class="docutils literal notranslate">v6.0.0 -> 7.4.4 </code></td>
 </tr>
 <tr>
 <td>[enable]</td>
 <td><code class="docutils literal notranslate">v6.0.0 -> 7.4.4</code></td>
 <tr>
 <td>[disable]</td>
 <td><code class="docutils literal notranslate">v6.0.0 -> 7.4.4</code></td>
 </table>
 </div>
 </li>
            </ul>
        <li> <span class="li-head">name</span> - Managed-switch name. <span class="li-normal">type: str</span>
 <a id='label134' href="javascript:ContentClick('label135', 'label134');" onmouseover="ContentPreview('label135');" onmouseout="ContentUnpreview('label135');" title="click to collapse or expand..."> more... </a>
 <div id="label135" style="display:none">
 <table border="1">
 <tr>
 <td></td>
 <td colspan="1">Supported Version Ranges</td>
 </tr>
 <tr>
 <td>name</td>
 <td><code class="docutils literal notranslate">v6.0.0 -> v7.2.4 </code></td>
 </tr>
 </table>
 </div>
 </li>
        <li> <span class="li-head">override_snmp_community</span> - Enable/disable overriding the global SNMP communities. <span class="li-normal">type: str</span> <span class="li-normal">choices: enable, disable</span>
 <a id='label136' href="javascript:ContentClick('label137', 'label136');" onmouseover="ContentPreview('label137');" onmouseout="ContentUnpreview('label137');" title="click to collapse or expand..."> more... </a>
 <div id="label137" style="display:none">
 <table border="1">
 <tr>
 <td></td>
 <td colspan="1">Supported Version Ranges</td>
 </tr>
 <tr>
 <td>override_snmp_community</td>
 <td><code class="docutils literal notranslate">v6.2.0 -> 7.4.4 </code></td>
 </tr>
 <tr>
 <td>[enable]</td>
 <td><code class="docutils literal notranslate">v6.2.0 -> 7.4.4</code></td>
 <tr>
 <td>[disable]</td>
 <td><code class="docutils literal notranslate">v6.2.0 -> 7.4.4</code></td>
 </table>
 </div>
 </li>
        <li> <span class="li-head">override_snmp_sysinfo</span> - Enable/disable overriding the global SNMP system information. <span class="li-normal">type: str</span> <span class="li-normal">choices: disable, enable</span>
 <a id='label138' href="javascript:ContentClick('label139', 'label138');" onmouseover="ContentPreview('label139');" onmouseout="ContentUnpreview('label139');" title="click to collapse or expand..."> more... </a>
 <div id="label139" style="display:none">
 <table border="1">
 <tr>
 <td></td>
 <td colspan="1">Supported Version Ranges</td>
 </tr>
 <tr>
 <td>override_snmp_sysinfo</td>
 <td><code class="docutils literal notranslate">v6.2.0 -> 7.4.4 </code></td>
 </tr>
 <tr>
 <td>[disable]</td>
 <td><code class="docutils literal notranslate">v6.2.0 -> 7.4.4</code></td>
 <tr>
 <td>[enable]</td>
 <td><code class="docutils literal notranslate">v6.2.0 -> 7.4.4</code></td>
 </table>
 </div>
 </li>
        <li> <span class="li-head">override_snmp_trap_threshold</span> - Enable/disable overriding the global SNMP trap threshold values. <span class="li-normal">type: str</span> <span class="li-normal">choices: enable, disable</span>
 <a id='label140' href="javascript:ContentClick('label141', 'label140');" onmouseover="ContentPreview('label141');" onmouseout="ContentUnpreview('label141');" title="click to collapse or expand..."> more... </a>
 <div id="label141" style="display:none">
 <table border="1">
 <tr>
 <td></td>
 <td colspan="1">Supported Version Ranges</td>
 </tr>
 <tr>
 <td>override_snmp_trap_threshold</td>
 <td><code class="docutils literal notranslate">v6.2.0 -> 7.4.4 </code></td>
 </tr>
 <tr>
 <td>[enable]</td>
 <td><code class="docutils literal notranslate">v6.2.0 -> 7.4.4</code></td>
 <tr>
 <td>[disable]</td>
 <td><code class="docutils literal notranslate">v6.2.0 -> 7.4.4</code></td>
 </table>
 </div>
 </li>
        <li> <span class="li-head">override_snmp_user</span> - Enable/disable overriding the global SNMP users. <span class="li-normal">type: str</span> <span class="li-normal">choices: enable, disable</span>
 <a id='label142' href="javascript:ContentClick('label143', 'label142');" onmouseover="ContentPreview('label143');" onmouseout="ContentUnpreview('label143');" title="click to collapse or expand..."> more... </a>
 <div id="label143" style="display:none">
 <table border="1">
 <tr>
 <td></td>
 <td colspan="1">Supported Version Ranges</td>
 </tr>
 <tr>
 <td>override_snmp_user</td>
 <td><code class="docutils literal notranslate">v6.2.0 -> 7.4.4 </code></td>
 </tr>
 <tr>
 <td>[enable]</td>
 <td><code class="docutils literal notranslate">v6.2.0 -> 7.4.4</code></td>
 <tr>
 <td>[disable]</td>
 <td><code class="docutils literal notranslate">v6.2.0 -> 7.4.4</code></td>
 </table>
 </div>
 </li>
        <li> <span class="li-head">owner_vdom</span> - VDOM which owner of port belongs to. <span class="li-normal">type: str</span>
 <a id='label144' href="javascript:ContentClick('label145', 'label144');" onmouseover="ContentPreview('label145');" onmouseout="ContentUnpreview('label145');" title="click to collapse or expand..."> more... </a>
 <div id="label145" style="display:none">
 <table border="1">
 <tr>
 <td></td>
 <td colspan="1">Supported Version Ranges</td>
 </tr>
 <tr>
 <td>owner_vdom</td>
 <td><code class="docutils literal notranslate">v6.0.0 -> 7.4.4 </code></td>
 </tr>
 </table>
 </div>
 </li>
        <li> <span class="li-head">poe_detection_type</span> - PoE detection type for FortiSwitch. <span class="li-normal">type: int</span>
 <a id='label146' href="javascript:ContentClick('label147', 'label146');" onmouseover="ContentPreview('label147');" onmouseout="ContentUnpreview('label147');" title="click to collapse or expand..."> more... </a>
 <div id="label147" style="display:none">
 <table border="1">
 <tr>
 <td></td>
 <td colspan="1">Supported Version Ranges</td>
 </tr>
 <tr>
 <td>poe_detection_type</td>
 <td><code class="docutils literal notranslate">v6.0.0 -> 7.4.4 </code></td>
 </tr>
 </table>
 </div>
 </li>
        <li> <span class="li-head">poe_lldp_detection</span> - Enable/disable PoE LLDP detection. <span class="li-normal">type: str</span> <span class="li-normal">choices: enable, disable</span>
 <a id='label148' href="javascript:ContentClick('label149', 'label148');" onmouseover="ContentPreview('label149');" onmouseout="ContentUnpreview('label149');" title="click to collapse or expand..."> more... </a>
 <div id="label149" style="display:none">
 <table border="1">
 <tr>
 <td></td>
 <td colspan="1">Supported Version Ranges</td>
 </tr>
 <tr>
 <td>poe_lldp_detection</td>
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
        <li> <span class="li-head">poe_pre_standard_detection</span> - Enable/disable PoE pre-standard detection. <span class="li-normal">type: str</span> <span class="li-normal">choices: enable, disable</span>
 <a id='label150' href="javascript:ContentClick('label151', 'label150');" onmouseover="ContentPreview('label151');" onmouseout="ContentUnpreview('label151');" title="click to collapse or expand..."> more... </a>
 <div id="label151" style="display:none">
 <table border="1">
 <tr>
 <td></td>
 <td colspan="1">Supported Version Ranges</td>
 </tr>
 <tr>
 <td>poe_pre_standard_detection</td>
 <td><code class="docutils literal notranslate">v6.0.0 -> 7.4.4 </code></td>
 </tr>
 <tr>
 <td>[enable]</td>
 <td><code class="docutils literal notranslate">v6.0.0 -> 7.4.4</code></td>
 <tr>
 <td>[disable]</td>
 <td><code class="docutils literal notranslate">v6.0.0 -> 7.4.4</code></td>
 </table>
 </div>
 </li>
        <li> <span class="li-head">ports</span> - Managed-switch port list. <span class="li-normal">type: list</span> <span style="font-family:'Courier New'" class="li-required">member_path: ports:port_name</span>
 <a id='label152' href="javascript:ContentClick('label153', 'label152');" onmouseover="ContentPreview('label153');" onmouseout="ContentUnpreview('label153');" title="click to collapse or expand..."> more... </a>
 <div id="label153" style="display:none">
 <table border="1">
 <tr>
 <td></td><td colspan="1">Supported Version Ranges</td>
 </tr>
 <tr>
 <td>ports</td>
 <td><code class="docutils literal notranslate">v6.0.0 -> 7.4.4 </code></td>
 </tr>
 </table>
 </div>
 </li>
            <ul class="ul-self">
            <li> <span class="li-head">access_mode</span> - Access mode of the port. <span class="li-normal">type: str</span> <span class="li-normal">choices: dynamic, nac, static, normal</span>
 <a id='label154' href="javascript:ContentClick('label155', 'label154');" onmouseover="ContentPreview('label155');" onmouseout="ContentUnpreview('label155');" title="click to collapse or expand..."> more... </a>
 <div id="label155" style="display:none">
 <table border="1">
 <tr>
 <td></td>
 <td colspan="1">Supported Version Ranges</td>
 </tr>
 <tr>
 <td>access_mode</td>
 <td><code class="docutils literal notranslate">v6.4.0 -> 7.4.4 </code></td>
 </tr>
 <tr>
 <td>[dynamic]</td>
 <td><code class="docutils literal notranslate">v7.0.0 -> 7.4.4</code></td>
 </tr>
 <tr>
 <td>[nac]</td>
 <td><code class="docutils literal notranslate">v6.4.0 -> 7.4.4</code></td>
 <tr>
 <td>[static]</td>
 <td><code class="docutils literal notranslate">v7.0.0 -> 7.4.4</code></td>
 </tr>
 <tr>
 <td>[normal]</td>
 <td><code class="docutils literal notranslate">v6.4.0 -> v6.4.4</code></td>
 </tr>
 </table>
 </div>
 </li>
            <li> <span class="li-head">acl_group</span> - ACL groups on this port. <span class="li-normal">type: list</span> <span style="font-family:'Courier New'" class="li-required">member_path: ports:port_name/acl_group:name</span>
 <a id='label156' href="javascript:ContentClick('label157', 'label156');" onmouseover="ContentPreview('label157');" onmouseout="ContentUnpreview('label157');" title="click to collapse or expand..."> more... </a>
 <div id="label157" style="display:none">
 <table border="1">
 <tr>
 <td></td><td colspan="1">Supported Version Ranges</td>
 </tr>
 <tr>
 <td>acl_group</td>
 <td><code class="docutils literal notranslate">v7.4.0 -> 7.4.4 </code></td>
 </tr>
 </table>
 </div>
 </li>
                <ul class="ul-self">
                <li> <span class="li-head">name</span> - ACL group name. Source switch-controller.acl.group.name. <span class="li-normal">type: str</span> <span class="li-required">required: true</span>
 <a id='label158' href="javascript:ContentClick('label159', 'label158');" onmouseover="ContentPreview('label159');" onmouseout="ContentUnpreview('label159');" title="click to collapse or expand..."> more... </a>
 <div id="label159" style="display:none">
 <table border="1">
 <tr>
 <td></td>
 <td colspan="1">Supported Version Ranges</td>
 </tr>
 <tr>
 <td>name</td>
 <td><code class="docutils literal notranslate">v7.4.0 -> 7.4.4 </code></td>
 </tr>
 </table>
 </div>
 </li>
                </ul>
            <li> <span class="li-head">aggregator_mode</span> - LACP member select mode. <span class="li-normal">type: str</span> <span class="li-normal">choices: bandwidth, count</span>
 <a id='label160' href="javascript:ContentClick('label161', 'label160');" onmouseover="ContentPreview('label161');" onmouseout="ContentUnpreview('label161');" title="click to collapse or expand..."> more... </a>
 <div id="label161" style="display:none">
 <table border="1">
 <tr>
 <td></td>
 <td colspan="2">Supported Version Ranges</td>
 </tr>
 <tr>
 <td>aggregator_mode</td>
 <td><code class="docutils literal notranslate">v6.4.0 -> v6.4.0 </code></td>
 <td><code class="docutils literal notranslate">v6.4.4 -> 7.4.4 </code></td>
 </tr>
 <tr>
 <td>[bandwidth]</td>
 <td><code class="docutils literal notranslate">v6.4.0 -> v6.4.0</code></td>
 <tr>
 <td>[count]</td>
 <td><code class="docutils literal notranslate">v6.4.0 -> v6.4.0</code></td>
 </table>
 </div>
 </li>
            <li> <span class="li-head">allow_arp_monitor</span> - Enable/Disable allow ARP monitor. <span class="li-normal">type: str</span> <span class="li-normal">choices: disable, enable</span>
 <a id='label162' href="javascript:ContentClick('label163', 'label162');" onmouseover="ContentPreview('label163');" onmouseout="ContentUnpreview('label163');" title="click to collapse or expand..."> more... </a>
 <div id="label163" style="display:none">
 <table border="1">
 <tr>
 <td></td>
 <td colspan="1">Supported Version Ranges</td>
 </tr>
 <tr>
 <td>allow_arp_monitor</td>
 <td><code class="docutils literal notranslate">v7.4.4 -> 7.4.4 </code></td>
 </tr>
 <tr>
 <td>[disable]</td>
 <td><code class="docutils literal notranslate">v7.4.4 -> 7.4.4</code></td>
 <tr>
 <td>[enable]</td>
 <td><code class="docutils literal notranslate">v7.4.4 -> 7.4.4</code></td>
 </table>
 </div>
 </li>
            <li> <span class="li-head">allowed_vlans</span> - Configure switch port tagged VLANs. <span class="li-normal">type: list</span> <span style="font-family:'Courier New'" class="li-required">member_path: ports:port_name/allowed_vlans:vlan_name</span>
 <a id='label164' href="javascript:ContentClick('label165', 'label164');" onmouseover="ContentPreview('label165');" onmouseout="ContentUnpreview('label165');" title="click to collapse or expand..."> more... </a>
 <div id="label165" style="display:none">
 <table border="1">
 <tr>
 <td></td><td colspan="1">Supported Version Ranges</td>
 </tr>
 <tr>
 <td>allowed_vlans</td>
 <td><code class="docutils literal notranslate">v6.0.0 -> 7.4.4 </code></td>
 </tr>
 </table>
 </div>
 </li>
                <ul class="ul-self">
                <li> <span class="li-head">vlan_name</span> - VLAN name. Source system.interface.name. <span class="li-normal">type: str</span> <span class="li-required">required: true</span>
 <a id='label166' href="javascript:ContentClick('label167', 'label166');" onmouseover="ContentPreview('label167');" onmouseout="ContentUnpreview('label167');" title="click to collapse or expand..."> more... </a>
 <div id="label167" style="display:none">
 <table border="1">
 <tr>
 <td></td>
 <td colspan="1">Supported Version Ranges</td>
 </tr>
 <tr>
 <td>vlan_name</td>
 <td><code class="docutils literal notranslate">v6.0.0 -> 7.4.4 </code></td>
 </tr>
 </table>
 </div>
 </li>
                </ul>
            <li> <span class="li-head">allowed_vlans_all</span> - Enable/disable all defined vlans on this port. <span class="li-normal">type: str</span> <span class="li-normal">choices: enable, disable</span>
 <a id='label168' href="javascript:ContentClick('label169', 'label168');" onmouseover="ContentPreview('label169');" onmouseout="ContentUnpreview('label169');" title="click to collapse or expand..."> more... </a>
 <div id="label169" style="display:none">
 <table border="1">
 <tr>
 <td></td>
 <td colspan="1">Supported Version Ranges</td>
 </tr>
 <tr>
 <td>allowed_vlans_all</td>
 <td><code class="docutils literal notranslate">v6.0.0 -> 7.4.4 </code></td>
 </tr>
 <tr>
 <td>[enable]</td>
 <td><code class="docutils literal notranslate">v6.0.0 -> 7.4.4</code></td>
 <tr>
 <td>[disable]</td>
 <td><code class="docutils literal notranslate">v6.0.0 -> 7.4.4</code></td>
 </table>
 </div>
 </li>
            <li> <span class="li-head">arp_inspection_trust</span> - Trusted or untrusted dynamic ARP inspection. <span class="li-normal">type: str</span> <span class="li-normal">choices: untrusted, trusted</span>
 <a id='label170' href="javascript:ContentClick('label171', 'label170');" onmouseover="ContentPreview('label171');" onmouseout="ContentUnpreview('label171');" title="click to collapse or expand..."> more... </a>
 <div id="label171" style="display:none">
 <table border="1">
 <tr>
 <td></td>
 <td colspan="1">Supported Version Ranges</td>
 </tr>
 <tr>
 <td>arp_inspection_trust</td>
 <td><code class="docutils literal notranslate">v6.0.0 -> 7.4.4 </code></td>
 </tr>
 <tr>
 <td>[untrusted]</td>
 <td><code class="docutils literal notranslate">v6.0.0 -> 7.4.4</code></td>
 <tr>
 <td>[trusted]</td>
 <td><code class="docutils literal notranslate">v6.0.0 -> 7.4.4</code></td>
 </table>
 </div>
 </li>
            <li> <span class="li-head">bundle</span> - Enable/disable Link Aggregation Group (LAG) bundling for non-FortiLink interfaces. <span class="li-normal">type: str</span> <span class="li-normal">choices: enable, disable</span>
 <a id='label172' href="javascript:ContentClick('label173', 'label172');" onmouseover="ContentPreview('label173');" onmouseout="ContentUnpreview('label173');" title="click to collapse or expand..."> more... </a>
 <div id="label173" style="display:none">
 <table border="1">
 <tr>
 <td></td>
 <td colspan="1">Supported Version Ranges</td>
 </tr>
 <tr>
 <td>bundle</td>
 <td><code class="docutils literal notranslate">v6.0.0 -> 7.4.4 </code></td>
 </tr>
 <tr>
 <td>[enable]</td>
 <td><code class="docutils literal notranslate">v6.0.0 -> 7.4.4</code></td>
 <tr>
 <td>[disable]</td>
 <td><code class="docutils literal notranslate">v6.0.0 -> 7.4.4</code></td>
 </table>
 </div>
 </li>
            <li> <span class="li-head">description</span> - Description for port. <span class="li-normal">type: str</span>
 <a id='label174' href="javascript:ContentClick('label175', 'label174');" onmouseover="ContentPreview('label175');" onmouseout="ContentUnpreview('label175');" title="click to collapse or expand..."> more... </a>
 <div id="label175" style="display:none">
 <table border="1">
 <tr>
 <td></td>
 <td colspan="1">Supported Version Ranges</td>
 </tr>
 <tr>
 <td>description</td>
 <td><code class="docutils literal notranslate">v6.0.0 -> 7.4.4 </code></td>
 </tr>
 </table>
 </div>
 </li>
            <li> <span class="li-head">dhcp_snoop_option82_override</span> - Configure DHCP snooping option 82 override. <span class="li-normal">type: list</span> <span style="font-family:'Courier New'" class="li-required">member_path: ports:port_name/dhcp_snoop_option82_override:vlan_name</span>
 <a id='label176' href="javascript:ContentClick('label177', 'label176');" onmouseover="ContentPreview('label177');" onmouseout="ContentUnpreview('label177');" title="click to collapse or expand..."> more... </a>
 <div id="label177" style="display:none">
 <table border="1">
 <tr>
 <td></td><td colspan="1">Supported Version Ranges</td>
 </tr>
 <tr>
 <td>dhcp_snoop_option82_override</td>
 <td><code class="docutils literal notranslate">v7.4.0 -> 7.4.4 </code></td>
 </tr>
 </table>
 </div>
 </li>
                <ul class="ul-self">
                <li> <span class="li-head">circuit_id</span> - Circuit ID string. <span class="li-normal">type: str</span>
 <a id='label178' href="javascript:ContentClick('label179', 'label178');" onmouseover="ContentPreview('label179');" onmouseout="ContentUnpreview('label179');" title="click to collapse or expand..."> more... </a>
 <div id="label179" style="display:none">
 <table border="1">
 <tr>
 <td></td>
 <td colspan="1">Supported Version Ranges</td>
 </tr>
 <tr>
 <td>circuit_id</td>
 <td><code class="docutils literal notranslate">v7.4.0 -> 7.4.4 </code></td>
 </tr>
 </table>
 </div>
 </li>
                <li> <span class="li-head">remote_id</span> - Remote ID string. <span class="li-normal">type: str</span>
 <a id='label180' href="javascript:ContentClick('label181', 'label180');" onmouseover="ContentPreview('label181');" onmouseout="ContentUnpreview('label181');" title="click to collapse or expand..."> more... </a>
 <div id="label181" style="display:none">
 <table border="1">
 <tr>
 <td></td>
 <td colspan="1">Supported Version Ranges</td>
 </tr>
 <tr>
 <td>remote_id</td>
 <td><code class="docutils literal notranslate">v7.4.0 -> 7.4.4 </code></td>
 </tr>
 </table>
 </div>
 </li>
                <li> <span class="li-head">vlan_name</span> - DHCP snooping option 82 VLAN. Source system.interface.name. <span class="li-normal">type: str</span> <span class="li-required">required: true</span>
 <a id='label182' href="javascript:ContentClick('label183', 'label182');" onmouseover="ContentPreview('label183');" onmouseout="ContentUnpreview('label183');" title="click to collapse or expand..."> more... </a>
 <div id="label183" style="display:none">
 <table border="1">
 <tr>
 <td></td>
 <td colspan="1">Supported Version Ranges</td>
 </tr>
 <tr>
 <td>vlan_name</td>
 <td><code class="docutils literal notranslate">v7.4.0 -> 7.4.4 </code></td>
 </tr>
 </table>
 </div>
 </li>
                </ul>
            <li> <span class="li-head">dhcp_snoop_option82_trust</span> - Enable/disable allowance of DHCP with option-82 on untrusted interface. <span class="li-normal">type: str</span> <span class="li-normal">choices: enable, disable</span>
 <a id='label184' href="javascript:ContentClick('label185', 'label184');" onmouseover="ContentPreview('label185');" onmouseout="ContentUnpreview('label185');" title="click to collapse or expand..."> more... </a>
 <div id="label185" style="display:none">
 <table border="1">
 <tr>
 <td></td>
 <td colspan="1">Supported Version Ranges</td>
 </tr>
 <tr>
 <td>dhcp_snoop_option82_trust</td>
 <td><code class="docutils literal notranslate">v6.0.0 -> 7.4.4 </code></td>
 </tr>
 <tr>
 <td>[enable]</td>
 <td><code class="docutils literal notranslate">v6.0.0 -> 7.4.4</code></td>
 <tr>
 <td>[disable]</td>
 <td><code class="docutils literal notranslate">v6.0.0 -> 7.4.4</code></td>
 </table>
 </div>
 </li>
            <li> <span class="li-head">dhcp_snooping</span> - Trusted or untrusted DHCP-snooping interface. <span class="li-normal">type: str</span> <span class="li-normal">choices: untrusted, trusted</span>
 <a id='label186' href="javascript:ContentClick('label187', 'label186');" onmouseover="ContentPreview('label187');" onmouseout="ContentUnpreview('label187');" title="click to collapse or expand..."> more... </a>
 <div id="label187" style="display:none">
 <table border="1">
 <tr>
 <td></td>
 <td colspan="1">Supported Version Ranges</td>
 </tr>
 <tr>
 <td>dhcp_snooping</td>
 <td><code class="docutils literal notranslate">v6.0.0 -> 7.4.4 </code></td>
 </tr>
 <tr>
 <td>[untrusted]</td>
 <td><code class="docutils literal notranslate">v6.0.0 -> 7.4.4</code></td>
 <tr>
 <td>[trusted]</td>
 <td><code class="docutils literal notranslate">v6.0.0 -> 7.4.4</code></td>
 </table>
 </div>
 </li>
            <li> <span class="li-head">discard_mode</span> - Configure discard mode for port. <span class="li-normal">type: str</span> <span class="li-normal">choices: none, all-untagged, all-tagged</span>
 <a id='label188' href="javascript:ContentClick('label189', 'label188');" onmouseover="ContentPreview('label189');" onmouseout="ContentUnpreview('label189');" title="click to collapse or expand..."> more... </a>
 <div id="label189" style="display:none">
 <table border="1">
 <tr>
 <td></td>
 <td colspan="1">Supported Version Ranges</td>
 </tr>
 <tr>
 <td>discard_mode</td>
 <td><code class="docutils literal notranslate">v6.0.0 -> 7.4.4 </code></td>
 </tr>
 <tr>
 <td>[none]</td>
 <td><code class="docutils literal notranslate">v6.0.0 -> 7.4.4</code></td>
 <tr>
 <td>[all-untagged]</td>
 <td><code class="docutils literal notranslate">v6.0.0 -> 7.4.4</code></td>
 <tr>
 <td>[all-tagged]</td>
 <td><code class="docutils literal notranslate">v6.0.0 -> 7.4.4</code></td>
 </table>
 </div>
 </li>
            <li> <span class="li-head">edge_port</span> - Enable/disable this interface as an edge port, bridging connections between workstations and/or computers. <span class="li-normal">type: str</span> <span class="li-normal">choices: enable, disable</span>
 <a id='label190' href="javascript:ContentClick('label191', 'label190');" onmouseover="ContentPreview('label191');" onmouseout="ContentUnpreview('label191');" title="click to collapse or expand..."> more... </a>
 <div id="label191" style="display:none">
 <table border="1">
 <tr>
 <td></td>
 <td colspan="1">Supported Version Ranges</td>
 </tr>
 <tr>
 <td>edge_port</td>
 <td><code class="docutils literal notranslate">v6.0.0 -> 7.4.4 </code></td>
 </tr>
 <tr>
 <td>[enable]</td>
 <td><code class="docutils literal notranslate">v6.0.0 -> 7.4.4</code></td>
 <tr>
 <td>[disable]</td>
 <td><code class="docutils literal notranslate">v6.0.0 -> 7.4.4</code></td>
 </table>
 </div>
 </li>
            <li> <span class="li-head">export_tags</span> - Configure export tag(s) for FortiSwitch port when exported to a virtual port pool. <span class="li-normal">type: list</span> <span style="font-family:'Courier New'" class="li-required">member_path: ports:port_name/export_tags:tag_name</span>
 <a id='label192' href="javascript:ContentClick('label193', 'label192');" onmouseover="ContentPreview('label193');" onmouseout="ContentUnpreview('label193');" title="click to collapse or expand..."> more... </a>
 <div id="label193" style="display:none">
 <table border="1">
 <tr>
 <td></td><td colspan="1">Supported Version Ranges</td>
 </tr>
 <tr>
 <td>export_tags</td>
 <td><code class="docutils literal notranslate">v6.0.0 -> v7.0.1 </code></td>
 </tr>
 </table>
 </div>
 </li>
                <ul class="ul-self">
                <li> <span class="li-head">tag_name</span> - FortiSwitch port tag name when exported to a virtual port pool. Source switch-controller.switch-interface-tag.name. <span class="li-normal">type: str</span> <span class="li-required">required: true</span>
 <a id='label194' href="javascript:ContentClick('label195', 'label194');" onmouseover="ContentPreview('label195');" onmouseout="ContentUnpreview('label195');" title="click to collapse or expand..."> more... </a>
 <div id="label195" style="display:none">
 <table border="1">
 <tr>
 <td></td>
 <td colspan="1">Supported Version Ranges</td>
 </tr>
 <tr>
 <td>tag_name</td>
 <td><code class="docutils literal notranslate">v6.0.0 -> v7.0.1 </code></td>
 </tr>
 </table>
 </div>
 </li>
                </ul>
            <li> <span class="li-head">export_to</span> - Export managed-switch port to a tenant VDOM. Source system.vdom.name. <span class="li-normal">type: str</span>
 <a id='label196' href="javascript:ContentClick('label197', 'label196');" onmouseover="ContentPreview('label197');" onmouseout="ContentUnpreview('label197');" title="click to collapse or expand..."> more... </a>
 <div id="label197" style="display:none">
 <table border="1">
 <tr>
 <td></td>
 <td colspan="1">Supported Version Ranges</td>
 </tr>
 <tr>
 <td>export_to</td>
 <td><code class="docutils literal notranslate">v6.0.0 -> 7.4.4 </code></td>
 </tr>
 </table>
 </div>
 </li>
            <li> <span class="li-head">export_to_pool</span> - Switch controller export port to pool-list. Source switch-controller.virtual-port-pool.name. <span class="li-normal">type: str</span>
 <a id='label198' href="javascript:ContentClick('label199', 'label198');" onmouseover="ContentPreview('label199');" onmouseout="ContentUnpreview('label199');" title="click to collapse or expand..."> more... </a>
 <div id="label199" style="display:none">
 <table border="1">
 <tr>
 <td></td>
 <td colspan="1">Supported Version Ranges</td>
 </tr>
 <tr>
 <td>export_to_pool</td>
 <td><code class="docutils literal notranslate">v6.0.0 -> 7.4.4 </code></td>
 </tr>
 </table>
 </div>
 </li>
            <li> <span class="li-head">export_to_pool_flag</span> - Switch controller export port to pool-list. <span class="li-normal">type: int</span>
 <a id='label200' href="javascript:ContentClick('label201', 'label200');" onmouseover="ContentPreview('label201');" onmouseout="ContentUnpreview('label201');" title="click to collapse or expand..."> more... </a>
 <div id="label201" style="display:none">
 <table border="1">
 <tr>
 <td></td>
 <td colspan="2">Supported Version Ranges</td>
 </tr>
 <tr>
 <td>export_to_pool_flag</td>
 <td><code class="docutils literal notranslate">v6.0.0 -> v6.0.11 </code></td>
 <td><code class="docutils literal notranslate">v6.2.3 -> v6.2.3 </code></td>
 </tr>
 </table>
 </div>
 </li>
            <li> <span class="li-head">fallback_port</span> - LACP fallback port. <span class="li-normal">type: str</span>
 <a id='label202' href="javascript:ContentClick('label203', 'label202');" onmouseover="ContentPreview('label203');" onmouseout="ContentUnpreview('label203');" title="click to collapse or expand..."> more... </a>
 <div id="label203" style="display:none">
 <table border="1">
 <tr>
 <td></td>
 <td colspan="1">Supported Version Ranges</td>
 </tr>
 <tr>
 <td>fallback_port</td>
 <td><code class="docutils literal notranslate">v7.4.4 -> 7.4.4 </code></td>
 </tr>
 </table>
 </div>
 </li>
            <li> <span class="li-head">fec_capable</span> - FEC capable. <span class="li-normal">type: int</span>
 <a id='label204' href="javascript:ContentClick('label205', 'label204');" onmouseover="ContentPreview('label205');" onmouseout="ContentUnpreview('label205');" title="click to collapse or expand..."> more... </a>
 <div id="label205" style="display:none">
 <table border="1">
 <tr>
 <td></td>
 <td colspan="1">Supported Version Ranges</td>
 </tr>
 <tr>
 <td>fec_capable</td>
 <td><code class="docutils literal notranslate">v7.0.0 -> 7.4.4 </code></td>
 </tr>
 </table>
 </div>
 </li>
            <li> <span class="li-head">fec_state</span> - State of forward error correction. <span class="li-normal">type: str</span> <span class="li-normal">choices: disabled, cl74, cl91, detect-by-module</span>
 <a id='label206' href="javascript:ContentClick('label207', 'label206');" onmouseover="ContentPreview('label207');" onmouseout="ContentUnpreview('label207');" title="click to collapse or expand..."> more... </a>
 <div id="label207" style="display:none">
 <table border="1">
 <tr>
 <td></td>
 <td colspan="1">Supported Version Ranges</td>
 </tr>
 <tr>
 <td>fec_state</td>
 <td><code class="docutils literal notranslate">v7.0.0 -> 7.4.4 </code></td>
 </tr>
 <tr>
 <td>[disabled]</td>
 <td><code class="docutils literal notranslate">v7.0.0 -> 7.4.4</code></td>
 <tr>
 <td>[cl74]</td>
 <td><code class="docutils literal notranslate">v7.0.0 -> 7.4.4</code></td>
 <tr>
 <td>[cl91]</td>
 <td><code class="docutils literal notranslate">v7.0.0 -> 7.4.4</code></td>
 <tr>
 <td>[detect-by-module]</td>
 <td><code class="docutils literal notranslate">v7.4.2 -> 7.4.4</code></td>
 </tr>
 </table>
 </div>
 </li>
            <li> <span class="li-head">fgt_peer_device_name</span> - FGT peer device name. <span class="li-normal">type: str</span>
 <a id='label208' href="javascript:ContentClick('label209', 'label208');" onmouseover="ContentPreview('label209');" onmouseout="ContentUnpreview('label209');" title="click to collapse or expand..."> more... </a>
 <div id="label209" style="display:none">
 <table border="1">
 <tr>
 <td></td>
 <td colspan="2">Supported Version Ranges</td>
 </tr>
 <tr>
 <td>fgt_peer_device_name</td>
 <td><code class="docutils literal notranslate">v6.0.0 -> v7.0.5 </code></td>
 <td><code class="docutils literal notranslate">v7.2.0 -> v7.2.0 </code></td>
 </tr>
 </table>
 </div>
 </li>
            <li> <span class="li-head">fgt_peer_port_name</span> - FGT peer port name. <span class="li-normal">type: str</span>
 <a id='label210' href="javascript:ContentClick('label211', 'label210');" onmouseover="ContentPreview('label211');" onmouseout="ContentUnpreview('label211');" title="click to collapse or expand..."> more... </a>
 <div id="label211" style="display:none">
 <table border="1">
 <tr>
 <td></td>
 <td colspan="2">Supported Version Ranges</td>
 </tr>
 <tr>
 <td>fgt_peer_port_name</td>
 <td><code class="docutils literal notranslate">v6.0.0 -> v7.0.5 </code></td>
 <td><code class="docutils literal notranslate">v7.2.0 -> v7.2.0 </code></td>
 </tr>
 </table>
 </div>
 </li>
            <li> <span class="li-head">fiber_port</span> - Fiber-port. <span class="li-normal">type: int</span>
 <a id='label212' href="javascript:ContentClick('label213', 'label212');" onmouseover="ContentPreview('label213');" onmouseout="ContentUnpreview('label213');" title="click to collapse or expand..."> more... </a>
 <div id="label213" style="display:none">
 <table border="1">
 <tr>
 <td></td>
 <td colspan="2">Supported Version Ranges</td>
 </tr>
 <tr>
 <td>fiber_port</td>
 <td><code class="docutils literal notranslate">v6.0.0 -> v7.0.5 </code></td>
 <td><code class="docutils literal notranslate">v7.2.0 -> v7.2.0 </code></td>
 </tr>
 </table>
 </div>
 </li>
            <li> <span class="li-head">flags</span> - Port properties flags. <span class="li-normal">type: int</span>
 <a id='label214' href="javascript:ContentClick('label215', 'label214');" onmouseover="ContentPreview('label215');" onmouseout="ContentUnpreview('label215');" title="click to collapse or expand..."> more... </a>
 <div id="label215" style="display:none">
 <table border="1">
 <tr>
 <td></td>
 <td colspan="2">Supported Version Ranges</td>
 </tr>
 <tr>
 <td>flags</td>
 <td><code class="docutils literal notranslate">v6.0.0 -> v7.0.5 </code></td>
 <td><code class="docutils literal notranslate">v7.2.0 -> v7.2.0 </code></td>
 </tr>
 </table>
 </div>
 </li>
            <li> <span class="li-head">flap_duration</span> - Period over which flap events are calculated (seconds). <span class="li-normal">type: int</span>
 <a id='label216' href="javascript:ContentClick('label217', 'label216');" onmouseover="ContentPreview('label217');" onmouseout="ContentUnpreview('label217');" title="click to collapse or expand..."> more... </a>
 <div id="label217" style="display:none">
 <table border="1">
 <tr>
 <td></td>
 <td colspan="1">Supported Version Ranges</td>
 </tr>
 <tr>
 <td>flap_duration</td>
 <td><code class="docutils literal notranslate">v7.2.0 -> 7.4.4 </code></td>
 </tr>
 </table>
 </div>
 </li>
            <li> <span class="li-head">flap_rate</span> - Number of stage change events needed within flap-duration. <span class="li-normal">type: int</span>
 <a id='label218' href="javascript:ContentClick('label219', 'label218');" onmouseover="ContentPreview('label219');" onmouseout="ContentUnpreview('label219');" title="click to collapse or expand..."> more... </a>
 <div id="label219" style="display:none">
 <table border="1">
 <tr>
 <td></td>
 <td colspan="1">Supported Version Ranges</td>
 </tr>
 <tr>
 <td>flap_rate</td>
 <td><code class="docutils literal notranslate">v7.2.0 -> 7.4.4 </code></td>
 </tr>
 </table>
 </div>
 </li>
            <li> <span class="li-head">flap_timeout</span> - Flap guard disabling protection (min). <span class="li-normal">type: int</span>
 <a id='label220' href="javascript:ContentClick('label221', 'label220');" onmouseover="ContentPreview('label221');" onmouseout="ContentUnpreview('label221');" title="click to collapse or expand..."> more... </a>
 <div id="label221" style="display:none">
 <table border="1">
 <tr>
 <td></td>
 <td colspan="1">Supported Version Ranges</td>
 </tr>
 <tr>
 <td>flap_timeout</td>
 <td><code class="docutils literal notranslate">v7.2.0 -> 7.4.4 </code></td>
 </tr>
 </table>
 </div>
 </li>
            <li> <span class="li-head">flapguard</span> - Enable/disable flap guard. <span class="li-normal">type: str</span> <span class="li-normal">choices: enable, disable</span>
 <a id='label222' href="javascript:ContentClick('label223', 'label222');" onmouseover="ContentPreview('label223');" onmouseout="ContentUnpreview('label223');" title="click to collapse or expand..."> more... </a>
 <div id="label223" style="display:none">
 <table border="1">
 <tr>
 <td></td>
 <td colspan="1">Supported Version Ranges</td>
 </tr>
 <tr>
 <td>flapguard</td>
 <td><code class="docutils literal notranslate">v7.2.0 -> 7.4.4 </code></td>
 </tr>
 <tr>
 <td>[enable]</td>
 <td><code class="docutils literal notranslate">v7.2.0 -> 7.4.4</code></td>
 <tr>
 <td>[disable]</td>
 <td><code class="docutils literal notranslate">v7.2.0 -> 7.4.4</code></td>
 </table>
 </div>
 </li>
            <li> <span class="li-head">flow_control</span> - Flow control direction. <span class="li-normal">type: str</span> <span class="li-normal">choices: disable, tx, rx, both</span>
 <a id='label224' href="javascript:ContentClick('label225', 'label224');" onmouseover="ContentPreview('label225');" onmouseout="ContentUnpreview('label225');" title="click to collapse or expand..."> more... </a>
 <div id="label225" style="display:none">
 <table border="1">
 <tr>
 <td></td>
 <td colspan="1">Supported Version Ranges</td>
 </tr>
 <tr>
 <td>flow_control</td>
 <td><code class="docutils literal notranslate">v6.4.4 -> 7.4.4 </code></td>
 </tr>
 <tr>
 <td>[disable]</td>
 <td><code class="docutils literal notranslate">v6.4.4 -> 7.4.4</code></td>
 <tr>
 <td>[tx]</td>
 <td><code class="docutils literal notranslate">v6.4.4 -> 7.4.4</code></td>
 <tr>
 <td>[rx]</td>
 <td><code class="docutils literal notranslate">v6.4.4 -> 7.4.4</code></td>
 <tr>
 <td>[both]</td>
 <td><code class="docutils literal notranslate">v6.4.4 -> 7.4.4</code></td>
 </table>
 </div>
 </li>
            <li> <span class="li-head">fortilink_port</span> - FortiLink uplink port. <span class="li-normal">type: int</span>
 <a id='label226' href="javascript:ContentClick('label227', 'label226');" onmouseover="ContentPreview('label227');" onmouseout="ContentUnpreview('label227');" title="click to collapse or expand..."> more... </a>
 <div id="label227" style="display:none">
 <table border="1">
 <tr>
 <td></td>
 <td colspan="2">Supported Version Ranges</td>
 </tr>
 <tr>
 <td>fortilink_port</td>
 <td><code class="docutils literal notranslate">v6.0.0 -> v7.0.5 </code></td>
 <td><code class="docutils literal notranslate">v7.2.0 -> v7.2.0 </code></td>
 </tr>
 </table>
 </div>
 </li>
            <li> <span class="li-head">fortiswitch_acls</span> - ACLs on this port. <span class="li-normal">type: list</span> <span style="font-family:'Courier New'" class="li-required">member_path: ports:port_name/fortiswitch_acls:id</span>
 <a id='label228' href="javascript:ContentClick('label229', 'label228');" onmouseover="ContentPreview('label229');" onmouseout="ContentUnpreview('label229');" title="click to collapse or expand..."> more... </a>
 <div id="label229" style="display:none">
 <table border="1">
 <tr>
 <td></td><td colspan="1">Supported Version Ranges</td>
 </tr>
 <tr>
 <td>fortiswitch_acls</td>
 <td><code class="docutils literal notranslate">v7.4.0 -> 7.4.4 </code></td>
 </tr>
 </table>
 </div>
 </li>
                <ul class="ul-self">
                <li> <span class="li-head">id</span> - ACL ID. see <a href='#notes'>Notes</a>. <span class="li-normal">type: int</span> <span class="li-required">required: true</span>
 <a id='label230' href="javascript:ContentClick('label231', 'label230');" onmouseover="ContentPreview('label231');" onmouseout="ContentUnpreview('label231');" title="click to collapse or expand..."> more... </a>
 <div id="label231" style="display:none">
 <table border="1">
 <tr>
 <td></td>
 <td colspan="1">Supported Version Ranges</td>
 </tr>
 <tr>
 <td>id</td>
 <td><code class="docutils literal notranslate">v7.4.0 -> 7.4.4 </code></td>
 </tr>
 </table>
 </div>
 </li>
                </ul>
            <li> <span class="li-head">igmp_snooping</span> - Set IGMP snooping mode for the physical port interface. <span class="li-normal">type: str</span> <span class="li-normal">choices: enable, disable</span>
 <a id='label232' href="javascript:ContentClick('label233', 'label232');" onmouseover="ContentPreview('label233');" onmouseout="ContentUnpreview('label233');" title="click to collapse or expand..."> more... </a>
 <div id="label233" style="display:none">
 <table border="1">
 <tr>
 <td></td>
 <td colspan="1">Supported Version Ranges</td>
 </tr>
 <tr>
 <td>igmp_snooping</td>
 <td><code class="docutils literal notranslate">v6.0.0 -> v6.2.7 </code></td>
 </tr>
 <tr>
 <td>[enable]</td>
 <td><code class="docutils literal notranslate">v6.0.0 -> v6.2.7</code></td>
 <tr>
 <td>[disable]</td>
 <td><code class="docutils literal notranslate">v6.0.0 -> v6.2.7</code></td>
 </table>
 </div>
 </li>
            <li> <span class="li-head">igmp_snooping_flood_reports</span> - Enable/disable flooding of IGMP reports to this interface when igmp-snooping enabled. <span class="li-normal">type: str</span> <span class="li-normal">choices: enable, disable</span>
 <a id='label234' href="javascript:ContentClick('label235', 'label234');" onmouseover="ContentPreview('label235');" onmouseout="ContentUnpreview('label235');" title="click to collapse or expand..."> more... </a>
 <div id="label235" style="display:none">
 <table border="1">
 <tr>
 <td></td>
 <td colspan="1">Supported Version Ranges</td>
 </tr>
 <tr>
 <td>igmp_snooping_flood_reports</td>
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
            <li> <span class="li-head">igmps_flood_reports</span> - Enable/disable flooding of IGMP reports to this interface when igmp-snooping enabled. <span class="li-normal">type: str</span> <span class="li-normal">choices: enable, disable</span>
 <a id='label236' href="javascript:ContentClick('label237', 'label236');" onmouseover="ContentPreview('label237');" onmouseout="ContentUnpreview('label237');" title="click to collapse or expand..."> more... </a>
 <div id="label237" style="display:none">
 <table border="1">
 <tr>
 <td></td>
 <td colspan="1">Supported Version Ranges</td>
 </tr>
 <tr>
 <td>igmps_flood_reports</td>
 <td><code class="docutils literal notranslate">v6.0.0 -> v7.2.0 </code></td>
 </tr>
 <tr>
 <td>[enable]</td>
 <td><code class="docutils literal notranslate">v6.0.0 -> v7.2.0</code></td>
 <tr>
 <td>[disable]</td>
 <td><code class="docutils literal notranslate">v6.0.0 -> v7.2.0</code></td>
 </table>
 </div>
 </li>
            <li> <span class="li-head">igmps_flood_traffic</span> - Enable/disable flooding of IGMP snooping traffic to this interface. <span class="li-normal">type: str</span> <span class="li-normal">choices: enable, disable</span>
 <a id='label238' href="javascript:ContentClick('label239', 'label238');" onmouseover="ContentPreview('label239');" onmouseout="ContentUnpreview('label239');" title="click to collapse or expand..."> more... </a>
 <div id="label239" style="display:none">
 <table border="1">
 <tr>
 <td></td>
 <td colspan="1">Supported Version Ranges</td>
 </tr>
 <tr>
 <td>igmps_flood_traffic</td>
 <td><code class="docutils literal notranslate">v6.0.0 -> v7.2.0 </code></td>
 </tr>
 <tr>
 <td>[enable]</td>
 <td><code class="docutils literal notranslate">v6.0.0 -> v7.2.0</code></td>
 <tr>
 <td>[disable]</td>
 <td><code class="docutils literal notranslate">v6.0.0 -> v7.2.0</code></td>
 </table>
 </div>
 </li>
            <li> <span class="li-head">interface_tags</span> - Tag(s) associated with the interface for various features including virtual port pool, dynamic port policy. <span class="li-normal">type: list</span> <span style="font-family:'Courier New'" class="li-required">member_path: ports:port_name/interface_tags:tag_name</span>
 <a id='label240' href="javascript:ContentClick('label241', 'label240');" onmouseover="ContentPreview('label241');" onmouseout="ContentUnpreview('label241');" title="click to collapse or expand..."> more... </a>
 <div id="label241" style="display:none">
 <table border="1">
 <tr>
 <td></td><td colspan="1">Supported Version Ranges</td>
 </tr>
 <tr>
 <td>interface_tags</td>
 <td><code class="docutils literal notranslate">v7.0.2 -> 7.4.4 </code></td>
 </tr>
 </table>
 </div>
 </li>
                <ul class="ul-self">
                <li> <span class="li-head">tag_name</span> - FortiSwitch port tag name when exported to a virtual port pool or matched to dynamic port policy. Source switch-controller.switch-interface-tag.name. <span class="li-normal">type: str</span> <span class="li-required">required: true</span>
 <a id='label242' href="javascript:ContentClick('label243', 'label242');" onmouseover="ContentPreview('label243');" onmouseout="ContentUnpreview('label243');" title="click to collapse or expand..."> more... </a>
 <div id="label243" style="display:none">
 <table border="1">
 <tr>
 <td></td>
 <td colspan="1">Supported Version Ranges</td>
 </tr>
 <tr>
 <td>tag_name</td>
 <td><code class="docutils literal notranslate">v7.0.2 -> 7.4.4 </code></td>
 </tr>
 </table>
 </div>
 </li>
                </ul>
            <li> <span class="li-head">ip_source_guard</span> - Enable/disable IP source guard. <span class="li-normal">type: str</span> <span class="li-normal">choices: disable, enable</span>
 <a id='label244' href="javascript:ContentClick('label245', 'label244');" onmouseover="ContentPreview('label245');" onmouseout="ContentUnpreview('label245');" title="click to collapse or expand..."> more... </a>
 <div id="label245" style="display:none">
 <table border="1">
 <tr>
 <td></td>
 <td colspan="1">Supported Version Ranges</td>
 </tr>
 <tr>
 <td>ip_source_guard</td>
 <td><code class="docutils literal notranslate">v6.4.0 -> 7.4.4 </code></td>
 </tr>
 <tr>
 <td>[disable]</td>
 <td><code class="docutils literal notranslate">v6.4.0 -> 7.4.4</code></td>
 <tr>
 <td>[enable]</td>
 <td><code class="docutils literal notranslate">v6.4.0 -> 7.4.4</code></td>
 </table>
 </div>
 </li>
            <li> <span class="li-head">isl_local_trunk_name</span> - ISL local trunk name. <span class="li-normal">type: str</span>
 <a id='label246' href="javascript:ContentClick('label247', 'label246');" onmouseover="ContentPreview('label247');" onmouseout="ContentUnpreview('label247');" title="click to collapse or expand..."> more... </a>
 <div id="label247" style="display:none">
 <table border="1">
 <tr>
 <td></td>
 <td colspan="2">Supported Version Ranges</td>
 </tr>
 <tr>
 <td>isl_local_trunk_name</td>
 <td><code class="docutils literal notranslate">v6.0.0 -> v7.0.5 </code></td>
 <td><code class="docutils literal notranslate">v7.2.0 -> v7.2.0 </code></td>
 </tr>
 </table>
 </div>
 </li>
            <li> <span class="li-head">isl_peer_device_name</span> - ISL peer device name. <span class="li-normal">type: str</span>
 <a id='label248' href="javascript:ContentClick('label249', 'label248');" onmouseover="ContentPreview('label249');" onmouseout="ContentUnpreview('label249');" title="click to collapse or expand..."> more... </a>
 <div id="label249" style="display:none">
 <table border="1">
 <tr>
 <td></td>
 <td colspan="2">Supported Version Ranges</td>
 </tr>
 <tr>
 <td>isl_peer_device_name</td>
 <td><code class="docutils literal notranslate">v6.0.0 -> v7.0.5 </code></td>
 <td><code class="docutils literal notranslate">v7.2.0 -> v7.2.0 </code></td>
 </tr>
 </table>
 </div>
 </li>
            <li> <span class="li-head">isl_peer_port_name</span> - ISL peer port name. <span class="li-normal">type: str</span>
 <a id='label250' href="javascript:ContentClick('label251', 'label250');" onmouseover="ContentPreview('label251');" onmouseout="ContentUnpreview('label251');" title="click to collapse or expand..."> more... </a>
 <div id="label251" style="display:none">
 <table border="1">
 <tr>
 <td></td>
 <td colspan="2">Supported Version Ranges</td>
 </tr>
 <tr>
 <td>isl_peer_port_name</td>
 <td><code class="docutils literal notranslate">v6.0.0 -> v7.0.5 </code></td>
 <td><code class="docutils literal notranslate">v7.2.0 -> v7.2.0 </code></td>
 </tr>
 </table>
 </div>
 </li>
            <li> <span class="li-head">lacp_speed</span> - End Link Aggregation Control Protocol (LACP) messages every 30 seconds (slow) or every second (fast). <span class="li-normal">type: str</span> <span class="li-normal">choices: slow, fast</span>
 <a id='label252' href="javascript:ContentClick('label253', 'label252');" onmouseover="ContentPreview('label253');" onmouseout="ContentUnpreview('label253');" title="click to collapse or expand..."> more... </a>
 <div id="label253" style="display:none">
 <table border="1">
 <tr>
 <td></td>
 <td colspan="1">Supported Version Ranges</td>
 </tr>
 <tr>
 <td>lacp_speed</td>
 <td><code class="docutils literal notranslate">v6.0.0 -> 7.4.4 </code></td>
 </tr>
 <tr>
 <td>[slow]</td>
 <td><code class="docutils literal notranslate">v6.0.0 -> 7.4.4</code></td>
 <tr>
 <td>[fast]</td>
 <td><code class="docutils literal notranslate">v6.0.0 -> 7.4.4</code></td>
 </table>
 </div>
 </li>
            <li> <span class="li-head">learning_limit</span> - Limit the number of dynamic MAC addresses on this Port (1 - 128, 0 = no limit, default). <span class="li-normal">type: int</span>
 <a id='label254' href="javascript:ContentClick('label255', 'label254');" onmouseover="ContentPreview('label255');" onmouseout="ContentUnpreview('label255');" title="click to collapse or expand..."> more... </a>
 <div id="label255" style="display:none">
 <table border="1">
 <tr>
 <td></td>
 <td colspan="1">Supported Version Ranges</td>
 </tr>
 <tr>
 <td>learning_limit</td>
 <td><code class="docutils literal notranslate">v6.0.0 -> 7.4.4 </code></td>
 </tr>
 </table>
 </div>
 </li>
            <li> <span class="li-head">lldp_profile</span> - LLDP port TLV profile. Source switch-controller.lldp-profile.name. <span class="li-normal">type: str</span>
 <a id='label256' href="javascript:ContentClick('label257', 'label256');" onmouseover="ContentPreview('label257');" onmouseout="ContentUnpreview('label257');" title="click to collapse or expand..."> more... </a>
 <div id="label257" style="display:none">
 <table border="1">
 <tr>
 <td></td>
 <td colspan="1">Supported Version Ranges</td>
 </tr>
 <tr>
 <td>lldp_profile</td>
 <td><code class="docutils literal notranslate">v6.0.0 -> 7.4.4 </code></td>
 </tr>
 </table>
 </div>
 </li>
            <li> <span class="li-head">lldp_status</span> - LLDP transmit and receive status. <span class="li-normal">type: str</span> <span class="li-normal">choices: disable, rx-only, tx-only, tx-rx</span>
 <a id='label258' href="javascript:ContentClick('label259', 'label258');" onmouseover="ContentPreview('label259');" onmouseout="ContentUnpreview('label259');" title="click to collapse or expand..."> more... </a>
 <div id="label259" style="display:none">
 <table border="1">
 <tr>
 <td></td>
 <td colspan="1">Supported Version Ranges</td>
 </tr>
 <tr>
 <td>lldp_status</td>
 <td><code class="docutils literal notranslate">v6.0.0 -> 7.4.4 </code></td>
 </tr>
 <tr>
 <td>[disable]</td>
 <td><code class="docutils literal notranslate">v6.0.0 -> 7.4.4</code></td>
 <tr>
 <td>[rx-only]</td>
 <td><code class="docutils literal notranslate">v6.0.0 -> 7.4.4</code></td>
 <tr>
 <td>[tx-only]</td>
 <td><code class="docutils literal notranslate">v6.0.0 -> 7.4.4</code></td>
 <tr>
 <td>[tx-rx]</td>
 <td><code class="docutils literal notranslate">v6.0.0 -> 7.4.4</code></td>
 </table>
 </div>
 </li>
            <li> <span class="li-head">loop_guard</span> - Enable/disable loop-guard on this interface, an STP optimization used to prevent network loops. <span class="li-normal">type: str</span> <span class="li-normal">choices: enabled, disabled</span>
 <a id='label260' href="javascript:ContentClick('label261', 'label260');" onmouseover="ContentPreview('label261');" onmouseout="ContentUnpreview('label261');" title="click to collapse or expand..."> more... </a>
 <div id="label261" style="display:none">
 <table border="1">
 <tr>
 <td></td>
 <td colspan="1">Supported Version Ranges</td>
 </tr>
 <tr>
 <td>loop_guard</td>
 <td><code class="docutils literal notranslate">v6.0.0 -> 7.4.4 </code></td>
 </tr>
 <tr>
 <td>[enabled]</td>
 <td><code class="docutils literal notranslate">v6.0.0 -> 7.4.4</code></td>
 <tr>
 <td>[disabled]</td>
 <td><code class="docutils literal notranslate">v6.0.0 -> 7.4.4</code></td>
 </table>
 </div>
 </li>
            <li> <span class="li-head">loop_guard_timeout</span> - Loop-guard timeout (0 - 120 min). <span class="li-normal">type: int</span>
 <a id='label262' href="javascript:ContentClick('label263', 'label262');" onmouseover="ContentPreview('label263');" onmouseout="ContentUnpreview('label263');" title="click to collapse or expand..."> more... </a>
 <div id="label263" style="display:none">
 <table border="1">
 <tr>
 <td></td>
 <td colspan="1">Supported Version Ranges</td>
 </tr>
 <tr>
 <td>loop_guard_timeout</td>
 <td><code class="docutils literal notranslate">v6.0.0 -> 7.4.4 </code></td>
 </tr>
 </table>
 </div>
 </li>
            <li> <span class="li-head">mac_addr</span> - Port/Trunk MAC. <span class="li-normal">type: str</span>
 <a id='label264' href="javascript:ContentClick('label265', 'label264');" onmouseover="ContentPreview('label265');" onmouseout="ContentUnpreview('label265');" title="click to collapse or expand..."> more... </a>
 <div id="label265" style="display:none">
 <table border="1">
 <tr>
 <td></td>
 <td colspan="1">Supported Version Ranges</td>
 </tr>
 <tr>
 <td>mac_addr</td>
 <td><code class="docutils literal notranslate">v6.2.0 -> 7.4.4 </code></td>
 </tr>
 </table>
 </div>
 </li>
            <li> <span class="li-head">matched_dpp_intf_tags</span> - Matched interface tags in the dynamic port policy. <span class="li-normal">type: str</span>
 <a id='label266' href="javascript:ContentClick('label267', 'label266');" onmouseover="ContentPreview('label267');" onmouseout="ContentUnpreview('label267');" title="click to collapse or expand..."> more... </a>
 <div id="label267" style="display:none">
 <table border="1">
 <tr>
 <td></td>
 <td colspan="1">Supported Version Ranges</td>
 </tr>
 <tr>
 <td>matched_dpp_intf_tags</td>
 <td><code class="docutils literal notranslate">v7.0.0 -> 7.4.4 </code></td>
 </tr>
 </table>
 </div>
 </li>
            <li> <span class="li-head">matched_dpp_policy</span> - Matched child policy in the dynamic port policy. <span class="li-normal">type: str</span>
 <a id='label268' href="javascript:ContentClick('label269', 'label268');" onmouseover="ContentPreview('label269');" onmouseout="ContentUnpreview('label269');" title="click to collapse or expand..."> more... </a>
 <div id="label269" style="display:none">
 <table border="1">
 <tr>
 <td></td>
 <td colspan="1">Supported Version Ranges</td>
 </tr>
 <tr>
 <td>matched_dpp_policy</td>
 <td><code class="docutils literal notranslate">v7.0.0 -> 7.4.4 </code></td>
 </tr>
 </table>
 </div>
 </li>
            <li> <span class="li-head">max_bundle</span> - Maximum size of LAG bundle (1 - 24). <span class="li-normal">type: int</span>
 <a id='label270' href="javascript:ContentClick('label271', 'label270');" onmouseover="ContentPreview('label271');" onmouseout="ContentUnpreview('label271');" title="click to collapse or expand..."> more... </a>
 <div id="label271" style="display:none">
 <table border="1">
 <tr>
 <td></td>
 <td colspan="1">Supported Version Ranges</td>
 </tr>
 <tr>
 <td>max_bundle</td>
 <td><code class="docutils literal notranslate">v6.0.0 -> 7.4.4 </code></td>
 </tr>
 </table>
 </div>
 </li>
            <li> <span class="li-head">mcast_snooping_flood_traffic</span> - Enable/disable flooding of IGMP snooping traffic to this interface. <span class="li-normal">type: str</span> <span class="li-normal">choices: enable, disable</span>
 <a id='label272' href="javascript:ContentClick('label273', 'label272');" onmouseover="ContentPreview('label273');" onmouseout="ContentUnpreview('label273');" title="click to collapse or expand..."> more... </a>
 <div id="label273" style="display:none">
 <table border="1">
 <tr>
 <td></td>
 <td colspan="1">Supported Version Ranges</td>
 </tr>
 <tr>
 <td>mcast_snooping_flood_traffic</td>
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
            <li> <span class="li-head">mclag</span> - Enable/disable multi-chassis link aggregation (MCLAG). <span class="li-normal">type: str</span> <span class="li-normal">choices: enable, disable</span>
 <a id='label274' href="javascript:ContentClick('label275', 'label274');" onmouseover="ContentPreview('label275');" onmouseout="ContentUnpreview('label275');" title="click to collapse or expand..."> more... </a>
 <div id="label275" style="display:none">
 <table border="1">
 <tr>
 <td></td>
 <td colspan="1">Supported Version Ranges</td>
 </tr>
 <tr>
 <td>mclag</td>
 <td><code class="docutils literal notranslate">v6.0.0 -> 7.4.4 </code></td>
 </tr>
 <tr>
 <td>[enable]</td>
 <td><code class="docutils literal notranslate">v6.0.0 -> 7.4.4</code></td>
 <tr>
 <td>[disable]</td>
 <td><code class="docutils literal notranslate">v6.0.0 -> 7.4.4</code></td>
 </table>
 </div>
 </li>
            <li> <span class="li-head">mclag_icl_port</span> - MCLAG-ICL port. <span class="li-normal">type: int</span>
 <a id='label276' href="javascript:ContentClick('label277', 'label276');" onmouseover="ContentPreview('label277');" onmouseout="ContentUnpreview('label277');" title="click to collapse or expand..."> more... </a>
 <div id="label277" style="display:none">
 <table border="1">
 <tr>
 <td></td>
 <td colspan="2">Supported Version Ranges</td>
 </tr>
 <tr>
 <td>mclag_icl_port</td>
 <td><code class="docutils literal notranslate">v6.4.0 -> v7.0.5 </code></td>
 <td><code class="docutils literal notranslate">v7.2.0 -> v7.2.0 </code></td>
 </tr>
 </table>
 </div>
 </li>
            <li> <span class="li-head">media_type</span> - Media type. <span class="li-normal">type: str</span>
 <a id='label278' href="javascript:ContentClick('label279', 'label278');" onmouseover="ContentPreview('label279');" onmouseout="ContentUnpreview('label279');" title="click to collapse or expand..."> more... </a>
 <div id="label279" style="display:none">
 <table border="1">
 <tr>
 <td></td>
 <td colspan="2">Supported Version Ranges</td>
 </tr>
 <tr>
 <td>media_type</td>
 <td><code class="docutils literal notranslate">v6.4.4 -> v7.0.5 </code></td>
 <td><code class="docutils literal notranslate">v7.2.0 -> v7.2.0 </code></td>
 </tr>
 </table>
 </div>
 </li>
            <li> <span class="li-head">member_withdrawal_behavior</span> - Port behavior after it withdraws because of loss of control packets. <span class="li-normal">type: str</span> <span class="li-normal">choices: forward, block</span>
 <a id='label280' href="javascript:ContentClick('label281', 'label280');" onmouseover="ContentPreview('label281');" onmouseout="ContentUnpreview('label281');" title="click to collapse or expand..."> more... </a>
 <div id="label281" style="display:none">
 <table border="1">
 <tr>
 <td></td>
 <td colspan="1">Supported Version Ranges</td>
 </tr>
 <tr>
 <td>member_withdrawal_behavior</td>
 <td><code class="docutils literal notranslate">v6.0.0 -> 7.4.4 </code></td>
 </tr>
 <tr>
 <td>[forward]</td>
 <td><code class="docutils literal notranslate">v6.0.0 -> 7.4.4</code></td>
 <tr>
 <td>[block]</td>
 <td><code class="docutils literal notranslate">v6.0.0 -> 7.4.4</code></td>
 </table>
 </div>
 </li>
            <li> <span class="li-head">members</span> - Aggregated LAG bundle interfaces. <span class="li-normal">type: list</span> <span style="font-family:'Courier New'" class="li-required">member_path: ports:port_name/members:member_name</span>
 <a id='label282' href="javascript:ContentClick('label283', 'label282');" onmouseover="ContentPreview('label283');" onmouseout="ContentUnpreview('label283');" title="click to collapse or expand..."> more... </a>
 <div id="label283" style="display:none">
 <table border="1">
 <tr>
 <td></td><td colspan="1">Supported Version Ranges</td>
 </tr>
 <tr>
 <td>members</td>
 <td><code class="docutils literal notranslate">v6.0.0 -> 7.4.4 </code></td>
 </tr>
 </table>
 </div>
 </li>
                <ul class="ul-self">
                <li> <span class="li-head">member_name</span> - Interface name from available options. <span class="li-normal">type: str</span> <span class="li-required">required: true</span>
 <a id='label284' href="javascript:ContentClick('label285', 'label284');" onmouseover="ContentPreview('label285');" onmouseout="ContentUnpreview('label285');" title="click to collapse or expand..."> more... </a>
 <div id="label285" style="display:none">
 <table border="1">
 <tr>
 <td></td>
 <td colspan="1">Supported Version Ranges</td>
 </tr>
 <tr>
 <td>member_name</td>
 <td><code class="docutils literal notranslate">v6.0.0 -> 7.4.4 </code></td>
 </tr>
 </table>
 </div>
 </li>
                </ul>
            <li> <span class="li-head">min_bundle</span> - Minimum size of LAG bundle (1 - 24). <span class="li-normal">type: int</span>
 <a id='label286' href="javascript:ContentClick('label287', 'label286');" onmouseover="ContentPreview('label287');" onmouseout="ContentUnpreview('label287');" title="click to collapse or expand..."> more... </a>
 <div id="label287" style="display:none">
 <table border="1">
 <tr>
 <td></td>
 <td colspan="1">Supported Version Ranges</td>
 </tr>
 <tr>
 <td>min_bundle</td>
 <td><code class="docutils literal notranslate">v6.0.0 -> 7.4.4 </code></td>
 </tr>
 </table>
 </div>
 </li>
            <li> <span class="li-head">mode</span> - LACP mode: ignore and do not send control messages, or negotiate 802.3ad aggregation passively or actively. <span class="li-normal">type: str</span> <span class="li-normal">choices: static, lacp-passive, lacp-active</span>
 <a id='label288' href="javascript:ContentClick('label289', 'label288');" onmouseover="ContentPreview('label289');" onmouseout="ContentUnpreview('label289');" title="click to collapse or expand..."> more... </a>
 <div id="label289" style="display:none">
 <table border="1">
 <tr>
 <td></td>
 <td colspan="1">Supported Version Ranges</td>
 </tr>
 <tr>
 <td>mode</td>
 <td><code class="docutils literal notranslate">v6.0.0 -> 7.4.4 </code></td>
 </tr>
 <tr>
 <td>[static]</td>
 <td><code class="docutils literal notranslate">v6.0.0 -> 7.4.4</code></td>
 <tr>
 <td>[lacp-passive]</td>
 <td><code class="docutils literal notranslate">v6.0.0 -> 7.4.4</code></td>
 <tr>
 <td>[lacp-active]</td>
 <td><code class="docutils literal notranslate">v6.0.0 -> 7.4.4</code></td>
 </table>
 </div>
 </li>
            <li> <span class="li-head">p2p_port</span> - General peer to peer tunnel port. <span class="li-normal">type: int</span>
 <a id='label290' href="javascript:ContentClick('label291', 'label290');" onmouseover="ContentPreview('label291');" onmouseout="ContentUnpreview('label291');" title="click to collapse or expand..."> more... </a>
 <div id="label291" style="display:none">
 <table border="1">
 <tr>
 <td></td>
 <td colspan="2">Supported Version Ranges</td>
 </tr>
 <tr>
 <td>p2p_port</td>
 <td><code class="docutils literal notranslate">v6.4.0 -> v7.0.5 </code></td>
 <td><code class="docutils literal notranslate">v7.2.0 -> v7.2.0 </code></td>
 </tr>
 </table>
 </div>
 </li>
            <li> <span class="li-head">packet_sample_rate</span> - Packet sampling rate (0 - 99999 p/sec). <span class="li-normal">type: int</span>
 <a id='label292' href="javascript:ContentClick('label293', 'label292');" onmouseover="ContentPreview('label293');" onmouseout="ContentUnpreview('label293');" title="click to collapse or expand..."> more... </a>
 <div id="label293" style="display:none">
 <table border="1">
 <tr>
 <td></td>
 <td colspan="1">Supported Version Ranges</td>
 </tr>
 <tr>
 <td>packet_sample_rate</td>
 <td><code class="docutils literal notranslate">v6.2.0 -> 7.4.4 </code></td>
 </tr>
 </table>
 </div>
 </li>
            <li> <span class="li-head">packet_sampler</span> - Enable/disable packet sampling on this interface. <span class="li-normal">type: str</span> <span class="li-normal">choices: enabled, disabled</span>
 <a id='label294' href="javascript:ContentClick('label295', 'label294');" onmouseover="ContentPreview('label295');" onmouseout="ContentUnpreview('label295');" title="click to collapse or expand..."> more... </a>
 <div id="label295" style="display:none">
 <table border="1">
 <tr>
 <td></td>
 <td colspan="1">Supported Version Ranges</td>
 </tr>
 <tr>
 <td>packet_sampler</td>
 <td><code class="docutils literal notranslate">v6.2.0 -> 7.4.4 </code></td>
 </tr>
 <tr>
 <td>[enabled]</td>
 <td><code class="docutils literal notranslate">v6.2.0 -> 7.4.4</code></td>
 <tr>
 <td>[disabled]</td>
 <td><code class="docutils literal notranslate">v6.2.0 -> 7.4.4</code></td>
 </table>
 </div>
 </li>
            <li> <span class="li-head">pause_meter</span> - Configure ingress pause metering rate, in kbps . <span class="li-normal">type: int</span>
 <a id='label296' href="javascript:ContentClick('label297', 'label296');" onmouseover="ContentPreview('label297');" onmouseout="ContentUnpreview('label297');" title="click to collapse or expand..."> more... </a>
 <div id="label297" style="display:none">
 <table border="1">
 <tr>
 <td></td>
 <td colspan="1">Supported Version Ranges</td>
 </tr>
 <tr>
 <td>pause_meter</td>
 <td><code class="docutils literal notranslate">v6.4.4 -> 7.4.4 </code></td>
 </tr>
 </table>
 </div>
 </li>
            <li> <span class="li-head">pause_meter_resume</span> - Resume threshold for resuming traffic on ingress port. <span class="li-normal">type: str</span> <span class="li-normal">choices: 75%, 50%, 25%</span>
 <a id='label298' href="javascript:ContentClick('label299', 'label298');" onmouseover="ContentPreview('label299');" onmouseout="ContentUnpreview('label299');" title="click to collapse or expand..."> more... </a>
 <div id="label299" style="display:none">
 <table border="1">
 <tr>
 <td></td>
 <td colspan="1">Supported Version Ranges</td>
 </tr>
 <tr>
 <td>pause_meter_resume</td>
 <td><code class="docutils literal notranslate">v6.4.4 -> 7.4.4 </code></td>
 </tr>
 <tr>
 <td>[75%]</td>
 <td><code class="docutils literal notranslate">v6.4.4 -> 7.4.4</code></td>
 <tr>
 <td>[50%]</td>
 <td><code class="docutils literal notranslate">v6.4.4 -> 7.4.4</code></td>
 <tr>
 <td>[25%]</td>
 <td><code class="docutils literal notranslate">v6.4.4 -> 7.4.4</code></td>
 </table>
 </div>
 </li>
            <li> <span class="li-head">poe_capable</span> - PoE capable. <span class="li-normal">type: int</span>
 <a id='label300' href="javascript:ContentClick('label301', 'label300');" onmouseover="ContentPreview('label301');" onmouseout="ContentUnpreview('label301');" title="click to collapse or expand..."> more... </a>
 <div id="label301" style="display:none">
 <table border="1">
 <tr>
 <td></td>
 <td colspan="1">Supported Version Ranges</td>
 </tr>
 <tr>
 <td>poe_capable</td>
 <td><code class="docutils literal notranslate">v6.0.0 -> 7.4.4 </code></td>
 </tr>
 </table>
 </div>
 </li>
            <li> <span class="li-head">poe_max_power</span> - PoE maximum power. <span class="li-normal">type: str</span>
 <a id='label302' href="javascript:ContentClick('label303', 'label302');" onmouseover="ContentPreview('label303');" onmouseout="ContentUnpreview('label303');" title="click to collapse or expand..."> more... </a>
 <div id="label303" style="display:none">
 <table border="1">
 <tr>
 <td></td>
 <td colspan="2">Supported Version Ranges</td>
 </tr>
 <tr>
 <td>poe_max_power</td>
 <td><code class="docutils literal notranslate">v7.0.1 -> v7.0.5 </code></td>
 <td><code class="docutils literal notranslate">v7.2.0 -> v7.2.0 </code></td>
 </tr>
 </table>
 </div>
 </li>
            <li> <span class="li-head">poe_mode_bt_cabable</span> - PoE mode IEEE 802.3BT capable. <span class="li-normal">type: int</span>
 <a id='label304' href="javascript:ContentClick('label305', 'label304');" onmouseover="ContentPreview('label305');" onmouseout="ContentUnpreview('label305');" title="click to collapse or expand..."> more... </a>
 <div id="label305" style="display:none">
 <table border="1">
 <tr>
 <td></td>
 <td colspan="1">Supported Version Ranges</td>
 </tr>
 <tr>
 <td>poe_mode_bt_cabable</td>
 <td><code class="docutils literal notranslate">v7.2.4 -> 7.4.4 </code></td>
 </tr>
 </table>
 </div>
 </li>
            <li> <span class="li-head">poe_port_mode</span> - Configure PoE port mode. <span class="li-normal">type: str</span> <span class="li-normal">choices: ieee802-3af, ieee802-3at, ieee802-3bt</span>
 <a id='label306' href="javascript:ContentClick('label307', 'label306');" onmouseover="ContentPreview('label307');" onmouseout="ContentUnpreview('label307');" title="click to collapse or expand..."> more... </a>
 <div id="label307" style="display:none">
 <table border="1">
 <tr>
 <td></td>
 <td colspan="1">Supported Version Ranges</td>
 </tr>
 <tr>
 <td>poe_port_mode</td>
 <td><code class="docutils literal notranslate">v7.2.4 -> 7.4.4 </code></td>
 </tr>
 <tr>
 <td>[ieee802-3af]</td>
 <td><code class="docutils literal notranslate">v7.2.4 -> 7.4.4</code></td>
 <tr>
 <td>[ieee802-3at]</td>
 <td><code class="docutils literal notranslate">v7.2.4 -> 7.4.4</code></td>
 <tr>
 <td>[ieee802-3bt]</td>
 <td><code class="docutils literal notranslate">v7.2.4 -> 7.4.4</code></td>
 </table>
 </div>
 </li>
            <li> <span class="li-head">poe_port_power</span> - Configure PoE port power. <span class="li-normal">type: str</span> <span class="li-normal">choices: normal, perpetual, perpetual-fast</span>
 <a id='label308' href="javascript:ContentClick('label309', 'label308');" onmouseover="ContentPreview('label309');" onmouseout="ContentUnpreview('label309');" title="click to collapse or expand..."> more... </a>
 <div id="label309" style="display:none">
 <table border="1">
 <tr>
 <td></td>
 <td colspan="1">Supported Version Ranges</td>
 </tr>
 <tr>
 <td>poe_port_power</td>
 <td><code class="docutils literal notranslate">v7.2.4 -> 7.4.4 </code></td>
 </tr>
 <tr>
 <td>[normal]</td>
 <td><code class="docutils literal notranslate">v7.2.4 -> 7.4.4</code></td>
 <tr>
 <td>[perpetual]</td>
 <td><code class="docutils literal notranslate">v7.2.4 -> 7.4.4</code></td>
 <tr>
 <td>[perpetual-fast]</td>
 <td><code class="docutils literal notranslate">v7.2.4 -> 7.4.4</code></td>
 </table>
 </div>
 </li>
            <li> <span class="li-head">poe_port_priority</span> - Configure PoE port priority. <span class="li-normal">type: str</span> <span class="li-normal">choices: critical-priority, high-priority, low-priority, medium-priority</span>
 <a id='label310' href="javascript:ContentClick('label311', 'label310');" onmouseover="ContentPreview('label311');" onmouseout="ContentUnpreview('label311');" title="click to collapse or expand..."> more... </a>
 <div id="label311" style="display:none">
 <table border="1">
 <tr>
 <td></td>
 <td colspan="1">Supported Version Ranges</td>
 </tr>
 <tr>
 <td>poe_port_priority</td>
 <td><code class="docutils literal notranslate">v7.2.4 -> 7.4.4 </code></td>
 </tr>
 <tr>
 <td>[critical-priority]</td>
 <td><code class="docutils literal notranslate">v7.2.4 -> 7.4.4</code></td>
 <tr>
 <td>[high-priority]</td>
 <td><code class="docutils literal notranslate">v7.2.4 -> 7.4.4</code></td>
 <tr>
 <td>[low-priority]</td>
 <td><code class="docutils literal notranslate">v7.2.4 -> 7.4.4</code></td>
 <tr>
 <td>[medium-priority]</td>
 <td><code class="docutils literal notranslate">v7.2.4 -> 7.4.4</code></td>
 </table>
 </div>
 </li>
            <li> <span class="li-head">poe_pre_standard_detection</span> - Enable/disable PoE pre-standard detection. <span class="li-normal">type: str</span> <span class="li-normal">choices: enable, disable</span>
 <a id='label312' href="javascript:ContentClick('label313', 'label312');" onmouseover="ContentPreview('label313');" onmouseout="ContentUnpreview('label313');" title="click to collapse or expand..."> more... </a>
 <div id="label313" style="display:none">
 <table border="1">
 <tr>
 <td></td>
 <td colspan="1">Supported Version Ranges</td>
 </tr>
 <tr>
 <td>poe_pre_standard_detection</td>
 <td><code class="docutils literal notranslate">v6.0.0 -> 7.4.4 </code></td>
 </tr>
 <tr>
 <td>[enable]</td>
 <td><code class="docutils literal notranslate">v6.0.0 -> 7.4.4</code></td>
 <tr>
 <td>[disable]</td>
 <td><code class="docutils literal notranslate">v6.0.0 -> 7.4.4</code></td>
 </table>
 </div>
 </li>
            <li> <span class="li-head">poe_standard</span> - PoE standard supported. <span class="li-normal">type: str</span>
 <a id='label314' href="javascript:ContentClick('label315', 'label314');" onmouseover="ContentPreview('label315');" onmouseout="ContentUnpreview('label315');" title="click to collapse or expand..."> more... </a>
 <div id="label315" style="display:none">
 <table border="1">
 <tr>
 <td></td>
 <td colspan="2">Supported Version Ranges</td>
 </tr>
 <tr>
 <td>poe_standard</td>
 <td><code class="docutils literal notranslate">v7.0.1 -> v7.0.5 </code></td>
 <td><code class="docutils literal notranslate">v7.2.0 -> v7.2.0 </code></td>
 </tr>
 </table>
 </div>
 </li>
            <li> <span class="li-head">poe_status</span> - Enable/disable PoE status. <span class="li-normal">type: str</span> <span class="li-normal">choices: enable, disable</span>
 <a id='label316' href="javascript:ContentClick('label317', 'label316');" onmouseover="ContentPreview('label317');" onmouseout="ContentUnpreview('label317');" title="click to collapse or expand..."> more... </a>
 <div id="label317" style="display:none">
 <table border="1">
 <tr>
 <td></td>
 <td colspan="1">Supported Version Ranges</td>
 </tr>
 <tr>
 <td>poe_status</td>
 <td><code class="docutils literal notranslate">v6.0.0 -> 7.4.4 </code></td>
 </tr>
 <tr>
 <td>[enable]</td>
 <td><code class="docutils literal notranslate">v6.0.0 -> 7.4.4</code></td>
 <tr>
 <td>[disable]</td>
 <td><code class="docutils literal notranslate">v6.0.0 -> 7.4.4</code></td>
 </table>
 </div>
 </li>
            <li> <span class="li-head">port_name</span> - Switch port name. <span class="li-normal">type: str</span> <span class="li-required">required: true</span>
 <a id='label318' href="javascript:ContentClick('label319', 'label318');" onmouseover="ContentPreview('label319');" onmouseout="ContentUnpreview('label319');" title="click to collapse or expand..."> more... </a>
 <div id="label319" style="display:none">
 <table border="1">
 <tr>
 <td></td>
 <td colspan="1">Supported Version Ranges</td>
 </tr>
 <tr>
 <td>port_name</td>
 <td><code class="docutils literal notranslate">v6.0.0 -> 7.4.4 </code></td>
 </tr>
 </table>
 </div>
 </li>
            <li> <span class="li-head">port_number</span> - Port number. <span class="li-normal">type: int</span>
 <a id='label320' href="javascript:ContentClick('label321', 'label320');" onmouseover="ContentPreview('label321');" onmouseout="ContentUnpreview('label321');" title="click to collapse or expand..."> more... </a>
 <div id="label321" style="display:none">
 <table border="1">
 <tr>
 <td></td>
 <td colspan="2">Supported Version Ranges</td>
 </tr>
 <tr>
 <td>port_number</td>
 <td><code class="docutils literal notranslate">v6.0.0 -> v7.0.5 </code></td>
 <td><code class="docutils literal notranslate">v7.2.0 -> v7.2.0 </code></td>
 </tr>
 </table>
 </div>
 </li>
            <li> <span class="li-head">port_owner</span> - Switch port name. <span class="li-normal">type: str</span>
 <a id='label322' href="javascript:ContentClick('label323', 'label322');" onmouseover="ContentPreview('label323');" onmouseout="ContentUnpreview('label323');" title="click to collapse or expand..."> more... </a>
 <div id="label323" style="display:none">
 <table border="1">
 <tr>
 <td></td>
 <td colspan="1">Supported Version Ranges</td>
 </tr>
 <tr>
 <td>port_owner</td>
 <td><code class="docutils literal notranslate">v6.0.0 -> 7.4.4 </code></td>
 </tr>
 </table>
 </div>
 </li>
            <li> <span class="li-head">port_policy</span> - Switch controller dynamic port policy from available options. Source switch-controller.dynamic-port-policy.name. <span class="li-normal">type: str</span>
 <a id='label324' href="javascript:ContentClick('label325', 'label324');" onmouseover="ContentPreview('label325');" onmouseout="ContentUnpreview('label325');" title="click to collapse or expand..."> more... </a>
 <div id="label325" style="display:none">
 <table border="1">
 <tr>
 <td></td>
 <td colspan="1">Supported Version Ranges</td>
 </tr>
 <tr>
 <td>port_policy</td>
 <td><code class="docutils literal notranslate">v7.0.0 -> 7.4.4 </code></td>
 </tr>
 </table>
 </div>
 </li>
            <li> <span class="li-head">port_prefix_type</span> - Port prefix type. <span class="li-normal">type: int</span>
 <a id='label326' href="javascript:ContentClick('label327', 'label326');" onmouseover="ContentPreview('label327');" onmouseout="ContentUnpreview('label327');" title="click to collapse or expand..."> more... </a>
 <div id="label327" style="display:none">
 <table border="1">
 <tr>
 <td></td>
 <td colspan="2">Supported Version Ranges</td>
 </tr>
 <tr>
 <td>port_prefix_type</td>
 <td><code class="docutils literal notranslate">v6.0.0 -> v7.0.5 </code></td>
 <td><code class="docutils literal notranslate">v7.2.0 -> v7.2.0 </code></td>
 </tr>
 </table>
 </div>
 </li>
            <li> <span class="li-head">port_security_policy</span> - Switch controller authentication policy to apply to this managed switch from available options. Source switch-controller .security-policy.802-1X.name. <span class="li-normal">type: str</span>
 <a id='label328' href="javascript:ContentClick('label329', 'label328');" onmouseover="ContentPreview('label329');" onmouseout="ContentUnpreview('label329');" title="click to collapse or expand..."> more... </a>
 <div id="label329" style="display:none">
 <table border="1">
 <tr>
 <td></td>
 <td colspan="1">Supported Version Ranges</td>
 </tr>
 <tr>
 <td>port_security_policy</td>
 <td><code class="docutils literal notranslate">v6.0.0 -> 7.4.4 </code></td>
 </tr>
 </table>
 </div>
 </li>
            <li> <span class="li-head">port_selection_criteria</span> - Algorithm for aggregate port selection. <span class="li-normal">type: str</span> <span class="li-normal">choices: src-mac, dst-mac, src-dst-mac, src-ip, dst-ip, src-dst-ip</span>
 <a id='label330' href="javascript:ContentClick('label331', 'label330');" onmouseover="ContentPreview('label331');" onmouseout="ContentUnpreview('label331');" title="click to collapse or expand..."> more... </a>
 <div id="label331" style="display:none">
 <table border="1">
 <tr>
 <td></td>
 <td colspan="1">Supported Version Ranges</td>
 </tr>
 <tr>
 <td>port_selection_criteria</td>
 <td><code class="docutils literal notranslate">v6.0.0 -> 7.4.4 </code></td>
 </tr>
 <tr>
 <td>[src-mac]</td>
 <td><code class="docutils literal notranslate">v6.0.0 -> 7.4.4</code></td>
 <tr>
 <td>[dst-mac]</td>
 <td><code class="docutils literal notranslate">v6.0.0 -> 7.4.4</code></td>
 <tr>
 <td>[src-dst-mac]</td>
 <td><code class="docutils literal notranslate">v6.0.0 -> 7.4.4</code></td>
 <tr>
 <td>[src-ip]</td>
 <td><code class="docutils literal notranslate">v6.0.0 -> 7.4.4</code></td>
 <tr>
 <td>[dst-ip]</td>
 <td><code class="docutils literal notranslate">v6.0.0 -> 7.4.4</code></td>
 <tr>
 <td>[src-dst-ip]</td>
 <td><code class="docutils literal notranslate">v6.0.0 -> 7.4.4</code></td>
 </table>
 </div>
 </li>
            <li> <span class="li-head">ptp_policy</span> - PTP policy configuration. Source switch-controller.ptp.interface-policy.name. <span class="li-normal">type: str</span>
 <a id='label332' href="javascript:ContentClick('label333', 'label332');" onmouseover="ContentPreview('label333');" onmouseout="ContentUnpreview('label333');" title="click to collapse or expand..."> more... </a>
 <div id="label333" style="display:none">
 <table border="1">
 <tr>
 <td></td>
 <td colspan="2">Supported Version Ranges</td>
 </tr>
 <tr>
 <td>ptp_policy</td>
 <td><code class="docutils literal notranslate">v6.4.0 -> v6.4.0 </code></td>
 <td><code class="docutils literal notranslate">v6.4.4 -> 7.4.4 </code></td>
 </tr>
 </table>
 </div>
 </li>
            <li> <span class="li-head">ptp_status</span> - Enable/disable PTP policy on this FortiSwitch port. <span class="li-normal">type: str</span> <span class="li-normal">choices: disable, enable</span>
 <a id='label334' href="javascript:ContentClick('label335', 'label334');" onmouseover="ContentPreview('label335');" onmouseout="ContentUnpreview('label335');" title="click to collapse or expand..."> more... </a>
 <div id="label335" style="display:none">
 <table border="1">
 <tr>
 <td></td>
 <td colspan="1">Supported Version Ranges</td>
 </tr>
 <tr>
 <td>ptp_status</td>
 <td><code class="docutils literal notranslate">v7.4.1 -> 7.4.4 </code></td>
 </tr>
 <tr>
 <td>[disable]</td>
 <td><code class="docutils literal notranslate">v7.4.1 -> 7.4.4</code></td>
 <tr>
 <td>[enable]</td>
 <td><code class="docutils literal notranslate">v7.4.1 -> 7.4.4</code></td>
 </table>
 </div>
 </li>
            <li> <span class="li-head">qos_policy</span> - Switch controller QoS policy from available options. Source switch-controller.qos.qos-policy.name. <span class="li-normal">type: str</span>
 <a id='label336' href="javascript:ContentClick('label337', 'label336');" onmouseover="ContentPreview('label337');" onmouseout="ContentUnpreview('label337');" title="click to collapse or expand..."> more... </a>
 <div id="label337" style="display:none">
 <table border="1">
 <tr>
 <td></td>
 <td colspan="1">Supported Version Ranges</td>
 </tr>
 <tr>
 <td>qos_policy</td>
 <td><code class="docutils literal notranslate">v6.0.0 -> 7.4.4 </code></td>
 </tr>
 </table>
 </div>
 </li>
            <li> <span class="li-head">rpvst_port</span> - Enable/disable inter-operability with rapid PVST on this interface. <span class="li-normal">type: str</span> <span class="li-normal">choices: disabled, enabled</span>
 <a id='label338' href="javascript:ContentClick('label339', 'label338');" onmouseover="ContentPreview('label339');" onmouseout="ContentUnpreview('label339');" title="click to collapse or expand..."> more... </a>
 <div id="label339" style="display:none">
 <table border="1">
 <tr>
 <td></td>
 <td colspan="2">Supported Version Ranges</td>
 </tr>
 <tr>
 <td>rpvst_port</td>
 <td><code class="docutils literal notranslate">v6.4.0 -> v6.4.0 </code></td>
 <td><code class="docutils literal notranslate">v6.4.4 -> 7.4.4 </code></td>
 </tr>
 <tr>
 <td>[disabled]</td>
 <td><code class="docutils literal notranslate">v6.4.0 -> v6.4.0</code></td>
 <tr>
 <td>[enabled]</td>
 <td><code class="docutils literal notranslate">v6.4.0 -> v6.4.0</code></td>
 </table>
 </div>
 </li>
            <li> <span class="li-head">sample_direction</span> - Packet sampling direction. <span class="li-normal">type: str</span> <span class="li-normal">choices: tx, rx, both</span>
 <a id='label340' href="javascript:ContentClick('label341', 'label340');" onmouseover="ContentPreview('label341');" onmouseout="ContentUnpreview('label341');" title="click to collapse or expand..."> more... </a>
 <div id="label341" style="display:none">
 <table border="1">
 <tr>
 <td></td>
 <td colspan="1">Supported Version Ranges</td>
 </tr>
 <tr>
 <td>sample_direction</td>
 <td><code class="docutils literal notranslate">v6.0.0 -> 7.4.4 </code></td>
 </tr>
 <tr>
 <td>[tx]</td>
 <td><code class="docutils literal notranslate">v6.0.0 -> 7.4.4</code></td>
 <tr>
 <td>[rx]</td>
 <td><code class="docutils literal notranslate">v6.0.0 -> 7.4.4</code></td>
 <tr>
 <td>[both]</td>
 <td><code class="docutils literal notranslate">v6.0.0 -> 7.4.4</code></td>
 </table>
 </div>
 </li>
            <li> <span class="li-head">sflow_counter_interval</span> - sFlow sampling counter polling interval in seconds (0 - 255). <span class="li-normal">type: int</span>
 <a id='label342' href="javascript:ContentClick('label343', 'label342');" onmouseover="ContentPreview('label343');" onmouseout="ContentUnpreview('label343');" title="click to collapse or expand..."> more... </a>
 <div id="label343" style="display:none">
 <table border="1">
 <tr>
 <td></td>
 <td colspan="1">Supported Version Ranges</td>
 </tr>
 <tr>
 <td>sflow_counter_interval</td>
 <td><code class="docutils literal notranslate">v6.0.0 -> 7.4.4 </code></td>
 </tr>
 </table>
 </div>
 </li>
            <li> <span class="li-head">sflow_sample_rate</span> - sFlow sampler sample rate (0 - 99999 p/sec). <span class="li-normal">type: int</span>
 <a id='label344' href="javascript:ContentClick('label345', 'label344');" onmouseover="ContentPreview('label345');" onmouseout="ContentUnpreview('label345');" title="click to collapse or expand..."> more... </a>
 <div id="label345" style="display:none">
 <table border="1">
 <tr>
 <td></td>
 <td colspan="1">Supported Version Ranges</td>
 </tr>
 <tr>
 <td>sflow_sample_rate</td>
 <td><code class="docutils literal notranslate">v6.0.0 -> v6.0.11 </code></td>
 </tr>
 </table>
 </div>
 </li>
            <li> <span class="li-head">sflow_sampler</span> - Enable/disable sFlow protocol on this interface. <span class="li-normal">type: str</span> <span class="li-normal">choices: enabled, disabled</span>
 <a id='label346' href="javascript:ContentClick('label347', 'label346');" onmouseover="ContentPreview('label347');" onmouseout="ContentUnpreview('label347');" title="click to collapse or expand..."> more... </a>
 <div id="label347" style="display:none">
 <table border="1">
 <tr>
 <td></td>
 <td colspan="1">Supported Version Ranges</td>
 </tr>
 <tr>
 <td>sflow_sampler</td>
 <td><code class="docutils literal notranslate">v6.0.0 -> v6.0.11 </code></td>
 </tr>
 <tr>
 <td>[enabled]</td>
 <td><code class="docutils literal notranslate">v6.0.0 -> v6.0.11</code></td>
 <tr>
 <td>[disabled]</td>
 <td><code class="docutils literal notranslate">v6.0.0 -> v6.0.11</code></td>
 </table>
 </div>
 </li>
            <li> <span class="li-head">speed</span> - Switch port speed; default and available settings depend on hardware. <span class="li-normal">type: str</span> <span class="li-normal">choices: 10half, 10full, 100half, 100full, 1000full, 10000full, auto, 1000auto, 1000full-fiber, 40000full, auto-module, 100FX-half, 100FX-full, 100000full, 2500auto, 2500full, 25000full, 50000full, 10000cr, 10000sr, 100000sr4, 100000cr4, 40000sr4, 40000cr4, 40000auto, 25000cr, 25000sr, 50000cr, 50000sr, 5000auto, 1000fiber, 10000, 40000, 25000cr4, 25000sr4, 5000full</span>
 <a id='label348' href="javascript:ContentClick('label349', 'label348');" onmouseover="ContentPreview('label349');" onmouseout="ContentUnpreview('label349');" title="click to collapse or expand..."> more... </a>
 <div id="label349" style="display:none">
 <table border="1">
 <tr>
 <td></td>
 <td colspan="1">Supported Version Ranges</td>
 </tr>
 <tr>
 <td>speed</td>
 <td><code class="docutils literal notranslate">v6.0.0 -> 7.4.4 </code></td>
 </tr>
 <tr>
 <td>[10half]</td>
 <td><code class="docutils literal notranslate">v6.0.0 -> 7.4.4</code></td>
 <tr>
 <td>[10full]</td>
 <td><code class="docutils literal notranslate">v6.0.0 -> 7.4.4</code></td>
 <tr>
 <td>[100half]</td>
 <td><code class="docutils literal notranslate">v6.0.0 -> 7.4.4</code></td>
 <tr>
 <td>[100full]</td>
 <td><code class="docutils literal notranslate">v6.0.0 -> 7.4.4</code></td>
 <tr>
 <td>[1000full]</td>
 <td><code class="docutils literal notranslate">v6.0.0 -> 7.4.4</code></td>
 <tr>
 <td>[10000full]</td>
 <td><code class="docutils literal notranslate">v7.0.8 -> v7.0.12</code></td>
 <td><code class="docutils literal notranslate">v7.2.4 -> 7.4.4</code></td>
 </tr>
 <tr>
 <td>[auto]</td>
 <td><code class="docutils literal notranslate">v6.0.0 -> 7.4.4</code></td>
 <tr>
 <td>[1000auto]</td>
 <td><code class="docutils literal notranslate">v6.0.0 -> 7.4.4</code></td>
 <tr>
 <td>[1000full-fiber]</td>
 <td><code class="docutils literal notranslate">v7.0.8 -> v7.0.12</code></td>
 <td><code class="docutils literal notranslate">v7.2.4 -> 7.4.4</code></td>
 </tr>
 <tr>
 <td>[40000full]</td>
 <td><code class="docutils literal notranslate">v7.0.8 -> v7.0.12</code></td>
 <td><code class="docutils literal notranslate">v7.2.4 -> 7.4.4</code></td>
 </tr>
 <tr>
 <td>[auto-module]</td>
 <td><code class="docutils literal notranslate">v6.0.0 -> 7.4.4</code></td>
 <tr>
 <td>[100FX-half]</td>
 <td><code class="docutils literal notranslate">v6.0.0 -> 7.4.4</code></td>
 <tr>
 <td>[100FX-full]</td>
 <td><code class="docutils literal notranslate">v6.0.0 -> 7.4.4</code></td>
 <tr>
 <td>[100000full]</td>
 <td><code class="docutils literal notranslate">v6.0.0 -> 7.4.4</code></td>
 <tr>
 <td>[2500auto]</td>
 <td><code class="docutils literal notranslate">v6.2.0 -> v6.2.0</code></td>
 <td><code class="docutils literal notranslate">v6.2.5 -> 7.4.4</code></td>
 </tr>
 <tr>
 <td>[2500full]</td>
 <td><code class="docutils literal notranslate">v6.0.0 -> v6.0.11</code></td>
 <td><code class="docutils literal notranslate">v6.2.3 -> v6.2.3</code></td>
 <td><code class="docutils literal notranslate">v7.4.4 -> 7.4.4</code></td>
 </tr>
 <tr>
 <td>[25000full]</td>
 <td><code class="docutils literal notranslate">v6.0.0 -> 7.4.4</code></td>
 <tr>
 <td>[50000full]</td>
 <td><code class="docutils literal notranslate">v6.0.0 -> 7.4.4</code></td>
 <tr>
 <td>[10000cr]</td>
 <td><code class="docutils literal notranslate">v6.0.0 -> v6.0.0</code></td>
 <td><code class="docutils literal notranslate">v6.0.11 -> 7.4.4</code></td>
 </tr>
 <tr>
 <td>[10000sr]</td>
 <td><code class="docutils literal notranslate">v6.0.0 -> v6.0.0</code></td>
 <td><code class="docutils literal notranslate">v6.0.11 -> 7.4.4</code></td>
 </tr>
 <tr>
 <td>[100000sr4]</td>
 <td><code class="docutils literal notranslate">v6.0.0 -> v6.0.0</code></td>
 <td><code class="docutils literal notranslate">v6.0.11 -> 7.4.4</code></td>
 </tr>
 <tr>
 <td>[100000cr4]</td>
 <td><code class="docutils literal notranslate">v6.0.0 -> v6.0.0</code></td>
 <td><code class="docutils literal notranslate">v6.0.11 -> 7.4.4</code></td>
 </tr>
 <tr>
 <td>[40000sr4]</td>
 <td><code class="docutils literal notranslate">v7.0.8 -> v7.0.12</code></td>
 <td><code class="docutils literal notranslate">v7.2.4 -> 7.4.4</code></td>
 </tr>
 <tr>
 <td>[40000cr4]</td>
 <td><code class="docutils literal notranslate">v7.0.8 -> v7.0.12</code></td>
 <td><code class="docutils literal notranslate">v7.2.4 -> 7.4.4</code></td>
 </tr>
 <tr>
 <td>[40000auto]</td>
 <td><code class="docutils literal notranslate">v7.4.4 -> 7.4.4</code></td>
 </tr>
 <tr>
 <td>[25000cr]</td>
 <td><code class="docutils literal notranslate">v7.0.8 -> v7.0.12</code></td>
 <td><code class="docutils literal notranslate">v7.2.4 -> 7.4.4</code></td>
 </tr>
 <tr>
 <td>[25000sr]</td>
 <td><code class="docutils literal notranslate">v7.0.8 -> v7.0.12</code></td>
 <td><code class="docutils literal notranslate">v7.2.4 -> 7.4.4</code></td>
 </tr>
 <tr>
 <td>[50000cr]</td>
 <td><code class="docutils literal notranslate">v7.0.8 -> v7.0.12</code></td>
 <td><code class="docutils literal notranslate">v7.2.4 -> 7.4.4</code></td>
 </tr>
 <tr>
 <td>[50000sr]</td>
 <td><code class="docutils literal notranslate">v7.0.8 -> v7.0.12</code></td>
 <td><code class="docutils literal notranslate">v7.2.4 -> 7.4.4</code></td>
 </tr>
 <tr>
 <td>[5000auto]</td>
 <td><code class="docutils literal notranslate">v7.0.8 -> v7.0.12</code></td>
 <td><code class="docutils literal notranslate">v7.2.4 -> 7.4.4</code></td>
 </tr>
 <tr>
 <td>[1000fiber]</td>
 <td><code class="docutils literal notranslate">v6.0.0 -> v7.0.7</code></td>
 <td><code class="docutils literal notranslate">v7.2.0 -> v7.2.2</code></td>
 </tr>
 <tr>
 <td>[10000]</td>
 <td><code class="docutils literal notranslate">v6.0.0 -> v7.0.7</code></td>
 <td><code class="docutils literal notranslate">v7.2.0 -> v7.2.2</code></td>
 </tr>
 <tr>
 <td>[40000]</td>
 <td><code class="docutils literal notranslate">v6.0.0 -> v7.0.7</code></td>
 <td><code class="docutils literal notranslate">v7.2.0 -> v7.2.2</code></td>
 </tr>
 <tr>
 <td>[25000cr4]</td>
 <td><code class="docutils literal notranslate">v6.0.0 -> v6.0.0</code></td>
 <td><code class="docutils literal notranslate">v6.0.11 -> v7.0.7</code></td>
 <td><code class="docutils literal notranslate">v7.2.0 -> v7.2.2</code></td>
 </tr>
 <tr>
 <td>[25000sr4]</td>
 <td><code class="docutils literal notranslate">v6.0.0 -> v6.0.0</code></td>
 <td><code class="docutils literal notranslate">v6.0.11 -> v7.0.7</code></td>
 <td><code class="docutils literal notranslate">v7.2.0 -> v7.2.2</code></td>
 </tr>
 <tr>
 <td>[5000full]</td>
 <td><code class="docutils literal notranslate">v6.0.0 -> v6.0.0</code></td>
 <td><code class="docutils literal notranslate">v6.0.11 -> v7.0.7</code></td>
 <td><code class="docutils literal notranslate">v7.2.0 -> v7.2.2</code></td>
 </tr>
 </table>
 </div>
 </li>
            <li> <span class="li-head">speed_mask</span> - Switch port speed mask. <span class="li-normal">type: int</span>
 <a id='label350' href="javascript:ContentClick('label351', 'label350');" onmouseover="ContentPreview('label351');" onmouseout="ContentUnpreview('label351');" title="click to collapse or expand..."> more... </a>
 <div id="label351" style="display:none">
 <table border="1">
 <tr>
 <td></td>
 <td colspan="2">Supported Version Ranges</td>
 </tr>
 <tr>
 <td>speed_mask</td>
 <td><code class="docutils literal notranslate">v6.0.0 -> v6.0.11 </code></td>
 <td><code class="docutils literal notranslate">v6.2.3 -> v6.2.3 </code></td>
 </tr>
 </table>
 </div>
 </li>
            <li> <span class="li-head">stacking_port</span> - Stacking port. <span class="li-normal">type: int</span>
 <a id='label352' href="javascript:ContentClick('label353', 'label352');" onmouseover="ContentPreview('label353');" onmouseout="ContentUnpreview('label353');" title="click to collapse or expand..."> more... </a>
 <div id="label353" style="display:none">
 <table border="1">
 <tr>
 <td></td>
 <td colspan="2">Supported Version Ranges</td>
 </tr>
 <tr>
 <td>stacking_port</td>
 <td><code class="docutils literal notranslate">v6.0.0 -> v7.0.5 </code></td>
 <td><code class="docutils literal notranslate">v7.2.0 -> v7.2.0 </code></td>
 </tr>
 </table>
 </div>
 </li>
            <li> <span class="li-head">status</span> - Switch port admin status: up or down. <span class="li-normal">type: str</span> <span class="li-normal">choices: up, down</span>
 <a id='label354' href="javascript:ContentClick('label355', 'label354');" onmouseover="ContentPreview('label355');" onmouseout="ContentUnpreview('label355');" title="click to collapse or expand..."> more... </a>
 <div id="label355" style="display:none">
 <table border="1">
 <tr>
 <td></td>
 <td colspan="1">Supported Version Ranges</td>
 </tr>
 <tr>
 <td>status</td>
 <td><code class="docutils literal notranslate">v6.0.0 -> 7.4.4 </code></td>
 </tr>
 <tr>
 <td>[up]</td>
 <td><code class="docutils literal notranslate">v6.0.0 -> 7.4.4</code></td>
 <tr>
 <td>[down]</td>
 <td><code class="docutils literal notranslate">v6.0.0 -> 7.4.4</code></td>
 </table>
 </div>
 </li>
            <li> <span class="li-head">sticky_mac</span> - Enable or disable sticky-mac on the interface. <span class="li-normal">type: str</span> <span class="li-normal">choices: enable, disable</span>
 <a id='label356' href="javascript:ContentClick('label357', 'label356');" onmouseover="ContentPreview('label357');" onmouseout="ContentUnpreview('label357');" title="click to collapse or expand..."> more... </a>
 <div id="label357" style="display:none">
 <table border="1">
 <tr>
 <td></td>
 <td colspan="1">Supported Version Ranges</td>
 </tr>
 <tr>
 <td>sticky_mac</td>
 <td><code class="docutils literal notranslate">v6.2.0 -> 7.4.4 </code></td>
 </tr>
 <tr>
 <td>[enable]</td>
 <td><code class="docutils literal notranslate">v6.2.0 -> 7.4.4</code></td>
 <tr>
 <td>[disable]</td>
 <td><code class="docutils literal notranslate">v6.2.0 -> 7.4.4</code></td>
 </table>
 </div>
 </li>
            <li> <span class="li-head">storm_control_policy</span> - Switch controller storm control policy from available options. Source switch-controller.storm-control-policy.name. <span class="li-normal">type: str</span>
 <a id='label358' href="javascript:ContentClick('label359', 'label358');" onmouseover="ContentPreview('label359');" onmouseout="ContentUnpreview('label359');" title="click to collapse or expand..."> more... </a>
 <div id="label359" style="display:none">
 <table border="1">
 <tr>
 <td></td>
 <td colspan="1">Supported Version Ranges</td>
 </tr>
 <tr>
 <td>storm_control_policy</td>
 <td><code class="docutils literal notranslate">v6.2.0 -> 7.4.4 </code></td>
 </tr>
 </table>
 </div>
 </li>
            <li> <span class="li-head">stp_bpdu_guard</span> - Enable/disable STP BPDU guard on this interface. <span class="li-normal">type: str</span> <span class="li-normal">choices: enabled, disabled</span>
 <a id='label360' href="javascript:ContentClick('label361', 'label360');" onmouseover="ContentPreview('label361');" onmouseout="ContentUnpreview('label361');" title="click to collapse or expand..."> more... </a>
 <div id="label361" style="display:none">
 <table border="1">
 <tr>
 <td></td>
 <td colspan="1">Supported Version Ranges</td>
 </tr>
 <tr>
 <td>stp_bpdu_guard</td>
 <td><code class="docutils literal notranslate">v6.0.0 -> 7.4.4 </code></td>
 </tr>
 <tr>
 <td>[enabled]</td>
 <td><code class="docutils literal notranslate">v6.0.0 -> 7.4.4</code></td>
 <tr>
 <td>[disabled]</td>
 <td><code class="docutils literal notranslate">v6.0.0 -> 7.4.4</code></td>
 </table>
 </div>
 </li>
            <li> <span class="li-head">stp_bpdu_guard_timeout</span> - BPDU Guard disabling protection (0 - 120 min). <span class="li-normal">type: int</span>
 <a id='label362' href="javascript:ContentClick('label363', 'label362');" onmouseover="ContentPreview('label363');" onmouseout="ContentUnpreview('label363');" title="click to collapse or expand..."> more... </a>
 <div id="label363" style="display:none">
 <table border="1">
 <tr>
 <td></td>
 <td colspan="1">Supported Version Ranges</td>
 </tr>
 <tr>
 <td>stp_bpdu_guard_timeout</td>
 <td><code class="docutils literal notranslate">v6.0.0 -> 7.4.4 </code></td>
 </tr>
 </table>
 </div>
 </li>
            <li> <span class="li-head">stp_root_guard</span> - Enable/disable STP root guard on this interface. <span class="li-normal">type: str</span> <span class="li-normal">choices: enabled, disabled</span>
 <a id='label364' href="javascript:ContentClick('label365', 'label364');" onmouseover="ContentPreview('label365');" onmouseout="ContentUnpreview('label365');" title="click to collapse or expand..."> more... </a>
 <div id="label365" style="display:none">
 <table border="1">
 <tr>
 <td></td>
 <td colspan="1">Supported Version Ranges</td>
 </tr>
 <tr>
 <td>stp_root_guard</td>
 <td><code class="docutils literal notranslate">v6.0.0 -> 7.4.4 </code></td>
 </tr>
 <tr>
 <td>[enabled]</td>
 <td><code class="docutils literal notranslate">v6.0.0 -> 7.4.4</code></td>
 <tr>
 <td>[disabled]</td>
 <td><code class="docutils literal notranslate">v6.0.0 -> 7.4.4</code></td>
 </table>
 </div>
 </li>
            <li> <span class="li-head">stp_state</span> - Enable/disable Spanning Tree Protocol (STP) on this interface. <span class="li-normal">type: str</span> <span class="li-normal">choices: enabled, disabled</span>
 <a id='label366' href="javascript:ContentClick('label367', 'label366');" onmouseover="ContentPreview('label367');" onmouseout="ContentUnpreview('label367');" title="click to collapse or expand..."> more... </a>
 <div id="label367" style="display:none">
 <table border="1">
 <tr>
 <td></td>
 <td colspan="1">Supported Version Ranges</td>
 </tr>
 <tr>
 <td>stp_state</td>
 <td><code class="docutils literal notranslate">v6.0.0 -> 7.4.4 </code></td>
 </tr>
 <tr>
 <td>[enabled]</td>
 <td><code class="docutils literal notranslate">v6.0.0 -> 7.4.4</code></td>
 <tr>
 <td>[disabled]</td>
 <td><code class="docutils literal notranslate">v6.0.0 -> 7.4.4</code></td>
 </table>
 </div>
 </li>
            <li> <span class="li-head">switch_id</span> - Switch id. <span class="li-normal">type: str</span>
 <a id='label368' href="javascript:ContentClick('label369', 'label368');" onmouseover="ContentPreview('label369');" onmouseout="ContentUnpreview('label369');" title="click to collapse or expand..."> more... </a>
 <div id="label369" style="display:none">
 <table border="1">
 <tr>
 <td></td>
 <td colspan="2">Supported Version Ranges</td>
 </tr>
 <tr>
 <td>switch_id</td>
 <td><code class="docutils literal notranslate">v6.0.0 -> v7.0.5 </code></td>
 <td><code class="docutils literal notranslate">v7.2.0 -> v7.2.0 </code></td>
 </tr>
 </table>
 </div>
 </li>
            <li> <span class="li-head">type</span> - Interface type: physical or trunk port. <span class="li-normal">type: str</span> <span class="li-normal">choices: physical, trunk</span>
 <a id='label370' href="javascript:ContentClick('label371', 'label370');" onmouseover="ContentPreview('label371');" onmouseout="ContentUnpreview('label371');" title="click to collapse or expand..."> more... </a>
 <div id="label371" style="display:none">
 <table border="1">
 <tr>
 <td></td>
 <td colspan="1">Supported Version Ranges</td>
 </tr>
 <tr>
 <td>type</td>
 <td><code class="docutils literal notranslate">v6.0.0 -> 7.4.4 </code></td>
 </tr>
 <tr>
 <td>[physical]</td>
 <td><code class="docutils literal notranslate">v6.0.0 -> 7.4.4</code></td>
 <tr>
 <td>[trunk]</td>
 <td><code class="docutils literal notranslate">v6.0.0 -> 7.4.4</code></td>
 </table>
 </div>
 </li>
            <li> <span class="li-head">untagged_vlans</span> - Configure switch port untagged VLANs. <span class="li-normal">type: list</span> <span style="font-family:'Courier New'" class="li-required">member_path: ports:port_name/untagged_vlans:vlan_name</span>
 <a id='label372' href="javascript:ContentClick('label373', 'label372');" onmouseover="ContentPreview('label373');" onmouseout="ContentUnpreview('label373');" title="click to collapse or expand..."> more... </a>
 <div id="label373" style="display:none">
 <table border="1">
 <tr>
 <td></td><td colspan="1">Supported Version Ranges</td>
 </tr>
 <tr>
 <td>untagged_vlans</td>
 <td><code class="docutils literal notranslate">v6.0.0 -> 7.4.4 </code></td>
 </tr>
 </table>
 </div>
 </li>
                <ul class="ul-self">
                <li> <span class="li-head">vlan_name</span> - VLAN name. Source system.interface.name. <span class="li-normal">type: str</span> <span class="li-required">required: true</span>
 <a id='label374' href="javascript:ContentClick('label375', 'label374');" onmouseover="ContentPreview('label375');" onmouseout="ContentUnpreview('label375');" title="click to collapse or expand..."> more... </a>
 <div id="label375" style="display:none">
 <table border="1">
 <tr>
 <td></td>
 <td colspan="1">Supported Version Ranges</td>
 </tr>
 <tr>
 <td>vlan_name</td>
 <td><code class="docutils literal notranslate">v6.0.0 -> 7.4.4 </code></td>
 </tr>
 </table>
 </div>
 </li>
                </ul>
            <li> <span class="li-head">virtual_port</span> - Virtualized switch port. <span class="li-normal">type: int</span>
 <a id='label376' href="javascript:ContentClick('label377', 'label376');" onmouseover="ContentPreview('label377');" onmouseout="ContentUnpreview('label377');" title="click to collapse or expand..."> more... </a>
 <div id="label377" style="display:none">
 <table border="1">
 <tr>
 <td></td>
 <td colspan="2">Supported Version Ranges</td>
 </tr>
 <tr>
 <td>virtual_port</td>
 <td><code class="docutils literal notranslate">v6.0.0 -> v6.0.11 </code></td>
 <td><code class="docutils literal notranslate">v6.2.3 -> v6.2.3 </code></td>
 </tr>
 </table>
 </div>
 </li>
            <li> <span class="li-head">vlan</span> - Assign switch ports to a VLAN. Source system.interface.name. <span class="li-normal">type: str</span>
 <a id='label378' href="javascript:ContentClick('label379', 'label378');" onmouseover="ContentPreview('label379');" onmouseout="ContentUnpreview('label379');" title="click to collapse or expand..."> more... </a>
 <div id="label379" style="display:none">
 <table border="1">
 <tr>
 <td></td>
 <td colspan="1">Supported Version Ranges</td>
 </tr>
 <tr>
 <td>vlan</td>
 <td><code class="docutils literal notranslate">v6.0.0 -> 7.4.4 </code></td>
 </tr>
 </table>
 </div>
 </li>
            </ul>
        <li> <span class="li-head">pre_provisioned</span> - Pre-provisioned managed switch. <span class="li-normal">type: int</span>
 <a id='label380' href="javascript:ContentClick('label381', 'label380');" onmouseover="ContentPreview('label381');" onmouseout="ContentUnpreview('label381');" title="click to collapse or expand..."> more... </a>
 <div id="label381" style="display:none">
 <table border="1">
 <tr>
 <td></td>
 <td colspan="1">Supported Version Ranges</td>
 </tr>
 <tr>
 <td>pre_provisioned</td>
 <td><code class="docutils literal notranslate">v6.0.0 -> 7.4.4 </code></td>
 </tr>
 </table>
 </div>
 </li>
        <li> <span class="li-head">ptp_profile</span> - PTP profile configuration. Source switch-controller.ptp.profile.name. <span class="li-normal">type: str</span>
 <a id='label382' href="javascript:ContentClick('label383', 'label382');" onmouseover="ContentPreview('label383');" onmouseout="ContentUnpreview('label383');" title="click to collapse or expand..."> more... </a>
 <div id="label383" style="display:none">
 <table border="1">
 <tr>
 <td></td>
 <td colspan="1">Supported Version Ranges</td>
 </tr>
 <tr>
 <td>ptp_profile</td>
 <td><code class="docutils literal notranslate">v7.4.1 -> 7.4.4 </code></td>
 </tr>
 </table>
 </div>
 </li>
        <li> <span class="li-head">ptp_status</span> - Enable/disable PTP profile on this FortiSwitch. <span class="li-normal">type: str</span> <span class="li-normal">choices: disable, enable</span>
 <a id='label384' href="javascript:ContentClick('label385', 'label384');" onmouseover="ContentPreview('label385');" onmouseout="ContentUnpreview('label385');" title="click to collapse or expand..."> more... </a>
 <div id="label385" style="display:none">
 <table border="1">
 <tr>
 <td></td>
 <td colspan="1">Supported Version Ranges</td>
 </tr>
 <tr>
 <td>ptp_status</td>
 <td><code class="docutils literal notranslate">v7.4.1 -> 7.4.4 </code></td>
 </tr>
 <tr>
 <td>[disable]</td>
 <td><code class="docutils literal notranslate">v7.4.1 -> 7.4.4</code></td>
 <tr>
 <td>[enable]</td>
 <td><code class="docutils literal notranslate">v7.4.1 -> 7.4.4</code></td>
 </table>
 </div>
 </li>
        <li> <span class="li-head">purdue_level</span> - Purdue Level of this FortiSwitch. <span class="li-normal">type: str</span> <span class="li-normal">choices: 1, 1.5, 2, 2.5, 3, 3.5, 4, 5, 5.5</span>
 <a id='label386' href="javascript:ContentClick('label387', 'label386');" onmouseover="ContentPreview('label387');" onmouseout="ContentUnpreview('label387');" title="click to collapse or expand..."> more... </a>
 <div id="label387" style="display:none">
 <table border="1">
 <tr>
 <td></td>
 <td colspan="1">Supported Version Ranges</td>
 </tr>
 <tr>
 <td>purdue_level</td>
 <td><code class="docutils literal notranslate">v7.4.2 -> 7.4.4 </code></td>
 </tr>
 <tr>
 <td>[1]</td>
 <td><code class="docutils literal notranslate">v7.4.2 -> 7.4.4</code></td>
 <tr>
 <td>[1.5]</td>
 <td><code class="docutils literal notranslate">v7.4.2 -> 7.4.4</code></td>
 <tr>
 <td>[2]</td>
 <td><code class="docutils literal notranslate">v7.4.2 -> 7.4.4</code></td>
 <tr>
 <td>[2.5]</td>
 <td><code class="docutils literal notranslate">v7.4.2 -> 7.4.4</code></td>
 <tr>
 <td>[3]</td>
 <td><code class="docutils literal notranslate">v7.4.2 -> 7.4.4</code></td>
 <tr>
 <td>[3.5]</td>
 <td><code class="docutils literal notranslate">v7.4.2 -> 7.4.4</code></td>
 <tr>
 <td>[4]</td>
 <td><code class="docutils literal notranslate">v7.4.2 -> 7.4.4</code></td>
 <tr>
 <td>[5]</td>
 <td><code class="docutils literal notranslate">v7.4.2 -> 7.4.4</code></td>
 <tr>
 <td>[5.5]</td>
 <td><code class="docutils literal notranslate">v7.4.2 -> 7.4.4</code></td>
 </table>
 </div>
 </li>
        <li> <span class="li-head">qos_drop_policy</span> - Set QoS drop-policy. <span class="li-normal">type: str</span> <span class="li-normal">choices: taildrop, random-early-detection</span>
 <a id='label388' href="javascript:ContentClick('label389', 'label388');" onmouseover="ContentPreview('label389');" onmouseout="ContentUnpreview('label389');" title="click to collapse or expand..."> more... </a>
 <div id="label389" style="display:none">
 <table border="1">
 <tr>
 <td></td>
 <td colspan="1">Supported Version Ranges</td>
 </tr>
 <tr>
 <td>qos_drop_policy</td>
 <td><code class="docutils literal notranslate">v6.4.0 -> 7.4.4 </code></td>
 </tr>
 <tr>
 <td>[taildrop]</td>
 <td><code class="docutils literal notranslate">v6.4.0 -> 7.4.4</code></td>
 <tr>
 <td>[random-early-detection]</td>
 <td><code class="docutils literal notranslate">v6.4.0 -> 7.4.4</code></td>
 </table>
 </div>
 </li>
        <li> <span class="li-head">qos_red_probability</span> - Set QoS RED/WRED drop probability. <span class="li-normal">type: int</span>
 <a id='label390' href="javascript:ContentClick('label391', 'label390');" onmouseover="ContentPreview('label391');" onmouseout="ContentUnpreview('label391');" title="click to collapse or expand..."> more... </a>
 <div id="label391" style="display:none">
 <table border="1">
 <tr>
 <td></td>
 <td colspan="1">Supported Version Ranges</td>
 </tr>
 <tr>
 <td>qos_red_probability</td>
 <td><code class="docutils literal notranslate">v6.4.0 -> 7.4.4 </code></td>
 </tr>
 </table>
 </div>
 </li>
        <li> <span class="li-head">radius_nas_ip</span> - NAS-IP address. <span class="li-normal">type: str</span>
 <a id='label392' href="javascript:ContentClick('label393', 'label392');" onmouseover="ContentPreview('label393');" onmouseout="ContentUnpreview('label393');" title="click to collapse or expand..."> more... </a>
 <div id="label393" style="display:none">
 <table border="1">
 <tr>
 <td></td>
 <td colspan="1">Supported Version Ranges</td>
 </tr>
 <tr>
 <td>radius_nas_ip</td>
 <td><code class="docutils literal notranslate">v7.4.2 -> 7.4.4 </code></td>
 </tr>
 </table>
 </div>
 </li>
        <li> <span class="li-head">radius_nas_ip_override</span> - Use locally defined NAS-IP. <span class="li-normal">type: str</span> <span class="li-normal">choices: disable, enable</span>
 <a id='label394' href="javascript:ContentClick('label395', 'label394');" onmouseover="ContentPreview('label395');" onmouseout="ContentUnpreview('label395');" title="click to collapse or expand..."> more... </a>
 <div id="label395" style="display:none">
 <table border="1">
 <tr>
 <td></td>
 <td colspan="1">Supported Version Ranges</td>
 </tr>
 <tr>
 <td>radius_nas_ip_override</td>
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
        <li> <span class="li-head">remote_log</span> - Configure logging by FortiSwitch device to a remote syslog server. <span class="li-normal">type: list</span> <span style="font-family:'Courier New'" class="li-required">member_path: remote_log:name</span>
 <a id='label396' href="javascript:ContentClick('label397', 'label396');" onmouseover="ContentPreview('label397');" onmouseout="ContentUnpreview('label397');" title="click to collapse or expand..."> more... </a>
 <div id="label397" style="display:none">
 <table border="1">
 <tr>
 <td></td><td colspan="1">Supported Version Ranges</td>
 </tr>
 <tr>
 <td>remote_log</td>
 <td><code class="docutils literal notranslate">v6.2.0 -> 7.4.4 </code></td>
 </tr>
 </table>
 </div>
 </li>
            <ul class="ul-self">
            <li> <span class="li-head">csv</span> - Enable/disable comma-separated value (CSV) strings. <span class="li-normal">type: str</span> <span class="li-normal">choices: enable, disable</span>
 <a id='label398' href="javascript:ContentClick('label399', 'label398');" onmouseover="ContentPreview('label399');" onmouseout="ContentUnpreview('label399');" title="click to collapse or expand..."> more... </a>
 <div id="label399" style="display:none">
 <table border="1">
 <tr>
 <td></td>
 <td colspan="1">Supported Version Ranges</td>
 </tr>
 <tr>
 <td>csv</td>
 <td><code class="docutils literal notranslate">v6.2.0 -> 7.4.4 </code></td>
 </tr>
 <tr>
 <td>[enable]</td>
 <td><code class="docutils literal notranslate">v6.2.0 -> 7.4.4</code></td>
 <tr>
 <td>[disable]</td>
 <td><code class="docutils literal notranslate">v6.2.0 -> 7.4.4</code></td>
 </table>
 </div>
 </li>
            <li> <span class="li-head">facility</span> - Facility to log to remote syslog server. <span class="li-normal">type: str</span> <span class="li-normal">choices: kernel, user, mail, daemon, auth, syslog, lpr, news, uucp, cron, authpriv, ftp, ntp, audit, alert, clock, local0, local1, local2, local3, local4, local5, local6, local7</span>
 <a id='label400' href="javascript:ContentClick('label401', 'label400');" onmouseover="ContentPreview('label401');" onmouseout="ContentUnpreview('label401');" title="click to collapse or expand..."> more... </a>
 <div id="label401" style="display:none">
 <table border="1">
 <tr>
 <td></td>
 <td colspan="1">Supported Version Ranges</td>
 </tr>
 <tr>
 <td>facility</td>
 <td><code class="docutils literal notranslate">v6.2.0 -> 7.4.4 </code></td>
 </tr>
 <tr>
 <td>[kernel]</td>
 <td><code class="docutils literal notranslate">v6.2.0 -> 7.4.4</code></td>
 <tr>
 <td>[user]</td>
 <td><code class="docutils literal notranslate">v6.2.0 -> 7.4.4</code></td>
 <tr>
 <td>[mail]</td>
 <td><code class="docutils literal notranslate">v6.2.0 -> 7.4.4</code></td>
 <tr>
 <td>[daemon]</td>
 <td><code class="docutils literal notranslate">v6.2.0 -> 7.4.4</code></td>
 <tr>
 <td>[auth]</td>
 <td><code class="docutils literal notranslate">v6.2.0 -> 7.4.4</code></td>
 <tr>
 <td>[syslog]</td>
 <td><code class="docutils literal notranslate">v6.2.0 -> 7.4.4</code></td>
 <tr>
 <td>[lpr]</td>
 <td><code class="docutils literal notranslate">v6.2.0 -> 7.4.4</code></td>
 <tr>
 <td>[news]</td>
 <td><code class="docutils literal notranslate">v6.2.0 -> 7.4.4</code></td>
 <tr>
 <td>[uucp]</td>
 <td><code class="docutils literal notranslate">v6.2.0 -> 7.4.4</code></td>
 <tr>
 <td>[cron]</td>
 <td><code class="docutils literal notranslate">v6.2.0 -> 7.4.4</code></td>
 <tr>
 <td>[authpriv]</td>
 <td><code class="docutils literal notranslate">v6.2.0 -> 7.4.4</code></td>
 <tr>
 <td>[ftp]</td>
 <td><code class="docutils literal notranslate">v6.2.0 -> 7.4.4</code></td>
 <tr>
 <td>[ntp]</td>
 <td><code class="docutils literal notranslate">v6.2.0 -> 7.4.4</code></td>
 <tr>
 <td>[audit]</td>
 <td><code class="docutils literal notranslate">v6.2.0 -> 7.4.4</code></td>
 <tr>
 <td>[alert]</td>
 <td><code class="docutils literal notranslate">v6.2.0 -> 7.4.4</code></td>
 <tr>
 <td>[clock]</td>
 <td><code class="docutils literal notranslate">v6.2.0 -> 7.4.4</code></td>
 <tr>
 <td>[local0]</td>
 <td><code class="docutils literal notranslate">v6.2.0 -> 7.4.4</code></td>
 <tr>
 <td>[local1]</td>
 <td><code class="docutils literal notranslate">v6.2.0 -> 7.4.4</code></td>
 <tr>
 <td>[local2]</td>
 <td><code class="docutils literal notranslate">v6.2.0 -> 7.4.4</code></td>
 <tr>
 <td>[local3]</td>
 <td><code class="docutils literal notranslate">v6.2.0 -> 7.4.4</code></td>
 <tr>
 <td>[local4]</td>
 <td><code class="docutils literal notranslate">v6.2.0 -> 7.4.4</code></td>
 <tr>
 <td>[local5]</td>
 <td><code class="docutils literal notranslate">v6.2.0 -> 7.4.4</code></td>
 <tr>
 <td>[local6]</td>
 <td><code class="docutils literal notranslate">v6.2.0 -> 7.4.4</code></td>
 <tr>
 <td>[local7]</td>
 <td><code class="docutils literal notranslate">v6.2.0 -> 7.4.4</code></td>
 </table>
 </div>
 </li>
            <li> <span class="li-head">name</span> - Remote log name. <span class="li-normal">type: str</span> <span class="li-required">required: true</span>
 <a id='label402' href="javascript:ContentClick('label403', 'label402');" onmouseover="ContentPreview('label403');" onmouseout="ContentUnpreview('label403');" title="click to collapse or expand..."> more... </a>
 <div id="label403" style="display:none">
 <table border="1">
 <tr>
 <td></td>
 <td colspan="1">Supported Version Ranges</td>
 </tr>
 <tr>
 <td>name</td>
 <td><code class="docutils literal notranslate">v6.2.0 -> 7.4.4 </code></td>
 </tr>
 </table>
 </div>
 </li>
            <li> <span class="li-head">port</span> - Remote syslog server listening port. <span class="li-normal">type: int</span>
 <a id='label404' href="javascript:ContentClick('label405', 'label404');" onmouseover="ContentPreview('label405');" onmouseout="ContentUnpreview('label405');" title="click to collapse or expand..."> more... </a>
 <div id="label405" style="display:none">
 <table border="1">
 <tr>
 <td></td>
 <td colspan="1">Supported Version Ranges</td>
 </tr>
 <tr>
 <td>port</td>
 <td><code class="docutils literal notranslate">v6.2.0 -> 7.4.4 </code></td>
 </tr>
 </table>
 </div>
 </li>
            <li> <span class="li-head">server</span> - IPv4 address of the remote syslog server. <span class="li-normal">type: str</span>
 <a id='label406' href="javascript:ContentClick('label407', 'label406');" onmouseover="ContentPreview('label407');" onmouseout="ContentUnpreview('label407');" title="click to collapse or expand..."> more... </a>
 <div id="label407" style="display:none">
 <table border="1">
 <tr>
 <td></td>
 <td colspan="1">Supported Version Ranges</td>
 </tr>
 <tr>
 <td>server</td>
 <td><code class="docutils literal notranslate">v6.2.0 -> 7.4.4 </code></td>
 </tr>
 </table>
 </div>
 </li>
            <li> <span class="li-head">severity</span> - Severity of logs to be transferred to remote log server. <span class="li-normal">type: str</span> <span class="li-normal">choices: emergency, alert, critical, error, warning, notification, information, debug</span>
 <a id='label408' href="javascript:ContentClick('label409', 'label408');" onmouseover="ContentPreview('label409');" onmouseout="ContentUnpreview('label409');" title="click to collapse or expand..."> more... </a>
 <div id="label409" style="display:none">
 <table border="1">
 <tr>
 <td></td>
 <td colspan="1">Supported Version Ranges</td>
 </tr>
 <tr>
 <td>severity</td>
 <td><code class="docutils literal notranslate">v6.2.0 -> 7.4.4 </code></td>
 </tr>
 <tr>
 <td>[emergency]</td>
 <td><code class="docutils literal notranslate">v6.2.0 -> 7.4.4</code></td>
 <tr>
 <td>[alert]</td>
 <td><code class="docutils literal notranslate">v6.2.0 -> 7.4.4</code></td>
 <tr>
 <td>[critical]</td>
 <td><code class="docutils literal notranslate">v6.2.0 -> 7.4.4</code></td>
 <tr>
 <td>[error]</td>
 <td><code class="docutils literal notranslate">v6.2.0 -> 7.4.4</code></td>
 <tr>
 <td>[warning]</td>
 <td><code class="docutils literal notranslate">v6.2.0 -> 7.4.4</code></td>
 <tr>
 <td>[notification]</td>
 <td><code class="docutils literal notranslate">v6.2.0 -> 7.4.4</code></td>
 <tr>
 <td>[information]</td>
 <td><code class="docutils literal notranslate">v6.2.0 -> 7.4.4</code></td>
 <tr>
 <td>[debug]</td>
 <td><code class="docutils literal notranslate">v6.2.0 -> 7.4.4</code></td>
 </table>
 </div>
 </li>
            <li> <span class="li-head">status</span> - Enable/disable logging by FortiSwitch device to a remote syslog server. <span class="li-normal">type: str</span> <span class="li-normal">choices: enable, disable</span>
 <a id='label410' href="javascript:ContentClick('label411', 'label410');" onmouseover="ContentPreview('label411');" onmouseout="ContentUnpreview('label411');" title="click to collapse or expand..."> more... </a>
 <div id="label411" style="display:none">
 <table border="1">
 <tr>
 <td></td>
 <td colspan="1">Supported Version Ranges</td>
 </tr>
 <tr>
 <td>status</td>
 <td><code class="docutils literal notranslate">v6.2.0 -> 7.4.4 </code></td>
 </tr>
 <tr>
 <td>[enable]</td>
 <td><code class="docutils literal notranslate">v6.2.0 -> 7.4.4</code></td>
 <tr>
 <td>[disable]</td>
 <td><code class="docutils literal notranslate">v6.2.0 -> 7.4.4</code></td>
 </table>
 </div>
 </li>
            </ul>
        <li> <span class="li-head">route_offload</span> - Enable/disable route offload on this FortiSwitch. <span class="li-normal">type: str</span> <span class="li-normal">choices: disable, enable</span>
 <a id='label412' href="javascript:ContentClick('label413', 'label412');" onmouseover="ContentPreview('label413');" onmouseout="ContentUnpreview('label413');" title="click to collapse or expand..."> more... </a>
 <div id="label413" style="display:none">
 <table border="1">
 <tr>
 <td></td>
 <td colspan="1">Supported Version Ranges</td>
 </tr>
 <tr>
 <td>route_offload</td>
 <td><code class="docutils literal notranslate">v7.4.1 -> 7.4.4 </code></td>
 </tr>
 <tr>
 <td>[disable]</td>
 <td><code class="docutils literal notranslate">v7.4.1 -> 7.4.4</code></td>
 <tr>
 <td>[enable]</td>
 <td><code class="docutils literal notranslate">v7.4.1 -> 7.4.4</code></td>
 </table>
 </div>
 </li>
        <li> <span class="li-head">route_offload_mclag</span> - Enable/disable route offload MCLAG on this FortiSwitch. <span class="li-normal">type: str</span> <span class="li-normal">choices: disable, enable</span>
 <a id='label414' href="javascript:ContentClick('label415', 'label414');" onmouseover="ContentPreview('label415');" onmouseout="ContentUnpreview('label415');" title="click to collapse or expand..."> more... </a>
 <div id="label415" style="display:none">
 <table border="1">
 <tr>
 <td></td>
 <td colspan="1">Supported Version Ranges</td>
 </tr>
 <tr>
 <td>route_offload_mclag</td>
 <td><code class="docutils literal notranslate">v7.4.1 -> 7.4.4 </code></td>
 </tr>
 <tr>
 <td>[disable]</td>
 <td><code class="docutils literal notranslate">v7.4.1 -> 7.4.4</code></td>
 <tr>
 <td>[enable]</td>
 <td><code class="docutils literal notranslate">v7.4.1 -> 7.4.4</code></td>
 </table>
 </div>
 </li>
        <li> <span class="li-head">route_offload_router</span> - Configure route offload MCLAG IP address. <span class="li-normal">type: list</span> <span style="font-family:'Courier New'" class="li-required">member_path: route_offload_router:vlan_name</span>
 <a id='label416' href="javascript:ContentClick('label417', 'label416');" onmouseover="ContentPreview('label417');" onmouseout="ContentUnpreview('label417');" title="click to collapse or expand..."> more... </a>
 <div id="label417" style="display:none">
 <table border="1">
 <tr>
 <td></td><td colspan="1">Supported Version Ranges</td>
 </tr>
 <tr>
 <td>route_offload_router</td>
 <td><code class="docutils literal notranslate">v7.4.1 -> 7.4.4 </code></td>
 </tr>
 </table>
 </div>
 </li>
            <ul class="ul-self">
            <li> <span class="li-head">router_ip</span> - Router IP address. <span class="li-normal">type: str</span>
 <a id='label418' href="javascript:ContentClick('label419', 'label418');" onmouseover="ContentPreview('label419');" onmouseout="ContentUnpreview('label419');" title="click to collapse or expand..."> more... </a>
 <div id="label419" style="display:none">
 <table border="1">
 <tr>
 <td></td>
 <td colspan="1">Supported Version Ranges</td>
 </tr>
 <tr>
 <td>router_ip</td>
 <td><code class="docutils literal notranslate">v7.4.1 -> 7.4.4 </code></td>
 </tr>
 </table>
 </div>
 </li>
            <li> <span class="li-head">vlan_name</span> - VLAN name. Source system.interface.name. <span class="li-normal">type: str</span> <span class="li-required">required: true</span>
 <a id='label420' href="javascript:ContentClick('label421', 'label420');" onmouseover="ContentPreview('label421');" onmouseout="ContentUnpreview('label421');" title="click to collapse or expand..."> more... </a>
 <div id="label421" style="display:none">
 <table border="1">
 <tr>
 <td></td>
 <td colspan="1">Supported Version Ranges</td>
 </tr>
 <tr>
 <td>vlan_name</td>
 <td><code class="docutils literal notranslate">v7.4.1 -> 7.4.4 </code></td>
 </tr>
 </table>
 </div>
 </li>
            </ul>
        <li> <span class="li-head">sn</span> - Managed-switch serial number. <span class="li-normal">type: str</span>
 <a id='label422' href="javascript:ContentClick('label423', 'label422');" onmouseover="ContentPreview('label423');" onmouseout="ContentUnpreview('label423');" title="click to collapse or expand..."> more... </a>
 <div id="label423" style="display:none">
 <table border="1">
 <tr>
 <td></td>
 <td colspan="1">Supported Version Ranges</td>
 </tr>
 <tr>
 <td>sn</td>
 <td><code class="docutils literal notranslate">v7.4.0 -> 7.4.4 </code></td>
 </tr>
 </table>
 </div>
 </li>
        <li> <span class="li-head">snmp_community</span> - Configuration method to edit Simple Network Management Protocol (SNMP) communities. <span class="li-normal">type: list</span> <span style="font-family:'Courier New'" class="li-required">member_path: snmp_community:id</span>
 <a id='label424' href="javascript:ContentClick('label425', 'label424');" onmouseover="ContentPreview('label425');" onmouseout="ContentUnpreview('label425');" title="click to collapse or expand..."> more... </a>
 <div id="label425" style="display:none">
 <table border="1">
 <tr>
 <td></td><td colspan="1">Supported Version Ranges</td>
 </tr>
 <tr>
 <td>snmp_community</td>
 <td><code class="docutils literal notranslate">v6.2.0 -> 7.4.4 </code></td>
 </tr>
 </table>
 </div>
 </li>
            <ul class="ul-self">
            <li> <span class="li-head">events</span> - SNMP notifications (traps) to send. <span class="li-normal">type: list</span> <span class="li-normal">choices: cpu-high, mem-low, log-full, intf-ip, ent-conf-change</span>
 <a id='label426' href="javascript:ContentClick('label427', 'label426');" onmouseover="ContentPreview('label427');" onmouseout="ContentUnpreview('label427');" title="click to collapse or expand..."> more... </a>
 <div id="label427" style="display:none">
 <table border="1">
 <tr>
 <td></td>
 <td colspan="1">Supported Version Ranges</td>
 </tr>
 <tr>
 <td>events</td>
 <td><code class="docutils literal notranslate">v6.2.0 -> 7.4.4 </code></td>
 </tr>
 <tr>
 <td>[cpu-high]</td>
 <td><code class="docutils literal notranslate">v6.2.0 -> 7.4.4</code></td>
 <tr>
 <td>[mem-low]</td>
 <td><code class="docutils literal notranslate">v6.2.0 -> 7.4.4</code></td>
 <tr>
 <td>[log-full]</td>
 <td><code class="docutils literal notranslate">v6.2.0 -> 7.4.4</code></td>
 <tr>
 <td>[intf-ip]</td>
 <td><code class="docutils literal notranslate">v6.2.0 -> 7.4.4</code></td>
 <tr>
 <td>[ent-conf-change]</td>
 <td><code class="docutils literal notranslate">v6.2.0 -> 7.4.4</code></td>
 </table>
 </div>
 </li>
            <li> <span class="li-head">hosts</span> - Configure IPv4 SNMP managers (hosts). <span class="li-normal">type: list</span> <span style="font-family:'Courier New'" class="li-required">member_path: snmp_community:id/hosts:id</span>
 <a id='label428' href="javascript:ContentClick('label429', 'label428');" onmouseover="ContentPreview('label429');" onmouseout="ContentUnpreview('label429');" title="click to collapse or expand..."> more... </a>
 <div id="label429" style="display:none">
 <table border="1">
 <tr>
 <td></td><td colspan="1">Supported Version Ranges</td>
 </tr>
 <tr>
 <td>hosts</td>
 <td><code class="docutils literal notranslate">v6.2.0 -> 7.4.4 </code></td>
 </tr>
 </table>
 </div>
 </li>
                <ul class="ul-self">
                <li> <span class="li-head">id</span> - Host entry ID. see <a href='#notes'>Notes</a>. <span class="li-normal">type: int</span> <span class="li-required">required: true</span>
 <a id='label430' href="javascript:ContentClick('label431', 'label430');" onmouseover="ContentPreview('label431');" onmouseout="ContentUnpreview('label431');" title="click to collapse or expand..."> more... </a>
 <div id="label431" style="display:none">
 <table border="1">
 <tr>
 <td></td>
 <td colspan="1">Supported Version Ranges</td>
 </tr>
 <tr>
 <td>id</td>
 <td><code class="docutils literal notranslate">v6.2.0 -> 7.4.4 </code></td>
 </tr>
 </table>
 </div>
 </li>
                <li> <span class="li-head">ip</span> - IPv4 address of the SNMP manager (host). <span class="li-normal">type: str</span>
 <a id='label432' href="javascript:ContentClick('label433', 'label432');" onmouseover="ContentPreview('label433');" onmouseout="ContentUnpreview('label433');" title="click to collapse or expand..."> more... </a>
 <div id="label433" style="display:none">
 <table border="1">
 <tr>
 <td></td>
 <td colspan="1">Supported Version Ranges</td>
 </tr>
 <tr>
 <td>ip</td>
 <td><code class="docutils literal notranslate">v6.2.0 -> 7.4.4 </code></td>
 </tr>
 </table>
 </div>
 </li>
                </ul>
            <li> <span class="li-head">id</span> - SNMP community ID. see <a href='#notes'>Notes</a>. <span class="li-normal">type: int</span> <span class="li-required">required: true</span>
 <a id='label434' href="javascript:ContentClick('label435', 'label434');" onmouseover="ContentPreview('label435');" onmouseout="ContentUnpreview('label435');" title="click to collapse or expand..."> more... </a>
 <div id="label435" style="display:none">
 <table border="1">
 <tr>
 <td></td>
 <td colspan="1">Supported Version Ranges</td>
 </tr>
 <tr>
 <td>id</td>
 <td><code class="docutils literal notranslate">v6.2.0 -> 7.4.4 </code></td>
 </tr>
 </table>
 </div>
 </li>
            <li> <span class="li-head">name</span> - SNMP community name. <span class="li-normal">type: str</span>
 <a id='label436' href="javascript:ContentClick('label437', 'label436');" onmouseover="ContentPreview('label437');" onmouseout="ContentUnpreview('label437');" title="click to collapse or expand..."> more... </a>
 <div id="label437" style="display:none">
 <table border="1">
 <tr>
 <td></td>
 <td colspan="1">Supported Version Ranges</td>
 </tr>
 <tr>
 <td>name</td>
 <td><code class="docutils literal notranslate">v6.2.0 -> 7.4.4 </code></td>
 </tr>
 </table>
 </div>
 </li>
            <li> <span class="li-head">query_v1_port</span> - SNMP v1 query port . <span class="li-normal">type: int</span>
 <a id='label438' href="javascript:ContentClick('label439', 'label438');" onmouseover="ContentPreview('label439');" onmouseout="ContentUnpreview('label439');" title="click to collapse or expand..."> more... </a>
 <div id="label439" style="display:none">
 <table border="1">
 <tr>
 <td></td>
 <td colspan="1">Supported Version Ranges</td>
 </tr>
 <tr>
 <td>query_v1_port</td>
 <td><code class="docutils literal notranslate">v6.2.0 -> 7.4.4 </code></td>
 </tr>
 </table>
 </div>
 </li>
            <li> <span class="li-head">query_v1_status</span> - Enable/disable SNMP v1 queries. <span class="li-normal">type: str</span> <span class="li-normal">choices: disable, enable</span>
 <a id='label440' href="javascript:ContentClick('label441', 'label440');" onmouseover="ContentPreview('label441');" onmouseout="ContentUnpreview('label441');" title="click to collapse or expand..."> more... </a>
 <div id="label441" style="display:none">
 <table border="1">
 <tr>
 <td></td>
 <td colspan="1">Supported Version Ranges</td>
 </tr>
 <tr>
 <td>query_v1_status</td>
 <td><code class="docutils literal notranslate">v6.2.0 -> 7.4.4 </code></td>
 </tr>
 <tr>
 <td>[disable]</td>
 <td><code class="docutils literal notranslate">v6.2.0 -> 7.4.4</code></td>
 <tr>
 <td>[enable]</td>
 <td><code class="docutils literal notranslate">v6.2.0 -> 7.4.4</code></td>
 </table>
 </div>
 </li>
            <li> <span class="li-head">query_v2c_port</span> - SNMP v2c query port . <span class="li-normal">type: int</span>
 <a id='label442' href="javascript:ContentClick('label443', 'label442');" onmouseover="ContentPreview('label443');" onmouseout="ContentUnpreview('label443');" title="click to collapse or expand..."> more... </a>
 <div id="label443" style="display:none">
 <table border="1">
 <tr>
 <td></td>
 <td colspan="1">Supported Version Ranges</td>
 </tr>
 <tr>
 <td>query_v2c_port</td>
 <td><code class="docutils literal notranslate">v6.2.0 -> 7.4.4 </code></td>
 </tr>
 </table>
 </div>
 </li>
            <li> <span class="li-head">query_v2c_status</span> - Enable/disable SNMP v2c queries. <span class="li-normal">type: str</span> <span class="li-normal">choices: disable, enable</span>
 <a id='label444' href="javascript:ContentClick('label445', 'label444');" onmouseover="ContentPreview('label445');" onmouseout="ContentUnpreview('label445');" title="click to collapse or expand..."> more... </a>
 <div id="label445" style="display:none">
 <table border="1">
 <tr>
 <td></td>
 <td colspan="1">Supported Version Ranges</td>
 </tr>
 <tr>
 <td>query_v2c_status</td>
 <td><code class="docutils literal notranslate">v6.2.0 -> 7.4.4 </code></td>
 </tr>
 <tr>
 <td>[disable]</td>
 <td><code class="docutils literal notranslate">v6.2.0 -> 7.4.4</code></td>
 <tr>
 <td>[enable]</td>
 <td><code class="docutils literal notranslate">v6.2.0 -> 7.4.4</code></td>
 </table>
 </div>
 </li>
            <li> <span class="li-head">status</span> - Enable/disable this SNMP community. <span class="li-normal">type: str</span> <span class="li-normal">choices: disable, enable</span>
 <a id='label446' href="javascript:ContentClick('label447', 'label446');" onmouseover="ContentPreview('label447');" onmouseout="ContentUnpreview('label447');" title="click to collapse or expand..."> more... </a>
 <div id="label447" style="display:none">
 <table border="1">
 <tr>
 <td></td>
 <td colspan="1">Supported Version Ranges</td>
 </tr>
 <tr>
 <td>status</td>
 <td><code class="docutils literal notranslate">v6.2.0 -> 7.4.4 </code></td>
 </tr>
 <tr>
 <td>[disable]</td>
 <td><code class="docutils literal notranslate">v6.2.0 -> 7.4.4</code></td>
 <tr>
 <td>[enable]</td>
 <td><code class="docutils literal notranslate">v6.2.0 -> 7.4.4</code></td>
 </table>
 </div>
 </li>
            <li> <span class="li-head">trap_v1_lport</span> - SNMP v2c trap local port . <span class="li-normal">type: int</span>
 <a id='label448' href="javascript:ContentClick('label449', 'label448');" onmouseover="ContentPreview('label449');" onmouseout="ContentUnpreview('label449');" title="click to collapse or expand..."> more... </a>
 <div id="label449" style="display:none">
 <table border="1">
 <tr>
 <td></td>
 <td colspan="1">Supported Version Ranges</td>
 </tr>
 <tr>
 <td>trap_v1_lport</td>
 <td><code class="docutils literal notranslate">v6.2.0 -> 7.4.4 </code></td>
 </tr>
 </table>
 </div>
 </li>
            <li> <span class="li-head">trap_v1_rport</span> - SNMP v2c trap remote port . <span class="li-normal">type: int</span>
 <a id='label450' href="javascript:ContentClick('label451', 'label450');" onmouseover="ContentPreview('label451');" onmouseout="ContentUnpreview('label451');" title="click to collapse or expand..."> more... </a>
 <div id="label451" style="display:none">
 <table border="1">
 <tr>
 <td></td>
 <td colspan="1">Supported Version Ranges</td>
 </tr>
 <tr>
 <td>trap_v1_rport</td>
 <td><code class="docutils literal notranslate">v6.2.0 -> 7.4.4 </code></td>
 </tr>
 </table>
 </div>
 </li>
            <li> <span class="li-head">trap_v1_status</span> - Enable/disable SNMP v1 traps. <span class="li-normal">type: str</span> <span class="li-normal">choices: disable, enable</span>
 <a id='label452' href="javascript:ContentClick('label453', 'label452');" onmouseover="ContentPreview('label453');" onmouseout="ContentUnpreview('label453');" title="click to collapse or expand..."> more... </a>
 <div id="label453" style="display:none">
 <table border="1">
 <tr>
 <td></td>
 <td colspan="1">Supported Version Ranges</td>
 </tr>
 <tr>
 <td>trap_v1_status</td>
 <td><code class="docutils literal notranslate">v6.2.0 -> 7.4.4 </code></td>
 </tr>
 <tr>
 <td>[disable]</td>
 <td><code class="docutils literal notranslate">v6.2.0 -> 7.4.4</code></td>
 <tr>
 <td>[enable]</td>
 <td><code class="docutils literal notranslate">v6.2.0 -> 7.4.4</code></td>
 </table>
 </div>
 </li>
            <li> <span class="li-head">trap_v2c_lport</span> - SNMP v2c trap local port . <span class="li-normal">type: int</span>
 <a id='label454' href="javascript:ContentClick('label455', 'label454');" onmouseover="ContentPreview('label455');" onmouseout="ContentUnpreview('label455');" title="click to collapse or expand..."> more... </a>
 <div id="label455" style="display:none">
 <table border="1">
 <tr>
 <td></td>
 <td colspan="1">Supported Version Ranges</td>
 </tr>
 <tr>
 <td>trap_v2c_lport</td>
 <td><code class="docutils literal notranslate">v6.2.0 -> 7.4.4 </code></td>
 </tr>
 </table>
 </div>
 </li>
            <li> <span class="li-head">trap_v2c_rport</span> - SNMP v2c trap remote port . <span class="li-normal">type: int</span>
 <a id='label456' href="javascript:ContentClick('label457', 'label456');" onmouseover="ContentPreview('label457');" onmouseout="ContentUnpreview('label457');" title="click to collapse or expand..."> more... </a>
 <div id="label457" style="display:none">
 <table border="1">
 <tr>
 <td></td>
 <td colspan="1">Supported Version Ranges</td>
 </tr>
 <tr>
 <td>trap_v2c_rport</td>
 <td><code class="docutils literal notranslate">v6.2.0 -> 7.4.4 </code></td>
 </tr>
 </table>
 </div>
 </li>
            <li> <span class="li-head">trap_v2c_status</span> - Enable/disable SNMP v2c traps. <span class="li-normal">type: str</span> <span class="li-normal">choices: disable, enable</span>
 <a id='label458' href="javascript:ContentClick('label459', 'label458');" onmouseover="ContentPreview('label459');" onmouseout="ContentUnpreview('label459');" title="click to collapse or expand..."> more... </a>
 <div id="label459" style="display:none">
 <table border="1">
 <tr>
 <td></td>
 <td colspan="1">Supported Version Ranges</td>
 </tr>
 <tr>
 <td>trap_v2c_status</td>
 <td><code class="docutils literal notranslate">v6.2.0 -> 7.4.4 </code></td>
 </tr>
 <tr>
 <td>[disable]</td>
 <td><code class="docutils literal notranslate">v6.2.0 -> 7.4.4</code></td>
 <tr>
 <td>[enable]</td>
 <td><code class="docutils literal notranslate">v6.2.0 -> 7.4.4</code></td>
 </table>
 </div>
 </li>
            </ul>
        <li> <span class="li-head">snmp_sysinfo</span> - Configuration method to edit Simple Network Management Protocol (SNMP) system info. <span class="li-normal">type: dict</span>
 <a id='label460' href="javascript:ContentClick('label461', 'label460');" onmouseover="ContentPreview('label461');" onmouseout="ContentUnpreview('label461');" title="click to collapse or expand..."> more... </a>
 <div id="label461" style="display:none">
 <table border="1">
 <tr>
 <td></td><td colspan="1">Supported Version Ranges</td>
 </tr>
 <tr>
 <td>snmp_sysinfo</td>
 <td><code class="docutils literal notranslate">v6.2.0 -> 7.4.4 </code></td>
 </tr>
 </table>
 </div>
 </li>
            <ul class="ul-self">
            <li> <span class="li-head">contact_info</span> - Contact information. <span class="li-normal">type: str</span>
 <a id='label462' href="javascript:ContentClick('label463', 'label462');" onmouseover="ContentPreview('label463');" onmouseout="ContentUnpreview('label463');" title="click to collapse or expand..."> more... </a>
 <div id="label463" style="display:none">
 <table border="1">
 <tr>
 <td></td>
 <td colspan="1">Supported Version Ranges</td>
 </tr>
 <tr>
 <td>contact_info</td>
 <td><code class="docutils literal notranslate">v6.2.0 -> 7.4.4 </code></td>
 </tr>
 </table>
 </div>
 </li>
            <li> <span class="li-head">description</span> - System description. <span class="li-normal">type: str</span>
 <a id='label464' href="javascript:ContentClick('label465', 'label464');" onmouseover="ContentPreview('label465');" onmouseout="ContentUnpreview('label465');" title="click to collapse or expand..."> more... </a>
 <div id="label465" style="display:none">
 <table border="1">
 <tr>
 <td></td>
 <td colspan="1">Supported Version Ranges</td>
 </tr>
 <tr>
 <td>description</td>
 <td><code class="docutils literal notranslate">v6.2.0 -> 7.4.4 </code></td>
 </tr>
 </table>
 </div>
 </li>
            <li> <span class="li-head">engine_id</span> - Local SNMP engine ID string (max 24 char). <span class="li-normal">type: str</span>
 <a id='label466' href="javascript:ContentClick('label467', 'label466');" onmouseover="ContentPreview('label467');" onmouseout="ContentUnpreview('label467');" title="click to collapse or expand..."> more... </a>
 <div id="label467" style="display:none">
 <table border="1">
 <tr>
 <td></td>
 <td colspan="1">Supported Version Ranges</td>
 </tr>
 <tr>
 <td>engine_id</td>
 <td><code class="docutils literal notranslate">v6.2.0 -> 7.4.4 </code></td>
 </tr>
 </table>
 </div>
 </li>
            <li> <span class="li-head">location</span> - System location. <span class="li-normal">type: str</span>
 <a id='label468' href="javascript:ContentClick('label469', 'label468');" onmouseover="ContentPreview('label469');" onmouseout="ContentUnpreview('label469');" title="click to collapse or expand..."> more... </a>
 <div id="label469" style="display:none">
 <table border="1">
 <tr>
 <td></td>
 <td colspan="1">Supported Version Ranges</td>
 </tr>
 <tr>
 <td>location</td>
 <td><code class="docutils literal notranslate">v6.2.0 -> 7.4.4 </code></td>
 </tr>
 </table>
 </div>
 </li>
            <li> <span class="li-head">status</span> - Enable/disable SNMP. <span class="li-normal">type: str</span> <span class="li-normal">choices: disable, enable</span>
 <a id='label470' href="javascript:ContentClick('label471', 'label470');" onmouseover="ContentPreview('label471');" onmouseout="ContentUnpreview('label471');" title="click to collapse or expand..."> more... </a>
 <div id="label471" style="display:none">
 <table border="1">
 <tr>
 <td></td>
 <td colspan="1">Supported Version Ranges</td>
 </tr>
 <tr>
 <td>status</td>
 <td><code class="docutils literal notranslate">v6.2.0 -> 7.4.4 </code></td>
 </tr>
 <tr>
 <td>[disable]</td>
 <td><code class="docutils literal notranslate">v6.2.0 -> 7.4.4</code></td>
 <tr>
 <td>[enable]</td>
 <td><code class="docutils literal notranslate">v6.2.0 -> 7.4.4</code></td>
 </table>
 </div>
 </li>
            </ul>
        <li> <span class="li-head">snmp_trap_threshold</span> - Configuration method to edit Simple Network Management Protocol (SNMP) trap threshold values. <span class="li-normal">type: dict</span>
 <a id='label472' href="javascript:ContentClick('label473', 'label472');" onmouseover="ContentPreview('label473');" onmouseout="ContentUnpreview('label473');" title="click to collapse or expand..."> more... </a>
 <div id="label473" style="display:none">
 <table border="1">
 <tr>
 <td></td><td colspan="1">Supported Version Ranges</td>
 </tr>
 <tr>
 <td>snmp_trap_threshold</td>
 <td><code class="docutils literal notranslate">v6.2.0 -> 7.4.4 </code></td>
 </tr>
 </table>
 </div>
 </li>
            <ul class="ul-self">
            <li> <span class="li-head">trap_high_cpu_threshold</span> - CPU usage when trap is sent. <span class="li-normal">type: int</span>
 <a id='label474' href="javascript:ContentClick('label475', 'label474');" onmouseover="ContentPreview('label475');" onmouseout="ContentUnpreview('label475');" title="click to collapse or expand..."> more... </a>
 <div id="label475" style="display:none">
 <table border="1">
 <tr>
 <td></td>
 <td colspan="1">Supported Version Ranges</td>
 </tr>
 <tr>
 <td>trap_high_cpu_threshold</td>
 <td><code class="docutils literal notranslate">v6.2.0 -> 7.4.4 </code></td>
 </tr>
 </table>
 </div>
 </li>
            <li> <span class="li-head">trap_log_full_threshold</span> - Log disk usage when trap is sent. <span class="li-normal">type: int</span>
 <a id='label476' href="javascript:ContentClick('label477', 'label476');" onmouseover="ContentPreview('label477');" onmouseout="ContentUnpreview('label477');" title="click to collapse or expand..."> more... </a>
 <div id="label477" style="display:none">
 <table border="1">
 <tr>
 <td></td>
 <td colspan="1">Supported Version Ranges</td>
 </tr>
 <tr>
 <td>trap_log_full_threshold</td>
 <td><code class="docutils literal notranslate">v6.2.0 -> 7.4.4 </code></td>
 </tr>
 </table>
 </div>
 </li>
            <li> <span class="li-head">trap_low_memory_threshold</span> - Memory usage when trap is sent. <span class="li-normal">type: int</span>
 <a id='label478' href="javascript:ContentClick('label479', 'label478');" onmouseover="ContentPreview('label479');" onmouseout="ContentUnpreview('label479');" title="click to collapse or expand..."> more... </a>
 <div id="label479" style="display:none">
 <table border="1">
 <tr>
 <td></td>
 <td colspan="1">Supported Version Ranges</td>
 </tr>
 <tr>
 <td>trap_low_memory_threshold</td>
 <td><code class="docutils literal notranslate">v6.2.0 -> 7.4.4 </code></td>
 </tr>
 </table>
 </div>
 </li>
            </ul>
        <li> <span class="li-head">snmp_user</span> - Configuration method to edit Simple Network Management Protocol (SNMP) users. <span class="li-normal">type: list</span> <span style="font-family:'Courier New'" class="li-required">member_path: snmp_user:name</span>
 <a id='label480' href="javascript:ContentClick('label481', 'label480');" onmouseover="ContentPreview('label481');" onmouseout="ContentUnpreview('label481');" title="click to collapse or expand..."> more... </a>
 <div id="label481" style="display:none">
 <table border="1">
 <tr>
 <td></td><td colspan="1">Supported Version Ranges</td>
 </tr>
 <tr>
 <td>snmp_user</td>
 <td><code class="docutils literal notranslate">v6.2.0 -> 7.4.4 </code></td>
 </tr>
 </table>
 </div>
 </li>
            <ul class="ul-self">
            <li> <span class="li-head">auth_proto</span> - Authentication protocol. <span class="li-normal">type: str</span> <span class="li-normal">choices: md5, sha1, sha224, sha256, sha384, sha512, sha</span>
 <a id='label482' href="javascript:ContentClick('label483', 'label482');" onmouseover="ContentPreview('label483');" onmouseout="ContentUnpreview('label483');" title="click to collapse or expand..."> more... </a>
 <div id="label483" style="display:none">
 <table border="1">
 <tr>
 <td></td>
 <td colspan="1">Supported Version Ranges</td>
 </tr>
 <tr>
 <td>auth_proto</td>
 <td><code class="docutils literal notranslate">v6.2.0 -> 7.4.4 </code></td>
 </tr>
 <tr>
 <td>[md5]</td>
 <td><code class="docutils literal notranslate">v6.2.0 -> 7.4.4</code></td>
 <tr>
 <td>[sha1]</td>
 <td><code class="docutils literal notranslate">v7.0.0 -> 7.4.4</code></td>
 </tr>
 <tr>
 <td>[sha224]</td>
 <td><code class="docutils literal notranslate">v7.0.0 -> 7.4.4</code></td>
 </tr>
 <tr>
 <td>[sha256]</td>
 <td><code class="docutils literal notranslate">v7.0.0 -> 7.4.4</code></td>
 </tr>
 <tr>
 <td>[sha384]</td>
 <td><code class="docutils literal notranslate">v7.0.0 -> 7.4.4</code></td>
 </tr>
 <tr>
 <td>[sha512]</td>
 <td><code class="docutils literal notranslate">v7.0.0 -> 7.4.4</code></td>
 </tr>
 <tr>
 <td>[sha]</td>
 <td><code class="docutils literal notranslate">v6.2.0 -> v6.4.4</code></td>
 </tr>
 </table>
 </div>
 </li>
            <li> <span class="li-head">auth_pwd</span> - Password for authentication protocol. <span class="li-normal">type: str</span>
 <a id='label484' href="javascript:ContentClick('label485', 'label484');" onmouseover="ContentPreview('label485');" onmouseout="ContentUnpreview('label485');" title="click to collapse or expand..."> more... </a>
 <div id="label485" style="display:none">
 <table border="1">
 <tr>
 <td></td>
 <td colspan="1">Supported Version Ranges</td>
 </tr>
 <tr>
 <td>auth_pwd</td>
 <td><code class="docutils literal notranslate">v6.2.0 -> 7.4.4 </code></td>
 </tr>
 </table>
 </div>
 </li>
            <li> <span class="li-head">name</span> - SNMP user name. <span class="li-normal">type: str</span> <span class="li-required">required: true</span>
 <a id='label486' href="javascript:ContentClick('label487', 'label486');" onmouseover="ContentPreview('label487');" onmouseout="ContentUnpreview('label487');" title="click to collapse or expand..."> more... </a>
 <div id="label487" style="display:none">
 <table border="1">
 <tr>
 <td></td>
 <td colspan="1">Supported Version Ranges</td>
 </tr>
 <tr>
 <td>name</td>
 <td><code class="docutils literal notranslate">v6.2.0 -> 7.4.4 </code></td>
 </tr>
 </table>
 </div>
 </li>
            <li> <span class="li-head">priv_proto</span> - Privacy (encryption) protocol. <span class="li-normal">type: str</span> <span class="li-normal">choices: aes128, aes192, aes192c, aes256, aes256c, des, aes</span>
 <a id='label488' href="javascript:ContentClick('label489', 'label488');" onmouseover="ContentPreview('label489');" onmouseout="ContentUnpreview('label489');" title="click to collapse or expand..."> more... </a>
 <div id="label489" style="display:none">
 <table border="1">
 <tr>
 <td></td>
 <td colspan="1">Supported Version Ranges</td>
 </tr>
 <tr>
 <td>priv_proto</td>
 <td><code class="docutils literal notranslate">v6.2.0 -> 7.4.4 </code></td>
 </tr>
 <tr>
 <td>[aes128]</td>
 <td><code class="docutils literal notranslate">v7.0.0 -> 7.4.4</code></td>
 </tr>
 <tr>
 <td>[aes192]</td>
 <td><code class="docutils literal notranslate">v7.0.0 -> 7.4.4</code></td>
 </tr>
 <tr>
 <td>[aes192c]</td>
 <td><code class="docutils literal notranslate">v7.0.0 -> 7.4.4</code></td>
 </tr>
 <tr>
 <td>[aes256]</td>
 <td><code class="docutils literal notranslate">v7.0.0 -> 7.4.4</code></td>
 </tr>
 <tr>
 <td>[aes256c]</td>
 <td><code class="docutils literal notranslate">v7.0.0 -> 7.4.4</code></td>
 </tr>
 <tr>
 <td>[des]</td>
 <td><code class="docutils literal notranslate">v6.2.0 -> 7.4.4</code></td>
 <tr>
 <td>[aes]</td>
 <td><code class="docutils literal notranslate">v6.2.0 -> v6.4.4</code></td>
 </tr>
 </table>
 </div>
 </li>
            <li> <span class="li-head">priv_pwd</span> - Password for privacy (encryption) protocol. <span class="li-normal">type: str</span>
 <a id='label490' href="javascript:ContentClick('label491', 'label490');" onmouseover="ContentPreview('label491');" onmouseout="ContentUnpreview('label491');" title="click to collapse or expand..."> more... </a>
 <div id="label491" style="display:none">
 <table border="1">
 <tr>
 <td></td>
 <td colspan="1">Supported Version Ranges</td>
 </tr>
 <tr>
 <td>priv_pwd</td>
 <td><code class="docutils literal notranslate">v6.2.0 -> 7.4.4 </code></td>
 </tr>
 </table>
 </div>
 </li>
            <li> <span class="li-head">queries</span> - Enable/disable SNMP queries for this user. <span class="li-normal">type: str</span> <span class="li-normal">choices: disable, enable</span>
 <a id='label492' href="javascript:ContentClick('label493', 'label492');" onmouseover="ContentPreview('label493');" onmouseout="ContentUnpreview('label493');" title="click to collapse or expand..."> more... </a>
 <div id="label493" style="display:none">
 <table border="1">
 <tr>
 <td></td>
 <td colspan="1">Supported Version Ranges</td>
 </tr>
 <tr>
 <td>queries</td>
 <td><code class="docutils literal notranslate">v6.2.0 -> 7.4.4 </code></td>
 </tr>
 <tr>
 <td>[disable]</td>
 <td><code class="docutils literal notranslate">v6.2.0 -> 7.4.4</code></td>
 <tr>
 <td>[enable]</td>
 <td><code class="docutils literal notranslate">v6.2.0 -> 7.4.4</code></td>
 </table>
 </div>
 </li>
            <li> <span class="li-head">query_port</span> - SNMPv3 query port . <span class="li-normal">type: int</span>
 <a id='label494' href="javascript:ContentClick('label495', 'label494');" onmouseover="ContentPreview('label495');" onmouseout="ContentUnpreview('label495');" title="click to collapse or expand..."> more... </a>
 <div id="label495" style="display:none">
 <table border="1">
 <tr>
 <td></td>
 <td colspan="1">Supported Version Ranges</td>
 </tr>
 <tr>
 <td>query_port</td>
 <td><code class="docutils literal notranslate">v6.2.0 -> 7.4.4 </code></td>
 </tr>
 </table>
 </div>
 </li>
            <li> <span class="li-head">security_level</span> - Security level for message authentication and encryption. <span class="li-normal">type: str</span> <span class="li-normal">choices: no-auth-no-priv, auth-no-priv, auth-priv</span>
 <a id='label496' href="javascript:ContentClick('label497', 'label496');" onmouseover="ContentPreview('label497');" onmouseout="ContentUnpreview('label497');" title="click to collapse or expand..."> more... </a>
 <div id="label497" style="display:none">
 <table border="1">
 <tr>
 <td></td>
 <td colspan="1">Supported Version Ranges</td>
 </tr>
 <tr>
 <td>security_level</td>
 <td><code class="docutils literal notranslate">v6.2.0 -> 7.4.4 </code></td>
 </tr>
 <tr>
 <td>[no-auth-no-priv]</td>
 <td><code class="docutils literal notranslate">v6.2.0 -> 7.4.4</code></td>
 <tr>
 <td>[auth-no-priv]</td>
 <td><code class="docutils literal notranslate">v6.2.0 -> 7.4.4</code></td>
 <tr>
 <td>[auth-priv]</td>
 <td><code class="docutils literal notranslate">v6.2.0 -> 7.4.4</code></td>
 </table>
 </div>
 </li>
            </ul>
        <li> <span class="li-head">staged_image_version</span> - Staged image version for FortiSwitch. <span class="li-normal">type: str</span>
 <a id='label498' href="javascript:ContentClick('label499', 'label498');" onmouseover="ContentPreview('label499');" onmouseout="ContentUnpreview('label499');" title="click to collapse or expand..."> more... </a>
 <div id="label499" style="display:none">
 <table border="1">
 <tr>
 <td></td>
 <td colspan="1">Supported Version Ranges</td>
 </tr>
 <tr>
 <td>staged_image_version</td>
 <td><code class="docutils literal notranslate">v6.0.0 -> 7.4.4 </code></td>
 </tr>
 </table>
 </div>
 </li>
        <li> <span class="li-head">static_mac</span> - Configuration method to edit FortiSwitch Static and Sticky MAC. <span class="li-normal">type: list</span> <span style="font-family:'Courier New'" class="li-required">member_path: static_mac:id</span>
 <a id='label500' href="javascript:ContentClick('label501', 'label500');" onmouseover="ContentPreview('label501');" onmouseout="ContentUnpreview('label501');" title="click to collapse or expand..."> more... </a>
 <div id="label501" style="display:none">
 <table border="1">
 <tr>
 <td></td><td colspan="1">Supported Version Ranges</td>
 </tr>
 <tr>
 <td>static_mac</td>
 <td><code class="docutils literal notranslate">v6.2.0 -> 7.4.4 </code></td>
 </tr>
 </table>
 </div>
 </li>
            <ul class="ul-self">
            <li> <span class="li-head">description</span> - Description. <span class="li-normal">type: str</span>
 <a id='label502' href="javascript:ContentClick('label503', 'label502');" onmouseover="ContentPreview('label503');" onmouseout="ContentUnpreview('label503');" title="click to collapse or expand..."> more... </a>
 <div id="label503" style="display:none">
 <table border="1">
 <tr>
 <td></td>
 <td colspan="1">Supported Version Ranges</td>
 </tr>
 <tr>
 <td>description</td>
 <td><code class="docutils literal notranslate">v6.2.0 -> 7.4.4 </code></td>
 </tr>
 </table>
 </div>
 </li>
            <li> <span class="li-head">id</span> - ID. see <a href='#notes'>Notes</a>. <span class="li-normal">type: int</span> <span class="li-required">required: true</span>
 <a id='label504' href="javascript:ContentClick('label505', 'label504');" onmouseover="ContentPreview('label505');" onmouseout="ContentUnpreview('label505');" title="click to collapse or expand..."> more... </a>
 <div id="label505" style="display:none">
 <table border="1">
 <tr>
 <td></td>
 <td colspan="1">Supported Version Ranges</td>
 </tr>
 <tr>
 <td>id</td>
 <td><code class="docutils literal notranslate">v6.2.0 -> 7.4.4 </code></td>
 </tr>
 </table>
 </div>
 </li>
            <li> <span class="li-head">interface</span> - Interface name. <span class="li-normal">type: str</span>
 <a id='label506' href="javascript:ContentClick('label507', 'label506');" onmouseover="ContentPreview('label507');" onmouseout="ContentUnpreview('label507');" title="click to collapse or expand..."> more... </a>
 <div id="label507" style="display:none">
 <table border="1">
 <tr>
 <td></td>
 <td colspan="1">Supported Version Ranges</td>
 </tr>
 <tr>
 <td>interface</td>
 <td><code class="docutils literal notranslate">v6.2.0 -> 7.4.4 </code></td>
 </tr>
 </table>
 </div>
 </li>
            <li> <span class="li-head">mac</span> - MAC address. <span class="li-normal">type: str</span>
 <a id='label508' href="javascript:ContentClick('label509', 'label508');" onmouseover="ContentPreview('label509');" onmouseout="ContentUnpreview('label509');" title="click to collapse or expand..."> more... </a>
 <div id="label509" style="display:none">
 <table border="1">
 <tr>
 <td></td>
 <td colspan="1">Supported Version Ranges</td>
 </tr>
 <tr>
 <td>mac</td>
 <td><code class="docutils literal notranslate">v6.2.0 -> 7.4.4 </code></td>
 </tr>
 </table>
 </div>
 </li>
            <li> <span class="li-head">type</span> - Type. <span class="li-normal">type: str</span> <span class="li-normal">choices: static, sticky</span>
 <a id='label510' href="javascript:ContentClick('label511', 'label510');" onmouseover="ContentPreview('label511');" onmouseout="ContentUnpreview('label511');" title="click to collapse or expand..."> more... </a>
 <div id="label511" style="display:none">
 <table border="1">
 <tr>
 <td></td>
 <td colspan="1">Supported Version Ranges</td>
 </tr>
 <tr>
 <td>type</td>
 <td><code class="docutils literal notranslate">v6.2.0 -> 7.4.4 </code></td>
 </tr>
 <tr>
 <td>[static]</td>
 <td><code class="docutils literal notranslate">v6.2.0 -> 7.4.4</code></td>
 <tr>
 <td>[sticky]</td>
 <td><code class="docutils literal notranslate">v6.2.0 -> 7.4.4</code></td>
 </table>
 </div>
 </li>
            <li> <span class="li-head">vlan</span> - Vlan. Source system.interface.name. <span class="li-normal">type: str</span>
 <a id='label512' href="javascript:ContentClick('label513', 'label512');" onmouseover="ContentPreview('label513');" onmouseout="ContentUnpreview('label513');" title="click to collapse or expand..."> more... </a>
 <div id="label513" style="display:none">
 <table border="1">
 <tr>
 <td></td>
 <td colspan="1">Supported Version Ranges</td>
 </tr>
 <tr>
 <td>vlan</td>
 <td><code class="docutils literal notranslate">v6.2.0 -> 7.4.4 </code></td>
 </tr>
 </table>
 </div>
 </li>
            </ul>
        <li> <span class="li-head">storm_control</span> - Configuration method to edit FortiSwitch storm control for measuring traffic activity using data rates to prevent traffic disruption. <span class="li-normal">type: dict</span>
 <a id='label514' href="javascript:ContentClick('label515', 'label514');" onmouseover="ContentPreview('label515');" onmouseout="ContentUnpreview('label515');" title="click to collapse or expand..."> more... </a>
 <div id="label515" style="display:none">
 <table border="1">
 <tr>
 <td></td><td colspan="1">Supported Version Ranges</td>
 </tr>
 <tr>
 <td>storm_control</td>
 <td><code class="docutils literal notranslate">v6.0.0 -> 7.4.4 </code></td>
 </tr>
 </table>
 </div>
 </li>
            <ul class="ul-self">
            <li> <span class="li-head">broadcast</span> - Enable/disable storm control to drop broadcast traffic. <span class="li-normal">type: str</span> <span class="li-normal">choices: enable, disable</span>
 <a id='label516' href="javascript:ContentClick('label517', 'label516');" onmouseover="ContentPreview('label517');" onmouseout="ContentUnpreview('label517');" title="click to collapse or expand..."> more... </a>
 <div id="label517" style="display:none">
 <table border="1">
 <tr>
 <td></td>
 <td colspan="1">Supported Version Ranges</td>
 </tr>
 <tr>
 <td>broadcast</td>
 <td><code class="docutils literal notranslate">v6.0.0 -> 7.4.4 </code></td>
 </tr>
 <tr>
 <td>[enable]</td>
 <td><code class="docutils literal notranslate">v6.0.0 -> 7.4.4</code></td>
 <tr>
 <td>[disable]</td>
 <td><code class="docutils literal notranslate">v6.0.0 -> 7.4.4</code></td>
 </table>
 </div>
 </li>
            <li> <span class="li-head">local_override</span> - Enable to override global FortiSwitch storm control settings for this FortiSwitch. <span class="li-normal">type: str</span> <span class="li-normal">choices: enable, disable</span>
 <a id='label518' href="javascript:ContentClick('label519', 'label518');" onmouseover="ContentPreview('label519');" onmouseout="ContentUnpreview('label519');" title="click to collapse or expand..."> more... </a>
 <div id="label519" style="display:none">
 <table border="1">
 <tr>
 <td></td>
 <td colspan="1">Supported Version Ranges</td>
 </tr>
 <tr>
 <td>local_override</td>
 <td><code class="docutils literal notranslate">v6.0.0 -> 7.4.4 </code></td>
 </tr>
 <tr>
 <td>[enable]</td>
 <td><code class="docutils literal notranslate">v6.0.0 -> 7.4.4</code></td>
 <tr>
 <td>[disable]</td>
 <td><code class="docutils literal notranslate">v6.0.0 -> 7.4.4</code></td>
 </table>
 </div>
 </li>
            <li> <span class="li-head">rate</span> - Rate in packets per second at which storm control drops excess traffic(0-10000000). <span class="li-normal">type: int</span>
 <a id='label520' href="javascript:ContentClick('label521', 'label520');" onmouseover="ContentPreview('label521');" onmouseout="ContentUnpreview('label521');" title="click to collapse or expand..."> more... </a>
 <div id="label521" style="display:none">
 <table border="1">
 <tr>
 <td></td>
 <td colspan="1">Supported Version Ranges</td>
 </tr>
 <tr>
 <td>rate</td>
 <td><code class="docutils literal notranslate">v6.0.0 -> 7.4.4 </code></td>
 </tr>
 </table>
 </div>
 </li>
            <li> <span class="li-head">unknown_multicast</span> - Enable/disable storm control to drop unknown multicast traffic. <span class="li-normal">type: str</span> <span class="li-normal">choices: enable, disable</span>
 <a id='label522' href="javascript:ContentClick('label523', 'label522');" onmouseover="ContentPreview('label523');" onmouseout="ContentUnpreview('label523');" title="click to collapse or expand..."> more... </a>
 <div id="label523" style="display:none">
 <table border="1">
 <tr>
 <td></td>
 <td colspan="1">Supported Version Ranges</td>
 </tr>
 <tr>
 <td>unknown_multicast</td>
 <td><code class="docutils literal notranslate">v6.0.0 -> 7.4.4 </code></td>
 </tr>
 <tr>
 <td>[enable]</td>
 <td><code class="docutils literal notranslate">v6.0.0 -> 7.4.4</code></td>
 <tr>
 <td>[disable]</td>
 <td><code class="docutils literal notranslate">v6.0.0 -> 7.4.4</code></td>
 </table>
 </div>
 </li>
            <li> <span class="li-head">unknown_unicast</span> - Enable/disable storm control to drop unknown unicast traffic. <span class="li-normal">type: str</span> <span class="li-normal">choices: enable, disable</span>
 <a id='label524' href="javascript:ContentClick('label525', 'label524');" onmouseover="ContentPreview('label525');" onmouseout="ContentUnpreview('label525');" title="click to collapse or expand..."> more... </a>
 <div id="label525" style="display:none">
 <table border="1">
 <tr>
 <td></td>
 <td colspan="1">Supported Version Ranges</td>
 </tr>
 <tr>
 <td>unknown_unicast</td>
 <td><code class="docutils literal notranslate">v6.0.0 -> 7.4.4 </code></td>
 </tr>
 <tr>
 <td>[enable]</td>
 <td><code class="docutils literal notranslate">v6.0.0 -> 7.4.4</code></td>
 <tr>
 <td>[disable]</td>
 <td><code class="docutils literal notranslate">v6.0.0 -> 7.4.4</code></td>
 </table>
 </div>
 </li>
            </ul>
        <li> <span class="li-head">stp_instance</span> - Configuration method to edit Spanning Tree Protocol (STP) instances. <span class="li-normal">type: list</span> <span style="font-family:'Courier New'" class="li-required">member_path: stp_instance:id</span>
 <a id='label526' href="javascript:ContentClick('label527', 'label526');" onmouseover="ContentPreview('label527');" onmouseout="ContentUnpreview('label527');" title="click to collapse or expand..."> more... </a>
 <div id="label527" style="display:none">
 <table border="1">
 <tr>
 <td></td><td colspan="1">Supported Version Ranges</td>
 </tr>
 <tr>
 <td>stp_instance</td>
 <td><code class="docutils literal notranslate">v6.2.0 -> 7.4.4 </code></td>
 </tr>
 </table>
 </div>
 </li>
            <ul class="ul-self">
            <li> <span class="li-head">id</span> - Instance ID. <span class="li-normal">type: str</span> <span class="li-required">required: true</span>
 <a id='label528' href="javascript:ContentClick('label529', 'label528');" onmouseover="ContentPreview('label529');" onmouseout="ContentUnpreview('label529');" title="click to collapse or expand..."> more... </a>
 <div id="label529" style="display:none">
 <table border="1">
 <tr>
 <td></td>
 <td colspan="1">Supported Version Ranges</td>
 </tr>
 <tr>
 <td>id</td>
 <td><code class="docutils literal notranslate">v6.2.0 -> 7.4.4 </code></td>
 </tr>
 </table>
 </div>
 </li>
            <li> <span class="li-head">priority</span> - Priority. <span class="li-normal">type: str</span> <span class="li-normal">choices: 0, 4096, 8192, 12288, 16384, 20480, 24576, 28672, 32768, 36864, 40960, 45056, 49152, 53248, 57344, 61440</span>
 <a id='label530' href="javascript:ContentClick('label531', 'label530');" onmouseover="ContentPreview('label531');" onmouseout="ContentUnpreview('label531');" title="click to collapse or expand..."> more... </a>
 <div id="label531" style="display:none">
 <table border="1">
 <tr>
 <td></td>
 <td colspan="1">Supported Version Ranges</td>
 </tr>
 <tr>
 <td>priority</td>
 <td><code class="docutils literal notranslate">v6.2.0 -> 7.4.4 </code></td>
 </tr>
 <tr>
 <td>[0]</td>
 <td><code class="docutils literal notranslate">v6.2.0 -> 7.4.4</code></td>
 <tr>
 <td>[4096]</td>
 <td><code class="docutils literal notranslate">v6.2.0 -> 7.4.4</code></td>
 <tr>
 <td>[8192]</td>
 <td><code class="docutils literal notranslate">v6.2.0 -> 7.4.4</code></td>
 <tr>
 <td>[12288]</td>
 <td><code class="docutils literal notranslate">v6.2.0 -> 7.4.4</code></td>
 <tr>
 <td>[16384]</td>
 <td><code class="docutils literal notranslate">v6.2.0 -> 7.4.4</code></td>
 <tr>
 <td>[20480]</td>
 <td><code class="docutils literal notranslate">v6.2.0 -> 7.4.4</code></td>
 <tr>
 <td>[24576]</td>
 <td><code class="docutils literal notranslate">v6.2.0 -> 7.4.4</code></td>
 <tr>
 <td>[28672]</td>
 <td><code class="docutils literal notranslate">v6.2.0 -> 7.4.4</code></td>
 <tr>
 <td>[32768]</td>
 <td><code class="docutils literal notranslate">v6.2.0 -> 7.4.4</code></td>
 <tr>
 <td>[36864]</td>
 <td><code class="docutils literal notranslate">v6.2.0 -> 7.4.4</code></td>
 <tr>
 <td>[40960]</td>
 <td><code class="docutils literal notranslate">v6.2.0 -> 7.4.4</code></td>
 <tr>
 <td>[45056]</td>
 <td><code class="docutils literal notranslate">v6.2.0 -> 7.4.4</code></td>
 <tr>
 <td>[49152]</td>
 <td><code class="docutils literal notranslate">v6.2.0 -> 7.4.4</code></td>
 <tr>
 <td>[53248]</td>
 <td><code class="docutils literal notranslate">v6.2.0 -> 7.4.4</code></td>
 <tr>
 <td>[57344]</td>
 <td><code class="docutils literal notranslate">v6.2.0 -> 7.4.4</code></td>
 <tr>
 <td>[61440]</td>
 <td><code class="docutils literal notranslate">v6.2.0 -> 7.4.4</code></td>
 </table>
 </div>
 </li>
            </ul>
        <li> <span class="li-head">stp_settings</span> - Configuration method to edit Spanning Tree Protocol (STP) settings used to prevent bridge loops. <span class="li-normal">type: dict</span>
 <a id='label532' href="javascript:ContentClick('label533', 'label532');" onmouseover="ContentPreview('label533');" onmouseout="ContentUnpreview('label533');" title="click to collapse or expand..."> more... </a>
 <div id="label533" style="display:none">
 <table border="1">
 <tr>
 <td></td><td colspan="1">Supported Version Ranges</td>
 </tr>
 <tr>
 <td>stp_settings</td>
 <td><code class="docutils literal notranslate">v6.0.0 -> 7.4.4 </code></td>
 </tr>
 </table>
 </div>
 </li>
            <ul class="ul-self">
            <li> <span class="li-head">forward_time</span> - Period of time a port is in listening and learning state (4 - 30 sec). <span class="li-normal">type: int</span>
 <a id='label534' href="javascript:ContentClick('label535', 'label534');" onmouseover="ContentPreview('label535');" onmouseout="ContentUnpreview('label535');" title="click to collapse or expand..."> more... </a>
 <div id="label535" style="display:none">
 <table border="1">
 <tr>
 <td></td>
 <td colspan="1">Supported Version Ranges</td>
 </tr>
 <tr>
 <td>forward_time</td>
 <td><code class="docutils literal notranslate">v6.0.0 -> 7.4.4 </code></td>
 </tr>
 </table>
 </div>
 </li>
            <li> <span class="li-head">hello_time</span> - Period of time between successive STP frame Bridge Protocol Data Units (BPDUs) sent on a port (1 - 10 sec). <span class="li-normal">type: int</span>
 <a id='label536' href="javascript:ContentClick('label537', 'label536');" onmouseover="ContentPreview('label537');" onmouseout="ContentUnpreview('label537');" title="click to collapse or expand..."> more... </a>
 <div id="label537" style="display:none">
 <table border="1">
 <tr>
 <td></td>
 <td colspan="1">Supported Version Ranges</td>
 </tr>
 <tr>
 <td>hello_time</td>
 <td><code class="docutils literal notranslate">v6.0.0 -> 7.4.4 </code></td>
 </tr>
 </table>
 </div>
 </li>
            <li> <span class="li-head">local_override</span> - Enable to configure local STP settings that override global STP settings. <span class="li-normal">type: str</span> <span class="li-normal">choices: enable, disable</span>
 <a id='label538' href="javascript:ContentClick('label539', 'label538');" onmouseover="ContentPreview('label539');" onmouseout="ContentUnpreview('label539');" title="click to collapse or expand..."> more... </a>
 <div id="label539" style="display:none">
 <table border="1">
 <tr>
 <td></td>
 <td colspan="1">Supported Version Ranges</td>
 </tr>
 <tr>
 <td>local_override</td>
 <td><code class="docutils literal notranslate">v6.0.0 -> 7.4.4 </code></td>
 </tr>
 <tr>
 <td>[enable]</td>
 <td><code class="docutils literal notranslate">v6.0.0 -> 7.4.4</code></td>
 <tr>
 <td>[disable]</td>
 <td><code class="docutils literal notranslate">v6.0.0 -> 7.4.4</code></td>
 </table>
 </div>
 </li>
            <li> <span class="li-head">max_age</span> - Maximum time before a bridge port saves its configuration BPDU information (6 - 40 sec). <span class="li-normal">type: int</span>
 <a id='label540' href="javascript:ContentClick('label541', 'label540');" onmouseover="ContentPreview('label541');" onmouseout="ContentUnpreview('label541');" title="click to collapse or expand..."> more... </a>
 <div id="label541" style="display:none">
 <table border="1">
 <tr>
 <td></td>
 <td colspan="1">Supported Version Ranges</td>
 </tr>
 <tr>
 <td>max_age</td>
 <td><code class="docutils literal notranslate">v6.0.0 -> 7.4.4 </code></td>
 </tr>
 </table>
 </div>
 </li>
            <li> <span class="li-head">max_hops</span> - Maximum number of hops between the root bridge and the furthest bridge (1- 40). <span class="li-normal">type: int</span>
 <a id='label542' href="javascript:ContentClick('label543', 'label542');" onmouseover="ContentPreview('label543');" onmouseout="ContentUnpreview('label543');" title="click to collapse or expand..."> more... </a>
 <div id="label543" style="display:none">
 <table border="1">
 <tr>
 <td></td>
 <td colspan="1">Supported Version Ranges</td>
 </tr>
 <tr>
 <td>max_hops</td>
 <td><code class="docutils literal notranslate">v6.0.0 -> 7.4.4 </code></td>
 </tr>
 </table>
 </div>
 </li>
            <li> <span class="li-head">name</span> - Name of local STP settings configuration. <span class="li-normal">type: str</span>
 <a id='label544' href="javascript:ContentClick('label545', 'label544');" onmouseover="ContentPreview('label545');" onmouseout="ContentUnpreview('label545');" title="click to collapse or expand..."> more... </a>
 <div id="label545" style="display:none">
 <table border="1">
 <tr>
 <td></td>
 <td colspan="1">Supported Version Ranges</td>
 </tr>
 <tr>
 <td>name</td>
 <td><code class="docutils literal notranslate">v6.0.0 -> 7.4.4 </code></td>
 </tr>
 </table>
 </div>
 </li>
            <li> <span class="li-head">pending_timer</span> - Pending time (1 - 15 sec). <span class="li-normal">type: int</span>
 <a id='label546' href="javascript:ContentClick('label547', 'label546');" onmouseover="ContentPreview('label547');" onmouseout="ContentUnpreview('label547');" title="click to collapse or expand..."> more... </a>
 <div id="label547" style="display:none">
 <table border="1">
 <tr>
 <td></td>
 <td colspan="1">Supported Version Ranges</td>
 </tr>
 <tr>
 <td>pending_timer</td>
 <td><code class="docutils literal notranslate">v6.0.0 -> 7.4.4 </code></td>
 </tr>
 </table>
 </div>
 </li>
            <li> <span class="li-head">revision</span> - STP revision number (0 - 65535). <span class="li-normal">type: int</span>
 <a id='label548' href="javascript:ContentClick('label549', 'label548');" onmouseover="ContentPreview('label549');" onmouseout="ContentUnpreview('label549');" title="click to collapse or expand..."> more... </a>
 <div id="label549" style="display:none">
 <table border="1">
 <tr>
 <td></td>
 <td colspan="1">Supported Version Ranges</td>
 </tr>
 <tr>
 <td>revision</td>
 <td><code class="docutils literal notranslate">v6.0.0 -> 7.4.4 </code></td>
 </tr>
 </table>
 </div>
 </li>
            <li> <span class="li-head">status</span> - Enable/disable STP. <span class="li-normal">type: str</span> <span class="li-normal">choices: enable, disable</span>
 <a id='label550' href="javascript:ContentClick('label551', 'label550');" onmouseover="ContentPreview('label551');" onmouseout="ContentUnpreview('label551');" title="click to collapse or expand..."> more... </a>
 <div id="label551" style="display:none">
 <table border="1">
 <tr>
 <td></td>
 <td colspan="2">Supported Version Ranges</td>
 </tr>
 <tr>
 <td>status</td>
 <td><code class="docutils literal notranslate">v6.0.0 -> v6.0.11 </code></td>
 <td><code class="docutils literal notranslate">v6.2.3 -> v6.2.3 </code></td>
 </tr>
 <tr>
 <td>[enable]</td>
 <td><code class="docutils literal notranslate">v6.0.0 -> v6.0.11</code></td>
 <tr>
 <td>[disable]</td>
 <td><code class="docutils literal notranslate">v6.0.0 -> v6.0.11</code></td>
 </table>
 </div>
 </li>
            </ul>
        <li> <span class="li-head">switch_device_tag</span> - User definable label/tag. <span class="li-normal">type: str</span>
 <a id='label552' href="javascript:ContentClick('label553', 'label552');" onmouseover="ContentPreview('label553');" onmouseout="ContentUnpreview('label553');" title="click to collapse or expand..."> more... </a>
 <div id="label553" style="display:none">
 <table border="1">
 <tr>
 <td></td>
 <td colspan="1">Supported Version Ranges</td>
 </tr>
 <tr>
 <td>switch_device_tag</td>
 <td><code class="docutils literal notranslate">v6.0.0 -> 7.4.4 </code></td>
 </tr>
 </table>
 </div>
 </li>
        <li> <span class="li-head">switch_dhcp_opt43_key</span> - DHCP option43 key. <span class="li-normal">type: str</span>
 <a id='label554' href="javascript:ContentClick('label555', 'label554');" onmouseover="ContentPreview('label555');" onmouseout="ContentUnpreview('label555');" title="click to collapse or expand..."> more... </a>
 <div id="label555" style="display:none">
 <table border="1">
 <tr>
 <td></td>
 <td colspan="1">Supported Version Ranges</td>
 </tr>
 <tr>
 <td>switch_dhcp_opt43_key</td>
 <td><code class="docutils literal notranslate">v6.4.0 -> 7.4.4 </code></td>
 </tr>
 </table>
 </div>
 </li>
        <li> <span class="li-head">switch_id</span> - Managed-switch name. <span class="li-normal">type: str</span> <span class="li-required">required: true</span>
 <a id='label556' href="javascript:ContentClick('label557', 'label556');" onmouseover="ContentPreview('label557');" onmouseout="ContentUnpreview('label557');" title="click to collapse or expand..."> more... </a>
 <div id="label557" style="display:none">
 <table border="1">
 <tr>
 <td></td>
 <td colspan="1">Supported Version Ranges</td>
 </tr>
 <tr>
 <td>switch_id</td>
 <td><code class="docutils literal notranslate">v6.0.0 -> 7.4.4 </code></td>
 </tr>
 </table>
 </div>
 </li>
        <li> <span class="li-head">switch_log</span> - Configuration method to edit FortiSwitch logging settings (logs are transferred to and inserted into the FortiGate event log). <span class="li-normal">type: dict</span>
 <a id='label558' href="javascript:ContentClick('label559', 'label558');" onmouseover="ContentPreview('label559');" onmouseout="ContentUnpreview('label559');" title="click to collapse or expand..."> more... </a>
 <div id="label559" style="display:none">
 <table border="1">
 <tr>
 <td></td><td colspan="1">Supported Version Ranges</td>
 </tr>
 <tr>
 <td>switch_log</td>
 <td><code class="docutils literal notranslate">v6.0.0 -> 7.4.4 </code></td>
 </tr>
 </table>
 </div>
 </li>
            <ul class="ul-self">
            <li> <span class="li-head">local_override</span> - Enable to configure local logging settings that override global logging settings. <span class="li-normal">type: str</span> <span class="li-normal">choices: enable, disable</span>
 <a id='label560' href="javascript:ContentClick('label561', 'label560');" onmouseover="ContentPreview('label561');" onmouseout="ContentUnpreview('label561');" title="click to collapse or expand..."> more... </a>
 <div id="label561" style="display:none">
 <table border="1">
 <tr>
 <td></td>
 <td colspan="1">Supported Version Ranges</td>
 </tr>
 <tr>
 <td>local_override</td>
 <td><code class="docutils literal notranslate">v6.0.0 -> 7.4.4 </code></td>
 </tr>
 <tr>
 <td>[enable]</td>
 <td><code class="docutils literal notranslate">v6.0.0 -> 7.4.4</code></td>
 <tr>
 <td>[disable]</td>
 <td><code class="docutils literal notranslate">v6.0.0 -> 7.4.4</code></td>
 </table>
 </div>
 </li>
            <li> <span class="li-head">severity</span> - Severity of FortiSwitch logs that are added to the FortiGate event log. <span class="li-normal">type: str</span> <span class="li-normal">choices: emergency, alert, critical, error, warning, notification, information, debug</span>
 <a id='label562' href="javascript:ContentClick('label563', 'label562');" onmouseover="ContentPreview('label563');" onmouseout="ContentUnpreview('label563');" title="click to collapse or expand..."> more... </a>
 <div id="label563" style="display:none">
 <table border="1">
 <tr>
 <td></td>
 <td colspan="1">Supported Version Ranges</td>
 </tr>
 <tr>
 <td>severity</td>
 <td><code class="docutils literal notranslate">v6.0.0 -> 7.4.4 </code></td>
 </tr>
 <tr>
 <td>[emergency]</td>
 <td><code class="docutils literal notranslate">v6.0.0 -> 7.4.4</code></td>
 <tr>
 <td>[alert]</td>
 <td><code class="docutils literal notranslate">v6.0.0 -> 7.4.4</code></td>
 <tr>
 <td>[critical]</td>
 <td><code class="docutils literal notranslate">v6.0.0 -> 7.4.4</code></td>
 <tr>
 <td>[error]</td>
 <td><code class="docutils literal notranslate">v6.0.0 -> 7.4.4</code></td>
 <tr>
 <td>[warning]</td>
 <td><code class="docutils literal notranslate">v6.0.0 -> 7.4.4</code></td>
 <tr>
 <td>[notification]</td>
 <td><code class="docutils literal notranslate">v6.0.0 -> 7.4.4</code></td>
 <tr>
 <td>[information]</td>
 <td><code class="docutils literal notranslate">v6.0.0 -> 7.4.4</code></td>
 <tr>
 <td>[debug]</td>
 <td><code class="docutils literal notranslate">v6.0.0 -> 7.4.4</code></td>
 </table>
 </div>
 </li>
            <li> <span class="li-head">status</span> - Enable/disable adding FortiSwitch logs to the FortiGate event log. <span class="li-normal">type: str</span> <span class="li-normal">choices: enable, disable</span>
 <a id='label564' href="javascript:ContentClick('label565', 'label564');" onmouseover="ContentPreview('label565');" onmouseout="ContentUnpreview('label565');" title="click to collapse or expand..."> more... </a>
 <div id="label565" style="display:none">
 <table border="1">
 <tr>
 <td></td>
 <td colspan="1">Supported Version Ranges</td>
 </tr>
 <tr>
 <td>status</td>
 <td><code class="docutils literal notranslate">v6.0.0 -> 7.4.4 </code></td>
 </tr>
 <tr>
 <td>[enable]</td>
 <td><code class="docutils literal notranslate">v6.0.0 -> 7.4.4</code></td>
 <tr>
 <td>[disable]</td>
 <td><code class="docutils literal notranslate">v6.0.0 -> 7.4.4</code></td>
 </table>
 </div>
 </li>
            </ul>
        <li> <span class="li-head">switch_profile</span> - FortiSwitch profile. Source switch-controller.switch-profile.name. <span class="li-normal">type: str</span>
 <a id='label566' href="javascript:ContentClick('label567', 'label566');" onmouseover="ContentPreview('label567');" onmouseout="ContentUnpreview('label567');" title="click to collapse or expand..."> more... </a>
 <div id="label567" style="display:none">
 <table border="1">
 <tr>
 <td></td>
 <td colspan="1">Supported Version Ranges</td>
 </tr>
 <tr>
 <td>switch_profile</td>
 <td><code class="docutils literal notranslate">v6.0.0 -> 7.4.4 </code></td>
 </tr>
 </table>
 </div>
 </li>
        <li> <span class="li-head">switch_stp_settings</span> - Configure spanning tree protocol (STP). <span class="li-normal">type: dict</span>
 <a id='label568' href="javascript:ContentClick('label569', 'label568');" onmouseover="ContentPreview('label569');" onmouseout="ContentUnpreview('label569');" title="click to collapse or expand..."> more... </a>
 <div id="label569" style="display:none">
 <table border="1">
 <tr>
 <td></td><td colspan="2">Supported Version Ranges</td>
 </tr>
 <tr>
 <td>switch_stp_settings</td>
 <td><code class="docutils literal notranslate">v6.0.0 -> v6.0.11 </code></td>
 <td><code class="docutils literal notranslate">v6.2.3 -> v6.2.3 </code></td>
 </tr>
 </table>
 </div>
 </li>
            <ul class="ul-self">
            <li> <span class="li-head">status</span> - Enable/disable STP. <span class="li-normal">type: str</span> <span class="li-normal">choices: enable, disable</span>
 <a id='label570' href="javascript:ContentClick('label571', 'label570');" onmouseover="ContentPreview('label571');" onmouseout="ContentUnpreview('label571');" title="click to collapse or expand..."> more... </a>
 <div id="label571" style="display:none">
 <table border="1">
 <tr>
 <td></td>
 <td colspan="2">Supported Version Ranges</td>
 </tr>
 <tr>
 <td>status</td>
 <td><code class="docutils literal notranslate">v6.0.0 -> v6.0.11 </code></td>
 <td><code class="docutils literal notranslate">v6.2.3 -> v6.2.3 </code></td>
 </tr>
 <tr>
 <td>[enable]</td>
 <td><code class="docutils literal notranslate">v6.0.0 -> v6.0.11</code></td>
 <tr>
 <td>[disable]</td>
 <td><code class="docutils literal notranslate">v6.0.0 -> v6.0.11</code></td>
 </table>
 </div>
 </li>
            </ul>
        <li> <span class="li-head">tdr_supported</span> - TDR supported. <span class="li-normal">type: str</span>
 <a id='label572' href="javascript:ContentClick('label573', 'label572');" onmouseover="ContentPreview('label573');" onmouseout="ContentUnpreview('label573');" title="click to collapse or expand..."> more... </a>
 <div id="label573" style="display:none">
 <table border="1">
 <tr>
 <td></td>
 <td colspan="2">Supported Version Ranges</td>
 </tr>
 <tr>
 <td>tdr_supported</td>
 <td><code class="docutils literal notranslate">v6.4.4 -> v7.0.5 </code></td>
 <td><code class="docutils literal notranslate">v7.2.0 -> v7.2.0 </code></td>
 </tr>
 </table>
 </div>
 </li>
        <li> <span class="li-head">type</span> - Indication of switch type, physical or virtual. <span class="li-normal">type: str</span> <span class="li-normal">choices: virtual, physical</span>
 <a id='label574' href="javascript:ContentClick('label575', 'label574');" onmouseover="ContentPreview('label575');" onmouseout="ContentUnpreview('label575');" title="click to collapse or expand..."> more... </a>
 <div id="label575" style="display:none">
 <table border="1">
 <tr>
 <td></td>
 <td colspan="1">Supported Version Ranges</td>
 </tr>
 <tr>
 <td>type</td>
 <td><code class="docutils literal notranslate">v6.0.0 -> 7.4.4 </code></td>
 </tr>
 <tr>
 <td>[virtual]</td>
 <td><code class="docutils literal notranslate">v6.0.0 -> 7.4.4</code></td>
 <tr>
 <td>[physical]</td>
 <td><code class="docutils literal notranslate">v6.0.0 -> 7.4.4</code></td>
 </table>
 </div>
 </li>
        <li> <span class="li-head">version</span> - FortiSwitch version. <span class="li-normal">type: int</span>
 <a id='label576' href="javascript:ContentClick('label577', 'label576');" onmouseover="ContentPreview('label577');" onmouseout="ContentUnpreview('label577');" title="click to collapse or expand..."> more... </a>
 <div id="label577" style="display:none">
 <table border="1">
 <tr>
 <td></td>
 <td colspan="1">Supported Version Ranges</td>
 </tr>
 <tr>
 <td>version</td>
 <td><code class="docutils literal notranslate">v6.0.0 -> 7.4.4 </code></td>
 </tr>
 </table>
 </div>
 </li>
        <li> <span class="li-head">vlan</span> - Configure VLAN assignment priority. <span class="li-normal">type: list</span> <span style="font-family:'Courier New'" class="li-required">member_path: vlan:vlan_name</span>
 <a id='label578' href="javascript:ContentClick('label579', 'label578');" onmouseover="ContentPreview('label579');" onmouseout="ContentUnpreview('label579');" title="click to collapse or expand..."> more... </a>
 <div id="label579" style="display:none">
 <table border="1">
 <tr>
 <td></td><td colspan="1">Supported Version Ranges</td>
 </tr>
 <tr>
 <td>vlan</td>
 <td><code class="docutils literal notranslate">v7.4.2 -> 7.4.4 </code></td>
 </tr>
 </table>
 </div>
 </li>
            <ul class="ul-self">
            <li> <span class="li-head">assignment_priority</span> - 802.1x Radius (Tunnel-Private-Group-Id) VLANID assign-by-name priority. A smaller value has a higher priority. <span class="li-normal">type: int</span>
 <a id='label580' href="javascript:ContentClick('label581', 'label580');" onmouseover="ContentPreview('label581');" onmouseout="ContentUnpreview('label581');" title="click to collapse or expand..."> more... </a>
 <div id="label581" style="display:none">
 <table border="1">
 <tr>
 <td></td>
 <td colspan="1">Supported Version Ranges</td>
 </tr>
 <tr>
 <td>assignment_priority</td>
 <td><code class="docutils literal notranslate">v7.4.2 -> 7.4.4 </code></td>
 </tr>
 </table>
 </div>
 </li>
            <li> <span class="li-head">vlan_name</span> - VLAN name. Source system.interface.name. <span class="li-normal">type: str</span> <span class="li-required">required: true</span>
 <a id='label582' href="javascript:ContentClick('label583', 'label582');" onmouseover="ContentPreview('label583');" onmouseout="ContentUnpreview('label583');" title="click to collapse or expand..."> more... </a>
 <div id="label583" style="display:none">
 <table border="1">
 <tr>
 <td></td>
 <td colspan="1">Supported Version Ranges</td>
 </tr>
 <tr>
 <td>vlan_name</td>
 <td><code class="docutils literal notranslate">v7.4.2 -> 7.4.4 </code></td>
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

   - The module supports check_mode.



Examples
--------

.. code-block:: yaml+jinja
    
    - name: Configure FortiSwitch devices that are managed by this FortiGate.
      fortinet.fortios.fortios_switch_controller_managed_switch:
          vdom: "{{ vdom }}"
          state: "present"
          access_token: "<your_own_value>"
          switch_controller_managed_switch:
              settings_802_1X:
                  link_down_auth: "set-unauth"
                  local_override: "enable"
                  mab_reauth: "disable"
                  mac_called_station_delimiter: "colon"
                  mac_calling_station_delimiter: "colon"
                  mac_case: "lowercase"
                  mac_password_delimiter: "colon"
                  mac_username_delimiter: "colon"
                  max_reauth_attempt: "3"
                  reauth_period: "60"
                  tx_period: "30"
              access_profile: "<your_own_value> (source switch-controller.security-policy.local-access.name)"
              custom_command:
                  -
                      command_entry: "<your_own_value>"
                      command_name: "<your_own_value> (source switch-controller.custom-command.command-name)"
              delayed_restart_trigger: "0"
              description: "<your_own_value>"
              dhcp_server_access_list: "global"
              dhcp_snooping_static_client:
                  -
                      ip: "<your_own_value>"
                      mac: "<your_own_value>"
                      name: "default_name_25"
                      port: "<your_own_value>"
                      vlan: "<your_own_value> (source system.interface.name)"
              directly_connected: "0"
              dynamic_capability: "<your_own_value>"
              dynamically_discovered: "0"
              firmware_provision: "enable"
              firmware_provision_latest: "disable"
              firmware_provision_version: "<your_own_value>"
              flow_identity: "<your_own_value>"
              fsw_wan1_admin: "discovered"
              fsw_wan1_peer: "<your_own_value> (source system.interface.name)"
              fsw_wan2_admin: "discovered"
              fsw_wan2_peer: "<your_own_value>"
              igmp_snooping:
                  aging_time: "300"
                  flood_unknown_multicast: "enable"
                  local_override: "enable"
                  vlans:
                      -
                          proxy: "disable"
                          querier: "disable"
                          querier_addr: "<your_own_value>"
                          version: "2"
                          vlan_name: "<your_own_value> (source system.interface.name)"
              ip_source_guard:
                  -
                      binding_entry:
                          -
                              entry_name: "<your_own_value>"
                              ip: "<your_own_value>"
                              mac: "<your_own_value>"
                      description: "<your_own_value>"
                      port: "<your_own_value>"
              l3_discovered: "0"
              max_allowed_trunk_members: "0"
              mclag_igmp_snooping_aware: "enable"
              mgmt_mode: "0"
              mirror:
                  -
                      dst: "<your_own_value>"
                      name: "default_name_62"
                      src_egress:
                          -
                              name: "default_name_64"
                      src_ingress:
                          -
                              name: "default_name_66"
                      status: "active"
                      switching_packet: "enable"
              name: "default_name_69"
              override_snmp_community: "enable"
              override_snmp_sysinfo: "disable"
              override_snmp_trap_threshold: "enable"
              override_snmp_user: "enable"
              owner_vdom: "<your_own_value>"
              poe_detection_type: "0"
              poe_lldp_detection: "enable"
              poe_pre_standard_detection: "enable"
              ports:
                  -
                      access_mode: "dynamic"
                      acl_group:
                          -
                              name: "default_name_81 (source switch-controller.acl.group.name)"
                      aggregator_mode: "bandwidth"
                      allow_arp_monitor: "disable"
                      allowed_vlans:
                          -
                              vlan_name: "<your_own_value> (source system.interface.name)"
                      allowed_vlans_all: "enable"
                      arp_inspection_trust: "untrusted"
                      bundle: "enable"
                      description: "<your_own_value>"
                      dhcp_snoop_option82_override:
                          -
                              circuit_id: "<your_own_value>"
                              remote_id: "<your_own_value>"
                              vlan_name: "<your_own_value> (source system.interface.name)"
                      dhcp_snoop_option82_trust: "enable"
                      dhcp_snooping: "untrusted"
                      discard_mode: "none"
                      edge_port: "enable"
                      export_tags:
                          -
                              tag_name: "<your_own_value> (source switch-controller.switch-interface-tag.name)"
                      export_to: "<your_own_value> (source system.vdom.name)"
                      export_to_pool: "<your_own_value> (source switch-controller.virtual-port-pool.name)"
                      export_to_pool_flag: "0"
                      fallback_port: "<your_own_value>"
                      fec_capable: "0"
                      fec_state: "disabled"
                      fgt_peer_device_name: "<your_own_value>"
                      fgt_peer_port_name: "<your_own_value>"
                      fiber_port: "0"
                      flags: "0"
                      flap_duration: "30"
                      flap_rate: "5"
                      flap_timeout: "0"
                      flapguard: "enable"
                      flow_control: "disable"
                      fortilink_port: "0"
                      fortiswitch_acls:
                          -
                              id: "117"
                      igmp_snooping: "enable"
                      igmp_snooping_flood_reports: "enable"
                      igmps_flood_reports: "enable"
                      igmps_flood_traffic: "enable"
                      interface_tags:
                          -
                              tag_name: "<your_own_value> (source switch-controller.switch-interface-tag.name)"
                      ip_source_guard: "disable"
                      isl_local_trunk_name: "<your_own_value>"
                      isl_peer_device_name: "<your_own_value>"
                      isl_peer_port_name: "<your_own_value>"
                      lacp_speed: "slow"
                      learning_limit: "0"
                      lldp_profile: "<your_own_value> (source switch-controller.lldp-profile.name)"
                      lldp_status: "disable"
                      loop_guard: "enabled"
                      loop_guard_timeout: "45"
                      mac_addr: "<your_own_value>"
                      matched_dpp_intf_tags: "<your_own_value>"
                      matched_dpp_policy: "<your_own_value>"
                      max_bundle: "24"
                      mcast_snooping_flood_traffic: "enable"
                      mclag: "enable"
                      mclag_icl_port: "0"
                      media_type: "<your_own_value>"
                      member_withdrawal_behavior: "forward"
                      members:
                          -
                              member_name: "<your_own_value>"
                      min_bundle: "1"
                      mode: "static"
                      p2p_port: "0"
                      packet_sample_rate: "512"
                      packet_sampler: "enabled"
                      pause_meter: "0"
                      pause_meter_resume: "75%"
                      poe_capable: "0"
                      poe_max_power: "<your_own_value>"
                      poe_mode_bt_cabable: "0"
                      poe_port_mode: "ieee802-3af"
                      poe_port_power: "normal"
                      poe_port_priority: "critical-priority"
                      poe_pre_standard_detection: "enable"
                      poe_standard: "<your_own_value>"
                      poe_status: "enable"
                      port_name: "<your_own_value>"
                      port_number: "0"
                      port_owner: "<your_own_value>"
                      port_policy: "<your_own_value> (source switch-controller.dynamic-port-policy.name)"
                      port_prefix_type: "0"
                      port_security_policy: "<your_own_value> (source switch-controller.security-policy.802-1X.name)"
                      port_selection_criteria: "src-mac"
                      ptp_policy: "<your_own_value> (source switch-controller.ptp.interface-policy.name)"
                      ptp_status: "disable"
                      qos_policy: "<your_own_value> (source switch-controller.qos.qos-policy.name)"
                      rpvst_port: "disabled"
                      sample_direction: "tx"
                      sflow_counter_interval: "0"
                      sflow_sample_rate: "49999"
                      sflow_sampler: "enabled"
                      speed: "10half"
                      speed_mask: "2147483647"
                      stacking_port: "0"
                      status: "up"
                      sticky_mac: "enable"
                      storm_control_policy: "<your_own_value> (source switch-controller.storm-control-policy.name)"
                      stp_bpdu_guard: "enabled"
                      stp_bpdu_guard_timeout: "5"
                      stp_root_guard: "enabled"
                      stp_state: "enabled"
                      switch_id: "<your_own_value>"
                      type: "physical"
                      untagged_vlans:
                          -
                              vlan_name: "<your_own_value> (source system.interface.name)"
                      virtual_port: "0"
                      vlan: "<your_own_value> (source system.interface.name)"
              pre_provisioned: "0"
              ptp_profile: "<your_own_value> (source switch-controller.ptp.profile.name)"
              ptp_status: "disable"
              purdue_level: "1"
              qos_drop_policy: "taildrop"
              qos_red_probability: "12"
              radius_nas_ip: "<your_own_value>"
              radius_nas_ip_override: "disable"
              remote_log:
                  -
                      csv: "enable"
                      facility: "kernel"
                      name: "default_name_203"
                      port: "514"
                      server: "192.168.100.40"
                      severity: "emergency"
                      status: "enable"
              route_offload: "disable"
              route_offload_mclag: "disable"
              route_offload_router:
                  -
                      router_ip: "<your_own_value>"
                      vlan_name: "<your_own_value> (source system.interface.name)"
              sn: "<your_own_value>"
              snmp_community:
                  -
                      events: "cpu-high"
                      hosts:
                          -
                              id: "217"
                              ip: "<your_own_value>"
                      id: "219"
                      name: "default_name_220"
                      query_v1_port: "161"
                      query_v1_status: "disable"
                      query_v2c_port: "161"
                      query_v2c_status: "disable"
                      status: "disable"
                      trap_v1_lport: "162"
                      trap_v1_rport: "162"
                      trap_v1_status: "disable"
                      trap_v2c_lport: "162"
                      trap_v2c_rport: "162"
                      trap_v2c_status: "disable"
              snmp_sysinfo:
                  contact_info: "<your_own_value>"
                  description: "<your_own_value>"
                  engine_id: "<your_own_value>"
                  location: "<your_own_value>"
                  status: "disable"
              snmp_trap_threshold:
                  trap_high_cpu_threshold: "80"
                  trap_log_full_threshold: "90"
                  trap_low_memory_threshold: "80"
              snmp_user:
                  -
                      auth_proto: "md5"
                      auth_pwd: "<your_own_value>"
                      name: "default_name_245"
                      priv_proto: "aes128"
                      priv_pwd: "<your_own_value>"
                      queries: "disable"
                      query_port: "161"
                      security_level: "no-auth-no-priv"
              staged_image_version: "<your_own_value>"
              static_mac:
                  -
                      description: "<your_own_value>"
                      id: "254"
                      interface: "<your_own_value>"
                      mac: "<your_own_value>"
                      type: "static"
                      vlan: "<your_own_value> (source system.interface.name)"
              storm_control:
                  broadcast: "enable"
                  local_override: "enable"
                  rate: "500"
                  unknown_multicast: "enable"
                  unknown_unicast: "enable"
              stp_instance:
                  -
                      id: "266"
                      priority: "0"
              stp_settings:
                  forward_time: "15"
                  hello_time: "2"
                  local_override: "enable"
                  max_age: "20"
                  max_hops: "20"
                  name: "default_name_274"
                  pending_timer: "4"
                  revision: "0"
                  status: "enable"
              switch_device_tag: "<your_own_value>"
              switch_dhcp_opt43_key: "<your_own_value>"
              switch_id: "<your_own_value>"
              switch_log:
                  local_override: "enable"
                  severity: "emergency"
                  status: "enable"
              switch_profile: "<your_own_value> (source switch-controller.switch-profile.name)"
              switch_stp_settings:
                  status: "enable"
              tdr_supported: "<your_own_value>"
              type: "virtual"
              version: "0"
              vlan:
                  -
                      assignment_priority: "128"
                      vlan_name: "<your_own_value> (source system.interface.name)"


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
