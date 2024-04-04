:source: fortios_system_sdn_connector.py

:orphan:

.. fortios_system_sdn_connector:

fortios_system_sdn_connector -- Configure connection to SDN Connector in Fortinet's FortiOS and FortiGate.
++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++

.. versionadded:: 2.0.0

.. contents::
   :local:
   :depth: 1


Synopsis
--------
- This module is able to configure a FortiGate or FortiOS (FOS) device by allowing the user to set and modify system feature and sdn_connector category. Examples include all parameters and values need to be adjusted to datasources before usage. Tested with FOS v6.0.0



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
    <li> <span class="li-head">state</span> - Indicates whether to create or remove the object. <span class="li-normal">type: str</span> <span class="li-required">required: true</span> <span class="li-normal">choices: present, absent</span> </li>
    <li> <span class="li-head">system_sdn_connector</span> - Configure connection to SDN Connector. <span class="li-normal">type: dict</span>
 <a id='label0' href="javascript:ContentClick('label1', 'label0');" onmouseover="ContentPreview('label1');" onmouseout="ContentUnpreview('label1');" title="click to collapse or expand..."> more... </a>
 <div id="label1" style="display:none">
 <table border="1">
 <tr>
 <td></td><td colspan="1">Supported Version Ranges</td>
 </tr>
 <tr>
 <td>system_sdn_connector</td>
 <td><code class="docutils literal notranslate">v6.0.0 -> 7.4.3 </code></td>
 </tr>
 </table>
 </div>
 </li>
        <ul class="ul-self">
        <li> <span class="li-head">access_key</span> - AWS / ACS access key ID. <span class="li-normal">type: str</span>
 <a id='label2' href="javascript:ContentClick('label3', 'label2');" onmouseover="ContentPreview('label3');" onmouseout="ContentUnpreview('label3');" title="click to collapse or expand..."> more... </a>
 <div id="label3" style="display:none">
 <table border="1">
 <tr>
 <td></td>
 <td colspan="1">Supported Version Ranges</td>
 </tr>
 <tr>
 <td>access_key</td>
 <td><code class="docutils literal notranslate">v6.0.0 -> 7.4.3 </code></td>
 </tr>
 </table>
 </div>
 </li>
        <li> <span class="li-head">alt_resource_ip</span> - Enable/disable AWS alternative resource IP. <span class="li-normal">type: str</span> <span class="li-normal">choices: disable, enable</span>
 <a id='label4' href="javascript:ContentClick('label5', 'label4');" onmouseover="ContentPreview('label5');" onmouseout="ContentUnpreview('label5');" title="click to collapse or expand..."> more... </a>
 <div id="label5" style="display:none">
 <table border="1">
 <tr>
 <td></td>
 <td colspan="1">Supported Version Ranges</td>
 </tr>
 <tr>
 <td>alt_resource_ip</td>
 <td><code class="docutils literal notranslate">v7.2.4 -> 7.4.3 </code></td>
 </tr>
 <tr>
 <td>[disable]</td>
 <td><code class="docutils literal notranslate">v7.2.4 -> 7.4.3</code></td>
 <tr>
 <td>[enable]</td>
 <td><code class="docutils literal notranslate">v7.2.4 -> 7.4.3</code></td>
 </table>
 </div>
 </li>
        <li> <span class="li-head">api_key</span> - IBM cloud API key or service ID API key. <span class="li-normal">type: str</span>
 <a id='label6' href="javascript:ContentClick('label7', 'label6');" onmouseover="ContentPreview('label7');" onmouseout="ContentUnpreview('label7');" title="click to collapse or expand..."> more... </a>
 <div id="label7" style="display:none">
 <table border="1">
 <tr>
 <td></td>
 <td colspan="1">Supported Version Ranges</td>
 </tr>
 <tr>
 <td>api_key</td>
 <td><code class="docutils literal notranslate">v6.4.0 -> 7.4.3 </code></td>
 </tr>
 </table>
 </div>
 </li>
        <li> <span class="li-head">azure_region</span> - Azure server region. <span class="li-normal">type: str</span> <span class="li-normal">choices: global, china, germany, usgov, local</span>
 <a id='label8' href="javascript:ContentClick('label9', 'label8');" onmouseover="ContentPreview('label9');" onmouseout="ContentUnpreview('label9');" title="click to collapse or expand..."> more... </a>
 <div id="label9" style="display:none">
 <table border="1">
 <tr>
 <td></td>
 <td colspan="1">Supported Version Ranges</td>
 </tr>
 <tr>
 <td>azure_region</td>
 <td><code class="docutils literal notranslate">v6.0.0 -> 7.4.3 </code></td>
 </tr>
 <tr>
 <td>[global]</td>
 <td><code class="docutils literal notranslate">v6.0.0 -> 7.4.3</code></td>
 <tr>
 <td>[china]</td>
 <td><code class="docutils literal notranslate">v6.0.0 -> 7.4.3</code></td>
 <tr>
 <td>[germany]</td>
 <td><code class="docutils literal notranslate">v6.0.0 -> 7.4.3</code></td>
 <tr>
 <td>[usgov]</td>
 <td><code class="docutils literal notranslate">v6.0.0 -> 7.4.3</code></td>
 <tr>
 <td>[local]</td>
 <td><code class="docutils literal notranslate">v6.0.0 -> 7.4.3</code></td>
 </table>
 </div>
 </li>
        <li> <span class="li-head">client_id</span> - Azure client ID (application ID). <span class="li-normal">type: str</span>
 <a id='label10' href="javascript:ContentClick('label11', 'label10');" onmouseover="ContentPreview('label11');" onmouseout="ContentUnpreview('label11');" title="click to collapse or expand..."> more... </a>
 <div id="label11" style="display:none">
 <table border="1">
 <tr>
 <td></td>
 <td colspan="1">Supported Version Ranges</td>
 </tr>
 <tr>
 <td>client_id</td>
 <td><code class="docutils literal notranslate">v6.0.0 -> 7.4.3 </code></td>
 </tr>
 </table>
 </div>
 </li>
        <li> <span class="li-head">client_secret</span> - Azure client secret (application key). <span class="li-normal">type: str</span>
 <a id='label12' href="javascript:ContentClick('label13', 'label12');" onmouseover="ContentPreview('label13');" onmouseout="ContentUnpreview('label13');" title="click to collapse or expand..."> more... </a>
 <div id="label13" style="display:none">
 <table border="1">
 <tr>
 <td></td>
 <td colspan="1">Supported Version Ranges</td>
 </tr>
 <tr>
 <td>client_secret</td>
 <td><code class="docutils literal notranslate">v6.0.0 -> 7.4.3 </code></td>
 </tr>
 </table>
 </div>
 </li>
        <li> <span class="li-head">compartment_id</span> - Compartment ID. <span class="li-normal">type: str</span>
 <a id='label14' href="javascript:ContentClick('label15', 'label14');" onmouseover="ContentPreview('label15');" onmouseout="ContentUnpreview('label15');" title="click to collapse or expand..."> more... </a>
 <div id="label15" style="display:none">
 <table border="1">
 <tr>
 <td></td>
 <td colspan="1">Supported Version Ranges</td>
 </tr>
 <tr>
 <td>compartment_id</td>
 <td><code class="docutils literal notranslate">v6.0.0 -> v7.2.4 </code></td>
 </tr>
 </table>
 </div>
 </li>
        <li> <span class="li-head">compartment_list</span> - Configure OCI compartment list. <span class="li-normal">type: list</span> <span style="font-family:'Courier New'" class="li-required">member_path: compartment_list:compartment_id</span>
 <a id='label16' href="javascript:ContentClick('label17', 'label16');" onmouseover="ContentPreview('label17');" onmouseout="ContentUnpreview('label17');" title="click to collapse or expand..."> more... </a>
 <div id="label17" style="display:none">
 <table border="1">
 <tr>
 <td></td><td colspan="1">Supported Version Ranges</td>
 </tr>
 <tr>
 <td>compartment_list</td>
 <td><code class="docutils literal notranslate">v7.4.0 -> 7.4.3 </code></td>
 </tr>
 </table>
 </div>
 </li>
            <ul class="ul-self">
            <li> <span class="li-head">compartment_id</span> - OCI compartment ID. <span class="li-normal">type: str</span> <span class="li-required">required: true</span>
 <a id='label18' href="javascript:ContentClick('label19', 'label18');" onmouseover="ContentPreview('label19');" onmouseout="ContentUnpreview('label19');" title="click to collapse or expand..."> more... </a>
 <div id="label19" style="display:none">
 <table border="1">
 <tr>
 <td></td>
 <td colspan="1">Supported Version Ranges</td>
 </tr>
 <tr>
 <td>compartment_id</td>
 <td><code class="docutils literal notranslate">v7.4.0 -> 7.4.3 </code></td>
 </tr>
 </table>
 </div>
 </li>
            </ul>
        <li> <span class="li-head">compute_generation</span> - Compute generation for IBM cloud infrastructure. <span class="li-normal">type: int</span>
 <a id='label20' href="javascript:ContentClick('label21', 'label20');" onmouseover="ContentPreview('label21');" onmouseout="ContentUnpreview('label21');" title="click to collapse or expand..."> more... </a>
 <div id="label21" style="display:none">
 <table border="1">
 <tr>
 <td></td>
 <td colspan="1">Supported Version Ranges</td>
 </tr>
 <tr>
 <td>compute_generation</td>
 <td><code class="docutils literal notranslate">v6.4.0 -> 7.4.3 </code></td>
 </tr>
 </table>
 </div>
 </li>
        <li> <span class="li-head">domain</span> - Domain name. <span class="li-normal">type: str</span>
 <a id='label22' href="javascript:ContentClick('label23', 'label22');" onmouseover="ContentPreview('label23');" onmouseout="ContentUnpreview('label23');" title="click to collapse or expand..."> more... </a>
 <div id="label23" style="display:none">
 <table border="1">
 <tr>
 <td></td>
 <td colspan="1">Supported Version Ranges</td>
 </tr>
 <tr>
 <td>domain</td>
 <td><code class="docutils literal notranslate">v6.2.0 -> 7.4.3 </code></td>
 </tr>
 </table>
 </div>
 </li>
        <li> <span class="li-head">external_account_list</span> - Configure AWS external account list. <span class="li-normal">type: list</span> <span style="font-family:'Courier New'" class="li-required">member_path: external_account_list:role_arn</span>
 <a id='label24' href="javascript:ContentClick('label25', 'label24');" onmouseover="ContentPreview('label25');" onmouseout="ContentUnpreview('label25');" title="click to collapse or expand..."> more... </a>
 <div id="label25" style="display:none">
 <table border="1">
 <tr>
 <td></td><td colspan="1">Supported Version Ranges</td>
 </tr>
 <tr>
 <td>external_account_list</td>
 <td><code class="docutils literal notranslate">v7.0.4 -> 7.4.3 </code></td>
 </tr>
 </table>
 </div>
 </li>
            <ul class="ul-self">
            <li> <span class="li-head">external_id</span> - AWS external ID. <span class="li-normal">type: str</span>
 <a id='label26' href="javascript:ContentClick('label27', 'label26');" onmouseover="ContentPreview('label27');" onmouseout="ContentUnpreview('label27');" title="click to collapse or expand..."> more... </a>
 <div id="label27" style="display:none">
 <table border="1">
 <tr>
 <td></td>
 <td colspan="2">Supported Version Ranges</td>
 </tr>
 <tr>
 <td>external_id</td>
 <td><code class="docutils literal notranslate">v7.0.8 -> v7.0.12 </code></td>
 <td><code class="docutils literal notranslate">v7.2.1 -> 7.4.3 </code></td>
 </tr>
 </table>
 </div>
 </li>
            <li> <span class="li-head">region_list</span> - AWS region name list. <span class="li-normal">type: list</span> <span style="font-family:'Courier New'" class="li-required">member_path: external_account_list:role_arn/region_list:region</span>
 <a id='label28' href="javascript:ContentClick('label29', 'label28');" onmouseover="ContentPreview('label29');" onmouseout="ContentUnpreview('label29');" title="click to collapse or expand..."> more... </a>
 <div id="label29" style="display:none">
 <table border="1">
 <tr>
 <td></td><td colspan="1">Supported Version Ranges</td>
 </tr>
 <tr>
 <td>region_list</td>
 <td><code class="docutils literal notranslate">v7.0.4 -> 7.4.3 </code></td>
 </tr>
 </table>
 </div>
 </li>
                <ul class="ul-self">
                <li> <span class="li-head">region</span> - AWS region name. <span class="li-normal">type: str</span> <span class="li-required">required: true</span>
 <a id='label30' href="javascript:ContentClick('label31', 'label30');" onmouseover="ContentPreview('label31');" onmouseout="ContentUnpreview('label31');" title="click to collapse or expand..."> more... </a>
 <div id="label31" style="display:none">
 <table border="1">
 <tr>
 <td></td>
 <td colspan="1">Supported Version Ranges</td>
 </tr>
 <tr>
 <td>region</td>
 <td><code class="docutils literal notranslate">v7.0.4 -> 7.4.3 </code></td>
 </tr>
 </table>
 </div>
 </li>
                </ul>
            <li> <span class="li-head">role_arn</span> - AWS role ARN to assume. <span class="li-normal">type: str</span> <span class="li-required">required: true</span>
 <a id='label32' href="javascript:ContentClick('label33', 'label32');" onmouseover="ContentPreview('label33');" onmouseout="ContentUnpreview('label33');" title="click to collapse or expand..."> more... </a>
 <div id="label33" style="display:none">
 <table border="1">
 <tr>
 <td></td>
 <td colspan="1">Supported Version Ranges</td>
 </tr>
 <tr>
 <td>role_arn</td>
 <td><code class="docutils literal notranslate">v7.0.4 -> 7.4.3 </code></td>
 </tr>
 </table>
 </div>
 </li>
            </ul>
        <li> <span class="li-head">external_ip</span> - Configure GCP external IP. <span class="li-normal">type: list</span> <span style="font-family:'Courier New'" class="li-required">member_path: external_ip:name</span>
 <a id='label34' href="javascript:ContentClick('label35', 'label34');" onmouseover="ContentPreview('label35');" onmouseout="ContentUnpreview('label35');" title="click to collapse or expand..."> more... </a>
 <div id="label35" style="display:none">
 <table border="1">
 <tr>
 <td></td><td colspan="1">Supported Version Ranges</td>
 </tr>
 <tr>
 <td>external_ip</td>
 <td><code class="docutils literal notranslate">v6.0.0 -> 7.4.3 </code></td>
 </tr>
 </table>
 </div>
 </li>
            <ul class="ul-self">
            <li> <span class="li-head">name</span> - External IP name. <span class="li-normal">type: str</span> <span class="li-required">required: true</span>
 <a id='label36' href="javascript:ContentClick('label37', 'label36');" onmouseover="ContentPreview('label37');" onmouseout="ContentUnpreview('label37');" title="click to collapse or expand..."> more... </a>
 <div id="label37" style="display:none">
 <table border="1">
 <tr>
 <td></td>
 <td colspan="1">Supported Version Ranges</td>
 </tr>
 <tr>
 <td>name</td>
 <td><code class="docutils literal notranslate">v6.0.0 -> 7.4.3 </code></td>
 </tr>
 </table>
 </div>
 </li>
            </ul>
        <li> <span class="li-head">forwarding_rule</span> - Configure GCP forwarding rule. <span class="li-normal">type: list</span> <span style="font-family:'Courier New'" class="li-required">member_path: forwarding_rule:rule_name</span>
 <a id='label38' href="javascript:ContentClick('label39', 'label38');" onmouseover="ContentPreview('label39');" onmouseout="ContentUnpreview('label39');" title="click to collapse or expand..."> more... </a>
 <div id="label39" style="display:none">
 <table border="1">
 <tr>
 <td></td><td colspan="1">Supported Version Ranges</td>
 </tr>
 <tr>
 <td>forwarding_rule</td>
 <td><code class="docutils literal notranslate">v7.0.2 -> 7.4.3 </code></td>
 </tr>
 </table>
 </div>
 </li>
            <ul class="ul-self">
            <li> <span class="li-head">rule_name</span> - Forwarding rule name. <span class="li-normal">type: str</span> <span class="li-required">required: true</span>
 <a id='label40' href="javascript:ContentClick('label41', 'label40');" onmouseover="ContentPreview('label41');" onmouseout="ContentUnpreview('label41');" title="click to collapse or expand..."> more... </a>
 <div id="label41" style="display:none">
 <table border="1">
 <tr>
 <td></td>
 <td colspan="1">Supported Version Ranges</td>
 </tr>
 <tr>
 <td>rule_name</td>
 <td><code class="docutils literal notranslate">v7.0.2 -> 7.4.3 </code></td>
 </tr>
 </table>
 </div>
 </li>
            <li> <span class="li-head">target</span> - Target instance name. <span class="li-normal">type: str</span>
 <a id='label42' href="javascript:ContentClick('label43', 'label42');" onmouseover="ContentPreview('label43');" onmouseout="ContentUnpreview('label43');" title="click to collapse or expand..."> more... </a>
 <div id="label43" style="display:none">
 <table border="1">
 <tr>
 <td></td>
 <td colspan="1">Supported Version Ranges</td>
 </tr>
 <tr>
 <td>target</td>
 <td><code class="docutils literal notranslate">v7.0.2 -> 7.4.3 </code></td>
 </tr>
 </table>
 </div>
 </li>
            </ul>
        <li> <span class="li-head">gcp_project</span> - GCP project name. <span class="li-normal">type: str</span>
 <a id='label44' href="javascript:ContentClick('label45', 'label44');" onmouseover="ContentPreview('label45');" onmouseout="ContentUnpreview('label45');" title="click to collapse or expand..."> more... </a>
 <div id="label45" style="display:none">
 <table border="1">
 <tr>
 <td></td>
 <td colspan="1">Supported Version Ranges</td>
 </tr>
 <tr>
 <td>gcp_project</td>
 <td><code class="docutils literal notranslate">v6.0.0 -> v7.0.3 </code></td>
 </tr>
 </table>
 </div>
 </li>
        <li> <span class="li-head">gcp_project_list</span> - Configure GCP project list. <span class="li-normal">type: list</span> <span style="font-family:'Courier New'" class="li-required">member_path: gcp_project_list:id</span>
 <a id='label46' href="javascript:ContentClick('label47', 'label46');" onmouseover="ContentPreview('label47');" onmouseout="ContentUnpreview('label47');" title="click to collapse or expand..."> more... </a>
 <div id="label47" style="display:none">
 <table border="1">
 <tr>
 <td></td><td colspan="1">Supported Version Ranges</td>
 </tr>
 <tr>
 <td>gcp_project_list</td>
 <td><code class="docutils literal notranslate">v7.0.4 -> 7.4.3 </code></td>
 </tr>
 </table>
 </div>
 </li>
            <ul class="ul-self">
            <li> <span class="li-head">gcp_zone_list</span> - Configure GCP zone list. <span class="li-normal">type: list</span> <span style="font-family:'Courier New'" class="li-required">member_path: gcp_project_list:id/gcp_zone_list:name</span>
 <a id='label48' href="javascript:ContentClick('label49', 'label48');" onmouseover="ContentPreview('label49');" onmouseout="ContentUnpreview('label49');" title="click to collapse or expand..."> more... </a>
 <div id="label49" style="display:none">
 <table border="1">
 <tr>
 <td></td><td colspan="1">Supported Version Ranges</td>
 </tr>
 <tr>
 <td>gcp_zone_list</td>
 <td><code class="docutils literal notranslate">v7.0.4 -> 7.4.3 </code></td>
 </tr>
 </table>
 </div>
 </li>
                <ul class="ul-self">
                <li> <span class="li-head">name</span> - GCP zone name. <span class="li-normal">type: str</span> <span class="li-required">required: true</span>
 <a id='label50' href="javascript:ContentClick('label51', 'label50');" onmouseover="ContentPreview('label51');" onmouseout="ContentUnpreview('label51');" title="click to collapse or expand..."> more... </a>
 <div id="label51" style="display:none">
 <table border="1">
 <tr>
 <td></td>
 <td colspan="1">Supported Version Ranges</td>
 </tr>
 <tr>
 <td>name</td>
 <td><code class="docutils literal notranslate">v7.0.4 -> 7.4.3 </code></td>
 </tr>
 </table>
 </div>
 </li>
                </ul>
            <li> <span class="li-head">id</span> - GCP project ID. <span class="li-normal">type: str</span> <span class="li-required">required: true</span>
 <a id='label52' href="javascript:ContentClick('label53', 'label52');" onmouseover="ContentPreview('label53');" onmouseout="ContentUnpreview('label53');" title="click to collapse or expand..."> more... </a>
 <div id="label53" style="display:none">
 <table border="1">
 <tr>
 <td></td>
 <td colspan="1">Supported Version Ranges</td>
 </tr>
 <tr>
 <td>id</td>
 <td><code class="docutils literal notranslate">v7.0.4 -> 7.4.3 </code></td>
 </tr>
 </table>
 </div>
 </li>
            </ul>
        <li> <span class="li-head">group_name</span> - Full path group name of computers. <span class="li-normal">type: str</span>
 <a id='label54' href="javascript:ContentClick('label55', 'label54');" onmouseover="ContentPreview('label55');" onmouseout="ContentUnpreview('label55');" title="click to collapse or expand..."> more... </a>
 <div id="label55" style="display:none">
 <table border="1">
 <tr>
 <td></td>
 <td colspan="1">Supported Version Ranges</td>
 </tr>
 <tr>
 <td>group_name</td>
 <td><code class="docutils literal notranslate">v6.2.0 -> 7.4.3 </code></td>
 </tr>
 </table>
 </div>
 </li>
        <li> <span class="li-head">ha_status</span> - Enable/disable use for FortiGate HA service. <span class="li-normal">type: str</span> <span class="li-normal">choices: disable, enable</span>
 <a id='label56' href="javascript:ContentClick('label57', 'label56');" onmouseover="ContentPreview('label57');" onmouseout="ContentUnpreview('label57');" title="click to collapse or expand..."> more... </a>
 <div id="label57" style="display:none">
 <table border="1">
 <tr>
 <td></td>
 <td colspan="1">Supported Version Ranges</td>
 </tr>
 <tr>
 <td>ha_status</td>
 <td><code class="docutils literal notranslate">v6.2.0 -> 7.4.3 </code></td>
 </tr>
 <tr>
 <td>[disable]</td>
 <td><code class="docutils literal notranslate">v6.2.0 -> 7.4.3</code></td>
 <tr>
 <td>[enable]</td>
 <td><code class="docutils literal notranslate">v6.2.0 -> 7.4.3</code></td>
 </table>
 </div>
 </li>
        <li> <span class="li-head">ibm_region</span> - IBM cloud region name. <span class="li-normal">type: str</span> <span class="li-normal">choices: dallas, washington-dc, london, frankfurt, sydney, tokyo, osaka, toronto, sao-paulo, us-south, us-east, germany, great-britain, japan, australia</span>
 <a id='label58' href="javascript:ContentClick('label59', 'label58');" onmouseover="ContentPreview('label59');" onmouseout="ContentUnpreview('label59');" title="click to collapse or expand..."> more... </a>
 <div id="label59" style="display:none">
 <table border="1">
 <tr>
 <td></td>
 <td colspan="2">Supported Version Ranges</td>
 </tr>
 <tr>
 <td>ibm_region</td>
 <td><code class="docutils literal notranslate">v6.4.0 -> v6.4.0 </code></td>
 <td><code class="docutils literal notranslate">v6.4.4 -> 7.4.3 </code></td>
 </tr>
 <tr>
 <td>[dallas]</td>
 <td><code class="docutils literal notranslate">v7.0.4 -> 7.4.3</code></td>
 </tr>
 <tr>
 <td>[washington-dc]</td>
 <td><code class="docutils literal notranslate">v7.0.4 -> 7.4.3</code></td>
 </tr>
 <tr>
 <td>[london]</td>
 <td><code class="docutils literal notranslate">v7.0.4 -> 7.4.3</code></td>
 </tr>
 <tr>
 <td>[frankfurt]</td>
 <td><code class="docutils literal notranslate">v7.0.4 -> 7.4.3</code></td>
 </tr>
 <tr>
 <td>[sydney]</td>
 <td><code class="docutils literal notranslate">v7.0.4 -> 7.4.3</code></td>
 </tr>
 <tr>
 <td>[tokyo]</td>
 <td><code class="docutils literal notranslate">v7.0.4 -> 7.4.3</code></td>
 </tr>
 <tr>
 <td>[osaka]</td>
 <td><code class="docutils literal notranslate">v7.0.4 -> 7.4.3</code></td>
 </tr>
 <tr>
 <td>[toronto]</td>
 <td><code class="docutils literal notranslate">v7.0.4 -> 7.4.3</code></td>
 </tr>
 <tr>
 <td>[sao-paulo]</td>
 <td><code class="docutils literal notranslate">v7.0.4 -> 7.4.3</code></td>
 </tr>
 <tr>
 <td>[us-south]</td>
 <td><code class="docutils literal notranslate">v6.4.0 -> v6.4.0</code></td>
 <td><code class="docutils literal notranslate">v6.4.4 -> v7.0.3</code></td>
 </tr>
 <tr>
 <td>[us-east]</td>
 <td><code class="docutils literal notranslate">v6.4.0 -> v6.4.0</code></td>
 <td><code class="docutils literal notranslate">v6.4.4 -> v7.0.3</code></td>
 </tr>
 <tr>
 <td>[germany]</td>
 <td><code class="docutils literal notranslate">v6.4.0 -> v6.4.0</code></td>
 <td><code class="docutils literal notranslate">v6.4.4 -> v7.0.3</code></td>
 </tr>
 <tr>
 <td>[great-britain]</td>
 <td><code class="docutils literal notranslate">v6.4.0 -> v6.4.0</code></td>
 <td><code class="docutils literal notranslate">v6.4.4 -> v7.0.3</code></td>
 </tr>
 <tr>
 <td>[japan]</td>
 <td><code class="docutils literal notranslate">v6.4.0 -> v6.4.0</code></td>
 <td><code class="docutils literal notranslate">v6.4.4 -> v7.0.3</code></td>
 </tr>
 <tr>
 <td>[australia]</td>
 <td><code class="docutils literal notranslate">v6.4.0 -> v6.4.0</code></td>
 <td><code class="docutils literal notranslate">v6.4.4 -> v7.0.3</code></td>
 </tr>
 </table>
 </div>
 </li>
        <li> <span class="li-head">ibm_region_gen1</span> - IBM cloud compute generation 1 region name. <span class="li-normal">type: str</span> <span class="li-normal">choices: us-south, us-east, germany, great-britain, japan, australia</span>
 <a id='label60' href="javascript:ContentClick('label61', 'label60');" onmouseover="ContentPreview('label61');" onmouseout="ContentUnpreview('label61');" title="click to collapse or expand..."> more... </a>
 <div id="label61" style="display:none">
 <table border="1">
 <tr>
 <td></td>
 <td colspan="1">Supported Version Ranges</td>
 </tr>
 <tr>
 <td>ibm_region_gen1</td>
 <td><code class="docutils literal notranslate">v6.4.1 -> v6.4.1 </code></td>
 </tr>
 <tr>
 <td>[us-south]</td>
 <td><code class="docutils literal notranslate">v6.4.1 -> v6.4.1</code></td>
 <tr>
 <td>[us-east]</td>
 <td><code class="docutils literal notranslate">v6.4.1 -> v6.4.1</code></td>
 <tr>
 <td>[germany]</td>
 <td><code class="docutils literal notranslate">v6.4.1 -> v6.4.1</code></td>
 <tr>
 <td>[great-britain]</td>
 <td><code class="docutils literal notranslate">v6.4.1 -> v6.4.1</code></td>
 <tr>
 <td>[japan]</td>
 <td><code class="docutils literal notranslate">v6.4.1 -> v6.4.1</code></td>
 <tr>
 <td>[australia]</td>
 <td><code class="docutils literal notranslate">v6.4.1 -> v6.4.1</code></td>
 </table>
 </div>
 </li>
        <li> <span class="li-head">ibm_region_gen2</span> - IBM cloud compute generation 2 region name. <span class="li-normal">type: str</span> <span class="li-normal">choices: us-south, us-east, great-britain</span>
 <a id='label62' href="javascript:ContentClick('label63', 'label62');" onmouseover="ContentPreview('label63');" onmouseout="ContentUnpreview('label63');" title="click to collapse or expand..."> more... </a>
 <div id="label63" style="display:none">
 <table border="1">
 <tr>
 <td></td>
 <td colspan="1">Supported Version Ranges</td>
 </tr>
 <tr>
 <td>ibm_region_gen2</td>
 <td><code class="docutils literal notranslate">v6.4.1 -> v6.4.1 </code></td>
 </tr>
 <tr>
 <td>[us-south]</td>
 <td><code class="docutils literal notranslate">v6.4.1 -> v6.4.1</code></td>
 <tr>
 <td>[us-east]</td>
 <td><code class="docutils literal notranslate">v6.4.1 -> v6.4.1</code></td>
 <tr>
 <td>[great-britain]</td>
 <td><code class="docutils literal notranslate">v6.4.1 -> v6.4.1</code></td>
 </table>
 </div>
 </li>
        <li> <span class="li-head">key_passwd</span> - Private key password. <span class="li-normal">type: str</span>
 <a id='label64' href="javascript:ContentClick('label65', 'label64');" onmouseover="ContentPreview('label65');" onmouseout="ContentUnpreview('label65');" title="click to collapse or expand..."> more... </a>
 <div id="label65" style="display:none">
 <table border="1">
 <tr>
 <td></td>
 <td colspan="2">Supported Version Ranges</td>
 </tr>
 <tr>
 <td>key_passwd</td>
 <td><code class="docutils literal notranslate">v6.0.0 -> v6.0.11 </code></td>
 <td><code class="docutils literal notranslate">v6.2.3 -> v6.2.3 </code></td>
 </tr>
 </table>
 </div>
 </li>
        <li> <span class="li-head">login_endpoint</span> - Azure Stack login endpoint. <span class="li-normal">type: str</span>
 <a id='label66' href="javascript:ContentClick('label67', 'label66');" onmouseover="ContentPreview('label67');" onmouseout="ContentUnpreview('label67');" title="click to collapse or expand..."> more... </a>
 <div id="label67" style="display:none">
 <table border="1">
 <tr>
 <td></td>
 <td colspan="1">Supported Version Ranges</td>
 </tr>
 <tr>
 <td>login_endpoint</td>
 <td><code class="docutils literal notranslate">v6.0.0 -> 7.4.3 </code></td>
 </tr>
 </table>
 </div>
 </li>
        <li> <span class="li-head">name</span> - SDN connector name. <span class="li-normal">type: str</span> <span class="li-required">required: true</span>
 <a id='label68' href="javascript:ContentClick('label69', 'label68');" onmouseover="ContentPreview('label69');" onmouseout="ContentUnpreview('label69');" title="click to collapse or expand..."> more... </a>
 <div id="label69" style="display:none">
 <table border="1">
 <tr>
 <td></td>
 <td colspan="1">Supported Version Ranges</td>
 </tr>
 <tr>
 <td>name</td>
 <td><code class="docutils literal notranslate">v6.0.0 -> 7.4.3 </code></td>
 </tr>
 </table>
 </div>
 </li>
        <li> <span class="li-head">nic</span> - Configure Azure network interface. <span class="li-normal">type: list</span> <span style="font-family:'Courier New'" class="li-required">member_path: nic:name</span>
 <a id='label70' href="javascript:ContentClick('label71', 'label70');" onmouseover="ContentPreview('label71');" onmouseout="ContentUnpreview('label71');" title="click to collapse or expand..."> more... </a>
 <div id="label71" style="display:none">
 <table border="1">
 <tr>
 <td></td><td colspan="1">Supported Version Ranges</td>
 </tr>
 <tr>
 <td>nic</td>
 <td><code class="docutils literal notranslate">v6.0.0 -> 7.4.3 </code></td>
 </tr>
 </table>
 </div>
 </li>
            <ul class="ul-self">
            <li> <span class="li-head">ip</span> - Configure IP configuration. <span class="li-normal">type: list</span> <span style="font-family:'Courier New'" class="li-required">member_path: nic:name/ip:name</span>
 <a id='label72' href="javascript:ContentClick('label73', 'label72');" onmouseover="ContentPreview('label73');" onmouseout="ContentUnpreview('label73');" title="click to collapse or expand..."> more... </a>
 <div id="label73" style="display:none">
 <table border="1">
 <tr>
 <td></td><td colspan="1">Supported Version Ranges</td>
 </tr>
 <tr>
 <td>ip</td>
 <td><code class="docutils literal notranslate">v6.0.0 -> 7.4.3 </code></td>
 </tr>
 </table>
 </div>
 </li>
                <ul class="ul-self">
                <li> <span class="li-head">name</span> - IP configuration name. <span class="li-normal">type: str</span> <span class="li-required">required: true</span>
 <a id='label74' href="javascript:ContentClick('label75', 'label74');" onmouseover="ContentPreview('label75');" onmouseout="ContentUnpreview('label75');" title="click to collapse or expand..."> more... </a>
 <div id="label75" style="display:none">
 <table border="1">
 <tr>
 <td></td>
 <td colspan="1">Supported Version Ranges</td>
 </tr>
 <tr>
 <td>name</td>
 <td><code class="docutils literal notranslate">v6.0.0 -> 7.4.3 </code></td>
 </tr>
 </table>
 </div>
 </li>
                <li> <span class="li-head">public_ip</span> - Public IP name. <span class="li-normal">type: str</span>
 <a id='label76' href="javascript:ContentClick('label77', 'label76');" onmouseover="ContentPreview('label77');" onmouseout="ContentUnpreview('label77');" title="click to collapse or expand..."> more... </a>
 <div id="label77" style="display:none">
 <table border="1">
 <tr>
 <td></td>
 <td colspan="1">Supported Version Ranges</td>
 </tr>
 <tr>
 <td>public_ip</td>
 <td><code class="docutils literal notranslate">v6.0.0 -> 7.4.3 </code></td>
 </tr>
 </table>
 </div>
 </li>
                <li> <span class="li-head">resource_group</span> - Resource group of Azure public IP. <span class="li-normal">type: str</span>
 <a id='label78' href="javascript:ContentClick('label79', 'label78');" onmouseover="ContentPreview('label79');" onmouseout="ContentUnpreview('label79');" title="click to collapse or expand..."> more... </a>
 <div id="label79" style="display:none">
 <table border="1">
 <tr>
 <td></td>
 <td colspan="1">Supported Version Ranges</td>
 </tr>
 <tr>
 <td>resource_group</td>
 <td><code class="docutils literal notranslate">v6.2.0 -> 7.4.3 </code></td>
 </tr>
 </table>
 </div>
 </li>
                </ul>
            <li> <span class="li-head">name</span> - Network interface name. <span class="li-normal">type: str</span> <span class="li-required">required: true</span>
 <a id='label80' href="javascript:ContentClick('label81', 'label80');" onmouseover="ContentPreview('label81');" onmouseout="ContentUnpreview('label81');" title="click to collapse or expand..."> more... </a>
 <div id="label81" style="display:none">
 <table border="1">
 <tr>
 <td></td>
 <td colspan="1">Supported Version Ranges</td>
 </tr>
 <tr>
 <td>name</td>
 <td><code class="docutils literal notranslate">v6.0.0 -> 7.4.3 </code></td>
 </tr>
 </table>
 </div>
 </li>
            </ul>
        <li> <span class="li-head">oci_cert</span> - OCI certificate. Source certificate.local.name. <span class="li-normal">type: str</span>
 <a id='label82' href="javascript:ContentClick('label83', 'label82');" onmouseover="ContentPreview('label83');" onmouseout="ContentUnpreview('label83');" title="click to collapse or expand..."> more... </a>
 <div id="label83" style="display:none">
 <table border="1">
 <tr>
 <td></td>
 <td colspan="1">Supported Version Ranges</td>
 </tr>
 <tr>
 <td>oci_cert</td>
 <td><code class="docutils literal notranslate">v6.0.0 -> 7.4.3 </code></td>
 </tr>
 </table>
 </div>
 </li>
        <li> <span class="li-head">oci_fingerprint</span> - OCI pubkey fingerprint. <span class="li-normal">type: str</span>
 <a id='label84' href="javascript:ContentClick('label85', 'label84');" onmouseover="ContentPreview('label85');" onmouseout="ContentUnpreview('label85');" title="click to collapse or expand..."> more... </a>
 <div id="label85" style="display:none">
 <table border="1">
 <tr>
 <td></td>
 <td colspan="2">Supported Version Ranges</td>
 </tr>
 <tr>
 <td>oci_fingerprint</td>
 <td><code class="docutils literal notranslate">v6.0.0 -> v7.0.5 </code></td>
 <td><code class="docutils literal notranslate">v7.2.0 -> v7.2.0 </code></td>
 </tr>
 </table>
 </div>
 </li>
        <li> <span class="li-head">oci_region</span> - OCI server region. <span class="li-normal">type: str</span> <span class="li-normal">choices: phoenix, ashburn, frankfurt, london</span>
 <a id='label86' href="javascript:ContentClick('label87', 'label86');" onmouseover="ContentPreview('label87');" onmouseout="ContentUnpreview('label87');" title="click to collapse or expand..."> more... </a>
 <div id="label87" style="display:none">
 <table border="1">
 <tr>
 <td></td>
 <td colspan="1">Supported Version Ranges</td>
 </tr>
 <tr>
 <td>oci_region</td>
 <td><code class="docutils literal notranslate">v6.0.0 -> v7.2.4 </code></td>
 </tr>
 <tr>
 <td>[phoenix]</td>
 <td><code class="docutils literal notranslate">v6.0.0 -> v6.0.11</code></td>
 </tr>
 <tr>
 <td>[ashburn]</td>
 <td><code class="docutils literal notranslate">v6.0.0 -> v6.0.11</code></td>
 </tr>
 <tr>
 <td>[frankfurt]</td>
 <td><code class="docutils literal notranslate">v6.0.0 -> v6.0.11</code></td>
 </tr>
 <tr>
 <td>[london]</td>
 <td><code class="docutils literal notranslate">v6.0.0 -> v6.0.11</code></td>
 </tr>
 </table>
 </div>
 </li>
        <li> <span class="li-head">oci_region_list</span> - Configure OCI region list. <span class="li-normal">type: list</span> <span style="font-family:'Courier New'" class="li-required">member_path: oci_region_list:region</span>
 <a id='label88' href="javascript:ContentClick('label89', 'label88');" onmouseover="ContentPreview('label89');" onmouseout="ContentUnpreview('label89');" title="click to collapse or expand..."> more... </a>
 <div id="label89" style="display:none">
 <table border="1">
 <tr>
 <td></td><td colspan="1">Supported Version Ranges</td>
 </tr>
 <tr>
 <td>oci_region_list</td>
 <td><code class="docutils literal notranslate">v7.4.0 -> 7.4.3 </code></td>
 </tr>
 </table>
 </div>
 </li>
            <ul class="ul-self">
            <li> <span class="li-head">region</span> - OCI region. <span class="li-normal">type: str</span> <span class="li-required">required: true</span>
 <a id='label90' href="javascript:ContentClick('label91', 'label90');" onmouseover="ContentPreview('label91');" onmouseout="ContentUnpreview('label91');" title="click to collapse or expand..."> more... </a>
 <div id="label91" style="display:none">
 <table border="1">
 <tr>
 <td></td>
 <td colspan="1">Supported Version Ranges</td>
 </tr>
 <tr>
 <td>region</td>
 <td><code class="docutils literal notranslate">v7.4.0 -> 7.4.3 </code></td>
 </tr>
 </table>
 </div>
 </li>
            </ul>
        <li> <span class="li-head">oci_region_type</span> - OCI region type. <span class="li-normal">type: str</span> <span class="li-normal">choices: commercial, government</span>
 <a id='label92' href="javascript:ContentClick('label93', 'label92');" onmouseover="ContentPreview('label93');" onmouseout="ContentUnpreview('label93');" title="click to collapse or expand..."> more... </a>
 <div id="label93" style="display:none">
 <table border="1">
 <tr>
 <td></td>
 <td colspan="1">Supported Version Ranges</td>
 </tr>
 <tr>
 <td>oci_region_type</td>
 <td><code class="docutils literal notranslate">v6.2.0 -> 7.4.3 </code></td>
 </tr>
 <tr>
 <td>[commercial]</td>
 <td><code class="docutils literal notranslate">v6.2.0 -> 7.4.3</code></td>
 <tr>
 <td>[government]</td>
 <td><code class="docutils literal notranslate">v6.2.0 -> 7.4.3</code></td>
 </table>
 </div>
 </li>
        <li> <span class="li-head">password</span> - Password of the remote SDN connector as login credentials. <span class="li-normal">type: str</span>
 <a id='label94' href="javascript:ContentClick('label95', 'label94');" onmouseover="ContentPreview('label95');" onmouseout="ContentUnpreview('label95');" title="click to collapse or expand..."> more... </a>
 <div id="label95" style="display:none">
 <table border="1">
 <tr>
 <td></td>
 <td colspan="1">Supported Version Ranges</td>
 </tr>
 <tr>
 <td>password</td>
 <td><code class="docutils literal notranslate">v6.0.0 -> 7.4.3 </code></td>
 </tr>
 </table>
 </div>
 </li>
        <li> <span class="li-head">private_key</span> - Private key of GCP service account. <span class="li-normal">type: str</span>
 <a id='label96' href="javascript:ContentClick('label97', 'label96');" onmouseover="ContentPreview('label97');" onmouseout="ContentUnpreview('label97');" title="click to collapse or expand..."> more... </a>
 <div id="label97" style="display:none">
 <table border="1">
 <tr>
 <td></td>
 <td colspan="1">Supported Version Ranges</td>
 </tr>
 <tr>
 <td>private_key</td>
 <td><code class="docutils literal notranslate">v6.0.0 -> 7.4.3 </code></td>
 </tr>
 </table>
 </div>
 </li>
        <li> <span class="li-head">proxy</span> - SDN proxy. Source system.sdn-proxy.name. <span class="li-normal">type: str</span>
 <a id='label98' href="javascript:ContentClick('label99', 'label98');" onmouseover="ContentPreview('label99');" onmouseout="ContentUnpreview('label99');" title="click to collapse or expand..."> more... </a>
 <div id="label99" style="display:none">
 <table border="1">
 <tr>
 <td></td>
 <td colspan="1">Supported Version Ranges</td>
 </tr>
 <tr>
 <td>proxy</td>
 <td><code class="docutils literal notranslate">v7.4.0 -> 7.4.3 </code></td>
 </tr>
 </table>
 </div>
 </li>
        <li> <span class="li-head">region</span> - AWS / ACS region name. <span class="li-normal">type: str</span>
 <a id='label100' href="javascript:ContentClick('label101', 'label100');" onmouseover="ContentPreview('label101');" onmouseout="ContentUnpreview('label101');" title="click to collapse or expand..."> more... </a>
 <div id="label101" style="display:none">
 <table border="1">
 <tr>
 <td></td>
 <td colspan="1">Supported Version Ranges</td>
 </tr>
 <tr>
 <td>region</td>
 <td><code class="docutils literal notranslate">v6.0.0 -> 7.4.3 </code></td>
 </tr>
 </table>
 </div>
 </li>
        <li> <span class="li-head">resource_group</span> - Azure resource group. <span class="li-normal">type: str</span>
 <a id='label102' href="javascript:ContentClick('label103', 'label102');" onmouseover="ContentPreview('label103');" onmouseout="ContentUnpreview('label103');" title="click to collapse or expand..."> more... </a>
 <div id="label103" style="display:none">
 <table border="1">
 <tr>
 <td></td>
 <td colspan="1">Supported Version Ranges</td>
 </tr>
 <tr>
 <td>resource_group</td>
 <td><code class="docutils literal notranslate">v6.0.0 -> 7.4.3 </code></td>
 </tr>
 </table>
 </div>
 </li>
        <li> <span class="li-head">resource_url</span> - Azure Stack resource URL. <span class="li-normal">type: str</span>
 <a id='label104' href="javascript:ContentClick('label105', 'label104');" onmouseover="ContentPreview('label105');" onmouseout="ContentUnpreview('label105');" title="click to collapse or expand..."> more... </a>
 <div id="label105" style="display:none">
 <table border="1">
 <tr>
 <td></td>
 <td colspan="1">Supported Version Ranges</td>
 </tr>
 <tr>
 <td>resource_url</td>
 <td><code class="docutils literal notranslate">v6.0.0 -> 7.4.3 </code></td>
 </tr>
 </table>
 </div>
 </li>
        <li> <span class="li-head">route</span> - Configure GCP route. <span class="li-normal">type: list</span> <span style="font-family:'Courier New'" class="li-required">member_path: route:name</span>
 <a id='label106' href="javascript:ContentClick('label107', 'label106');" onmouseover="ContentPreview('label107');" onmouseout="ContentUnpreview('label107');" title="click to collapse or expand..."> more... </a>
 <div id="label107" style="display:none">
 <table border="1">
 <tr>
 <td></td><td colspan="1">Supported Version Ranges</td>
 </tr>
 <tr>
 <td>route</td>
 <td><code class="docutils literal notranslate">v6.0.0 -> 7.4.3 </code></td>
 </tr>
 </table>
 </div>
 </li>
            <ul class="ul-self">
            <li> <span class="li-head">name</span> - Route name. <span class="li-normal">type: str</span> <span class="li-required">required: true</span>
 <a id='label108' href="javascript:ContentClick('label109', 'label108');" onmouseover="ContentPreview('label109');" onmouseout="ContentUnpreview('label109');" title="click to collapse or expand..."> more... </a>
 <div id="label109" style="display:none">
 <table border="1">
 <tr>
 <td></td>
 <td colspan="1">Supported Version Ranges</td>
 </tr>
 <tr>
 <td>name</td>
 <td><code class="docutils literal notranslate">v6.0.0 -> 7.4.3 </code></td>
 </tr>
 </table>
 </div>
 </li>
            </ul>
        <li> <span class="li-head">route_table</span> - Configure Azure route table. <span class="li-normal">type: list</span> <span style="font-family:'Courier New'" class="li-required">member_path: route_table:name</span>
 <a id='label110' href="javascript:ContentClick('label111', 'label110');" onmouseover="ContentPreview('label111');" onmouseout="ContentUnpreview('label111');" title="click to collapse or expand..."> more... </a>
 <div id="label111" style="display:none">
 <table border="1">
 <tr>
 <td></td><td colspan="1">Supported Version Ranges</td>
 </tr>
 <tr>
 <td>route_table</td>
 <td><code class="docutils literal notranslate">v6.0.0 -> 7.4.3 </code></td>
 </tr>
 </table>
 </div>
 </li>
            <ul class="ul-self">
            <li> <span class="li-head">name</span> - Route table name. <span class="li-normal">type: str</span> <span class="li-required">required: true</span>
 <a id='label112' href="javascript:ContentClick('label113', 'label112');" onmouseover="ContentPreview('label113');" onmouseout="ContentUnpreview('label113');" title="click to collapse or expand..."> more... </a>
 <div id="label113" style="display:none">
 <table border="1">
 <tr>
 <td></td>
 <td colspan="1">Supported Version Ranges</td>
 </tr>
 <tr>
 <td>name</td>
 <td><code class="docutils literal notranslate">v6.0.0 -> 7.4.3 </code></td>
 </tr>
 </table>
 </div>
 </li>
            <li> <span class="li-head">resource_group</span> - Resource group of Azure route table. <span class="li-normal">type: str</span>
 <a id='label114' href="javascript:ContentClick('label115', 'label114');" onmouseover="ContentPreview('label115');" onmouseout="ContentUnpreview('label115');" title="click to collapse or expand..."> more... </a>
 <div id="label115" style="display:none">
 <table border="1">
 <tr>
 <td></td>
 <td colspan="1">Supported Version Ranges</td>
 </tr>
 <tr>
 <td>resource_group</td>
 <td><code class="docutils literal notranslate">v6.2.0 -> 7.4.3 </code></td>
 </tr>
 </table>
 </div>
 </li>
            <li> <span class="li-head">route</span> - Configure Azure route. <span class="li-normal">type: list</span> <span style="font-family:'Courier New'" class="li-required">member_path: route_table:name/route:name</span>
 <a id='label116' href="javascript:ContentClick('label117', 'label116');" onmouseover="ContentPreview('label117');" onmouseout="ContentUnpreview('label117');" title="click to collapse or expand..."> more... </a>
 <div id="label117" style="display:none">
 <table border="1">
 <tr>
 <td></td><td colspan="1">Supported Version Ranges</td>
 </tr>
 <tr>
 <td>route</td>
 <td><code class="docutils literal notranslate">v6.0.0 -> 7.4.3 </code></td>
 </tr>
 </table>
 </div>
 </li>
                <ul class="ul-self">
                <li> <span class="li-head">name</span> - Route name. <span class="li-normal">type: str</span> <span class="li-required">required: true</span>
 <a id='label118' href="javascript:ContentClick('label119', 'label118');" onmouseover="ContentPreview('label119');" onmouseout="ContentUnpreview('label119');" title="click to collapse or expand..."> more... </a>
 <div id="label119" style="display:none">
 <table border="1">
 <tr>
 <td></td>
 <td colspan="1">Supported Version Ranges</td>
 </tr>
 <tr>
 <td>name</td>
 <td><code class="docutils literal notranslate">v6.0.0 -> 7.4.3 </code></td>
 </tr>
 </table>
 </div>
 </li>
                <li> <span class="li-head">next_hop</span> - Next hop address. <span class="li-normal">type: str</span>
 <a id='label120' href="javascript:ContentClick('label121', 'label120');" onmouseover="ContentPreview('label121');" onmouseout="ContentUnpreview('label121');" title="click to collapse or expand..."> more... </a>
 <div id="label121" style="display:none">
 <table border="1">
 <tr>
 <td></td>
 <td colspan="1">Supported Version Ranges</td>
 </tr>
 <tr>
 <td>next_hop</td>
 <td><code class="docutils literal notranslate">v6.0.0 -> 7.4.3 </code></td>
 </tr>
 </table>
 </div>
 </li>
                </ul>
            <li> <span class="li-head">subscription_id</span> - Subscription ID of Azure route table. <span class="li-normal">type: str</span>
 <a id='label122' href="javascript:ContentClick('label123', 'label122');" onmouseover="ContentPreview('label123');" onmouseout="ContentUnpreview('label123');" title="click to collapse or expand..."> more... </a>
 <div id="label123" style="display:none">
 <table border="1">
 <tr>
 <td></td>
 <td colspan="2">Supported Version Ranges</td>
 </tr>
 <tr>
 <td>subscription_id</td>
 <td><code class="docutils literal notranslate">v6.2.0 -> v6.2.0 </code></td>
 <td><code class="docutils literal notranslate">v6.2.5 -> 7.4.3 </code></td>
 </tr>
 </table>
 </div>
 </li>
            </ul>
        <li> <span class="li-head">secret_key</span> - AWS / ACS secret access key. <span class="li-normal">type: str</span>
 <a id='label124' href="javascript:ContentClick('label125', 'label124');" onmouseover="ContentPreview('label125');" onmouseout="ContentUnpreview('label125');" title="click to collapse or expand..."> more... </a>
 <div id="label125" style="display:none">
 <table border="1">
 <tr>
 <td></td>
 <td colspan="1">Supported Version Ranges</td>
 </tr>
 <tr>
 <td>secret_key</td>
 <td><code class="docutils literal notranslate">v6.0.0 -> 7.4.3 </code></td>
 </tr>
 </table>
 </div>
 </li>
        <li> <span class="li-head">secret_token</span> - Secret token of Kubernetes service account. <span class="li-normal">type: str</span>
 <a id='label126' href="javascript:ContentClick('label127', 'label126');" onmouseover="ContentPreview('label127');" onmouseout="ContentUnpreview('label127');" title="click to collapse or expand..."> more... </a>
 <div id="label127" style="display:none">
 <table border="1">
 <tr>
 <td></td>
 <td colspan="1">Supported Version Ranges</td>
 </tr>
 <tr>
 <td>secret_token</td>
 <td><code class="docutils literal notranslate">v6.2.0 -> 7.4.3 </code></td>
 </tr>
 </table>
 </div>
 </li>
        <li> <span class="li-head">server</span> - Server address of the remote SDN connector. <span class="li-normal">type: str</span>
 <a id='label128' href="javascript:ContentClick('label129', 'label128');" onmouseover="ContentPreview('label129');" onmouseout="ContentUnpreview('label129');" title="click to collapse or expand..."> more... </a>
 <div id="label129" style="display:none">
 <table border="1">
 <tr>
 <td></td>
 <td colspan="1">Supported Version Ranges</td>
 </tr>
 <tr>
 <td>server</td>
 <td><code class="docutils literal notranslate">v6.0.0 -> 7.4.3 </code></td>
 </tr>
 </table>
 </div>
 </li>
        <li> <span class="li-head">server_ca_cert</span> - Trust only those servers whose certificate is directly/indirectly signed by this certificate. Source certificate.remote.name certificate .ca.name. <span class="li-normal">type: str</span>
 <a id='label130' href="javascript:ContentClick('label131', 'label130');" onmouseover="ContentPreview('label131');" onmouseout="ContentUnpreview('label131');" title="click to collapse or expand..."> more... </a>
 <div id="label131" style="display:none">
 <table border="1">
 <tr>
 <td></td>
 <td colspan="1">Supported Version Ranges</td>
 </tr>
 <tr>
 <td>server_ca_cert</td>
 <td><code class="docutils literal notranslate">v7.2.4 -> 7.4.3 </code></td>
 </tr>
 </table>
 </div>
 </li>
        <li> <span class="li-head">server_cert</span> - Trust servers that contain this certificate only. Source certificate.remote.name. <span class="li-normal">type: str</span>
 <a id='label132' href="javascript:ContentClick('label133', 'label132');" onmouseover="ContentPreview('label133');" onmouseout="ContentUnpreview('label133');" title="click to collapse or expand..."> more... </a>
 <div id="label133" style="display:none">
 <table border="1">
 <tr>
 <td></td>
 <td colspan="1">Supported Version Ranges</td>
 </tr>
 <tr>
 <td>server_cert</td>
 <td><code class="docutils literal notranslate">v7.2.4 -> 7.4.3 </code></td>
 </tr>
 </table>
 </div>
 </li>
        <li> <span class="li-head">server_list</span> - Server address list of the remote SDN connector. <span class="li-normal">type: list</span> <span style="font-family:'Courier New'" class="li-required">member_path: server_list:ip</span>
 <a id='label134' href="javascript:ContentClick('label135', 'label134');" onmouseover="ContentPreview('label135');" onmouseout="ContentUnpreview('label135');" title="click to collapse or expand..."> more... </a>
 <div id="label135" style="display:none">
 <table border="1">
 <tr>
 <td></td><td colspan="1">Supported Version Ranges</td>
 </tr>
 <tr>
 <td>server_list</td>
 <td><code class="docutils literal notranslate">v6.4.4 -> 7.4.3 </code></td>
 </tr>
 </table>
 </div>
 </li>
            <ul class="ul-self">
            <li> <span class="li-head">ip</span> - IPv4 address. <span class="li-normal">type: str</span> <span class="li-required">required: true</span>
 <a id='label136' href="javascript:ContentClick('label137', 'label136');" onmouseover="ContentPreview('label137');" onmouseout="ContentUnpreview('label137');" title="click to collapse or expand..."> more... </a>
 <div id="label137" style="display:none">
 <table border="1">
 <tr>
 <td></td>
 <td colspan="1">Supported Version Ranges</td>
 </tr>
 <tr>
 <td>ip</td>
 <td><code class="docutils literal notranslate">v6.4.4 -> 7.4.3 </code></td>
 </tr>
 </table>
 </div>
 </li>
            </ul>
        <li> <span class="li-head">server_port</span> - Port number of the remote SDN connector. <span class="li-normal">type: int</span>
 <a id='label138' href="javascript:ContentClick('label139', 'label138');" onmouseover="ContentPreview('label139');" onmouseout="ContentUnpreview('label139');" title="click to collapse or expand..."> more... </a>
 <div id="label139" style="display:none">
 <table border="1">
 <tr>
 <td></td>
 <td colspan="1">Supported Version Ranges</td>
 </tr>
 <tr>
 <td>server_port</td>
 <td><code class="docutils literal notranslate">v6.0.0 -> 7.4.3 </code></td>
 </tr>
 </table>
 </div>
 </li>
        <li> <span class="li-head">service_account</span> - GCP service account email. <span class="li-normal">type: str</span>
 <a id='label140' href="javascript:ContentClick('label141', 'label140');" onmouseover="ContentPreview('label141');" onmouseout="ContentUnpreview('label141');" title="click to collapse or expand..."> more... </a>
 <div id="label141" style="display:none">
 <table border="1">
 <tr>
 <td></td>
 <td colspan="1">Supported Version Ranges</td>
 </tr>
 <tr>
 <td>service_account</td>
 <td><code class="docutils literal notranslate">v6.0.0 -> 7.4.3 </code></td>
 </tr>
 </table>
 </div>
 </li>
        <li> <span class="li-head">status</span> - Enable/disable connection to the remote SDN connector. <span class="li-normal">type: str</span> <span class="li-normal">choices: disable, enable</span>
 <a id='label142' href="javascript:ContentClick('label143', 'label142');" onmouseover="ContentPreview('label143');" onmouseout="ContentUnpreview('label143');" title="click to collapse or expand..."> more... </a>
 <div id="label143" style="display:none">
 <table border="1">
 <tr>
 <td></td>
 <td colspan="1">Supported Version Ranges</td>
 </tr>
 <tr>
 <td>status</td>
 <td><code class="docutils literal notranslate">v6.0.0 -> 7.4.3 </code></td>
 </tr>
 <tr>
 <td>[disable]</td>
 <td><code class="docutils literal notranslate">v6.0.0 -> 7.4.3</code></td>
 <tr>
 <td>[enable]</td>
 <td><code class="docutils literal notranslate">v6.0.0 -> 7.4.3</code></td>
 </table>
 </div>
 </li>
        <li> <span class="li-head">subscription_id</span> - Azure subscription ID. <span class="li-normal">type: str</span>
 <a id='label144' href="javascript:ContentClick('label145', 'label144');" onmouseover="ContentPreview('label145');" onmouseout="ContentUnpreview('label145');" title="click to collapse or expand..."> more... </a>
 <div id="label145" style="display:none">
 <table border="1">
 <tr>
 <td></td>
 <td colspan="1">Supported Version Ranges</td>
 </tr>
 <tr>
 <td>subscription_id</td>
 <td><code class="docutils literal notranslate">v6.0.0 -> 7.4.3 </code></td>
 </tr>
 </table>
 </div>
 </li>
        <li> <span class="li-head">tenant_id</span> - Tenant ID (directory ID). <span class="li-normal">type: str</span>
 <a id='label146' href="javascript:ContentClick('label147', 'label146');" onmouseover="ContentPreview('label147');" onmouseout="ContentUnpreview('label147');" title="click to collapse or expand..."> more... </a>
 <div id="label147" style="display:none">
 <table border="1">
 <tr>
 <td></td>
 <td colspan="1">Supported Version Ranges</td>
 </tr>
 <tr>
 <td>tenant_id</td>
 <td><code class="docutils literal notranslate">v6.0.0 -> 7.4.3 </code></td>
 </tr>
 </table>
 </div>
 </li>
        <li> <span class="li-head">type</span> - Type of SDN connector. <span class="li-normal">type: str</span> <span class="li-normal">choices: aci, alicloud, aws, azure, gcp, nsx, nuage, oci, openstack, kubernetes, vmware, sepm, aci-direct, ibm, nutanix, sap</span>
 <a id='label148' href="javascript:ContentClick('label149', 'label148');" onmouseover="ContentPreview('label149');" onmouseout="ContentUnpreview('label149');" title="click to collapse or expand..."> more... </a>
 <div id="label149" style="display:none">
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
 <td>[aci]</td>
 <td><code class="docutils literal notranslate">v6.0.0 -> 7.4.3</code></td>
 <tr>
 <td>[alicloud]</td>
 <td><code class="docutils literal notranslate">v6.2.0 -> 7.4.3</code></td>
 </tr>
 <tr>
 <td>[aws]</td>
 <td><code class="docutils literal notranslate">v6.0.0 -> 7.4.3</code></td>
 <tr>
 <td>[azure]</td>
 <td><code class="docutils literal notranslate">v6.0.0 -> 7.4.3</code></td>
 <tr>
 <td>[gcp]</td>
 <td><code class="docutils literal notranslate">v6.0.0 -> 7.4.3</code></td>
 <tr>
 <td>[nsx]</td>
 <td><code class="docutils literal notranslate">v6.0.0 -> 7.4.3</code></td>
 <tr>
 <td>[nuage]</td>
 <td><code class="docutils literal notranslate">v6.0.0 -> 7.4.3</code></td>
 <tr>
 <td>[oci]</td>
 <td><code class="docutils literal notranslate">v6.0.0 -> 7.4.3</code></td>
 <tr>
 <td>[openstack]</td>
 <td><code class="docutils literal notranslate">v6.0.0 -> 7.4.3</code></td>
 <tr>
 <td>[kubernetes]</td>
 <td><code class="docutils literal notranslate">v6.2.0 -> 7.4.3</code></td>
 </tr>
 <tr>
 <td>[vmware]</td>
 <td><code class="docutils literal notranslate">v6.2.0 -> 7.4.3</code></td>
 </tr>
 <tr>
 <td>[sepm]</td>
 <td><code class="docutils literal notranslate">v6.2.0 -> 7.4.3</code></td>
 </tr>
 <tr>
 <td>[aci-direct]</td>
 <td><code class="docutils literal notranslate">v6.4.0 -> 7.4.3</code></td>
 </tr>
 <tr>
 <td>[ibm]</td>
 <td><code class="docutils literal notranslate">v6.4.0 -> 7.4.3</code></td>
 </tr>
 <tr>
 <td>[nutanix]</td>
 <td><code class="docutils literal notranslate">v7.0.0 -> 7.4.3</code></td>
 </tr>
 <tr>
 <td>[sap]</td>
 <td><code class="docutils literal notranslate">v7.2.1 -> 7.4.3</code></td>
 </tr>
 </table>
 </div>
 </li>
        <li> <span class="li-head">update_interval</span> - Dynamic object update interval (30 - 3600 sec). <span class="li-normal">type: int</span>
 <a id='label150' href="javascript:ContentClick('label151', 'label150');" onmouseover="ContentPreview('label151');" onmouseout="ContentUnpreview('label151');" title="click to collapse or expand..."> more... </a>
 <div id="label151" style="display:none">
 <table border="1">
 <tr>
 <td></td>
 <td colspan="1">Supported Version Ranges</td>
 </tr>
 <tr>
 <td>update_interval</td>
 <td><code class="docutils literal notranslate">v6.0.0 -> 7.4.3 </code></td>
 </tr>
 </table>
 </div>
 </li>
        <li> <span class="li-head">use_metadata_iam</span> - Enable/disable use of IAM role from metadata to call API. <span class="li-normal">type: str</span> <span class="li-normal">choices: disable, enable</span>
 <a id='label152' href="javascript:ContentClick('label153', 'label152');" onmouseover="ContentPreview('label153');" onmouseout="ContentUnpreview('label153');" title="click to collapse or expand..."> more... </a>
 <div id="label153" style="display:none">
 <table border="1">
 <tr>
 <td></td>
 <td colspan="1">Supported Version Ranges</td>
 </tr>
 <tr>
 <td>use_metadata_iam</td>
 <td><code class="docutils literal notranslate">v6.0.0 -> 7.4.3 </code></td>
 </tr>
 <tr>
 <td>[disable]</td>
 <td><code class="docutils literal notranslate">v6.0.0 -> 7.4.3</code></td>
 <tr>
 <td>[enable]</td>
 <td><code class="docutils literal notranslate">v6.0.0 -> 7.4.3</code></td>
 </table>
 </div>
 </li>
        <li> <span class="li-head">user_id</span> - User ID. <span class="li-normal">type: str</span>
 <a id='label154' href="javascript:ContentClick('label155', 'label154');" onmouseover="ContentPreview('label155');" onmouseout="ContentUnpreview('label155');" title="click to collapse or expand..."> more... </a>
 <div id="label155" style="display:none">
 <table border="1">
 <tr>
 <td></td>
 <td colspan="1">Supported Version Ranges</td>
 </tr>
 <tr>
 <td>user_id</td>
 <td><code class="docutils literal notranslate">v6.0.0 -> 7.4.3 </code></td>
 </tr>
 </table>
 </div>
 </li>
        <li> <span class="li-head">username</span> - Username of the remote SDN connector as login credentials. <span class="li-normal">type: str</span>
 <a id='label156' href="javascript:ContentClick('label157', 'label156');" onmouseover="ContentPreview('label157');" onmouseout="ContentUnpreview('label157');" title="click to collapse or expand..."> more... </a>
 <div id="label157" style="display:none">
 <table border="1">
 <tr>
 <td></td>
 <td colspan="1">Supported Version Ranges</td>
 </tr>
 <tr>
 <td>username</td>
 <td><code class="docutils literal notranslate">v6.0.0 -> 7.4.3 </code></td>
 </tr>
 </table>
 </div>
 </li>
        <li> <span class="li-head">vcenter_password</span> - vCenter server password for NSX quarantine. <span class="li-normal">type: str</span>
 <a id='label158' href="javascript:ContentClick('label159', 'label158');" onmouseover="ContentPreview('label159');" onmouseout="ContentUnpreview('label159');" title="click to collapse or expand..."> more... </a>
 <div id="label159" style="display:none">
 <table border="1">
 <tr>
 <td></td>
 <td colspan="1">Supported Version Ranges</td>
 </tr>
 <tr>
 <td>vcenter_password</td>
 <td><code class="docutils literal notranslate">v6.4.0 -> 7.4.3 </code></td>
 </tr>
 </table>
 </div>
 </li>
        <li> <span class="li-head">vcenter_server</span> - vCenter server address for NSX quarantine. <span class="li-normal">type: str</span>
 <a id='label160' href="javascript:ContentClick('label161', 'label160');" onmouseover="ContentPreview('label161');" onmouseout="ContentUnpreview('label161');" title="click to collapse or expand..."> more... </a>
 <div id="label161" style="display:none">
 <table border="1">
 <tr>
 <td></td>
 <td colspan="1">Supported Version Ranges</td>
 </tr>
 <tr>
 <td>vcenter_server</td>
 <td><code class="docutils literal notranslate">v6.4.0 -> 7.4.3 </code></td>
 </tr>
 </table>
 </div>
 </li>
        <li> <span class="li-head">vcenter_username</span> - vCenter server username for NSX quarantine. <span class="li-normal">type: str</span>
 <a id='label162' href="javascript:ContentClick('label163', 'label162');" onmouseover="ContentPreview('label163');" onmouseout="ContentUnpreview('label163');" title="click to collapse or expand..."> more... </a>
 <div id="label163" style="display:none">
 <table border="1">
 <tr>
 <td></td>
 <td colspan="1">Supported Version Ranges</td>
 </tr>
 <tr>
 <td>vcenter_username</td>
 <td><code class="docutils literal notranslate">v6.4.0 -> 7.4.3 </code></td>
 </tr>
 </table>
 </div>
 </li>
        <li> <span class="li-head">verify_certificate</span> - Enable/disable server certificate verification. <span class="li-normal">type: str</span> <span class="li-normal">choices: disable, enable</span>
 <a id='label164' href="javascript:ContentClick('label165', 'label164');" onmouseover="ContentPreview('label165');" onmouseout="ContentUnpreview('label165');" title="click to collapse or expand..."> more... </a>
 <div id="label165" style="display:none">
 <table border="1">
 <tr>
 <td></td>
 <td colspan="1">Supported Version Ranges</td>
 </tr>
 <tr>
 <td>verify_certificate</td>
 <td><code class="docutils literal notranslate">v7.0.1 -> 7.4.3 </code></td>
 </tr>
 <tr>
 <td>[disable]</td>
 <td><code class="docutils literal notranslate">v7.0.1 -> 7.4.3</code></td>
 <tr>
 <td>[enable]</td>
 <td><code class="docutils literal notranslate">v7.0.1 -> 7.4.3</code></td>
 </table>
 </div>
 </li>
        <li> <span class="li-head">vpc_id</span> - AWS VPC ID. <span class="li-normal">type: str</span>
 <a id='label166' href="javascript:ContentClick('label167', 'label166');" onmouseover="ContentPreview('label167');" onmouseout="ContentUnpreview('label167');" title="click to collapse or expand..."> more... </a>
 <div id="label167" style="display:none">
 <table border="1">
 <tr>
 <td></td>
 <td colspan="1">Supported Version Ranges</td>
 </tr>
 <tr>
 <td>vpc_id</td>
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
    
    - name: Configure connection to SDN Connector.
      fortinet.fortios.fortios_system_sdn_connector:
          vdom: "{{ vdom }}"
          state: "present"
          access_token: "<your_own_value>"
          system_sdn_connector:
              access_key: "<your_own_value>"
              alt_resource_ip: "disable"
              api_key: "<your_own_value>"
              azure_region: "global"
              client_id: "<your_own_value>"
              client_secret: "<your_own_value>"
              compartment_id: "<your_own_value>"
              compartment_list:
                  -
                      compartment_id: "<your_own_value>"
              compute_generation: "2"
              domain: "<your_own_value>"
              external_account_list:
                  -
                      external_id: "<your_own_value>"
                      region_list:
                          -
                              region: "<your_own_value>"
                      role_arn: "<your_own_value>"
              external_ip:
                  -
                      name: "default_name_20"
              forwarding_rule:
                  -
                      rule_name: "<your_own_value>"
                      target: "<your_own_value>"
              gcp_project: "<your_own_value>"
              gcp_project_list:
                  -
                      gcp_zone_list:
                          -
                              name: "default_name_27"
                      id: "28"
              group_name: "<your_own_value>"
              ha_status: "disable"
              ibm_region: "dallas"
              ibm_region_gen1: "us-south"
              ibm_region_gen2: "us-south"
              key_passwd: "<your_own_value>"
              login_endpoint: "<your_own_value>"
              name: "default_name_36"
              nic:
                  -
                      ip:
                          -
                              name: "default_name_39"
                              public_ip: "<your_own_value>"
                              resource_group: "<your_own_value>"
                      name: "default_name_42"
              oci_cert: "<your_own_value> (source certificate.local.name)"
              oci_fingerprint: "<your_own_value>"
              oci_region: "phoenix"
              oci_region_list:
                  -
                      region: "<your_own_value>"
              oci_region_type: "commercial"
              password: "<your_own_value>"
              private_key: "<your_own_value>"
              proxy: "<your_own_value> (source system.sdn-proxy.name)"
              region: "<your_own_value>"
              resource_group: "<your_own_value>"
              resource_url: "<your_own_value>"
              route:
                  -
                      name: "default_name_56"
              route_table:
                  -
                      name: "default_name_58"
                      resource_group: "<your_own_value>"
                      route:
                          -
                              name: "default_name_61"
                              next_hop: "<your_own_value>"
                      subscription_id: "<your_own_value>"
              secret_key: "<your_own_value>"
              secret_token: "<your_own_value>"
              server: "192.168.100.40"
              server_ca_cert: "<your_own_value> (source certificate.remote.name certificate.ca.name)"
              server_cert: "<your_own_value> (source certificate.remote.name)"
              server_list:
                  -
                      ip: "<your_own_value>"
              server_port: "0"
              service_account: "<your_own_value>"
              status: "disable"
              subscription_id: "<your_own_value>"
              tenant_id: "<your_own_value>"
              type: "aci"
              update_interval: "60"
              use_metadata_iam: "disable"
              user_id: "<your_own_value>"
              username: "<your_own_value>"
              vcenter_password: "<your_own_value>"
              vcenter_server: "<your_own_value>"
              vcenter_username: "<your_own_value>"
              verify_certificate: "disable"
              vpc_id: "<your_own_value>"


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
