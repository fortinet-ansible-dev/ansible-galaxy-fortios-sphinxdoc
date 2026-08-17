:source: fortios_router_multicast6.py

:orphan:

.. fortios_router_multicast6:

fortios_router_multicast6 -- Configure IPv6 multicast in Fortinet's FortiOS and FortiGate.
++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++

.. versionadded:: 2.0.0

.. contents::
   :local:
   :depth: 1


Synopsis
--------
- This module is able to configure a FortiGate or FortiOS (FOS) device by allowing the user to set and modify router feature and multicast6 category. Examples include all parameters and values need to be adjusted to datasources before usage. Tested with FOS v6.0.0



Requirements
------------
The below requirements are needed on the host that executes this module.

- ansible>=2.16


Tips
----
Using member operation to add an element to an existing object.

FortiOS Version Compatibility
-----------------------------
Supported Version Ranges: v6.0.0 -> v8.0.0


Parameters
----------


.. raw:: html

    <ul>
    <li> <span class="li-head">access_token</span> - Token-based authentication. Generated from GUI of Fortigate. <span class="li-normal">type: str</span> <span class="li-required">required: false</span> </li>
    <li> <span class="li-head">enable_log</span> - Enable/Disable logging for task. <span class="li-normal">type: bool</span> <span class="li-required">required: false</span> <span class="li-normal">default: False</span> </li>
    <li> <span class="li-head">vdom</span> - Virtual domain, among those defined previously. A vdom is a virtual instance of the FortiGate that can be configured and used as a different unit. <span class="li-normal">type: str</span> <span class="li-normal">default: root</span> </li>
    <li> <span class="li-head">member_path</span> - Member attribute path to operate on. <span class="li-normal">type: str</span> </li>
    <li> <span class="li-head">member_state</span> - Add or delete a member under specified attribute path. <span class="li-normal">type: str</span> <span class="li-normal">choices: present, absent</span> </li>
    <li> <span class="li-head">router_multicast6</span> - Configure IPv6 multicast. <span class="li-normal">type: dict</span>
 <a id='label0' href="javascript:ContentClick('label1', 'label0');" onmouseover="ContentPreview('label1');" onmouseout="ContentUnpreview('label1');" title="click to collapse or expand..."> more... </a>
 <div id="label1" style="display:none">
 <table border="1">
 <tr>
 <td></td><td colspan="1">Supported Version Ranges</td>
 </tr>
 <tr>
 <td>router_multicast6</td>
 <td><code class="docutils literal notranslate">v6.0.0 -> 8.0.0 </code></td>
 </tr>
 </table>
 </div>
 </li>
        <ul class="ul-self">
        <li> <span class="li-head">interface</span> - Protocol Independent Multicast (PIM) interfaces. <span class="li-normal">type: list</span> <span style="font-family:'Courier New'" class="li-required">member_path: interface:name</span>
 <a id='label2' href="javascript:ContentClick('label3', 'label2');" onmouseover="ContentPreview('label3');" onmouseout="ContentUnpreview('label3');" title="click to collapse or expand..."> more... </a>
 <div id="label3" style="display:none">
 <table border="1">
 <tr>
 <td></td><td colspan="1">Supported Version Ranges</td>
 </tr>
 <tr>
 <td>interface</td>
 <td><code class="docutils literal notranslate">v6.0.0 -> 8.0.0 </code></td>
 </tr>
 </table>
 </div>
 </li>
            <ul class="ul-self">
            <li> <span class="li-head">hello_holdtime</span> - Time before old neighbor information expires in seconds (1 - 65535). <span class="li-normal">type: int</span>
 <a id='label4' href="javascript:ContentClick('label5', 'label4');" onmouseover="ContentPreview('label5');" onmouseout="ContentUnpreview('label5');" title="click to collapse or expand..."> more... </a>
 <div id="label5" style="display:none">
 <table border="1">
 <tr>
 <td></td>
 <td colspan="1">Supported Version Ranges</td>
 </tr>
 <tr>
 <td>hello_holdtime</td>
 <td><code class="docutils literal notranslate">v6.0.0 -> 8.0.0 </code></td>
 </tr>
 </table>
 </div>
 </li>
            <li> <span class="li-head">hello_interval</span> - Interval between sending PIM hello messages in seconds (1 - 65535). <span class="li-normal">type: int</span>
 <a id='label6' href="javascript:ContentClick('label7', 'label6');" onmouseover="ContentPreview('label7');" onmouseout="ContentUnpreview('label7');" title="click to collapse or expand..."> more... </a>
 <div id="label7" style="display:none">
 <table border="1">
 <tr>
 <td></td>
 <td colspan="1">Supported Version Ranges</td>
 </tr>
 <tr>
 <td>hello_interval</td>
 <td><code class="docutils literal notranslate">v6.0.0 -> 8.0.0 </code></td>
 </tr>
 </table>
 </div>
 </li>
            <li> <span class="li-head">name</span> - Interface name. Source system.interface.name. <span class="li-normal">type: str</span> <span class="li-required">required: true</span>
 <a id='label8' href="javascript:ContentClick('label9', 'label8');" onmouseover="ContentPreview('label9');" onmouseout="ContentUnpreview('label9');" title="click to collapse or expand..."> more... </a>
 <div id="label9" style="display:none">
 <table border="1">
 <tr>
 <td></td>
 <td colspan="1">Supported Version Ranges</td>
 </tr>
 <tr>
 <td>name</td>
 <td><code class="docutils literal notranslate">v6.0.0 -> 8.0.0 </code></td>
 </tr>
 </table>
 </div>
 </li>
            <li> <span class="li-head">rp_candidate</span> - Enable/disable compete to become RP in elections. <span class="li-normal">type: str</span> <span class="li-normal">choices: enable, disable</span>
 <a id='label10' href="javascript:ContentClick('label11', 'label10');" onmouseover="ContentPreview('label11');" onmouseout="ContentUnpreview('label11');" title="click to collapse or expand..."> more... </a>
 <div id="label11" style="display:none">
 <table border="1">
 <tr>
 <td></td>
 <td colspan="1">Supported Version Ranges</td>
 </tr>
 <tr>
 <td>rp_candidate</td>
 <td><code class="docutils literal notranslate">v8.0.0 -> 8.0.0 </code></td>
 </tr>
 <tr>
 <td>[enable]</td>
 <td><code class="docutils literal notranslate">v8.0.0 -> 8.0.0</code></td>
 <tr>
 <td>[disable]</td>
 <td><code class="docutils literal notranslate">v8.0.0 -> 8.0.0</code></td>
 </table>
 </div>
 </li>
            <li> <span class="li-head">rp_candidate_group</span> - Multicast groups managed by this RP. Source router.access-list6.name. <span class="li-normal">type: str</span>
 <a id='label12' href="javascript:ContentClick('label13', 'label12');" onmouseover="ContentPreview('label13');" onmouseout="ContentUnpreview('label13');" title="click to collapse or expand..."> more... </a>
 <div id="label13" style="display:none">
 <table border="1">
 <tr>
 <td></td>
 <td colspan="1">Supported Version Ranges</td>
 </tr>
 <tr>
 <td>rp_candidate_group</td>
 <td><code class="docutils literal notranslate">v8.0.0 -> 8.0.0 </code></td>
 </tr>
 </table>
 </div>
 </li>
            <li> <span class="li-head">rp_candidate_interval</span> - RP candidate advertisement interval (1 - 16383 sec). <span class="li-normal">type: int</span>
 <a id='label14' href="javascript:ContentClick('label15', 'label14');" onmouseover="ContentPreview('label15');" onmouseout="ContentUnpreview('label15');" title="click to collapse or expand..."> more... </a>
 <div id="label15" style="display:none">
 <table border="1">
 <tr>
 <td></td>
 <td colspan="1">Supported Version Ranges</td>
 </tr>
 <tr>
 <td>rp_candidate_interval</td>
 <td><code class="docutils literal notranslate">v8.0.0 -> 8.0.0 </code></td>
 </tr>
 </table>
 </div>
 </li>
            <li> <span class="li-head">rp_candidate_priority</span> - Router"s priority as RP. <span class="li-normal">type: int</span>
 <a id='label16' href="javascript:ContentClick('label17', 'label16');" onmouseover="ContentPreview('label17');" onmouseout="ContentUnpreview('label17');" title="click to collapse or expand..."> more... </a>
 <div id="label17" style="display:none">
 <table border="1">
 <tr>
 <td></td>
 <td colspan="1">Supported Version Ranges</td>
 </tr>
 <tr>
 <td>rp_candidate_priority</td>
 <td><code class="docutils literal notranslate">v8.0.0 -> 8.0.0 </code></td>
 </tr>
 </table>
 </div>
 </li>
            <li> <span class="li-head">static_group</span> - Statically set IPv6 multicast groups to forward out. Source router.multicast6-flow.name. <span class="li-normal">type: str</span>
 <a id='label18' href="javascript:ContentClick('label19', 'label18');" onmouseover="ContentPreview('label19');" onmouseout="ContentUnpreview('label19');" title="click to collapse or expand..."> more... </a>
 <div id="label19" style="display:none">
 <table border="1">
 <tr>
 <td></td>
 <td colspan="1">Supported Version Ranges</td>
 </tr>
 <tr>
 <td>static_group</td>
 <td><code class="docutils literal notranslate">v8.0.0 -> 8.0.0 </code></td>
 </tr>
 </table>
 </div>
 </li>
            </ul>
        <li> <span class="li-head">multicast_pmtu</span> - Enable/disable PMTU for IPv6 multicast. <span class="li-normal">type: str</span> <span class="li-normal">choices: enable, disable</span>
 <a id='label20' href="javascript:ContentClick('label21', 'label20');" onmouseover="ContentPreview('label21');" onmouseout="ContentUnpreview('label21');" title="click to collapse or expand..."> more... </a>
 <div id="label21" style="display:none">
 <table border="1">
 <tr>
 <td></td>
 <td colspan="1">Supported Version Ranges</td>
 </tr>
 <tr>
 <td>multicast_pmtu</td>
 <td><code class="docutils literal notranslate">v6.0.0 -> 8.0.0 </code></td>
 </tr>
 <tr>
 <td>[enable]</td>
 <td><code class="docutils literal notranslate">v6.0.0 -> 8.0.0</code></td>
 <tr>
 <td>[disable]</td>
 <td><code class="docutils literal notranslate">v6.0.0 -> 8.0.0</code></td>
 </table>
 </div>
 </li>
        <li> <span class="li-head">multicast_routing</span> - Enable/disable IPv6 multicast routing. <span class="li-normal">type: str</span> <span class="li-normal">choices: enable, disable</span>
 <a id='label22' href="javascript:ContentClick('label23', 'label22');" onmouseover="ContentPreview('label23');" onmouseout="ContentUnpreview('label23');" title="click to collapse or expand..."> more... </a>
 <div id="label23" style="display:none">
 <table border="1">
 <tr>
 <td></td>
 <td colspan="1">Supported Version Ranges</td>
 </tr>
 <tr>
 <td>multicast_routing</td>
 <td><code class="docutils literal notranslate">v6.0.0 -> 8.0.0 </code></td>
 </tr>
 <tr>
 <td>[enable]</td>
 <td><code class="docutils literal notranslate">v6.0.0 -> 8.0.0</code></td>
 <tr>
 <td>[disable]</td>
 <td><code class="docutils literal notranslate">v6.0.0 -> 8.0.0</code></td>
 </table>
 </div>
 </li>
        <li> <span class="li-head">pim_sm_global</span> - PIM sparse-mode global settings. <span class="li-normal">type: dict</span>
 <a id='label24' href="javascript:ContentClick('label25', 'label24');" onmouseover="ContentPreview('label25');" onmouseout="ContentUnpreview('label25');" title="click to collapse or expand..."> more... </a>
 <div id="label25" style="display:none">
 <table border="1">
 <tr>
 <td></td><td colspan="1">Supported Version Ranges</td>
 </tr>
 <tr>
 <td>pim_sm_global</td>
 <td><code class="docutils literal notranslate">v6.0.0 -> 8.0.0 </code></td>
 </tr>
 </table>
 </div>
 </li>
            <ul class="ul-self">
            <li> <span class="li-head">bsr_allow_quick_refresh</span> - Enable/disable accept BSR quick refresh packets from neighbors. <span class="li-normal">type: str</span> <span class="li-normal">choices: enable, disable</span>
 <a id='label26' href="javascript:ContentClick('label27', 'label26');" onmouseover="ContentPreview('label27');" onmouseout="ContentUnpreview('label27');" title="click to collapse or expand..."> more... </a>
 <div id="label27" style="display:none">
 <table border="1">
 <tr>
 <td></td>
 <td colspan="1">Supported Version Ranges</td>
 </tr>
 <tr>
 <td>bsr_allow_quick_refresh</td>
 <td><code class="docutils literal notranslate">v8.0.0 -> 8.0.0 </code></td>
 </tr>
 <tr>
 <td>[enable]</td>
 <td><code class="docutils literal notranslate">v8.0.0 -> 8.0.0</code></td>
 <tr>
 <td>[disable]</td>
 <td><code class="docutils literal notranslate">v8.0.0 -> 8.0.0</code></td>
 </table>
 </div>
 </li>
            <li> <span class="li-head">bsr_candidate</span> - Enable/disable allowing this router to become a bootstrap router (BSR). <span class="li-normal">type: str</span> <span class="li-normal">choices: enable, disable</span>
 <a id='label28' href="javascript:ContentClick('label29', 'label28');" onmouseover="ContentPreview('label29');" onmouseout="ContentUnpreview('label29');" title="click to collapse or expand..."> more... </a>
 <div id="label29" style="display:none">
 <table border="1">
 <tr>
 <td></td>
 <td colspan="1">Supported Version Ranges</td>
 </tr>
 <tr>
 <td>bsr_candidate</td>
 <td><code class="docutils literal notranslate">v8.0.0 -> 8.0.0 </code></td>
 </tr>
 <tr>
 <td>[enable]</td>
 <td><code class="docutils literal notranslate">v8.0.0 -> 8.0.0</code></td>
 <tr>
 <td>[disable]</td>
 <td><code class="docutils literal notranslate">v8.0.0 -> 8.0.0</code></td>
 </table>
 </div>
 </li>
            <li> <span class="li-head">bsr_hash</span> - BSR hash length (0 - 128). <span class="li-normal">type: int</span>
 <a id='label30' href="javascript:ContentClick('label31', 'label30');" onmouseover="ContentPreview('label31');" onmouseout="ContentUnpreview('label31');" title="click to collapse or expand..."> more... </a>
 <div id="label31" style="display:none">
 <table border="1">
 <tr>
 <td></td>
 <td colspan="1">Supported Version Ranges</td>
 </tr>
 <tr>
 <td>bsr_hash</td>
 <td><code class="docutils literal notranslate">v8.0.0 -> 8.0.0 </code></td>
 </tr>
 </table>
 </div>
 </li>
            <li> <span class="li-head">bsr_interface</span> - Interface to advertise as candidate BSR. Source system.interface.name. <span class="li-normal">type: str</span>
 <a id='label32' href="javascript:ContentClick('label33', 'label32');" onmouseover="ContentPreview('label33');" onmouseout="ContentUnpreview('label33');" title="click to collapse or expand..."> more... </a>
 <div id="label33" style="display:none">
 <table border="1">
 <tr>
 <td></td>
 <td colspan="1">Supported Version Ranges</td>
 </tr>
 <tr>
 <td>bsr_interface</td>
 <td><code class="docutils literal notranslate">v8.0.0 -> 8.0.0 </code></td>
 </tr>
 </table>
 </div>
 </li>
            <li> <span class="li-head">bsr_priority</span> - BSR priority (0 - 255). <span class="li-normal">type: int</span>
 <a id='label34' href="javascript:ContentClick('label35', 'label34');" onmouseover="ContentPreview('label35');" onmouseout="ContentUnpreview('label35');" title="click to collapse or expand..."> more... </a>
 <div id="label35" style="display:none">
 <table border="1">
 <tr>
 <td></td>
 <td colspan="1">Supported Version Ranges</td>
 </tr>
 <tr>
 <td>bsr_priority</td>
 <td><code class="docutils literal notranslate">v8.0.0 -> 8.0.0 </code></td>
 </tr>
 </table>
 </div>
 </li>
            <li> <span class="li-head">cisco_crp_prefix</span> - Enable/disable making candidate RP compatible with old Cisco IOS. <span class="li-normal">type: str</span> <span class="li-normal">choices: enable, disable</span>
 <a id='label36' href="javascript:ContentClick('label37', 'label36');" onmouseover="ContentPreview('label37');" onmouseout="ContentUnpreview('label37');" title="click to collapse or expand..."> more... </a>
 <div id="label37" style="display:none">
 <table border="1">
 <tr>
 <td></td>
 <td colspan="1">Supported Version Ranges</td>
 </tr>
 <tr>
 <td>cisco_crp_prefix</td>
 <td><code class="docutils literal notranslate">v8.0.0 -> 8.0.0 </code></td>
 </tr>
 <tr>
 <td>[enable]</td>
 <td><code class="docutils literal notranslate">v8.0.0 -> 8.0.0</code></td>
 <tr>
 <td>[disable]</td>
 <td><code class="docutils literal notranslate">v8.0.0 -> 8.0.0</code></td>
 </table>
 </div>
 </li>
            <li> <span class="li-head">cisco_ignore_rp_set_priority</span> - Use only hash for RP selection (compatibility with old Cisco IOS). <span class="li-normal">type: str</span> <span class="li-normal">choices: enable, disable</span>
 <a id='label38' href="javascript:ContentClick('label39', 'label38');" onmouseover="ContentPreview('label39');" onmouseout="ContentUnpreview('label39');" title="click to collapse or expand..."> more... </a>
 <div id="label39" style="display:none">
 <table border="1">
 <tr>
 <td></td>
 <td colspan="1">Supported Version Ranges</td>
 </tr>
 <tr>
 <td>cisco_ignore_rp_set_priority</td>
 <td><code class="docutils literal notranslate">v8.0.0 -> 8.0.0 </code></td>
 </tr>
 <tr>
 <td>[enable]</td>
 <td><code class="docutils literal notranslate">v8.0.0 -> 8.0.0</code></td>
 <tr>
 <td>[disable]</td>
 <td><code class="docutils literal notranslate">v8.0.0 -> 8.0.0</code></td>
 </table>
 </div>
 </li>
            <li> <span class="li-head">pim_use_sdwan</span> - Enable/disable use of SDWAN when checking RPF neighbor and sending of REG packet. <span class="li-normal">type: str</span> <span class="li-normal">choices: enable, disable</span>
 <a id='label40' href="javascript:ContentClick('label41', 'label40');" onmouseover="ContentPreview('label41');" onmouseout="ContentUnpreview('label41');" title="click to collapse or expand..."> more... </a>
 <div id="label41" style="display:none">
 <table border="1">
 <tr>
 <td></td>
 <td colspan="1">Supported Version Ranges</td>
 </tr>
 <tr>
 <td>pim_use_sdwan</td>
 <td><code class="docutils literal notranslate">v7.6.0 -> 8.0.0 </code></td>
 </tr>
 <tr>
 <td>[enable]</td>
 <td><code class="docutils literal notranslate">v7.6.0 -> 8.0.0</code></td>
 <tr>
 <td>[disable]</td>
 <td><code class="docutils literal notranslate">v7.6.0 -> 8.0.0</code></td>
 </table>
 </div>
 </li>
            <li> <span class="li-head">register_rate_limit</span> - Limit of packets/sec per source registered through this RP (0 means unlimited). <span class="li-normal">type: int</span>
 <a id='label42' href="javascript:ContentClick('label43', 'label42');" onmouseover="ContentPreview('label43');" onmouseout="ContentUnpreview('label43');" title="click to collapse or expand..."> more... </a>
 <div id="label43" style="display:none">
 <table border="1">
 <tr>
 <td></td>
 <td colspan="1">Supported Version Ranges</td>
 </tr>
 <tr>
 <td>register_rate_limit</td>
 <td><code class="docutils literal notranslate">v6.0.0 -> 8.0.0 </code></td>
 </tr>
 </table>
 </div>
 </li>
            <li> <span class="li-head">rp_address</span> - Statically configured RP addresses. <span class="li-normal">type: list</span> <span style="font-family:'Courier New'" class="li-required">member_path: pim_sm_global/rp_address:id</span>
 <a id='label44' href="javascript:ContentClick('label45', 'label44');" onmouseover="ContentPreview('label45');" onmouseout="ContentUnpreview('label45');" title="click to collapse or expand..."> more... </a>
 <div id="label45" style="display:none">
 <table border="1">
 <tr>
 <td></td><td colspan="1">Supported Version Ranges</td>
 </tr>
 <tr>
 <td>rp_address</td>
 <td><code class="docutils literal notranslate">v6.0.0 -> 8.0.0 </code></td>
 </tr>
 </table>
 </div>
 </li>
                <ul class="ul-self">
                <li> <span class="li-head">group</span> - Groups to use this RP. Source router.access-list6.name. <span class="li-normal">type: str</span>
 <a id='label46' href="javascript:ContentClick('label47', 'label46');" onmouseover="ContentPreview('label47');" onmouseout="ContentUnpreview('label47');" title="click to collapse or expand..."> more... </a>
 <div id="label47" style="display:none">
 <table border="1">
 <tr>
 <td></td>
 <td colspan="1">Supported Version Ranges</td>
 </tr>
 <tr>
 <td>group</td>
 <td><code class="docutils literal notranslate">v8.0.0 -> 8.0.0 </code></td>
 </tr>
 </table>
 </div>
 </li>
                <li> <span class="li-head">id</span> - ID of the entry. see <a href='#notes'>Notes</a>. <span class="li-normal">type: int</span> <span class="li-required">required: true</span>
 <a id='label48' href="javascript:ContentClick('label49', 'label48');" onmouseover="ContentPreview('label49');" onmouseout="ContentUnpreview('label49');" title="click to collapse or expand..."> more... </a>
 <div id="label49" style="display:none">
 <table border="1">
 <tr>
 <td></td>
 <td colspan="1">Supported Version Ranges</td>
 </tr>
 <tr>
 <td>id</td>
 <td><code class="docutils literal notranslate">v6.0.0 -> 8.0.0 </code></td>
 </tr>
 </table>
 </div>
 </li>
                <li> <span class="li-head">ip6_address</span> - RP router IPv6 address. <span class="li-normal">type: str</span>
 <a id='label50' href="javascript:ContentClick('label51', 'label50');" onmouseover="ContentPreview('label51');" onmouseout="ContentUnpreview('label51');" title="click to collapse or expand..."> more... </a>
 <div id="label51" style="display:none">
 <table border="1">
 <tr>
 <td></td>
 <td colspan="1">Supported Version Ranges</td>
 </tr>
 <tr>
 <td>ip6_address</td>
 <td><code class="docutils literal notranslate">v6.0.0 -> 8.0.0 </code></td>
 </tr>
 </table>
 </div>
 </li>
                </ul>
            <li> <span class="li-head">spt_threshold</span> - Enable/disable switching to source specific trees. <span class="li-normal">type: str</span> <span class="li-normal">choices: enable, disable</span>
 <a id='label52' href="javascript:ContentClick('label53', 'label52');" onmouseover="ContentPreview('label53');" onmouseout="ContentUnpreview('label53');" title="click to collapse or expand..."> more... </a>
 <div id="label53" style="display:none">
 <table border="1">
 <tr>
 <td></td>
 <td colspan="1">Supported Version Ranges</td>
 </tr>
 <tr>
 <td>spt_threshold</td>
 <td><code class="docutils literal notranslate">v8.0.0 -> 8.0.0 </code></td>
 </tr>
 <tr>
 <td>[enable]</td>
 <td><code class="docutils literal notranslate">v8.0.0 -> 8.0.0</code></td>
 <tr>
 <td>[disable]</td>
 <td><code class="docutils literal notranslate">v8.0.0 -> 8.0.0</code></td>
 </table>
 </div>
 </li>
            <li> <span class="li-head">spt_threshold_group</span> - Groups allowed to switch to source tree. Source router.access-list6.name. <span class="li-normal">type: str</span>
 <a id='label54' href="javascript:ContentClick('label55', 'label54');" onmouseover="ContentPreview('label55');" onmouseout="ContentUnpreview('label55');" title="click to collapse or expand..."> more... </a>
 <div id="label55" style="display:none">
 <table border="1">
 <tr>
 <td></td>
 <td colspan="1">Supported Version Ranges</td>
 </tr>
 <tr>
 <td>spt_threshold_group</td>
 <td><code class="docutils literal notranslate">v8.0.0 -> 8.0.0 </code></td>
 </tr>
 </table>
 </div>
 </li>
            </ul>
        <li> <span class="li-head">pim_sm_global_vrf</span> - per-VRF PIM sparse-mode global settings. <span class="li-normal">type: list</span> <span style="font-family:'Courier New'" class="li-required">member_path: pim_sm_global_vrf:vrf</span>
 <a id='label56' href="javascript:ContentClick('label57', 'label56');" onmouseover="ContentPreview('label57');" onmouseout="ContentUnpreview('label57');" title="click to collapse or expand..."> more... </a>
 <div id="label57" style="display:none">
 <table border="1">
 <tr>
 <td></td><td colspan="1">Supported Version Ranges</td>
 </tr>
 <tr>
 <td>pim_sm_global_vrf</td>
 <td><code class="docutils literal notranslate">v8.0.0 -> 8.0.0 </code></td>
 </tr>
 </table>
 </div>
 </li>
            <ul class="ul-self">
            <li> <span class="li-head">bsr_allow_quick_refresh</span> - Enable/disable accept BSR quick refresh packets from neighbors. <span class="li-normal">type: str</span> <span class="li-normal">choices: enable, disable</span>
 <a id='label58' href="javascript:ContentClick('label59', 'label58');" onmouseover="ContentPreview('label59');" onmouseout="ContentUnpreview('label59');" title="click to collapse or expand..."> more... </a>
 <div id="label59" style="display:none">
 <table border="1">
 <tr>
 <td></td>
 <td colspan="1">Supported Version Ranges</td>
 </tr>
 <tr>
 <td>bsr_allow_quick_refresh</td>
 <td><code class="docutils literal notranslate">v8.0.0 -> 8.0.0 </code></td>
 </tr>
 <tr>
 <td>[enable]</td>
 <td><code class="docutils literal notranslate">v8.0.0 -> 8.0.0</code></td>
 <tr>
 <td>[disable]</td>
 <td><code class="docutils literal notranslate">v8.0.0 -> 8.0.0</code></td>
 </table>
 </div>
 </li>
            <li> <span class="li-head">bsr_candidate</span> - Enable/disable allowing this router to become a bootstrap router (BSR). <span class="li-normal">type: str</span> <span class="li-normal">choices: enable, disable</span>
 <a id='label60' href="javascript:ContentClick('label61', 'label60');" onmouseover="ContentPreview('label61');" onmouseout="ContentUnpreview('label61');" title="click to collapse or expand..."> more... </a>
 <div id="label61" style="display:none">
 <table border="1">
 <tr>
 <td></td>
 <td colspan="1">Supported Version Ranges</td>
 </tr>
 <tr>
 <td>bsr_candidate</td>
 <td><code class="docutils literal notranslate">v8.0.0 -> 8.0.0 </code></td>
 </tr>
 <tr>
 <td>[enable]</td>
 <td><code class="docutils literal notranslate">v8.0.0 -> 8.0.0</code></td>
 <tr>
 <td>[disable]</td>
 <td><code class="docutils literal notranslate">v8.0.0 -> 8.0.0</code></td>
 </table>
 </div>
 </li>
            <li> <span class="li-head">bsr_hash</span> - BSR hash length (0 - 128). <span class="li-normal">type: int</span>
 <a id='label62' href="javascript:ContentClick('label63', 'label62');" onmouseover="ContentPreview('label63');" onmouseout="ContentUnpreview('label63');" title="click to collapse or expand..."> more... </a>
 <div id="label63" style="display:none">
 <table border="1">
 <tr>
 <td></td>
 <td colspan="1">Supported Version Ranges</td>
 </tr>
 <tr>
 <td>bsr_hash</td>
 <td><code class="docutils literal notranslate">v8.0.0 -> 8.0.0 </code></td>
 </tr>
 </table>
 </div>
 </li>
            <li> <span class="li-head">bsr_interface</span> - Interface to advertise as candidate BSR. Source system.interface.name. <span class="li-normal">type: str</span>
 <a id='label64' href="javascript:ContentClick('label65', 'label64');" onmouseover="ContentPreview('label65');" onmouseout="ContentUnpreview('label65');" title="click to collapse or expand..."> more... </a>
 <div id="label65" style="display:none">
 <table border="1">
 <tr>
 <td></td>
 <td colspan="1">Supported Version Ranges</td>
 </tr>
 <tr>
 <td>bsr_interface</td>
 <td><code class="docutils literal notranslate">v8.0.0 -> 8.0.0 </code></td>
 </tr>
 </table>
 </div>
 </li>
            <li> <span class="li-head">bsr_priority</span> - BSR priority (0 - 255). <span class="li-normal">type: int</span>
 <a id='label66' href="javascript:ContentClick('label67', 'label66');" onmouseover="ContentPreview('label67');" onmouseout="ContentUnpreview('label67');" title="click to collapse or expand..."> more... </a>
 <div id="label67" style="display:none">
 <table border="1">
 <tr>
 <td></td>
 <td colspan="1">Supported Version Ranges</td>
 </tr>
 <tr>
 <td>bsr_priority</td>
 <td><code class="docutils literal notranslate">v8.0.0 -> 8.0.0 </code></td>
 </tr>
 </table>
 </div>
 </li>
            <li> <span class="li-head">cisco_crp_prefix</span> - Enable/disable making candidate RP compatible with old Cisco IOS. <span class="li-normal">type: str</span> <span class="li-normal">choices: enable, disable</span>
 <a id='label68' href="javascript:ContentClick('label69', 'label68');" onmouseover="ContentPreview('label69');" onmouseout="ContentUnpreview('label69');" title="click to collapse or expand..."> more... </a>
 <div id="label69" style="display:none">
 <table border="1">
 <tr>
 <td></td>
 <td colspan="1">Supported Version Ranges</td>
 </tr>
 <tr>
 <td>cisco_crp_prefix</td>
 <td><code class="docutils literal notranslate">v8.0.0 -> 8.0.0 </code></td>
 </tr>
 <tr>
 <td>[enable]</td>
 <td><code class="docutils literal notranslate">v8.0.0 -> 8.0.0</code></td>
 <tr>
 <td>[disable]</td>
 <td><code class="docutils literal notranslate">v8.0.0 -> 8.0.0</code></td>
 </table>
 </div>
 </li>
            <li> <span class="li-head">rp_address</span> - Statically configured RP addresses. <span class="li-normal">type: list</span> <span style="font-family:'Courier New'" class="li-required">member_path: pim_sm_global_vrf:vrf/rp_address:id</span>
 <a id='label70' href="javascript:ContentClick('label71', 'label70');" onmouseover="ContentPreview('label71');" onmouseout="ContentUnpreview('label71');" title="click to collapse or expand..."> more... </a>
 <div id="label71" style="display:none">
 <table border="1">
 <tr>
 <td></td><td colspan="1">Supported Version Ranges</td>
 </tr>
 <tr>
 <td>rp_address</td>
 <td><code class="docutils literal notranslate">v8.0.0 -> 8.0.0 </code></td>
 </tr>
 </table>
 </div>
 </li>
                <ul class="ul-self">
                <li> <span class="li-head">group</span> - Groups to use this RP. Source router.access-list6.name. <span class="li-normal">type: str</span>
 <a id='label72' href="javascript:ContentClick('label73', 'label72');" onmouseover="ContentPreview('label73');" onmouseout="ContentUnpreview('label73');" title="click to collapse or expand..."> more... </a>
 <div id="label73" style="display:none">
 <table border="1">
 <tr>
 <td></td>
 <td colspan="1">Supported Version Ranges</td>
 </tr>
 <tr>
 <td>group</td>
 <td><code class="docutils literal notranslate">v8.0.0 -> 8.0.0 </code></td>
 </tr>
 </table>
 </div>
 </li>
                <li> <span class="li-head">id</span> - ID of the entry. see <a href='#notes'>Notes</a>. <span class="li-normal">type: int</span> <span class="li-required">required: true</span>
 <a id='label74' href="javascript:ContentClick('label75', 'label74');" onmouseover="ContentPreview('label75');" onmouseout="ContentUnpreview('label75');" title="click to collapse or expand..."> more... </a>
 <div id="label75" style="display:none">
 <table border="1">
 <tr>
 <td></td>
 <td colspan="1">Supported Version Ranges</td>
 </tr>
 <tr>
 <td>id</td>
 <td><code class="docutils literal notranslate">v8.0.0 -> 8.0.0 </code></td>
 </tr>
 </table>
 </div>
 </li>
                <li> <span class="li-head">ip6_address</span> - RP router IPv6 address. <span class="li-normal">type: str</span>
 <a id='label76' href="javascript:ContentClick('label77', 'label76');" onmouseover="ContentPreview('label77');" onmouseout="ContentUnpreview('label77');" title="click to collapse or expand..."> more... </a>
 <div id="label77" style="display:none">
 <table border="1">
 <tr>
 <td></td>
 <td colspan="1">Supported Version Ranges</td>
 </tr>
 <tr>
 <td>ip6_address</td>
 <td><code class="docutils literal notranslate">v8.0.0 -> 8.0.0 </code></td>
 </tr>
 </table>
 </div>
 </li>
                </ul>
            <li> <span class="li-head">vrf</span> - VRF ID. see <a href='#notes'>Notes</a>. <span class="li-normal">type: int</span> <span class="li-required">required: true</span>
 <a id='label78' href="javascript:ContentClick('label79', 'label78');" onmouseover="ContentPreview('label79');" onmouseout="ContentUnpreview('label79');" title="click to collapse or expand..."> more... </a>
 <div id="label79" style="display:none">
 <table border="1">
 <tr>
 <td></td>
 <td colspan="1">Supported Version Ranges</td>
 </tr>
 <tr>
 <td>vrf</td>
 <td><code class="docutils literal notranslate">v8.0.0 -> 8.0.0 </code></td>
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
    
    - name: Configure IPv6 multicast.
      fortinet.fortios.fortios_router_multicast6:
          vdom: "{{ vdom }}"
          router_multicast6:
              interface:
                  -
                      hello_holdtime: ""
                      hello_interval: "30"
                      name: "default_name_6 (source system.interface.name)"
                      rp_candidate: "enable"
                      rp_candidate_group: "<your_own_value> (source router.access-list6.name)"
                      rp_candidate_interval: "60"
                      rp_candidate_priority: "192"
                      static_group: "<your_own_value> (source router.multicast6-flow.name)"
              multicast_pmtu: "enable"
              multicast_routing: "enable"
              pim_sm_global:
                  bsr_allow_quick_refresh: "enable"
                  bsr_candidate: "enable"
                  bsr_hash: "126"
                  bsr_interface: "<your_own_value> (source system.interface.name)"
                  bsr_priority: "0"
                  cisco_crp_prefix: "enable"
                  cisco_ignore_rp_set_priority: "enable"
                  pim_use_sdwan: "enable"
                  register_rate_limit: "0"
                  rp_address:
                      -
                          group: "<your_own_value> (source router.access-list6.name)"
                          id: "26"
                          ip6_address: "<your_own_value>"
                  spt_threshold: "enable"
                  spt_threshold_group: "<your_own_value> (source router.access-list6.name)"
              pim_sm_global_vrf:
                  -
                      bsr_allow_quick_refresh: "enable"
                      bsr_candidate: "enable"
                      bsr_hash: "126"
                      bsr_interface: "<your_own_value> (source system.interface.name)"
                      bsr_priority: "0"
                      cisco_crp_prefix: "enable"
                      rp_address:
                          -
                              group: "<your_own_value> (source router.access-list6.name)"
                              id: "39"
                              ip6_address: "<your_own_value>"
                      vrf: "<you_own_value>"


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
