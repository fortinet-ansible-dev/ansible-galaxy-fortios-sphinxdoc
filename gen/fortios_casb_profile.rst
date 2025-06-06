:source: fortios_casb_profile.py

:orphan:

.. fortios_casb_profile:

fortios_casb_profile -- Configure CASB profile in Fortinet's FortiOS and FortiGate.
+++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++

.. versionadded:: 2.0.0

.. contents::
   :local:
   :depth: 1


Synopsis
--------
- This module is able to configure a FortiGate or FortiOS (FOS) device by allowing the user to set and modify casb feature and profile category. Examples include all parameters and values need to be adjusted to datasources before usage. Tested with FOS v6.0.0



Requirements
------------
The below requirements are needed on the host that executes this module.

- ansible>=2.15


Tips
----
Using member operation to add an element to an existing object.

FortiOS Version Compatibility
-----------------------------
Supported Version Ranges: v7.4.1 -> v7.6.2


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
    <li> <span class="li-head">casb_profile</span> - Configure CASB profile. <span class="li-normal">type: dict</span>
 <a id='label0' href="javascript:ContentClick('label1', 'label0');" onmouseover="ContentPreview('label1');" onmouseout="ContentUnpreview('label1');" title="click to collapse or expand..."> more... </a>
 <div id="label1" style="display:none">
 <table border="1">
 <tr>
 <td></td><td colspan="1">Supported Version Ranges</td>
 </tr>
 <tr>
 <td>casb_profile</td>
 <td><code class="docutils literal notranslate">v7.4.1 -> 7.6.2 </code></td>
 </tr>
 </table>
 </div>
 </li>
        <ul class="ul-self">
        <li> <span class="li-head">comment</span> - Comment. <span class="li-normal">type: str</span>
 <a id='label2' href="javascript:ContentClick('label3', 'label2');" onmouseover="ContentPreview('label3');" onmouseout="ContentUnpreview('label3');" title="click to collapse or expand..."> more... </a>
 <div id="label3" style="display:none">
 <table border="1">
 <tr>
 <td></td>
 <td colspan="1">Supported Version Ranges</td>
 </tr>
 <tr>
 <td>comment</td>
 <td><code class="docutils literal notranslate">v7.4.4 -> 7.6.2 </code></td>
 </tr>
 </table>
 </div>
 </li>
        <li> <span class="li-head">name</span> - CASB profile name. <span class="li-normal">type: str</span> <span class="li-required">required: true</span>
 <a id='label4' href="javascript:ContentClick('label5', 'label4');" onmouseover="ContentPreview('label5');" onmouseout="ContentUnpreview('label5');" title="click to collapse or expand..."> more... </a>
 <div id="label5" style="display:none">
 <table border="1">
 <tr>
 <td></td>
 <td colspan="1">Supported Version Ranges</td>
 </tr>
 <tr>
 <td>name</td>
 <td><code class="docutils literal notranslate">v7.4.1 -> 7.6.2 </code></td>
 </tr>
 </table>
 </div>
 </li>
        <li> <span class="li-head">saas_application</span> - CASB profile SaaS application. <span class="li-normal">type: list</span> <span style="font-family:'Courier New'" class="li-required">member_path: saas_application:name</span>
 <a id='label6' href="javascript:ContentClick('label7', 'label6');" onmouseover="ContentPreview('label7');" onmouseout="ContentUnpreview('label7');" title="click to collapse or expand..."> more... </a>
 <div id="label7" style="display:none">
 <table border="1">
 <tr>
 <td></td><td colspan="1">Supported Version Ranges</td>
 </tr>
 <tr>
 <td>saas_application</td>
 <td><code class="docutils literal notranslate">v7.4.1 -> 7.6.2 </code></td>
 </tr>
 </table>
 </div>
 </li>
            <ul class="ul-self">
            <li> <span class="li-head">access_rule</span> - CASB profile access rule. <span class="li-normal">type: list</span> <span style="font-family:'Courier New'" class="li-required">member_path: saas_application:name/access_rule:name</span>
 <a id='label8' href="javascript:ContentClick('label9', 'label8');" onmouseover="ContentPreview('label9');" onmouseout="ContentUnpreview('label9');" title="click to collapse or expand..."> more... </a>
 <div id="label9" style="display:none">
 <table border="1">
 <tr>
 <td></td><td colspan="1">Supported Version Ranges</td>
 </tr>
 <tr>
 <td>access_rule</td>
 <td><code class="docutils literal notranslate">v7.4.1 -> 7.6.2 </code></td>
 </tr>
 </table>
 </div>
 </li>
                <ul class="ul-self">
                <li> <span class="li-head">action</span> - CASB access rule action. <span class="li-normal">type: str</span> <span class="li-normal">choices: monitor, bypass, block</span>
 <a id='label10' href="javascript:ContentClick('label11', 'label10');" onmouseover="ContentPreview('label11');" onmouseout="ContentUnpreview('label11');" title="click to collapse or expand..."> more... </a>
 <div id="label11" style="display:none">
 <table border="1">
 <tr>
 <td></td>
 <td colspan="1">Supported Version Ranges</td>
 </tr>
 <tr>
 <td>action</td>
 <td><code class="docutils literal notranslate">v7.4.1 -> 7.6.2 </code></td>
 </tr>
 <tr>
 <td>[monitor]</td>
 <td><code class="docutils literal notranslate">v7.4.1 -> 7.6.2</code></td>
 <tr>
 <td>[bypass]</td>
 <td><code class="docutils literal notranslate">v7.4.1 -> 7.6.2</code></td>
 <tr>
 <td>[block]</td>
 <td><code class="docutils literal notranslate">v7.4.1 -> 7.6.2</code></td>
 </table>
 </div>
 </li>
                <li> <span class="li-head">attribute_filter</span> - CASB profile attribute filter. <span class="li-normal">type: list</span> <span style="font-family:'Courier New'" class="li-required">member_path: saas_application:name/access_rule:name/attribute_filter:id</span>
 <a id='label12' href="javascript:ContentClick('label13', 'label12');" onmouseover="ContentPreview('label13');" onmouseout="ContentUnpreview('label13');" title="click to collapse or expand..."> more... </a>
 <div id="label13" style="display:none">
 <table border="1">
 <tr>
 <td></td><td colspan="1">Supported Version Ranges</td>
 </tr>
 <tr>
 <td>attribute_filter</td>
 <td><code class="docutils literal notranslate">v7.6.1 -> 7.6.2 </code></td>
 </tr>
 </table>
 </div>
 </li>
                    <ul class="ul-self">
                    <li> <span class="li-head">action</span> - CASB access rule tenant control action. <span class="li-normal">type: str</span> <span class="li-normal">choices: monitor, bypass, block</span>
 <a id='label14' href="javascript:ContentClick('label15', 'label14');" onmouseover="ContentPreview('label15');" onmouseout="ContentUnpreview('label15');" title="click to collapse or expand..."> more... </a>
 <div id="label15" style="display:none">
 <table border="1">
 <tr>
 <td></td>
 <td colspan="1">Supported Version Ranges</td>
 </tr>
 <tr>
 <td>action</td>
 <td><code class="docutils literal notranslate">v7.6.1 -> 7.6.2 </code></td>
 </tr>
 <tr>
 <td>[monitor]</td>
 <td><code class="docutils literal notranslate">v7.6.1 -> 7.6.2</code></td>
 <tr>
 <td>[bypass]</td>
 <td><code class="docutils literal notranslate">v7.6.1 -> 7.6.2</code></td>
 <tr>
 <td>[block]</td>
 <td><code class="docutils literal notranslate">v7.6.1 -> 7.6.2</code></td>
 </table>
 </div>
 </li>
                    <li> <span class="li-head">attribute_match</span> - CASB access rule tenant match. Source casb.attribute-match.name. <span class="li-normal">type: str</span>
 <a id='label16' href="javascript:ContentClick('label17', 'label16');" onmouseover="ContentPreview('label17');" onmouseout="ContentUnpreview('label17');" title="click to collapse or expand..."> more... </a>
 <div id="label17" style="display:none">
 <table border="1">
 <tr>
 <td></td>
 <td colspan="1">Supported Version Ranges</td>
 </tr>
 <tr>
 <td>attribute_match</td>
 <td><code class="docutils literal notranslate">v7.6.1 -> 7.6.2 </code></td>
 </tr>
 </table>
 </div>
 </li>
                    <li> <span class="li-head">id</span> - CASB tenant control ID. see <a href='#notes'>Notes</a>. <span class="li-normal">type: int</span> <span class="li-required">required: true</span>
 <a id='label18' href="javascript:ContentClick('label19', 'label18');" onmouseover="ContentPreview('label19');" onmouseout="ContentUnpreview('label19');" title="click to collapse or expand..."> more... </a>
 <div id="label19" style="display:none">
 <table border="1">
 <tr>
 <td></td>
 <td colspan="1">Supported Version Ranges</td>
 </tr>
 <tr>
 <td>id</td>
 <td><code class="docutils literal notranslate">v7.6.1 -> 7.6.2 </code></td>
 </tr>
 </table>
 </div>
 </li>
                    </ul>
                <li> <span class="li-head">bypass</span> - CASB bypass options. <span class="li-normal">type: list</span> <span class="li-normal">choices: av, dlp, web-filter, file-filter, video-filter</span>
 <a id='label20' href="javascript:ContentClick('label21', 'label20');" onmouseover="ContentPreview('label21');" onmouseout="ContentUnpreview('label21');" title="click to collapse or expand..."> more... </a>
 <div id="label21" style="display:none">
 <table border="1">
 <tr>
 <td></td>
 <td colspan="1">Supported Version Ranges</td>
 </tr>
 <tr>
 <td>bypass</td>
 <td><code class="docutils literal notranslate">v7.4.1 -> 7.6.2 </code></td>
 </tr>
 <tr>
 <td>[av]</td>
 <td><code class="docutils literal notranslate">v7.4.1 -> 7.6.2</code></td>
 <tr>
 <td>[dlp]</td>
 <td><code class="docutils literal notranslate">v7.4.1 -> 7.6.2</code></td>
 <tr>
 <td>[web-filter]</td>
 <td><code class="docutils literal notranslate">v7.4.1 -> 7.6.2</code></td>
 <tr>
 <td>[file-filter]</td>
 <td><code class="docutils literal notranslate">v7.4.1 -> 7.6.2</code></td>
 <tr>
 <td>[video-filter]</td>
 <td><code class="docutils literal notranslate">v7.4.1 -> 7.6.2</code></td>
 </table>
 </div>
 </li>
                <li> <span class="li-head">name</span> - CASB access rule activity name. Source casb.user-activity.name. <span class="li-normal">type: str</span> <span class="li-required">required: true</span>
 <a id='label22' href="javascript:ContentClick('label23', 'label22');" onmouseover="ContentPreview('label23');" onmouseout="ContentUnpreview('label23');" title="click to collapse or expand..."> more... </a>
 <div id="label23" style="display:none">
 <table border="1">
 <tr>
 <td></td>
 <td colspan="1">Supported Version Ranges</td>
 </tr>
 <tr>
 <td>name</td>
 <td><code class="docutils literal notranslate">v7.4.1 -> 7.6.2 </code></td>
 </tr>
 </table>
 </div>
 </li>
                </ul>
            <li> <span class="li-head">advanced_tenant_control</span> - CASB profile advanced tenant control. <span class="li-normal">type: list</span> <span style="font-family:'Courier New'" class="li-required">member_path: saas_application:name/advanced_tenant_control:name</span>
 <a id='label24' href="javascript:ContentClick('label25', 'label24');" onmouseover="ContentPreview('label25');" onmouseout="ContentUnpreview('label25');" title="click to collapse or expand..."> more... </a>
 <div id="label25" style="display:none">
 <table border="1">
 <tr>
 <td></td><td colspan="1">Supported Version Ranges</td>
 </tr>
 <tr>
 <td>advanced_tenant_control</td>
 <td><code class="docutils literal notranslate">v7.6.1 -> 7.6.2 </code></td>
 </tr>
 </table>
 </div>
 </li>
                <ul class="ul-self">
                <li> <span class="li-head">attribute</span> - CASB advanced tenant control attribute. <span class="li-normal">type: list</span> <span style="font-family:'Courier New'" class="li-required">member_path: saas_application:name/advanced_tenant_control:name/attribute:name</span>
 <a id='label26' href="javascript:ContentClick('label27', 'label26');" onmouseover="ContentPreview('label27');" onmouseout="ContentUnpreview('label27');" title="click to collapse or expand..."> more... </a>
 <div id="label27" style="display:none">
 <table border="1">
 <tr>
 <td></td><td colspan="1">Supported Version Ranges</td>
 </tr>
 <tr>
 <td>attribute</td>
 <td><code class="docutils literal notranslate">v7.6.1 -> 7.6.2 </code></td>
 </tr>
 </table>
 </div>
 </li>
                    <ul class="ul-self">
                    <li> <span class="li-head">input</span> - CASB extend user input value. <span class="li-normal">type: list</span> <span style="font-family:'Courier New'" class="li-required">member_path: saas_application:name/advanced_tenant_control:name/attribute:name/input:value</span>
 <a id='label28' href="javascript:ContentClick('label29', 'label28');" onmouseover="ContentPreview('label29');" onmouseout="ContentUnpreview('label29');" title="click to collapse or expand..."> more... </a>
 <div id="label29" style="display:none">
 <table border="1">
 <tr>
 <td></td><td colspan="1">Supported Version Ranges</td>
 </tr>
 <tr>
 <td>input</td>
 <td><code class="docutils literal notranslate">v7.6.1 -> 7.6.2 </code></td>
 </tr>
 </table>
 </div>
 </li>
                        <ul class="ul-self">
                        <li> <span class="li-head">value</span> - User input value. <span class="li-normal">type: str</span> <span class="li-required">required: true</span>
 <a id='label30' href="javascript:ContentClick('label31', 'label30');" onmouseover="ContentPreview('label31');" onmouseout="ContentUnpreview('label31');" title="click to collapse or expand..."> more... </a>
 <div id="label31" style="display:none">
 <table border="1">
 <tr>
 <td></td>
 <td colspan="1">Supported Version Ranges</td>
 </tr>
 <tr>
 <td>value</td>
 <td><code class="docutils literal notranslate">v7.6.1 -> 7.6.2 </code></td>
 </tr>
 </table>
 </div>
 </li>
                        </ul>
                    <li> <span class="li-head">name</span> - CASB extend user input name. <span class="li-normal">type: str</span> <span class="li-required">required: true</span>
 <a id='label32' href="javascript:ContentClick('label33', 'label32');" onmouseover="ContentPreview('label33');" onmouseout="ContentUnpreview('label33');" title="click to collapse or expand..."> more... </a>
 <div id="label33" style="display:none">
 <table border="1">
 <tr>
 <td></td>
 <td colspan="1">Supported Version Ranges</td>
 </tr>
 <tr>
 <td>name</td>
 <td><code class="docutils literal notranslate">v7.6.1 -> 7.6.2 </code></td>
 </tr>
 </table>
 </div>
 </li>
                    </ul>
                <li> <span class="li-head">name</span> - CASB advanced tenant control name. Source casb.user-activity.name. <span class="li-normal">type: str</span> <span class="li-required">required: true</span>
 <a id='label34' href="javascript:ContentClick('label35', 'label34');" onmouseover="ContentPreview('label35');" onmouseout="ContentUnpreview('label35');" title="click to collapse or expand..."> more... </a>
 <div id="label35" style="display:none">
 <table border="1">
 <tr>
 <td></td>
 <td colspan="1">Supported Version Ranges</td>
 </tr>
 <tr>
 <td>name</td>
 <td><code class="docutils literal notranslate">v7.6.1 -> 7.6.2 </code></td>
 </tr>
 </table>
 </div>
 </li>
                </ul>
            <li> <span class="li-head">custom_control</span> - CASB profile custom control. <span class="li-normal">type: list</span> <span style="font-family:'Courier New'" class="li-required">member_path: saas_application:name/custom_control:name</span>
 <a id='label36' href="javascript:ContentClick('label37', 'label36');" onmouseover="ContentPreview('label37');" onmouseout="ContentUnpreview('label37');" title="click to collapse or expand..."> more... </a>
 <div id="label37" style="display:none">
 <table border="1">
 <tr>
 <td></td><td colspan="1">Supported Version Ranges</td>
 </tr>
 <tr>
 <td>custom_control</td>
 <td><code class="docutils literal notranslate">v7.4.1 -> 7.6.2 </code></td>
 </tr>
 </table>
 </div>
 </li>
                <ul class="ul-self">
                <li> <span class="li-head">attribute_filter</span> - CASB attribute filter. <span class="li-normal">type: list</span> <span style="font-family:'Courier New'" class="li-required">member_path: saas_application:name/custom_control:name/attribute_filter:id</span>
 <a id='label38' href="javascript:ContentClick('label39', 'label38');" onmouseover="ContentPreview('label39');" onmouseout="ContentUnpreview('label39');" title="click to collapse or expand..."> more... </a>
 <div id="label39" style="display:none">
 <table border="1">
 <tr>
 <td></td><td colspan="1">Supported Version Ranges</td>
 </tr>
 <tr>
 <td>attribute_filter</td>
 <td><code class="docutils literal notranslate">v7.6.1 -> 7.6.2 </code></td>
 </tr>
 </table>
 </div>
 </li>
                    <ul class="ul-self">
                    <li> <span class="li-head">action</span> - CASB access rule tenant control action. <span class="li-normal">type: str</span> <span class="li-normal">choices: monitor, bypass, block</span>
 <a id='label40' href="javascript:ContentClick('label41', 'label40');" onmouseover="ContentPreview('label41');" onmouseout="ContentUnpreview('label41');" title="click to collapse or expand..."> more... </a>
 <div id="label41" style="display:none">
 <table border="1">
 <tr>
 <td></td>
 <td colspan="1">Supported Version Ranges</td>
 </tr>
 <tr>
 <td>action</td>
 <td><code class="docutils literal notranslate">v7.6.1 -> 7.6.2 </code></td>
 </tr>
 <tr>
 <td>[monitor]</td>
 <td><code class="docutils literal notranslate">v7.6.1 -> 7.6.2</code></td>
 <tr>
 <td>[bypass]</td>
 <td><code class="docutils literal notranslate">v7.6.1 -> 7.6.2</code></td>
 <tr>
 <td>[block]</td>
 <td><code class="docutils literal notranslate">v7.6.1 -> 7.6.2</code></td>
 </table>
 </div>
 </li>
                    <li> <span class="li-head">attribute_match</span> - CASB access rule tenant match. Source casb.attribute-match.name. <span class="li-normal">type: str</span>
 <a id='label42' href="javascript:ContentClick('label43', 'label42');" onmouseover="ContentPreview('label43');" onmouseout="ContentUnpreview('label43');" title="click to collapse or expand..."> more... </a>
 <div id="label43" style="display:none">
 <table border="1">
 <tr>
 <td></td>
 <td colspan="1">Supported Version Ranges</td>
 </tr>
 <tr>
 <td>attribute_match</td>
 <td><code class="docutils literal notranslate">v7.6.1 -> 7.6.2 </code></td>
 </tr>
 </table>
 </div>
 </li>
                    <li> <span class="li-head">id</span> - CASB tenant control ID. see <a href='#notes'>Notes</a>. <span class="li-normal">type: int</span> <span class="li-required">required: true</span>
 <a id='label44' href="javascript:ContentClick('label45', 'label44');" onmouseover="ContentPreview('label45');" onmouseout="ContentUnpreview('label45');" title="click to collapse or expand..."> more... </a>
 <div id="label45" style="display:none">
 <table border="1">
 <tr>
 <td></td>
 <td colspan="1">Supported Version Ranges</td>
 </tr>
 <tr>
 <td>id</td>
 <td><code class="docutils literal notranslate">v7.6.1 -> 7.6.2 </code></td>
 </tr>
 </table>
 </div>
 </li>
                    </ul>
                <li> <span class="li-head">name</span> - CASB custom control user activity name. Source casb.user-activity.name. <span class="li-normal">type: str</span> <span class="li-required">required: true</span>
 <a id='label46' href="javascript:ContentClick('label47', 'label46');" onmouseover="ContentPreview('label47');" onmouseout="ContentUnpreview('label47');" title="click to collapse or expand..."> more... </a>
 <div id="label47" style="display:none">
 <table border="1">
 <tr>
 <td></td>
 <td colspan="1">Supported Version Ranges</td>
 </tr>
 <tr>
 <td>name</td>
 <td><code class="docutils literal notranslate">v7.4.1 -> 7.6.2 </code></td>
 </tr>
 </table>
 </div>
 </li>
                <li> <span class="li-head">option</span> - CASB custom control option. <span class="li-normal">type: list</span> <span style="font-family:'Courier New'" class="li-required">member_path: saas_application:name/custom_control:name/option:name</span>
 <a id='label48' href="javascript:ContentClick('label49', 'label48');" onmouseover="ContentPreview('label49');" onmouseout="ContentUnpreview('label49');" title="click to collapse or expand..."> more... </a>
 <div id="label49" style="display:none">
 <table border="1">
 <tr>
 <td></td><td colspan="1">Supported Version Ranges</td>
 </tr>
 <tr>
 <td>option</td>
 <td><code class="docutils literal notranslate">v7.4.1 -> 7.6.2 </code></td>
 </tr>
 </table>
 </div>
 </li>
                    <ul class="ul-self">
                    <li> <span class="li-head">name</span> - CASB custom control option name. <span class="li-normal">type: str</span> <span class="li-required">required: true</span>
 <a id='label50' href="javascript:ContentClick('label51', 'label50');" onmouseover="ContentPreview('label51');" onmouseout="ContentUnpreview('label51');" title="click to collapse or expand..."> more... </a>
 <div id="label51" style="display:none">
 <table border="1">
 <tr>
 <td></td>
 <td colspan="1">Supported Version Ranges</td>
 </tr>
 <tr>
 <td>name</td>
 <td><code class="docutils literal notranslate">v7.4.1 -> 7.6.2 </code></td>
 </tr>
 </table>
 </div>
 </li>
                    <li> <span class="li-head">user_input</span> - CASB custom control user input. <span class="li-normal">type: list</span> <span style="font-family:'Courier New'" class="li-required">member_path: saas_application:name/custom_control:name/option:name/user_input:value</span>
 <a id='label52' href="javascript:ContentClick('label53', 'label52');" onmouseover="ContentPreview('label53');" onmouseout="ContentUnpreview('label53');" title="click to collapse or expand..."> more... </a>
 <div id="label53" style="display:none">
 <table border="1">
 <tr>
 <td></td><td colspan="1">Supported Version Ranges</td>
 </tr>
 <tr>
 <td>user_input</td>
 <td><code class="docutils literal notranslate">v7.4.1 -> 7.6.2 </code></td>
 </tr>
 </table>
 </div>
 </li>
                        <ul class="ul-self">
                        <li> <span class="li-head">value</span> - user input value. <span class="li-normal">type: str</span> <span class="li-required">required: true</span>
 <a id='label54' href="javascript:ContentClick('label55', 'label54');" onmouseover="ContentPreview('label55');" onmouseout="ContentUnpreview('label55');" title="click to collapse or expand..."> more... </a>
 <div id="label55" style="display:none">
 <table border="1">
 <tr>
 <td></td>
 <td colspan="1">Supported Version Ranges</td>
 </tr>
 <tr>
 <td>value</td>
 <td><code class="docutils literal notranslate">v7.4.1 -> 7.6.2 </code></td>
 </tr>
 </table>
 </div>
 </li>
                        </ul>
                    </ul>
                </ul>
            <li> <span class="li-head">domain_control</span> - Enable/disable domain control. <span class="li-normal">type: str</span> <span class="li-normal">choices: enable, disable</span>
 <a id='label56' href="javascript:ContentClick('label57', 'label56');" onmouseover="ContentPreview('label57');" onmouseout="ContentUnpreview('label57');" title="click to collapse or expand..."> more... </a>
 <div id="label57" style="display:none">
 <table border="1">
 <tr>
 <td></td>
 <td colspan="1">Supported Version Ranges</td>
 </tr>
 <tr>
 <td>domain_control</td>
 <td><code class="docutils literal notranslate">v7.4.1 -> 7.6.2 </code></td>
 </tr>
 <tr>
 <td>[enable]</td>
 <td><code class="docutils literal notranslate">v7.4.1 -> 7.6.2</code></td>
 <tr>
 <td>[disable]</td>
 <td><code class="docutils literal notranslate">v7.4.1 -> 7.6.2</code></td>
 </table>
 </div>
 </li>
            <li> <span class="li-head">domain_control_domains</span> - CASB profile domain control domains. <span class="li-normal">type: list</span> <span style="font-family:'Courier New'" class="li-required">member_path: saas_application:name/domain_control_domains:name</span>
 <a id='label58' href="javascript:ContentClick('label59', 'label58');" onmouseover="ContentPreview('label59');" onmouseout="ContentUnpreview('label59');" title="click to collapse or expand..."> more... </a>
 <div id="label59" style="display:none">
 <table border="1">
 <tr>
 <td></td><td colspan="1">Supported Version Ranges</td>
 </tr>
 <tr>
 <td>domain_control_domains</td>
 <td><code class="docutils literal notranslate">v7.4.1 -> 7.6.2 </code></td>
 </tr>
 </table>
 </div>
 </li>
                <ul class="ul-self">
                <li> <span class="li-head">name</span> - Domain control domain name. <span class="li-normal">type: str</span> <span class="li-required">required: true</span>
 <a id='label60' href="javascript:ContentClick('label61', 'label60');" onmouseover="ContentPreview('label61');" onmouseout="ContentUnpreview('label61');" title="click to collapse or expand..."> more... </a>
 <div id="label61" style="display:none">
 <table border="1">
 <tr>
 <td></td>
 <td colspan="1">Supported Version Ranges</td>
 </tr>
 <tr>
 <td>name</td>
 <td><code class="docutils literal notranslate">v7.4.1 -> 7.6.2 </code></td>
 </tr>
 </table>
 </div>
 </li>
                </ul>
            <li> <span class="li-head">log</span> - Enable/disable log settings. <span class="li-normal">type: str</span> <span class="li-normal">choices: enable, disable</span>
 <a id='label62' href="javascript:ContentClick('label63', 'label62');" onmouseover="ContentPreview('label63');" onmouseout="ContentUnpreview('label63');" title="click to collapse or expand..."> more... </a>
 <div id="label63" style="display:none">
 <table border="1">
 <tr>
 <td></td>
 <td colspan="1">Supported Version Ranges</td>
 </tr>
 <tr>
 <td>log</td>
 <td><code class="docutils literal notranslate">v7.4.1 -> 7.6.2 </code></td>
 </tr>
 <tr>
 <td>[enable]</td>
 <td><code class="docutils literal notranslate">v7.4.1 -> 7.6.2</code></td>
 <tr>
 <td>[disable]</td>
 <td><code class="docutils literal notranslate">v7.4.1 -> 7.6.2</code></td>
 </table>
 </div>
 </li>
            <li> <span class="li-head">name</span> - CASB profile SaaS application name. Source casb.saas-application.name. <span class="li-normal">type: str</span> <span class="li-required">required: true</span>
 <a id='label64' href="javascript:ContentClick('label65', 'label64');" onmouseover="ContentPreview('label65');" onmouseout="ContentUnpreview('label65');" title="click to collapse or expand..."> more... </a>
 <div id="label65" style="display:none">
 <table border="1">
 <tr>
 <td></td>
 <td colspan="1">Supported Version Ranges</td>
 </tr>
 <tr>
 <td>name</td>
 <td><code class="docutils literal notranslate">v7.4.1 -> 7.6.2 </code></td>
 </tr>
 </table>
 </div>
 </li>
            <li> <span class="li-head">safe_search</span> - Enable/disable safe search. <span class="li-normal">type: str</span> <span class="li-normal">choices: enable, disable</span>
 <a id='label66' href="javascript:ContentClick('label67', 'label66');" onmouseover="ContentPreview('label67');" onmouseout="ContentUnpreview('label67');" title="click to collapse or expand..."> more... </a>
 <div id="label67" style="display:none">
 <table border="1">
 <tr>
 <td></td>
 <td colspan="1">Supported Version Ranges</td>
 </tr>
 <tr>
 <td>safe_search</td>
 <td><code class="docutils literal notranslate">v7.4.1 -> 7.6.2 </code></td>
 </tr>
 <tr>
 <td>[enable]</td>
 <td><code class="docutils literal notranslate">v7.4.1 -> 7.6.2</code></td>
 <tr>
 <td>[disable]</td>
 <td><code class="docutils literal notranslate">v7.4.1 -> 7.6.2</code></td>
 </table>
 </div>
 </li>
            <li> <span class="li-head">safe_search_control</span> - CASB profile safe search control. <span class="li-normal">type: list</span> <span style="font-family:'Courier New'" class="li-required">member_path: saas_application:name/safe_search_control:name</span>
 <a id='label68' href="javascript:ContentClick('label69', 'label68');" onmouseover="ContentPreview('label69');" onmouseout="ContentUnpreview('label69');" title="click to collapse or expand..."> more... </a>
 <div id="label69" style="display:none">
 <table border="1">
 <tr>
 <td></td><td colspan="1">Supported Version Ranges</td>
 </tr>
 <tr>
 <td>safe_search_control</td>
 <td><code class="docutils literal notranslate">v7.4.1 -> 7.6.2 </code></td>
 </tr>
 </table>
 </div>
 </li>
                <ul class="ul-self">
                <li> <span class="li-head">name</span> - Safe search control name. <span class="li-normal">type: str</span> <span class="li-required">required: true</span>
 <a id='label70' href="javascript:ContentClick('label71', 'label70');" onmouseover="ContentPreview('label71');" onmouseout="ContentUnpreview('label71');" title="click to collapse or expand..."> more... </a>
 <div id="label71" style="display:none">
 <table border="1">
 <tr>
 <td></td>
 <td colspan="1">Supported Version Ranges</td>
 </tr>
 <tr>
 <td>name</td>
 <td><code class="docutils literal notranslate">v7.4.1 -> 7.6.2 </code></td>
 </tr>
 </table>
 </div>
 </li>
                </ul>
            <li> <span class="li-head">status</span> - Enable/disable setting. <span class="li-normal">type: str</span> <span class="li-normal">choices: enable, disable</span>
 <a id='label72' href="javascript:ContentClick('label73', 'label72');" onmouseover="ContentPreview('label73');" onmouseout="ContentUnpreview('label73');" title="click to collapse or expand..."> more... </a>
 <div id="label73" style="display:none">
 <table border="1">
 <tr>
 <td></td>
 <td colspan="1">Supported Version Ranges</td>
 </tr>
 <tr>
 <td>status</td>
 <td><code class="docutils literal notranslate">v7.4.2 -> 7.6.2 </code></td>
 </tr>
 <tr>
 <td>[enable]</td>
 <td><code class="docutils literal notranslate">v7.4.2 -> 7.6.2</code></td>
 <tr>
 <td>[disable]</td>
 <td><code class="docutils literal notranslate">v7.4.2 -> 7.6.2</code></td>
 </table>
 </div>
 </li>
            <li> <span class="li-head">tenant_control</span> - Enable/disable tenant control. <span class="li-normal">type: str</span> <span class="li-normal">choices: enable, disable</span>
 <a id='label74' href="javascript:ContentClick('label75', 'label74');" onmouseover="ContentPreview('label75');" onmouseout="ContentUnpreview('label75');" title="click to collapse or expand..."> more... </a>
 <div id="label75" style="display:none">
 <table border="1">
 <tr>
 <td></td>
 <td colspan="1">Supported Version Ranges</td>
 </tr>
 <tr>
 <td>tenant_control</td>
 <td><code class="docutils literal notranslate">v7.4.1 -> 7.6.2 </code></td>
 </tr>
 <tr>
 <td>[enable]</td>
 <td><code class="docutils literal notranslate">v7.4.1 -> 7.6.2</code></td>
 <tr>
 <td>[disable]</td>
 <td><code class="docutils literal notranslate">v7.4.1 -> 7.6.2</code></td>
 </table>
 </div>
 </li>
            <li> <span class="li-head">tenant_control_tenants</span> - CASB profile tenant control tenants. <span class="li-normal">type: list</span> <span style="font-family:'Courier New'" class="li-required">member_path: saas_application:name/tenant_control_tenants:name</span>
 <a id='label76' href="javascript:ContentClick('label77', 'label76');" onmouseover="ContentPreview('label77');" onmouseout="ContentUnpreview('label77');" title="click to collapse or expand..."> more... </a>
 <div id="label77" style="display:none">
 <table border="1">
 <tr>
 <td></td><td colspan="1">Supported Version Ranges</td>
 </tr>
 <tr>
 <td>tenant_control_tenants</td>
 <td><code class="docutils literal notranslate">v7.4.1 -> 7.6.2 </code></td>
 </tr>
 </table>
 </div>
 </li>
                <ul class="ul-self">
                <li> <span class="li-head">name</span> - Tenant control tenants name. <span class="li-normal">type: str</span> <span class="li-required">required: true</span>
 <a id='label78' href="javascript:ContentClick('label79', 'label78');" onmouseover="ContentPreview('label79');" onmouseout="ContentUnpreview('label79');" title="click to collapse or expand..."> more... </a>
 <div id="label79" style="display:none">
 <table border="1">
 <tr>
 <td></td>
 <td colspan="1">Supported Version Ranges</td>
 </tr>
 <tr>
 <td>name</td>
 <td><code class="docutils literal notranslate">v7.4.1 -> 7.6.2 </code></td>
 </tr>
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
    
    - name: Configure CASB profile.
      fortinet.fortios.fortios_casb_profile:
          vdom: "{{ vdom }}"
          state: "present"
          access_token: "<your_own_value>"
          casb_profile:
              comment: "Comment."
              name: "default_name_4"
              saas_application:
                  -
                      access_rule:
                          -
                              action: "monitor"
                              attribute_filter:
                                  -
                                      action: "monitor"
                                      attribute_match: "<your_own_value> (source casb.attribute-match.name)"
                                      id: "11"
                              bypass: "av"
                              name: "default_name_13 (source casb.user-activity.name)"
                      advanced_tenant_control:
                          -
                              attribute:
                                  -
                                      input:
                                          -
                                              value: "<your_own_value>"
                                      name: "default_name_18"
                              name: "default_name_19 (source casb.user-activity.name)"
                      custom_control:
                          -
                              attribute_filter:
                                  -
                                      action: "monitor"
                                      attribute_match: "<your_own_value> (source casb.attribute-match.name)"
                                      id: "24"
                              name: "default_name_25 (source casb.user-activity.name)"
                              option:
                                  -
                                      name: "default_name_27"
                                      user_input:
                                          -
                                              value: "<your_own_value>"
                      domain_control: "enable"
                      domain_control_domains:
                          -
                              name: "default_name_32"
                      log: "enable"
                      name: "default_name_34 (source casb.saas-application.name)"
                      safe_search: "enable"
                      safe_search_control:
                          -
                              name: "default_name_37"
                      status: "enable"
                      tenant_control: "enable"
                      tenant_control_tenants:
                          -
                              name: "default_name_41"


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
