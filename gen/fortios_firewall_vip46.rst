:source: fortios_firewall_vip46.py

:orphan:

.. fortios_firewall_vip46:

fortios_firewall_vip46 -- Configure IPv4 to IPv6 virtual IPs in Fortinet's FortiOS and FortiGate.
+++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++

.. versionadded:: 2.0.0

.. contents::
   :local:
   :depth: 1


Synopsis
--------
- This module is able to configure a FortiGate or FortiOS (FOS) device by allowing the user to set and modify firewall feature and vip46 category. Examples include all parameters and values need to be adjusted to datasources before usage. Tested with FOS v6.0.0



Requirements
------------
The below requirements are needed on the host that executes this module.

- ansible>=2.15


Tips
----
Using member operation to add an element to an existing object.

FortiOS Version Compatibility
-----------------------------
Supported Version Ranges: v6.0.0 -> v7.0.0


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
    <li> <span class="li-head">firewall_vip46</span> - Configure IPv4 to IPv6 virtual IPs. <span class="li-normal">type: dict</span>
 <a id='label0' href="javascript:ContentClick('label1', 'label0');" onmouseover="ContentPreview('label1');" onmouseout="ContentUnpreview('label1');" title="click to collapse or expand..."> more... </a>
 <div id="label1" style="display:none">
 <table border="1">
 <tr>
 <td></td><td colspan="1">Supported Version Ranges</td>
 </tr>
 <tr>
 <td>firewall_vip46</td>
 <td><code class="docutils literal notranslate">v6.0.0 -> v7.0.0 </code></td>
 </tr>
 </table>
 </div>
 </li>
        <ul class="ul-self">
        <li> <span class="li-head">arp_reply</span> - Enable ARP reply. <span class="li-normal">type: str</span> <span class="li-normal">choices: disable, enable</span>
 <a id='label2' href="javascript:ContentClick('label3', 'label2');" onmouseover="ContentPreview('label3');" onmouseout="ContentUnpreview('label3');" title="click to collapse or expand..."> more... </a>
 <div id="label3" style="display:none">
 <table border="1">
 <tr>
 <td></td>
 <td colspan="1">Supported Version Ranges</td>
 </tr>
 <tr>
 <td>arp_reply</td>
 <td><code class="docutils literal notranslate">v6.0.0 -> v7.0.0 </code></td>
 </tr>
 <tr>
 <td>[disable]</td>
 <td><code class="docutils literal notranslate">v6.0.0 -> v7.0.0</code></td>
 <tr>
 <td>[enable]</td>
 <td><code class="docutils literal notranslate">v6.0.0 -> v7.0.0</code></td>
 </table>
 </div>
 </li>
        <li> <span class="li-head">color</span> - Color of icon on the GUI. <span class="li-normal">type: int</span>
 <a id='label4' href="javascript:ContentClick('label5', 'label4');" onmouseover="ContentPreview('label5');" onmouseout="ContentUnpreview('label5');" title="click to collapse or expand..."> more... </a>
 <div id="label5" style="display:none">
 <table border="1">
 <tr>
 <td></td>
 <td colspan="1">Supported Version Ranges</td>
 </tr>
 <tr>
 <td>color</td>
 <td><code class="docutils literal notranslate">v6.0.0 -> v7.0.0 </code></td>
 </tr>
 </table>
 </div>
 </li>
        <li> <span class="li-head">comment</span> - Comment. <span class="li-normal">type: str</span>
 <a id='label6' href="javascript:ContentClick('label7', 'label6');" onmouseover="ContentPreview('label7');" onmouseout="ContentUnpreview('label7');" title="click to collapse or expand..."> more... </a>
 <div id="label7" style="display:none">
 <table border="1">
 <tr>
 <td></td>
 <td colspan="1">Supported Version Ranges</td>
 </tr>
 <tr>
 <td>comment</td>
 <td><code class="docutils literal notranslate">v6.0.0 -> v7.0.0 </code></td>
 </tr>
 </table>
 </div>
 </li>
        <li> <span class="li-head">extip</span> - Start-external-IP [-end-external-IP]. <span class="li-normal">type: str</span>
 <a id='label8' href="javascript:ContentClick('label9', 'label8');" onmouseover="ContentPreview('label9');" onmouseout="ContentUnpreview('label9');" title="click to collapse or expand..."> more... </a>
 <div id="label9" style="display:none">
 <table border="1">
 <tr>
 <td></td>
 <td colspan="1">Supported Version Ranges</td>
 </tr>
 <tr>
 <td>extip</td>
 <td><code class="docutils literal notranslate">v6.0.0 -> v7.0.0 </code></td>
 </tr>
 </table>
 </div>
 </li>
        <li> <span class="li-head">extport</span> - External service port. <span class="li-normal">type: str</span>
 <a id='label10' href="javascript:ContentClick('label11', 'label10');" onmouseover="ContentPreview('label11');" onmouseout="ContentUnpreview('label11');" title="click to collapse or expand..."> more... </a>
 <div id="label11" style="display:none">
 <table border="1">
 <tr>
 <td></td>
 <td colspan="1">Supported Version Ranges</td>
 </tr>
 <tr>
 <td>extport</td>
 <td><code class="docutils literal notranslate">v6.0.0 -> v7.0.0 </code></td>
 </tr>
 </table>
 </div>
 </li>
        <li> <span class="li-head">id</span> - Custom defined id. <span class="li-normal">type: int</span>
 <a id='label12' href="javascript:ContentClick('label13', 'label12');" onmouseover="ContentPreview('label13');" onmouseout="ContentUnpreview('label13');" title="click to collapse or expand..."> more... </a>
 <div id="label13" style="display:none">
 <table border="1">
 <tr>
 <td></td>
 <td colspan="1">Supported Version Ranges</td>
 </tr>
 <tr>
 <td>id</td>
 <td><code class="docutils literal notranslate">v6.0.0 -> v7.0.0 </code></td>
 </tr>
 </table>
 </div>
 </li>
        <li> <span class="li-head">ldb_method</span> - Load balance method. <span class="li-normal">type: str</span> <span class="li-normal">choices: static, round-robin, weighted, least-session, least-rtt, first-alive</span>
 <a id='label14' href="javascript:ContentClick('label15', 'label14');" onmouseover="ContentPreview('label15');" onmouseout="ContentUnpreview('label15');" title="click to collapse or expand..."> more... </a>
 <div id="label15" style="display:none">
 <table border="1">
 <tr>
 <td></td>
 <td colspan="1">Supported Version Ranges</td>
 </tr>
 <tr>
 <td>ldb_method</td>
 <td><code class="docutils literal notranslate">v6.0.0 -> v7.0.0 </code></td>
 </tr>
 <tr>
 <td>[static]</td>
 <td><code class="docutils literal notranslate">v6.0.0 -> v7.0.0</code></td>
 <tr>
 <td>[round-robin]</td>
 <td><code class="docutils literal notranslate">v6.0.0 -> v7.0.0</code></td>
 <tr>
 <td>[weighted]</td>
 <td><code class="docutils literal notranslate">v6.0.0 -> v7.0.0</code></td>
 <tr>
 <td>[least-session]</td>
 <td><code class="docutils literal notranslate">v6.0.0 -> v7.0.0</code></td>
 <tr>
 <td>[least-rtt]</td>
 <td><code class="docutils literal notranslate">v6.0.0 -> v7.0.0</code></td>
 <tr>
 <td>[first-alive]</td>
 <td><code class="docutils literal notranslate">v6.0.0 -> v7.0.0</code></td>
 </table>
 </div>
 </li>
        <li> <span class="li-head">mappedip</span> - Start-mapped-IPv6-address [-end mapped-IPv6-address]. <span class="li-normal">type: str</span>
 <a id='label16' href="javascript:ContentClick('label17', 'label16');" onmouseover="ContentPreview('label17');" onmouseout="ContentUnpreview('label17');" title="click to collapse or expand..."> more... </a>
 <div id="label17" style="display:none">
 <table border="1">
 <tr>
 <td></td>
 <td colspan="1">Supported Version Ranges</td>
 </tr>
 <tr>
 <td>mappedip</td>
 <td><code class="docutils literal notranslate">v6.0.0 -> v7.0.0 </code></td>
 </tr>
 </table>
 </div>
 </li>
        <li> <span class="li-head">mappedport</span> - Mapped service port. <span class="li-normal">type: str</span>
 <a id='label18' href="javascript:ContentClick('label19', 'label18');" onmouseover="ContentPreview('label19');" onmouseout="ContentUnpreview('label19');" title="click to collapse or expand..."> more... </a>
 <div id="label19" style="display:none">
 <table border="1">
 <tr>
 <td></td>
 <td colspan="1">Supported Version Ranges</td>
 </tr>
 <tr>
 <td>mappedport</td>
 <td><code class="docutils literal notranslate">v6.0.0 -> v7.0.0 </code></td>
 </tr>
 </table>
 </div>
 </li>
        <li> <span class="li-head">monitor</span> - Health monitors. <span class="li-normal">type: list</span> <span style="font-family:'Courier New'" class="li-required">member_path: monitor:name</span>
 <a id='label20' href="javascript:ContentClick('label21', 'label20');" onmouseover="ContentPreview('label21');" onmouseout="ContentUnpreview('label21');" title="click to collapse or expand..."> more... </a>
 <div id="label21" style="display:none">
 <table border="1">
 <tr>
 <td></td><td colspan="1">Supported Version Ranges</td>
 </tr>
 <tr>
 <td>monitor</td>
 <td><code class="docutils literal notranslate">v6.0.0 -> v7.0.0 </code></td>
 </tr>
 </table>
 </div>
 </li>
            <ul class="ul-self">
            <li> <span class="li-head">name</span> - Health monitor name. Source firewall.ldb-monitor.name. <span class="li-normal">type: str</span> <span class="li-required">required: true</span>
 <a id='label22' href="javascript:ContentClick('label23', 'label22');" onmouseover="ContentPreview('label23');" onmouseout="ContentUnpreview('label23');" title="click to collapse or expand..."> more... </a>
 <div id="label23" style="display:none">
 <table border="1">
 <tr>
 <td></td>
 <td colspan="1">Supported Version Ranges</td>
 </tr>
 <tr>
 <td>name</td>
 <td><code class="docutils literal notranslate">v6.0.0 -> v7.0.0 </code></td>
 </tr>
 </table>
 </div>
 </li>
            </ul>
        <li> <span class="li-head">name</span> - VIP46 name. <span class="li-normal">type: str</span> <span class="li-required">required: true</span>
 <a id='label24' href="javascript:ContentClick('label25', 'label24');" onmouseover="ContentPreview('label25');" onmouseout="ContentUnpreview('label25');" title="click to collapse or expand..."> more... </a>
 <div id="label25" style="display:none">
 <table border="1">
 <tr>
 <td></td>
 <td colspan="1">Supported Version Ranges</td>
 </tr>
 <tr>
 <td>name</td>
 <td><code class="docutils literal notranslate">v6.0.0 -> v7.0.0 </code></td>
 </tr>
 </table>
 </div>
 </li>
        <li> <span class="li-head">portforward</span> - Enable port forwarding. <span class="li-normal">type: str</span> <span class="li-normal">choices: disable, enable</span>
 <a id='label26' href="javascript:ContentClick('label27', 'label26');" onmouseover="ContentPreview('label27');" onmouseout="ContentUnpreview('label27');" title="click to collapse or expand..."> more... </a>
 <div id="label27" style="display:none">
 <table border="1">
 <tr>
 <td></td>
 <td colspan="1">Supported Version Ranges</td>
 </tr>
 <tr>
 <td>portforward</td>
 <td><code class="docutils literal notranslate">v6.0.0 -> v7.0.0 </code></td>
 </tr>
 <tr>
 <td>[disable]</td>
 <td><code class="docutils literal notranslate">v6.0.0 -> v7.0.0</code></td>
 <tr>
 <td>[enable]</td>
 <td><code class="docutils literal notranslate">v6.0.0 -> v7.0.0</code></td>
 </table>
 </div>
 </li>
        <li> <span class="li-head">protocol</span> - Mapped port protocol. <span class="li-normal">type: str</span> <span class="li-normal">choices: tcp, udp</span>
 <a id='label28' href="javascript:ContentClick('label29', 'label28');" onmouseover="ContentPreview('label29');" onmouseout="ContentUnpreview('label29');" title="click to collapse or expand..."> more... </a>
 <div id="label29" style="display:none">
 <table border="1">
 <tr>
 <td></td>
 <td colspan="1">Supported Version Ranges</td>
 </tr>
 <tr>
 <td>protocol</td>
 <td><code class="docutils literal notranslate">v6.0.0 -> v7.0.0 </code></td>
 </tr>
 <tr>
 <td>[tcp]</td>
 <td><code class="docutils literal notranslate">v6.0.0 -> v7.0.0</code></td>
 <tr>
 <td>[udp]</td>
 <td><code class="docutils literal notranslate">v6.0.0 -> v7.0.0</code></td>
 </table>
 </div>
 </li>
        <li> <span class="li-head">realservers</span> - Real servers. <span class="li-normal">type: list</span> <span style="font-family:'Courier New'" class="li-required">member_path: realservers:id</span>
 <a id='label30' href="javascript:ContentClick('label31', 'label30');" onmouseover="ContentPreview('label31');" onmouseout="ContentUnpreview('label31');" title="click to collapse or expand..."> more... </a>
 <div id="label31" style="display:none">
 <table border="1">
 <tr>
 <td></td><td colspan="1">Supported Version Ranges</td>
 </tr>
 <tr>
 <td>realservers</td>
 <td><code class="docutils literal notranslate">v6.0.0 -> v7.0.0 </code></td>
 </tr>
 </table>
 </div>
 </li>
            <ul class="ul-self">
            <li> <span class="li-head">client_ip</span> - Restrict server to a client IP in this range. <span class="li-normal">type: str</span>
 <a id='label32' href="javascript:ContentClick('label33', 'label32');" onmouseover="ContentPreview('label33');" onmouseout="ContentUnpreview('label33');" title="click to collapse or expand..."> more... </a>
 <div id="label33" style="display:none">
 <table border="1">
 <tr>
 <td></td>
 <td colspan="1">Supported Version Ranges</td>
 </tr>
 <tr>
 <td>client_ip</td>
 <td><code class="docutils literal notranslate">v6.0.0 -> v7.0.0 </code></td>
 </tr>
 </table>
 </div>
 </li>
            <li> <span class="li-head">healthcheck</span> - Per server health check. <span class="li-normal">type: str</span> <span class="li-normal">choices: disable, enable, vip</span>
 <a id='label34' href="javascript:ContentClick('label35', 'label34');" onmouseover="ContentPreview('label35');" onmouseout="ContentUnpreview('label35');" title="click to collapse or expand..."> more... </a>
 <div id="label35" style="display:none">
 <table border="1">
 <tr>
 <td></td>
 <td colspan="1">Supported Version Ranges</td>
 </tr>
 <tr>
 <td>healthcheck</td>
 <td><code class="docutils literal notranslate">v6.0.0 -> v7.0.0 </code></td>
 </tr>
 <tr>
 <td>[disable]</td>
 <td><code class="docutils literal notranslate">v6.0.0 -> v7.0.0</code></td>
 <tr>
 <td>[enable]</td>
 <td><code class="docutils literal notranslate">v6.0.0 -> v7.0.0</code></td>
 <tr>
 <td>[vip]</td>
 <td><code class="docutils literal notranslate">v6.0.0 -> v7.0.0</code></td>
 </table>
 </div>
 </li>
            <li> <span class="li-head">holddown_interval</span> - Hold down interval. <span class="li-normal">type: int</span>
 <a id='label36' href="javascript:ContentClick('label37', 'label36');" onmouseover="ContentPreview('label37');" onmouseout="ContentUnpreview('label37');" title="click to collapse or expand..."> more... </a>
 <div id="label37" style="display:none">
 <table border="1">
 <tr>
 <td></td>
 <td colspan="1">Supported Version Ranges</td>
 </tr>
 <tr>
 <td>holddown_interval</td>
 <td><code class="docutils literal notranslate">v6.0.0 -> v7.0.0 </code></td>
 </tr>
 </table>
 </div>
 </li>
            <li> <span class="li-head">id</span> - Real server ID. see <a href='#notes'>Notes</a>. <span class="li-normal">type: int</span> <span class="li-required">required: true</span>
 <a id='label38' href="javascript:ContentClick('label39', 'label38');" onmouseover="ContentPreview('label39');" onmouseout="ContentUnpreview('label39');" title="click to collapse or expand..."> more... </a>
 <div id="label39" style="display:none">
 <table border="1">
 <tr>
 <td></td>
 <td colspan="1">Supported Version Ranges</td>
 </tr>
 <tr>
 <td>id</td>
 <td><code class="docutils literal notranslate">v6.0.0 -> v7.0.0 </code></td>
 </tr>
 </table>
 </div>
 </li>
            <li> <span class="li-head">ip</span> - Mapped server IPv6. <span class="li-normal">type: str</span>
 <a id='label40' href="javascript:ContentClick('label41', 'label40');" onmouseover="ContentPreview('label41');" onmouseout="ContentUnpreview('label41');" title="click to collapse or expand..."> more... </a>
 <div id="label41" style="display:none">
 <table border="1">
 <tr>
 <td></td>
 <td colspan="1">Supported Version Ranges</td>
 </tr>
 <tr>
 <td>ip</td>
 <td><code class="docutils literal notranslate">v6.0.0 -> v7.0.0 </code></td>
 </tr>
 </table>
 </div>
 </li>
            <li> <span class="li-head">max_connections</span> - Maximum number of connections allowed to server. <span class="li-normal">type: int</span>
 <a id='label42' href="javascript:ContentClick('label43', 'label42');" onmouseover="ContentPreview('label43');" onmouseout="ContentUnpreview('label43');" title="click to collapse or expand..."> more... </a>
 <div id="label43" style="display:none">
 <table border="1">
 <tr>
 <td></td>
 <td colspan="1">Supported Version Ranges</td>
 </tr>
 <tr>
 <td>max_connections</td>
 <td><code class="docutils literal notranslate">v6.0.0 -> v7.0.0 </code></td>
 </tr>
 </table>
 </div>
 </li>
            <li> <span class="li-head">monitor</span> - Health monitors. Source firewall.ldb-monitor.name. <span class="li-normal">type: list</span> <span style="font-family:'Courier New'" class="li-required">member_path: realservers:id/monitor:name</span>
 <a id='label44' href="javascript:ContentClick('label45', 'label44');" onmouseover="ContentPreview('label45');" onmouseout="ContentUnpreview('label45');" title="click to collapse or expand..."> more... </a>
 <div id="label45" style="display:none">
 <table border="1">
 <tr>
 <td></td><td colspan="1">Supported Version Ranges</td>
 </tr>
 <tr>
 <td>monitor</td>
 <td><code class="docutils literal notranslate">v6.0.0 -> v7.0.0 </code></td>
 </tr>
 </table>
 </div>
 </li>
                <ul class="ul-self">
                <li> <span class="li-head">name</span> - Health monitor name. Source firewall.ldb-monitor.name. <span class="li-normal">type: str</span> <span class="li-required">required: true</span>
 <a id='label46' href="javascript:ContentClick('label47', 'label46');" onmouseover="ContentPreview('label47');" onmouseout="ContentUnpreview('label47');" title="click to collapse or expand..."> more... </a>
 <div id="label47" style="display:none">
 <table border="1">
 <tr>
 <td></td>
 <td colspan="1">Supported Version Ranges</td>
 </tr>
 <tr>
 <td>name</td>
 <td><code class="docutils literal notranslate">v6.4.4 -> v7.0.0 </code></td>
 </tr>
 </table>
 </div>
 </li>
                </ul>
            <li> <span class="li-head">port</span> - Mapped server port. <span class="li-normal">type: int</span>
 <a id='label48' href="javascript:ContentClick('label49', 'label48');" onmouseover="ContentPreview('label49');" onmouseout="ContentUnpreview('label49');" title="click to collapse or expand..."> more... </a>
 <div id="label49" style="display:none">
 <table border="1">
 <tr>
 <td></td>
 <td colspan="1">Supported Version Ranges</td>
 </tr>
 <tr>
 <td>port</td>
 <td><code class="docutils literal notranslate">v6.0.0 -> v7.0.0 </code></td>
 </tr>
 </table>
 </div>
 </li>
            <li> <span class="li-head">status</span> - Server administrative status. <span class="li-normal">type: str</span> <span class="li-normal">choices: active, standby, disable</span>
 <a id='label50' href="javascript:ContentClick('label51', 'label50');" onmouseover="ContentPreview('label51');" onmouseout="ContentUnpreview('label51');" title="click to collapse or expand..."> more... </a>
 <div id="label51" style="display:none">
 <table border="1">
 <tr>
 <td></td>
 <td colspan="1">Supported Version Ranges</td>
 </tr>
 <tr>
 <td>status</td>
 <td><code class="docutils literal notranslate">v6.0.0 -> v7.0.0 </code></td>
 </tr>
 <tr>
 <td>[active]</td>
 <td><code class="docutils literal notranslate">v6.0.0 -> v7.0.0</code></td>
 <tr>
 <td>[standby]</td>
 <td><code class="docutils literal notranslate">v6.0.0 -> v7.0.0</code></td>
 <tr>
 <td>[disable]</td>
 <td><code class="docutils literal notranslate">v6.0.0 -> v7.0.0</code></td>
 </table>
 </div>
 </li>
            <li> <span class="li-head">weight</span> - weight <span class="li-normal">type: int</span>
 <a id='label52' href="javascript:ContentClick('label53', 'label52');" onmouseover="ContentPreview('label53');" onmouseout="ContentUnpreview('label53');" title="click to collapse or expand..."> more... </a>
 <div id="label53" style="display:none">
 <table border="1">
 <tr>
 <td></td>
 <td colspan="1">Supported Version Ranges</td>
 </tr>
 <tr>
 <td>weight</td>
 <td><code class="docutils literal notranslate">v6.0.0 -> v7.0.0 </code></td>
 </tr>
 </table>
 </div>
 </li>
            </ul>
        <li> <span class="li-head">server_type</span> - Server type. <span class="li-normal">type: str</span> <span class="li-normal">choices: http, tcp, udp, ip</span>
 <a id='label54' href="javascript:ContentClick('label55', 'label54');" onmouseover="ContentPreview('label55');" onmouseout="ContentUnpreview('label55');" title="click to collapse or expand..."> more... </a>
 <div id="label55" style="display:none">
 <table border="1">
 <tr>
 <td></td>
 <td colspan="1">Supported Version Ranges</td>
 </tr>
 <tr>
 <td>server_type</td>
 <td><code class="docutils literal notranslate">v6.0.0 -> v7.0.0 </code></td>
 </tr>
 <tr>
 <td>[http]</td>
 <td><code class="docutils literal notranslate">v6.0.0 -> v7.0.0</code></td>
 <tr>
 <td>[tcp]</td>
 <td><code class="docutils literal notranslate">v6.0.0 -> v7.0.0</code></td>
 <tr>
 <td>[udp]</td>
 <td><code class="docutils literal notranslate">v6.0.0 -> v7.0.0</code></td>
 <tr>
 <td>[ip]</td>
 <td><code class="docutils literal notranslate">v6.0.0 -> v7.0.0</code></td>
 </table>
 </div>
 </li>
        <li> <span class="li-head">src_filter</span> - Source IP filter (x.x.x.x/x). <span class="li-normal">type: list</span> <span style="font-family:'Courier New'" class="li-required">member_path: src_filter:range</span>
 <a id='label56' href="javascript:ContentClick('label57', 'label56');" onmouseover="ContentPreview('label57');" onmouseout="ContentUnpreview('label57');" title="click to collapse or expand..."> more... </a>
 <div id="label57" style="display:none">
 <table border="1">
 <tr>
 <td></td><td colspan="1">Supported Version Ranges</td>
 </tr>
 <tr>
 <td>src_filter</td>
 <td><code class="docutils literal notranslate">v6.0.0 -> v7.0.0 </code></td>
 </tr>
 </table>
 </div>
 </li>
            <ul class="ul-self">
            <li> <span class="li-head">range</span> - Src-filter range. <span class="li-normal">type: str</span> <span class="li-required">required: true</span>
 <a id='label58' href="javascript:ContentClick('label59', 'label58');" onmouseover="ContentPreview('label59');" onmouseout="ContentUnpreview('label59');" title="click to collapse or expand..."> more... </a>
 <div id="label59" style="display:none">
 <table border="1">
 <tr>
 <td></td>
 <td colspan="1">Supported Version Ranges</td>
 </tr>
 <tr>
 <td>range</td>
 <td><code class="docutils literal notranslate">v6.0.0 -> v7.0.0 </code></td>
 </tr>
 </table>
 </div>
 </li>
            </ul>
        <li> <span class="li-head">srcintf_filter</span> - Interfaces to which the VIP46 applies. Separate the names with spaces. <span class="li-normal">type: list</span> <span style="font-family:'Courier New'" class="li-required">member_path: srcintf_filter:interface_name</span>
 <a id='label60' href="javascript:ContentClick('label61', 'label60');" onmouseover="ContentPreview('label61');" onmouseout="ContentUnpreview('label61');" title="click to collapse or expand..."> more... </a>
 <div id="label61" style="display:none">
 <table border="1">
 <tr>
 <td></td><td colspan="2">Supported Version Ranges</td>
 </tr>
 <tr>
 <td>srcintf_filter</td>
 <td><code class="docutils literal notranslate">v6.2.7 -> v6.2.7 </code></td>
 <td><code class="docutils literal notranslate">v6.4.4 -> v6.4.4 </code></td>
 </tr>
 </table>
 </div>
 </li>
            <ul class="ul-self">
            <li> <span class="li-head">interface_name</span> - Interface name. Source system.interface.name. <span class="li-normal">type: str</span> <span class="li-required">required: true</span>
 <a id='label62' href="javascript:ContentClick('label63', 'label62');" onmouseover="ContentPreview('label63');" onmouseout="ContentUnpreview('label63');" title="click to collapse or expand..."> more... </a>
 <div id="label63" style="display:none">
 <table border="1">
 <tr>
 <td></td>
 <td colspan="2">Supported Version Ranges</td>
 </tr>
 <tr>
 <td>interface_name</td>
 <td><code class="docutils literal notranslate">v6.2.7 -> v6.2.7 </code></td>
 <td><code class="docutils literal notranslate">v6.4.4 -> v6.4.4 </code></td>
 </tr>
 </table>
 </div>
 </li>
            </ul>
        <li> <span class="li-head">type</span> - VIP type: static NAT or server load balance. <span class="li-normal">type: str</span> <span class="li-normal">choices: static-nat, server-load-balance</span>
 <a id='label64' href="javascript:ContentClick('label65', 'label64');" onmouseover="ContentPreview('label65');" onmouseout="ContentUnpreview('label65');" title="click to collapse or expand..."> more... </a>
 <div id="label65" style="display:none">
 <table border="1">
 <tr>
 <td></td>
 <td colspan="1">Supported Version Ranges</td>
 </tr>
 <tr>
 <td>type</td>
 <td><code class="docutils literal notranslate">v6.0.0 -> v7.0.0 </code></td>
 </tr>
 <tr>
 <td>[static-nat]</td>
 <td><code class="docutils literal notranslate">v6.0.0 -> v7.0.0</code></td>
 <tr>
 <td>[server-load-balance]</td>
 <td><code class="docutils literal notranslate">v6.0.0 -> v7.0.0</code></td>
 </table>
 </div>
 </li>
        <li> <span class="li-head">uuid</span> - Universally Unique Identifier (UUID; automatically assigned but can be manually reset). <span class="li-normal">type: str</span>
 <a id='label66' href="javascript:ContentClick('label67', 'label66');" onmouseover="ContentPreview('label67');" onmouseout="ContentUnpreview('label67');" title="click to collapse or expand..."> more... </a>
 <div id="label67" style="display:none">
 <table border="1">
 <tr>
 <td></td>
 <td colspan="1">Supported Version Ranges</td>
 </tr>
 <tr>
 <td>uuid</td>
 <td><code class="docutils literal notranslate">v6.0.0 -> v7.0.0 </code></td>
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
    
    - name: Configure IPv4 to IPv6 virtual IPs.
      fortinet.fortios.fortios_firewall_vip46:
          vdom: "{{ vdom }}"
          state: "present"
          access_token: "<your_own_value>"
          firewall_vip46:
              arp_reply: "disable"
              color: "0"
              comment: "Comment."
              extip: "<your_own_value>"
              extport: "<your_own_value>"
              id: "8"
              ldb_method: "static"
              mappedip: "<your_own_value>"
              mappedport: "<your_own_value>"
              monitor:
                  -
                      name: "default_name_13 (source firewall.ldb-monitor.name)"
              name: "default_name_14"
              portforward: "disable"
              protocol: "tcp"
              realservers:
                  -
                      client_ip: "<your_own_value>"
                      healthcheck: "disable"
                      holddown_interval: "300"
                      id: "21"
                      ip: "<your_own_value>"
                      max_connections: "0"
                      monitor:
                          -
                              name: "default_name_25 (source firewall.ldb-monitor.name)"
                      port: "0"
                      status: "active"
                      weight: "1"
              server_type: "http"
              src_filter:
                  -
                      range: "<your_own_value>"
              srcintf_filter:
                  -
                      interface_name: "<your_own_value> (source system.interface.name)"
              type: "static-nat"
              uuid: "<your_own_value>"


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
