:source: fortios_system_npu.py

:orphan:

.. fortios_system_npu:

fortios_system_npu -- Configure NPU attributes in Fortinet's FortiOS and FortiGate.
+++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++

.. versionadded:: 2.0.0

.. contents::
   :local:
   :depth: 1


Synopsis
--------
- This module is able to configure a FortiGate or FortiOS (FOS) device by allowing the user to set and modify system feature and npu category. Examples include all parameters and values need to be adjusted to datasources before usage. Tested with FOS v6.0.0



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
    <li> <span class="li-head">system_npu</span> - Configure NPU attributes. <span class="li-normal">type: dict</span>
 <a id='label0' href="javascript:ContentClick('label1', 'label0');" onmouseover="ContentPreview('label1');" onmouseout="ContentUnpreview('label1');" title="click to collapse or expand..."> more... </a>
 <div id="label1" style="display:none">
 <table border="1">
 <tr>
 <td></td><td colspan="1">Supported Version Ranges</td>
 </tr>
 <tr>
 <td>system_npu</td>
 <td><code class="docutils literal notranslate">v6.0.0 -> 7.6.4 </code></td>
 </tr>
 </table>
 </div>
 </li>
        <ul class="ul-self">
        <li> <span class="li-head">capwap_offload</span> - Enable/disable offloading managed FortiAP and FortiLink CAPWAP sessions. <span class="li-normal">type: str</span> <span class="li-normal">choices: enable, disable</span>
 <a id='label2' href="javascript:ContentClick('label3', 'label2');" onmouseover="ContentPreview('label3');" onmouseout="ContentUnpreview('label3');" title="click to collapse or expand..."> more... </a>
 <div id="label3" style="display:none">
 <table border="1">
 <tr>
 <td></td>
 <td colspan="1">Supported Version Ranges</td>
 </tr>
 <tr>
 <td>capwap_offload</td>
 <td><code class="docutils literal notranslate">v6.0.0 -> 7.6.4 </code></td>
 </tr>
 <tr>
 <td>[enable]</td>
 <td><code class="docutils literal notranslate">v6.0.0 -> 7.6.4</code></td>
 <tr>
 <td>[disable]</td>
 <td><code class="docutils literal notranslate">v6.0.0 -> 7.6.4</code></td>
 </table>
 </div>
 </li>
        <li> <span class="li-head">dedicated_management_affinity</span> - Affinity setting for management daemons (hexadecimal value up to 256 bits in the format of xxxxxxxxxxxxxxxx). <span class="li-normal">type: str</span>
 <a id='label4' href="javascript:ContentClick('label5', 'label4');" onmouseover="ContentPreview('label5');" onmouseout="ContentUnpreview('label5');" title="click to collapse or expand..."> more... </a>
 <div id="label5" style="display:none">
 <table border="1">
 <tr>
 <td></td>
 <td colspan="1">Supported Version Ranges</td>
 </tr>
 <tr>
 <td>dedicated_management_affinity</td>
 <td><code class="docutils literal notranslate">v7.0.1 -> 7.6.4 </code></td>
 </tr>
 </table>
 </div>
 </li>
        <li> <span class="li-head">dedicated_management_cpu</span> - Enable to dedicate one CPU for GUI and CLI connections when NPs are busy. <span class="li-normal">type: str</span> <span class="li-normal">choices: enable, disable</span>
 <a id='label6' href="javascript:ContentClick('label7', 'label6');" onmouseover="ContentPreview('label7');" onmouseout="ContentUnpreview('label7');" title="click to collapse or expand..."> more... </a>
 <div id="label7" style="display:none">
 <table border="1">
 <tr>
 <td></td>
 <td colspan="1">Supported Version Ranges</td>
 </tr>
 <tr>
 <td>dedicated_management_cpu</td>
 <td><code class="docutils literal notranslate">v6.0.0 -> 7.6.4 </code></td>
 </tr>
 <tr>
 <td>[enable]</td>
 <td><code class="docutils literal notranslate">v6.0.0 -> 7.6.4</code></td>
 <tr>
 <td>[disable]</td>
 <td><code class="docutils literal notranslate">v6.0.0 -> 7.6.4</code></td>
 </table>
 </div>
 </li>
        <li> <span class="li-head">default_qos_type</span> - Set default QoS type. <span class="li-normal">type: str</span> <span class="li-normal">choices: policing, shaping, policing-enhanced</span>
 <a id='label8' href="javascript:ContentClick('label9', 'label8');" onmouseover="ContentPreview('label9');" onmouseout="ContentUnpreview('label9');" title="click to collapse or expand..."> more... </a>
 <div id="label9" style="display:none">
 <table border="1">
 <tr>
 <td></td>
 <td colspan="1">Supported Version Ranges</td>
 </tr>
 <tr>
 <td>default_qos_type</td>
 <td><code class="docutils literal notranslate">v7.4.2 -> v7.4.2 </code></td>
 </tr>
 <tr>
 <td>[policing]</td>
 <td><code class="docutils literal notranslate">v7.4.2 -> v7.4.2</code></td>
 <tr>
 <td>[shaping]</td>
 <td><code class="docutils literal notranslate">v7.4.2 -> v7.4.2</code></td>
 <tr>
 <td>[policing-enhanced]</td>
 <td><code class="docutils literal notranslate">v7.4.2 -> v7.4.2</code></td>
 </table>
 </div>
 </li>
        <li> <span class="li-head">dos_options</span> - NPU DoS configurations. <span class="li-normal">type: dict</span>
 <a id='label10' href="javascript:ContentClick('label11', 'label10');" onmouseover="ContentPreview('label11');" onmouseout="ContentUnpreview('label11');" title="click to collapse or expand..."> more... </a>
 <div id="label11" style="display:none">
 <table border="1">
 <tr>
 <td></td><td colspan="1">Supported Version Ranges</td>
 </tr>
 <tr>
 <td>dos_options</td>
 <td><code class="docutils literal notranslate">v7.4.2 -> v7.4.2 </code></td>
 </tr>
 </table>
 </div>
 </li>
            <ul class="ul-self">
            <li> <span class="li-head">npu_dos_meter_mode</span> - Set DoS meter NPU offloading mode. <span class="li-normal">type: str</span> <span class="li-normal">choices: global, local</span>
 <a id='label12' href="javascript:ContentClick('label13', 'label12');" onmouseover="ContentPreview('label13');" onmouseout="ContentUnpreview('label13');" title="click to collapse or expand..."> more... </a>
 <div id="label13" style="display:none">
 <table border="1">
 <tr>
 <td></td>
 <td colspan="1">Supported Version Ranges</td>
 </tr>
 <tr>
 <td>npu_dos_meter_mode</td>
 <td><code class="docutils literal notranslate">v7.4.2 -> v7.4.2 </code></td>
 </tr>
 <tr>
 <td>[global]</td>
 <td><code class="docutils literal notranslate">v7.4.2 -> v7.4.2</code></td>
 <tr>
 <td>[local]</td>
 <td><code class="docutils literal notranslate">v7.4.2 -> v7.4.2</code></td>
 </table>
 </div>
 </li>
            <li> <span class="li-head">npu_dos_tpe_mode</span> - Enable/disable insertion of DoS meter ID to session table. <span class="li-normal">type: str</span> <span class="li-normal">choices: enable, disable</span>
 <a id='label14' href="javascript:ContentClick('label15', 'label14');" onmouseover="ContentPreview('label15');" onmouseout="ContentUnpreview('label15');" title="click to collapse or expand..."> more... </a>
 <div id="label15" style="display:none">
 <table border="1">
 <tr>
 <td></td>
 <td colspan="1">Supported Version Ranges</td>
 </tr>
 <tr>
 <td>npu_dos_tpe_mode</td>
 <td><code class="docutils literal notranslate">v7.4.2 -> v7.4.2 </code></td>
 </tr>
 <tr>
 <td>[enable]</td>
 <td><code class="docutils literal notranslate">v7.4.2 -> v7.4.2</code></td>
 <tr>
 <td>[disable]</td>
 <td><code class="docutils literal notranslate">v7.4.2 -> v7.4.2</code></td>
 </table>
 </div>
 </li>
            </ul>
        <li> <span class="li-head">double_level_mcast_offload</span> - Enable double level mcast offload. <span class="li-normal">type: str</span> <span class="li-normal">choices: enable, disable</span>
 <a id='label16' href="javascript:ContentClick('label17', 'label16');" onmouseover="ContentPreview('label17');" onmouseout="ContentUnpreview('label17');" title="click to collapse or expand..."> more... </a>
 <div id="label17" style="display:none">
 <table border="1">
 <tr>
 <td></td>
 <td colspan="1">Supported Version Ranges</td>
 </tr>
 <tr>
 <td>double_level_mcast_offload</td>
 <td><code class="docutils literal notranslate">v7.4.2 -> v7.4.2 </code></td>
 </tr>
 <tr>
 <td>[enable]</td>
 <td><code class="docutils literal notranslate">v7.4.2 -> v7.4.2</code></td>
 <tr>
 <td>[disable]</td>
 <td><code class="docutils literal notranslate">v7.4.2 -> v7.4.2</code></td>
 </table>
 </div>
 </li>
        <li> <span class="li-head">dsw_dts_profile</span> - Configure NPU DSW DTS profile. <span class="li-normal">type: list</span> <span style="font-family:'Courier New'" class="li-required">member_path: dsw_dts_profile:profile_id</span>
 <a id='label18' href="javascript:ContentClick('label19', 'label18');" onmouseover="ContentPreview('label19');" onmouseout="ContentUnpreview('label19');" title="click to collapse or expand..."> more... </a>
 <div id="label19" style="display:none">
 <table border="1">
 <tr>
 <td></td><td colspan="1">Supported Version Ranges</td>
 </tr>
 <tr>
 <td>dsw_dts_profile</td>
 <td><code class="docutils literal notranslate">v7.4.2 -> v7.4.2 </code></td>
 </tr>
 </table>
 </div>
 </li>
            <ul class="ul-self">
            <li> <span class="li-head">action</span> - Set NPU DSW DTS profile action. <span class="li-normal">type: str</span> <span class="li-normal">choices: wait, drop, drop_tmr_0, drop_tmr_1, enque, enque_0, enque_1</span>
 <a id='label20' href="javascript:ContentClick('label21', 'label20');" onmouseover="ContentPreview('label21');" onmouseout="ContentUnpreview('label21');" title="click to collapse or expand..."> more... </a>
 <div id="label21" style="display:none">
 <table border="1">
 <tr>
 <td></td>
 <td colspan="1">Supported Version Ranges</td>
 </tr>
 <tr>
 <td>action</td>
 <td><code class="docutils literal notranslate">v7.4.2 -> v7.4.2 </code></td>
 </tr>
 <tr>
 <td>[wait]</td>
 <td><code class="docutils literal notranslate">v7.4.2 -> v7.4.2</code></td>
 <tr>
 <td>[drop]</td>
 <td><code class="docutils literal notranslate">v7.4.2 -> v7.4.2</code></td>
 <tr>
 <td>[drop_tmr_0]</td>
 <td><code class="docutils literal notranslate">v7.4.2 -> v7.4.2</code></td>
 <tr>
 <td>[drop_tmr_1]</td>
 <td><code class="docutils literal notranslate">v7.4.2 -> v7.4.2</code></td>
 <tr>
 <td>[enque]</td>
 <td><code class="docutils literal notranslate">v7.4.2 -> v7.4.2</code></td>
 <tr>
 <td>[enque_0]</td>
 <td><code class="docutils literal notranslate">v7.4.2 -> v7.4.2</code></td>
 <tr>
 <td>[enque_1]</td>
 <td><code class="docutils literal notranslate">v7.4.2 -> v7.4.2</code></td>
 </table>
 </div>
 </li>
            <li> <span class="li-head">min_limit</span> - Set NPU DSW DTS profile min-limt. <span class="li-normal">type: int</span>
 <a id='label22' href="javascript:ContentClick('label23', 'label22');" onmouseover="ContentPreview('label23');" onmouseout="ContentUnpreview('label23');" title="click to collapse or expand..."> more... </a>
 <div id="label23" style="display:none">
 <table border="1">
 <tr>
 <td></td>
 <td colspan="1">Supported Version Ranges</td>
 </tr>
 <tr>
 <td>min_limit</td>
 <td><code class="docutils literal notranslate">v7.4.2 -> v7.4.2 </code></td>
 </tr>
 </table>
 </div>
 </li>
            <li> <span class="li-head">profile_id</span> - Set NPU DSW DTS profile profile id. see <a href='#notes'>Notes</a>. <span class="li-normal">type: int</span> <span class="li-required">required: true</span>
 <a id='label24' href="javascript:ContentClick('label25', 'label24');" onmouseover="ContentPreview('label25');" onmouseout="ContentUnpreview('label25');" title="click to collapse or expand..."> more... </a>
 <div id="label25" style="display:none">
 <table border="1">
 <tr>
 <td></td>
 <td colspan="1">Supported Version Ranges</td>
 </tr>
 <tr>
 <td>profile_id</td>
 <td><code class="docutils literal notranslate">v7.4.2 -> v7.4.2 </code></td>
 </tr>
 </table>
 </div>
 </li>
            <li> <span class="li-head">step</span> - Set NPU DSW DTS profile step. <span class="li-normal">type: int</span>
 <a id='label26' href="javascript:ContentClick('label27', 'label26');" onmouseover="ContentPreview('label27');" onmouseout="ContentUnpreview('label27');" title="click to collapse or expand..."> more... </a>
 <div id="label27" style="display:none">
 <table border="1">
 <tr>
 <td></td>
 <td colspan="1">Supported Version Ranges</td>
 </tr>
 <tr>
 <td>step</td>
 <td><code class="docutils literal notranslate">v7.4.2 -> v7.4.2 </code></td>
 </tr>
 </table>
 </div>
 </li>
            </ul>
        <li> <span class="li-head">dsw_queue_dts_profile</span> - Configure NPU DSW Queue DTS profile. <span class="li-normal">type: list</span> <span style="font-family:'Courier New'" class="li-required">member_path: dsw_queue_dts_profile:name</span>
 <a id='label28' href="javascript:ContentClick('label29', 'label28');" onmouseover="ContentPreview('label29');" onmouseout="ContentUnpreview('label29');" title="click to collapse or expand..."> more... </a>
 <div id="label29" style="display:none">
 <table border="1">
 <tr>
 <td></td><td colspan="1">Supported Version Ranges</td>
 </tr>
 <tr>
 <td>dsw_queue_dts_profile</td>
 <td><code class="docutils literal notranslate">v7.4.2 -> v7.4.2 </code></td>
 </tr>
 </table>
 </div>
 </li>
            <ul class="ul-self">
            <li> <span class="li-head">iport</span> - Set NPU DSW DTS in port. <span class="li-normal">type: str</span> <span class="li-normal">choices: eif0, eif1, eif2, eif3, eif4, eif5, eif6, eif7, htx0, htx1, sse0, sse1, sse2, sse3, rlt, dfr, ipseci, ipseco, ipti, ipto, vep0, vep2, vep4, vep6, ivs, l2ti1, l2to, l2ti0, ple, spath, qtm</span>
 <a id='label30' href="javascript:ContentClick('label31', 'label30');" onmouseover="ContentPreview('label31');" onmouseout="ContentUnpreview('label31');" title="click to collapse or expand..."> more... </a>
 <div id="label31" style="display:none">
 <table border="1">
 <tr>
 <td></td>
 <td colspan="1">Supported Version Ranges</td>
 </tr>
 <tr>
 <td>iport</td>
 <td><code class="docutils literal notranslate">v7.4.2 -> v7.4.2 </code></td>
 </tr>
 <tr>
 <td>[eif0]</td>
 <td><code class="docutils literal notranslate">v7.4.2 -> v7.4.2</code></td>
 <tr>
 <td>[eif1]</td>
 <td><code class="docutils literal notranslate">v7.4.2 -> v7.4.2</code></td>
 <tr>
 <td>[eif2]</td>
 <td><code class="docutils literal notranslate">v7.4.2 -> v7.4.2</code></td>
 <tr>
 <td>[eif3]</td>
 <td><code class="docutils literal notranslate">v7.4.2 -> v7.4.2</code></td>
 <tr>
 <td>[eif4]</td>
 <td><code class="docutils literal notranslate">v7.4.2 -> v7.4.2</code></td>
 <tr>
 <td>[eif5]</td>
 <td><code class="docutils literal notranslate">v7.4.2 -> v7.4.2</code></td>
 <tr>
 <td>[eif6]</td>
 <td><code class="docutils literal notranslate">v7.4.2 -> v7.4.2</code></td>
 <tr>
 <td>[eif7]</td>
 <td><code class="docutils literal notranslate">v7.4.2 -> v7.4.2</code></td>
 <tr>
 <td>[htx0]</td>
 <td><code class="docutils literal notranslate">v7.4.2 -> v7.4.2</code></td>
 <tr>
 <td>[htx1]</td>
 <td><code class="docutils literal notranslate">v7.4.2 -> v7.4.2</code></td>
 <tr>
 <td>[sse0]</td>
 <td><code class="docutils literal notranslate">v7.4.2 -> v7.4.2</code></td>
 <tr>
 <td>[sse1]</td>
 <td><code class="docutils literal notranslate">v7.4.2 -> v7.4.2</code></td>
 <tr>
 <td>[sse2]</td>
 <td><code class="docutils literal notranslate">v7.4.2 -> v7.4.2</code></td>
 <tr>
 <td>[sse3]</td>
 <td><code class="docutils literal notranslate">v7.4.2 -> v7.4.2</code></td>
 <tr>
 <td>[rlt]</td>
 <td><code class="docutils literal notranslate">v7.4.2 -> v7.4.2</code></td>
 <tr>
 <td>[dfr]</td>
 <td><code class="docutils literal notranslate">v7.4.2 -> v7.4.2</code></td>
 <tr>
 <td>[ipseci]</td>
 <td><code class="docutils literal notranslate">v7.4.2 -> v7.4.2</code></td>
 <tr>
 <td>[ipseco]</td>
 <td><code class="docutils literal notranslate">v7.4.2 -> v7.4.2</code></td>
 <tr>
 <td>[ipti]</td>
 <td><code class="docutils literal notranslate">v7.4.2 -> v7.4.2</code></td>
 <tr>
 <td>[ipto]</td>
 <td><code class="docutils literal notranslate">v7.4.2 -> v7.4.2</code></td>
 <tr>
 <td>[vep0]</td>
 <td><code class="docutils literal notranslate">v7.4.2 -> v7.4.2</code></td>
 <tr>
 <td>[vep2]</td>
 <td><code class="docutils literal notranslate">v7.4.2 -> v7.4.2</code></td>
 <tr>
 <td>[vep4]</td>
 <td><code class="docutils literal notranslate">v7.4.2 -> v7.4.2</code></td>
 <tr>
 <td>[vep6]</td>
 <td><code class="docutils literal notranslate">v7.4.2 -> v7.4.2</code></td>
 <tr>
 <td>[ivs]</td>
 <td><code class="docutils literal notranslate">v7.4.2 -> v7.4.2</code></td>
 <tr>
 <td>[l2ti1]</td>
 <td><code class="docutils literal notranslate">v7.4.2 -> v7.4.2</code></td>
 <tr>
 <td>[l2to]</td>
 <td><code class="docutils literal notranslate">v7.4.2 -> v7.4.2</code></td>
 <tr>
 <td>[l2ti0]</td>
 <td><code class="docutils literal notranslate">v7.4.2 -> v7.4.2</code></td>
 <tr>
 <td>[ple]</td>
 <td><code class="docutils literal notranslate">v7.4.2 -> v7.4.2</code></td>
 <tr>
 <td>[spath]</td>
 <td><code class="docutils literal notranslate">v7.4.2 -> v7.4.2</code></td>
 <tr>
 <td>[qtm]</td>
 <td><code class="docutils literal notranslate">v7.4.2 -> v7.4.2</code></td>
 </table>
 </div>
 </li>
            <li> <span class="li-head">name</span> - Name. <span class="li-normal">type: str</span> <span class="li-required">required: true</span>
 <a id='label32' href="javascript:ContentClick('label33', 'label32');" onmouseover="ContentPreview('label33');" onmouseout="ContentUnpreview('label33');" title="click to collapse or expand..."> more... </a>
 <div id="label33" style="display:none">
 <table border="1">
 <tr>
 <td></td>
 <td colspan="1">Supported Version Ranges</td>
 </tr>
 <tr>
 <td>name</td>
 <td><code class="docutils literal notranslate">v7.4.2 -> v7.4.2 </code></td>
 </tr>
 </table>
 </div>
 </li>
            <li> <span class="li-head">oport</span> - Set NPU DSW DTS out port. <span class="li-normal">type: str</span> <span class="li-normal">choices: eif0, eif1, eif2, eif3, eif4, eif5, eif6, eif7, hrx, sse0, sse1, sse2, sse3, rlt, dfr, ipseci, ipseco, ipti, ipto, vep0, vep2, vep4, vep6, ivs, l2ti1, l2to, l2ti0, ple, sync, nss, tsk, qtm</span>
 <a id='label34' href="javascript:ContentClick('label35', 'label34');" onmouseover="ContentPreview('label35');" onmouseout="ContentUnpreview('label35');" title="click to collapse or expand..."> more... </a>
 <div id="label35" style="display:none">
 <table border="1">
 <tr>
 <td></td>
 <td colspan="1">Supported Version Ranges</td>
 </tr>
 <tr>
 <td>oport</td>
 <td><code class="docutils literal notranslate">v7.4.2 -> v7.4.2 </code></td>
 </tr>
 <tr>
 <td>[eif0]</td>
 <td><code class="docutils literal notranslate">v7.4.2 -> v7.4.2</code></td>
 <tr>
 <td>[eif1]</td>
 <td><code class="docutils literal notranslate">v7.4.2 -> v7.4.2</code></td>
 <tr>
 <td>[eif2]</td>
 <td><code class="docutils literal notranslate">v7.4.2 -> v7.4.2</code></td>
 <tr>
 <td>[eif3]</td>
 <td><code class="docutils literal notranslate">v7.4.2 -> v7.4.2</code></td>
 <tr>
 <td>[eif4]</td>
 <td><code class="docutils literal notranslate">v7.4.2 -> v7.4.2</code></td>
 <tr>
 <td>[eif5]</td>
 <td><code class="docutils literal notranslate">v7.4.2 -> v7.4.2</code></td>
 <tr>
 <td>[eif6]</td>
 <td><code class="docutils literal notranslate">v7.4.2 -> v7.4.2</code></td>
 <tr>
 <td>[eif7]</td>
 <td><code class="docutils literal notranslate">v7.4.2 -> v7.4.2</code></td>
 <tr>
 <td>[hrx]</td>
 <td><code class="docutils literal notranslate">v7.4.2 -> v7.4.2</code></td>
 <tr>
 <td>[sse0]</td>
 <td><code class="docutils literal notranslate">v7.4.2 -> v7.4.2</code></td>
 <tr>
 <td>[sse1]</td>
 <td><code class="docutils literal notranslate">v7.4.2 -> v7.4.2</code></td>
 <tr>
 <td>[sse2]</td>
 <td><code class="docutils literal notranslate">v7.4.2 -> v7.4.2</code></td>
 <tr>
 <td>[sse3]</td>
 <td><code class="docutils literal notranslate">v7.4.2 -> v7.4.2</code></td>
 <tr>
 <td>[rlt]</td>
 <td><code class="docutils literal notranslate">v7.4.2 -> v7.4.2</code></td>
 <tr>
 <td>[dfr]</td>
 <td><code class="docutils literal notranslate">v7.4.2 -> v7.4.2</code></td>
 <tr>
 <td>[ipseci]</td>
 <td><code class="docutils literal notranslate">v7.4.2 -> v7.4.2</code></td>
 <tr>
 <td>[ipseco]</td>
 <td><code class="docutils literal notranslate">v7.4.2 -> v7.4.2</code></td>
 <tr>
 <td>[ipti]</td>
 <td><code class="docutils literal notranslate">v7.4.2 -> v7.4.2</code></td>
 <tr>
 <td>[ipto]</td>
 <td><code class="docutils literal notranslate">v7.4.2 -> v7.4.2</code></td>
 <tr>
 <td>[vep0]</td>
 <td><code class="docutils literal notranslate">v7.4.2 -> v7.4.2</code></td>
 <tr>
 <td>[vep2]</td>
 <td><code class="docutils literal notranslate">v7.4.2 -> v7.4.2</code></td>
 <tr>
 <td>[vep4]</td>
 <td><code class="docutils literal notranslate">v7.4.2 -> v7.4.2</code></td>
 <tr>
 <td>[vep6]</td>
 <td><code class="docutils literal notranslate">v7.4.2 -> v7.4.2</code></td>
 <tr>
 <td>[ivs]</td>
 <td><code class="docutils literal notranslate">v7.4.2 -> v7.4.2</code></td>
 <tr>
 <td>[l2ti1]</td>
 <td><code class="docutils literal notranslate">v7.4.2 -> v7.4.2</code></td>
 <tr>
 <td>[l2to]</td>
 <td><code class="docutils literal notranslate">v7.4.2 -> v7.4.2</code></td>
 <tr>
 <td>[l2ti0]</td>
 <td><code class="docutils literal notranslate">v7.4.2 -> v7.4.2</code></td>
 <tr>
 <td>[ple]</td>
 <td><code class="docutils literal notranslate">v7.4.2 -> v7.4.2</code></td>
 <tr>
 <td>[sync]</td>
 <td><code class="docutils literal notranslate">v7.4.2 -> v7.4.2</code></td>
 <tr>
 <td>[nss]</td>
 <td><code class="docutils literal notranslate">v7.4.2 -> v7.4.2</code></td>
 <tr>
 <td>[tsk]</td>
 <td><code class="docutils literal notranslate">v7.4.2 -> v7.4.2</code></td>
 <tr>
 <td>[qtm]</td>
 <td><code class="docutils literal notranslate">v7.4.2 -> v7.4.2</code></td>
 </table>
 </div>
 </li>
            <li> <span class="li-head">profile_id</span> - Set NPU DSW DTS profile ID. <span class="li-normal">type: int</span>
 <a id='label36' href="javascript:ContentClick('label37', 'label36');" onmouseover="ContentPreview('label37');" onmouseout="ContentUnpreview('label37');" title="click to collapse or expand..."> more... </a>
 <div id="label37" style="display:none">
 <table border="1">
 <tr>
 <td></td>
 <td colspan="1">Supported Version Ranges</td>
 </tr>
 <tr>
 <td>profile_id</td>
 <td><code class="docutils literal notranslate">v7.4.2 -> v7.4.2 </code></td>
 </tr>
 </table>
 </div>
 </li>
            <li> <span class="li-head">queue_select</span> - Set NPU DSW DTS queue ID select (0 - reset to default). <span class="li-normal">type: int</span>
 <a id='label38' href="javascript:ContentClick('label39', 'label38');" onmouseover="ContentPreview('label39');" onmouseout="ContentUnpreview('label39');" title="click to collapse or expand..."> more... </a>
 <div id="label39" style="display:none">
 <table border="1">
 <tr>
 <td></td>
 <td colspan="1">Supported Version Ranges</td>
 </tr>
 <tr>
 <td>queue_select</td>
 <td><code class="docutils literal notranslate">v7.4.2 -> v7.4.2 </code></td>
 </tr>
 </table>
 </div>
 </li>
            </ul>
        <li> <span class="li-head">fastpath</span> - Enable/disable NP6 offloading (also called fast path). <span class="li-normal">type: str</span> <span class="li-normal">choices: disable, enable</span>
 <a id='label40' href="javascript:ContentClick('label41', 'label40');" onmouseover="ContentPreview('label41');" onmouseout="ContentUnpreview('label41');" title="click to collapse or expand..."> more... </a>
 <div id="label41" style="display:none">
 <table border="1">
 <tr>
 <td></td>
 <td colspan="2">Supported Version Ranges</td>
 </tr>
 <tr>
 <td>fastpath</td>
 <td><code class="docutils literal notranslate">v6.0.0 -> v7.4.1 </code></td>
 <td><code class="docutils literal notranslate">v7.4.3 -> 7.6.4 </code></td>
 </tr>
 <tr>
 <td>[disable]</td>
 <td><code class="docutils literal notranslate">v6.0.0 -> v7.4.1</code></td>
 <tr>
 <td>[enable]</td>
 <td><code class="docutils literal notranslate">v6.0.0 -> v7.4.1</code></td>
 </table>
 </div>
 </li>
        <li> <span class="li-head">fp_anomaly</span> - IPv4/IPv6 anomaly protection. <span class="li-normal">type: dict</span>
 <a id='label42' href="javascript:ContentClick('label43', 'label42');" onmouseover="ContentPreview('label43');" onmouseout="ContentUnpreview('label43');" title="click to collapse or expand..."> more... </a>
 <div id="label43" style="display:none">
 <table border="1">
 <tr>
 <td></td><td colspan="1">Supported Version Ranges</td>
 </tr>
 <tr>
 <td>fp_anomaly</td>
 <td><code class="docutils literal notranslate">v7.4.2 -> v7.4.2 </code></td>
 </tr>
 </table>
 </div>
 </li>
            <ul class="ul-self">
            <li> <span class="li-head">icmp_csum_err</span> - Invalid IPv4 ICMP checksum anomalies. <span class="li-normal">type: str</span> <span class="li-normal">choices: drop, trap-to-host</span>
 <a id='label44' href="javascript:ContentClick('label45', 'label44');" onmouseover="ContentPreview('label45');" onmouseout="ContentUnpreview('label45');" title="click to collapse or expand..."> more... </a>
 <div id="label45" style="display:none">
 <table border="1">
 <tr>
 <td></td>
 <td colspan="1">Supported Version Ranges</td>
 </tr>
 <tr>
 <td>icmp_csum_err</td>
 <td><code class="docutils literal notranslate">v7.4.2 -> v7.4.2 </code></td>
 </tr>
 <tr>
 <td>[drop]</td>
 <td><code class="docutils literal notranslate">v7.4.2 -> v7.4.2</code></td>
 <tr>
 <td>[trap-to-host]</td>
 <td><code class="docutils literal notranslate">v7.4.2 -> v7.4.2</code></td>
 </table>
 </div>
 </li>
            <li> <span class="li-head">icmp_frag</span> - Layer 3 fragmented packets that could be part of layer 4 ICMP anomalies. <span class="li-normal">type: str</span> <span class="li-normal">choices: allow, drop, trap-to-host</span>
 <a id='label46' href="javascript:ContentClick('label47', 'label46');" onmouseover="ContentPreview('label47');" onmouseout="ContentUnpreview('label47');" title="click to collapse or expand..."> more... </a>
 <div id="label47" style="display:none">
 <table border="1">
 <tr>
 <td></td>
 <td colspan="1">Supported Version Ranges</td>
 </tr>
 <tr>
 <td>icmp_frag</td>
 <td><code class="docutils literal notranslate">v7.4.2 -> v7.4.2 </code></td>
 </tr>
 <tr>
 <td>[allow]</td>
 <td><code class="docutils literal notranslate">v7.4.2 -> v7.4.2</code></td>
 <tr>
 <td>[drop]</td>
 <td><code class="docutils literal notranslate">v7.4.2 -> v7.4.2</code></td>
 <tr>
 <td>[trap-to-host]</td>
 <td><code class="docutils literal notranslate">v7.4.2 -> v7.4.2</code></td>
 </table>
 </div>
 </li>
            <li> <span class="li-head">icmp_land</span> - ICMP land anomalies. <span class="li-normal">type: str</span> <span class="li-normal">choices: allow, drop, trap-to-host</span>
 <a id='label48' href="javascript:ContentClick('label49', 'label48');" onmouseover="ContentPreview('label49');" onmouseout="ContentUnpreview('label49');" title="click to collapse or expand..."> more... </a>
 <div id="label49" style="display:none">
 <table border="1">
 <tr>
 <td></td>
 <td colspan="1">Supported Version Ranges</td>
 </tr>
 <tr>
 <td>icmp_land</td>
 <td><code class="docutils literal notranslate">v7.4.2 -> v7.4.2 </code></td>
 </tr>
 <tr>
 <td>[allow]</td>
 <td><code class="docutils literal notranslate">v7.4.2 -> v7.4.2</code></td>
 <tr>
 <td>[drop]</td>
 <td><code class="docutils literal notranslate">v7.4.2 -> v7.4.2</code></td>
 <tr>
 <td>[trap-to-host]</td>
 <td><code class="docutils literal notranslate">v7.4.2 -> v7.4.2</code></td>
 </table>
 </div>
 </li>
            <li> <span class="li-head">ipv4_csum_err</span> - Invalid IPv4 IP checksum anomalies. <span class="li-normal">type: str</span> <span class="li-normal">choices: drop, trap-to-host</span>
 <a id='label50' href="javascript:ContentClick('label51', 'label50');" onmouseover="ContentPreview('label51');" onmouseout="ContentUnpreview('label51');" title="click to collapse or expand..."> more... </a>
 <div id="label51" style="display:none">
 <table border="1">
 <tr>
 <td></td>
 <td colspan="1">Supported Version Ranges</td>
 </tr>
 <tr>
 <td>ipv4_csum_err</td>
 <td><code class="docutils literal notranslate">v7.4.2 -> v7.4.2 </code></td>
 </tr>
 <tr>
 <td>[drop]</td>
 <td><code class="docutils literal notranslate">v7.4.2 -> v7.4.2</code></td>
 <tr>
 <td>[trap-to-host]</td>
 <td><code class="docutils literal notranslate">v7.4.2 -> v7.4.2</code></td>
 </table>
 </div>
 </li>
            <li> <span class="li-head">ipv4_land</span> - Land anomalies. <span class="li-normal">type: str</span> <span class="li-normal">choices: allow, drop, trap-to-host</span>
 <a id='label52' href="javascript:ContentClick('label53', 'label52');" onmouseover="ContentPreview('label53');" onmouseout="ContentUnpreview('label53');" title="click to collapse or expand..."> more... </a>
 <div id="label53" style="display:none">
 <table border="1">
 <tr>
 <td></td>
 <td colspan="1">Supported Version Ranges</td>
 </tr>
 <tr>
 <td>ipv4_land</td>
 <td><code class="docutils literal notranslate">v7.4.2 -> v7.4.2 </code></td>
 </tr>
 <tr>
 <td>[allow]</td>
 <td><code class="docutils literal notranslate">v7.4.2 -> v7.4.2</code></td>
 <tr>
 <td>[drop]</td>
 <td><code class="docutils literal notranslate">v7.4.2 -> v7.4.2</code></td>
 <tr>
 <td>[trap-to-host]</td>
 <td><code class="docutils literal notranslate">v7.4.2 -> v7.4.2</code></td>
 </table>
 </div>
 </li>
            <li> <span class="li-head">ipv4_optlsrr</span> - Loose source record route option anomalies. <span class="li-normal">type: str</span> <span class="li-normal">choices: allow, drop, trap-to-host</span>
 <a id='label54' href="javascript:ContentClick('label55', 'label54');" onmouseover="ContentPreview('label55');" onmouseout="ContentUnpreview('label55');" title="click to collapse or expand..."> more... </a>
 <div id="label55" style="display:none">
 <table border="1">
 <tr>
 <td></td>
 <td colspan="1">Supported Version Ranges</td>
 </tr>
 <tr>
 <td>ipv4_optlsrr</td>
 <td><code class="docutils literal notranslate">v7.4.2 -> v7.4.2 </code></td>
 </tr>
 <tr>
 <td>[allow]</td>
 <td><code class="docutils literal notranslate">v7.4.2 -> v7.4.2</code></td>
 <tr>
 <td>[drop]</td>
 <td><code class="docutils literal notranslate">v7.4.2 -> v7.4.2</code></td>
 <tr>
 <td>[trap-to-host]</td>
 <td><code class="docutils literal notranslate">v7.4.2 -> v7.4.2</code></td>
 </table>
 </div>
 </li>
            <li> <span class="li-head">ipv4_optrr</span> - Record route option anomalies. <span class="li-normal">type: str</span> <span class="li-normal">choices: allow, drop, trap-to-host</span>
 <a id='label56' href="javascript:ContentClick('label57', 'label56');" onmouseover="ContentPreview('label57');" onmouseout="ContentUnpreview('label57');" title="click to collapse or expand..."> more... </a>
 <div id="label57" style="display:none">
 <table border="1">
 <tr>
 <td></td>
 <td colspan="1">Supported Version Ranges</td>
 </tr>
 <tr>
 <td>ipv4_optrr</td>
 <td><code class="docutils literal notranslate">v7.4.2 -> v7.4.2 </code></td>
 </tr>
 <tr>
 <td>[allow]</td>
 <td><code class="docutils literal notranslate">v7.4.2 -> v7.4.2</code></td>
 <tr>
 <td>[drop]</td>
 <td><code class="docutils literal notranslate">v7.4.2 -> v7.4.2</code></td>
 <tr>
 <td>[trap-to-host]</td>
 <td><code class="docutils literal notranslate">v7.4.2 -> v7.4.2</code></td>
 </table>
 </div>
 </li>
            <li> <span class="li-head">ipv4_optsecurity</span> - Security option anomalies. <span class="li-normal">type: str</span> <span class="li-normal">choices: allow, drop, trap-to-host</span>
 <a id='label58' href="javascript:ContentClick('label59', 'label58');" onmouseover="ContentPreview('label59');" onmouseout="ContentUnpreview('label59');" title="click to collapse or expand..."> more... </a>
 <div id="label59" style="display:none">
 <table border="1">
 <tr>
 <td></td>
 <td colspan="1">Supported Version Ranges</td>
 </tr>
 <tr>
 <td>ipv4_optsecurity</td>
 <td><code class="docutils literal notranslate">v7.4.2 -> v7.4.2 </code></td>
 </tr>
 <tr>
 <td>[allow]</td>
 <td><code class="docutils literal notranslate">v7.4.2 -> v7.4.2</code></td>
 <tr>
 <td>[drop]</td>
 <td><code class="docutils literal notranslate">v7.4.2 -> v7.4.2</code></td>
 <tr>
 <td>[trap-to-host]</td>
 <td><code class="docutils literal notranslate">v7.4.2 -> v7.4.2</code></td>
 </table>
 </div>
 </li>
            <li> <span class="li-head">ipv4_optssrr</span> - Strict source record route option anomalies. <span class="li-normal">type: str</span> <span class="li-normal">choices: allow, drop, trap-to-host</span>
 <a id='label60' href="javascript:ContentClick('label61', 'label60');" onmouseover="ContentPreview('label61');" onmouseout="ContentUnpreview('label61');" title="click to collapse or expand..."> more... </a>
 <div id="label61" style="display:none">
 <table border="1">
 <tr>
 <td></td>
 <td colspan="1">Supported Version Ranges</td>
 </tr>
 <tr>
 <td>ipv4_optssrr</td>
 <td><code class="docutils literal notranslate">v7.4.2 -> v7.4.2 </code></td>
 </tr>
 <tr>
 <td>[allow]</td>
 <td><code class="docutils literal notranslate">v7.4.2 -> v7.4.2</code></td>
 <tr>
 <td>[drop]</td>
 <td><code class="docutils literal notranslate">v7.4.2 -> v7.4.2</code></td>
 <tr>
 <td>[trap-to-host]</td>
 <td><code class="docutils literal notranslate">v7.4.2 -> v7.4.2</code></td>
 </table>
 </div>
 </li>
            <li> <span class="li-head">ipv4_optstream</span> - Stream option anomalies. <span class="li-normal">type: str</span> <span class="li-normal">choices: allow, drop, trap-to-host</span>
 <a id='label62' href="javascript:ContentClick('label63', 'label62');" onmouseover="ContentPreview('label63');" onmouseout="ContentUnpreview('label63');" title="click to collapse or expand..."> more... </a>
 <div id="label63" style="display:none">
 <table border="1">
 <tr>
 <td></td>
 <td colspan="1">Supported Version Ranges</td>
 </tr>
 <tr>
 <td>ipv4_optstream</td>
 <td><code class="docutils literal notranslate">v7.4.2 -> v7.4.2 </code></td>
 </tr>
 <tr>
 <td>[allow]</td>
 <td><code class="docutils literal notranslate">v7.4.2 -> v7.4.2</code></td>
 <tr>
 <td>[drop]</td>
 <td><code class="docutils literal notranslate">v7.4.2 -> v7.4.2</code></td>
 <tr>
 <td>[trap-to-host]</td>
 <td><code class="docutils literal notranslate">v7.4.2 -> v7.4.2</code></td>
 </table>
 </div>
 </li>
            <li> <span class="li-head">ipv4_opttimestamp</span> - Timestamp option anomalies. <span class="li-normal">type: str</span> <span class="li-normal">choices: allow, drop, trap-to-host</span>
 <a id='label64' href="javascript:ContentClick('label65', 'label64');" onmouseover="ContentPreview('label65');" onmouseout="ContentUnpreview('label65');" title="click to collapse or expand..."> more... </a>
 <div id="label65" style="display:none">
 <table border="1">
 <tr>
 <td></td>
 <td colspan="1">Supported Version Ranges</td>
 </tr>
 <tr>
 <td>ipv4_opttimestamp</td>
 <td><code class="docutils literal notranslate">v7.4.2 -> v7.4.2 </code></td>
 </tr>
 <tr>
 <td>[allow]</td>
 <td><code class="docutils literal notranslate">v7.4.2 -> v7.4.2</code></td>
 <tr>
 <td>[drop]</td>
 <td><code class="docutils literal notranslate">v7.4.2 -> v7.4.2</code></td>
 <tr>
 <td>[trap-to-host]</td>
 <td><code class="docutils literal notranslate">v7.4.2 -> v7.4.2</code></td>
 </table>
 </div>
 </li>
            <li> <span class="li-head">ipv4_proto_err</span> - Invalid layer 4 protocol anomalies. <span class="li-normal">type: str</span> <span class="li-normal">choices: allow, drop, trap-to-host</span>
 <a id='label66' href="javascript:ContentClick('label67', 'label66');" onmouseover="ContentPreview('label67');" onmouseout="ContentUnpreview('label67');" title="click to collapse or expand..."> more... </a>
 <div id="label67" style="display:none">
 <table border="1">
 <tr>
 <td></td>
 <td colspan="1">Supported Version Ranges</td>
 </tr>
 <tr>
 <td>ipv4_proto_err</td>
 <td><code class="docutils literal notranslate">v7.4.2 -> v7.4.2 </code></td>
 </tr>
 <tr>
 <td>[allow]</td>
 <td><code class="docutils literal notranslate">v7.4.2 -> v7.4.2</code></td>
 <tr>
 <td>[drop]</td>
 <td><code class="docutils literal notranslate">v7.4.2 -> v7.4.2</code></td>
 <tr>
 <td>[trap-to-host]</td>
 <td><code class="docutils literal notranslate">v7.4.2 -> v7.4.2</code></td>
 </table>
 </div>
 </li>
            <li> <span class="li-head">ipv4_unknopt</span> - Unknown option anomalies. <span class="li-normal">type: str</span> <span class="li-normal">choices: allow, drop, trap-to-host</span>
 <a id='label68' href="javascript:ContentClick('label69', 'label68');" onmouseover="ContentPreview('label69');" onmouseout="ContentUnpreview('label69');" title="click to collapse or expand..."> more... </a>
 <div id="label69" style="display:none">
 <table border="1">
 <tr>
 <td></td>
 <td colspan="1">Supported Version Ranges</td>
 </tr>
 <tr>
 <td>ipv4_unknopt</td>
 <td><code class="docutils literal notranslate">v7.4.2 -> v7.4.2 </code></td>
 </tr>
 <tr>
 <td>[allow]</td>
 <td><code class="docutils literal notranslate">v7.4.2 -> v7.4.2</code></td>
 <tr>
 <td>[drop]</td>
 <td><code class="docutils literal notranslate">v7.4.2 -> v7.4.2</code></td>
 <tr>
 <td>[trap-to-host]</td>
 <td><code class="docutils literal notranslate">v7.4.2 -> v7.4.2</code></td>
 </table>
 </div>
 </li>
            <li> <span class="li-head">ipv6_daddr_err</span> - Destination address as unspecified or loopback address anomalies. <span class="li-normal">type: str</span> <span class="li-normal">choices: allow, drop, trap-to-host</span>
 <a id='label70' href="javascript:ContentClick('label71', 'label70');" onmouseover="ContentPreview('label71');" onmouseout="ContentUnpreview('label71');" title="click to collapse or expand..."> more... </a>
 <div id="label71" style="display:none">
 <table border="1">
 <tr>
 <td></td>
 <td colspan="1">Supported Version Ranges</td>
 </tr>
 <tr>
 <td>ipv6_daddr_err</td>
 <td><code class="docutils literal notranslate">v7.4.2 -> v7.4.2 </code></td>
 </tr>
 <tr>
 <td>[allow]</td>
 <td><code class="docutils literal notranslate">v7.4.2 -> v7.4.2</code></td>
 <tr>
 <td>[drop]</td>
 <td><code class="docutils literal notranslate">v7.4.2 -> v7.4.2</code></td>
 <tr>
 <td>[trap-to-host]</td>
 <td><code class="docutils literal notranslate">v7.4.2 -> v7.4.2</code></td>
 </table>
 </div>
 </li>
            <li> <span class="li-head">ipv6_land</span> - Land anomalies. <span class="li-normal">type: str</span> <span class="li-normal">choices: allow, drop, trap-to-host</span>
 <a id='label72' href="javascript:ContentClick('label73', 'label72');" onmouseover="ContentPreview('label73');" onmouseout="ContentUnpreview('label73');" title="click to collapse or expand..."> more... </a>
 <div id="label73" style="display:none">
 <table border="1">
 <tr>
 <td></td>
 <td colspan="1">Supported Version Ranges</td>
 </tr>
 <tr>
 <td>ipv6_land</td>
 <td><code class="docutils literal notranslate">v7.4.2 -> v7.4.2 </code></td>
 </tr>
 <tr>
 <td>[allow]</td>
 <td><code class="docutils literal notranslate">v7.4.2 -> v7.4.2</code></td>
 <tr>
 <td>[drop]</td>
 <td><code class="docutils literal notranslate">v7.4.2 -> v7.4.2</code></td>
 <tr>
 <td>[trap-to-host]</td>
 <td><code class="docutils literal notranslate">v7.4.2 -> v7.4.2</code></td>
 </table>
 </div>
 </li>
            <li> <span class="li-head">ipv6_optendpid</span> - End point identification anomalies. <span class="li-normal">type: str</span> <span class="li-normal">choices: allow, drop, trap-to-host</span>
 <a id='label74' href="javascript:ContentClick('label75', 'label74');" onmouseover="ContentPreview('label75');" onmouseout="ContentUnpreview('label75');" title="click to collapse or expand..."> more... </a>
 <div id="label75" style="display:none">
 <table border="1">
 <tr>
 <td></td>
 <td colspan="1">Supported Version Ranges</td>
 </tr>
 <tr>
 <td>ipv6_optendpid</td>
 <td><code class="docutils literal notranslate">v7.4.2 -> v7.4.2 </code></td>
 </tr>
 <tr>
 <td>[allow]</td>
 <td><code class="docutils literal notranslate">v7.4.2 -> v7.4.2</code></td>
 <tr>
 <td>[drop]</td>
 <td><code class="docutils literal notranslate">v7.4.2 -> v7.4.2</code></td>
 <tr>
 <td>[trap-to-host]</td>
 <td><code class="docutils literal notranslate">v7.4.2 -> v7.4.2</code></td>
 </table>
 </div>
 </li>
            <li> <span class="li-head">ipv6_opthomeaddr</span> - Home address option anomalies. <span class="li-normal">type: str</span> <span class="li-normal">choices: allow, drop, trap-to-host</span>
 <a id='label76' href="javascript:ContentClick('label77', 'label76');" onmouseover="ContentPreview('label77');" onmouseout="ContentUnpreview('label77');" title="click to collapse or expand..."> more... </a>
 <div id="label77" style="display:none">
 <table border="1">
 <tr>
 <td></td>
 <td colspan="1">Supported Version Ranges</td>
 </tr>
 <tr>
 <td>ipv6_opthomeaddr</td>
 <td><code class="docutils literal notranslate">v7.4.2 -> v7.4.2 </code></td>
 </tr>
 <tr>
 <td>[allow]</td>
 <td><code class="docutils literal notranslate">v7.4.2 -> v7.4.2</code></td>
 <tr>
 <td>[drop]</td>
 <td><code class="docutils literal notranslate">v7.4.2 -> v7.4.2</code></td>
 <tr>
 <td>[trap-to-host]</td>
 <td><code class="docutils literal notranslate">v7.4.2 -> v7.4.2</code></td>
 </table>
 </div>
 </li>
            <li> <span class="li-head">ipv6_optinvld</span> - Invalid option anomalies.Invalid option anomalies. <span class="li-normal">type: str</span> <span class="li-normal">choices: allow, drop, trap-to-host</span>
 <a id='label78' href="javascript:ContentClick('label79', 'label78');" onmouseover="ContentPreview('label79');" onmouseout="ContentUnpreview('label79');" title="click to collapse or expand..."> more... </a>
 <div id="label79" style="display:none">
 <table border="1">
 <tr>
 <td></td>
 <td colspan="1">Supported Version Ranges</td>
 </tr>
 <tr>
 <td>ipv6_optinvld</td>
 <td><code class="docutils literal notranslate">v7.4.2 -> v7.4.2 </code></td>
 </tr>
 <tr>
 <td>[allow]</td>
 <td><code class="docutils literal notranslate">v7.4.2 -> v7.4.2</code></td>
 <tr>
 <td>[drop]</td>
 <td><code class="docutils literal notranslate">v7.4.2 -> v7.4.2</code></td>
 <tr>
 <td>[trap-to-host]</td>
 <td><code class="docutils literal notranslate">v7.4.2 -> v7.4.2</code></td>
 </table>
 </div>
 </li>
            <li> <span class="li-head">ipv6_optjumbo</span> - Jumbo options anomalies. <span class="li-normal">type: str</span> <span class="li-normal">choices: allow, drop, trap-to-host</span>
 <a id='label80' href="javascript:ContentClick('label81', 'label80');" onmouseover="ContentPreview('label81');" onmouseout="ContentUnpreview('label81');" title="click to collapse or expand..."> more... </a>
 <div id="label81" style="display:none">
 <table border="1">
 <tr>
 <td></td>
 <td colspan="1">Supported Version Ranges</td>
 </tr>
 <tr>
 <td>ipv6_optjumbo</td>
 <td><code class="docutils literal notranslate">v7.4.2 -> v7.4.2 </code></td>
 </tr>
 <tr>
 <td>[allow]</td>
 <td><code class="docutils literal notranslate">v7.4.2 -> v7.4.2</code></td>
 <tr>
 <td>[drop]</td>
 <td><code class="docutils literal notranslate">v7.4.2 -> v7.4.2</code></td>
 <tr>
 <td>[trap-to-host]</td>
 <td><code class="docutils literal notranslate">v7.4.2 -> v7.4.2</code></td>
 </table>
 </div>
 </li>
            <li> <span class="li-head">ipv6_optnsap</span> - Network service access point address option anomalies. <span class="li-normal">type: str</span> <span class="li-normal">choices: allow, drop, trap-to-host</span>
 <a id='label82' href="javascript:ContentClick('label83', 'label82');" onmouseover="ContentPreview('label83');" onmouseout="ContentUnpreview('label83');" title="click to collapse or expand..."> more... </a>
 <div id="label83" style="display:none">
 <table border="1">
 <tr>
 <td></td>
 <td colspan="1">Supported Version Ranges</td>
 </tr>
 <tr>
 <td>ipv6_optnsap</td>
 <td><code class="docutils literal notranslate">v7.4.2 -> v7.4.2 </code></td>
 </tr>
 <tr>
 <td>[allow]</td>
 <td><code class="docutils literal notranslate">v7.4.2 -> v7.4.2</code></td>
 <tr>
 <td>[drop]</td>
 <td><code class="docutils literal notranslate">v7.4.2 -> v7.4.2</code></td>
 <tr>
 <td>[trap-to-host]</td>
 <td><code class="docutils literal notranslate">v7.4.2 -> v7.4.2</code></td>
 </table>
 </div>
 </li>
            <li> <span class="li-head">ipv6_optralert</span> - Router alert option anomalies. <span class="li-normal">type: str</span> <span class="li-normal">choices: allow, drop, trap-to-host</span>
 <a id='label84' href="javascript:ContentClick('label85', 'label84');" onmouseover="ContentPreview('label85');" onmouseout="ContentUnpreview('label85');" title="click to collapse or expand..."> more... </a>
 <div id="label85" style="display:none">
 <table border="1">
 <tr>
 <td></td>
 <td colspan="1">Supported Version Ranges</td>
 </tr>
 <tr>
 <td>ipv6_optralert</td>
 <td><code class="docutils literal notranslate">v7.4.2 -> v7.4.2 </code></td>
 </tr>
 <tr>
 <td>[allow]</td>
 <td><code class="docutils literal notranslate">v7.4.2 -> v7.4.2</code></td>
 <tr>
 <td>[drop]</td>
 <td><code class="docutils literal notranslate">v7.4.2 -> v7.4.2</code></td>
 <tr>
 <td>[trap-to-host]</td>
 <td><code class="docutils literal notranslate">v7.4.2 -> v7.4.2</code></td>
 </table>
 </div>
 </li>
            <li> <span class="li-head">ipv6_opttunnel</span> - Tunnel encapsulation limit option anomalies. <span class="li-normal">type: str</span> <span class="li-normal">choices: allow, drop, trap-to-host</span>
 <a id='label86' href="javascript:ContentClick('label87', 'label86');" onmouseover="ContentPreview('label87');" onmouseout="ContentUnpreview('label87');" title="click to collapse or expand..."> more... </a>
 <div id="label87" style="display:none">
 <table border="1">
 <tr>
 <td></td>
 <td colspan="1">Supported Version Ranges</td>
 </tr>
 <tr>
 <td>ipv6_opttunnel</td>
 <td><code class="docutils literal notranslate">v7.4.2 -> v7.4.2 </code></td>
 </tr>
 <tr>
 <td>[allow]</td>
 <td><code class="docutils literal notranslate">v7.4.2 -> v7.4.2</code></td>
 <tr>
 <td>[drop]</td>
 <td><code class="docutils literal notranslate">v7.4.2 -> v7.4.2</code></td>
 <tr>
 <td>[trap-to-host]</td>
 <td><code class="docutils literal notranslate">v7.4.2 -> v7.4.2</code></td>
 </table>
 </div>
 </li>
            <li> <span class="li-head">ipv6_proto_err</span> - Layer 4 invalid protocol anomalies. <span class="li-normal">type: str</span> <span class="li-normal">choices: allow, drop, trap-to-host</span>
 <a id='label88' href="javascript:ContentClick('label89', 'label88');" onmouseover="ContentPreview('label89');" onmouseout="ContentUnpreview('label89');" title="click to collapse or expand..."> more... </a>
 <div id="label89" style="display:none">
 <table border="1">
 <tr>
 <td></td>
 <td colspan="1">Supported Version Ranges</td>
 </tr>
 <tr>
 <td>ipv6_proto_err</td>
 <td><code class="docutils literal notranslate">v7.4.2 -> v7.4.2 </code></td>
 </tr>
 <tr>
 <td>[allow]</td>
 <td><code class="docutils literal notranslate">v7.4.2 -> v7.4.2</code></td>
 <tr>
 <td>[drop]</td>
 <td><code class="docutils literal notranslate">v7.4.2 -> v7.4.2</code></td>
 <tr>
 <td>[trap-to-host]</td>
 <td><code class="docutils literal notranslate">v7.4.2 -> v7.4.2</code></td>
 </table>
 </div>
 </li>
            <li> <span class="li-head">ipv6_saddr_err</span> - Source address as multicast anomalies. <span class="li-normal">type: str</span> <span class="li-normal">choices: allow, drop, trap-to-host</span>
 <a id='label90' href="javascript:ContentClick('label91', 'label90');" onmouseover="ContentPreview('label91');" onmouseout="ContentUnpreview('label91');" title="click to collapse or expand..."> more... </a>
 <div id="label91" style="display:none">
 <table border="1">
 <tr>
 <td></td>
 <td colspan="1">Supported Version Ranges</td>
 </tr>
 <tr>
 <td>ipv6_saddr_err</td>
 <td><code class="docutils literal notranslate">v7.4.2 -> v7.4.2 </code></td>
 </tr>
 <tr>
 <td>[allow]</td>
 <td><code class="docutils literal notranslate">v7.4.2 -> v7.4.2</code></td>
 <tr>
 <td>[drop]</td>
 <td><code class="docutils literal notranslate">v7.4.2 -> v7.4.2</code></td>
 <tr>
 <td>[trap-to-host]</td>
 <td><code class="docutils literal notranslate">v7.4.2 -> v7.4.2</code></td>
 </table>
 </div>
 </li>
            <li> <span class="li-head">ipv6_unknopt</span> - Unknown option anomalies. <span class="li-normal">type: str</span> <span class="li-normal">choices: allow, drop, trap-to-host</span>
 <a id='label92' href="javascript:ContentClick('label93', 'label92');" onmouseover="ContentPreview('label93');" onmouseout="ContentUnpreview('label93');" title="click to collapse or expand..."> more... </a>
 <div id="label93" style="display:none">
 <table border="1">
 <tr>
 <td></td>
 <td colspan="1">Supported Version Ranges</td>
 </tr>
 <tr>
 <td>ipv6_unknopt</td>
 <td><code class="docutils literal notranslate">v7.4.2 -> v7.4.2 </code></td>
 </tr>
 <tr>
 <td>[allow]</td>
 <td><code class="docutils literal notranslate">v7.4.2 -> v7.4.2</code></td>
 <tr>
 <td>[drop]</td>
 <td><code class="docutils literal notranslate">v7.4.2 -> v7.4.2</code></td>
 <tr>
 <td>[trap-to-host]</td>
 <td><code class="docutils literal notranslate">v7.4.2 -> v7.4.2</code></td>
 </table>
 </div>
 </li>
            <li> <span class="li-head">tcp_csum_err</span> - Invalid IPv4 TCP checksum anomalies. <span class="li-normal">type: str</span> <span class="li-normal">choices: drop, trap-to-host</span>
 <a id='label94' href="javascript:ContentClick('label95', 'label94');" onmouseover="ContentPreview('label95');" onmouseout="ContentUnpreview('label95');" title="click to collapse or expand..."> more... </a>
 <div id="label95" style="display:none">
 <table border="1">
 <tr>
 <td></td>
 <td colspan="1">Supported Version Ranges</td>
 </tr>
 <tr>
 <td>tcp_csum_err</td>
 <td><code class="docutils literal notranslate">v7.4.2 -> v7.4.2 </code></td>
 </tr>
 <tr>
 <td>[drop]</td>
 <td><code class="docutils literal notranslate">v7.4.2 -> v7.4.2</code></td>
 <tr>
 <td>[trap-to-host]</td>
 <td><code class="docutils literal notranslate">v7.4.2 -> v7.4.2</code></td>
 </table>
 </div>
 </li>
            <li> <span class="li-head">tcp_fin_noack</span> - TCP SYN flood with FIN flag set without ACK setting anomalies. <span class="li-normal">type: str</span> <span class="li-normal">choices: allow, drop, trap-to-host</span>
 <a id='label96' href="javascript:ContentClick('label97', 'label96');" onmouseover="ContentPreview('label97');" onmouseout="ContentUnpreview('label97');" title="click to collapse or expand..."> more... </a>
 <div id="label97" style="display:none">
 <table border="1">
 <tr>
 <td></td>
 <td colspan="1">Supported Version Ranges</td>
 </tr>
 <tr>
 <td>tcp_fin_noack</td>
 <td><code class="docutils literal notranslate">v7.4.2 -> v7.4.2 </code></td>
 </tr>
 <tr>
 <td>[allow]</td>
 <td><code class="docutils literal notranslate">v7.4.2 -> v7.4.2</code></td>
 <tr>
 <td>[drop]</td>
 <td><code class="docutils literal notranslate">v7.4.2 -> v7.4.2</code></td>
 <tr>
 <td>[trap-to-host]</td>
 <td><code class="docutils literal notranslate">v7.4.2 -> v7.4.2</code></td>
 </table>
 </div>
 </li>
            <li> <span class="li-head">tcp_fin_only</span> - TCP SYN flood with only FIN flag set anomalies. <span class="li-normal">type: str</span> <span class="li-normal">choices: allow, drop, trap-to-host</span>
 <a id='label98' href="javascript:ContentClick('label99', 'label98');" onmouseover="ContentPreview('label99');" onmouseout="ContentUnpreview('label99');" title="click to collapse or expand..."> more... </a>
 <div id="label99" style="display:none">
 <table border="1">
 <tr>
 <td></td>
 <td colspan="1">Supported Version Ranges</td>
 </tr>
 <tr>
 <td>tcp_fin_only</td>
 <td><code class="docutils literal notranslate">v7.4.2 -> v7.4.2 </code></td>
 </tr>
 <tr>
 <td>[allow]</td>
 <td><code class="docutils literal notranslate">v7.4.2 -> v7.4.2</code></td>
 <tr>
 <td>[drop]</td>
 <td><code class="docutils literal notranslate">v7.4.2 -> v7.4.2</code></td>
 <tr>
 <td>[trap-to-host]</td>
 <td><code class="docutils literal notranslate">v7.4.2 -> v7.4.2</code></td>
 </table>
 </div>
 </li>
            <li> <span class="li-head">tcp_land</span> - TCP land anomalies. <span class="li-normal">type: str</span> <span class="li-normal">choices: allow, drop, trap-to-host</span>
 <a id='label100' href="javascript:ContentClick('label101', 'label100');" onmouseover="ContentPreview('label101');" onmouseout="ContentUnpreview('label101');" title="click to collapse or expand..."> more... </a>
 <div id="label101" style="display:none">
 <table border="1">
 <tr>
 <td></td>
 <td colspan="1">Supported Version Ranges</td>
 </tr>
 <tr>
 <td>tcp_land</td>
 <td><code class="docutils literal notranslate">v7.4.2 -> v7.4.2 </code></td>
 </tr>
 <tr>
 <td>[allow]</td>
 <td><code class="docutils literal notranslate">v7.4.2 -> v7.4.2</code></td>
 <tr>
 <td>[drop]</td>
 <td><code class="docutils literal notranslate">v7.4.2 -> v7.4.2</code></td>
 <tr>
 <td>[trap-to-host]</td>
 <td><code class="docutils literal notranslate">v7.4.2 -> v7.4.2</code></td>
 </table>
 </div>
 </li>
            <li> <span class="li-head">tcp_no_flag</span> - TCP SYN flood with no flag set anomalies. <span class="li-normal">type: str</span> <span class="li-normal">choices: allow, drop, trap-to-host</span>
 <a id='label102' href="javascript:ContentClick('label103', 'label102');" onmouseover="ContentPreview('label103');" onmouseout="ContentUnpreview('label103');" title="click to collapse or expand..."> more... </a>
 <div id="label103" style="display:none">
 <table border="1">
 <tr>
 <td></td>
 <td colspan="1">Supported Version Ranges</td>
 </tr>
 <tr>
 <td>tcp_no_flag</td>
 <td><code class="docutils literal notranslate">v7.4.2 -> v7.4.2 </code></td>
 </tr>
 <tr>
 <td>[allow]</td>
 <td><code class="docutils literal notranslate">v7.4.2 -> v7.4.2</code></td>
 <tr>
 <td>[drop]</td>
 <td><code class="docutils literal notranslate">v7.4.2 -> v7.4.2</code></td>
 <tr>
 <td>[trap-to-host]</td>
 <td><code class="docutils literal notranslate">v7.4.2 -> v7.4.2</code></td>
 </table>
 </div>
 </li>
            <li> <span class="li-head">tcp_syn_data</span> - TCP SYN flood packets with data anomalies. <span class="li-normal">type: str</span> <span class="li-normal">choices: allow, drop, trap-to-host</span>
 <a id='label104' href="javascript:ContentClick('label105', 'label104');" onmouseover="ContentPreview('label105');" onmouseout="ContentUnpreview('label105');" title="click to collapse or expand..."> more... </a>
 <div id="label105" style="display:none">
 <table border="1">
 <tr>
 <td></td>
 <td colspan="1">Supported Version Ranges</td>
 </tr>
 <tr>
 <td>tcp_syn_data</td>
 <td><code class="docutils literal notranslate">v7.4.2 -> v7.4.2 </code></td>
 </tr>
 <tr>
 <td>[allow]</td>
 <td><code class="docutils literal notranslate">v7.4.2 -> v7.4.2</code></td>
 <tr>
 <td>[drop]</td>
 <td><code class="docutils literal notranslate">v7.4.2 -> v7.4.2</code></td>
 <tr>
 <td>[trap-to-host]</td>
 <td><code class="docutils literal notranslate">v7.4.2 -> v7.4.2</code></td>
 </table>
 </div>
 </li>
            <li> <span class="li-head">tcp_syn_fin</span> - TCP SYN flood SYN/FIN flag set anomalies. <span class="li-normal">type: str</span> <span class="li-normal">choices: allow, drop, trap-to-host</span>
 <a id='label106' href="javascript:ContentClick('label107', 'label106');" onmouseover="ContentPreview('label107');" onmouseout="ContentUnpreview('label107');" title="click to collapse or expand..."> more... </a>
 <div id="label107" style="display:none">
 <table border="1">
 <tr>
 <td></td>
 <td colspan="1">Supported Version Ranges</td>
 </tr>
 <tr>
 <td>tcp_syn_fin</td>
 <td><code class="docutils literal notranslate">v7.4.2 -> v7.4.2 </code></td>
 </tr>
 <tr>
 <td>[allow]</td>
 <td><code class="docutils literal notranslate">v7.4.2 -> v7.4.2</code></td>
 <tr>
 <td>[drop]</td>
 <td><code class="docutils literal notranslate">v7.4.2 -> v7.4.2</code></td>
 <tr>
 <td>[trap-to-host]</td>
 <td><code class="docutils literal notranslate">v7.4.2 -> v7.4.2</code></td>
 </table>
 </div>
 </li>
            <li> <span class="li-head">tcp_winnuke</span> - TCP WinNuke anomalies. <span class="li-normal">type: str</span> <span class="li-normal">choices: allow, drop, trap-to-host</span>
 <a id='label108' href="javascript:ContentClick('label109', 'label108');" onmouseover="ContentPreview('label109');" onmouseout="ContentUnpreview('label109');" title="click to collapse or expand..."> more... </a>
 <div id="label109" style="display:none">
 <table border="1">
 <tr>
 <td></td>
 <td colspan="1">Supported Version Ranges</td>
 </tr>
 <tr>
 <td>tcp_winnuke</td>
 <td><code class="docutils literal notranslate">v7.4.2 -> v7.4.2 </code></td>
 </tr>
 <tr>
 <td>[allow]</td>
 <td><code class="docutils literal notranslate">v7.4.2 -> v7.4.2</code></td>
 <tr>
 <td>[drop]</td>
 <td><code class="docutils literal notranslate">v7.4.2 -> v7.4.2</code></td>
 <tr>
 <td>[trap-to-host]</td>
 <td><code class="docutils literal notranslate">v7.4.2 -> v7.4.2</code></td>
 </table>
 </div>
 </li>
            <li> <span class="li-head">udp_csum_err</span> - Invalid IPv4 UDP checksum anomalies. <span class="li-normal">type: str</span> <span class="li-normal">choices: drop, trap-to-host</span>
 <a id='label110' href="javascript:ContentClick('label111', 'label110');" onmouseover="ContentPreview('label111');" onmouseout="ContentUnpreview('label111');" title="click to collapse or expand..."> more... </a>
 <div id="label111" style="display:none">
 <table border="1">
 <tr>
 <td></td>
 <td colspan="1">Supported Version Ranges</td>
 </tr>
 <tr>
 <td>udp_csum_err</td>
 <td><code class="docutils literal notranslate">v7.4.2 -> v7.4.2 </code></td>
 </tr>
 <tr>
 <td>[drop]</td>
 <td><code class="docutils literal notranslate">v7.4.2 -> v7.4.2</code></td>
 <tr>
 <td>[trap-to-host]</td>
 <td><code class="docutils literal notranslate">v7.4.2 -> v7.4.2</code></td>
 </table>
 </div>
 </li>
            <li> <span class="li-head">udp_land</span> - UDP land anomalies. <span class="li-normal">type: str</span> <span class="li-normal">choices: allow, drop, trap-to-host</span>
 <a id='label112' href="javascript:ContentClick('label113', 'label112');" onmouseover="ContentPreview('label113');" onmouseout="ContentUnpreview('label113');" title="click to collapse or expand..."> more... </a>
 <div id="label113" style="display:none">
 <table border="1">
 <tr>
 <td></td>
 <td colspan="1">Supported Version Ranges</td>
 </tr>
 <tr>
 <td>udp_land</td>
 <td><code class="docutils literal notranslate">v7.4.2 -> v7.4.2 </code></td>
 </tr>
 <tr>
 <td>[allow]</td>
 <td><code class="docutils literal notranslate">v7.4.2 -> v7.4.2</code></td>
 <tr>
 <td>[drop]</td>
 <td><code class="docutils literal notranslate">v7.4.2 -> v7.4.2</code></td>
 <tr>
 <td>[trap-to-host]</td>
 <td><code class="docutils literal notranslate">v7.4.2 -> v7.4.2</code></td>
 </table>
 </div>
 </li>
            </ul>
        <li> <span class="li-head">gtp_enhanced_cpu_range</span> - GTP enhanced CPU range option. <span class="li-normal">type: str</span> <span class="li-normal">choices: 0, 1, 2</span>
 <a id='label114' href="javascript:ContentClick('label115', 'label114');" onmouseover="ContentPreview('label115');" onmouseout="ContentUnpreview('label115');" title="click to collapse or expand..."> more... </a>
 <div id="label115" style="display:none">
 <table border="1">
 <tr>
 <td></td>
 <td colspan="2">Supported Version Ranges</td>
 </tr>
 <tr>
 <td>gtp_enhanced_cpu_range</td>
 <td><code class="docutils literal notranslate">v6.0.0 -> v7.4.1 </code></td>
 <td><code class="docutils literal notranslate">v7.4.3 -> 7.6.4 </code></td>
 </tr>
 <tr>
 <td>[0]</td>
 <td><code class="docutils literal notranslate">v6.0.0 -> v7.4.1</code></td>
 <tr>
 <td>[1]</td>
 <td><code class="docutils literal notranslate">v6.0.0 -> v7.4.1</code></td>
 <tr>
 <td>[2]</td>
 <td><code class="docutils literal notranslate">v6.0.0 -> v7.4.1</code></td>
 </table>
 </div>
 </li>
        <li> <span class="li-head">gtp_enhanced_mode</span> - Enable/disable GTP enhanced mode. <span class="li-normal">type: str</span> <span class="li-normal">choices: enable, disable</span>
 <a id='label116' href="javascript:ContentClick('label117', 'label116');" onmouseover="ContentPreview('label117');" onmouseout="ContentUnpreview('label117');" title="click to collapse or expand..."> more... </a>
 <div id="label117" style="display:none">
 <table border="1">
 <tr>
 <td></td>
 <td colspan="1">Supported Version Ranges</td>
 </tr>
 <tr>
 <td>gtp_enhanced_mode</td>
 <td><code class="docutils literal notranslate">v6.0.0 -> 7.6.4 </code></td>
 </tr>
 <tr>
 <td>[enable]</td>
 <td><code class="docutils literal notranslate">v6.0.0 -> 7.6.4</code></td>
 <tr>
 <td>[disable]</td>
 <td><code class="docutils literal notranslate">v6.0.0 -> 7.6.4</code></td>
 </table>
 </div>
 </li>
        <li> <span class="li-head">gtp_support</span> - Enable/Disable NP7 GTP support <span class="li-normal">type: str</span> <span class="li-normal">choices: enable, disable</span>
 <a id='label118' href="javascript:ContentClick('label119', 'label118');" onmouseover="ContentPreview('label119');" onmouseout="ContentUnpreview('label119');" title="click to collapse or expand..."> more... </a>
 <div id="label119" style="display:none">
 <table border="1">
 <tr>
 <td></td>
 <td colspan="1">Supported Version Ranges</td>
 </tr>
 <tr>
 <td>gtp_support</td>
 <td><code class="docutils literal notranslate">v7.4.2 -> v7.4.2 </code></td>
 </tr>
 <tr>
 <td>[enable]</td>
 <td><code class="docutils literal notranslate">v7.4.2 -> v7.4.2</code></td>
 <tr>
 <td>[disable]</td>
 <td><code class="docutils literal notranslate">v7.4.2 -> v7.4.2</code></td>
 </table>
 </div>
 </li>
        <li> <span class="li-head">hash_tbl_spread</span> - Enable/disable hash table entry spread . <span class="li-normal">type: str</span> <span class="li-normal">choices: enable, disable</span>
 <a id='label120' href="javascript:ContentClick('label121', 'label120');" onmouseover="ContentPreview('label121');" onmouseout="ContentUnpreview('label121');" title="click to collapse or expand..."> more... </a>
 <div id="label121" style="display:none">
 <table border="1">
 <tr>
 <td></td>
 <td colspan="1">Supported Version Ranges</td>
 </tr>
 <tr>
 <td>hash_tbl_spread</td>
 <td><code class="docutils literal notranslate">v7.4.2 -> v7.4.2 </code></td>
 </tr>
 <tr>
 <td>[enable]</td>
 <td><code class="docutils literal notranslate">v7.4.2 -> v7.4.2</code></td>
 <tr>
 <td>[disable]</td>
 <td><code class="docutils literal notranslate">v7.4.2 -> v7.4.2</code></td>
 </table>
 </div>
 </li>
        <li> <span class="li-head">hpe</span> - Host protection engine configuration. <span class="li-normal">type: dict</span>
 <a id='label122' href="javascript:ContentClick('label123', 'label122');" onmouseover="ContentPreview('label123');" onmouseout="ContentUnpreview('label123');" title="click to collapse or expand..."> more... </a>
 <div id="label123" style="display:none">
 <table border="1">
 <tr>
 <td></td><td colspan="1">Supported Version Ranges</td>
 </tr>
 <tr>
 <td>hpe</td>
 <td><code class="docutils literal notranslate">v7.4.2 -> v7.4.2 </code></td>
 </tr>
 </table>
 </div>
 </li>
            <ul class="ul-self">
            <li> <span class="li-head">all_protocol</span> - Maximum packet rate of each host queue except high priority traffic(1K - 32M pps), set 0 to disable. <span class="li-normal">type: int</span>
 <a id='label124' href="javascript:ContentClick('label125', 'label124');" onmouseover="ContentPreview('label125');" onmouseout="ContentUnpreview('label125');" title="click to collapse or expand..."> more... </a>
 <div id="label125" style="display:none">
 <table border="1">
 <tr>
 <td></td>
 <td colspan="1">Supported Version Ranges</td>
 </tr>
 <tr>
 <td>all_protocol</td>
 <td><code class="docutils literal notranslate">v7.4.2 -> v7.4.2 </code></td>
 </tr>
 </table>
 </div>
 </li>
            <li> <span class="li-head">arp_max</span> - Maximum ARP packet rate (1K - 32M pps). Entry is valid when ARP is removed from high-priority traffic. <span class="li-normal">type: int</span>
 <a id='label126' href="javascript:ContentClick('label127', 'label126');" onmouseover="ContentPreview('label127');" onmouseout="ContentUnpreview('label127');" title="click to collapse or expand..."> more... </a>
 <div id="label127" style="display:none">
 <table border="1">
 <tr>
 <td></td>
 <td colspan="1">Supported Version Ranges</td>
 </tr>
 <tr>
 <td>arp_max</td>
 <td><code class="docutils literal notranslate">v7.4.2 -> v7.4.2 </code></td>
 </tr>
 </table>
 </div>
 </li>
            <li> <span class="li-head">enable_shaper</span> - Enable/Disable NPU Host Protection Engine (HPE) for packet type shaper. <span class="li-normal">type: str</span> <span class="li-normal">choices: disable, enable</span>
 <a id='label128' href="javascript:ContentClick('label129', 'label128');" onmouseover="ContentPreview('label129');" onmouseout="ContentUnpreview('label129');" title="click to collapse or expand..."> more... </a>
 <div id="label129" style="display:none">
 <table border="1">
 <tr>
 <td></td>
 <td colspan="1">Supported Version Ranges</td>
 </tr>
 <tr>
 <td>enable_shaper</td>
 <td><code class="docutils literal notranslate">v7.4.2 -> v7.4.2 </code></td>
 </tr>
 <tr>
 <td>[disable]</td>
 <td><code class="docutils literal notranslate">v7.4.2 -> v7.4.2</code></td>
 <tr>
 <td>[enable]</td>
 <td><code class="docutils literal notranslate">v7.4.2 -> v7.4.2</code></td>
 </table>
 </div>
 </li>
            <li> <span class="li-head">esp_max</span> - Maximum ESP packet rate (1K - 32M pps). <span class="li-normal">type: int</span>
 <a id='label130' href="javascript:ContentClick('label131', 'label130');" onmouseover="ContentPreview('label131');" onmouseout="ContentUnpreview('label131');" title="click to collapse or expand..."> more... </a>
 <div id="label131" style="display:none">
 <table border="1">
 <tr>
 <td></td>
 <td colspan="1">Supported Version Ranges</td>
 </tr>
 <tr>
 <td>esp_max</td>
 <td><code class="docutils literal notranslate">v7.4.2 -> v7.4.2 </code></td>
 </tr>
 </table>
 </div>
 </li>
            <li> <span class="li-head">high_priority</span> - Maximum packet rate for high priority traffic packets (1K - 32M pps). <span class="li-normal">type: int</span>
 <a id='label132' href="javascript:ContentClick('label133', 'label132');" onmouseover="ContentPreview('label133');" onmouseout="ContentUnpreview('label133');" title="click to collapse or expand..."> more... </a>
 <div id="label133" style="display:none">
 <table border="1">
 <tr>
 <td></td>
 <td colspan="1">Supported Version Ranges</td>
 </tr>
 <tr>
 <td>high_priority</td>
 <td><code class="docutils literal notranslate">v7.4.2 -> v7.4.2 </code></td>
 </tr>
 </table>
 </div>
 </li>
            <li> <span class="li-head">icmp_max</span> - Maximum ICMP packet rate (1K - 32M pps). <span class="li-normal">type: int</span>
 <a id='label134' href="javascript:ContentClick('label135', 'label134');" onmouseover="ContentPreview('label135');" onmouseout="ContentUnpreview('label135');" title="click to collapse or expand..."> more... </a>
 <div id="label135" style="display:none">
 <table border="1">
 <tr>
 <td></td>
 <td colspan="1">Supported Version Ranges</td>
 </tr>
 <tr>
 <td>icmp_max</td>
 <td><code class="docutils literal notranslate">v7.4.2 -> v7.4.2 </code></td>
 </tr>
 </table>
 </div>
 </li>
            <li> <span class="li-head">ip_frag_max</span> - Maximum fragmented IP packet rate (1K - 32M pps). <span class="li-normal">type: int</span>
 <a id='label136' href="javascript:ContentClick('label137', 'label136');" onmouseover="ContentPreview('label137');" onmouseout="ContentUnpreview('label137');" title="click to collapse or expand..."> more... </a>
 <div id="label137" style="display:none">
 <table border="1">
 <tr>
 <td></td>
 <td colspan="1">Supported Version Ranges</td>
 </tr>
 <tr>
 <td>ip_frag_max</td>
 <td><code class="docutils literal notranslate">v7.4.2 -> v7.4.2 </code></td>
 </tr>
 </table>
 </div>
 </li>
            <li> <span class="li-head">ip_others_max</span> - Maximum IP packet rate for other packets (packet types that cannot be set with other options) (1K - 32G pps). <span class="li-normal">type: int</span>
 <a id='label138' href="javascript:ContentClick('label139', 'label138');" onmouseover="ContentPreview('label139');" onmouseout="ContentUnpreview('label139');" title="click to collapse or expand..."> more... </a>
 <div id="label139" style="display:none">
 <table border="1">
 <tr>
 <td></td>
 <td colspan="1">Supported Version Ranges</td>
 </tr>
 <tr>
 <td>ip_others_max</td>
 <td><code class="docutils literal notranslate">v7.4.2 -> v7.4.2 </code></td>
 </tr>
 </table>
 </div>
 </li>
            <li> <span class="li-head">l2_others_max</span> - Maximum L2 packet rate for L2 packets that are not ARP packets (1K - 32M pps). <span class="li-normal">type: int</span>
 <a id='label140' href="javascript:ContentClick('label141', 'label140');" onmouseover="ContentPreview('label141');" onmouseout="ContentUnpreview('label141');" title="click to collapse or expand..."> more... </a>
 <div id="label141" style="display:none">
 <table border="1">
 <tr>
 <td></td>
 <td colspan="1">Supported Version Ranges</td>
 </tr>
 <tr>
 <td>l2_others_max</td>
 <td><code class="docutils literal notranslate">v7.4.2 -> v7.4.2 </code></td>
 </tr>
 </table>
 </div>
 </li>
            <li> <span class="li-head">sctp_max</span> - Maximum SCTP packet rate (1K - 32M pps). <span class="li-normal">type: int</span>
 <a id='label142' href="javascript:ContentClick('label143', 'label142');" onmouseover="ContentPreview('label143');" onmouseout="ContentUnpreview('label143');" title="click to collapse or expand..."> more... </a>
 <div id="label143" style="display:none">
 <table border="1">
 <tr>
 <td></td>
 <td colspan="1">Supported Version Ranges</td>
 </tr>
 <tr>
 <td>sctp_max</td>
 <td><code class="docutils literal notranslate">v7.4.2 -> v7.4.2 </code></td>
 </tr>
 </table>
 </div>
 </li>
            <li> <span class="li-head">tcp_max</span> - Maximum TCP packet rate (1K - 32M pps). <span class="li-normal">type: int</span>
 <a id='label144' href="javascript:ContentClick('label145', 'label144');" onmouseover="ContentPreview('label145');" onmouseout="ContentUnpreview('label145');" title="click to collapse or expand..."> more... </a>
 <div id="label145" style="display:none">
 <table border="1">
 <tr>
 <td></td>
 <td colspan="1">Supported Version Ranges</td>
 </tr>
 <tr>
 <td>tcp_max</td>
 <td><code class="docutils literal notranslate">v7.4.2 -> v7.4.2 </code></td>
 </tr>
 </table>
 </div>
 </li>
            <li> <span class="li-head">tcpfin_rst_max</span> - Maximum TCP carries FIN or RST flags packet rate (1K - 32M pps). <span class="li-normal">type: int</span>
 <a id='label146' href="javascript:ContentClick('label147', 'label146');" onmouseover="ContentPreview('label147');" onmouseout="ContentUnpreview('label147');" title="click to collapse or expand..."> more... </a>
 <div id="label147" style="display:none">
 <table border="1">
 <tr>
 <td></td>
 <td colspan="1">Supported Version Ranges</td>
 </tr>
 <tr>
 <td>tcpfin_rst_max</td>
 <td><code class="docutils literal notranslate">v7.4.2 -> v7.4.2 </code></td>
 </tr>
 </table>
 </div>
 </li>
            <li> <span class="li-head">tcpsyn_ack_max</span> - Maximum TCP carries SYN and ACK flags packet rate (1K - 32M pps). <span class="li-normal">type: int</span>
 <a id='label148' href="javascript:ContentClick('label149', 'label148');" onmouseover="ContentPreview('label149');" onmouseout="ContentUnpreview('label149');" title="click to collapse or expand..."> more... </a>
 <div id="label149" style="display:none">
 <table border="1">
 <tr>
 <td></td>
 <td colspan="1">Supported Version Ranges</td>
 </tr>
 <tr>
 <td>tcpsyn_ack_max</td>
 <td><code class="docutils literal notranslate">v7.4.2 -> v7.4.2 </code></td>
 </tr>
 </table>
 </div>
 </li>
            <li> <span class="li-head">tcpsyn_max</span> - Maximum TCP SYN packet rate (1K - 40M pps). <span class="li-normal">type: int</span>
 <a id='label150' href="javascript:ContentClick('label151', 'label150');" onmouseover="ContentPreview('label151');" onmouseout="ContentUnpreview('label151');" title="click to collapse or expand..."> more... </a>
 <div id="label151" style="display:none">
 <table border="1">
 <tr>
 <td></td>
 <td colspan="1">Supported Version Ranges</td>
 </tr>
 <tr>
 <td>tcpsyn_max</td>
 <td><code class="docutils literal notranslate">v7.4.2 -> v7.4.2 </code></td>
 </tr>
 </table>
 </div>
 </li>
            <li> <span class="li-head">udp_max</span> - Maximum UDP packet rate (1K - 32M pps). <span class="li-normal">type: int</span>
 <a id='label152' href="javascript:ContentClick('label153', 'label152');" onmouseover="ContentPreview('label153');" onmouseout="ContentUnpreview('label153');" title="click to collapse or expand..."> more... </a>
 <div id="label153" style="display:none">
 <table border="1">
 <tr>
 <td></td>
 <td colspan="1">Supported Version Ranges</td>
 </tr>
 <tr>
 <td>udp_max</td>
 <td><code class="docutils literal notranslate">v7.4.2 -> v7.4.2 </code></td>
 </tr>
 </table>
 </div>
 </li>
            </ul>
        <li> <span class="li-head">htab_dedi_queue_nr</span> - Set the number of dedicate queue for hash table messages. <span class="li-normal">type: int</span>
 <a id='label154' href="javascript:ContentClick('label155', 'label154');" onmouseover="ContentPreview('label155');" onmouseout="ContentUnpreview('label155');" title="click to collapse or expand..."> more... </a>
 <div id="label155" style="display:none">
 <table border="1">
 <tr>
 <td></td>
 <td colspan="1">Supported Version Ranges</td>
 </tr>
 <tr>
 <td>htab_dedi_queue_nr</td>
 <td><code class="docutils literal notranslate">v7.4.2 -> v7.4.2 </code></td>
 </tr>
 </table>
 </div>
 </li>
        <li> <span class="li-head">htab_msg_queue</span> - Set hash table message queue mode. <span class="li-normal">type: str</span> <span class="li-normal">choices: data, idle, dedicated</span>
 <a id='label156' href="javascript:ContentClick('label157', 'label156');" onmouseover="ContentPreview('label157');" onmouseout="ContentUnpreview('label157');" title="click to collapse or expand..."> more... </a>
 <div id="label157" style="display:none">
 <table border="1">
 <tr>
 <td></td>
 <td colspan="1">Supported Version Ranges</td>
 </tr>
 <tr>
 <td>htab_msg_queue</td>
 <td><code class="docutils literal notranslate">v7.4.2 -> v7.4.2 </code></td>
 </tr>
 <tr>
 <td>[data]</td>
 <td><code class="docutils literal notranslate">v7.4.2 -> v7.4.2</code></td>
 <tr>
 <td>[idle]</td>
 <td><code class="docutils literal notranslate">v7.4.2 -> v7.4.2</code></td>
 <tr>
 <td>[dedicated]</td>
 <td><code class="docutils literal notranslate">v7.4.2 -> v7.4.2</code></td>
 </table>
 </div>
 </li>
        <li> <span class="li-head">htx_icmp_csum_chk</span> - Set HTX icmp csum checking mode. <span class="li-normal">type: str</span> <span class="li-normal">choices: drop, pass</span>
 <a id='label158' href="javascript:ContentClick('label159', 'label158');" onmouseover="ContentPreview('label159');" onmouseout="ContentUnpreview('label159');" title="click to collapse or expand..."> more... </a>
 <div id="label159" style="display:none">
 <table border="1">
 <tr>
 <td></td>
 <td colspan="1">Supported Version Ranges</td>
 </tr>
 <tr>
 <td>htx_icmp_csum_chk</td>
 <td><code class="docutils literal notranslate">v7.4.2 -> v7.4.2 </code></td>
 </tr>
 <tr>
 <td>[drop]</td>
 <td><code class="docutils literal notranslate">v7.4.2 -> v7.4.2</code></td>
 <tr>
 <td>[pass]</td>
 <td><code class="docutils literal notranslate">v7.4.2 -> v7.4.2</code></td>
 </table>
 </div>
 </li>
        <li> <span class="li-head">inbound_dscp_copy_port</span> - Physical interfaces that support inbound-dscp-copy. <span class="li-normal">type: list</span> <span style="font-family:'Courier New'" class="li-required">member_path: inbound_dscp_copy_port:interface</span>
 <a id='label160' href="javascript:ContentClick('label161', 'label160');" onmouseover="ContentPreview('label161');" onmouseout="ContentUnpreview('label161');" title="click to collapse or expand..."> more... </a>
 <div id="label161" style="display:none">
 <table border="1">
 <tr>
 <td></td><td colspan="1">Supported Version Ranges</td>
 </tr>
 <tr>
 <td>inbound_dscp_copy_port</td>
 <td><code class="docutils literal notranslate">v7.4.2 -> v7.4.2 </code></td>
 </tr>
 </table>
 </div>
 </li>
            <ul class="ul-self">
            <li> <span class="li-head">interface</span> - Physical interface name. <span class="li-normal">type: str</span> <span class="li-required">required: true</span>
 <a id='label162' href="javascript:ContentClick('label163', 'label162');" onmouseover="ContentPreview('label163');" onmouseout="ContentUnpreview('label163');" title="click to collapse or expand..."> more... </a>
 <div id="label163" style="display:none">
 <table border="1">
 <tr>
 <td></td>
 <td colspan="1">Supported Version Ranges</td>
 </tr>
 <tr>
 <td>interface</td>
 <td><code class="docutils literal notranslate">v7.4.2 -> v7.4.2 </code></td>
 </tr>
 </table>
 </div>
 </li>
            </ul>
        <li> <span class="li-head">intf_shaping_offload</span> - Enable/disable NPU offload when doing interface-based traffic shaping according to the egress-shaping-profile. <span class="li-normal">type: str</span> <span class="li-normal">choices: enable, disable</span>
 <a id='label164' href="javascript:ContentClick('label165', 'label164');" onmouseover="ContentPreview('label165');" onmouseout="ContentUnpreview('label165');" title="click to collapse or expand..."> more... </a>
 <div id="label165" style="display:none">
 <table border="1">
 <tr>
 <td></td>
 <td colspan="2">Supported Version Ranges</td>
 </tr>
 <tr>
 <td>intf_shaping_offload</td>
 <td><code class="docutils literal notranslate">v6.4.0 -> v7.4.1 </code></td>
 <td><code class="docutils literal notranslate">v7.4.3 -> 7.6.4 </code></td>
 </tr>
 <tr>
 <td>[enable]</td>
 <td><code class="docutils literal notranslate">v6.4.0 -> v7.4.1</code></td>
 <tr>
 <td>[disable]</td>
 <td><code class="docutils literal notranslate">v6.4.0 -> v7.4.1</code></td>
 </table>
 </div>
 </li>
        <li> <span class="li-head">ip_fragment_offload</span> - Enable/disable NP7 NPU IP fragment offload. <span class="li-normal">type: str</span> <span class="li-normal">choices: disable, enable</span>
 <a id='label166' href="javascript:ContentClick('label167', 'label166');" onmouseover="ContentPreview('label167');" onmouseout="ContentUnpreview('label167');" title="click to collapse or expand..."> more... </a>
 <div id="label167" style="display:none">
 <table border="1">
 <tr>
 <td></td>
 <td colspan="1">Supported Version Ranges</td>
 </tr>
 <tr>
 <td>ip_fragment_offload</td>
 <td><code class="docutils literal notranslate">v7.4.2 -> v7.4.2 </code></td>
 </tr>
 <tr>
 <td>[disable]</td>
 <td><code class="docutils literal notranslate">v7.4.2 -> v7.4.2</code></td>
 <tr>
 <td>[enable]</td>
 <td><code class="docutils literal notranslate">v7.4.2 -> v7.4.2</code></td>
 </table>
 </div>
 </li>
        <li> <span class="li-head">ip_reassembly</span> - IP reassebmly engine configuration. <span class="li-normal">type: dict</span>
 <a id='label168' href="javascript:ContentClick('label169', 'label168');" onmouseover="ContentPreview('label169');" onmouseout="ContentUnpreview('label169');" title="click to collapse or expand..."> more... </a>
 <div id="label169" style="display:none">
 <table border="1">
 <tr>
 <td></td><td colspan="1">Supported Version Ranges</td>
 </tr>
 <tr>
 <td>ip_reassembly</td>
 <td><code class="docutils literal notranslate">v7.4.2 -> v7.4.2 </code></td>
 </tr>
 </table>
 </div>
 </li>
            <ul class="ul-self">
            <li> <span class="li-head">max_timeout</span> - Maximum timeout value for IP reassembly (5 us - 600,000,000 us). <span class="li-normal">type: int</span>
 <a id='label170' href="javascript:ContentClick('label171', 'label170');" onmouseover="ContentPreview('label171');" onmouseout="ContentUnpreview('label171');" title="click to collapse or expand..."> more... </a>
 <div id="label171" style="display:none">
 <table border="1">
 <tr>
 <td></td>
 <td colspan="1">Supported Version Ranges</td>
 </tr>
 <tr>
 <td>max_timeout</td>
 <td><code class="docutils literal notranslate">v7.4.2 -> v7.4.2 </code></td>
 </tr>
 </table>
 </div>
 </li>
            <li> <span class="li-head">min_timeout</span> - Minimum timeout value for IP reassembly (5 us - 600,000,000 us). <span class="li-normal">type: int</span>
 <a id='label172' href="javascript:ContentClick('label173', 'label172');" onmouseover="ContentPreview('label173');" onmouseout="ContentUnpreview('label173');" title="click to collapse or expand..."> more... </a>
 <div id="label173" style="display:none">
 <table border="1">
 <tr>
 <td></td>
 <td colspan="1">Supported Version Ranges</td>
 </tr>
 <tr>
 <td>min_timeout</td>
 <td><code class="docutils literal notranslate">v7.4.2 -> v7.4.2 </code></td>
 </tr>
 </table>
 </div>
 </li>
            <li> <span class="li-head">status</span> - Set IP reassembly processing status. <span class="li-normal">type: str</span> <span class="li-normal">choices: disable, enable</span>
 <a id='label174' href="javascript:ContentClick('label175', 'label174');" onmouseover="ContentPreview('label175');" onmouseout="ContentUnpreview('label175');" title="click to collapse or expand..."> more... </a>
 <div id="label175" style="display:none">
 <table border="1">
 <tr>
 <td></td>
 <td colspan="1">Supported Version Ranges</td>
 </tr>
 <tr>
 <td>status</td>
 <td><code class="docutils literal notranslate">v7.4.2 -> v7.4.2 </code></td>
 </tr>
 <tr>
 <td>[disable]</td>
 <td><code class="docutils literal notranslate">v7.4.2 -> v7.4.2</code></td>
 <tr>
 <td>[enable]</td>
 <td><code class="docutils literal notranslate">v7.4.2 -> v7.4.2</code></td>
 </table>
 </div>
 </li>
            </ul>
        <li> <span class="li-head">ipsec_dec_subengine_mask</span> - IPsec decryption subengine mask (0x1 - 0xff). <span class="li-normal">type: str</span>
 <a id='label176' href="javascript:ContentClick('label177', 'label176');" onmouseover="ContentPreview('label177');" onmouseout="ContentUnpreview('label177');" title="click to collapse or expand..."> more... </a>
 <div id="label177" style="display:none">
 <table border="1">
 <tr>
 <td></td>
 <td colspan="2">Supported Version Ranges</td>
 </tr>
 <tr>
 <td>ipsec_dec_subengine_mask</td>
 <td><code class="docutils literal notranslate">v6.0.0 -> v7.4.1 </code></td>
 <td><code class="docutils literal notranslate">v7.4.3 -> 7.6.4 </code></td>
 </tr>
 </table>
 </div>
 </li>
        <li> <span class="li-head">ipsec_enc_subengine_mask</span> - IPsec encryption subengine mask (0x1 - 0xff). <span class="li-normal">type: str</span>
 <a id='label178' href="javascript:ContentClick('label179', 'label178');" onmouseover="ContentPreview('label179');" onmouseout="ContentUnpreview('label179');" title="click to collapse or expand..."> more... </a>
 <div id="label179" style="display:none">
 <table border="1">
 <tr>
 <td></td>
 <td colspan="2">Supported Version Ranges</td>
 </tr>
 <tr>
 <td>ipsec_enc_subengine_mask</td>
 <td><code class="docutils literal notranslate">v6.0.0 -> v7.4.1 </code></td>
 <td><code class="docutils literal notranslate">v7.4.3 -> 7.6.4 </code></td>
 </tr>
 </table>
 </div>
 </li>
        <li> <span class="li-head">ipsec_inbound_cache</span> - Enable/disable IPsec inbound cache for anti-replay. <span class="li-normal">type: str</span> <span class="li-normal">choices: enable, disable</span>
 <a id='label180' href="javascript:ContentClick('label181', 'label180');" onmouseover="ContentPreview('label181');" onmouseout="ContentUnpreview('label181');" title="click to collapse or expand..."> more... </a>
 <div id="label181" style="display:none">
 <table border="1">
 <tr>
 <td></td>
 <td colspan="2">Supported Version Ranges</td>
 </tr>
 <tr>
 <td>ipsec_inbound_cache</td>
 <td><code class="docutils literal notranslate">v6.2.0 -> v7.4.1 </code></td>
 <td><code class="docutils literal notranslate">v7.4.3 -> 7.6.4 </code></td>
 </tr>
 <tr>
 <td>[enable]</td>
 <td><code class="docutils literal notranslate">v6.2.0 -> v7.4.1</code></td>
 <tr>
 <td>[disable]</td>
 <td><code class="docutils literal notranslate">v6.2.0 -> v7.4.1</code></td>
 </table>
 </div>
 </li>
        <li> <span class="li-head">ipsec_mtu_override</span> - Enable/disable NP6 IPsec MTU override. <span class="li-normal">type: str</span> <span class="li-normal">choices: disable, enable</span>
 <a id='label182' href="javascript:ContentClick('label183', 'label182');" onmouseover="ContentPreview('label183');" onmouseout="ContentUnpreview('label183');" title="click to collapse or expand..."> more... </a>
 <div id="label183" style="display:none">
 <table border="1">
 <tr>
 <td></td>
 <td colspan="4">Supported Version Ranges</td>
 </tr>
 <tr>
 <td>ipsec_mtu_override</td>
 <td><code class="docutils literal notranslate">v6.2.0 -> v6.2.0 </code></td>
 <td><code class="docutils literal notranslate">v6.2.7 -> v6.2.7 </code></td>
 <td><code class="docutils literal notranslate">v6.4.4 -> v7.4.1 </code></td>
 <td><code class="docutils literal notranslate">v7.4.3 -> 7.6.4 </code></td>
 </tr>
 <tr>
 <td>[disable]</td>
 <td><code class="docutils literal notranslate">v6.2.0 -> v6.2.0</code></td>
 <tr>
 <td>[enable]</td>
 <td><code class="docutils literal notranslate">v6.2.0 -> v6.2.0</code></td>
 </table>
 </div>
 </li>
        <li> <span class="li-head">ipsec_ob_np_sel</span> - IPsec NP selection for OB SA offloading. <span class="li-normal">type: str</span> <span class="li-normal">choices: rr, Packet, Hash</span>
 <a id='label184' href="javascript:ContentClick('label185', 'label184');" onmouseover="ContentPreview('label185');" onmouseout="ContentUnpreview('label185');" title="click to collapse or expand..."> more... </a>
 <div id="label185" style="display:none">
 <table border="1">
 <tr>
 <td></td>
 <td colspan="1">Supported Version Ranges</td>
 </tr>
 <tr>
 <td>ipsec_ob_np_sel</td>
 <td><code class="docutils literal notranslate">v7.4.2 -> v7.4.2 </code></td>
 </tr>
 <tr>
 <td>[rr]</td>
 <td><code class="docutils literal notranslate">v7.4.2 -> v7.4.2</code></td>
 <tr>
 <td>[Packet]</td>
 <td><code class="docutils literal notranslate">v7.4.2 -> v7.4.2</code></td>
 <tr>
 <td>[Hash]</td>
 <td><code class="docutils literal notranslate">v7.4.2 -> v7.4.2</code></td>
 </table>
 </div>
 </li>
        <li> <span class="li-head">ipsec_over_vlink</span> - Enable/disable IPsec over vlink. <span class="li-normal">type: str</span> <span class="li-normal">choices: enable, disable</span>
 <a id='label186' href="javascript:ContentClick('label187', 'label186');" onmouseover="ContentPreview('label187');" onmouseout="ContentUnpreview('label187');" title="click to collapse or expand..."> more... </a>
 <div id="label187" style="display:none">
 <table border="1">
 <tr>
 <td></td>
 <td colspan="2">Supported Version Ranges</td>
 </tr>
 <tr>
 <td>ipsec_over_vlink</td>
 <td><code class="docutils literal notranslate">v6.0.0 -> v7.4.1 </code></td>
 <td><code class="docutils literal notranslate">v7.4.3 -> 7.6.4 </code></td>
 </tr>
 <tr>
 <td>[enable]</td>
 <td><code class="docutils literal notranslate">v6.0.0 -> v7.4.1</code></td>
 <tr>
 <td>[disable]</td>
 <td><code class="docutils literal notranslate">v6.0.0 -> v7.4.1</code></td>
 </table>
 </div>
 </li>
        <li> <span class="li-head">isf_np_queues</span> - Configure queues of switch port connected to NP6 XAUI on ingress path. <span class="li-normal">type: dict</span>
 <a id='label188' href="javascript:ContentClick('label189', 'label188');" onmouseover="ContentPreview('label189');" onmouseout="ContentUnpreview('label189');" title="click to collapse or expand..."> more... </a>
 <div id="label189" style="display:none">
 <table border="1">
 <tr>
 <td></td><td colspan="4">Supported Version Ranges</td>
 </tr>
 <tr>
 <td>isf_np_queues</td>
 <td><code class="docutils literal notranslate">v6.4.0 -> v6.4.0 </code></td>
 <td><code class="docutils literal notranslate">v7.2.0 -> v7.2.0 </code></td>
 <td><code class="docutils literal notranslate">v7.4.0 -> v7.4.1 </code></td>
 <td><code class="docutils literal notranslate">v7.4.3 -> 7.6.4 </code></td>
 </tr>
 </table>
 </div>
 </li>
            <ul class="ul-self">
            <li> <span class="li-head">cos0</span> - CoS profile name for CoS 0. Source system.isf-queue-profile.name. <span class="li-normal">type: str</span>
 <a id='label190' href="javascript:ContentClick('label191', 'label190');" onmouseover="ContentPreview('label191');" onmouseout="ContentUnpreview('label191');" title="click to collapse or expand..."> more... </a>
 <div id="label191" style="display:none">
 <table border="1">
 <tr>
 <td></td>
 <td colspan="4">Supported Version Ranges</td>
 </tr>
 <tr>
 <td>cos0</td>
 <td><code class="docutils literal notranslate">v6.4.0 -> v6.4.0 </code></td>
 <td><code class="docutils literal notranslate">v7.2.0 -> v7.2.0 </code></td>
 <td><code class="docutils literal notranslate">v7.4.0 -> v7.4.1 </code></td>
 <td><code class="docutils literal notranslate">v7.4.3 -> 7.6.4 </code></td>
 </tr>
 </table>
 </div>
 </li>
            <li> <span class="li-head">cos1</span> - CoS profile name for CoS 1. Source system.isf-queue-profile.name. <span class="li-normal">type: str</span>
 <a id='label192' href="javascript:ContentClick('label193', 'label192');" onmouseover="ContentPreview('label193');" onmouseout="ContentUnpreview('label193');" title="click to collapse or expand..."> more... </a>
 <div id="label193" style="display:none">
 <table border="1">
 <tr>
 <td></td>
 <td colspan="4">Supported Version Ranges</td>
 </tr>
 <tr>
 <td>cos1</td>
 <td><code class="docutils literal notranslate">v6.4.0 -> v6.4.0 </code></td>
 <td><code class="docutils literal notranslate">v7.2.0 -> v7.2.0 </code></td>
 <td><code class="docutils literal notranslate">v7.4.0 -> v7.4.1 </code></td>
 <td><code class="docutils literal notranslate">v7.4.3 -> 7.6.4 </code></td>
 </tr>
 </table>
 </div>
 </li>
            <li> <span class="li-head">cos2</span> - CoS profile name for CoS 2. Source system.isf-queue-profile.name. <span class="li-normal">type: str</span>
 <a id='label194' href="javascript:ContentClick('label195', 'label194');" onmouseover="ContentPreview('label195');" onmouseout="ContentUnpreview('label195');" title="click to collapse or expand..."> more... </a>
 <div id="label195" style="display:none">
 <table border="1">
 <tr>
 <td></td>
 <td colspan="4">Supported Version Ranges</td>
 </tr>
 <tr>
 <td>cos2</td>
 <td><code class="docutils literal notranslate">v6.4.0 -> v6.4.0 </code></td>
 <td><code class="docutils literal notranslate">v7.2.0 -> v7.2.0 </code></td>
 <td><code class="docutils literal notranslate">v7.4.0 -> v7.4.1 </code></td>
 <td><code class="docutils literal notranslate">v7.4.3 -> 7.6.4 </code></td>
 </tr>
 </table>
 </div>
 </li>
            <li> <span class="li-head">cos3</span> - CoS profile name for CoS 3. Source system.isf-queue-profile.name. <span class="li-normal">type: str</span>
 <a id='label196' href="javascript:ContentClick('label197', 'label196');" onmouseover="ContentPreview('label197');" onmouseout="ContentUnpreview('label197');" title="click to collapse or expand..."> more... </a>
 <div id="label197" style="display:none">
 <table border="1">
 <tr>
 <td></td>
 <td colspan="4">Supported Version Ranges</td>
 </tr>
 <tr>
 <td>cos3</td>
 <td><code class="docutils literal notranslate">v6.4.0 -> v6.4.0 </code></td>
 <td><code class="docutils literal notranslate">v7.2.0 -> v7.2.0 </code></td>
 <td><code class="docutils literal notranslate">v7.4.0 -> v7.4.1 </code></td>
 <td><code class="docutils literal notranslate">v7.4.3 -> 7.6.4 </code></td>
 </tr>
 </table>
 </div>
 </li>
            <li> <span class="li-head">cos4</span> - CoS profile name for CoS 4. Source system.isf-queue-profile.name. <span class="li-normal">type: str</span>
 <a id='label198' href="javascript:ContentClick('label199', 'label198');" onmouseover="ContentPreview('label199');" onmouseout="ContentUnpreview('label199');" title="click to collapse or expand..."> more... </a>
 <div id="label199" style="display:none">
 <table border="1">
 <tr>
 <td></td>
 <td colspan="4">Supported Version Ranges</td>
 </tr>
 <tr>
 <td>cos4</td>
 <td><code class="docutils literal notranslate">v6.4.0 -> v6.4.0 </code></td>
 <td><code class="docutils literal notranslate">v7.2.0 -> v7.2.0 </code></td>
 <td><code class="docutils literal notranslate">v7.4.0 -> v7.4.1 </code></td>
 <td><code class="docutils literal notranslate">v7.4.3 -> 7.6.4 </code></td>
 </tr>
 </table>
 </div>
 </li>
            <li> <span class="li-head">cos5</span> - CoS profile name for CoS 5. Source system.isf-queue-profile.name. <span class="li-normal">type: str</span>
 <a id='label200' href="javascript:ContentClick('label201', 'label200');" onmouseover="ContentPreview('label201');" onmouseout="ContentUnpreview('label201');" title="click to collapse or expand..."> more... </a>
 <div id="label201" style="display:none">
 <table border="1">
 <tr>
 <td></td>
 <td colspan="4">Supported Version Ranges</td>
 </tr>
 <tr>
 <td>cos5</td>
 <td><code class="docutils literal notranslate">v6.4.0 -> v6.4.0 </code></td>
 <td><code class="docutils literal notranslate">v7.2.0 -> v7.2.0 </code></td>
 <td><code class="docutils literal notranslate">v7.4.0 -> v7.4.1 </code></td>
 <td><code class="docutils literal notranslate">v7.4.3 -> 7.6.4 </code></td>
 </tr>
 </table>
 </div>
 </li>
            <li> <span class="li-head">cos6</span> - CoS profile name for CoS 6. Source system.isf-queue-profile.name. <span class="li-normal">type: str</span>
 <a id='label202' href="javascript:ContentClick('label203', 'label202');" onmouseover="ContentPreview('label203');" onmouseout="ContentUnpreview('label203');" title="click to collapse or expand..."> more... </a>
 <div id="label203" style="display:none">
 <table border="1">
 <tr>
 <td></td>
 <td colspan="4">Supported Version Ranges</td>
 </tr>
 <tr>
 <td>cos6</td>
 <td><code class="docutils literal notranslate">v6.4.0 -> v6.4.0 </code></td>
 <td><code class="docutils literal notranslate">v7.2.0 -> v7.2.0 </code></td>
 <td><code class="docutils literal notranslate">v7.4.0 -> v7.4.1 </code></td>
 <td><code class="docutils literal notranslate">v7.4.3 -> 7.6.4 </code></td>
 </tr>
 </table>
 </div>
 </li>
            <li> <span class="li-head">cos7</span> - CoS profile name for CoS 7. Source system.isf-queue-profile.name. <span class="li-normal">type: str</span>
 <a id='label204' href="javascript:ContentClick('label205', 'label204');" onmouseover="ContentPreview('label205');" onmouseout="ContentUnpreview('label205');" title="click to collapse or expand..."> more... </a>
 <div id="label205" style="display:none">
 <table border="1">
 <tr>
 <td></td>
 <td colspan="4">Supported Version Ranges</td>
 </tr>
 <tr>
 <td>cos7</td>
 <td><code class="docutils literal notranslate">v6.4.0 -> v6.4.0 </code></td>
 <td><code class="docutils literal notranslate">v7.2.0 -> v7.2.0 </code></td>
 <td><code class="docutils literal notranslate">v7.4.0 -> v7.4.1 </code></td>
 <td><code class="docutils literal notranslate">v7.4.3 -> 7.6.4 </code></td>
 </tr>
 </table>
 </div>
 </li>
            </ul>
        <li> <span class="li-head">lag_out_port_select</span> - Enable/disable LAG outgoing port selection based on incoming traffic port. <span class="li-normal">type: str</span> <span class="li-normal">choices: disable, enable</span>
 <a id='label206' href="javascript:ContentClick('label207', 'label206');" onmouseover="ContentPreview('label207');" onmouseout="ContentUnpreview('label207');" title="click to collapse or expand..."> more... </a>
 <div id="label207" style="display:none">
 <table border="1">
 <tr>
 <td></td>
 <td colspan="3">Supported Version Ranges</td>
 </tr>
 <tr>
 <td>lag_out_port_select</td>
 <td><code class="docutils literal notranslate">v6.2.0 -> v6.2.7 </code></td>
 <td><code class="docutils literal notranslate">v6.4.1 -> v7.4.1 </code></td>
 <td><code class="docutils literal notranslate">v7.4.3 -> 7.6.4 </code></td>
 </tr>
 <tr>
 <td>[disable]</td>
 <td><code class="docutils literal notranslate">v6.2.0 -> v6.2.7</code></td>
 <tr>
 <td>[enable]</td>
 <td><code class="docutils literal notranslate">v6.2.0 -> v6.2.7</code></td>
 </table>
 </div>
 </li>
        <li> <span class="li-head">max_receive_unit</span> - Set the maximum packet size for receive, larger packets will be silently dropped. <span class="li-normal">type: int</span>
 <a id='label208' href="javascript:ContentClick('label209', 'label208');" onmouseover="ContentPreview('label209');" onmouseout="ContentUnpreview('label209');" title="click to collapse or expand..."> more... </a>
 <div id="label209" style="display:none">
 <table border="1">
 <tr>
 <td></td>
 <td colspan="1">Supported Version Ranges</td>
 </tr>
 <tr>
 <td>max_receive_unit</td>
 <td><code class="docutils literal notranslate">v7.4.2 -> v7.4.2 </code></td>
 </tr>
 </table>
 </div>
 </li>
        <li> <span class="li-head">max_session_timeout</span> - Maximum time interval for refreshing NPU-offloaded sessions (10 - 1000 sec). <span class="li-normal">type: int</span>
 <a id='label210' href="javascript:ContentClick('label211', 'label210');" onmouseover="ContentPreview('label211');" onmouseout="ContentUnpreview('label211');" title="click to collapse or expand..."> more... </a>
 <div id="label211" style="display:none">
 <table border="1">
 <tr>
 <td></td>
 <td colspan="1">Supported Version Ranges</td>
 </tr>
 <tr>
 <td>max_session_timeout</td>
 <td><code class="docutils literal notranslate">v7.4.2 -> v7.4.2 </code></td>
 </tr>
 </table>
 </div>
 </li>
        <li> <span class="li-head">mcast_session_accounting</span> - Enable/disable traffic accounting for each multicast session through TAE counter. <span class="li-normal">type: str</span> <span class="li-normal">choices: tpe-based, session-based, disable</span>
 <a id='label212' href="javascript:ContentClick('label213', 'label212');" onmouseover="ContentPreview('label213');" onmouseout="ContentUnpreview('label213');" title="click to collapse or expand..."> more... </a>
 <div id="label213" style="display:none">
 <table border="1">
 <tr>
 <td></td>
 <td colspan="5">Supported Version Ranges</td>
 </tr>
 <tr>
 <td>mcast_session_accounting</td>
 <td><code class="docutils literal notranslate">v6.0.0 -> v6.0.0 </code></td>
 <td><code class="docutils literal notranslate">v6.0.11 -> v6.2.0 </code></td>
 <td><code class="docutils literal notranslate">v6.2.5 -> v6.2.7 </code></td>
 <td><code class="docutils literal notranslate">v6.4.4 -> v7.4.1 </code></td>
 <td><code class="docutils literal notranslate">v7.4.3 -> 7.6.4 </code></td>
 </tr>
 <tr>
 <td>[tpe-based]</td>
 <td><code class="docutils literal notranslate">v6.0.0 -> v6.0.0</code></td>
 <tr>
 <td>[session-based]</td>
 <td><code class="docutils literal notranslate">v6.0.0 -> v6.0.0</code></td>
 <tr>
 <td>[disable]</td>
 <td><code class="docutils literal notranslate">v6.0.0 -> v6.0.0</code></td>
 </table>
 </div>
 </li>
        <li> <span class="li-head">napi_break_interval</span> - NAPI break interval . <span class="li-normal">type: int</span>
 <a id='label214' href="javascript:ContentClick('label215', 'label214');" onmouseover="ContentPreview('label215');" onmouseout="ContentUnpreview('label215');" title="click to collapse or expand..."> more... </a>
 <div id="label215" style="display:none">
 <table border="1">
 <tr>
 <td></td>
 <td colspan="1">Supported Version Ranges</td>
 </tr>
 <tr>
 <td>napi_break_interval</td>
 <td><code class="docutils literal notranslate">v7.4.2 -> v7.4.2 </code></td>
 </tr>
 </table>
 </div>
 </li>
        <li> <span class="li-head">np_queues</span> - Configure queue assignment on NP7. <span class="li-normal">type: dict</span>
 <a id='label216' href="javascript:ContentClick('label217', 'label216');" onmouseover="ContentPreview('label217');" onmouseout="ContentUnpreview('label217');" title="click to collapse or expand..."> more... </a>
 <div id="label217" style="display:none">
 <table border="1">
 <tr>
 <td></td><td colspan="1">Supported Version Ranges</td>
 </tr>
 <tr>
 <td>np_queues</td>
 <td><code class="docutils literal notranslate">v7.4.2 -> v7.4.2 </code></td>
 </tr>
 </table>
 </div>
 </li>
            <ul class="ul-self">
            <li> <span class="li-head">ethernet_type</span> - Configure a NP7 QoS Ethernet Type. <span class="li-normal">type: list</span> <span style="font-family:'Courier New'" class="li-required">member_path: np_queues/ethernet_type:name</span>
 <a id='label218' href="javascript:ContentClick('label219', 'label218');" onmouseover="ContentPreview('label219');" onmouseout="ContentUnpreview('label219');" title="click to collapse or expand..."> more... </a>
 <div id="label219" style="display:none">
 <table border="1">
 <tr>
 <td></td><td colspan="1">Supported Version Ranges</td>
 </tr>
 <tr>
 <td>ethernet_type</td>
 <td><code class="docutils literal notranslate">v7.4.2 -> v7.4.2 </code></td>
 </tr>
 </table>
 </div>
 </li>
                <ul class="ul-self">
                <li> <span class="li-head">name</span> - Ethernet Type Name. <span class="li-normal">type: str</span> <span class="li-required">required: true</span>
 <a id='label220' href="javascript:ContentClick('label221', 'label220');" onmouseover="ContentPreview('label221');" onmouseout="ContentUnpreview('label221');" title="click to collapse or expand..."> more... </a>
 <div id="label221" style="display:none">
 <table border="1">
 <tr>
 <td></td>
 <td colspan="1">Supported Version Ranges</td>
 </tr>
 <tr>
 <td>name</td>
 <td><code class="docutils literal notranslate">v7.4.2 -> v7.4.2 </code></td>
 </tr>
 </table>
 </div>
 </li>
                <li> <span class="li-head">queue</span> - Queue Number. <span class="li-normal">type: int</span>
 <a id='label222' href="javascript:ContentClick('label223', 'label222');" onmouseover="ContentPreview('label223');" onmouseout="ContentUnpreview('label223');" title="click to collapse or expand..."> more... </a>
 <div id="label223" style="display:none">
 <table border="1">
 <tr>
 <td></td>
 <td colspan="1">Supported Version Ranges</td>
 </tr>
 <tr>
 <td>queue</td>
 <td><code class="docutils literal notranslate">v7.4.2 -> v7.4.2 </code></td>
 </tr>
 </table>
 </div>
 </li>
                <li> <span class="li-head">type</span> - Ethernet Type. <span class="li-normal">type: str</span>
 <a id='label224' href="javascript:ContentClick('label225', 'label224');" onmouseover="ContentPreview('label225');" onmouseout="ContentUnpreview('label225');" title="click to collapse or expand..."> more... </a>
 <div id="label225" style="display:none">
 <table border="1">
 <tr>
 <td></td>
 <td colspan="1">Supported Version Ranges</td>
 </tr>
 <tr>
 <td>type</td>
 <td><code class="docutils literal notranslate">v7.4.2 -> v7.4.2 </code></td>
 </tr>
 </table>
 </div>
 </li>
                <li> <span class="li-head">weight</span> - Class Weight. <span class="li-normal">type: int</span>
 <a id='label226' href="javascript:ContentClick('label227', 'label226');" onmouseover="ContentPreview('label227');" onmouseout="ContentUnpreview('label227');" title="click to collapse or expand..."> more... </a>
 <div id="label227" style="display:none">
 <table border="1">
 <tr>
 <td></td>
 <td colspan="1">Supported Version Ranges</td>
 </tr>
 <tr>
 <td>weight</td>
 <td><code class="docutils literal notranslate">v7.4.2 -> v7.4.2 </code></td>
 </tr>
 </table>
 </div>
 </li>
                </ul>
            <li> <span class="li-head">ip_protocol</span> - Configure a NP7 QoS IP Protocol. <span class="li-normal">type: list</span> <span style="font-family:'Courier New'" class="li-required">member_path: np_queues/ip_protocol:name</span>
 <a id='label228' href="javascript:ContentClick('label229', 'label228');" onmouseover="ContentPreview('label229');" onmouseout="ContentUnpreview('label229');" title="click to collapse or expand..."> more... </a>
 <div id="label229" style="display:none">
 <table border="1">
 <tr>
 <td></td><td colspan="1">Supported Version Ranges</td>
 </tr>
 <tr>
 <td>ip_protocol</td>
 <td><code class="docutils literal notranslate">v7.4.2 -> v7.4.2 </code></td>
 </tr>
 </table>
 </div>
 </li>
                <ul class="ul-self">
                <li> <span class="li-head">name</span> - IP Protocol Name. <span class="li-normal">type: str</span> <span class="li-required">required: true</span>
 <a id='label230' href="javascript:ContentClick('label231', 'label230');" onmouseover="ContentPreview('label231');" onmouseout="ContentUnpreview('label231');" title="click to collapse or expand..."> more... </a>
 <div id="label231" style="display:none">
 <table border="1">
 <tr>
 <td></td>
 <td colspan="1">Supported Version Ranges</td>
 </tr>
 <tr>
 <td>name</td>
 <td><code class="docutils literal notranslate">v7.4.2 -> v7.4.2 </code></td>
 </tr>
 </table>
 </div>
 </li>
                <li> <span class="li-head">protocol</span> - IP Protocol. <span class="li-normal">type: int</span>
 <a id='label232' href="javascript:ContentClick('label233', 'label232');" onmouseover="ContentPreview('label233');" onmouseout="ContentUnpreview('label233');" title="click to collapse or expand..."> more... </a>
 <div id="label233" style="display:none">
 <table border="1">
 <tr>
 <td></td>
 <td colspan="1">Supported Version Ranges</td>
 </tr>
 <tr>
 <td>protocol</td>
 <td><code class="docutils literal notranslate">v7.4.2 -> v7.4.2 </code></td>
 </tr>
 </table>
 </div>
 </li>
                <li> <span class="li-head">queue</span> - Queue Number. <span class="li-normal">type: int</span>
 <a id='label234' href="javascript:ContentClick('label235', 'label234');" onmouseover="ContentPreview('label235');" onmouseout="ContentUnpreview('label235');" title="click to collapse or expand..."> more... </a>
 <div id="label235" style="display:none">
 <table border="1">
 <tr>
 <td></td>
 <td colspan="1">Supported Version Ranges</td>
 </tr>
 <tr>
 <td>queue</td>
 <td><code class="docutils literal notranslate">v7.4.2 -> v7.4.2 </code></td>
 </tr>
 </table>
 </div>
 </li>
                <li> <span class="li-head">weight</span> - Class Weight. <span class="li-normal">type: int</span>
 <a id='label236' href="javascript:ContentClick('label237', 'label236');" onmouseover="ContentPreview('label237');" onmouseout="ContentUnpreview('label237');" title="click to collapse or expand..."> more... </a>
 <div id="label237" style="display:none">
 <table border="1">
 <tr>
 <td></td>
 <td colspan="1">Supported Version Ranges</td>
 </tr>
 <tr>
 <td>weight</td>
 <td><code class="docutils literal notranslate">v7.4.2 -> v7.4.2 </code></td>
 </tr>
 </table>
 </div>
 </li>
                </ul>
            <li> <span class="li-head">ip_service</span> - Configure a NP7 QoS IP Service. <span class="li-normal">type: list</span> <span style="font-family:'Courier New'" class="li-required">member_path: np_queues/ip_service:name</span>
 <a id='label238' href="javascript:ContentClick('label239', 'label238');" onmouseover="ContentPreview('label239');" onmouseout="ContentUnpreview('label239');" title="click to collapse or expand..."> more... </a>
 <div id="label239" style="display:none">
 <table border="1">
 <tr>
 <td></td><td colspan="1">Supported Version Ranges</td>
 </tr>
 <tr>
 <td>ip_service</td>
 <td><code class="docutils literal notranslate">v7.4.2 -> v7.4.2 </code></td>
 </tr>
 </table>
 </div>
 </li>
                <ul class="ul-self">
                <li> <span class="li-head">dport</span> - Destination port. <span class="li-normal">type: int</span>
 <a id='label240' href="javascript:ContentClick('label241', 'label240');" onmouseover="ContentPreview('label241');" onmouseout="ContentUnpreview('label241');" title="click to collapse or expand..."> more... </a>
 <div id="label241" style="display:none">
 <table border="1">
 <tr>
 <td></td>
 <td colspan="1">Supported Version Ranges</td>
 </tr>
 <tr>
 <td>dport</td>
 <td><code class="docutils literal notranslate">v7.4.2 -> v7.4.2 </code></td>
 </tr>
 </table>
 </div>
 </li>
                <li> <span class="li-head">name</span> - IP service name. <span class="li-normal">type: str</span> <span class="li-required">required: true</span>
 <a id='label242' href="javascript:ContentClick('label243', 'label242');" onmouseover="ContentPreview('label243');" onmouseout="ContentUnpreview('label243');" title="click to collapse or expand..."> more... </a>
 <div id="label243" style="display:none">
 <table border="1">
 <tr>
 <td></td>
 <td colspan="1">Supported Version Ranges</td>
 </tr>
 <tr>
 <td>name</td>
 <td><code class="docutils literal notranslate">v7.4.2 -> v7.4.2 </code></td>
 </tr>
 </table>
 </div>
 </li>
                <li> <span class="li-head">protocol</span> - IP protocol. <span class="li-normal">type: int</span>
 <a id='label244' href="javascript:ContentClick('label245', 'label244');" onmouseover="ContentPreview('label245');" onmouseout="ContentUnpreview('label245');" title="click to collapse or expand..."> more... </a>
 <div id="label245" style="display:none">
 <table border="1">
 <tr>
 <td></td>
 <td colspan="1">Supported Version Ranges</td>
 </tr>
 <tr>
 <td>protocol</td>
 <td><code class="docutils literal notranslate">v7.4.2 -> v7.4.2 </code></td>
 </tr>
 </table>
 </div>
 </li>
                <li> <span class="li-head">queue</span> - Queue number. <span class="li-normal">type: int</span>
 <a id='label246' href="javascript:ContentClick('label247', 'label246');" onmouseover="ContentPreview('label247');" onmouseout="ContentUnpreview('label247');" title="click to collapse or expand..."> more... </a>
 <div id="label247" style="display:none">
 <table border="1">
 <tr>
 <td></td>
 <td colspan="1">Supported Version Ranges</td>
 </tr>
 <tr>
 <td>queue</td>
 <td><code class="docutils literal notranslate">v7.4.2 -> v7.4.2 </code></td>
 </tr>
 </table>
 </div>
 </li>
                <li> <span class="li-head">sport</span> - Source port. <span class="li-normal">type: int</span>
 <a id='label248' href="javascript:ContentClick('label249', 'label248');" onmouseover="ContentPreview('label249');" onmouseout="ContentUnpreview('label249');" title="click to collapse or expand..."> more... </a>
 <div id="label249" style="display:none">
 <table border="1">
 <tr>
 <td></td>
 <td colspan="1">Supported Version Ranges</td>
 </tr>
 <tr>
 <td>sport</td>
 <td><code class="docutils literal notranslate">v7.4.2 -> v7.4.2 </code></td>
 </tr>
 </table>
 </div>
 </li>
                <li> <span class="li-head">weight</span> - Class weight. <span class="li-normal">type: int</span>
 <a id='label250' href="javascript:ContentClick('label251', 'label250');" onmouseover="ContentPreview('label251');" onmouseout="ContentUnpreview('label251');" title="click to collapse or expand..."> more... </a>
 <div id="label251" style="display:none">
 <table border="1">
 <tr>
 <td></td>
 <td colspan="1">Supported Version Ranges</td>
 </tr>
 <tr>
 <td>weight</td>
 <td><code class="docutils literal notranslate">v7.4.2 -> v7.4.2 </code></td>
 </tr>
 </table>
 </div>
 </li>
                </ul>
            <li> <span class="li-head">profile</span> - Configure a NP7 class profile. <span class="li-normal">type: list</span> <span style="font-family:'Courier New'" class="li-required">member_path: np_queues/profile:id</span>
 <a id='label252' href="javascript:ContentClick('label253', 'label252');" onmouseover="ContentPreview('label253');" onmouseout="ContentUnpreview('label253');" title="click to collapse or expand..."> more... </a>
 <div id="label253" style="display:none">
 <table border="1">
 <tr>
 <td></td><td colspan="1">Supported Version Ranges</td>
 </tr>
 <tr>
 <td>profile</td>
 <td><code class="docutils literal notranslate">v7.4.2 -> v7.4.2 </code></td>
 </tr>
 </table>
 </div>
 </li>
                <ul class="ul-self">
                <li> <span class="li-head">cos0</span> - Queue number of CoS 0. <span class="li-normal">type: str</span> <span class="li-normal">choices: queue0, queue1, queue2, queue3, queue4, queue5, queue6, queue7</span>
 <a id='label254' href="javascript:ContentClick('label255', 'label254');" onmouseover="ContentPreview('label255');" onmouseout="ContentUnpreview('label255');" title="click to collapse or expand..."> more... </a>
 <div id="label255" style="display:none">
 <table border="1">
 <tr>
 <td></td>
 <td colspan="1">Supported Version Ranges</td>
 </tr>
 <tr>
 <td>cos0</td>
 <td><code class="docutils literal notranslate">v7.4.2 -> v7.4.2 </code></td>
 </tr>
 <tr>
 <td>[queue0]</td>
 <td><code class="docutils literal notranslate">v7.4.2 -> v7.4.2</code></td>
 <tr>
 <td>[queue1]</td>
 <td><code class="docutils literal notranslate">v7.4.2 -> v7.4.2</code></td>
 <tr>
 <td>[queue2]</td>
 <td><code class="docutils literal notranslate">v7.4.2 -> v7.4.2</code></td>
 <tr>
 <td>[queue3]</td>
 <td><code class="docutils literal notranslate">v7.4.2 -> v7.4.2</code></td>
 <tr>
 <td>[queue4]</td>
 <td><code class="docutils literal notranslate">v7.4.2 -> v7.4.2</code></td>
 <tr>
 <td>[queue5]</td>
 <td><code class="docutils literal notranslate">v7.4.2 -> v7.4.2</code></td>
 <tr>
 <td>[queue6]</td>
 <td><code class="docutils literal notranslate">v7.4.2 -> v7.4.2</code></td>
 <tr>
 <td>[queue7]</td>
 <td><code class="docutils literal notranslate">v7.4.2 -> v7.4.2</code></td>
 </table>
 </div>
 </li>
                <li> <span class="li-head">cos1</span> - Queue number of CoS 1. <span class="li-normal">type: str</span> <span class="li-normal">choices: queue0, queue1, queue2, queue3, queue4, queue5, queue6, queue7</span>
 <a id='label256' href="javascript:ContentClick('label257', 'label256');" onmouseover="ContentPreview('label257');" onmouseout="ContentUnpreview('label257');" title="click to collapse or expand..."> more... </a>
 <div id="label257" style="display:none">
 <table border="1">
 <tr>
 <td></td>
 <td colspan="1">Supported Version Ranges</td>
 </tr>
 <tr>
 <td>cos1</td>
 <td><code class="docutils literal notranslate">v7.4.2 -> v7.4.2 </code></td>
 </tr>
 <tr>
 <td>[queue0]</td>
 <td><code class="docutils literal notranslate">v7.4.2 -> v7.4.2</code></td>
 <tr>
 <td>[queue1]</td>
 <td><code class="docutils literal notranslate">v7.4.2 -> v7.4.2</code></td>
 <tr>
 <td>[queue2]</td>
 <td><code class="docutils literal notranslate">v7.4.2 -> v7.4.2</code></td>
 <tr>
 <td>[queue3]</td>
 <td><code class="docutils literal notranslate">v7.4.2 -> v7.4.2</code></td>
 <tr>
 <td>[queue4]</td>
 <td><code class="docutils literal notranslate">v7.4.2 -> v7.4.2</code></td>
 <tr>
 <td>[queue5]</td>
 <td><code class="docutils literal notranslate">v7.4.2 -> v7.4.2</code></td>
 <tr>
 <td>[queue6]</td>
 <td><code class="docutils literal notranslate">v7.4.2 -> v7.4.2</code></td>
 <tr>
 <td>[queue7]</td>
 <td><code class="docutils literal notranslate">v7.4.2 -> v7.4.2</code></td>
 </table>
 </div>
 </li>
                <li> <span class="li-head">cos2</span> - Queue number of CoS 2. <span class="li-normal">type: str</span> <span class="li-normal">choices: queue0, queue1, queue2, queue3, queue4, queue5, queue6, queue7</span>
 <a id='label258' href="javascript:ContentClick('label259', 'label258');" onmouseover="ContentPreview('label259');" onmouseout="ContentUnpreview('label259');" title="click to collapse or expand..."> more... </a>
 <div id="label259" style="display:none">
 <table border="1">
 <tr>
 <td></td>
 <td colspan="1">Supported Version Ranges</td>
 </tr>
 <tr>
 <td>cos2</td>
 <td><code class="docutils literal notranslate">v7.4.2 -> v7.4.2 </code></td>
 </tr>
 <tr>
 <td>[queue0]</td>
 <td><code class="docutils literal notranslate">v7.4.2 -> v7.4.2</code></td>
 <tr>
 <td>[queue1]</td>
 <td><code class="docutils literal notranslate">v7.4.2 -> v7.4.2</code></td>
 <tr>
 <td>[queue2]</td>
 <td><code class="docutils literal notranslate">v7.4.2 -> v7.4.2</code></td>
 <tr>
 <td>[queue3]</td>
 <td><code class="docutils literal notranslate">v7.4.2 -> v7.4.2</code></td>
 <tr>
 <td>[queue4]</td>
 <td><code class="docutils literal notranslate">v7.4.2 -> v7.4.2</code></td>
 <tr>
 <td>[queue5]</td>
 <td><code class="docutils literal notranslate">v7.4.2 -> v7.4.2</code></td>
 <tr>
 <td>[queue6]</td>
 <td><code class="docutils literal notranslate">v7.4.2 -> v7.4.2</code></td>
 <tr>
 <td>[queue7]</td>
 <td><code class="docutils literal notranslate">v7.4.2 -> v7.4.2</code></td>
 </table>
 </div>
 </li>
                <li> <span class="li-head">cos3</span> - Queue number of CoS 3. <span class="li-normal">type: str</span> <span class="li-normal">choices: queue0, queue1, queue2, queue3, queue4, queue5, queue6, queue7</span>
 <a id='label260' href="javascript:ContentClick('label261', 'label260');" onmouseover="ContentPreview('label261');" onmouseout="ContentUnpreview('label261');" title="click to collapse or expand..."> more... </a>
 <div id="label261" style="display:none">
 <table border="1">
 <tr>
 <td></td>
 <td colspan="1">Supported Version Ranges</td>
 </tr>
 <tr>
 <td>cos3</td>
 <td><code class="docutils literal notranslate">v7.4.2 -> v7.4.2 </code></td>
 </tr>
 <tr>
 <td>[queue0]</td>
 <td><code class="docutils literal notranslate">v7.4.2 -> v7.4.2</code></td>
 <tr>
 <td>[queue1]</td>
 <td><code class="docutils literal notranslate">v7.4.2 -> v7.4.2</code></td>
 <tr>
 <td>[queue2]</td>
 <td><code class="docutils literal notranslate">v7.4.2 -> v7.4.2</code></td>
 <tr>
 <td>[queue3]</td>
 <td><code class="docutils literal notranslate">v7.4.2 -> v7.4.2</code></td>
 <tr>
 <td>[queue4]</td>
 <td><code class="docutils literal notranslate">v7.4.2 -> v7.4.2</code></td>
 <tr>
 <td>[queue5]</td>
 <td><code class="docutils literal notranslate">v7.4.2 -> v7.4.2</code></td>
 <tr>
 <td>[queue6]</td>
 <td><code class="docutils literal notranslate">v7.4.2 -> v7.4.2</code></td>
 <tr>
 <td>[queue7]</td>
 <td><code class="docutils literal notranslate">v7.4.2 -> v7.4.2</code></td>
 </table>
 </div>
 </li>
                <li> <span class="li-head">cos4</span> - Queue number of CoS 4. <span class="li-normal">type: str</span> <span class="li-normal">choices: queue0, queue1, queue2, queue3, queue4, queue5, queue6, queue7</span>
 <a id='label262' href="javascript:ContentClick('label263', 'label262');" onmouseover="ContentPreview('label263');" onmouseout="ContentUnpreview('label263');" title="click to collapse or expand..."> more... </a>
 <div id="label263" style="display:none">
 <table border="1">
 <tr>
 <td></td>
 <td colspan="1">Supported Version Ranges</td>
 </tr>
 <tr>
 <td>cos4</td>
 <td><code class="docutils literal notranslate">v7.4.2 -> v7.4.2 </code></td>
 </tr>
 <tr>
 <td>[queue0]</td>
 <td><code class="docutils literal notranslate">v7.4.2 -> v7.4.2</code></td>
 <tr>
 <td>[queue1]</td>
 <td><code class="docutils literal notranslate">v7.4.2 -> v7.4.2</code></td>
 <tr>
 <td>[queue2]</td>
 <td><code class="docutils literal notranslate">v7.4.2 -> v7.4.2</code></td>
 <tr>
 <td>[queue3]</td>
 <td><code class="docutils literal notranslate">v7.4.2 -> v7.4.2</code></td>
 <tr>
 <td>[queue4]</td>
 <td><code class="docutils literal notranslate">v7.4.2 -> v7.4.2</code></td>
 <tr>
 <td>[queue5]</td>
 <td><code class="docutils literal notranslate">v7.4.2 -> v7.4.2</code></td>
 <tr>
 <td>[queue6]</td>
 <td><code class="docutils literal notranslate">v7.4.2 -> v7.4.2</code></td>
 <tr>
 <td>[queue7]</td>
 <td><code class="docutils literal notranslate">v7.4.2 -> v7.4.2</code></td>
 </table>
 </div>
 </li>
                <li> <span class="li-head">cos5</span> - Queue number of CoS 5. <span class="li-normal">type: str</span> <span class="li-normal">choices: queue0, queue1, queue2, queue3, queue4, queue5, queue6, queue7</span>
 <a id='label264' href="javascript:ContentClick('label265', 'label264');" onmouseover="ContentPreview('label265');" onmouseout="ContentUnpreview('label265');" title="click to collapse or expand..."> more... </a>
 <div id="label265" style="display:none">
 <table border="1">
 <tr>
 <td></td>
 <td colspan="1">Supported Version Ranges</td>
 </tr>
 <tr>
 <td>cos5</td>
 <td><code class="docutils literal notranslate">v7.4.2 -> v7.4.2 </code></td>
 </tr>
 <tr>
 <td>[queue0]</td>
 <td><code class="docutils literal notranslate">v7.4.2 -> v7.4.2</code></td>
 <tr>
 <td>[queue1]</td>
 <td><code class="docutils literal notranslate">v7.4.2 -> v7.4.2</code></td>
 <tr>
 <td>[queue2]</td>
 <td><code class="docutils literal notranslate">v7.4.2 -> v7.4.2</code></td>
 <tr>
 <td>[queue3]</td>
 <td><code class="docutils literal notranslate">v7.4.2 -> v7.4.2</code></td>
 <tr>
 <td>[queue4]</td>
 <td><code class="docutils literal notranslate">v7.4.2 -> v7.4.2</code></td>
 <tr>
 <td>[queue5]</td>
 <td><code class="docutils literal notranslate">v7.4.2 -> v7.4.2</code></td>
 <tr>
 <td>[queue6]</td>
 <td><code class="docutils literal notranslate">v7.4.2 -> v7.4.2</code></td>
 <tr>
 <td>[queue7]</td>
 <td><code class="docutils literal notranslate">v7.4.2 -> v7.4.2</code></td>
 </table>
 </div>
 </li>
                <li> <span class="li-head">cos6</span> - Queue number of CoS 6. <span class="li-normal">type: str</span> <span class="li-normal">choices: queue0, queue1, queue2, queue3, queue4, queue5, queue6, queue7</span>
 <a id='label266' href="javascript:ContentClick('label267', 'label266');" onmouseover="ContentPreview('label267');" onmouseout="ContentUnpreview('label267');" title="click to collapse or expand..."> more... </a>
 <div id="label267" style="display:none">
 <table border="1">
 <tr>
 <td></td>
 <td colspan="1">Supported Version Ranges</td>
 </tr>
 <tr>
 <td>cos6</td>
 <td><code class="docutils literal notranslate">v7.4.2 -> v7.4.2 </code></td>
 </tr>
 <tr>
 <td>[queue0]</td>
 <td><code class="docutils literal notranslate">v7.4.2 -> v7.4.2</code></td>
 <tr>
 <td>[queue1]</td>
 <td><code class="docutils literal notranslate">v7.4.2 -> v7.4.2</code></td>
 <tr>
 <td>[queue2]</td>
 <td><code class="docutils literal notranslate">v7.4.2 -> v7.4.2</code></td>
 <tr>
 <td>[queue3]</td>
 <td><code class="docutils literal notranslate">v7.4.2 -> v7.4.2</code></td>
 <tr>
 <td>[queue4]</td>
 <td><code class="docutils literal notranslate">v7.4.2 -> v7.4.2</code></td>
 <tr>
 <td>[queue5]</td>
 <td><code class="docutils literal notranslate">v7.4.2 -> v7.4.2</code></td>
 <tr>
 <td>[queue6]</td>
 <td><code class="docutils literal notranslate">v7.4.2 -> v7.4.2</code></td>
 <tr>
 <td>[queue7]</td>
 <td><code class="docutils literal notranslate">v7.4.2 -> v7.4.2</code></td>
 </table>
 </div>
 </li>
                <li> <span class="li-head">cos7</span> - Queue number of CoS 7. <span class="li-normal">type: str</span> <span class="li-normal">choices: queue0, queue1, queue2, queue3, queue4, queue5, queue6, queue7</span>
 <a id='label268' href="javascript:ContentClick('label269', 'label268');" onmouseover="ContentPreview('label269');" onmouseout="ContentUnpreview('label269');" title="click to collapse or expand..."> more... </a>
 <div id="label269" style="display:none">
 <table border="1">
 <tr>
 <td></td>
 <td colspan="1">Supported Version Ranges</td>
 </tr>
 <tr>
 <td>cos7</td>
 <td><code class="docutils literal notranslate">v7.4.2 -> v7.4.2 </code></td>
 </tr>
 <tr>
 <td>[queue0]</td>
 <td><code class="docutils literal notranslate">v7.4.2 -> v7.4.2</code></td>
 <tr>
 <td>[queue1]</td>
 <td><code class="docutils literal notranslate">v7.4.2 -> v7.4.2</code></td>
 <tr>
 <td>[queue2]</td>
 <td><code class="docutils literal notranslate">v7.4.2 -> v7.4.2</code></td>
 <tr>
 <td>[queue3]</td>
 <td><code class="docutils literal notranslate">v7.4.2 -> v7.4.2</code></td>
 <tr>
 <td>[queue4]</td>
 <td><code class="docutils literal notranslate">v7.4.2 -> v7.4.2</code></td>
 <tr>
 <td>[queue5]</td>
 <td><code class="docutils literal notranslate">v7.4.2 -> v7.4.2</code></td>
 <tr>
 <td>[queue6]</td>
 <td><code class="docutils literal notranslate">v7.4.2 -> v7.4.2</code></td>
 <tr>
 <td>[queue7]</td>
 <td><code class="docutils literal notranslate">v7.4.2 -> v7.4.2</code></td>
 </table>
 </div>
 </li>
                <li> <span class="li-head">dscp0</span> - Queue number of DSCP 0. <span class="li-normal">type: str</span> <span class="li-normal">choices: queue0, queue1, queue2, queue3, queue4, queue5, queue6, queue7</span>
 <a id='label270' href="javascript:ContentClick('label271', 'label270');" onmouseover="ContentPreview('label271');" onmouseout="ContentUnpreview('label271');" title="click to collapse or expand..."> more... </a>
 <div id="label271" style="display:none">
 <table border="1">
 <tr>
 <td></td>
 <td colspan="1">Supported Version Ranges</td>
 </tr>
 <tr>
 <td>dscp0</td>
 <td><code class="docutils literal notranslate">v7.4.2 -> v7.4.2 </code></td>
 </tr>
 <tr>
 <td>[queue0]</td>
 <td><code class="docutils literal notranslate">v7.4.2 -> v7.4.2</code></td>
 <tr>
 <td>[queue1]</td>
 <td><code class="docutils literal notranslate">v7.4.2 -> v7.4.2</code></td>
 <tr>
 <td>[queue2]</td>
 <td><code class="docutils literal notranslate">v7.4.2 -> v7.4.2</code></td>
 <tr>
 <td>[queue3]</td>
 <td><code class="docutils literal notranslate">v7.4.2 -> v7.4.2</code></td>
 <tr>
 <td>[queue4]</td>
 <td><code class="docutils literal notranslate">v7.4.2 -> v7.4.2</code></td>
 <tr>
 <td>[queue5]</td>
 <td><code class="docutils literal notranslate">v7.4.2 -> v7.4.2</code></td>
 <tr>
 <td>[queue6]</td>
 <td><code class="docutils literal notranslate">v7.4.2 -> v7.4.2</code></td>
 <tr>
 <td>[queue7]</td>
 <td><code class="docutils literal notranslate">v7.4.2 -> v7.4.2</code></td>
 </table>
 </div>
 </li>
                <li> <span class="li-head">dscp1</span> - Queue number of DSCP 1. <span class="li-normal">type: str</span> <span class="li-normal">choices: queue0, queue1, queue2, queue3, queue4, queue5, queue6, queue7</span>
 <a id='label272' href="javascript:ContentClick('label273', 'label272');" onmouseover="ContentPreview('label273');" onmouseout="ContentUnpreview('label273');" title="click to collapse or expand..."> more... </a>
 <div id="label273" style="display:none">
 <table border="1">
 <tr>
 <td></td>
 <td colspan="1">Supported Version Ranges</td>
 </tr>
 <tr>
 <td>dscp1</td>
 <td><code class="docutils literal notranslate">v7.4.2 -> v7.4.2 </code></td>
 </tr>
 <tr>
 <td>[queue0]</td>
 <td><code class="docutils literal notranslate">v7.4.2 -> v7.4.2</code></td>
 <tr>
 <td>[queue1]</td>
 <td><code class="docutils literal notranslate">v7.4.2 -> v7.4.2</code></td>
 <tr>
 <td>[queue2]</td>
 <td><code class="docutils literal notranslate">v7.4.2 -> v7.4.2</code></td>
 <tr>
 <td>[queue3]</td>
 <td><code class="docutils literal notranslate">v7.4.2 -> v7.4.2</code></td>
 <tr>
 <td>[queue4]</td>
 <td><code class="docutils literal notranslate">v7.4.2 -> v7.4.2</code></td>
 <tr>
 <td>[queue5]</td>
 <td><code class="docutils literal notranslate">v7.4.2 -> v7.4.2</code></td>
 <tr>
 <td>[queue6]</td>
 <td><code class="docutils literal notranslate">v7.4.2 -> v7.4.2</code></td>
 <tr>
 <td>[queue7]</td>
 <td><code class="docutils literal notranslate">v7.4.2 -> v7.4.2</code></td>
 </table>
 </div>
 </li>
                <li> <span class="li-head">dscp10</span> - Queue number of DSCP 10. <span class="li-normal">type: str</span> <span class="li-normal">choices: queue0, queue1, queue2, queue3, queue4, queue5, queue6, queue7</span>
 <a id='label274' href="javascript:ContentClick('label275', 'label274');" onmouseover="ContentPreview('label275');" onmouseout="ContentUnpreview('label275');" title="click to collapse or expand..."> more... </a>
 <div id="label275" style="display:none">
 <table border="1">
 <tr>
 <td></td>
 <td colspan="1">Supported Version Ranges</td>
 </tr>
 <tr>
 <td>dscp10</td>
 <td><code class="docutils literal notranslate">v7.4.2 -> v7.4.2 </code></td>
 </tr>
 <tr>
 <td>[queue0]</td>
 <td><code class="docutils literal notranslate">v7.4.2 -> v7.4.2</code></td>
 <tr>
 <td>[queue1]</td>
 <td><code class="docutils literal notranslate">v7.4.2 -> v7.4.2</code></td>
 <tr>
 <td>[queue2]</td>
 <td><code class="docutils literal notranslate">v7.4.2 -> v7.4.2</code></td>
 <tr>
 <td>[queue3]</td>
 <td><code class="docutils literal notranslate">v7.4.2 -> v7.4.2</code></td>
 <tr>
 <td>[queue4]</td>
 <td><code class="docutils literal notranslate">v7.4.2 -> v7.4.2</code></td>
 <tr>
 <td>[queue5]</td>
 <td><code class="docutils literal notranslate">v7.4.2 -> v7.4.2</code></td>
 <tr>
 <td>[queue6]</td>
 <td><code class="docutils literal notranslate">v7.4.2 -> v7.4.2</code></td>
 <tr>
 <td>[queue7]</td>
 <td><code class="docutils literal notranslate">v7.4.2 -> v7.4.2</code></td>
 </table>
 </div>
 </li>
                <li> <span class="li-head">dscp11</span> - Queue number of DSCP 11. <span class="li-normal">type: str</span> <span class="li-normal">choices: queue0, queue1, queue2, queue3, queue4, queue5, queue6, queue7</span>
 <a id='label276' href="javascript:ContentClick('label277', 'label276');" onmouseover="ContentPreview('label277');" onmouseout="ContentUnpreview('label277');" title="click to collapse or expand..."> more... </a>
 <div id="label277" style="display:none">
 <table border="1">
 <tr>
 <td></td>
 <td colspan="1">Supported Version Ranges</td>
 </tr>
 <tr>
 <td>dscp11</td>
 <td><code class="docutils literal notranslate">v7.4.2 -> v7.4.2 </code></td>
 </tr>
 <tr>
 <td>[queue0]</td>
 <td><code class="docutils literal notranslate">v7.4.2 -> v7.4.2</code></td>
 <tr>
 <td>[queue1]</td>
 <td><code class="docutils literal notranslate">v7.4.2 -> v7.4.2</code></td>
 <tr>
 <td>[queue2]</td>
 <td><code class="docutils literal notranslate">v7.4.2 -> v7.4.2</code></td>
 <tr>
 <td>[queue3]</td>
 <td><code class="docutils literal notranslate">v7.4.2 -> v7.4.2</code></td>
 <tr>
 <td>[queue4]</td>
 <td><code class="docutils literal notranslate">v7.4.2 -> v7.4.2</code></td>
 <tr>
 <td>[queue5]</td>
 <td><code class="docutils literal notranslate">v7.4.2 -> v7.4.2</code></td>
 <tr>
 <td>[queue6]</td>
 <td><code class="docutils literal notranslate">v7.4.2 -> v7.4.2</code></td>
 <tr>
 <td>[queue7]</td>
 <td><code class="docutils literal notranslate">v7.4.2 -> v7.4.2</code></td>
 </table>
 </div>
 </li>
                <li> <span class="li-head">dscp12</span> - Queue number of DSCP 12. <span class="li-normal">type: str</span> <span class="li-normal">choices: queue0, queue1, queue2, queue3, queue4, queue5, queue6, queue7</span>
 <a id='label278' href="javascript:ContentClick('label279', 'label278');" onmouseover="ContentPreview('label279');" onmouseout="ContentUnpreview('label279');" title="click to collapse or expand..."> more... </a>
 <div id="label279" style="display:none">
 <table border="1">
 <tr>
 <td></td>
 <td colspan="1">Supported Version Ranges</td>
 </tr>
 <tr>
 <td>dscp12</td>
 <td><code class="docutils literal notranslate">v7.4.2 -> v7.4.2 </code></td>
 </tr>
 <tr>
 <td>[queue0]</td>
 <td><code class="docutils literal notranslate">v7.4.2 -> v7.4.2</code></td>
 <tr>
 <td>[queue1]</td>
 <td><code class="docutils literal notranslate">v7.4.2 -> v7.4.2</code></td>
 <tr>
 <td>[queue2]</td>
 <td><code class="docutils literal notranslate">v7.4.2 -> v7.4.2</code></td>
 <tr>
 <td>[queue3]</td>
 <td><code class="docutils literal notranslate">v7.4.2 -> v7.4.2</code></td>
 <tr>
 <td>[queue4]</td>
 <td><code class="docutils literal notranslate">v7.4.2 -> v7.4.2</code></td>
 <tr>
 <td>[queue5]</td>
 <td><code class="docutils literal notranslate">v7.4.2 -> v7.4.2</code></td>
 <tr>
 <td>[queue6]</td>
 <td><code class="docutils literal notranslate">v7.4.2 -> v7.4.2</code></td>
 <tr>
 <td>[queue7]</td>
 <td><code class="docutils literal notranslate">v7.4.2 -> v7.4.2</code></td>
 </table>
 </div>
 </li>
                <li> <span class="li-head">dscp13</span> - Queue number of DSCP 13. <span class="li-normal">type: str</span> <span class="li-normal">choices: queue0, queue1, queue2, queue3, queue4, queue5, queue6, queue7</span>
 <a id='label280' href="javascript:ContentClick('label281', 'label280');" onmouseover="ContentPreview('label281');" onmouseout="ContentUnpreview('label281');" title="click to collapse or expand..."> more... </a>
 <div id="label281" style="display:none">
 <table border="1">
 <tr>
 <td></td>
 <td colspan="1">Supported Version Ranges</td>
 </tr>
 <tr>
 <td>dscp13</td>
 <td><code class="docutils literal notranslate">v7.4.2 -> v7.4.2 </code></td>
 </tr>
 <tr>
 <td>[queue0]</td>
 <td><code class="docutils literal notranslate">v7.4.2 -> v7.4.2</code></td>
 <tr>
 <td>[queue1]</td>
 <td><code class="docutils literal notranslate">v7.4.2 -> v7.4.2</code></td>
 <tr>
 <td>[queue2]</td>
 <td><code class="docutils literal notranslate">v7.4.2 -> v7.4.2</code></td>
 <tr>
 <td>[queue3]</td>
 <td><code class="docutils literal notranslate">v7.4.2 -> v7.4.2</code></td>
 <tr>
 <td>[queue4]</td>
 <td><code class="docutils literal notranslate">v7.4.2 -> v7.4.2</code></td>
 <tr>
 <td>[queue5]</td>
 <td><code class="docutils literal notranslate">v7.4.2 -> v7.4.2</code></td>
 <tr>
 <td>[queue6]</td>
 <td><code class="docutils literal notranslate">v7.4.2 -> v7.4.2</code></td>
 <tr>
 <td>[queue7]</td>
 <td><code class="docutils literal notranslate">v7.4.2 -> v7.4.2</code></td>
 </table>
 </div>
 </li>
                <li> <span class="li-head">dscp14</span> - Queue number of DSCP 14. <span class="li-normal">type: str</span> <span class="li-normal">choices: queue0, queue1, queue2, queue3, queue4, queue5, queue6, queue7</span>
 <a id='label282' href="javascript:ContentClick('label283', 'label282');" onmouseover="ContentPreview('label283');" onmouseout="ContentUnpreview('label283');" title="click to collapse or expand..."> more... </a>
 <div id="label283" style="display:none">
 <table border="1">
 <tr>
 <td></td>
 <td colspan="1">Supported Version Ranges</td>
 </tr>
 <tr>
 <td>dscp14</td>
 <td><code class="docutils literal notranslate">v7.4.2 -> v7.4.2 </code></td>
 </tr>
 <tr>
 <td>[queue0]</td>
 <td><code class="docutils literal notranslate">v7.4.2 -> v7.4.2</code></td>
 <tr>
 <td>[queue1]</td>
 <td><code class="docutils literal notranslate">v7.4.2 -> v7.4.2</code></td>
 <tr>
 <td>[queue2]</td>
 <td><code class="docutils literal notranslate">v7.4.2 -> v7.4.2</code></td>
 <tr>
 <td>[queue3]</td>
 <td><code class="docutils literal notranslate">v7.4.2 -> v7.4.2</code></td>
 <tr>
 <td>[queue4]</td>
 <td><code class="docutils literal notranslate">v7.4.2 -> v7.4.2</code></td>
 <tr>
 <td>[queue5]</td>
 <td><code class="docutils literal notranslate">v7.4.2 -> v7.4.2</code></td>
 <tr>
 <td>[queue6]</td>
 <td><code class="docutils literal notranslate">v7.4.2 -> v7.4.2</code></td>
 <tr>
 <td>[queue7]</td>
 <td><code class="docutils literal notranslate">v7.4.2 -> v7.4.2</code></td>
 </table>
 </div>
 </li>
                <li> <span class="li-head">dscp15</span> - Queue number of DSCP 15. <span class="li-normal">type: str</span> <span class="li-normal">choices: queue0, queue1, queue2, queue3, queue4, queue5, queue6, queue7</span>
 <a id='label284' href="javascript:ContentClick('label285', 'label284');" onmouseover="ContentPreview('label285');" onmouseout="ContentUnpreview('label285');" title="click to collapse or expand..."> more... </a>
 <div id="label285" style="display:none">
 <table border="1">
 <tr>
 <td></td>
 <td colspan="1">Supported Version Ranges</td>
 </tr>
 <tr>
 <td>dscp15</td>
 <td><code class="docutils literal notranslate">v7.4.2 -> v7.4.2 </code></td>
 </tr>
 <tr>
 <td>[queue0]</td>
 <td><code class="docutils literal notranslate">v7.4.2 -> v7.4.2</code></td>
 <tr>
 <td>[queue1]</td>
 <td><code class="docutils literal notranslate">v7.4.2 -> v7.4.2</code></td>
 <tr>
 <td>[queue2]</td>
 <td><code class="docutils literal notranslate">v7.4.2 -> v7.4.2</code></td>
 <tr>
 <td>[queue3]</td>
 <td><code class="docutils literal notranslate">v7.4.2 -> v7.4.2</code></td>
 <tr>
 <td>[queue4]</td>
 <td><code class="docutils literal notranslate">v7.4.2 -> v7.4.2</code></td>
 <tr>
 <td>[queue5]</td>
 <td><code class="docutils literal notranslate">v7.4.2 -> v7.4.2</code></td>
 <tr>
 <td>[queue6]</td>
 <td><code class="docutils literal notranslate">v7.4.2 -> v7.4.2</code></td>
 <tr>
 <td>[queue7]</td>
 <td><code class="docutils literal notranslate">v7.4.2 -> v7.4.2</code></td>
 </table>
 </div>
 </li>
                <li> <span class="li-head">dscp16</span> - Queue number of DSCP 16. <span class="li-normal">type: str</span> <span class="li-normal">choices: queue0, queue1, queue2, queue3, queue4, queue5, queue6, queue7</span>
 <a id='label286' href="javascript:ContentClick('label287', 'label286');" onmouseover="ContentPreview('label287');" onmouseout="ContentUnpreview('label287');" title="click to collapse or expand..."> more... </a>
 <div id="label287" style="display:none">
 <table border="1">
 <tr>
 <td></td>
 <td colspan="1">Supported Version Ranges</td>
 </tr>
 <tr>
 <td>dscp16</td>
 <td><code class="docutils literal notranslate">v7.4.2 -> v7.4.2 </code></td>
 </tr>
 <tr>
 <td>[queue0]</td>
 <td><code class="docutils literal notranslate">v7.4.2 -> v7.4.2</code></td>
 <tr>
 <td>[queue1]</td>
 <td><code class="docutils literal notranslate">v7.4.2 -> v7.4.2</code></td>
 <tr>
 <td>[queue2]</td>
 <td><code class="docutils literal notranslate">v7.4.2 -> v7.4.2</code></td>
 <tr>
 <td>[queue3]</td>
 <td><code class="docutils literal notranslate">v7.4.2 -> v7.4.2</code></td>
 <tr>
 <td>[queue4]</td>
 <td><code class="docutils literal notranslate">v7.4.2 -> v7.4.2</code></td>
 <tr>
 <td>[queue5]</td>
 <td><code class="docutils literal notranslate">v7.4.2 -> v7.4.2</code></td>
 <tr>
 <td>[queue6]</td>
 <td><code class="docutils literal notranslate">v7.4.2 -> v7.4.2</code></td>
 <tr>
 <td>[queue7]</td>
 <td><code class="docutils literal notranslate">v7.4.2 -> v7.4.2</code></td>
 </table>
 </div>
 </li>
                <li> <span class="li-head">dscp17</span> - Queue number of DSCP 17. <span class="li-normal">type: str</span> <span class="li-normal">choices: queue0, queue1, queue2, queue3, queue4, queue5, queue6, queue7</span>
 <a id='label288' href="javascript:ContentClick('label289', 'label288');" onmouseover="ContentPreview('label289');" onmouseout="ContentUnpreview('label289');" title="click to collapse or expand..."> more... </a>
 <div id="label289" style="display:none">
 <table border="1">
 <tr>
 <td></td>
 <td colspan="1">Supported Version Ranges</td>
 </tr>
 <tr>
 <td>dscp17</td>
 <td><code class="docutils literal notranslate">v7.4.2 -> v7.4.2 </code></td>
 </tr>
 <tr>
 <td>[queue0]</td>
 <td><code class="docutils literal notranslate">v7.4.2 -> v7.4.2</code></td>
 <tr>
 <td>[queue1]</td>
 <td><code class="docutils literal notranslate">v7.4.2 -> v7.4.2</code></td>
 <tr>
 <td>[queue2]</td>
 <td><code class="docutils literal notranslate">v7.4.2 -> v7.4.2</code></td>
 <tr>
 <td>[queue3]</td>
 <td><code class="docutils literal notranslate">v7.4.2 -> v7.4.2</code></td>
 <tr>
 <td>[queue4]</td>
 <td><code class="docutils literal notranslate">v7.4.2 -> v7.4.2</code></td>
 <tr>
 <td>[queue5]</td>
 <td><code class="docutils literal notranslate">v7.4.2 -> v7.4.2</code></td>
 <tr>
 <td>[queue6]</td>
 <td><code class="docutils literal notranslate">v7.4.2 -> v7.4.2</code></td>
 <tr>
 <td>[queue7]</td>
 <td><code class="docutils literal notranslate">v7.4.2 -> v7.4.2</code></td>
 </table>
 </div>
 </li>
                <li> <span class="li-head">dscp18</span> - Queue number of DSCP 18. <span class="li-normal">type: str</span> <span class="li-normal">choices: queue0, queue1, queue2, queue3, queue4, queue5, queue6, queue7</span>
 <a id='label290' href="javascript:ContentClick('label291', 'label290');" onmouseover="ContentPreview('label291');" onmouseout="ContentUnpreview('label291');" title="click to collapse or expand..."> more... </a>
 <div id="label291" style="display:none">
 <table border="1">
 <tr>
 <td></td>
 <td colspan="1">Supported Version Ranges</td>
 </tr>
 <tr>
 <td>dscp18</td>
 <td><code class="docutils literal notranslate">v7.4.2 -> v7.4.2 </code></td>
 </tr>
 <tr>
 <td>[queue0]</td>
 <td><code class="docutils literal notranslate">v7.4.2 -> v7.4.2</code></td>
 <tr>
 <td>[queue1]</td>
 <td><code class="docutils literal notranslate">v7.4.2 -> v7.4.2</code></td>
 <tr>
 <td>[queue2]</td>
 <td><code class="docutils literal notranslate">v7.4.2 -> v7.4.2</code></td>
 <tr>
 <td>[queue3]</td>
 <td><code class="docutils literal notranslate">v7.4.2 -> v7.4.2</code></td>
 <tr>
 <td>[queue4]</td>
 <td><code class="docutils literal notranslate">v7.4.2 -> v7.4.2</code></td>
 <tr>
 <td>[queue5]</td>
 <td><code class="docutils literal notranslate">v7.4.2 -> v7.4.2</code></td>
 <tr>
 <td>[queue6]</td>
 <td><code class="docutils literal notranslate">v7.4.2 -> v7.4.2</code></td>
 <tr>
 <td>[queue7]</td>
 <td><code class="docutils literal notranslate">v7.4.2 -> v7.4.2</code></td>
 </table>
 </div>
 </li>
                <li> <span class="li-head">dscp19</span> - Queue number of DSCP 19. <span class="li-normal">type: str</span> <span class="li-normal">choices: queue0, queue1, queue2, queue3, queue4, queue5, queue6, queue7</span>
 <a id='label292' href="javascript:ContentClick('label293', 'label292');" onmouseover="ContentPreview('label293');" onmouseout="ContentUnpreview('label293');" title="click to collapse or expand..."> more... </a>
 <div id="label293" style="display:none">
 <table border="1">
 <tr>
 <td></td>
 <td colspan="1">Supported Version Ranges</td>
 </tr>
 <tr>
 <td>dscp19</td>
 <td><code class="docutils literal notranslate">v7.4.2 -> v7.4.2 </code></td>
 </tr>
 <tr>
 <td>[queue0]</td>
 <td><code class="docutils literal notranslate">v7.4.2 -> v7.4.2</code></td>
 <tr>
 <td>[queue1]</td>
 <td><code class="docutils literal notranslate">v7.4.2 -> v7.4.2</code></td>
 <tr>
 <td>[queue2]</td>
 <td><code class="docutils literal notranslate">v7.4.2 -> v7.4.2</code></td>
 <tr>
 <td>[queue3]</td>
 <td><code class="docutils literal notranslate">v7.4.2 -> v7.4.2</code></td>
 <tr>
 <td>[queue4]</td>
 <td><code class="docutils literal notranslate">v7.4.2 -> v7.4.2</code></td>
 <tr>
 <td>[queue5]</td>
 <td><code class="docutils literal notranslate">v7.4.2 -> v7.4.2</code></td>
 <tr>
 <td>[queue6]</td>
 <td><code class="docutils literal notranslate">v7.4.2 -> v7.4.2</code></td>
 <tr>
 <td>[queue7]</td>
 <td><code class="docutils literal notranslate">v7.4.2 -> v7.4.2</code></td>
 </table>
 </div>
 </li>
                <li> <span class="li-head">dscp2</span> - Queue number of DSCP 2. <span class="li-normal">type: str</span> <span class="li-normal">choices: queue0, queue1, queue2, queue3, queue4, queue5, queue6, queue7</span>
 <a id='label294' href="javascript:ContentClick('label295', 'label294');" onmouseover="ContentPreview('label295');" onmouseout="ContentUnpreview('label295');" title="click to collapse or expand..."> more... </a>
 <div id="label295" style="display:none">
 <table border="1">
 <tr>
 <td></td>
 <td colspan="1">Supported Version Ranges</td>
 </tr>
 <tr>
 <td>dscp2</td>
 <td><code class="docutils literal notranslate">v7.4.2 -> v7.4.2 </code></td>
 </tr>
 <tr>
 <td>[queue0]</td>
 <td><code class="docutils literal notranslate">v7.4.2 -> v7.4.2</code></td>
 <tr>
 <td>[queue1]</td>
 <td><code class="docutils literal notranslate">v7.4.2 -> v7.4.2</code></td>
 <tr>
 <td>[queue2]</td>
 <td><code class="docutils literal notranslate">v7.4.2 -> v7.4.2</code></td>
 <tr>
 <td>[queue3]</td>
 <td><code class="docutils literal notranslate">v7.4.2 -> v7.4.2</code></td>
 <tr>
 <td>[queue4]</td>
 <td><code class="docutils literal notranslate">v7.4.2 -> v7.4.2</code></td>
 <tr>
 <td>[queue5]</td>
 <td><code class="docutils literal notranslate">v7.4.2 -> v7.4.2</code></td>
 <tr>
 <td>[queue6]</td>
 <td><code class="docutils literal notranslate">v7.4.2 -> v7.4.2</code></td>
 <tr>
 <td>[queue7]</td>
 <td><code class="docutils literal notranslate">v7.4.2 -> v7.4.2</code></td>
 </table>
 </div>
 </li>
                <li> <span class="li-head">dscp20</span> - Queue number of DSCP 20. <span class="li-normal">type: str</span> <span class="li-normal">choices: queue0, queue1, queue2, queue3, queue4, queue5, queue6, queue7</span>
 <a id='label296' href="javascript:ContentClick('label297', 'label296');" onmouseover="ContentPreview('label297');" onmouseout="ContentUnpreview('label297');" title="click to collapse or expand..."> more... </a>
 <div id="label297" style="display:none">
 <table border="1">
 <tr>
 <td></td>
 <td colspan="1">Supported Version Ranges</td>
 </tr>
 <tr>
 <td>dscp20</td>
 <td><code class="docutils literal notranslate">v7.4.2 -> v7.4.2 </code></td>
 </tr>
 <tr>
 <td>[queue0]</td>
 <td><code class="docutils literal notranslate">v7.4.2 -> v7.4.2</code></td>
 <tr>
 <td>[queue1]</td>
 <td><code class="docutils literal notranslate">v7.4.2 -> v7.4.2</code></td>
 <tr>
 <td>[queue2]</td>
 <td><code class="docutils literal notranslate">v7.4.2 -> v7.4.2</code></td>
 <tr>
 <td>[queue3]</td>
 <td><code class="docutils literal notranslate">v7.4.2 -> v7.4.2</code></td>
 <tr>
 <td>[queue4]</td>
 <td><code class="docutils literal notranslate">v7.4.2 -> v7.4.2</code></td>
 <tr>
 <td>[queue5]</td>
 <td><code class="docutils literal notranslate">v7.4.2 -> v7.4.2</code></td>
 <tr>
 <td>[queue6]</td>
 <td><code class="docutils literal notranslate">v7.4.2 -> v7.4.2</code></td>
 <tr>
 <td>[queue7]</td>
 <td><code class="docutils literal notranslate">v7.4.2 -> v7.4.2</code></td>
 </table>
 </div>
 </li>
                <li> <span class="li-head">dscp21</span> - Queue number of DSCP 21. <span class="li-normal">type: str</span> <span class="li-normal">choices: queue0, queue1, queue2, queue3, queue4, queue5, queue6, queue7</span>
 <a id='label298' href="javascript:ContentClick('label299', 'label298');" onmouseover="ContentPreview('label299');" onmouseout="ContentUnpreview('label299');" title="click to collapse or expand..."> more... </a>
 <div id="label299" style="display:none">
 <table border="1">
 <tr>
 <td></td>
 <td colspan="1">Supported Version Ranges</td>
 </tr>
 <tr>
 <td>dscp21</td>
 <td><code class="docutils literal notranslate">v7.4.2 -> v7.4.2 </code></td>
 </tr>
 <tr>
 <td>[queue0]</td>
 <td><code class="docutils literal notranslate">v7.4.2 -> v7.4.2</code></td>
 <tr>
 <td>[queue1]</td>
 <td><code class="docutils literal notranslate">v7.4.2 -> v7.4.2</code></td>
 <tr>
 <td>[queue2]</td>
 <td><code class="docutils literal notranslate">v7.4.2 -> v7.4.2</code></td>
 <tr>
 <td>[queue3]</td>
 <td><code class="docutils literal notranslate">v7.4.2 -> v7.4.2</code></td>
 <tr>
 <td>[queue4]</td>
 <td><code class="docutils literal notranslate">v7.4.2 -> v7.4.2</code></td>
 <tr>
 <td>[queue5]</td>
 <td><code class="docutils literal notranslate">v7.4.2 -> v7.4.2</code></td>
 <tr>
 <td>[queue6]</td>
 <td><code class="docutils literal notranslate">v7.4.2 -> v7.4.2</code></td>
 <tr>
 <td>[queue7]</td>
 <td><code class="docutils literal notranslate">v7.4.2 -> v7.4.2</code></td>
 </table>
 </div>
 </li>
                <li> <span class="li-head">dscp22</span> - Queue number of DSCP 22. <span class="li-normal">type: str</span> <span class="li-normal">choices: queue0, queue1, queue2, queue3, queue4, queue5, queue6, queue7</span>
 <a id='label300' href="javascript:ContentClick('label301', 'label300');" onmouseover="ContentPreview('label301');" onmouseout="ContentUnpreview('label301');" title="click to collapse or expand..."> more... </a>
 <div id="label301" style="display:none">
 <table border="1">
 <tr>
 <td></td>
 <td colspan="1">Supported Version Ranges</td>
 </tr>
 <tr>
 <td>dscp22</td>
 <td><code class="docutils literal notranslate">v7.4.2 -> v7.4.2 </code></td>
 </tr>
 <tr>
 <td>[queue0]</td>
 <td><code class="docutils literal notranslate">v7.4.2 -> v7.4.2</code></td>
 <tr>
 <td>[queue1]</td>
 <td><code class="docutils literal notranslate">v7.4.2 -> v7.4.2</code></td>
 <tr>
 <td>[queue2]</td>
 <td><code class="docutils literal notranslate">v7.4.2 -> v7.4.2</code></td>
 <tr>
 <td>[queue3]</td>
 <td><code class="docutils literal notranslate">v7.4.2 -> v7.4.2</code></td>
 <tr>
 <td>[queue4]</td>
 <td><code class="docutils literal notranslate">v7.4.2 -> v7.4.2</code></td>
 <tr>
 <td>[queue5]</td>
 <td><code class="docutils literal notranslate">v7.4.2 -> v7.4.2</code></td>
 <tr>
 <td>[queue6]</td>
 <td><code class="docutils literal notranslate">v7.4.2 -> v7.4.2</code></td>
 <tr>
 <td>[queue7]</td>
 <td><code class="docutils literal notranslate">v7.4.2 -> v7.4.2</code></td>
 </table>
 </div>
 </li>
                <li> <span class="li-head">dscp23</span> - Queue number of DSCP 23. <span class="li-normal">type: str</span> <span class="li-normal">choices: queue0, queue1, queue2, queue3, queue4, queue5, queue6, queue7</span>
 <a id='label302' href="javascript:ContentClick('label303', 'label302');" onmouseover="ContentPreview('label303');" onmouseout="ContentUnpreview('label303');" title="click to collapse or expand..."> more... </a>
 <div id="label303" style="display:none">
 <table border="1">
 <tr>
 <td></td>
 <td colspan="1">Supported Version Ranges</td>
 </tr>
 <tr>
 <td>dscp23</td>
 <td><code class="docutils literal notranslate">v7.4.2 -> v7.4.2 </code></td>
 </tr>
 <tr>
 <td>[queue0]</td>
 <td><code class="docutils literal notranslate">v7.4.2 -> v7.4.2</code></td>
 <tr>
 <td>[queue1]</td>
 <td><code class="docutils literal notranslate">v7.4.2 -> v7.4.2</code></td>
 <tr>
 <td>[queue2]</td>
 <td><code class="docutils literal notranslate">v7.4.2 -> v7.4.2</code></td>
 <tr>
 <td>[queue3]</td>
 <td><code class="docutils literal notranslate">v7.4.2 -> v7.4.2</code></td>
 <tr>
 <td>[queue4]</td>
 <td><code class="docutils literal notranslate">v7.4.2 -> v7.4.2</code></td>
 <tr>
 <td>[queue5]</td>
 <td><code class="docutils literal notranslate">v7.4.2 -> v7.4.2</code></td>
 <tr>
 <td>[queue6]</td>
 <td><code class="docutils literal notranslate">v7.4.2 -> v7.4.2</code></td>
 <tr>
 <td>[queue7]</td>
 <td><code class="docutils literal notranslate">v7.4.2 -> v7.4.2</code></td>
 </table>
 </div>
 </li>
                <li> <span class="li-head">dscp24</span> - Queue number of DSCP 24. <span class="li-normal">type: str</span> <span class="li-normal">choices: queue0, queue1, queue2, queue3, queue4, queue5, queue6, queue7</span>
 <a id='label304' href="javascript:ContentClick('label305', 'label304');" onmouseover="ContentPreview('label305');" onmouseout="ContentUnpreview('label305');" title="click to collapse or expand..."> more... </a>
 <div id="label305" style="display:none">
 <table border="1">
 <tr>
 <td></td>
 <td colspan="1">Supported Version Ranges</td>
 </tr>
 <tr>
 <td>dscp24</td>
 <td><code class="docutils literal notranslate">v7.4.2 -> v7.4.2 </code></td>
 </tr>
 <tr>
 <td>[queue0]</td>
 <td><code class="docutils literal notranslate">v7.4.2 -> v7.4.2</code></td>
 <tr>
 <td>[queue1]</td>
 <td><code class="docutils literal notranslate">v7.4.2 -> v7.4.2</code></td>
 <tr>
 <td>[queue2]</td>
 <td><code class="docutils literal notranslate">v7.4.2 -> v7.4.2</code></td>
 <tr>
 <td>[queue3]</td>
 <td><code class="docutils literal notranslate">v7.4.2 -> v7.4.2</code></td>
 <tr>
 <td>[queue4]</td>
 <td><code class="docutils literal notranslate">v7.4.2 -> v7.4.2</code></td>
 <tr>
 <td>[queue5]</td>
 <td><code class="docutils literal notranslate">v7.4.2 -> v7.4.2</code></td>
 <tr>
 <td>[queue6]</td>
 <td><code class="docutils literal notranslate">v7.4.2 -> v7.4.2</code></td>
 <tr>
 <td>[queue7]</td>
 <td><code class="docutils literal notranslate">v7.4.2 -> v7.4.2</code></td>
 </table>
 </div>
 </li>
                <li> <span class="li-head">dscp25</span> - Queue number of DSCP 25. <span class="li-normal">type: str</span> <span class="li-normal">choices: queue0, queue1, queue2, queue3, queue4, queue5, queue6, queue7</span>
 <a id='label306' href="javascript:ContentClick('label307', 'label306');" onmouseover="ContentPreview('label307');" onmouseout="ContentUnpreview('label307');" title="click to collapse or expand..."> more... </a>
 <div id="label307" style="display:none">
 <table border="1">
 <tr>
 <td></td>
 <td colspan="1">Supported Version Ranges</td>
 </tr>
 <tr>
 <td>dscp25</td>
 <td><code class="docutils literal notranslate">v7.4.2 -> v7.4.2 </code></td>
 </tr>
 <tr>
 <td>[queue0]</td>
 <td><code class="docutils literal notranslate">v7.4.2 -> v7.4.2</code></td>
 <tr>
 <td>[queue1]</td>
 <td><code class="docutils literal notranslate">v7.4.2 -> v7.4.2</code></td>
 <tr>
 <td>[queue2]</td>
 <td><code class="docutils literal notranslate">v7.4.2 -> v7.4.2</code></td>
 <tr>
 <td>[queue3]</td>
 <td><code class="docutils literal notranslate">v7.4.2 -> v7.4.2</code></td>
 <tr>
 <td>[queue4]</td>
 <td><code class="docutils literal notranslate">v7.4.2 -> v7.4.2</code></td>
 <tr>
 <td>[queue5]</td>
 <td><code class="docutils literal notranslate">v7.4.2 -> v7.4.2</code></td>
 <tr>
 <td>[queue6]</td>
 <td><code class="docutils literal notranslate">v7.4.2 -> v7.4.2</code></td>
 <tr>
 <td>[queue7]</td>
 <td><code class="docutils literal notranslate">v7.4.2 -> v7.4.2</code></td>
 </table>
 </div>
 </li>
                <li> <span class="li-head">dscp26</span> - Queue number of DSCP 26. <span class="li-normal">type: str</span> <span class="li-normal">choices: queue0, queue1, queue2, queue3, queue4, queue5, queue6, queue7</span>
 <a id='label308' href="javascript:ContentClick('label309', 'label308');" onmouseover="ContentPreview('label309');" onmouseout="ContentUnpreview('label309');" title="click to collapse or expand..."> more... </a>
 <div id="label309" style="display:none">
 <table border="1">
 <tr>
 <td></td>
 <td colspan="1">Supported Version Ranges</td>
 </tr>
 <tr>
 <td>dscp26</td>
 <td><code class="docutils literal notranslate">v7.4.2 -> v7.4.2 </code></td>
 </tr>
 <tr>
 <td>[queue0]</td>
 <td><code class="docutils literal notranslate">v7.4.2 -> v7.4.2</code></td>
 <tr>
 <td>[queue1]</td>
 <td><code class="docutils literal notranslate">v7.4.2 -> v7.4.2</code></td>
 <tr>
 <td>[queue2]</td>
 <td><code class="docutils literal notranslate">v7.4.2 -> v7.4.2</code></td>
 <tr>
 <td>[queue3]</td>
 <td><code class="docutils literal notranslate">v7.4.2 -> v7.4.2</code></td>
 <tr>
 <td>[queue4]</td>
 <td><code class="docutils literal notranslate">v7.4.2 -> v7.4.2</code></td>
 <tr>
 <td>[queue5]</td>
 <td><code class="docutils literal notranslate">v7.4.2 -> v7.4.2</code></td>
 <tr>
 <td>[queue6]</td>
 <td><code class="docutils literal notranslate">v7.4.2 -> v7.4.2</code></td>
 <tr>
 <td>[queue7]</td>
 <td><code class="docutils literal notranslate">v7.4.2 -> v7.4.2</code></td>
 </table>
 </div>
 </li>
                <li> <span class="li-head">dscp27</span> - Queue number of DSCP 27. <span class="li-normal">type: str</span> <span class="li-normal">choices: queue0, queue1, queue2, queue3, queue4, queue5, queue6, queue7</span>
 <a id='label310' href="javascript:ContentClick('label311', 'label310');" onmouseover="ContentPreview('label311');" onmouseout="ContentUnpreview('label311');" title="click to collapse or expand..."> more... </a>
 <div id="label311" style="display:none">
 <table border="1">
 <tr>
 <td></td>
 <td colspan="1">Supported Version Ranges</td>
 </tr>
 <tr>
 <td>dscp27</td>
 <td><code class="docutils literal notranslate">v7.4.2 -> v7.4.2 </code></td>
 </tr>
 <tr>
 <td>[queue0]</td>
 <td><code class="docutils literal notranslate">v7.4.2 -> v7.4.2</code></td>
 <tr>
 <td>[queue1]</td>
 <td><code class="docutils literal notranslate">v7.4.2 -> v7.4.2</code></td>
 <tr>
 <td>[queue2]</td>
 <td><code class="docutils literal notranslate">v7.4.2 -> v7.4.2</code></td>
 <tr>
 <td>[queue3]</td>
 <td><code class="docutils literal notranslate">v7.4.2 -> v7.4.2</code></td>
 <tr>
 <td>[queue4]</td>
 <td><code class="docutils literal notranslate">v7.4.2 -> v7.4.2</code></td>
 <tr>
 <td>[queue5]</td>
 <td><code class="docutils literal notranslate">v7.4.2 -> v7.4.2</code></td>
 <tr>
 <td>[queue6]</td>
 <td><code class="docutils literal notranslate">v7.4.2 -> v7.4.2</code></td>
 <tr>
 <td>[queue7]</td>
 <td><code class="docutils literal notranslate">v7.4.2 -> v7.4.2</code></td>
 </table>
 </div>
 </li>
                <li> <span class="li-head">dscp28</span> - Queue number of DSCP 28. <span class="li-normal">type: str</span> <span class="li-normal">choices: queue0, queue1, queue2, queue3, queue4, queue5, queue6, queue7</span>
 <a id='label312' href="javascript:ContentClick('label313', 'label312');" onmouseover="ContentPreview('label313');" onmouseout="ContentUnpreview('label313');" title="click to collapse or expand..."> more... </a>
 <div id="label313" style="display:none">
 <table border="1">
 <tr>
 <td></td>
 <td colspan="1">Supported Version Ranges</td>
 </tr>
 <tr>
 <td>dscp28</td>
 <td><code class="docutils literal notranslate">v7.4.2 -> v7.4.2 </code></td>
 </tr>
 <tr>
 <td>[queue0]</td>
 <td><code class="docutils literal notranslate">v7.4.2 -> v7.4.2</code></td>
 <tr>
 <td>[queue1]</td>
 <td><code class="docutils literal notranslate">v7.4.2 -> v7.4.2</code></td>
 <tr>
 <td>[queue2]</td>
 <td><code class="docutils literal notranslate">v7.4.2 -> v7.4.2</code></td>
 <tr>
 <td>[queue3]</td>
 <td><code class="docutils literal notranslate">v7.4.2 -> v7.4.2</code></td>
 <tr>
 <td>[queue4]</td>
 <td><code class="docutils literal notranslate">v7.4.2 -> v7.4.2</code></td>
 <tr>
 <td>[queue5]</td>
 <td><code class="docutils literal notranslate">v7.4.2 -> v7.4.2</code></td>
 <tr>
 <td>[queue6]</td>
 <td><code class="docutils literal notranslate">v7.4.2 -> v7.4.2</code></td>
 <tr>
 <td>[queue7]</td>
 <td><code class="docutils literal notranslate">v7.4.2 -> v7.4.2</code></td>
 </table>
 </div>
 </li>
                <li> <span class="li-head">dscp29</span> - Queue number of DSCP 29. <span class="li-normal">type: str</span> <span class="li-normal">choices: queue0, queue1, queue2, queue3, queue4, queue5, queue6, queue7</span>
 <a id='label314' href="javascript:ContentClick('label315', 'label314');" onmouseover="ContentPreview('label315');" onmouseout="ContentUnpreview('label315');" title="click to collapse or expand..."> more... </a>
 <div id="label315" style="display:none">
 <table border="1">
 <tr>
 <td></td>
 <td colspan="1">Supported Version Ranges</td>
 </tr>
 <tr>
 <td>dscp29</td>
 <td><code class="docutils literal notranslate">v7.4.2 -> v7.4.2 </code></td>
 </tr>
 <tr>
 <td>[queue0]</td>
 <td><code class="docutils literal notranslate">v7.4.2 -> v7.4.2</code></td>
 <tr>
 <td>[queue1]</td>
 <td><code class="docutils literal notranslate">v7.4.2 -> v7.4.2</code></td>
 <tr>
 <td>[queue2]</td>
 <td><code class="docutils literal notranslate">v7.4.2 -> v7.4.2</code></td>
 <tr>
 <td>[queue3]</td>
 <td><code class="docutils literal notranslate">v7.4.2 -> v7.4.2</code></td>
 <tr>
 <td>[queue4]</td>
 <td><code class="docutils literal notranslate">v7.4.2 -> v7.4.2</code></td>
 <tr>
 <td>[queue5]</td>
 <td><code class="docutils literal notranslate">v7.4.2 -> v7.4.2</code></td>
 <tr>
 <td>[queue6]</td>
 <td><code class="docutils literal notranslate">v7.4.2 -> v7.4.2</code></td>
 <tr>
 <td>[queue7]</td>
 <td><code class="docutils literal notranslate">v7.4.2 -> v7.4.2</code></td>
 </table>
 </div>
 </li>
                <li> <span class="li-head">dscp3</span> - Queue number of DSCP 3. <span class="li-normal">type: str</span> <span class="li-normal">choices: queue0, queue1, queue2, queue3, queue4, queue5, queue6, queue7</span>
 <a id='label316' href="javascript:ContentClick('label317', 'label316');" onmouseover="ContentPreview('label317');" onmouseout="ContentUnpreview('label317');" title="click to collapse or expand..."> more... </a>
 <div id="label317" style="display:none">
 <table border="1">
 <tr>
 <td></td>
 <td colspan="1">Supported Version Ranges</td>
 </tr>
 <tr>
 <td>dscp3</td>
 <td><code class="docutils literal notranslate">v7.4.2 -> v7.4.2 </code></td>
 </tr>
 <tr>
 <td>[queue0]</td>
 <td><code class="docutils literal notranslate">v7.4.2 -> v7.4.2</code></td>
 <tr>
 <td>[queue1]</td>
 <td><code class="docutils literal notranslate">v7.4.2 -> v7.4.2</code></td>
 <tr>
 <td>[queue2]</td>
 <td><code class="docutils literal notranslate">v7.4.2 -> v7.4.2</code></td>
 <tr>
 <td>[queue3]</td>
 <td><code class="docutils literal notranslate">v7.4.2 -> v7.4.2</code></td>
 <tr>
 <td>[queue4]</td>
 <td><code class="docutils literal notranslate">v7.4.2 -> v7.4.2</code></td>
 <tr>
 <td>[queue5]</td>
 <td><code class="docutils literal notranslate">v7.4.2 -> v7.4.2</code></td>
 <tr>
 <td>[queue6]</td>
 <td><code class="docutils literal notranslate">v7.4.2 -> v7.4.2</code></td>
 <tr>
 <td>[queue7]</td>
 <td><code class="docutils literal notranslate">v7.4.2 -> v7.4.2</code></td>
 </table>
 </div>
 </li>
                <li> <span class="li-head">dscp30</span> - Queue number of DSCP 30. <span class="li-normal">type: str</span> <span class="li-normal">choices: queue0, queue1, queue2, queue3, queue4, queue5, queue6, queue7</span>
 <a id='label318' href="javascript:ContentClick('label319', 'label318');" onmouseover="ContentPreview('label319');" onmouseout="ContentUnpreview('label319');" title="click to collapse or expand..."> more... </a>
 <div id="label319" style="display:none">
 <table border="1">
 <tr>
 <td></td>
 <td colspan="1">Supported Version Ranges</td>
 </tr>
 <tr>
 <td>dscp30</td>
 <td><code class="docutils literal notranslate">v7.4.2 -> v7.4.2 </code></td>
 </tr>
 <tr>
 <td>[queue0]</td>
 <td><code class="docutils literal notranslate">v7.4.2 -> v7.4.2</code></td>
 <tr>
 <td>[queue1]</td>
 <td><code class="docutils literal notranslate">v7.4.2 -> v7.4.2</code></td>
 <tr>
 <td>[queue2]</td>
 <td><code class="docutils literal notranslate">v7.4.2 -> v7.4.2</code></td>
 <tr>
 <td>[queue3]</td>
 <td><code class="docutils literal notranslate">v7.4.2 -> v7.4.2</code></td>
 <tr>
 <td>[queue4]</td>
 <td><code class="docutils literal notranslate">v7.4.2 -> v7.4.2</code></td>
 <tr>
 <td>[queue5]</td>
 <td><code class="docutils literal notranslate">v7.4.2 -> v7.4.2</code></td>
 <tr>
 <td>[queue6]</td>
 <td><code class="docutils literal notranslate">v7.4.2 -> v7.4.2</code></td>
 <tr>
 <td>[queue7]</td>
 <td><code class="docutils literal notranslate">v7.4.2 -> v7.4.2</code></td>
 </table>
 </div>
 </li>
                <li> <span class="li-head">dscp31</span> - Queue number of DSCP 31. <span class="li-normal">type: str</span> <span class="li-normal">choices: queue0, queue1, queue2, queue3, queue4, queue5, queue6, queue7</span>
 <a id='label320' href="javascript:ContentClick('label321', 'label320');" onmouseover="ContentPreview('label321');" onmouseout="ContentUnpreview('label321');" title="click to collapse or expand..."> more... </a>
 <div id="label321" style="display:none">
 <table border="1">
 <tr>
 <td></td>
 <td colspan="1">Supported Version Ranges</td>
 </tr>
 <tr>
 <td>dscp31</td>
 <td><code class="docutils literal notranslate">v7.4.2 -> v7.4.2 </code></td>
 </tr>
 <tr>
 <td>[queue0]</td>
 <td><code class="docutils literal notranslate">v7.4.2 -> v7.4.2</code></td>
 <tr>
 <td>[queue1]</td>
 <td><code class="docutils literal notranslate">v7.4.2 -> v7.4.2</code></td>
 <tr>
 <td>[queue2]</td>
 <td><code class="docutils literal notranslate">v7.4.2 -> v7.4.2</code></td>
 <tr>
 <td>[queue3]</td>
 <td><code class="docutils literal notranslate">v7.4.2 -> v7.4.2</code></td>
 <tr>
 <td>[queue4]</td>
 <td><code class="docutils literal notranslate">v7.4.2 -> v7.4.2</code></td>
 <tr>
 <td>[queue5]</td>
 <td><code class="docutils literal notranslate">v7.4.2 -> v7.4.2</code></td>
 <tr>
 <td>[queue6]</td>
 <td><code class="docutils literal notranslate">v7.4.2 -> v7.4.2</code></td>
 <tr>
 <td>[queue7]</td>
 <td><code class="docutils literal notranslate">v7.4.2 -> v7.4.2</code></td>
 </table>
 </div>
 </li>
                <li> <span class="li-head">dscp32</span> - Queue number of DSCP 32. <span class="li-normal">type: str</span> <span class="li-normal">choices: queue0, queue1, queue2, queue3, queue4, queue5, queue6, queue7</span>
 <a id='label322' href="javascript:ContentClick('label323', 'label322');" onmouseover="ContentPreview('label323');" onmouseout="ContentUnpreview('label323');" title="click to collapse or expand..."> more... </a>
 <div id="label323" style="display:none">
 <table border="1">
 <tr>
 <td></td>
 <td colspan="1">Supported Version Ranges</td>
 </tr>
 <tr>
 <td>dscp32</td>
 <td><code class="docutils literal notranslate">v7.4.2 -> v7.4.2 </code></td>
 </tr>
 <tr>
 <td>[queue0]</td>
 <td><code class="docutils literal notranslate">v7.4.2 -> v7.4.2</code></td>
 <tr>
 <td>[queue1]</td>
 <td><code class="docutils literal notranslate">v7.4.2 -> v7.4.2</code></td>
 <tr>
 <td>[queue2]</td>
 <td><code class="docutils literal notranslate">v7.4.2 -> v7.4.2</code></td>
 <tr>
 <td>[queue3]</td>
 <td><code class="docutils literal notranslate">v7.4.2 -> v7.4.2</code></td>
 <tr>
 <td>[queue4]</td>
 <td><code class="docutils literal notranslate">v7.4.2 -> v7.4.2</code></td>
 <tr>
 <td>[queue5]</td>
 <td><code class="docutils literal notranslate">v7.4.2 -> v7.4.2</code></td>
 <tr>
 <td>[queue6]</td>
 <td><code class="docutils literal notranslate">v7.4.2 -> v7.4.2</code></td>
 <tr>
 <td>[queue7]</td>
 <td><code class="docutils literal notranslate">v7.4.2 -> v7.4.2</code></td>
 </table>
 </div>
 </li>
                <li> <span class="li-head">dscp33</span> - Queue number of DSCP 33. <span class="li-normal">type: str</span> <span class="li-normal">choices: queue0, queue1, queue2, queue3, queue4, queue5, queue6, queue7</span>
 <a id='label324' href="javascript:ContentClick('label325', 'label324');" onmouseover="ContentPreview('label325');" onmouseout="ContentUnpreview('label325');" title="click to collapse or expand..."> more... </a>
 <div id="label325" style="display:none">
 <table border="1">
 <tr>
 <td></td>
 <td colspan="1">Supported Version Ranges</td>
 </tr>
 <tr>
 <td>dscp33</td>
 <td><code class="docutils literal notranslate">v7.4.2 -> v7.4.2 </code></td>
 </tr>
 <tr>
 <td>[queue0]</td>
 <td><code class="docutils literal notranslate">v7.4.2 -> v7.4.2</code></td>
 <tr>
 <td>[queue1]</td>
 <td><code class="docutils literal notranslate">v7.4.2 -> v7.4.2</code></td>
 <tr>
 <td>[queue2]</td>
 <td><code class="docutils literal notranslate">v7.4.2 -> v7.4.2</code></td>
 <tr>
 <td>[queue3]</td>
 <td><code class="docutils literal notranslate">v7.4.2 -> v7.4.2</code></td>
 <tr>
 <td>[queue4]</td>
 <td><code class="docutils literal notranslate">v7.4.2 -> v7.4.2</code></td>
 <tr>
 <td>[queue5]</td>
 <td><code class="docutils literal notranslate">v7.4.2 -> v7.4.2</code></td>
 <tr>
 <td>[queue6]</td>
 <td><code class="docutils literal notranslate">v7.4.2 -> v7.4.2</code></td>
 <tr>
 <td>[queue7]</td>
 <td><code class="docutils literal notranslate">v7.4.2 -> v7.4.2</code></td>
 </table>
 </div>
 </li>
                <li> <span class="li-head">dscp34</span> - Queue number of DSCP 34. <span class="li-normal">type: str</span> <span class="li-normal">choices: queue0, queue1, queue2, queue3, queue4, queue5, queue6, queue7</span>
 <a id='label326' href="javascript:ContentClick('label327', 'label326');" onmouseover="ContentPreview('label327');" onmouseout="ContentUnpreview('label327');" title="click to collapse or expand..."> more... </a>
 <div id="label327" style="display:none">
 <table border="1">
 <tr>
 <td></td>
 <td colspan="1">Supported Version Ranges</td>
 </tr>
 <tr>
 <td>dscp34</td>
 <td><code class="docutils literal notranslate">v7.4.2 -> v7.4.2 </code></td>
 </tr>
 <tr>
 <td>[queue0]</td>
 <td><code class="docutils literal notranslate">v7.4.2 -> v7.4.2</code></td>
 <tr>
 <td>[queue1]</td>
 <td><code class="docutils literal notranslate">v7.4.2 -> v7.4.2</code></td>
 <tr>
 <td>[queue2]</td>
 <td><code class="docutils literal notranslate">v7.4.2 -> v7.4.2</code></td>
 <tr>
 <td>[queue3]</td>
 <td><code class="docutils literal notranslate">v7.4.2 -> v7.4.2</code></td>
 <tr>
 <td>[queue4]</td>
 <td><code class="docutils literal notranslate">v7.4.2 -> v7.4.2</code></td>
 <tr>
 <td>[queue5]</td>
 <td><code class="docutils literal notranslate">v7.4.2 -> v7.4.2</code></td>
 <tr>
 <td>[queue6]</td>
 <td><code class="docutils literal notranslate">v7.4.2 -> v7.4.2</code></td>
 <tr>
 <td>[queue7]</td>
 <td><code class="docutils literal notranslate">v7.4.2 -> v7.4.2</code></td>
 </table>
 </div>
 </li>
                <li> <span class="li-head">dscp35</span> - Queue number of DSCP 35. <span class="li-normal">type: str</span> <span class="li-normal">choices: queue0, queue1, queue2, queue3, queue4, queue5, queue6, queue7</span>
 <a id='label328' href="javascript:ContentClick('label329', 'label328');" onmouseover="ContentPreview('label329');" onmouseout="ContentUnpreview('label329');" title="click to collapse or expand..."> more... </a>
 <div id="label329" style="display:none">
 <table border="1">
 <tr>
 <td></td>
 <td colspan="1">Supported Version Ranges</td>
 </tr>
 <tr>
 <td>dscp35</td>
 <td><code class="docutils literal notranslate">v7.4.2 -> v7.4.2 </code></td>
 </tr>
 <tr>
 <td>[queue0]</td>
 <td><code class="docutils literal notranslate">v7.4.2 -> v7.4.2</code></td>
 <tr>
 <td>[queue1]</td>
 <td><code class="docutils literal notranslate">v7.4.2 -> v7.4.2</code></td>
 <tr>
 <td>[queue2]</td>
 <td><code class="docutils literal notranslate">v7.4.2 -> v7.4.2</code></td>
 <tr>
 <td>[queue3]</td>
 <td><code class="docutils literal notranslate">v7.4.2 -> v7.4.2</code></td>
 <tr>
 <td>[queue4]</td>
 <td><code class="docutils literal notranslate">v7.4.2 -> v7.4.2</code></td>
 <tr>
 <td>[queue5]</td>
 <td><code class="docutils literal notranslate">v7.4.2 -> v7.4.2</code></td>
 <tr>
 <td>[queue6]</td>
 <td><code class="docutils literal notranslate">v7.4.2 -> v7.4.2</code></td>
 <tr>
 <td>[queue7]</td>
 <td><code class="docutils literal notranslate">v7.4.2 -> v7.4.2</code></td>
 </table>
 </div>
 </li>
                <li> <span class="li-head">dscp36</span> - Queue number of DSCP 36. <span class="li-normal">type: str</span> <span class="li-normal">choices: queue0, queue1, queue2, queue3, queue4, queue5, queue6, queue7</span>
 <a id='label330' href="javascript:ContentClick('label331', 'label330');" onmouseover="ContentPreview('label331');" onmouseout="ContentUnpreview('label331');" title="click to collapse or expand..."> more... </a>
 <div id="label331" style="display:none">
 <table border="1">
 <tr>
 <td></td>
 <td colspan="1">Supported Version Ranges</td>
 </tr>
 <tr>
 <td>dscp36</td>
 <td><code class="docutils literal notranslate">v7.4.2 -> v7.4.2 </code></td>
 </tr>
 <tr>
 <td>[queue0]</td>
 <td><code class="docutils literal notranslate">v7.4.2 -> v7.4.2</code></td>
 <tr>
 <td>[queue1]</td>
 <td><code class="docutils literal notranslate">v7.4.2 -> v7.4.2</code></td>
 <tr>
 <td>[queue2]</td>
 <td><code class="docutils literal notranslate">v7.4.2 -> v7.4.2</code></td>
 <tr>
 <td>[queue3]</td>
 <td><code class="docutils literal notranslate">v7.4.2 -> v7.4.2</code></td>
 <tr>
 <td>[queue4]</td>
 <td><code class="docutils literal notranslate">v7.4.2 -> v7.4.2</code></td>
 <tr>
 <td>[queue5]</td>
 <td><code class="docutils literal notranslate">v7.4.2 -> v7.4.2</code></td>
 <tr>
 <td>[queue6]</td>
 <td><code class="docutils literal notranslate">v7.4.2 -> v7.4.2</code></td>
 <tr>
 <td>[queue7]</td>
 <td><code class="docutils literal notranslate">v7.4.2 -> v7.4.2</code></td>
 </table>
 </div>
 </li>
                <li> <span class="li-head">dscp37</span> - Queue number of DSCP 37. <span class="li-normal">type: str</span> <span class="li-normal">choices: queue0, queue1, queue2, queue3, queue4, queue5, queue6, queue7</span>
 <a id='label332' href="javascript:ContentClick('label333', 'label332');" onmouseover="ContentPreview('label333');" onmouseout="ContentUnpreview('label333');" title="click to collapse or expand..."> more... </a>
 <div id="label333" style="display:none">
 <table border="1">
 <tr>
 <td></td>
 <td colspan="1">Supported Version Ranges</td>
 </tr>
 <tr>
 <td>dscp37</td>
 <td><code class="docutils literal notranslate">v7.4.2 -> v7.4.2 </code></td>
 </tr>
 <tr>
 <td>[queue0]</td>
 <td><code class="docutils literal notranslate">v7.4.2 -> v7.4.2</code></td>
 <tr>
 <td>[queue1]</td>
 <td><code class="docutils literal notranslate">v7.4.2 -> v7.4.2</code></td>
 <tr>
 <td>[queue2]</td>
 <td><code class="docutils literal notranslate">v7.4.2 -> v7.4.2</code></td>
 <tr>
 <td>[queue3]</td>
 <td><code class="docutils literal notranslate">v7.4.2 -> v7.4.2</code></td>
 <tr>
 <td>[queue4]</td>
 <td><code class="docutils literal notranslate">v7.4.2 -> v7.4.2</code></td>
 <tr>
 <td>[queue5]</td>
 <td><code class="docutils literal notranslate">v7.4.2 -> v7.4.2</code></td>
 <tr>
 <td>[queue6]</td>
 <td><code class="docutils literal notranslate">v7.4.2 -> v7.4.2</code></td>
 <tr>
 <td>[queue7]</td>
 <td><code class="docutils literal notranslate">v7.4.2 -> v7.4.2</code></td>
 </table>
 </div>
 </li>
                <li> <span class="li-head">dscp38</span> - Queue number of DSCP 38. <span class="li-normal">type: str</span> <span class="li-normal">choices: queue0, queue1, queue2, queue3, queue4, queue5, queue6, queue7</span>
 <a id='label334' href="javascript:ContentClick('label335', 'label334');" onmouseover="ContentPreview('label335');" onmouseout="ContentUnpreview('label335');" title="click to collapse or expand..."> more... </a>
 <div id="label335" style="display:none">
 <table border="1">
 <tr>
 <td></td>
 <td colspan="1">Supported Version Ranges</td>
 </tr>
 <tr>
 <td>dscp38</td>
 <td><code class="docutils literal notranslate">v7.4.2 -> v7.4.2 </code></td>
 </tr>
 <tr>
 <td>[queue0]</td>
 <td><code class="docutils literal notranslate">v7.4.2 -> v7.4.2</code></td>
 <tr>
 <td>[queue1]</td>
 <td><code class="docutils literal notranslate">v7.4.2 -> v7.4.2</code></td>
 <tr>
 <td>[queue2]</td>
 <td><code class="docutils literal notranslate">v7.4.2 -> v7.4.2</code></td>
 <tr>
 <td>[queue3]</td>
 <td><code class="docutils literal notranslate">v7.4.2 -> v7.4.2</code></td>
 <tr>
 <td>[queue4]</td>
 <td><code class="docutils literal notranslate">v7.4.2 -> v7.4.2</code></td>
 <tr>
 <td>[queue5]</td>
 <td><code class="docutils literal notranslate">v7.4.2 -> v7.4.2</code></td>
 <tr>
 <td>[queue6]</td>
 <td><code class="docutils literal notranslate">v7.4.2 -> v7.4.2</code></td>
 <tr>
 <td>[queue7]</td>
 <td><code class="docutils literal notranslate">v7.4.2 -> v7.4.2</code></td>
 </table>
 </div>
 </li>
                <li> <span class="li-head">dscp39</span> - Queue number of DSCP 39. <span class="li-normal">type: str</span> <span class="li-normal">choices: queue0, queue1, queue2, queue3, queue4, queue5, queue6, queue7</span>
 <a id='label336' href="javascript:ContentClick('label337', 'label336');" onmouseover="ContentPreview('label337');" onmouseout="ContentUnpreview('label337');" title="click to collapse or expand..."> more... </a>
 <div id="label337" style="display:none">
 <table border="1">
 <tr>
 <td></td>
 <td colspan="1">Supported Version Ranges</td>
 </tr>
 <tr>
 <td>dscp39</td>
 <td><code class="docutils literal notranslate">v7.4.2 -> v7.4.2 </code></td>
 </tr>
 <tr>
 <td>[queue0]</td>
 <td><code class="docutils literal notranslate">v7.4.2 -> v7.4.2</code></td>
 <tr>
 <td>[queue1]</td>
 <td><code class="docutils literal notranslate">v7.4.2 -> v7.4.2</code></td>
 <tr>
 <td>[queue2]</td>
 <td><code class="docutils literal notranslate">v7.4.2 -> v7.4.2</code></td>
 <tr>
 <td>[queue3]</td>
 <td><code class="docutils literal notranslate">v7.4.2 -> v7.4.2</code></td>
 <tr>
 <td>[queue4]</td>
 <td><code class="docutils literal notranslate">v7.4.2 -> v7.4.2</code></td>
 <tr>
 <td>[queue5]</td>
 <td><code class="docutils literal notranslate">v7.4.2 -> v7.4.2</code></td>
 <tr>
 <td>[queue6]</td>
 <td><code class="docutils literal notranslate">v7.4.2 -> v7.4.2</code></td>
 <tr>
 <td>[queue7]</td>
 <td><code class="docutils literal notranslate">v7.4.2 -> v7.4.2</code></td>
 </table>
 </div>
 </li>
                <li> <span class="li-head">dscp4</span> - Queue number of DSCP 4. <span class="li-normal">type: str</span> <span class="li-normal">choices: queue0, queue1, queue2, queue3, queue4, queue5, queue6, queue7</span>
 <a id='label338' href="javascript:ContentClick('label339', 'label338');" onmouseover="ContentPreview('label339');" onmouseout="ContentUnpreview('label339');" title="click to collapse or expand..."> more... </a>
 <div id="label339" style="display:none">
 <table border="1">
 <tr>
 <td></td>
 <td colspan="1">Supported Version Ranges</td>
 </tr>
 <tr>
 <td>dscp4</td>
 <td><code class="docutils literal notranslate">v7.4.2 -> v7.4.2 </code></td>
 </tr>
 <tr>
 <td>[queue0]</td>
 <td><code class="docutils literal notranslate">v7.4.2 -> v7.4.2</code></td>
 <tr>
 <td>[queue1]</td>
 <td><code class="docutils literal notranslate">v7.4.2 -> v7.4.2</code></td>
 <tr>
 <td>[queue2]</td>
 <td><code class="docutils literal notranslate">v7.4.2 -> v7.4.2</code></td>
 <tr>
 <td>[queue3]</td>
 <td><code class="docutils literal notranslate">v7.4.2 -> v7.4.2</code></td>
 <tr>
 <td>[queue4]</td>
 <td><code class="docutils literal notranslate">v7.4.2 -> v7.4.2</code></td>
 <tr>
 <td>[queue5]</td>
 <td><code class="docutils literal notranslate">v7.4.2 -> v7.4.2</code></td>
 <tr>
 <td>[queue6]</td>
 <td><code class="docutils literal notranslate">v7.4.2 -> v7.4.2</code></td>
 <tr>
 <td>[queue7]</td>
 <td><code class="docutils literal notranslate">v7.4.2 -> v7.4.2</code></td>
 </table>
 </div>
 </li>
                <li> <span class="li-head">dscp40</span> - Queue number of DSCP 40. <span class="li-normal">type: str</span> <span class="li-normal">choices: queue0, queue1, queue2, queue3, queue4, queue5, queue6, queue7</span>
 <a id='label340' href="javascript:ContentClick('label341', 'label340');" onmouseover="ContentPreview('label341');" onmouseout="ContentUnpreview('label341');" title="click to collapse or expand..."> more... </a>
 <div id="label341" style="display:none">
 <table border="1">
 <tr>
 <td></td>
 <td colspan="1">Supported Version Ranges</td>
 </tr>
 <tr>
 <td>dscp40</td>
 <td><code class="docutils literal notranslate">v7.4.2 -> v7.4.2 </code></td>
 </tr>
 <tr>
 <td>[queue0]</td>
 <td><code class="docutils literal notranslate">v7.4.2 -> v7.4.2</code></td>
 <tr>
 <td>[queue1]</td>
 <td><code class="docutils literal notranslate">v7.4.2 -> v7.4.2</code></td>
 <tr>
 <td>[queue2]</td>
 <td><code class="docutils literal notranslate">v7.4.2 -> v7.4.2</code></td>
 <tr>
 <td>[queue3]</td>
 <td><code class="docutils literal notranslate">v7.4.2 -> v7.4.2</code></td>
 <tr>
 <td>[queue4]</td>
 <td><code class="docutils literal notranslate">v7.4.2 -> v7.4.2</code></td>
 <tr>
 <td>[queue5]</td>
 <td><code class="docutils literal notranslate">v7.4.2 -> v7.4.2</code></td>
 <tr>
 <td>[queue6]</td>
 <td><code class="docutils literal notranslate">v7.4.2 -> v7.4.2</code></td>
 <tr>
 <td>[queue7]</td>
 <td><code class="docutils literal notranslate">v7.4.2 -> v7.4.2</code></td>
 </table>
 </div>
 </li>
                <li> <span class="li-head">dscp41</span> - Queue number of DSCP 41. <span class="li-normal">type: str</span> <span class="li-normal">choices: queue0, queue1, queue2, queue3, queue4, queue5, queue6, queue7</span>
 <a id='label342' href="javascript:ContentClick('label343', 'label342');" onmouseover="ContentPreview('label343');" onmouseout="ContentUnpreview('label343');" title="click to collapse or expand..."> more... </a>
 <div id="label343" style="display:none">
 <table border="1">
 <tr>
 <td></td>
 <td colspan="1">Supported Version Ranges</td>
 </tr>
 <tr>
 <td>dscp41</td>
 <td><code class="docutils literal notranslate">v7.4.2 -> v7.4.2 </code></td>
 </tr>
 <tr>
 <td>[queue0]</td>
 <td><code class="docutils literal notranslate">v7.4.2 -> v7.4.2</code></td>
 <tr>
 <td>[queue1]</td>
 <td><code class="docutils literal notranslate">v7.4.2 -> v7.4.2</code></td>
 <tr>
 <td>[queue2]</td>
 <td><code class="docutils literal notranslate">v7.4.2 -> v7.4.2</code></td>
 <tr>
 <td>[queue3]</td>
 <td><code class="docutils literal notranslate">v7.4.2 -> v7.4.2</code></td>
 <tr>
 <td>[queue4]</td>
 <td><code class="docutils literal notranslate">v7.4.2 -> v7.4.2</code></td>
 <tr>
 <td>[queue5]</td>
 <td><code class="docutils literal notranslate">v7.4.2 -> v7.4.2</code></td>
 <tr>
 <td>[queue6]</td>
 <td><code class="docutils literal notranslate">v7.4.2 -> v7.4.2</code></td>
 <tr>
 <td>[queue7]</td>
 <td><code class="docutils literal notranslate">v7.4.2 -> v7.4.2</code></td>
 </table>
 </div>
 </li>
                <li> <span class="li-head">dscp42</span> - Queue number of DSCP 42. <span class="li-normal">type: str</span> <span class="li-normal">choices: queue0, queue1, queue2, queue3, queue4, queue5, queue6, queue7</span>
 <a id='label344' href="javascript:ContentClick('label345', 'label344');" onmouseover="ContentPreview('label345');" onmouseout="ContentUnpreview('label345');" title="click to collapse or expand..."> more... </a>
 <div id="label345" style="display:none">
 <table border="1">
 <tr>
 <td></td>
 <td colspan="1">Supported Version Ranges</td>
 </tr>
 <tr>
 <td>dscp42</td>
 <td><code class="docutils literal notranslate">v7.4.2 -> v7.4.2 </code></td>
 </tr>
 <tr>
 <td>[queue0]</td>
 <td><code class="docutils literal notranslate">v7.4.2 -> v7.4.2</code></td>
 <tr>
 <td>[queue1]</td>
 <td><code class="docutils literal notranslate">v7.4.2 -> v7.4.2</code></td>
 <tr>
 <td>[queue2]</td>
 <td><code class="docutils literal notranslate">v7.4.2 -> v7.4.2</code></td>
 <tr>
 <td>[queue3]</td>
 <td><code class="docutils literal notranslate">v7.4.2 -> v7.4.2</code></td>
 <tr>
 <td>[queue4]</td>
 <td><code class="docutils literal notranslate">v7.4.2 -> v7.4.2</code></td>
 <tr>
 <td>[queue5]</td>
 <td><code class="docutils literal notranslate">v7.4.2 -> v7.4.2</code></td>
 <tr>
 <td>[queue6]</td>
 <td><code class="docutils literal notranslate">v7.4.2 -> v7.4.2</code></td>
 <tr>
 <td>[queue7]</td>
 <td><code class="docutils literal notranslate">v7.4.2 -> v7.4.2</code></td>
 </table>
 </div>
 </li>
                <li> <span class="li-head">dscp43</span> - Queue number of DSCP 43. <span class="li-normal">type: str</span> <span class="li-normal">choices: queue0, queue1, queue2, queue3, queue4, queue5, queue6, queue7</span>
 <a id='label346' href="javascript:ContentClick('label347', 'label346');" onmouseover="ContentPreview('label347');" onmouseout="ContentUnpreview('label347');" title="click to collapse or expand..."> more... </a>
 <div id="label347" style="display:none">
 <table border="1">
 <tr>
 <td></td>
 <td colspan="1">Supported Version Ranges</td>
 </tr>
 <tr>
 <td>dscp43</td>
 <td><code class="docutils literal notranslate">v7.4.2 -> v7.4.2 </code></td>
 </tr>
 <tr>
 <td>[queue0]</td>
 <td><code class="docutils literal notranslate">v7.4.2 -> v7.4.2</code></td>
 <tr>
 <td>[queue1]</td>
 <td><code class="docutils literal notranslate">v7.4.2 -> v7.4.2</code></td>
 <tr>
 <td>[queue2]</td>
 <td><code class="docutils literal notranslate">v7.4.2 -> v7.4.2</code></td>
 <tr>
 <td>[queue3]</td>
 <td><code class="docutils literal notranslate">v7.4.2 -> v7.4.2</code></td>
 <tr>
 <td>[queue4]</td>
 <td><code class="docutils literal notranslate">v7.4.2 -> v7.4.2</code></td>
 <tr>
 <td>[queue5]</td>
 <td><code class="docutils literal notranslate">v7.4.2 -> v7.4.2</code></td>
 <tr>
 <td>[queue6]</td>
 <td><code class="docutils literal notranslate">v7.4.2 -> v7.4.2</code></td>
 <tr>
 <td>[queue7]</td>
 <td><code class="docutils literal notranslate">v7.4.2 -> v7.4.2</code></td>
 </table>
 </div>
 </li>
                <li> <span class="li-head">dscp44</span> - Queue number of DSCP 44. <span class="li-normal">type: str</span> <span class="li-normal">choices: queue0, queue1, queue2, queue3, queue4, queue5, queue6, queue7</span>
 <a id='label348' href="javascript:ContentClick('label349', 'label348');" onmouseover="ContentPreview('label349');" onmouseout="ContentUnpreview('label349');" title="click to collapse or expand..."> more... </a>
 <div id="label349" style="display:none">
 <table border="1">
 <tr>
 <td></td>
 <td colspan="1">Supported Version Ranges</td>
 </tr>
 <tr>
 <td>dscp44</td>
 <td><code class="docutils literal notranslate">v7.4.2 -> v7.4.2 </code></td>
 </tr>
 <tr>
 <td>[queue0]</td>
 <td><code class="docutils literal notranslate">v7.4.2 -> v7.4.2</code></td>
 <tr>
 <td>[queue1]</td>
 <td><code class="docutils literal notranslate">v7.4.2 -> v7.4.2</code></td>
 <tr>
 <td>[queue2]</td>
 <td><code class="docutils literal notranslate">v7.4.2 -> v7.4.2</code></td>
 <tr>
 <td>[queue3]</td>
 <td><code class="docutils literal notranslate">v7.4.2 -> v7.4.2</code></td>
 <tr>
 <td>[queue4]</td>
 <td><code class="docutils literal notranslate">v7.4.2 -> v7.4.2</code></td>
 <tr>
 <td>[queue5]</td>
 <td><code class="docutils literal notranslate">v7.4.2 -> v7.4.2</code></td>
 <tr>
 <td>[queue6]</td>
 <td><code class="docutils literal notranslate">v7.4.2 -> v7.4.2</code></td>
 <tr>
 <td>[queue7]</td>
 <td><code class="docutils literal notranslate">v7.4.2 -> v7.4.2</code></td>
 </table>
 </div>
 </li>
                <li> <span class="li-head">dscp45</span> - Queue number of DSCP 45. <span class="li-normal">type: str</span> <span class="li-normal">choices: queue0, queue1, queue2, queue3, queue4, queue5, queue6, queue7</span>
 <a id='label350' href="javascript:ContentClick('label351', 'label350');" onmouseover="ContentPreview('label351');" onmouseout="ContentUnpreview('label351');" title="click to collapse or expand..."> more... </a>
 <div id="label351" style="display:none">
 <table border="1">
 <tr>
 <td></td>
 <td colspan="1">Supported Version Ranges</td>
 </tr>
 <tr>
 <td>dscp45</td>
 <td><code class="docutils literal notranslate">v7.4.2 -> v7.4.2 </code></td>
 </tr>
 <tr>
 <td>[queue0]</td>
 <td><code class="docutils literal notranslate">v7.4.2 -> v7.4.2</code></td>
 <tr>
 <td>[queue1]</td>
 <td><code class="docutils literal notranslate">v7.4.2 -> v7.4.2</code></td>
 <tr>
 <td>[queue2]</td>
 <td><code class="docutils literal notranslate">v7.4.2 -> v7.4.2</code></td>
 <tr>
 <td>[queue3]</td>
 <td><code class="docutils literal notranslate">v7.4.2 -> v7.4.2</code></td>
 <tr>
 <td>[queue4]</td>
 <td><code class="docutils literal notranslate">v7.4.2 -> v7.4.2</code></td>
 <tr>
 <td>[queue5]</td>
 <td><code class="docutils literal notranslate">v7.4.2 -> v7.4.2</code></td>
 <tr>
 <td>[queue6]</td>
 <td><code class="docutils literal notranslate">v7.4.2 -> v7.4.2</code></td>
 <tr>
 <td>[queue7]</td>
 <td><code class="docutils literal notranslate">v7.4.2 -> v7.4.2</code></td>
 </table>
 </div>
 </li>
                <li> <span class="li-head">dscp46</span> - Queue number of DSCP 46. <span class="li-normal">type: str</span> <span class="li-normal">choices: queue0, queue1, queue2, queue3, queue4, queue5, queue6, queue7</span>
 <a id='label352' href="javascript:ContentClick('label353', 'label352');" onmouseover="ContentPreview('label353');" onmouseout="ContentUnpreview('label353');" title="click to collapse or expand..."> more... </a>
 <div id="label353" style="display:none">
 <table border="1">
 <tr>
 <td></td>
 <td colspan="1">Supported Version Ranges</td>
 </tr>
 <tr>
 <td>dscp46</td>
 <td><code class="docutils literal notranslate">v7.4.2 -> v7.4.2 </code></td>
 </tr>
 <tr>
 <td>[queue0]</td>
 <td><code class="docutils literal notranslate">v7.4.2 -> v7.4.2</code></td>
 <tr>
 <td>[queue1]</td>
 <td><code class="docutils literal notranslate">v7.4.2 -> v7.4.2</code></td>
 <tr>
 <td>[queue2]</td>
 <td><code class="docutils literal notranslate">v7.4.2 -> v7.4.2</code></td>
 <tr>
 <td>[queue3]</td>
 <td><code class="docutils literal notranslate">v7.4.2 -> v7.4.2</code></td>
 <tr>
 <td>[queue4]</td>
 <td><code class="docutils literal notranslate">v7.4.2 -> v7.4.2</code></td>
 <tr>
 <td>[queue5]</td>
 <td><code class="docutils literal notranslate">v7.4.2 -> v7.4.2</code></td>
 <tr>
 <td>[queue6]</td>
 <td><code class="docutils literal notranslate">v7.4.2 -> v7.4.2</code></td>
 <tr>
 <td>[queue7]</td>
 <td><code class="docutils literal notranslate">v7.4.2 -> v7.4.2</code></td>
 </table>
 </div>
 </li>
                <li> <span class="li-head">dscp47</span> - Queue number of DSCP 47. <span class="li-normal">type: str</span> <span class="li-normal">choices: queue0, queue1, queue2, queue3, queue4, queue5, queue6, queue7</span>
 <a id='label354' href="javascript:ContentClick('label355', 'label354');" onmouseover="ContentPreview('label355');" onmouseout="ContentUnpreview('label355');" title="click to collapse or expand..."> more... </a>
 <div id="label355" style="display:none">
 <table border="1">
 <tr>
 <td></td>
 <td colspan="1">Supported Version Ranges</td>
 </tr>
 <tr>
 <td>dscp47</td>
 <td><code class="docutils literal notranslate">v7.4.2 -> v7.4.2 </code></td>
 </tr>
 <tr>
 <td>[queue0]</td>
 <td><code class="docutils literal notranslate">v7.4.2 -> v7.4.2</code></td>
 <tr>
 <td>[queue1]</td>
 <td><code class="docutils literal notranslate">v7.4.2 -> v7.4.2</code></td>
 <tr>
 <td>[queue2]</td>
 <td><code class="docutils literal notranslate">v7.4.2 -> v7.4.2</code></td>
 <tr>
 <td>[queue3]</td>
 <td><code class="docutils literal notranslate">v7.4.2 -> v7.4.2</code></td>
 <tr>
 <td>[queue4]</td>
 <td><code class="docutils literal notranslate">v7.4.2 -> v7.4.2</code></td>
 <tr>
 <td>[queue5]</td>
 <td><code class="docutils literal notranslate">v7.4.2 -> v7.4.2</code></td>
 <tr>
 <td>[queue6]</td>
 <td><code class="docutils literal notranslate">v7.4.2 -> v7.4.2</code></td>
 <tr>
 <td>[queue7]</td>
 <td><code class="docutils literal notranslate">v7.4.2 -> v7.4.2</code></td>
 </table>
 </div>
 </li>
                <li> <span class="li-head">dscp48</span> - Queue number of DSCP 48. <span class="li-normal">type: str</span> <span class="li-normal">choices: queue0, queue1, queue2, queue3, queue4, queue5, queue6, queue7</span>
 <a id='label356' href="javascript:ContentClick('label357', 'label356');" onmouseover="ContentPreview('label357');" onmouseout="ContentUnpreview('label357');" title="click to collapse or expand..."> more... </a>
 <div id="label357" style="display:none">
 <table border="1">
 <tr>
 <td></td>
 <td colspan="1">Supported Version Ranges</td>
 </tr>
 <tr>
 <td>dscp48</td>
 <td><code class="docutils literal notranslate">v7.4.2 -> v7.4.2 </code></td>
 </tr>
 <tr>
 <td>[queue0]</td>
 <td><code class="docutils literal notranslate">v7.4.2 -> v7.4.2</code></td>
 <tr>
 <td>[queue1]</td>
 <td><code class="docutils literal notranslate">v7.4.2 -> v7.4.2</code></td>
 <tr>
 <td>[queue2]</td>
 <td><code class="docutils literal notranslate">v7.4.2 -> v7.4.2</code></td>
 <tr>
 <td>[queue3]</td>
 <td><code class="docutils literal notranslate">v7.4.2 -> v7.4.2</code></td>
 <tr>
 <td>[queue4]</td>
 <td><code class="docutils literal notranslate">v7.4.2 -> v7.4.2</code></td>
 <tr>
 <td>[queue5]</td>
 <td><code class="docutils literal notranslate">v7.4.2 -> v7.4.2</code></td>
 <tr>
 <td>[queue6]</td>
 <td><code class="docutils literal notranslate">v7.4.2 -> v7.4.2</code></td>
 <tr>
 <td>[queue7]</td>
 <td><code class="docutils literal notranslate">v7.4.2 -> v7.4.2</code></td>
 </table>
 </div>
 </li>
                <li> <span class="li-head">dscp49</span> - Queue number of DSCP 49. <span class="li-normal">type: str</span> <span class="li-normal">choices: queue0, queue1, queue2, queue3, queue4, queue5, queue6, queue7</span>
 <a id='label358' href="javascript:ContentClick('label359', 'label358');" onmouseover="ContentPreview('label359');" onmouseout="ContentUnpreview('label359');" title="click to collapse or expand..."> more... </a>
 <div id="label359" style="display:none">
 <table border="1">
 <tr>
 <td></td>
 <td colspan="1">Supported Version Ranges</td>
 </tr>
 <tr>
 <td>dscp49</td>
 <td><code class="docutils literal notranslate">v7.4.2 -> v7.4.2 </code></td>
 </tr>
 <tr>
 <td>[queue0]</td>
 <td><code class="docutils literal notranslate">v7.4.2 -> v7.4.2</code></td>
 <tr>
 <td>[queue1]</td>
 <td><code class="docutils literal notranslate">v7.4.2 -> v7.4.2</code></td>
 <tr>
 <td>[queue2]</td>
 <td><code class="docutils literal notranslate">v7.4.2 -> v7.4.2</code></td>
 <tr>
 <td>[queue3]</td>
 <td><code class="docutils literal notranslate">v7.4.2 -> v7.4.2</code></td>
 <tr>
 <td>[queue4]</td>
 <td><code class="docutils literal notranslate">v7.4.2 -> v7.4.2</code></td>
 <tr>
 <td>[queue5]</td>
 <td><code class="docutils literal notranslate">v7.4.2 -> v7.4.2</code></td>
 <tr>
 <td>[queue6]</td>
 <td><code class="docutils literal notranslate">v7.4.2 -> v7.4.2</code></td>
 <tr>
 <td>[queue7]</td>
 <td><code class="docutils literal notranslate">v7.4.2 -> v7.4.2</code></td>
 </table>
 </div>
 </li>
                <li> <span class="li-head">dscp5</span> - Queue number of DSCP 5. <span class="li-normal">type: str</span> <span class="li-normal">choices: queue0, queue1, queue2, queue3, queue4, queue5, queue6, queue7</span>
 <a id='label360' href="javascript:ContentClick('label361', 'label360');" onmouseover="ContentPreview('label361');" onmouseout="ContentUnpreview('label361');" title="click to collapse or expand..."> more... </a>
 <div id="label361" style="display:none">
 <table border="1">
 <tr>
 <td></td>
 <td colspan="1">Supported Version Ranges</td>
 </tr>
 <tr>
 <td>dscp5</td>
 <td><code class="docutils literal notranslate">v7.4.2 -> v7.4.2 </code></td>
 </tr>
 <tr>
 <td>[queue0]</td>
 <td><code class="docutils literal notranslate">v7.4.2 -> v7.4.2</code></td>
 <tr>
 <td>[queue1]</td>
 <td><code class="docutils literal notranslate">v7.4.2 -> v7.4.2</code></td>
 <tr>
 <td>[queue2]</td>
 <td><code class="docutils literal notranslate">v7.4.2 -> v7.4.2</code></td>
 <tr>
 <td>[queue3]</td>
 <td><code class="docutils literal notranslate">v7.4.2 -> v7.4.2</code></td>
 <tr>
 <td>[queue4]</td>
 <td><code class="docutils literal notranslate">v7.4.2 -> v7.4.2</code></td>
 <tr>
 <td>[queue5]</td>
 <td><code class="docutils literal notranslate">v7.4.2 -> v7.4.2</code></td>
 <tr>
 <td>[queue6]</td>
 <td><code class="docutils literal notranslate">v7.4.2 -> v7.4.2</code></td>
 <tr>
 <td>[queue7]</td>
 <td><code class="docutils literal notranslate">v7.4.2 -> v7.4.2</code></td>
 </table>
 </div>
 </li>
                <li> <span class="li-head">dscp50</span> - Queue number of DSCP 50. <span class="li-normal">type: str</span> <span class="li-normal">choices: queue0, queue1, queue2, queue3, queue4, queue5, queue6, queue7</span>
 <a id='label362' href="javascript:ContentClick('label363', 'label362');" onmouseover="ContentPreview('label363');" onmouseout="ContentUnpreview('label363');" title="click to collapse or expand..."> more... </a>
 <div id="label363" style="display:none">
 <table border="1">
 <tr>
 <td></td>
 <td colspan="1">Supported Version Ranges</td>
 </tr>
 <tr>
 <td>dscp50</td>
 <td><code class="docutils literal notranslate">v7.4.2 -> v7.4.2 </code></td>
 </tr>
 <tr>
 <td>[queue0]</td>
 <td><code class="docutils literal notranslate">v7.4.2 -> v7.4.2</code></td>
 <tr>
 <td>[queue1]</td>
 <td><code class="docutils literal notranslate">v7.4.2 -> v7.4.2</code></td>
 <tr>
 <td>[queue2]</td>
 <td><code class="docutils literal notranslate">v7.4.2 -> v7.4.2</code></td>
 <tr>
 <td>[queue3]</td>
 <td><code class="docutils literal notranslate">v7.4.2 -> v7.4.2</code></td>
 <tr>
 <td>[queue4]</td>
 <td><code class="docutils literal notranslate">v7.4.2 -> v7.4.2</code></td>
 <tr>
 <td>[queue5]</td>
 <td><code class="docutils literal notranslate">v7.4.2 -> v7.4.2</code></td>
 <tr>
 <td>[queue6]</td>
 <td><code class="docutils literal notranslate">v7.4.2 -> v7.4.2</code></td>
 <tr>
 <td>[queue7]</td>
 <td><code class="docutils literal notranslate">v7.4.2 -> v7.4.2</code></td>
 </table>
 </div>
 </li>
                <li> <span class="li-head">dscp51</span> - Queue number of DSCP 51. <span class="li-normal">type: str</span> <span class="li-normal">choices: queue0, queue1, queue2, queue3, queue4, queue5, queue6, queue7</span>
 <a id='label364' href="javascript:ContentClick('label365', 'label364');" onmouseover="ContentPreview('label365');" onmouseout="ContentUnpreview('label365');" title="click to collapse or expand..."> more... </a>
 <div id="label365" style="display:none">
 <table border="1">
 <tr>
 <td></td>
 <td colspan="1">Supported Version Ranges</td>
 </tr>
 <tr>
 <td>dscp51</td>
 <td><code class="docutils literal notranslate">v7.4.2 -> v7.4.2 </code></td>
 </tr>
 <tr>
 <td>[queue0]</td>
 <td><code class="docutils literal notranslate">v7.4.2 -> v7.4.2</code></td>
 <tr>
 <td>[queue1]</td>
 <td><code class="docutils literal notranslate">v7.4.2 -> v7.4.2</code></td>
 <tr>
 <td>[queue2]</td>
 <td><code class="docutils literal notranslate">v7.4.2 -> v7.4.2</code></td>
 <tr>
 <td>[queue3]</td>
 <td><code class="docutils literal notranslate">v7.4.2 -> v7.4.2</code></td>
 <tr>
 <td>[queue4]</td>
 <td><code class="docutils literal notranslate">v7.4.2 -> v7.4.2</code></td>
 <tr>
 <td>[queue5]</td>
 <td><code class="docutils literal notranslate">v7.4.2 -> v7.4.2</code></td>
 <tr>
 <td>[queue6]</td>
 <td><code class="docutils literal notranslate">v7.4.2 -> v7.4.2</code></td>
 <tr>
 <td>[queue7]</td>
 <td><code class="docutils literal notranslate">v7.4.2 -> v7.4.2</code></td>
 </table>
 </div>
 </li>
                <li> <span class="li-head">dscp52</span> - Queue number of DSCP 52. <span class="li-normal">type: str</span> <span class="li-normal">choices: queue0, queue1, queue2, queue3, queue4, queue5, queue6, queue7</span>
 <a id='label366' href="javascript:ContentClick('label367', 'label366');" onmouseover="ContentPreview('label367');" onmouseout="ContentUnpreview('label367');" title="click to collapse or expand..."> more... </a>
 <div id="label367" style="display:none">
 <table border="1">
 <tr>
 <td></td>
 <td colspan="1">Supported Version Ranges</td>
 </tr>
 <tr>
 <td>dscp52</td>
 <td><code class="docutils literal notranslate">v7.4.2 -> v7.4.2 </code></td>
 </tr>
 <tr>
 <td>[queue0]</td>
 <td><code class="docutils literal notranslate">v7.4.2 -> v7.4.2</code></td>
 <tr>
 <td>[queue1]</td>
 <td><code class="docutils literal notranslate">v7.4.2 -> v7.4.2</code></td>
 <tr>
 <td>[queue2]</td>
 <td><code class="docutils literal notranslate">v7.4.2 -> v7.4.2</code></td>
 <tr>
 <td>[queue3]</td>
 <td><code class="docutils literal notranslate">v7.4.2 -> v7.4.2</code></td>
 <tr>
 <td>[queue4]</td>
 <td><code class="docutils literal notranslate">v7.4.2 -> v7.4.2</code></td>
 <tr>
 <td>[queue5]</td>
 <td><code class="docutils literal notranslate">v7.4.2 -> v7.4.2</code></td>
 <tr>
 <td>[queue6]</td>
 <td><code class="docutils literal notranslate">v7.4.2 -> v7.4.2</code></td>
 <tr>
 <td>[queue7]</td>
 <td><code class="docutils literal notranslate">v7.4.2 -> v7.4.2</code></td>
 </table>
 </div>
 </li>
                <li> <span class="li-head">dscp53</span> - Queue number of DSCP 53. <span class="li-normal">type: str</span> <span class="li-normal">choices: queue0, queue1, queue2, queue3, queue4, queue5, queue6, queue7</span>
 <a id='label368' href="javascript:ContentClick('label369', 'label368');" onmouseover="ContentPreview('label369');" onmouseout="ContentUnpreview('label369');" title="click to collapse or expand..."> more... </a>
 <div id="label369" style="display:none">
 <table border="1">
 <tr>
 <td></td>
 <td colspan="1">Supported Version Ranges</td>
 </tr>
 <tr>
 <td>dscp53</td>
 <td><code class="docutils literal notranslate">v7.4.2 -> v7.4.2 </code></td>
 </tr>
 <tr>
 <td>[queue0]</td>
 <td><code class="docutils literal notranslate">v7.4.2 -> v7.4.2</code></td>
 <tr>
 <td>[queue1]</td>
 <td><code class="docutils literal notranslate">v7.4.2 -> v7.4.2</code></td>
 <tr>
 <td>[queue2]</td>
 <td><code class="docutils literal notranslate">v7.4.2 -> v7.4.2</code></td>
 <tr>
 <td>[queue3]</td>
 <td><code class="docutils literal notranslate">v7.4.2 -> v7.4.2</code></td>
 <tr>
 <td>[queue4]</td>
 <td><code class="docutils literal notranslate">v7.4.2 -> v7.4.2</code></td>
 <tr>
 <td>[queue5]</td>
 <td><code class="docutils literal notranslate">v7.4.2 -> v7.4.2</code></td>
 <tr>
 <td>[queue6]</td>
 <td><code class="docutils literal notranslate">v7.4.2 -> v7.4.2</code></td>
 <tr>
 <td>[queue7]</td>
 <td><code class="docutils literal notranslate">v7.4.2 -> v7.4.2</code></td>
 </table>
 </div>
 </li>
                <li> <span class="li-head">dscp54</span> - Queue number of DSCP 54. <span class="li-normal">type: str</span> <span class="li-normal">choices: queue0, queue1, queue2, queue3, queue4, queue5, queue6, queue7</span>
 <a id='label370' href="javascript:ContentClick('label371', 'label370');" onmouseover="ContentPreview('label371');" onmouseout="ContentUnpreview('label371');" title="click to collapse or expand..."> more... </a>
 <div id="label371" style="display:none">
 <table border="1">
 <tr>
 <td></td>
 <td colspan="1">Supported Version Ranges</td>
 </tr>
 <tr>
 <td>dscp54</td>
 <td><code class="docutils literal notranslate">v7.4.2 -> v7.4.2 </code></td>
 </tr>
 <tr>
 <td>[queue0]</td>
 <td><code class="docutils literal notranslate">v7.4.2 -> v7.4.2</code></td>
 <tr>
 <td>[queue1]</td>
 <td><code class="docutils literal notranslate">v7.4.2 -> v7.4.2</code></td>
 <tr>
 <td>[queue2]</td>
 <td><code class="docutils literal notranslate">v7.4.2 -> v7.4.2</code></td>
 <tr>
 <td>[queue3]</td>
 <td><code class="docutils literal notranslate">v7.4.2 -> v7.4.2</code></td>
 <tr>
 <td>[queue4]</td>
 <td><code class="docutils literal notranslate">v7.4.2 -> v7.4.2</code></td>
 <tr>
 <td>[queue5]</td>
 <td><code class="docutils literal notranslate">v7.4.2 -> v7.4.2</code></td>
 <tr>
 <td>[queue6]</td>
 <td><code class="docutils literal notranslate">v7.4.2 -> v7.4.2</code></td>
 <tr>
 <td>[queue7]</td>
 <td><code class="docutils literal notranslate">v7.4.2 -> v7.4.2</code></td>
 </table>
 </div>
 </li>
                <li> <span class="li-head">dscp55</span> - Queue number of DSCP 55. <span class="li-normal">type: str</span> <span class="li-normal">choices: queue0, queue1, queue2, queue3, queue4, queue5, queue6, queue7</span>
 <a id='label372' href="javascript:ContentClick('label373', 'label372');" onmouseover="ContentPreview('label373');" onmouseout="ContentUnpreview('label373');" title="click to collapse or expand..."> more... </a>
 <div id="label373" style="display:none">
 <table border="1">
 <tr>
 <td></td>
 <td colspan="1">Supported Version Ranges</td>
 </tr>
 <tr>
 <td>dscp55</td>
 <td><code class="docutils literal notranslate">v7.4.2 -> v7.4.2 </code></td>
 </tr>
 <tr>
 <td>[queue0]</td>
 <td><code class="docutils literal notranslate">v7.4.2 -> v7.4.2</code></td>
 <tr>
 <td>[queue1]</td>
 <td><code class="docutils literal notranslate">v7.4.2 -> v7.4.2</code></td>
 <tr>
 <td>[queue2]</td>
 <td><code class="docutils literal notranslate">v7.4.2 -> v7.4.2</code></td>
 <tr>
 <td>[queue3]</td>
 <td><code class="docutils literal notranslate">v7.4.2 -> v7.4.2</code></td>
 <tr>
 <td>[queue4]</td>
 <td><code class="docutils literal notranslate">v7.4.2 -> v7.4.2</code></td>
 <tr>
 <td>[queue5]</td>
 <td><code class="docutils literal notranslate">v7.4.2 -> v7.4.2</code></td>
 <tr>
 <td>[queue6]</td>
 <td><code class="docutils literal notranslate">v7.4.2 -> v7.4.2</code></td>
 <tr>
 <td>[queue7]</td>
 <td><code class="docutils literal notranslate">v7.4.2 -> v7.4.2</code></td>
 </table>
 </div>
 </li>
                <li> <span class="li-head">dscp56</span> - Queue number of DSCP 56. <span class="li-normal">type: str</span> <span class="li-normal">choices: queue0, queue1, queue2, queue3, queue4, queue5, queue6, queue7</span>
 <a id='label374' href="javascript:ContentClick('label375', 'label374');" onmouseover="ContentPreview('label375');" onmouseout="ContentUnpreview('label375');" title="click to collapse or expand..."> more... </a>
 <div id="label375" style="display:none">
 <table border="1">
 <tr>
 <td></td>
 <td colspan="1">Supported Version Ranges</td>
 </tr>
 <tr>
 <td>dscp56</td>
 <td><code class="docutils literal notranslate">v7.4.2 -> v7.4.2 </code></td>
 </tr>
 <tr>
 <td>[queue0]</td>
 <td><code class="docutils literal notranslate">v7.4.2 -> v7.4.2</code></td>
 <tr>
 <td>[queue1]</td>
 <td><code class="docutils literal notranslate">v7.4.2 -> v7.4.2</code></td>
 <tr>
 <td>[queue2]</td>
 <td><code class="docutils literal notranslate">v7.4.2 -> v7.4.2</code></td>
 <tr>
 <td>[queue3]</td>
 <td><code class="docutils literal notranslate">v7.4.2 -> v7.4.2</code></td>
 <tr>
 <td>[queue4]</td>
 <td><code class="docutils literal notranslate">v7.4.2 -> v7.4.2</code></td>
 <tr>
 <td>[queue5]</td>
 <td><code class="docutils literal notranslate">v7.4.2 -> v7.4.2</code></td>
 <tr>
 <td>[queue6]</td>
 <td><code class="docutils literal notranslate">v7.4.2 -> v7.4.2</code></td>
 <tr>
 <td>[queue7]</td>
 <td><code class="docutils literal notranslate">v7.4.2 -> v7.4.2</code></td>
 </table>
 </div>
 </li>
                <li> <span class="li-head">dscp57</span> - Queue number of DSCP 57. <span class="li-normal">type: str</span> <span class="li-normal">choices: queue0, queue1, queue2, queue3, queue4, queue5, queue6, queue7</span>
 <a id='label376' href="javascript:ContentClick('label377', 'label376');" onmouseover="ContentPreview('label377');" onmouseout="ContentUnpreview('label377');" title="click to collapse or expand..."> more... </a>
 <div id="label377" style="display:none">
 <table border="1">
 <tr>
 <td></td>
 <td colspan="1">Supported Version Ranges</td>
 </tr>
 <tr>
 <td>dscp57</td>
 <td><code class="docutils literal notranslate">v7.4.2 -> v7.4.2 </code></td>
 </tr>
 <tr>
 <td>[queue0]</td>
 <td><code class="docutils literal notranslate">v7.4.2 -> v7.4.2</code></td>
 <tr>
 <td>[queue1]</td>
 <td><code class="docutils literal notranslate">v7.4.2 -> v7.4.2</code></td>
 <tr>
 <td>[queue2]</td>
 <td><code class="docutils literal notranslate">v7.4.2 -> v7.4.2</code></td>
 <tr>
 <td>[queue3]</td>
 <td><code class="docutils literal notranslate">v7.4.2 -> v7.4.2</code></td>
 <tr>
 <td>[queue4]</td>
 <td><code class="docutils literal notranslate">v7.4.2 -> v7.4.2</code></td>
 <tr>
 <td>[queue5]</td>
 <td><code class="docutils literal notranslate">v7.4.2 -> v7.4.2</code></td>
 <tr>
 <td>[queue6]</td>
 <td><code class="docutils literal notranslate">v7.4.2 -> v7.4.2</code></td>
 <tr>
 <td>[queue7]</td>
 <td><code class="docutils literal notranslate">v7.4.2 -> v7.4.2</code></td>
 </table>
 </div>
 </li>
                <li> <span class="li-head">dscp58</span> - Queue number of DSCP 58. <span class="li-normal">type: str</span> <span class="li-normal">choices: queue0, queue1, queue2, queue3, queue4, queue5, queue6, queue7</span>
 <a id='label378' href="javascript:ContentClick('label379', 'label378');" onmouseover="ContentPreview('label379');" onmouseout="ContentUnpreview('label379');" title="click to collapse or expand..."> more... </a>
 <div id="label379" style="display:none">
 <table border="1">
 <tr>
 <td></td>
 <td colspan="1">Supported Version Ranges</td>
 </tr>
 <tr>
 <td>dscp58</td>
 <td><code class="docutils literal notranslate">v7.4.2 -> v7.4.2 </code></td>
 </tr>
 <tr>
 <td>[queue0]</td>
 <td><code class="docutils literal notranslate">v7.4.2 -> v7.4.2</code></td>
 <tr>
 <td>[queue1]</td>
 <td><code class="docutils literal notranslate">v7.4.2 -> v7.4.2</code></td>
 <tr>
 <td>[queue2]</td>
 <td><code class="docutils literal notranslate">v7.4.2 -> v7.4.2</code></td>
 <tr>
 <td>[queue3]</td>
 <td><code class="docutils literal notranslate">v7.4.2 -> v7.4.2</code></td>
 <tr>
 <td>[queue4]</td>
 <td><code class="docutils literal notranslate">v7.4.2 -> v7.4.2</code></td>
 <tr>
 <td>[queue5]</td>
 <td><code class="docutils literal notranslate">v7.4.2 -> v7.4.2</code></td>
 <tr>
 <td>[queue6]</td>
 <td><code class="docutils literal notranslate">v7.4.2 -> v7.4.2</code></td>
 <tr>
 <td>[queue7]</td>
 <td><code class="docutils literal notranslate">v7.4.2 -> v7.4.2</code></td>
 </table>
 </div>
 </li>
                <li> <span class="li-head">dscp59</span> - Queue number of DSCP 59. <span class="li-normal">type: str</span> <span class="li-normal">choices: queue0, queue1, queue2, queue3, queue4, queue5, queue6, queue7</span>
 <a id='label380' href="javascript:ContentClick('label381', 'label380');" onmouseover="ContentPreview('label381');" onmouseout="ContentUnpreview('label381');" title="click to collapse or expand..."> more... </a>
 <div id="label381" style="display:none">
 <table border="1">
 <tr>
 <td></td>
 <td colspan="1">Supported Version Ranges</td>
 </tr>
 <tr>
 <td>dscp59</td>
 <td><code class="docutils literal notranslate">v7.4.2 -> v7.4.2 </code></td>
 </tr>
 <tr>
 <td>[queue0]</td>
 <td><code class="docutils literal notranslate">v7.4.2 -> v7.4.2</code></td>
 <tr>
 <td>[queue1]</td>
 <td><code class="docutils literal notranslate">v7.4.2 -> v7.4.2</code></td>
 <tr>
 <td>[queue2]</td>
 <td><code class="docutils literal notranslate">v7.4.2 -> v7.4.2</code></td>
 <tr>
 <td>[queue3]</td>
 <td><code class="docutils literal notranslate">v7.4.2 -> v7.4.2</code></td>
 <tr>
 <td>[queue4]</td>
 <td><code class="docutils literal notranslate">v7.4.2 -> v7.4.2</code></td>
 <tr>
 <td>[queue5]</td>
 <td><code class="docutils literal notranslate">v7.4.2 -> v7.4.2</code></td>
 <tr>
 <td>[queue6]</td>
 <td><code class="docutils literal notranslate">v7.4.2 -> v7.4.2</code></td>
 <tr>
 <td>[queue7]</td>
 <td><code class="docutils literal notranslate">v7.4.2 -> v7.4.2</code></td>
 </table>
 </div>
 </li>
                <li> <span class="li-head">dscp6</span> - Queue number of DSCP 6. <span class="li-normal">type: str</span> <span class="li-normal">choices: queue0, queue1, queue2, queue3, queue4, queue5, queue6, queue7</span>
 <a id='label382' href="javascript:ContentClick('label383', 'label382');" onmouseover="ContentPreview('label383');" onmouseout="ContentUnpreview('label383');" title="click to collapse or expand..."> more... </a>
 <div id="label383" style="display:none">
 <table border="1">
 <tr>
 <td></td>
 <td colspan="1">Supported Version Ranges</td>
 </tr>
 <tr>
 <td>dscp6</td>
 <td><code class="docutils literal notranslate">v7.4.2 -> v7.4.2 </code></td>
 </tr>
 <tr>
 <td>[queue0]</td>
 <td><code class="docutils literal notranslate">v7.4.2 -> v7.4.2</code></td>
 <tr>
 <td>[queue1]</td>
 <td><code class="docutils literal notranslate">v7.4.2 -> v7.4.2</code></td>
 <tr>
 <td>[queue2]</td>
 <td><code class="docutils literal notranslate">v7.4.2 -> v7.4.2</code></td>
 <tr>
 <td>[queue3]</td>
 <td><code class="docutils literal notranslate">v7.4.2 -> v7.4.2</code></td>
 <tr>
 <td>[queue4]</td>
 <td><code class="docutils literal notranslate">v7.4.2 -> v7.4.2</code></td>
 <tr>
 <td>[queue5]</td>
 <td><code class="docutils literal notranslate">v7.4.2 -> v7.4.2</code></td>
 <tr>
 <td>[queue6]</td>
 <td><code class="docutils literal notranslate">v7.4.2 -> v7.4.2</code></td>
 <tr>
 <td>[queue7]</td>
 <td><code class="docutils literal notranslate">v7.4.2 -> v7.4.2</code></td>
 </table>
 </div>
 </li>
                <li> <span class="li-head">dscp60</span> - Queue number of DSCP 60. <span class="li-normal">type: str</span> <span class="li-normal">choices: queue0, queue1, queue2, queue3, queue4, queue5, queue6, queue7</span>
 <a id='label384' href="javascript:ContentClick('label385', 'label384');" onmouseover="ContentPreview('label385');" onmouseout="ContentUnpreview('label385');" title="click to collapse or expand..."> more... </a>
 <div id="label385" style="display:none">
 <table border="1">
 <tr>
 <td></td>
 <td colspan="1">Supported Version Ranges</td>
 </tr>
 <tr>
 <td>dscp60</td>
 <td><code class="docutils literal notranslate">v7.4.2 -> v7.4.2 </code></td>
 </tr>
 <tr>
 <td>[queue0]</td>
 <td><code class="docutils literal notranslate">v7.4.2 -> v7.4.2</code></td>
 <tr>
 <td>[queue1]</td>
 <td><code class="docutils literal notranslate">v7.4.2 -> v7.4.2</code></td>
 <tr>
 <td>[queue2]</td>
 <td><code class="docutils literal notranslate">v7.4.2 -> v7.4.2</code></td>
 <tr>
 <td>[queue3]</td>
 <td><code class="docutils literal notranslate">v7.4.2 -> v7.4.2</code></td>
 <tr>
 <td>[queue4]</td>
 <td><code class="docutils literal notranslate">v7.4.2 -> v7.4.2</code></td>
 <tr>
 <td>[queue5]</td>
 <td><code class="docutils literal notranslate">v7.4.2 -> v7.4.2</code></td>
 <tr>
 <td>[queue6]</td>
 <td><code class="docutils literal notranslate">v7.4.2 -> v7.4.2</code></td>
 <tr>
 <td>[queue7]</td>
 <td><code class="docutils literal notranslate">v7.4.2 -> v7.4.2</code></td>
 </table>
 </div>
 </li>
                <li> <span class="li-head">dscp61</span> - Queue number of DSCP 61. <span class="li-normal">type: str</span> <span class="li-normal">choices: queue0, queue1, queue2, queue3, queue4, queue5, queue6, queue7</span>
 <a id='label386' href="javascript:ContentClick('label387', 'label386');" onmouseover="ContentPreview('label387');" onmouseout="ContentUnpreview('label387');" title="click to collapse or expand..."> more... </a>
 <div id="label387" style="display:none">
 <table border="1">
 <tr>
 <td></td>
 <td colspan="1">Supported Version Ranges</td>
 </tr>
 <tr>
 <td>dscp61</td>
 <td><code class="docutils literal notranslate">v7.4.2 -> v7.4.2 </code></td>
 </tr>
 <tr>
 <td>[queue0]</td>
 <td><code class="docutils literal notranslate">v7.4.2 -> v7.4.2</code></td>
 <tr>
 <td>[queue1]</td>
 <td><code class="docutils literal notranslate">v7.4.2 -> v7.4.2</code></td>
 <tr>
 <td>[queue2]</td>
 <td><code class="docutils literal notranslate">v7.4.2 -> v7.4.2</code></td>
 <tr>
 <td>[queue3]</td>
 <td><code class="docutils literal notranslate">v7.4.2 -> v7.4.2</code></td>
 <tr>
 <td>[queue4]</td>
 <td><code class="docutils literal notranslate">v7.4.2 -> v7.4.2</code></td>
 <tr>
 <td>[queue5]</td>
 <td><code class="docutils literal notranslate">v7.4.2 -> v7.4.2</code></td>
 <tr>
 <td>[queue6]</td>
 <td><code class="docutils literal notranslate">v7.4.2 -> v7.4.2</code></td>
 <tr>
 <td>[queue7]</td>
 <td><code class="docutils literal notranslate">v7.4.2 -> v7.4.2</code></td>
 </table>
 </div>
 </li>
                <li> <span class="li-head">dscp62</span> - Queue number of DSCP 62. <span class="li-normal">type: str</span> <span class="li-normal">choices: queue0, queue1, queue2, queue3, queue4, queue5, queue6, queue7</span>
 <a id='label388' href="javascript:ContentClick('label389', 'label388');" onmouseover="ContentPreview('label389');" onmouseout="ContentUnpreview('label389');" title="click to collapse or expand..."> more... </a>
 <div id="label389" style="display:none">
 <table border="1">
 <tr>
 <td></td>
 <td colspan="1">Supported Version Ranges</td>
 </tr>
 <tr>
 <td>dscp62</td>
 <td><code class="docutils literal notranslate">v7.4.2 -> v7.4.2 </code></td>
 </tr>
 <tr>
 <td>[queue0]</td>
 <td><code class="docutils literal notranslate">v7.4.2 -> v7.4.2</code></td>
 <tr>
 <td>[queue1]</td>
 <td><code class="docutils literal notranslate">v7.4.2 -> v7.4.2</code></td>
 <tr>
 <td>[queue2]</td>
 <td><code class="docutils literal notranslate">v7.4.2 -> v7.4.2</code></td>
 <tr>
 <td>[queue3]</td>
 <td><code class="docutils literal notranslate">v7.4.2 -> v7.4.2</code></td>
 <tr>
 <td>[queue4]</td>
 <td><code class="docutils literal notranslate">v7.4.2 -> v7.4.2</code></td>
 <tr>
 <td>[queue5]</td>
 <td><code class="docutils literal notranslate">v7.4.2 -> v7.4.2</code></td>
 <tr>
 <td>[queue6]</td>
 <td><code class="docutils literal notranslate">v7.4.2 -> v7.4.2</code></td>
 <tr>
 <td>[queue7]</td>
 <td><code class="docutils literal notranslate">v7.4.2 -> v7.4.2</code></td>
 </table>
 </div>
 </li>
                <li> <span class="li-head">dscp63</span> - Queue number of DSCP 63. <span class="li-normal">type: str</span> <span class="li-normal">choices: queue0, queue1, queue2, queue3, queue4, queue5, queue6, queue7</span>
 <a id='label390' href="javascript:ContentClick('label391', 'label390');" onmouseover="ContentPreview('label391');" onmouseout="ContentUnpreview('label391');" title="click to collapse or expand..."> more... </a>
 <div id="label391" style="display:none">
 <table border="1">
 <tr>
 <td></td>
 <td colspan="1">Supported Version Ranges</td>
 </tr>
 <tr>
 <td>dscp63</td>
 <td><code class="docutils literal notranslate">v7.4.2 -> v7.4.2 </code></td>
 </tr>
 <tr>
 <td>[queue0]</td>
 <td><code class="docutils literal notranslate">v7.4.2 -> v7.4.2</code></td>
 <tr>
 <td>[queue1]</td>
 <td><code class="docutils literal notranslate">v7.4.2 -> v7.4.2</code></td>
 <tr>
 <td>[queue2]</td>
 <td><code class="docutils literal notranslate">v7.4.2 -> v7.4.2</code></td>
 <tr>
 <td>[queue3]</td>
 <td><code class="docutils literal notranslate">v7.4.2 -> v7.4.2</code></td>
 <tr>
 <td>[queue4]</td>
 <td><code class="docutils literal notranslate">v7.4.2 -> v7.4.2</code></td>
 <tr>
 <td>[queue5]</td>
 <td><code class="docutils literal notranslate">v7.4.2 -> v7.4.2</code></td>
 <tr>
 <td>[queue6]</td>
 <td><code class="docutils literal notranslate">v7.4.2 -> v7.4.2</code></td>
 <tr>
 <td>[queue7]</td>
 <td><code class="docutils literal notranslate">v7.4.2 -> v7.4.2</code></td>
 </table>
 </div>
 </li>
                <li> <span class="li-head">dscp7</span> - Queue number of DSCP 7. <span class="li-normal">type: str</span> <span class="li-normal">choices: queue0, queue1, queue2, queue3, queue4, queue5, queue6, queue7</span>
 <a id='label392' href="javascript:ContentClick('label393', 'label392');" onmouseover="ContentPreview('label393');" onmouseout="ContentUnpreview('label393');" title="click to collapse or expand..."> more... </a>
 <div id="label393" style="display:none">
 <table border="1">
 <tr>
 <td></td>
 <td colspan="1">Supported Version Ranges</td>
 </tr>
 <tr>
 <td>dscp7</td>
 <td><code class="docutils literal notranslate">v7.4.2 -> v7.4.2 </code></td>
 </tr>
 <tr>
 <td>[queue0]</td>
 <td><code class="docutils literal notranslate">v7.4.2 -> v7.4.2</code></td>
 <tr>
 <td>[queue1]</td>
 <td><code class="docutils literal notranslate">v7.4.2 -> v7.4.2</code></td>
 <tr>
 <td>[queue2]</td>
 <td><code class="docutils literal notranslate">v7.4.2 -> v7.4.2</code></td>
 <tr>
 <td>[queue3]</td>
 <td><code class="docutils literal notranslate">v7.4.2 -> v7.4.2</code></td>
 <tr>
 <td>[queue4]</td>
 <td><code class="docutils literal notranslate">v7.4.2 -> v7.4.2</code></td>
 <tr>
 <td>[queue5]</td>
 <td><code class="docutils literal notranslate">v7.4.2 -> v7.4.2</code></td>
 <tr>
 <td>[queue6]</td>
 <td><code class="docutils literal notranslate">v7.4.2 -> v7.4.2</code></td>
 <tr>
 <td>[queue7]</td>
 <td><code class="docutils literal notranslate">v7.4.2 -> v7.4.2</code></td>
 </table>
 </div>
 </li>
                <li> <span class="li-head">dscp8</span> - Queue number of DSCP 8. <span class="li-normal">type: str</span> <span class="li-normal">choices: queue0, queue1, queue2, queue3, queue4, queue5, queue6, queue7</span>
 <a id='label394' href="javascript:ContentClick('label395', 'label394');" onmouseover="ContentPreview('label395');" onmouseout="ContentUnpreview('label395');" title="click to collapse or expand..."> more... </a>
 <div id="label395" style="display:none">
 <table border="1">
 <tr>
 <td></td>
 <td colspan="1">Supported Version Ranges</td>
 </tr>
 <tr>
 <td>dscp8</td>
 <td><code class="docutils literal notranslate">v7.4.2 -> v7.4.2 </code></td>
 </tr>
 <tr>
 <td>[queue0]</td>
 <td><code class="docutils literal notranslate">v7.4.2 -> v7.4.2</code></td>
 <tr>
 <td>[queue1]</td>
 <td><code class="docutils literal notranslate">v7.4.2 -> v7.4.2</code></td>
 <tr>
 <td>[queue2]</td>
 <td><code class="docutils literal notranslate">v7.4.2 -> v7.4.2</code></td>
 <tr>
 <td>[queue3]</td>
 <td><code class="docutils literal notranslate">v7.4.2 -> v7.4.2</code></td>
 <tr>
 <td>[queue4]</td>
 <td><code class="docutils literal notranslate">v7.4.2 -> v7.4.2</code></td>
 <tr>
 <td>[queue5]</td>
 <td><code class="docutils literal notranslate">v7.4.2 -> v7.4.2</code></td>
 <tr>
 <td>[queue6]</td>
 <td><code class="docutils literal notranslate">v7.4.2 -> v7.4.2</code></td>
 <tr>
 <td>[queue7]</td>
 <td><code class="docutils literal notranslate">v7.4.2 -> v7.4.2</code></td>
 </table>
 </div>
 </li>
                <li> <span class="li-head">dscp9</span> - Queue number of DSCP 9. <span class="li-normal">type: str</span> <span class="li-normal">choices: queue0, queue1, queue2, queue3, queue4, queue5, queue6, queue7</span>
 <a id='label396' href="javascript:ContentClick('label397', 'label396');" onmouseover="ContentPreview('label397');" onmouseout="ContentUnpreview('label397');" title="click to collapse or expand..."> more... </a>
 <div id="label397" style="display:none">
 <table border="1">
 <tr>
 <td></td>
 <td colspan="1">Supported Version Ranges</td>
 </tr>
 <tr>
 <td>dscp9</td>
 <td><code class="docutils literal notranslate">v7.4.2 -> v7.4.2 </code></td>
 </tr>
 <tr>
 <td>[queue0]</td>
 <td><code class="docutils literal notranslate">v7.4.2 -> v7.4.2</code></td>
 <tr>
 <td>[queue1]</td>
 <td><code class="docutils literal notranslate">v7.4.2 -> v7.4.2</code></td>
 <tr>
 <td>[queue2]</td>
 <td><code class="docutils literal notranslate">v7.4.2 -> v7.4.2</code></td>
 <tr>
 <td>[queue3]</td>
 <td><code class="docutils literal notranslate">v7.4.2 -> v7.4.2</code></td>
 <tr>
 <td>[queue4]</td>
 <td><code class="docutils literal notranslate">v7.4.2 -> v7.4.2</code></td>
 <tr>
 <td>[queue5]</td>
 <td><code class="docutils literal notranslate">v7.4.2 -> v7.4.2</code></td>
 <tr>
 <td>[queue6]</td>
 <td><code class="docutils literal notranslate">v7.4.2 -> v7.4.2</code></td>
 <tr>
 <td>[queue7]</td>
 <td><code class="docutils literal notranslate">v7.4.2 -> v7.4.2</code></td>
 </table>
 </div>
 </li>
                <li> <span class="li-head">id</span> - Profile ID. see <a href='#notes'>Notes</a>. <span class="li-normal">type: int</span> <span class="li-required">required: true</span>
 <a id='label398' href="javascript:ContentClick('label399', 'label398');" onmouseover="ContentPreview('label399');" onmouseout="ContentUnpreview('label399');" title="click to collapse or expand..."> more... </a>
 <div id="label399" style="display:none">
 <table border="1">
 <tr>
 <td></td>
 <td colspan="1">Supported Version Ranges</td>
 </tr>
 <tr>
 <td>id</td>
 <td><code class="docutils literal notranslate">v7.4.2 -> v7.4.2 </code></td>
 </tr>
 </table>
 </div>
 </li>
                <li> <span class="li-head">type</span> - Profile type. <span class="li-normal">type: str</span> <span class="li-normal">choices: cos, dscp</span>
 <a id='label400' href="javascript:ContentClick('label401', 'label400');" onmouseover="ContentPreview('label401');" onmouseout="ContentUnpreview('label401');" title="click to collapse or expand..."> more... </a>
 <div id="label401" style="display:none">
 <table border="1">
 <tr>
 <td></td>
 <td colspan="1">Supported Version Ranges</td>
 </tr>
 <tr>
 <td>type</td>
 <td><code class="docutils literal notranslate">v7.4.2 -> v7.4.2 </code></td>
 </tr>
 <tr>
 <td>[cos]</td>
 <td><code class="docutils literal notranslate">v7.4.2 -> v7.4.2</code></td>
 <tr>
 <td>[dscp]</td>
 <td><code class="docutils literal notranslate">v7.4.2 -> v7.4.2</code></td>
 </table>
 </div>
 </li>
                <li> <span class="li-head">weight</span> - Class weight. <span class="li-normal">type: int</span>
 <a id='label402' href="javascript:ContentClick('label403', 'label402');" onmouseover="ContentPreview('label403');" onmouseout="ContentUnpreview('label403');" title="click to collapse or expand..."> more... </a>
 <div id="label403" style="display:none">
 <table border="1">
 <tr>
 <td></td>
 <td colspan="1">Supported Version Ranges</td>
 </tr>
 <tr>
 <td>weight</td>
 <td><code class="docutils literal notranslate">v7.4.2 -> v7.4.2 </code></td>
 </tr>
 </table>
 </div>
 </li>
                </ul>
            <li> <span class="li-head">scheduler</span> - Configure a NP7 QoS Scheduler. <span class="li-normal">type: list</span> <span style="font-family:'Courier New'" class="li-required">member_path: np_queues/scheduler:name</span>
 <a id='label404' href="javascript:ContentClick('label405', 'label404');" onmouseover="ContentPreview('label405');" onmouseout="ContentUnpreview('label405');" title="click to collapse or expand..."> more... </a>
 <div id="label405" style="display:none">
 <table border="1">
 <tr>
 <td></td><td colspan="1">Supported Version Ranges</td>
 </tr>
 <tr>
 <td>scheduler</td>
 <td><code class="docutils literal notranslate">v7.4.2 -> v7.4.2 </code></td>
 </tr>
 </table>
 </div>
 </li>
                <ul class="ul-self">
                <li> <span class="li-head">mode</span> - Scheduler mode. <span class="li-normal">type: str</span> <span class="li-normal">choices: none, priority, round-robin</span>
 <a id='label406' href="javascript:ContentClick('label407', 'label406');" onmouseover="ContentPreview('label407');" onmouseout="ContentUnpreview('label407');" title="click to collapse or expand..."> more... </a>
 <div id="label407" style="display:none">
 <table border="1">
 <tr>
 <td></td>
 <td colspan="1">Supported Version Ranges</td>
 </tr>
 <tr>
 <td>mode</td>
 <td><code class="docutils literal notranslate">v7.4.2 -> v7.4.2 </code></td>
 </tr>
 <tr>
 <td>[none]</td>
 <td><code class="docutils literal notranslate">v7.4.2 -> v7.4.2</code></td>
 <tr>
 <td>[priority]</td>
 <td><code class="docutils literal notranslate">v7.4.2 -> v7.4.2</code></td>
 <tr>
 <td>[round-robin]</td>
 <td><code class="docutils literal notranslate">v7.4.2 -> v7.4.2</code></td>
 </table>
 </div>
 </li>
                <li> <span class="li-head">name</span> - Scheduler name. <span class="li-normal">type: str</span> <span class="li-required">required: true</span>
 <a id='label408' href="javascript:ContentClick('label409', 'label408');" onmouseover="ContentPreview('label409');" onmouseout="ContentUnpreview('label409');" title="click to collapse or expand..."> more... </a>
 <div id="label409" style="display:none">
 <table border="1">
 <tr>
 <td></td>
 <td colspan="1">Supported Version Ranges</td>
 </tr>
 <tr>
 <td>name</td>
 <td><code class="docutils literal notranslate">v7.4.2 -> v7.4.2 </code></td>
 </tr>
 </table>
 </div>
 </li>
                </ul>
            </ul>
        <li> <span class="li-head">npu_group_effective_scope</span> - npu-group-effective-scope defines under which npu-group cmds such as list/purge will be excecuted. Default scope is for all four HS-ok groups. (0-3). <span class="li-normal">type: int</span>
 <a id='label410' href="javascript:ContentClick('label411', 'label410');" onmouseover="ContentPreview('label411');" onmouseout="ContentUnpreview('label411');" title="click to collapse or expand..."> more... </a>
 <div id="label411" style="display:none">
 <table border="1">
 <tr>
 <td></td>
 <td colspan="1">Supported Version Ranges</td>
 </tr>
 <tr>
 <td>npu_group_effective_scope</td>
 <td><code class="docutils literal notranslate">v7.4.2 -> v7.4.2 </code></td>
 </tr>
 </table>
 </div>
 </li>
        <li> <span class="li-head">npu_tcam</span> - Configure NPU TCAM policies. <span class="li-normal">type: list</span> <span style="font-family:'Courier New'" class="li-required">member_path: npu_tcam:name</span>
 <a id='label412' href="javascript:ContentClick('label413', 'label412');" onmouseover="ContentPreview('label413');" onmouseout="ContentUnpreview('label413');" title="click to collapse or expand..."> more... </a>
 <div id="label413" style="display:none">
 <table border="1">
 <tr>
 <td></td><td colspan="1">Supported Version Ranges</td>
 </tr>
 <tr>
 <td>npu_tcam</td>
 <td><code class="docutils literal notranslate">v7.4.2 -> v7.4.2 </code></td>
 </tr>
 </table>
 </div>
 </li>
            <ul class="ul-self">
            <li> <span class="li-head">data</span> - Data fields of TCAM. <span class="li-normal">type: dict</span>
 <a id='label414' href="javascript:ContentClick('label415', 'label414');" onmouseover="ContentPreview('label415');" onmouseout="ContentUnpreview('label415');" title="click to collapse or expand..."> more... </a>
 <div id="label415" style="display:none">
 <table border="1">
 <tr>
 <td></td><td colspan="1">Supported Version Ranges</td>
 </tr>
 <tr>
 <td>data</td>
 <td><code class="docutils literal notranslate">v7.4.2 -> v7.4.2 </code></td>
 </tr>
 </table>
 </div>
 </li>
                <ul class="ul-self">
                <li> <span class="li-head">df</span> - tcam data ip flag df. <span class="li-normal">type: str</span> <span class="li-normal">choices: enable, disable</span>
 <a id='label416' href="javascript:ContentClick('label417', 'label416');" onmouseover="ContentPreview('label417');" onmouseout="ContentUnpreview('label417');" title="click to collapse or expand..."> more... </a>
 <div id="label417" style="display:none">
 <table border="1">
 <tr>
 <td></td>
 <td colspan="1">Supported Version Ranges</td>
 </tr>
 <tr>
 <td>df</td>
 <td><code class="docutils literal notranslate">v7.4.2 -> v7.4.2 </code></td>
 </tr>
 <tr>
 <td>[enable]</td>
 <td><code class="docutils literal notranslate">v7.4.2 -> v7.4.2</code></td>
 <tr>
 <td>[disable]</td>
 <td><code class="docutils literal notranslate">v7.4.2 -> v7.4.2</code></td>
 </table>
 </div>
 </li>
                <li> <span class="li-head">dstip</span> - tcam data dst ipv4 address. <span class="li-normal">type: str</span>
 <a id='label418' href="javascript:ContentClick('label419', 'label418');" onmouseover="ContentPreview('label419');" onmouseout="ContentUnpreview('label419');" title="click to collapse or expand..."> more... </a>
 <div id="label419" style="display:none">
 <table border="1">
 <tr>
 <td></td>
 <td colspan="1">Supported Version Ranges</td>
 </tr>
 <tr>
 <td>dstip</td>
 <td><code class="docutils literal notranslate">v7.4.2 -> v7.4.2 </code></td>
 </tr>
 </table>
 </div>
 </li>
                <li> <span class="li-head">dstipv6</span> - tcam data dst ipv6 address. <span class="li-normal">type: str</span>
 <a id='label420' href="javascript:ContentClick('label421', 'label420');" onmouseover="ContentPreview('label421');" onmouseout="ContentUnpreview('label421');" title="click to collapse or expand..."> more... </a>
 <div id="label421" style="display:none">
 <table border="1">
 <tr>
 <td></td>
 <td colspan="1">Supported Version Ranges</td>
 </tr>
 <tr>
 <td>dstipv6</td>
 <td><code class="docutils literal notranslate">v7.4.2 -> v7.4.2 </code></td>
 </tr>
 </table>
 </div>
 </li>
                <li> <span class="li-head">dstmac</span> - tcam data dst macaddr. <span class="li-normal">type: str</span>
 <a id='label422' href="javascript:ContentClick('label423', 'label422');" onmouseover="ContentPreview('label423');" onmouseout="ContentUnpreview('label423');" title="click to collapse or expand..."> more... </a>
 <div id="label423" style="display:none">
 <table border="1">
 <tr>
 <td></td>
 <td colspan="1">Supported Version Ranges</td>
 </tr>
 <tr>
 <td>dstmac</td>
 <td><code class="docutils literal notranslate">v7.4.2 -> v7.4.2 </code></td>
 </tr>
 </table>
 </div>
 </li>
                <li> <span class="li-head">dstport</span> - tcam data L4 dst port. <span class="li-normal">type: int</span>
 <a id='label424' href="javascript:ContentClick('label425', 'label424');" onmouseover="ContentPreview('label425');" onmouseout="ContentUnpreview('label425');" title="click to collapse or expand..."> more... </a>
 <div id="label425" style="display:none">
 <table border="1">
 <tr>
 <td></td>
 <td colspan="1">Supported Version Ranges</td>
 </tr>
 <tr>
 <td>dstport</td>
 <td><code class="docutils literal notranslate">v7.4.2 -> v7.4.2 </code></td>
 </tr>
 </table>
 </div>
 </li>
                <li> <span class="li-head">ethertype</span> - tcam data ethertype. <span class="li-normal">type: str</span>
 <a id='label426' href="javascript:ContentClick('label427', 'label426');" onmouseover="ContentPreview('label427');" onmouseout="ContentUnpreview('label427');" title="click to collapse or expand..."> more... </a>
 <div id="label427" style="display:none">
 <table border="1">
 <tr>
 <td></td>
 <td colspan="1">Supported Version Ranges</td>
 </tr>
 <tr>
 <td>ethertype</td>
 <td><code class="docutils literal notranslate">v7.4.2 -> v7.4.2 </code></td>
 </tr>
 </table>
 </div>
 </li>
                <li> <span class="li-head">ext_tag</span> - tcam data extension tag. <span class="li-normal">type: str</span> <span class="li-normal">choices: enable, disable</span>
 <a id='label428' href="javascript:ContentClick('label429', 'label428');" onmouseover="ContentPreview('label429');" onmouseout="ContentUnpreview('label429');" title="click to collapse or expand..."> more... </a>
 <div id="label429" style="display:none">
 <table border="1">
 <tr>
 <td></td>
 <td colspan="1">Supported Version Ranges</td>
 </tr>
 <tr>
 <td>ext_tag</td>
 <td><code class="docutils literal notranslate">v7.4.2 -> v7.4.2 </code></td>
 </tr>
 <tr>
 <td>[enable]</td>
 <td><code class="docutils literal notranslate">v7.4.2 -> v7.4.2</code></td>
 <tr>
 <td>[disable]</td>
 <td><code class="docutils literal notranslate">v7.4.2 -> v7.4.2</code></td>
 </table>
 </div>
 </li>
                <li> <span class="li-head">frag_off</span> - tcam data ip flag fragment offset. <span class="li-normal">type: int</span>
 <a id='label430' href="javascript:ContentClick('label431', 'label430');" onmouseover="ContentPreview('label431');" onmouseout="ContentUnpreview('label431');" title="click to collapse or expand..."> more... </a>
 <div id="label431" style="display:none">
 <table border="1">
 <tr>
 <td></td>
 <td colspan="1">Supported Version Ranges</td>
 </tr>
 <tr>
 <td>frag_off</td>
 <td><code class="docutils literal notranslate">v7.4.2 -> v7.4.2 </code></td>
 </tr>
 </table>
 </div>
 </li>
                <li> <span class="li-head">gen_buf_cnt</span> - tcam data gen info buffer count. <span class="li-normal">type: int</span>
 <a id='label432' href="javascript:ContentClick('label433', 'label432');" onmouseover="ContentPreview('label433');" onmouseout="ContentUnpreview('label433');" title="click to collapse or expand..."> more... </a>
 <div id="label433" style="display:none">
 <table border="1">
 <tr>
 <td></td>
 <td colspan="1">Supported Version Ranges</td>
 </tr>
 <tr>
 <td>gen_buf_cnt</td>
 <td><code class="docutils literal notranslate">v7.4.2 -> v7.4.2 </code></td>
 </tr>
 </table>
 </div>
 </li>
                <li> <span class="li-head">gen_iv</span> - tcam data gen info iv. <span class="li-normal">type: str</span> <span class="li-normal">choices: valid, invalid</span>
 <a id='label434' href="javascript:ContentClick('label435', 'label434');" onmouseover="ContentPreview('label435');" onmouseout="ContentUnpreview('label435');" title="click to collapse or expand..."> more... </a>
 <div id="label435" style="display:none">
 <table border="1">
 <tr>
 <td></td>
 <td colspan="1">Supported Version Ranges</td>
 </tr>
 <tr>
 <td>gen_iv</td>
 <td><code class="docutils literal notranslate">v7.4.2 -> v7.4.2 </code></td>
 </tr>
 <tr>
 <td>[valid]</td>
 <td><code class="docutils literal notranslate">v7.4.2 -> v7.4.2</code></td>
 <tr>
 <td>[invalid]</td>
 <td><code class="docutils literal notranslate">v7.4.2 -> v7.4.2</code></td>
 </table>
 </div>
 </li>
                <li> <span class="li-head">gen_l3_flags</span> - tcam data gen info L3 flags. <span class="li-normal">type: int</span>
 <a id='label436' href="javascript:ContentClick('label437', 'label436');" onmouseover="ContentPreview('label437');" onmouseout="ContentUnpreview('label437');" title="click to collapse or expand..."> more... </a>
 <div id="label437" style="display:none">
 <table border="1">
 <tr>
 <td></td>
 <td colspan="1">Supported Version Ranges</td>
 </tr>
 <tr>
 <td>gen_l3_flags</td>
 <td><code class="docutils literal notranslate">v7.4.2 -> v7.4.2 </code></td>
 </tr>
 </table>
 </div>
 </li>
                <li> <span class="li-head">gen_l4_flags</span> - tcam data gen info L4 flags. <span class="li-normal">type: int</span>
 <a id='label438' href="javascript:ContentClick('label439', 'label438');" onmouseover="ContentPreview('label439');" onmouseout="ContentUnpreview('label439');" title="click to collapse or expand..."> more... </a>
 <div id="label439" style="display:none">
 <table border="1">
 <tr>
 <td></td>
 <td colspan="1">Supported Version Ranges</td>
 </tr>
 <tr>
 <td>gen_l4_flags</td>
 <td><code class="docutils literal notranslate">v7.4.2 -> v7.4.2 </code></td>
 </tr>
 </table>
 </div>
 </li>
                <li> <span class="li-head">gen_pkt_ctrl</span> - tcam data gen info packet control. <span class="li-normal">type: int</span>
 <a id='label440' href="javascript:ContentClick('label441', 'label440');" onmouseover="ContentPreview('label441');" onmouseout="ContentUnpreview('label441');" title="click to collapse or expand..."> more... </a>
 <div id="label441" style="display:none">
 <table border="1">
 <tr>
 <td></td>
 <td colspan="1">Supported Version Ranges</td>
 </tr>
 <tr>
 <td>gen_pkt_ctrl</td>
 <td><code class="docutils literal notranslate">v7.4.2 -> v7.4.2 </code></td>
 </tr>
 </table>
 </div>
 </li>
                <li> <span class="li-head">gen_pri</span> - tcam data gen info priority. <span class="li-normal">type: int</span>
 <a id='label442' href="javascript:ContentClick('label443', 'label442');" onmouseover="ContentPreview('label443');" onmouseout="ContentUnpreview('label443');" title="click to collapse or expand..."> more... </a>
 <div id="label443" style="display:none">
 <table border="1">
 <tr>
 <td></td>
 <td colspan="1">Supported Version Ranges</td>
 </tr>
 <tr>
 <td>gen_pri</td>
 <td><code class="docutils literal notranslate">v7.4.2 -> v7.4.2 </code></td>
 </tr>
 </table>
 </div>
 </li>
                <li> <span class="li-head">gen_pri_v</span> - tcam data gen info priority valid. <span class="li-normal">type: str</span> <span class="li-normal">choices: valid, invalid</span>
 <a id='label444' href="javascript:ContentClick('label445', 'label444');" onmouseover="ContentPreview('label445');" onmouseout="ContentUnpreview('label445');" title="click to collapse or expand..."> more... </a>
 <div id="label445" style="display:none">
 <table border="1">
 <tr>
 <td></td>
 <td colspan="1">Supported Version Ranges</td>
 </tr>
 <tr>
 <td>gen_pri_v</td>
 <td><code class="docutils literal notranslate">v7.4.2 -> v7.4.2 </code></td>
 </tr>
 <tr>
 <td>[valid]</td>
 <td><code class="docutils literal notranslate">v7.4.2 -> v7.4.2</code></td>
 <tr>
 <td>[invalid]</td>
 <td><code class="docutils literal notranslate">v7.4.2 -> v7.4.2</code></td>
 </table>
 </div>
 </li>
                <li> <span class="li-head">gen_tv</span> - tcam data gen info tv. <span class="li-normal">type: str</span> <span class="li-normal">choices: valid, invalid</span>
 <a id='label446' href="javascript:ContentClick('label447', 'label446');" onmouseover="ContentPreview('label447');" onmouseout="ContentUnpreview('label447');" title="click to collapse or expand..."> more... </a>
 <div id="label447" style="display:none">
 <table border="1">
 <tr>
 <td></td>
 <td colspan="1">Supported Version Ranges</td>
 </tr>
 <tr>
 <td>gen_tv</td>
 <td><code class="docutils literal notranslate">v7.4.2 -> v7.4.2 </code></td>
 </tr>
 <tr>
 <td>[valid]</td>
 <td><code class="docutils literal notranslate">v7.4.2 -> v7.4.2</code></td>
 <tr>
 <td>[invalid]</td>
 <td><code class="docutils literal notranslate">v7.4.2 -> v7.4.2</code></td>
 </table>
 </div>
 </li>
                <li> <span class="li-head">ihl</span> - tcam data ipv4 IHL. <span class="li-normal">type: int</span>
 <a id='label448' href="javascript:ContentClick('label449', 'label448');" onmouseover="ContentPreview('label449');" onmouseout="ContentUnpreview('label449');" title="click to collapse or expand..."> more... </a>
 <div id="label449" style="display:none">
 <table border="1">
 <tr>
 <td></td>
 <td colspan="1">Supported Version Ranges</td>
 </tr>
 <tr>
 <td>ihl</td>
 <td><code class="docutils literal notranslate">v7.4.2 -> v7.4.2 </code></td>
 </tr>
 </table>
 </div>
 </li>
                <li> <span class="li-head">ip4_id</span> - tcam data ipv4 id. <span class="li-normal">type: int</span>
 <a id='label450' href="javascript:ContentClick('label451', 'label450');" onmouseover="ContentPreview('label451');" onmouseout="ContentUnpreview('label451');" title="click to collapse or expand..."> more... </a>
 <div id="label451" style="display:none">
 <table border="1">
 <tr>
 <td></td>
 <td colspan="1">Supported Version Ranges</td>
 </tr>
 <tr>
 <td>ip4_id</td>
 <td><code class="docutils literal notranslate">v7.4.2 -> v7.4.2 </code></td>
 </tr>
 </table>
 </div>
 </li>
                <li> <span class="li-head">ip6_fl</span> - tcam data ipv6 flow label. <span class="li-normal">type: int</span>
 <a id='label452' href="javascript:ContentClick('label453', 'label452');" onmouseover="ContentPreview('label453');" onmouseout="ContentUnpreview('label453');" title="click to collapse or expand..."> more... </a>
 <div id="label453" style="display:none">
 <table border="1">
 <tr>
 <td></td>
 <td colspan="1">Supported Version Ranges</td>
 </tr>
 <tr>
 <td>ip6_fl</td>
 <td><code class="docutils literal notranslate">v7.4.2 -> v7.4.2 </code></td>
 </tr>
 </table>
 </div>
 </li>
                <li> <span class="li-head">ipver</span> - tcam data ip header version. <span class="li-normal">type: int</span>
 <a id='label454' href="javascript:ContentClick('label455', 'label454');" onmouseover="ContentPreview('label455');" onmouseout="ContentUnpreview('label455');" title="click to collapse or expand..."> more... </a>
 <div id="label455" style="display:none">
 <table border="1">
 <tr>
 <td></td>
 <td colspan="1">Supported Version Ranges</td>
 </tr>
 <tr>
 <td>ipver</td>
 <td><code class="docutils literal notranslate">v7.4.2 -> v7.4.2 </code></td>
 </tr>
 </table>
 </div>
 </li>
                <li> <span class="li-head">l4_wd10</span> - tcam data L4 word10. <span class="li-normal">type: int</span>
 <a id='label456' href="javascript:ContentClick('label457', 'label456');" onmouseover="ContentPreview('label457');" onmouseout="ContentUnpreview('label457');" title="click to collapse or expand..."> more... </a>
 <div id="label457" style="display:none">
 <table border="1">
 <tr>
 <td></td>
 <td colspan="1">Supported Version Ranges</td>
 </tr>
 <tr>
 <td>l4_wd10</td>
 <td><code class="docutils literal notranslate">v7.4.2 -> v7.4.2 </code></td>
 </tr>
 </table>
 </div>
 </li>
                <li> <span class="li-head">l4_wd11</span> - tcam data L4 word11. <span class="li-normal">type: int</span>
 <a id='label458' href="javascript:ContentClick('label459', 'label458');" onmouseover="ContentPreview('label459');" onmouseout="ContentUnpreview('label459');" title="click to collapse or expand..."> more... </a>
 <div id="label459" style="display:none">
 <table border="1">
 <tr>
 <td></td>
 <td colspan="1">Supported Version Ranges</td>
 </tr>
 <tr>
 <td>l4_wd11</td>
 <td><code class="docutils literal notranslate">v7.4.2 -> v7.4.2 </code></td>
 </tr>
 </table>
 </div>
 </li>
                <li> <span class="li-head">l4_wd8</span> - tcam data L4 word8. <span class="li-normal">type: int</span>
 <a id='label460' href="javascript:ContentClick('label461', 'label460');" onmouseover="ContentPreview('label461');" onmouseout="ContentUnpreview('label461');" title="click to collapse or expand..."> more... </a>
 <div id="label461" style="display:none">
 <table border="1">
 <tr>
 <td></td>
 <td colspan="1">Supported Version Ranges</td>
 </tr>
 <tr>
 <td>l4_wd8</td>
 <td><code class="docutils literal notranslate">v7.4.2 -> v7.4.2 </code></td>
 </tr>
 </table>
 </div>
 </li>
                <li> <span class="li-head">l4_wd9</span> - tcam data L4 word9. <span class="li-normal">type: int</span>
 <a id='label462' href="javascript:ContentClick('label463', 'label462');" onmouseover="ContentPreview('label463');" onmouseout="ContentUnpreview('label463');" title="click to collapse or expand..."> more... </a>
 <div id="label463" style="display:none">
 <table border="1">
 <tr>
 <td></td>
 <td colspan="1">Supported Version Ranges</td>
 </tr>
 <tr>
 <td>l4_wd9</td>
 <td><code class="docutils literal notranslate">v7.4.2 -> v7.4.2 </code></td>
 </tr>
 </table>
 </div>
 </li>
                <li> <span class="li-head">mf</span> - tcam data ip flag mf. <span class="li-normal">type: str</span> <span class="li-normal">choices: enable, disable</span>
 <a id='label464' href="javascript:ContentClick('label465', 'label464');" onmouseover="ContentPreview('label465');" onmouseout="ContentUnpreview('label465');" title="click to collapse or expand..."> more... </a>
 <div id="label465" style="display:none">
 <table border="1">
 <tr>
 <td></td>
 <td colspan="1">Supported Version Ranges</td>
 </tr>
 <tr>
 <td>mf</td>
 <td><code class="docutils literal notranslate">v7.4.2 -> v7.4.2 </code></td>
 </tr>
 <tr>
 <td>[enable]</td>
 <td><code class="docutils literal notranslate">v7.4.2 -> v7.4.2</code></td>
 <tr>
 <td>[disable]</td>
 <td><code class="docutils literal notranslate">v7.4.2 -> v7.4.2</code></td>
 </table>
 </div>
 </li>
                <li> <span class="li-head">protocol</span> - tcam data ip protocol. <span class="li-normal">type: int</span>
 <a id='label466' href="javascript:ContentClick('label467', 'label466');" onmouseover="ContentPreview('label467');" onmouseout="ContentUnpreview('label467');" title="click to collapse or expand..."> more... </a>
 <div id="label467" style="display:none">
 <table border="1">
 <tr>
 <td></td>
 <td colspan="1">Supported Version Ranges</td>
 </tr>
 <tr>
 <td>protocol</td>
 <td><code class="docutils literal notranslate">v7.4.2 -> v7.4.2 </code></td>
 </tr>
 </table>
 </div>
 </li>
                <li> <span class="li-head">slink</span> - tcam data sublink. <span class="li-normal">type: int</span>
 <a id='label468' href="javascript:ContentClick('label469', 'label468');" onmouseover="ContentPreview('label469');" onmouseout="ContentUnpreview('label469');" title="click to collapse or expand..."> more... </a>
 <div id="label469" style="display:none">
 <table border="1">
 <tr>
 <td></td>
 <td colspan="1">Supported Version Ranges</td>
 </tr>
 <tr>
 <td>slink</td>
 <td><code class="docutils literal notranslate">v7.4.2 -> v7.4.2 </code></td>
 </tr>
 </table>
 </div>
 </li>
                <li> <span class="li-head">smac_change</span> - tcam data source MAC change. <span class="li-normal">type: str</span> <span class="li-normal">choices: enable, disable</span>
 <a id='label470' href="javascript:ContentClick('label471', 'label470');" onmouseover="ContentPreview('label471');" onmouseout="ContentUnpreview('label471');" title="click to collapse or expand..."> more... </a>
 <div id="label471" style="display:none">
 <table border="1">
 <tr>
 <td></td>
 <td colspan="1">Supported Version Ranges</td>
 </tr>
 <tr>
 <td>smac_change</td>
 <td><code class="docutils literal notranslate">v7.4.2 -> v7.4.2 </code></td>
 </tr>
 <tr>
 <td>[enable]</td>
 <td><code class="docutils literal notranslate">v7.4.2 -> v7.4.2</code></td>
 <tr>
 <td>[disable]</td>
 <td><code class="docutils literal notranslate">v7.4.2 -> v7.4.2</code></td>
 </table>
 </div>
 </li>
                <li> <span class="li-head">sp</span> - tcam data source port. <span class="li-normal">type: int</span>
 <a id='label472' href="javascript:ContentClick('label473', 'label472');" onmouseover="ContentPreview('label473');" onmouseout="ContentUnpreview('label473');" title="click to collapse or expand..."> more... </a>
 <div id="label473" style="display:none">
 <table border="1">
 <tr>
 <td></td>
 <td colspan="1">Supported Version Ranges</td>
 </tr>
 <tr>
 <td>sp</td>
 <td><code class="docutils literal notranslate">v7.4.2 -> v7.4.2 </code></td>
 </tr>
 </table>
 </div>
 </li>
                <li> <span class="li-head">src_cfi</span> - tcam data source cfi. <span class="li-normal">type: str</span> <span class="li-normal">choices: enable, disable</span>
 <a id='label474' href="javascript:ContentClick('label475', 'label474');" onmouseover="ContentPreview('label475');" onmouseout="ContentUnpreview('label475');" title="click to collapse or expand..."> more... </a>
 <div id="label475" style="display:none">
 <table border="1">
 <tr>
 <td></td>
 <td colspan="1">Supported Version Ranges</td>
 </tr>
 <tr>
 <td>src_cfi</td>
 <td><code class="docutils literal notranslate">v7.4.2 -> v7.4.2 </code></td>
 </tr>
 <tr>
 <td>[enable]</td>
 <td><code class="docutils literal notranslate">v7.4.2 -> v7.4.2</code></td>
 <tr>
 <td>[disable]</td>
 <td><code class="docutils literal notranslate">v7.4.2 -> v7.4.2</code></td>
 </table>
 </div>
 </li>
                <li> <span class="li-head">src_prio</span> - tcam data source priority. <span class="li-normal">type: int</span>
 <a id='label476' href="javascript:ContentClick('label477', 'label476');" onmouseover="ContentPreview('label477');" onmouseout="ContentUnpreview('label477');" title="click to collapse or expand..."> more... </a>
 <div id="label477" style="display:none">
 <table border="1">
 <tr>
 <td></td>
 <td colspan="1">Supported Version Ranges</td>
 </tr>
 <tr>
 <td>src_prio</td>
 <td><code class="docutils literal notranslate">v7.4.2 -> v7.4.2 </code></td>
 </tr>
 </table>
 </div>
 </li>
                <li> <span class="li-head">src_updt</span> - tcam data source update. <span class="li-normal">type: str</span> <span class="li-normal">choices: enable, disable</span>
 <a id='label478' href="javascript:ContentClick('label479', 'label478');" onmouseover="ContentPreview('label479');" onmouseout="ContentUnpreview('label479');" title="click to collapse or expand..."> more... </a>
 <div id="label479" style="display:none">
 <table border="1">
 <tr>
 <td></td>
 <td colspan="1">Supported Version Ranges</td>
 </tr>
 <tr>
 <td>src_updt</td>
 <td><code class="docutils literal notranslate">v7.4.2 -> v7.4.2 </code></td>
 </tr>
 <tr>
 <td>[enable]</td>
 <td><code class="docutils literal notranslate">v7.4.2 -> v7.4.2</code></td>
 <tr>
 <td>[disable]</td>
 <td><code class="docutils literal notranslate">v7.4.2 -> v7.4.2</code></td>
 </table>
 </div>
 </li>
                <li> <span class="li-head">srcip</span> - tcam data src ipv4 address. <span class="li-normal">type: str</span>
 <a id='label480' href="javascript:ContentClick('label481', 'label480');" onmouseover="ContentPreview('label481');" onmouseout="ContentUnpreview('label481');" title="click to collapse or expand..."> more... </a>
 <div id="label481" style="display:none">
 <table border="1">
 <tr>
 <td></td>
 <td colspan="1">Supported Version Ranges</td>
 </tr>
 <tr>
 <td>srcip</td>
 <td><code class="docutils literal notranslate">v7.4.2 -> v7.4.2 </code></td>
 </tr>
 </table>
 </div>
 </li>
                <li> <span class="li-head">srcipv6</span> - tcam data src ipv6 address. <span class="li-normal">type: str</span>
 <a id='label482' href="javascript:ContentClick('label483', 'label482');" onmouseover="ContentPreview('label483');" onmouseout="ContentUnpreview('label483');" title="click to collapse or expand..."> more... </a>
 <div id="label483" style="display:none">
 <table border="1">
 <tr>
 <td></td>
 <td colspan="1">Supported Version Ranges</td>
 </tr>
 <tr>
 <td>srcipv6</td>
 <td><code class="docutils literal notranslate">v7.4.2 -> v7.4.2 </code></td>
 </tr>
 </table>
 </div>
 </li>
                <li> <span class="li-head">srcmac</span> - tcam data src macaddr. <span class="li-normal">type: str</span>
 <a id='label484' href="javascript:ContentClick('label485', 'label484');" onmouseover="ContentPreview('label485');" onmouseout="ContentUnpreview('label485');" title="click to collapse or expand..."> more... </a>
 <div id="label485" style="display:none">
 <table border="1">
 <tr>
 <td></td>
 <td colspan="1">Supported Version Ranges</td>
 </tr>
 <tr>
 <td>srcmac</td>
 <td><code class="docutils literal notranslate">v7.4.2 -> v7.4.2 </code></td>
 </tr>
 </table>
 </div>
 </li>
                <li> <span class="li-head">srcport</span> - tcam data L4 src port. <span class="li-normal">type: int</span>
 <a id='label486' href="javascript:ContentClick('label487', 'label486');" onmouseover="ContentPreview('label487');" onmouseout="ContentUnpreview('label487');" title="click to collapse or expand..."> more... </a>
 <div id="label487" style="display:none">
 <table border="1">
 <tr>
 <td></td>
 <td colspan="1">Supported Version Ranges</td>
 </tr>
 <tr>
 <td>srcport</td>
 <td><code class="docutils literal notranslate">v7.4.2 -> v7.4.2 </code></td>
 </tr>
 </table>
 </div>
 </li>
                <li> <span class="li-head">svid</span> - tcam data source vid. <span class="li-normal">type: int</span>
 <a id='label488' href="javascript:ContentClick('label489', 'label488');" onmouseover="ContentPreview('label489');" onmouseout="ContentUnpreview('label489');" title="click to collapse or expand..."> more... </a>
 <div id="label489" style="display:none">
 <table border="1">
 <tr>
 <td></td>
 <td colspan="1">Supported Version Ranges</td>
 </tr>
 <tr>
 <td>svid</td>
 <td><code class="docutils literal notranslate">v7.4.2 -> v7.4.2 </code></td>
 </tr>
 </table>
 </div>
 </li>
                <li> <span class="li-head">tcp_ack</span> - tcam data tcp flag ack. <span class="li-normal">type: str</span> <span class="li-normal">choices: enable, disable</span>
 <a id='label490' href="javascript:ContentClick('label491', 'label490');" onmouseover="ContentPreview('label491');" onmouseout="ContentUnpreview('label491');" title="click to collapse or expand..."> more... </a>
 <div id="label491" style="display:none">
 <table border="1">
 <tr>
 <td></td>
 <td colspan="1">Supported Version Ranges</td>
 </tr>
 <tr>
 <td>tcp_ack</td>
 <td><code class="docutils literal notranslate">v7.4.2 -> v7.4.2 </code></td>
 </tr>
 <tr>
 <td>[enable]</td>
 <td><code class="docutils literal notranslate">v7.4.2 -> v7.4.2</code></td>
 <tr>
 <td>[disable]</td>
 <td><code class="docutils literal notranslate">v7.4.2 -> v7.4.2</code></td>
 </table>
 </div>
 </li>
                <li> <span class="li-head">tcp_cwr</span> - tcam data tcp flag cwr. <span class="li-normal">type: str</span> <span class="li-normal">choices: enable, disable</span>
 <a id='label492' href="javascript:ContentClick('label493', 'label492');" onmouseover="ContentPreview('label493');" onmouseout="ContentUnpreview('label493');" title="click to collapse or expand..."> more... </a>
 <div id="label493" style="display:none">
 <table border="1">
 <tr>
 <td></td>
 <td colspan="1">Supported Version Ranges</td>
 </tr>
 <tr>
 <td>tcp_cwr</td>
 <td><code class="docutils literal notranslate">v7.4.2 -> v7.4.2 </code></td>
 </tr>
 <tr>
 <td>[enable]</td>
 <td><code class="docutils literal notranslate">v7.4.2 -> v7.4.2</code></td>
 <tr>
 <td>[disable]</td>
 <td><code class="docutils literal notranslate">v7.4.2 -> v7.4.2</code></td>
 </table>
 </div>
 </li>
                <li> <span class="li-head">tcp_ece</span> - tcam data tcp flag ece. <span class="li-normal">type: str</span> <span class="li-normal">choices: enable, disable</span>
 <a id='label494' href="javascript:ContentClick('label495', 'label494');" onmouseover="ContentPreview('label495');" onmouseout="ContentUnpreview('label495');" title="click to collapse or expand..."> more... </a>
 <div id="label495" style="display:none">
 <table border="1">
 <tr>
 <td></td>
 <td colspan="1">Supported Version Ranges</td>
 </tr>
 <tr>
 <td>tcp_ece</td>
 <td><code class="docutils literal notranslate">v7.4.2 -> v7.4.2 </code></td>
 </tr>
 <tr>
 <td>[enable]</td>
 <td><code class="docutils literal notranslate">v7.4.2 -> v7.4.2</code></td>
 <tr>
 <td>[disable]</td>
 <td><code class="docutils literal notranslate">v7.4.2 -> v7.4.2</code></td>
 </table>
 </div>
 </li>
                <li> <span class="li-head">tcp_fin</span> - tcam data tcp flag fin. <span class="li-normal">type: str</span> <span class="li-normal">choices: enable, disable</span>
 <a id='label496' href="javascript:ContentClick('label497', 'label496');" onmouseover="ContentPreview('label497');" onmouseout="ContentUnpreview('label497');" title="click to collapse or expand..."> more... </a>
 <div id="label497" style="display:none">
 <table border="1">
 <tr>
 <td></td>
 <td colspan="1">Supported Version Ranges</td>
 </tr>
 <tr>
 <td>tcp_fin</td>
 <td><code class="docutils literal notranslate">v7.4.2 -> v7.4.2 </code></td>
 </tr>
 <tr>
 <td>[enable]</td>
 <td><code class="docutils literal notranslate">v7.4.2 -> v7.4.2</code></td>
 <tr>
 <td>[disable]</td>
 <td><code class="docutils literal notranslate">v7.4.2 -> v7.4.2</code></td>
 </table>
 </div>
 </li>
                <li> <span class="li-head">tcp_push</span> - tcam data tcp flag push. <span class="li-normal">type: str</span> <span class="li-normal">choices: enable, disable</span>
 <a id='label498' href="javascript:ContentClick('label499', 'label498');" onmouseover="ContentPreview('label499');" onmouseout="ContentUnpreview('label499');" title="click to collapse or expand..."> more... </a>
 <div id="label499" style="display:none">
 <table border="1">
 <tr>
 <td></td>
 <td colspan="1">Supported Version Ranges</td>
 </tr>
 <tr>
 <td>tcp_push</td>
 <td><code class="docutils literal notranslate">v7.4.2 -> v7.4.2 </code></td>
 </tr>
 <tr>
 <td>[enable]</td>
 <td><code class="docutils literal notranslate">v7.4.2 -> v7.4.2</code></td>
 <tr>
 <td>[disable]</td>
 <td><code class="docutils literal notranslate">v7.4.2 -> v7.4.2</code></td>
 </table>
 </div>
 </li>
                <li> <span class="li-head">tcp_rst</span> - tcam data tcp flag rst. <span class="li-normal">type: str</span> <span class="li-normal">choices: enable, disable</span>
 <a id='label500' href="javascript:ContentClick('label501', 'label500');" onmouseover="ContentPreview('label501');" onmouseout="ContentUnpreview('label501');" title="click to collapse or expand..."> more... </a>
 <div id="label501" style="display:none">
 <table border="1">
 <tr>
 <td></td>
 <td colspan="1">Supported Version Ranges</td>
 </tr>
 <tr>
 <td>tcp_rst</td>
 <td><code class="docutils literal notranslate">v7.4.2 -> v7.4.2 </code></td>
 </tr>
 <tr>
 <td>[enable]</td>
 <td><code class="docutils literal notranslate">v7.4.2 -> v7.4.2</code></td>
 <tr>
 <td>[disable]</td>
 <td><code class="docutils literal notranslate">v7.4.2 -> v7.4.2</code></td>
 </table>
 </div>
 </li>
                <li> <span class="li-head">tcp_syn</span> - tcam data tcp flag syn. <span class="li-normal">type: str</span> <span class="li-normal">choices: enable, disable</span>
 <a id='label502' href="javascript:ContentClick('label503', 'label502');" onmouseover="ContentPreview('label503');" onmouseout="ContentUnpreview('label503');" title="click to collapse or expand..."> more... </a>
 <div id="label503" style="display:none">
 <table border="1">
 <tr>
 <td></td>
 <td colspan="1">Supported Version Ranges</td>
 </tr>
 <tr>
 <td>tcp_syn</td>
 <td><code class="docutils literal notranslate">v7.4.2 -> v7.4.2 </code></td>
 </tr>
 <tr>
 <td>[enable]</td>
 <td><code class="docutils literal notranslate">v7.4.2 -> v7.4.2</code></td>
 <tr>
 <td>[disable]</td>
 <td><code class="docutils literal notranslate">v7.4.2 -> v7.4.2</code></td>
 </table>
 </div>
 </li>
                <li> <span class="li-head">tcp_urg</span> - tcam data tcp flag urg. <span class="li-normal">type: str</span> <span class="li-normal">choices: enable, disable</span>
 <a id='label504' href="javascript:ContentClick('label505', 'label504');" onmouseover="ContentPreview('label505');" onmouseout="ContentUnpreview('label505');" title="click to collapse or expand..."> more... </a>
 <div id="label505" style="display:none">
 <table border="1">
 <tr>
 <td></td>
 <td colspan="1">Supported Version Ranges</td>
 </tr>
 <tr>
 <td>tcp_urg</td>
 <td><code class="docutils literal notranslate">v7.4.2 -> v7.4.2 </code></td>
 </tr>
 <tr>
 <td>[enable]</td>
 <td><code class="docutils literal notranslate">v7.4.2 -> v7.4.2</code></td>
 <tr>
 <td>[disable]</td>
 <td><code class="docutils literal notranslate">v7.4.2 -> v7.4.2</code></td>
 </table>
 </div>
 </li>
                <li> <span class="li-head">tgt_cfi</span> - tcam data target cfi. <span class="li-normal">type: str</span> <span class="li-normal">choices: enable, disable</span>
 <a id='label506' href="javascript:ContentClick('label507', 'label506');" onmouseover="ContentPreview('label507');" onmouseout="ContentUnpreview('label507');" title="click to collapse or expand..."> more... </a>
 <div id="label507" style="display:none">
 <table border="1">
 <tr>
 <td></td>
 <td colspan="1">Supported Version Ranges</td>
 </tr>
 <tr>
 <td>tgt_cfi</td>
 <td><code class="docutils literal notranslate">v7.4.2 -> v7.4.2 </code></td>
 </tr>
 <tr>
 <td>[enable]</td>
 <td><code class="docutils literal notranslate">v7.4.2 -> v7.4.2</code></td>
 <tr>
 <td>[disable]</td>
 <td><code class="docutils literal notranslate">v7.4.2 -> v7.4.2</code></td>
 </table>
 </div>
 </li>
                <li> <span class="li-head">tgt_prio</span> - tcam data target priority. <span class="li-normal">type: int</span>
 <a id='label508' href="javascript:ContentClick('label509', 'label508');" onmouseover="ContentPreview('label509');" onmouseout="ContentUnpreview('label509');" title="click to collapse or expand..."> more... </a>
 <div id="label509" style="display:none">
 <table border="1">
 <tr>
 <td></td>
 <td colspan="1">Supported Version Ranges</td>
 </tr>
 <tr>
 <td>tgt_prio</td>
 <td><code class="docutils literal notranslate">v7.4.2 -> v7.4.2 </code></td>
 </tr>
 </table>
 </div>
 </li>
                <li> <span class="li-head">tgt_updt</span> - tcam data target port update. <span class="li-normal">type: str</span> <span class="li-normal">choices: enable, disable</span>
 <a id='label510' href="javascript:ContentClick('label511', 'label510');" onmouseover="ContentPreview('label511');" onmouseout="ContentUnpreview('label511');" title="click to collapse or expand..."> more... </a>
 <div id="label511" style="display:none">
 <table border="1">
 <tr>
 <td></td>
 <td colspan="1">Supported Version Ranges</td>
 </tr>
 <tr>
 <td>tgt_updt</td>
 <td><code class="docutils literal notranslate">v7.4.2 -> v7.4.2 </code></td>
 </tr>
 <tr>
 <td>[enable]</td>
 <td><code class="docutils literal notranslate">v7.4.2 -> v7.4.2</code></td>
 <tr>
 <td>[disable]</td>
 <td><code class="docutils literal notranslate">v7.4.2 -> v7.4.2</code></td>
 </table>
 </div>
 </li>
                <li> <span class="li-head">tgt_v</span> - tcam data target valid. <span class="li-normal">type: str</span> <span class="li-normal">choices: valid, invalid</span>
 <a id='label512' href="javascript:ContentClick('label513', 'label512');" onmouseover="ContentPreview('label513');" onmouseout="ContentUnpreview('label513');" title="click to collapse or expand..."> more... </a>
 <div id="label513" style="display:none">
 <table border="1">
 <tr>
 <td></td>
 <td colspan="1">Supported Version Ranges</td>
 </tr>
 <tr>
 <td>tgt_v</td>
 <td><code class="docutils literal notranslate">v7.4.2 -> v7.4.2 </code></td>
 </tr>
 <tr>
 <td>[valid]</td>
 <td><code class="docutils literal notranslate">v7.4.2 -> v7.4.2</code></td>
 <tr>
 <td>[invalid]</td>
 <td><code class="docutils literal notranslate">v7.4.2 -> v7.4.2</code></td>
 </table>
 </div>
 </li>
                <li> <span class="li-head">tos</span> - tcam data ip tos. <span class="li-normal">type: int</span>
 <a id='label514' href="javascript:ContentClick('label515', 'label514');" onmouseover="ContentPreview('label515');" onmouseout="ContentUnpreview('label515');" title="click to collapse or expand..."> more... </a>
 <div id="label515" style="display:none">
 <table border="1">
 <tr>
 <td></td>
 <td colspan="1">Supported Version Ranges</td>
 </tr>
 <tr>
 <td>tos</td>
 <td><code class="docutils literal notranslate">v7.4.2 -> v7.4.2 </code></td>
 </tr>
 </table>
 </div>
 </li>
                <li> <span class="li-head">tp</span> - tcam data target port. <span class="li-normal">type: int</span>
 <a id='label516' href="javascript:ContentClick('label517', 'label516');" onmouseover="ContentPreview('label517');" onmouseout="ContentUnpreview('label517');" title="click to collapse or expand..."> more... </a>
 <div id="label517" style="display:none">
 <table border="1">
 <tr>
 <td></td>
 <td colspan="1">Supported Version Ranges</td>
 </tr>
 <tr>
 <td>tp</td>
 <td><code class="docutils literal notranslate">v7.4.2 -> v7.4.2 </code></td>
 </tr>
 </table>
 </div>
 </li>
                <li> <span class="li-head">ttl</span> - tcam data ip ttl. <span class="li-normal">type: int</span>
 <a id='label518' href="javascript:ContentClick('label519', 'label518');" onmouseover="ContentPreview('label519');" onmouseout="ContentUnpreview('label519');" title="click to collapse or expand..."> more... </a>
 <div id="label519" style="display:none">
 <table border="1">
 <tr>
 <td></td>
 <td colspan="1">Supported Version Ranges</td>
 </tr>
 <tr>
 <td>ttl</td>
 <td><code class="docutils literal notranslate">v7.4.2 -> v7.4.2 </code></td>
 </tr>
 </table>
 </div>
 </li>
                <li> <span class="li-head">tvid</span> - tcam data target vid. <span class="li-normal">type: int</span>
 <a id='label520' href="javascript:ContentClick('label521', 'label520');" onmouseover="ContentPreview('label521');" onmouseout="ContentUnpreview('label521');" title="click to collapse or expand..."> more... </a>
 <div id="label521" style="display:none">
 <table border="1">
 <tr>
 <td></td>
 <td colspan="1">Supported Version Ranges</td>
 </tr>
 <tr>
 <td>tvid</td>
 <td><code class="docutils literal notranslate">v7.4.2 -> v7.4.2 </code></td>
 </tr>
 </table>
 </div>
 </li>
                <li> <span class="li-head">vdid</span> - tcam data vdom id. <span class="li-normal">type: int</span>
 <a id='label522' href="javascript:ContentClick('label523', 'label522');" onmouseover="ContentPreview('label523');" onmouseout="ContentUnpreview('label523');" title="click to collapse or expand..."> more... </a>
 <div id="label523" style="display:none">
 <table border="1">
 <tr>
 <td></td>
 <td colspan="1">Supported Version Ranges</td>
 </tr>
 <tr>
 <td>vdid</td>
 <td><code class="docutils literal notranslate">v7.4.2 -> v7.4.2 </code></td>
 </tr>
 </table>
 </div>
 </li>
                </ul>
            <li> <span class="li-head">mask</span> - Mask fields of TCAM. <span class="li-normal">type: dict</span>
 <a id='label524' href="javascript:ContentClick('label525', 'label524');" onmouseover="ContentPreview('label525');" onmouseout="ContentUnpreview('label525');" title="click to collapse or expand..."> more... </a>
 <div id="label525" style="display:none">
 <table border="1">
 <tr>
 <td></td><td colspan="1">Supported Version Ranges</td>
 </tr>
 <tr>
 <td>mask</td>
 <td><code class="docutils literal notranslate">v7.4.2 -> v7.4.2 </code></td>
 </tr>
 </table>
 </div>
 </li>
                <ul class="ul-self">
                <li> <span class="li-head">df</span> - tcam mask ip flag df. <span class="li-normal">type: str</span> <span class="li-normal">choices: enable, disable</span>
 <a id='label526' href="javascript:ContentClick('label527', 'label526');" onmouseover="ContentPreview('label527');" onmouseout="ContentUnpreview('label527');" title="click to collapse or expand..."> more... </a>
 <div id="label527" style="display:none">
 <table border="1">
 <tr>
 <td></td>
 <td colspan="1">Supported Version Ranges</td>
 </tr>
 <tr>
 <td>df</td>
 <td><code class="docutils literal notranslate">v7.4.2 -> v7.4.2 </code></td>
 </tr>
 <tr>
 <td>[enable]</td>
 <td><code class="docutils literal notranslate">v7.4.2 -> v7.4.2</code></td>
 <tr>
 <td>[disable]</td>
 <td><code class="docutils literal notranslate">v7.4.2 -> v7.4.2</code></td>
 </table>
 </div>
 </li>
                <li> <span class="li-head">dstip</span> - tcam mask dst ipv4 address. <span class="li-normal">type: str</span>
 <a id='label528' href="javascript:ContentClick('label529', 'label528');" onmouseover="ContentPreview('label529');" onmouseout="ContentUnpreview('label529');" title="click to collapse or expand..."> more... </a>
 <div id="label529" style="display:none">
 <table border="1">
 <tr>
 <td></td>
 <td colspan="1">Supported Version Ranges</td>
 </tr>
 <tr>
 <td>dstip</td>
 <td><code class="docutils literal notranslate">v7.4.2 -> v7.4.2 </code></td>
 </tr>
 </table>
 </div>
 </li>
                <li> <span class="li-head">dstipv6</span> - tcam mask dst ipv6 address. <span class="li-normal">type: str</span>
 <a id='label530' href="javascript:ContentClick('label531', 'label530');" onmouseover="ContentPreview('label531');" onmouseout="ContentUnpreview('label531');" title="click to collapse or expand..."> more... </a>
 <div id="label531" style="display:none">
 <table border="1">
 <tr>
 <td></td>
 <td colspan="1">Supported Version Ranges</td>
 </tr>
 <tr>
 <td>dstipv6</td>
 <td><code class="docutils literal notranslate">v7.4.2 -> v7.4.2 </code></td>
 </tr>
 </table>
 </div>
 </li>
                <li> <span class="li-head">dstmac</span> - tcam mask dst macaddr. <span class="li-normal">type: str</span>
 <a id='label532' href="javascript:ContentClick('label533', 'label532');" onmouseover="ContentPreview('label533');" onmouseout="ContentUnpreview('label533');" title="click to collapse or expand..."> more... </a>
 <div id="label533" style="display:none">
 <table border="1">
 <tr>
 <td></td>
 <td colspan="1">Supported Version Ranges</td>
 </tr>
 <tr>
 <td>dstmac</td>
 <td><code class="docutils literal notranslate">v7.4.2 -> v7.4.2 </code></td>
 </tr>
 </table>
 </div>
 </li>
                <li> <span class="li-head">dstport</span> - tcam mask L4 dst port. <span class="li-normal">type: int</span>
 <a id='label534' href="javascript:ContentClick('label535', 'label534');" onmouseover="ContentPreview('label535');" onmouseout="ContentUnpreview('label535');" title="click to collapse or expand..."> more... </a>
 <div id="label535" style="display:none">
 <table border="1">
 <tr>
 <td></td>
 <td colspan="1">Supported Version Ranges</td>
 </tr>
 <tr>
 <td>dstport</td>
 <td><code class="docutils literal notranslate">v7.4.2 -> v7.4.2 </code></td>
 </tr>
 </table>
 </div>
 </li>
                <li> <span class="li-head">ethertype</span> - tcam mask ethertype. <span class="li-normal">type: str</span>
 <a id='label536' href="javascript:ContentClick('label537', 'label536');" onmouseover="ContentPreview('label537');" onmouseout="ContentUnpreview('label537');" title="click to collapse or expand..."> more... </a>
 <div id="label537" style="display:none">
 <table border="1">
 <tr>
 <td></td>
 <td colspan="1">Supported Version Ranges</td>
 </tr>
 <tr>
 <td>ethertype</td>
 <td><code class="docutils literal notranslate">v7.4.2 -> v7.4.2 </code></td>
 </tr>
 </table>
 </div>
 </li>
                <li> <span class="li-head">ext_tag</span> - tcam mask extension tag. <span class="li-normal">type: str</span> <span class="li-normal">choices: enable, disable</span>
 <a id='label538' href="javascript:ContentClick('label539', 'label538');" onmouseover="ContentPreview('label539');" onmouseout="ContentUnpreview('label539');" title="click to collapse or expand..."> more... </a>
 <div id="label539" style="display:none">
 <table border="1">
 <tr>
 <td></td>
 <td colspan="1">Supported Version Ranges</td>
 </tr>
 <tr>
 <td>ext_tag</td>
 <td><code class="docutils literal notranslate">v7.4.2 -> v7.4.2 </code></td>
 </tr>
 <tr>
 <td>[enable]</td>
 <td><code class="docutils literal notranslate">v7.4.2 -> v7.4.2</code></td>
 <tr>
 <td>[disable]</td>
 <td><code class="docutils literal notranslate">v7.4.2 -> v7.4.2</code></td>
 </table>
 </div>
 </li>
                <li> <span class="li-head">frag_off</span> - tcam data ip flag fragment offset. <span class="li-normal">type: int</span>
 <a id='label540' href="javascript:ContentClick('label541', 'label540');" onmouseover="ContentPreview('label541');" onmouseout="ContentUnpreview('label541');" title="click to collapse or expand..."> more... </a>
 <div id="label541" style="display:none">
 <table border="1">
 <tr>
 <td></td>
 <td colspan="1">Supported Version Ranges</td>
 </tr>
 <tr>
 <td>frag_off</td>
 <td><code class="docutils literal notranslate">v7.4.2 -> v7.4.2 </code></td>
 </tr>
 </table>
 </div>
 </li>
                <li> <span class="li-head">gen_buf_cnt</span> - tcam mask gen info buffer count. <span class="li-normal">type: int</span>
 <a id='label542' href="javascript:ContentClick('label543', 'label542');" onmouseover="ContentPreview('label543');" onmouseout="ContentUnpreview('label543');" title="click to collapse or expand..."> more... </a>
 <div id="label543" style="display:none">
 <table border="1">
 <tr>
 <td></td>
 <td colspan="1">Supported Version Ranges</td>
 </tr>
 <tr>
 <td>gen_buf_cnt</td>
 <td><code class="docutils literal notranslate">v7.4.2 -> v7.4.2 </code></td>
 </tr>
 </table>
 </div>
 </li>
                <li> <span class="li-head">gen_iv</span> - tcam mask gen info iv. <span class="li-normal">type: str</span> <span class="li-normal">choices: valid, invalid</span>
 <a id='label544' href="javascript:ContentClick('label545', 'label544');" onmouseover="ContentPreview('label545');" onmouseout="ContentUnpreview('label545');" title="click to collapse or expand..."> more... </a>
 <div id="label545" style="display:none">
 <table border="1">
 <tr>
 <td></td>
 <td colspan="1">Supported Version Ranges</td>
 </tr>
 <tr>
 <td>gen_iv</td>
 <td><code class="docutils literal notranslate">v7.4.2 -> v7.4.2 </code></td>
 </tr>
 <tr>
 <td>[valid]</td>
 <td><code class="docutils literal notranslate">v7.4.2 -> v7.4.2</code></td>
 <tr>
 <td>[invalid]</td>
 <td><code class="docutils literal notranslate">v7.4.2 -> v7.4.2</code></td>
 </table>
 </div>
 </li>
                <li> <span class="li-head">gen_l3_flags</span> - tcam mask gen info L3 flags. <span class="li-normal">type: int</span>
 <a id='label546' href="javascript:ContentClick('label547', 'label546');" onmouseover="ContentPreview('label547');" onmouseout="ContentUnpreview('label547');" title="click to collapse or expand..."> more... </a>
 <div id="label547" style="display:none">
 <table border="1">
 <tr>
 <td></td>
 <td colspan="1">Supported Version Ranges</td>
 </tr>
 <tr>
 <td>gen_l3_flags</td>
 <td><code class="docutils literal notranslate">v7.4.2 -> v7.4.2 </code></td>
 </tr>
 </table>
 </div>
 </li>
                <li> <span class="li-head">gen_l4_flags</span> - tcam mask gen info L4 flags. <span class="li-normal">type: int</span>
 <a id='label548' href="javascript:ContentClick('label549', 'label548');" onmouseover="ContentPreview('label549');" onmouseout="ContentUnpreview('label549');" title="click to collapse or expand..."> more... </a>
 <div id="label549" style="display:none">
 <table border="1">
 <tr>
 <td></td>
 <td colspan="1">Supported Version Ranges</td>
 </tr>
 <tr>
 <td>gen_l4_flags</td>
 <td><code class="docutils literal notranslate">v7.4.2 -> v7.4.2 </code></td>
 </tr>
 </table>
 </div>
 </li>
                <li> <span class="li-head">gen_pkt_ctrl</span> - tcam mask gen info packet control. <span class="li-normal">type: int</span>
 <a id='label550' href="javascript:ContentClick('label551', 'label550');" onmouseover="ContentPreview('label551');" onmouseout="ContentUnpreview('label551');" title="click to collapse or expand..."> more... </a>
 <div id="label551" style="display:none">
 <table border="1">
 <tr>
 <td></td>
 <td colspan="1">Supported Version Ranges</td>
 </tr>
 <tr>
 <td>gen_pkt_ctrl</td>
 <td><code class="docutils literal notranslate">v7.4.2 -> v7.4.2 </code></td>
 </tr>
 </table>
 </div>
 </li>
                <li> <span class="li-head">gen_pri</span> - tcam mask gen info priority. <span class="li-normal">type: int</span>
 <a id='label552' href="javascript:ContentClick('label553', 'label552');" onmouseover="ContentPreview('label553');" onmouseout="ContentUnpreview('label553');" title="click to collapse or expand..."> more... </a>
 <div id="label553" style="display:none">
 <table border="1">
 <tr>
 <td></td>
 <td colspan="1">Supported Version Ranges</td>
 </tr>
 <tr>
 <td>gen_pri</td>
 <td><code class="docutils literal notranslate">v7.4.2 -> v7.4.2 </code></td>
 </tr>
 </table>
 </div>
 </li>
                <li> <span class="li-head">gen_pri_v</span> - tcam mask gen info priority valid. <span class="li-normal">type: str</span> <span class="li-normal">choices: valid, invalid</span>
 <a id='label554' href="javascript:ContentClick('label555', 'label554');" onmouseover="ContentPreview('label555');" onmouseout="ContentUnpreview('label555');" title="click to collapse or expand..."> more... </a>
 <div id="label555" style="display:none">
 <table border="1">
 <tr>
 <td></td>
 <td colspan="1">Supported Version Ranges</td>
 </tr>
 <tr>
 <td>gen_pri_v</td>
 <td><code class="docutils literal notranslate">v7.4.2 -> v7.4.2 </code></td>
 </tr>
 <tr>
 <td>[valid]</td>
 <td><code class="docutils literal notranslate">v7.4.2 -> v7.4.2</code></td>
 <tr>
 <td>[invalid]</td>
 <td><code class="docutils literal notranslate">v7.4.2 -> v7.4.2</code></td>
 </table>
 </div>
 </li>
                <li> <span class="li-head">gen_tv</span> - tcam mask gen info tv. <span class="li-normal">type: str</span> <span class="li-normal">choices: valid, invalid</span>
 <a id='label556' href="javascript:ContentClick('label557', 'label556');" onmouseover="ContentPreview('label557');" onmouseout="ContentUnpreview('label557');" title="click to collapse or expand..."> more... </a>
 <div id="label557" style="display:none">
 <table border="1">
 <tr>
 <td></td>
 <td colspan="1">Supported Version Ranges</td>
 </tr>
 <tr>
 <td>gen_tv</td>
 <td><code class="docutils literal notranslate">v7.4.2 -> v7.4.2 </code></td>
 </tr>
 <tr>
 <td>[valid]</td>
 <td><code class="docutils literal notranslate">v7.4.2 -> v7.4.2</code></td>
 <tr>
 <td>[invalid]</td>
 <td><code class="docutils literal notranslate">v7.4.2 -> v7.4.2</code></td>
 </table>
 </div>
 </li>
                <li> <span class="li-head">ihl</span> - tcam mask ipv4 IHL. <span class="li-normal">type: int</span>
 <a id='label558' href="javascript:ContentClick('label559', 'label558');" onmouseover="ContentPreview('label559');" onmouseout="ContentUnpreview('label559');" title="click to collapse or expand..."> more... </a>
 <div id="label559" style="display:none">
 <table border="1">
 <tr>
 <td></td>
 <td colspan="1">Supported Version Ranges</td>
 </tr>
 <tr>
 <td>ihl</td>
 <td><code class="docutils literal notranslate">v7.4.2 -> v7.4.2 </code></td>
 </tr>
 </table>
 </div>
 </li>
                <li> <span class="li-head">ip4_id</span> - tcam mask ipv4 id. <span class="li-normal">type: int</span>
 <a id='label560' href="javascript:ContentClick('label561', 'label560');" onmouseover="ContentPreview('label561');" onmouseout="ContentUnpreview('label561');" title="click to collapse or expand..."> more... </a>
 <div id="label561" style="display:none">
 <table border="1">
 <tr>
 <td></td>
 <td colspan="1">Supported Version Ranges</td>
 </tr>
 <tr>
 <td>ip4_id</td>
 <td><code class="docutils literal notranslate">v7.4.2 -> v7.4.2 </code></td>
 </tr>
 </table>
 </div>
 </li>
                <li> <span class="li-head">ip6_fl</span> - tcam mask ipv6 flow label. <span class="li-normal">type: int</span>
 <a id='label562' href="javascript:ContentClick('label563', 'label562');" onmouseover="ContentPreview('label563');" onmouseout="ContentUnpreview('label563');" title="click to collapse or expand..."> more... </a>
 <div id="label563" style="display:none">
 <table border="1">
 <tr>
 <td></td>
 <td colspan="1">Supported Version Ranges</td>
 </tr>
 <tr>
 <td>ip6_fl</td>
 <td><code class="docutils literal notranslate">v7.4.2 -> v7.4.2 </code></td>
 </tr>
 </table>
 </div>
 </li>
                <li> <span class="li-head">ipver</span> - tcam mask ip header version. <span class="li-normal">type: int</span>
 <a id='label564' href="javascript:ContentClick('label565', 'label564');" onmouseover="ContentPreview('label565');" onmouseout="ContentUnpreview('label565');" title="click to collapse or expand..."> more... </a>
 <div id="label565" style="display:none">
 <table border="1">
 <tr>
 <td></td>
 <td colspan="1">Supported Version Ranges</td>
 </tr>
 <tr>
 <td>ipver</td>
 <td><code class="docutils literal notranslate">v7.4.2 -> v7.4.2 </code></td>
 </tr>
 </table>
 </div>
 </li>
                <li> <span class="li-head">l4_wd10</span> - tcam mask L4 word10. <span class="li-normal">type: int</span>
 <a id='label566' href="javascript:ContentClick('label567', 'label566');" onmouseover="ContentPreview('label567');" onmouseout="ContentUnpreview('label567');" title="click to collapse or expand..."> more... </a>
 <div id="label567" style="display:none">
 <table border="1">
 <tr>
 <td></td>
 <td colspan="1">Supported Version Ranges</td>
 </tr>
 <tr>
 <td>l4_wd10</td>
 <td><code class="docutils literal notranslate">v7.4.2 -> v7.4.2 </code></td>
 </tr>
 </table>
 </div>
 </li>
                <li> <span class="li-head">l4_wd11</span> - tcam mask L4 word11. <span class="li-normal">type: int</span>
 <a id='label568' href="javascript:ContentClick('label569', 'label568');" onmouseover="ContentPreview('label569');" onmouseout="ContentUnpreview('label569');" title="click to collapse or expand..."> more... </a>
 <div id="label569" style="display:none">
 <table border="1">
 <tr>
 <td></td>
 <td colspan="1">Supported Version Ranges</td>
 </tr>
 <tr>
 <td>l4_wd11</td>
 <td><code class="docutils literal notranslate">v7.4.2 -> v7.4.2 </code></td>
 </tr>
 </table>
 </div>
 </li>
                <li> <span class="li-head">l4_wd8</span> - tcam mask L4 word8. <span class="li-normal">type: int</span>
 <a id='label570' href="javascript:ContentClick('label571', 'label570');" onmouseover="ContentPreview('label571');" onmouseout="ContentUnpreview('label571');" title="click to collapse or expand..."> more... </a>
 <div id="label571" style="display:none">
 <table border="1">
 <tr>
 <td></td>
 <td colspan="1">Supported Version Ranges</td>
 </tr>
 <tr>
 <td>l4_wd8</td>
 <td><code class="docutils literal notranslate">v7.4.2 -> v7.4.2 </code></td>
 </tr>
 </table>
 </div>
 </li>
                <li> <span class="li-head">l4_wd9</span> - tcam mask L4 word9. <span class="li-normal">type: int</span>
 <a id='label572' href="javascript:ContentClick('label573', 'label572');" onmouseover="ContentPreview('label573');" onmouseout="ContentUnpreview('label573');" title="click to collapse or expand..."> more... </a>
 <div id="label573" style="display:none">
 <table border="1">
 <tr>
 <td></td>
 <td colspan="1">Supported Version Ranges</td>
 </tr>
 <tr>
 <td>l4_wd9</td>
 <td><code class="docutils literal notranslate">v7.4.2 -> v7.4.2 </code></td>
 </tr>
 </table>
 </div>
 </li>
                <li> <span class="li-head">mf</span> - tcam mask ip flag mf. <span class="li-normal">type: str</span> <span class="li-normal">choices: enable, disable</span>
 <a id='label574' href="javascript:ContentClick('label575', 'label574');" onmouseover="ContentPreview('label575');" onmouseout="ContentUnpreview('label575');" title="click to collapse or expand..."> more... </a>
 <div id="label575" style="display:none">
 <table border="1">
 <tr>
 <td></td>
 <td colspan="1">Supported Version Ranges</td>
 </tr>
 <tr>
 <td>mf</td>
 <td><code class="docutils literal notranslate">v7.4.2 -> v7.4.2 </code></td>
 </tr>
 <tr>
 <td>[enable]</td>
 <td><code class="docutils literal notranslate">v7.4.2 -> v7.4.2</code></td>
 <tr>
 <td>[disable]</td>
 <td><code class="docutils literal notranslate">v7.4.2 -> v7.4.2</code></td>
 </table>
 </div>
 </li>
                <li> <span class="li-head">protocol</span> - tcam mask ip protocol. <span class="li-normal">type: int</span>
 <a id='label576' href="javascript:ContentClick('label577', 'label576');" onmouseover="ContentPreview('label577');" onmouseout="ContentUnpreview('label577');" title="click to collapse or expand..."> more... </a>
 <div id="label577" style="display:none">
 <table border="1">
 <tr>
 <td></td>
 <td colspan="1">Supported Version Ranges</td>
 </tr>
 <tr>
 <td>protocol</td>
 <td><code class="docutils literal notranslate">v7.4.2 -> v7.4.2 </code></td>
 </tr>
 </table>
 </div>
 </li>
                <li> <span class="li-head">slink</span> - tcam mask sublink. <span class="li-normal">type: int</span>
 <a id='label578' href="javascript:ContentClick('label579', 'label578');" onmouseover="ContentPreview('label579');" onmouseout="ContentUnpreview('label579');" title="click to collapse or expand..."> more... </a>
 <div id="label579" style="display:none">
 <table border="1">
 <tr>
 <td></td>
 <td colspan="1">Supported Version Ranges</td>
 </tr>
 <tr>
 <td>slink</td>
 <td><code class="docutils literal notranslate">v7.4.2 -> v7.4.2 </code></td>
 </tr>
 </table>
 </div>
 </li>
                <li> <span class="li-head">smac_change</span> - tcam mask source MAC change. <span class="li-normal">type: str</span> <span class="li-normal">choices: enable, disable</span>
 <a id='label580' href="javascript:ContentClick('label581', 'label580');" onmouseover="ContentPreview('label581');" onmouseout="ContentUnpreview('label581');" title="click to collapse or expand..."> more... </a>
 <div id="label581" style="display:none">
 <table border="1">
 <tr>
 <td></td>
 <td colspan="1">Supported Version Ranges</td>
 </tr>
 <tr>
 <td>smac_change</td>
 <td><code class="docutils literal notranslate">v7.4.2 -> v7.4.2 </code></td>
 </tr>
 <tr>
 <td>[enable]</td>
 <td><code class="docutils literal notranslate">v7.4.2 -> v7.4.2</code></td>
 <tr>
 <td>[disable]</td>
 <td><code class="docutils literal notranslate">v7.4.2 -> v7.4.2</code></td>
 </table>
 </div>
 </li>
                <li> <span class="li-head">sp</span> - tcam mask source port. <span class="li-normal">type: int</span>
 <a id='label582' href="javascript:ContentClick('label583', 'label582');" onmouseover="ContentPreview('label583');" onmouseout="ContentUnpreview('label583');" title="click to collapse or expand..."> more... </a>
 <div id="label583" style="display:none">
 <table border="1">
 <tr>
 <td></td>
 <td colspan="1">Supported Version Ranges</td>
 </tr>
 <tr>
 <td>sp</td>
 <td><code class="docutils literal notranslate">v7.4.2 -> v7.4.2 </code></td>
 </tr>
 </table>
 </div>
 </li>
                <li> <span class="li-head">src_cfi</span> - tcam mask source cfi. <span class="li-normal">type: str</span> <span class="li-normal">choices: enable, disable</span>
 <a id='label584' href="javascript:ContentClick('label585', 'label584');" onmouseover="ContentPreview('label585');" onmouseout="ContentUnpreview('label585');" title="click to collapse or expand..."> more... </a>
 <div id="label585" style="display:none">
 <table border="1">
 <tr>
 <td></td>
 <td colspan="1">Supported Version Ranges</td>
 </tr>
 <tr>
 <td>src_cfi</td>
 <td><code class="docutils literal notranslate">v7.4.2 -> v7.4.2 </code></td>
 </tr>
 <tr>
 <td>[enable]</td>
 <td><code class="docutils literal notranslate">v7.4.2 -> v7.4.2</code></td>
 <tr>
 <td>[disable]</td>
 <td><code class="docutils literal notranslate">v7.4.2 -> v7.4.2</code></td>
 </table>
 </div>
 </li>
                <li> <span class="li-head">src_prio</span> - tcam mask source priority. <span class="li-normal">type: int</span>
 <a id='label586' href="javascript:ContentClick('label587', 'label586');" onmouseover="ContentPreview('label587');" onmouseout="ContentUnpreview('label587');" title="click to collapse or expand..."> more... </a>
 <div id="label587" style="display:none">
 <table border="1">
 <tr>
 <td></td>
 <td colspan="1">Supported Version Ranges</td>
 </tr>
 <tr>
 <td>src_prio</td>
 <td><code class="docutils literal notranslate">v7.4.2 -> v7.4.2 </code></td>
 </tr>
 </table>
 </div>
 </li>
                <li> <span class="li-head">src_updt</span> - tcam mask source update. <span class="li-normal">type: str</span> <span class="li-normal">choices: enable, disable</span>
 <a id='label588' href="javascript:ContentClick('label589', 'label588');" onmouseover="ContentPreview('label589');" onmouseout="ContentUnpreview('label589');" title="click to collapse or expand..."> more... </a>
 <div id="label589" style="display:none">
 <table border="1">
 <tr>
 <td></td>
 <td colspan="1">Supported Version Ranges</td>
 </tr>
 <tr>
 <td>src_updt</td>
 <td><code class="docutils literal notranslate">v7.4.2 -> v7.4.2 </code></td>
 </tr>
 <tr>
 <td>[enable]</td>
 <td><code class="docutils literal notranslate">v7.4.2 -> v7.4.2</code></td>
 <tr>
 <td>[disable]</td>
 <td><code class="docutils literal notranslate">v7.4.2 -> v7.4.2</code></td>
 </table>
 </div>
 </li>
                <li> <span class="li-head">srcip</span> - tcam mask src ipv4 address. <span class="li-normal">type: str</span>
 <a id='label590' href="javascript:ContentClick('label591', 'label590');" onmouseover="ContentPreview('label591');" onmouseout="ContentUnpreview('label591');" title="click to collapse or expand..."> more... </a>
 <div id="label591" style="display:none">
 <table border="1">
 <tr>
 <td></td>
 <td colspan="1">Supported Version Ranges</td>
 </tr>
 <tr>
 <td>srcip</td>
 <td><code class="docutils literal notranslate">v7.4.2 -> v7.4.2 </code></td>
 </tr>
 </table>
 </div>
 </li>
                <li> <span class="li-head">srcipv6</span> - tcam mask src ipv6 address. <span class="li-normal">type: str</span>
 <a id='label592' href="javascript:ContentClick('label593', 'label592');" onmouseover="ContentPreview('label593');" onmouseout="ContentUnpreview('label593');" title="click to collapse or expand..."> more... </a>
 <div id="label593" style="display:none">
 <table border="1">
 <tr>
 <td></td>
 <td colspan="1">Supported Version Ranges</td>
 </tr>
 <tr>
 <td>srcipv6</td>
 <td><code class="docutils literal notranslate">v7.4.2 -> v7.4.2 </code></td>
 </tr>
 </table>
 </div>
 </li>
                <li> <span class="li-head">srcmac</span> - tcam mask src macaddr. <span class="li-normal">type: str</span>
 <a id='label594' href="javascript:ContentClick('label595', 'label594');" onmouseover="ContentPreview('label595');" onmouseout="ContentUnpreview('label595');" title="click to collapse or expand..."> more... </a>
 <div id="label595" style="display:none">
 <table border="1">
 <tr>
 <td></td>
 <td colspan="1">Supported Version Ranges</td>
 </tr>
 <tr>
 <td>srcmac</td>
 <td><code class="docutils literal notranslate">v7.4.2 -> v7.4.2 </code></td>
 </tr>
 </table>
 </div>
 </li>
                <li> <span class="li-head">srcport</span> - tcam mask L4 src port. <span class="li-normal">type: int</span>
 <a id='label596' href="javascript:ContentClick('label597', 'label596');" onmouseover="ContentPreview('label597');" onmouseout="ContentUnpreview('label597');" title="click to collapse or expand..."> more... </a>
 <div id="label597" style="display:none">
 <table border="1">
 <tr>
 <td></td>
 <td colspan="1">Supported Version Ranges</td>
 </tr>
 <tr>
 <td>srcport</td>
 <td><code class="docutils literal notranslate">v7.4.2 -> v7.4.2 </code></td>
 </tr>
 </table>
 </div>
 </li>
                <li> <span class="li-head">svid</span> - tcam mask source vid. <span class="li-normal">type: int</span>
 <a id='label598' href="javascript:ContentClick('label599', 'label598');" onmouseover="ContentPreview('label599');" onmouseout="ContentUnpreview('label599');" title="click to collapse or expand..."> more... </a>
 <div id="label599" style="display:none">
 <table border="1">
 <tr>
 <td></td>
 <td colspan="1">Supported Version Ranges</td>
 </tr>
 <tr>
 <td>svid</td>
 <td><code class="docutils literal notranslate">v7.4.2 -> v7.4.2 </code></td>
 </tr>
 </table>
 </div>
 </li>
                <li> <span class="li-head">tcp_ack</span> - tcam mask tcp flag ack. <span class="li-normal">type: str</span> <span class="li-normal">choices: enable, disable</span>
 <a id='label600' href="javascript:ContentClick('label601', 'label600');" onmouseover="ContentPreview('label601');" onmouseout="ContentUnpreview('label601');" title="click to collapse or expand..."> more... </a>
 <div id="label601" style="display:none">
 <table border="1">
 <tr>
 <td></td>
 <td colspan="1">Supported Version Ranges</td>
 </tr>
 <tr>
 <td>tcp_ack</td>
 <td><code class="docutils literal notranslate">v7.4.2 -> v7.4.2 </code></td>
 </tr>
 <tr>
 <td>[enable]</td>
 <td><code class="docutils literal notranslate">v7.4.2 -> v7.4.2</code></td>
 <tr>
 <td>[disable]</td>
 <td><code class="docutils literal notranslate">v7.4.2 -> v7.4.2</code></td>
 </table>
 </div>
 </li>
                <li> <span class="li-head">tcp_cwr</span> - tcam mask tcp flag cwr. <span class="li-normal">type: str</span> <span class="li-normal">choices: enable, disable</span>
 <a id='label602' href="javascript:ContentClick('label603', 'label602');" onmouseover="ContentPreview('label603');" onmouseout="ContentUnpreview('label603');" title="click to collapse or expand..."> more... </a>
 <div id="label603" style="display:none">
 <table border="1">
 <tr>
 <td></td>
 <td colspan="1">Supported Version Ranges</td>
 </tr>
 <tr>
 <td>tcp_cwr</td>
 <td><code class="docutils literal notranslate">v7.4.2 -> v7.4.2 </code></td>
 </tr>
 <tr>
 <td>[enable]</td>
 <td><code class="docutils literal notranslate">v7.4.2 -> v7.4.2</code></td>
 <tr>
 <td>[disable]</td>
 <td><code class="docutils literal notranslate">v7.4.2 -> v7.4.2</code></td>
 </table>
 </div>
 </li>
                <li> <span class="li-head">tcp_ece</span> - tcam mask tcp flag ece. <span class="li-normal">type: str</span> <span class="li-normal">choices: enable, disable</span>
 <a id='label604' href="javascript:ContentClick('label605', 'label604');" onmouseover="ContentPreview('label605');" onmouseout="ContentUnpreview('label605');" title="click to collapse or expand..."> more... </a>
 <div id="label605" style="display:none">
 <table border="1">
 <tr>
 <td></td>
 <td colspan="1">Supported Version Ranges</td>
 </tr>
 <tr>
 <td>tcp_ece</td>
 <td><code class="docutils literal notranslate">v7.4.2 -> v7.4.2 </code></td>
 </tr>
 <tr>
 <td>[enable]</td>
 <td><code class="docutils literal notranslate">v7.4.2 -> v7.4.2</code></td>
 <tr>
 <td>[disable]</td>
 <td><code class="docutils literal notranslate">v7.4.2 -> v7.4.2</code></td>
 </table>
 </div>
 </li>
                <li> <span class="li-head">tcp_fin</span> - tcam mask tcp flag fin. <span class="li-normal">type: str</span> <span class="li-normal">choices: enable, disable</span>
 <a id='label606' href="javascript:ContentClick('label607', 'label606');" onmouseover="ContentPreview('label607');" onmouseout="ContentUnpreview('label607');" title="click to collapse or expand..."> more... </a>
 <div id="label607" style="display:none">
 <table border="1">
 <tr>
 <td></td>
 <td colspan="1">Supported Version Ranges</td>
 </tr>
 <tr>
 <td>tcp_fin</td>
 <td><code class="docutils literal notranslate">v7.4.2 -> v7.4.2 </code></td>
 </tr>
 <tr>
 <td>[enable]</td>
 <td><code class="docutils literal notranslate">v7.4.2 -> v7.4.2</code></td>
 <tr>
 <td>[disable]</td>
 <td><code class="docutils literal notranslate">v7.4.2 -> v7.4.2</code></td>
 </table>
 </div>
 </li>
                <li> <span class="li-head">tcp_push</span> - tcam mask tcp flag push. <span class="li-normal">type: str</span> <span class="li-normal">choices: enable, disable</span>
 <a id='label608' href="javascript:ContentClick('label609', 'label608');" onmouseover="ContentPreview('label609');" onmouseout="ContentUnpreview('label609');" title="click to collapse or expand..."> more... </a>
 <div id="label609" style="display:none">
 <table border="1">
 <tr>
 <td></td>
 <td colspan="1">Supported Version Ranges</td>
 </tr>
 <tr>
 <td>tcp_push</td>
 <td><code class="docutils literal notranslate">v7.4.2 -> v7.4.2 </code></td>
 </tr>
 <tr>
 <td>[enable]</td>
 <td><code class="docutils literal notranslate">v7.4.2 -> v7.4.2</code></td>
 <tr>
 <td>[disable]</td>
 <td><code class="docutils literal notranslate">v7.4.2 -> v7.4.2</code></td>
 </table>
 </div>
 </li>
                <li> <span class="li-head">tcp_rst</span> - tcam mask tcp flag rst. <span class="li-normal">type: str</span> <span class="li-normal">choices: enable, disable</span>
 <a id='label610' href="javascript:ContentClick('label611', 'label610');" onmouseover="ContentPreview('label611');" onmouseout="ContentUnpreview('label611');" title="click to collapse or expand..."> more... </a>
 <div id="label611" style="display:none">
 <table border="1">
 <tr>
 <td></td>
 <td colspan="1">Supported Version Ranges</td>
 </tr>
 <tr>
 <td>tcp_rst</td>
 <td><code class="docutils literal notranslate">v7.4.2 -> v7.4.2 </code></td>
 </tr>
 <tr>
 <td>[enable]</td>
 <td><code class="docutils literal notranslate">v7.4.2 -> v7.4.2</code></td>
 <tr>
 <td>[disable]</td>
 <td><code class="docutils literal notranslate">v7.4.2 -> v7.4.2</code></td>
 </table>
 </div>
 </li>
                <li> <span class="li-head">tcp_syn</span> - tcam mask tcp flag syn. <span class="li-normal">type: str</span> <span class="li-normal">choices: enable, disable</span>
 <a id='label612' href="javascript:ContentClick('label613', 'label612');" onmouseover="ContentPreview('label613');" onmouseout="ContentUnpreview('label613');" title="click to collapse or expand..."> more... </a>
 <div id="label613" style="display:none">
 <table border="1">
 <tr>
 <td></td>
 <td colspan="1">Supported Version Ranges</td>
 </tr>
 <tr>
 <td>tcp_syn</td>
 <td><code class="docutils literal notranslate">v7.4.2 -> v7.4.2 </code></td>
 </tr>
 <tr>
 <td>[enable]</td>
 <td><code class="docutils literal notranslate">v7.4.2 -> v7.4.2</code></td>
 <tr>
 <td>[disable]</td>
 <td><code class="docutils literal notranslate">v7.4.2 -> v7.4.2</code></td>
 </table>
 </div>
 </li>
                <li> <span class="li-head">tcp_urg</span> - tcam mask tcp flag urg. <span class="li-normal">type: str</span> <span class="li-normal">choices: enable, disable</span>
 <a id='label614' href="javascript:ContentClick('label615', 'label614');" onmouseover="ContentPreview('label615');" onmouseout="ContentUnpreview('label615');" title="click to collapse or expand..."> more... </a>
 <div id="label615" style="display:none">
 <table border="1">
 <tr>
 <td></td>
 <td colspan="1">Supported Version Ranges</td>
 </tr>
 <tr>
 <td>tcp_urg</td>
 <td><code class="docutils literal notranslate">v7.4.2 -> v7.4.2 </code></td>
 </tr>
 <tr>
 <td>[enable]</td>
 <td><code class="docutils literal notranslate">v7.4.2 -> v7.4.2</code></td>
 <tr>
 <td>[disable]</td>
 <td><code class="docutils literal notranslate">v7.4.2 -> v7.4.2</code></td>
 </table>
 </div>
 </li>
                <li> <span class="li-head">tgt_cfi</span> - tcam mask target cfi. <span class="li-normal">type: str</span> <span class="li-normal">choices: enable, disable</span>
 <a id='label616' href="javascript:ContentClick('label617', 'label616');" onmouseover="ContentPreview('label617');" onmouseout="ContentUnpreview('label617');" title="click to collapse or expand..."> more... </a>
 <div id="label617" style="display:none">
 <table border="1">
 <tr>
 <td></td>
 <td colspan="1">Supported Version Ranges</td>
 </tr>
 <tr>
 <td>tgt_cfi</td>
 <td><code class="docutils literal notranslate">v7.4.2 -> v7.4.2 </code></td>
 </tr>
 <tr>
 <td>[enable]</td>
 <td><code class="docutils literal notranslate">v7.4.2 -> v7.4.2</code></td>
 <tr>
 <td>[disable]</td>
 <td><code class="docutils literal notranslate">v7.4.2 -> v7.4.2</code></td>
 </table>
 </div>
 </li>
                <li> <span class="li-head">tgt_prio</span> - tcam mask target priority. <span class="li-normal">type: int</span>
 <a id='label618' href="javascript:ContentClick('label619', 'label618');" onmouseover="ContentPreview('label619');" onmouseout="ContentUnpreview('label619');" title="click to collapse or expand..."> more... </a>
 <div id="label619" style="display:none">
 <table border="1">
 <tr>
 <td></td>
 <td colspan="1">Supported Version Ranges</td>
 </tr>
 <tr>
 <td>tgt_prio</td>
 <td><code class="docutils literal notranslate">v7.4.2 -> v7.4.2 </code></td>
 </tr>
 </table>
 </div>
 </li>
                <li> <span class="li-head">tgt_updt</span> - tcam mask target port update. <span class="li-normal">type: str</span> <span class="li-normal">choices: enable, disable</span>
 <a id='label620' href="javascript:ContentClick('label621', 'label620');" onmouseover="ContentPreview('label621');" onmouseout="ContentUnpreview('label621');" title="click to collapse or expand..."> more... </a>
 <div id="label621" style="display:none">
 <table border="1">
 <tr>
 <td></td>
 <td colspan="1">Supported Version Ranges</td>
 </tr>
 <tr>
 <td>tgt_updt</td>
 <td><code class="docutils literal notranslate">v7.4.2 -> v7.4.2 </code></td>
 </tr>
 <tr>
 <td>[enable]</td>
 <td><code class="docutils literal notranslate">v7.4.2 -> v7.4.2</code></td>
 <tr>
 <td>[disable]</td>
 <td><code class="docutils literal notranslate">v7.4.2 -> v7.4.2</code></td>
 </table>
 </div>
 </li>
                <li> <span class="li-head">tgt_v</span> - tcam mask target valid. <span class="li-normal">type: str</span> <span class="li-normal">choices: valid, invalid</span>
 <a id='label622' href="javascript:ContentClick('label623', 'label622');" onmouseover="ContentPreview('label623');" onmouseout="ContentUnpreview('label623');" title="click to collapse or expand..."> more... </a>
 <div id="label623" style="display:none">
 <table border="1">
 <tr>
 <td></td>
 <td colspan="1">Supported Version Ranges</td>
 </tr>
 <tr>
 <td>tgt_v</td>
 <td><code class="docutils literal notranslate">v7.4.2 -> v7.4.2 </code></td>
 </tr>
 <tr>
 <td>[valid]</td>
 <td><code class="docutils literal notranslate">v7.4.2 -> v7.4.2</code></td>
 <tr>
 <td>[invalid]</td>
 <td><code class="docutils literal notranslate">v7.4.2 -> v7.4.2</code></td>
 </table>
 </div>
 </li>
                <li> <span class="li-head">tos</span> - tcam mask ip tos. <span class="li-normal">type: int</span>
 <a id='label624' href="javascript:ContentClick('label625', 'label624');" onmouseover="ContentPreview('label625');" onmouseout="ContentUnpreview('label625');" title="click to collapse or expand..."> more... </a>
 <div id="label625" style="display:none">
 <table border="1">
 <tr>
 <td></td>
 <td colspan="1">Supported Version Ranges</td>
 </tr>
 <tr>
 <td>tos</td>
 <td><code class="docutils literal notranslate">v7.4.2 -> v7.4.2 </code></td>
 </tr>
 </table>
 </div>
 </li>
                <li> <span class="li-head">tp</span> - tcam mask target port. <span class="li-normal">type: int</span>
 <a id='label626' href="javascript:ContentClick('label627', 'label626');" onmouseover="ContentPreview('label627');" onmouseout="ContentUnpreview('label627');" title="click to collapse or expand..."> more... </a>
 <div id="label627" style="display:none">
 <table border="1">
 <tr>
 <td></td>
 <td colspan="1">Supported Version Ranges</td>
 </tr>
 <tr>
 <td>tp</td>
 <td><code class="docutils literal notranslate">v7.4.2 -> v7.4.2 </code></td>
 </tr>
 </table>
 </div>
 </li>
                <li> <span class="li-head">ttl</span> - tcam mask ip ttl. <span class="li-normal">type: int</span>
 <a id='label628' href="javascript:ContentClick('label629', 'label628');" onmouseover="ContentPreview('label629');" onmouseout="ContentUnpreview('label629');" title="click to collapse or expand..."> more... </a>
 <div id="label629" style="display:none">
 <table border="1">
 <tr>
 <td></td>
 <td colspan="1">Supported Version Ranges</td>
 </tr>
 <tr>
 <td>ttl</td>
 <td><code class="docutils literal notranslate">v7.4.2 -> v7.4.2 </code></td>
 </tr>
 </table>
 </div>
 </li>
                <li> <span class="li-head">tvid</span> - tcam mask target vid. <span class="li-normal">type: int</span>
 <a id='label630' href="javascript:ContentClick('label631', 'label630');" onmouseover="ContentPreview('label631');" onmouseout="ContentUnpreview('label631');" title="click to collapse or expand..."> more... </a>
 <div id="label631" style="display:none">
 <table border="1">
 <tr>
 <td></td>
 <td colspan="1">Supported Version Ranges</td>
 </tr>
 <tr>
 <td>tvid</td>
 <td><code class="docutils literal notranslate">v7.4.2 -> v7.4.2 </code></td>
 </tr>
 </table>
 </div>
 </li>
                <li> <span class="li-head">vdid</span> - tcam mask vdom id. <span class="li-normal">type: int</span>
 <a id='label632' href="javascript:ContentClick('label633', 'label632');" onmouseover="ContentPreview('label633');" onmouseout="ContentUnpreview('label633');" title="click to collapse or expand..."> more... </a>
 <div id="label633" style="display:none">
 <table border="1">
 <tr>
 <td></td>
 <td colspan="1">Supported Version Ranges</td>
 </tr>
 <tr>
 <td>vdid</td>
 <td><code class="docutils literal notranslate">v7.4.2 -> v7.4.2 </code></td>
 </tr>
 </table>
 </div>
 </li>
                </ul>
            <li> <span class="li-head">mir_act</span> - Mirror action of TCAM. <span class="li-normal">type: dict</span>
 <a id='label634' href="javascript:ContentClick('label635', 'label634');" onmouseover="ContentPreview('label635');" onmouseout="ContentUnpreview('label635');" title="click to collapse or expand..."> more... </a>
 <div id="label635" style="display:none">
 <table border="1">
 <tr>
 <td></td><td colspan="1">Supported Version Ranges</td>
 </tr>
 <tr>
 <td>mir_act</td>
 <td><code class="docutils literal notranslate">v7.4.2 -> v7.4.2 </code></td>
 </tr>
 </table>
 </div>
 </li>
                <ul class="ul-self">
                <li> <span class="li-head">vlif</span> - tcam mirror action vlif. <span class="li-normal">type: int</span>
 <a id='label636' href="javascript:ContentClick('label637', 'label636');" onmouseover="ContentPreview('label637');" onmouseout="ContentUnpreview('label637');" title="click to collapse or expand..."> more... </a>
 <div id="label637" style="display:none">
 <table border="1">
 <tr>
 <td></td>
 <td colspan="1">Supported Version Ranges</td>
 </tr>
 <tr>
 <td>vlif</td>
 <td><code class="docutils literal notranslate">v7.4.2 -> v7.4.2 </code></td>
 </tr>
 </table>
 </div>
 </li>
                </ul>
            <li> <span class="li-head">name</span> - NPU TCAM policies name. <span class="li-normal">type: str</span> <span class="li-required">required: true</span>
 <a id='label638' href="javascript:ContentClick('label639', 'label638');" onmouseover="ContentPreview('label639');" onmouseout="ContentUnpreview('label639');" title="click to collapse or expand..."> more... </a>
 <div id="label639" style="display:none">
 <table border="1">
 <tr>
 <td></td>
 <td colspan="1">Supported Version Ranges</td>
 </tr>
 <tr>
 <td>name</td>
 <td><code class="docutils literal notranslate">v7.4.2 -> v7.4.2 </code></td>
 </tr>
 </table>
 </div>
 </li>
            <li> <span class="li-head">oid</span> - NPU TCAM OID. <span class="li-normal">type: int</span>
 <a id='label640' href="javascript:ContentClick('label641', 'label640');" onmouseover="ContentPreview('label641');" onmouseout="ContentUnpreview('label641');" title="click to collapse or expand..."> more... </a>
 <div id="label641" style="display:none">
 <table border="1">
 <tr>
 <td></td>
 <td colspan="1">Supported Version Ranges</td>
 </tr>
 <tr>
 <td>oid</td>
 <td><code class="docutils literal notranslate">v7.4.2 -> v7.4.2 </code></td>
 </tr>
 </table>
 </div>
 </li>
            <li> <span class="li-head">pri_act</span> - Priority action of TCAM. <span class="li-normal">type: dict</span>
 <a id='label642' href="javascript:ContentClick('label643', 'label642');" onmouseover="ContentPreview('label643');" onmouseout="ContentUnpreview('label643');" title="click to collapse or expand..."> more... </a>
 <div id="label643" style="display:none">
 <table border="1">
 <tr>
 <td></td><td colspan="1">Supported Version Ranges</td>
 </tr>
 <tr>
 <td>pri_act</td>
 <td><code class="docutils literal notranslate">v7.4.2 -> v7.4.2 </code></td>
 </tr>
 </table>
 </div>
 </li>
                <ul class="ul-self">
                <li> <span class="li-head">priority</span> - tcam priority action priority. <span class="li-normal">type: int</span>
 <a id='label644' href="javascript:ContentClick('label645', 'label644');" onmouseover="ContentPreview('label645');" onmouseout="ContentUnpreview('label645');" title="click to collapse or expand..."> more... </a>
 <div id="label645" style="display:none">
 <table border="1">
 <tr>
 <td></td>
 <td colspan="1">Supported Version Ranges</td>
 </tr>
 <tr>
 <td>priority</td>
 <td><code class="docutils literal notranslate">v7.4.2 -> v7.4.2 </code></td>
 </tr>
 </table>
 </div>
 </li>
                <li> <span class="li-head">weight</span> - tcam priority action weight. <span class="li-normal">type: int</span>
 <a id='label646' href="javascript:ContentClick('label647', 'label646');" onmouseover="ContentPreview('label647');" onmouseout="ContentUnpreview('label647');" title="click to collapse or expand..."> more... </a>
 <div id="label647" style="display:none">
 <table border="1">
 <tr>
 <td></td>
 <td colspan="1">Supported Version Ranges</td>
 </tr>
 <tr>
 <td>weight</td>
 <td><code class="docutils literal notranslate">v7.4.2 -> v7.4.2 </code></td>
 </tr>
 </table>
 </div>
 </li>
                </ul>
            <li> <span class="li-head">sact</span> - Source action of TCAM. <span class="li-normal">type: dict</span>
 <a id='label648' href="javascript:ContentClick('label649', 'label648');" onmouseover="ContentPreview('label649');" onmouseout="ContentUnpreview('label649');" title="click to collapse or expand..."> more... </a>
 <div id="label649" style="display:none">
 <table border="1">
 <tr>
 <td></td><td colspan="1">Supported Version Ranges</td>
 </tr>
 <tr>
 <td>sact</td>
 <td><code class="docutils literal notranslate">v7.4.2 -> v7.4.2 </code></td>
 </tr>
 </table>
 </div>
 </li>
                <ul class="ul-self">
                <li> <span class="li-head">act</span> - tcam sact act. <span class="li-normal">type: int</span>
 <a id='label650' href="javascript:ContentClick('label651', 'label650');" onmouseover="ContentPreview('label651');" onmouseout="ContentUnpreview('label651');" title="click to collapse or expand..."> more... </a>
 <div id="label651" style="display:none">
 <table border="1">
 <tr>
 <td></td>
 <td colspan="1">Supported Version Ranges</td>
 </tr>
 <tr>
 <td>act</td>
 <td><code class="docutils literal notranslate">v7.4.2 -> v7.4.2 </code></td>
 </tr>
 </table>
 </div>
 </li>
                <li> <span class="li-head">act_v</span> - Enable to set sact act. <span class="li-normal">type: str</span> <span class="li-normal">choices: enable, disable</span>
 <a id='label652' href="javascript:ContentClick('label653', 'label652');" onmouseover="ContentPreview('label653');" onmouseout="ContentUnpreview('label653');" title="click to collapse or expand..."> more... </a>
 <div id="label653" style="display:none">
 <table border="1">
 <tr>
 <td></td>
 <td colspan="1">Supported Version Ranges</td>
 </tr>
 <tr>
 <td>act_v</td>
 <td><code class="docutils literal notranslate">v7.4.2 -> v7.4.2 </code></td>
 </tr>
 <tr>
 <td>[enable]</td>
 <td><code class="docutils literal notranslate">v7.4.2 -> v7.4.2</code></td>
 <tr>
 <td>[disable]</td>
 <td><code class="docutils literal notranslate">v7.4.2 -> v7.4.2</code></td>
 </table>
 </div>
 </li>
                <li> <span class="li-head">bmproc</span> - tcam sact bmproc. <span class="li-normal">type: int</span>
 <a id='label654' href="javascript:ContentClick('label655', 'label654');" onmouseover="ContentPreview('label655');" onmouseout="ContentUnpreview('label655');" title="click to collapse or expand..."> more... </a>
 <div id="label655" style="display:none">
 <table border="1">
 <tr>
 <td></td>
 <td colspan="1">Supported Version Ranges</td>
 </tr>
 <tr>
 <td>bmproc</td>
 <td><code class="docutils literal notranslate">v7.4.2 -> v7.4.2 </code></td>
 </tr>
 </table>
 </div>
 </li>
                <li> <span class="li-head">bmproc_v</span> - Enable to set sact bmproc. <span class="li-normal">type: str</span> <span class="li-normal">choices: enable, disable</span>
 <a id='label656' href="javascript:ContentClick('label657', 'label656');" onmouseover="ContentPreview('label657');" onmouseout="ContentUnpreview('label657');" title="click to collapse or expand..."> more... </a>
 <div id="label657" style="display:none">
 <table border="1">
 <tr>
 <td></td>
 <td colspan="1">Supported Version Ranges</td>
 </tr>
 <tr>
 <td>bmproc_v</td>
 <td><code class="docutils literal notranslate">v7.4.2 -> v7.4.2 </code></td>
 </tr>
 <tr>
 <td>[enable]</td>
 <td><code class="docutils literal notranslate">v7.4.2 -> v7.4.2</code></td>
 <tr>
 <td>[disable]</td>
 <td><code class="docutils literal notranslate">v7.4.2 -> v7.4.2</code></td>
 </table>
 </div>
 </li>
                <li> <span class="li-head">df_lif</span> - tcam sact df-lif. <span class="li-normal">type: int</span>
 <a id='label658' href="javascript:ContentClick('label659', 'label658');" onmouseover="ContentPreview('label659');" onmouseout="ContentUnpreview('label659');" title="click to collapse or expand..."> more... </a>
 <div id="label659" style="display:none">
 <table border="1">
 <tr>
 <td></td>
 <td colspan="1">Supported Version Ranges</td>
 </tr>
 <tr>
 <td>df_lif</td>
 <td><code class="docutils literal notranslate">v7.4.2 -> v7.4.2 </code></td>
 </tr>
 </table>
 </div>
 </li>
                <li> <span class="li-head">df_lif_v</span> - Enable to set sact df-lif. <span class="li-normal">type: str</span> <span class="li-normal">choices: enable, disable</span>
 <a id='label660' href="javascript:ContentClick('label661', 'label660');" onmouseover="ContentPreview('label661');" onmouseout="ContentUnpreview('label661');" title="click to collapse or expand..."> more... </a>
 <div id="label661" style="display:none">
 <table border="1">
 <tr>
 <td></td>
 <td colspan="1">Supported Version Ranges</td>
 </tr>
 <tr>
 <td>df_lif_v</td>
 <td><code class="docutils literal notranslate">v7.4.2 -> v7.4.2 </code></td>
 </tr>
 <tr>
 <td>[enable]</td>
 <td><code class="docutils literal notranslate">v7.4.2 -> v7.4.2</code></td>
 <tr>
 <td>[disable]</td>
 <td><code class="docutils literal notranslate">v7.4.2 -> v7.4.2</code></td>
 </table>
 </div>
 </li>
                <li> <span class="li-head">dfr</span> - tcam sact dfr. <span class="li-normal">type: int</span>
 <a id='label662' href="javascript:ContentClick('label663', 'label662');" onmouseover="ContentPreview('label663');" onmouseout="ContentUnpreview('label663');" title="click to collapse or expand..."> more... </a>
 <div id="label663" style="display:none">
 <table border="1">
 <tr>
 <td></td>
 <td colspan="1">Supported Version Ranges</td>
 </tr>
 <tr>
 <td>dfr</td>
 <td><code class="docutils literal notranslate">v7.4.2 -> v7.4.2 </code></td>
 </tr>
 </table>
 </div>
 </li>
                <li> <span class="li-head">dfr_v</span> - Enable to set sact dfr. <span class="li-normal">type: str</span> <span class="li-normal">choices: enable, disable</span>
 <a id='label664' href="javascript:ContentClick('label665', 'label664');" onmouseover="ContentPreview('label665');" onmouseout="ContentUnpreview('label665');" title="click to collapse or expand..."> more... </a>
 <div id="label665" style="display:none">
 <table border="1">
 <tr>
 <td></td>
 <td colspan="1">Supported Version Ranges</td>
 </tr>
 <tr>
 <td>dfr_v</td>
 <td><code class="docutils literal notranslate">v7.4.2 -> v7.4.2 </code></td>
 </tr>
 <tr>
 <td>[enable]</td>
 <td><code class="docutils literal notranslate">v7.4.2 -> v7.4.2</code></td>
 <tr>
 <td>[disable]</td>
 <td><code class="docutils literal notranslate">v7.4.2 -> v7.4.2</code></td>
 </table>
 </div>
 </li>
                <li> <span class="li-head">dmac_skip</span> - tcam sact dmac-skip. <span class="li-normal">type: int</span>
 <a id='label666' href="javascript:ContentClick('label667', 'label666');" onmouseover="ContentPreview('label667');" onmouseout="ContentUnpreview('label667');" title="click to collapse or expand..."> more... </a>
 <div id="label667" style="display:none">
 <table border="1">
 <tr>
 <td></td>
 <td colspan="1">Supported Version Ranges</td>
 </tr>
 <tr>
 <td>dmac_skip</td>
 <td><code class="docutils literal notranslate">v7.4.2 -> v7.4.2 </code></td>
 </tr>
 </table>
 </div>
 </li>
                <li> <span class="li-head">dmac_skip_v</span> - Enable to set sact dmac-skip. <span class="li-normal">type: str</span> <span class="li-normal">choices: enable, disable</span>
 <a id='label668' href="javascript:ContentClick('label669', 'label668');" onmouseover="ContentPreview('label669');" onmouseout="ContentUnpreview('label669');" title="click to collapse or expand..."> more... </a>
 <div id="label669" style="display:none">
 <table border="1">
 <tr>
 <td></td>
 <td colspan="1">Supported Version Ranges</td>
 </tr>
 <tr>
 <td>dmac_skip_v</td>
 <td><code class="docutils literal notranslate">v7.4.2 -> v7.4.2 </code></td>
 </tr>
 <tr>
 <td>[enable]</td>
 <td><code class="docutils literal notranslate">v7.4.2 -> v7.4.2</code></td>
 <tr>
 <td>[disable]</td>
 <td><code class="docutils literal notranslate">v7.4.2 -> v7.4.2</code></td>
 </table>
 </div>
 </li>
                <li> <span class="li-head">dosen</span> - tcam sact dosen. <span class="li-normal">type: int</span>
 <a id='label670' href="javascript:ContentClick('label671', 'label670');" onmouseover="ContentPreview('label671');" onmouseout="ContentUnpreview('label671');" title="click to collapse or expand..."> more... </a>
 <div id="label671" style="display:none">
 <table border="1">
 <tr>
 <td></td>
 <td colspan="1">Supported Version Ranges</td>
 </tr>
 <tr>
 <td>dosen</td>
 <td><code class="docutils literal notranslate">v7.4.2 -> v7.4.2 </code></td>
 </tr>
 </table>
 </div>
 </li>
                <li> <span class="li-head">dosen_v</span> - Enable to set sact dosen. <span class="li-normal">type: str</span> <span class="li-normal">choices: enable, disable</span>
 <a id='label672' href="javascript:ContentClick('label673', 'label672');" onmouseover="ContentPreview('label673');" onmouseout="ContentUnpreview('label673');" title="click to collapse or expand..."> more... </a>
 <div id="label673" style="display:none">
 <table border="1">
 <tr>
 <td></td>
 <td colspan="1">Supported Version Ranges</td>
 </tr>
 <tr>
 <td>dosen_v</td>
 <td><code class="docutils literal notranslate">v7.4.2 -> v7.4.2 </code></td>
 </tr>
 <tr>
 <td>[enable]</td>
 <td><code class="docutils literal notranslate">v7.4.2 -> v7.4.2</code></td>
 <tr>
 <td>[disable]</td>
 <td><code class="docutils literal notranslate">v7.4.2 -> v7.4.2</code></td>
 </table>
 </div>
 </li>
                <li> <span class="li-head">espff_proc</span> - tcam sact espff-proc. <span class="li-normal">type: int</span>
 <a id='label674' href="javascript:ContentClick('label675', 'label674');" onmouseover="ContentPreview('label675');" onmouseout="ContentUnpreview('label675');" title="click to collapse or expand..."> more... </a>
 <div id="label675" style="display:none">
 <table border="1">
 <tr>
 <td></td>
 <td colspan="1">Supported Version Ranges</td>
 </tr>
 <tr>
 <td>espff_proc</td>
 <td><code class="docutils literal notranslate">v7.4.2 -> v7.4.2 </code></td>
 </tr>
 </table>
 </div>
 </li>
                <li> <span class="li-head">espff_proc_v</span> - Enable to set sact espff-proc. <span class="li-normal">type: str</span> <span class="li-normal">choices: enable, disable</span>
 <a id='label676' href="javascript:ContentClick('label677', 'label676');" onmouseover="ContentPreview('label677');" onmouseout="ContentUnpreview('label677');" title="click to collapse or expand..."> more... </a>
 <div id="label677" style="display:none">
 <table border="1">
 <tr>
 <td></td>
 <td colspan="1">Supported Version Ranges</td>
 </tr>
 <tr>
 <td>espff_proc_v</td>
 <td><code class="docutils literal notranslate">v7.4.2 -> v7.4.2 </code></td>
 </tr>
 <tr>
 <td>[enable]</td>
 <td><code class="docutils literal notranslate">v7.4.2 -> v7.4.2</code></td>
 <tr>
 <td>[disable]</td>
 <td><code class="docutils literal notranslate">v7.4.2 -> v7.4.2</code></td>
 </table>
 </div>
 </li>
                <li> <span class="li-head">etype_pid</span> - tcam sact etype-pid. <span class="li-normal">type: int</span>
 <a id='label678' href="javascript:ContentClick('label679', 'label678');" onmouseover="ContentPreview('label679');" onmouseout="ContentUnpreview('label679');" title="click to collapse or expand..."> more... </a>
 <div id="label679" style="display:none">
 <table border="1">
 <tr>
 <td></td>
 <td colspan="1">Supported Version Ranges</td>
 </tr>
 <tr>
 <td>etype_pid</td>
 <td><code class="docutils literal notranslate">v7.4.2 -> v7.4.2 </code></td>
 </tr>
 </table>
 </div>
 </li>
                <li> <span class="li-head">etype_pid_v</span> - Enable to set sact etype-pid. <span class="li-normal">type: str</span> <span class="li-normal">choices: enable, disable</span>
 <a id='label680' href="javascript:ContentClick('label681', 'label680');" onmouseover="ContentPreview('label681');" onmouseout="ContentUnpreview('label681');" title="click to collapse or expand..."> more... </a>
 <div id="label681" style="display:none">
 <table border="1">
 <tr>
 <td></td>
 <td colspan="1">Supported Version Ranges</td>
 </tr>
 <tr>
 <td>etype_pid_v</td>
 <td><code class="docutils literal notranslate">v7.4.2 -> v7.4.2 </code></td>
 </tr>
 <tr>
 <td>[enable]</td>
 <td><code class="docutils literal notranslate">v7.4.2 -> v7.4.2</code></td>
 <tr>
 <td>[disable]</td>
 <td><code class="docutils literal notranslate">v7.4.2 -> v7.4.2</code></td>
 </table>
 </div>
 </li>
                <li> <span class="li-head">frag_proc</span> - tcam sact frag-proc. <span class="li-normal">type: int</span>
 <a id='label682' href="javascript:ContentClick('label683', 'label682');" onmouseover="ContentPreview('label683');" onmouseout="ContentUnpreview('label683');" title="click to collapse or expand..."> more... </a>
 <div id="label683" style="display:none">
 <table border="1">
 <tr>
 <td></td>
 <td colspan="1">Supported Version Ranges</td>
 </tr>
 <tr>
 <td>frag_proc</td>
 <td><code class="docutils literal notranslate">v7.4.2 -> v7.4.2 </code></td>
 </tr>
 </table>
 </div>
 </li>
                <li> <span class="li-head">frag_proc_v</span> - Enable to set sact frag-proc. <span class="li-normal">type: str</span> <span class="li-normal">choices: enable, disable</span>
 <a id='label684' href="javascript:ContentClick('label685', 'label684');" onmouseover="ContentPreview('label685');" onmouseout="ContentUnpreview('label685');" title="click to collapse or expand..."> more... </a>
 <div id="label685" style="display:none">
 <table border="1">
 <tr>
 <td></td>
 <td colspan="1">Supported Version Ranges</td>
 </tr>
 <tr>
 <td>frag_proc_v</td>
 <td><code class="docutils literal notranslate">v7.4.2 -> v7.4.2 </code></td>
 </tr>
 <tr>
 <td>[enable]</td>
 <td><code class="docutils literal notranslate">v7.4.2 -> v7.4.2</code></td>
 <tr>
 <td>[disable]</td>
 <td><code class="docutils literal notranslate">v7.4.2 -> v7.4.2</code></td>
 </table>
 </div>
 </li>
                <li> <span class="li-head">fwd</span> - tcam sact fwd. <span class="li-normal">type: int</span>
 <a id='label686' href="javascript:ContentClick('label687', 'label686');" onmouseover="ContentPreview('label687');" onmouseout="ContentUnpreview('label687');" title="click to collapse or expand..."> more... </a>
 <div id="label687" style="display:none">
 <table border="1">
 <tr>
 <td></td>
 <td colspan="1">Supported Version Ranges</td>
 </tr>
 <tr>
 <td>fwd</td>
 <td><code class="docutils literal notranslate">v7.4.2 -> v7.4.2 </code></td>
 </tr>
 </table>
 </div>
 </li>
                <li> <span class="li-head">fwd_lif</span> - tcam sact fwd-lif. <span class="li-normal">type: int</span>
 <a id='label688' href="javascript:ContentClick('label689', 'label688');" onmouseover="ContentPreview('label689');" onmouseout="ContentUnpreview('label689');" title="click to collapse or expand..."> more... </a>
 <div id="label689" style="display:none">
 <table border="1">
 <tr>
 <td></td>
 <td colspan="1">Supported Version Ranges</td>
 </tr>
 <tr>
 <td>fwd_lif</td>
 <td><code class="docutils literal notranslate">v7.4.2 -> v7.4.2 </code></td>
 </tr>
 </table>
 </div>
 </li>
                <li> <span class="li-head">fwd_lif_v</span> - Enable to set sact fwd-lif. <span class="li-normal">type: str</span> <span class="li-normal">choices: enable, disable</span>
 <a id='label690' href="javascript:ContentClick('label691', 'label690');" onmouseover="ContentPreview('label691');" onmouseout="ContentUnpreview('label691');" title="click to collapse or expand..."> more... </a>
 <div id="label691" style="display:none">
 <table border="1">
 <tr>
 <td></td>
 <td colspan="1">Supported Version Ranges</td>
 </tr>
 <tr>
 <td>fwd_lif_v</td>
 <td><code class="docutils literal notranslate">v7.4.2 -> v7.4.2 </code></td>
 </tr>
 <tr>
 <td>[enable]</td>
 <td><code class="docutils literal notranslate">v7.4.2 -> v7.4.2</code></td>
 <tr>
 <td>[disable]</td>
 <td><code class="docutils literal notranslate">v7.4.2 -> v7.4.2</code></td>
 </table>
 </div>
 </li>
                <li> <span class="li-head">fwd_tvid</span> - tcam sact fwd-tvid. <span class="li-normal">type: int</span>
 <a id='label692' href="javascript:ContentClick('label693', 'label692');" onmouseover="ContentPreview('label693');" onmouseout="ContentUnpreview('label693');" title="click to collapse or expand..."> more... </a>
 <div id="label693" style="display:none">
 <table border="1">
 <tr>
 <td></td>
 <td colspan="1">Supported Version Ranges</td>
 </tr>
 <tr>
 <td>fwd_tvid</td>
 <td><code class="docutils literal notranslate">v7.4.2 -> v7.4.2 </code></td>
 </tr>
 </table>
 </div>
 </li>
                <li> <span class="li-head">fwd_tvid_v</span> - Enable to set sact fwd-vid. <span class="li-normal">type: str</span> <span class="li-normal">choices: enable, disable</span>
 <a id='label694' href="javascript:ContentClick('label695', 'label694');" onmouseover="ContentPreview('label695');" onmouseout="ContentUnpreview('label695');" title="click to collapse or expand..."> more... </a>
 <div id="label695" style="display:none">
 <table border="1">
 <tr>
 <td></td>
 <td colspan="1">Supported Version Ranges</td>
 </tr>
 <tr>
 <td>fwd_tvid_v</td>
 <td><code class="docutils literal notranslate">v7.4.2 -> v7.4.2 </code></td>
 </tr>
 <tr>
 <td>[enable]</td>
 <td><code class="docutils literal notranslate">v7.4.2 -> v7.4.2</code></td>
 <tr>
 <td>[disable]</td>
 <td><code class="docutils literal notranslate">v7.4.2 -> v7.4.2</code></td>
 </table>
 </div>
 </li>
                <li> <span class="li-head">fwd_v</span> - Enable to set sact fwd. <span class="li-normal">type: str</span> <span class="li-normal">choices: enable, disable</span>
 <a id='label696' href="javascript:ContentClick('label697', 'label696');" onmouseover="ContentPreview('label697');" onmouseout="ContentUnpreview('label697');" title="click to collapse or expand..."> more... </a>
 <div id="label697" style="display:none">
 <table border="1">
 <tr>
 <td></td>
 <td colspan="1">Supported Version Ranges</td>
 </tr>
 <tr>
 <td>fwd_v</td>
 <td><code class="docutils literal notranslate">v7.4.2 -> v7.4.2 </code></td>
 </tr>
 <tr>
 <td>[enable]</td>
 <td><code class="docutils literal notranslate">v7.4.2 -> v7.4.2</code></td>
 <tr>
 <td>[disable]</td>
 <td><code class="docutils literal notranslate">v7.4.2 -> v7.4.2</code></td>
 </table>
 </div>
 </li>
                <li> <span class="li-head">icpen</span> - tcam sact icpen. <span class="li-normal">type: int</span>
 <a id='label698' href="javascript:ContentClick('label699', 'label698');" onmouseover="ContentPreview('label699');" onmouseout="ContentUnpreview('label699');" title="click to collapse or expand..."> more... </a>
 <div id="label699" style="display:none">
 <table border="1">
 <tr>
 <td></td>
 <td colspan="1">Supported Version Ranges</td>
 </tr>
 <tr>
 <td>icpen</td>
 <td><code class="docutils literal notranslate">v7.4.2 -> v7.4.2 </code></td>
 </tr>
 </table>
 </div>
 </li>
                <li> <span class="li-head">icpen_v</span> - Enable to set sact icpen. <span class="li-normal">type: str</span> <span class="li-normal">choices: enable, disable</span>
 <a id='label700' href="javascript:ContentClick('label701', 'label700');" onmouseover="ContentPreview('label701');" onmouseout="ContentUnpreview('label701');" title="click to collapse or expand..."> more... </a>
 <div id="label701" style="display:none">
 <table border="1">
 <tr>
 <td></td>
 <td colspan="1">Supported Version Ranges</td>
 </tr>
 <tr>
 <td>icpen_v</td>
 <td><code class="docutils literal notranslate">v7.4.2 -> v7.4.2 </code></td>
 </tr>
 <tr>
 <td>[enable]</td>
 <td><code class="docutils literal notranslate">v7.4.2 -> v7.4.2</code></td>
 <tr>
 <td>[disable]</td>
 <td><code class="docutils literal notranslate">v7.4.2 -> v7.4.2</code></td>
 </table>
 </div>
 </li>
                <li> <span class="li-head">igmp_mld_snp</span> - tcam sact igmp-mld-snp. <span class="li-normal">type: int</span>
 <a id='label702' href="javascript:ContentClick('label703', 'label702');" onmouseover="ContentPreview('label703');" onmouseout="ContentUnpreview('label703');" title="click to collapse or expand..."> more... </a>
 <div id="label703" style="display:none">
 <table border="1">
 <tr>
 <td></td>
 <td colspan="1">Supported Version Ranges</td>
 </tr>
 <tr>
 <td>igmp_mld_snp</td>
 <td><code class="docutils literal notranslate">v7.4.2 -> v7.4.2 </code></td>
 </tr>
 </table>
 </div>
 </li>
                <li> <span class="li-head">igmp_mld_snp_v</span> - Enable to set sact igmp-mld-snp. <span class="li-normal">type: str</span> <span class="li-normal">choices: enable, disable</span>
 <a id='label704' href="javascript:ContentClick('label705', 'label704');" onmouseover="ContentPreview('label705');" onmouseout="ContentUnpreview('label705');" title="click to collapse or expand..."> more... </a>
 <div id="label705" style="display:none">
 <table border="1">
 <tr>
 <td></td>
 <td colspan="1">Supported Version Ranges</td>
 </tr>
 <tr>
 <td>igmp_mld_snp_v</td>
 <td><code class="docutils literal notranslate">v7.4.2 -> v7.4.2 </code></td>
 </tr>
 <tr>
 <td>[enable]</td>
 <td><code class="docutils literal notranslate">v7.4.2 -> v7.4.2</code></td>
 <tr>
 <td>[disable]</td>
 <td><code class="docutils literal notranslate">v7.4.2 -> v7.4.2</code></td>
 </table>
 </div>
 </li>
                <li> <span class="li-head">learn</span> - tcam sact learn. <span class="li-normal">type: int</span>
 <a id='label706' href="javascript:ContentClick('label707', 'label706');" onmouseover="ContentPreview('label707');" onmouseout="ContentUnpreview('label707');" title="click to collapse or expand..."> more... </a>
 <div id="label707" style="display:none">
 <table border="1">
 <tr>
 <td></td>
 <td colspan="1">Supported Version Ranges</td>
 </tr>
 <tr>
 <td>learn</td>
 <td><code class="docutils literal notranslate">v7.4.2 -> v7.4.2 </code></td>
 </tr>
 </table>
 </div>
 </li>
                <li> <span class="li-head">learn_v</span> - Enable to set sact learn. <span class="li-normal">type: str</span> <span class="li-normal">choices: enable, disable</span>
 <a id='label708' href="javascript:ContentClick('label709', 'label708');" onmouseover="ContentPreview('label709');" onmouseout="ContentUnpreview('label709');" title="click to collapse or expand..."> more... </a>
 <div id="label709" style="display:none">
 <table border="1">
 <tr>
 <td></td>
 <td colspan="1">Supported Version Ranges</td>
 </tr>
 <tr>
 <td>learn_v</td>
 <td><code class="docutils literal notranslate">v7.4.2 -> v7.4.2 </code></td>
 </tr>
 <tr>
 <td>[enable]</td>
 <td><code class="docutils literal notranslate">v7.4.2 -> v7.4.2</code></td>
 <tr>
 <td>[disable]</td>
 <td><code class="docutils literal notranslate">v7.4.2 -> v7.4.2</code></td>
 </table>
 </div>
 </li>
                <li> <span class="li-head">m_srh_ctrl</span> - tcam sact m-srh-ctrl. <span class="li-normal">type: int</span>
 <a id='label710' href="javascript:ContentClick('label711', 'label710');" onmouseover="ContentPreview('label711');" onmouseout="ContentUnpreview('label711');" title="click to collapse or expand..."> more... </a>
 <div id="label711" style="display:none">
 <table border="1">
 <tr>
 <td></td>
 <td colspan="1">Supported Version Ranges</td>
 </tr>
 <tr>
 <td>m_srh_ctrl</td>
 <td><code class="docutils literal notranslate">v7.4.2 -> v7.4.2 </code></td>
 </tr>
 </table>
 </div>
 </li>
                <li> <span class="li-head">m_srh_ctrl_v</span> - Enable to set sact m-srh-ctrl. <span class="li-normal">type: str</span> <span class="li-normal">choices: enable, disable</span>
 <a id='label712' href="javascript:ContentClick('label713', 'label712');" onmouseover="ContentPreview('label713');" onmouseout="ContentUnpreview('label713');" title="click to collapse or expand..."> more... </a>
 <div id="label713" style="display:none">
 <table border="1">
 <tr>
 <td></td>
 <td colspan="1">Supported Version Ranges</td>
 </tr>
 <tr>
 <td>m_srh_ctrl_v</td>
 <td><code class="docutils literal notranslate">v7.4.2 -> v7.4.2 </code></td>
 </tr>
 <tr>
 <td>[enable]</td>
 <td><code class="docutils literal notranslate">v7.4.2 -> v7.4.2</code></td>
 <tr>
 <td>[disable]</td>
 <td><code class="docutils literal notranslate">v7.4.2 -> v7.4.2</code></td>
 </table>
 </div>
 </li>
                <li> <span class="li-head">mac_id</span> - tcam sact mac-id. <span class="li-normal">type: int</span>
 <a id='label714' href="javascript:ContentClick('label715', 'label714');" onmouseover="ContentPreview('label715');" onmouseout="ContentUnpreview('label715');" title="click to collapse or expand..."> more... </a>
 <div id="label715" style="display:none">
 <table border="1">
 <tr>
 <td></td>
 <td colspan="1">Supported Version Ranges</td>
 </tr>
 <tr>
 <td>mac_id</td>
 <td><code class="docutils literal notranslate">v7.4.2 -> v7.4.2 </code></td>
 </tr>
 </table>
 </div>
 </li>
                <li> <span class="li-head">mac_id_v</span> - Enable to set sact mac-id. <span class="li-normal">type: str</span> <span class="li-normal">choices: enable, disable</span>
 <a id='label716' href="javascript:ContentClick('label717', 'label716');" onmouseover="ContentPreview('label717');" onmouseout="ContentUnpreview('label717');" title="click to collapse or expand..."> more... </a>
 <div id="label717" style="display:none">
 <table border="1">
 <tr>
 <td></td>
 <td colspan="1">Supported Version Ranges</td>
 </tr>
 <tr>
 <td>mac_id_v</td>
 <td><code class="docutils literal notranslate">v7.4.2 -> v7.4.2 </code></td>
 </tr>
 <tr>
 <td>[enable]</td>
 <td><code class="docutils literal notranslate">v7.4.2 -> v7.4.2</code></td>
 <tr>
 <td>[disable]</td>
 <td><code class="docutils literal notranslate">v7.4.2 -> v7.4.2</code></td>
 </table>
 </div>
 </li>
                <li> <span class="li-head">mss</span> - tcam sact mss. <span class="li-normal">type: int</span>
 <a id='label718' href="javascript:ContentClick('label719', 'label718');" onmouseover="ContentPreview('label719');" onmouseout="ContentUnpreview('label719');" title="click to collapse or expand..."> more... </a>
 <div id="label719" style="display:none">
 <table border="1">
 <tr>
 <td></td>
 <td colspan="1">Supported Version Ranges</td>
 </tr>
 <tr>
 <td>mss</td>
 <td><code class="docutils literal notranslate">v7.4.2 -> v7.4.2 </code></td>
 </tr>
 </table>
 </div>
 </li>
                <li> <span class="li-head">mss_v</span> - Enable to set sact mss. <span class="li-normal">type: str</span> <span class="li-normal">choices: enable, disable</span>
 <a id='label720' href="javascript:ContentClick('label721', 'label720');" onmouseover="ContentPreview('label721');" onmouseout="ContentUnpreview('label721');" title="click to collapse or expand..."> more... </a>
 <div id="label721" style="display:none">
 <table border="1">
 <tr>
 <td></td>
 <td colspan="1">Supported Version Ranges</td>
 </tr>
 <tr>
 <td>mss_v</td>
 <td><code class="docutils literal notranslate">v7.4.2 -> v7.4.2 </code></td>
 </tr>
 <tr>
 <td>[enable]</td>
 <td><code class="docutils literal notranslate">v7.4.2 -> v7.4.2</code></td>
 <tr>
 <td>[disable]</td>
 <td><code class="docutils literal notranslate">v7.4.2 -> v7.4.2</code></td>
 </table>
 </div>
 </li>
                <li> <span class="li-head">pleen</span> - tcam sact pleen. <span class="li-normal">type: int</span>
 <a id='label722' href="javascript:ContentClick('label723', 'label722');" onmouseover="ContentPreview('label723');" onmouseout="ContentUnpreview('label723');" title="click to collapse or expand..."> more... </a>
 <div id="label723" style="display:none">
 <table border="1">
 <tr>
 <td></td>
 <td colspan="1">Supported Version Ranges</td>
 </tr>
 <tr>
 <td>pleen</td>
 <td><code class="docutils literal notranslate">v7.4.2 -> v7.4.2 </code></td>
 </tr>
 </table>
 </div>
 </li>
                <li> <span class="li-head">pleen_v</span> - Enable to set sact pleen. <span class="li-normal">type: str</span> <span class="li-normal">choices: enable, disable</span>
 <a id='label724' href="javascript:ContentClick('label725', 'label724');" onmouseover="ContentPreview('label725');" onmouseout="ContentUnpreview('label725');" title="click to collapse or expand..."> more... </a>
 <div id="label725" style="display:none">
 <table border="1">
 <tr>
 <td></td>
 <td colspan="1">Supported Version Ranges</td>
 </tr>
 <tr>
 <td>pleen_v</td>
 <td><code class="docutils literal notranslate">v7.4.2 -> v7.4.2 </code></td>
 </tr>
 <tr>
 <td>[enable]</td>
 <td><code class="docutils literal notranslate">v7.4.2 -> v7.4.2</code></td>
 <tr>
 <td>[disable]</td>
 <td><code class="docutils literal notranslate">v7.4.2 -> v7.4.2</code></td>
 </table>
 </div>
 </li>
                <li> <span class="li-head">prio_pid</span> - tcam sact prio-pid. <span class="li-normal">type: int</span>
 <a id='label726' href="javascript:ContentClick('label727', 'label726');" onmouseover="ContentPreview('label727');" onmouseout="ContentUnpreview('label727');" title="click to collapse or expand..."> more... </a>
 <div id="label727" style="display:none">
 <table border="1">
 <tr>
 <td></td>
 <td colspan="1">Supported Version Ranges</td>
 </tr>
 <tr>
 <td>prio_pid</td>
 <td><code class="docutils literal notranslate">v7.4.2 -> v7.4.2 </code></td>
 </tr>
 </table>
 </div>
 </li>
                <li> <span class="li-head">prio_pid_v</span> - Enable to set sact prio-pid. <span class="li-normal">type: str</span> <span class="li-normal">choices: enable, disable</span>
 <a id='label728' href="javascript:ContentClick('label729', 'label728');" onmouseover="ContentPreview('label729');" onmouseout="ContentUnpreview('label729');" title="click to collapse or expand..."> more... </a>
 <div id="label729" style="display:none">
 <table border="1">
 <tr>
 <td></td>
 <td colspan="1">Supported Version Ranges</td>
 </tr>
 <tr>
 <td>prio_pid_v</td>
 <td><code class="docutils literal notranslate">v7.4.2 -> v7.4.2 </code></td>
 </tr>
 <tr>
 <td>[enable]</td>
 <td><code class="docutils literal notranslate">v7.4.2 -> v7.4.2</code></td>
 <tr>
 <td>[disable]</td>
 <td><code class="docutils literal notranslate">v7.4.2 -> v7.4.2</code></td>
 </table>
 </div>
 </li>
                <li> <span class="li-head">promis</span> - tcam sact promis. <span class="li-normal">type: int</span>
 <a id='label730' href="javascript:ContentClick('label731', 'label730');" onmouseover="ContentPreview('label731');" onmouseout="ContentUnpreview('label731');" title="click to collapse or expand..."> more... </a>
 <div id="label731" style="display:none">
 <table border="1">
 <tr>
 <td></td>
 <td colspan="1">Supported Version Ranges</td>
 </tr>
 <tr>
 <td>promis</td>
 <td><code class="docutils literal notranslate">v7.4.2 -> v7.4.2 </code></td>
 </tr>
 </table>
 </div>
 </li>
                <li> <span class="li-head">promis_v</span> - Enable to set sact promis. <span class="li-normal">type: str</span> <span class="li-normal">choices: enable, disable</span>
 <a id='label732' href="javascript:ContentClick('label733', 'label732');" onmouseover="ContentPreview('label733');" onmouseout="ContentUnpreview('label733');" title="click to collapse or expand..."> more... </a>
 <div id="label733" style="display:none">
 <table border="1">
 <tr>
 <td></td>
 <td colspan="1">Supported Version Ranges</td>
 </tr>
 <tr>
 <td>promis_v</td>
 <td><code class="docutils literal notranslate">v7.4.2 -> v7.4.2 </code></td>
 </tr>
 <tr>
 <td>[enable]</td>
 <td><code class="docutils literal notranslate">v7.4.2 -> v7.4.2</code></td>
 <tr>
 <td>[disable]</td>
 <td><code class="docutils literal notranslate">v7.4.2 -> v7.4.2</code></td>
 </table>
 </div>
 </li>
                <li> <span class="li-head">rfsh</span> - tcam sact rfsh. <span class="li-normal">type: int</span>
 <a id='label734' href="javascript:ContentClick('label735', 'label734');" onmouseover="ContentPreview('label735');" onmouseout="ContentUnpreview('label735');" title="click to collapse or expand..."> more... </a>
 <div id="label735" style="display:none">
 <table border="1">
 <tr>
 <td></td>
 <td colspan="1">Supported Version Ranges</td>
 </tr>
 <tr>
 <td>rfsh</td>
 <td><code class="docutils literal notranslate">v7.4.2 -> v7.4.2 </code></td>
 </tr>
 </table>
 </div>
 </li>
                <li> <span class="li-head">rfsh_v</span> - Enable to set sact rfsh. <span class="li-normal">type: str</span> <span class="li-normal">choices: enable, disable</span>
 <a id='label736' href="javascript:ContentClick('label737', 'label736');" onmouseover="ContentPreview('label737');" onmouseout="ContentUnpreview('label737');" title="click to collapse or expand..."> more... </a>
 <div id="label737" style="display:none">
 <table border="1">
 <tr>
 <td></td>
 <td colspan="1">Supported Version Ranges</td>
 </tr>
 <tr>
 <td>rfsh_v</td>
 <td><code class="docutils literal notranslate">v7.4.2 -> v7.4.2 </code></td>
 </tr>
 <tr>
 <td>[enable]</td>
 <td><code class="docutils literal notranslate">v7.4.2 -> v7.4.2</code></td>
 <tr>
 <td>[disable]</td>
 <td><code class="docutils literal notranslate">v7.4.2 -> v7.4.2</code></td>
 </table>
 </div>
 </li>
                <li> <span class="li-head">smac_skip</span> - tcam sact smac-skip. <span class="li-normal">type: int</span>
 <a id='label738' href="javascript:ContentClick('label739', 'label738');" onmouseover="ContentPreview('label739');" onmouseout="ContentUnpreview('label739');" title="click to collapse or expand..."> more... </a>
 <div id="label739" style="display:none">
 <table border="1">
 <tr>
 <td></td>
 <td colspan="1">Supported Version Ranges</td>
 </tr>
 <tr>
 <td>smac_skip</td>
 <td><code class="docutils literal notranslate">v7.4.2 -> v7.4.2 </code></td>
 </tr>
 </table>
 </div>
 </li>
                <li> <span class="li-head">smac_skip_v</span> - Enable to set sact smac-skip. <span class="li-normal">type: str</span> <span class="li-normal">choices: enable, disable</span>
 <a id='label740' href="javascript:ContentClick('label741', 'label740');" onmouseover="ContentPreview('label741');" onmouseout="ContentUnpreview('label741');" title="click to collapse or expand..."> more... </a>
 <div id="label741" style="display:none">
 <table border="1">
 <tr>
 <td></td>
 <td colspan="1">Supported Version Ranges</td>
 </tr>
 <tr>
 <td>smac_skip_v</td>
 <td><code class="docutils literal notranslate">v7.4.2 -> v7.4.2 </code></td>
 </tr>
 <tr>
 <td>[enable]</td>
 <td><code class="docutils literal notranslate">v7.4.2 -> v7.4.2</code></td>
 <tr>
 <td>[disable]</td>
 <td><code class="docutils literal notranslate">v7.4.2 -> v7.4.2</code></td>
 </table>
 </div>
 </li>
                <li> <span class="li-head">tp_smchk</span> - tcam sact tp mode. <span class="li-normal">type: int</span>
 <a id='label742' href="javascript:ContentClick('label743', 'label742');" onmouseover="ContentPreview('label743');" onmouseout="ContentUnpreview('label743');" title="click to collapse or expand..."> more... </a>
 <div id="label743" style="display:none">
 <table border="1">
 <tr>
 <td></td>
 <td colspan="1">Supported Version Ranges</td>
 </tr>
 <tr>
 <td>tp_smchk</td>
 <td><code class="docutils literal notranslate">v7.4.2 -> v7.4.2 </code></td>
 </tr>
 </table>
 </div>
 </li>
                <li> <span class="li-head">tp_smchk_v</span> - Enable to set sact tp mode. <span class="li-normal">type: str</span> <span class="li-normal">choices: enable, disable</span>
 <a id='label744' href="javascript:ContentClick('label745', 'label744');" onmouseover="ContentPreview('label745');" onmouseout="ContentUnpreview('label745');" title="click to collapse or expand..."> more... </a>
 <div id="label745" style="display:none">
 <table border="1">
 <tr>
 <td></td>
 <td colspan="1">Supported Version Ranges</td>
 </tr>
 <tr>
 <td>tp_smchk_v</td>
 <td><code class="docutils literal notranslate">v7.4.2 -> v7.4.2 </code></td>
 </tr>
 <tr>
 <td>[enable]</td>
 <td><code class="docutils literal notranslate">v7.4.2 -> v7.4.2</code></td>
 <tr>
 <td>[disable]</td>
 <td><code class="docutils literal notranslate">v7.4.2 -> v7.4.2</code></td>
 </table>
 </div>
 </li>
                <li> <span class="li-head">tpe_id</span> - tcam sact tpe-id. <span class="li-normal">type: int</span>
 <a id='label746' href="javascript:ContentClick('label747', 'label746');" onmouseover="ContentPreview('label747');" onmouseout="ContentUnpreview('label747');" title="click to collapse or expand..."> more... </a>
 <div id="label747" style="display:none">
 <table border="1">
 <tr>
 <td></td>
 <td colspan="1">Supported Version Ranges</td>
 </tr>
 <tr>
 <td>tpe_id</td>
 <td><code class="docutils literal notranslate">v7.4.2 -> v7.4.2 </code></td>
 </tr>
 </table>
 </div>
 </li>
                <li> <span class="li-head">tpe_id_v</span> - Enable to set sact tpe-id. <span class="li-normal">type: str</span> <span class="li-normal">choices: enable, disable</span>
 <a id='label748' href="javascript:ContentClick('label749', 'label748');" onmouseover="ContentPreview('label749');" onmouseout="ContentUnpreview('label749');" title="click to collapse or expand..."> more... </a>
 <div id="label749" style="display:none">
 <table border="1">
 <tr>
 <td></td>
 <td colspan="1">Supported Version Ranges</td>
 </tr>
 <tr>
 <td>tpe_id_v</td>
 <td><code class="docutils literal notranslate">v7.4.2 -> v7.4.2 </code></td>
 </tr>
 <tr>
 <td>[enable]</td>
 <td><code class="docutils literal notranslate">v7.4.2 -> v7.4.2</code></td>
 <tr>
 <td>[disable]</td>
 <td><code class="docutils literal notranslate">v7.4.2 -> v7.4.2</code></td>
 </table>
 </div>
 </li>
                <li> <span class="li-head">vdm</span> - tcam sact vdm. <span class="li-normal">type: int</span>
 <a id='label750' href="javascript:ContentClick('label751', 'label750');" onmouseover="ContentPreview('label751');" onmouseout="ContentUnpreview('label751');" title="click to collapse or expand..."> more... </a>
 <div id="label751" style="display:none">
 <table border="1">
 <tr>
 <td></td>
 <td colspan="1">Supported Version Ranges</td>
 </tr>
 <tr>
 <td>vdm</td>
 <td><code class="docutils literal notranslate">v7.4.2 -> v7.4.2 </code></td>
 </tr>
 </table>
 </div>
 </li>
                <li> <span class="li-head">vdm_v</span> - Enable to set sact vdm. <span class="li-normal">type: str</span> <span class="li-normal">choices: enable, disable</span>
 <a id='label752' href="javascript:ContentClick('label753', 'label752');" onmouseover="ContentPreview('label753');" onmouseout="ContentUnpreview('label753');" title="click to collapse or expand..."> more... </a>
 <div id="label753" style="display:none">
 <table border="1">
 <tr>
 <td></td>
 <td colspan="1">Supported Version Ranges</td>
 </tr>
 <tr>
 <td>vdm_v</td>
 <td><code class="docutils literal notranslate">v7.4.2 -> v7.4.2 </code></td>
 </tr>
 <tr>
 <td>[enable]</td>
 <td><code class="docutils literal notranslate">v7.4.2 -> v7.4.2</code></td>
 <tr>
 <td>[disable]</td>
 <td><code class="docutils literal notranslate">v7.4.2 -> v7.4.2</code></td>
 </table>
 </div>
 </li>
                <li> <span class="li-head">vdom_id</span> - tcam sact vdom-id. <span class="li-normal">type: int</span>
 <a id='label754' href="javascript:ContentClick('label755', 'label754');" onmouseover="ContentPreview('label755');" onmouseout="ContentUnpreview('label755');" title="click to collapse or expand..."> more... </a>
 <div id="label755" style="display:none">
 <table border="1">
 <tr>
 <td></td>
 <td colspan="1">Supported Version Ranges</td>
 </tr>
 <tr>
 <td>vdom_id</td>
 <td><code class="docutils literal notranslate">v7.4.2 -> v7.4.2 </code></td>
 </tr>
 </table>
 </div>
 </li>
                <li> <span class="li-head">vdom_id_v</span> - Enable to set sact vdom-id. <span class="li-normal">type: str</span> <span class="li-normal">choices: enable, disable</span>
 <a id='label756' href="javascript:ContentClick('label757', 'label756');" onmouseover="ContentPreview('label757');" onmouseout="ContentUnpreview('label757');" title="click to collapse or expand..."> more... </a>
 <div id="label757" style="display:none">
 <table border="1">
 <tr>
 <td></td>
 <td colspan="1">Supported Version Ranges</td>
 </tr>
 <tr>
 <td>vdom_id_v</td>
 <td><code class="docutils literal notranslate">v7.4.2 -> v7.4.2 </code></td>
 </tr>
 <tr>
 <td>[enable]</td>
 <td><code class="docutils literal notranslate">v7.4.2 -> v7.4.2</code></td>
 <tr>
 <td>[disable]</td>
 <td><code class="docutils literal notranslate">v7.4.2 -> v7.4.2</code></td>
 </table>
 </div>
 </li>
                <li> <span class="li-head">x_mode</span> - tcam sact x-mode. <span class="li-normal">type: int</span>
 <a id='label758' href="javascript:ContentClick('label759', 'label758');" onmouseover="ContentPreview('label759');" onmouseout="ContentUnpreview('label759');" title="click to collapse or expand..."> more... </a>
 <div id="label759" style="display:none">
 <table border="1">
 <tr>
 <td></td>
 <td colspan="1">Supported Version Ranges</td>
 </tr>
 <tr>
 <td>x_mode</td>
 <td><code class="docutils literal notranslate">v7.4.2 -> v7.4.2 </code></td>
 </tr>
 </table>
 </div>
 </li>
                <li> <span class="li-head">x_mode_v</span> - Enable to set sact x-mode. <span class="li-normal">type: str</span> <span class="li-normal">choices: enable, disable</span>
 <a id='label760' href="javascript:ContentClick('label761', 'label760');" onmouseover="ContentPreview('label761');" onmouseout="ContentUnpreview('label761');" title="click to collapse or expand..."> more... </a>
 <div id="label761" style="display:none">
 <table border="1">
 <tr>
 <td></td>
 <td colspan="1">Supported Version Ranges</td>
 </tr>
 <tr>
 <td>x_mode_v</td>
 <td><code class="docutils literal notranslate">v7.4.2 -> v7.4.2 </code></td>
 </tr>
 <tr>
 <td>[enable]</td>
 <td><code class="docutils literal notranslate">v7.4.2 -> v7.4.2</code></td>
 <tr>
 <td>[disable]</td>
 <td><code class="docutils literal notranslate">v7.4.2 -> v7.4.2</code></td>
 </table>
 </div>
 </li>
                </ul>
            <li> <span class="li-head">tact</span> - Target action of TCAM. <span class="li-normal">type: dict</span>
 <a id='label762' href="javascript:ContentClick('label763', 'label762');" onmouseover="ContentPreview('label763');" onmouseout="ContentUnpreview('label763');" title="click to collapse or expand..."> more... </a>
 <div id="label763" style="display:none">
 <table border="1">
 <tr>
 <td></td><td colspan="1">Supported Version Ranges</td>
 </tr>
 <tr>
 <td>tact</td>
 <td><code class="docutils literal notranslate">v7.4.2 -> v7.4.2 </code></td>
 </tr>
 </table>
 </div>
 </li>
                <ul class="ul-self">
                <li> <span class="li-head">act</span> - tcam tact act. <span class="li-normal">type: int</span>
 <a id='label764' href="javascript:ContentClick('label765', 'label764');" onmouseover="ContentPreview('label765');" onmouseout="ContentUnpreview('label765');" title="click to collapse or expand..."> more... </a>
 <div id="label765" style="display:none">
 <table border="1">
 <tr>
 <td></td>
 <td colspan="1">Supported Version Ranges</td>
 </tr>
 <tr>
 <td>act</td>
 <td><code class="docutils literal notranslate">v7.4.2 -> v7.4.2 </code></td>
 </tr>
 </table>
 </div>
 </li>
                <li> <span class="li-head">act_v</span> - Enable to set tact act. <span class="li-normal">type: str</span> <span class="li-normal">choices: enable, disable</span>
 <a id='label766' href="javascript:ContentClick('label767', 'label766');" onmouseover="ContentPreview('label767');" onmouseout="ContentUnpreview('label767');" title="click to collapse or expand..."> more... </a>
 <div id="label767" style="display:none">
 <table border="1">
 <tr>
 <td></td>
 <td colspan="1">Supported Version Ranges</td>
 </tr>
 <tr>
 <td>act_v</td>
 <td><code class="docutils literal notranslate">v7.4.2 -> v7.4.2 </code></td>
 </tr>
 <tr>
 <td>[enable]</td>
 <td><code class="docutils literal notranslate">v7.4.2 -> v7.4.2</code></td>
 <tr>
 <td>[disable]</td>
 <td><code class="docutils literal notranslate">v7.4.2 -> v7.4.2</code></td>
 </table>
 </div>
 </li>
                <li> <span class="li-head">fmtuv4_s</span> - tcam tact fmtuv4-s. <span class="li-normal">type: int</span>
 <a id='label768' href="javascript:ContentClick('label769', 'label768');" onmouseover="ContentPreview('label769');" onmouseout="ContentUnpreview('label769');" title="click to collapse or expand..."> more... </a>
 <div id="label769" style="display:none">
 <table border="1">
 <tr>
 <td></td>
 <td colspan="1">Supported Version Ranges</td>
 </tr>
 <tr>
 <td>fmtuv4_s</td>
 <td><code class="docutils literal notranslate">v7.4.2 -> v7.4.2 </code></td>
 </tr>
 </table>
 </div>
 </li>
                <li> <span class="li-head">fmtuv4_s_v</span> - Enable to set tact fmtuv4-s. <span class="li-normal">type: str</span> <span class="li-normal">choices: enable, disable</span>
 <a id='label770' href="javascript:ContentClick('label771', 'label770');" onmouseover="ContentPreview('label771');" onmouseout="ContentUnpreview('label771');" title="click to collapse or expand..."> more... </a>
 <div id="label771" style="display:none">
 <table border="1">
 <tr>
 <td></td>
 <td colspan="1">Supported Version Ranges</td>
 </tr>
 <tr>
 <td>fmtuv4_s_v</td>
 <td><code class="docutils literal notranslate">v7.4.2 -> v7.4.2 </code></td>
 </tr>
 <tr>
 <td>[enable]</td>
 <td><code class="docutils literal notranslate">v7.4.2 -> v7.4.2</code></td>
 <tr>
 <td>[disable]</td>
 <td><code class="docutils literal notranslate">v7.4.2 -> v7.4.2</code></td>
 </table>
 </div>
 </li>
                <li> <span class="li-head">fmtuv6_s</span> - tcam tact fmtuv6-s. <span class="li-normal">type: int</span>
 <a id='label772' href="javascript:ContentClick('label773', 'label772');" onmouseover="ContentPreview('label773');" onmouseout="ContentUnpreview('label773');" title="click to collapse or expand..."> more... </a>
 <div id="label773" style="display:none">
 <table border="1">
 <tr>
 <td></td>
 <td colspan="1">Supported Version Ranges</td>
 </tr>
 <tr>
 <td>fmtuv6_s</td>
 <td><code class="docutils literal notranslate">v7.4.2 -> v7.4.2 </code></td>
 </tr>
 </table>
 </div>
 </li>
                <li> <span class="li-head">fmtuv6_s_v</span> - Enable to set tact fmtuv6-s. <span class="li-normal">type: str</span> <span class="li-normal">choices: enable, disable</span>
 <a id='label774' href="javascript:ContentClick('label775', 'label774');" onmouseover="ContentPreview('label775');" onmouseout="ContentUnpreview('label775');" title="click to collapse or expand..."> more... </a>
 <div id="label775" style="display:none">
 <table border="1">
 <tr>
 <td></td>
 <td colspan="1">Supported Version Ranges</td>
 </tr>
 <tr>
 <td>fmtuv6_s_v</td>
 <td><code class="docutils literal notranslate">v7.4.2 -> v7.4.2 </code></td>
 </tr>
 <tr>
 <td>[enable]</td>
 <td><code class="docutils literal notranslate">v7.4.2 -> v7.4.2</code></td>
 <tr>
 <td>[disable]</td>
 <td><code class="docutils literal notranslate">v7.4.2 -> v7.4.2</code></td>
 </table>
 </div>
 </li>
                <li> <span class="li-head">lnkid</span> - tcam tact lnkid. <span class="li-normal">type: int</span>
 <a id='label776' href="javascript:ContentClick('label777', 'label776');" onmouseover="ContentPreview('label777');" onmouseout="ContentUnpreview('label777');" title="click to collapse or expand..."> more... </a>
 <div id="label777" style="display:none">
 <table border="1">
 <tr>
 <td></td>
 <td colspan="1">Supported Version Ranges</td>
 </tr>
 <tr>
 <td>lnkid</td>
 <td><code class="docutils literal notranslate">v7.4.2 -> v7.4.2 </code></td>
 </tr>
 </table>
 </div>
 </li>
                <li> <span class="li-head">lnkid_v</span> - Enable to set tact lnkid. <span class="li-normal">type: str</span> <span class="li-normal">choices: enable, disable</span>
 <a id='label778' href="javascript:ContentClick('label779', 'label778');" onmouseover="ContentPreview('label779');" onmouseout="ContentUnpreview('label779');" title="click to collapse or expand..."> more... </a>
 <div id="label779" style="display:none">
 <table border="1">
 <tr>
 <td></td>
 <td colspan="1">Supported Version Ranges</td>
 </tr>
 <tr>
 <td>lnkid_v</td>
 <td><code class="docutils literal notranslate">v7.4.2 -> v7.4.2 </code></td>
 </tr>
 <tr>
 <td>[enable]</td>
 <td><code class="docutils literal notranslate">v7.4.2 -> v7.4.2</code></td>
 <tr>
 <td>[disable]</td>
 <td><code class="docutils literal notranslate">v7.4.2 -> v7.4.2</code></td>
 </table>
 </div>
 </li>
                <li> <span class="li-head">mac_id</span> - tcam tact mac-id. <span class="li-normal">type: int</span>
 <a id='label780' href="javascript:ContentClick('label781', 'label780');" onmouseover="ContentPreview('label781');" onmouseout="ContentUnpreview('label781');" title="click to collapse or expand..."> more... </a>
 <div id="label781" style="display:none">
 <table border="1">
 <tr>
 <td></td>
 <td colspan="1">Supported Version Ranges</td>
 </tr>
 <tr>
 <td>mac_id</td>
 <td><code class="docutils literal notranslate">v7.4.2 -> v7.4.2 </code></td>
 </tr>
 </table>
 </div>
 </li>
                <li> <span class="li-head">mac_id_v</span> - Enable to set tact mac-id. <span class="li-normal">type: str</span> <span class="li-normal">choices: enable, disable</span>
 <a id='label782' href="javascript:ContentClick('label783', 'label782');" onmouseover="ContentPreview('label783');" onmouseout="ContentUnpreview('label783');" title="click to collapse or expand..."> more... </a>
 <div id="label783" style="display:none">
 <table border="1">
 <tr>
 <td></td>
 <td colspan="1">Supported Version Ranges</td>
 </tr>
 <tr>
 <td>mac_id_v</td>
 <td><code class="docutils literal notranslate">v7.4.2 -> v7.4.2 </code></td>
 </tr>
 <tr>
 <td>[enable]</td>
 <td><code class="docutils literal notranslate">v7.4.2 -> v7.4.2</code></td>
 <tr>
 <td>[disable]</td>
 <td><code class="docutils literal notranslate">v7.4.2 -> v7.4.2</code></td>
 </table>
 </div>
 </li>
                <li> <span class="li-head">mss_t</span> - tcam tact mss. <span class="li-normal">type: int</span>
 <a id='label784' href="javascript:ContentClick('label785', 'label784');" onmouseover="ContentPreview('label785');" onmouseout="ContentUnpreview('label785');" title="click to collapse or expand..."> more... </a>
 <div id="label785" style="display:none">
 <table border="1">
 <tr>
 <td></td>
 <td colspan="1">Supported Version Ranges</td>
 </tr>
 <tr>
 <td>mss_t</td>
 <td><code class="docutils literal notranslate">v7.4.2 -> v7.4.2 </code></td>
 </tr>
 </table>
 </div>
 </li>
                <li> <span class="li-head">mss_t_v</span> - Enable to set tact mss. <span class="li-normal">type: str</span> <span class="li-normal">choices: enable, disable</span>
 <a id='label786' href="javascript:ContentClick('label787', 'label786');" onmouseover="ContentPreview('label787');" onmouseout="ContentUnpreview('label787');" title="click to collapse or expand..."> more... </a>
 <div id="label787" style="display:none">
 <table border="1">
 <tr>
 <td></td>
 <td colspan="1">Supported Version Ranges</td>
 </tr>
 <tr>
 <td>mss_t_v</td>
 <td><code class="docutils literal notranslate">v7.4.2 -> v7.4.2 </code></td>
 </tr>
 <tr>
 <td>[enable]</td>
 <td><code class="docutils literal notranslate">v7.4.2 -> v7.4.2</code></td>
 <tr>
 <td>[disable]</td>
 <td><code class="docutils literal notranslate">v7.4.2 -> v7.4.2</code></td>
 </table>
 </div>
 </li>
                <li> <span class="li-head">mtuv4</span> - tcam tact mtuv4. <span class="li-normal">type: int</span>
 <a id='label788' href="javascript:ContentClick('label789', 'label788');" onmouseover="ContentPreview('label789');" onmouseout="ContentUnpreview('label789');" title="click to collapse or expand..."> more... </a>
 <div id="label789" style="display:none">
 <table border="1">
 <tr>
 <td></td>
 <td colspan="1">Supported Version Ranges</td>
 </tr>
 <tr>
 <td>mtuv4</td>
 <td><code class="docutils literal notranslate">v7.4.2 -> v7.4.2 </code></td>
 </tr>
 </table>
 </div>
 </li>
                <li> <span class="li-head">mtuv4_v</span> - Enable to set tact mtuv4. <span class="li-normal">type: str</span> <span class="li-normal">choices: enable, disable</span>
 <a id='label790' href="javascript:ContentClick('label791', 'label790');" onmouseover="ContentPreview('label791');" onmouseout="ContentUnpreview('label791');" title="click to collapse or expand..."> more... </a>
 <div id="label791" style="display:none">
 <table border="1">
 <tr>
 <td></td>
 <td colspan="1">Supported Version Ranges</td>
 </tr>
 <tr>
 <td>mtuv4_v</td>
 <td><code class="docutils literal notranslate">v7.4.2 -> v7.4.2 </code></td>
 </tr>
 <tr>
 <td>[enable]</td>
 <td><code class="docutils literal notranslate">v7.4.2 -> v7.4.2</code></td>
 <tr>
 <td>[disable]</td>
 <td><code class="docutils literal notranslate">v7.4.2 -> v7.4.2</code></td>
 </table>
 </div>
 </li>
                <li> <span class="li-head">mtuv6</span> - tcam tact mtuv6. <span class="li-normal">type: int</span>
 <a id='label792' href="javascript:ContentClick('label793', 'label792');" onmouseover="ContentPreview('label793');" onmouseout="ContentUnpreview('label793');" title="click to collapse or expand..."> more... </a>
 <div id="label793" style="display:none">
 <table border="1">
 <tr>
 <td></td>
 <td colspan="1">Supported Version Ranges</td>
 </tr>
 <tr>
 <td>mtuv6</td>
 <td><code class="docutils literal notranslate">v7.4.2 -> v7.4.2 </code></td>
 </tr>
 </table>
 </div>
 </li>
                <li> <span class="li-head">mtuv6_v</span> - Enable to set tact mtuv6. <span class="li-normal">type: str</span> <span class="li-normal">choices: enable, disable</span>
 <a id='label794' href="javascript:ContentClick('label795', 'label794');" onmouseover="ContentPreview('label795');" onmouseout="ContentUnpreview('label795');" title="click to collapse or expand..."> more... </a>
 <div id="label795" style="display:none">
 <table border="1">
 <tr>
 <td></td>
 <td colspan="1">Supported Version Ranges</td>
 </tr>
 <tr>
 <td>mtuv6_v</td>
 <td><code class="docutils literal notranslate">v7.4.2 -> v7.4.2 </code></td>
 </tr>
 <tr>
 <td>[enable]</td>
 <td><code class="docutils literal notranslate">v7.4.2 -> v7.4.2</code></td>
 <tr>
 <td>[disable]</td>
 <td><code class="docutils literal notranslate">v7.4.2 -> v7.4.2</code></td>
 </table>
 </div>
 </li>
                <li> <span class="li-head">slif_act</span> - tcam tact slif-act. <span class="li-normal">type: int</span>
 <a id='label796' href="javascript:ContentClick('label797', 'label796');" onmouseover="ContentPreview('label797');" onmouseout="ContentUnpreview('label797');" title="click to collapse or expand..."> more... </a>
 <div id="label797" style="display:none">
 <table border="1">
 <tr>
 <td></td>
 <td colspan="1">Supported Version Ranges</td>
 </tr>
 <tr>
 <td>slif_act</td>
 <td><code class="docutils literal notranslate">v7.4.2 -> v7.4.2 </code></td>
 </tr>
 </table>
 </div>
 </li>
                <li> <span class="li-head">slif_act_v</span> - Enable to set tact slif-act. <span class="li-normal">type: str</span> <span class="li-normal">choices: enable, disable</span>
 <a id='label798' href="javascript:ContentClick('label799', 'label798');" onmouseover="ContentPreview('label799');" onmouseout="ContentUnpreview('label799');" title="click to collapse or expand..."> more... </a>
 <div id="label799" style="display:none">
 <table border="1">
 <tr>
 <td></td>
 <td colspan="1">Supported Version Ranges</td>
 </tr>
 <tr>
 <td>slif_act_v</td>
 <td><code class="docutils literal notranslate">v7.4.2 -> v7.4.2 </code></td>
 </tr>
 <tr>
 <td>[enable]</td>
 <td><code class="docutils literal notranslate">v7.4.2 -> v7.4.2</code></td>
 <tr>
 <td>[disable]</td>
 <td><code class="docutils literal notranslate">v7.4.2 -> v7.4.2</code></td>
 </table>
 </div>
 </li>
                <li> <span class="li-head">sublnkid</span> - tcam tact sublnkid. <span class="li-normal">type: int</span>
 <a id='label800' href="javascript:ContentClick('label801', 'label800');" onmouseover="ContentPreview('label801');" onmouseout="ContentUnpreview('label801');" title="click to collapse or expand..."> more... </a>
 <div id="label801" style="display:none">
 <table border="1">
 <tr>
 <td></td>
 <td colspan="1">Supported Version Ranges</td>
 </tr>
 <tr>
 <td>sublnkid</td>
 <td><code class="docutils literal notranslate">v7.4.2 -> v7.4.2 </code></td>
 </tr>
 </table>
 </div>
 </li>
                <li> <span class="li-head">sublnkid_v</span> - Enable to set tact sublnkid. <span class="li-normal">type: str</span> <span class="li-normal">choices: enable, disable</span>
 <a id='label802' href="javascript:ContentClick('label803', 'label802');" onmouseover="ContentPreview('label803');" onmouseout="ContentUnpreview('label803');" title="click to collapse or expand..."> more... </a>
 <div id="label803" style="display:none">
 <table border="1">
 <tr>
 <td></td>
 <td colspan="1">Supported Version Ranges</td>
 </tr>
 <tr>
 <td>sublnkid_v</td>
 <td><code class="docutils literal notranslate">v7.4.2 -> v7.4.2 </code></td>
 </tr>
 <tr>
 <td>[enable]</td>
 <td><code class="docutils literal notranslate">v7.4.2 -> v7.4.2</code></td>
 <tr>
 <td>[disable]</td>
 <td><code class="docutils literal notranslate">v7.4.2 -> v7.4.2</code></td>
 </table>
 </div>
 </li>
                <li> <span class="li-head">tgtv_act</span> - tcam tact tgtv-act. <span class="li-normal">type: int</span>
 <a id='label804' href="javascript:ContentClick('label805', 'label804');" onmouseover="ContentPreview('label805');" onmouseout="ContentUnpreview('label805');" title="click to collapse or expand..."> more... </a>
 <div id="label805" style="display:none">
 <table border="1">
 <tr>
 <td></td>
 <td colspan="1">Supported Version Ranges</td>
 </tr>
 <tr>
 <td>tgtv_act</td>
 <td><code class="docutils literal notranslate">v7.4.2 -> v7.4.2 </code></td>
 </tr>
 </table>
 </div>
 </li>
                <li> <span class="li-head">tgtv_act_v</span> - Enable to set tact tgtv-act. <span class="li-normal">type: str</span> <span class="li-normal">choices: enable, disable</span>
 <a id='label806' href="javascript:ContentClick('label807', 'label806');" onmouseover="ContentPreview('label807');" onmouseout="ContentUnpreview('label807');" title="click to collapse or expand..."> more... </a>
 <div id="label807" style="display:none">
 <table border="1">
 <tr>
 <td></td>
 <td colspan="1">Supported Version Ranges</td>
 </tr>
 <tr>
 <td>tgtv_act_v</td>
 <td><code class="docutils literal notranslate">v7.4.2 -> v7.4.2 </code></td>
 </tr>
 <tr>
 <td>[enable]</td>
 <td><code class="docutils literal notranslate">v7.4.2 -> v7.4.2</code></td>
 <tr>
 <td>[disable]</td>
 <td><code class="docutils literal notranslate">v7.4.2 -> v7.4.2</code></td>
 </table>
 </div>
 </li>
                <li> <span class="li-head">tlif_act</span> - tcam tact tlif-act. <span class="li-normal">type: int</span>
 <a id='label808' href="javascript:ContentClick('label809', 'label808');" onmouseover="ContentPreview('label809');" onmouseout="ContentUnpreview('label809');" title="click to collapse or expand..."> more... </a>
 <div id="label809" style="display:none">
 <table border="1">
 <tr>
 <td></td>
 <td colspan="1">Supported Version Ranges</td>
 </tr>
 <tr>
 <td>tlif_act</td>
 <td><code class="docutils literal notranslate">v7.4.2 -> v7.4.2 </code></td>
 </tr>
 </table>
 </div>
 </li>
                <li> <span class="li-head">tlif_act_v</span> - Enable to set tact tlif-act. <span class="li-normal">type: str</span> <span class="li-normal">choices: enable, disable</span>
 <a id='label810' href="javascript:ContentClick('label811', 'label810');" onmouseover="ContentPreview('label811');" onmouseout="ContentUnpreview('label811');" title="click to collapse or expand..."> more... </a>
 <div id="label811" style="display:none">
 <table border="1">
 <tr>
 <td></td>
 <td colspan="1">Supported Version Ranges</td>
 </tr>
 <tr>
 <td>tlif_act_v</td>
 <td><code class="docutils literal notranslate">v7.4.2 -> v7.4.2 </code></td>
 </tr>
 <tr>
 <td>[enable]</td>
 <td><code class="docutils literal notranslate">v7.4.2 -> v7.4.2</code></td>
 <tr>
 <td>[disable]</td>
 <td><code class="docutils literal notranslate">v7.4.2 -> v7.4.2</code></td>
 </table>
 </div>
 </li>
                <li> <span class="li-head">tpeid</span> - tcam tact tpeid. <span class="li-normal">type: int</span>
 <a id='label812' href="javascript:ContentClick('label813', 'label812');" onmouseover="ContentPreview('label813');" onmouseout="ContentUnpreview('label813');" title="click to collapse or expand..."> more... </a>
 <div id="label813" style="display:none">
 <table border="1">
 <tr>
 <td></td>
 <td colspan="1">Supported Version Ranges</td>
 </tr>
 <tr>
 <td>tpeid</td>
 <td><code class="docutils literal notranslate">v7.4.2 -> v7.4.2 </code></td>
 </tr>
 </table>
 </div>
 </li>
                <li> <span class="li-head">tpeid_v</span> - Enable to set tact tpeid. <span class="li-normal">type: str</span> <span class="li-normal">choices: enable, disable</span>
 <a id='label814' href="javascript:ContentClick('label815', 'label814');" onmouseover="ContentPreview('label815');" onmouseout="ContentUnpreview('label815');" title="click to collapse or expand..."> more... </a>
 <div id="label815" style="display:none">
 <table border="1">
 <tr>
 <td></td>
 <td colspan="1">Supported Version Ranges</td>
 </tr>
 <tr>
 <td>tpeid_v</td>
 <td><code class="docutils literal notranslate">v7.4.2 -> v7.4.2 </code></td>
 </tr>
 <tr>
 <td>[enable]</td>
 <td><code class="docutils literal notranslate">v7.4.2 -> v7.4.2</code></td>
 <tr>
 <td>[disable]</td>
 <td><code class="docutils literal notranslate">v7.4.2 -> v7.4.2</code></td>
 </table>
 </div>
 </li>
                <li> <span class="li-head">v6fe</span> - tcam tact v6fe. <span class="li-normal">type: int</span>
 <a id='label816' href="javascript:ContentClick('label817', 'label816');" onmouseover="ContentPreview('label817');" onmouseout="ContentUnpreview('label817');" title="click to collapse or expand..."> more... </a>
 <div id="label817" style="display:none">
 <table border="1">
 <tr>
 <td></td>
 <td colspan="1">Supported Version Ranges</td>
 </tr>
 <tr>
 <td>v6fe</td>
 <td><code class="docutils literal notranslate">v7.4.2 -> v7.4.2 </code></td>
 </tr>
 </table>
 </div>
 </li>
                <li> <span class="li-head">v6fe_v</span> - Enable to set tact v6fe. <span class="li-normal">type: str</span> <span class="li-normal">choices: enable, disable</span>
 <a id='label818' href="javascript:ContentClick('label819', 'label818');" onmouseover="ContentPreview('label819');" onmouseout="ContentUnpreview('label819');" title="click to collapse or expand..."> more... </a>
 <div id="label819" style="display:none">
 <table border="1">
 <tr>
 <td></td>
 <td colspan="1">Supported Version Ranges</td>
 </tr>
 <tr>
 <td>v6fe_v</td>
 <td><code class="docutils literal notranslate">v7.4.2 -> v7.4.2 </code></td>
 </tr>
 <tr>
 <td>[enable]</td>
 <td><code class="docutils literal notranslate">v7.4.2 -> v7.4.2</code></td>
 <tr>
 <td>[disable]</td>
 <td><code class="docutils literal notranslate">v7.4.2 -> v7.4.2</code></td>
 </table>
 </div>
 </li>
                <li> <span class="li-head">vep_en</span> - tcam tact vep_en. <span class="li-normal">type: int</span>
 <a id='label820' href="javascript:ContentClick('label821', 'label820');" onmouseover="ContentPreview('label821');" onmouseout="ContentUnpreview('label821');" title="click to collapse or expand..."> more... </a>
 <div id="label821" style="display:none">
 <table border="1">
 <tr>
 <td></td>
 <td colspan="1">Supported Version Ranges</td>
 </tr>
 <tr>
 <td>vep_en</td>
 <td><code class="docutils literal notranslate">v7.4.2 -> v7.4.2 </code></td>
 </tr>
 </table>
 </div>
 </li>
                <li> <span class="li-head">vep_en_v</span> - Enable to set tact vep-en. <span class="li-normal">type: str</span> <span class="li-normal">choices: enable, disable</span>
 <a id='label822' href="javascript:ContentClick('label823', 'label822');" onmouseover="ContentPreview('label823');" onmouseout="ContentUnpreview('label823');" title="click to collapse or expand..."> more... </a>
 <div id="label823" style="display:none">
 <table border="1">
 <tr>
 <td></td>
 <td colspan="1">Supported Version Ranges</td>
 </tr>
 <tr>
 <td>vep_en_v</td>
 <td><code class="docutils literal notranslate">v7.4.2 -> v7.4.2 </code></td>
 </tr>
 <tr>
 <td>[enable]</td>
 <td><code class="docutils literal notranslate">v7.4.2 -> v7.4.2</code></td>
 <tr>
 <td>[disable]</td>
 <td><code class="docutils literal notranslate">v7.4.2 -> v7.4.2</code></td>
 </table>
 </div>
 </li>
                <li> <span class="li-head">vep_slid</span> - tcam tact vep_slid. <span class="li-normal">type: int</span>
 <a id='label824' href="javascript:ContentClick('label825', 'label824');" onmouseover="ContentPreview('label825');" onmouseout="ContentUnpreview('label825');" title="click to collapse or expand..."> more... </a>
 <div id="label825" style="display:none">
 <table border="1">
 <tr>
 <td></td>
 <td colspan="1">Supported Version Ranges</td>
 </tr>
 <tr>
 <td>vep_slid</td>
 <td><code class="docutils literal notranslate">v7.4.2 -> v7.4.2 </code></td>
 </tr>
 </table>
 </div>
 </li>
                <li> <span class="li-head">vep_slid_v</span> - Enable to set tact vep-slid. <span class="li-normal">type: str</span> <span class="li-normal">choices: enable, disable</span>
 <a id='label826' href="javascript:ContentClick('label827', 'label826');" onmouseover="ContentPreview('label827');" onmouseout="ContentUnpreview('label827');" title="click to collapse or expand..."> more... </a>
 <div id="label827" style="display:none">
 <table border="1">
 <tr>
 <td></td>
 <td colspan="1">Supported Version Ranges</td>
 </tr>
 <tr>
 <td>vep_slid_v</td>
 <td><code class="docutils literal notranslate">v7.4.2 -> v7.4.2 </code></td>
 </tr>
 <tr>
 <td>[enable]</td>
 <td><code class="docutils literal notranslate">v7.4.2 -> v7.4.2</code></td>
 <tr>
 <td>[disable]</td>
 <td><code class="docutils literal notranslate">v7.4.2 -> v7.4.2</code></td>
 </table>
 </div>
 </li>
                <li> <span class="li-head">xlt_lif</span> - tcam tact xlt-lif. <span class="li-normal">type: int</span>
 <a id='label828' href="javascript:ContentClick('label829', 'label828');" onmouseover="ContentPreview('label829');" onmouseout="ContentUnpreview('label829');" title="click to collapse or expand..."> more... </a>
 <div id="label829" style="display:none">
 <table border="1">
 <tr>
 <td></td>
 <td colspan="1">Supported Version Ranges</td>
 </tr>
 <tr>
 <td>xlt_lif</td>
 <td><code class="docutils literal notranslate">v7.4.2 -> v7.4.2 </code></td>
 </tr>
 </table>
 </div>
 </li>
                <li> <span class="li-head">xlt_lif_v</span> - Enable to set tact xlt-lif. <span class="li-normal">type: str</span> <span class="li-normal">choices: enable, disable</span>
 <a id='label830' href="javascript:ContentClick('label831', 'label830');" onmouseover="ContentPreview('label831');" onmouseout="ContentUnpreview('label831');" title="click to collapse or expand..."> more... </a>
 <div id="label831" style="display:none">
 <table border="1">
 <tr>
 <td></td>
 <td colspan="1">Supported Version Ranges</td>
 </tr>
 <tr>
 <td>xlt_lif_v</td>
 <td><code class="docutils literal notranslate">v7.4.2 -> v7.4.2 </code></td>
 </tr>
 <tr>
 <td>[enable]</td>
 <td><code class="docutils literal notranslate">v7.4.2 -> v7.4.2</code></td>
 <tr>
 <td>[disable]</td>
 <td><code class="docutils literal notranslate">v7.4.2 -> v7.4.2</code></td>
 </table>
 </div>
 </li>
                <li> <span class="li-head">xlt_vid</span> - tcam tact xlt-vid. <span class="li-normal">type: int</span>
 <a id='label832' href="javascript:ContentClick('label833', 'label832');" onmouseover="ContentPreview('label833');" onmouseout="ContentUnpreview('label833');" title="click to collapse or expand..."> more... </a>
 <div id="label833" style="display:none">
 <table border="1">
 <tr>
 <td></td>
 <td colspan="1">Supported Version Ranges</td>
 </tr>
 <tr>
 <td>xlt_vid</td>
 <td><code class="docutils literal notranslate">v7.4.2 -> v7.4.2 </code></td>
 </tr>
 </table>
 </div>
 </li>
                <li> <span class="li-head">xlt_vid_v</span> - Enable to set tact xlt-vid. <span class="li-normal">type: str</span> <span class="li-normal">choices: enable, disable</span>
 <a id='label834' href="javascript:ContentClick('label835', 'label834');" onmouseover="ContentPreview('label835');" onmouseout="ContentUnpreview('label835');" title="click to collapse or expand..."> more... </a>
 <div id="label835" style="display:none">
 <table border="1">
 <tr>
 <td></td>
 <td colspan="1">Supported Version Ranges</td>
 </tr>
 <tr>
 <td>xlt_vid_v</td>
 <td><code class="docutils literal notranslate">v7.4.2 -> v7.4.2 </code></td>
 </tr>
 <tr>
 <td>[enable]</td>
 <td><code class="docutils literal notranslate">v7.4.2 -> v7.4.2</code></td>
 <tr>
 <td>[disable]</td>
 <td><code class="docutils literal notranslate">v7.4.2 -> v7.4.2</code></td>
 </table>
 </div>
 </li>
                </ul>
            <li> <span class="li-head">type</span> - TCAM policy type. <span class="li-normal">type: str</span> <span class="li-normal">choices: L2_src_tc, L2_tgt_tc, L2_src_mir, L2_tgt_mir, L2_src_act, L2_tgt_act, IPv4_src_tc, IPv4_tgt_tc, IPv4_src_mir, IPv4_tgt_mir, IPv4_src_act, IPv4_tgt_act, IPv6_src_tc, IPv6_tgt_tc, IPv6_src_mir, IPv6_tgt_mir, IPv6_src_act, IPv6_tgt_act</span>
 <a id='label836' href="javascript:ContentClick('label837', 'label836');" onmouseover="ContentPreview('label837');" onmouseout="ContentUnpreview('label837');" title="click to collapse or expand..."> more... </a>
 <div id="label837" style="display:none">
 <table border="1">
 <tr>
 <td></td>
 <td colspan="1">Supported Version Ranges</td>
 </tr>
 <tr>
 <td>type</td>
 <td><code class="docutils literal notranslate">v7.4.2 -> v7.4.2 </code></td>
 </tr>
 <tr>
 <td>[L2_src_tc]</td>
 <td><code class="docutils literal notranslate">v7.4.2 -> v7.4.2</code></td>
 <tr>
 <td>[L2_tgt_tc]</td>
 <td><code class="docutils literal notranslate">v7.4.2 -> v7.4.2</code></td>
 <tr>
 <td>[L2_src_mir]</td>
 <td><code class="docutils literal notranslate">v7.4.2 -> v7.4.2</code></td>
 <tr>
 <td>[L2_tgt_mir]</td>
 <td><code class="docutils literal notranslate">v7.4.2 -> v7.4.2</code></td>
 <tr>
 <td>[L2_src_act]</td>
 <td><code class="docutils literal notranslate">v7.4.2 -> v7.4.2</code></td>
 <tr>
 <td>[L2_tgt_act]</td>
 <td><code class="docutils literal notranslate">v7.4.2 -> v7.4.2</code></td>
 <tr>
 <td>[IPv4_src_tc]</td>
 <td><code class="docutils literal notranslate">v7.4.2 -> v7.4.2</code></td>
 <tr>
 <td>[IPv4_tgt_tc]</td>
 <td><code class="docutils literal notranslate">v7.4.2 -> v7.4.2</code></td>
 <tr>
 <td>[IPv4_src_mir]</td>
 <td><code class="docutils literal notranslate">v7.4.2 -> v7.4.2</code></td>
 <tr>
 <td>[IPv4_tgt_mir]</td>
 <td><code class="docutils literal notranslate">v7.4.2 -> v7.4.2</code></td>
 <tr>
 <td>[IPv4_src_act]</td>
 <td><code class="docutils literal notranslate">v7.4.2 -> v7.4.2</code></td>
 <tr>
 <td>[IPv4_tgt_act]</td>
 <td><code class="docutils literal notranslate">v7.4.2 -> v7.4.2</code></td>
 <tr>
 <td>[IPv6_src_tc]</td>
 <td><code class="docutils literal notranslate">v7.4.2 -> v7.4.2</code></td>
 <tr>
 <td>[IPv6_tgt_tc]</td>
 <td><code class="docutils literal notranslate">v7.4.2 -> v7.4.2</code></td>
 <tr>
 <td>[IPv6_src_mir]</td>
 <td><code class="docutils literal notranslate">v7.4.2 -> v7.4.2</code></td>
 <tr>
 <td>[IPv6_tgt_mir]</td>
 <td><code class="docutils literal notranslate">v7.4.2 -> v7.4.2</code></td>
 <tr>
 <td>[IPv6_src_act]</td>
 <td><code class="docutils literal notranslate">v7.4.2 -> v7.4.2</code></td>
 <tr>
 <td>[IPv6_tgt_act]</td>
 <td><code class="docutils literal notranslate">v7.4.2 -> v7.4.2</code></td>
 </table>
 </div>
 </li>
            <li> <span class="li-head">vid</span> - NPU TCAM VID. <span class="li-normal">type: int</span>
 <a id='label838' href="javascript:ContentClick('label839', 'label838');" onmouseover="ContentPreview('label839');" onmouseout="ContentUnpreview('label839');" title="click to collapse or expand..."> more... </a>
 <div id="label839" style="display:none">
 <table border="1">
 <tr>
 <td></td>
 <td colspan="1">Supported Version Ranges</td>
 </tr>
 <tr>
 <td>vid</td>
 <td><code class="docutils literal notranslate">v7.4.2 -> v7.4.2 </code></td>
 </tr>
 </table>
 </div>
 </li>
            </ul>
        <li> <span class="li-head">per_session_accounting</span> - Set per-session accounting. <span class="li-normal">type: str</span> <span class="li-normal">choices: traffic-log-only, disable, enable</span>
 <a id='label840' href="javascript:ContentClick('label841', 'label840');" onmouseover="ContentPreview('label841');" onmouseout="ContentUnpreview('label841');" title="click to collapse or expand..."> more... </a>
 <div id="label841" style="display:none">
 <table border="1">
 <tr>
 <td></td>
 <td colspan="1">Supported Version Ranges</td>
 </tr>
 <tr>
 <td>per_session_accounting</td>
 <td><code class="docutils literal notranslate">v7.4.2 -> v7.4.2 </code></td>
 </tr>
 <tr>
 <td>[traffic-log-only]</td>
 <td><code class="docutils literal notranslate">v7.4.2 -> v7.4.2</code></td>
 <tr>
 <td>[disable]</td>
 <td><code class="docutils literal notranslate">v7.4.2 -> v7.4.2</code></td>
 <tr>
 <td>[enable]</td>
 <td><code class="docutils literal notranslate">v7.4.2 -> v7.4.2</code></td>
 </table>
 </div>
 </li>
        <li> <span class="li-head">port_cpu_map</span> - Configure NPU interface to CPU core mapping. <span class="li-normal">type: list</span> <span style="font-family:'Courier New'" class="li-required">member_path: port_cpu_map:interface</span>
 <a id='label842' href="javascript:ContentClick('label843', 'label842');" onmouseover="ContentPreview('label843');" onmouseout="ContentUnpreview('label843');" title="click to collapse or expand..."> more... </a>
 <div id="label843" style="display:none">
 <table border="1">
 <tr>
 <td></td><td colspan="4">Supported Version Ranges</td>
 </tr>
 <tr>
 <td>port_cpu_map</td>
 <td><code class="docutils literal notranslate">v6.4.0 -> v6.4.0 </code></td>
 <td><code class="docutils literal notranslate">v7.2.0 -> v7.2.0 </code></td>
 <td><code class="docutils literal notranslate">v7.4.0 -> v7.4.1 </code></td>
 <td><code class="docutils literal notranslate">v7.4.3 -> 7.6.4 </code></td>
 </tr>
 </table>
 </div>
 </li>
            <ul class="ul-self">
            <li> <span class="li-head">cpu_core</span> - The CPU core to map to an interface. <span class="li-normal">type: str</span>
 <a id='label844' href="javascript:ContentClick('label845', 'label844');" onmouseover="ContentPreview('label845');" onmouseout="ContentUnpreview('label845');" title="click to collapse or expand..."> more... </a>
 <div id="label845" style="display:none">
 <table border="1">
 <tr>
 <td></td>
 <td colspan="4">Supported Version Ranges</td>
 </tr>
 <tr>
 <td>cpu_core</td>
 <td><code class="docutils literal notranslate">v6.4.0 -> v6.4.0 </code></td>
 <td><code class="docutils literal notranslate">v7.2.0 -> v7.2.0 </code></td>
 <td><code class="docutils literal notranslate">v7.4.0 -> v7.4.1 </code></td>
 <td><code class="docutils literal notranslate">v7.4.3 -> 7.6.4 </code></td>
 </tr>
 </table>
 </div>
 </li>
            <li> <span class="li-head">interface</span> - The interface to map to a CPU core. <span class="li-normal">type: str</span> <span class="li-required">required: true</span>
 <a id='label846' href="javascript:ContentClick('label847', 'label846');" onmouseover="ContentPreview('label847');" onmouseout="ContentUnpreview('label847');" title="click to collapse or expand..."> more... </a>
 <div id="label847" style="display:none">
 <table border="1">
 <tr>
 <td></td>
 <td colspan="4">Supported Version Ranges</td>
 </tr>
 <tr>
 <td>interface</td>
 <td><code class="docutils literal notranslate">v6.4.0 -> v6.4.0 </code></td>
 <td><code class="docutils literal notranslate">v7.2.0 -> v7.2.0 </code></td>
 <td><code class="docutils literal notranslate">v7.4.0 -> v7.4.1 </code></td>
 <td><code class="docutils literal notranslate">v7.4.3 -> 7.6.4 </code></td>
 </tr>
 </table>
 </div>
 </li>
            </ul>
        <li> <span class="li-head">port_npu_map</span> - Configure port to NPU group mapping. <span class="li-normal">type: list</span> <span style="font-family:'Courier New'" class="li-required">member_path: port_npu_map:interface</span>
 <a id='label848' href="javascript:ContentClick('label849', 'label848');" onmouseover="ContentPreview('label849');" onmouseout="ContentUnpreview('label849');" title="click to collapse or expand..."> more... </a>
 <div id="label849" style="display:none">
 <table border="1">
 <tr>
 <td></td><td colspan="4">Supported Version Ranges</td>
 </tr>
 <tr>
 <td>port_npu_map</td>
 <td><code class="docutils literal notranslate">v6.0.0 -> v6.2.7 </code></td>
 <td><code class="docutils literal notranslate">v6.4.1 -> v7.0.12 </code></td>
 <td><code class="docutils literal notranslate">v7.2.1 -> v7.2.4 </code></td>
 <td><code class="docutils literal notranslate">v7.4.2 -> v7.4.2 </code></td>
 </tr>
 </table>
 </div>
 </li>
            <ul class="ul-self">
            <li> <span class="li-head">interface</span> - Set NPU interface port for NPU group mapping. <span class="li-normal">type: str</span> <span class="li-required">required: true</span>
 <a id='label850' href="javascript:ContentClick('label851', 'label850');" onmouseover="ContentPreview('label851');" onmouseout="ContentUnpreview('label851');" title="click to collapse or expand..."> more... </a>
 <div id="label851" style="display:none">
 <table border="1">
 <tr>
 <td></td>
 <td colspan="4">Supported Version Ranges</td>
 </tr>
 <tr>
 <td>interface</td>
 <td><code class="docutils literal notranslate">v6.0.0 -> v6.2.7 </code></td>
 <td><code class="docutils literal notranslate">v6.4.1 -> v7.0.12 </code></td>
 <td><code class="docutils literal notranslate">v7.2.1 -> v7.2.4 </code></td>
 <td><code class="docutils literal notranslate">v7.4.2 -> v7.4.2 </code></td>
 </tr>
 </table>
 </div>
 </li>
            <li> <span class="li-head">npu_group_index</span> - Mapping NPU group index. <span class="li-normal">type: int</span>
 <a id='label852' href="javascript:ContentClick('label853', 'label852');" onmouseover="ContentPreview('label853');" onmouseout="ContentUnpreview('label853');" title="click to collapse or expand..."> more... </a>
 <div id="label853" style="display:none">
 <table border="1">
 <tr>
 <td></td>
 <td colspan="4">Supported Version Ranges</td>
 </tr>
 <tr>
 <td>npu_group_index</td>
 <td><code class="docutils literal notranslate">v6.0.0 -> v6.2.7 </code></td>
 <td><code class="docutils literal notranslate">v6.4.1 -> v7.0.12 </code></td>
 <td><code class="docutils literal notranslate">v7.2.1 -> v7.2.4 </code></td>
 <td><code class="docutils literal notranslate">v7.4.2 -> v7.4.2 </code></td>
 </tr>
 </table>
 </div>
 </li>
            </ul>
        <li> <span class="li-head">port_path_option</span> - Configure port using NPU or Intel-NIC. <span class="li-normal">type: dict</span>
 <a id='label854' href="javascript:ContentClick('label855', 'label854');" onmouseover="ContentPreview('label855');" onmouseout="ContentUnpreview('label855');" title="click to collapse or expand..."> more... </a>
 <div id="label855" style="display:none">
 <table border="1">
 <tr>
 <td></td><td colspan="1">Supported Version Ranges</td>
 </tr>
 <tr>
 <td>port_path_option</td>
 <td><code class="docutils literal notranslate">v7.4.2 -> v7.4.2 </code></td>
 </tr>
 </table>
 </div>
 </li>
            <ul class="ul-self">
            <li> <span class="li-head">ports_using_npu</span> - Set ha/aux ports to handle traffic with NPU (otherwise traffic goes to Intel-NIC and then CPU). <span class="li-normal">type: list</span> <span style="font-family:'Courier New'" class="li-required">member_path: port_path_option/ports_using_npu:interface_name</span>
 <a id='label856' href="javascript:ContentClick('label857', 'label856');" onmouseover="ContentPreview('label857');" onmouseout="ContentUnpreview('label857');" title="click to collapse or expand..."> more... </a>
 <div id="label857" style="display:none">
 <table border="1">
 <tr>
 <td></td><td colspan="1">Supported Version Ranges</td>
 </tr>
 <tr>
 <td>ports_using_npu</td>
 <td><code class="docutils literal notranslate">v7.4.2 -> v7.4.2 </code></td>
 </tr>
 </table>
 </div>
 </li>
                <ul class="ul-self">
                <li> <span class="li-head">interface_name</span> - Available interfaces for NPU path. <span class="li-normal">type: str</span> <span class="li-required">required: true</span>
 <a id='label858' href="javascript:ContentClick('label859', 'label858');" onmouseover="ContentPreview('label859');" onmouseout="ContentUnpreview('label859');" title="click to collapse or expand..."> more... </a>
 <div id="label859" style="display:none">
 <table border="1">
 <tr>
 <td></td>
 <td colspan="1">Supported Version Ranges</td>
 </tr>
 <tr>
 <td>interface_name</td>
 <td><code class="docutils literal notranslate">v7.4.2 -> v7.4.2 </code></td>
 </tr>
 </table>
 </div>
 </li>
                </ul>
            </ul>
        <li> <span class="li-head">priority_protocol</span> - Configure NPU priority protocol. <span class="li-normal">type: dict</span>
 <a id='label860' href="javascript:ContentClick('label861', 'label860');" onmouseover="ContentPreview('label861');" onmouseout="ContentUnpreview('label861');" title="click to collapse or expand..."> more... </a>
 <div id="label861" style="display:none">
 <table border="1">
 <tr>
 <td></td><td colspan="3">Supported Version Ranges</td>
 </tr>
 <tr>
 <td>priority_protocol</td>
 <td><code class="docutils literal notranslate">v6.0.0 -> v6.0.0 </code></td>
 <td><code class="docutils literal notranslate">v6.0.11 -> v7.4.1 </code></td>
 <td><code class="docutils literal notranslate">v7.4.3 -> 7.6.4 </code></td>
 </tr>
 </table>
 </div>
 </li>
            <ul class="ul-self">
            <li> <span class="li-head">bfd</span> - Enable/disable NPU BFD priority protocol. <span class="li-normal">type: str</span> <span class="li-normal">choices: enable, disable</span>
 <a id='label862' href="javascript:ContentClick('label863', 'label862');" onmouseover="ContentPreview('label863');" onmouseout="ContentUnpreview('label863');" title="click to collapse or expand..."> more... </a>
 <div id="label863" style="display:none">
 <table border="1">
 <tr>
 <td></td>
 <td colspan="3">Supported Version Ranges</td>
 </tr>
 <tr>
 <td>bfd</td>
 <td><code class="docutils literal notranslate">v6.0.0 -> v6.0.0 </code></td>
 <td><code class="docutils literal notranslate">v6.0.11 -> v7.4.1 </code></td>
 <td><code class="docutils literal notranslate">v7.4.3 -> 7.6.4 </code></td>
 </tr>
 <tr>
 <td>[enable]</td>
 <td><code class="docutils literal notranslate">v6.0.0 -> v6.0.0</code></td>
 <tr>
 <td>[disable]</td>
 <td><code class="docutils literal notranslate">v6.0.0 -> v6.0.0</code></td>
 </table>
 </div>
 </li>
            <li> <span class="li-head">bgp</span> - Enable/disable NPU BGP priority protocol. <span class="li-normal">type: str</span> <span class="li-normal">choices: enable, disable</span>
 <a id='label864' href="javascript:ContentClick('label865', 'label864');" onmouseover="ContentPreview('label865');" onmouseout="ContentUnpreview('label865');" title="click to collapse or expand..."> more... </a>
 <div id="label865" style="display:none">
 <table border="1">
 <tr>
 <td></td>
 <td colspan="3">Supported Version Ranges</td>
 </tr>
 <tr>
 <td>bgp</td>
 <td><code class="docutils literal notranslate">v6.0.0 -> v6.0.0 </code></td>
 <td><code class="docutils literal notranslate">v6.0.11 -> v7.4.1 </code></td>
 <td><code class="docutils literal notranslate">v7.4.3 -> 7.6.4 </code></td>
 </tr>
 <tr>
 <td>[enable]</td>
 <td><code class="docutils literal notranslate">v6.0.0 -> v6.0.0</code></td>
 <tr>
 <td>[disable]</td>
 <td><code class="docutils literal notranslate">v6.0.0 -> v6.0.0</code></td>
 </table>
 </div>
 </li>
            <li> <span class="li-head">slbc</span> - Enable/disable NPU SLBC priority protocol. <span class="li-normal">type: str</span> <span class="li-normal">choices: enable, disable</span>
 <a id='label866' href="javascript:ContentClick('label867', 'label866');" onmouseover="ContentPreview('label867');" onmouseout="ContentUnpreview('label867');" title="click to collapse or expand..."> more... </a>
 <div id="label867" style="display:none">
 <table border="1">
 <tr>
 <td></td>
 <td colspan="3">Supported Version Ranges</td>
 </tr>
 <tr>
 <td>slbc</td>
 <td><code class="docutils literal notranslate">v6.0.0 -> v6.0.0 </code></td>
 <td><code class="docutils literal notranslate">v6.0.11 -> v7.4.1 </code></td>
 <td><code class="docutils literal notranslate">v7.4.3 -> 7.6.4 </code></td>
 </tr>
 <tr>
 <td>[enable]</td>
 <td><code class="docutils literal notranslate">v6.0.0 -> v6.0.0</code></td>
 <tr>
 <td>[disable]</td>
 <td><code class="docutils literal notranslate">v6.0.0 -> v6.0.0</code></td>
 </table>
 </div>
 </li>
            </ul>
        <li> <span class="li-head">qos_mode</span> - QoS mode on switch and NP. <span class="li-normal">type: str</span> <span class="li-normal">choices: disable, priority, round-robin</span>
 <a id='label868' href="javascript:ContentClick('label869', 'label868');" onmouseover="ContentPreview('label869');" onmouseout="ContentUnpreview('label869');" title="click to collapse or expand..."> more... </a>
 <div id="label869" style="display:none">
 <table border="1">
 <tr>
 <td></td>
 <td colspan="4">Supported Version Ranges</td>
 </tr>
 <tr>
 <td>qos_mode</td>
 <td><code class="docutils literal notranslate">v6.4.0 -> v6.4.0 </code></td>
 <td><code class="docutils literal notranslate">v7.2.0 -> v7.2.0 </code></td>
 <td><code class="docutils literal notranslate">v7.4.0 -> v7.4.1 </code></td>
 <td><code class="docutils literal notranslate">v7.4.3 -> 7.6.4 </code></td>
 </tr>
 <tr>
 <td>[disable]</td>
 <td><code class="docutils literal notranslate">v6.4.0 -> v6.4.0</code></td>
 <tr>
 <td>[priority]</td>
 <td><code class="docutils literal notranslate">v6.4.0 -> v6.4.0</code></td>
 <tr>
 <td>[round-robin]</td>
 <td><code class="docutils literal notranslate">v6.4.0 -> v6.4.0</code></td>
 </table>
 </div>
 </li>
        <li> <span class="li-head">qtm_buf_mode</span> - QTM channel configuration for packet buffer. <span class="li-normal">type: str</span> <span class="li-normal">choices: 6ch, 4ch</span>
 <a id='label870' href="javascript:ContentClick('label871', 'label870');" onmouseover="ContentPreview('label871');" onmouseout="ContentUnpreview('label871');" title="click to collapse or expand..."> more... </a>
 <div id="label871" style="display:none">
 <table border="1">
 <tr>
 <td></td>
 <td colspan="1">Supported Version Ranges</td>
 </tr>
 <tr>
 <td>qtm_buf_mode</td>
 <td><code class="docutils literal notranslate">v7.4.2 -> v7.4.2 </code></td>
 </tr>
 <tr>
 <td>[6ch]</td>
 <td><code class="docutils literal notranslate">v7.4.2 -> v7.4.2</code></td>
 <tr>
 <td>[4ch]</td>
 <td><code class="docutils literal notranslate">v7.4.2 -> v7.4.2</code></td>
 </table>
 </div>
 </li>
        <li> <span class="li-head">rdp_offload</span> - Enable/disable RDP offload. <span class="li-normal">type: str</span> <span class="li-normal">choices: enable, disable</span>
 <a id='label872' href="javascript:ContentClick('label873', 'label872');" onmouseover="ContentPreview('label873');" onmouseout="ContentUnpreview('label873');" title="click to collapse or expand..."> more... </a>
 <div id="label873" style="display:none">
 <table border="1">
 <tr>
 <td></td>
 <td colspan="2">Supported Version Ranges</td>
 </tr>
 <tr>
 <td>rdp_offload</td>
 <td><code class="docutils literal notranslate">v6.0.0 -> v7.4.1 </code></td>
 <td><code class="docutils literal notranslate">v7.4.3 -> 7.6.4 </code></td>
 </tr>
 <tr>
 <td>[enable]</td>
 <td><code class="docutils literal notranslate">v6.0.0 -> v7.4.1</code></td>
 <tr>
 <td>[disable]</td>
 <td><code class="docutils literal notranslate">v6.0.0 -> v7.4.1</code></td>
 </table>
 </div>
 </li>
        <li> <span class="li-head">session_acct_interval</span> - Session accounting update interval (1 - 10 sec). <span class="li-normal">type: int</span>
 <a id='label874' href="javascript:ContentClick('label875', 'label874');" onmouseover="ContentPreview('label875');" onmouseout="ContentUnpreview('label875');" title="click to collapse or expand..."> more... </a>
 <div id="label875" style="display:none">
 <table border="1">
 <tr>
 <td></td>
 <td colspan="1">Supported Version Ranges</td>
 </tr>
 <tr>
 <td>session_acct_interval</td>
 <td><code class="docutils literal notranslate">v7.4.2 -> v7.4.2 </code></td>
 </tr>
 </table>
 </div>
 </li>
        <li> <span class="li-head">session_denied_offload</span> - Enable/disable offloading of denied sessions. Requires ses-denied-traffic to be set. <span class="li-normal">type: str</span> <span class="li-normal">choices: disable, enable</span>
 <a id='label876' href="javascript:ContentClick('label877', 'label876');" onmouseover="ContentPreview('label877');" onmouseout="ContentUnpreview('label877');" title="click to collapse or expand..."> more... </a>
 <div id="label877" style="display:none">
 <table border="1">
 <tr>
 <td></td>
 <td colspan="2">Supported Version Ranges</td>
 </tr>
 <tr>
 <td>session_denied_offload</td>
 <td><code class="docutils literal notranslate">v7.0.0 -> v7.4.1 </code></td>
 <td><code class="docutils literal notranslate">v7.4.3 -> 7.6.4 </code></td>
 </tr>
 <tr>
 <td>[disable]</td>
 <td><code class="docutils literal notranslate">v7.0.0 -> v7.4.1</code></td>
 <tr>
 <td>[enable]</td>
 <td><code class="docutils literal notranslate">v7.0.0 -> v7.4.1</code></td>
 </table>
 </div>
 </li>
        <li> <span class="li-head">shaping_stats</span> - Enable/disable NP7 traffic shaping statistics . <span class="li-normal">type: str</span> <span class="li-normal">choices: disable, enable</span>
 <a id='label878' href="javascript:ContentClick('label879', 'label878');" onmouseover="ContentPreview('label879');" onmouseout="ContentUnpreview('label879');" title="click to collapse or expand..."> more... </a>
 <div id="label879" style="display:none">
 <table border="1">
 <tr>
 <td></td>
 <td colspan="1">Supported Version Ranges</td>
 </tr>
 <tr>
 <td>shaping_stats</td>
 <td><code class="docutils literal notranslate">v7.4.2 -> v7.4.2 </code></td>
 </tr>
 <tr>
 <td>[disable]</td>
 <td><code class="docutils literal notranslate">v7.4.2 -> v7.4.2</code></td>
 <tr>
 <td>[enable]</td>
 <td><code class="docutils literal notranslate">v7.4.2 -> v7.4.2</code></td>
 </table>
 </div>
 </li>
        <li> <span class="li-head">sse_backpressure</span> - Enable/disable SSE backpressure. <span class="li-normal">type: str</span> <span class="li-normal">choices: enable, disable</span>
 <a id='label880' href="javascript:ContentClick('label881', 'label880');" onmouseover="ContentPreview('label881');" onmouseout="ContentUnpreview('label881');" title="click to collapse or expand..."> more... </a>
 <div id="label881" style="display:none">
 <table border="1">
 <tr>
 <td></td>
 <td colspan="2">Supported Version Ranges</td>
 </tr>
 <tr>
 <td>sse_backpressure</td>
 <td><code class="docutils literal notranslate">v6.0.0 -> v7.4.1 </code></td>
 <td><code class="docutils literal notranslate">v7.4.3 -> 7.6.4 </code></td>
 </tr>
 <tr>
 <td>[enable]</td>
 <td><code class="docutils literal notranslate">v6.0.0 -> v7.4.1</code></td>
 <tr>
 <td>[disable]</td>
 <td><code class="docutils literal notranslate">v6.0.0 -> v7.4.1</code></td>
 </table>
 </div>
 </li>
        <li> <span class="li-head">strip_clear_text_padding</span> - Enable/disable stripping clear text padding. <span class="li-normal">type: str</span> <span class="li-normal">choices: enable, disable</span>
 <a id='label882' href="javascript:ContentClick('label883', 'label882');" onmouseover="ContentPreview('label883');" onmouseout="ContentUnpreview('label883');" title="click to collapse or expand..."> more... </a>
 <div id="label883" style="display:none">
 <table border="1">
 <tr>
 <td></td>
 <td colspan="2">Supported Version Ranges</td>
 </tr>
 <tr>
 <td>strip_clear_text_padding</td>
 <td><code class="docutils literal notranslate">v6.0.0 -> v7.4.1 </code></td>
 <td><code class="docutils literal notranslate">v7.4.3 -> 7.6.4 </code></td>
 </tr>
 <tr>
 <td>[enable]</td>
 <td><code class="docutils literal notranslate">v6.0.0 -> v7.4.1</code></td>
 <tr>
 <td>[disable]</td>
 <td><code class="docutils literal notranslate">v6.0.0 -> v7.4.1</code></td>
 </table>
 </div>
 </li>
        <li> <span class="li-head">strip_esp_padding</span> - Enable/disable stripping ESP padding. <span class="li-normal">type: str</span> <span class="li-normal">choices: enable, disable</span>
 <a id='label884' href="javascript:ContentClick('label885', 'label884');" onmouseover="ContentPreview('label885');" onmouseout="ContentUnpreview('label885');" title="click to collapse or expand..."> more... </a>
 <div id="label885" style="display:none">
 <table border="1">
 <tr>
 <td></td>
 <td colspan="2">Supported Version Ranges</td>
 </tr>
 <tr>
 <td>strip_esp_padding</td>
 <td><code class="docutils literal notranslate">v6.0.0 -> v7.4.1 </code></td>
 <td><code class="docutils literal notranslate">v7.4.3 -> 7.6.4 </code></td>
 </tr>
 <tr>
 <td>[enable]</td>
 <td><code class="docutils literal notranslate">v6.0.0 -> v7.4.1</code></td>
 <tr>
 <td>[disable]</td>
 <td><code class="docutils literal notranslate">v6.0.0 -> v7.4.1</code></td>
 </table>
 </div>
 </li>
        <li> <span class="li-head">sw_eh_hash</span> - Configure switch enhanced hashing. <span class="li-normal">type: dict</span>
 <a id='label886' href="javascript:ContentClick('label887', 'label886');" onmouseover="ContentPreview('label887');" onmouseout="ContentUnpreview('label887');" title="click to collapse or expand..."> more... </a>
 <div id="label887" style="display:none">
 <table border="1">
 <tr>
 <td></td><td colspan="3">Supported Version Ranges</td>
 </tr>
 <tr>
 <td>sw_eh_hash</td>
 <td><code class="docutils literal notranslate">v7.2.0 -> v7.2.0 </code></td>
 <td><code class="docutils literal notranslate">v7.4.0 -> v7.4.1 </code></td>
 <td><code class="docutils literal notranslate">v7.4.3 -> 7.6.4 </code></td>
 </tr>
 </table>
 </div>
 </li>
            <ul class="ul-self">
            <li> <span class="li-head">computation</span> - Set hashing computation. <span class="li-normal">type: str</span> <span class="li-normal">choices: xor16, xor8, xor4, crc16</span>
 <a id='label888' href="javascript:ContentClick('label889', 'label888');" onmouseover="ContentPreview('label889');" onmouseout="ContentUnpreview('label889');" title="click to collapse or expand..."> more... </a>
 <div id="label889" style="display:none">
 <table border="1">
 <tr>
 <td></td>
 <td colspan="3">Supported Version Ranges</td>
 </tr>
 <tr>
 <td>computation</td>
 <td><code class="docutils literal notranslate">v7.2.0 -> v7.2.0 </code></td>
 <td><code class="docutils literal notranslate">v7.4.0 -> v7.4.1 </code></td>
 <td><code class="docutils literal notranslate">v7.4.3 -> 7.6.4 </code></td>
 </tr>
 <tr>
 <td>[xor16]</td>
 <td><code class="docutils literal notranslate">v7.2.0 -> v7.2.0</code></td>
 <tr>
 <td>[xor8]</td>
 <td><code class="docutils literal notranslate">v7.2.0 -> v7.2.0</code></td>
 <tr>
 <td>[xor4]</td>
 <td><code class="docutils literal notranslate">v7.2.0 -> v7.2.0</code></td>
 <tr>
 <td>[crc16]</td>
 <td><code class="docutils literal notranslate">v7.2.0 -> v7.2.0</code></td>
 </table>
 </div>
 </li>
            <li> <span class="li-head">destination_ip_lower_16</span> - Include/exclude destination IP address lower 16 bits. <span class="li-normal">type: str</span> <span class="li-normal">choices: include, exclude</span>
 <a id='label890' href="javascript:ContentClick('label891', 'label890');" onmouseover="ContentPreview('label891');" onmouseout="ContentUnpreview('label891');" title="click to collapse or expand..."> more... </a>
 <div id="label891" style="display:none">
 <table border="1">
 <tr>
 <td></td>
 <td colspan="3">Supported Version Ranges</td>
 </tr>
 <tr>
 <td>destination_ip_lower_16</td>
 <td><code class="docutils literal notranslate">v7.2.0 -> v7.2.0 </code></td>
 <td><code class="docutils literal notranslate">v7.4.0 -> v7.4.1 </code></td>
 <td><code class="docutils literal notranslate">v7.4.3 -> 7.6.4 </code></td>
 </tr>
 <tr>
 <td>[include]</td>
 <td><code class="docutils literal notranslate">v7.2.0 -> v7.2.0</code></td>
 <tr>
 <td>[exclude]</td>
 <td><code class="docutils literal notranslate">v7.2.0 -> v7.2.0</code></td>
 </table>
 </div>
 </li>
            <li> <span class="li-head">destination_ip_upper_16</span> - Include/exclude destination IP address upper 16 bits. <span class="li-normal">type: str</span> <span class="li-normal">choices: include, exclude</span>
 <a id='label892' href="javascript:ContentClick('label893', 'label892');" onmouseover="ContentPreview('label893');" onmouseout="ContentUnpreview('label893');" title="click to collapse or expand..."> more... </a>
 <div id="label893" style="display:none">
 <table border="1">
 <tr>
 <td></td>
 <td colspan="3">Supported Version Ranges</td>
 </tr>
 <tr>
 <td>destination_ip_upper_16</td>
 <td><code class="docutils literal notranslate">v7.2.0 -> v7.2.0 </code></td>
 <td><code class="docutils literal notranslate">v7.4.0 -> v7.4.1 </code></td>
 <td><code class="docutils literal notranslate">v7.4.3 -> 7.6.4 </code></td>
 </tr>
 <tr>
 <td>[include]</td>
 <td><code class="docutils literal notranslate">v7.2.0 -> v7.2.0</code></td>
 <tr>
 <td>[exclude]</td>
 <td><code class="docutils literal notranslate">v7.2.0 -> v7.2.0</code></td>
 </table>
 </div>
 </li>
            <li> <span class="li-head">destination_port</span> - Include/exclude destination port if TCP/UDP. <span class="li-normal">type: str</span> <span class="li-normal">choices: include, exclude</span>
 <a id='label894' href="javascript:ContentClick('label895', 'label894');" onmouseover="ContentPreview('label895');" onmouseout="ContentUnpreview('label895');" title="click to collapse or expand..."> more... </a>
 <div id="label895" style="display:none">
 <table border="1">
 <tr>
 <td></td>
 <td colspan="3">Supported Version Ranges</td>
 </tr>
 <tr>
 <td>destination_port</td>
 <td><code class="docutils literal notranslate">v7.2.0 -> v7.2.0 </code></td>
 <td><code class="docutils literal notranslate">v7.4.0 -> v7.4.1 </code></td>
 <td><code class="docutils literal notranslate">v7.4.3 -> 7.6.4 </code></td>
 </tr>
 <tr>
 <td>[include]</td>
 <td><code class="docutils literal notranslate">v7.2.0 -> v7.2.0</code></td>
 <tr>
 <td>[exclude]</td>
 <td><code class="docutils literal notranslate">v7.2.0 -> v7.2.0</code></td>
 </table>
 </div>
 </li>
            <li> <span class="li-head">ip_protocol</span> - Include/exclude IP protocol. <span class="li-normal">type: str</span> <span class="li-normal">choices: include, exclude</span>
 <a id='label896' href="javascript:ContentClick('label897', 'label896');" onmouseover="ContentPreview('label897');" onmouseout="ContentUnpreview('label897');" title="click to collapse or expand..."> more... </a>
 <div id="label897" style="display:none">
 <table border="1">
 <tr>
 <td></td>
 <td colspan="3">Supported Version Ranges</td>
 </tr>
 <tr>
 <td>ip_protocol</td>
 <td><code class="docutils literal notranslate">v7.2.0 -> v7.2.0 </code></td>
 <td><code class="docutils literal notranslate">v7.4.0 -> v7.4.1 </code></td>
 <td><code class="docutils literal notranslate">v7.4.3 -> 7.6.4 </code></td>
 </tr>
 <tr>
 <td>[include]</td>
 <td><code class="docutils literal notranslate">v7.2.0 -> v7.2.0</code></td>
 <tr>
 <td>[exclude]</td>
 <td><code class="docutils literal notranslate">v7.2.0 -> v7.2.0</code></td>
 </table>
 </div>
 </li>
            <li> <span class="li-head">netmask_length</span> - Network mask length. <span class="li-normal">type: int</span>
 <a id='label898' href="javascript:ContentClick('label899', 'label898');" onmouseover="ContentPreview('label899');" onmouseout="ContentUnpreview('label899');" title="click to collapse or expand..."> more... </a>
 <div id="label899" style="display:none">
 <table border="1">
 <tr>
 <td></td>
 <td colspan="3">Supported Version Ranges</td>
 </tr>
 <tr>
 <td>netmask_length</td>
 <td><code class="docutils literal notranslate">v7.2.0 -> v7.2.0 </code></td>
 <td><code class="docutils literal notranslate">v7.4.0 -> v7.4.1 </code></td>
 <td><code class="docutils literal notranslate">v7.4.3 -> 7.6.4 </code></td>
 </tr>
 </table>
 </div>
 </li>
            <li> <span class="li-head">source_ip_lower_16</span> - Include/exclude source IP address lower 16 bits. <span class="li-normal">type: str</span> <span class="li-normal">choices: include, exclude</span>
 <a id='label900' href="javascript:ContentClick('label901', 'label900');" onmouseover="ContentPreview('label901');" onmouseout="ContentUnpreview('label901');" title="click to collapse or expand..."> more... </a>
 <div id="label901" style="display:none">
 <table border="1">
 <tr>
 <td></td>
 <td colspan="3">Supported Version Ranges</td>
 </tr>
 <tr>
 <td>source_ip_lower_16</td>
 <td><code class="docutils literal notranslate">v7.2.0 -> v7.2.0 </code></td>
 <td><code class="docutils literal notranslate">v7.4.0 -> v7.4.1 </code></td>
 <td><code class="docutils literal notranslate">v7.4.3 -> 7.6.4 </code></td>
 </tr>
 <tr>
 <td>[include]</td>
 <td><code class="docutils literal notranslate">v7.2.0 -> v7.2.0</code></td>
 <tr>
 <td>[exclude]</td>
 <td><code class="docutils literal notranslate">v7.2.0 -> v7.2.0</code></td>
 </table>
 </div>
 </li>
            <li> <span class="li-head">source_ip_upper_16</span> - Include/exclude source IP address upper 16 bits. <span class="li-normal">type: str</span> <span class="li-normal">choices: include, exclude</span>
 <a id='label902' href="javascript:ContentClick('label903', 'label902');" onmouseover="ContentPreview('label903');" onmouseout="ContentUnpreview('label903');" title="click to collapse or expand..."> more... </a>
 <div id="label903" style="display:none">
 <table border="1">
 <tr>
 <td></td>
 <td colspan="3">Supported Version Ranges</td>
 </tr>
 <tr>
 <td>source_ip_upper_16</td>
 <td><code class="docutils literal notranslate">v7.2.0 -> v7.2.0 </code></td>
 <td><code class="docutils literal notranslate">v7.4.0 -> v7.4.1 </code></td>
 <td><code class="docutils literal notranslate">v7.4.3 -> 7.6.4 </code></td>
 </tr>
 <tr>
 <td>[include]</td>
 <td><code class="docutils literal notranslate">v7.2.0 -> v7.2.0</code></td>
 <tr>
 <td>[exclude]</td>
 <td><code class="docutils literal notranslate">v7.2.0 -> v7.2.0</code></td>
 </table>
 </div>
 </li>
            <li> <span class="li-head">source_port</span> - Include/exclude source port if TCP/UDP. <span class="li-normal">type: str</span> <span class="li-normal">choices: include, exclude</span>
 <a id='label904' href="javascript:ContentClick('label905', 'label904');" onmouseover="ContentPreview('label905');" onmouseout="ContentUnpreview('label905');" title="click to collapse or expand..."> more... </a>
 <div id="label905" style="display:none">
 <table border="1">
 <tr>
 <td></td>
 <td colspan="3">Supported Version Ranges</td>
 </tr>
 <tr>
 <td>source_port</td>
 <td><code class="docutils literal notranslate">v7.2.0 -> v7.2.0 </code></td>
 <td><code class="docutils literal notranslate">v7.4.0 -> v7.4.1 </code></td>
 <td><code class="docutils literal notranslate">v7.4.3 -> 7.6.4 </code></td>
 </tr>
 <tr>
 <td>[include]</td>
 <td><code class="docutils literal notranslate">v7.2.0 -> v7.2.0</code></td>
 <tr>
 <td>[exclude]</td>
 <td><code class="docutils literal notranslate">v7.2.0 -> v7.2.0</code></td>
 </table>
 </div>
 </li>
            </ul>
        <li> <span class="li-head">sw_np_bandwidth</span> - Bandwidth from switch to NP. <span class="li-normal">type: str</span> <span class="li-normal">choices: 0G, 2G, 4G, 5G, 6G, 7G, 8G, 9G</span>
 <a id='label906' href="javascript:ContentClick('label907', 'label906');" onmouseover="ContentPreview('label907');" onmouseout="ContentUnpreview('label907');" title="click to collapse or expand..."> more... </a>
 <div id="label907" style="display:none">
 <table border="1">
 <tr>
 <td></td>
 <td colspan="2">Supported Version Ranges</td>
 </tr>
 <tr>
 <td>sw_np_bandwidth</td>
 <td><code class="docutils literal notranslate">v6.2.0 -> v7.4.1 </code></td>
 <td><code class="docutils literal notranslate">v7.4.3 -> 7.6.4 </code></td>
 </tr>
 <tr>
 <td>[0G]</td>
 <td><code class="docutils literal notranslate">v6.2.0 -> v7.4.1</code></td>
 <tr>
 <td>[2G]</td>
 <td><code class="docutils literal notranslate">v6.2.0 -> v7.4.1</code></td>
 <tr>
 <td>[4G]</td>
 <td><code class="docutils literal notranslate">v6.2.0 -> v7.4.1</code></td>
 <tr>
 <td>[5G]</td>
 <td><code class="docutils literal notranslate">v6.2.0 -> v7.4.1</code></td>
 <tr>
 <td>[6G]</td>
 <td><code class="docutils literal notranslate">v6.2.0 -> v7.4.1</code></td>
 <tr>
 <td>[7G]</td>
 <td><code class="docutils literal notranslate">v7.4.0 -> v7.4.1</code></td>
 <td><code class="docutils literal notranslate">v7.4.3 -> 7.6.4</code></td>
 </tr>
 <tr>
 <td>[8G]</td>
 <td><code class="docutils literal notranslate">v7.4.0 -> v7.4.1</code></td>
 <td><code class="docutils literal notranslate">v7.4.3 -> 7.6.4</code></td>
 </tr>
 <tr>
 <td>[9G]</td>
 <td><code class="docutils literal notranslate">v7.4.0 -> v7.4.1</code></td>
 <td><code class="docutils literal notranslate">v7.4.3 -> 7.6.4</code></td>
 </tr>
 </table>
 </div>
 </li>
        <li> <span class="li-head">sw_tr_hash</span> - Configure switch traditional hashing. <span class="li-normal">type: dict</span>
 <a id='label908' href="javascript:ContentClick('label909', 'label908');" onmouseover="ContentPreview('label909');" onmouseout="ContentUnpreview('label909');" title="click to collapse or expand..."> more... </a>
 <div id="label909" style="display:none">
 <table border="1">
 <tr>
 <td></td><td colspan="2">Supported Version Ranges</td>
 </tr>
 <tr>
 <td>sw_tr_hash</td>
 <td><code class="docutils literal notranslate">v7.4.0 -> v7.4.1 </code></td>
 <td><code class="docutils literal notranslate">v7.4.3 -> 7.6.4 </code></td>
 </tr>
 </table>
 </div>
 </li>
            <ul class="ul-self">
            <li> <span class="li-head">draco15</span> - Enable/disable DRACO15 hashing. <span class="li-normal">type: str</span> <span class="li-normal">choices: enable, disable</span>
 <a id='label910' href="javascript:ContentClick('label911', 'label910');" onmouseover="ContentPreview('label911');" onmouseout="ContentUnpreview('label911');" title="click to collapse or expand..."> more... </a>
 <div id="label911" style="display:none">
 <table border="1">
 <tr>
 <td></td>
 <td colspan="2">Supported Version Ranges</td>
 </tr>
 <tr>
 <td>draco15</td>
 <td><code class="docutils literal notranslate">v7.4.0 -> v7.4.1 </code></td>
 <td><code class="docutils literal notranslate">v7.4.3 -> 7.6.4 </code></td>
 </tr>
 <tr>
 <td>[enable]</td>
 <td><code class="docutils literal notranslate">v7.4.0 -> v7.4.1</code></td>
 <tr>
 <td>[disable]</td>
 <td><code class="docutils literal notranslate">v7.4.0 -> v7.4.1</code></td>
 </table>
 </div>
 </li>
            <li> <span class="li-head">tcp_udp_port</span> - Include/exclude TCP/UDP source and destination port for unicast trunk traffic. <span class="li-normal">type: str</span> <span class="li-normal">choices: include, exclude</span>
 <a id='label912' href="javascript:ContentClick('label913', 'label912');" onmouseover="ContentPreview('label913');" onmouseout="ContentUnpreview('label913');" title="click to collapse or expand..."> more... </a>
 <div id="label913" style="display:none">
 <table border="1">
 <tr>
 <td></td>
 <td colspan="2">Supported Version Ranges</td>
 </tr>
 <tr>
 <td>tcp_udp_port</td>
 <td><code class="docutils literal notranslate">v7.4.0 -> v7.4.1 </code></td>
 <td><code class="docutils literal notranslate">v7.4.3 -> 7.6.4 </code></td>
 </tr>
 <tr>
 <td>[include]</td>
 <td><code class="docutils literal notranslate">v7.4.0 -> v7.4.1</code></td>
 <tr>
 <td>[exclude]</td>
 <td><code class="docutils literal notranslate">v7.4.0 -> v7.4.1</code></td>
 </table>
 </div>
 </li>
            </ul>
        <li> <span class="li-head">tunnel_over_vlink</span> - Enable/disable selection of which NP6 chip the tunnel uses . <span class="li-normal">type: str</span> <span class="li-normal">choices: enable, disable</span>
 <a id='label914' href="javascript:ContentClick('label915', 'label914');" onmouseover="ContentPreview('label915');" onmouseout="ContentUnpreview('label915');" title="click to collapse or expand..."> more... </a>
 <div id="label915" style="display:none">
 <table border="1">
 <tr>
 <td></td>
 <td colspan="1">Supported Version Ranges</td>
 </tr>
 <tr>
 <td>tunnel_over_vlink</td>
 <td><code class="docutils literal notranslate">v7.4.4 -> 7.6.4 </code></td>
 </tr>
 <tr>
 <td>[enable]</td>
 <td><code class="docutils literal notranslate">v7.4.4 -> 7.6.4</code></td>
 <tr>
 <td>[disable]</td>
 <td><code class="docutils literal notranslate">v7.4.4 -> 7.6.4</code></td>
 </table>
 </div>
 </li>
        <li> <span class="li-head">uesp_offload</span> - Enable/disable UDP-encapsulated ESP offload . <span class="li-normal">type: str</span> <span class="li-normal">choices: enable, disable</span>
 <a id='label916' href="javascript:ContentClick('label917', 'label916');" onmouseover="ContentPreview('label917');" onmouseout="ContentUnpreview('label917');" title="click to collapse or expand..."> more... </a>
 <div id="label917" style="display:none">
 <table border="1">
 <tr>
 <td></td>
 <td colspan="2">Supported Version Ranges</td>
 </tr>
 <tr>
 <td>uesp_offload</td>
 <td><code class="docutils literal notranslate">v7.0.0 -> v7.4.1 </code></td>
 <td><code class="docutils literal notranslate">v7.4.3 -> 7.6.4 </code></td>
 </tr>
 <tr>
 <td>[enable]</td>
 <td><code class="docutils literal notranslate">v7.0.0 -> v7.4.1</code></td>
 <tr>
 <td>[disable]</td>
 <td><code class="docutils literal notranslate">v7.0.0 -> v7.4.1</code></td>
 </table>
 </div>
 </li>
        <li> <span class="li-head">ull_port_mode</span> - Set ULL port"s speed to 10G/25G . <span class="li-normal">type: str</span> <span class="li-normal">choices: 10G, 25G</span>
 <a id='label918' href="javascript:ContentClick('label919', 'label918');" onmouseover="ContentPreview('label919');" onmouseout="ContentUnpreview('label919');" title="click to collapse or expand..."> more... </a>
 <div id="label919" style="display:none">
 <table border="1">
 <tr>
 <td></td>
 <td colspan="1">Supported Version Ranges</td>
 </tr>
 <tr>
 <td>ull_port_mode</td>
 <td><code class="docutils literal notranslate">v7.4.2 -> v7.4.2 </code></td>
 </tr>
 <tr>
 <td>[10G]</td>
 <td><code class="docutils literal notranslate">v7.4.2 -> v7.4.2</code></td>
 <tr>
 <td>[25G]</td>
 <td><code class="docutils literal notranslate">v7.4.2 -> v7.4.2</code></td>
 </table>
 </div>
 </li>
        <li> <span class="li-head">vlan_lookup_cache</span> - Enable/disable vlan lookup cache . <span class="li-normal">type: str</span> <span class="li-normal">choices: enable, disable</span>
 <a id='label920' href="javascript:ContentClick('label921', 'label920');" onmouseover="ContentPreview('label921');" onmouseout="ContentUnpreview('label921');" title="click to collapse or expand..."> more... </a>
 <div id="label921" style="display:none">
 <table border="1">
 <tr>
 <td></td>
 <td colspan="1">Supported Version Ranges</td>
 </tr>
 <tr>
 <td>vlan_lookup_cache</td>
 <td><code class="docutils literal notranslate">v7.4.2 -> v7.4.2 </code></td>
 </tr>
 <tr>
 <td>[enable]</td>
 <td><code class="docutils literal notranslate">v7.4.2 -> v7.4.2</code></td>
 <tr>
 <td>[disable]</td>
 <td><code class="docutils literal notranslate">v7.4.2 -> v7.4.2</code></td>
 </table>
 </div>
 </li>
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
    
    - name: Configure NPU attributes.
      fortinet.fortios.fortios_system_npu:
          vdom: "{{ vdom }}"
          system_npu:
              capwap_offload: "enable"
              dedicated_management_affinity: "<your_own_value>"
              dedicated_management_cpu: "enable"
              default_qos_type: "policing"
              dos_options:
                  npu_dos_meter_mode: "global"
                  npu_dos_tpe_mode: "enable"
              double_level_mcast_offload: "enable"
              dsw_dts_profile:
                  -
                      action: "wait"
                      min_limit: "0"
                      profile_id: "<you_own_value>"
                      step: "0"
              dsw_queue_dts_profile:
                  -
                      iport: "eif0"
                      name: "default_name_18"
                      oport: "eif0"
                      profile_id: "0"
                      queue_select: "0"
              fastpath: "disable"
              fp_anomaly:
                  icmp_csum_err: "drop"
                  icmp_frag: "allow"
                  icmp_land: "allow"
                  ipv4_csum_err: "drop"
                  ipv4_land: "allow"
                  ipv4_optlsrr: "allow"
                  ipv4_optrr: "allow"
                  ipv4_optsecurity: "allow"
                  ipv4_optssrr: "allow"
                  ipv4_optstream: "allow"
                  ipv4_opttimestamp: "allow"
                  ipv4_proto_err: "allow"
                  ipv4_unknopt: "allow"
                  ipv6_daddr_err: "allow"
                  ipv6_land: "allow"
                  ipv6_optendpid: "allow"
                  ipv6_opthomeaddr: "allow"
                  ipv6_optinvld: "allow"
                  ipv6_optjumbo: "allow"
                  ipv6_optnsap: "allow"
                  ipv6_optralert: "allow"
                  ipv6_opttunnel: "allow"
                  ipv6_proto_err: "allow"
                  ipv6_saddr_err: "allow"
                  ipv6_unknopt: "allow"
                  tcp_csum_err: "drop"
                  tcp_fin_noack: "allow"
                  tcp_fin_only: "allow"
                  tcp_land: "allow"
                  tcp_no_flag: "allow"
                  tcp_syn_data: "allow"
                  tcp_syn_fin: "allow"
                  tcp_winnuke: "allow"
                  udp_csum_err: "drop"
                  udp_land: "allow"
              gtp_enhanced_cpu_range: "0"
              gtp_enhanced_mode: "enable"
              gtp_support: "enable"
              hash_tbl_spread: "enable"
              hpe:
                  all_protocol: "400000"
                  arp_max: "5000"
                  enable_shaper: "disable"
                  esp_max: "5000"
                  high_priority: "400000"
                  icmp_max: "5000"
                  ip_frag_max: "5000"
                  ip_others_max: "5000"
                  l2_others_max: "5000"
                  sctp_max: "5000"
                  tcp_max: "40000"
                  tcpfin_rst_max: "40000"
                  tcpsyn_ack_max: "40000"
                  tcpsyn_max: "40000"
                  udp_max: "40000"
              htab_dedi_queue_nr: "4"
              htab_msg_queue: "data"
              htx_icmp_csum_chk: "drop"
              inbound_dscp_copy_port:
                  -
                      interface: "<your_own_value>"
              intf_shaping_offload: "enable"
              ip_fragment_offload: "disable"
              ip_reassembly:
                  max_timeout: "200000"
                  min_timeout: "64"
                  status: "disable"
              ipsec_dec_subengine_mask: "<your_own_value>"
              ipsec_enc_subengine_mask: "<your_own_value>"
              ipsec_inbound_cache: "enable"
              ipsec_mtu_override: "disable"
              ipsec_ob_np_sel: "rr"
              ipsec_over_vlink: "enable"
              isf_np_queues:
                  cos0: "<your_own_value> (source system.isf-queue-profile.name)"
                  cos1: "<your_own_value> (source system.isf-queue-profile.name)"
                  cos2: "<your_own_value> (source system.isf-queue-profile.name)"
                  cos3: "<your_own_value> (source system.isf-queue-profile.name)"
                  cos4: "<your_own_value> (source system.isf-queue-profile.name)"
                  cos5: "<your_own_value> (source system.isf-queue-profile.name)"
                  cos6: "<your_own_value> (source system.isf-queue-profile.name)"
                  cos7: "<your_own_value> (source system.isf-queue-profile.name)"
              lag_out_port_select: "disable"
              max_receive_unit: "0"
              max_session_timeout: "40"
              mcast_session_accounting: "tpe-based"
              napi_break_interval: "0"
              np_queues:
                  ethernet_type:
                      -
                          name: "default_name_112"
                          queue: "0"
                          type: "<your_own_value>"
                          weight: "15"
                  ip_protocol:
                      -
                          name: "default_name_117"
                          protocol: "0"
                          queue: "0"
                          weight: "14"
                  ip_service:
                      -
                          dport: "0"
                          name: "default_name_123"
                          protocol: "0"
                          queue: "0"
                          sport: "0"
                          weight: "13"
                  profile:
                      -
                          cos0: "queue0"
                          cos1: "queue0"
                          cos2: "queue0"
                          cos3: "queue0"
                          cos4: "queue0"
                          cos5: "queue0"
                          cos6: "queue0"
                          cos7: "queue0"
                          dscp0: "queue0"
                          dscp1: "queue0"
                          dscp10: "queue0"
                          dscp11: "queue0"
                          dscp12: "queue0"
                          dscp13: "queue0"
                          dscp14: "queue0"
                          dscp15: "queue0"
                          dscp16: "queue0"
                          dscp17: "queue0"
                          dscp18: "queue0"
                          dscp19: "queue0"
                          dscp2: "queue0"
                          dscp20: "queue0"
                          dscp21: "queue0"
                          dscp22: "queue0"
                          dscp23: "queue0"
                          dscp24: "queue0"
                          dscp25: "queue0"
                          dscp26: "queue0"
                          dscp27: "queue0"
                          dscp28: "queue0"
                          dscp29: "queue0"
                          dscp3: "queue0"
                          dscp30: "queue0"
                          dscp31: "queue0"
                          dscp32: "queue0"
                          dscp33: "queue0"
                          dscp34: "queue0"
                          dscp35: "queue0"
                          dscp36: "queue0"
                          dscp37: "queue0"
                          dscp38: "queue0"
                          dscp39: "queue0"
                          dscp4: "queue0"
                          dscp40: "queue0"
                          dscp41: "queue0"
                          dscp42: "queue0"
                          dscp43: "queue0"
                          dscp44: "queue0"
                          dscp45: "queue0"
                          dscp46: "queue0"
                          dscp47: "queue0"
                          dscp48: "queue0"
                          dscp49: "queue0"
                          dscp5: "queue0"
                          dscp50: "queue0"
                          dscp51: "queue0"
                          dscp52: "queue0"
                          dscp53: "queue0"
                          dscp54: "queue0"
                          dscp55: "queue0"
                          dscp56: "queue0"
                          dscp57: "queue0"
                          dscp58: "queue0"
                          dscp59: "queue0"
                          dscp6: "queue0"
                          dscp60: "queue0"
                          dscp61: "queue0"
                          dscp62: "queue0"
                          dscp63: "queue0"
                          dscp7: "queue0"
                          dscp8: "queue0"
                          dscp9: "queue0"
                          id: "201"
                          type: "cos"
                          weight: "6"
                  scheduler:
                      -
                          mode: "none"
                          name: "default_name_206"
              npu_group_effective_scope: "255"
              npu_tcam:
                  -
                      data:
                          df: "enable"
                          dstip: "<your_own_value>"
                          dstipv6: "<your_own_value>"
                          dstmac: "<your_own_value>"
                          dstport: "0"
                          ethertype: "<your_own_value>"
                          ext_tag: "enable"
                          frag_off: "0"
                          gen_buf_cnt: "0"
                          gen_iv: "valid"
                          gen_l3_flags: "0"
                          gen_l4_flags: "0"
                          gen_pkt_ctrl: "0"
                          gen_pri: "0"
                          gen_pri_v: "valid"
                          gen_tv: "valid"
                          ihl: "0"
                          ip4_id: "0"
                          ip6_fl: "0"
                          ipver: "0"
                          l4_wd10: "0"
                          l4_wd11: "0"
                          l4_wd8: "0"
                          l4_wd9: "0"
                          mf: "enable"
                          protocol: "0"
                          slink: "0"
                          smac_change: "enable"
                          sp: "0"
                          src_cfi: "enable"
                          src_prio: "0"
                          src_updt: "enable"
                          srcip: "<your_own_value>"
                          srcipv6: "<your_own_value>"
                          srcmac: "<your_own_value>"
                          srcport: "0"
                          svid: "0"
                          tcp_ack: "enable"
                          tcp_cwr: "enable"
                          tcp_ece: "enable"
                          tcp_fin: "enable"
                          tcp_push: "enable"
                          tcp_rst: "enable"
                          tcp_syn: "enable"
                          tcp_urg: "enable"
                          tgt_cfi: "enable"
                          tgt_prio: "0"
                          tgt_updt: "enable"
                          tgt_v: "valid"
                          tos: "0"
                          tp: "0"
                          ttl: "0"
                          tvid: "0"
                          vdid: "0"
                      mask:
                          df: "enable"
                          dstip: "<your_own_value>"
                          dstipv6: "<your_own_value>"
                          dstmac: "<your_own_value>"
                          dstport: "0"
                          ethertype: "<your_own_value>"
                          ext_tag: "enable"
                          frag_off: "0"
                          gen_buf_cnt: "0"
                          gen_iv: "valid"
                          gen_l3_flags: "0"
                          gen_l4_flags: "0"
                          gen_pkt_ctrl: "0"
                          gen_pri: "0"
                          gen_pri_v: "valid"
                          gen_tv: "valid"
                          ihl: "0"
                          ip4_id: "0"
                          ip6_fl: "0"
                          ipver: "0"
                          l4_wd10: "0"
                          l4_wd11: "0"
                          l4_wd8: "0"
                          l4_wd9: "0"
                          mf: "enable"
                          protocol: "0"
                          slink: "0"
                          smac_change: "enable"
                          sp: "0"
                          src_cfi: "enable"
                          src_prio: "0"
                          src_updt: "enable"
                          srcip: "<your_own_value>"
                          srcipv6: "<your_own_value>"
                          srcmac: "<your_own_value>"
                          srcport: "0"
                          svid: "0"
                          tcp_ack: "enable"
                          tcp_cwr: "enable"
                          tcp_ece: "enable"
                          tcp_fin: "enable"
                          tcp_push: "enable"
                          tcp_rst: "enable"
                          tcp_syn: "enable"
                          tcp_urg: "enable"
                          tgt_cfi: "enable"
                          tgt_prio: "0"
                          tgt_updt: "enable"
                          tgt_v: "valid"
                          tos: "0"
                          tp: "0"
                          ttl: "0"
                          tvid: "0"
                          vdid: "0"
                      mir_act:
                          vlif: "0"
                      name: "default_name_321"
                      oid: "0"
                      pri_act:
                          priority: "0"
                          weight: "0"
                      sact:
                          act: "0"
                          act_v: "enable"
                          bmproc: "0"
                          bmproc_v: "enable"
                          df_lif: "0"
                          df_lif_v: "enable"
                          dfr: "0"
                          dfr_v: "enable"
                          dmac_skip: "0"
                          dmac_skip_v: "enable"
                          dosen: "0"
                          dosen_v: "enable"
                          espff_proc: "0"
                          espff_proc_v: "enable"
                          etype_pid: "0"
                          etype_pid_v: "enable"
                          frag_proc: "0"
                          frag_proc_v: "enable"
                          fwd: "0"
                          fwd_lif: "0"
                          fwd_lif_v: "enable"
                          fwd_tvid: "0"
                          fwd_tvid_v: "enable"
                          fwd_v: "enable"
                          icpen: "0"
                          icpen_v: "enable"
                          igmp_mld_snp: "0"
                          igmp_mld_snp_v: "enable"
                          learn: "0"
                          learn_v: "enable"
                          m_srh_ctrl: "0"
                          m_srh_ctrl_v: "enable"
                          mac_id: "0"
                          mac_id_v: "enable"
                          mss: "0"
                          mss_v: "enable"
                          pleen: "0"
                          pleen_v: "enable"
                          prio_pid: "0"
                          prio_pid_v: "enable"
                          promis: "0"
                          promis_v: "enable"
                          rfsh: "0"
                          rfsh_v: "enable"
                          smac_skip: "0"
                          smac_skip_v: "enable"
                          tp_smchk: "0"
                          tp_smchk_v: "enable"
                          tpe_id: "0"
                          tpe_id_v: "enable"
                          vdm: "0"
                          vdm_v: "enable"
                          vdom_id: "0"
                          vdom_id_v: "enable"
                          x_mode: "0"
                          x_mode_v: "enable"
                      tact:
                          act: "0"
                          act_v: "enable"
                          fmtuv4_s: "0"
                          fmtuv4_s_v: "enable"
                          fmtuv6_s: "0"
                          fmtuv6_s_v: "enable"
                          lnkid: "0"
                          lnkid_v: "enable"
                          mac_id: "0"
                          mac_id_v: "enable"
                          mss_t: "0"
                          mss_t_v: "enable"
                          mtuv4: "0"
                          mtuv4_v: "enable"
                          mtuv6: "0"
                          mtuv6_v: "enable"
                          slif_act: "0"
                          slif_act_v: "enable"
                          sublnkid: "0"
                          sublnkid_v: "enable"
                          tgtv_act: "0"
                          tgtv_act_v: "enable"
                          tlif_act: "0"
                          tlif_act_v: "enable"
                          tpeid: "0"
                          tpeid_v: "enable"
                          v6fe: "0"
                          v6fe_v: "enable"
                          vep_en: "0"
                          vep_en_v: "enable"
                          vep_slid: "0"
                          vep_slid_v: "enable"
                          xlt_lif: "0"
                          xlt_lif_v: "enable"
                          xlt_vid: "0"
                          xlt_vid_v: "enable"
                      type: "L2_src_tc"
                      vid: "0"
              per_session_accounting: "traffic-log-only"
              port_cpu_map:
                  -
                      cpu_core: "<your_own_value>"
                      interface: "<your_own_value>"
              port_npu_map:
                  -
                      interface: "<your_own_value>"
                      npu_group_index: "0"
              port_path_option:
                  ports_using_npu:
                      -
                          interface_name: "<your_own_value>"
              priority_protocol:
                  bfd: "enable"
                  bgp: "enable"
                  slbc: "enable"
              qos_mode: "disable"
              qtm_buf_mode: "6ch"
              rdp_offload: "enable"
              session_acct_interval: "5"
              session_denied_offload: "disable"
              shaping_stats: "disable"
              sse_backpressure: "enable"
              strip_clear_text_padding: "enable"
              strip_esp_padding: "enable"
              sw_eh_hash:
                  computation: "xor16"
                  destination_ip_lower_16: "include"
                  destination_ip_upper_16: "include"
                  destination_port: "include"
                  ip_protocol: "include"
                  netmask_length: "32"
                  source_ip_lower_16: "include"
                  source_ip_upper_16: "include"
                  source_port: "include"
              sw_np_bandwidth: "0G"
              sw_tr_hash:
                  draco15: "enable"
                  tcp_udp_port: "include"
              tunnel_over_vlink: "enable"
              uesp_offload: "enable"
              ull_port_mode: "10G"
              vlan_lookup_cache: "enable"


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
