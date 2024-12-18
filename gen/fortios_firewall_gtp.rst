:source: fortios_firewall_gtp.py

:orphan:

.. fortios_firewall_gtp:

fortios_firewall_gtp -- Configure GTP in Fortinet's FortiOS and FortiGate.
++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++

.. versionadded:: 2.0.0

.. contents::
   :local:
   :depth: 1


Synopsis
--------
- This module is able to configure a FortiGate or FortiOS (FOS) device by allowing the user to set and modify firewall feature and gtp category. Examples include all parameters and values need to be adjusted to datasources before usage. Tested with FOS v6.0.0



Requirements
------------
The below requirements are needed on the host that executes this module.

- ansible>=2.15


Tips
----
Using member operation to add an element to an existing object.

FortiOS Version Compatibility
-----------------------------
Supported Version Ranges: v6.0.0 -> v7.0.8, v7.2.0 -> v7.2.4, v7.4.3 -> v7.6.0


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
    <li> <span class="li-head">firewall_gtp</span> - Configure GTP. <span class="li-normal">type: dict</span>
 <a id='label0' href="javascript:ContentClick('label1', 'label0');" onmouseover="ContentPreview('label1');" onmouseout="ContentUnpreview('label1');" title="click to collapse or expand..."> more... </a>
 <div id="label1" style="display:none">
 <table border="1">
 <tr>
 <td></td><td colspan="3">Supported Version Ranges</td>
 </tr>
 <tr>
 <td>firewall_gtp</td>
 <td><code class="docutils literal notranslate">v6.0.0 -> v7.0.8 </code></td>
 <td><code class="docutils literal notranslate">v7.2.0 -> v7.2.4 </code></td>
 <td><code class="docutils literal notranslate">v7.4.3 -> 7.6.0 </code></td>
 </tr>
 </table>
 </div>
 </li>
        <ul class="ul-self">
        <li> <span class="li-head">addr_notify</span> - overbilling notify address <span class="li-normal">type: str</span>
 <a id='label2' href="javascript:ContentClick('label3', 'label2');" onmouseover="ContentPreview('label3');" onmouseout="ContentUnpreview('label3');" title="click to collapse or expand..."> more... </a>
 <div id="label3" style="display:none">
 <table border="1">
 <tr>
 <td></td>
 <td colspan="3">Supported Version Ranges</td>
 </tr>
 <tr>
 <td>addr_notify</td>
 <td><code class="docutils literal notranslate">v6.0.0 -> v7.0.8 </code></td>
 <td><code class="docutils literal notranslate">v7.2.0 -> v7.2.4 </code></td>
 <td><code class="docutils literal notranslate">v7.4.3 -> 7.6.0 </code></td>
 </tr>
 </table>
 </div>
 </li>
        <li> <span class="li-head">apn</span> - APN. <span class="li-normal">type: list</span> <span style="font-family:'Courier New'" class="li-required">member_path: apn:id</span>
 <a id='label4' href="javascript:ContentClick('label5', 'label4');" onmouseover="ContentPreview('label5');" onmouseout="ContentUnpreview('label5');" title="click to collapse or expand..."> more... </a>
 <div id="label5" style="display:none">
 <table border="1">
 <tr>
 <td></td><td colspan="3">Supported Version Ranges</td>
 </tr>
 <tr>
 <td>apn</td>
 <td><code class="docutils literal notranslate">v6.0.0 -> v7.0.8 </code></td>
 <td><code class="docutils literal notranslate">v7.2.0 -> v7.2.4 </code></td>
 <td><code class="docutils literal notranslate">v7.4.3 -> 7.6.0 </code></td>
 </tr>
 </table>
 </div>
 </li>
            <ul class="ul-self">
            <li> <span class="li-head">action</span> - Action. <span class="li-normal">type: str</span> <span class="li-normal">choices: allow, deny</span>
 <a id='label6' href="javascript:ContentClick('label7', 'label6');" onmouseover="ContentPreview('label7');" onmouseout="ContentUnpreview('label7');" title="click to collapse or expand..."> more... </a>
 <div id="label7" style="display:none">
 <table border="1">
 <tr>
 <td></td>
 <td colspan="3">Supported Version Ranges</td>
 </tr>
 <tr>
 <td>action</td>
 <td><code class="docutils literal notranslate">v6.0.0 -> v7.0.8 </code></td>
 <td><code class="docutils literal notranslate">v7.2.0 -> v7.2.4 </code></td>
 <td><code class="docutils literal notranslate">v7.4.3 -> 7.6.0 </code></td>
 </tr>
 <tr>
 <td>[allow]</td>
 <td><code class="docutils literal notranslate">v6.0.0 -> v7.0.8</code></td>
 <tr>
 <td>[deny]</td>
 <td><code class="docutils literal notranslate">v6.0.0 -> v7.0.8</code></td>
 </table>
 </div>
 </li>
            <li> <span class="li-head">apnmember</span> - APN member. <span class="li-normal">type: list</span> <span style="font-family:'Courier New'" class="li-required">member_path: apn:id/apnmember:name</span>
 <a id='label8' href="javascript:ContentClick('label9', 'label8');" onmouseover="ContentPreview('label9');" onmouseout="ContentUnpreview('label9');" title="click to collapse or expand..."> more... </a>
 <div id="label9" style="display:none">
 <table border="1">
 <tr>
 <td></td><td colspan="3">Supported Version Ranges</td>
 </tr>
 <tr>
 <td>apnmember</td>
 <td><code class="docutils literal notranslate">v6.0.0 -> v7.0.8 </code></td>
 <td><code class="docutils literal notranslate">v7.2.0 -> v7.2.4 </code></td>
 <td><code class="docutils literal notranslate">v7.4.3 -> 7.6.0 </code></td>
 </tr>
 </table>
 </div>
 </li>
                <ul class="ul-self">
                <li> <span class="li-head">name</span> - APN name. Source gtp.apn.name gtp.apngrp.name. <span class="li-normal">type: str</span> <span class="li-required">required: true</span>
 <a id='label10' href="javascript:ContentClick('label11', 'label10');" onmouseover="ContentPreview('label11');" onmouseout="ContentUnpreview('label11');" title="click to collapse or expand..."> more... </a>
 <div id="label11" style="display:none">
 <table border="1">
 <tr>
 <td></td>
 <td colspan="3">Supported Version Ranges</td>
 </tr>
 <tr>
 <td>name</td>
 <td><code class="docutils literal notranslate">v6.0.0 -> v7.0.8 </code></td>
 <td><code class="docutils literal notranslate">v7.2.0 -> v7.2.4 </code></td>
 <td><code class="docutils literal notranslate">v7.4.3 -> 7.6.0 </code></td>
 </tr>
 </table>
 </div>
 </li>
                </ul>
            <li> <span class="li-head">id</span> - ID. see <a href='#notes'>Notes</a>. <span class="li-normal">type: int</span> <span class="li-required">required: true</span>
 <a id='label12' href="javascript:ContentClick('label13', 'label12');" onmouseover="ContentPreview('label13');" onmouseout="ContentUnpreview('label13');" title="click to collapse or expand..."> more... </a>
 <div id="label13" style="display:none">
 <table border="1">
 <tr>
 <td></td>
 <td colspan="3">Supported Version Ranges</td>
 </tr>
 <tr>
 <td>id</td>
 <td><code class="docutils literal notranslate">v6.0.0 -> v7.0.8 </code></td>
 <td><code class="docutils literal notranslate">v7.2.0 -> v7.2.4 </code></td>
 <td><code class="docutils literal notranslate">v7.4.3 -> 7.6.0 </code></td>
 </tr>
 </table>
 </div>
 </li>
            <li> <span class="li-head">selection_mode</span> - APN selection mode. <span class="li-normal">type: list</span> <span class="li-normal">choices: ms, net, vrf</span>
 <a id='label14' href="javascript:ContentClick('label15', 'label14');" onmouseover="ContentPreview('label15');" onmouseout="ContentUnpreview('label15');" title="click to collapse or expand..."> more... </a>
 <div id="label15" style="display:none">
 <table border="1">
 <tr>
 <td></td>
 <td colspan="3">Supported Version Ranges</td>
 </tr>
 <tr>
 <td>selection_mode</td>
 <td><code class="docutils literal notranslate">v6.0.0 -> v7.0.8 </code></td>
 <td><code class="docutils literal notranslate">v7.2.0 -> v7.2.4 </code></td>
 <td><code class="docutils literal notranslate">v7.4.3 -> 7.6.0 </code></td>
 </tr>
 <tr>
 <td>[ms]</td>
 <td><code class="docutils literal notranslate">v6.0.0 -> v7.0.8</code></td>
 <tr>
 <td>[net]</td>
 <td><code class="docutils literal notranslate">v6.0.0 -> v7.0.8</code></td>
 <tr>
 <td>[vrf]</td>
 <td><code class="docutils literal notranslate">v6.0.0 -> v7.0.8</code></td>
 </table>
 </div>
 </li>
            </ul>
        <li> <span class="li-head">apn_filter</span> - apn filter <span class="li-normal">type: str</span> <span class="li-normal">choices: enable, disable</span>
 <a id='label16' href="javascript:ContentClick('label17', 'label16');" onmouseover="ContentPreview('label17');" onmouseout="ContentUnpreview('label17');" title="click to collapse or expand..."> more... </a>
 <div id="label17" style="display:none">
 <table border="1">
 <tr>
 <td></td>
 <td colspan="3">Supported Version Ranges</td>
 </tr>
 <tr>
 <td>apn_filter</td>
 <td><code class="docutils literal notranslate">v6.0.0 -> v7.0.8 </code></td>
 <td><code class="docutils literal notranslate">v7.2.0 -> v7.2.4 </code></td>
 <td><code class="docutils literal notranslate">v7.4.3 -> 7.6.0 </code></td>
 </tr>
 <tr>
 <td>[enable]</td>
 <td><code class="docutils literal notranslate">v6.0.0 -> v7.0.8</code></td>
 <tr>
 <td>[disable]</td>
 <td><code class="docutils literal notranslate">v6.0.0 -> v7.0.8</code></td>
 </table>
 </div>
 </li>
        <li> <span class="li-head">authorized_ggsns</span> - Authorized GGSN/PGW group. Source firewall.address.name firewall.addrgrp.name. <span class="li-normal">type: str</span>
 <a id='label18' href="javascript:ContentClick('label19', 'label18');" onmouseover="ContentPreview('label19');" onmouseout="ContentUnpreview('label19');" title="click to collapse or expand..."> more... </a>
 <div id="label19" style="display:none">
 <table border="1">
 <tr>
 <td></td>
 <td colspan="3">Supported Version Ranges</td>
 </tr>
 <tr>
 <td>authorized_ggsns</td>
 <td><code class="docutils literal notranslate">v6.0.0 -> v7.0.8 </code></td>
 <td><code class="docutils literal notranslate">v7.2.0 -> v7.2.4 </code></td>
 <td><code class="docutils literal notranslate">v7.4.3 -> 7.6.0 </code></td>
 </tr>
 </table>
 </div>
 </li>
        <li> <span class="li-head">authorized_ggsns6</span> - Authorized GGSN/PGW IPv6 group. Source firewall.address6.name firewall.addrgrp6.name. <span class="li-normal">type: str</span>
 <a id='label20' href="javascript:ContentClick('label21', 'label20');" onmouseover="ContentPreview('label21');" onmouseout="ContentUnpreview('label21');" title="click to collapse or expand..."> more... </a>
 <div id="label21" style="display:none">
 <table border="1">
 <tr>
 <td></td>
 <td colspan="4">Supported Version Ranges</td>
 </tr>
 <tr>
 <td>authorized_ggsns6</td>
 <td><code class="docutils literal notranslate">v6.4.0 -> v6.4.0 </code></td>
 <td><code class="docutils literal notranslate">v6.4.4 -> v7.0.8 </code></td>
 <td><code class="docutils literal notranslate">v7.2.0 -> v7.2.4 </code></td>
 <td><code class="docutils literal notranslate">v7.4.3 -> 7.6.0 </code></td>
 </tr>
 </table>
 </div>
 </li>
        <li> <span class="li-head">authorized_sgsns</span> - Authorized SGSN/SGW group. Source firewall.address.name firewall.addrgrp.name. <span class="li-normal">type: str</span>
 <a id='label22' href="javascript:ContentClick('label23', 'label22');" onmouseover="ContentPreview('label23');" onmouseout="ContentUnpreview('label23');" title="click to collapse or expand..."> more... </a>
 <div id="label23" style="display:none">
 <table border="1">
 <tr>
 <td></td>
 <td colspan="3">Supported Version Ranges</td>
 </tr>
 <tr>
 <td>authorized_sgsns</td>
 <td><code class="docutils literal notranslate">v6.0.0 -> v7.0.8 </code></td>
 <td><code class="docutils literal notranslate">v7.2.0 -> v7.2.4 </code></td>
 <td><code class="docutils literal notranslate">v7.4.3 -> 7.6.0 </code></td>
 </tr>
 </table>
 </div>
 </li>
        <li> <span class="li-head">authorized_sgsns6</span> - Authorized SGSN/SGW IPv6 group. Source firewall.address6.name firewall.addrgrp6.name. <span class="li-normal">type: str</span>
 <a id='label24' href="javascript:ContentClick('label25', 'label24');" onmouseover="ContentPreview('label25');" onmouseout="ContentUnpreview('label25');" title="click to collapse or expand..."> more... </a>
 <div id="label25" style="display:none">
 <table border="1">
 <tr>
 <td></td>
 <td colspan="4">Supported Version Ranges</td>
 </tr>
 <tr>
 <td>authorized_sgsns6</td>
 <td><code class="docutils literal notranslate">v6.4.0 -> v6.4.0 </code></td>
 <td><code class="docutils literal notranslate">v6.4.4 -> v7.0.8 </code></td>
 <td><code class="docutils literal notranslate">v7.2.0 -> v7.2.4 </code></td>
 <td><code class="docutils literal notranslate">v7.4.3 -> 7.6.0 </code></td>
 </tr>
 </table>
 </div>
 </li>
        <li> <span class="li-head">comment</span> - Comment. <span class="li-normal">type: str</span>
 <a id='label26' href="javascript:ContentClick('label27', 'label26');" onmouseover="ContentPreview('label27');" onmouseout="ContentUnpreview('label27');" title="click to collapse or expand..."> more... </a>
 <div id="label27" style="display:none">
 <table border="1">
 <tr>
 <td></td>
 <td colspan="3">Supported Version Ranges</td>
 </tr>
 <tr>
 <td>comment</td>
 <td><code class="docutils literal notranslate">v6.0.0 -> v7.0.8 </code></td>
 <td><code class="docutils literal notranslate">v7.2.0 -> v7.2.4 </code></td>
 <td><code class="docutils literal notranslate">v7.4.3 -> 7.6.0 </code></td>
 </tr>
 </table>
 </div>
 </li>
        <li> <span class="li-head">context_id</span> - Overbilling context. <span class="li-normal">type: int</span>
 <a id='label28' href="javascript:ContentClick('label29', 'label28');" onmouseover="ContentPreview('label29');" onmouseout="ContentUnpreview('label29');" title="click to collapse or expand..."> more... </a>
 <div id="label29" style="display:none">
 <table border="1">
 <tr>
 <td></td>
 <td colspan="3">Supported Version Ranges</td>
 </tr>
 <tr>
 <td>context_id</td>
 <td><code class="docutils literal notranslate">v6.0.0 -> v7.0.8 </code></td>
 <td><code class="docutils literal notranslate">v7.2.0 -> v7.2.4 </code></td>
 <td><code class="docutils literal notranslate">v7.4.3 -> 7.6.0 </code></td>
 </tr>
 </table>
 </div>
 </li>
        <li> <span class="li-head">control_plane_message_rate_limit</span> - control plane message rate limit <span class="li-normal">type: int</span>
 <a id='label30' href="javascript:ContentClick('label31', 'label30');" onmouseover="ContentPreview('label31');" onmouseout="ContentUnpreview('label31');" title="click to collapse or expand..."> more... </a>
 <div id="label31" style="display:none">
 <table border="1">
 <tr>
 <td></td>
 <td colspan="3">Supported Version Ranges</td>
 </tr>
 <tr>
 <td>control_plane_message_rate_limit</td>
 <td><code class="docutils literal notranslate">v6.0.0 -> v7.0.8 </code></td>
 <td><code class="docutils literal notranslate">v7.2.0 -> v7.2.4 </code></td>
 <td><code class="docutils literal notranslate">v7.4.3 -> 7.6.0 </code></td>
 </tr>
 </table>
 </div>
 </li>
        <li> <span class="li-head">default_apn_action</span> - default apn action <span class="li-normal">type: str</span> <span class="li-normal">choices: allow, deny</span>
 <a id='label32' href="javascript:ContentClick('label33', 'label32');" onmouseover="ContentPreview('label33');" onmouseout="ContentUnpreview('label33');" title="click to collapse or expand..."> more... </a>
 <div id="label33" style="display:none">
 <table border="1">
 <tr>
 <td></td>
 <td colspan="3">Supported Version Ranges</td>
 </tr>
 <tr>
 <td>default_apn_action</td>
 <td><code class="docutils literal notranslate">v6.0.0 -> v7.0.8 </code></td>
 <td><code class="docutils literal notranslate">v7.2.0 -> v7.2.4 </code></td>
 <td><code class="docutils literal notranslate">v7.4.3 -> 7.6.0 </code></td>
 </tr>
 <tr>
 <td>[allow]</td>
 <td><code class="docutils literal notranslate">v6.0.0 -> v7.0.8</code></td>
 <tr>
 <td>[deny]</td>
 <td><code class="docutils literal notranslate">v6.0.0 -> v7.0.8</code></td>
 </table>
 </div>
 </li>
        <li> <span class="li-head">default_imsi_action</span> - default imsi action <span class="li-normal">type: str</span> <span class="li-normal">choices: allow, deny</span>
 <a id='label34' href="javascript:ContentClick('label35', 'label34');" onmouseover="ContentPreview('label35');" onmouseout="ContentUnpreview('label35');" title="click to collapse or expand..."> more... </a>
 <div id="label35" style="display:none">
 <table border="1">
 <tr>
 <td></td>
 <td colspan="3">Supported Version Ranges</td>
 </tr>
 <tr>
 <td>default_imsi_action</td>
 <td><code class="docutils literal notranslate">v6.0.0 -> v7.0.8 </code></td>
 <td><code class="docutils literal notranslate">v7.2.0 -> v7.2.4 </code></td>
 <td><code class="docutils literal notranslate">v7.4.3 -> 7.6.0 </code></td>
 </tr>
 <tr>
 <td>[allow]</td>
 <td><code class="docutils literal notranslate">v6.0.0 -> v7.0.8</code></td>
 <tr>
 <td>[deny]</td>
 <td><code class="docutils literal notranslate">v6.0.0 -> v7.0.8</code></td>
 </table>
 </div>
 </li>
        <li> <span class="li-head">default_ip_action</span> - default action for encapsulated IP traffic <span class="li-normal">type: str</span> <span class="li-normal">choices: allow, deny</span>
 <a id='label36' href="javascript:ContentClick('label37', 'label36');" onmouseover="ContentPreview('label37');" onmouseout="ContentUnpreview('label37');" title="click to collapse or expand..."> more... </a>
 <div id="label37" style="display:none">
 <table border="1">
 <tr>
 <td></td>
 <td colspan="3">Supported Version Ranges</td>
 </tr>
 <tr>
 <td>default_ip_action</td>
 <td><code class="docutils literal notranslate">v6.0.0 -> v7.0.8 </code></td>
 <td><code class="docutils literal notranslate">v7.2.0 -> v7.2.4 </code></td>
 <td><code class="docutils literal notranslate">v7.4.3 -> 7.6.0 </code></td>
 </tr>
 <tr>
 <td>[allow]</td>
 <td><code class="docutils literal notranslate">v6.0.0 -> v7.0.8</code></td>
 <tr>
 <td>[deny]</td>
 <td><code class="docutils literal notranslate">v6.0.0 -> v7.0.8</code></td>
 </table>
 </div>
 </li>
        <li> <span class="li-head">default_noip_action</span> - default action for encapsulated non-IP traffic <span class="li-normal">type: str</span> <span class="li-normal">choices: allow, deny</span>
 <a id='label38' href="javascript:ContentClick('label39', 'label38');" onmouseover="ContentPreview('label39');" onmouseout="ContentUnpreview('label39');" title="click to collapse or expand..."> more... </a>
 <div id="label39" style="display:none">
 <table border="1">
 <tr>
 <td></td>
 <td colspan="3">Supported Version Ranges</td>
 </tr>
 <tr>
 <td>default_noip_action</td>
 <td><code class="docutils literal notranslate">v6.0.0 -> v7.0.8 </code></td>
 <td><code class="docutils literal notranslate">v7.2.0 -> v7.2.4 </code></td>
 <td><code class="docutils literal notranslate">v7.4.3 -> 7.6.0 </code></td>
 </tr>
 <tr>
 <td>[allow]</td>
 <td><code class="docutils literal notranslate">v6.0.0 -> v7.0.8</code></td>
 <tr>
 <td>[deny]</td>
 <td><code class="docutils literal notranslate">v6.0.0 -> v7.0.8</code></td>
 </table>
 </div>
 </li>
        <li> <span class="li-head">default_policy_action</span> - default advanced policy action <span class="li-normal">type: str</span> <span class="li-normal">choices: allow, deny</span>
 <a id='label40' href="javascript:ContentClick('label41', 'label40');" onmouseover="ContentPreview('label41');" onmouseout="ContentUnpreview('label41');" title="click to collapse or expand..."> more... </a>
 <div id="label41" style="display:none">
 <table border="1">
 <tr>
 <td></td>
 <td colspan="3">Supported Version Ranges</td>
 </tr>
 <tr>
 <td>default_policy_action</td>
 <td><code class="docutils literal notranslate">v6.0.0 -> v7.0.8 </code></td>
 <td><code class="docutils literal notranslate">v7.2.0 -> v7.2.4 </code></td>
 <td><code class="docutils literal notranslate">v7.4.3 -> 7.6.0 </code></td>
 </tr>
 <tr>
 <td>[allow]</td>
 <td><code class="docutils literal notranslate">v6.0.0 -> v7.0.8</code></td>
 <tr>
 <td>[deny]</td>
 <td><code class="docutils literal notranslate">v6.0.0 -> v7.0.8</code></td>
 </table>
 </div>
 </li>
        <li> <span class="li-head">denied_log</span> - log denied <span class="li-normal">type: str</span> <span class="li-normal">choices: enable, disable</span>
 <a id='label42' href="javascript:ContentClick('label43', 'label42');" onmouseover="ContentPreview('label43');" onmouseout="ContentUnpreview('label43');" title="click to collapse or expand..."> more... </a>
 <div id="label43" style="display:none">
 <table border="1">
 <tr>
 <td></td>
 <td colspan="3">Supported Version Ranges</td>
 </tr>
 <tr>
 <td>denied_log</td>
 <td><code class="docutils literal notranslate">v6.0.0 -> v7.0.8 </code></td>
 <td><code class="docutils literal notranslate">v7.2.0 -> v7.2.4 </code></td>
 <td><code class="docutils literal notranslate">v7.4.3 -> 7.6.0 </code></td>
 </tr>
 <tr>
 <td>[enable]</td>
 <td><code class="docutils literal notranslate">v6.0.0 -> v7.0.8</code></td>
 <tr>
 <td>[disable]</td>
 <td><code class="docutils literal notranslate">v6.0.0 -> v7.0.8</code></td>
 </table>
 </div>
 </li>
        <li> <span class="li-head">echo_request_interval</span> - echo request interval (in seconds) <span class="li-normal">type: int</span>
 <a id='label44' href="javascript:ContentClick('label45', 'label44');" onmouseover="ContentPreview('label45');" onmouseout="ContentUnpreview('label45');" title="click to collapse or expand..."> more... </a>
 <div id="label45" style="display:none">
 <table border="1">
 <tr>
 <td></td>
 <td colspan="3">Supported Version Ranges</td>
 </tr>
 <tr>
 <td>echo_request_interval</td>
 <td><code class="docutils literal notranslate">v6.0.0 -> v7.0.8 </code></td>
 <td><code class="docutils literal notranslate">v7.2.0 -> v7.2.4 </code></td>
 <td><code class="docutils literal notranslate">v7.4.3 -> 7.6.0 </code></td>
 </tr>
 </table>
 </div>
 </li>
        <li> <span class="li-head">extension_log</span> - log in extension format <span class="li-normal">type: str</span> <span class="li-normal">choices: enable, disable</span>
 <a id='label46' href="javascript:ContentClick('label47', 'label46');" onmouseover="ContentPreview('label47');" onmouseout="ContentUnpreview('label47');" title="click to collapse or expand..."> more... </a>
 <div id="label47" style="display:none">
 <table border="1">
 <tr>
 <td></td>
 <td colspan="3">Supported Version Ranges</td>
 </tr>
 <tr>
 <td>extension_log</td>
 <td><code class="docutils literal notranslate">v6.0.0 -> v7.0.8 </code></td>
 <td><code class="docutils literal notranslate">v7.2.0 -> v7.2.4 </code></td>
 <td><code class="docutils literal notranslate">v7.4.3 -> 7.6.0 </code></td>
 </tr>
 <tr>
 <td>[enable]</td>
 <td><code class="docutils literal notranslate">v6.0.0 -> v7.0.8</code></td>
 <tr>
 <td>[disable]</td>
 <td><code class="docutils literal notranslate">v6.0.0 -> v7.0.8</code></td>
 </table>
 </div>
 </li>
        <li> <span class="li-head">forwarded_log</span> - log forwarded <span class="li-normal">type: str</span> <span class="li-normal">choices: enable, disable</span>
 <a id='label48' href="javascript:ContentClick('label49', 'label48');" onmouseover="ContentPreview('label49');" onmouseout="ContentUnpreview('label49');" title="click to collapse or expand..."> more... </a>
 <div id="label49" style="display:none">
 <table border="1">
 <tr>
 <td></td>
 <td colspan="3">Supported Version Ranges</td>
 </tr>
 <tr>
 <td>forwarded_log</td>
 <td><code class="docutils literal notranslate">v6.0.0 -> v7.0.8 </code></td>
 <td><code class="docutils literal notranslate">v7.2.0 -> v7.2.4 </code></td>
 <td><code class="docutils literal notranslate">v7.4.3 -> 7.6.0 </code></td>
 </tr>
 <tr>
 <td>[enable]</td>
 <td><code class="docutils literal notranslate">v6.0.0 -> v7.0.8</code></td>
 <tr>
 <td>[disable]</td>
 <td><code class="docutils literal notranslate">v6.0.0 -> v7.0.8</code></td>
 </table>
 </div>
 </li>
        <li> <span class="li-head">global_tunnel_limit</span> - Global tunnel limit. Source gtp.tunnel-limit.name. <span class="li-normal">type: str</span>
 <a id='label50' href="javascript:ContentClick('label51', 'label50');" onmouseover="ContentPreview('label51');" onmouseout="ContentUnpreview('label51');" title="click to collapse or expand..."> more... </a>
 <div id="label51" style="display:none">
 <table border="1">
 <tr>
 <td></td>
 <td colspan="3">Supported Version Ranges</td>
 </tr>
 <tr>
 <td>global_tunnel_limit</td>
 <td><code class="docutils literal notranslate">v6.0.0 -> v7.0.8 </code></td>
 <td><code class="docutils literal notranslate">v7.2.0 -> v7.2.4 </code></td>
 <td><code class="docutils literal notranslate">v7.4.3 -> 7.6.0 </code></td>
 </tr>
 </table>
 </div>
 </li>
        <li> <span class="li-head">gtp_in_gtp</span> - gtp in gtp <span class="li-normal">type: str</span> <span class="li-normal">choices: allow, deny</span>
 <a id='label52' href="javascript:ContentClick('label53', 'label52');" onmouseover="ContentPreview('label53');" onmouseout="ContentUnpreview('label53');" title="click to collapse or expand..."> more... </a>
 <div id="label53" style="display:none">
 <table border="1">
 <tr>
 <td></td>
 <td colspan="3">Supported Version Ranges</td>
 </tr>
 <tr>
 <td>gtp_in_gtp</td>
 <td><code class="docutils literal notranslate">v6.0.0 -> v7.0.8 </code></td>
 <td><code class="docutils literal notranslate">v7.2.0 -> v7.2.4 </code></td>
 <td><code class="docutils literal notranslate">v7.4.3 -> 7.6.0 </code></td>
 </tr>
 <tr>
 <td>[allow]</td>
 <td><code class="docutils literal notranslate">v6.0.0 -> v7.0.8</code></td>
 <tr>
 <td>[deny]</td>
 <td><code class="docutils literal notranslate">v6.0.0 -> v7.0.8</code></td>
 </table>
 </div>
 </li>
        <li> <span class="li-head">gtpu_denied_log</span> - Enable/disable logging of denied GTP-U packets. <span class="li-normal">type: str</span> <span class="li-normal">choices: enable, disable</span>
 <a id='label54' href="javascript:ContentClick('label55', 'label54');" onmouseover="ContentPreview('label55');" onmouseout="ContentUnpreview('label55');" title="click to collapse or expand..."> more... </a>
 <div id="label55" style="display:none">
 <table border="1">
 <tr>
 <td></td>
 <td colspan="3">Supported Version Ranges</td>
 </tr>
 <tr>
 <td>gtpu_denied_log</td>
 <td><code class="docutils literal notranslate">v6.0.0 -> v7.0.8 </code></td>
 <td><code class="docutils literal notranslate">v7.2.0 -> v7.2.4 </code></td>
 <td><code class="docutils literal notranslate">v7.4.3 -> 7.6.0 </code></td>
 </tr>
 <tr>
 <td>[enable]</td>
 <td><code class="docutils literal notranslate">v6.0.0 -> v7.0.8</code></td>
 <tr>
 <td>[disable]</td>
 <td><code class="docutils literal notranslate">v6.0.0 -> v7.0.8</code></td>
 </table>
 </div>
 </li>
        <li> <span class="li-head">gtpu_forwarded_log</span> - Enable/disable logging of forwarded GTP-U packets. <span class="li-normal">type: str</span> <span class="li-normal">choices: enable, disable</span>
 <a id='label56' href="javascript:ContentClick('label57', 'label56');" onmouseover="ContentPreview('label57');" onmouseout="ContentUnpreview('label57');" title="click to collapse or expand..."> more... </a>
 <div id="label57" style="display:none">
 <table border="1">
 <tr>
 <td></td>
 <td colspan="3">Supported Version Ranges</td>
 </tr>
 <tr>
 <td>gtpu_forwarded_log</td>
 <td><code class="docutils literal notranslate">v6.0.0 -> v7.0.8 </code></td>
 <td><code class="docutils literal notranslate">v7.2.0 -> v7.2.4 </code></td>
 <td><code class="docutils literal notranslate">v7.4.3 -> 7.6.0 </code></td>
 </tr>
 <tr>
 <td>[enable]</td>
 <td><code class="docutils literal notranslate">v6.0.0 -> v7.0.8</code></td>
 <tr>
 <td>[disable]</td>
 <td><code class="docutils literal notranslate">v6.0.0 -> v7.0.8</code></td>
 </table>
 </div>
 </li>
        <li> <span class="li-head">gtpu_log_freq</span> - Logging of frequency of GTP-U packets. <span class="li-normal">type: int</span>
 <a id='label58' href="javascript:ContentClick('label59', 'label58');" onmouseover="ContentPreview('label59');" onmouseout="ContentUnpreview('label59');" title="click to collapse or expand..."> more... </a>
 <div id="label59" style="display:none">
 <table border="1">
 <tr>
 <td></td>
 <td colspan="3">Supported Version Ranges</td>
 </tr>
 <tr>
 <td>gtpu_log_freq</td>
 <td><code class="docutils literal notranslate">v6.0.0 -> v7.0.8 </code></td>
 <td><code class="docutils literal notranslate">v7.2.0 -> v7.2.4 </code></td>
 <td><code class="docutils literal notranslate">v7.4.3 -> 7.6.0 </code></td>
 </tr>
 </table>
 </div>
 </li>
        <li> <span class="li-head">gtpv0</span> - GTPv0 traffic. <span class="li-normal">type: str</span> <span class="li-normal">choices: allow, deny</span>
 <a id='label60' href="javascript:ContentClick('label61', 'label60');" onmouseover="ContentPreview('label61');" onmouseout="ContentUnpreview('label61');" title="click to collapse or expand..."> more... </a>
 <div id="label61" style="display:none">
 <table border="1">
 <tr>
 <td></td>
 <td colspan="1">Supported Version Ranges</td>
 </tr>
 <tr>
 <td>gtpv0</td>
 <td><code class="docutils literal notranslate">v7.6.0 -> 7.6.0 </code></td>
 </tr>
 <tr>
 <td>[allow]</td>
 <td><code class="docutils literal notranslate">v7.6.0 -> 7.6.0</code></td>
 <tr>
 <td>[deny]</td>
 <td><code class="docutils literal notranslate">v7.6.0 -> 7.6.0</code></td>
 </table>
 </div>
 </li>
        <li> <span class="li-head">half_close_timeout</span> - Half-close tunnel timeout (in seconds). <span class="li-normal">type: int</span>
 <a id='label62' href="javascript:ContentClick('label63', 'label62');" onmouseover="ContentPreview('label63');" onmouseout="ContentUnpreview('label63');" title="click to collapse or expand..."> more... </a>
 <div id="label63" style="display:none">
 <table border="1">
 <tr>
 <td></td>
 <td colspan="3">Supported Version Ranges</td>
 </tr>
 <tr>
 <td>half_close_timeout</td>
 <td><code class="docutils literal notranslate">v6.0.0 -> v7.0.8 </code></td>
 <td><code class="docutils literal notranslate">v7.2.0 -> v7.2.4 </code></td>
 <td><code class="docutils literal notranslate">v7.4.3 -> 7.6.0 </code></td>
 </tr>
 </table>
 </div>
 </li>
        <li> <span class="li-head">half_open_timeout</span> - Half-open tunnel timeout (in seconds). <span class="li-normal">type: int</span>
 <a id='label64' href="javascript:ContentClick('label65', 'label64');" onmouseover="ContentPreview('label65');" onmouseout="ContentUnpreview('label65');" title="click to collapse or expand..."> more... </a>
 <div id="label65" style="display:none">
 <table border="1">
 <tr>
 <td></td>
 <td colspan="3">Supported Version Ranges</td>
 </tr>
 <tr>
 <td>half_open_timeout</td>
 <td><code class="docutils literal notranslate">v6.0.0 -> v7.0.8 </code></td>
 <td><code class="docutils literal notranslate">v7.2.0 -> v7.2.4 </code></td>
 <td><code class="docutils literal notranslate">v7.4.3 -> 7.6.0 </code></td>
 </tr>
 </table>
 </div>
 </li>
        <li> <span class="li-head">handover_group</span> - Handover SGSN/SGW group. Source firewall.address.name firewall.addrgrp.name. <span class="li-normal">type: str</span>
 <a id='label66' href="javascript:ContentClick('label67', 'label66');" onmouseover="ContentPreview('label67');" onmouseout="ContentUnpreview('label67');" title="click to collapse or expand..."> more... </a>
 <div id="label67" style="display:none">
 <table border="1">
 <tr>
 <td></td>
 <td colspan="3">Supported Version Ranges</td>
 </tr>
 <tr>
 <td>handover_group</td>
 <td><code class="docutils literal notranslate">v6.0.0 -> v7.0.8 </code></td>
 <td><code class="docutils literal notranslate">v7.2.0 -> v7.2.4 </code></td>
 <td><code class="docutils literal notranslate">v7.4.3 -> 7.6.0 </code></td>
 </tr>
 </table>
 </div>
 </li>
        <li> <span class="li-head">handover_group6</span> - Handover SGSN/SGW IPv6 group. Source firewall.address6.name firewall.addrgrp6.name. <span class="li-normal">type: str</span>
 <a id='label68' href="javascript:ContentClick('label69', 'label68');" onmouseover="ContentPreview('label69');" onmouseout="ContentUnpreview('label69');" title="click to collapse or expand..."> more... </a>
 <div id="label69" style="display:none">
 <table border="1">
 <tr>
 <td></td>
 <td colspan="4">Supported Version Ranges</td>
 </tr>
 <tr>
 <td>handover_group6</td>
 <td><code class="docutils literal notranslate">v6.4.0 -> v6.4.0 </code></td>
 <td><code class="docutils literal notranslate">v6.4.4 -> v7.0.8 </code></td>
 <td><code class="docutils literal notranslate">v7.2.0 -> v7.2.4 </code></td>
 <td><code class="docutils literal notranslate">v7.4.3 -> 7.6.0 </code></td>
 </tr>
 </table>
 </div>
 </li>
        <li> <span class="li-head">ie_allow_list_v0v1</span> - IE allow list. Source gtp.ie-allow-list.name. <span class="li-normal">type: str</span>
 <a id='label70' href="javascript:ContentClick('label71', 'label70');" onmouseover="ContentPreview('label71');" onmouseout="ContentUnpreview('label71');" title="click to collapse or expand..."> more... </a>
 <div id="label71" style="display:none">
 <table border="1">
 <tr>
 <td></td>
 <td colspan="3">Supported Version Ranges</td>
 </tr>
 <tr>
 <td>ie_allow_list_v0v1</td>
 <td><code class="docutils literal notranslate">v7.0.0 -> v7.0.8 </code></td>
 <td><code class="docutils literal notranslate">v7.2.0 -> v7.2.4 </code></td>
 <td><code class="docutils literal notranslate">v7.4.3 -> 7.6.0 </code></td>
 </tr>
 </table>
 </div>
 </li>
        <li> <span class="li-head">ie_allow_list_v2</span> - IE allow list. Source gtp.ie-allow-list.name. <span class="li-normal">type: str</span>
 <a id='label72' href="javascript:ContentClick('label73', 'label72');" onmouseover="ContentPreview('label73');" onmouseout="ContentUnpreview('label73');" title="click to collapse or expand..."> more... </a>
 <div id="label73" style="display:none">
 <table border="1">
 <tr>
 <td></td>
 <td colspan="3">Supported Version Ranges</td>
 </tr>
 <tr>
 <td>ie_allow_list_v2</td>
 <td><code class="docutils literal notranslate">v7.0.0 -> v7.0.8 </code></td>
 <td><code class="docutils literal notranslate">v7.2.0 -> v7.2.4 </code></td>
 <td><code class="docutils literal notranslate">v7.4.3 -> 7.6.0 </code></td>
 </tr>
 </table>
 </div>
 </li>
        <li> <span class="li-head">ie_remove_policy</span> - IE remove policy. <span class="li-normal">type: list</span> <span style="font-family:'Courier New'" class="li-required">member_path: ie_remove_policy:id</span>
 <a id='label74' href="javascript:ContentClick('label75', 'label74');" onmouseover="ContentPreview('label75');" onmouseout="ContentUnpreview('label75');" title="click to collapse or expand..."> more... </a>
 <div id="label75" style="display:none">
 <table border="1">
 <tr>
 <td></td><td colspan="3">Supported Version Ranges</td>
 </tr>
 <tr>
 <td>ie_remove_policy</td>
 <td><code class="docutils literal notranslate">v6.0.0 -> v7.0.8 </code></td>
 <td><code class="docutils literal notranslate">v7.2.0 -> v7.2.4 </code></td>
 <td><code class="docutils literal notranslate">v7.4.3 -> 7.6.0 </code></td>
 </tr>
 </table>
 </div>
 </li>
            <ul class="ul-self">
            <li> <span class="li-head">id</span> - ID. see <a href='#notes'>Notes</a>. <span class="li-normal">type: int</span> <span class="li-required">required: true</span>
 <a id='label76' href="javascript:ContentClick('label77', 'label76');" onmouseover="ContentPreview('label77');" onmouseout="ContentUnpreview('label77');" title="click to collapse or expand..."> more... </a>
 <div id="label77" style="display:none">
 <table border="1">
 <tr>
 <td></td>
 <td colspan="3">Supported Version Ranges</td>
 </tr>
 <tr>
 <td>id</td>
 <td><code class="docutils literal notranslate">v6.0.0 -> v7.0.8 </code></td>
 <td><code class="docutils literal notranslate">v7.2.0 -> v7.2.4 </code></td>
 <td><code class="docutils literal notranslate">v7.4.3 -> 7.6.0 </code></td>
 </tr>
 </table>
 </div>
 </li>
            <li> <span class="li-head">remove_ies</span> - GTP IEs to be removed. <span class="li-normal">type: list</span> <span class="li-normal">choices: apn-restriction, rat-type, rai, uli, imei</span>
 <a id='label78' href="javascript:ContentClick('label79', 'label78');" onmouseover="ContentPreview('label79');" onmouseout="ContentUnpreview('label79');" title="click to collapse or expand..."> more... </a>
 <div id="label79" style="display:none">
 <table border="1">
 <tr>
 <td></td>
 <td colspan="3">Supported Version Ranges</td>
 </tr>
 <tr>
 <td>remove_ies</td>
 <td><code class="docutils literal notranslate">v6.0.0 -> v7.0.8 </code></td>
 <td><code class="docutils literal notranslate">v7.2.0 -> v7.2.4 </code></td>
 <td><code class="docutils literal notranslate">v7.4.3 -> 7.6.0 </code></td>
 </tr>
 <tr>
 <td>[apn-restriction]</td>
 <td><code class="docutils literal notranslate">v6.0.0 -> v7.0.8</code></td>
 <tr>
 <td>[rat-type]</td>
 <td><code class="docutils literal notranslate">v6.0.0 -> v7.0.8</code></td>
 <tr>
 <td>[rai]</td>
 <td><code class="docutils literal notranslate">v6.0.0 -> v7.0.8</code></td>
 <tr>
 <td>[uli]</td>
 <td><code class="docutils literal notranslate">v6.0.0 -> v7.0.8</code></td>
 <tr>
 <td>[imei]</td>
 <td><code class="docutils literal notranslate">v6.0.0 -> v7.0.8</code></td>
 </table>
 </div>
 </li>
            <li> <span class="li-head">sgsn_addr</span> - SGSN address name. Source firewall.address.name firewall.addrgrp.name. <span class="li-normal">type: str</span>
 <a id='label80' href="javascript:ContentClick('label81', 'label80');" onmouseover="ContentPreview('label81');" onmouseout="ContentUnpreview('label81');" title="click to collapse or expand..."> more... </a>
 <div id="label81" style="display:none">
 <table border="1">
 <tr>
 <td></td>
 <td colspan="3">Supported Version Ranges</td>
 </tr>
 <tr>
 <td>sgsn_addr</td>
 <td><code class="docutils literal notranslate">v6.0.0 -> v7.0.8 </code></td>
 <td><code class="docutils literal notranslate">v7.2.0 -> v7.2.4 </code></td>
 <td><code class="docutils literal notranslate">v7.4.3 -> 7.6.0 </code></td>
 </tr>
 </table>
 </div>
 </li>
            <li> <span class="li-head">sgsn_addr6</span> - SGSN IPv6 address name. Source firewall.address6.name firewall.addrgrp6.name. <span class="li-normal">type: str</span>
 <a id='label82' href="javascript:ContentClick('label83', 'label82');" onmouseover="ContentPreview('label83');" onmouseout="ContentUnpreview('label83');" title="click to collapse or expand..."> more... </a>
 <div id="label83" style="display:none">
 <table border="1">
 <tr>
 <td></td>
 <td colspan="4">Supported Version Ranges</td>
 </tr>
 <tr>
 <td>sgsn_addr6</td>
 <td><code class="docutils literal notranslate">v6.4.0 -> v6.4.0 </code></td>
 <td><code class="docutils literal notranslate">v6.4.4 -> v7.0.8 </code></td>
 <td><code class="docutils literal notranslate">v7.2.0 -> v7.2.4 </code></td>
 <td><code class="docutils literal notranslate">v7.4.3 -> 7.6.0 </code></td>
 </tr>
 </table>
 </div>
 </li>
            </ul>
        <li> <span class="li-head">ie_remover</span> - IE removal policy. <span class="li-normal">type: str</span> <span class="li-normal">choices: enable, disable</span>
 <a id='label84' href="javascript:ContentClick('label85', 'label84');" onmouseover="ContentPreview('label85');" onmouseout="ContentUnpreview('label85');" title="click to collapse or expand..."> more... </a>
 <div id="label85" style="display:none">
 <table border="1">
 <tr>
 <td></td>
 <td colspan="3">Supported Version Ranges</td>
 </tr>
 <tr>
 <td>ie_remover</td>
 <td><code class="docutils literal notranslate">v6.0.0 -> v7.0.8 </code></td>
 <td><code class="docutils literal notranslate">v7.2.0 -> v7.2.4 </code></td>
 <td><code class="docutils literal notranslate">v7.4.3 -> 7.6.0 </code></td>
 </tr>
 <tr>
 <td>[enable]</td>
 <td><code class="docutils literal notranslate">v6.0.0 -> v7.0.8</code></td>
 <tr>
 <td>[disable]</td>
 <td><code class="docutils literal notranslate">v6.0.0 -> v7.0.8</code></td>
 </table>
 </div>
 </li>
        <li> <span class="li-head">ie_validation</span> - IE validation. <span class="li-normal">type: dict</span>
 <a id='label86' href="javascript:ContentClick('label87', 'label86');" onmouseover="ContentPreview('label87');" onmouseout="ContentUnpreview('label87');" title="click to collapse or expand..."> more... </a>
 <div id="label87" style="display:none">
 <table border="1">
 <tr>
 <td></td><td colspan="3">Supported Version Ranges</td>
 </tr>
 <tr>
 <td>ie_validation</td>
 <td><code class="docutils literal notranslate">v6.0.0 -> v7.0.8 </code></td>
 <td><code class="docutils literal notranslate">v7.2.0 -> v7.2.4 </code></td>
 <td><code class="docutils literal notranslate">v7.4.3 -> 7.6.0 </code></td>
 </tr>
 </table>
 </div>
 </li>
            <ul class="ul-self">
            <li> <span class="li-head">apn_restriction</span> - Validate APN restriction. <span class="li-normal">type: str</span> <span class="li-normal">choices: enable, disable</span>
 <a id='label88' href="javascript:ContentClick('label89', 'label88');" onmouseover="ContentPreview('label89');" onmouseout="ContentUnpreview('label89');" title="click to collapse or expand..."> more... </a>
 <div id="label89" style="display:none">
 <table border="1">
 <tr>
 <td></td>
 <td colspan="3">Supported Version Ranges</td>
 </tr>
 <tr>
 <td>apn_restriction</td>
 <td><code class="docutils literal notranslate">v6.0.0 -> v7.0.8 </code></td>
 <td><code class="docutils literal notranslate">v7.2.0 -> v7.2.4 </code></td>
 <td><code class="docutils literal notranslate">v7.4.3 -> 7.6.0 </code></td>
 </tr>
 <tr>
 <td>[enable]</td>
 <td><code class="docutils literal notranslate">v6.0.0 -> v7.0.8</code></td>
 <tr>
 <td>[disable]</td>
 <td><code class="docutils literal notranslate">v6.0.0 -> v7.0.8</code></td>
 </table>
 </div>
 </li>
            <li> <span class="li-head">charging_gateway_addr</span> - Validate charging gateway address. <span class="li-normal">type: str</span> <span class="li-normal">choices: enable, disable</span>
 <a id='label90' href="javascript:ContentClick('label91', 'label90');" onmouseover="ContentPreview('label91');" onmouseout="ContentUnpreview('label91');" title="click to collapse or expand..."> more... </a>
 <div id="label91" style="display:none">
 <table border="1">
 <tr>
 <td></td>
 <td colspan="3">Supported Version Ranges</td>
 </tr>
 <tr>
 <td>charging_gateway_addr</td>
 <td><code class="docutils literal notranslate">v6.0.0 -> v7.0.8 </code></td>
 <td><code class="docutils literal notranslate">v7.2.0 -> v7.2.4 </code></td>
 <td><code class="docutils literal notranslate">v7.4.3 -> 7.6.0 </code></td>
 </tr>
 <tr>
 <td>[enable]</td>
 <td><code class="docutils literal notranslate">v6.0.0 -> v7.0.8</code></td>
 <tr>
 <td>[disable]</td>
 <td><code class="docutils literal notranslate">v6.0.0 -> v7.0.8</code></td>
 </table>
 </div>
 </li>
            <li> <span class="li-head">charging_ID</span> - Validate charging ID. <span class="li-normal">type: str</span> <span class="li-normal">choices: enable, disable</span>
 <a id='label92' href="javascript:ContentClick('label93', 'label92');" onmouseover="ContentPreview('label93');" onmouseout="ContentUnpreview('label93');" title="click to collapse or expand..."> more... </a>
 <div id="label93" style="display:none">
 <table border="1">
 <tr>
 <td></td>
 <td colspan="3">Supported Version Ranges</td>
 </tr>
 <tr>
 <td>charging_ID</td>
 <td><code class="docutils literal notranslate">v6.0.0 -> v7.0.8 </code></td>
 <td><code class="docutils literal notranslate">v7.2.0 -> v7.2.4 </code></td>
 <td><code class="docutils literal notranslate">v7.4.3 -> 7.6.0 </code></td>
 </tr>
 <tr>
 <td>[enable]</td>
 <td><code class="docutils literal notranslate">v6.0.0 -> v7.0.8</code></td>
 <tr>
 <td>[disable]</td>
 <td><code class="docutils literal notranslate">v6.0.0 -> v7.0.8</code></td>
 </table>
 </div>
 </li>
            <li> <span class="li-head">end_user_addr</span> - Validate end user address. <span class="li-normal">type: str</span> <span class="li-normal">choices: enable, disable</span>
 <a id='label94' href="javascript:ContentClick('label95', 'label94');" onmouseover="ContentPreview('label95');" onmouseout="ContentUnpreview('label95');" title="click to collapse or expand..."> more... </a>
 <div id="label95" style="display:none">
 <table border="1">
 <tr>
 <td></td>
 <td colspan="3">Supported Version Ranges</td>
 </tr>
 <tr>
 <td>end_user_addr</td>
 <td><code class="docutils literal notranslate">v6.0.0 -> v7.0.8 </code></td>
 <td><code class="docutils literal notranslate">v7.2.0 -> v7.2.4 </code></td>
 <td><code class="docutils literal notranslate">v7.4.3 -> 7.6.0 </code></td>
 </tr>
 <tr>
 <td>[enable]</td>
 <td><code class="docutils literal notranslate">v6.0.0 -> v7.0.8</code></td>
 <tr>
 <td>[disable]</td>
 <td><code class="docutils literal notranslate">v6.0.0 -> v7.0.8</code></td>
 </table>
 </div>
 </li>
            <li> <span class="li-head">gsn_addr</span> - Validate GSN address. <span class="li-normal">type: str</span> <span class="li-normal">choices: enable, disable</span>
 <a id='label96' href="javascript:ContentClick('label97', 'label96');" onmouseover="ContentPreview('label97');" onmouseout="ContentUnpreview('label97');" title="click to collapse or expand..."> more... </a>
 <div id="label97" style="display:none">
 <table border="1">
 <tr>
 <td></td>
 <td colspan="3">Supported Version Ranges</td>
 </tr>
 <tr>
 <td>gsn_addr</td>
 <td><code class="docutils literal notranslate">v6.0.0 -> v7.0.8 </code></td>
 <td><code class="docutils literal notranslate">v7.2.0 -> v7.2.4 </code></td>
 <td><code class="docutils literal notranslate">v7.4.3 -> 7.6.0 </code></td>
 </tr>
 <tr>
 <td>[enable]</td>
 <td><code class="docutils literal notranslate">v6.0.0 -> v7.0.8</code></td>
 <tr>
 <td>[disable]</td>
 <td><code class="docutils literal notranslate">v6.0.0 -> v7.0.8</code></td>
 </table>
 </div>
 </li>
            <li> <span class="li-head">imei</span> - Validate IMEI(SV). <span class="li-normal">type: str</span> <span class="li-normal">choices: enable, disable</span>
 <a id='label98' href="javascript:ContentClick('label99', 'label98');" onmouseover="ContentPreview('label99');" onmouseout="ContentUnpreview('label99');" title="click to collapse or expand..."> more... </a>
 <div id="label99" style="display:none">
 <table border="1">
 <tr>
 <td></td>
 <td colspan="3">Supported Version Ranges</td>
 </tr>
 <tr>
 <td>imei</td>
 <td><code class="docutils literal notranslate">v6.0.0 -> v7.0.8 </code></td>
 <td><code class="docutils literal notranslate">v7.2.0 -> v7.2.4 </code></td>
 <td><code class="docutils literal notranslate">v7.4.3 -> 7.6.0 </code></td>
 </tr>
 <tr>
 <td>[enable]</td>
 <td><code class="docutils literal notranslate">v6.0.0 -> v7.0.8</code></td>
 <tr>
 <td>[disable]</td>
 <td><code class="docutils literal notranslate">v6.0.0 -> v7.0.8</code></td>
 </table>
 </div>
 </li>
            <li> <span class="li-head">imsi</span> - Validate IMSI. <span class="li-normal">type: str</span> <span class="li-normal">choices: enable, disable</span>
 <a id='label100' href="javascript:ContentClick('label101', 'label100');" onmouseover="ContentPreview('label101');" onmouseout="ContentUnpreview('label101');" title="click to collapse or expand..."> more... </a>
 <div id="label101" style="display:none">
 <table border="1">
 <tr>
 <td></td>
 <td colspan="3">Supported Version Ranges</td>
 </tr>
 <tr>
 <td>imsi</td>
 <td><code class="docutils literal notranslate">v6.0.0 -> v7.0.8 </code></td>
 <td><code class="docutils literal notranslate">v7.2.0 -> v7.2.4 </code></td>
 <td><code class="docutils literal notranslate">v7.4.3 -> 7.6.0 </code></td>
 </tr>
 <tr>
 <td>[enable]</td>
 <td><code class="docutils literal notranslate">v6.0.0 -> v7.0.8</code></td>
 <tr>
 <td>[disable]</td>
 <td><code class="docutils literal notranslate">v6.0.0 -> v7.0.8</code></td>
 </table>
 </div>
 </li>
            <li> <span class="li-head">mm_context</span> - Validate MM context. <span class="li-normal">type: str</span> <span class="li-normal">choices: enable, disable</span>
 <a id='label102' href="javascript:ContentClick('label103', 'label102');" onmouseover="ContentPreview('label103');" onmouseout="ContentUnpreview('label103');" title="click to collapse or expand..."> more... </a>
 <div id="label103" style="display:none">
 <table border="1">
 <tr>
 <td></td>
 <td colspan="3">Supported Version Ranges</td>
 </tr>
 <tr>
 <td>mm_context</td>
 <td><code class="docutils literal notranslate">v6.0.0 -> v7.0.8 </code></td>
 <td><code class="docutils literal notranslate">v7.2.0 -> v7.2.4 </code></td>
 <td><code class="docutils literal notranslate">v7.4.3 -> 7.6.0 </code></td>
 </tr>
 <tr>
 <td>[enable]</td>
 <td><code class="docutils literal notranslate">v6.0.0 -> v7.0.8</code></td>
 <tr>
 <td>[disable]</td>
 <td><code class="docutils literal notranslate">v6.0.0 -> v7.0.8</code></td>
 </table>
 </div>
 </li>
            <li> <span class="li-head">ms_tzone</span> - Validate MS time zone. <span class="li-normal">type: str</span> <span class="li-normal">choices: enable, disable</span>
 <a id='label104' href="javascript:ContentClick('label105', 'label104');" onmouseover="ContentPreview('label105');" onmouseout="ContentUnpreview('label105');" title="click to collapse or expand..."> more... </a>
 <div id="label105" style="display:none">
 <table border="1">
 <tr>
 <td></td>
 <td colspan="3">Supported Version Ranges</td>
 </tr>
 <tr>
 <td>ms_tzone</td>
 <td><code class="docutils literal notranslate">v6.0.0 -> v7.0.8 </code></td>
 <td><code class="docutils literal notranslate">v7.2.0 -> v7.2.4 </code></td>
 <td><code class="docutils literal notranslate">v7.4.3 -> 7.6.0 </code></td>
 </tr>
 <tr>
 <td>[enable]</td>
 <td><code class="docutils literal notranslate">v6.0.0 -> v7.0.8</code></td>
 <tr>
 <td>[disable]</td>
 <td><code class="docutils literal notranslate">v6.0.0 -> v7.0.8</code></td>
 </table>
 </div>
 </li>
            <li> <span class="li-head">ms_validated</span> - Validate MS validated. <span class="li-normal">type: str</span> <span class="li-normal">choices: enable, disable</span>
 <a id='label106' href="javascript:ContentClick('label107', 'label106');" onmouseover="ContentPreview('label107');" onmouseout="ContentUnpreview('label107');" title="click to collapse or expand..."> more... </a>
 <div id="label107" style="display:none">
 <table border="1">
 <tr>
 <td></td>
 <td colspan="3">Supported Version Ranges</td>
 </tr>
 <tr>
 <td>ms_validated</td>
 <td><code class="docutils literal notranslate">v6.0.0 -> v7.0.8 </code></td>
 <td><code class="docutils literal notranslate">v7.2.0 -> v7.2.4 </code></td>
 <td><code class="docutils literal notranslate">v7.4.3 -> 7.6.0 </code></td>
 </tr>
 <tr>
 <td>[enable]</td>
 <td><code class="docutils literal notranslate">v6.0.0 -> v7.0.8</code></td>
 <tr>
 <td>[disable]</td>
 <td><code class="docutils literal notranslate">v6.0.0 -> v7.0.8</code></td>
 </table>
 </div>
 </li>
            <li> <span class="li-head">msisdn</span> - Validate MSISDN. <span class="li-normal">type: str</span> <span class="li-normal">choices: enable, disable</span>
 <a id='label108' href="javascript:ContentClick('label109', 'label108');" onmouseover="ContentPreview('label109');" onmouseout="ContentUnpreview('label109');" title="click to collapse or expand..."> more... </a>
 <div id="label109" style="display:none">
 <table border="1">
 <tr>
 <td></td>
 <td colspan="3">Supported Version Ranges</td>
 </tr>
 <tr>
 <td>msisdn</td>
 <td><code class="docutils literal notranslate">v6.0.0 -> v7.0.8 </code></td>
 <td><code class="docutils literal notranslate">v7.2.0 -> v7.2.4 </code></td>
 <td><code class="docutils literal notranslate">v7.4.3 -> 7.6.0 </code></td>
 </tr>
 <tr>
 <td>[enable]</td>
 <td><code class="docutils literal notranslate">v6.0.0 -> v7.0.8</code></td>
 <tr>
 <td>[disable]</td>
 <td><code class="docutils literal notranslate">v6.0.0 -> v7.0.8</code></td>
 </table>
 </div>
 </li>
            <li> <span class="li-head">nsapi</span> - Validate NSAPI. <span class="li-normal">type: str</span> <span class="li-normal">choices: enable, disable</span>
 <a id='label110' href="javascript:ContentClick('label111', 'label110');" onmouseover="ContentPreview('label111');" onmouseout="ContentUnpreview('label111');" title="click to collapse or expand..."> more... </a>
 <div id="label111" style="display:none">
 <table border="1">
 <tr>
 <td></td>
 <td colspan="3">Supported Version Ranges</td>
 </tr>
 <tr>
 <td>nsapi</td>
 <td><code class="docutils literal notranslate">v6.0.0 -> v7.0.8 </code></td>
 <td><code class="docutils literal notranslate">v7.2.0 -> v7.2.4 </code></td>
 <td><code class="docutils literal notranslate">v7.4.3 -> 7.6.0 </code></td>
 </tr>
 <tr>
 <td>[enable]</td>
 <td><code class="docutils literal notranslate">v6.0.0 -> v7.0.8</code></td>
 <tr>
 <td>[disable]</td>
 <td><code class="docutils literal notranslate">v6.0.0 -> v7.0.8</code></td>
 </table>
 </div>
 </li>
            <li> <span class="li-head">pdp_context</span> - Validate PDP context. <span class="li-normal">type: str</span> <span class="li-normal">choices: enable, disable</span>
 <a id='label112' href="javascript:ContentClick('label113', 'label112');" onmouseover="ContentPreview('label113');" onmouseout="ContentUnpreview('label113');" title="click to collapse or expand..."> more... </a>
 <div id="label113" style="display:none">
 <table border="1">
 <tr>
 <td></td>
 <td colspan="3">Supported Version Ranges</td>
 </tr>
 <tr>
 <td>pdp_context</td>
 <td><code class="docutils literal notranslate">v6.0.0 -> v7.0.8 </code></td>
 <td><code class="docutils literal notranslate">v7.2.0 -> v7.2.4 </code></td>
 <td><code class="docutils literal notranslate">v7.4.3 -> 7.6.0 </code></td>
 </tr>
 <tr>
 <td>[enable]</td>
 <td><code class="docutils literal notranslate">v6.0.0 -> v7.0.8</code></td>
 <tr>
 <td>[disable]</td>
 <td><code class="docutils literal notranslate">v6.0.0 -> v7.0.8</code></td>
 </table>
 </div>
 </li>
            <li> <span class="li-head">qos_profile</span> - Validate Quality of Service(QoS) profile. <span class="li-normal">type: str</span> <span class="li-normal">choices: enable, disable</span>
 <a id='label114' href="javascript:ContentClick('label115', 'label114');" onmouseover="ContentPreview('label115');" onmouseout="ContentUnpreview('label115');" title="click to collapse or expand..."> more... </a>
 <div id="label115" style="display:none">
 <table border="1">
 <tr>
 <td></td>
 <td colspan="3">Supported Version Ranges</td>
 </tr>
 <tr>
 <td>qos_profile</td>
 <td><code class="docutils literal notranslate">v6.0.0 -> v7.0.8 </code></td>
 <td><code class="docutils literal notranslate">v7.2.0 -> v7.2.4 </code></td>
 <td><code class="docutils literal notranslate">v7.4.3 -> 7.6.0 </code></td>
 </tr>
 <tr>
 <td>[enable]</td>
 <td><code class="docutils literal notranslate">v6.0.0 -> v7.0.8</code></td>
 <tr>
 <td>[disable]</td>
 <td><code class="docutils literal notranslate">v6.0.0 -> v7.0.8</code></td>
 </table>
 </div>
 </li>
            <li> <span class="li-head">rai</span> - Validate RAI. <span class="li-normal">type: str</span> <span class="li-normal">choices: enable, disable</span>
 <a id='label116' href="javascript:ContentClick('label117', 'label116');" onmouseover="ContentPreview('label117');" onmouseout="ContentUnpreview('label117');" title="click to collapse or expand..."> more... </a>
 <div id="label117" style="display:none">
 <table border="1">
 <tr>
 <td></td>
 <td colspan="3">Supported Version Ranges</td>
 </tr>
 <tr>
 <td>rai</td>
 <td><code class="docutils literal notranslate">v6.0.0 -> v7.0.8 </code></td>
 <td><code class="docutils literal notranslate">v7.2.0 -> v7.2.4 </code></td>
 <td><code class="docutils literal notranslate">v7.4.3 -> 7.6.0 </code></td>
 </tr>
 <tr>
 <td>[enable]</td>
 <td><code class="docutils literal notranslate">v6.0.0 -> v7.0.8</code></td>
 <tr>
 <td>[disable]</td>
 <td><code class="docutils literal notranslate">v6.0.0 -> v7.0.8</code></td>
 </table>
 </div>
 </li>
            <li> <span class="li-head">rat_type</span> - Validate RAT type. <span class="li-normal">type: str</span> <span class="li-normal">choices: enable, disable</span>
 <a id='label118' href="javascript:ContentClick('label119', 'label118');" onmouseover="ContentPreview('label119');" onmouseout="ContentUnpreview('label119');" title="click to collapse or expand..."> more... </a>
 <div id="label119" style="display:none">
 <table border="1">
 <tr>
 <td></td>
 <td colspan="3">Supported Version Ranges</td>
 </tr>
 <tr>
 <td>rat_type</td>
 <td><code class="docutils literal notranslate">v6.0.0 -> v7.0.8 </code></td>
 <td><code class="docutils literal notranslate">v7.2.0 -> v7.2.4 </code></td>
 <td><code class="docutils literal notranslate">v7.4.3 -> 7.6.0 </code></td>
 </tr>
 <tr>
 <td>[enable]</td>
 <td><code class="docutils literal notranslate">v6.0.0 -> v7.0.8</code></td>
 <tr>
 <td>[disable]</td>
 <td><code class="docutils literal notranslate">v6.0.0 -> v7.0.8</code></td>
 </table>
 </div>
 </li>
            <li> <span class="li-head">reordering_required</span> - Validate re-ordering required. <span class="li-normal">type: str</span> <span class="li-normal">choices: enable, disable</span>
 <a id='label120' href="javascript:ContentClick('label121', 'label120');" onmouseover="ContentPreview('label121');" onmouseout="ContentUnpreview('label121');" title="click to collapse or expand..."> more... </a>
 <div id="label121" style="display:none">
 <table border="1">
 <tr>
 <td></td>
 <td colspan="3">Supported Version Ranges</td>
 </tr>
 <tr>
 <td>reordering_required</td>
 <td><code class="docutils literal notranslate">v6.0.0 -> v7.0.8 </code></td>
 <td><code class="docutils literal notranslate">v7.2.0 -> v7.2.4 </code></td>
 <td><code class="docutils literal notranslate">v7.4.3 -> 7.6.0 </code></td>
 </tr>
 <tr>
 <td>[enable]</td>
 <td><code class="docutils literal notranslate">v6.0.0 -> v7.0.8</code></td>
 <tr>
 <td>[disable]</td>
 <td><code class="docutils literal notranslate">v6.0.0 -> v7.0.8</code></td>
 </table>
 </div>
 </li>
            <li> <span class="li-head">selection_mode</span> - Validate selection mode. <span class="li-normal">type: str</span> <span class="li-normal">choices: enable, disable</span>
 <a id='label122' href="javascript:ContentClick('label123', 'label122');" onmouseover="ContentPreview('label123');" onmouseout="ContentUnpreview('label123');" title="click to collapse or expand..."> more... </a>
 <div id="label123" style="display:none">
 <table border="1">
 <tr>
 <td></td>
 <td colspan="3">Supported Version Ranges</td>
 </tr>
 <tr>
 <td>selection_mode</td>
 <td><code class="docutils literal notranslate">v6.0.0 -> v7.0.8 </code></td>
 <td><code class="docutils literal notranslate">v7.2.0 -> v7.2.4 </code></td>
 <td><code class="docutils literal notranslate">v7.4.3 -> 7.6.0 </code></td>
 </tr>
 <tr>
 <td>[enable]</td>
 <td><code class="docutils literal notranslate">v6.0.0 -> v7.0.8</code></td>
 <tr>
 <td>[disable]</td>
 <td><code class="docutils literal notranslate">v6.0.0 -> v7.0.8</code></td>
 </table>
 </div>
 </li>
            <li> <span class="li-head">uli</span> - Validate user location information. <span class="li-normal">type: str</span> <span class="li-normal">choices: enable, disable</span>
 <a id='label124' href="javascript:ContentClick('label125', 'label124');" onmouseover="ContentPreview('label125');" onmouseout="ContentUnpreview('label125');" title="click to collapse or expand..."> more... </a>
 <div id="label125" style="display:none">
 <table border="1">
 <tr>
 <td></td>
 <td colspan="3">Supported Version Ranges</td>
 </tr>
 <tr>
 <td>uli</td>
 <td><code class="docutils literal notranslate">v6.0.0 -> v7.0.8 </code></td>
 <td><code class="docutils literal notranslate">v7.2.0 -> v7.2.4 </code></td>
 <td><code class="docutils literal notranslate">v7.4.3 -> 7.6.0 </code></td>
 </tr>
 <tr>
 <td>[enable]</td>
 <td><code class="docutils literal notranslate">v6.0.0 -> v7.0.8</code></td>
 <tr>
 <td>[disable]</td>
 <td><code class="docutils literal notranslate">v6.0.0 -> v7.0.8</code></td>
 </table>
 </div>
 </li>
            </ul>
        <li> <span class="li-head">ie_white_list_v0v1</span> - IE white list. Source gtp.ie-white-list.name. <span class="li-normal">type: str</span>
 <a id='label126' href="javascript:ContentClick('label127', 'label126');" onmouseover="ContentPreview('label127');" onmouseout="ContentUnpreview('label127');" title="click to collapse or expand..."> more... </a>
 <div id="label127" style="display:none">
 <table border="1">
 <tr>
 <td></td>
 <td colspan="1">Supported Version Ranges</td>
 </tr>
 <tr>
 <td>ie_white_list_v0v1</td>
 <td><code class="docutils literal notranslate">v6.0.0 -> v6.4.4 </code></td>
 </tr>
 </table>
 </div>
 </li>
        <li> <span class="li-head">ie_white_list_v2</span> - IE white list. Source gtp.ie-white-list.name. <span class="li-normal">type: str</span>
 <a id='label128' href="javascript:ContentClick('label129', 'label128');" onmouseover="ContentPreview('label129');" onmouseout="ContentUnpreview('label129');" title="click to collapse or expand..."> more... </a>
 <div id="label129" style="display:none">
 <table border="1">
 <tr>
 <td></td>
 <td colspan="1">Supported Version Ranges</td>
 </tr>
 <tr>
 <td>ie_white_list_v2</td>
 <td><code class="docutils literal notranslate">v6.0.0 -> v6.4.4 </code></td>
 </tr>
 </table>
 </div>
 </li>
        <li> <span class="li-head">imsi</span> - IMSI. <span class="li-normal">type: list</span> <span style="font-family:'Courier New'" class="li-required">member_path: imsi:id</span>
 <a id='label130' href="javascript:ContentClick('label131', 'label130');" onmouseover="ContentPreview('label131');" onmouseout="ContentUnpreview('label131');" title="click to collapse or expand..."> more... </a>
 <div id="label131" style="display:none">
 <table border="1">
 <tr>
 <td></td><td colspan="3">Supported Version Ranges</td>
 </tr>
 <tr>
 <td>imsi</td>
 <td><code class="docutils literal notranslate">v6.0.0 -> v7.0.8 </code></td>
 <td><code class="docutils literal notranslate">v7.2.0 -> v7.2.4 </code></td>
 <td><code class="docutils literal notranslate">v7.4.3 -> 7.6.0 </code></td>
 </tr>
 </table>
 </div>
 </li>
            <ul class="ul-self">
            <li> <span class="li-head">action</span> - Action. <span class="li-normal">type: str</span> <span class="li-normal">choices: allow, deny</span>
 <a id='label132' href="javascript:ContentClick('label133', 'label132');" onmouseover="ContentPreview('label133');" onmouseout="ContentUnpreview('label133');" title="click to collapse or expand..."> more... </a>
 <div id="label133" style="display:none">
 <table border="1">
 <tr>
 <td></td>
 <td colspan="3">Supported Version Ranges</td>
 </tr>
 <tr>
 <td>action</td>
 <td><code class="docutils literal notranslate">v6.0.0 -> v7.0.8 </code></td>
 <td><code class="docutils literal notranslate">v7.2.0 -> v7.2.4 </code></td>
 <td><code class="docutils literal notranslate">v7.4.3 -> 7.6.0 </code></td>
 </tr>
 <tr>
 <td>[allow]</td>
 <td><code class="docutils literal notranslate">v6.0.0 -> v7.0.8</code></td>
 <tr>
 <td>[deny]</td>
 <td><code class="docutils literal notranslate">v6.0.0 -> v7.0.8</code></td>
 </table>
 </div>
 </li>
            <li> <span class="li-head">apnmember</span> - APN member. <span class="li-normal">type: list</span> <span style="font-family:'Courier New'" class="li-required">member_path: imsi:id/apnmember:name</span>
 <a id='label134' href="javascript:ContentClick('label135', 'label134');" onmouseover="ContentPreview('label135');" onmouseout="ContentUnpreview('label135');" title="click to collapse or expand..."> more... </a>
 <div id="label135" style="display:none">
 <table border="1">
 <tr>
 <td></td><td colspan="3">Supported Version Ranges</td>
 </tr>
 <tr>
 <td>apnmember</td>
 <td><code class="docutils literal notranslate">v6.0.0 -> v7.0.8 </code></td>
 <td><code class="docutils literal notranslate">v7.2.0 -> v7.2.4 </code></td>
 <td><code class="docutils literal notranslate">v7.4.3 -> 7.6.0 </code></td>
 </tr>
 </table>
 </div>
 </li>
                <ul class="ul-self">
                <li> <span class="li-head">name</span> - APN name. Source gtp.apn.name gtp.apngrp.name. <span class="li-normal">type: str</span> <span class="li-required">required: true</span>
 <a id='label136' href="javascript:ContentClick('label137', 'label136');" onmouseover="ContentPreview('label137');" onmouseout="ContentUnpreview('label137');" title="click to collapse or expand..."> more... </a>
 <div id="label137" style="display:none">
 <table border="1">
 <tr>
 <td></td>
 <td colspan="3">Supported Version Ranges</td>
 </tr>
 <tr>
 <td>name</td>
 <td><code class="docutils literal notranslate">v6.0.0 -> v7.0.8 </code></td>
 <td><code class="docutils literal notranslate">v7.2.0 -> v7.2.4 </code></td>
 <td><code class="docutils literal notranslate">v7.4.3 -> 7.6.0 </code></td>
 </tr>
 </table>
 </div>
 </li>
                </ul>
            <li> <span class="li-head">id</span> - ID. see <a href='#notes'>Notes</a>. <span class="li-normal">type: int</span> <span class="li-required">required: true</span>
 <a id='label138' href="javascript:ContentClick('label139', 'label138');" onmouseover="ContentPreview('label139');" onmouseout="ContentUnpreview('label139');" title="click to collapse or expand..."> more... </a>
 <div id="label139" style="display:none">
 <table border="1">
 <tr>
 <td></td>
 <td colspan="3">Supported Version Ranges</td>
 </tr>
 <tr>
 <td>id</td>
 <td><code class="docutils literal notranslate">v6.0.0 -> v7.0.8 </code></td>
 <td><code class="docutils literal notranslate">v7.2.0 -> v7.2.4 </code></td>
 <td><code class="docutils literal notranslate">v7.4.3 -> 7.6.0 </code></td>
 </tr>
 </table>
 </div>
 </li>
            <li> <span class="li-head">mcc_mnc</span> - MCC MNC. <span class="li-normal">type: str</span>
 <a id='label140' href="javascript:ContentClick('label141', 'label140');" onmouseover="ContentPreview('label141');" onmouseout="ContentUnpreview('label141');" title="click to collapse or expand..."> more... </a>
 <div id="label141" style="display:none">
 <table border="1">
 <tr>
 <td></td>
 <td colspan="3">Supported Version Ranges</td>
 </tr>
 <tr>
 <td>mcc_mnc</td>
 <td><code class="docutils literal notranslate">v6.0.0 -> v7.0.8 </code></td>
 <td><code class="docutils literal notranslate">v7.2.0 -> v7.2.4 </code></td>
 <td><code class="docutils literal notranslate">v7.4.3 -> 7.6.0 </code></td>
 </tr>
 </table>
 </div>
 </li>
            <li> <span class="li-head">msisdn_prefix</span> - MSISDN prefix. <span class="li-normal">type: str</span>
 <a id='label142' href="javascript:ContentClick('label143', 'label142');" onmouseover="ContentPreview('label143');" onmouseout="ContentUnpreview('label143');" title="click to collapse or expand..."> more... </a>
 <div id="label143" style="display:none">
 <table border="1">
 <tr>
 <td></td>
 <td colspan="3">Supported Version Ranges</td>
 </tr>
 <tr>
 <td>msisdn_prefix</td>
 <td><code class="docutils literal notranslate">v6.0.0 -> v7.0.8 </code></td>
 <td><code class="docutils literal notranslate">v7.2.0 -> v7.2.4 </code></td>
 <td><code class="docutils literal notranslate">v7.4.3 -> 7.6.0 </code></td>
 </tr>
 </table>
 </div>
 </li>
            <li> <span class="li-head">selection_mode</span> - APN selection mode. <span class="li-normal">type: list</span> <span class="li-normal">choices: ms, net, vrf</span>
 <a id='label144' href="javascript:ContentClick('label145', 'label144');" onmouseover="ContentPreview('label145');" onmouseout="ContentUnpreview('label145');" title="click to collapse or expand..."> more... </a>
 <div id="label145" style="display:none">
 <table border="1">
 <tr>
 <td></td>
 <td colspan="3">Supported Version Ranges</td>
 </tr>
 <tr>
 <td>selection_mode</td>
 <td><code class="docutils literal notranslate">v6.0.0 -> v7.0.8 </code></td>
 <td><code class="docutils literal notranslate">v7.2.0 -> v7.2.4 </code></td>
 <td><code class="docutils literal notranslate">v7.4.3 -> 7.6.0 </code></td>
 </tr>
 <tr>
 <td>[ms]</td>
 <td><code class="docutils literal notranslate">v6.0.0 -> v7.0.8</code></td>
 <tr>
 <td>[net]</td>
 <td><code class="docutils literal notranslate">v6.0.0 -> v7.0.8</code></td>
 <tr>
 <td>[vrf]</td>
 <td><code class="docutils literal notranslate">v6.0.0 -> v7.0.8</code></td>
 </table>
 </div>
 </li>
            </ul>
        <li> <span class="li-head">imsi_filter</span> - imsi filter <span class="li-normal">type: str</span> <span class="li-normal">choices: enable, disable</span>
 <a id='label146' href="javascript:ContentClick('label147', 'label146');" onmouseover="ContentPreview('label147');" onmouseout="ContentUnpreview('label147');" title="click to collapse or expand..."> more... </a>
 <div id="label147" style="display:none">
 <table border="1">
 <tr>
 <td></td>
 <td colspan="3">Supported Version Ranges</td>
 </tr>
 <tr>
 <td>imsi_filter</td>
 <td><code class="docutils literal notranslate">v6.0.0 -> v7.0.8 </code></td>
 <td><code class="docutils literal notranslate">v7.2.0 -> v7.2.4 </code></td>
 <td><code class="docutils literal notranslate">v7.4.3 -> 7.6.0 </code></td>
 </tr>
 <tr>
 <td>[enable]</td>
 <td><code class="docutils literal notranslate">v6.0.0 -> v7.0.8</code></td>
 <tr>
 <td>[disable]</td>
 <td><code class="docutils literal notranslate">v6.0.0 -> v7.0.8</code></td>
 </table>
 </div>
 </li>
        <li> <span class="li-head">interface_notify</span> - overbilling interface Source system.interface.name. <span class="li-normal">type: str</span>
 <a id='label148' href="javascript:ContentClick('label149', 'label148');" onmouseover="ContentPreview('label149');" onmouseout="ContentUnpreview('label149');" title="click to collapse or expand..."> more... </a>
 <div id="label149" style="display:none">
 <table border="1">
 <tr>
 <td></td>
 <td colspan="3">Supported Version Ranges</td>
 </tr>
 <tr>
 <td>interface_notify</td>
 <td><code class="docutils literal notranslate">v6.0.0 -> v7.0.8 </code></td>
 <td><code class="docutils literal notranslate">v7.2.0 -> v7.2.4 </code></td>
 <td><code class="docutils literal notranslate">v7.4.3 -> 7.6.0 </code></td>
 </tr>
 </table>
 </div>
 </li>
        <li> <span class="li-head">invalid_reserved_field</span> - Invalid reserved field in GTP header <span class="li-normal">type: str</span> <span class="li-normal">choices: allow, deny</span>
 <a id='label150' href="javascript:ContentClick('label151', 'label150');" onmouseover="ContentPreview('label151');" onmouseout="ContentUnpreview('label151');" title="click to collapse or expand..."> more... </a>
 <div id="label151" style="display:none">
 <table border="1">
 <tr>
 <td></td>
 <td colspan="3">Supported Version Ranges</td>
 </tr>
 <tr>
 <td>invalid_reserved_field</td>
 <td><code class="docutils literal notranslate">v6.0.0 -> v7.0.8 </code></td>
 <td><code class="docutils literal notranslate">v7.2.0 -> v7.2.4 </code></td>
 <td><code class="docutils literal notranslate">v7.4.3 -> 7.6.0 </code></td>
 </tr>
 <tr>
 <td>[allow]</td>
 <td><code class="docutils literal notranslate">v6.0.0 -> v7.0.8</code></td>
 <tr>
 <td>[deny]</td>
 <td><code class="docutils literal notranslate">v6.0.0 -> v7.0.8</code></td>
 </table>
 </div>
 </li>
        <li> <span class="li-head">invalid_sgsns_to_log</span> - Invalid SGSN group to be logged Source firewall.address.name firewall.addrgrp.name. <span class="li-normal">type: str</span>
 <a id='label152' href="javascript:ContentClick('label153', 'label152');" onmouseover="ContentPreview('label153');" onmouseout="ContentUnpreview('label153');" title="click to collapse or expand..."> more... </a>
 <div id="label153" style="display:none">
 <table border="1">
 <tr>
 <td></td>
 <td colspan="3">Supported Version Ranges</td>
 </tr>
 <tr>
 <td>invalid_sgsns_to_log</td>
 <td><code class="docutils literal notranslate">v6.0.0 -> v7.0.8 </code></td>
 <td><code class="docutils literal notranslate">v7.2.0 -> v7.2.4 </code></td>
 <td><code class="docutils literal notranslate">v7.4.3 -> 7.6.0 </code></td>
 </tr>
 </table>
 </div>
 </li>
        <li> <span class="li-head">invalid_sgsns6_to_log</span> - Invalid SGSN IPv6 group to be logged. Source firewall.address6.name firewall.addrgrp6.name. <span class="li-normal">type: str</span>
 <a id='label154' href="javascript:ContentClick('label155', 'label154');" onmouseover="ContentPreview('label155');" onmouseout="ContentUnpreview('label155');" title="click to collapse or expand..."> more... </a>
 <div id="label155" style="display:none">
 <table border="1">
 <tr>
 <td></td>
 <td colspan="4">Supported Version Ranges</td>
 </tr>
 <tr>
 <td>invalid_sgsns6_to_log</td>
 <td><code class="docutils literal notranslate">v6.4.0 -> v6.4.0 </code></td>
 <td><code class="docutils literal notranslate">v6.4.4 -> v7.0.8 </code></td>
 <td><code class="docutils literal notranslate">v7.2.0 -> v7.2.4 </code></td>
 <td><code class="docutils literal notranslate">v7.4.3 -> 7.6.0 </code></td>
 </tr>
 </table>
 </div>
 </li>
        <li> <span class="li-head">ip_filter</span> - IP filter for encapsulted traffic <span class="li-normal">type: str</span> <span class="li-normal">choices: enable, disable</span>
 <a id='label156' href="javascript:ContentClick('label157', 'label156');" onmouseover="ContentPreview('label157');" onmouseout="ContentUnpreview('label157');" title="click to collapse or expand..."> more... </a>
 <div id="label157" style="display:none">
 <table border="1">
 <tr>
 <td></td>
 <td colspan="3">Supported Version Ranges</td>
 </tr>
 <tr>
 <td>ip_filter</td>
 <td><code class="docutils literal notranslate">v6.0.0 -> v7.0.8 </code></td>
 <td><code class="docutils literal notranslate">v7.2.0 -> v7.2.4 </code></td>
 <td><code class="docutils literal notranslate">v7.4.3 -> 7.6.0 </code></td>
 </tr>
 <tr>
 <td>[enable]</td>
 <td><code class="docutils literal notranslate">v6.0.0 -> v7.0.8</code></td>
 <tr>
 <td>[disable]</td>
 <td><code class="docutils literal notranslate">v6.0.0 -> v7.0.8</code></td>
 </table>
 </div>
 </li>
        <li> <span class="li-head">ip_policy</span> - IP policy. <span class="li-normal">type: list</span> <span style="font-family:'Courier New'" class="li-required">member_path: ip_policy:id</span>
 <a id='label158' href="javascript:ContentClick('label159', 'label158');" onmouseover="ContentPreview('label159');" onmouseout="ContentUnpreview('label159');" title="click to collapse or expand..."> more... </a>
 <div id="label159" style="display:none">
 <table border="1">
 <tr>
 <td></td><td colspan="3">Supported Version Ranges</td>
 </tr>
 <tr>
 <td>ip_policy</td>
 <td><code class="docutils literal notranslate">v6.0.0 -> v7.0.8 </code></td>
 <td><code class="docutils literal notranslate">v7.2.0 -> v7.2.4 </code></td>
 <td><code class="docutils literal notranslate">v7.4.3 -> 7.6.0 </code></td>
 </tr>
 </table>
 </div>
 </li>
            <ul class="ul-self">
            <li> <span class="li-head">action</span> - Action. <span class="li-normal">type: str</span> <span class="li-normal">choices: allow, deny</span>
 <a id='label160' href="javascript:ContentClick('label161', 'label160');" onmouseover="ContentPreview('label161');" onmouseout="ContentUnpreview('label161');" title="click to collapse or expand..."> more... </a>
 <div id="label161" style="display:none">
 <table border="1">
 <tr>
 <td></td>
 <td colspan="3">Supported Version Ranges</td>
 </tr>
 <tr>
 <td>action</td>
 <td><code class="docutils literal notranslate">v6.0.0 -> v7.0.8 </code></td>
 <td><code class="docutils literal notranslate">v7.2.0 -> v7.2.4 </code></td>
 <td><code class="docutils literal notranslate">v7.4.3 -> 7.6.0 </code></td>
 </tr>
 <tr>
 <td>[allow]</td>
 <td><code class="docutils literal notranslate">v6.0.0 -> v7.0.8</code></td>
 <tr>
 <td>[deny]</td>
 <td><code class="docutils literal notranslate">v6.0.0 -> v7.0.8</code></td>
 </table>
 </div>
 </li>
            <li> <span class="li-head">dstaddr</span> - Destination address name. Source firewall.address.name firewall.addrgrp.name. <span class="li-normal">type: str</span>
 <a id='label162' href="javascript:ContentClick('label163', 'label162');" onmouseover="ContentPreview('label163');" onmouseout="ContentUnpreview('label163');" title="click to collapse or expand..."> more... </a>
 <div id="label163" style="display:none">
 <table border="1">
 <tr>
 <td></td>
 <td colspan="3">Supported Version Ranges</td>
 </tr>
 <tr>
 <td>dstaddr</td>
 <td><code class="docutils literal notranslate">v6.0.0 -> v7.0.8 </code></td>
 <td><code class="docutils literal notranslate">v7.2.0 -> v7.2.4 </code></td>
 <td><code class="docutils literal notranslate">v7.4.3 -> 7.6.0 </code></td>
 </tr>
 </table>
 </div>
 </li>
            <li> <span class="li-head">dstaddr6</span> - Destination IPv6 address name. Source firewall.address6.name firewall.addrgrp6.name. <span class="li-normal">type: str</span>
 <a id='label164' href="javascript:ContentClick('label165', 'label164');" onmouseover="ContentPreview('label165');" onmouseout="ContentUnpreview('label165');" title="click to collapse or expand..."> more... </a>
 <div id="label165" style="display:none">
 <table border="1">
 <tr>
 <td></td>
 <td colspan="4">Supported Version Ranges</td>
 </tr>
 <tr>
 <td>dstaddr6</td>
 <td><code class="docutils literal notranslate">v6.4.0 -> v6.4.0 </code></td>
 <td><code class="docutils literal notranslate">v6.4.4 -> v7.0.8 </code></td>
 <td><code class="docutils literal notranslate">v7.2.0 -> v7.2.4 </code></td>
 <td><code class="docutils literal notranslate">v7.4.3 -> 7.6.0 </code></td>
 </tr>
 </table>
 </div>
 </li>
            <li> <span class="li-head">id</span> - ID. see <a href='#notes'>Notes</a>. <span class="li-normal">type: int</span> <span class="li-required">required: true</span>
 <a id='label166' href="javascript:ContentClick('label167', 'label166');" onmouseover="ContentPreview('label167');" onmouseout="ContentUnpreview('label167');" title="click to collapse or expand..."> more... </a>
 <div id="label167" style="display:none">
 <table border="1">
 <tr>
 <td></td>
 <td colspan="3">Supported Version Ranges</td>
 </tr>
 <tr>
 <td>id</td>
 <td><code class="docutils literal notranslate">v6.0.0 -> v7.0.8 </code></td>
 <td><code class="docutils literal notranslate">v7.2.0 -> v7.2.4 </code></td>
 <td><code class="docutils literal notranslate">v7.4.3 -> 7.6.0 </code></td>
 </tr>
 </table>
 </div>
 </li>
            <li> <span class="li-head">srcaddr</span> - Source address name. Source firewall.address.name firewall.addrgrp.name. <span class="li-normal">type: str</span>
 <a id='label168' href="javascript:ContentClick('label169', 'label168');" onmouseover="ContentPreview('label169');" onmouseout="ContentUnpreview('label169');" title="click to collapse or expand..."> more... </a>
 <div id="label169" style="display:none">
 <table border="1">
 <tr>
 <td></td>
 <td colspan="3">Supported Version Ranges</td>
 </tr>
 <tr>
 <td>srcaddr</td>
 <td><code class="docutils literal notranslate">v6.0.0 -> v7.0.8 </code></td>
 <td><code class="docutils literal notranslate">v7.2.0 -> v7.2.4 </code></td>
 <td><code class="docutils literal notranslate">v7.4.3 -> 7.6.0 </code></td>
 </tr>
 </table>
 </div>
 </li>
            <li> <span class="li-head">srcaddr6</span> - Source IPv6 address name. Source firewall.address6.name firewall.addrgrp6.name. <span class="li-normal">type: str</span>
 <a id='label170' href="javascript:ContentClick('label171', 'label170');" onmouseover="ContentPreview('label171');" onmouseout="ContentUnpreview('label171');" title="click to collapse or expand..."> more... </a>
 <div id="label171" style="display:none">
 <table border="1">
 <tr>
 <td></td>
 <td colspan="4">Supported Version Ranges</td>
 </tr>
 <tr>
 <td>srcaddr6</td>
 <td><code class="docutils literal notranslate">v6.4.0 -> v6.4.0 </code></td>
 <td><code class="docutils literal notranslate">v6.4.4 -> v7.0.8 </code></td>
 <td><code class="docutils literal notranslate">v7.2.0 -> v7.2.4 </code></td>
 <td><code class="docutils literal notranslate">v7.4.3 -> 7.6.0 </code></td>
 </tr>
 </table>
 </div>
 </li>
            </ul>
        <li> <span class="li-head">log_freq</span> - Logging of frequency of GTP-C packets. <span class="li-normal">type: int</span>
 <a id='label172' href="javascript:ContentClick('label173', 'label172');" onmouseover="ContentPreview('label173');" onmouseout="ContentUnpreview('label173');" title="click to collapse or expand..."> more... </a>
 <div id="label173" style="display:none">
 <table border="1">
 <tr>
 <td></td>
 <td colspan="3">Supported Version Ranges</td>
 </tr>
 <tr>
 <td>log_freq</td>
 <td><code class="docutils literal notranslate">v6.0.0 -> v7.0.8 </code></td>
 <td><code class="docutils literal notranslate">v7.2.0 -> v7.2.4 </code></td>
 <td><code class="docutils literal notranslate">v7.4.3 -> 7.6.0 </code></td>
 </tr>
 </table>
 </div>
 </li>
        <li> <span class="li-head">log_gtpu_limit</span> - the user data log limit (0-512 bytes) <span class="li-normal">type: int</span>
 <a id='label174' href="javascript:ContentClick('label175', 'label174');" onmouseover="ContentPreview('label175');" onmouseout="ContentUnpreview('label175');" title="click to collapse or expand..."> more... </a>
 <div id="label175" style="display:none">
 <table border="1">
 <tr>
 <td></td>
 <td colspan="3">Supported Version Ranges</td>
 </tr>
 <tr>
 <td>log_gtpu_limit</td>
 <td><code class="docutils literal notranslate">v6.0.0 -> v7.0.8 </code></td>
 <td><code class="docutils literal notranslate">v7.2.0 -> v7.2.4 </code></td>
 <td><code class="docutils literal notranslate">v7.4.3 -> 7.6.0 </code></td>
 </tr>
 </table>
 </div>
 </li>
        <li> <span class="li-head">log_imsi_prefix</span> - IMSI prefix for selective logging. <span class="li-normal">type: str</span>
 <a id='label176' href="javascript:ContentClick('label177', 'label176');" onmouseover="ContentPreview('label177');" onmouseout="ContentUnpreview('label177');" title="click to collapse or expand..."> more... </a>
 <div id="label177" style="display:none">
 <table border="1">
 <tr>
 <td></td>
 <td colspan="3">Supported Version Ranges</td>
 </tr>
 <tr>
 <td>log_imsi_prefix</td>
 <td><code class="docutils literal notranslate">v6.0.0 -> v7.0.8 </code></td>
 <td><code class="docutils literal notranslate">v7.2.0 -> v7.2.4 </code></td>
 <td><code class="docutils literal notranslate">v7.4.3 -> 7.6.0 </code></td>
 </tr>
 </table>
 </div>
 </li>
        <li> <span class="li-head">log_msisdn_prefix</span> - the msisdn prefix for selective logging <span class="li-normal">type: str</span>
 <a id='label178' href="javascript:ContentClick('label179', 'label178');" onmouseover="ContentPreview('label179');" onmouseout="ContentUnpreview('label179');" title="click to collapse or expand..."> more... </a>
 <div id="label179" style="display:none">
 <table border="1">
 <tr>
 <td></td>
 <td colspan="3">Supported Version Ranges</td>
 </tr>
 <tr>
 <td>log_msisdn_prefix</td>
 <td><code class="docutils literal notranslate">v6.0.0 -> v7.0.8 </code></td>
 <td><code class="docutils literal notranslate">v7.2.0 -> v7.2.4 </code></td>
 <td><code class="docutils literal notranslate">v7.4.3 -> 7.6.0 </code></td>
 </tr>
 </table>
 </div>
 </li>
        <li> <span class="li-head">max_message_length</span> - max message length <span class="li-normal">type: int</span>
 <a id='label180' href="javascript:ContentClick('label181', 'label180');" onmouseover="ContentPreview('label181');" onmouseout="ContentUnpreview('label181');" title="click to collapse or expand..."> more... </a>
 <div id="label181" style="display:none">
 <table border="1">
 <tr>
 <td></td>
 <td colspan="3">Supported Version Ranges</td>
 </tr>
 <tr>
 <td>max_message_length</td>
 <td><code class="docutils literal notranslate">v6.0.0 -> v7.0.8 </code></td>
 <td><code class="docutils literal notranslate">v7.2.0 -> v7.2.4 </code></td>
 <td><code class="docutils literal notranslate">v7.4.3 -> 7.6.0 </code></td>
 </tr>
 </table>
 </div>
 </li>
        <li> <span class="li-head">message_filter_v0v1</span> - Message filter. Source gtp.message-filter-v0v1.name. <span class="li-normal">type: str</span>
 <a id='label182' href="javascript:ContentClick('label183', 'label182');" onmouseover="ContentPreview('label183');" onmouseout="ContentUnpreview('label183');" title="click to collapse or expand..."> more... </a>
 <div id="label183" style="display:none">
 <table border="1">
 <tr>
 <td></td>
 <td colspan="3">Supported Version Ranges</td>
 </tr>
 <tr>
 <td>message_filter_v0v1</td>
 <td><code class="docutils literal notranslate">v6.0.0 -> v7.0.8 </code></td>
 <td><code class="docutils literal notranslate">v7.2.0 -> v7.2.4 </code></td>
 <td><code class="docutils literal notranslate">v7.4.3 -> 7.6.0 </code></td>
 </tr>
 </table>
 </div>
 </li>
        <li> <span class="li-head">message_filter_v2</span> - Message filter. Source gtp.message-filter-v2.name. <span class="li-normal">type: str</span>
 <a id='label184' href="javascript:ContentClick('label185', 'label184');" onmouseover="ContentPreview('label185');" onmouseout="ContentUnpreview('label185');" title="click to collapse or expand..."> more... </a>
 <div id="label185" style="display:none">
 <table border="1">
 <tr>
 <td></td>
 <td colspan="3">Supported Version Ranges</td>
 </tr>
 <tr>
 <td>message_filter_v2</td>
 <td><code class="docutils literal notranslate">v6.0.0 -> v7.0.8 </code></td>
 <td><code class="docutils literal notranslate">v7.2.0 -> v7.2.4 </code></td>
 <td><code class="docutils literal notranslate">v7.4.3 -> 7.6.0 </code></td>
 </tr>
 </table>
 </div>
 </li>
        <li> <span class="li-head">message_rate_limit</span> - Message rate limiting. <span class="li-normal">type: dict</span>
 <a id='label186' href="javascript:ContentClick('label187', 'label186');" onmouseover="ContentPreview('label187');" onmouseout="ContentUnpreview('label187');" title="click to collapse or expand..."> more... </a>
 <div id="label187" style="display:none">
 <table border="1">
 <tr>
 <td></td><td colspan="3">Supported Version Ranges</td>
 </tr>
 <tr>
 <td>message_rate_limit</td>
 <td><code class="docutils literal notranslate">v6.0.0 -> v7.0.8 </code></td>
 <td><code class="docutils literal notranslate">v7.2.0 -> v7.2.4 </code></td>
 <td><code class="docutils literal notranslate">v7.4.3 -> 7.6.0 </code></td>
 </tr>
 </table>
 </div>
 </li>
            <ul class="ul-self">
            <li> <span class="li-head">create_aa_pdp_request</span> - Rate limit for create AA PDP context request (packets per second). <span class="li-normal">type: int</span>
 <a id='label188' href="javascript:ContentClick('label189', 'label188');" onmouseover="ContentPreview('label189');" onmouseout="ContentUnpreview('label189');" title="click to collapse or expand..."> more... </a>
 <div id="label189" style="display:none">
 <table border="1">
 <tr>
 <td></td>
 <td colspan="3">Supported Version Ranges</td>
 </tr>
 <tr>
 <td>create_aa_pdp_request</td>
 <td><code class="docutils literal notranslate">v6.0.0 -> v7.0.8 </code></td>
 <td><code class="docutils literal notranslate">v7.2.0 -> v7.2.4 </code></td>
 <td><code class="docutils literal notranslate">v7.4.3 -> 7.6.0 </code></td>
 </tr>
 </table>
 </div>
 </li>
            <li> <span class="li-head">create_aa_pdp_response</span> - Rate limit for create AA PDP context response (packets per second). <span class="li-normal">type: int</span>
 <a id='label190' href="javascript:ContentClick('label191', 'label190');" onmouseover="ContentPreview('label191');" onmouseout="ContentUnpreview('label191');" title="click to collapse or expand..."> more... </a>
 <div id="label191" style="display:none">
 <table border="1">
 <tr>
 <td></td>
 <td colspan="3">Supported Version Ranges</td>
 </tr>
 <tr>
 <td>create_aa_pdp_response</td>
 <td><code class="docutils literal notranslate">v6.0.0 -> v7.0.8 </code></td>
 <td><code class="docutils literal notranslate">v7.2.0 -> v7.2.4 </code></td>
 <td><code class="docutils literal notranslate">v7.4.3 -> 7.6.0 </code></td>
 </tr>
 </table>
 </div>
 </li>
            <li> <span class="li-head">create_mbms_request</span> - Rate limit for create MBMS context request (packets per second). <span class="li-normal">type: int</span>
 <a id='label192' href="javascript:ContentClick('label193', 'label192');" onmouseover="ContentPreview('label193');" onmouseout="ContentUnpreview('label193');" title="click to collapse or expand..."> more... </a>
 <div id="label193" style="display:none">
 <table border="1">
 <tr>
 <td></td>
 <td colspan="3">Supported Version Ranges</td>
 </tr>
 <tr>
 <td>create_mbms_request</td>
 <td><code class="docutils literal notranslate">v6.0.0 -> v7.0.8 </code></td>
 <td><code class="docutils literal notranslate">v7.2.0 -> v7.2.4 </code></td>
 <td><code class="docutils literal notranslate">v7.4.3 -> 7.6.0 </code></td>
 </tr>
 </table>
 </div>
 </li>
            <li> <span class="li-head">create_mbms_response</span> - Rate limit for create MBMS context response (packets per second). <span class="li-normal">type: int</span>
 <a id='label194' href="javascript:ContentClick('label195', 'label194');" onmouseover="ContentPreview('label195');" onmouseout="ContentUnpreview('label195');" title="click to collapse or expand..."> more... </a>
 <div id="label195" style="display:none">
 <table border="1">
 <tr>
 <td></td>
 <td colspan="3">Supported Version Ranges</td>
 </tr>
 <tr>
 <td>create_mbms_response</td>
 <td><code class="docutils literal notranslate">v6.0.0 -> v7.0.8 </code></td>
 <td><code class="docutils literal notranslate">v7.2.0 -> v7.2.4 </code></td>
 <td><code class="docutils literal notranslate">v7.4.3 -> 7.6.0 </code></td>
 </tr>
 </table>
 </div>
 </li>
            <li> <span class="li-head">create_pdp_request</span> - Rate limit for create PDP context request (packets per second). <span class="li-normal">type: int</span>
 <a id='label196' href="javascript:ContentClick('label197', 'label196');" onmouseover="ContentPreview('label197');" onmouseout="ContentUnpreview('label197');" title="click to collapse or expand..."> more... </a>
 <div id="label197" style="display:none">
 <table border="1">
 <tr>
 <td></td>
 <td colspan="3">Supported Version Ranges</td>
 </tr>
 <tr>
 <td>create_pdp_request</td>
 <td><code class="docutils literal notranslate">v6.0.0 -> v7.0.8 </code></td>
 <td><code class="docutils literal notranslate">v7.2.0 -> v7.2.4 </code></td>
 <td><code class="docutils literal notranslate">v7.4.3 -> 7.6.0 </code></td>
 </tr>
 </table>
 </div>
 </li>
            <li> <span class="li-head">create_pdp_response</span> - Rate limit for create PDP context response (packets per second). <span class="li-normal">type: int</span>
 <a id='label198' href="javascript:ContentClick('label199', 'label198');" onmouseover="ContentPreview('label199');" onmouseout="ContentUnpreview('label199');" title="click to collapse or expand..."> more... </a>
 <div id="label199" style="display:none">
 <table border="1">
 <tr>
 <td></td>
 <td colspan="3">Supported Version Ranges</td>
 </tr>
 <tr>
 <td>create_pdp_response</td>
 <td><code class="docutils literal notranslate">v6.0.0 -> v7.0.8 </code></td>
 <td><code class="docutils literal notranslate">v7.2.0 -> v7.2.4 </code></td>
 <td><code class="docutils literal notranslate">v7.4.3 -> 7.6.0 </code></td>
 </tr>
 </table>
 </div>
 </li>
            <li> <span class="li-head">delete_aa_pdp_request</span> - Rate limit for delete AA PDP context request (packets per second). <span class="li-normal">type: int</span>
 <a id='label200' href="javascript:ContentClick('label201', 'label200');" onmouseover="ContentPreview('label201');" onmouseout="ContentUnpreview('label201');" title="click to collapse or expand..."> more... </a>
 <div id="label201" style="display:none">
 <table border="1">
 <tr>
 <td></td>
 <td colspan="3">Supported Version Ranges</td>
 </tr>
 <tr>
 <td>delete_aa_pdp_request</td>
 <td><code class="docutils literal notranslate">v6.0.0 -> v7.0.8 </code></td>
 <td><code class="docutils literal notranslate">v7.2.0 -> v7.2.4 </code></td>
 <td><code class="docutils literal notranslate">v7.4.3 -> 7.6.0 </code></td>
 </tr>
 </table>
 </div>
 </li>
            <li> <span class="li-head">delete_aa_pdp_response</span> - Rate limit for delete AA PDP context response (packets per second). <span class="li-normal">type: int</span>
 <a id='label202' href="javascript:ContentClick('label203', 'label202');" onmouseover="ContentPreview('label203');" onmouseout="ContentUnpreview('label203');" title="click to collapse or expand..."> more... </a>
 <div id="label203" style="display:none">
 <table border="1">
 <tr>
 <td></td>
 <td colspan="3">Supported Version Ranges</td>
 </tr>
 <tr>
 <td>delete_aa_pdp_response</td>
 <td><code class="docutils literal notranslate">v6.0.0 -> v7.0.8 </code></td>
 <td><code class="docutils literal notranslate">v7.2.0 -> v7.2.4 </code></td>
 <td><code class="docutils literal notranslate">v7.4.3 -> 7.6.0 </code></td>
 </tr>
 </table>
 </div>
 </li>
            <li> <span class="li-head">delete_mbms_request</span> - Rate limit for delete MBMS context request (packets per second). <span class="li-normal">type: int</span>
 <a id='label204' href="javascript:ContentClick('label205', 'label204');" onmouseover="ContentPreview('label205');" onmouseout="ContentUnpreview('label205');" title="click to collapse or expand..."> more... </a>
 <div id="label205" style="display:none">
 <table border="1">
 <tr>
 <td></td>
 <td colspan="3">Supported Version Ranges</td>
 </tr>
 <tr>
 <td>delete_mbms_request</td>
 <td><code class="docutils literal notranslate">v6.0.0 -> v7.0.8 </code></td>
 <td><code class="docutils literal notranslate">v7.2.0 -> v7.2.4 </code></td>
 <td><code class="docutils literal notranslate">v7.4.3 -> 7.6.0 </code></td>
 </tr>
 </table>
 </div>
 </li>
            <li> <span class="li-head">delete_mbms_response</span> - Rate limit for delete MBMS context response (packets per second). <span class="li-normal">type: int</span>
 <a id='label206' href="javascript:ContentClick('label207', 'label206');" onmouseover="ContentPreview('label207');" onmouseout="ContentUnpreview('label207');" title="click to collapse or expand..."> more... </a>
 <div id="label207" style="display:none">
 <table border="1">
 <tr>
 <td></td>
 <td colspan="3">Supported Version Ranges</td>
 </tr>
 <tr>
 <td>delete_mbms_response</td>
 <td><code class="docutils literal notranslate">v6.0.0 -> v7.0.8 </code></td>
 <td><code class="docutils literal notranslate">v7.2.0 -> v7.2.4 </code></td>
 <td><code class="docutils literal notranslate">v7.4.3 -> 7.6.0 </code></td>
 </tr>
 </table>
 </div>
 </li>
            <li> <span class="li-head">delete_pdp_request</span> - Rate limit for delete PDP context request (packets per second). <span class="li-normal">type: int</span>
 <a id='label208' href="javascript:ContentClick('label209', 'label208');" onmouseover="ContentPreview('label209');" onmouseout="ContentUnpreview('label209');" title="click to collapse or expand..."> more... </a>
 <div id="label209" style="display:none">
 <table border="1">
 <tr>
 <td></td>
 <td colspan="3">Supported Version Ranges</td>
 </tr>
 <tr>
 <td>delete_pdp_request</td>
 <td><code class="docutils literal notranslate">v6.0.0 -> v7.0.8 </code></td>
 <td><code class="docutils literal notranslate">v7.2.0 -> v7.2.4 </code></td>
 <td><code class="docutils literal notranslate">v7.4.3 -> 7.6.0 </code></td>
 </tr>
 </table>
 </div>
 </li>
            <li> <span class="li-head">delete_pdp_response</span> - Rate limit for delete PDP context response (packets per second). <span class="li-normal">type: int</span>
 <a id='label210' href="javascript:ContentClick('label211', 'label210');" onmouseover="ContentPreview('label211');" onmouseout="ContentUnpreview('label211');" title="click to collapse or expand..."> more... </a>
 <div id="label211" style="display:none">
 <table border="1">
 <tr>
 <td></td>
 <td colspan="3">Supported Version Ranges</td>
 </tr>
 <tr>
 <td>delete_pdp_response</td>
 <td><code class="docutils literal notranslate">v6.0.0 -> v7.0.8 </code></td>
 <td><code class="docutils literal notranslate">v7.2.0 -> v7.2.4 </code></td>
 <td><code class="docutils literal notranslate">v7.4.3 -> 7.6.0 </code></td>
 </tr>
 </table>
 </div>
 </li>
            <li> <span class="li-head">echo_reponse</span> - Rate limit for echo response (packets per second). <span class="li-normal">type: int</span>
 <a id='label212' href="javascript:ContentClick('label213', 'label212');" onmouseover="ContentPreview('label213');" onmouseout="ContentUnpreview('label213');" title="click to collapse or expand..."> more... </a>
 <div id="label213" style="display:none">
 <table border="1">
 <tr>
 <td></td>
 <td colspan="3">Supported Version Ranges</td>
 </tr>
 <tr>
 <td>echo_reponse</td>
 <td><code class="docutils literal notranslate">v6.0.0 -> v7.0.8 </code></td>
 <td><code class="docutils literal notranslate">v7.2.0 -> v7.2.4 </code></td>
 <td><code class="docutils literal notranslate">v7.4.3 -> v7.4.3 </code></td>
 </tr>
 </table>
 </div>
 </li>
            <li> <span class="li-head">echo_request</span> - Rate limit for echo requests (packets per second). <span class="li-normal">type: int</span>
 <a id='label214' href="javascript:ContentClick('label215', 'label214');" onmouseover="ContentPreview('label215');" onmouseout="ContentUnpreview('label215');" title="click to collapse or expand..."> more... </a>
 <div id="label215" style="display:none">
 <table border="1">
 <tr>
 <td></td>
 <td colspan="3">Supported Version Ranges</td>
 </tr>
 <tr>
 <td>echo_request</td>
 <td><code class="docutils literal notranslate">v6.0.0 -> v7.0.8 </code></td>
 <td><code class="docutils literal notranslate">v7.2.0 -> v7.2.4 </code></td>
 <td><code class="docutils literal notranslate">v7.4.3 -> 7.6.0 </code></td>
 </tr>
 </table>
 </div>
 </li>
            <li> <span class="li-head">echo_response</span> - Rate limit for echo response (packets per second). <span class="li-normal">type: int</span>
 <a id='label216' href="javascript:ContentClick('label217', 'label216');" onmouseover="ContentPreview('label217');" onmouseout="ContentUnpreview('label217');" title="click to collapse or expand..."> more... </a>
 <div id="label217" style="display:none">
 <table border="1">
 <tr>
 <td></td>
 <td colspan="1">Supported Version Ranges</td>
 </tr>
 <tr>
 <td>echo_response</td>
 <td><code class="docutils literal notranslate">v7.4.4 -> 7.6.0 </code></td>
 </tr>
 </table>
 </div>
 </li>
            <li> <span class="li-head">error_indication</span> - Rate limit for error indication (packets per second). <span class="li-normal">type: int</span>
 <a id='label218' href="javascript:ContentClick('label219', 'label218');" onmouseover="ContentPreview('label219');" onmouseout="ContentUnpreview('label219');" title="click to collapse or expand..."> more... </a>
 <div id="label219" style="display:none">
 <table border="1">
 <tr>
 <td></td>
 <td colspan="3">Supported Version Ranges</td>
 </tr>
 <tr>
 <td>error_indication</td>
 <td><code class="docutils literal notranslate">v6.0.0 -> v7.0.8 </code></td>
 <td><code class="docutils literal notranslate">v7.2.0 -> v7.2.4 </code></td>
 <td><code class="docutils literal notranslate">v7.4.3 -> 7.6.0 </code></td>
 </tr>
 </table>
 </div>
 </li>
            <li> <span class="li-head">failure_report_request</span> - Rate limit for failure report request (packets per second). <span class="li-normal">type: int</span>
 <a id='label220' href="javascript:ContentClick('label221', 'label220');" onmouseover="ContentPreview('label221');" onmouseout="ContentUnpreview('label221');" title="click to collapse or expand..."> more... </a>
 <div id="label221" style="display:none">
 <table border="1">
 <tr>
 <td></td>
 <td colspan="3">Supported Version Ranges</td>
 </tr>
 <tr>
 <td>failure_report_request</td>
 <td><code class="docutils literal notranslate">v6.0.0 -> v7.0.8 </code></td>
 <td><code class="docutils literal notranslate">v7.2.0 -> v7.2.4 </code></td>
 <td><code class="docutils literal notranslate">v7.4.3 -> 7.6.0 </code></td>
 </tr>
 </table>
 </div>
 </li>
            <li> <span class="li-head">failure_report_response</span> - Rate limit for failure report response (packets per second). <span class="li-normal">type: int</span>
 <a id='label222' href="javascript:ContentClick('label223', 'label222');" onmouseover="ContentPreview('label223');" onmouseout="ContentUnpreview('label223');" title="click to collapse or expand..."> more... </a>
 <div id="label223" style="display:none">
 <table border="1">
 <tr>
 <td></td>
 <td colspan="3">Supported Version Ranges</td>
 </tr>
 <tr>
 <td>failure_report_response</td>
 <td><code class="docutils literal notranslate">v6.0.0 -> v7.0.8 </code></td>
 <td><code class="docutils literal notranslate">v7.2.0 -> v7.2.4 </code></td>
 <td><code class="docutils literal notranslate">v7.4.3 -> 7.6.0 </code></td>
 </tr>
 </table>
 </div>
 </li>
            <li> <span class="li-head">fwd_reloc_complete_ack</span> - Rate limit for forward relocation complete acknowledge (packets per second). <span class="li-normal">type: int</span>
 <a id='label224' href="javascript:ContentClick('label225', 'label224');" onmouseover="ContentPreview('label225');" onmouseout="ContentUnpreview('label225');" title="click to collapse or expand..."> more... </a>
 <div id="label225" style="display:none">
 <table border="1">
 <tr>
 <td></td>
 <td colspan="3">Supported Version Ranges</td>
 </tr>
 <tr>
 <td>fwd_reloc_complete_ack</td>
 <td><code class="docutils literal notranslate">v6.0.0 -> v7.0.8 </code></td>
 <td><code class="docutils literal notranslate">v7.2.0 -> v7.2.4 </code></td>
 <td><code class="docutils literal notranslate">v7.4.3 -> 7.6.0 </code></td>
 </tr>
 </table>
 </div>
 </li>
            <li> <span class="li-head">fwd_relocation_complete</span> - Rate limit for forward relocation complete (packets per second). <span class="li-normal">type: int</span>
 <a id='label226' href="javascript:ContentClick('label227', 'label226');" onmouseover="ContentPreview('label227');" onmouseout="ContentUnpreview('label227');" title="click to collapse or expand..."> more... </a>
 <div id="label227" style="display:none">
 <table border="1">
 <tr>
 <td></td>
 <td colspan="3">Supported Version Ranges</td>
 </tr>
 <tr>
 <td>fwd_relocation_complete</td>
 <td><code class="docutils literal notranslate">v6.0.0 -> v7.0.8 </code></td>
 <td><code class="docutils literal notranslate">v7.2.0 -> v7.2.4 </code></td>
 <td><code class="docutils literal notranslate">v7.4.3 -> 7.6.0 </code></td>
 </tr>
 </table>
 </div>
 </li>
            <li> <span class="li-head">fwd_relocation_request</span> - Rate limit for forward relocation request (packets per second). <span class="li-normal">type: int</span>
 <a id='label228' href="javascript:ContentClick('label229', 'label228');" onmouseover="ContentPreview('label229');" onmouseout="ContentUnpreview('label229');" title="click to collapse or expand..."> more... </a>
 <div id="label229" style="display:none">
 <table border="1">
 <tr>
 <td></td>
 <td colspan="3">Supported Version Ranges</td>
 </tr>
 <tr>
 <td>fwd_relocation_request</td>
 <td><code class="docutils literal notranslate">v6.0.0 -> v7.0.8 </code></td>
 <td><code class="docutils literal notranslate">v7.2.0 -> v7.2.4 </code></td>
 <td><code class="docutils literal notranslate">v7.4.3 -> 7.6.0 </code></td>
 </tr>
 </table>
 </div>
 </li>
            <li> <span class="li-head">fwd_relocation_response</span> - Rate limit for forward relocation response (packets per second). <span class="li-normal">type: int</span>
 <a id='label230' href="javascript:ContentClick('label231', 'label230');" onmouseover="ContentPreview('label231');" onmouseout="ContentUnpreview('label231');" title="click to collapse or expand..."> more... </a>
 <div id="label231" style="display:none">
 <table border="1">
 <tr>
 <td></td>
 <td colspan="3">Supported Version Ranges</td>
 </tr>
 <tr>
 <td>fwd_relocation_response</td>
 <td><code class="docutils literal notranslate">v6.0.0 -> v7.0.8 </code></td>
 <td><code class="docutils literal notranslate">v7.2.0 -> v7.2.4 </code></td>
 <td><code class="docutils literal notranslate">v7.4.3 -> 7.6.0 </code></td>
 </tr>
 </table>
 </div>
 </li>
            <li> <span class="li-head">fwd_srns_context</span> - Rate limit for forward SRNS context (packets per second). <span class="li-normal">type: int</span>
 <a id='label232' href="javascript:ContentClick('label233', 'label232');" onmouseover="ContentPreview('label233');" onmouseout="ContentUnpreview('label233');" title="click to collapse or expand..."> more... </a>
 <div id="label233" style="display:none">
 <table border="1">
 <tr>
 <td></td>
 <td colspan="3">Supported Version Ranges</td>
 </tr>
 <tr>
 <td>fwd_srns_context</td>
 <td><code class="docutils literal notranslate">v6.0.0 -> v7.0.8 </code></td>
 <td><code class="docutils literal notranslate">v7.2.0 -> v7.2.4 </code></td>
 <td><code class="docutils literal notranslate">v7.4.3 -> 7.6.0 </code></td>
 </tr>
 </table>
 </div>
 </li>
            <li> <span class="li-head">fwd_srns_context_ack</span> - Rate limit for forward SRNS context acknowledge (packets per second). <span class="li-normal">type: int</span>
 <a id='label234' href="javascript:ContentClick('label235', 'label234');" onmouseover="ContentPreview('label235');" onmouseout="ContentUnpreview('label235');" title="click to collapse or expand..."> more... </a>
 <div id="label235" style="display:none">
 <table border="1">
 <tr>
 <td></td>
 <td colspan="3">Supported Version Ranges</td>
 </tr>
 <tr>
 <td>fwd_srns_context_ack</td>
 <td><code class="docutils literal notranslate">v6.0.0 -> v7.0.8 </code></td>
 <td><code class="docutils literal notranslate">v7.2.0 -> v7.2.4 </code></td>
 <td><code class="docutils literal notranslate">v7.4.3 -> 7.6.0 </code></td>
 </tr>
 </table>
 </div>
 </li>
            <li> <span class="li-head">g_pdu</span> - Rate limit for G-PDU (packets per second). <span class="li-normal">type: int</span>
 <a id='label236' href="javascript:ContentClick('label237', 'label236');" onmouseover="ContentPreview('label237');" onmouseout="ContentUnpreview('label237');" title="click to collapse or expand..."> more... </a>
 <div id="label237" style="display:none">
 <table border="1">
 <tr>
 <td></td>
 <td colspan="3">Supported Version Ranges</td>
 </tr>
 <tr>
 <td>g_pdu</td>
 <td><code class="docutils literal notranslate">v6.0.0 -> v7.0.8 </code></td>
 <td><code class="docutils literal notranslate">v7.2.0 -> v7.2.4 </code></td>
 <td><code class="docutils literal notranslate">v7.4.3 -> 7.6.0 </code></td>
 </tr>
 </table>
 </div>
 </li>
            <li> <span class="li-head">identification_request</span> - Rate limit for identification request (packets per second). <span class="li-normal">type: int</span>
 <a id='label238' href="javascript:ContentClick('label239', 'label238');" onmouseover="ContentPreview('label239');" onmouseout="ContentUnpreview('label239');" title="click to collapse or expand..."> more... </a>
 <div id="label239" style="display:none">
 <table border="1">
 <tr>
 <td></td>
 <td colspan="3">Supported Version Ranges</td>
 </tr>
 <tr>
 <td>identification_request</td>
 <td><code class="docutils literal notranslate">v6.0.0 -> v7.0.8 </code></td>
 <td><code class="docutils literal notranslate">v7.2.0 -> v7.2.4 </code></td>
 <td><code class="docutils literal notranslate">v7.4.3 -> 7.6.0 </code></td>
 </tr>
 </table>
 </div>
 </li>
            <li> <span class="li-head">identification_response</span> - Rate limit for identification response (packets per second). <span class="li-normal">type: int</span>
 <a id='label240' href="javascript:ContentClick('label241', 'label240');" onmouseover="ContentPreview('label241');" onmouseout="ContentUnpreview('label241');" title="click to collapse or expand..."> more... </a>
 <div id="label241" style="display:none">
 <table border="1">
 <tr>
 <td></td>
 <td colspan="3">Supported Version Ranges</td>
 </tr>
 <tr>
 <td>identification_response</td>
 <td><code class="docutils literal notranslate">v6.0.0 -> v7.0.8 </code></td>
 <td><code class="docutils literal notranslate">v7.2.0 -> v7.2.4 </code></td>
 <td><code class="docutils literal notranslate">v7.4.3 -> 7.6.0 </code></td>
 </tr>
 </table>
 </div>
 </li>
            <li> <span class="li-head">mbms_de_reg_request</span> - Rate limit for MBMS de-registration request (packets per second). <span class="li-normal">type: int</span>
 <a id='label242' href="javascript:ContentClick('label243', 'label242');" onmouseover="ContentPreview('label243');" onmouseout="ContentUnpreview('label243');" title="click to collapse or expand..."> more... </a>
 <div id="label243" style="display:none">
 <table border="1">
 <tr>
 <td></td>
 <td colspan="3">Supported Version Ranges</td>
 </tr>
 <tr>
 <td>mbms_de_reg_request</td>
 <td><code class="docutils literal notranslate">v6.0.0 -> v7.0.8 </code></td>
 <td><code class="docutils literal notranslate">v7.2.0 -> v7.2.4 </code></td>
 <td><code class="docutils literal notranslate">v7.4.3 -> 7.6.0 </code></td>
 </tr>
 </table>
 </div>
 </li>
            <li> <span class="li-head">mbms_de_reg_response</span> - Rate limit for MBMS de-registration response (packets per second). <span class="li-normal">type: int</span>
 <a id='label244' href="javascript:ContentClick('label245', 'label244');" onmouseover="ContentPreview('label245');" onmouseout="ContentUnpreview('label245');" title="click to collapse or expand..."> more... </a>
 <div id="label245" style="display:none">
 <table border="1">
 <tr>
 <td></td>
 <td colspan="3">Supported Version Ranges</td>
 </tr>
 <tr>
 <td>mbms_de_reg_response</td>
 <td><code class="docutils literal notranslate">v6.0.0 -> v7.0.8 </code></td>
 <td><code class="docutils literal notranslate">v7.2.0 -> v7.2.4 </code></td>
 <td><code class="docutils literal notranslate">v7.4.3 -> 7.6.0 </code></td>
 </tr>
 </table>
 </div>
 </li>
            <li> <span class="li-head">mbms_notify_rej_request</span> - Rate limit for MBMS notification reject request (packets per second). <span class="li-normal">type: int</span>
 <a id='label246' href="javascript:ContentClick('label247', 'label246');" onmouseover="ContentPreview('label247');" onmouseout="ContentUnpreview('label247');" title="click to collapse or expand..."> more... </a>
 <div id="label247" style="display:none">
 <table border="1">
 <tr>
 <td></td>
 <td colspan="3">Supported Version Ranges</td>
 </tr>
 <tr>
 <td>mbms_notify_rej_request</td>
 <td><code class="docutils literal notranslate">v6.0.0 -> v7.0.8 </code></td>
 <td><code class="docutils literal notranslate">v7.2.0 -> v7.2.4 </code></td>
 <td><code class="docutils literal notranslate">v7.4.3 -> 7.6.0 </code></td>
 </tr>
 </table>
 </div>
 </li>
            <li> <span class="li-head">mbms_notify_rej_response</span> - Rate limit for MBMS notification reject response (packets per second). <span class="li-normal">type: int</span>
 <a id='label248' href="javascript:ContentClick('label249', 'label248');" onmouseover="ContentPreview('label249');" onmouseout="ContentUnpreview('label249');" title="click to collapse or expand..."> more... </a>
 <div id="label249" style="display:none">
 <table border="1">
 <tr>
 <td></td>
 <td colspan="3">Supported Version Ranges</td>
 </tr>
 <tr>
 <td>mbms_notify_rej_response</td>
 <td><code class="docutils literal notranslate">v6.0.0 -> v7.0.8 </code></td>
 <td><code class="docutils literal notranslate">v7.2.0 -> v7.2.4 </code></td>
 <td><code class="docutils literal notranslate">v7.4.3 -> 7.6.0 </code></td>
 </tr>
 </table>
 </div>
 </li>
            <li> <span class="li-head">mbms_notify_request</span> - Rate limit for MBMS notification request (packets per second). <span class="li-normal">type: int</span>
 <a id='label250' href="javascript:ContentClick('label251', 'label250');" onmouseover="ContentPreview('label251');" onmouseout="ContentUnpreview('label251');" title="click to collapse or expand..."> more... </a>
 <div id="label251" style="display:none">
 <table border="1">
 <tr>
 <td></td>
 <td colspan="3">Supported Version Ranges</td>
 </tr>
 <tr>
 <td>mbms_notify_request</td>
 <td><code class="docutils literal notranslate">v6.0.0 -> v7.0.8 </code></td>
 <td><code class="docutils literal notranslate">v7.2.0 -> v7.2.4 </code></td>
 <td><code class="docutils literal notranslate">v7.4.3 -> 7.6.0 </code></td>
 </tr>
 </table>
 </div>
 </li>
            <li> <span class="li-head">mbms_notify_response</span> - Rate limit for MBMS notification response (packets per second). <span class="li-normal">type: int</span>
 <a id='label252' href="javascript:ContentClick('label253', 'label252');" onmouseover="ContentPreview('label253');" onmouseout="ContentUnpreview('label253');" title="click to collapse or expand..."> more... </a>
 <div id="label253" style="display:none">
 <table border="1">
 <tr>
 <td></td>
 <td colspan="3">Supported Version Ranges</td>
 </tr>
 <tr>
 <td>mbms_notify_response</td>
 <td><code class="docutils literal notranslate">v6.0.0 -> v7.0.8 </code></td>
 <td><code class="docutils literal notranslate">v7.2.0 -> v7.2.4 </code></td>
 <td><code class="docutils literal notranslate">v7.4.3 -> 7.6.0 </code></td>
 </tr>
 </table>
 </div>
 </li>
            <li> <span class="li-head">mbms_reg_request</span> - Rate limit for MBMS registration request (packets per second). <span class="li-normal">type: int</span>
 <a id='label254' href="javascript:ContentClick('label255', 'label254');" onmouseover="ContentPreview('label255');" onmouseout="ContentUnpreview('label255');" title="click to collapse or expand..."> more... </a>
 <div id="label255" style="display:none">
 <table border="1">
 <tr>
 <td></td>
 <td colspan="3">Supported Version Ranges</td>
 </tr>
 <tr>
 <td>mbms_reg_request</td>
 <td><code class="docutils literal notranslate">v6.0.0 -> v7.0.8 </code></td>
 <td><code class="docutils literal notranslate">v7.2.0 -> v7.2.4 </code></td>
 <td><code class="docutils literal notranslate">v7.4.3 -> 7.6.0 </code></td>
 </tr>
 </table>
 </div>
 </li>
            <li> <span class="li-head">mbms_reg_response</span> - Rate limit for MBMS registration response (packets per second). <span class="li-normal">type: int</span>
 <a id='label256' href="javascript:ContentClick('label257', 'label256');" onmouseover="ContentPreview('label257');" onmouseout="ContentUnpreview('label257');" title="click to collapse or expand..."> more... </a>
 <div id="label257" style="display:none">
 <table border="1">
 <tr>
 <td></td>
 <td colspan="3">Supported Version Ranges</td>
 </tr>
 <tr>
 <td>mbms_reg_response</td>
 <td><code class="docutils literal notranslate">v6.0.0 -> v7.0.8 </code></td>
 <td><code class="docutils literal notranslate">v7.2.0 -> v7.2.4 </code></td>
 <td><code class="docutils literal notranslate">v7.4.3 -> 7.6.0 </code></td>
 </tr>
 </table>
 </div>
 </li>
            <li> <span class="li-head">mbms_ses_start_request</span> - Rate limit for MBMS session start request (packets per second). <span class="li-normal">type: int</span>
 <a id='label258' href="javascript:ContentClick('label259', 'label258');" onmouseover="ContentPreview('label259');" onmouseout="ContentUnpreview('label259');" title="click to collapse or expand..."> more... </a>
 <div id="label259" style="display:none">
 <table border="1">
 <tr>
 <td></td>
 <td colspan="3">Supported Version Ranges</td>
 </tr>
 <tr>
 <td>mbms_ses_start_request</td>
 <td><code class="docutils literal notranslate">v6.0.0 -> v7.0.8 </code></td>
 <td><code class="docutils literal notranslate">v7.2.0 -> v7.2.4 </code></td>
 <td><code class="docutils literal notranslate">v7.4.3 -> 7.6.0 </code></td>
 </tr>
 </table>
 </div>
 </li>
            <li> <span class="li-head">mbms_ses_start_response</span> - Rate limit for MBMS session start response (packets per second). <span class="li-normal">type: int</span>
 <a id='label260' href="javascript:ContentClick('label261', 'label260');" onmouseover="ContentPreview('label261');" onmouseout="ContentUnpreview('label261');" title="click to collapse or expand..."> more... </a>
 <div id="label261" style="display:none">
 <table border="1">
 <tr>
 <td></td>
 <td colspan="3">Supported Version Ranges</td>
 </tr>
 <tr>
 <td>mbms_ses_start_response</td>
 <td><code class="docutils literal notranslate">v6.0.0 -> v7.0.8 </code></td>
 <td><code class="docutils literal notranslate">v7.2.0 -> v7.2.4 </code></td>
 <td><code class="docutils literal notranslate">v7.4.3 -> 7.6.0 </code></td>
 </tr>
 </table>
 </div>
 </li>
            <li> <span class="li-head">mbms_ses_stop_request</span> - Rate limit for MBMS session stop request (packets per second). <span class="li-normal">type: int</span>
 <a id='label262' href="javascript:ContentClick('label263', 'label262');" onmouseover="ContentPreview('label263');" onmouseout="ContentUnpreview('label263');" title="click to collapse or expand..."> more... </a>
 <div id="label263" style="display:none">
 <table border="1">
 <tr>
 <td></td>
 <td colspan="3">Supported Version Ranges</td>
 </tr>
 <tr>
 <td>mbms_ses_stop_request</td>
 <td><code class="docutils literal notranslate">v6.0.0 -> v7.0.8 </code></td>
 <td><code class="docutils literal notranslate">v7.2.0 -> v7.2.4 </code></td>
 <td><code class="docutils literal notranslate">v7.4.3 -> 7.6.0 </code></td>
 </tr>
 </table>
 </div>
 </li>
            <li> <span class="li-head">mbms_ses_stop_response</span> - Rate limit for MBMS session stop response (packets per second). <span class="li-normal">type: int</span>
 <a id='label264' href="javascript:ContentClick('label265', 'label264');" onmouseover="ContentPreview('label265');" onmouseout="ContentUnpreview('label265');" title="click to collapse or expand..."> more... </a>
 <div id="label265" style="display:none">
 <table border="1">
 <tr>
 <td></td>
 <td colspan="3">Supported Version Ranges</td>
 </tr>
 <tr>
 <td>mbms_ses_stop_response</td>
 <td><code class="docutils literal notranslate">v6.0.0 -> v7.0.8 </code></td>
 <td><code class="docutils literal notranslate">v7.2.0 -> v7.2.4 </code></td>
 <td><code class="docutils literal notranslate">v7.4.3 -> 7.6.0 </code></td>
 </tr>
 </table>
 </div>
 </li>
            <li> <span class="li-head">note_ms_request</span> - Rate limit for note MS GPRS present request (packets per second). <span class="li-normal">type: int</span>
 <a id='label266' href="javascript:ContentClick('label267', 'label266');" onmouseover="ContentPreview('label267');" onmouseout="ContentUnpreview('label267');" title="click to collapse or expand..."> more... </a>
 <div id="label267" style="display:none">
 <table border="1">
 <tr>
 <td></td>
 <td colspan="3">Supported Version Ranges</td>
 </tr>
 <tr>
 <td>note_ms_request</td>
 <td><code class="docutils literal notranslate">v6.0.0 -> v7.0.8 </code></td>
 <td><code class="docutils literal notranslate">v7.2.0 -> v7.2.4 </code></td>
 <td><code class="docutils literal notranslate">v7.4.3 -> 7.6.0 </code></td>
 </tr>
 </table>
 </div>
 </li>
            <li> <span class="li-head">note_ms_response</span> - Rate limit for note MS GPRS present response (packets per second). <span class="li-normal">type: int</span>
 <a id='label268' href="javascript:ContentClick('label269', 'label268');" onmouseover="ContentPreview('label269');" onmouseout="ContentUnpreview('label269');" title="click to collapse or expand..."> more... </a>
 <div id="label269" style="display:none">
 <table border="1">
 <tr>
 <td></td>
 <td colspan="3">Supported Version Ranges</td>
 </tr>
 <tr>
 <td>note_ms_response</td>
 <td><code class="docutils literal notranslate">v6.0.0 -> v7.0.8 </code></td>
 <td><code class="docutils literal notranslate">v7.2.0 -> v7.2.4 </code></td>
 <td><code class="docutils literal notranslate">v7.4.3 -> 7.6.0 </code></td>
 </tr>
 </table>
 </div>
 </li>
            <li> <span class="li-head">pdu_notify_rej_request</span> - Rate limit for PDU notify reject request (packets per second). <span class="li-normal">type: int</span>
 <a id='label270' href="javascript:ContentClick('label271', 'label270');" onmouseover="ContentPreview('label271');" onmouseout="ContentUnpreview('label271');" title="click to collapse or expand..."> more... </a>
 <div id="label271" style="display:none">
 <table border="1">
 <tr>
 <td></td>
 <td colspan="3">Supported Version Ranges</td>
 </tr>
 <tr>
 <td>pdu_notify_rej_request</td>
 <td><code class="docutils literal notranslate">v6.0.0 -> v7.0.8 </code></td>
 <td><code class="docutils literal notranslate">v7.2.0 -> v7.2.4 </code></td>
 <td><code class="docutils literal notranslate">v7.4.3 -> 7.6.0 </code></td>
 </tr>
 </table>
 </div>
 </li>
            <li> <span class="li-head">pdu_notify_rej_response</span> - Rate limit for PDU notify reject response (packets per second). <span class="li-normal">type: int</span>
 <a id='label272' href="javascript:ContentClick('label273', 'label272');" onmouseover="ContentPreview('label273');" onmouseout="ContentUnpreview('label273');" title="click to collapse or expand..."> more... </a>
 <div id="label273" style="display:none">
 <table border="1">
 <tr>
 <td></td>
 <td colspan="3">Supported Version Ranges</td>
 </tr>
 <tr>
 <td>pdu_notify_rej_response</td>
 <td><code class="docutils literal notranslate">v6.0.0 -> v7.0.8 </code></td>
 <td><code class="docutils literal notranslate">v7.2.0 -> v7.2.4 </code></td>
 <td><code class="docutils literal notranslate">v7.4.3 -> 7.6.0 </code></td>
 </tr>
 </table>
 </div>
 </li>
            <li> <span class="li-head">pdu_notify_request</span> - Rate limit for PDU notify request (packets per second). <span class="li-normal">type: int</span>
 <a id='label274' href="javascript:ContentClick('label275', 'label274');" onmouseover="ContentPreview('label275');" onmouseout="ContentUnpreview('label275');" title="click to collapse or expand..."> more... </a>
 <div id="label275" style="display:none">
 <table border="1">
 <tr>
 <td></td>
 <td colspan="3">Supported Version Ranges</td>
 </tr>
 <tr>
 <td>pdu_notify_request</td>
 <td><code class="docutils literal notranslate">v6.0.0 -> v7.0.8 </code></td>
 <td><code class="docutils literal notranslate">v7.2.0 -> v7.2.4 </code></td>
 <td><code class="docutils literal notranslate">v7.4.3 -> 7.6.0 </code></td>
 </tr>
 </table>
 </div>
 </li>
            <li> <span class="li-head">pdu_notify_response</span> - Rate limit for PDU notify response (packets per second). <span class="li-normal">type: int</span>
 <a id='label276' href="javascript:ContentClick('label277', 'label276');" onmouseover="ContentPreview('label277');" onmouseout="ContentUnpreview('label277');" title="click to collapse or expand..."> more... </a>
 <div id="label277" style="display:none">
 <table border="1">
 <tr>
 <td></td>
 <td colspan="3">Supported Version Ranges</td>
 </tr>
 <tr>
 <td>pdu_notify_response</td>
 <td><code class="docutils literal notranslate">v6.0.0 -> v7.0.8 </code></td>
 <td><code class="docutils literal notranslate">v7.2.0 -> v7.2.4 </code></td>
 <td><code class="docutils literal notranslate">v7.4.3 -> 7.6.0 </code></td>
 </tr>
 </table>
 </div>
 </li>
            <li> <span class="li-head">ran_info</span> - Rate limit for RAN information relay (packets per second). <span class="li-normal">type: int</span>
 <a id='label278' href="javascript:ContentClick('label279', 'label278');" onmouseover="ContentPreview('label279');" onmouseout="ContentUnpreview('label279');" title="click to collapse or expand..."> more... </a>
 <div id="label279" style="display:none">
 <table border="1">
 <tr>
 <td></td>
 <td colspan="3">Supported Version Ranges</td>
 </tr>
 <tr>
 <td>ran_info</td>
 <td><code class="docutils literal notranslate">v6.0.0 -> v7.0.8 </code></td>
 <td><code class="docutils literal notranslate">v7.2.0 -> v7.2.4 </code></td>
 <td><code class="docutils literal notranslate">v7.4.3 -> 7.6.0 </code></td>
 </tr>
 </table>
 </div>
 </li>
            <li> <span class="li-head">relocation_cancel_request</span> - Rate limit for relocation cancel request (packets per second). <span class="li-normal">type: int</span>
 <a id='label280' href="javascript:ContentClick('label281', 'label280');" onmouseover="ContentPreview('label281');" onmouseout="ContentUnpreview('label281');" title="click to collapse or expand..."> more... </a>
 <div id="label281" style="display:none">
 <table border="1">
 <tr>
 <td></td>
 <td colspan="3">Supported Version Ranges</td>
 </tr>
 <tr>
 <td>relocation_cancel_request</td>
 <td><code class="docutils literal notranslate">v6.0.0 -> v7.0.8 </code></td>
 <td><code class="docutils literal notranslate">v7.2.0 -> v7.2.4 </code></td>
 <td><code class="docutils literal notranslate">v7.4.3 -> 7.6.0 </code></td>
 </tr>
 </table>
 </div>
 </li>
            <li> <span class="li-head">relocation_cancel_response</span> - Rate limit for relocation cancel response (packets per second). <span class="li-normal">type: int</span>
 <a id='label282' href="javascript:ContentClick('label283', 'label282');" onmouseover="ContentPreview('label283');" onmouseout="ContentUnpreview('label283');" title="click to collapse or expand..."> more... </a>
 <div id="label283" style="display:none">
 <table border="1">
 <tr>
 <td></td>
 <td colspan="3">Supported Version Ranges</td>
 </tr>
 <tr>
 <td>relocation_cancel_response</td>
 <td><code class="docutils literal notranslate">v6.0.0 -> v7.0.8 </code></td>
 <td><code class="docutils literal notranslate">v7.2.0 -> v7.2.4 </code></td>
 <td><code class="docutils literal notranslate">v7.4.3 -> 7.6.0 </code></td>
 </tr>
 </table>
 </div>
 </li>
            <li> <span class="li-head">send_route_request</span> - Rate limit for send routing information for GPRS request (packets per second). <span class="li-normal">type: int</span>
 <a id='label284' href="javascript:ContentClick('label285', 'label284');" onmouseover="ContentPreview('label285');" onmouseout="ContentUnpreview('label285');" title="click to collapse or expand..."> more... </a>
 <div id="label285" style="display:none">
 <table border="1">
 <tr>
 <td></td>
 <td colspan="3">Supported Version Ranges</td>
 </tr>
 <tr>
 <td>send_route_request</td>
 <td><code class="docutils literal notranslate">v6.0.0 -> v7.0.8 </code></td>
 <td><code class="docutils literal notranslate">v7.2.0 -> v7.2.4 </code></td>
 <td><code class="docutils literal notranslate">v7.4.3 -> 7.6.0 </code></td>
 </tr>
 </table>
 </div>
 </li>
            <li> <span class="li-head">send_route_response</span> - Rate limit for send routing information for GPRS response (packets per second). <span class="li-normal">type: int</span>
 <a id='label286' href="javascript:ContentClick('label287', 'label286');" onmouseover="ContentPreview('label287');" onmouseout="ContentUnpreview('label287');" title="click to collapse or expand..."> more... </a>
 <div id="label287" style="display:none">
 <table border="1">
 <tr>
 <td></td>
 <td colspan="3">Supported Version Ranges</td>
 </tr>
 <tr>
 <td>send_route_response</td>
 <td><code class="docutils literal notranslate">v6.0.0 -> v7.0.8 </code></td>
 <td><code class="docutils literal notranslate">v7.2.0 -> v7.2.4 </code></td>
 <td><code class="docutils literal notranslate">v7.4.3 -> 7.6.0 </code></td>
 </tr>
 </table>
 </div>
 </li>
            <li> <span class="li-head">sgsn_context_ack</span> - Rate limit for SGSN context acknowledgement (packets per second). <span class="li-normal">type: int</span>
 <a id='label288' href="javascript:ContentClick('label289', 'label288');" onmouseover="ContentPreview('label289');" onmouseout="ContentUnpreview('label289');" title="click to collapse or expand..."> more... </a>
 <div id="label289" style="display:none">
 <table border="1">
 <tr>
 <td></td>
 <td colspan="3">Supported Version Ranges</td>
 </tr>
 <tr>
 <td>sgsn_context_ack</td>
 <td><code class="docutils literal notranslate">v6.0.0 -> v7.0.8 </code></td>
 <td><code class="docutils literal notranslate">v7.2.0 -> v7.2.4 </code></td>
 <td><code class="docutils literal notranslate">v7.4.3 -> 7.6.0 </code></td>
 </tr>
 </table>
 </div>
 </li>
            <li> <span class="li-head">sgsn_context_request</span> - Rate limit for SGSN context request (packets per second). <span class="li-normal">type: int</span>
 <a id='label290' href="javascript:ContentClick('label291', 'label290');" onmouseover="ContentPreview('label291');" onmouseout="ContentUnpreview('label291');" title="click to collapse or expand..."> more... </a>
 <div id="label291" style="display:none">
 <table border="1">
 <tr>
 <td></td>
 <td colspan="3">Supported Version Ranges</td>
 </tr>
 <tr>
 <td>sgsn_context_request</td>
 <td><code class="docutils literal notranslate">v6.0.0 -> v7.0.8 </code></td>
 <td><code class="docutils literal notranslate">v7.2.0 -> v7.2.4 </code></td>
 <td><code class="docutils literal notranslate">v7.4.3 -> 7.6.0 </code></td>
 </tr>
 </table>
 </div>
 </li>
            <li> <span class="li-head">sgsn_context_response</span> - Rate limit for SGSN context response (packets per second). <span class="li-normal">type: int</span>
 <a id='label292' href="javascript:ContentClick('label293', 'label292');" onmouseover="ContentPreview('label293');" onmouseout="ContentUnpreview('label293');" title="click to collapse or expand..."> more... </a>
 <div id="label293" style="display:none">
 <table border="1">
 <tr>
 <td></td>
 <td colspan="3">Supported Version Ranges</td>
 </tr>
 <tr>
 <td>sgsn_context_response</td>
 <td><code class="docutils literal notranslate">v6.0.0 -> v7.0.8 </code></td>
 <td><code class="docutils literal notranslate">v7.2.0 -> v7.2.4 </code></td>
 <td><code class="docutils literal notranslate">v7.4.3 -> 7.6.0 </code></td>
 </tr>
 </table>
 </div>
 </li>
            <li> <span class="li-head">support_ext_hdr_notify</span> - Rate limit for support extension headers notification (packets per second). <span class="li-normal">type: int</span>
 <a id='label294' href="javascript:ContentClick('label295', 'label294');" onmouseover="ContentPreview('label295');" onmouseout="ContentUnpreview('label295');" title="click to collapse or expand..."> more... </a>
 <div id="label295" style="display:none">
 <table border="1">
 <tr>
 <td></td>
 <td colspan="3">Supported Version Ranges</td>
 </tr>
 <tr>
 <td>support_ext_hdr_notify</td>
 <td><code class="docutils literal notranslate">v6.0.0 -> v7.0.8 </code></td>
 <td><code class="docutils literal notranslate">v7.2.0 -> v7.2.4 </code></td>
 <td><code class="docutils literal notranslate">v7.4.3 -> 7.6.0 </code></td>
 </tr>
 </table>
 </div>
 </li>
            <li> <span class="li-head">update_mbms_request</span> - Rate limit for update MBMS context request (packets per second). <span class="li-normal">type: int</span>
 <a id='label296' href="javascript:ContentClick('label297', 'label296');" onmouseover="ContentPreview('label297');" onmouseout="ContentUnpreview('label297');" title="click to collapse or expand..."> more... </a>
 <div id="label297" style="display:none">
 <table border="1">
 <tr>
 <td></td>
 <td colspan="3">Supported Version Ranges</td>
 </tr>
 <tr>
 <td>update_mbms_request</td>
 <td><code class="docutils literal notranslate">v6.0.0 -> v7.0.8 </code></td>
 <td><code class="docutils literal notranslate">v7.2.0 -> v7.2.4 </code></td>
 <td><code class="docutils literal notranslate">v7.4.3 -> 7.6.0 </code></td>
 </tr>
 </table>
 </div>
 </li>
            <li> <span class="li-head">update_mbms_response</span> - Rate limit for update MBMS context response (packets per second). <span class="li-normal">type: int</span>
 <a id='label298' href="javascript:ContentClick('label299', 'label298');" onmouseover="ContentPreview('label299');" onmouseout="ContentUnpreview('label299');" title="click to collapse or expand..."> more... </a>
 <div id="label299" style="display:none">
 <table border="1">
 <tr>
 <td></td>
 <td colspan="3">Supported Version Ranges</td>
 </tr>
 <tr>
 <td>update_mbms_response</td>
 <td><code class="docutils literal notranslate">v6.0.0 -> v7.0.8 </code></td>
 <td><code class="docutils literal notranslate">v7.2.0 -> v7.2.4 </code></td>
 <td><code class="docutils literal notranslate">v7.4.3 -> 7.6.0 </code></td>
 </tr>
 </table>
 </div>
 </li>
            <li> <span class="li-head">update_pdp_request</span> - Rate limit for update PDP context request (packets per second). <span class="li-normal">type: int</span>
 <a id='label300' href="javascript:ContentClick('label301', 'label300');" onmouseover="ContentPreview('label301');" onmouseout="ContentUnpreview('label301');" title="click to collapse or expand..."> more... </a>
 <div id="label301" style="display:none">
 <table border="1">
 <tr>
 <td></td>
 <td colspan="3">Supported Version Ranges</td>
 </tr>
 <tr>
 <td>update_pdp_request</td>
 <td><code class="docutils literal notranslate">v6.0.0 -> v7.0.8 </code></td>
 <td><code class="docutils literal notranslate">v7.2.0 -> v7.2.4 </code></td>
 <td><code class="docutils literal notranslate">v7.4.3 -> 7.6.0 </code></td>
 </tr>
 </table>
 </div>
 </li>
            <li> <span class="li-head">update_pdp_response</span> - Rate limit for update PDP context response (packets per second). <span class="li-normal">type: int</span>
 <a id='label302' href="javascript:ContentClick('label303', 'label302');" onmouseover="ContentPreview('label303');" onmouseout="ContentUnpreview('label303');" title="click to collapse or expand..."> more... </a>
 <div id="label303" style="display:none">
 <table border="1">
 <tr>
 <td></td>
 <td colspan="3">Supported Version Ranges</td>
 </tr>
 <tr>
 <td>update_pdp_response</td>
 <td><code class="docutils literal notranslate">v6.0.0 -> v7.0.8 </code></td>
 <td><code class="docutils literal notranslate">v7.2.0 -> v7.2.4 </code></td>
 <td><code class="docutils literal notranslate">v7.4.3 -> 7.6.0 </code></td>
 </tr>
 </table>
 </div>
 </li>
            <li> <span class="li-head">version_not_support</span> - Rate limit for version not supported (packets per second). <span class="li-normal">type: int</span>
 <a id='label304' href="javascript:ContentClick('label305', 'label304');" onmouseover="ContentPreview('label305');" onmouseout="ContentUnpreview('label305');" title="click to collapse or expand..."> more... </a>
 <div id="label305" style="display:none">
 <table border="1">
 <tr>
 <td></td>
 <td colspan="3">Supported Version Ranges</td>
 </tr>
 <tr>
 <td>version_not_support</td>
 <td><code class="docutils literal notranslate">v6.0.0 -> v7.0.8 </code></td>
 <td><code class="docutils literal notranslate">v7.2.0 -> v7.2.4 </code></td>
 <td><code class="docutils literal notranslate">v7.4.3 -> 7.6.0 </code></td>
 </tr>
 </table>
 </div>
 </li>
            </ul>
        <li> <span class="li-head">message_rate_limit_v0</span> - Message rate limiting for GTP version 0. <span class="li-normal">type: dict</span>
 <a id='label306' href="javascript:ContentClick('label307', 'label306');" onmouseover="ContentPreview('label307');" onmouseout="ContentUnpreview('label307');" title="click to collapse or expand..."> more... </a>
 <div id="label307" style="display:none">
 <table border="1">
 <tr>
 <td></td><td colspan="3">Supported Version Ranges</td>
 </tr>
 <tr>
 <td>message_rate_limit_v0</td>
 <td><code class="docutils literal notranslate">v6.0.0 -> v7.0.8 </code></td>
 <td><code class="docutils literal notranslate">v7.2.0 -> v7.2.4 </code></td>
 <td><code class="docutils literal notranslate">v7.4.3 -> 7.6.0 </code></td>
 </tr>
 </table>
 </div>
 </li>
            <ul class="ul-self">
            <li> <span class="li-head">create_pdp_request</span> - Rate limit (packets/s) for create PDP context request. <span class="li-normal">type: int</span>
 <a id='label308' href="javascript:ContentClick('label309', 'label308');" onmouseover="ContentPreview('label309');" onmouseout="ContentUnpreview('label309');" title="click to collapse or expand..."> more... </a>
 <div id="label309" style="display:none">
 <table border="1">
 <tr>
 <td></td>
 <td colspan="3">Supported Version Ranges</td>
 </tr>
 <tr>
 <td>create_pdp_request</td>
 <td><code class="docutils literal notranslate">v6.0.0 -> v7.0.8 </code></td>
 <td><code class="docutils literal notranslate">v7.2.0 -> v7.2.4 </code></td>
 <td><code class="docutils literal notranslate">v7.4.3 -> 7.6.0 </code></td>
 </tr>
 </table>
 </div>
 </li>
            <li> <span class="li-head">delete_pdp_request</span> - Rate limit (packets/s) for delete PDP context request. <span class="li-normal">type: int</span>
 <a id='label310' href="javascript:ContentClick('label311', 'label310');" onmouseover="ContentPreview('label311');" onmouseout="ContentUnpreview('label311');" title="click to collapse or expand..."> more... </a>
 <div id="label311" style="display:none">
 <table border="1">
 <tr>
 <td></td>
 <td colspan="3">Supported Version Ranges</td>
 </tr>
 <tr>
 <td>delete_pdp_request</td>
 <td><code class="docutils literal notranslate">v6.0.0 -> v7.0.8 </code></td>
 <td><code class="docutils literal notranslate">v7.2.0 -> v7.2.4 </code></td>
 <td><code class="docutils literal notranslate">v7.4.3 -> 7.6.0 </code></td>
 </tr>
 </table>
 </div>
 </li>
            <li> <span class="li-head">echo_request</span> - Rate limit (packets/s) for echo request. <span class="li-normal">type: int</span>
 <a id='label312' href="javascript:ContentClick('label313', 'label312');" onmouseover="ContentPreview('label313');" onmouseout="ContentUnpreview('label313');" title="click to collapse or expand..."> more... </a>
 <div id="label313" style="display:none">
 <table border="1">
 <tr>
 <td></td>
 <td colspan="3">Supported Version Ranges</td>
 </tr>
 <tr>
 <td>echo_request</td>
 <td><code class="docutils literal notranslate">v6.0.0 -> v7.0.8 </code></td>
 <td><code class="docutils literal notranslate">v7.2.0 -> v7.2.4 </code></td>
 <td><code class="docutils literal notranslate">v7.4.3 -> 7.6.0 </code></td>
 </tr>
 </table>
 </div>
 </li>
            </ul>
        <li> <span class="li-head">message_rate_limit_v1</span> - Message rate limiting for GTP version 1. <span class="li-normal">type: dict</span>
 <a id='label314' href="javascript:ContentClick('label315', 'label314');" onmouseover="ContentPreview('label315');" onmouseout="ContentUnpreview('label315');" title="click to collapse or expand..."> more... </a>
 <div id="label315" style="display:none">
 <table border="1">
 <tr>
 <td></td><td colspan="3">Supported Version Ranges</td>
 </tr>
 <tr>
 <td>message_rate_limit_v1</td>
 <td><code class="docutils literal notranslate">v6.0.0 -> v7.0.8 </code></td>
 <td><code class="docutils literal notranslate">v7.2.0 -> v7.2.4 </code></td>
 <td><code class="docutils literal notranslate">v7.4.3 -> 7.6.0 </code></td>
 </tr>
 </table>
 </div>
 </li>
            <ul class="ul-self">
            <li> <span class="li-head">create_pdp_request</span> - Rate limit (packets/s) for create PDP context request. <span class="li-normal">type: int</span>
 <a id='label316' href="javascript:ContentClick('label317', 'label316');" onmouseover="ContentPreview('label317');" onmouseout="ContentUnpreview('label317');" title="click to collapse or expand..."> more... </a>
 <div id="label317" style="display:none">
 <table border="1">
 <tr>
 <td></td>
 <td colspan="3">Supported Version Ranges</td>
 </tr>
 <tr>
 <td>create_pdp_request</td>
 <td><code class="docutils literal notranslate">v6.0.0 -> v7.0.8 </code></td>
 <td><code class="docutils literal notranslate">v7.2.0 -> v7.2.4 </code></td>
 <td><code class="docutils literal notranslate">v7.4.3 -> 7.6.0 </code></td>
 </tr>
 </table>
 </div>
 </li>
            <li> <span class="li-head">delete_pdp_request</span> - Rate limit (packets/s) for delete PDP context request. <span class="li-normal">type: int</span>
 <a id='label318' href="javascript:ContentClick('label319', 'label318');" onmouseover="ContentPreview('label319');" onmouseout="ContentUnpreview('label319');" title="click to collapse or expand..."> more... </a>
 <div id="label319" style="display:none">
 <table border="1">
 <tr>
 <td></td>
 <td colspan="3">Supported Version Ranges</td>
 </tr>
 <tr>
 <td>delete_pdp_request</td>
 <td><code class="docutils literal notranslate">v6.0.0 -> v7.0.8 </code></td>
 <td><code class="docutils literal notranslate">v7.2.0 -> v7.2.4 </code></td>
 <td><code class="docutils literal notranslate">v7.4.3 -> 7.6.0 </code></td>
 </tr>
 </table>
 </div>
 </li>
            <li> <span class="li-head">echo_request</span> - Rate limit (packets/s) for echo request. <span class="li-normal">type: int</span>
 <a id='label320' href="javascript:ContentClick('label321', 'label320');" onmouseover="ContentPreview('label321');" onmouseout="ContentUnpreview('label321');" title="click to collapse or expand..."> more... </a>
 <div id="label321" style="display:none">
 <table border="1">
 <tr>
 <td></td>
 <td colspan="3">Supported Version Ranges</td>
 </tr>
 <tr>
 <td>echo_request</td>
 <td><code class="docutils literal notranslate">v6.0.0 -> v7.0.8 </code></td>
 <td><code class="docutils literal notranslate">v7.2.0 -> v7.2.4 </code></td>
 <td><code class="docutils literal notranslate">v7.4.3 -> 7.6.0 </code></td>
 </tr>
 </table>
 </div>
 </li>
            </ul>
        <li> <span class="li-head">message_rate_limit_v2</span> - Message rate limiting for GTP version 2. <span class="li-normal">type: dict</span>
 <a id='label322' href="javascript:ContentClick('label323', 'label322');" onmouseover="ContentPreview('label323');" onmouseout="ContentUnpreview('label323');" title="click to collapse or expand..."> more... </a>
 <div id="label323" style="display:none">
 <table border="1">
 <tr>
 <td></td><td colspan="3">Supported Version Ranges</td>
 </tr>
 <tr>
 <td>message_rate_limit_v2</td>
 <td><code class="docutils literal notranslate">v6.0.0 -> v7.0.8 </code></td>
 <td><code class="docutils literal notranslate">v7.2.0 -> v7.2.4 </code></td>
 <td><code class="docutils literal notranslate">v7.4.3 -> 7.6.0 </code></td>
 </tr>
 </table>
 </div>
 </li>
            <ul class="ul-self">
            <li> <span class="li-head">create_session_request</span> - Rate limit (packets/s) for create session request. <span class="li-normal">type: int</span>
 <a id='label324' href="javascript:ContentClick('label325', 'label324');" onmouseover="ContentPreview('label325');" onmouseout="ContentUnpreview('label325');" title="click to collapse or expand..."> more... </a>
 <div id="label325" style="display:none">
 <table border="1">
 <tr>
 <td></td>
 <td colspan="3">Supported Version Ranges</td>
 </tr>
 <tr>
 <td>create_session_request</td>
 <td><code class="docutils literal notranslate">v6.0.0 -> v7.0.8 </code></td>
 <td><code class="docutils literal notranslate">v7.2.0 -> v7.2.4 </code></td>
 <td><code class="docutils literal notranslate">v7.4.3 -> 7.6.0 </code></td>
 </tr>
 </table>
 </div>
 </li>
            <li> <span class="li-head">delete_session_request</span> - Rate limit (packets/s) for delete session request. <span class="li-normal">type: int</span>
 <a id='label326' href="javascript:ContentClick('label327', 'label326');" onmouseover="ContentPreview('label327');" onmouseout="ContentUnpreview('label327');" title="click to collapse or expand..."> more... </a>
 <div id="label327" style="display:none">
 <table border="1">
 <tr>
 <td></td>
 <td colspan="3">Supported Version Ranges</td>
 </tr>
 <tr>
 <td>delete_session_request</td>
 <td><code class="docutils literal notranslate">v6.0.0 -> v7.0.8 </code></td>
 <td><code class="docutils literal notranslate">v7.2.0 -> v7.2.4 </code></td>
 <td><code class="docutils literal notranslate">v7.4.3 -> 7.6.0 </code></td>
 </tr>
 </table>
 </div>
 </li>
            <li> <span class="li-head">echo_request</span> - Rate limit (packets/s) for echo request. <span class="li-normal">type: int</span>
 <a id='label328' href="javascript:ContentClick('label329', 'label328');" onmouseover="ContentPreview('label329');" onmouseout="ContentUnpreview('label329');" title="click to collapse or expand..."> more... </a>
 <div id="label329" style="display:none">
 <table border="1">
 <tr>
 <td></td>
 <td colspan="3">Supported Version Ranges</td>
 </tr>
 <tr>
 <td>echo_request</td>
 <td><code class="docutils literal notranslate">v6.0.0 -> v7.0.8 </code></td>
 <td><code class="docutils literal notranslate">v7.2.0 -> v7.2.4 </code></td>
 <td><code class="docutils literal notranslate">v7.4.3 -> 7.6.0 </code></td>
 </tr>
 </table>
 </div>
 </li>
            </ul>
        <li> <span class="li-head">min_message_length</span> - min message length <span class="li-normal">type: int</span>
 <a id='label330' href="javascript:ContentClick('label331', 'label330');" onmouseover="ContentPreview('label331');" onmouseout="ContentUnpreview('label331');" title="click to collapse or expand..."> more... </a>
 <div id="label331" style="display:none">
 <table border="1">
 <tr>
 <td></td>
 <td colspan="3">Supported Version Ranges</td>
 </tr>
 <tr>
 <td>min_message_length</td>
 <td><code class="docutils literal notranslate">v6.0.0 -> v7.0.8 </code></td>
 <td><code class="docutils literal notranslate">v7.2.0 -> v7.2.4 </code></td>
 <td><code class="docutils literal notranslate">v7.4.3 -> 7.6.0 </code></td>
 </tr>
 </table>
 </div>
 </li>
        <li> <span class="li-head">miss_must_ie</span> - Missing mandatory information element <span class="li-normal">type: str</span> <span class="li-normal">choices: allow, deny</span>
 <a id='label332' href="javascript:ContentClick('label333', 'label332');" onmouseover="ContentPreview('label333');" onmouseout="ContentUnpreview('label333');" title="click to collapse or expand..."> more... </a>
 <div id="label333" style="display:none">
 <table border="1">
 <tr>
 <td></td>
 <td colspan="3">Supported Version Ranges</td>
 </tr>
 <tr>
 <td>miss_must_ie</td>
 <td><code class="docutils literal notranslate">v6.0.0 -> v7.0.8 </code></td>
 <td><code class="docutils literal notranslate">v7.2.0 -> v7.2.4 </code></td>
 <td><code class="docutils literal notranslate">v7.4.3 -> 7.6.0 </code></td>
 </tr>
 <tr>
 <td>[allow]</td>
 <td><code class="docutils literal notranslate">v6.0.0 -> v7.0.8</code></td>
 <tr>
 <td>[deny]</td>
 <td><code class="docutils literal notranslate">v6.0.0 -> v7.0.8</code></td>
 </table>
 </div>
 </li>
        <li> <span class="li-head">monitor_mode</span> - GTP monitor mode. <span class="li-normal">type: str</span> <span class="li-normal">choices: enable, disable, vdom</span>
 <a id='label334' href="javascript:ContentClick('label335', 'label334');" onmouseover="ContentPreview('label335');" onmouseout="ContentUnpreview('label335');" title="click to collapse or expand..."> more... </a>
 <div id="label335" style="display:none">
 <table border="1">
 <tr>
 <td></td>
 <td colspan="3">Supported Version Ranges</td>
 </tr>
 <tr>
 <td>monitor_mode</td>
 <td><code class="docutils literal notranslate">v6.0.0 -> v7.0.8 </code></td>
 <td><code class="docutils literal notranslate">v7.2.0 -> v7.2.4 </code></td>
 <td><code class="docutils literal notranslate">v7.4.3 -> 7.6.0 </code></td>
 </tr>
 <tr>
 <td>[enable]</td>
 <td><code class="docutils literal notranslate">v6.0.0 -> v7.0.8</code></td>
 <tr>
 <td>[disable]</td>
 <td><code class="docutils literal notranslate">v6.0.0 -> v7.0.8</code></td>
 <tr>
 <td>[vdom]</td>
 <td><code class="docutils literal notranslate">v6.2.0 -> v7.0.8</code></td>
 <td><code class="docutils literal notranslate">v7.2.0 -> v7.2.4</code></td>
 <td><code class="docutils literal notranslate">v7.4.3 -> 7.6.0</code></td>
 </tr>
 </table>
 </div>
 </li>
        <li> <span class="li-head">name</span> - Profile name. <span class="li-normal">type: str</span> <span class="li-required">required: true</span>
 <a id='label336' href="javascript:ContentClick('label337', 'label336');" onmouseover="ContentPreview('label337');" onmouseout="ContentUnpreview('label337');" title="click to collapse or expand..."> more... </a>
 <div id="label337" style="display:none">
 <table border="1">
 <tr>
 <td></td>
 <td colspan="3">Supported Version Ranges</td>
 </tr>
 <tr>
 <td>name</td>
 <td><code class="docutils literal notranslate">v6.0.0 -> v7.0.8 </code></td>
 <td><code class="docutils literal notranslate">v7.2.0 -> v7.2.4 </code></td>
 <td><code class="docutils literal notranslate">v7.4.3 -> 7.6.0 </code></td>
 </tr>
 </table>
 </div>
 </li>
        <li> <span class="li-head">noip_filter</span> - non-IP filter for encapsulted traffic <span class="li-normal">type: str</span> <span class="li-normal">choices: enable, disable</span>
 <a id='label338' href="javascript:ContentClick('label339', 'label338');" onmouseover="ContentPreview('label339');" onmouseout="ContentUnpreview('label339');" title="click to collapse or expand..."> more... </a>
 <div id="label339" style="display:none">
 <table border="1">
 <tr>
 <td></td>
 <td colspan="3">Supported Version Ranges</td>
 </tr>
 <tr>
 <td>noip_filter</td>
 <td><code class="docutils literal notranslate">v6.0.0 -> v7.0.8 </code></td>
 <td><code class="docutils literal notranslate">v7.2.0 -> v7.2.4 </code></td>
 <td><code class="docutils literal notranslate">v7.4.3 -> 7.6.0 </code></td>
 </tr>
 <tr>
 <td>[enable]</td>
 <td><code class="docutils literal notranslate">v6.0.0 -> v7.0.8</code></td>
 <tr>
 <td>[disable]</td>
 <td><code class="docutils literal notranslate">v6.0.0 -> v7.0.8</code></td>
 </table>
 </div>
 </li>
        <li> <span class="li-head">noip_policy</span> - No IP policy. <span class="li-normal">type: list</span> <span style="font-family:'Courier New'" class="li-required">member_path: noip_policy:id</span>
 <a id='label340' href="javascript:ContentClick('label341', 'label340');" onmouseover="ContentPreview('label341');" onmouseout="ContentUnpreview('label341');" title="click to collapse or expand..."> more... </a>
 <div id="label341" style="display:none">
 <table border="1">
 <tr>
 <td></td><td colspan="3">Supported Version Ranges</td>
 </tr>
 <tr>
 <td>noip_policy</td>
 <td><code class="docutils literal notranslate">v6.0.0 -> v7.0.8 </code></td>
 <td><code class="docutils literal notranslate">v7.2.0 -> v7.2.4 </code></td>
 <td><code class="docutils literal notranslate">v7.4.3 -> 7.6.0 </code></td>
 </tr>
 </table>
 </div>
 </li>
            <ul class="ul-self">
            <li> <span class="li-head">action</span> - Action. <span class="li-normal">type: str</span> <span class="li-normal">choices: allow, deny</span>
 <a id='label342' href="javascript:ContentClick('label343', 'label342');" onmouseover="ContentPreview('label343');" onmouseout="ContentUnpreview('label343');" title="click to collapse or expand..."> more... </a>
 <div id="label343" style="display:none">
 <table border="1">
 <tr>
 <td></td>
 <td colspan="3">Supported Version Ranges</td>
 </tr>
 <tr>
 <td>action</td>
 <td><code class="docutils literal notranslate">v6.0.0 -> v7.0.8 </code></td>
 <td><code class="docutils literal notranslate">v7.2.0 -> v7.2.4 </code></td>
 <td><code class="docutils literal notranslate">v7.4.3 -> 7.6.0 </code></td>
 </tr>
 <tr>
 <td>[allow]</td>
 <td><code class="docutils literal notranslate">v6.0.0 -> v7.0.8</code></td>
 <tr>
 <td>[deny]</td>
 <td><code class="docutils literal notranslate">v6.0.0 -> v7.0.8</code></td>
 </table>
 </div>
 </li>
            <li> <span class="li-head">end</span> - End of protocol range (0 - 255). <span class="li-normal">type: int</span>
 <a id='label344' href="javascript:ContentClick('label345', 'label344');" onmouseover="ContentPreview('label345');" onmouseout="ContentUnpreview('label345');" title="click to collapse or expand..."> more... </a>
 <div id="label345" style="display:none">
 <table border="1">
 <tr>
 <td></td>
 <td colspan="3">Supported Version Ranges</td>
 </tr>
 <tr>
 <td>end</td>
 <td><code class="docutils literal notranslate">v6.0.0 -> v7.0.8 </code></td>
 <td><code class="docutils literal notranslate">v7.2.0 -> v7.2.4 </code></td>
 <td><code class="docutils literal notranslate">v7.4.3 -> 7.6.0 </code></td>
 </tr>
 </table>
 </div>
 </li>
            <li> <span class="li-head">id</span> - ID. see <a href='#notes'>Notes</a>. <span class="li-normal">type: int</span> <span class="li-required">required: true</span>
 <a id='label346' href="javascript:ContentClick('label347', 'label346');" onmouseover="ContentPreview('label347');" onmouseout="ContentUnpreview('label347');" title="click to collapse or expand..."> more... </a>
 <div id="label347" style="display:none">
 <table border="1">
 <tr>
 <td></td>
 <td colspan="3">Supported Version Ranges</td>
 </tr>
 <tr>
 <td>id</td>
 <td><code class="docutils literal notranslate">v6.0.0 -> v7.0.8 </code></td>
 <td><code class="docutils literal notranslate">v7.2.0 -> v7.2.4 </code></td>
 <td><code class="docutils literal notranslate">v7.4.3 -> 7.6.0 </code></td>
 </tr>
 </table>
 </div>
 </li>
            <li> <span class="li-head">start</span> - Start of protocol range (0 - 255). <span class="li-normal">type: int</span>
 <a id='label348' href="javascript:ContentClick('label349', 'label348');" onmouseover="ContentPreview('label349');" onmouseout="ContentUnpreview('label349');" title="click to collapse or expand..."> more... </a>
 <div id="label349" style="display:none">
 <table border="1">
 <tr>
 <td></td>
 <td colspan="3">Supported Version Ranges</td>
 </tr>
 <tr>
 <td>start</td>
 <td><code class="docutils literal notranslate">v6.0.0 -> v7.0.8 </code></td>
 <td><code class="docutils literal notranslate">v7.2.0 -> v7.2.4 </code></td>
 <td><code class="docutils literal notranslate">v7.4.3 -> 7.6.0 </code></td>
 </tr>
 </table>
 </div>
 </li>
            <li> <span class="li-head">type</span> - Protocol field type. <span class="li-normal">type: str</span> <span class="li-normal">choices: etsi, ietf</span>
 <a id='label350' href="javascript:ContentClick('label351', 'label350');" onmouseover="ContentPreview('label351');" onmouseout="ContentUnpreview('label351');" title="click to collapse or expand..."> more... </a>
 <div id="label351" style="display:none">
 <table border="1">
 <tr>
 <td></td>
 <td colspan="3">Supported Version Ranges</td>
 </tr>
 <tr>
 <td>type</td>
 <td><code class="docutils literal notranslate">v6.0.0 -> v7.0.8 </code></td>
 <td><code class="docutils literal notranslate">v7.2.0 -> v7.2.4 </code></td>
 <td><code class="docutils literal notranslate">v7.4.3 -> 7.6.0 </code></td>
 </tr>
 <tr>
 <td>[etsi]</td>
 <td><code class="docutils literal notranslate">v6.0.0 -> v7.0.8</code></td>
 <tr>
 <td>[ietf]</td>
 <td><code class="docutils literal notranslate">v6.0.0 -> v7.0.8</code></td>
 </table>
 </div>
 </li>
            </ul>
        <li> <span class="li-head">out_of_state_ie</span> - Out of state information element. <span class="li-normal">type: str</span> <span class="li-normal">choices: allow, deny</span>
 <a id='label352' href="javascript:ContentClick('label353', 'label352');" onmouseover="ContentPreview('label353');" onmouseout="ContentUnpreview('label353');" title="click to collapse or expand..."> more... </a>
 <div id="label353" style="display:none">
 <table border="1">
 <tr>
 <td></td>
 <td colspan="3">Supported Version Ranges</td>
 </tr>
 <tr>
 <td>out_of_state_ie</td>
 <td><code class="docutils literal notranslate">v6.0.0 -> v7.0.8 </code></td>
 <td><code class="docutils literal notranslate">v7.2.0 -> v7.2.4 </code></td>
 <td><code class="docutils literal notranslate">v7.4.3 -> 7.6.0 </code></td>
 </tr>
 <tr>
 <td>[allow]</td>
 <td><code class="docutils literal notranslate">v6.0.0 -> v7.0.8</code></td>
 <tr>
 <td>[deny]</td>
 <td><code class="docutils literal notranslate">v6.0.0 -> v7.0.8</code></td>
 </table>
 </div>
 </li>
        <li> <span class="li-head">out_of_state_message</span> - Out of state GTP message <span class="li-normal">type: str</span> <span class="li-normal">choices: allow, deny</span>
 <a id='label354' href="javascript:ContentClick('label355', 'label354');" onmouseover="ContentPreview('label355');" onmouseout="ContentUnpreview('label355');" title="click to collapse or expand..."> more... </a>
 <div id="label355" style="display:none">
 <table border="1">
 <tr>
 <td></td>
 <td colspan="3">Supported Version Ranges</td>
 </tr>
 <tr>
 <td>out_of_state_message</td>
 <td><code class="docutils literal notranslate">v6.0.0 -> v7.0.8 </code></td>
 <td><code class="docutils literal notranslate">v7.2.0 -> v7.2.4 </code></td>
 <td><code class="docutils literal notranslate">v7.4.3 -> 7.6.0 </code></td>
 </tr>
 <tr>
 <td>[allow]</td>
 <td><code class="docutils literal notranslate">v6.0.0 -> v7.0.8</code></td>
 <tr>
 <td>[deny]</td>
 <td><code class="docutils literal notranslate">v6.0.0 -> v7.0.8</code></td>
 </table>
 </div>
 </li>
        <li> <span class="li-head">per_apn_shaper</span> - Per APN shaper. <span class="li-normal">type: list</span> <span style="font-family:'Courier New'" class="li-required">member_path: per_apn_shaper:id</span>
 <a id='label356' href="javascript:ContentClick('label357', 'label356');" onmouseover="ContentPreview('label357');" onmouseout="ContentUnpreview('label357');" title="click to collapse or expand..."> more... </a>
 <div id="label357" style="display:none">
 <table border="1">
 <tr>
 <td></td><td colspan="3">Supported Version Ranges</td>
 </tr>
 <tr>
 <td>per_apn_shaper</td>
 <td><code class="docutils literal notranslate">v6.0.0 -> v7.0.8 </code></td>
 <td><code class="docutils literal notranslate">v7.2.0 -> v7.2.4 </code></td>
 <td><code class="docutils literal notranslate">v7.4.3 -> 7.6.0 </code></td>
 </tr>
 </table>
 </div>
 </li>
            <ul class="ul-self">
            <li> <span class="li-head">apn</span> - APN name. Source gtp.apn.name. <span class="li-normal">type: str</span>
 <a id='label358' href="javascript:ContentClick('label359', 'label358');" onmouseover="ContentPreview('label359');" onmouseout="ContentUnpreview('label359');" title="click to collapse or expand..."> more... </a>
 <div id="label359" style="display:none">
 <table border="1">
 <tr>
 <td></td>
 <td colspan="3">Supported Version Ranges</td>
 </tr>
 <tr>
 <td>apn</td>
 <td><code class="docutils literal notranslate">v6.0.0 -> v7.0.8 </code></td>
 <td><code class="docutils literal notranslate">v7.2.0 -> v7.2.4 </code></td>
 <td><code class="docutils literal notranslate">v7.4.3 -> 7.6.0 </code></td>
 </tr>
 </table>
 </div>
 </li>
            <li> <span class="li-head">id</span> - ID. see <a href='#notes'>Notes</a>. <span class="li-normal">type: int</span> <span class="li-required">required: true</span>
 <a id='label360' href="javascript:ContentClick('label361', 'label360');" onmouseover="ContentPreview('label361');" onmouseout="ContentUnpreview('label361');" title="click to collapse or expand..."> more... </a>
 <div id="label361" style="display:none">
 <table border="1">
 <tr>
 <td></td>
 <td colspan="3">Supported Version Ranges</td>
 </tr>
 <tr>
 <td>id</td>
 <td><code class="docutils literal notranslate">v6.0.0 -> v7.0.8 </code></td>
 <td><code class="docutils literal notranslate">v7.2.0 -> v7.2.4 </code></td>
 <td><code class="docutils literal notranslate">v7.4.3 -> 7.6.0 </code></td>
 </tr>
 </table>
 </div>
 </li>
            <li> <span class="li-head">rate_limit</span> - Rate limit (packets/s) for create PDP context request. <span class="li-normal">type: int</span>
 <a id='label362' href="javascript:ContentClick('label363', 'label362');" onmouseover="ContentPreview('label363');" onmouseout="ContentUnpreview('label363');" title="click to collapse or expand..."> more... </a>
 <div id="label363" style="display:none">
 <table border="1">
 <tr>
 <td></td>
 <td colspan="3">Supported Version Ranges</td>
 </tr>
 <tr>
 <td>rate_limit</td>
 <td><code class="docutils literal notranslate">v6.0.0 -> v7.0.8 </code></td>
 <td><code class="docutils literal notranslate">v7.2.0 -> v7.2.4 </code></td>
 <td><code class="docutils literal notranslate">v7.4.3 -> 7.6.0 </code></td>
 </tr>
 </table>
 </div>
 </li>
            <li> <span class="li-head">version</span> - GTP version number: 0 or 1. <span class="li-normal">type: int</span>
 <a id='label364' href="javascript:ContentClick('label365', 'label364');" onmouseover="ContentPreview('label365');" onmouseout="ContentUnpreview('label365');" title="click to collapse or expand..."> more... </a>
 <div id="label365" style="display:none">
 <table border="1">
 <tr>
 <td></td>
 <td colspan="3">Supported Version Ranges</td>
 </tr>
 <tr>
 <td>version</td>
 <td><code class="docutils literal notranslate">v6.0.0 -> v7.0.8 </code></td>
 <td><code class="docutils literal notranslate">v7.2.0 -> v7.2.4 </code></td>
 <td><code class="docutils literal notranslate">v7.4.3 -> 7.6.0 </code></td>
 </tr>
 </table>
 </div>
 </li>
            </ul>
        <li> <span class="li-head">policy</span> - Policy. <span class="li-normal">type: list</span> <span style="font-family:'Courier New'" class="li-required">member_path: policy:id</span>
 <a id='label366' href="javascript:ContentClick('label367', 'label366');" onmouseover="ContentPreview('label367');" onmouseout="ContentUnpreview('label367');" title="click to collapse or expand..."> more... </a>
 <div id="label367" style="display:none">
 <table border="1">
 <tr>
 <td></td><td colspan="3">Supported Version Ranges</td>
 </tr>
 <tr>
 <td>policy</td>
 <td><code class="docutils literal notranslate">v6.0.0 -> v7.0.8 </code></td>
 <td><code class="docutils literal notranslate">v7.2.0 -> v7.2.4 </code></td>
 <td><code class="docutils literal notranslate">v7.4.3 -> 7.6.0 </code></td>
 </tr>
 </table>
 </div>
 </li>
            <ul class="ul-self">
            <li> <span class="li-head">action</span> - Action. <span class="li-normal">type: str</span> <span class="li-normal">choices: allow, deny</span>
 <a id='label368' href="javascript:ContentClick('label369', 'label368');" onmouseover="ContentPreview('label369');" onmouseout="ContentUnpreview('label369');" title="click to collapse or expand..."> more... </a>
 <div id="label369" style="display:none">
 <table border="1">
 <tr>
 <td></td>
 <td colspan="3">Supported Version Ranges</td>
 </tr>
 <tr>
 <td>action</td>
 <td><code class="docutils literal notranslate">v6.0.0 -> v7.0.8 </code></td>
 <td><code class="docutils literal notranslate">v7.2.0 -> v7.2.4 </code></td>
 <td><code class="docutils literal notranslate">v7.4.3 -> 7.6.0 </code></td>
 </tr>
 <tr>
 <td>[allow]</td>
 <td><code class="docutils literal notranslate">v6.0.0 -> v7.0.8</code></td>
 <tr>
 <td>[deny]</td>
 <td><code class="docutils literal notranslate">v6.0.0 -> v7.0.8</code></td>
 </table>
 </div>
 </li>
            <li> <span class="li-head">apn_sel_mode</span> - APN selection mode. <span class="li-normal">type: list</span> <span class="li-normal">choices: ms, net, vrf</span>
 <a id='label370' href="javascript:ContentClick('label371', 'label370');" onmouseover="ContentPreview('label371');" onmouseout="ContentUnpreview('label371');" title="click to collapse or expand..."> more... </a>
 <div id="label371" style="display:none">
 <table border="1">
 <tr>
 <td></td>
 <td colspan="3">Supported Version Ranges</td>
 </tr>
 <tr>
 <td>apn_sel_mode</td>
 <td><code class="docutils literal notranslate">v6.0.0 -> v7.0.8 </code></td>
 <td><code class="docutils literal notranslate">v7.2.0 -> v7.2.4 </code></td>
 <td><code class="docutils literal notranslate">v7.4.3 -> 7.6.0 </code></td>
 </tr>
 <tr>
 <td>[ms]</td>
 <td><code class="docutils literal notranslate">v6.0.0 -> v7.0.8</code></td>
 <tr>
 <td>[net]</td>
 <td><code class="docutils literal notranslate">v6.0.0 -> v7.0.8</code></td>
 <tr>
 <td>[vrf]</td>
 <td><code class="docutils literal notranslate">v6.0.0 -> v7.0.8</code></td>
 </table>
 </div>
 </li>
            <li> <span class="li-head">apnmember</span> - APN member. <span class="li-normal">type: list</span> <span style="font-family:'Courier New'" class="li-required">member_path: policy:id/apnmember:name</span>
 <a id='label372' href="javascript:ContentClick('label373', 'label372');" onmouseover="ContentPreview('label373');" onmouseout="ContentUnpreview('label373');" title="click to collapse or expand..."> more... </a>
 <div id="label373" style="display:none">
 <table border="1">
 <tr>
 <td></td><td colspan="3">Supported Version Ranges</td>
 </tr>
 <tr>
 <td>apnmember</td>
 <td><code class="docutils literal notranslate">v6.0.0 -> v7.0.8 </code></td>
 <td><code class="docutils literal notranslate">v7.2.0 -> v7.2.4 </code></td>
 <td><code class="docutils literal notranslate">v7.4.3 -> 7.6.0 </code></td>
 </tr>
 </table>
 </div>
 </li>
                <ul class="ul-self">
                <li> <span class="li-head">name</span> - APN name. Source gtp.apn.name gtp.apngrp.name. <span class="li-normal">type: str</span> <span class="li-required">required: true</span>
 <a id='label374' href="javascript:ContentClick('label375', 'label374');" onmouseover="ContentPreview('label375');" onmouseout="ContentUnpreview('label375');" title="click to collapse or expand..."> more... </a>
 <div id="label375" style="display:none">
 <table border="1">
 <tr>
 <td></td>
 <td colspan="3">Supported Version Ranges</td>
 </tr>
 <tr>
 <td>name</td>
 <td><code class="docutils literal notranslate">v6.0.0 -> v7.0.8 </code></td>
 <td><code class="docutils literal notranslate">v7.2.0 -> v7.2.4 </code></td>
 <td><code class="docutils literal notranslate">v7.4.3 -> 7.6.0 </code></td>
 </tr>
 </table>
 </div>
 </li>
                </ul>
            <li> <span class="li-head">id</span> - ID. see <a href='#notes'>Notes</a>. <span class="li-normal">type: int</span> <span class="li-required">required: true</span>
 <a id='label376' href="javascript:ContentClick('label377', 'label376');" onmouseover="ContentPreview('label377');" onmouseout="ContentUnpreview('label377');" title="click to collapse or expand..."> more... </a>
 <div id="label377" style="display:none">
 <table border="1">
 <tr>
 <td></td>
 <td colspan="3">Supported Version Ranges</td>
 </tr>
 <tr>
 <td>id</td>
 <td><code class="docutils literal notranslate">v6.0.0 -> v7.0.8 </code></td>
 <td><code class="docutils literal notranslate">v7.2.0 -> v7.2.4 </code></td>
 <td><code class="docutils literal notranslate">v7.4.3 -> 7.6.0 </code></td>
 </tr>
 </table>
 </div>
 </li>
            <li> <span class="li-head">imei</span> - IMEI pattern. <span class="li-normal">type: str</span>
 <a id='label378' href="javascript:ContentClick('label379', 'label378');" onmouseover="ContentPreview('label379');" onmouseout="ContentUnpreview('label379');" title="click to collapse or expand..."> more... </a>
 <div id="label379" style="display:none">
 <table border="1">
 <tr>
 <td></td>
 <td colspan="3">Supported Version Ranges</td>
 </tr>
 <tr>
 <td>imei</td>
 <td><code class="docutils literal notranslate">v6.0.0 -> v7.0.8 </code></td>
 <td><code class="docutils literal notranslate">v7.2.0 -> v7.2.4 </code></td>
 <td><code class="docutils literal notranslate">v7.4.3 -> 7.6.0 </code></td>
 </tr>
 </table>
 </div>
 </li>
            <li> <span class="li-head">imsi</span> - IMSI prefix. <span class="li-normal">type: str</span>
 <a id='label380' href="javascript:ContentClick('label381', 'label380');" onmouseover="ContentPreview('label381');" onmouseout="ContentUnpreview('label381');" title="click to collapse or expand..."> more... </a>
 <div id="label381" style="display:none">
 <table border="1">
 <tr>
 <td></td>
 <td colspan="1">Supported Version Ranges</td>
 </tr>
 <tr>
 <td>imsi</td>
 <td><code class="docutils literal notranslate">v6.0.0 -> v6.0.11 </code></td>
 </tr>
 </table>
 </div>
 </li>
            <li> <span class="li-head">imsi_prefix</span> - IMSI prefix. <span class="li-normal">type: str</span>
 <a id='label382' href="javascript:ContentClick('label383', 'label382');" onmouseover="ContentPreview('label383');" onmouseout="ContentUnpreview('label383');" title="click to collapse or expand..."> more... </a>
 <div id="label383" style="display:none">
 <table border="1">
 <tr>
 <td></td>
 <td colspan="3">Supported Version Ranges</td>
 </tr>
 <tr>
 <td>imsi_prefix</td>
 <td><code class="docutils literal notranslate">v6.2.0 -> v7.0.8 </code></td>
 <td><code class="docutils literal notranslate">v7.2.0 -> v7.2.4 </code></td>
 <td><code class="docutils literal notranslate">v7.4.3 -> 7.6.0 </code></td>
 </tr>
 </table>
 </div>
 </li>
            <li> <span class="li-head">max_apn_restriction</span> - Maximum APN restriction value. <span class="li-normal">type: str</span> <span class="li-normal">choices: all, public-1, public-2, private-1, private-2</span>
 <a id='label384' href="javascript:ContentClick('label385', 'label384');" onmouseover="ContentPreview('label385');" onmouseout="ContentUnpreview('label385');" title="click to collapse or expand..."> more... </a>
 <div id="label385" style="display:none">
 <table border="1">
 <tr>
 <td></td>
 <td colspan="3">Supported Version Ranges</td>
 </tr>
 <tr>
 <td>max_apn_restriction</td>
 <td><code class="docutils literal notranslate">v6.0.0 -> v7.0.8 </code></td>
 <td><code class="docutils literal notranslate">v7.2.0 -> v7.2.4 </code></td>
 <td><code class="docutils literal notranslate">v7.4.3 -> 7.6.0 </code></td>
 </tr>
 <tr>
 <td>[all]</td>
 <td><code class="docutils literal notranslate">v6.0.0 -> v7.0.8</code></td>
 <tr>
 <td>[public-1]</td>
 <td><code class="docutils literal notranslate">v6.0.0 -> v7.0.8</code></td>
 <tr>
 <td>[public-2]</td>
 <td><code class="docutils literal notranslate">v6.0.0 -> v7.0.8</code></td>
 <tr>
 <td>[private-1]</td>
 <td><code class="docutils literal notranslate">v6.0.0 -> v7.0.8</code></td>
 <tr>
 <td>[private-2]</td>
 <td><code class="docutils literal notranslate">v6.0.0 -> v7.0.8</code></td>
 </table>
 </div>
 </li>
            <li> <span class="li-head">messages</span> - GTP messages. <span class="li-normal">type: list</span> <span class="li-normal">choices: create-req, create-res, update-req, update-res</span>
 <a id='label386' href="javascript:ContentClick('label387', 'label386');" onmouseover="ContentPreview('label387');" onmouseout="ContentUnpreview('label387');" title="click to collapse or expand..."> more... </a>
 <div id="label387" style="display:none">
 <table border="1">
 <tr>
 <td></td>
 <td colspan="3">Supported Version Ranges</td>
 </tr>
 <tr>
 <td>messages</td>
 <td><code class="docutils literal notranslate">v6.0.0 -> v7.0.8 </code></td>
 <td><code class="docutils literal notranslate">v7.2.0 -> v7.2.4 </code></td>
 <td><code class="docutils literal notranslate">v7.4.3 -> 7.6.0 </code></td>
 </tr>
 <tr>
 <td>[create-req]</td>
 <td><code class="docutils literal notranslate">v6.0.0 -> v7.0.8</code></td>
 <tr>
 <td>[create-res]</td>
 <td><code class="docutils literal notranslate">v6.0.0 -> v7.0.8</code></td>
 <tr>
 <td>[update-req]</td>
 <td><code class="docutils literal notranslate">v6.0.0 -> v7.0.8</code></td>
 <tr>
 <td>[update-res]</td>
 <td><code class="docutils literal notranslate">v6.0.0 -> v7.0.8</code></td>
 </table>
 </div>
 </li>
            <li> <span class="li-head">msisdn</span> - MSISDN prefix. <span class="li-normal">type: str</span>
 <a id='label388' href="javascript:ContentClick('label389', 'label388');" onmouseover="ContentPreview('label389');" onmouseout="ContentUnpreview('label389');" title="click to collapse or expand..."> more... </a>
 <div id="label389" style="display:none">
 <table border="1">
 <tr>
 <td></td>
 <td colspan="1">Supported Version Ranges</td>
 </tr>
 <tr>
 <td>msisdn</td>
 <td><code class="docutils literal notranslate">v6.0.0 -> v6.0.11 </code></td>
 </tr>
 </table>
 </div>
 </li>
            <li> <span class="li-head">msisdn_prefix</span> - MSISDN prefix. <span class="li-normal">type: str</span>
 <a id='label390' href="javascript:ContentClick('label391', 'label390');" onmouseover="ContentPreview('label391');" onmouseout="ContentUnpreview('label391');" title="click to collapse or expand..."> more... </a>
 <div id="label391" style="display:none">
 <table border="1">
 <tr>
 <td></td>
 <td colspan="3">Supported Version Ranges</td>
 </tr>
 <tr>
 <td>msisdn_prefix</td>
 <td><code class="docutils literal notranslate">v6.2.0 -> v7.0.8 </code></td>
 <td><code class="docutils literal notranslate">v7.2.0 -> v7.2.4 </code></td>
 <td><code class="docutils literal notranslate">v7.4.3 -> 7.6.0 </code></td>
 </tr>
 </table>
 </div>
 </li>
            <li> <span class="li-head">rai</span> - RAI pattern. <span class="li-normal">type: str</span>
 <a id='label392' href="javascript:ContentClick('label393', 'label392');" onmouseover="ContentPreview('label393');" onmouseout="ContentUnpreview('label393');" title="click to collapse or expand..."> more... </a>
 <div id="label393" style="display:none">
 <table border="1">
 <tr>
 <td></td>
 <td colspan="3">Supported Version Ranges</td>
 </tr>
 <tr>
 <td>rai</td>
 <td><code class="docutils literal notranslate">v6.0.0 -> v7.0.8 </code></td>
 <td><code class="docutils literal notranslate">v7.2.0 -> v7.2.4 </code></td>
 <td><code class="docutils literal notranslate">v7.4.3 -> 7.6.0 </code></td>
 </tr>
 </table>
 </div>
 </li>
            <li> <span class="li-head">rat_type</span> - RAT Type. <span class="li-normal">type: list</span> <span class="li-normal">choices: any, utran, geran, wlan, gan, hspa, eutran, virtual, nbiot</span>
 <a id='label394' href="javascript:ContentClick('label395', 'label394');" onmouseover="ContentPreview('label395');" onmouseout="ContentUnpreview('label395');" title="click to collapse or expand..."> more... </a>
 <div id="label395" style="display:none">
 <table border="1">
 <tr>
 <td></td>
 <td colspan="3">Supported Version Ranges</td>
 </tr>
 <tr>
 <td>rat_type</td>
 <td><code class="docutils literal notranslate">v6.0.0 -> v7.0.8 </code></td>
 <td><code class="docutils literal notranslate">v7.2.0 -> v7.2.4 </code></td>
 <td><code class="docutils literal notranslate">v7.4.3 -> 7.6.0 </code></td>
 </tr>
 <tr>
 <td>[any]</td>
 <td><code class="docutils literal notranslate">v6.0.0 -> v7.0.8</code></td>
 <tr>
 <td>[utran]</td>
 <td><code class="docutils literal notranslate">v6.0.0 -> v7.0.8</code></td>
 <tr>
 <td>[geran]</td>
 <td><code class="docutils literal notranslate">v6.0.0 -> v7.0.8</code></td>
 <tr>
 <td>[wlan]</td>
 <td><code class="docutils literal notranslate">v6.0.0 -> v7.0.8</code></td>
 <tr>
 <td>[gan]</td>
 <td><code class="docutils literal notranslate">v6.0.0 -> v7.0.8</code></td>
 <tr>
 <td>[hspa]</td>
 <td><code class="docutils literal notranslate">v6.0.0 -> v7.0.8</code></td>
 <tr>
 <td>[eutran]</td>
 <td><code class="docutils literal notranslate">v6.2.0 -> v7.0.8</code></td>
 <td><code class="docutils literal notranslate">v7.2.0 -> v7.2.4</code></td>
 <td><code class="docutils literal notranslate">v7.4.3 -> 7.6.0</code></td>
 </tr>
 <tr>
 <td>[virtual]</td>
 <td><code class="docutils literal notranslate">v6.2.0 -> v7.0.8</code></td>
 <td><code class="docutils literal notranslate">v7.2.0 -> v7.2.4</code></td>
 <td><code class="docutils literal notranslate">v7.4.3 -> 7.6.0</code></td>
 </tr>
 <tr>
 <td>[nbiot]</td>
 <td><code class="docutils literal notranslate">v6.2.0 -> v7.0.8</code></td>
 <td><code class="docutils literal notranslate">v7.2.0 -> v7.2.4</code></td>
 <td><code class="docutils literal notranslate">v7.4.3 -> 7.6.0</code></td>
 </tr>
 </table>
 </div>
 </li>
            <li> <span class="li-head">uli</span> - ULI pattern. <span class="li-normal">type: str</span>
 <a id='label396' href="javascript:ContentClick('label397', 'label396');" onmouseover="ContentPreview('label397');" onmouseout="ContentUnpreview('label397');" title="click to collapse or expand..."> more... </a>
 <div id="label397" style="display:none">
 <table border="1">
 <tr>
 <td></td>
 <td colspan="3">Supported Version Ranges</td>
 </tr>
 <tr>
 <td>uli</td>
 <td><code class="docutils literal notranslate">v6.0.0 -> v7.0.8 </code></td>
 <td><code class="docutils literal notranslate">v7.2.0 -> v7.2.4 </code></td>
 <td><code class="docutils literal notranslate">v7.4.3 -> 7.6.0 </code></td>
 </tr>
 </table>
 </div>
 </li>
            </ul>
        <li> <span class="li-head">policy_filter</span> - Advanced policy filter <span class="li-normal">type: str</span> <span class="li-normal">choices: enable, disable</span>
 <a id='label398' href="javascript:ContentClick('label399', 'label398');" onmouseover="ContentPreview('label399');" onmouseout="ContentUnpreview('label399');" title="click to collapse or expand..."> more... </a>
 <div id="label399" style="display:none">
 <table border="1">
 <tr>
 <td></td>
 <td colspan="3">Supported Version Ranges</td>
 </tr>
 <tr>
 <td>policy_filter</td>
 <td><code class="docutils literal notranslate">v6.0.0 -> v7.0.8 </code></td>
 <td><code class="docutils literal notranslate">v7.2.0 -> v7.2.4 </code></td>
 <td><code class="docutils literal notranslate">v7.4.3 -> 7.6.0 </code></td>
 </tr>
 <tr>
 <td>[enable]</td>
 <td><code class="docutils literal notranslate">v6.0.0 -> v7.0.8</code></td>
 <tr>
 <td>[disable]</td>
 <td><code class="docutils literal notranslate">v6.0.0 -> v7.0.8</code></td>
 </table>
 </div>
 </li>
        <li> <span class="li-head">policy_v2</span> - Apply allow or deny action to each GTPv2-c packet. <span class="li-normal">type: list</span> <span style="font-family:'Courier New'" class="li-required">member_path: policy_v2:id</span>
 <a id='label400' href="javascript:ContentClick('label401', 'label400');" onmouseover="ContentPreview('label401');" onmouseout="ContentUnpreview('label401');" title="click to collapse or expand..."> more... </a>
 <div id="label401" style="display:none">
 <table border="1">
 <tr>
 <td></td><td colspan="3">Supported Version Ranges</td>
 </tr>
 <tr>
 <td>policy_v2</td>
 <td><code class="docutils literal notranslate">v6.2.0 -> v7.0.8 </code></td>
 <td><code class="docutils literal notranslate">v7.2.0 -> v7.2.4 </code></td>
 <td><code class="docutils literal notranslate">v7.4.3 -> 7.6.0 </code></td>
 </tr>
 </table>
 </div>
 </li>
            <ul class="ul-self">
            <li> <span class="li-head">action</span> - Action. <span class="li-normal">type: str</span> <span class="li-normal">choices: allow, deny</span>
 <a id='label402' href="javascript:ContentClick('label403', 'label402');" onmouseover="ContentPreview('label403');" onmouseout="ContentUnpreview('label403');" title="click to collapse or expand..."> more... </a>
 <div id="label403" style="display:none">
 <table border="1">
 <tr>
 <td></td>
 <td colspan="3">Supported Version Ranges</td>
 </tr>
 <tr>
 <td>action</td>
 <td><code class="docutils literal notranslate">v6.2.0 -> v7.0.8 </code></td>
 <td><code class="docutils literal notranslate">v7.2.0 -> v7.2.4 </code></td>
 <td><code class="docutils literal notranslate">v7.4.3 -> 7.6.0 </code></td>
 </tr>
 <tr>
 <td>[allow]</td>
 <td><code class="docutils literal notranslate">v6.2.0 -> v7.0.8</code></td>
 <tr>
 <td>[deny]</td>
 <td><code class="docutils literal notranslate">v6.2.0 -> v7.0.8</code></td>
 </table>
 </div>
 </li>
            <li> <span class="li-head">apn_sel_mode</span> - APN selection mode. <span class="li-normal">type: list</span> <span class="li-normal">choices: ms, net, vrf</span>
 <a id='label404' href="javascript:ContentClick('label405', 'label404');" onmouseover="ContentPreview('label405');" onmouseout="ContentUnpreview('label405');" title="click to collapse or expand..."> more... </a>
 <div id="label405" style="display:none">
 <table border="1">
 <tr>
 <td></td>
 <td colspan="3">Supported Version Ranges</td>
 </tr>
 <tr>
 <td>apn_sel_mode</td>
 <td><code class="docutils literal notranslate">v6.2.0 -> v7.0.8 </code></td>
 <td><code class="docutils literal notranslate">v7.2.0 -> v7.2.4 </code></td>
 <td><code class="docutils literal notranslate">v7.4.3 -> 7.6.0 </code></td>
 </tr>
 <tr>
 <td>[ms]</td>
 <td><code class="docutils literal notranslate">v6.2.0 -> v7.0.8</code></td>
 <tr>
 <td>[net]</td>
 <td><code class="docutils literal notranslate">v6.2.0 -> v7.0.8</code></td>
 <tr>
 <td>[vrf]</td>
 <td><code class="docutils literal notranslate">v6.2.0 -> v7.0.8</code></td>
 </table>
 </div>
 </li>
            <li> <span class="li-head">apnmember</span> - APN member. <span class="li-normal">type: list</span> <span style="font-family:'Courier New'" class="li-required">member_path: policy_v2:id/apnmember:name</span>
 <a id='label406' href="javascript:ContentClick('label407', 'label406');" onmouseover="ContentPreview('label407');" onmouseout="ContentUnpreview('label407');" title="click to collapse or expand..."> more... </a>
 <div id="label407" style="display:none">
 <table border="1">
 <tr>
 <td></td><td colspan="3">Supported Version Ranges</td>
 </tr>
 <tr>
 <td>apnmember</td>
 <td><code class="docutils literal notranslate">v6.2.0 -> v7.0.8 </code></td>
 <td><code class="docutils literal notranslate">v7.2.0 -> v7.2.4 </code></td>
 <td><code class="docutils literal notranslate">v7.4.3 -> 7.6.0 </code></td>
 </tr>
 </table>
 </div>
 </li>
                <ul class="ul-self">
                <li> <span class="li-head">name</span> - APN name. Source gtp.apn.name gtp.apngrp.name. <span class="li-normal">type: str</span> <span class="li-required">required: true</span>
 <a id='label408' href="javascript:ContentClick('label409', 'label408');" onmouseover="ContentPreview('label409');" onmouseout="ContentUnpreview('label409');" title="click to collapse or expand..."> more... </a>
 <div id="label409" style="display:none">
 <table border="1">
 <tr>
 <td></td>
 <td colspan="3">Supported Version Ranges</td>
 </tr>
 <tr>
 <td>name</td>
 <td><code class="docutils literal notranslate">v6.2.0 -> v7.0.8 </code></td>
 <td><code class="docutils literal notranslate">v7.2.0 -> v7.2.4 </code></td>
 <td><code class="docutils literal notranslate">v7.4.3 -> 7.6.0 </code></td>
 </tr>
 </table>
 </div>
 </li>
                </ul>
            <li> <span class="li-head">id</span> - ID. see <a href='#notes'>Notes</a>. <span class="li-normal">type: int</span> <span class="li-required">required: true</span>
 <a id='label410' href="javascript:ContentClick('label411', 'label410');" onmouseover="ContentPreview('label411');" onmouseout="ContentUnpreview('label411');" title="click to collapse or expand..."> more... </a>
 <div id="label411" style="display:none">
 <table border="1">
 <tr>
 <td></td>
 <td colspan="3">Supported Version Ranges</td>
 </tr>
 <tr>
 <td>id</td>
 <td><code class="docutils literal notranslate">v6.2.0 -> v7.0.8 </code></td>
 <td><code class="docutils literal notranslate">v7.2.0 -> v7.2.4 </code></td>
 <td><code class="docutils literal notranslate">v7.4.3 -> 7.6.0 </code></td>
 </tr>
 </table>
 </div>
 </li>
            <li> <span class="li-head">imsi_prefix</span> - IMSI prefix. <span class="li-normal">type: str</span>
 <a id='label412' href="javascript:ContentClick('label413', 'label412');" onmouseover="ContentPreview('label413');" onmouseout="ContentUnpreview('label413');" title="click to collapse or expand..."> more... </a>
 <div id="label413" style="display:none">
 <table border="1">
 <tr>
 <td></td>
 <td colspan="3">Supported Version Ranges</td>
 </tr>
 <tr>
 <td>imsi_prefix</td>
 <td><code class="docutils literal notranslate">v6.2.0 -> v7.0.8 </code></td>
 <td><code class="docutils literal notranslate">v7.2.0 -> v7.2.4 </code></td>
 <td><code class="docutils literal notranslate">v7.4.3 -> 7.6.0 </code></td>
 </tr>
 </table>
 </div>
 </li>
            <li> <span class="li-head">max_apn_restriction</span> - Maximum APN restriction value. <span class="li-normal">type: str</span> <span class="li-normal">choices: all, public-1, public-2, private-1, private-2</span>
 <a id='label414' href="javascript:ContentClick('label415', 'label414');" onmouseover="ContentPreview('label415');" onmouseout="ContentUnpreview('label415');" title="click to collapse or expand..."> more... </a>
 <div id="label415" style="display:none">
 <table border="1">
 <tr>
 <td></td>
 <td colspan="3">Supported Version Ranges</td>
 </tr>
 <tr>
 <td>max_apn_restriction</td>
 <td><code class="docutils literal notranslate">v6.2.0 -> v7.0.8 </code></td>
 <td><code class="docutils literal notranslate">v7.2.0 -> v7.2.4 </code></td>
 <td><code class="docutils literal notranslate">v7.4.3 -> 7.6.0 </code></td>
 </tr>
 <tr>
 <td>[all]</td>
 <td><code class="docutils literal notranslate">v6.2.0 -> v7.0.8</code></td>
 <tr>
 <td>[public-1]</td>
 <td><code class="docutils literal notranslate">v6.2.0 -> v7.0.8</code></td>
 <tr>
 <td>[public-2]</td>
 <td><code class="docutils literal notranslate">v6.2.0 -> v7.0.8</code></td>
 <tr>
 <td>[private-1]</td>
 <td><code class="docutils literal notranslate">v6.2.0 -> v7.0.8</code></td>
 <tr>
 <td>[private-2]</td>
 <td><code class="docutils literal notranslate">v6.2.0 -> v7.0.8</code></td>
 </table>
 </div>
 </li>
            <li> <span class="li-head">mei</span> - MEI pattern. <span class="li-normal">type: str</span>
 <a id='label416' href="javascript:ContentClick('label417', 'label416');" onmouseover="ContentPreview('label417');" onmouseout="ContentUnpreview('label417');" title="click to collapse or expand..."> more... </a>
 <div id="label417" style="display:none">
 <table border="1">
 <tr>
 <td></td>
 <td colspan="3">Supported Version Ranges</td>
 </tr>
 <tr>
 <td>mei</td>
 <td><code class="docutils literal notranslate">v6.2.0 -> v7.0.8 </code></td>
 <td><code class="docutils literal notranslate">v7.2.0 -> v7.2.4 </code></td>
 <td><code class="docutils literal notranslate">v7.4.3 -> 7.6.0 </code></td>
 </tr>
 </table>
 </div>
 </li>
            <li> <span class="li-head">messages</span> - GTP messages. <span class="li-normal">type: list</span> <span class="li-normal">choices: create-ses-req, create-ses-res, modify-bearer-req, modify-bearer-res</span>
 <a id='label418' href="javascript:ContentClick('label419', 'label418');" onmouseover="ContentPreview('label419');" onmouseout="ContentUnpreview('label419');" title="click to collapse or expand..."> more... </a>
 <div id="label419" style="display:none">
 <table border="1">
 <tr>
 <td></td>
 <td colspan="3">Supported Version Ranges</td>
 </tr>
 <tr>
 <td>messages</td>
 <td><code class="docutils literal notranslate">v6.2.0 -> v7.0.8 </code></td>
 <td><code class="docutils literal notranslate">v7.2.0 -> v7.2.4 </code></td>
 <td><code class="docutils literal notranslate">v7.4.3 -> 7.6.0 </code></td>
 </tr>
 <tr>
 <td>[create-ses-req]</td>
 <td><code class="docutils literal notranslate">v6.2.0 -> v7.0.8</code></td>
 <tr>
 <td>[create-ses-res]</td>
 <td><code class="docutils literal notranslate">v6.2.0 -> v7.0.8</code></td>
 <tr>
 <td>[modify-bearer-req]</td>
 <td><code class="docutils literal notranslate">v6.2.0 -> v7.0.8</code></td>
 <tr>
 <td>[modify-bearer-res]</td>
 <td><code class="docutils literal notranslate">v6.2.0 -> v7.0.8</code></td>
 </table>
 </div>
 </li>
            <li> <span class="li-head">msisdn_prefix</span> - MSISDN prefix. <span class="li-normal">type: str</span>
 <a id='label420' href="javascript:ContentClick('label421', 'label420');" onmouseover="ContentPreview('label421');" onmouseout="ContentUnpreview('label421');" title="click to collapse or expand..."> more... </a>
 <div id="label421" style="display:none">
 <table border="1">
 <tr>
 <td></td>
 <td colspan="3">Supported Version Ranges</td>
 </tr>
 <tr>
 <td>msisdn_prefix</td>
 <td><code class="docutils literal notranslate">v6.2.0 -> v7.0.8 </code></td>
 <td><code class="docutils literal notranslate">v7.2.0 -> v7.2.4 </code></td>
 <td><code class="docutils literal notranslate">v7.4.3 -> 7.6.0 </code></td>
 </tr>
 </table>
 </div>
 </li>
            <li> <span class="li-head">rat_type</span> - RAT Type. <span class="li-normal">type: list</span> <span class="li-normal">choices: any, utran, geran, wlan, gan, hspa, eutran, virtual, nbiot, ltem, nr</span>
 <a id='label422' href="javascript:ContentClick('label423', 'label422');" onmouseover="ContentPreview('label423');" onmouseout="ContentUnpreview('label423');" title="click to collapse or expand..."> more... </a>
 <div id="label423" style="display:none">
 <table border="1">
 <tr>
 <td></td>
 <td colspan="3">Supported Version Ranges</td>
 </tr>
 <tr>
 <td>rat_type</td>
 <td><code class="docutils literal notranslate">v6.2.0 -> v7.0.8 </code></td>
 <td><code class="docutils literal notranslate">v7.2.0 -> v7.2.4 </code></td>
 <td><code class="docutils literal notranslate">v7.4.3 -> 7.6.0 </code></td>
 </tr>
 <tr>
 <td>[any]</td>
 <td><code class="docutils literal notranslate">v6.2.0 -> v7.0.8</code></td>
 <tr>
 <td>[utran]</td>
 <td><code class="docutils literal notranslate">v6.2.0 -> v7.0.8</code></td>
 <tr>
 <td>[geran]</td>
 <td><code class="docutils literal notranslate">v6.2.0 -> v7.0.8</code></td>
 <tr>
 <td>[wlan]</td>
 <td><code class="docutils literal notranslate">v6.2.0 -> v7.0.8</code></td>
 <tr>
 <td>[gan]</td>
 <td><code class="docutils literal notranslate">v6.2.0 -> v7.0.8</code></td>
 <tr>
 <td>[hspa]</td>
 <td><code class="docutils literal notranslate">v6.2.0 -> v7.0.8</code></td>
 <tr>
 <td>[eutran]</td>
 <td><code class="docutils literal notranslate">v6.2.0 -> v7.0.8</code></td>
 <tr>
 <td>[virtual]</td>
 <td><code class="docutils literal notranslate">v6.2.0 -> v7.0.8</code></td>
 <tr>
 <td>[nbiot]</td>
 <td><code class="docutils literal notranslate">v6.2.0 -> v7.0.8</code></td>
 <tr>
 <td>[ltem]</td>
 <td><code class="docutils literal notranslate">v6.4.0 -> v6.4.0</code></td>
 <td><code class="docutils literal notranslate">v6.4.4 -> v7.0.8</code></td>
 <td><code class="docutils literal notranslate">v7.2.0 -> v7.2.4</code></td>
 <td><code class="docutils literal notranslate">v7.4.3 -> 7.6.0</code></td>
 </tr>
 <tr>
 <td>[nr]</td>
 <td><code class="docutils literal notranslate">v6.4.0 -> v6.4.0</code></td>
 <td><code class="docutils literal notranslate">v6.4.4 -> v7.0.8</code></td>
 <td><code class="docutils literal notranslate">v7.2.0 -> v7.2.4</code></td>
 <td><code class="docutils literal notranslate">v7.4.3 -> 7.6.0</code></td>
 </tr>
 </table>
 </div>
 </li>
            <li> <span class="li-head">uli</span> - GTPv2 ULI patterns (in order of CGI SAI RAI TAI ECGI LAI). <span class="li-normal">type: list</span> </li>
            </ul>
        <li> <span class="li-head">port_notify</span> - overbilling notify port <span class="li-normal">type: int</span>
 <a id='label424' href="javascript:ContentClick('label425', 'label424');" onmouseover="ContentPreview('label425');" onmouseout="ContentUnpreview('label425');" title="click to collapse or expand..."> more... </a>
 <div id="label425" style="display:none">
 <table border="1">
 <tr>
 <td></td>
 <td colspan="3">Supported Version Ranges</td>
 </tr>
 <tr>
 <td>port_notify</td>
 <td><code class="docutils literal notranslate">v6.0.0 -> v7.0.8 </code></td>
 <td><code class="docutils literal notranslate">v7.2.0 -> v7.2.4 </code></td>
 <td><code class="docutils literal notranslate">v7.4.3 -> 7.6.0 </code></td>
 </tr>
 </table>
 </div>
 </li>
        <li> <span class="li-head">rat_timeout_profile</span> - RAT timeout profile. Source gtp.rat-timeout-profile.name. <span class="li-normal">type: str</span>
 <a id='label426' href="javascript:ContentClick('label427', 'label426');" onmouseover="ContentPreview('label427');" onmouseout="ContentUnpreview('label427');" title="click to collapse or expand..."> more... </a>
 <div id="label427" style="display:none">
 <table border="1">
 <tr>
 <td></td>
 <td colspan="3">Supported Version Ranges</td>
 </tr>
 <tr>
 <td>rat_timeout_profile</td>
 <td><code class="docutils literal notranslate">v7.0.1 -> v7.0.8 </code></td>
 <td><code class="docutils literal notranslate">v7.2.0 -> v7.2.4 </code></td>
 <td><code class="docutils literal notranslate">v7.4.3 -> 7.6.0 </code></td>
 </tr>
 </table>
 </div>
 </li>
        <li> <span class="li-head">rate_limit_mode</span> - GTP rate limit mode. <span class="li-normal">type: str</span> <span class="li-normal">choices: per-profile, per-stream, per-apn</span>
 <a id='label428' href="javascript:ContentClick('label429', 'label428');" onmouseover="ContentPreview('label429');" onmouseout="ContentUnpreview('label429');" title="click to collapse or expand..."> more... </a>
 <div id="label429" style="display:none">
 <table border="1">
 <tr>
 <td></td>
 <td colspan="3">Supported Version Ranges</td>
 </tr>
 <tr>
 <td>rate_limit_mode</td>
 <td><code class="docutils literal notranslate">v6.0.0 -> v7.0.8 </code></td>
 <td><code class="docutils literal notranslate">v7.2.0 -> v7.2.4 </code></td>
 <td><code class="docutils literal notranslate">v7.4.3 -> 7.6.0 </code></td>
 </tr>
 <tr>
 <td>[per-profile]</td>
 <td><code class="docutils literal notranslate">v6.0.0 -> v7.0.8</code></td>
 <tr>
 <td>[per-stream]</td>
 <td><code class="docutils literal notranslate">v6.0.0 -> v7.0.8</code></td>
 <tr>
 <td>[per-apn]</td>
 <td><code class="docutils literal notranslate">v6.0.0 -> v7.0.8</code></td>
 </table>
 </div>
 </li>
        <li> <span class="li-head">rate_limited_log</span> - log rate limited <span class="li-normal">type: str</span> <span class="li-normal">choices: enable, disable</span>
 <a id='label430' href="javascript:ContentClick('label431', 'label430');" onmouseover="ContentPreview('label431');" onmouseout="ContentUnpreview('label431');" title="click to collapse or expand..."> more... </a>
 <div id="label431" style="display:none">
 <table border="1">
 <tr>
 <td></td>
 <td colspan="3">Supported Version Ranges</td>
 </tr>
 <tr>
 <td>rate_limited_log</td>
 <td><code class="docutils literal notranslate">v6.0.0 -> v7.0.8 </code></td>
 <td><code class="docutils literal notranslate">v7.2.0 -> v7.2.4 </code></td>
 <td><code class="docutils literal notranslate">v7.4.3 -> 7.6.0 </code></td>
 </tr>
 <tr>
 <td>[enable]</td>
 <td><code class="docutils literal notranslate">v6.0.0 -> v7.0.8</code></td>
 <tr>
 <td>[disable]</td>
 <td><code class="docutils literal notranslate">v6.0.0 -> v7.0.8</code></td>
 </table>
 </div>
 </li>
        <li> <span class="li-head">rate_sampling_interval</span> - rate sampling interval (1-3600 seconds) <span class="li-normal">type: int</span>
 <a id='label432' href="javascript:ContentClick('label433', 'label432');" onmouseover="ContentPreview('label433');" onmouseout="ContentUnpreview('label433');" title="click to collapse or expand..."> more... </a>
 <div id="label433" style="display:none">
 <table border="1">
 <tr>
 <td></td>
 <td colspan="3">Supported Version Ranges</td>
 </tr>
 <tr>
 <td>rate_sampling_interval</td>
 <td><code class="docutils literal notranslate">v6.0.0 -> v7.0.8 </code></td>
 <td><code class="docutils literal notranslate">v7.2.0 -> v7.2.4 </code></td>
 <td><code class="docutils literal notranslate">v7.4.3 -> 7.6.0 </code></td>
 </tr>
 </table>
 </div>
 </li>
        <li> <span class="li-head">remove_if_echo_expires</span> - remove if echo response expires <span class="li-normal">type: str</span> <span class="li-normal">choices: enable, disable</span>
 <a id='label434' href="javascript:ContentClick('label435', 'label434');" onmouseover="ContentPreview('label435');" onmouseout="ContentUnpreview('label435');" title="click to collapse or expand..."> more... </a>
 <div id="label435" style="display:none">
 <table border="1">
 <tr>
 <td></td>
 <td colspan="3">Supported Version Ranges</td>
 </tr>
 <tr>
 <td>remove_if_echo_expires</td>
 <td><code class="docutils literal notranslate">v6.0.0 -> v7.0.8 </code></td>
 <td><code class="docutils literal notranslate">v7.2.0 -> v7.2.4 </code></td>
 <td><code class="docutils literal notranslate">v7.4.3 -> 7.6.0 </code></td>
 </tr>
 <tr>
 <td>[enable]</td>
 <td><code class="docutils literal notranslate">v6.0.0 -> v7.0.8</code></td>
 <tr>
 <td>[disable]</td>
 <td><code class="docutils literal notranslate">v6.0.0 -> v7.0.8</code></td>
 </table>
 </div>
 </li>
        <li> <span class="li-head">remove_if_recovery_differ</span> - remove upon different Recovery IE <span class="li-normal">type: str</span> <span class="li-normal">choices: enable, disable</span>
 <a id='label436' href="javascript:ContentClick('label437', 'label436');" onmouseover="ContentPreview('label437');" onmouseout="ContentUnpreview('label437');" title="click to collapse or expand..."> more... </a>
 <div id="label437" style="display:none">
 <table border="1">
 <tr>
 <td></td>
 <td colspan="3">Supported Version Ranges</td>
 </tr>
 <tr>
 <td>remove_if_recovery_differ</td>
 <td><code class="docutils literal notranslate">v6.0.0 -> v7.0.8 </code></td>
 <td><code class="docutils literal notranslate">v7.2.0 -> v7.2.4 </code></td>
 <td><code class="docutils literal notranslate">v7.4.3 -> 7.6.0 </code></td>
 </tr>
 <tr>
 <td>[enable]</td>
 <td><code class="docutils literal notranslate">v6.0.0 -> v7.0.8</code></td>
 <tr>
 <td>[disable]</td>
 <td><code class="docutils literal notranslate">v6.0.0 -> v7.0.8</code></td>
 </table>
 </div>
 </li>
        <li> <span class="li-head">reserved_ie</span> - reserved information element <span class="li-normal">type: str</span> <span class="li-normal">choices: allow, deny</span>
 <a id='label438' href="javascript:ContentClick('label439', 'label438');" onmouseover="ContentPreview('label439');" onmouseout="ContentUnpreview('label439');" title="click to collapse or expand..."> more... </a>
 <div id="label439" style="display:none">
 <table border="1">
 <tr>
 <td></td>
 <td colspan="3">Supported Version Ranges</td>
 </tr>
 <tr>
 <td>reserved_ie</td>
 <td><code class="docutils literal notranslate">v6.0.0 -> v7.0.8 </code></td>
 <td><code class="docutils literal notranslate">v7.2.0 -> v7.2.4 </code></td>
 <td><code class="docutils literal notranslate">v7.4.3 -> 7.6.0 </code></td>
 </tr>
 <tr>
 <td>[allow]</td>
 <td><code class="docutils literal notranslate">v6.0.0 -> v7.0.8</code></td>
 <tr>
 <td>[deny]</td>
 <td><code class="docutils literal notranslate">v6.0.0 -> v7.0.8</code></td>
 </table>
 </div>
 </li>
        <li> <span class="li-head">send_delete_when_timeout</span> - send DELETE request to path endpoints when GTPv0/v1 tunnel timeout. <span class="li-normal">type: str</span> <span class="li-normal">choices: enable, disable</span>
 <a id='label440' href="javascript:ContentClick('label441', 'label440');" onmouseover="ContentPreview('label441');" onmouseout="ContentUnpreview('label441');" title="click to collapse or expand..."> more... </a>
 <div id="label441" style="display:none">
 <table border="1">
 <tr>
 <td></td>
 <td colspan="3">Supported Version Ranges</td>
 </tr>
 <tr>
 <td>send_delete_when_timeout</td>
 <td><code class="docutils literal notranslate">v6.0.0 -> v7.0.8 </code></td>
 <td><code class="docutils literal notranslate">v7.2.0 -> v7.2.4 </code></td>
 <td><code class="docutils literal notranslate">v7.4.3 -> 7.6.0 </code></td>
 </tr>
 <tr>
 <td>[enable]</td>
 <td><code class="docutils literal notranslate">v6.0.0 -> v7.0.8</code></td>
 <tr>
 <td>[disable]</td>
 <td><code class="docutils literal notranslate">v6.0.0 -> v7.0.8</code></td>
 </table>
 </div>
 </li>
        <li> <span class="li-head">send_delete_when_timeout_v2</span> - send DELETE request to path endpoints when GTPv2 tunnel timeout. <span class="li-normal">type: str</span> <span class="li-normal">choices: enable, disable</span>
 <a id='label442' href="javascript:ContentClick('label443', 'label442');" onmouseover="ContentPreview('label443');" onmouseout="ContentUnpreview('label443');" title="click to collapse or expand..."> more... </a>
 <div id="label443" style="display:none">
 <table border="1">
 <tr>
 <td></td>
 <td colspan="3">Supported Version Ranges</td>
 </tr>
 <tr>
 <td>send_delete_when_timeout_v2</td>
 <td><code class="docutils literal notranslate">v6.0.0 -> v7.0.8 </code></td>
 <td><code class="docutils literal notranslate">v7.2.0 -> v7.2.4 </code></td>
 <td><code class="docutils literal notranslate">v7.4.3 -> 7.6.0 </code></td>
 </tr>
 <tr>
 <td>[enable]</td>
 <td><code class="docutils literal notranslate">v6.0.0 -> v7.0.8</code></td>
 <tr>
 <td>[disable]</td>
 <td><code class="docutils literal notranslate">v6.0.0 -> v7.0.8</code></td>
 </table>
 </div>
 </li>
        <li> <span class="li-head">spoof_src_addr</span> - Spoofed source address for Mobile Station. <span class="li-normal">type: str</span> <span class="li-normal">choices: allow, deny</span>
 <a id='label444' href="javascript:ContentClick('label445', 'label444');" onmouseover="ContentPreview('label445');" onmouseout="ContentUnpreview('label445');" title="click to collapse or expand..."> more... </a>
 <div id="label445" style="display:none">
 <table border="1">
 <tr>
 <td></td>
 <td colspan="3">Supported Version Ranges</td>
 </tr>
 <tr>
 <td>spoof_src_addr</td>
 <td><code class="docutils literal notranslate">v6.0.0 -> v7.0.8 </code></td>
 <td><code class="docutils literal notranslate">v7.2.0 -> v7.2.4 </code></td>
 <td><code class="docutils literal notranslate">v7.4.3 -> 7.6.0 </code></td>
 </tr>
 <tr>
 <td>[allow]</td>
 <td><code class="docutils literal notranslate">v6.0.0 -> v7.0.8</code></td>
 <tr>
 <td>[deny]</td>
 <td><code class="docutils literal notranslate">v6.0.0 -> v7.0.8</code></td>
 </table>
 </div>
 </li>
        <li> <span class="li-head">state_invalid_log</span> - log state invalid <span class="li-normal">type: str</span> <span class="li-normal">choices: enable, disable</span>
 <a id='label446' href="javascript:ContentClick('label447', 'label446');" onmouseover="ContentPreview('label447');" onmouseout="ContentUnpreview('label447');" title="click to collapse or expand..."> more... </a>
 <div id="label447" style="display:none">
 <table border="1">
 <tr>
 <td></td>
 <td colspan="3">Supported Version Ranges</td>
 </tr>
 <tr>
 <td>state_invalid_log</td>
 <td><code class="docutils literal notranslate">v6.0.0 -> v7.0.8 </code></td>
 <td><code class="docutils literal notranslate">v7.2.0 -> v7.2.4 </code></td>
 <td><code class="docutils literal notranslate">v7.4.3 -> 7.6.0 </code></td>
 </tr>
 <tr>
 <td>[enable]</td>
 <td><code class="docutils literal notranslate">v6.0.0 -> v7.0.8</code></td>
 <tr>
 <td>[disable]</td>
 <td><code class="docutils literal notranslate">v6.0.0 -> v7.0.8</code></td>
 </table>
 </div>
 </li>
        <li> <span class="li-head">sub_second_interval</span> - Sub-second interval (0.1, 0.25, or 0.5 sec). <span class="li-normal">type: str</span> <span class="li-normal">choices: 0.5, 0.25, 0.1</span>
 <a id='label448' href="javascript:ContentClick('label449', 'label448');" onmouseover="ContentPreview('label449');" onmouseout="ContentUnpreview('label449');" title="click to collapse or expand..."> more... </a>
 <div id="label449" style="display:none">
 <table border="1">
 <tr>
 <td></td>
 <td colspan="3">Supported Version Ranges</td>
 </tr>
 <tr>
 <td>sub_second_interval</td>
 <td><code class="docutils literal notranslate">v6.2.0 -> v7.0.8 </code></td>
 <td><code class="docutils literal notranslate">v7.2.0 -> v7.2.4 </code></td>
 <td><code class="docutils literal notranslate">v7.4.3 -> 7.6.0 </code></td>
 </tr>
 <tr>
 <td>[0.5]</td>
 <td><code class="docutils literal notranslate">v6.2.0 -> v7.0.8</code></td>
 <tr>
 <td>[0.25]</td>
 <td><code class="docutils literal notranslate">v6.2.0 -> v7.0.8</code></td>
 <tr>
 <td>[0.1]</td>
 <td><code class="docutils literal notranslate">v6.2.0 -> v7.0.8</code></td>
 </table>
 </div>
 </li>
        <li> <span class="li-head">sub_second_sampling</span> - Enable/disable sub-second sampling. <span class="li-normal">type: str</span> <span class="li-normal">choices: enable, disable</span>
 <a id='label450' href="javascript:ContentClick('label451', 'label450');" onmouseover="ContentPreview('label451');" onmouseout="ContentUnpreview('label451');" title="click to collapse or expand..."> more... </a>
 <div id="label451" style="display:none">
 <table border="1">
 <tr>
 <td></td>
 <td colspan="3">Supported Version Ranges</td>
 </tr>
 <tr>
 <td>sub_second_sampling</td>
 <td><code class="docutils literal notranslate">v6.2.0 -> v7.0.8 </code></td>
 <td><code class="docutils literal notranslate">v7.2.0 -> v7.2.4 </code></td>
 <td><code class="docutils literal notranslate">v7.4.3 -> 7.6.0 </code></td>
 </tr>
 <tr>
 <td>[enable]</td>
 <td><code class="docutils literal notranslate">v6.2.0 -> v7.0.8</code></td>
 <tr>
 <td>[disable]</td>
 <td><code class="docutils literal notranslate">v6.2.0 -> v7.0.8</code></td>
 </table>
 </div>
 </li>
        <li> <span class="li-head">traffic_count_log</span> - log tunnel traffic counter <span class="li-normal">type: str</span> <span class="li-normal">choices: enable, disable</span>
 <a id='label452' href="javascript:ContentClick('label453', 'label452');" onmouseover="ContentPreview('label453');" onmouseout="ContentUnpreview('label453');" title="click to collapse or expand..."> more... </a>
 <div id="label453" style="display:none">
 <table border="1">
 <tr>
 <td></td>
 <td colspan="3">Supported Version Ranges</td>
 </tr>
 <tr>
 <td>traffic_count_log</td>
 <td><code class="docutils literal notranslate">v6.0.0 -> v7.0.8 </code></td>
 <td><code class="docutils literal notranslate">v7.2.0 -> v7.2.4 </code></td>
 <td><code class="docutils literal notranslate">v7.4.3 -> 7.6.0 </code></td>
 </tr>
 <tr>
 <td>[enable]</td>
 <td><code class="docutils literal notranslate">v6.0.0 -> v7.0.8</code></td>
 <tr>
 <td>[disable]</td>
 <td><code class="docutils literal notranslate">v6.0.0 -> v7.0.8</code></td>
 </table>
 </div>
 </li>
        <li> <span class="li-head">tunnel_limit</span> - tunnel limit <span class="li-normal">type: int</span>
 <a id='label454' href="javascript:ContentClick('label455', 'label454');" onmouseover="ContentPreview('label455');" onmouseout="ContentUnpreview('label455');" title="click to collapse or expand..."> more... </a>
 <div id="label455" style="display:none">
 <table border="1">
 <tr>
 <td></td>
 <td colspan="3">Supported Version Ranges</td>
 </tr>
 <tr>
 <td>tunnel_limit</td>
 <td><code class="docutils literal notranslate">v6.0.0 -> v7.0.8 </code></td>
 <td><code class="docutils literal notranslate">v7.2.0 -> v7.2.4 </code></td>
 <td><code class="docutils literal notranslate">v7.4.3 -> 7.6.0 </code></td>
 </tr>
 </table>
 </div>
 </li>
        <li> <span class="li-head">tunnel_limit_log</span> - tunnel limit <span class="li-normal">type: str</span> <span class="li-normal">choices: enable, disable</span>
 <a id='label456' href="javascript:ContentClick('label457', 'label456');" onmouseover="ContentPreview('label457');" onmouseout="ContentUnpreview('label457');" title="click to collapse or expand..."> more... </a>
 <div id="label457" style="display:none">
 <table border="1">
 <tr>
 <td></td>
 <td colspan="3">Supported Version Ranges</td>
 </tr>
 <tr>
 <td>tunnel_limit_log</td>
 <td><code class="docutils literal notranslate">v6.0.0 -> v7.0.8 </code></td>
 <td><code class="docutils literal notranslate">v7.2.0 -> v7.2.4 </code></td>
 <td><code class="docutils literal notranslate">v7.4.3 -> 7.6.0 </code></td>
 </tr>
 <tr>
 <td>[enable]</td>
 <td><code class="docutils literal notranslate">v6.0.0 -> v7.0.8</code></td>
 <tr>
 <td>[disable]</td>
 <td><code class="docutils literal notranslate">v6.0.0 -> v7.0.8</code></td>
 </table>
 </div>
 </li>
        <li> <span class="li-head">tunnel_timeout</span> - Established tunnel timeout (in seconds). <span class="li-normal">type: int</span>
 <a id='label458' href="javascript:ContentClick('label459', 'label458');" onmouseover="ContentPreview('label459');" onmouseout="ContentUnpreview('label459');" title="click to collapse or expand..."> more... </a>
 <div id="label459" style="display:none">
 <table border="1">
 <tr>
 <td></td>
 <td colspan="3">Supported Version Ranges</td>
 </tr>
 <tr>
 <td>tunnel_timeout</td>
 <td><code class="docutils literal notranslate">v6.0.0 -> v7.0.8 </code></td>
 <td><code class="docutils literal notranslate">v7.2.0 -> v7.2.4 </code></td>
 <td><code class="docutils literal notranslate">v7.4.3 -> 7.6.0 </code></td>
 </tr>
 </table>
 </div>
 </li>
        <li> <span class="li-head">unknown_version_action</span> - action for unknown gtp version <span class="li-normal">type: str</span> <span class="li-normal">choices: allow, deny</span>
 <a id='label460' href="javascript:ContentClick('label461', 'label460');" onmouseover="ContentPreview('label461');" onmouseout="ContentUnpreview('label461');" title="click to collapse or expand..."> more... </a>
 <div id="label461" style="display:none">
 <table border="1">
 <tr>
 <td></td>
 <td colspan="3">Supported Version Ranges</td>
 </tr>
 <tr>
 <td>unknown_version_action</td>
 <td><code class="docutils literal notranslate">v6.0.0 -> v7.0.8 </code></td>
 <td><code class="docutils literal notranslate">v7.2.0 -> v7.2.4 </code></td>
 <td><code class="docutils literal notranslate">v7.4.3 -> 7.6.0 </code></td>
 </tr>
 <tr>
 <td>[allow]</td>
 <td><code class="docutils literal notranslate">v6.0.0 -> v7.0.8</code></td>
 <tr>
 <td>[deny]</td>
 <td><code class="docutils literal notranslate">v6.0.0 -> v7.0.8</code></td>
 </table>
 </div>
 </li>
        <li> <span class="li-head">user_plane_message_rate_limit</span> - user plane message rate limit <span class="li-normal">type: int</span>
 <a id='label462' href="javascript:ContentClick('label463', 'label462');" onmouseover="ContentPreview('label463');" onmouseout="ContentUnpreview('label463');" title="click to collapse or expand..."> more... </a>
 <div id="label463" style="display:none">
 <table border="1">
 <tr>
 <td></td>
 <td colspan="3">Supported Version Ranges</td>
 </tr>
 <tr>
 <td>user_plane_message_rate_limit</td>
 <td><code class="docutils literal notranslate">v6.0.0 -> v7.0.8 </code></td>
 <td><code class="docutils literal notranslate">v7.2.0 -> v7.2.4 </code></td>
 <td><code class="docutils literal notranslate">v7.4.3 -> 7.6.0 </code></td>
 </tr>
 </table>
 </div>
 </li>
        <li> <span class="li-head">warning_threshold</span> - Warning threshold for rate limiting (0 - 99 percent). <span class="li-normal">type: int</span>
 <a id='label464' href="javascript:ContentClick('label465', 'label464');" onmouseover="ContentPreview('label465');" onmouseout="ContentUnpreview('label465');" title="click to collapse or expand..."> more... </a>
 <div id="label465" style="display:none">
 <table border="1">
 <tr>
 <td></td>
 <td colspan="3">Supported Version Ranges</td>
 </tr>
 <tr>
 <td>warning_threshold</td>
 <td><code class="docutils literal notranslate">v6.0.0 -> v7.0.8 </code></td>
 <td><code class="docutils literal notranslate">v7.2.0 -> v7.2.4 </code></td>
 <td><code class="docutils literal notranslate">v7.4.3 -> 7.6.0 </code></td>
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

   - The module supports check_mode.



Examples
--------

.. code-block:: yaml+jinja
    
    - name: Configure GTP.
      fortinet.fortios.fortios_firewall_gtp:
          vdom: "{{ vdom }}"
          state: "present"
          access_token: "<your_own_value>"
          firewall_gtp:
              addr_notify: "<your_own_value>"
              apn:
                  -
                      action: "allow"
                      apnmember:
                          -
                              name: "default_name_7 (source gtp.apn.name gtp.apngrp.name)"
                      id: "8"
                      selection_mode: "ms"
              apn_filter: "enable"
              authorized_ggsns: "<your_own_value> (source firewall.address.name firewall.addrgrp.name)"
              authorized_ggsns6: "<your_own_value> (source firewall.address6.name firewall.addrgrp6.name)"
              authorized_sgsns: "<your_own_value> (source firewall.address.name firewall.addrgrp.name)"
              authorized_sgsns6: "<your_own_value> (source firewall.address6.name firewall.addrgrp6.name)"
              comment: "Comment."
              context_id: "696"
              control_plane_message_rate_limit: "0"
              default_apn_action: "allow"
              default_imsi_action: "allow"
              default_ip_action: "allow"
              default_noip_action: "allow"
              default_policy_action: "allow"
              denied_log: "enable"
              echo_request_interval: "0"
              extension_log: "enable"
              forwarded_log: "enable"
              global_tunnel_limit: "<your_own_value> (source gtp.tunnel-limit.name)"
              gtp_in_gtp: "allow"
              gtpu_denied_log: "enable"
              gtpu_forwarded_log: "enable"
              gtpu_log_freq: "0"
              gtpv0: "allow"
              half_close_timeout: "10"
              half_open_timeout: "300"
              handover_group: "<your_own_value> (source firewall.address.name firewall.addrgrp.name)"
              handover_group6: "<your_own_value> (source firewall.address6.name firewall.addrgrp6.name)"
              ie_allow_list_v0v1: "<your_own_value> (source gtp.ie-allow-list.name)"
              ie_allow_list_v2: "<your_own_value> (source gtp.ie-allow-list.name)"
              ie_remove_policy:
                  -
                      id: "40"
                      remove_ies: "apn-restriction"
                      sgsn_addr: "<your_own_value> (source firewall.address.name firewall.addrgrp.name)"
                      sgsn_addr6: "<your_own_value> (source firewall.address6.name firewall.addrgrp6.name)"
              ie_remover: "enable"
              ie_validation:
                  apn_restriction: "enable"
                  charging_gateway_addr: "enable"
                  charging_ID: "enable"
                  end_user_addr: "enable"
                  gsn_addr: "enable"
                  imei: "enable"
                  imsi: "enable"
                  mm_context: "enable"
                  ms_tzone: "enable"
                  ms_validated: "enable"
                  msisdn: "enable"
                  nsapi: "enable"
                  pdp_context: "enable"
                  qos_profile: "enable"
                  rai: "enable"
                  rat_type: "enable"
                  reordering_required: "enable"
                  selection_mode: "enable"
                  uli: "enable"
              ie_white_list_v0v1: "<your_own_value> (source gtp.ie-white-list.name)"
              ie_white_list_v2: "<your_own_value> (source gtp.ie-white-list.name)"
              imsi:
                  -
                      action: "allow"
                      apnmember:
                          -
                              name: "default_name_70 (source gtp.apn.name gtp.apngrp.name)"
                      id: "71"
                      mcc_mnc: "<your_own_value>"
                      msisdn_prefix: "<your_own_value>"
                      selection_mode: "ms"
              imsi_filter: "enable"
              interface_notify: "<your_own_value> (source system.interface.name)"
              invalid_reserved_field: "allow"
              invalid_sgsns_to_log: "<your_own_value> (source firewall.address.name firewall.addrgrp.name)"
              invalid_sgsns6_to_log: "<your_own_value> (source firewall.address6.name firewall.addrgrp6.name)"
              ip_filter: "enable"
              ip_policy:
                  -
                      action: "allow"
                      dstaddr: "<your_own_value> (source firewall.address.name firewall.addrgrp.name)"
                      dstaddr6: "<your_own_value> (source firewall.address6.name firewall.addrgrp6.name)"
                      id: "85"
                      srcaddr: "<your_own_value> (source firewall.address.name firewall.addrgrp.name)"
                      srcaddr6: "<your_own_value> (source firewall.address6.name firewall.addrgrp6.name)"
              log_freq: "0"
              log_gtpu_limit: "0"
              log_imsi_prefix: "<your_own_value>"
              log_msisdn_prefix: "<your_own_value>"
              max_message_length: "1452"
              message_filter_v0v1: "<your_own_value> (source gtp.message-filter-v0v1.name)"
              message_filter_v2: "<your_own_value> (source gtp.message-filter-v2.name)"
              message_rate_limit:
                  create_aa_pdp_request: "0"
                  create_aa_pdp_response: "0"
                  create_mbms_request: "0"
                  create_mbms_response: "0"
                  create_pdp_request: "0"
                  create_pdp_response: "0"
                  delete_aa_pdp_request: "0"
                  delete_aa_pdp_response: "0"
                  delete_mbms_request: "0"
                  delete_mbms_response: "0"
                  delete_pdp_request: "0"
                  delete_pdp_response: "0"
                  echo_reponse: "0"
                  echo_request: "0"
                  echo_response: "0"
                  error_indication: "0"
                  failure_report_request: "0"
                  failure_report_response: "0"
                  fwd_reloc_complete_ack: "0"
                  fwd_relocation_complete: "0"
                  fwd_relocation_request: "0"
                  fwd_relocation_response: "0"
                  fwd_srns_context: "0"
                  fwd_srns_context_ack: "0"
                  g_pdu: "0"
                  identification_request: "0"
                  identification_response: "0"
                  mbms_de_reg_request: "0"
                  mbms_de_reg_response: "0"
                  mbms_notify_rej_request: "0"
                  mbms_notify_rej_response: "0"
                  mbms_notify_request: "0"
                  mbms_notify_response: "0"
                  mbms_reg_request: "0"
                  mbms_reg_response: "0"
                  mbms_ses_start_request: "0"
                  mbms_ses_start_response: "0"
                  mbms_ses_stop_request: "0"
                  mbms_ses_stop_response: "0"
                  note_ms_request: "0"
                  note_ms_response: "0"
                  pdu_notify_rej_request: "0"
                  pdu_notify_rej_response: "0"
                  pdu_notify_request: "0"
                  pdu_notify_response: "0"
                  ran_info: "0"
                  relocation_cancel_request: "0"
                  relocation_cancel_response: "0"
                  send_route_request: "0"
                  send_route_response: "0"
                  sgsn_context_ack: "0"
                  sgsn_context_request: "0"
                  sgsn_context_response: "0"
                  support_ext_hdr_notify: "0"
                  update_mbms_request: "0"
                  update_mbms_response: "0"
                  update_pdp_request: "0"
                  update_pdp_response: "0"
                  version_not_support: "0"
              message_rate_limit_v0:
                  create_pdp_request: "0"
                  delete_pdp_request: "0"
                  echo_request: "0"
              message_rate_limit_v1:
                  create_pdp_request: "0"
                  delete_pdp_request: "0"
                  echo_request: "0"
              message_rate_limit_v2:
                  create_session_request: "0"
                  delete_session_request: "0"
                  echo_request: "0"
              min_message_length: "0"
              miss_must_ie: "allow"
              monitor_mode: "enable"
              name: "default_name_170"
              noip_filter: "enable"
              noip_policy:
                  -
                      action: "allow"
                      end: "0"
                      id: "175"
                      start: "0"
                      type: "etsi"
              out_of_state_ie: "allow"
              out_of_state_message: "allow"
              per_apn_shaper:
                  -
                      apn: "<your_own_value> (source gtp.apn.name)"
                      id: "182"
                      rate_limit: "0"
                      version: "1"
              policy:
                  -
                      action: "allow"
                      apn_sel_mode: "ms"
                      apnmember:
                          -
                              name: "default_name_189 (source gtp.apn.name gtp.apngrp.name)"
                      id: "190"
                      imei: "<your_own_value>"
                      imsi: "<your_own_value>"
                      imsi_prefix: "<your_own_value>"
                      max_apn_restriction: "all"
                      messages: "create-req"
                      msisdn: "<your_own_value>"
                      msisdn_prefix: "<your_own_value>"
                      rai: "<your_own_value>"
                      rat_type: "any"
                      uli: "<your_own_value>"
              policy_filter: "enable"
              policy_v2:
                  -
                      action: "allow"
                      apn_sel_mode: "ms"
                      apnmember:
                          -
                              name: "default_name_206 (source gtp.apn.name gtp.apngrp.name)"
                      id: "207"
                      imsi_prefix: "<your_own_value>"
                      max_apn_restriction: "all"
                      mei: "<your_own_value>"
                      messages: "create-ses-req"
                      msisdn_prefix: "<your_own_value>"
                      rat_type: "any"
                      uli: "<your_own_value>"
              port_notify: "21123"
              rat_timeout_profile: "<your_own_value> (source gtp.rat-timeout-profile.name)"
              rate_limit_mode: "per-profile"
              rate_limited_log: "enable"
              rate_sampling_interval: "1"
              remove_if_echo_expires: "enable"
              remove_if_recovery_differ: "enable"
              reserved_ie: "allow"
              send_delete_when_timeout: "enable"
              send_delete_when_timeout_v2: "enable"
              spoof_src_addr: "allow"
              state_invalid_log: "enable"
              sub_second_interval: "0.5"
              sub_second_sampling: "enable"
              traffic_count_log: "enable"
              tunnel_limit: "0"
              tunnel_limit_log: "enable"
              tunnel_timeout: "86400"
              unknown_version_action: "allow"
              user_plane_message_rate_limit: "0"
              warning_threshold: "0"


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
