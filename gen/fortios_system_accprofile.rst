:source: fortios_system_accprofile.py

:orphan:

.. fortios_system_accprofile:

fortios_system_accprofile -- Configure access profiles for system administrators in Fortinet's FortiOS and FortiGate.
+++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++

.. versionadded:: 2.0.0

.. contents::
   :local:
   :depth: 1


Synopsis
--------
- This module is able to configure a FortiGate or FortiOS (FOS) device by allowing the user to set and modify system feature and accprofile category. Examples include all parameters and values need to be adjusted to datasources before usage. Tested with FOS v6.0.0



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
 <td>fortios_system_accprofile</td>
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
    <li> <span class="li-head">system_accprofile</span> - Configure access profiles for system administrators. <span class="li-normal">type: dict</span>
 <a id='label0' href="javascript:ContentClick('label1', 'label0');" onmouseover="ContentPreview('label1');" onmouseout="ContentUnpreview('label1');" title="click to collapse or expand..."> more... </a>
 <div id="label1" style="display:none">
 <table border="1">
 <tr>
 <td></td><td colspan="1">Supported Version Ranges</td>
 </tr>
 <tr>
 <td>system_accprofile</td>
 <td><code class="docutils literal notranslate">v6.0.0 -> latest </code></td>
 </tr>
 </table>
 </div>
 </li>
        <ul class="ul-self">
        <li> <span class="li-head">admintimeout</span> - Administrator timeout for this access profile (0 - 480 min). <span class="li-normal">type: int</span>
 <a id='label2' href="javascript:ContentClick('label3', 'label2');" onmouseover="ContentPreview('label3');" onmouseout="ContentUnpreview('label3');" title="click to collapse or expand..."> more... </a>
 <div id="label3" style="display:none">
 <table border="1">
 <tr>
 <td></td>
 <td colspan="1">Supported Version Ranges</td>
 </tr>
 <tr>
 <td>admintimeout</td>
 <td><code class="docutils literal notranslate">v6.0.0 -> latest </code></td>
 </tr>
 </table>
 </div>
 </li>
        <li> <span class="li-head">admintimeout_override</span> - Enable/disable overriding the global administrator idle timeout. <span class="li-normal">type: str</span> <span class="li-normal">choices: enable, disable</span>
 <a id='label4' href="javascript:ContentClick('label5', 'label4');" onmouseover="ContentPreview('label5');" onmouseout="ContentUnpreview('label5');" title="click to collapse or expand..."> more... </a>
 <div id="label5" style="display:none">
 <table border="1">
 <tr>
 <td></td>
 <td colspan="1">Supported Version Ranges</td>
 </tr>
 <tr>
 <td>admintimeout_override</td>
 <td><code class="docutils literal notranslate">v6.0.0 -> latest </code></td>
 </tr>
 <tr>
 <td>[enable]</td>
 <td><code class="docutils literal notranslate">v6.0.0 -> latest</code></td> <tr>
 <td>[disable]</td>
 <td><code class="docutils literal notranslate">v6.0.0 -> latest</code></td> </table>
 </div>
 </li>
        <li> <span class="li-head">authgrp</span> - Administrator access to Users and Devices. <span class="li-normal">type: str</span> <span class="li-normal">choices: none, read, read-write</span>
 <a id='label6' href="javascript:ContentClick('label7', 'label6');" onmouseover="ContentPreview('label7');" onmouseout="ContentUnpreview('label7');" title="click to collapse or expand..."> more... </a>
 <div id="label7" style="display:none">
 <table border="1">
 <tr>
 <td></td>
 <td colspan="1">Supported Version Ranges</td>
 </tr>
 <tr>
 <td>authgrp</td>
 <td><code class="docutils literal notranslate">v6.0.0 -> latest </code></td>
 </tr>
 <tr>
 <td>[none]</td>
 <td><code class="docutils literal notranslate">v6.0.0 -> latest</code></td> <tr>
 <td>[read]</td>
 <td><code class="docutils literal notranslate">v6.0.0 -> latest</code></td> <tr>
 <td>[read-write]</td>
 <td><code class="docutils literal notranslate">v6.0.0 -> latest</code></td> </table>
 </div>
 </li>
        <li> <span class="li-head">comments</span> - Comment. <span class="li-normal">type: str</span>
 <a id='label8' href="javascript:ContentClick('label9', 'label8');" onmouseover="ContentPreview('label9');" onmouseout="ContentUnpreview('label9');" title="click to collapse or expand..."> more... </a>
 <div id="label9" style="display:none">
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
        <li> <span class="li-head">ftviewgrp</span> - FortiView. <span class="li-normal">type: str</span> <span class="li-normal">choices: none, read, read-write</span>
 <a id='label10' href="javascript:ContentClick('label11', 'label10');" onmouseover="ContentPreview('label11');" onmouseout="ContentUnpreview('label11');" title="click to collapse or expand..."> more... </a>
 <div id="label11" style="display:none">
 <table border="1">
 <tr>
 <td></td>
 <td colspan="1">Supported Version Ranges</td>
 </tr>
 <tr>
 <td>ftviewgrp</td>
 <td><code class="docutils literal notranslate">v6.0.0 -> latest </code></td>
 </tr>
 <tr>
 <td>[none]</td>
 <td><code class="docutils literal notranslate">v6.0.0 -> latest</code></td> <tr>
 <td>[read]</td>
 <td><code class="docutils literal notranslate">v6.0.0 -> latest</code></td> <tr>
 <td>[read-write]</td>
 <td><code class="docutils literal notranslate">v6.0.0 -> latest</code></td> </table>
 </div>
 </li>
        <li> <span class="li-head">fwgrp</span> - Administrator access to the Firewall configuration. <span class="li-normal">type: str</span> <span class="li-normal">choices: none, read, read-write, custom</span>
 <a id='label12' href="javascript:ContentClick('label13', 'label12');" onmouseover="ContentPreview('label13');" onmouseout="ContentUnpreview('label13');" title="click to collapse or expand..."> more... </a>
 <div id="label13" style="display:none">
 <table border="1">
 <tr>
 <td></td>
 <td colspan="1">Supported Version Ranges</td>
 </tr>
 <tr>
 <td>fwgrp</td>
 <td><code class="docutils literal notranslate">v6.0.0 -> latest </code></td>
 </tr>
 <tr>
 <td>[none]</td>
 <td><code class="docutils literal notranslate">v6.0.0 -> latest</code></td> <tr>
 <td>[read]</td>
 <td><code class="docutils literal notranslate">v6.0.0 -> latest</code></td> <tr>
 <td>[read-write]</td>
 <td><code class="docutils literal notranslate">v6.0.0 -> latest</code></td> <tr>
 <td>[custom]</td>
 <td><code class="docutils literal notranslate">v6.0.0 -> latest</code></td> </table>
 </div>
 </li>
        <li> <span class="li-head">fwgrp_permission</span> - Custom firewall permission. <span class="li-normal">type: dict</span>
 <a id='label14' href="javascript:ContentClick('label15', 'label14');" onmouseover="ContentPreview('label15');" onmouseout="ContentUnpreview('label15');" title="click to collapse or expand..."> more... </a>
 <div id="label15" style="display:none">
 <table border="1">
 <tr>
 <td></td><td colspan="1">Supported Version Ranges</td>
 </tr>
 <tr>
 <td>fwgrp_permission</td>
 <td><code class="docutils literal notranslate">v6.0.0 -> latest </code></td>
 </tr>
 </table>
 </div>
 </li>
            <ul class="ul-self">
            <li> <span class="li-head">address</span> - Address Configuration. <span class="li-normal">type: str</span> <span class="li-normal">choices: none, read, read-write</span>
 <a id='label16' href="javascript:ContentClick('label17', 'label16');" onmouseover="ContentPreview('label17');" onmouseout="ContentUnpreview('label17');" title="click to collapse or expand..."> more... </a>
 <div id="label17" style="display:none">
 <table border="1">
 <tr>
 <td></td>
 <td colspan="1">Supported Version Ranges</td>
 </tr>
 <tr>
 <td>address</td>
 <td><code class="docutils literal notranslate">v6.0.0 -> latest </code></td>
 </tr>
 <tr>
 <td>[none]</td>
 <td><code class="docutils literal notranslate">v6.0.0 -> latest</code></td> <tr>
 <td>[read]</td>
 <td><code class="docutils literal notranslate">v6.0.0 -> latest</code></td> <tr>
 <td>[read-write]</td>
 <td><code class="docutils literal notranslate">v6.0.0 -> latest</code></td> </table>
 </div>
 </li>
            <li> <span class="li-head">others</span> - Other Firewall Configuration. <span class="li-normal">type: str</span> <span class="li-normal">choices: none, read, read-write</span>
 <a id='label18' href="javascript:ContentClick('label19', 'label18');" onmouseover="ContentPreview('label19');" onmouseout="ContentUnpreview('label19');" title="click to collapse or expand..."> more... </a>
 <div id="label19" style="display:none">
 <table border="1">
 <tr>
 <td></td>
 <td colspan="1">Supported Version Ranges</td>
 </tr>
 <tr>
 <td>others</td>
 <td><code class="docutils literal notranslate">v7.0.1 -> latest </code></td>
 </tr>
 <tr>
 <td>[none]</td>
 <td><code class="docutils literal notranslate">v6.0.0 -> latest</code></td> <tr>
 <td>[read]</td>
 <td><code class="docutils literal notranslate">v6.0.0 -> latest</code></td> <tr>
 <td>[read-write]</td>
 <td><code class="docutils literal notranslate">v6.0.0 -> latest</code></td> </table>
 </div>
 </li>
            <li> <span class="li-head">policy</span> - Policy Configuration. <span class="li-normal">type: str</span> <span class="li-normal">choices: none, read, read-write</span>
 <a id='label20' href="javascript:ContentClick('label21', 'label20');" onmouseover="ContentPreview('label21');" onmouseout="ContentUnpreview('label21');" title="click to collapse or expand..."> more... </a>
 <div id="label21" style="display:none">
 <table border="1">
 <tr>
 <td></td>
 <td colspan="1">Supported Version Ranges</td>
 </tr>
 <tr>
 <td>policy</td>
 <td><code class="docutils literal notranslate">v6.0.0 -> latest </code></td>
 </tr>
 <tr>
 <td>[none]</td>
 <td><code class="docutils literal notranslate">v6.0.0 -> latest</code></td> <tr>
 <td>[read]</td>
 <td><code class="docutils literal notranslate">v6.0.0 -> latest</code></td> <tr>
 <td>[read-write]</td>
 <td><code class="docutils literal notranslate">v6.0.0 -> latest</code></td> </table>
 </div>
 </li>
            <li> <span class="li-head">schedule</span> - Schedule Configuration. <span class="li-normal">type: str</span> <span class="li-normal">choices: none, read, read-write</span>
 <a id='label22' href="javascript:ContentClick('label23', 'label22');" onmouseover="ContentPreview('label23');" onmouseout="ContentUnpreview('label23');" title="click to collapse or expand..."> more... </a>
 <div id="label23" style="display:none">
 <table border="1">
 <tr>
 <td></td>
 <td colspan="1">Supported Version Ranges</td>
 </tr>
 <tr>
 <td>schedule</td>
 <td><code class="docutils literal notranslate">v6.0.0 -> latest </code></td>
 </tr>
 <tr>
 <td>[none]</td>
 <td><code class="docutils literal notranslate">v6.0.0 -> latest</code></td> <tr>
 <td>[read]</td>
 <td><code class="docutils literal notranslate">v6.0.0 -> latest</code></td> <tr>
 <td>[read-write]</td>
 <td><code class="docutils literal notranslate">v6.0.0 -> latest</code></td> </table>
 </div>
 </li>
            <li> <span class="li-head">service</span> - Service Configuration. <span class="li-normal">type: str</span> <span class="li-normal">choices: none, read, read-write</span>
 <a id='label24' href="javascript:ContentClick('label25', 'label24');" onmouseover="ContentPreview('label25');" onmouseout="ContentUnpreview('label25');" title="click to collapse or expand..."> more... </a>
 <div id="label25" style="display:none">
 <table border="1">
 <tr>
 <td></td>
 <td colspan="1">Supported Version Ranges</td>
 </tr>
 <tr>
 <td>service</td>
 <td><code class="docutils literal notranslate">v6.0.0 -> latest </code></td>
 </tr>
 <tr>
 <td>[none]</td>
 <td><code class="docutils literal notranslate">v6.0.0 -> latest</code></td> <tr>
 <td>[read]</td>
 <td><code class="docutils literal notranslate">v6.0.0 -> latest</code></td> <tr>
 <td>[read-write]</td>
 <td><code class="docutils literal notranslate">v6.0.0 -> latest</code></td> </table>
 </div>
 </li>
            </ul>
        <li> <span class="li-head">loggrp</span> - Administrator access to Logging and Reporting including viewing log messages. <span class="li-normal">type: str</span> <span class="li-normal">choices: none, read, read-write, custom</span>
 <a id='label26' href="javascript:ContentClick('label27', 'label26');" onmouseover="ContentPreview('label27');" onmouseout="ContentUnpreview('label27');" title="click to collapse or expand..."> more... </a>
 <div id="label27" style="display:none">
 <table border="1">
 <tr>
 <td></td>
 <td colspan="1">Supported Version Ranges</td>
 </tr>
 <tr>
 <td>loggrp</td>
 <td><code class="docutils literal notranslate">v6.0.0 -> latest </code></td>
 </tr>
 <tr>
 <td>[none]</td>
 <td><code class="docutils literal notranslate">v6.0.0 -> latest</code></td> <tr>
 <td>[read]</td>
 <td><code class="docutils literal notranslate">v6.0.0 -> latest</code></td> <tr>
 <td>[read-write]</td>
 <td><code class="docutils literal notranslate">v6.0.0 -> latest</code></td> <tr>
 <td>[custom]</td>
 <td><code class="docutils literal notranslate">v6.0.0 -> latest</code></td> </table>
 </div>
 </li>
        <li> <span class="li-head">loggrp_permission</span> - Custom Log & Report permission. <span class="li-normal">type: dict</span>
 <a id='label28' href="javascript:ContentClick('label29', 'label28');" onmouseover="ContentPreview('label29');" onmouseout="ContentUnpreview('label29');" title="click to collapse or expand..."> more... </a>
 <div id="label29" style="display:none">
 <table border="1">
 <tr>
 <td></td><td colspan="1">Supported Version Ranges</td>
 </tr>
 <tr>
 <td>loggrp_permission</td>
 <td><code class="docutils literal notranslate">v6.0.0 -> latest </code></td>
 </tr>
 </table>
 </div>
 </li>
            <ul class="ul-self">
            <li> <span class="li-head">config</span> - Log & Report configuration. <span class="li-normal">type: str</span> <span class="li-normal">choices: none, read, read-write</span>
 <a id='label30' href="javascript:ContentClick('label31', 'label30');" onmouseover="ContentPreview('label31');" onmouseout="ContentUnpreview('label31');" title="click to collapse or expand..."> more... </a>
 <div id="label31" style="display:none">
 <table border="1">
 <tr>
 <td></td>
 <td colspan="1">Supported Version Ranges</td>
 </tr>
 <tr>
 <td>config</td>
 <td><code class="docutils literal notranslate">v6.0.0 -> latest </code></td>
 </tr>
 <tr>
 <td>[none]</td>
 <td><code class="docutils literal notranslate">v6.0.0 -> latest</code></td> <tr>
 <td>[read]</td>
 <td><code class="docutils literal notranslate">v6.0.0 -> latest</code></td> <tr>
 <td>[read-write]</td>
 <td><code class="docutils literal notranslate">v6.0.0 -> latest</code></td> </table>
 </div>
 </li>
            <li> <span class="li-head">data_access</span> - Log & Report Data Access. <span class="li-normal">type: str</span> <span class="li-normal">choices: none, read, read-write</span>
 <a id='label32' href="javascript:ContentClick('label33', 'label32');" onmouseover="ContentPreview('label33');" onmouseout="ContentUnpreview('label33');" title="click to collapse or expand..."> more... </a>
 <div id="label33" style="display:none">
 <table border="1">
 <tr>
 <td></td>
 <td colspan="1">Supported Version Ranges</td>
 </tr>
 <tr>
 <td>data_access</td>
 <td><code class="docutils literal notranslate">v6.0.0 -> latest </code></td>
 </tr>
 <tr>
 <td>[none]</td>
 <td><code class="docutils literal notranslate">v6.0.0 -> latest</code></td> <tr>
 <td>[read]</td>
 <td><code class="docutils literal notranslate">v6.0.0 -> latest</code></td> <tr>
 <td>[read-write]</td>
 <td><code class="docutils literal notranslate">v6.0.0 -> latest</code></td> </table>
 </div>
 </li>
            <li> <span class="li-head">report_access</span> - Log & Report Report Access. <span class="li-normal">type: str</span> <span class="li-normal">choices: none, read, read-write</span>
 <a id='label34' href="javascript:ContentClick('label35', 'label34');" onmouseover="ContentPreview('label35');" onmouseout="ContentUnpreview('label35');" title="click to collapse or expand..."> more... </a>
 <div id="label35" style="display:none">
 <table border="1">
 <tr>
 <td></td>
 <td colspan="1">Supported Version Ranges</td>
 </tr>
 <tr>
 <td>report_access</td>
 <td><code class="docutils literal notranslate">v6.0.0 -> latest </code></td>
 </tr>
 <tr>
 <td>[none]</td>
 <td><code class="docutils literal notranslate">v6.0.0 -> latest</code></td> <tr>
 <td>[read]</td>
 <td><code class="docutils literal notranslate">v6.0.0 -> latest</code></td> <tr>
 <td>[read-write]</td>
 <td><code class="docutils literal notranslate">v6.0.0 -> latest</code></td> </table>
 </div>
 </li>
            <li> <span class="li-head">threat_weight</span> - Log & Report Threat Weight. <span class="li-normal">type: str</span> <span class="li-normal">choices: none, read, read-write</span>
 <a id='label36' href="javascript:ContentClick('label37', 'label36');" onmouseover="ContentPreview('label37');" onmouseout="ContentUnpreview('label37');" title="click to collapse or expand..."> more... </a>
 <div id="label37" style="display:none">
 <table border="1">
 <tr>
 <td></td>
 <td colspan="1">Supported Version Ranges</td>
 </tr>
 <tr>
 <td>threat_weight</td>
 <td><code class="docutils literal notranslate">v6.0.0 -> latest </code></td>
 </tr>
 <tr>
 <td>[none]</td>
 <td><code class="docutils literal notranslate">v6.0.0 -> latest</code></td> <tr>
 <td>[read]</td>
 <td><code class="docutils literal notranslate">v6.0.0 -> latest</code></td> <tr>
 <td>[read-write]</td>
 <td><code class="docutils literal notranslate">v6.0.0 -> latest</code></td> </table>
 </div>
 </li>
            </ul>
        <li> <span class="li-head">name</span> - Profile name. <span class="li-normal">type: str</span> <span class="li-required">required: true</span>
 <a id='label38' href="javascript:ContentClick('label39', 'label38');" onmouseover="ContentPreview('label39');" onmouseout="ContentUnpreview('label39');" title="click to collapse or expand..."> more... </a>
 <div id="label39" style="display:none">
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
        <li> <span class="li-head">netgrp</span> - Network Configuration. <span class="li-normal">type: str</span> <span class="li-normal">choices: none, read, read-write, custom</span>
 <a id='label40' href="javascript:ContentClick('label41', 'label40');" onmouseover="ContentPreview('label41');" onmouseout="ContentUnpreview('label41');" title="click to collapse or expand..."> more... </a>
 <div id="label41" style="display:none">
 <table border="1">
 <tr>
 <td></td>
 <td colspan="1">Supported Version Ranges</td>
 </tr>
 <tr>
 <td>netgrp</td>
 <td><code class="docutils literal notranslate">v6.0.0 -> latest </code></td>
 </tr>
 <tr>
 <td>[none]</td>
 <td><code class="docutils literal notranslate">v6.0.0 -> latest</code></td> <tr>
 <td>[read]</td>
 <td><code class="docutils literal notranslate">v6.0.0 -> latest</code></td> <tr>
 <td>[read-write]</td>
 <td><code class="docutils literal notranslate">v6.0.0 -> latest</code></td> <tr>
 <td>[custom]</td>
 <td><code class="docutils literal notranslate">v6.0.0 -> latest</code></td> </table>
 </div>
 </li>
        <li> <span class="li-head">netgrp_permission</span> - Custom network permission. <span class="li-normal">type: dict</span>
 <a id='label42' href="javascript:ContentClick('label43', 'label42');" onmouseover="ContentPreview('label43');" onmouseout="ContentUnpreview('label43');" title="click to collapse or expand..."> more... </a>
 <div id="label43" style="display:none">
 <table border="1">
 <tr>
 <td></td><td colspan="1">Supported Version Ranges</td>
 </tr>
 <tr>
 <td>netgrp_permission</td>
 <td><code class="docutils literal notranslate">v6.0.0 -> latest </code></td>
 </tr>
 </table>
 </div>
 </li>
            <ul class="ul-self">
            <li> <span class="li-head">cfg</span> - Network Configuration. <span class="li-normal">type: str</span> <span class="li-normal">choices: none, read, read-write</span>
 <a id='label44' href="javascript:ContentClick('label45', 'label44');" onmouseover="ContentPreview('label45');" onmouseout="ContentUnpreview('label45');" title="click to collapse or expand..."> more... </a>
 <div id="label45" style="display:none">
 <table border="1">
 <tr>
 <td></td>
 <td colspan="1">Supported Version Ranges</td>
 </tr>
 <tr>
 <td>cfg</td>
 <td><code class="docutils literal notranslate">v6.0.0 -> latest </code></td>
 </tr>
 <tr>
 <td>[none]</td>
 <td><code class="docutils literal notranslate">v6.0.0 -> latest</code></td> <tr>
 <td>[read]</td>
 <td><code class="docutils literal notranslate">v6.0.0 -> latest</code></td> <tr>
 <td>[read-write]</td>
 <td><code class="docutils literal notranslate">v6.0.0 -> latest</code></td> </table>
 </div>
 </li>
            <li> <span class="li-head">packet_capture</span> - Packet Capture Configuration. <span class="li-normal">type: str</span> <span class="li-normal">choices: none, read, read-write</span>
 <a id='label46' href="javascript:ContentClick('label47', 'label46');" onmouseover="ContentPreview('label47');" onmouseout="ContentUnpreview('label47');" title="click to collapse or expand..."> more... </a>
 <div id="label47" style="display:none">
 <table border="1">
 <tr>
 <td></td>
 <td colspan="1">Supported Version Ranges</td>
 </tr>
 <tr>
 <td>packet_capture</td>
 <td><code class="docutils literal notranslate">v6.0.0 -> latest </code></td>
 </tr>
 <tr>
 <td>[none]</td>
 <td><code class="docutils literal notranslate">v6.0.0 -> latest</code></td> <tr>
 <td>[read]</td>
 <td><code class="docutils literal notranslate">v6.0.0 -> latest</code></td> <tr>
 <td>[read-write]</td>
 <td><code class="docutils literal notranslate">v6.0.0 -> latest</code></td> </table>
 </div>
 </li>
            <li> <span class="li-head">route_cfg</span> - Router Configuration. <span class="li-normal">type: str</span> <span class="li-normal">choices: none, read, read-write</span>
 <a id='label48' href="javascript:ContentClick('label49', 'label48');" onmouseover="ContentPreview('label49');" onmouseout="ContentUnpreview('label49');" title="click to collapse or expand..."> more... </a>
 <div id="label49" style="display:none">
 <table border="1">
 <tr>
 <td></td>
 <td colspan="1">Supported Version Ranges</td>
 </tr>
 <tr>
 <td>route_cfg</td>
 <td><code class="docutils literal notranslate">v6.0.0 -> latest </code></td>
 </tr>
 <tr>
 <td>[none]</td>
 <td><code class="docutils literal notranslate">v6.0.0 -> latest</code></td> <tr>
 <td>[read]</td>
 <td><code class="docutils literal notranslate">v6.0.0 -> latest</code></td> <tr>
 <td>[read-write]</td>
 <td><code class="docutils literal notranslate">v6.0.0 -> latest</code></td> </table>
 </div>
 </li>
            </ul>
        <li> <span class="li-head">scope</span> - Scope of admin access: global or specific VDOM(s). <span class="li-normal">type: str</span> <span class="li-normal">choices: vdom, global</span>
 <a id='label50' href="javascript:ContentClick('label51', 'label50');" onmouseover="ContentPreview('label51');" onmouseout="ContentUnpreview('label51');" title="click to collapse or expand..."> more... </a>
 <div id="label51" style="display:none">
 <table border="1">
 <tr>
 <td></td>
 <td colspan="1">Supported Version Ranges</td>
 </tr>
 <tr>
 <td>scope</td>
 <td><code class="docutils literal notranslate">v6.0.0 -> latest </code></td>
 </tr>
 <tr>
 <td>[vdom]</td>
 <td><code class="docutils literal notranslate">v6.0.0 -> latest</code></td> <tr>
 <td>[global]</td>
 <td><code class="docutils literal notranslate">v6.0.0 -> latest</code></td> </table>
 </div>
 </li>
        <li> <span class="li-head">secfabgrp</span> - Security Fabric. <span class="li-normal">type: str</span> <span class="li-normal">choices: none, read, read-write</span>
 <a id='label52' href="javascript:ContentClick('label53', 'label52');" onmouseover="ContentPreview('label53');" onmouseout="ContentUnpreview('label53');" title="click to collapse or expand..."> more... </a>
 <div id="label53" style="display:none">
 <table border="1">
 <tr>
 <td></td>
 <td colspan="1">Supported Version Ranges</td>
 </tr>
 <tr>
 <td>secfabgrp</td>
 <td><code class="docutils literal notranslate">v6.0.0 -> latest </code></td>
 </tr>
 <tr>
 <td>[none]</td>
 <td><code class="docutils literal notranslate">v6.0.0 -> latest</code></td> <tr>
 <td>[read]</td>
 <td><code class="docutils literal notranslate">v6.0.0 -> latest</code></td> <tr>
 <td>[read-write]</td>
 <td><code class="docutils literal notranslate">v6.0.0 -> latest</code></td> </table>
 </div>
 </li>
        <li> <span class="li-head">sysgrp</span> - System Configuration. <span class="li-normal">type: str</span> <span class="li-normal">choices: none, read, read-write, custom</span>
 <a id='label54' href="javascript:ContentClick('label55', 'label54');" onmouseover="ContentPreview('label55');" onmouseout="ContentUnpreview('label55');" title="click to collapse or expand..."> more... </a>
 <div id="label55" style="display:none">
 <table border="1">
 <tr>
 <td></td>
 <td colspan="1">Supported Version Ranges</td>
 </tr>
 <tr>
 <td>sysgrp</td>
 <td><code class="docutils literal notranslate">v6.0.0 -> latest </code></td>
 </tr>
 <tr>
 <td>[none]</td>
 <td><code class="docutils literal notranslate">v6.0.0 -> latest</code></td> <tr>
 <td>[read]</td>
 <td><code class="docutils literal notranslate">v6.0.0 -> latest</code></td> <tr>
 <td>[read-write]</td>
 <td><code class="docutils literal notranslate">v6.0.0 -> latest</code></td> <tr>
 <td>[custom]</td>
 <td><code class="docutils literal notranslate">v6.0.0 -> latest</code></td> </table>
 </div>
 </li>
        <li> <span class="li-head">sysgrp_permission</span> - Custom system permission. <span class="li-normal">type: dict</span>
 <a id='label56' href="javascript:ContentClick('label57', 'label56');" onmouseover="ContentPreview('label57');" onmouseout="ContentUnpreview('label57');" title="click to collapse or expand..."> more... </a>
 <div id="label57" style="display:none">
 <table border="1">
 <tr>
 <td></td><td colspan="1">Supported Version Ranges</td>
 </tr>
 <tr>
 <td>sysgrp_permission</td>
 <td><code class="docutils literal notranslate">v6.0.0 -> latest </code></td>
 </tr>
 </table>
 </div>
 </li>
            <ul class="ul-self">
            <li> <span class="li-head">admin</span> - Administrator Users. <span class="li-normal">type: str</span> <span class="li-normal">choices: none, read, read-write</span>
 <a id='label58' href="javascript:ContentClick('label59', 'label58');" onmouseover="ContentPreview('label59');" onmouseout="ContentUnpreview('label59');" title="click to collapse or expand..."> more... </a>
 <div id="label59" style="display:none">
 <table border="1">
 <tr>
 <td></td>
 <td colspan="1">Supported Version Ranges</td>
 </tr>
 <tr>
 <td>admin</td>
 <td><code class="docutils literal notranslate">v6.0.0 -> latest </code></td>
 </tr>
 <tr>
 <td>[none]</td>
 <td><code class="docutils literal notranslate">v6.0.0 -> latest</code></td> <tr>
 <td>[read]</td>
 <td><code class="docutils literal notranslate">v6.0.0 -> latest</code></td> <tr>
 <td>[read-write]</td>
 <td><code class="docutils literal notranslate">v6.0.0 -> latest</code></td> </table>
 </div>
 </li>
            <li> <span class="li-head">cfg</span> - System Configuration. <span class="li-normal">type: str</span> <span class="li-normal">choices: none, read, read-write</span>
 <a id='label60' href="javascript:ContentClick('label61', 'label60');" onmouseover="ContentPreview('label61');" onmouseout="ContentUnpreview('label61');" title="click to collapse or expand..."> more... </a>
 <div id="label61" style="display:none">
 <table border="1">
 <tr>
 <td></td>
 <td colspan="1">Supported Version Ranges</td>
 </tr>
 <tr>
 <td>cfg</td>
 <td><code class="docutils literal notranslate">v6.0.0 -> latest </code></td>
 </tr>
 <tr>
 <td>[none]</td>
 <td><code class="docutils literal notranslate">v6.0.0 -> latest</code></td> <tr>
 <td>[read]</td>
 <td><code class="docutils literal notranslate">v6.0.0 -> latest</code></td> <tr>
 <td>[read-write]</td>
 <td><code class="docutils literal notranslate">v6.0.0 -> latest</code></td> </table>
 </div>
 </li>
            <li> <span class="li-head">mnt</span> - Maintenance. <span class="li-normal">type: str</span> <span class="li-normal">choices: none, read, read-write</span>
 <a id='label62' href="javascript:ContentClick('label63', 'label62');" onmouseover="ContentPreview('label63');" onmouseout="ContentUnpreview('label63');" title="click to collapse or expand..."> more... </a>
 <div id="label63" style="display:none">
 <table border="1">
 <tr>
 <td></td>
 <td colspan="1">Supported Version Ranges</td>
 </tr>
 <tr>
 <td>mnt</td>
 <td><code class="docutils literal notranslate">v6.0.0 -> latest </code></td>
 </tr>
 <tr>
 <td>[none]</td>
 <td><code class="docutils literal notranslate">v6.0.0 -> latest</code></td> <tr>
 <td>[read]</td>
 <td><code class="docutils literal notranslate">v6.0.0 -> latest</code></td> <tr>
 <td>[read-write]</td>
 <td><code class="docutils literal notranslate">v6.0.0 -> latest</code></td> </table>
 </div>
 </li>
            <li> <span class="li-head">upd</span> - FortiGuard Updates. <span class="li-normal">type: str</span> <span class="li-normal">choices: none, read, read-write</span>
 <a id='label64' href="javascript:ContentClick('label65', 'label64');" onmouseover="ContentPreview('label65');" onmouseout="ContentUnpreview('label65');" title="click to collapse or expand..."> more... </a>
 <div id="label65" style="display:none">
 <table border="1">
 <tr>
 <td></td>
 <td colspan="1">Supported Version Ranges</td>
 </tr>
 <tr>
 <td>upd</td>
 <td><code class="docutils literal notranslate">v6.0.0 -> latest </code></td>
 </tr>
 <tr>
 <td>[none]</td>
 <td><code class="docutils literal notranslate">v6.0.0 -> latest</code></td> <tr>
 <td>[read]</td>
 <td><code class="docutils literal notranslate">v6.0.0 -> latest</code></td> <tr>
 <td>[read-write]</td>
 <td><code class="docutils literal notranslate">v6.0.0 -> latest</code></td> </table>
 </div>
 </li>
            </ul>
        <li> <span class="li-head">system_diagnostics</span> - Enable/disable permission to run system diagnostic commands. <span class="li-normal">type: str</span> <span class="li-normal">choices: enable, disable</span>
 <a id='label66' href="javascript:ContentClick('label67', 'label66');" onmouseover="ContentPreview('label67');" onmouseout="ContentUnpreview('label67');" title="click to collapse or expand..."> more... </a>
 <div id="label67" style="display:none">
 <table border="1">
 <tr>
 <td></td>
 <td colspan="1">Supported Version Ranges</td>
 </tr>
 <tr>
 <td>system_diagnostics</td>
 <td><code class="docutils literal notranslate">v6.4.0 -> latest </code></td>
 </tr>
 <tr>
 <td>[enable]</td>
 <td><code class="docutils literal notranslate">v6.0.0 -> latest</code></td> <tr>
 <td>[disable]</td>
 <td><code class="docutils literal notranslate">v6.0.0 -> latest</code></td> </table>
 </div>
 </li>
        <li> <span class="li-head">system_execute_ssh</span> - Enable/disable permission to execute SSH commands. <span class="li-normal">type: str</span> <span class="li-normal">choices: enable, disable</span>
 <a id='label68' href="javascript:ContentClick('label69', 'label68');" onmouseover="ContentPreview('label69');" onmouseout="ContentUnpreview('label69');" title="click to collapse or expand..."> more... </a>
 <div id="label69" style="display:none">
 <table border="1">
 <tr>
 <td></td>
 <td colspan="1">Supported Version Ranges</td>
 </tr>
 <tr>
 <td>system_execute_ssh</td>
 <td><code class="docutils literal notranslate">v7.2.1 -> latest </code></td>
 </tr>
 <tr>
 <td>[enable]</td>
 <td><code class="docutils literal notranslate">v6.0.0 -> latest</code></td> <tr>
 <td>[disable]</td>
 <td><code class="docutils literal notranslate">v6.0.0 -> latest</code></td> </table>
 </div>
 </li>
        <li> <span class="li-head">system_execute_telnet</span> - Enable/disable permission to execute TELNET commands. <span class="li-normal">type: str</span> <span class="li-normal">choices: enable, disable</span>
 <a id='label70' href="javascript:ContentClick('label71', 'label70');" onmouseover="ContentPreview('label71');" onmouseout="ContentUnpreview('label71');" title="click to collapse or expand..."> more... </a>
 <div id="label71" style="display:none">
 <table border="1">
 <tr>
 <td></td>
 <td colspan="1">Supported Version Ranges</td>
 </tr>
 <tr>
 <td>system_execute_telnet</td>
 <td><code class="docutils literal notranslate">v7.2.1 -> latest </code></td>
 </tr>
 <tr>
 <td>[enable]</td>
 <td><code class="docutils literal notranslate">v6.0.0 -> latest</code></td> <tr>
 <td>[disable]</td>
 <td><code class="docutils literal notranslate">v6.0.0 -> latest</code></td> </table>
 </div>
 </li>
        <li> <span class="li-head">utmgrp</span> - Administrator access to Security Profiles. <span class="li-normal">type: str</span> <span class="li-normal">choices: none, read, read-write, custom</span>
 <a id='label72' href="javascript:ContentClick('label73', 'label72');" onmouseover="ContentPreview('label73');" onmouseout="ContentUnpreview('label73');" title="click to collapse or expand..."> more... </a>
 <div id="label73" style="display:none">
 <table border="1">
 <tr>
 <td></td>
 <td colspan="1">Supported Version Ranges</td>
 </tr>
 <tr>
 <td>utmgrp</td>
 <td><code class="docutils literal notranslate">v6.0.0 -> latest </code></td>
 </tr>
 <tr>
 <td>[none]</td>
 <td><code class="docutils literal notranslate">v6.0.0 -> latest</code></td> <tr>
 <td>[read]</td>
 <td><code class="docutils literal notranslate">v6.0.0 -> latest</code></td> <tr>
 <td>[read-write]</td>
 <td><code class="docutils literal notranslate">v6.0.0 -> latest</code></td> <tr>
 <td>[custom]</td>
 <td><code class="docutils literal notranslate">v6.0.0 -> latest</code></td> </table>
 </div>
 </li>
        <li> <span class="li-head">utmgrp_permission</span> - Custom Security Profile permissions. <span class="li-normal">type: dict</span>
 <a id='label74' href="javascript:ContentClick('label75', 'label74');" onmouseover="ContentPreview('label75');" onmouseout="ContentUnpreview('label75');" title="click to collapse or expand..."> more... </a>
 <div id="label75" style="display:none">
 <table border="1">
 <tr>
 <td></td><td colspan="1">Supported Version Ranges</td>
 </tr>
 <tr>
 <td>utmgrp_permission</td>
 <td><code class="docutils literal notranslate">v6.0.0 -> latest </code></td>
 </tr>
 </table>
 </div>
 </li>
            <ul class="ul-self">
            <li> <span class="li-head">antivirus</span> - Antivirus profiles and settings. <span class="li-normal">type: str</span> <span class="li-normal">choices: none, read, read-write</span>
 <a id='label76' href="javascript:ContentClick('label77', 'label76');" onmouseover="ContentPreview('label77');" onmouseout="ContentUnpreview('label77');" title="click to collapse or expand..."> more... </a>
 <div id="label77" style="display:none">
 <table border="1">
 <tr>
 <td></td>
 <td colspan="1">Supported Version Ranges</td>
 </tr>
 <tr>
 <td>antivirus</td>
 <td><code class="docutils literal notranslate">v6.0.0 -> latest </code></td>
 </tr>
 <tr>
 <td>[none]</td>
 <td><code class="docutils literal notranslate">v6.0.0 -> latest</code></td> <tr>
 <td>[read]</td>
 <td><code class="docutils literal notranslate">v6.0.0 -> latest</code></td> <tr>
 <td>[read-write]</td>
 <td><code class="docutils literal notranslate">v6.0.0 -> latest</code></td> </table>
 </div>
 </li>
            <li> <span class="li-head">application_control</span> - Application Control profiles and settings. <span class="li-normal">type: str</span> <span class="li-normal">choices: none, read, read-write</span>
 <a id='label78' href="javascript:ContentClick('label79', 'label78');" onmouseover="ContentPreview('label79');" onmouseout="ContentUnpreview('label79');" title="click to collapse or expand..."> more... </a>
 <div id="label79" style="display:none">
 <table border="1">
 <tr>
 <td></td>
 <td colspan="1">Supported Version Ranges</td>
 </tr>
 <tr>
 <td>application_control</td>
 <td><code class="docutils literal notranslate">v6.0.0 -> latest </code></td>
 </tr>
 <tr>
 <td>[none]</td>
 <td><code class="docutils literal notranslate">v6.0.0 -> latest</code></td> <tr>
 <td>[read]</td>
 <td><code class="docutils literal notranslate">v6.0.0 -> latest</code></td> <tr>
 <td>[read-write]</td>
 <td><code class="docutils literal notranslate">v6.0.0 -> latest</code></td> </table>
 </div>
 </li>
            <li> <span class="li-head">casb</span> - Inline CASB filter profile and settings <span class="li-normal">type: str</span> <span class="li-normal">choices: none, read, read-write</span>
 <a id='label80' href="javascript:ContentClick('label81', 'label80');" onmouseover="ContentPreview('label81');" onmouseout="ContentUnpreview('label81');" title="click to collapse or expand..."> more... </a>
 <div id="label81" style="display:none">
 <table border="1">
 <tr>
 <td></td>
 <td colspan="1">Supported Version Ranges</td>
 </tr>
 <tr>
 <td>casb</td>
 <td><code class="docutils literal notranslate">v7.4.1 -> latest </code></td>
 </tr>
 <tr>
 <td>[none]</td>
 <td><code class="docutils literal notranslate">v6.0.0 -> latest</code></td> <tr>
 <td>[read]</td>
 <td><code class="docutils literal notranslate">v6.0.0 -> latest</code></td> <tr>
 <td>[read-write]</td>
 <td><code class="docutils literal notranslate">v6.0.0 -> latest</code></td> </table>
 </div>
 </li>
            <li> <span class="li-head">data_leak_prevention</span> - DLP profiles and settings. <span class="li-normal">type: str</span> <span class="li-normal">choices: none, read, read-write</span>
 <a id='label82' href="javascript:ContentClick('label83', 'label82');" onmouseover="ContentPreview('label83');" onmouseout="ContentUnpreview('label83');" title="click to collapse or expand..."> more... </a>
 <div id="label83" style="display:none">
 <table border="1">
 <tr>
 <td></td>
 <td colspan="1">Supported Version Ranges</td>
 </tr>
 <tr>
 <td>data_leak_prevention</td>
 <td><code class="docutils literal notranslate">v7.2.4 -> latest </code></td>
 </tr>
 <tr>
 <td>[none]</td>
 <td><code class="docutils literal notranslate">v6.0.0 -> latest</code></td> <tr>
 <td>[read]</td>
 <td><code class="docutils literal notranslate">v6.0.0 -> latest</code></td> <tr>
 <td>[read-write]</td>
 <td><code class="docutils literal notranslate">v6.0.0 -> latest</code></td> </table>
 </div>
 </li>
            <li> <span class="li-head">data_loss_prevention</span> - DLP profiles and settings. <span class="li-normal">type: str</span> <span class="li-normal">choices: none, read, read-write</span>
 <a id='label84' href="javascript:ContentClick('label85', 'label84');" onmouseover="ContentPreview('label85');" onmouseout="ContentUnpreview('label85');" title="click to collapse or expand..."> more... </a>
 <div id="label85" style="display:none">
 <table border="1">
 <tr>
 <td></td>
 <td colspan="1">Supported Version Ranges</td>
 </tr>
 <tr>
 <td>data_loss_prevention</td>
 <td><code class="docutils literal notranslate">v6.0.0 -> v7.2.2 </code></td>
 </tr>
 <tr>
 <td>[none]</td>
 <td><code class="docutils literal notranslate">v6.0.0 -> latest</code></td> <tr>
 <td>[read]</td>
 <td><code class="docutils literal notranslate">v6.0.0 -> latest</code></td> <tr>
 <td>[read-write]</td>
 <td><code class="docutils literal notranslate">v6.0.0 -> latest</code></td> </table>
 </div>
 </li>
            <li> <span class="li-head">dnsfilter</span> - DNS Filter profiles and settings. <span class="li-normal">type: str</span> <span class="li-normal">choices: none, read, read-write</span>
 <a id='label86' href="javascript:ContentClick('label87', 'label86');" onmouseover="ContentPreview('label87');" onmouseout="ContentUnpreview('label87');" title="click to collapse or expand..."> more... </a>
 <div id="label87" style="display:none">
 <table border="1">
 <tr>
 <td></td>
 <td colspan="1">Supported Version Ranges</td>
 </tr>
 <tr>
 <td>dnsfilter</td>
 <td><code class="docutils literal notranslate">v6.0.0 -> latest </code></td>
 </tr>
 <tr>
 <td>[none]</td>
 <td><code class="docutils literal notranslate">v6.0.0 -> latest</code></td> <tr>
 <td>[read]</td>
 <td><code class="docutils literal notranslate">v6.0.0 -> latest</code></td> <tr>
 <td>[read-write]</td>
 <td><code class="docutils literal notranslate">v6.0.0 -> latest</code></td> </table>
 </div>
 </li>
            <li> <span class="li-head">emailfilter</span> - Email Filter and settings. <span class="li-normal">type: str</span> <span class="li-normal">choices: none, read, read-write</span>
 <a id='label88' href="javascript:ContentClick('label89', 'label88');" onmouseover="ContentPreview('label89');" onmouseout="ContentUnpreview('label89');" title="click to collapse or expand..."> more... </a>
 <div id="label89" style="display:none">
 <table border="1">
 <tr>
 <td></td>
 <td colspan="1">Supported Version Ranges</td>
 </tr>
 <tr>
 <td>emailfilter</td>
 <td><code class="docutils literal notranslate">v6.2.0 -> latest </code></td>
 </tr>
 <tr>
 <td>[none]</td>
 <td><code class="docutils literal notranslate">v6.0.0 -> latest</code></td> <tr>
 <td>[read]</td>
 <td><code class="docutils literal notranslate">v6.0.0 -> latest</code></td> <tr>
 <td>[read-write]</td>
 <td><code class="docutils literal notranslate">v6.0.0 -> latest</code></td> </table>
 </div>
 </li>
            <li> <span class="li-head">endpoint_control</span> - FortiClient Profiles. <span class="li-normal">type: str</span> <span class="li-normal">choices: none, read, read-write</span>
 <a id='label90' href="javascript:ContentClick('label91', 'label90');" onmouseover="ContentPreview('label91');" onmouseout="ContentUnpreview('label91');" title="click to collapse or expand..."> more... </a>
 <div id="label91" style="display:none">
 <table border="1">
 <tr>
 <td></td>
 <td colspan="1">Supported Version Ranges</td>
 </tr>
 <tr>
 <td>endpoint_control</td>
 <td><code class="docutils literal notranslate">v6.0.0 -> latest </code></td>
 </tr>
 <tr>
 <td>[none]</td>
 <td><code class="docutils literal notranslate">v6.0.0 -> latest</code></td> <tr>
 <td>[read]</td>
 <td><code class="docutils literal notranslate">v6.0.0 -> latest</code></td> <tr>
 <td>[read-write]</td>
 <td><code class="docutils literal notranslate">v6.0.0 -> latest</code></td> </table>
 </div>
 </li>
            <li> <span class="li-head">file_filter</span> - File-filter profiles and settings. <span class="li-normal">type: str</span> <span class="li-normal">choices: none, read, read-write</span>
 <a id='label92' href="javascript:ContentClick('label93', 'label92');" onmouseover="ContentPreview('label93');" onmouseout="ContentUnpreview('label93');" title="click to collapse or expand..."> more... </a>
 <div id="label93" style="display:none">
 <table border="1">
 <tr>
 <td></td>
 <td colspan="1">Supported Version Ranges</td>
 </tr>
 <tr>
 <td>file_filter</td>
 <td><code class="docutils literal notranslate">v6.4.0 -> latest </code></td>
 </tr>
 <tr>
 <td>[none]</td>
 <td><code class="docutils literal notranslate">v6.0.0 -> latest</code></td> <tr>
 <td>[read]</td>
 <td><code class="docutils literal notranslate">v6.0.0 -> latest</code></td> <tr>
 <td>[read-write]</td>
 <td><code class="docutils literal notranslate">v6.0.0 -> latest</code></td> </table>
 </div>
 </li>
            <li> <span class="li-head">icap</span> - ICAP profiles and settings. <span class="li-normal">type: str</span> <span class="li-normal">choices: none, read, read-write</span>
 <a id='label94' href="javascript:ContentClick('label95', 'label94');" onmouseover="ContentPreview('label95');" onmouseout="ContentUnpreview('label95');" title="click to collapse or expand..."> more... </a>
 <div id="label95" style="display:none">
 <table border="1">
 <tr>
 <td></td>
 <td colspan="1">Supported Version Ranges</td>
 </tr>
 <tr>
 <td>icap</td>
 <td><code class="docutils literal notranslate">v6.0.0 -> latest </code></td>
 </tr>
 <tr>
 <td>[none]</td>
 <td><code class="docutils literal notranslate">v6.0.0 -> latest</code></td> <tr>
 <td>[read]</td>
 <td><code class="docutils literal notranslate">v6.0.0 -> latest</code></td> <tr>
 <td>[read-write]</td>
 <td><code class="docutils literal notranslate">v6.0.0 -> latest</code></td> </table>
 </div>
 </li>
            <li> <span class="li-head">ips</span> - IPS profiles and settings. <span class="li-normal">type: str</span> <span class="li-normal">choices: none, read, read-write</span>
 <a id='label96' href="javascript:ContentClick('label97', 'label96');" onmouseover="ContentPreview('label97');" onmouseout="ContentUnpreview('label97');" title="click to collapse or expand..."> more... </a>
 <div id="label97" style="display:none">
 <table border="1">
 <tr>
 <td></td>
 <td colspan="1">Supported Version Ranges</td>
 </tr>
 <tr>
 <td>ips</td>
 <td><code class="docutils literal notranslate">v6.0.0 -> latest </code></td>
 </tr>
 <tr>
 <td>[none]</td>
 <td><code class="docutils literal notranslate">v6.0.0 -> latest</code></td> <tr>
 <td>[read]</td>
 <td><code class="docutils literal notranslate">v6.0.0 -> latest</code></td> <tr>
 <td>[read-write]</td>
 <td><code class="docutils literal notranslate">v6.0.0 -> latest</code></td> </table>
 </div>
 </li>
            <li> <span class="li-head">mmsgtp</span> - UTM permission. <span class="li-normal">type: str</span> <span class="li-normal">choices: none, read, read-write</span>
 <a id='label98' href="javascript:ContentClick('label99', 'label98');" onmouseover="ContentPreview('label99');" onmouseout="ContentUnpreview('label99');" title="click to collapse or expand..."> more... </a>
 <div id="label99" style="display:none">
 <table border="1">
 <tr>
 <td></td>
 <td colspan="2">Supported Version Ranges</td>
 </tr>
 <tr>
 <td>mmsgtp</td>
 <td><code class="docutils literal notranslate">v6.0.0 -> v7.0.8 </code></td>
 <td><code class="docutils literal notranslate">v7.2.0 -> v7.2.4 </code></td>
 </tr>
 <tr>
 <td>[none]</td>
 <td><code class="docutils literal notranslate">v6.0.0 -> latest</code></td> <tr>
 <td>[read]</td>
 <td><code class="docutils literal notranslate">v6.0.0 -> latest</code></td> <tr>
 <td>[read-write]</td>
 <td><code class="docutils literal notranslate">v6.0.0 -> latest</code></td> </table>
 </div>
 </li>
            <li> <span class="li-head">spamfilter</span> - AntiSpam filter and settings. <span class="li-normal">type: str</span> <span class="li-normal">choices: none, read, read-write</span>
 <a id='label100' href="javascript:ContentClick('label101', 'label100');" onmouseover="ContentPreview('label101');" onmouseout="ContentUnpreview('label101');" title="click to collapse or expand..."> more... </a>
 <div id="label101" style="display:none">
 <table border="1">
 <tr>
 <td></td>
 <td colspan="1">Supported Version Ranges</td>
 </tr>
 <tr>
 <td>spamfilter</td>
 <td><code class="docutils literal notranslate">v6.0.0 -> v6.0.11 </code></td>
 </tr>
 <tr>
 <td>[none]</td>
 <td><code class="docutils literal notranslate">v6.0.0 -> latest</code></td> <tr>
 <td>[read]</td>
 <td><code class="docutils literal notranslate">v6.0.0 -> latest</code></td> <tr>
 <td>[read-write]</td>
 <td><code class="docutils literal notranslate">v6.0.0 -> latest</code></td> </table>
 </div>
 </li>
            <li> <span class="li-head">videofilter</span> - Video filter profiles and settings. <span class="li-normal">type: str</span> <span class="li-normal">choices: none, read, read-write</span>
 <a id='label102' href="javascript:ContentClick('label103', 'label102');" onmouseover="ContentPreview('label103');" onmouseout="ContentUnpreview('label103');" title="click to collapse or expand..."> more... </a>
 <div id="label103" style="display:none">
 <table border="1">
 <tr>
 <td></td>
 <td colspan="1">Supported Version Ranges</td>
 </tr>
 <tr>
 <td>videofilter</td>
 <td><code class="docutils literal notranslate">v7.2.0 -> latest </code></td>
 </tr>
 <tr>
 <td>[none]</td>
 <td><code class="docutils literal notranslate">v6.0.0 -> latest</code></td> <tr>
 <td>[read]</td>
 <td><code class="docutils literal notranslate">v6.0.0 -> latest</code></td> <tr>
 <td>[read-write]</td>
 <td><code class="docutils literal notranslate">v6.0.0 -> latest</code></td> </table>
 </div>
 </li>
            <li> <span class="li-head">virtual_patch</span> - Virtual patch profiles and settings. <span class="li-normal">type: str</span> <span class="li-normal">choices: none, read, read-write</span>
 <a id='label104' href="javascript:ContentClick('label105', 'label104');" onmouseover="ContentPreview('label105');" onmouseout="ContentUnpreview('label105');" title="click to collapse or expand..."> more... </a>
 <div id="label105" style="display:none">
 <table border="1">
 <tr>
 <td></td>
 <td colspan="1">Supported Version Ranges</td>
 </tr>
 <tr>
 <td>virtual_patch</td>
 <td><code class="docutils literal notranslate">v7.4.1 -> latest </code></td>
 </tr>
 <tr>
 <td>[none]</td>
 <td><code class="docutils literal notranslate">v6.0.0 -> latest</code></td> <tr>
 <td>[read]</td>
 <td><code class="docutils literal notranslate">v6.0.0 -> latest</code></td> <tr>
 <td>[read-write]</td>
 <td><code class="docutils literal notranslate">v6.0.0 -> latest</code></td> </table>
 </div>
 </li>
            <li> <span class="li-head">voip</span> - VoIP profiles and settings. <span class="li-normal">type: str</span> <span class="li-normal">choices: none, read, read-write</span>
 <a id='label106' href="javascript:ContentClick('label107', 'label106');" onmouseover="ContentPreview('label107');" onmouseout="ContentUnpreview('label107');" title="click to collapse or expand..."> more... </a>
 <div id="label107" style="display:none">
 <table border="1">
 <tr>
 <td></td>
 <td colspan="1">Supported Version Ranges</td>
 </tr>
 <tr>
 <td>voip</td>
 <td><code class="docutils literal notranslate">v6.0.0 -> latest </code></td>
 </tr>
 <tr>
 <td>[none]</td>
 <td><code class="docutils literal notranslate">v6.0.0 -> latest</code></td> <tr>
 <td>[read]</td>
 <td><code class="docutils literal notranslate">v6.0.0 -> latest</code></td> <tr>
 <td>[read-write]</td>
 <td><code class="docutils literal notranslate">v6.0.0 -> latest</code></td> </table>
 </div>
 </li>
            <li> <span class="li-head">waf</span> - Web Application Firewall profiles and settings. <span class="li-normal">type: str</span> <span class="li-normal">choices: none, read, read-write</span>
 <a id='label108' href="javascript:ContentClick('label109', 'label108');" onmouseover="ContentPreview('label109');" onmouseout="ContentUnpreview('label109');" title="click to collapse or expand..."> more... </a>
 <div id="label109" style="display:none">
 <table border="1">
 <tr>
 <td></td>
 <td colspan="1">Supported Version Ranges</td>
 </tr>
 <tr>
 <td>waf</td>
 <td><code class="docutils literal notranslate">v6.0.0 -> latest </code></td>
 </tr>
 <tr>
 <td>[none]</td>
 <td><code class="docutils literal notranslate">v6.0.0 -> latest</code></td> <tr>
 <td>[read]</td>
 <td><code class="docutils literal notranslate">v6.0.0 -> latest</code></td> <tr>
 <td>[read-write]</td>
 <td><code class="docutils literal notranslate">v6.0.0 -> latest</code></td> </table>
 </div>
 </li>
            <li> <span class="li-head">webfilter</span> - Web Filter profiles and settings. <span class="li-normal">type: str</span> <span class="li-normal">choices: none, read, read-write</span>
 <a id='label110' href="javascript:ContentClick('label111', 'label110');" onmouseover="ContentPreview('label111');" onmouseout="ContentUnpreview('label111');" title="click to collapse or expand..."> more... </a>
 <div id="label111" style="display:none">
 <table border="1">
 <tr>
 <td></td>
 <td colspan="1">Supported Version Ranges</td>
 </tr>
 <tr>
 <td>webfilter</td>
 <td><code class="docutils literal notranslate">v6.0.0 -> latest </code></td>
 </tr>
 <tr>
 <td>[none]</td>
 <td><code class="docutils literal notranslate">v6.0.0 -> latest</code></td> <tr>
 <td>[read]</td>
 <td><code class="docutils literal notranslate">v6.0.0 -> latest</code></td> <tr>
 <td>[read-write]</td>
 <td><code class="docutils literal notranslate">v6.0.0 -> latest</code></td> </table>
 </div>
 </li>
            </ul>
        <li> <span class="li-head">vpngrp</span> - Administrator access to IPsec, SSL, PPTP, and L2TP VPN. <span class="li-normal">type: str</span> <span class="li-normal">choices: none, read, read-write</span>
 <a id='label112' href="javascript:ContentClick('label113', 'label112');" onmouseover="ContentPreview('label113');" onmouseout="ContentUnpreview('label113');" title="click to collapse or expand..."> more... </a>
 <div id="label113" style="display:none">
 <table border="1">
 <tr>
 <td></td>
 <td colspan="1">Supported Version Ranges</td>
 </tr>
 <tr>
 <td>vpngrp</td>
 <td><code class="docutils literal notranslate">v6.0.0 -> latest </code></td>
 </tr>
 <tr>
 <td>[none]</td>
 <td><code class="docutils literal notranslate">v6.0.0 -> latest</code></td> <tr>
 <td>[read]</td>
 <td><code class="docutils literal notranslate">v6.0.0 -> latest</code></td> <tr>
 <td>[read-write]</td>
 <td><code class="docutils literal notranslate">v6.0.0 -> latest</code></td> </table>
 </div>
 </li>
        <li> <span class="li-head">wanoptgrp</span> - Administrator access to WAN Opt & Cache. <span class="li-normal">type: str</span> <span class="li-normal">choices: none, read, read-write</span>
 <a id='label114' href="javascript:ContentClick('label115', 'label114');" onmouseover="ContentPreview('label115');" onmouseout="ContentUnpreview('label115');" title="click to collapse or expand..."> more... </a>
 <div id="label115" style="display:none">
 <table border="1">
 <tr>
 <td></td>
 <td colspan="1">Supported Version Ranges</td>
 </tr>
 <tr>
 <td>wanoptgrp</td>
 <td><code class="docutils literal notranslate">v6.0.0 -> latest </code></td>
 </tr>
 <tr>
 <td>[none]</td>
 <td><code class="docutils literal notranslate">v6.0.0 -> latest</code></td> <tr>
 <td>[read]</td>
 <td><code class="docutils literal notranslate">v6.0.0 -> latest</code></td> <tr>
 <td>[read-write]</td>
 <td><code class="docutils literal notranslate">v6.0.0 -> latest</code></td> </table>
 </div>
 </li>
        <li> <span class="li-head">wifi</span> - Administrator access to the WiFi controller and Switch controller. <span class="li-normal">type: str</span> <span class="li-normal">choices: none, read, read-write</span>
 <a id='label116' href="javascript:ContentClick('label117', 'label116');" onmouseover="ContentPreview('label117');" onmouseout="ContentUnpreview('label117');" title="click to collapse or expand..."> more... </a>
 <div id="label117" style="display:none">
 <table border="1">
 <tr>
 <td></td>
 <td colspan="1">Supported Version Ranges</td>
 </tr>
 <tr>
 <td>wifi</td>
 <td><code class="docutils literal notranslate">v6.0.0 -> latest </code></td>
 </tr>
 <tr>
 <td>[none]</td>
 <td><code class="docutils literal notranslate">v6.0.0 -> latest</code></td> <tr>
 <td>[read]</td>
 <td><code class="docutils literal notranslate">v6.0.0 -> latest</code></td> <tr>
 <td>[read-write]</td>
 <td><code class="docutils literal notranslate">v6.0.0 -> latest</code></td> </table>
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
    
    - name: Configure access profiles for system administrators.
      fortinet.fortios.fortios_system_accprofile:
          vdom: "{{ vdom }}"
          state: "present"
          access_token: "<your_own_value>"
          system_accprofile:
              admintimeout: "10"
              admintimeout_override: "enable"
              authgrp: "none"
              comments: "<your_own_value>"
              ftviewgrp: "none"
              fwgrp: "none"
              fwgrp_permission:
                  address: "none"
                  others: "none"
                  policy: "none"
                  schedule: "none"
                  service: "none"
              loggrp: "none"
              loggrp_permission:
                  config: "none"
                  data_access: "none"
                  report_access: "none"
                  threat_weight: "none"
              name: "default_name_21"
              netgrp: "none"
              netgrp_permission:
                  cfg: "none"
                  packet_capture: "none"
                  route_cfg: "none"
              scope: "vdom"
              secfabgrp: "none"
              sysgrp: "none"
              sysgrp_permission:
                  admin: "none"
                  cfg: "none"
                  mnt: "none"
                  upd: "none"
              system_diagnostics: "enable"
              system_execute_ssh: "enable"
              system_execute_telnet: "enable"
              utmgrp: "none"
              utmgrp_permission:
                  antivirus: "none"
                  application_control: "none"
                  casb: "none"
                  data_leak_prevention: "none"
                  data_loss_prevention: "none"
                  dnsfilter: "none"
                  emailfilter: "none"
                  endpoint_control: "none"
                  file_filter: "none"
                  icap: "none"
                  ips: "none"
                  mmsgtp: "none"
                  spamfilter: "none"
                  videofilter: "none"
                  virtual_patch: "none"
                  voip: "none"
                  waf: "none"
                  webfilter: "none"
              vpngrp: "none"
              wanoptgrp: "none"
              wifi: "none"


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
