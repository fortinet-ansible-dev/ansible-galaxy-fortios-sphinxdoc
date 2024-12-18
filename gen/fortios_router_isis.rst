:source: fortios_router_isis.py

:orphan:

.. fortios_router_isis:

fortios_router_isis -- Configure IS-IS in Fortinet's FortiOS and FortiGate.
+++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++

.. versionadded:: 2.0.0

.. contents::
   :local:
   :depth: 1


Synopsis
--------
- This module is able to configure a FortiGate or FortiOS (FOS) device by allowing the user to set and modify router feature and isis category. Examples include all parameters and values need to be adjusted to datasources before usage. Tested with FOS v6.0.0



Requirements
------------
The below requirements are needed on the host that executes this module.

- ansible>=2.15


Tips
----
Using member operation to add an element to an existing object.

FortiOS Version Compatibility
-----------------------------
Supported Version Ranges: v6.0.0 -> v7.6.0


Parameters
----------


.. raw:: html

    <ul>
    <li> <span class="li-head">access_token</span> - Token-based authentication. Generated from GUI of Fortigate. <span class="li-normal">type: str</span> <span class="li-required">required: false</span> </li>
    <li> <span class="li-head">enable_log</span> - Enable/Disable logging for task. <span class="li-normal">type: bool</span> <span class="li-required">required: false</span> <span class="li-normal">default: False</span> </li>
    <li> <span class="li-head">vdom</span> - Virtual domain, among those defined previously. A vdom is a virtual instance of the FortiGate that can be configured and used as a different unit. <span class="li-normal">type: str</span> <span class="li-normal">default: root</span> </li>
    <li> <span class="li-head">member_path</span> - Member attribute path to operate on. <span class="li-normal">type: str</span> </li>
    <li> <span class="li-head">member_state</span> - Add or delete a member under specified attribute path. <span class="li-normal">type: str</span> <span class="li-normal">choices: present, absent</span> </li>
    <li> <span class="li-head">router_isis</span> - Configure IS-IS. <span class="li-normal">type: dict</span>
 <a id='label0' href="javascript:ContentClick('label1', 'label0');" onmouseover="ContentPreview('label1');" onmouseout="ContentUnpreview('label1');" title="click to collapse or expand..."> more... </a>
 <div id="label1" style="display:none">
 <table border="1">
 <tr>
 <td></td><td colspan="1">Supported Version Ranges</td>
 </tr>
 <tr>
 <td>router_isis</td>
 <td><code class="docutils literal notranslate">v6.0.0 -> 7.6.0 </code></td>
 </tr>
 </table>
 </div>
 </li>
        <ul class="ul-self">
        <li> <span class="li-head">adjacency_check</span> - Enable/disable adjacency check. <span class="li-normal">type: str</span> <span class="li-normal">choices: enable, disable</span>
 <a id='label2' href="javascript:ContentClick('label3', 'label2');" onmouseover="ContentPreview('label3');" onmouseout="ContentUnpreview('label3');" title="click to collapse or expand..."> more... </a>
 <div id="label3" style="display:none">
 <table border="1">
 <tr>
 <td></td>
 <td colspan="1">Supported Version Ranges</td>
 </tr>
 <tr>
 <td>adjacency_check</td>
 <td><code class="docutils literal notranslate">v6.0.0 -> 7.6.0 </code></td>
 </tr>
 <tr>
 <td>[enable]</td>
 <td><code class="docutils literal notranslate">v6.0.0 -> 7.6.0</code></td>
 <tr>
 <td>[disable]</td>
 <td><code class="docutils literal notranslate">v6.0.0 -> 7.6.0</code></td>
 </table>
 </div>
 </li>
        <li> <span class="li-head">adjacency_check6</span> - Enable/disable IPv6 adjacency check. <span class="li-normal">type: str</span> <span class="li-normal">choices: enable, disable</span>
 <a id='label4' href="javascript:ContentClick('label5', 'label4');" onmouseover="ContentPreview('label5');" onmouseout="ContentUnpreview('label5');" title="click to collapse or expand..."> more... </a>
 <div id="label5" style="display:none">
 <table border="1">
 <tr>
 <td></td>
 <td colspan="1">Supported Version Ranges</td>
 </tr>
 <tr>
 <td>adjacency_check6</td>
 <td><code class="docutils literal notranslate">v6.0.0 -> 7.6.0 </code></td>
 </tr>
 <tr>
 <td>[enable]</td>
 <td><code class="docutils literal notranslate">v6.0.0 -> 7.6.0</code></td>
 <tr>
 <td>[disable]</td>
 <td><code class="docutils literal notranslate">v6.0.0 -> 7.6.0</code></td>
 </table>
 </div>
 </li>
        <li> <span class="li-head">adv_passive_only</span> - Enable/disable IS-IS advertisement of passive interfaces only. <span class="li-normal">type: str</span> <span class="li-normal">choices: enable, disable</span>
 <a id='label6' href="javascript:ContentClick('label7', 'label6');" onmouseover="ContentPreview('label7');" onmouseout="ContentUnpreview('label7');" title="click to collapse or expand..."> more... </a>
 <div id="label7" style="display:none">
 <table border="1">
 <tr>
 <td></td>
 <td colspan="1">Supported Version Ranges</td>
 </tr>
 <tr>
 <td>adv_passive_only</td>
 <td><code class="docutils literal notranslate">v6.0.0 -> 7.6.0 </code></td>
 </tr>
 <tr>
 <td>[enable]</td>
 <td><code class="docutils literal notranslate">v6.0.0 -> 7.6.0</code></td>
 <tr>
 <td>[disable]</td>
 <td><code class="docutils literal notranslate">v6.0.0 -> 7.6.0</code></td>
 </table>
 </div>
 </li>
        <li> <span class="li-head">adv_passive_only6</span> - Enable/disable IPv6 IS-IS advertisement of passive interfaces only. <span class="li-normal">type: str</span> <span class="li-normal">choices: enable, disable</span>
 <a id='label8' href="javascript:ContentClick('label9', 'label8');" onmouseover="ContentPreview('label9');" onmouseout="ContentUnpreview('label9');" title="click to collapse or expand..."> more... </a>
 <div id="label9" style="display:none">
 <table border="1">
 <tr>
 <td></td>
 <td colspan="1">Supported Version Ranges</td>
 </tr>
 <tr>
 <td>adv_passive_only6</td>
 <td><code class="docutils literal notranslate">v6.0.0 -> 7.6.0 </code></td>
 </tr>
 <tr>
 <td>[enable]</td>
 <td><code class="docutils literal notranslate">v6.0.0 -> 7.6.0</code></td>
 <tr>
 <td>[disable]</td>
 <td><code class="docutils literal notranslate">v6.0.0 -> 7.6.0</code></td>
 </table>
 </div>
 </li>
        <li> <span class="li-head">auth_keychain_l1</span> - Authentication key-chain for level 1 PDUs. Source router.key-chain.name. <span class="li-normal">type: str</span>
 <a id='label10' href="javascript:ContentClick('label11', 'label10');" onmouseover="ContentPreview('label11');" onmouseout="ContentUnpreview('label11');" title="click to collapse or expand..."> more... </a>
 <div id="label11" style="display:none">
 <table border="1">
 <tr>
 <td></td>
 <td colspan="1">Supported Version Ranges</td>
 </tr>
 <tr>
 <td>auth_keychain_l1</td>
 <td><code class="docutils literal notranslate">v6.0.0 -> 7.6.0 </code></td>
 </tr>
 </table>
 </div>
 </li>
        <li> <span class="li-head">auth_keychain_l2</span> - Authentication key-chain for level 2 PDUs. Source router.key-chain.name. <span class="li-normal">type: str</span>
 <a id='label12' href="javascript:ContentClick('label13', 'label12');" onmouseover="ContentPreview('label13');" onmouseout="ContentUnpreview('label13');" title="click to collapse or expand..."> more... </a>
 <div id="label13" style="display:none">
 <table border="1">
 <tr>
 <td></td>
 <td colspan="1">Supported Version Ranges</td>
 </tr>
 <tr>
 <td>auth_keychain_l2</td>
 <td><code class="docutils literal notranslate">v6.0.0 -> 7.6.0 </code></td>
 </tr>
 </table>
 </div>
 </li>
        <li> <span class="li-head">auth_mode_l1</span> - Level 1 authentication mode. <span class="li-normal">type: str</span> <span class="li-normal">choices: password, md5</span>
 <a id='label14' href="javascript:ContentClick('label15', 'label14');" onmouseover="ContentPreview('label15');" onmouseout="ContentUnpreview('label15');" title="click to collapse or expand..."> more... </a>
 <div id="label15" style="display:none">
 <table border="1">
 <tr>
 <td></td>
 <td colspan="1">Supported Version Ranges</td>
 </tr>
 <tr>
 <td>auth_mode_l1</td>
 <td><code class="docutils literal notranslate">v6.0.0 -> 7.6.0 </code></td>
 </tr>
 <tr>
 <td>[password]</td>
 <td><code class="docutils literal notranslate">v6.0.0 -> 7.6.0</code></td>
 <tr>
 <td>[md5]</td>
 <td><code class="docutils literal notranslate">v6.0.0 -> 7.6.0</code></td>
 </table>
 </div>
 </li>
        <li> <span class="li-head">auth_mode_l2</span> - Level 2 authentication mode. <span class="li-normal">type: str</span> <span class="li-normal">choices: password, md5</span>
 <a id='label16' href="javascript:ContentClick('label17', 'label16');" onmouseover="ContentPreview('label17');" onmouseout="ContentUnpreview('label17');" title="click to collapse or expand..."> more... </a>
 <div id="label17" style="display:none">
 <table border="1">
 <tr>
 <td></td>
 <td colspan="1">Supported Version Ranges</td>
 </tr>
 <tr>
 <td>auth_mode_l2</td>
 <td><code class="docutils literal notranslate">v6.0.0 -> 7.6.0 </code></td>
 </tr>
 <tr>
 <td>[password]</td>
 <td><code class="docutils literal notranslate">v6.0.0 -> 7.6.0</code></td>
 <tr>
 <td>[md5]</td>
 <td><code class="docutils literal notranslate">v6.0.0 -> 7.6.0</code></td>
 </table>
 </div>
 </li>
        <li> <span class="li-head">auth_password_l1</span> - Authentication password for level 1 PDUs. <span class="li-normal">type: str</span>
 <a id='label18' href="javascript:ContentClick('label19', 'label18');" onmouseover="ContentPreview('label19');" onmouseout="ContentUnpreview('label19');" title="click to collapse or expand..."> more... </a>
 <div id="label19" style="display:none">
 <table border="1">
 <tr>
 <td></td>
 <td colspan="1">Supported Version Ranges</td>
 </tr>
 <tr>
 <td>auth_password_l1</td>
 <td><code class="docutils literal notranslate">v6.0.0 -> 7.6.0 </code></td>
 </tr>
 </table>
 </div>
 </li>
        <li> <span class="li-head">auth_password_l2</span> - Authentication password for level 2 PDUs. <span class="li-normal">type: str</span>
 <a id='label20' href="javascript:ContentClick('label21', 'label20');" onmouseover="ContentPreview('label21');" onmouseout="ContentUnpreview('label21');" title="click to collapse or expand..."> more... </a>
 <div id="label21" style="display:none">
 <table border="1">
 <tr>
 <td></td>
 <td colspan="1">Supported Version Ranges</td>
 </tr>
 <tr>
 <td>auth_password_l2</td>
 <td><code class="docutils literal notranslate">v6.0.0 -> 7.6.0 </code></td>
 </tr>
 </table>
 </div>
 </li>
        <li> <span class="li-head">auth_sendonly_l1</span> - Enable/disable level 1 authentication send-only. <span class="li-normal">type: str</span> <span class="li-normal">choices: enable, disable</span>
 <a id='label22' href="javascript:ContentClick('label23', 'label22');" onmouseover="ContentPreview('label23');" onmouseout="ContentUnpreview('label23');" title="click to collapse or expand..."> more... </a>
 <div id="label23" style="display:none">
 <table border="1">
 <tr>
 <td></td>
 <td colspan="1">Supported Version Ranges</td>
 </tr>
 <tr>
 <td>auth_sendonly_l1</td>
 <td><code class="docutils literal notranslate">v6.0.0 -> 7.6.0 </code></td>
 </tr>
 <tr>
 <td>[enable]</td>
 <td><code class="docutils literal notranslate">v6.0.0 -> 7.6.0</code></td>
 <tr>
 <td>[disable]</td>
 <td><code class="docutils literal notranslate">v6.0.0 -> 7.6.0</code></td>
 </table>
 </div>
 </li>
        <li> <span class="li-head">auth_sendonly_l2</span> - Enable/disable level 2 authentication send-only. <span class="li-normal">type: str</span> <span class="li-normal">choices: enable, disable</span>
 <a id='label24' href="javascript:ContentClick('label25', 'label24');" onmouseover="ContentPreview('label25');" onmouseout="ContentUnpreview('label25');" title="click to collapse or expand..."> more... </a>
 <div id="label25" style="display:none">
 <table border="1">
 <tr>
 <td></td>
 <td colspan="1">Supported Version Ranges</td>
 </tr>
 <tr>
 <td>auth_sendonly_l2</td>
 <td><code class="docutils literal notranslate">v6.0.0 -> 7.6.0 </code></td>
 </tr>
 <tr>
 <td>[enable]</td>
 <td><code class="docutils literal notranslate">v6.0.0 -> 7.6.0</code></td>
 <tr>
 <td>[disable]</td>
 <td><code class="docutils literal notranslate">v6.0.0 -> 7.6.0</code></td>
 </table>
 </div>
 </li>
        <li> <span class="li-head">default_originate</span> - Enable/disable distribution of default route information. <span class="li-normal">type: str</span> <span class="li-normal">choices: enable, disable</span>
 <a id='label26' href="javascript:ContentClick('label27', 'label26');" onmouseover="ContentPreview('label27');" onmouseout="ContentUnpreview('label27');" title="click to collapse or expand..."> more... </a>
 <div id="label27" style="display:none">
 <table border="1">
 <tr>
 <td></td>
 <td colspan="1">Supported Version Ranges</td>
 </tr>
 <tr>
 <td>default_originate</td>
 <td><code class="docutils literal notranslate">v6.0.0 -> 7.6.0 </code></td>
 </tr>
 <tr>
 <td>[enable]</td>
 <td><code class="docutils literal notranslate">v6.0.0 -> 7.6.0</code></td>
 <tr>
 <td>[disable]</td>
 <td><code class="docutils literal notranslate">v6.0.0 -> 7.6.0</code></td>
 </table>
 </div>
 </li>
        <li> <span class="li-head">default_originate6</span> - Enable/disable distribution of default IPv6 route information. <span class="li-normal">type: str</span> <span class="li-normal">choices: enable, disable</span>
 <a id='label28' href="javascript:ContentClick('label29', 'label28');" onmouseover="ContentPreview('label29');" onmouseout="ContentUnpreview('label29');" title="click to collapse or expand..."> more... </a>
 <div id="label29" style="display:none">
 <table border="1">
 <tr>
 <td></td>
 <td colspan="1">Supported Version Ranges</td>
 </tr>
 <tr>
 <td>default_originate6</td>
 <td><code class="docutils literal notranslate">v6.0.0 -> 7.6.0 </code></td>
 </tr>
 <tr>
 <td>[enable]</td>
 <td><code class="docutils literal notranslate">v6.0.0 -> 7.6.0</code></td>
 <tr>
 <td>[disable]</td>
 <td><code class="docutils literal notranslate">v6.0.0 -> 7.6.0</code></td>
 </table>
 </div>
 </li>
        <li> <span class="li-head">dynamic_hostname</span> - Enable/disable dynamic hostname. <span class="li-normal">type: str</span> <span class="li-normal">choices: enable, disable</span>
 <a id='label30' href="javascript:ContentClick('label31', 'label30');" onmouseover="ContentPreview('label31');" onmouseout="ContentUnpreview('label31');" title="click to collapse or expand..."> more... </a>
 <div id="label31" style="display:none">
 <table border="1">
 <tr>
 <td></td>
 <td colspan="1">Supported Version Ranges</td>
 </tr>
 <tr>
 <td>dynamic_hostname</td>
 <td><code class="docutils literal notranslate">v6.0.0 -> 7.6.0 </code></td>
 </tr>
 <tr>
 <td>[enable]</td>
 <td><code class="docutils literal notranslate">v6.0.0 -> 7.6.0</code></td>
 <tr>
 <td>[disable]</td>
 <td><code class="docutils literal notranslate">v6.0.0 -> 7.6.0</code></td>
 </table>
 </div>
 </li>
        <li> <span class="li-head">ignore_lsp_errors</span> - Enable/disable ignoring of LSP errors with bad checksums. <span class="li-normal">type: str</span> <span class="li-normal">choices: enable, disable</span>
 <a id='label32' href="javascript:ContentClick('label33', 'label32');" onmouseover="ContentPreview('label33');" onmouseout="ContentUnpreview('label33');" title="click to collapse or expand..."> more... </a>
 <div id="label33" style="display:none">
 <table border="1">
 <tr>
 <td></td>
 <td colspan="1">Supported Version Ranges</td>
 </tr>
 <tr>
 <td>ignore_lsp_errors</td>
 <td><code class="docutils literal notranslate">v6.0.0 -> 7.6.0 </code></td>
 </tr>
 <tr>
 <td>[enable]</td>
 <td><code class="docutils literal notranslate">v6.0.0 -> 7.6.0</code></td>
 <tr>
 <td>[disable]</td>
 <td><code class="docutils literal notranslate">v6.0.0 -> 7.6.0</code></td>
 </table>
 </div>
 </li>
        <li> <span class="li-head">is_type</span> - IS type. <span class="li-normal">type: str</span> <span class="li-normal">choices: level-1-2, level-1, level-2-only</span>
 <a id='label34' href="javascript:ContentClick('label35', 'label34');" onmouseover="ContentPreview('label35');" onmouseout="ContentUnpreview('label35');" title="click to collapse or expand..."> more... </a>
 <div id="label35" style="display:none">
 <table border="1">
 <tr>
 <td></td>
 <td colspan="1">Supported Version Ranges</td>
 </tr>
 <tr>
 <td>is_type</td>
 <td><code class="docutils literal notranslate">v6.0.0 -> 7.6.0 </code></td>
 </tr>
 <tr>
 <td>[level-1-2]</td>
 <td><code class="docutils literal notranslate">v6.0.0 -> 7.6.0</code></td>
 <tr>
 <td>[level-1]</td>
 <td><code class="docutils literal notranslate">v6.0.0 -> 7.6.0</code></td>
 <tr>
 <td>[level-2-only]</td>
 <td><code class="docutils literal notranslate">v6.0.0 -> 7.6.0</code></td>
 </table>
 </div>
 </li>
        <li> <span class="li-head">isis_interface</span> - IS-IS interface configuration. <span class="li-normal">type: list</span> <span style="font-family:'Courier New'" class="li-required">member_path: isis_interface:name</span>
 <a id='label36' href="javascript:ContentClick('label37', 'label36');" onmouseover="ContentPreview('label37');" onmouseout="ContentUnpreview('label37');" title="click to collapse or expand..."> more... </a>
 <div id="label37" style="display:none">
 <table border="1">
 <tr>
 <td></td><td colspan="1">Supported Version Ranges</td>
 </tr>
 <tr>
 <td>isis_interface</td>
 <td><code class="docutils literal notranslate">v6.0.0 -> 7.6.0 </code></td>
 </tr>
 </table>
 </div>
 </li>
            <ul class="ul-self">
            <li> <span class="li-head">auth_keychain_l1</span> - Authentication key-chain for level 1 PDUs. Source router.key-chain.name. <span class="li-normal">type: str</span>
 <a id='label38' href="javascript:ContentClick('label39', 'label38');" onmouseover="ContentPreview('label39');" onmouseout="ContentUnpreview('label39');" title="click to collapse or expand..."> more... </a>
 <div id="label39" style="display:none">
 <table border="1">
 <tr>
 <td></td>
 <td colspan="1">Supported Version Ranges</td>
 </tr>
 <tr>
 <td>auth_keychain_l1</td>
 <td><code class="docutils literal notranslate">v6.0.0 -> 7.6.0 </code></td>
 </tr>
 </table>
 </div>
 </li>
            <li> <span class="li-head">auth_keychain_l2</span> - Authentication key-chain for level 2 PDUs. Source router.key-chain.name. <span class="li-normal">type: str</span>
 <a id='label40' href="javascript:ContentClick('label41', 'label40');" onmouseover="ContentPreview('label41');" onmouseout="ContentUnpreview('label41');" title="click to collapse or expand..."> more... </a>
 <div id="label41" style="display:none">
 <table border="1">
 <tr>
 <td></td>
 <td colspan="1">Supported Version Ranges</td>
 </tr>
 <tr>
 <td>auth_keychain_l2</td>
 <td><code class="docutils literal notranslate">v6.0.0 -> 7.6.0 </code></td>
 </tr>
 </table>
 </div>
 </li>
            <li> <span class="li-head">auth_mode_l1</span> - Level 1 authentication mode. <span class="li-normal">type: str</span> <span class="li-normal">choices: md5, password</span>
 <a id='label42' href="javascript:ContentClick('label43', 'label42');" onmouseover="ContentPreview('label43');" onmouseout="ContentUnpreview('label43');" title="click to collapse or expand..."> more... </a>
 <div id="label43" style="display:none">
 <table border="1">
 <tr>
 <td></td>
 <td colspan="1">Supported Version Ranges</td>
 </tr>
 <tr>
 <td>auth_mode_l1</td>
 <td><code class="docutils literal notranslate">v6.0.0 -> 7.6.0 </code></td>
 </tr>
 <tr>
 <td>[md5]</td>
 <td><code class="docutils literal notranslate">v6.0.0 -> 7.6.0</code></td>
 <tr>
 <td>[password]</td>
 <td><code class="docutils literal notranslate">v6.0.0 -> 7.6.0</code></td>
 </table>
 </div>
 </li>
            <li> <span class="li-head">auth_mode_l2</span> - Level 2 authentication mode. <span class="li-normal">type: str</span> <span class="li-normal">choices: md5, password</span>
 <a id='label44' href="javascript:ContentClick('label45', 'label44');" onmouseover="ContentPreview('label45');" onmouseout="ContentUnpreview('label45');" title="click to collapse or expand..."> more... </a>
 <div id="label45" style="display:none">
 <table border="1">
 <tr>
 <td></td>
 <td colspan="1">Supported Version Ranges</td>
 </tr>
 <tr>
 <td>auth_mode_l2</td>
 <td><code class="docutils literal notranslate">v6.0.0 -> 7.6.0 </code></td>
 </tr>
 <tr>
 <td>[md5]</td>
 <td><code class="docutils literal notranslate">v6.0.0 -> 7.6.0</code></td>
 <tr>
 <td>[password]</td>
 <td><code class="docutils literal notranslate">v6.0.0 -> 7.6.0</code></td>
 </table>
 </div>
 </li>
            <li> <span class="li-head">auth_password_l1</span> - Authentication password for level 1 PDUs. <span class="li-normal">type: str</span>
 <a id='label46' href="javascript:ContentClick('label47', 'label46');" onmouseover="ContentPreview('label47');" onmouseout="ContentUnpreview('label47');" title="click to collapse or expand..."> more... </a>
 <div id="label47" style="display:none">
 <table border="1">
 <tr>
 <td></td>
 <td colspan="1">Supported Version Ranges</td>
 </tr>
 <tr>
 <td>auth_password_l1</td>
 <td><code class="docutils literal notranslate">v6.0.0 -> 7.6.0 </code></td>
 </tr>
 </table>
 </div>
 </li>
            <li> <span class="li-head">auth_password_l2</span> - Authentication password for level 2 PDUs. <span class="li-normal">type: str</span>
 <a id='label48' href="javascript:ContentClick('label49', 'label48');" onmouseover="ContentPreview('label49');" onmouseout="ContentUnpreview('label49');" title="click to collapse or expand..."> more... </a>
 <div id="label49" style="display:none">
 <table border="1">
 <tr>
 <td></td>
 <td colspan="1">Supported Version Ranges</td>
 </tr>
 <tr>
 <td>auth_password_l2</td>
 <td><code class="docutils literal notranslate">v6.0.0 -> 7.6.0 </code></td>
 </tr>
 </table>
 </div>
 </li>
            <li> <span class="li-head">auth_send_only_l1</span> - Enable/disable authentication send-only for level 1 PDUs. <span class="li-normal">type: str</span> <span class="li-normal">choices: enable, disable</span>
 <a id='label50' href="javascript:ContentClick('label51', 'label50');" onmouseover="ContentPreview('label51');" onmouseout="ContentUnpreview('label51');" title="click to collapse or expand..."> more... </a>
 <div id="label51" style="display:none">
 <table border="1">
 <tr>
 <td></td>
 <td colspan="1">Supported Version Ranges</td>
 </tr>
 <tr>
 <td>auth_send_only_l1</td>
 <td><code class="docutils literal notranslate">v6.0.0 -> 7.6.0 </code></td>
 </tr>
 <tr>
 <td>[enable]</td>
 <td><code class="docutils literal notranslate">v6.0.0 -> 7.6.0</code></td>
 <tr>
 <td>[disable]</td>
 <td><code class="docutils literal notranslate">v6.0.0 -> 7.6.0</code></td>
 </table>
 </div>
 </li>
            <li> <span class="li-head">auth_send_only_l2</span> - Enable/disable authentication send-only for level 2 PDUs. <span class="li-normal">type: str</span> <span class="li-normal">choices: enable, disable</span>
 <a id='label52' href="javascript:ContentClick('label53', 'label52');" onmouseover="ContentPreview('label53');" onmouseout="ContentUnpreview('label53');" title="click to collapse or expand..."> more... </a>
 <div id="label53" style="display:none">
 <table border="1">
 <tr>
 <td></td>
 <td colspan="1">Supported Version Ranges</td>
 </tr>
 <tr>
 <td>auth_send_only_l2</td>
 <td><code class="docutils literal notranslate">v6.0.0 -> 7.6.0 </code></td>
 </tr>
 <tr>
 <td>[enable]</td>
 <td><code class="docutils literal notranslate">v6.0.0 -> 7.6.0</code></td>
 <tr>
 <td>[disable]</td>
 <td><code class="docutils literal notranslate">v6.0.0 -> 7.6.0</code></td>
 </table>
 </div>
 </li>
            <li> <span class="li-head">circuit_type</span> - IS-IS interface"s circuit type. <span class="li-normal">type: str</span> <span class="li-normal">choices: level-1-2, level-1, level-2</span>
 <a id='label54' href="javascript:ContentClick('label55', 'label54');" onmouseover="ContentPreview('label55');" onmouseout="ContentUnpreview('label55');" title="click to collapse or expand..."> more... </a>
 <div id="label55" style="display:none">
 <table border="1">
 <tr>
 <td></td>
 <td colspan="1">Supported Version Ranges</td>
 </tr>
 <tr>
 <td>circuit_type</td>
 <td><code class="docutils literal notranslate">v6.0.0 -> 7.6.0 </code></td>
 </tr>
 <tr>
 <td>[level-1-2]</td>
 <td><code class="docutils literal notranslate">v6.0.0 -> 7.6.0</code></td>
 <tr>
 <td>[level-1]</td>
 <td><code class="docutils literal notranslate">v6.0.0 -> 7.6.0</code></td>
 <tr>
 <td>[level-2]</td>
 <td><code class="docutils literal notranslate">v6.0.0 -> 7.6.0</code></td>
 </table>
 </div>
 </li>
            <li> <span class="li-head">csnp_interval_l1</span> - Level 1 CSNP interval. <span class="li-normal">type: int</span>
 <a id='label56' href="javascript:ContentClick('label57', 'label56');" onmouseover="ContentPreview('label57');" onmouseout="ContentUnpreview('label57');" title="click to collapse or expand..."> more... </a>
 <div id="label57" style="display:none">
 <table border="1">
 <tr>
 <td></td>
 <td colspan="1">Supported Version Ranges</td>
 </tr>
 <tr>
 <td>csnp_interval_l1</td>
 <td><code class="docutils literal notranslate">v6.0.0 -> 7.6.0 </code></td>
 </tr>
 </table>
 </div>
 </li>
            <li> <span class="li-head">csnp_interval_l2</span> - Level 2 CSNP interval. <span class="li-normal">type: int</span>
 <a id='label58' href="javascript:ContentClick('label59', 'label58');" onmouseover="ContentPreview('label59');" onmouseout="ContentUnpreview('label59');" title="click to collapse or expand..."> more... </a>
 <div id="label59" style="display:none">
 <table border="1">
 <tr>
 <td></td>
 <td colspan="1">Supported Version Ranges</td>
 </tr>
 <tr>
 <td>csnp_interval_l2</td>
 <td><code class="docutils literal notranslate">v6.0.0 -> 7.6.0 </code></td>
 </tr>
 </table>
 </div>
 </li>
            <li> <span class="li-head">hello_interval_l1</span> - Level 1 hello interval. <span class="li-normal">type: int</span>
 <a id='label60' href="javascript:ContentClick('label61', 'label60');" onmouseover="ContentPreview('label61');" onmouseout="ContentUnpreview('label61');" title="click to collapse or expand..."> more... </a>
 <div id="label61" style="display:none">
 <table border="1">
 <tr>
 <td></td>
 <td colspan="1">Supported Version Ranges</td>
 </tr>
 <tr>
 <td>hello_interval_l1</td>
 <td><code class="docutils literal notranslate">v6.0.0 -> 7.6.0 </code></td>
 </tr>
 </table>
 </div>
 </li>
            <li> <span class="li-head">hello_interval_l2</span> - Level 2 hello interval. <span class="li-normal">type: int</span>
 <a id='label62' href="javascript:ContentClick('label63', 'label62');" onmouseover="ContentPreview('label63');" onmouseout="ContentUnpreview('label63');" title="click to collapse or expand..."> more... </a>
 <div id="label63" style="display:none">
 <table border="1">
 <tr>
 <td></td>
 <td colspan="1">Supported Version Ranges</td>
 </tr>
 <tr>
 <td>hello_interval_l2</td>
 <td><code class="docutils literal notranslate">v6.0.0 -> 7.6.0 </code></td>
 </tr>
 </table>
 </div>
 </li>
            <li> <span class="li-head">hello_multiplier_l1</span> - Level 1 multiplier for Hello holding time. <span class="li-normal">type: int</span>
 <a id='label64' href="javascript:ContentClick('label65', 'label64');" onmouseover="ContentPreview('label65');" onmouseout="ContentUnpreview('label65');" title="click to collapse or expand..."> more... </a>
 <div id="label65" style="display:none">
 <table border="1">
 <tr>
 <td></td>
 <td colspan="1">Supported Version Ranges</td>
 </tr>
 <tr>
 <td>hello_multiplier_l1</td>
 <td><code class="docutils literal notranslate">v6.0.0 -> 7.6.0 </code></td>
 </tr>
 </table>
 </div>
 </li>
            <li> <span class="li-head">hello_multiplier_l2</span> - Level 2 multiplier for Hello holding time. <span class="li-normal">type: int</span>
 <a id='label66' href="javascript:ContentClick('label67', 'label66');" onmouseover="ContentPreview('label67');" onmouseout="ContentUnpreview('label67');" title="click to collapse or expand..."> more... </a>
 <div id="label67" style="display:none">
 <table border="1">
 <tr>
 <td></td>
 <td colspan="1">Supported Version Ranges</td>
 </tr>
 <tr>
 <td>hello_multiplier_l2</td>
 <td><code class="docutils literal notranslate">v6.0.0 -> 7.6.0 </code></td>
 </tr>
 </table>
 </div>
 </li>
            <li> <span class="li-head">hello_padding</span> - Enable/disable padding to IS-IS hello packets. <span class="li-normal">type: str</span> <span class="li-normal">choices: enable, disable</span>
 <a id='label68' href="javascript:ContentClick('label69', 'label68');" onmouseover="ContentPreview('label69');" onmouseout="ContentUnpreview('label69');" title="click to collapse or expand..."> more... </a>
 <div id="label69" style="display:none">
 <table border="1">
 <tr>
 <td></td>
 <td colspan="1">Supported Version Ranges</td>
 </tr>
 <tr>
 <td>hello_padding</td>
 <td><code class="docutils literal notranslate">v6.0.0 -> 7.6.0 </code></td>
 </tr>
 <tr>
 <td>[enable]</td>
 <td><code class="docutils literal notranslate">v6.0.0 -> 7.6.0</code></td>
 <tr>
 <td>[disable]</td>
 <td><code class="docutils literal notranslate">v6.0.0 -> 7.6.0</code></td>
 </table>
 </div>
 </li>
            <li> <span class="li-head">lsp_interval</span> - LSP transmission interval (milliseconds). <span class="li-normal">type: int</span>
 <a id='label70' href="javascript:ContentClick('label71', 'label70');" onmouseover="ContentPreview('label71');" onmouseout="ContentUnpreview('label71');" title="click to collapse or expand..."> more... </a>
 <div id="label71" style="display:none">
 <table border="1">
 <tr>
 <td></td>
 <td colspan="1">Supported Version Ranges</td>
 </tr>
 <tr>
 <td>lsp_interval</td>
 <td><code class="docutils literal notranslate">v6.0.0 -> 7.6.0 </code></td>
 </tr>
 </table>
 </div>
 </li>
            <li> <span class="li-head">lsp_retransmit_interval</span> - LSP retransmission interval (sec). <span class="li-normal">type: int</span>
 <a id='label72' href="javascript:ContentClick('label73', 'label72');" onmouseover="ContentPreview('label73');" onmouseout="ContentUnpreview('label73');" title="click to collapse or expand..."> more... </a>
 <div id="label73" style="display:none">
 <table border="1">
 <tr>
 <td></td>
 <td colspan="1">Supported Version Ranges</td>
 </tr>
 <tr>
 <td>lsp_retransmit_interval</td>
 <td><code class="docutils literal notranslate">v6.0.0 -> 7.6.0 </code></td>
 </tr>
 </table>
 </div>
 </li>
            <li> <span class="li-head">mesh_group</span> - Enable/disable IS-IS mesh group. <span class="li-normal">type: str</span> <span class="li-normal">choices: enable, disable</span>
 <a id='label74' href="javascript:ContentClick('label75', 'label74');" onmouseover="ContentPreview('label75');" onmouseout="ContentUnpreview('label75');" title="click to collapse or expand..."> more... </a>
 <div id="label75" style="display:none">
 <table border="1">
 <tr>
 <td></td>
 <td colspan="1">Supported Version Ranges</td>
 </tr>
 <tr>
 <td>mesh_group</td>
 <td><code class="docutils literal notranslate">v6.0.0 -> 7.6.0 </code></td>
 </tr>
 <tr>
 <td>[enable]</td>
 <td><code class="docutils literal notranslate">v6.0.0 -> 7.6.0</code></td>
 <tr>
 <td>[disable]</td>
 <td><code class="docutils literal notranslate">v6.0.0 -> 7.6.0</code></td>
 </table>
 </div>
 </li>
            <li> <span class="li-head">mesh_group_id</span> - Mesh group ID <0-4294967295>, 0: mesh-group blocked. <span class="li-normal">type: int</span>
 <a id='label76' href="javascript:ContentClick('label77', 'label76');" onmouseover="ContentPreview('label77');" onmouseout="ContentUnpreview('label77');" title="click to collapse or expand..."> more... </a>
 <div id="label77" style="display:none">
 <table border="1">
 <tr>
 <td></td>
 <td colspan="1">Supported Version Ranges</td>
 </tr>
 <tr>
 <td>mesh_group_id</td>
 <td><code class="docutils literal notranslate">v6.0.0 -> 7.6.0 </code></td>
 </tr>
 </table>
 </div>
 </li>
            <li> <span class="li-head">metric_l1</span> - Level 1 metric for interface. <span class="li-normal">type: int</span>
 <a id='label78' href="javascript:ContentClick('label79', 'label78');" onmouseover="ContentPreview('label79');" onmouseout="ContentUnpreview('label79');" title="click to collapse or expand..."> more... </a>
 <div id="label79" style="display:none">
 <table border="1">
 <tr>
 <td></td>
 <td colspan="1">Supported Version Ranges</td>
 </tr>
 <tr>
 <td>metric_l1</td>
 <td><code class="docutils literal notranslate">v6.0.0 -> 7.6.0 </code></td>
 </tr>
 </table>
 </div>
 </li>
            <li> <span class="li-head">metric_l2</span> - Level 2 metric for interface. <span class="li-normal">type: int</span>
 <a id='label80' href="javascript:ContentClick('label81', 'label80');" onmouseover="ContentPreview('label81');" onmouseout="ContentUnpreview('label81');" title="click to collapse or expand..."> more... </a>
 <div id="label81" style="display:none">
 <table border="1">
 <tr>
 <td></td>
 <td colspan="1">Supported Version Ranges</td>
 </tr>
 <tr>
 <td>metric_l2</td>
 <td><code class="docutils literal notranslate">v6.0.0 -> 7.6.0 </code></td>
 </tr>
 </table>
 </div>
 </li>
            <li> <span class="li-head">name</span> - IS-IS interface name. Source system.interface.name. <span class="li-normal">type: str</span> <span class="li-required">required: true</span>
 <a id='label82' href="javascript:ContentClick('label83', 'label82');" onmouseover="ContentPreview('label83');" onmouseout="ContentUnpreview('label83');" title="click to collapse or expand..."> more... </a>
 <div id="label83" style="display:none">
 <table border="1">
 <tr>
 <td></td>
 <td colspan="1">Supported Version Ranges</td>
 </tr>
 <tr>
 <td>name</td>
 <td><code class="docutils literal notranslate">v6.0.0 -> 7.6.0 </code></td>
 </tr>
 </table>
 </div>
 </li>
            <li> <span class="li-head">network_type</span> - IS-IS interface"s network type. <span class="li-normal">type: str</span> <span class="li-normal">choices: broadcast, point-to-point, loopback</span>
 <a id='label84' href="javascript:ContentClick('label85', 'label84');" onmouseover="ContentPreview('label85');" onmouseout="ContentUnpreview('label85');" title="click to collapse or expand..."> more... </a>
 <div id="label85" style="display:none">
 <table border="1">
 <tr>
 <td></td>
 <td colspan="1">Supported Version Ranges</td>
 </tr>
 <tr>
 <td>network_type</td>
 <td><code class="docutils literal notranslate">v6.0.0 -> 7.6.0 </code></td>
 </tr>
 <tr>
 <td>[broadcast]</td>
 <td><code class="docutils literal notranslate">v6.0.0 -> 7.6.0</code></td>
 <tr>
 <td>[point-to-point]</td>
 <td><code class="docutils literal notranslate">v6.0.0 -> 7.6.0</code></td>
 <tr>
 <td>[loopback]</td>
 <td><code class="docutils literal notranslate">v6.0.0 -> 7.6.0</code></td>
 </table>
 </div>
 </li>
            <li> <span class="li-head">priority_l1</span> - Level 1 priority. <span class="li-normal">type: int</span>
 <a id='label86' href="javascript:ContentClick('label87', 'label86');" onmouseover="ContentPreview('label87');" onmouseout="ContentUnpreview('label87');" title="click to collapse or expand..."> more... </a>
 <div id="label87" style="display:none">
 <table border="1">
 <tr>
 <td></td>
 <td colspan="1">Supported Version Ranges</td>
 </tr>
 <tr>
 <td>priority_l1</td>
 <td><code class="docutils literal notranslate">v6.0.0 -> 7.6.0 </code></td>
 </tr>
 </table>
 </div>
 </li>
            <li> <span class="li-head">priority_l2</span> - Level 2 priority. <span class="li-normal">type: int</span>
 <a id='label88' href="javascript:ContentClick('label89', 'label88');" onmouseover="ContentPreview('label89');" onmouseout="ContentUnpreview('label89');" title="click to collapse or expand..."> more... </a>
 <div id="label89" style="display:none">
 <table border="1">
 <tr>
 <td></td>
 <td colspan="1">Supported Version Ranges</td>
 </tr>
 <tr>
 <td>priority_l2</td>
 <td><code class="docutils literal notranslate">v6.0.0 -> 7.6.0 </code></td>
 </tr>
 </table>
 </div>
 </li>
            <li> <span class="li-head">status</span> - Enable/disable interface for IS-IS. <span class="li-normal">type: str</span> <span class="li-normal">choices: enable, disable</span>
 <a id='label90' href="javascript:ContentClick('label91', 'label90');" onmouseover="ContentPreview('label91');" onmouseout="ContentUnpreview('label91');" title="click to collapse or expand..."> more... </a>
 <div id="label91" style="display:none">
 <table border="1">
 <tr>
 <td></td>
 <td colspan="1">Supported Version Ranges</td>
 </tr>
 <tr>
 <td>status</td>
 <td><code class="docutils literal notranslate">v6.0.0 -> 7.6.0 </code></td>
 </tr>
 <tr>
 <td>[enable]</td>
 <td><code class="docutils literal notranslate">v6.0.0 -> 7.6.0</code></td>
 <tr>
 <td>[disable]</td>
 <td><code class="docutils literal notranslate">v6.0.0 -> 7.6.0</code></td>
 </table>
 </div>
 </li>
            <li> <span class="li-head">status6</span> - Enable/disable IPv6 interface for IS-IS. <span class="li-normal">type: str</span> <span class="li-normal">choices: enable, disable</span>
 <a id='label92' href="javascript:ContentClick('label93', 'label92');" onmouseover="ContentPreview('label93');" onmouseout="ContentUnpreview('label93');" title="click to collapse or expand..."> more... </a>
 <div id="label93" style="display:none">
 <table border="1">
 <tr>
 <td></td>
 <td colspan="1">Supported Version Ranges</td>
 </tr>
 <tr>
 <td>status6</td>
 <td><code class="docutils literal notranslate">v6.0.0 -> 7.6.0 </code></td>
 </tr>
 <tr>
 <td>[enable]</td>
 <td><code class="docutils literal notranslate">v6.0.0 -> 7.6.0</code></td>
 <tr>
 <td>[disable]</td>
 <td><code class="docutils literal notranslate">v6.0.0 -> 7.6.0</code></td>
 </table>
 </div>
 </li>
            <li> <span class="li-head">wide_metric_l1</span> - Level 1 wide metric for interface. <span class="li-normal">type: int</span>
 <a id='label94' href="javascript:ContentClick('label95', 'label94');" onmouseover="ContentPreview('label95');" onmouseout="ContentUnpreview('label95');" title="click to collapse or expand..."> more... </a>
 <div id="label95" style="display:none">
 <table border="1">
 <tr>
 <td></td>
 <td colspan="1">Supported Version Ranges</td>
 </tr>
 <tr>
 <td>wide_metric_l1</td>
 <td><code class="docutils literal notranslate">v6.0.0 -> 7.6.0 </code></td>
 </tr>
 </table>
 </div>
 </li>
            <li> <span class="li-head">wide_metric_l2</span> - Level 2 wide metric for interface. <span class="li-normal">type: int</span>
 <a id='label96' href="javascript:ContentClick('label97', 'label96');" onmouseover="ContentPreview('label97');" onmouseout="ContentUnpreview('label97');" title="click to collapse or expand..."> more... </a>
 <div id="label97" style="display:none">
 <table border="1">
 <tr>
 <td></td>
 <td colspan="1">Supported Version Ranges</td>
 </tr>
 <tr>
 <td>wide_metric_l2</td>
 <td><code class="docutils literal notranslate">v6.0.0 -> 7.6.0 </code></td>
 </tr>
 </table>
 </div>
 </li>
            </ul>
        <li> <span class="li-head">isis_net</span> - IS-IS net configuration. <span class="li-normal">type: list</span> <span style="font-family:'Courier New'" class="li-required">member_path: isis_net:id</span>
 <a id='label98' href="javascript:ContentClick('label99', 'label98');" onmouseover="ContentPreview('label99');" onmouseout="ContentUnpreview('label99');" title="click to collapse or expand..."> more... </a>
 <div id="label99" style="display:none">
 <table border="1">
 <tr>
 <td></td><td colspan="1">Supported Version Ranges</td>
 </tr>
 <tr>
 <td>isis_net</td>
 <td><code class="docutils literal notranslate">v6.0.0 -> 7.6.0 </code></td>
 </tr>
 </table>
 </div>
 </li>
            <ul class="ul-self">
            <li> <span class="li-head">id</span> - ISIS network ID. see <a href='#notes'>Notes</a>. <span class="li-normal">type: int</span> <span class="li-required">required: true</span>
 <a id='label100' href="javascript:ContentClick('label101', 'label100');" onmouseover="ContentPreview('label101');" onmouseout="ContentUnpreview('label101');" title="click to collapse or expand..."> more... </a>
 <div id="label101" style="display:none">
 <table border="1">
 <tr>
 <td></td>
 <td colspan="1">Supported Version Ranges</td>
 </tr>
 <tr>
 <td>id</td>
 <td><code class="docutils literal notranslate">v6.0.0 -> 7.6.0 </code></td>
 </tr>
 </table>
 </div>
 </li>
            <li> <span class="li-head">net</span> - IS-IS networks (format = xx.xxxx.  .xxxx.xx.). <span class="li-normal">type: str</span>
 <a id='label102' href="javascript:ContentClick('label103', 'label102');" onmouseover="ContentPreview('label103');" onmouseout="ContentUnpreview('label103');" title="click to collapse or expand..."> more... </a>
 <div id="label103" style="display:none">
 <table border="1">
 <tr>
 <td></td>
 <td colspan="1">Supported Version Ranges</td>
 </tr>
 <tr>
 <td>net</td>
 <td><code class="docutils literal notranslate">v6.0.0 -> 7.6.0 </code></td>
 </tr>
 </table>
 </div>
 </li>
            </ul>
        <li> <span class="li-head">lsp_gen_interval_l1</span> - Minimum interval for level 1 LSP regenerating. <span class="li-normal">type: int</span>
 <a id='label104' href="javascript:ContentClick('label105', 'label104');" onmouseover="ContentPreview('label105');" onmouseout="ContentUnpreview('label105');" title="click to collapse or expand..."> more... </a>
 <div id="label105" style="display:none">
 <table border="1">
 <tr>
 <td></td>
 <td colspan="1">Supported Version Ranges</td>
 </tr>
 <tr>
 <td>lsp_gen_interval_l1</td>
 <td><code class="docutils literal notranslate">v6.0.0 -> 7.6.0 </code></td>
 </tr>
 </table>
 </div>
 </li>
        <li> <span class="li-head">lsp_gen_interval_l2</span> - Minimum interval for level 2 LSP regenerating. <span class="li-normal">type: int</span>
 <a id='label106' href="javascript:ContentClick('label107', 'label106');" onmouseover="ContentPreview('label107');" onmouseout="ContentUnpreview('label107');" title="click to collapse or expand..."> more... </a>
 <div id="label107" style="display:none">
 <table border="1">
 <tr>
 <td></td>
 <td colspan="1">Supported Version Ranges</td>
 </tr>
 <tr>
 <td>lsp_gen_interval_l2</td>
 <td><code class="docutils literal notranslate">v6.0.0 -> 7.6.0 </code></td>
 </tr>
 </table>
 </div>
 </li>
        <li> <span class="li-head">lsp_refresh_interval</span> - LSP refresh time in seconds. <span class="li-normal">type: int</span>
 <a id='label108' href="javascript:ContentClick('label109', 'label108');" onmouseover="ContentPreview('label109');" onmouseout="ContentUnpreview('label109');" title="click to collapse or expand..."> more... </a>
 <div id="label109" style="display:none">
 <table border="1">
 <tr>
 <td></td>
 <td colspan="1">Supported Version Ranges</td>
 </tr>
 <tr>
 <td>lsp_refresh_interval</td>
 <td><code class="docutils literal notranslate">v6.0.0 -> 7.6.0 </code></td>
 </tr>
 </table>
 </div>
 </li>
        <li> <span class="li-head">max_lsp_lifetime</span> - Maximum LSP lifetime in seconds. <span class="li-normal">type: int</span>
 <a id='label110' href="javascript:ContentClick('label111', 'label110');" onmouseover="ContentPreview('label111');" onmouseout="ContentUnpreview('label111');" title="click to collapse or expand..."> more... </a>
 <div id="label111" style="display:none">
 <table border="1">
 <tr>
 <td></td>
 <td colspan="1">Supported Version Ranges</td>
 </tr>
 <tr>
 <td>max_lsp_lifetime</td>
 <td><code class="docutils literal notranslate">v6.0.0 -> 7.6.0 </code></td>
 </tr>
 </table>
 </div>
 </li>
        <li> <span class="li-head">metric_style</span> - Use old-style (ISO 10589) or new-style packet formats. <span class="li-normal">type: str</span> <span class="li-normal">choices: narrow, wide, transition, narrow-transition, narrow-transition-l1, narrow-transition-l2, wide-l1, wide-l2, wide-transition, wide-transition-l1, wide-transition-l2, transition-l1, transition-l2</span>
 <a id='label112' href="javascript:ContentClick('label113', 'label112');" onmouseover="ContentPreview('label113');" onmouseout="ContentUnpreview('label113');" title="click to collapse or expand..."> more... </a>
 <div id="label113" style="display:none">
 <table border="1">
 <tr>
 <td></td>
 <td colspan="1">Supported Version Ranges</td>
 </tr>
 <tr>
 <td>metric_style</td>
 <td><code class="docutils literal notranslate">v6.0.0 -> 7.6.0 </code></td>
 </tr>
 <tr>
 <td>[narrow]</td>
 <td><code class="docutils literal notranslate">v6.0.0 -> 7.6.0</code></td>
 <tr>
 <td>[wide]</td>
 <td><code class="docutils literal notranslate">v6.0.0 -> 7.6.0</code></td>
 <tr>
 <td>[transition]</td>
 <td><code class="docutils literal notranslate">v6.0.0 -> 7.6.0</code></td>
 <tr>
 <td>[narrow-transition]</td>
 <td><code class="docutils literal notranslate">v6.0.0 -> 7.6.0</code></td>
 <tr>
 <td>[narrow-transition-l1]</td>
 <td><code class="docutils literal notranslate">v6.0.0 -> 7.6.0</code></td>
 <tr>
 <td>[narrow-transition-l2]</td>
 <td><code class="docutils literal notranslate">v6.0.0 -> 7.6.0</code></td>
 <tr>
 <td>[wide-l1]</td>
 <td><code class="docutils literal notranslate">v6.0.0 -> 7.6.0</code></td>
 <tr>
 <td>[wide-l2]</td>
 <td><code class="docutils literal notranslate">v6.0.0 -> 7.6.0</code></td>
 <tr>
 <td>[wide-transition]</td>
 <td><code class="docutils literal notranslate">v6.0.0 -> 7.6.0</code></td>
 <tr>
 <td>[wide-transition-l1]</td>
 <td><code class="docutils literal notranslate">v6.0.0 -> 7.6.0</code></td>
 <tr>
 <td>[wide-transition-l2]</td>
 <td><code class="docutils literal notranslate">v6.0.0 -> 7.6.0</code></td>
 <tr>
 <td>[transition-l1]</td>
 <td><code class="docutils literal notranslate">v6.0.0 -> 7.6.0</code></td>
 <tr>
 <td>[transition-l2]</td>
 <td><code class="docutils literal notranslate">v6.0.0 -> 7.6.0</code></td>
 </table>
 </div>
 </li>
        <li> <span class="li-head">overload_bit</span> - Enable/disable signal other routers not to use us in SPF. <span class="li-normal">type: str</span> <span class="li-normal">choices: enable, disable</span>
 <a id='label114' href="javascript:ContentClick('label115', 'label114');" onmouseover="ContentPreview('label115');" onmouseout="ContentUnpreview('label115');" title="click to collapse or expand..."> more... </a>
 <div id="label115" style="display:none">
 <table border="1">
 <tr>
 <td></td>
 <td colspan="1">Supported Version Ranges</td>
 </tr>
 <tr>
 <td>overload_bit</td>
 <td><code class="docutils literal notranslate">v6.0.0 -> 7.6.0 </code></td>
 </tr>
 <tr>
 <td>[enable]</td>
 <td><code class="docutils literal notranslate">v6.0.0 -> 7.6.0</code></td>
 <tr>
 <td>[disable]</td>
 <td><code class="docutils literal notranslate">v6.0.0 -> 7.6.0</code></td>
 </table>
 </div>
 </li>
        <li> <span class="li-head">overload_bit_on_startup</span> - Overload-bit only temporarily after reboot. <span class="li-normal">type: int</span>
 <a id='label116' href="javascript:ContentClick('label117', 'label116');" onmouseover="ContentPreview('label117');" onmouseout="ContentUnpreview('label117');" title="click to collapse or expand..."> more... </a>
 <div id="label117" style="display:none">
 <table border="1">
 <tr>
 <td></td>
 <td colspan="1">Supported Version Ranges</td>
 </tr>
 <tr>
 <td>overload_bit_on_startup</td>
 <td><code class="docutils literal notranslate">v6.0.0 -> 7.6.0 </code></td>
 </tr>
 </table>
 </div>
 </li>
        <li> <span class="li-head">overload_bit_suppress</span> - Suppress overload-bit for the specific prefixes. <span class="li-normal">type: list</span> <span class="li-normal">choices: external, interlevel</span>
 <a id='label118' href="javascript:ContentClick('label119', 'label118');" onmouseover="ContentPreview('label119');" onmouseout="ContentUnpreview('label119');" title="click to collapse or expand..."> more... </a>
 <div id="label119" style="display:none">
 <table border="1">
 <tr>
 <td></td>
 <td colspan="1">Supported Version Ranges</td>
 </tr>
 <tr>
 <td>overload_bit_suppress</td>
 <td><code class="docutils literal notranslate">v6.0.0 -> 7.6.0 </code></td>
 </tr>
 <tr>
 <td>[external]</td>
 <td><code class="docutils literal notranslate">v6.0.0 -> 7.6.0</code></td>
 <tr>
 <td>[interlevel]</td>
 <td><code class="docutils literal notranslate">v6.0.0 -> 7.6.0</code></td>
 </table>
 </div>
 </li>
        <li> <span class="li-head">redistribute</span> - IS-IS redistribute protocols. <span class="li-normal">type: list</span> <span style="font-family:'Courier New'" class="li-required">member_path: redistribute:protocol</span>
 <a id='label120' href="javascript:ContentClick('label121', 'label120');" onmouseover="ContentPreview('label121');" onmouseout="ContentUnpreview('label121');" title="click to collapse or expand..."> more... </a>
 <div id="label121" style="display:none">
 <table border="1">
 <tr>
 <td></td><td colspan="2">Supported Version Ranges</td>
 </tr>
 <tr>
 <td>redistribute</td>
 <td><code class="docutils literal notranslate">v6.0.0 -> v7.0.5 </code></td>
 <td><code class="docutils literal notranslate">v7.2.0 -> v7.2.0 </code></td>
 </tr>
 </table>
 </div>
 </li>
            <ul class="ul-self">
            <li> <span class="li-head">level</span> - Level. <span class="li-normal">type: str</span> <span class="li-normal">choices: level-1-2, level-1, level-2</span>
 <a id='label122' href="javascript:ContentClick('label123', 'label122');" onmouseover="ContentPreview('label123');" onmouseout="ContentUnpreview('label123');" title="click to collapse or expand..."> more... </a>
 <div id="label123" style="display:none">
 <table border="1">
 <tr>
 <td></td>
 <td colspan="2">Supported Version Ranges</td>
 </tr>
 <tr>
 <td>level</td>
 <td><code class="docutils literal notranslate">v6.0.0 -> v7.0.5 </code></td>
 <td><code class="docutils literal notranslate">v7.2.0 -> v7.2.0 </code></td>
 </tr>
 <tr>
 <td>[level-1-2]</td>
 <td><code class="docutils literal notranslate">v6.0.0 -> v7.0.5</code></td>
 <tr>
 <td>[level-1]</td>
 <td><code class="docutils literal notranslate">v6.0.0 -> v7.0.5</code></td>
 <tr>
 <td>[level-2]</td>
 <td><code class="docutils literal notranslate">v6.0.0 -> v7.0.5</code></td>
 </table>
 </div>
 </li>
            <li> <span class="li-head">metric</span> - Metric. <span class="li-normal">type: int</span>
 <a id='label124' href="javascript:ContentClick('label125', 'label124');" onmouseover="ContentPreview('label125');" onmouseout="ContentUnpreview('label125');" title="click to collapse or expand..."> more... </a>
 <div id="label125" style="display:none">
 <table border="1">
 <tr>
 <td></td>
 <td colspan="2">Supported Version Ranges</td>
 </tr>
 <tr>
 <td>metric</td>
 <td><code class="docutils literal notranslate">v6.0.0 -> v7.0.5 </code></td>
 <td><code class="docutils literal notranslate">v7.2.0 -> v7.2.0 </code></td>
 </tr>
 </table>
 </div>
 </li>
            <li> <span class="li-head">metric_type</span> - Metric type. <span class="li-normal">type: str</span> <span class="li-normal">choices: external, internal</span>
 <a id='label126' href="javascript:ContentClick('label127', 'label126');" onmouseover="ContentPreview('label127');" onmouseout="ContentUnpreview('label127');" title="click to collapse or expand..."> more... </a>
 <div id="label127" style="display:none">
 <table border="1">
 <tr>
 <td></td>
 <td colspan="2">Supported Version Ranges</td>
 </tr>
 <tr>
 <td>metric_type</td>
 <td><code class="docutils literal notranslate">v6.0.0 -> v7.0.5 </code></td>
 <td><code class="docutils literal notranslate">v7.2.0 -> v7.2.0 </code></td>
 </tr>
 <tr>
 <td>[external]</td>
 <td><code class="docutils literal notranslate">v6.0.0 -> v7.0.5</code></td>
 <tr>
 <td>[internal]</td>
 <td><code class="docutils literal notranslate">v6.0.0 -> v7.0.5</code></td>
 </table>
 </div>
 </li>
            <li> <span class="li-head">protocol</span> - Protocol name. <span class="li-normal">type: str</span> <span class="li-required">required: true</span>
 <a id='label128' href="javascript:ContentClick('label129', 'label128');" onmouseover="ContentPreview('label129');" onmouseout="ContentUnpreview('label129');" title="click to collapse or expand..."> more... </a>
 <div id="label129" style="display:none">
 <table border="1">
 <tr>
 <td></td>
 <td colspan="2">Supported Version Ranges</td>
 </tr>
 <tr>
 <td>protocol</td>
 <td><code class="docutils literal notranslate">v6.0.0 -> v7.0.5 </code></td>
 <td><code class="docutils literal notranslate">v7.2.0 -> v7.2.0 </code></td>
 </tr>
 </table>
 </div>
 </li>
            <li> <span class="li-head">routemap</span> - Route map name. Source router.route-map.name. <span class="li-normal">type: str</span>
 <a id='label130' href="javascript:ContentClick('label131', 'label130');" onmouseover="ContentPreview('label131');" onmouseout="ContentUnpreview('label131');" title="click to collapse or expand..."> more... </a>
 <div id="label131" style="display:none">
 <table border="1">
 <tr>
 <td></td>
 <td colspan="2">Supported Version Ranges</td>
 </tr>
 <tr>
 <td>routemap</td>
 <td><code class="docutils literal notranslate">v6.0.0 -> v7.0.5 </code></td>
 <td><code class="docutils literal notranslate">v7.2.0 -> v7.2.0 </code></td>
 </tr>
 </table>
 </div>
 </li>
            <li> <span class="li-head">status</span> - Status. <span class="li-normal">type: str</span> <span class="li-normal">choices: enable, disable</span>
 <a id='label132' href="javascript:ContentClick('label133', 'label132');" onmouseover="ContentPreview('label133');" onmouseout="ContentUnpreview('label133');" title="click to collapse or expand..."> more... </a>
 <div id="label133" style="display:none">
 <table border="1">
 <tr>
 <td></td>
 <td colspan="2">Supported Version Ranges</td>
 </tr>
 <tr>
 <td>status</td>
 <td><code class="docutils literal notranslate">v6.0.0 -> v7.0.5 </code></td>
 <td><code class="docutils literal notranslate">v7.2.0 -> v7.2.0 </code></td>
 </tr>
 <tr>
 <td>[enable]</td>
 <td><code class="docutils literal notranslate">v6.0.0 -> v7.0.5</code></td>
 <tr>
 <td>[disable]</td>
 <td><code class="docutils literal notranslate">v6.0.0 -> v7.0.5</code></td>
 </table>
 </div>
 </li>
            </ul>
        <li> <span class="li-head">redistribute_l1</span> - Enable/disable redistribution of level 1 routes into level 2. <span class="li-normal">type: str</span> <span class="li-normal">choices: enable, disable</span>
 <a id='label134' href="javascript:ContentClick('label135', 'label134');" onmouseover="ContentPreview('label135');" onmouseout="ContentUnpreview('label135');" title="click to collapse or expand..."> more... </a>
 <div id="label135" style="display:none">
 <table border="1">
 <tr>
 <td></td>
 <td colspan="1">Supported Version Ranges</td>
 </tr>
 <tr>
 <td>redistribute_l1</td>
 <td><code class="docutils literal notranslate">v6.0.0 -> 7.6.0 </code></td>
 </tr>
 <tr>
 <td>[enable]</td>
 <td><code class="docutils literal notranslate">v6.0.0 -> 7.6.0</code></td>
 <tr>
 <td>[disable]</td>
 <td><code class="docutils literal notranslate">v6.0.0 -> 7.6.0</code></td>
 </table>
 </div>
 </li>
        <li> <span class="li-head">redistribute_l1_list</span> - Access-list for route redistribution from l1 to l2. Source router.access-list.name. <span class="li-normal">type: str</span>
 <a id='label136' href="javascript:ContentClick('label137', 'label136');" onmouseover="ContentPreview('label137');" onmouseout="ContentUnpreview('label137');" title="click to collapse or expand..."> more... </a>
 <div id="label137" style="display:none">
 <table border="1">
 <tr>
 <td></td>
 <td colspan="1">Supported Version Ranges</td>
 </tr>
 <tr>
 <td>redistribute_l1_list</td>
 <td><code class="docutils literal notranslate">v6.0.0 -> 7.6.0 </code></td>
 </tr>
 </table>
 </div>
 </li>
        <li> <span class="li-head">redistribute_l2</span> - Enable/disable redistribution of level 2 routes into level 1. <span class="li-normal">type: str</span> <span class="li-normal">choices: enable, disable</span>
 <a id='label138' href="javascript:ContentClick('label139', 'label138');" onmouseover="ContentPreview('label139');" onmouseout="ContentUnpreview('label139');" title="click to collapse or expand..."> more... </a>
 <div id="label139" style="display:none">
 <table border="1">
 <tr>
 <td></td>
 <td colspan="1">Supported Version Ranges</td>
 </tr>
 <tr>
 <td>redistribute_l2</td>
 <td><code class="docutils literal notranslate">v6.0.0 -> 7.6.0 </code></td>
 </tr>
 <tr>
 <td>[enable]</td>
 <td><code class="docutils literal notranslate">v6.0.0 -> 7.6.0</code></td>
 <tr>
 <td>[disable]</td>
 <td><code class="docutils literal notranslate">v6.0.0 -> 7.6.0</code></td>
 </table>
 </div>
 </li>
        <li> <span class="li-head">redistribute_l2_list</span> - Access-list for route redistribution from l2 to l1. Source router.access-list.name. <span class="li-normal">type: str</span>
 <a id='label140' href="javascript:ContentClick('label141', 'label140');" onmouseover="ContentPreview('label141');" onmouseout="ContentUnpreview('label141');" title="click to collapse or expand..."> more... </a>
 <div id="label141" style="display:none">
 <table border="1">
 <tr>
 <td></td>
 <td colspan="1">Supported Version Ranges</td>
 </tr>
 <tr>
 <td>redistribute_l2_list</td>
 <td><code class="docutils literal notranslate">v6.0.0 -> 7.6.0 </code></td>
 </tr>
 </table>
 </div>
 </li>
        <li> <span class="li-head">redistribute6</span> - IS-IS IPv6 redistribution for routing protocols. <span class="li-normal">type: list</span> <span style="font-family:'Courier New'" class="li-required">member_path: redistribute6:protocol</span>
 <a id='label142' href="javascript:ContentClick('label143', 'label142');" onmouseover="ContentPreview('label143');" onmouseout="ContentUnpreview('label143');" title="click to collapse or expand..."> more... </a>
 <div id="label143" style="display:none">
 <table border="1">
 <tr>
 <td></td><td colspan="2">Supported Version Ranges</td>
 </tr>
 <tr>
 <td>redistribute6</td>
 <td><code class="docutils literal notranslate">v6.0.0 -> v7.0.5 </code></td>
 <td><code class="docutils literal notranslate">v7.2.0 -> v7.2.0 </code></td>
 </tr>
 </table>
 </div>
 </li>
            <ul class="ul-self">
            <li> <span class="li-head">level</span> - Level. <span class="li-normal">type: str</span> <span class="li-normal">choices: level-1-2, level-1, level-2</span>
 <a id='label144' href="javascript:ContentClick('label145', 'label144');" onmouseover="ContentPreview('label145');" onmouseout="ContentUnpreview('label145');" title="click to collapse or expand..."> more... </a>
 <div id="label145" style="display:none">
 <table border="1">
 <tr>
 <td></td>
 <td colspan="2">Supported Version Ranges</td>
 </tr>
 <tr>
 <td>level</td>
 <td><code class="docutils literal notranslate">v6.0.0 -> v7.0.5 </code></td>
 <td><code class="docutils literal notranslate">v7.2.0 -> v7.2.0 </code></td>
 </tr>
 <tr>
 <td>[level-1-2]</td>
 <td><code class="docutils literal notranslate">v6.0.0 -> v7.0.5</code></td>
 <tr>
 <td>[level-1]</td>
 <td><code class="docutils literal notranslate">v6.0.0 -> v7.0.5</code></td>
 <tr>
 <td>[level-2]</td>
 <td><code class="docutils literal notranslate">v6.0.0 -> v7.0.5</code></td>
 </table>
 </div>
 </li>
            <li> <span class="li-head">metric</span> - Metric. <span class="li-normal">type: int</span>
 <a id='label146' href="javascript:ContentClick('label147', 'label146');" onmouseover="ContentPreview('label147');" onmouseout="ContentUnpreview('label147');" title="click to collapse or expand..."> more... </a>
 <div id="label147" style="display:none">
 <table border="1">
 <tr>
 <td></td>
 <td colspan="2">Supported Version Ranges</td>
 </tr>
 <tr>
 <td>metric</td>
 <td><code class="docutils literal notranslate">v6.0.0 -> v7.0.5 </code></td>
 <td><code class="docutils literal notranslate">v7.2.0 -> v7.2.0 </code></td>
 </tr>
 </table>
 </div>
 </li>
            <li> <span class="li-head">metric_type</span> - Metric type. <span class="li-normal">type: str</span> <span class="li-normal">choices: external, internal</span>
 <a id='label148' href="javascript:ContentClick('label149', 'label148');" onmouseover="ContentPreview('label149');" onmouseout="ContentUnpreview('label149');" title="click to collapse or expand..."> more... </a>
 <div id="label149" style="display:none">
 <table border="1">
 <tr>
 <td></td>
 <td colspan="2">Supported Version Ranges</td>
 </tr>
 <tr>
 <td>metric_type</td>
 <td><code class="docutils literal notranslate">v6.0.0 -> v7.0.5 </code></td>
 <td><code class="docutils literal notranslate">v7.2.0 -> v7.2.0 </code></td>
 </tr>
 <tr>
 <td>[external]</td>
 <td><code class="docutils literal notranslate">v6.0.0 -> v7.0.5</code></td>
 <tr>
 <td>[internal]</td>
 <td><code class="docutils literal notranslate">v6.0.0 -> v7.0.5</code></td>
 </table>
 </div>
 </li>
            <li> <span class="li-head">protocol</span> - Protocol name. <span class="li-normal">type: str</span> <span class="li-required">required: true</span>
 <a id='label150' href="javascript:ContentClick('label151', 'label150');" onmouseover="ContentPreview('label151');" onmouseout="ContentUnpreview('label151');" title="click to collapse or expand..."> more... </a>
 <div id="label151" style="display:none">
 <table border="1">
 <tr>
 <td></td>
 <td colspan="2">Supported Version Ranges</td>
 </tr>
 <tr>
 <td>protocol</td>
 <td><code class="docutils literal notranslate">v6.0.0 -> v7.0.5 </code></td>
 <td><code class="docutils literal notranslate">v7.2.0 -> v7.2.0 </code></td>
 </tr>
 </table>
 </div>
 </li>
            <li> <span class="li-head">routemap</span> - Route map name. Source router.route-map.name. <span class="li-normal">type: str</span>
 <a id='label152' href="javascript:ContentClick('label153', 'label152');" onmouseover="ContentPreview('label153');" onmouseout="ContentUnpreview('label153');" title="click to collapse or expand..."> more... </a>
 <div id="label153" style="display:none">
 <table border="1">
 <tr>
 <td></td>
 <td colspan="2">Supported Version Ranges</td>
 </tr>
 <tr>
 <td>routemap</td>
 <td><code class="docutils literal notranslate">v6.0.0 -> v7.0.5 </code></td>
 <td><code class="docutils literal notranslate">v7.2.0 -> v7.2.0 </code></td>
 </tr>
 </table>
 </div>
 </li>
            <li> <span class="li-head">status</span> - Enable/disable redistribution. <span class="li-normal">type: str</span> <span class="li-normal">choices: enable, disable</span>
 <a id='label154' href="javascript:ContentClick('label155', 'label154');" onmouseover="ContentPreview('label155');" onmouseout="ContentUnpreview('label155');" title="click to collapse or expand..."> more... </a>
 <div id="label155" style="display:none">
 <table border="1">
 <tr>
 <td></td>
 <td colspan="2">Supported Version Ranges</td>
 </tr>
 <tr>
 <td>status</td>
 <td><code class="docutils literal notranslate">v6.0.0 -> v7.0.5 </code></td>
 <td><code class="docutils literal notranslate">v7.2.0 -> v7.2.0 </code></td>
 </tr>
 <tr>
 <td>[enable]</td>
 <td><code class="docutils literal notranslate">v6.0.0 -> v7.0.5</code></td>
 <tr>
 <td>[disable]</td>
 <td><code class="docutils literal notranslate">v6.0.0 -> v7.0.5</code></td>
 </table>
 </div>
 </li>
            </ul>
        <li> <span class="li-head">redistribute6_l1</span> - Enable/disable redistribution of level 1 IPv6 routes into level 2. <span class="li-normal">type: str</span> <span class="li-normal">choices: enable, disable</span>
 <a id='label156' href="javascript:ContentClick('label157', 'label156');" onmouseover="ContentPreview('label157');" onmouseout="ContentUnpreview('label157');" title="click to collapse or expand..."> more... </a>
 <div id="label157" style="display:none">
 <table border="1">
 <tr>
 <td></td>
 <td colspan="1">Supported Version Ranges</td>
 </tr>
 <tr>
 <td>redistribute6_l1</td>
 <td><code class="docutils literal notranslate">v6.0.0 -> 7.6.0 </code></td>
 </tr>
 <tr>
 <td>[enable]</td>
 <td><code class="docutils literal notranslate">v6.0.0 -> 7.6.0</code></td>
 <tr>
 <td>[disable]</td>
 <td><code class="docutils literal notranslate">v6.0.0 -> 7.6.0</code></td>
 </table>
 </div>
 </li>
        <li> <span class="li-head">redistribute6_l1_list</span> - Access-list for IPv6 route redistribution from l1 to l2. Source router.access-list6.name. <span class="li-normal">type: str</span>
 <a id='label158' href="javascript:ContentClick('label159', 'label158');" onmouseover="ContentPreview('label159');" onmouseout="ContentUnpreview('label159');" title="click to collapse or expand..."> more... </a>
 <div id="label159" style="display:none">
 <table border="1">
 <tr>
 <td></td>
 <td colspan="1">Supported Version Ranges</td>
 </tr>
 <tr>
 <td>redistribute6_l1_list</td>
 <td><code class="docutils literal notranslate">v6.0.0 -> 7.6.0 </code></td>
 </tr>
 </table>
 </div>
 </li>
        <li> <span class="li-head">redistribute6_l2</span> - Enable/disable redistribution of level 2 IPv6 routes into level 1. <span class="li-normal">type: str</span> <span class="li-normal">choices: enable, disable</span>
 <a id='label160' href="javascript:ContentClick('label161', 'label160');" onmouseover="ContentPreview('label161');" onmouseout="ContentUnpreview('label161');" title="click to collapse or expand..."> more... </a>
 <div id="label161" style="display:none">
 <table border="1">
 <tr>
 <td></td>
 <td colspan="1">Supported Version Ranges</td>
 </tr>
 <tr>
 <td>redistribute6_l2</td>
 <td><code class="docutils literal notranslate">v6.0.0 -> 7.6.0 </code></td>
 </tr>
 <tr>
 <td>[enable]</td>
 <td><code class="docutils literal notranslate">v6.0.0 -> 7.6.0</code></td>
 <tr>
 <td>[disable]</td>
 <td><code class="docutils literal notranslate">v6.0.0 -> 7.6.0</code></td>
 </table>
 </div>
 </li>
        <li> <span class="li-head">redistribute6_l2_list</span> - Access-list for IPv6 route redistribution from l2 to l1. Source router.access-list6.name. <span class="li-normal">type: str</span>
 <a id='label162' href="javascript:ContentClick('label163', 'label162');" onmouseover="ContentPreview('label163');" onmouseout="ContentUnpreview('label163');" title="click to collapse or expand..."> more... </a>
 <div id="label163" style="display:none">
 <table border="1">
 <tr>
 <td></td>
 <td colspan="1">Supported Version Ranges</td>
 </tr>
 <tr>
 <td>redistribute6_l2_list</td>
 <td><code class="docutils literal notranslate">v6.0.0 -> 7.6.0 </code></td>
 </tr>
 </table>
 </div>
 </li>
        <li> <span class="li-head">spf_interval_exp_l1</span> - Level 1 SPF calculation delay. <span class="li-normal">type: str</span>
 <a id='label164' href="javascript:ContentClick('label165', 'label164');" onmouseover="ContentPreview('label165');" onmouseout="ContentUnpreview('label165');" title="click to collapse or expand..."> more... </a>
 <div id="label165" style="display:none">
 <table border="1">
 <tr>
 <td></td>
 <td colspan="1">Supported Version Ranges</td>
 </tr>
 <tr>
 <td>spf_interval_exp_l1</td>
 <td><code class="docutils literal notranslate">v6.0.0 -> 7.6.0 </code></td>
 </tr>
 </table>
 </div>
 </li>
        <li> <span class="li-head">spf_interval_exp_l2</span> - Level 2 SPF calculation delay. <span class="li-normal">type: str</span>
 <a id='label166' href="javascript:ContentClick('label167', 'label166');" onmouseover="ContentPreview('label167');" onmouseout="ContentUnpreview('label167');" title="click to collapse or expand..."> more... </a>
 <div id="label167" style="display:none">
 <table border="1">
 <tr>
 <td></td>
 <td colspan="1">Supported Version Ranges</td>
 </tr>
 <tr>
 <td>spf_interval_exp_l2</td>
 <td><code class="docutils literal notranslate">v6.0.0 -> 7.6.0 </code></td>
 </tr>
 </table>
 </div>
 </li>
        <li> <span class="li-head">summary_address</span> - IS-IS summary addresses. <span class="li-normal">type: list</span> <span style="font-family:'Courier New'" class="li-required">member_path: summary_address:id</span>
 <a id='label168' href="javascript:ContentClick('label169', 'label168');" onmouseover="ContentPreview('label169');" onmouseout="ContentUnpreview('label169');" title="click to collapse or expand..."> more... </a>
 <div id="label169" style="display:none">
 <table border="1">
 <tr>
 <td></td><td colspan="1">Supported Version Ranges</td>
 </tr>
 <tr>
 <td>summary_address</td>
 <td><code class="docutils literal notranslate">v6.0.0 -> 7.6.0 </code></td>
 </tr>
 </table>
 </div>
 </li>
            <ul class="ul-self">
            <li> <span class="li-head">id</span> - Summary address entry ID. see <a href='#notes'>Notes</a>. <span class="li-normal">type: int</span> <span class="li-required">required: true</span>
 <a id='label170' href="javascript:ContentClick('label171', 'label170');" onmouseover="ContentPreview('label171');" onmouseout="ContentUnpreview('label171');" title="click to collapse or expand..."> more... </a>
 <div id="label171" style="display:none">
 <table border="1">
 <tr>
 <td></td>
 <td colspan="1">Supported Version Ranges</td>
 </tr>
 <tr>
 <td>id</td>
 <td><code class="docutils literal notranslate">v6.0.0 -> 7.6.0 </code></td>
 </tr>
 </table>
 </div>
 </li>
            <li> <span class="li-head">level</span> - Level. <span class="li-normal">type: str</span> <span class="li-normal">choices: level-1-2, level-1, level-2</span>
 <a id='label172' href="javascript:ContentClick('label173', 'label172');" onmouseover="ContentPreview('label173');" onmouseout="ContentUnpreview('label173');" title="click to collapse or expand..."> more... </a>
 <div id="label173" style="display:none">
 <table border="1">
 <tr>
 <td></td>
 <td colspan="1">Supported Version Ranges</td>
 </tr>
 <tr>
 <td>level</td>
 <td><code class="docutils literal notranslate">v6.0.0 -> 7.6.0 </code></td>
 </tr>
 <tr>
 <td>[level-1-2]</td>
 <td><code class="docutils literal notranslate">v6.0.0 -> 7.6.0</code></td>
 <tr>
 <td>[level-1]</td>
 <td><code class="docutils literal notranslate">v6.0.0 -> 7.6.0</code></td>
 <tr>
 <td>[level-2]</td>
 <td><code class="docutils literal notranslate">v6.0.0 -> 7.6.0</code></td>
 </table>
 </div>
 </li>
            <li> <span class="li-head">prefix</span> - Prefix. <span class="li-normal">type: str</span>
 <a id='label174' href="javascript:ContentClick('label175', 'label174');" onmouseover="ContentPreview('label175');" onmouseout="ContentUnpreview('label175');" title="click to collapse or expand..."> more... </a>
 <div id="label175" style="display:none">
 <table border="1">
 <tr>
 <td></td>
 <td colspan="1">Supported Version Ranges</td>
 </tr>
 <tr>
 <td>prefix</td>
 <td><code class="docutils literal notranslate">v6.0.0 -> 7.6.0 </code></td>
 </tr>
 </table>
 </div>
 </li>
            </ul>
        <li> <span class="li-head">summary_address6</span> - IS-IS IPv6 summary address. <span class="li-normal">type: list</span> <span style="font-family:'Courier New'" class="li-required">member_path: summary_address6:id</span>
 <a id='label176' href="javascript:ContentClick('label177', 'label176');" onmouseover="ContentPreview('label177');" onmouseout="ContentUnpreview('label177');" title="click to collapse or expand..."> more... </a>
 <div id="label177" style="display:none">
 <table border="1">
 <tr>
 <td></td><td colspan="1">Supported Version Ranges</td>
 </tr>
 <tr>
 <td>summary_address6</td>
 <td><code class="docutils literal notranslate">v6.0.0 -> 7.6.0 </code></td>
 </tr>
 </table>
 </div>
 </li>
            <ul class="ul-self">
            <li> <span class="li-head">id</span> - Prefix entry ID. see <a href='#notes'>Notes</a>. <span class="li-normal">type: int</span> <span class="li-required">required: true</span>
 <a id='label178' href="javascript:ContentClick('label179', 'label178');" onmouseover="ContentPreview('label179');" onmouseout="ContentUnpreview('label179');" title="click to collapse or expand..."> more... </a>
 <div id="label179" style="display:none">
 <table border="1">
 <tr>
 <td></td>
 <td colspan="1">Supported Version Ranges</td>
 </tr>
 <tr>
 <td>id</td>
 <td><code class="docutils literal notranslate">v6.0.0 -> 7.6.0 </code></td>
 </tr>
 </table>
 </div>
 </li>
            <li> <span class="li-head">level</span> - Level. <span class="li-normal">type: str</span> <span class="li-normal">choices: level-1-2, level-1, level-2</span>
 <a id='label180' href="javascript:ContentClick('label181', 'label180');" onmouseover="ContentPreview('label181');" onmouseout="ContentUnpreview('label181');" title="click to collapse or expand..."> more... </a>
 <div id="label181" style="display:none">
 <table border="1">
 <tr>
 <td></td>
 <td colspan="1">Supported Version Ranges</td>
 </tr>
 <tr>
 <td>level</td>
 <td><code class="docutils literal notranslate">v6.0.0 -> 7.6.0 </code></td>
 </tr>
 <tr>
 <td>[level-1-2]</td>
 <td><code class="docutils literal notranslate">v6.0.0 -> 7.6.0</code></td>
 <tr>
 <td>[level-1]</td>
 <td><code class="docutils literal notranslate">v6.0.0 -> 7.6.0</code></td>
 <tr>
 <td>[level-2]</td>
 <td><code class="docutils literal notranslate">v6.0.0 -> 7.6.0</code></td>
 </table>
 </div>
 </li>
            <li> <span class="li-head">prefix6</span> - IPv6 prefix. <span class="li-normal">type: str</span>
 <a id='label182' href="javascript:ContentClick('label183', 'label182');" onmouseover="ContentPreview('label183');" onmouseout="ContentUnpreview('label183');" title="click to collapse or expand..."> more... </a>
 <div id="label183" style="display:none">
 <table border="1">
 <tr>
 <td></td>
 <td colspan="1">Supported Version Ranges</td>
 </tr>
 <tr>
 <td>prefix6</td>
 <td><code class="docutils literal notranslate">v6.0.0 -> 7.6.0 </code></td>
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
    
    - name: Configure IS-IS.
      fortinet.fortios.fortios_router_isis:
          vdom: "{{ vdom }}"
          router_isis:
              adjacency_check: "enable"
              adjacency_check6: "enable"
              adv_passive_only: "enable"
              adv_passive_only6: "enable"
              auth_keychain_l1: "<your_own_value> (source router.key-chain.name)"
              auth_keychain_l2: "<your_own_value> (source router.key-chain.name)"
              auth_mode_l1: "password"
              auth_mode_l2: "password"
              auth_password_l1: "<your_own_value>"
              auth_password_l2: "<your_own_value>"
              auth_sendonly_l1: "enable"
              auth_sendonly_l2: "enable"
              default_originate: "enable"
              default_originate6: "enable"
              dynamic_hostname: "enable"
              ignore_lsp_errors: "enable"
              is_type: "level-1-2"
              isis_interface:
                  -
                      auth_keychain_l1: "<your_own_value> (source router.key-chain.name)"
                      auth_keychain_l2: "<your_own_value> (source router.key-chain.name)"
                      auth_mode_l1: "md5"
                      auth_mode_l2: "md5"
                      auth_password_l1: "<your_own_value>"
                      auth_password_l2: "<your_own_value>"
                      auth_send_only_l1: "enable"
                      auth_send_only_l2: "enable"
                      circuit_type: "level-1-2"
                      csnp_interval_l1: "10"
                      csnp_interval_l2: "10"
                      hello_interval_l1: "10"
                      hello_interval_l2: "10"
                      hello_multiplier_l1: "3"
                      hello_multiplier_l2: "3"
                      hello_padding: "enable"
                      lsp_interval: "33"
                      lsp_retransmit_interval: "5"
                      mesh_group: "enable"
                      mesh_group_id: "0"
                      metric_l1: "10"
                      metric_l2: "10"
                      name: "default_name_43 (source system.interface.name)"
                      network_type: "broadcast"
                      priority_l1: "64"
                      priority_l2: "64"
                      status: "enable"
                      status6: "enable"
                      wide_metric_l1: "10"
                      wide_metric_l2: "10"
              isis_net:
                  -
                      id: "52"
                      net: "<your_own_value>"
              lsp_gen_interval_l1: "30"
              lsp_gen_interval_l2: "30"
              lsp_refresh_interval: "900"
              max_lsp_lifetime: "1200"
              metric_style: "narrow"
              overload_bit: "enable"
              overload_bit_on_startup: "0"
              overload_bit_suppress: "external"
              redistribute:
                  -
                      level: "level-1-2"
                      metric: "0"
                      metric_type: "external"
                      protocol: "<your_own_value>"
                      routemap: "<your_own_value> (source router.route-map.name)"
                      status: "enable"
              redistribute_l1: "enable"
              redistribute_l1_list: "<your_own_value> (source router.access-list.name)"
              redistribute_l2: "enable"
              redistribute_l2_list: "<your_own_value> (source router.access-list.name)"
              redistribute6:
                  -
                      level: "level-1-2"
                      metric: "0"
                      metric_type: "external"
                      protocol: "<your_own_value>"
                      routemap: "<your_own_value> (source router.route-map.name)"
                      status: "enable"
              redistribute6_l1: "enable"
              redistribute6_l1_list: "<your_own_value> (source router.access-list6.name)"
              redistribute6_l2: "enable"
              redistribute6_l2_list: "<your_own_value> (source router.access-list6.name)"
              spf_interval_exp_l1: "<your_own_value>"
              spf_interval_exp_l2: "<your_own_value>"
              summary_address:
                  -
                      id: "87"
                      level: "level-1-2"
                      prefix: "<your_own_value>"
              summary_address6:
                  -
                      id: "91"
                      level: "level-1-2"
                      prefix6: "<your_own_value>"


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
