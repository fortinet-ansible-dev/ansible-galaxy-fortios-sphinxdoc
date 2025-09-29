:source: fortios_wireless_controller_wtp_group.py

:orphan:

.. fortios_wireless_controller_wtp_group:

fortios_wireless_controller_wtp_group -- Configure WTP groups in Fortinet's FortiOS and FortiGate.
++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++

.. versionadded:: 2.0.0

.. contents::
   :local:
   :depth: 1


Synopsis
--------
- This module is able to configure a FortiGate or FortiOS (FOS) device by allowing the user to set and modify wireless_controller feature and wtp_group category. Examples include all parameters and values need to be adjusted to datasources before usage. Tested with FOS v6.0.0



Requirements
------------
The below requirements are needed on the host that executes this module.

- ansible>=2.15


Tips
----
Using member operation to add an element to an existing object.

FortiOS Version Compatibility
-----------------------------
Supported Version Ranges: v6.0.0 -> v7.6.4


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
    <li> <span class="li-head">wireless_controller_wtp_group</span> - Configure WTP groups. <span class="li-normal">type: dict</span>
 <a id='label0' href="javascript:ContentClick('label1', 'label0');" onmouseover="ContentPreview('label1');" onmouseout="ContentUnpreview('label1');" title="click to collapse or expand..."> more... </a>
 <div id="label1" style="display:none">
 <table border="1">
 <tr>
 <td></td><td colspan="1">Supported Version Ranges</td>
 </tr>
 <tr>
 <td>wireless_controller_wtp_group</td>
 <td><code class="docutils literal notranslate">v6.0.0 -> 7.6.4 </code></td>
 </tr>
 </table>
 </div>
 </li>
        <ul class="ul-self">
        <li> <span class="li-head">ble_major_id</span> - Override BLE Major ID. <span class="li-normal">type: int</span>
 <a id='label2' href="javascript:ContentClick('label3', 'label2');" onmouseover="ContentPreview('label3');" onmouseout="ContentUnpreview('label3');" title="click to collapse or expand..."> more... </a>
 <div id="label3" style="display:none">
 <table border="1">
 <tr>
 <td></td>
 <td colspan="1">Supported Version Ranges</td>
 </tr>
 <tr>
 <td>ble_major_id</td>
 <td><code class="docutils literal notranslate">v7.4.1 -> 7.6.4 </code></td>
 </tr>
 </table>
 </div>
 </li>
        <li> <span class="li-head">name</span> - WTP group name. <span class="li-normal">type: str</span> <span class="li-required">required: true</span>
 <a id='label4' href="javascript:ContentClick('label5', 'label4');" onmouseover="ContentPreview('label5');" onmouseout="ContentUnpreview('label5');" title="click to collapse or expand..."> more... </a>
 <div id="label5" style="display:none">
 <table border="1">
 <tr>
 <td></td>
 <td colspan="1">Supported Version Ranges</td>
 </tr>
 <tr>
 <td>name</td>
 <td><code class="docutils literal notranslate">v6.0.0 -> 7.6.4 </code></td>
 </tr>
 </table>
 </div>
 </li>
        <li> <span class="li-head">platform_type</span> - FortiAP models to define the WTP group platform type. <span class="li-normal">type: str</span> <span class="li-normal">choices: AP-11N, C24JE, 421E, 423E, 221E, 222E, 223E, 224E, 231E, 321E, 431F, 431FL, 432F, 432FR, 433F, 433FL, 231F, 231FL, 234F, 23JF, 831F, 231G, 233G, 234G, 431G, 432G, 433G, 231K, 23JK, 222KL, 241K, 243K, 244K, 441K, 443K, U421E, U422EV, U423E, U221EV, U223EV, U24JEV, U321EV, U323EV, U431F, U433F, U231F, U234F, U432F, U231G, 220B, 210B, 222B, 112B, 320B, 11C, 14C, 223B, 28C, 320C, 221C, 25D, 222C, 224D, 214B, 21D, 24D, 112D, 223C, 321C, C220C, C225C, C23JD, S321C, S322C, S323C, S311C, S313C, S321CR, S322CR, S323CR, S421E, S422E, S423E, S221E, S223E, U441G</span>
 <a id='label6' href="javascript:ContentClick('label7', 'label6');" onmouseover="ContentPreview('label7');" onmouseout="ContentUnpreview('label7');" title="click to collapse or expand..."> more... </a>
 <div id="label7" style="display:none">
 <table border="1">
 <tr>
 <td></td>
 <td colspan="1">Supported Version Ranges</td>
 </tr>
 <tr>
 <td>platform_type</td>
 <td><code class="docutils literal notranslate">v6.0.0 -> 7.6.4 </code></td>
 </tr>
 <tr>
 <td>[AP-11N]</td>
 <td><code class="docutils literal notranslate">v6.0.0 -> 7.6.4</code></td>
 <tr>
 <td>[C24JE]</td>
 <td><code class="docutils literal notranslate">v6.0.0 -> 7.6.4</code></td>
 <tr>
 <td>[421E]</td>
 <td><code class="docutils literal notranslate">v6.0.0 -> 7.6.4</code></td>
 <tr>
 <td>[423E]</td>
 <td><code class="docutils literal notranslate">v6.0.0 -> 7.6.4</code></td>
 <tr>
 <td>[221E]</td>
 <td><code class="docutils literal notranslate">v6.0.0 -> 7.6.4</code></td>
 <tr>
 <td>[222E]</td>
 <td><code class="docutils literal notranslate">v6.0.0 -> 7.6.4</code></td>
 <tr>
 <td>[223E]</td>
 <td><code class="docutils literal notranslate">v6.0.0 -> 7.6.4</code></td>
 <tr>
 <td>[224E]</td>
 <td><code class="docutils literal notranslate">v6.0.0 -> 7.6.4</code></td>
 <tr>
 <td>[231E]</td>
 <td><code class="docutils literal notranslate">v6.2.0 -> v6.2.0</code></td>
 <td><code class="docutils literal notranslate">v6.2.5 -> 7.6.4</code></td>
 </tr>
 <tr>
 <td>[321E]</td>
 <td><code class="docutils literal notranslate">v6.2.0 -> 7.6.4</code></td>
 </tr>
 <tr>
 <td>[431F]</td>
 <td><code class="docutils literal notranslate">v6.2.0 -> v6.2.0</code></td>
 <td><code class="docutils literal notranslate">v6.2.5 -> 7.6.4</code></td>
 </tr>
 <tr>
 <td>[431FL]</td>
 <td><code class="docutils literal notranslate">v7.0.8 -> v7.0.12</code></td>
 <td><code class="docutils literal notranslate">v7.2.1 -> 7.6.4</code></td>
 </tr>
 <tr>
 <td>[432F]</td>
 <td><code class="docutils literal notranslate">v6.2.0 -> v6.2.0</code></td>
 <td><code class="docutils literal notranslate">v6.2.5 -> v6.4.0</code></td>
 <td><code class="docutils literal notranslate">v6.4.4 -> 7.6.4</code></td>
 </tr>
 <tr>
 <td>[432FR]</td>
 <td><code class="docutils literal notranslate">v7.0.8 -> v7.0.12</code></td>
 <td><code class="docutils literal notranslate">v7.2.1 -> 7.6.4</code></td>
 </tr>
 <tr>
 <td>[433F]</td>
 <td><code class="docutils literal notranslate">v6.2.0 -> v6.2.0</code></td>
 <td><code class="docutils literal notranslate">v6.2.5 -> 7.6.4</code></td>
 </tr>
 <tr>
 <td>[433FL]</td>
 <td><code class="docutils literal notranslate">v7.0.8 -> v7.0.12</code></td>
 <td><code class="docutils literal notranslate">v7.2.1 -> 7.6.4</code></td>
 </tr>
 <tr>
 <td>[231F]</td>
 <td><code class="docutils literal notranslate">v6.2.0 -> v6.2.0</code></td>
 <td><code class="docutils literal notranslate">v6.2.5 -> v6.4.0</code></td>
 <td><code class="docutils literal notranslate">v6.4.4 -> 7.6.4</code></td>
 </tr>
 <tr>
 <td>[231FL]</td>
 <td><code class="docutils literal notranslate">v7.0.8 -> v7.0.12</code></td>
 <td><code class="docutils literal notranslate">v7.2.1 -> 7.6.4</code></td>
 </tr>
 <tr>
 <td>[234F]</td>
 <td><code class="docutils literal notranslate">v6.2.0 -> v6.2.0</code></td>
 <td><code class="docutils literal notranslate">v6.2.5 -> v6.4.0</code></td>
 <td><code class="docutils literal notranslate">v6.4.4 -> 7.6.4</code></td>
 </tr>
 <tr>
 <td>[23JF]</td>
 <td><code class="docutils literal notranslate">v6.2.0 -> v6.2.0</code></td>
 <td><code class="docutils literal notranslate">v6.2.5 -> v6.4.0</code></td>
 <td><code class="docutils literal notranslate">v6.4.4 -> 7.6.4</code></td>
 </tr>
 <tr>
 <td>[831F]</td>
 <td><code class="docutils literal notranslate">v6.4.4 -> 7.6.4</code></td>
 </tr>
 <tr>
 <td>[231G]</td>
 <td><code class="docutils literal notranslate">v7.0.8 -> v7.0.12</code></td>
 <td><code class="docutils literal notranslate">v7.2.1 -> 7.6.4</code></td>
 </tr>
 <tr>
 <td>[233G]</td>
 <td><code class="docutils literal notranslate">v7.0.8 -> v7.0.12</code></td>
 <td><code class="docutils literal notranslate">v7.2.1 -> 7.6.4</code></td>
 </tr>
 <tr>
 <td>[234G]</td>
 <td><code class="docutils literal notranslate">v7.4.0 -> 7.6.4</code></td>
 </tr>
 <tr>
 <td>[431G]</td>
 <td><code class="docutils literal notranslate">v7.0.8 -> v7.0.12</code></td>
 <td><code class="docutils literal notranslate">v7.2.1 -> 7.6.4</code></td>
 </tr>
 <tr>
 <td>[432G]</td>
 <td><code class="docutils literal notranslate">v7.4.2 -> 7.6.4</code></td>
 </tr>
 <tr>
 <td>[433G]</td>
 <td><code class="docutils literal notranslate">v7.0.8 -> v7.0.12</code></td>
 <td><code class="docutils literal notranslate">v7.2.1 -> 7.6.4</code></td>
 </tr>
 <tr>
 <td>[231K]</td>
 <td><code class="docutils literal notranslate">v7.6.1 -> 7.6.4</code></td>
 </tr>
 <tr>
 <td>[23JK]</td>
 <td><code class="docutils literal notranslate">v7.6.1 -> 7.6.4</code></td>
 </tr>
 <tr>
 <td>[222KL]</td>
 <td><code class="docutils literal notranslate">v7.6.4 -> 7.6.4</code></td>
 </tr>
 <tr>
 <td>[241K]</td>
 <td><code class="docutils literal notranslate">v7.4.2 -> 7.6.4</code></td>
 </tr>
 <tr>
 <td>[243K]</td>
 <td><code class="docutils literal notranslate">v7.4.2 -> 7.6.4</code></td>
 </tr>
 <tr>
 <td>[244K]</td>
 <td><code class="docutils literal notranslate">v7.6.4 -> 7.6.4</code></td>
 </tr>
 <tr>
 <td>[441K]</td>
 <td><code class="docutils literal notranslate">v7.4.2 -> 7.6.4</code></td>
 </tr>
 <tr>
 <td>[443K]</td>
 <td><code class="docutils literal notranslate">v7.4.2 -> 7.6.4</code></td>
 </tr>
 <tr>
 <td>[U421E]</td>
 <td><code class="docutils literal notranslate">v6.0.0 -> 7.6.4</code></td>
 <tr>
 <td>[U422EV]</td>
 <td><code class="docutils literal notranslate">v6.0.0 -> 7.6.4</code></td>
 <tr>
 <td>[U423E]</td>
 <td><code class="docutils literal notranslate">v6.0.0 -> 7.6.4</code></td>
 <tr>
 <td>[U221EV]</td>
 <td><code class="docutils literal notranslate">v6.0.0 -> 7.6.4</code></td>
 <tr>
 <td>[U223EV]</td>
 <td><code class="docutils literal notranslate">v6.0.0 -> 7.6.4</code></td>
 <tr>
 <td>[U24JEV]</td>
 <td><code class="docutils literal notranslate">v6.0.0 -> 7.6.4</code></td>
 <tr>
 <td>[U321EV]</td>
 <td><code class="docutils literal notranslate">v6.0.0 -> 7.6.4</code></td>
 <tr>
 <td>[U323EV]</td>
 <td><code class="docutils literal notranslate">v6.0.0 -> 7.6.4</code></td>
 <tr>
 <td>[U431F]</td>
 <td><code class="docutils literal notranslate">v6.2.0 -> 7.6.4</code></td>
 </tr>
 <tr>
 <td>[U433F]</td>
 <td><code class="docutils literal notranslate">v6.2.0 -> 7.6.4</code></td>
 </tr>
 <tr>
 <td>[U231F]</td>
 <td><code class="docutils literal notranslate">v6.4.4 -> 7.6.4</code></td>
 </tr>
 <tr>
 <td>[U234F]</td>
 <td><code class="docutils literal notranslate">v6.4.4 -> 7.6.4</code></td>
 </tr>
 <tr>
 <td>[U432F]</td>
 <td><code class="docutils literal notranslate">v6.4.4 -> 7.6.4</code></td>
 </tr>
 <tr>
 <td>[U231G]</td>
 <td><code class="docutils literal notranslate">v7.0.8 -> v7.0.12</code></td>
 <td><code class="docutils literal notranslate">v7.2.4 -> 7.6.4</code></td>
 </tr>
 <tr>
 <td>[220B]</td>
 <td><code class="docutils literal notranslate">v6.0.0 -> v7.2.4</code></td>
 </tr>
 <tr>
 <td>[210B]</td>
 <td><code class="docutils literal notranslate">v6.0.0 -> v7.2.4</code></td>
 </tr>
 <tr>
 <td>[222B]</td>
 <td><code class="docutils literal notranslate">v6.0.0 -> v7.2.4</code></td>
 </tr>
 <tr>
 <td>[112B]</td>
 <td><code class="docutils literal notranslate">v6.0.0 -> v7.2.4</code></td>
 </tr>
 <tr>
 <td>[320B]</td>
 <td><code class="docutils literal notranslate">v6.0.0 -> v7.2.4</code></td>
 </tr>
 <tr>
 <td>[11C]</td>
 <td><code class="docutils literal notranslate">v6.0.0 -> v7.2.4</code></td>
 </tr>
 <tr>
 <td>[14C]</td>
 <td><code class="docutils literal notranslate">v6.0.0 -> v7.2.4</code></td>
 </tr>
 <tr>
 <td>[223B]</td>
 <td><code class="docutils literal notranslate">v6.0.0 -> v7.2.4</code></td>
 </tr>
 <tr>
 <td>[28C]</td>
 <td><code class="docutils literal notranslate">v6.0.0 -> v7.2.4</code></td>
 </tr>
 <tr>
 <td>[320C]</td>
 <td><code class="docutils literal notranslate">v6.0.0 -> v7.2.4</code></td>
 </tr>
 <tr>
 <td>[221C]</td>
 <td><code class="docutils literal notranslate">v6.0.0 -> v7.2.4</code></td>
 </tr>
 <tr>
 <td>[25D]</td>
 <td><code class="docutils literal notranslate">v6.0.0 -> v7.2.4</code></td>
 </tr>
 <tr>
 <td>[222C]</td>
 <td><code class="docutils literal notranslate">v6.0.0 -> v7.2.4</code></td>
 </tr>
 <tr>
 <td>[224D]</td>
 <td><code class="docutils literal notranslate">v6.0.0 -> v7.2.4</code></td>
 </tr>
 <tr>
 <td>[214B]</td>
 <td><code class="docutils literal notranslate">v6.0.0 -> v7.2.4</code></td>
 </tr>
 <tr>
 <td>[21D]</td>
 <td><code class="docutils literal notranslate">v6.0.0 -> v7.2.4</code></td>
 </tr>
 <tr>
 <td>[24D]</td>
 <td><code class="docutils literal notranslate">v6.0.0 -> v7.2.4</code></td>
 </tr>
 <tr>
 <td>[112D]</td>
 <td><code class="docutils literal notranslate">v6.0.0 -> v7.2.4</code></td>
 </tr>
 <tr>
 <td>[223C]</td>
 <td><code class="docutils literal notranslate">v6.0.0 -> v7.2.4</code></td>
 </tr>
 <tr>
 <td>[321C]</td>
 <td><code class="docutils literal notranslate">v6.0.0 -> v7.2.4</code></td>
 </tr>
 <tr>
 <td>[C220C]</td>
 <td><code class="docutils literal notranslate">v6.0.0 -> v7.2.4</code></td>
 </tr>
 <tr>
 <td>[C225C]</td>
 <td><code class="docutils literal notranslate">v6.0.0 -> v7.2.4</code></td>
 </tr>
 <tr>
 <td>[C23JD]</td>
 <td><code class="docutils literal notranslate">v6.0.0 -> v7.2.4</code></td>
 </tr>
 <tr>
 <td>[S321C]</td>
 <td><code class="docutils literal notranslate">v6.0.0 -> v7.2.4</code></td>
 </tr>
 <tr>
 <td>[S322C]</td>
 <td><code class="docutils literal notranslate">v6.0.0 -> v7.2.4</code></td>
 </tr>
 <tr>
 <td>[S323C]</td>
 <td><code class="docutils literal notranslate">v6.0.0 -> v7.2.4</code></td>
 </tr>
 <tr>
 <td>[S311C]</td>
 <td><code class="docutils literal notranslate">v6.0.0 -> v7.2.4</code></td>
 </tr>
 <tr>
 <td>[S313C]</td>
 <td><code class="docutils literal notranslate">v6.0.0 -> v7.2.4</code></td>
 </tr>
 <tr>
 <td>[S321CR]</td>
 <td><code class="docutils literal notranslate">v6.0.0 -> v7.2.4</code></td>
 </tr>
 <tr>
 <td>[S322CR]</td>
 <td><code class="docutils literal notranslate">v6.0.0 -> v7.2.4</code></td>
 </tr>
 <tr>
 <td>[S323CR]</td>
 <td><code class="docutils literal notranslate">v6.0.0 -> v7.2.4</code></td>
 </tr>
 <tr>
 <td>[S421E]</td>
 <td><code class="docutils literal notranslate">v6.0.0 -> v7.2.4</code></td>
 </tr>
 <tr>
 <td>[S422E]</td>
 <td><code class="docutils literal notranslate">v6.0.0 -> v7.2.4</code></td>
 </tr>
 <tr>
 <td>[S423E]</td>
 <td><code class="docutils literal notranslate">v6.0.0 -> v7.2.4</code></td>
 </tr>
 <tr>
 <td>[S221E]</td>
 <td><code class="docutils literal notranslate">v6.0.0 -> v7.2.4</code></td>
 </tr>
 <tr>
 <td>[S223E]</td>
 <td><code class="docutils literal notranslate">v6.0.0 -> v7.2.4</code></td>
 </tr>
 <tr>
 <td>[U441G]</td>
 <td><code class="docutils literal notranslate">v7.0.8 -> v7.0.12</code></td>
 <td><code class="docutils literal notranslate">v7.2.4 -> v7.2.4</code></td>
 </tr>
 </table>
 </div>
 </li>
        <li> <span class="li-head">wtps</span> - WTP list. <span class="li-normal">type: list</span> <span style="font-family:'Courier New'" class="li-required">member_path: wtps:wtp_id</span>
 <a id='label8' href="javascript:ContentClick('label9', 'label8');" onmouseover="ContentPreview('label9');" onmouseout="ContentUnpreview('label9');" title="click to collapse or expand..."> more... </a>
 <div id="label9" style="display:none">
 <table border="1">
 <tr>
 <td></td><td colspan="1">Supported Version Ranges</td>
 </tr>
 <tr>
 <td>wtps</td>
 <td><code class="docutils literal notranslate">v6.0.0 -> 7.6.4 </code></td>
 </tr>
 </table>
 </div>
 </li>
            <ul class="ul-self">
            <li> <span class="li-head">wtp_id</span> - WTP ID. Source wireless-controller.wtp.wtp-id. <span class="li-normal">type: str</span> <span class="li-required">required: true</span>
 <a id='label10' href="javascript:ContentClick('label11', 'label10');" onmouseover="ContentPreview('label11');" onmouseout="ContentUnpreview('label11');" title="click to collapse or expand..."> more... </a>
 <div id="label11" style="display:none">
 <table border="1">
 <tr>
 <td></td>
 <td colspan="1">Supported Version Ranges</td>
 </tr>
 <tr>
 <td>wtp_id</td>
 <td><code class="docutils literal notranslate">v6.0.0 -> 7.6.4 </code></td>
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
    
    - name: Configure WTP groups.
      fortinet.fortios.fortios_wireless_controller_wtp_group:
          vdom: "{{ vdom }}"
          state: "present"
          access_token: "<your_own_value>"
          wireless_controller_wtp_group:
              ble_major_id: "0"
              name: "default_name_4"
              platform_type: "AP-11N"
              wtps:
                  -
                      wtp_id: "<your_own_value> (source wireless-controller.wtp.wtp-id)"


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
