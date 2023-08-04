:source: fortios_router_ripng.py

:orphan:

.. fortios_router_ripng:

fortios_router_ripng -- Configure RIPng in Fortinet's FortiOS and FortiGate.
++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++

.. versionadded:: 2.0.0

.. contents::
   :local:
   :depth: 1


Synopsis
--------
- This module is able to configure a FortiGate or FortiOS (FOS) device by allowing the user to set and modify router feature and ripng category. Examples include all parameters and values need to be adjusted to datasources before usage. Tested with FOS v6.0.0



Requirements
------------
The below requirements are needed on the host that executes this module.

- ansible>=2.9


Tips
----
Using member operation to add an element to an existing object.

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
 <td><code class="docutils literal notranslate">v7.0.6 </code></td>
 <td><code class="docutils literal notranslate">v7.0.7 </code></td>
 <td><code class="docutils literal notranslate">v7.0.8 </code></td>
 <td><code class="docutils literal notranslate">v7.0.12 </code></td>
 <td><code class="docutils literal notranslate">v7.2.0 </code></td>
 <td><code class="docutils literal notranslate">v7.2.1 </code></td>
 <td><code class="docutils literal notranslate">v7.2.2 </code></td>
 <td><code class="docutils literal notranslate">v7.2.4 </code></td>
 <td><code class="docutils literal notranslate">v7.4.0 </code></td>
 </tr>
 <tr>
 <td>fortios_router_ripng</td>
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
    <li> <span class="li-head">router_ripng</span> - Configure RIPng. <span class="li-normal">type: dict</span>
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
 <td><code class="docutils literal notranslate">v7.0.6 </code></td>
 <td><code class="docutils literal notranslate">v7.0.7 </code></td>
 <td><code class="docutils literal notranslate">v7.0.8 </code></td>
 <td><code class="docutils literal notranslate">v7.0.12 </code></td>
 <td><code class="docutils literal notranslate">v7.2.0 </code></td>
 <td><code class="docutils literal notranslate">v7.2.1 </code></td>
 <td><code class="docutils literal notranslate">v7.2.2 </code></td>
 <td><code class="docutils literal notranslate">v7.2.4 </code></td>
 <td><code class="docutils literal notranslate">v7.4.0 </code></td>
 </tr>
 <tr>
 <td>router_ripng</td>
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
        <li> <span class="li-head">aggregate_address</span> - Aggregate address. <span class="li-normal">type: list</span> <span style="font-family:'Courier New'" class="li-required">member_path: aggregate_address:id</span>
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
 <td><code class="docutils literal notranslate">v7.0.6 </code></td>
 <td><code class="docutils literal notranslate">v7.0.7 </code></td>
 <td><code class="docutils literal notranslate">v7.0.8 </code></td>
 <td><code class="docutils literal notranslate">v7.0.12 </code></td>
 <td><code class="docutils literal notranslate">v7.2.0 </code></td>
 <td><code class="docutils literal notranslate">v7.2.1 </code></td>
 <td><code class="docutils literal notranslate">v7.2.2 </code></td>
 <td><code class="docutils literal notranslate">v7.2.4 </code></td>
 <td><code class="docutils literal notranslate">v7.4.0 </code></td>
 </tr>
 <tr>
 <td>aggregate_address</td>
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
            <li> <span class="li-head">id</span> - Aggregate address entry ID. <span class="li-normal">type: int</span> <span class="li-required">required: true</span>
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
 <td><code class="docutils literal notranslate">v7.0.6 </code></td>
 <td><code class="docutils literal notranslate">v7.0.7 </code></td>
 <td><code class="docutils literal notranslate">v7.0.8 </code></td>
 <td><code class="docutils literal notranslate">v7.0.12 </code></td>
 <td><code class="docutils literal notranslate">v7.2.0 </code></td>
 <td><code class="docutils literal notranslate">v7.2.1 </code></td>
 <td><code class="docutils literal notranslate">v7.2.2 </code></td>
 <td><code class="docutils literal notranslate">v7.2.4 </code></td>
 <td><code class="docutils literal notranslate">v7.4.0 </code></td>
 </tr>
 <tr>
 <td>id</td>
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
            <li> <span class="li-head">prefix6</span> - Aggregate address prefix. <span class="li-normal">type: str</span>
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
 <td><code class="docutils literal notranslate">v7.0.6 </code></td>
 <td><code class="docutils literal notranslate">v7.0.7 </code></td>
 <td><code class="docutils literal notranslate">v7.0.8 </code></td>
 <td><code class="docutils literal notranslate">v7.0.12 </code></td>
 <td><code class="docutils literal notranslate">v7.2.0 </code></td>
 <td><code class="docutils literal notranslate">v7.2.1 </code></td>
 <td><code class="docutils literal notranslate">v7.2.2 </code></td>
 <td><code class="docutils literal notranslate">v7.2.4 </code></td>
 <td><code class="docutils literal notranslate">v7.4.0 </code></td>
 </tr>
 <tr>
 <td>prefix6</td>
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
        <li> <span class="li-head">default_information_originate</span> - Enable/disable generation of default route. <span class="li-normal">type: str</span> <span class="li-normal">choices: enable, disable</span>
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
 <td><code class="docutils literal notranslate">v7.0.6 </code></td>
 <td><code class="docutils literal notranslate">v7.0.7 </code></td>
 <td><code class="docutils literal notranslate">v7.0.8 </code></td>
 <td><code class="docutils literal notranslate">v7.0.12 </code></td>
 <td><code class="docutils literal notranslate">v7.2.0 </code></td>
 <td><code class="docutils literal notranslate">v7.2.1 </code></td>
 <td><code class="docutils literal notranslate">v7.2.2 </code></td>
 <td><code class="docutils literal notranslate">v7.2.4 </code></td>
 <td><code class="docutils literal notranslate">v7.4.0 </code></td>
 </tr>
 <tr>
 <td>default_information_originate</td>
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
        <li> <span class="li-head">default_metric</span> - Default metric. <span class="li-normal">type: int</span>
 <a id='label10' href="javascript:ContentClick('label11', 'label10');" onmouseover="ContentPreview('label11');" onmouseout="ContentUnpreview('label11');" title="click to collapse or expand..."> more... </a>
 <div id="label11" style="display:none">
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
 <td><code class="docutils literal notranslate">v7.0.6 </code></td>
 <td><code class="docutils literal notranslate">v7.0.7 </code></td>
 <td><code class="docutils literal notranslate">v7.0.8 </code></td>
 <td><code class="docutils literal notranslate">v7.0.12 </code></td>
 <td><code class="docutils literal notranslate">v7.2.0 </code></td>
 <td><code class="docutils literal notranslate">v7.2.1 </code></td>
 <td><code class="docutils literal notranslate">v7.2.2 </code></td>
 <td><code class="docutils literal notranslate">v7.2.4 </code></td>
 <td><code class="docutils literal notranslate">v7.4.0 </code></td>
 </tr>
 <tr>
 <td>default_metric</td>
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
        <li> <span class="li-head">distance</span> - Distance. <span class="li-normal">type: list</span> <span style="font-family:'Courier New'" class="li-required">member_path: distance:id</span>
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
 <td><code class="docutils literal notranslate">v7.0.6 </code></td>
 <td><code class="docutils literal notranslate">v7.0.7 </code></td>
 <td><code class="docutils literal notranslate">v7.0.8 </code></td>
 <td><code class="docutils literal notranslate">v7.0.12 </code></td>
 <td><code class="docutils literal notranslate">v7.2.0 </code></td>
 <td><code class="docutils literal notranslate">v7.2.1 </code></td>
 <td><code class="docutils literal notranslate">v7.2.2 </code></td>
 <td><code class="docutils literal notranslate">v7.2.4 </code></td>
 <td><code class="docutils literal notranslate">v7.4.0 </code></td>
 </tr>
 <tr>
 <td>distance</td>
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
            <li> <span class="li-head">access_list6</span> - Access list for route destination. Source router.access-list6.name. <span class="li-normal">type: str</span>
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
 <td><code class="docutils literal notranslate">v7.0.6 </code></td>
 <td><code class="docutils literal notranslate">v7.0.7 </code></td>
 <td><code class="docutils literal notranslate">v7.0.8 </code></td>
 <td><code class="docutils literal notranslate">v7.0.12 </code></td>
 <td><code class="docutils literal notranslate">v7.2.0 </code></td>
 <td><code class="docutils literal notranslate">v7.2.1 </code></td>
 <td><code class="docutils literal notranslate">v7.2.2 </code></td>
 <td><code class="docutils literal notranslate">v7.2.4 </code></td>
 <td><code class="docutils literal notranslate">v7.4.0 </code></td>
 </tr>
 <tr>
 <td>access_list6</td>
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
            <li> <span class="li-head">distance</span> - Distance (1 - 255). <span class="li-normal">type: int</span>
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
 <td><code class="docutils literal notranslate">v7.0.6 </code></td>
 <td><code class="docutils literal notranslate">v7.0.7 </code></td>
 <td><code class="docutils literal notranslate">v7.0.8 </code></td>
 <td><code class="docutils literal notranslate">v7.0.12 </code></td>
 <td><code class="docutils literal notranslate">v7.2.0 </code></td>
 <td><code class="docutils literal notranslate">v7.2.1 </code></td>
 <td><code class="docutils literal notranslate">v7.2.2 </code></td>
 <td><code class="docutils literal notranslate">v7.2.4 </code></td>
 <td><code class="docutils literal notranslate">v7.4.0 </code></td>
 </tr>
 <tr>
 <td>distance</td>
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
            <li> <span class="li-head">id</span> - Distance ID. <span class="li-normal">type: int</span> <span class="li-required">required: true</span>
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
 <td><code class="docutils literal notranslate">v7.0.6 </code></td>
 <td><code class="docutils literal notranslate">v7.0.7 </code></td>
 <td><code class="docutils literal notranslate">v7.0.8 </code></td>
 <td><code class="docutils literal notranslate">v7.0.12 </code></td>
 <td><code class="docutils literal notranslate">v7.2.0 </code></td>
 <td><code class="docutils literal notranslate">v7.2.1 </code></td>
 <td><code class="docutils literal notranslate">v7.2.2 </code></td>
 <td><code class="docutils literal notranslate">v7.2.4 </code></td>
 <td><code class="docutils literal notranslate">v7.4.0 </code></td>
 </tr>
 <tr>
 <td>id</td>
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
            <li> <span class="li-head">prefix6</span> - Distance prefix6. <span class="li-normal">type: str</span>
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
 <td><code class="docutils literal notranslate">v7.0.6 </code></td>
 <td><code class="docutils literal notranslate">v7.0.7 </code></td>
 <td><code class="docutils literal notranslate">v7.0.8 </code></td>
 <td><code class="docutils literal notranslate">v7.0.12 </code></td>
 <td><code class="docutils literal notranslate">v7.2.0 </code></td>
 <td><code class="docutils literal notranslate">v7.2.1 </code></td>
 <td><code class="docutils literal notranslate">v7.2.2 </code></td>
 <td><code class="docutils literal notranslate">v7.2.4 </code></td>
 <td><code class="docutils literal notranslate">v7.4.0 </code></td>
 </tr>
 <tr>
 <td>prefix6</td>
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
        <li> <span class="li-head">distribute_list</span> - Distribute list. <span class="li-normal">type: list</span> <span style="font-family:'Courier New'" class="li-required">member_path: distribute_list:id</span>
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
 <td><code class="docutils literal notranslate">v7.0.6 </code></td>
 <td><code class="docutils literal notranslate">v7.0.7 </code></td>
 <td><code class="docutils literal notranslate">v7.0.8 </code></td>
 <td><code class="docutils literal notranslate">v7.0.12 </code></td>
 <td><code class="docutils literal notranslate">v7.2.0 </code></td>
 <td><code class="docutils literal notranslate">v7.2.1 </code></td>
 <td><code class="docutils literal notranslate">v7.2.2 </code></td>
 <td><code class="docutils literal notranslate">v7.2.4 </code></td>
 <td><code class="docutils literal notranslate">v7.4.0 </code></td>
 </tr>
 <tr>
 <td>distribute_list</td>
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
            <li> <span class="li-head">direction</span> - Distribute list direction. <span class="li-normal">type: str</span> <span class="li-normal">choices: in, out</span>
 <a id='label24' href="javascript:ContentClick('label25', 'label24');" onmouseover="ContentPreview('label25');" onmouseout="ContentUnpreview('label25');" title="click to collapse or expand..."> more... </a>
 <div id="label25" style="display:none">
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
 <td><code class="docutils literal notranslate">v7.0.6 </code></td>
 <td><code class="docutils literal notranslate">v7.0.7 </code></td>
 <td><code class="docutils literal notranslate">v7.0.8 </code></td>
 <td><code class="docutils literal notranslate">v7.0.12 </code></td>
 <td><code class="docutils literal notranslate">v7.2.0 </code></td>
 <td><code class="docutils literal notranslate">v7.2.1 </code></td>
 <td><code class="docutils literal notranslate">v7.2.2 </code></td>
 <td><code class="docutils literal notranslate">v7.2.4 </code></td>
 <td><code class="docutils literal notranslate">v7.4.0 </code></td>
 </tr>
 <tr>
 <td>direction</td>
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
 <td>[in]</td>
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
 <td>[out]</td>
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
            <li> <span class="li-head">id</span> - Distribute list ID. <span class="li-normal">type: int</span> <span class="li-required">required: true</span>
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
 <td><code class="docutils literal notranslate">v7.0.6 </code></td>
 <td><code class="docutils literal notranslate">v7.0.7 </code></td>
 <td><code class="docutils literal notranslate">v7.0.8 </code></td>
 <td><code class="docutils literal notranslate">v7.0.12 </code></td>
 <td><code class="docutils literal notranslate">v7.2.0 </code></td>
 <td><code class="docutils literal notranslate">v7.2.1 </code></td>
 <td><code class="docutils literal notranslate">v7.2.2 </code></td>
 <td><code class="docutils literal notranslate">v7.2.4 </code></td>
 <td><code class="docutils literal notranslate">v7.4.0 </code></td>
 </tr>
 <tr>
 <td>id</td>
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
            <li> <span class="li-head">interface</span> - Distribute list interface name. Source system.interface.name. <span class="li-normal">type: str</span>
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
 <td><code class="docutils literal notranslate">v7.0.6 </code></td>
 <td><code class="docutils literal notranslate">v7.0.7 </code></td>
 <td><code class="docutils literal notranslate">v7.0.8 </code></td>
 <td><code class="docutils literal notranslate">v7.0.12 </code></td>
 <td><code class="docutils literal notranslate">v7.2.0 </code></td>
 <td><code class="docutils literal notranslate">v7.2.1 </code></td>
 <td><code class="docutils literal notranslate">v7.2.2 </code></td>
 <td><code class="docutils literal notranslate">v7.2.4 </code></td>
 <td><code class="docutils literal notranslate">v7.4.0 </code></td>
 </tr>
 <tr>
 <td>interface</td>
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
            <li> <span class="li-head">listname</span> - Distribute access/prefix list name. Source router.access-list6.name router.prefix-list6.name. <span class="li-normal">type: str</span>
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
 <td><code class="docutils literal notranslate">v7.0.6 </code></td>
 <td><code class="docutils literal notranslate">v7.0.7 </code></td>
 <td><code class="docutils literal notranslate">v7.0.8 </code></td>
 <td><code class="docutils literal notranslate">v7.0.12 </code></td>
 <td><code class="docutils literal notranslate">v7.2.0 </code></td>
 <td><code class="docutils literal notranslate">v7.2.1 </code></td>
 <td><code class="docutils literal notranslate">v7.2.2 </code></td>
 <td><code class="docutils literal notranslate">v7.2.4 </code></td>
 <td><code class="docutils literal notranslate">v7.4.0 </code></td>
 </tr>
 <tr>
 <td>listname</td>
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
            <li> <span class="li-head">status</span> - Status. <span class="li-normal">type: str</span> <span class="li-normal">choices: enable, disable</span>
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
 <td><code class="docutils literal notranslate">v7.0.6 </code></td>
 <td><code class="docutils literal notranslate">v7.0.7 </code></td>
 <td><code class="docutils literal notranslate">v7.0.8 </code></td>
 <td><code class="docutils literal notranslate">v7.0.12 </code></td>
 <td><code class="docutils literal notranslate">v7.2.0 </code></td>
 <td><code class="docutils literal notranslate">v7.2.1 </code></td>
 <td><code class="docutils literal notranslate">v7.2.2 </code></td>
 <td><code class="docutils literal notranslate">v7.2.4 </code></td>
 <td><code class="docutils literal notranslate">v7.4.0 </code></td>
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
        <li> <span class="li-head">garbage_timer</span> - Garbage timer. <span class="li-normal">type: int</span>
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
 <td><code class="docutils literal notranslate">v7.0.6 </code></td>
 <td><code class="docutils literal notranslate">v7.0.7 </code></td>
 <td><code class="docutils literal notranslate">v7.0.8 </code></td>
 <td><code class="docutils literal notranslate">v7.0.12 </code></td>
 <td><code class="docutils literal notranslate">v7.2.0 </code></td>
 <td><code class="docutils literal notranslate">v7.2.1 </code></td>
 <td><code class="docutils literal notranslate">v7.2.2 </code></td>
 <td><code class="docutils literal notranslate">v7.2.4 </code></td>
 <td><code class="docutils literal notranslate">v7.4.0 </code></td>
 </tr>
 <tr>
 <td>garbage_timer</td>
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
        <li> <span class="li-head">interface</span> - RIPng interface configuration. <span class="li-normal">type: list</span> <span style="font-family:'Courier New'" class="li-required">member_path: interface:name</span>
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
 <td><code class="docutils literal notranslate">v7.0.6 </code></td>
 <td><code class="docutils literal notranslate">v7.0.7 </code></td>
 <td><code class="docutils literal notranslate">v7.0.8 </code></td>
 <td><code class="docutils literal notranslate">v7.0.12 </code></td>
 <td><code class="docutils literal notranslate">v7.2.0 </code></td>
 <td><code class="docutils literal notranslate">v7.2.1 </code></td>
 <td><code class="docutils literal notranslate">v7.2.2 </code></td>
 <td><code class="docutils literal notranslate">v7.2.4 </code></td>
 <td><code class="docutils literal notranslate">v7.4.0 </code></td>
 </tr>
 <tr>
 <td>interface</td>
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
            <li> <span class="li-head">flags</span> - Flags. <span class="li-normal">type: int</span>
 <a id='label38' href="javascript:ContentClick('label39', 'label38');" onmouseover="ContentPreview('label39');" onmouseout="ContentUnpreview('label39');" title="click to collapse or expand..."> more... </a>
 <div id="label39" style="display:none">
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
 <td><code class="docutils literal notranslate">v7.2.0 </code></td>
 </tr>
 <tr>
 <td>flags</td>
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
 <td>yes</td>
 </tr>
 </table>
 </div>
 </li>
            <li> <span class="li-head">name</span> - Interface name. Source system.interface.name. <span class="li-normal">type: str</span> <span class="li-required">required: true</span>
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
 <td><code class="docutils literal notranslate">v7.0.6 </code></td>
 <td><code class="docutils literal notranslate">v7.0.7 </code></td>
 <td><code class="docutils literal notranslate">v7.0.8 </code></td>
 <td><code class="docutils literal notranslate">v7.0.12 </code></td>
 <td><code class="docutils literal notranslate">v7.2.0 </code></td>
 <td><code class="docutils literal notranslate">v7.2.1 </code></td>
 <td><code class="docutils literal notranslate">v7.2.2 </code></td>
 <td><code class="docutils literal notranslate">v7.2.4 </code></td>
 <td><code class="docutils literal notranslate">v7.4.0 </code></td>
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
            <li> <span class="li-head">split_horizon</span> - Enable/disable split horizon. <span class="li-normal">type: str</span> <span class="li-normal">choices: poisoned, regular</span>
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
 <td><code class="docutils literal notranslate">v7.0.6 </code></td>
 <td><code class="docutils literal notranslate">v7.0.7 </code></td>
 <td><code class="docutils literal notranslate">v7.0.8 </code></td>
 <td><code class="docutils literal notranslate">v7.0.12 </code></td>
 <td><code class="docutils literal notranslate">v7.2.0 </code></td>
 <td><code class="docutils literal notranslate">v7.2.1 </code></td>
 <td><code class="docutils literal notranslate">v7.2.2 </code></td>
 <td><code class="docutils literal notranslate">v7.2.4 </code></td>
 <td><code class="docutils literal notranslate">v7.4.0 </code></td>
 </tr>
 <tr>
 <td>split_horizon</td>
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
 <td>[poisoned]</td>
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
 <td>[regular]</td>
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
            <li> <span class="li-head">split_horizon_status</span> - Enable/disable split horizon. <span class="li-normal">type: str</span> <span class="li-normal">choices: enable, disable</span>
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
 <td><code class="docutils literal notranslate">v7.0.6 </code></td>
 <td><code class="docutils literal notranslate">v7.0.7 </code></td>
 <td><code class="docutils literal notranslate">v7.0.8 </code></td>
 <td><code class="docutils literal notranslate">v7.0.12 </code></td>
 <td><code class="docutils literal notranslate">v7.2.0 </code></td>
 <td><code class="docutils literal notranslate">v7.2.1 </code></td>
 <td><code class="docutils literal notranslate">v7.2.2 </code></td>
 <td><code class="docutils literal notranslate">v7.2.4 </code></td>
 <td><code class="docutils literal notranslate">v7.4.0 </code></td>
 </tr>
 <tr>
 <td>split_horizon_status</td>
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
        <li> <span class="li-head">max_out_metric</span> - Maximum metric allowed to output(0 means "not set"). <span class="li-normal">type: int</span>
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
 <td><code class="docutils literal notranslate">v7.0.6 </code></td>
 <td><code class="docutils literal notranslate">v7.0.7 </code></td>
 <td><code class="docutils literal notranslate">v7.0.8 </code></td>
 <td><code class="docutils literal notranslate">v7.0.12 </code></td>
 <td><code class="docutils literal notranslate">v7.2.0 </code></td>
 <td><code class="docutils literal notranslate">v7.2.1 </code></td>
 <td><code class="docutils literal notranslate">v7.2.2 </code></td>
 <td><code class="docutils literal notranslate">v7.2.4 </code></td>
 <td><code class="docutils literal notranslate">v7.4.0 </code></td>
 </tr>
 <tr>
 <td>max_out_metric</td>
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
        <li> <span class="li-head">neighbor</span> - Neighbor. <span class="li-normal">type: list</span> <span style="font-family:'Courier New'" class="li-required">member_path: neighbor:id</span>
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
 <td><code class="docutils literal notranslate">v7.0.6 </code></td>
 <td><code class="docutils literal notranslate">v7.0.7 </code></td>
 <td><code class="docutils literal notranslate">v7.0.8 </code></td>
 <td><code class="docutils literal notranslate">v7.0.12 </code></td>
 <td><code class="docutils literal notranslate">v7.2.0 </code></td>
 <td><code class="docutils literal notranslate">v7.2.1 </code></td>
 <td><code class="docutils literal notranslate">v7.2.2 </code></td>
 <td><code class="docutils literal notranslate">v7.2.4 </code></td>
 <td><code class="docutils literal notranslate">v7.4.0 </code></td>
 </tr>
 <tr>
 <td>neighbor</td>
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
            <li> <span class="li-head">id</span> - Neighbor entry ID. <span class="li-normal">type: int</span> <span class="li-required">required: true</span>
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
 <td><code class="docutils literal notranslate">v7.0.6 </code></td>
 <td><code class="docutils literal notranslate">v7.0.7 </code></td>
 <td><code class="docutils literal notranslate">v7.0.8 </code></td>
 <td><code class="docutils literal notranslate">v7.0.12 </code></td>
 <td><code class="docutils literal notranslate">v7.2.0 </code></td>
 <td><code class="docutils literal notranslate">v7.2.1 </code></td>
 <td><code class="docutils literal notranslate">v7.2.2 </code></td>
 <td><code class="docutils literal notranslate">v7.2.4 </code></td>
 <td><code class="docutils literal notranslate">v7.4.0 </code></td>
 </tr>
 <tr>
 <td>id</td>
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
            <li> <span class="li-head">interface</span> - Interface name. Source system.interface.name. <span class="li-normal">type: str</span>
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
 <td><code class="docutils literal notranslate">v7.0.6 </code></td>
 <td><code class="docutils literal notranslate">v7.0.7 </code></td>
 <td><code class="docutils literal notranslate">v7.0.8 </code></td>
 <td><code class="docutils literal notranslate">v7.0.12 </code></td>
 <td><code class="docutils literal notranslate">v7.2.0 </code></td>
 <td><code class="docutils literal notranslate">v7.2.1 </code></td>
 <td><code class="docutils literal notranslate">v7.2.2 </code></td>
 <td><code class="docutils literal notranslate">v7.2.4 </code></td>
 <td><code class="docutils literal notranslate">v7.4.0 </code></td>
 </tr>
 <tr>
 <td>interface</td>
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
            <li> <span class="li-head">ip6</span> - IPv6 link-local address. <span class="li-normal">type: str</span>
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
 <td><code class="docutils literal notranslate">v7.0.6 </code></td>
 <td><code class="docutils literal notranslate">v7.0.7 </code></td>
 <td><code class="docutils literal notranslate">v7.0.8 </code></td>
 <td><code class="docutils literal notranslate">v7.0.12 </code></td>
 <td><code class="docutils literal notranslate">v7.2.0 </code></td>
 <td><code class="docutils literal notranslate">v7.2.1 </code></td>
 <td><code class="docutils literal notranslate">v7.2.2 </code></td>
 <td><code class="docutils literal notranslate">v7.2.4 </code></td>
 <td><code class="docutils literal notranslate">v7.4.0 </code></td>
 </tr>
 <tr>
 <td>ip6</td>
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
        <li> <span class="li-head">network</span> - Network. <span class="li-normal">type: list</span> <span style="font-family:'Courier New'" class="li-required">member_path: network:id</span>
 <a id='label56' href="javascript:ContentClick('label57', 'label56');" onmouseover="ContentPreview('label57');" onmouseout="ContentUnpreview('label57');" title="click to collapse or expand..."> more... </a>
 <div id="label57" style="display:none">
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
 <td><code class="docutils literal notranslate">v7.0.6 </code></td>
 <td><code class="docutils literal notranslate">v7.0.7 </code></td>
 <td><code class="docutils literal notranslate">v7.0.8 </code></td>
 <td><code class="docutils literal notranslate">v7.0.12 </code></td>
 <td><code class="docutils literal notranslate">v7.2.0 </code></td>
 <td><code class="docutils literal notranslate">v7.2.1 </code></td>
 <td><code class="docutils literal notranslate">v7.2.2 </code></td>
 <td><code class="docutils literal notranslate">v7.2.4 </code></td>
 <td><code class="docutils literal notranslate">v7.4.0 </code></td>
 </tr>
 <tr>
 <td>network</td>
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
            <li> <span class="li-head">id</span> - Network entry ID. <span class="li-normal">type: int</span> <span class="li-required">required: true</span>
 <a id='label58' href="javascript:ContentClick('label59', 'label58');" onmouseover="ContentPreview('label59');" onmouseout="ContentUnpreview('label59');" title="click to collapse or expand..."> more... </a>
 <div id="label59" style="display:none">
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
 <td><code class="docutils literal notranslate">v7.0.6 </code></td>
 <td><code class="docutils literal notranslate">v7.0.7 </code></td>
 <td><code class="docutils literal notranslate">v7.0.8 </code></td>
 <td><code class="docutils literal notranslate">v7.0.12 </code></td>
 <td><code class="docutils literal notranslate">v7.2.0 </code></td>
 <td><code class="docutils literal notranslate">v7.2.1 </code></td>
 <td><code class="docutils literal notranslate">v7.2.2 </code></td>
 <td><code class="docutils literal notranslate">v7.2.4 </code></td>
 <td><code class="docutils literal notranslate">v7.4.0 </code></td>
 </tr>
 <tr>
 <td>id</td>
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
            <li> <span class="li-head">prefix</span> - Network IPv6 link-local prefix. <span class="li-normal">type: str</span>
 <a id='label60' href="javascript:ContentClick('label61', 'label60');" onmouseover="ContentPreview('label61');" onmouseout="ContentUnpreview('label61');" title="click to collapse or expand..."> more... </a>
 <div id="label61" style="display:none">
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
 <td><code class="docutils literal notranslate">v7.0.6 </code></td>
 <td><code class="docutils literal notranslate">v7.0.7 </code></td>
 <td><code class="docutils literal notranslate">v7.0.8 </code></td>
 <td><code class="docutils literal notranslate">v7.0.12 </code></td>
 <td><code class="docutils literal notranslate">v7.2.0 </code></td>
 <td><code class="docutils literal notranslate">v7.2.1 </code></td>
 <td><code class="docutils literal notranslate">v7.2.2 </code></td>
 <td><code class="docutils literal notranslate">v7.2.4 </code></td>
 <td><code class="docutils literal notranslate">v7.4.0 </code></td>
 </tr>
 <tr>
 <td>prefix</td>
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
        <li> <span class="li-head">offset_list</span> - Offset list. <span class="li-normal">type: list</span> <span style="font-family:'Courier New'" class="li-required">member_path: offset_list:id</span>
 <a id='label62' href="javascript:ContentClick('label63', 'label62');" onmouseover="ContentPreview('label63');" onmouseout="ContentUnpreview('label63');" title="click to collapse or expand..."> more... </a>
 <div id="label63" style="display:none">
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
 <td><code class="docutils literal notranslate">v7.0.6 </code></td>
 <td><code class="docutils literal notranslate">v7.0.7 </code></td>
 <td><code class="docutils literal notranslate">v7.0.8 </code></td>
 <td><code class="docutils literal notranslate">v7.0.12 </code></td>
 <td><code class="docutils literal notranslate">v7.2.0 </code></td>
 <td><code class="docutils literal notranslate">v7.2.1 </code></td>
 <td><code class="docutils literal notranslate">v7.2.2 </code></td>
 <td><code class="docutils literal notranslate">v7.2.4 </code></td>
 <td><code class="docutils literal notranslate">v7.4.0 </code></td>
 </tr>
 <tr>
 <td>offset_list</td>
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
            <li> <span class="li-head">access_list6</span> - IPv6 access list name. Source router.access-list6.name. <span class="li-normal">type: str</span>
 <a id='label64' href="javascript:ContentClick('label65', 'label64');" onmouseover="ContentPreview('label65');" onmouseout="ContentUnpreview('label65');" title="click to collapse or expand..."> more... </a>
 <div id="label65" style="display:none">
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
 <td><code class="docutils literal notranslate">v7.0.6 </code></td>
 <td><code class="docutils literal notranslate">v7.0.7 </code></td>
 <td><code class="docutils literal notranslate">v7.0.8 </code></td>
 <td><code class="docutils literal notranslate">v7.0.12 </code></td>
 <td><code class="docutils literal notranslate">v7.2.0 </code></td>
 <td><code class="docutils literal notranslate">v7.2.1 </code></td>
 <td><code class="docutils literal notranslate">v7.2.2 </code></td>
 <td><code class="docutils literal notranslate">v7.2.4 </code></td>
 <td><code class="docutils literal notranslate">v7.4.0 </code></td>
 </tr>
 <tr>
 <td>access_list6</td>
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
            <li> <span class="li-head">direction</span> - Offset list direction. <span class="li-normal">type: str</span> <span class="li-normal">choices: in, out</span>
 <a id='label66' href="javascript:ContentClick('label67', 'label66');" onmouseover="ContentPreview('label67');" onmouseout="ContentUnpreview('label67');" title="click to collapse or expand..."> more... </a>
 <div id="label67" style="display:none">
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
 <td><code class="docutils literal notranslate">v7.0.6 </code></td>
 <td><code class="docutils literal notranslate">v7.0.7 </code></td>
 <td><code class="docutils literal notranslate">v7.0.8 </code></td>
 <td><code class="docutils literal notranslate">v7.0.12 </code></td>
 <td><code class="docutils literal notranslate">v7.2.0 </code></td>
 <td><code class="docutils literal notranslate">v7.2.1 </code></td>
 <td><code class="docutils literal notranslate">v7.2.2 </code></td>
 <td><code class="docutils literal notranslate">v7.2.4 </code></td>
 <td><code class="docutils literal notranslate">v7.4.0 </code></td>
 </tr>
 <tr>
 <td>direction</td>
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
 <td>[in]</td>
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
 <td>[out]</td>
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
            <li> <span class="li-head">id</span> - Offset-list ID. <span class="li-normal">type: int</span> <span class="li-required">required: true</span>
 <a id='label68' href="javascript:ContentClick('label69', 'label68');" onmouseover="ContentPreview('label69');" onmouseout="ContentUnpreview('label69');" title="click to collapse or expand..."> more... </a>
 <div id="label69" style="display:none">
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
 <td><code class="docutils literal notranslate">v7.0.6 </code></td>
 <td><code class="docutils literal notranslate">v7.0.7 </code></td>
 <td><code class="docutils literal notranslate">v7.0.8 </code></td>
 <td><code class="docutils literal notranslate">v7.0.12 </code></td>
 <td><code class="docutils literal notranslate">v7.2.0 </code></td>
 <td><code class="docutils literal notranslate">v7.2.1 </code></td>
 <td><code class="docutils literal notranslate">v7.2.2 </code></td>
 <td><code class="docutils literal notranslate">v7.2.4 </code></td>
 <td><code class="docutils literal notranslate">v7.4.0 </code></td>
 </tr>
 <tr>
 <td>id</td>
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
            <li> <span class="li-head">interface</span> - Interface name. Source system.interface.name. <span class="li-normal">type: str</span>
 <a id='label70' href="javascript:ContentClick('label71', 'label70');" onmouseover="ContentPreview('label71');" onmouseout="ContentUnpreview('label71');" title="click to collapse or expand..."> more... </a>
 <div id="label71" style="display:none">
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
 <td><code class="docutils literal notranslate">v7.0.6 </code></td>
 <td><code class="docutils literal notranslate">v7.0.7 </code></td>
 <td><code class="docutils literal notranslate">v7.0.8 </code></td>
 <td><code class="docutils literal notranslate">v7.0.12 </code></td>
 <td><code class="docutils literal notranslate">v7.2.0 </code></td>
 <td><code class="docutils literal notranslate">v7.2.1 </code></td>
 <td><code class="docutils literal notranslate">v7.2.2 </code></td>
 <td><code class="docutils literal notranslate">v7.2.4 </code></td>
 <td><code class="docutils literal notranslate">v7.4.0 </code></td>
 </tr>
 <tr>
 <td>interface</td>
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
            <li> <span class="li-head">offset</span> - Offset. <span class="li-normal">type: int</span>
 <a id='label72' href="javascript:ContentClick('label73', 'label72');" onmouseover="ContentPreview('label73');" onmouseout="ContentUnpreview('label73');" title="click to collapse or expand..."> more... </a>
 <div id="label73" style="display:none">
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
 <td><code class="docutils literal notranslate">v7.0.6 </code></td>
 <td><code class="docutils literal notranslate">v7.0.7 </code></td>
 <td><code class="docutils literal notranslate">v7.0.8 </code></td>
 <td><code class="docutils literal notranslate">v7.0.12 </code></td>
 <td><code class="docutils literal notranslate">v7.2.0 </code></td>
 <td><code class="docutils literal notranslate">v7.2.1 </code></td>
 <td><code class="docutils literal notranslate">v7.2.2 </code></td>
 <td><code class="docutils literal notranslate">v7.2.4 </code></td>
 <td><code class="docutils literal notranslate">v7.4.0 </code></td>
 </tr>
 <tr>
 <td>offset</td>
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
            <li> <span class="li-head">status</span> - Status. <span class="li-normal">type: str</span> <span class="li-normal">choices: enable, disable</span>
 <a id='label74' href="javascript:ContentClick('label75', 'label74');" onmouseover="ContentPreview('label75');" onmouseout="ContentUnpreview('label75');" title="click to collapse or expand..."> more... </a>
 <div id="label75" style="display:none">
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
 <td><code class="docutils literal notranslate">v7.0.6 </code></td>
 <td><code class="docutils literal notranslate">v7.0.7 </code></td>
 <td><code class="docutils literal notranslate">v7.0.8 </code></td>
 <td><code class="docutils literal notranslate">v7.0.12 </code></td>
 <td><code class="docutils literal notranslate">v7.2.0 </code></td>
 <td><code class="docutils literal notranslate">v7.2.1 </code></td>
 <td><code class="docutils literal notranslate">v7.2.2 </code></td>
 <td><code class="docutils literal notranslate">v7.2.4 </code></td>
 <td><code class="docutils literal notranslate">v7.4.0 </code></td>
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
        <li> <span class="li-head">passive_interface</span> - Passive interface configuration. <span class="li-normal">type: list</span> <span style="font-family:'Courier New'" class="li-required">member_path: passive_interface:name</span>
 <a id='label76' href="javascript:ContentClick('label77', 'label76');" onmouseover="ContentPreview('label77');" onmouseout="ContentUnpreview('label77');" title="click to collapse or expand..."> more... </a>
 <div id="label77" style="display:none">
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
 <td><code class="docutils literal notranslate">v7.0.6 </code></td>
 <td><code class="docutils literal notranslate">v7.0.7 </code></td>
 <td><code class="docutils literal notranslate">v7.0.8 </code></td>
 <td><code class="docutils literal notranslate">v7.0.12 </code></td>
 <td><code class="docutils literal notranslate">v7.2.0 </code></td>
 <td><code class="docutils literal notranslate">v7.2.1 </code></td>
 <td><code class="docutils literal notranslate">v7.2.2 </code></td>
 <td><code class="docutils literal notranslate">v7.2.4 </code></td>
 <td><code class="docutils literal notranslate">v7.4.0 </code></td>
 </tr>
 <tr>
 <td>passive_interface</td>
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
            <li> <span class="li-head">name</span> - Passive interface name. Source system.interface.name. <span class="li-normal">type: str</span> <span class="li-required">required: true</span>
 <a id='label78' href="javascript:ContentClick('label79', 'label78');" onmouseover="ContentPreview('label79');" onmouseout="ContentUnpreview('label79');" title="click to collapse or expand..."> more... </a>
 <div id="label79" style="display:none">
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
 <td><code class="docutils literal notranslate">v7.0.6 </code></td>
 <td><code class="docutils literal notranslate">v7.0.7 </code></td>
 <td><code class="docutils literal notranslate">v7.0.8 </code></td>
 <td><code class="docutils literal notranslate">v7.0.12 </code></td>
 <td><code class="docutils literal notranslate">v7.2.0 </code></td>
 <td><code class="docutils literal notranslate">v7.2.1 </code></td>
 <td><code class="docutils literal notranslate">v7.2.2 </code></td>
 <td><code class="docutils literal notranslate">v7.2.4 </code></td>
 <td><code class="docutils literal notranslate">v7.4.0 </code></td>
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
        <li> <span class="li-head">redistribute</span> - Redistribute configuration. <span class="li-normal">type: list</span> <span style="font-family:'Courier New'" class="li-required">member_path: redistribute:name</span>
 <a id='label80' href="javascript:ContentClick('label81', 'label80');" onmouseover="ContentPreview('label81');" onmouseout="ContentUnpreview('label81');" title="click to collapse or expand..."> more... </a>
 <div id="label81" style="display:none">
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
 <td><code class="docutils literal notranslate">v7.2.0 </code></td>
 </tr>
 <tr>
 <td>redistribute</td>
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
 <td>yes</td>
 </tr>
 </table>
 </div>
 </li>
            <ul class="ul-self">
            <li> <span class="li-head">metric</span> - Redistribute metric setting. <span class="li-normal">type: int</span>
 <a id='label82' href="javascript:ContentClick('label83', 'label82');" onmouseover="ContentPreview('label83');" onmouseout="ContentUnpreview('label83');" title="click to collapse or expand..."> more... </a>
 <div id="label83" style="display:none">
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
 <td><code class="docutils literal notranslate">v7.2.0 </code></td>
 </tr>
 <tr>
 <td>metric</td>
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
 <td>yes</td>
 </tr>
 </table>
 </div>
 </li>
            <li> <span class="li-head">name</span> - Redistribute name. <span class="li-normal">type: str</span> <span class="li-required">required: true</span>
 <a id='label84' href="javascript:ContentClick('label85', 'label84');" onmouseover="ContentPreview('label85');" onmouseout="ContentUnpreview('label85');" title="click to collapse or expand..."> more... </a>
 <div id="label85" style="display:none">
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
 <td><code class="docutils literal notranslate">v7.2.0 </code></td>
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
 <td>yes</td>
 </tr>
 </table>
 </div>
 </li>
            <li> <span class="li-head">routemap</span> - Route map name. Source router.route-map.name. <span class="li-normal">type: str</span>
 <a id='label86' href="javascript:ContentClick('label87', 'label86');" onmouseover="ContentPreview('label87');" onmouseout="ContentUnpreview('label87');" title="click to collapse or expand..."> more... </a>
 <div id="label87" style="display:none">
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
 <td><code class="docutils literal notranslate">v7.2.0 </code></td>
 </tr>
 <tr>
 <td>routemap</td>
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
 <td>yes</td>
 </tr>
 </table>
 </div>
 </li>
            <li> <span class="li-head">status</span> - Status. <span class="li-normal">type: str</span> <span class="li-normal">choices: enable, disable</span>
 <a id='label88' href="javascript:ContentClick('label89', 'label88');" onmouseover="ContentPreview('label89');" onmouseout="ContentUnpreview('label89');" title="click to collapse or expand..."> more... </a>
 <div id="label89" style="display:none">
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
 <td><code class="docutils literal notranslate">v7.2.0 </code></td>
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
 <td>yes</td>
 </tr>
 </table>
 </div>
 </li>
            </ul>
        <li> <span class="li-head">timeout_timer</span> - Timeout timer. <span class="li-normal">type: int</span>
 <a id='label90' href="javascript:ContentClick('label91', 'label90');" onmouseover="ContentPreview('label91');" onmouseout="ContentUnpreview('label91');" title="click to collapse or expand..."> more... </a>
 <div id="label91" style="display:none">
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
 <td><code class="docutils literal notranslate">v7.0.6 </code></td>
 <td><code class="docutils literal notranslate">v7.0.7 </code></td>
 <td><code class="docutils literal notranslate">v7.0.8 </code></td>
 <td><code class="docutils literal notranslate">v7.0.12 </code></td>
 <td><code class="docutils literal notranslate">v7.2.0 </code></td>
 <td><code class="docutils literal notranslate">v7.2.1 </code></td>
 <td><code class="docutils literal notranslate">v7.2.2 </code></td>
 <td><code class="docutils literal notranslate">v7.2.4 </code></td>
 <td><code class="docutils literal notranslate">v7.4.0 </code></td>
 </tr>
 <tr>
 <td>timeout_timer</td>
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
        <li> <span class="li-head">update_timer</span> - Update timer. <span class="li-normal">type: int</span>
 <a id='label92' href="javascript:ContentClick('label93', 'label92');" onmouseover="ContentPreview('label93');" onmouseout="ContentUnpreview('label93');" title="click to collapse or expand..."> more... </a>
 <div id="label93" style="display:none">
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
 <td><code class="docutils literal notranslate">v7.0.6 </code></td>
 <td><code class="docutils literal notranslate">v7.0.7 </code></td>
 <td><code class="docutils literal notranslate">v7.0.8 </code></td>
 <td><code class="docutils literal notranslate">v7.0.12 </code></td>
 <td><code class="docutils literal notranslate">v7.2.0 </code></td>
 <td><code class="docutils literal notranslate">v7.2.1 </code></td>
 <td><code class="docutils literal notranslate">v7.2.2 </code></td>
 <td><code class="docutils literal notranslate">v7.2.4 </code></td>
 <td><code class="docutils literal notranslate">v7.4.0 </code></td>
 </tr>
 <tr>
 <td>update_timer</td>
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
      - name: Configure RIPng.
        fortios_router_ripng:
          vdom:  "{{ vdom }}"
          router_ripng:
            aggregate_address:
             -
                id:  "4"
                prefix6: "<your_own_value>"
            default_information_originate: "enable"
            default_metric: "1"
            distance:
             -
                access_list6: "<your_own_value> (source router.access-list6.name)"
                distance: "0"
                id:  "11"
                prefix6: "<your_own_value>"
            distribute_list:
             -
                direction: "in"
                id:  "15"
                interface: "<your_own_value> (source system.interface.name)"
                listname: "<your_own_value> (source router.access-list6.name router.prefix-list6.name)"
                status: "enable"
            garbage_timer: "120"
            interface:
             -
                flags: "8"
                name: "default_name_22 (source system.interface.name)"
                split_horizon: "poisoned"
                split_horizon_status: "enable"
            max_out_metric: "0"
            neighbor:
             -
                id:  "27"
                interface: "<your_own_value> (source system.interface.name)"
                ip6: "<your_own_value>"
            network:
             -
                id:  "31"
                prefix: "<your_own_value>"
            offset_list:
             -
                access_list6: "<your_own_value> (source router.access-list6.name)"
                direction: "in"
                id:  "36"
                interface: "<your_own_value> (source system.interface.name)"
                offset: "0"
                status: "enable"
            passive_interface:
             -
                name: "default_name_41 (source system.interface.name)"
            redistribute:
             -
                metric: "0"
                name: "default_name_44"
                routemap: "<your_own_value> (source router.route-map.name)"
                status: "enable"
            timeout_timer: "180"
            update_timer: "30"
    


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
