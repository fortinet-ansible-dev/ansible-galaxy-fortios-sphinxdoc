:source: fortios_system_central_management.py

:orphan:

.. fortios_system_central_management:

fortios_system_central_management -- Configure central management in Fortinet's FortiOS and FortiGate.
++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++

.. versionadded:: 2.0.0

.. contents::
   :local:
   :depth: 1


Synopsis
--------
- This module is able to configure a FortiGate or FortiOS (FOS) device by allowing the user to set and modify system feature and central_management category. Examples include all parameters and values need to be adjusted to datasources before usage. Tested with FOS v6.0.0



Requirements
------------
The below requirements are needed on the host that executes this module.

- ansible>=2.15


Tips
----
Using member operation to add an element to an existing object.

FortiOS Version Compatibility
-----------------------------
Supported Version Ranges: v6.0.0 -> 7.4.3



Parameters
----------


.. raw:: html

    <ul>
    <li> <span class="li-head">access_token</span> - Token-based authentication. Generated from GUI of Fortigate. <span class="li-normal">type: str</span> <span class="li-required">required: false</span> </li>
    <li> <span class="li-head">enable_log</span> - Enable/Disable logging for task. <span class="li-normal">type: bool</span> <span class="li-required">required: false</span> <span class="li-normal">default: False</span> </li>
    <li> <span class="li-head">vdom</span> - Virtual domain, among those defined previously. A vdom is a virtual instance of the FortiGate that can be configured and used as a different unit. <span class="li-normal">type: str</span> <span class="li-normal">default: root</span> </li>
    <li> <span class="li-head">member_path</span> - Member attribute path to operate on. <span class="li-normal">type: str</span> </li>
    <li> <span class="li-head">member_state</span> - Add or delete a member under specified attribute path. <span class="li-normal">type: str</span> <span class="li-normal">choices: present, absent</span> </li>
    <li> <span class="li-head">system_central_management</span> - Configure central management. <span class="li-normal">type: dict</span>
 <a id='label0' href="javascript:ContentClick('label1', 'label0');" onmouseover="ContentPreview('label1');" onmouseout="ContentUnpreview('label1');" title="click to collapse or expand..."> more... </a>
 <div id="label1" style="display:none">
 <table border="1">
 <tr>
 <td></td><td colspan="1">Supported Version Ranges</td>
 </tr>
 <tr>
 <td>system_central_management</td>
 <td><code class="docutils literal notranslate">v6.0.0 -> 7.4.3 </code></td>
 </tr>
 </table>
 </div>
 </li>
        <ul class="ul-self">
        <li> <span class="li-head">allow_monitor</span> - Enable/disable allowing the central management server to remotely monitor this FortiGate unit. <span class="li-normal">type: str</span> <span class="li-normal">choices: enable, disable</span>
 <a id='label2' href="javascript:ContentClick('label3', 'label2');" onmouseover="ContentPreview('label3');" onmouseout="ContentUnpreview('label3');" title="click to collapse or expand..."> more... </a>
 <div id="label3" style="display:none">
 <table border="1">
 <tr>
 <td></td>
 <td colspan="1">Supported Version Ranges</td>
 </tr>
 <tr>
 <td>allow_monitor</td>
 <td><code class="docutils literal notranslate">v6.0.0 -> 7.4.3 </code></td>
 </tr>
 <tr>
 <td>[enable]</td>
 <td><code class="docutils literal notranslate">v6.0.0 -> 7.4.3</code></td>
 <tr>
 <td>[disable]</td>
 <td><code class="docutils literal notranslate">v6.0.0 -> 7.4.3</code></td>
 </table>
 </div>
 </li>
        <li> <span class="li-head">allow_push_configuration</span> - Enable/disable allowing the central management server to push configuration changes to this FortiGate. <span class="li-normal">type: str</span> <span class="li-normal">choices: enable, disable</span>
 <a id='label4' href="javascript:ContentClick('label5', 'label4');" onmouseover="ContentPreview('label5');" onmouseout="ContentUnpreview('label5');" title="click to collapse or expand..."> more... </a>
 <div id="label5" style="display:none">
 <table border="1">
 <tr>
 <td></td>
 <td colspan="1">Supported Version Ranges</td>
 </tr>
 <tr>
 <td>allow_push_configuration</td>
 <td><code class="docutils literal notranslate">v6.0.0 -> 7.4.3 </code></td>
 </tr>
 <tr>
 <td>[enable]</td>
 <td><code class="docutils literal notranslate">v6.0.0 -> 7.4.3</code></td>
 <tr>
 <td>[disable]</td>
 <td><code class="docutils literal notranslate">v6.0.0 -> 7.4.3</code></td>
 </table>
 </div>
 </li>
        <li> <span class="li-head">allow_push_firmware</span> - Enable/disable allowing the central management server to push firmware updates to this FortiGate. <span class="li-normal">type: str</span> <span class="li-normal">choices: enable, disable</span>
 <a id='label6' href="javascript:ContentClick('label7', 'label6');" onmouseover="ContentPreview('label7');" onmouseout="ContentUnpreview('label7');" title="click to collapse or expand..."> more... </a>
 <div id="label7" style="display:none">
 <table border="1">
 <tr>
 <td></td>
 <td colspan="1">Supported Version Ranges</td>
 </tr>
 <tr>
 <td>allow_push_firmware</td>
 <td><code class="docutils literal notranslate">v6.0.0 -> 7.4.3 </code></td>
 </tr>
 <tr>
 <td>[enable]</td>
 <td><code class="docutils literal notranslate">v6.0.0 -> 7.4.3</code></td>
 <tr>
 <td>[disable]</td>
 <td><code class="docutils literal notranslate">v6.0.0 -> 7.4.3</code></td>
 </table>
 </div>
 </li>
        <li> <span class="li-head">allow_remote_firmware_upgrade</span> - Enable/disable remotely upgrading the firmware on this FortiGate from the central management server. <span class="li-normal">type: str</span> <span class="li-normal">choices: enable, disable</span>
 <a id='label8' href="javascript:ContentClick('label9', 'label8');" onmouseover="ContentPreview('label9');" onmouseout="ContentUnpreview('label9');" title="click to collapse or expand..."> more... </a>
 <div id="label9" style="display:none">
 <table border="1">
 <tr>
 <td></td>
 <td colspan="1">Supported Version Ranges</td>
 </tr>
 <tr>
 <td>allow_remote_firmware_upgrade</td>
 <td><code class="docutils literal notranslate">v6.0.0 -> 7.4.3 </code></td>
 </tr>
 <tr>
 <td>[enable]</td>
 <td><code class="docutils literal notranslate">v6.0.0 -> 7.4.3</code></td>
 <tr>
 <td>[disable]</td>
 <td><code class="docutils literal notranslate">v6.0.0 -> 7.4.3</code></td>
 </table>
 </div>
 </li>
        <li> <span class="li-head">ca_cert</span> - CA certificate to be used by FGFM protocol. <span class="li-normal">type: str</span>
 <a id='label10' href="javascript:ContentClick('label11', 'label10');" onmouseover="ContentPreview('label11');" onmouseout="ContentUnpreview('label11');" title="click to collapse or expand..."> more... </a>
 <div id="label11" style="display:none">
 <table border="1">
 <tr>
 <td></td>
 <td colspan="1">Supported Version Ranges</td>
 </tr>
 <tr>
 <td>ca_cert</td>
 <td><code class="docutils literal notranslate">v6.2.0 -> 7.4.3 </code></td>
 </tr>
 </table>
 </div>
 </li>
        <li> <span class="li-head">enc_algorithm</span> - Encryption strength for communications between the FortiGate and central management. <span class="li-normal">type: str</span> <span class="li-normal">choices: default, high, low</span>
 <a id='label12' href="javascript:ContentClick('label13', 'label12');" onmouseover="ContentPreview('label13');" onmouseout="ContentUnpreview('label13');" title="click to collapse or expand..."> more... </a>
 <div id="label13" style="display:none">
 <table border="1">
 <tr>
 <td></td>
 <td colspan="1">Supported Version Ranges</td>
 </tr>
 <tr>
 <td>enc_algorithm</td>
 <td><code class="docutils literal notranslate">v6.0.0 -> 7.4.3 </code></td>
 </tr>
 <tr>
 <td>[default]</td>
 <td><code class="docutils literal notranslate">v6.0.0 -> 7.4.3</code></td>
 <tr>
 <td>[high]</td>
 <td><code class="docutils literal notranslate">v6.0.0 -> 7.4.3</code></td>
 <tr>
 <td>[low]</td>
 <td><code class="docutils literal notranslate">v6.0.0 -> 7.4.3</code></td>
 </table>
 </div>
 </li>
        <li> <span class="li-head">fmg</span> - IP address or FQDN of the FortiManager. <span class="li-normal">type: str</span>
 <a id='label14' href="javascript:ContentClick('label15', 'label14');" onmouseover="ContentPreview('label15');" onmouseout="ContentUnpreview('label15');" title="click to collapse or expand..."> more... </a>
 <div id="label15" style="display:none">
 <table border="1">
 <tr>
 <td></td>
 <td colspan="1">Supported Version Ranges</td>
 </tr>
 <tr>
 <td>fmg</td>
 <td><code class="docutils literal notranslate">v6.0.0 -> 7.4.3 </code></td>
 </tr>
 </table>
 </div>
 </li>
        <li> <span class="li-head">fmg_source_ip</span> - IPv4 source address that this FortiGate uses when communicating with FortiManager. <span class="li-normal">type: str</span>
 <a id='label16' href="javascript:ContentClick('label17', 'label16');" onmouseover="ContentPreview('label17');" onmouseout="ContentUnpreview('label17');" title="click to collapse or expand..."> more... </a>
 <div id="label17" style="display:none">
 <table border="1">
 <tr>
 <td></td>
 <td colspan="1">Supported Version Ranges</td>
 </tr>
 <tr>
 <td>fmg_source_ip</td>
 <td><code class="docutils literal notranslate">v6.0.0 -> 7.4.3 </code></td>
 </tr>
 </table>
 </div>
 </li>
        <li> <span class="li-head">fmg_source_ip6</span> - IPv6 source address that this FortiGate uses when communicating with FortiManager. <span class="li-normal">type: str</span>
 <a id='label18' href="javascript:ContentClick('label19', 'label18');" onmouseover="ContentPreview('label19');" onmouseout="ContentUnpreview('label19');" title="click to collapse or expand..."> more... </a>
 <div id="label19" style="display:none">
 <table border="1">
 <tr>
 <td></td>
 <td colspan="1">Supported Version Ranges</td>
 </tr>
 <tr>
 <td>fmg_source_ip6</td>
 <td><code class="docutils literal notranslate">v6.0.0 -> 7.4.3 </code></td>
 </tr>
 </table>
 </div>
 </li>
        <li> <span class="li-head">fmg_update_port</span> - Port used to communicate with FortiManager that is acting as a FortiGuard update server. <span class="li-normal">type: str</span> <span class="li-normal">choices: 8890, 443</span>
 <a id='label20' href="javascript:ContentClick('label21', 'label20');" onmouseover="ContentPreview('label21');" onmouseout="ContentUnpreview('label21');" title="click to collapse or expand..."> more... </a>
 <div id="label21" style="display:none">
 <table border="1">
 <tr>
 <td></td>
 <td colspan="1">Supported Version Ranges</td>
 </tr>
 <tr>
 <td>fmg_update_port</td>
 <td><code class="docutils literal notranslate">v6.2.0 -> 7.4.3 </code></td>
 </tr>
 <tr>
 <td>[8890]</td>
 <td><code class="docutils literal notranslate">v6.2.0 -> 7.4.3</code></td>
 <tr>
 <td>[443]</td>
 <td><code class="docutils literal notranslate">v6.2.0 -> 7.4.3</code></td>
 </table>
 </div>
 </li>
        <li> <span class="li-head">fortigate_cloud_sso_default_profile</span> - Override access profile. Source system.accprofile.name. <span class="li-normal">type: str</span>
 <a id='label22' href="javascript:ContentClick('label23', 'label22');" onmouseover="ContentPreview('label23');" onmouseout="ContentUnpreview('label23');" title="click to collapse or expand..."> more... </a>
 <div id="label23" style="display:none">
 <table border="1">
 <tr>
 <td></td>
 <td colspan="1">Supported Version Ranges</td>
 </tr>
 <tr>
 <td>fortigate_cloud_sso_default_profile</td>
 <td><code class="docutils literal notranslate">v7.2.4 -> 7.4.3 </code></td>
 </tr>
 </table>
 </div>
 </li>
        <li> <span class="li-head">include_default_servers</span> - Enable/disable inclusion of public FortiGuard servers in the override server list. <span class="li-normal">type: str</span> <span class="li-normal">choices: enable, disable</span>
 <a id='label24' href="javascript:ContentClick('label25', 'label24');" onmouseover="ContentPreview('label25');" onmouseout="ContentUnpreview('label25');" title="click to collapse or expand..."> more... </a>
 <div id="label25" style="display:none">
 <table border="1">
 <tr>
 <td></td>
 <td colspan="1">Supported Version Ranges</td>
 </tr>
 <tr>
 <td>include_default_servers</td>
 <td><code class="docutils literal notranslate">v6.0.0 -> 7.4.3 </code></td>
 </tr>
 <tr>
 <td>[enable]</td>
 <td><code class="docutils literal notranslate">v6.0.0 -> 7.4.3</code></td>
 <tr>
 <td>[disable]</td>
 <td><code class="docutils literal notranslate">v6.0.0 -> 7.4.3</code></td>
 </table>
 </div>
 </li>
        <li> <span class="li-head">interface</span> - Specify outgoing interface to reach server. Source system.interface.name. <span class="li-normal">type: str</span>
 <a id='label26' href="javascript:ContentClick('label27', 'label26');" onmouseover="ContentPreview('label27');" onmouseout="ContentUnpreview('label27');" title="click to collapse or expand..."> more... </a>
 <div id="label27" style="display:none">
 <table border="1">
 <tr>
 <td></td>
 <td colspan="2">Supported Version Ranges</td>
 </tr>
 <tr>
 <td>interface</td>
 <td><code class="docutils literal notranslate">v6.2.0 -> v6.2.0 </code></td>
 <td><code class="docutils literal notranslate">v6.2.5 -> 7.4.3 </code></td>
 </tr>
 </table>
 </div>
 </li>
        <li> <span class="li-head">interface_select_method</span> - Specify how to select outgoing interface to reach server. <span class="li-normal">type: str</span> <span class="li-normal">choices: auto, sdwan, specify</span>
 <a id='label28' href="javascript:ContentClick('label29', 'label28');" onmouseover="ContentPreview('label29');" onmouseout="ContentUnpreview('label29');" title="click to collapse or expand..."> more... </a>
 <div id="label29" style="display:none">
 <table border="1">
 <tr>
 <td></td>
 <td colspan="2">Supported Version Ranges</td>
 </tr>
 <tr>
 <td>interface_select_method</td>
 <td><code class="docutils literal notranslate">v6.2.0 -> v6.2.0 </code></td>
 <td><code class="docutils literal notranslate">v6.2.5 -> 7.4.3 </code></td>
 </tr>
 <tr>
 <td>[auto]</td>
 <td><code class="docutils literal notranslate">v6.2.0 -> v6.2.0</code></td>
 <tr>
 <td>[sdwan]</td>
 <td><code class="docutils literal notranslate">v6.2.0 -> v6.2.0</code></td>
 <tr>
 <td>[specify]</td>
 <td><code class="docutils literal notranslate">v6.2.0 -> v6.2.0</code></td>
 </table>
 </div>
 </li>
        <li> <span class="li-head">local_cert</span> - Certificate to be used by FGFM protocol. <span class="li-normal">type: str</span>
 <a id='label30' href="javascript:ContentClick('label31', 'label30');" onmouseover="ContentPreview('label31');" onmouseout="ContentUnpreview('label31');" title="click to collapse or expand..."> more... </a>
 <div id="label31" style="display:none">
 <table border="1">
 <tr>
 <td></td>
 <td colspan="2">Supported Version Ranges</td>
 </tr>
 <tr>
 <td>local_cert</td>
 <td><code class="docutils literal notranslate">v6.0.0 -> v6.0.0 </code></td>
 <td><code class="docutils literal notranslate">v6.0.11 -> 7.4.3 </code></td>
 </tr>
 </table>
 </div>
 </li>
        <li> <span class="li-head">mode</span> - Central management mode. <span class="li-normal">type: str</span> <span class="li-normal">choices: normal, backup</span>
 <a id='label32' href="javascript:ContentClick('label33', 'label32');" onmouseover="ContentPreview('label33');" onmouseout="ContentUnpreview('label33');" title="click to collapse or expand..."> more... </a>
 <div id="label33" style="display:none">
 <table border="1">
 <tr>
 <td></td>
 <td colspan="1">Supported Version Ranges</td>
 </tr>
 <tr>
 <td>mode</td>
 <td><code class="docutils literal notranslate">v6.0.0 -> 7.4.3 </code></td>
 </tr>
 <tr>
 <td>[normal]</td>
 <td><code class="docutils literal notranslate">v6.0.0 -> 7.4.3</code></td>
 <tr>
 <td>[backup]</td>
 <td><code class="docutils literal notranslate">v6.0.0 -> 7.4.3</code></td>
 </table>
 </div>
 </li>
        <li> <span class="li-head">schedule_config_restore</span> - Enable/disable allowing the central management server to restore the configuration of this FortiGate. <span class="li-normal">type: str</span> <span class="li-normal">choices: enable, disable</span>
 <a id='label34' href="javascript:ContentClick('label35', 'label34');" onmouseover="ContentPreview('label35');" onmouseout="ContentUnpreview('label35');" title="click to collapse or expand..."> more... </a>
 <div id="label35" style="display:none">
 <table border="1">
 <tr>
 <td></td>
 <td colspan="1">Supported Version Ranges</td>
 </tr>
 <tr>
 <td>schedule_config_restore</td>
 <td><code class="docutils literal notranslate">v6.0.0 -> 7.4.3 </code></td>
 </tr>
 <tr>
 <td>[enable]</td>
 <td><code class="docutils literal notranslate">v6.0.0 -> 7.4.3</code></td>
 <tr>
 <td>[disable]</td>
 <td><code class="docutils literal notranslate">v6.0.0 -> 7.4.3</code></td>
 </table>
 </div>
 </li>
        <li> <span class="li-head">schedule_script_restore</span> - Enable/disable allowing the central management server to restore the scripts stored on this FortiGate. <span class="li-normal">type: str</span> <span class="li-normal">choices: enable, disable</span>
 <a id='label36' href="javascript:ContentClick('label37', 'label36');" onmouseover="ContentPreview('label37');" onmouseout="ContentUnpreview('label37');" title="click to collapse or expand..."> more... </a>
 <div id="label37" style="display:none">
 <table border="1">
 <tr>
 <td></td>
 <td colspan="1">Supported Version Ranges</td>
 </tr>
 <tr>
 <td>schedule_script_restore</td>
 <td><code class="docutils literal notranslate">v6.0.0 -> 7.4.3 </code></td>
 </tr>
 <tr>
 <td>[enable]</td>
 <td><code class="docutils literal notranslate">v6.0.0 -> 7.4.3</code></td>
 <tr>
 <td>[disable]</td>
 <td><code class="docutils literal notranslate">v6.0.0 -> 7.4.3</code></td>
 </table>
 </div>
 </li>
        <li> <span class="li-head">serial_number</span> - Serial number. <span class="li-normal">type: str</span>
 <a id='label38' href="javascript:ContentClick('label39', 'label38');" onmouseover="ContentPreview('label39');" onmouseout="ContentUnpreview('label39');" title="click to collapse or expand..."> more... </a>
 <div id="label39" style="display:none">
 <table border="1">
 <tr>
 <td></td>
 <td colspan="1">Supported Version Ranges</td>
 </tr>
 <tr>
 <td>serial_number</td>
 <td><code class="docutils literal notranslate">v6.0.0 -> 7.4.3 </code></td>
 </tr>
 </table>
 </div>
 </li>
        <li> <span class="li-head">server_list</span> - Additional severs that the FortiGate can use for updates (for AV, IPS, updates) and ratings (for web filter and antispam ratings) servers. <span class="li-normal">type: list</span> <span style="font-family:'Courier New'" class="li-required">member_path: server_list:id</span>
 <a id='label40' href="javascript:ContentClick('label41', 'label40');" onmouseover="ContentPreview('label41');" onmouseout="ContentUnpreview('label41');" title="click to collapse or expand..."> more... </a>
 <div id="label41" style="display:none">
 <table border="1">
 <tr>
 <td></td><td colspan="1">Supported Version Ranges</td>
 </tr>
 <tr>
 <td>server_list</td>
 <td><code class="docutils literal notranslate">v6.0.0 -> 7.4.3 </code></td>
 </tr>
 </table>
 </div>
 </li>
            <ul class="ul-self">
            <li> <span class="li-head">addr_type</span> - Indicate whether the FortiGate communicates with the override server using an IPv4 address, an IPv6 address or a FQDN. <span class="li-normal">type: str</span> <span class="li-normal">choices: ipv4, ipv6, fqdn</span>
 <a id='label42' href="javascript:ContentClick('label43', 'label42');" onmouseover="ContentPreview('label43');" onmouseout="ContentUnpreview('label43');" title="click to collapse or expand..."> more... </a>
 <div id="label43" style="display:none">
 <table border="1">
 <tr>
 <td></td>
 <td colspan="1">Supported Version Ranges</td>
 </tr>
 <tr>
 <td>addr_type</td>
 <td><code class="docutils literal notranslate">v6.0.0 -> 7.4.3 </code></td>
 </tr>
 <tr>
 <td>[ipv4]</td>
 <td><code class="docutils literal notranslate">v6.0.0 -> 7.4.3</code></td>
 <tr>
 <td>[ipv6]</td>
 <td><code class="docutils literal notranslate">v6.0.0 -> 7.4.3</code></td>
 <tr>
 <td>[fqdn]</td>
 <td><code class="docutils literal notranslate">v6.0.0 -> 7.4.3</code></td>
 </table>
 </div>
 </li>
            <li> <span class="li-head">fqdn</span> - FQDN address of override server. <span class="li-normal">type: str</span>
 <a id='label44' href="javascript:ContentClick('label45', 'label44');" onmouseover="ContentPreview('label45');" onmouseout="ContentUnpreview('label45');" title="click to collapse or expand..."> more... </a>
 <div id="label45" style="display:none">
 <table border="1">
 <tr>
 <td></td>
 <td colspan="1">Supported Version Ranges</td>
 </tr>
 <tr>
 <td>fqdn</td>
 <td><code class="docutils literal notranslate">v6.0.0 -> 7.4.3 </code></td>
 </tr>
 </table>
 </div>
 </li>
            <li> <span class="li-head">id</span> - ID. see <a href='#notes'>Notes</a>. <span class="li-normal">type: int</span> <span class="li-required">required: true</span>
 <a id='label46' href="javascript:ContentClick('label47', 'label46');" onmouseover="ContentPreview('label47');" onmouseout="ContentUnpreview('label47');" title="click to collapse or expand..."> more... </a>
 <div id="label47" style="display:none">
 <table border="1">
 <tr>
 <td></td>
 <td colspan="1">Supported Version Ranges</td>
 </tr>
 <tr>
 <td>id</td>
 <td><code class="docutils literal notranslate">v6.0.0 -> 7.4.3 </code></td>
 </tr>
 </table>
 </div>
 </li>
            <li> <span class="li-head">server_address</span> - IPv4 address of override server. <span class="li-normal">type: str</span>
 <a id='label48' href="javascript:ContentClick('label49', 'label48');" onmouseover="ContentPreview('label49');" onmouseout="ContentUnpreview('label49');" title="click to collapse or expand..."> more... </a>
 <div id="label49" style="display:none">
 <table border="1">
 <tr>
 <td></td>
 <td colspan="1">Supported Version Ranges</td>
 </tr>
 <tr>
 <td>server_address</td>
 <td><code class="docutils literal notranslate">v6.0.0 -> 7.4.3 </code></td>
 </tr>
 </table>
 </div>
 </li>
            <li> <span class="li-head">server_address6</span> - IPv6 address of override server. <span class="li-normal">type: str</span>
 <a id='label50' href="javascript:ContentClick('label51', 'label50');" onmouseover="ContentPreview('label51');" onmouseout="ContentUnpreview('label51');" title="click to collapse or expand..."> more... </a>
 <div id="label51" style="display:none">
 <table border="1">
 <tr>
 <td></td>
 <td colspan="1">Supported Version Ranges</td>
 </tr>
 <tr>
 <td>server_address6</td>
 <td><code class="docutils literal notranslate">v6.0.0 -> 7.4.3 </code></td>
 </tr>
 </table>
 </div>
 </li>
            <li> <span class="li-head">server_type</span> - FortiGuard service type. <span class="li-normal">type: list</span> <span class="li-normal">choices: update, rating, iot-query, iot-collect</span>
 <a id='label52' href="javascript:ContentClick('label53', 'label52');" onmouseover="ContentPreview('label53');" onmouseout="ContentUnpreview('label53');" title="click to collapse or expand..."> more... </a>
 <div id="label53" style="display:none">
 <table border="1">
 <tr>
 <td></td>
 <td colspan="1">Supported Version Ranges</td>
 </tr>
 <tr>
 <td>server_type</td>
 <td><code class="docutils literal notranslate">v6.0.0 -> 7.4.3 </code></td>
 </tr>
 <tr>
 <td>[update]</td>
 <td><code class="docutils literal notranslate">v6.0.0 -> 7.4.3</code></td>
 <tr>
 <td>[rating]</td>
 <td><code class="docutils literal notranslate">v6.0.0 -> 7.4.3</code></td>
 <tr>
 <td>[iot-query]</td>
 <td><code class="docutils literal notranslate">v7.2.1 -> 7.4.3</code></td>
 </tr>
 <tr>
 <td>[iot-collect]</td>
 <td><code class="docutils literal notranslate">v7.2.1 -> 7.4.3</code></td>
 </tr>
 </table>
 </div>
 </li>
            </ul>
        <li> <span class="li-head">type</span> - Central management type. <span class="li-normal">type: str</span> <span class="li-normal">choices: fortimanager, fortiguard, none</span>
 <a id='label54' href="javascript:ContentClick('label55', 'label54');" onmouseover="ContentPreview('label55');" onmouseout="ContentUnpreview('label55');" title="click to collapse or expand..."> more... </a>
 <div id="label55" style="display:none">
 <table border="1">
 <tr>
 <td></td>
 <td colspan="1">Supported Version Ranges</td>
 </tr>
 <tr>
 <td>type</td>
 <td><code class="docutils literal notranslate">v6.0.0 -> 7.4.3 </code></td>
 </tr>
 <tr>
 <td>[fortimanager]</td>
 <td><code class="docutils literal notranslate">v6.0.0 -> 7.4.3</code></td>
 <tr>
 <td>[fortiguard]</td>
 <td><code class="docutils literal notranslate">v6.0.0 -> 7.4.3</code></td>
 <tr>
 <td>[none]</td>
 <td><code class="docutils literal notranslate">v6.0.0 -> 7.4.3</code></td>
 </table>
 </div>
 </li>
        <li> <span class="li-head">vdom</span> - Virtual domain (VDOM) name to use when communicating with FortiManager. Source system.vdom.name. <span class="li-normal">type: str</span>
 <a id='label56' href="javascript:ContentClick('label57', 'label56');" onmouseover="ContentPreview('label57');" onmouseout="ContentUnpreview('label57');" title="click to collapse or expand..."> more... </a>
 <div id="label57" style="display:none">
 <table border="1">
 <tr>
 <td></td>
 <td colspan="1">Supported Version Ranges</td>
 </tr>
 <tr>
 <td>vdom</td>
 <td><code class="docutils literal notranslate">v6.0.0 -> 7.4.3 </code></td>
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
    
    - name: Configure central management.
      fortinet.fortios.fortios_system_central_management:
          vdom: "{{ vdom }}"
          system_central_management:
              allow_monitor: "enable"
              allow_push_configuration: "enable"
              allow_push_firmware: "enable"
              allow_remote_firmware_upgrade: "enable"
              ca_cert: "<your_own_value>"
              enc_algorithm: "default"
              fmg: "<your_own_value>"
              fmg_source_ip: "<your_own_value>"
              fmg_source_ip6: "<your_own_value>"
              fmg_update_port: "8890"
              fortigate_cloud_sso_default_profile: "<your_own_value> (source system.accprofile.name)"
              include_default_servers: "enable"
              interface: "<your_own_value> (source system.interface.name)"
              interface_select_method: "auto"
              local_cert: "<your_own_value>"
              mode: "normal"
              schedule_config_restore: "enable"
              schedule_script_restore: "enable"
              serial_number: "<your_own_value>"
              server_list:
                  -
                      addr_type: "ipv4"
                      fqdn: "<your_own_value>"
                      id: "25"
                      server_address: "<your_own_value>"
                      server_address6: "<your_own_value>"
                      server_type: "update"
              type: "fortimanager"
              vdom: "<your_own_value> (source system.vdom.name)"


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
