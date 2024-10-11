:source: fortios_system_standalone_cluster.py

:orphan:

.. fortios_system_standalone_cluster:

fortios_system_standalone_cluster -- Configure FortiGate Session Life Support Protocol (FGSP) cluster attributes in Fortinet's FortiOS and FortiGate.
+++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++

.. versionadded:: 2.0.0

.. contents::
   :local:
   :depth: 1


Synopsis
--------
- This module is able to configure a FortiGate or FortiOS (FOS) device by allowing the user to set and modify system feature and standalone_cluster category. Examples include all parameters and values need to be adjusted to datasources before usage. Tested with FOS v6.0.0



Requirements
------------
The below requirements are needed on the host that executes this module.

- ansible>=2.15


Tips
----
Using member operation to add an element to an existing object.

FortiOS Version Compatibility
-----------------------------
Supported Version Ranges: v6.4.0 -> v7.6.0


Parameters
----------


.. raw:: html

    <ul>
    <li> <span class="li-head">access_token</span> - Token-based authentication. Generated from GUI of Fortigate. <span class="li-normal">type: str</span> <span class="li-required">required: false</span> </li>
    <li> <span class="li-head">enable_log</span> - Enable/Disable logging for task. <span class="li-normal">type: bool</span> <span class="li-required">required: false</span> <span class="li-normal">default: False</span> </li>
    <li> <span class="li-head">vdom</span> - Virtual domain, among those defined previously. A vdom is a virtual instance of the FortiGate that can be configured and used as a different unit. <span class="li-normal">type: str</span> <span class="li-normal">default: root</span> </li>
    <li> <span class="li-head">member_path</span> - Member attribute path to operate on. <span class="li-normal">type: str</span> </li>
    <li> <span class="li-head">member_state</span> - Add or delete a member under specified attribute path. <span class="li-normal">type: str</span> <span class="li-normal">choices: present, absent</span> </li>
    <li> <span class="li-head">system_standalone_cluster</span> - Configure FortiGate Session Life Support Protocol (FGSP) cluster attributes. <span class="li-normal">type: dict</span>
 <a id='label0' href="javascript:ContentClick('label1', 'label0');" onmouseover="ContentPreview('label1');" onmouseout="ContentUnpreview('label1');" title="click to collapse or expand..."> more... </a>
 <div id="label1" style="display:none">
 <table border="1">
 <tr>
 <td></td><td colspan="1">Supported Version Ranges</td>
 </tr>
 <tr>
 <td>system_standalone_cluster</td>
 <td><code class="docutils literal notranslate">v6.4.0 -> 7.6.0 </code></td>
 </tr>
 </table>
 </div>
 </li>
        <ul class="ul-self">
        <li> <span class="li-head">asymmetric_traffic_control</span> - Asymmetric traffic control mode. <span class="li-normal">type: str</span> <span class="li-normal">choices: cps-preferred, strict-anti-replay</span>
 <a id='label2' href="javascript:ContentClick('label3', 'label2');" onmouseover="ContentPreview('label3');" onmouseout="ContentUnpreview('label3');" title="click to collapse or expand..."> more... </a>
 <div id="label3" style="display:none">
 <table border="1">
 <tr>
 <td></td>
 <td colspan="1">Supported Version Ranges</td>
 </tr>
 <tr>
 <td>asymmetric_traffic_control</td>
 <td><code class="docutils literal notranslate">v7.4.2 -> 7.6.0 </code></td>
 </tr>
 <tr>
 <td>[cps-preferred]</td>
 <td><code class="docutils literal notranslate">v7.4.2 -> 7.6.0</code></td>
 <tr>
 <td>[strict-anti-replay]</td>
 <td><code class="docutils literal notranslate">v7.4.2 -> 7.6.0</code></td>
 </table>
 </div>
 </li>
        <li> <span class="li-head">cluster_peer</span> - Configure FortiGate Session Life Support Protocol (FGSP) session synchronization. <span class="li-normal">type: list</span> <span style="font-family:'Courier New'" class="li-required">member_path: cluster_peer:sync_id</span>
 <a id='label4' href="javascript:ContentClick('label5', 'label4');" onmouseover="ContentPreview('label5');" onmouseout="ContentUnpreview('label5');" title="click to collapse or expand..."> more... </a>
 <div id="label5" style="display:none">
 <table border="1">
 <tr>
 <td></td><td colspan="1">Supported Version Ranges</td>
 </tr>
 <tr>
 <td>cluster_peer</td>
 <td><code class="docutils literal notranslate">v7.2.1 -> 7.6.0 </code></td>
 </tr>
 </table>
 </div>
 </li>
            <ul class="ul-self">
            <li> <span class="li-head">down_intfs_before_sess_sync</span> - List of interfaces to be turned down before session synchronization is complete. <span class="li-normal">type: list</span> <span style="font-family:'Courier New'" class="li-required">member_path: cluster_peer:sync_id/down_intfs_before_sess_sync:name</span>
 <a id='label6' href="javascript:ContentClick('label7', 'label6');" onmouseover="ContentPreview('label7');" onmouseout="ContentUnpreview('label7');" title="click to collapse or expand..."> more... </a>
 <div id="label7" style="display:none">
 <table border="1">
 <tr>
 <td></td><td colspan="1">Supported Version Ranges</td>
 </tr>
 <tr>
 <td>down_intfs_before_sess_sync</td>
 <td><code class="docutils literal notranslate">v7.2.1 -> 7.6.0 </code></td>
 </tr>
 </table>
 </div>
 </li>
                <ul class="ul-self">
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
 <td><code class="docutils literal notranslate">v7.2.1 -> 7.6.0 </code></td>
 </tr>
 </table>
 </div>
 </li>
                </ul>
            <li> <span class="li-head">hb_interval</span> - Heartbeat interval (1 - 20 (100*ms). Increase to reduce false positives. <span class="li-normal">type: int</span>
 <a id='label10' href="javascript:ContentClick('label11', 'label10');" onmouseover="ContentPreview('label11');" onmouseout="ContentUnpreview('label11');" title="click to collapse or expand..."> more... </a>
 <div id="label11" style="display:none">
 <table border="1">
 <tr>
 <td></td>
 <td colspan="1">Supported Version Ranges</td>
 </tr>
 <tr>
 <td>hb_interval</td>
 <td><code class="docutils literal notranslate">v7.2.1 -> 7.6.0 </code></td>
 </tr>
 </table>
 </div>
 </li>
            <li> <span class="li-head">hb_lost_threshold</span> - Lost heartbeat threshold (1 - 60). Increase to reduce false positives. <span class="li-normal">type: int</span>
 <a id='label12' href="javascript:ContentClick('label13', 'label12');" onmouseover="ContentPreview('label13');" onmouseout="ContentUnpreview('label13');" title="click to collapse or expand..."> more... </a>
 <div id="label13" style="display:none">
 <table border="1">
 <tr>
 <td></td>
 <td colspan="1">Supported Version Ranges</td>
 </tr>
 <tr>
 <td>hb_lost_threshold</td>
 <td><code class="docutils literal notranslate">v7.2.1 -> 7.6.0 </code></td>
 </tr>
 </table>
 </div>
 </li>
            <li> <span class="li-head">ipsec_tunnel_sync</span> - Enable/disable IPsec tunnel synchronization. <span class="li-normal">type: str</span> <span class="li-normal">choices: enable, disable</span>
 <a id='label14' href="javascript:ContentClick('label15', 'label14');" onmouseover="ContentPreview('label15');" onmouseout="ContentUnpreview('label15');" title="click to collapse or expand..."> more... </a>
 <div id="label15" style="display:none">
 <table border="1">
 <tr>
 <td></td>
 <td colspan="1">Supported Version Ranges</td>
 </tr>
 <tr>
 <td>ipsec_tunnel_sync</td>
 <td><code class="docutils literal notranslate">v7.2.1 -> 7.6.0 </code></td>
 </tr>
 <tr>
 <td>[enable]</td>
 <td><code class="docutils literal notranslate">v7.2.1 -> 7.6.0</code></td>
 <tr>
 <td>[disable]</td>
 <td><code class="docutils literal notranslate">v7.2.1 -> 7.6.0</code></td>
 </table>
 </div>
 </li>
            <li> <span class="li-head">peerip</span> - IP address of the interface on the peer unit that is used for the session synchronization link. <span class="li-normal">type: str</span>
 <a id='label16' href="javascript:ContentClick('label17', 'label16');" onmouseover="ContentPreview('label17');" onmouseout="ContentUnpreview('label17');" title="click to collapse or expand..."> more... </a>
 <div id="label17" style="display:none">
 <table border="1">
 <tr>
 <td></td>
 <td colspan="1">Supported Version Ranges</td>
 </tr>
 <tr>
 <td>peerip</td>
 <td><code class="docutils literal notranslate">v7.2.1 -> 7.6.0 </code></td>
 </tr>
 </table>
 </div>
 </li>
            <li> <span class="li-head">peervd</span> - VDOM that contains the session synchronization link interface on the peer unit. Usually both peers would have the same peervd. Source system.vdom.name. <span class="li-normal">type: str</span>
 <a id='label18' href="javascript:ContentClick('label19', 'label18');" onmouseover="ContentPreview('label19');" onmouseout="ContentUnpreview('label19');" title="click to collapse or expand..."> more... </a>
 <div id="label19" style="display:none">
 <table border="1">
 <tr>
 <td></td>
 <td colspan="1">Supported Version Ranges</td>
 </tr>
 <tr>
 <td>peervd</td>
 <td><code class="docutils literal notranslate">v7.2.1 -> 7.6.0 </code></td>
 </tr>
 </table>
 </div>
 </li>
            <li> <span class="li-head">secondary_add_ipsec_routes</span> - Enable/disable IKE route announcement on the backup unit. <span class="li-normal">type: str</span> <span class="li-normal">choices: enable, disable</span>
 <a id='label20' href="javascript:ContentClick('label21', 'label20');" onmouseover="ContentPreview('label21');" onmouseout="ContentUnpreview('label21');" title="click to collapse or expand..."> more... </a>
 <div id="label21" style="display:none">
 <table border="1">
 <tr>
 <td></td>
 <td colspan="1">Supported Version Ranges</td>
 </tr>
 <tr>
 <td>secondary_add_ipsec_routes</td>
 <td><code class="docutils literal notranslate">v7.2.1 -> 7.6.0 </code></td>
 </tr>
 <tr>
 <td>[enable]</td>
 <td><code class="docutils literal notranslate">v7.2.1 -> 7.6.0</code></td>
 <tr>
 <td>[disable]</td>
 <td><code class="docutils literal notranslate">v7.2.1 -> 7.6.0</code></td>
 </table>
 </div>
 </li>
            <li> <span class="li-head">session_sync_filter</span> - Add one or more filters if you only want to synchronize some sessions. Use the filter to configure the types of sessions to synchronize. <span class="li-normal">type: dict</span>
 <a id='label22' href="javascript:ContentClick('label23', 'label22');" onmouseover="ContentPreview('label23');" onmouseout="ContentUnpreview('label23');" title="click to collapse or expand..."> more... </a>
 <div id="label23" style="display:none">
 <table border="1">
 <tr>
 <td></td><td colspan="1">Supported Version Ranges</td>
 </tr>
 <tr>
 <td>session_sync_filter</td>
 <td><code class="docutils literal notranslate">v7.2.1 -> 7.6.0 </code></td>
 </tr>
 </table>
 </div>
 </li>
                <ul class="ul-self">
                <li> <span class="li-head">custom_service</span> - Only sessions using these custom services are synchronized. Use source and destination port ranges to define these custom services. <span class="li-normal">type: list</span> <span style="font-family:'Courier New'" class="li-required">member_path: cluster_peer:sync_id/session_sync_filter/custom_service:id</span>
 <a id='label24' href="javascript:ContentClick('label25', 'label24');" onmouseover="ContentPreview('label25');" onmouseout="ContentUnpreview('label25');" title="click to collapse or expand..."> more... </a>
 <div id="label25" style="display:none">
 <table border="1">
 <tr>
 <td></td><td colspan="1">Supported Version Ranges</td>
 </tr>
 <tr>
 <td>custom_service</td>
 <td><code class="docutils literal notranslate">v7.2.1 -> 7.6.0 </code></td>
 </tr>
 </table>
 </div>
 </li>
                    <ul class="ul-self">
                    <li> <span class="li-head">dst_port_range</span> - Custom service destination port range. <span class="li-normal">type: str</span>
 <a id='label26' href="javascript:ContentClick('label27', 'label26');" onmouseover="ContentPreview('label27');" onmouseout="ContentUnpreview('label27');" title="click to collapse or expand..."> more... </a>
 <div id="label27" style="display:none">
 <table border="1">
 <tr>
 <td></td>
 <td colspan="1">Supported Version Ranges</td>
 </tr>
 <tr>
 <td>dst_port_range</td>
 <td><code class="docutils literal notranslate">v7.2.1 -> 7.6.0 </code></td>
 </tr>
 </table>
 </div>
 </li>
                    <li> <span class="li-head">id</span> - Custom service ID. see <a href='#notes'>Notes</a>. <span class="li-normal">type: int</span> <span class="li-required">required: true</span>
 <a id='label28' href="javascript:ContentClick('label29', 'label28');" onmouseover="ContentPreview('label29');" onmouseout="ContentUnpreview('label29');" title="click to collapse or expand..."> more... </a>
 <div id="label29" style="display:none">
 <table border="1">
 <tr>
 <td></td>
 <td colspan="1">Supported Version Ranges</td>
 </tr>
 <tr>
 <td>id</td>
 <td><code class="docutils literal notranslate">v7.2.1 -> 7.6.0 </code></td>
 </tr>
 </table>
 </div>
 </li>
                    <li> <span class="li-head">src_port_range</span> - Custom service source port range. <span class="li-normal">type: str</span>
 <a id='label30' href="javascript:ContentClick('label31', 'label30');" onmouseover="ContentPreview('label31');" onmouseout="ContentUnpreview('label31');" title="click to collapse or expand..."> more... </a>
 <div id="label31" style="display:none">
 <table border="1">
 <tr>
 <td></td>
 <td colspan="1">Supported Version Ranges</td>
 </tr>
 <tr>
 <td>src_port_range</td>
 <td><code class="docutils literal notranslate">v7.2.1 -> 7.6.0 </code></td>
 </tr>
 </table>
 </div>
 </li>
                    </ul>
                <li> <span class="li-head">dstaddr</span> - Only sessions to this IPv4 address are synchronized. <span class="li-normal">type: str</span>
 <a id='label32' href="javascript:ContentClick('label33', 'label32');" onmouseover="ContentPreview('label33');" onmouseout="ContentUnpreview('label33');" title="click to collapse or expand..."> more... </a>
 <div id="label33" style="display:none">
 <table border="1">
 <tr>
 <td></td>
 <td colspan="1">Supported Version Ranges</td>
 </tr>
 <tr>
 <td>dstaddr</td>
 <td><code class="docutils literal notranslate">v7.2.1 -> 7.6.0 </code></td>
 </tr>
 </table>
 </div>
 </li>
                <li> <span class="li-head">dstaddr6</span> - Only sessions to this IPv6 address are synchronized. <span class="li-normal">type: str</span>
 <a id='label34' href="javascript:ContentClick('label35', 'label34');" onmouseover="ContentPreview('label35');" onmouseout="ContentUnpreview('label35');" title="click to collapse or expand..."> more... </a>
 <div id="label35" style="display:none">
 <table border="1">
 <tr>
 <td></td>
 <td colspan="1">Supported Version Ranges</td>
 </tr>
 <tr>
 <td>dstaddr6</td>
 <td><code class="docutils literal notranslate">v7.2.1 -> 7.6.0 </code></td>
 </tr>
 </table>
 </div>
 </li>
                <li> <span class="li-head">dstintf</span> - Only sessions to this interface are synchronized. Source system.interface.name. <span class="li-normal">type: str</span>
 <a id='label36' href="javascript:ContentClick('label37', 'label36');" onmouseover="ContentPreview('label37');" onmouseout="ContentUnpreview('label37');" title="click to collapse or expand..."> more... </a>
 <div id="label37" style="display:none">
 <table border="1">
 <tr>
 <td></td>
 <td colspan="1">Supported Version Ranges</td>
 </tr>
 <tr>
 <td>dstintf</td>
 <td><code class="docutils literal notranslate">v7.2.1 -> 7.6.0 </code></td>
 </tr>
 </table>
 </div>
 </li>
                <li> <span class="li-head">srcaddr</span> - Only sessions from this IPv4 address are synchronized. <span class="li-normal">type: str</span>
 <a id='label38' href="javascript:ContentClick('label39', 'label38');" onmouseover="ContentPreview('label39');" onmouseout="ContentUnpreview('label39');" title="click to collapse or expand..."> more... </a>
 <div id="label39" style="display:none">
 <table border="1">
 <tr>
 <td></td>
 <td colspan="1">Supported Version Ranges</td>
 </tr>
 <tr>
 <td>srcaddr</td>
 <td><code class="docutils literal notranslate">v7.2.1 -> 7.6.0 </code></td>
 </tr>
 </table>
 </div>
 </li>
                <li> <span class="li-head">srcaddr6</span> - Only sessions from this IPv6 address are synchronized. <span class="li-normal">type: str</span>
 <a id='label40' href="javascript:ContentClick('label41', 'label40');" onmouseover="ContentPreview('label41');" onmouseout="ContentUnpreview('label41');" title="click to collapse or expand..."> more... </a>
 <div id="label41" style="display:none">
 <table border="1">
 <tr>
 <td></td>
 <td colspan="1">Supported Version Ranges</td>
 </tr>
 <tr>
 <td>srcaddr6</td>
 <td><code class="docutils literal notranslate">v7.2.1 -> 7.6.0 </code></td>
 </tr>
 </table>
 </div>
 </li>
                <li> <span class="li-head">srcintf</span> - Only sessions from this interface are synchronized. Source system.interface.name. <span class="li-normal">type: str</span>
 <a id='label42' href="javascript:ContentClick('label43', 'label42');" onmouseover="ContentPreview('label43');" onmouseout="ContentUnpreview('label43');" title="click to collapse or expand..."> more... </a>
 <div id="label43" style="display:none">
 <table border="1">
 <tr>
 <td></td>
 <td colspan="1">Supported Version Ranges</td>
 </tr>
 <tr>
 <td>srcintf</td>
 <td><code class="docutils literal notranslate">v7.2.1 -> 7.6.0 </code></td>
 </tr>
 </table>
 </div>
 </li>
                </ul>
            <li> <span class="li-head">sync_id</span> - Sync ID. see <a href='#notes'>Notes</a>. <span class="li-normal">type: int</span> <span class="li-required">required: true</span>
 <a id='label44' href="javascript:ContentClick('label45', 'label44');" onmouseover="ContentPreview('label45');" onmouseout="ContentUnpreview('label45');" title="click to collapse or expand..."> more... </a>
 <div id="label45" style="display:none">
 <table border="1">
 <tr>
 <td></td>
 <td colspan="1">Supported Version Ranges</td>
 </tr>
 <tr>
 <td>sync_id</td>
 <td><code class="docutils literal notranslate">v7.2.1 -> 7.6.0 </code></td>
 </tr>
 </table>
 </div>
 </li>
            <li> <span class="li-head">syncvd</span> - Sessions from these VDOMs are synchronized using this session synchronization configuration. <span class="li-normal">type: list</span> <span style="font-family:'Courier New'" class="li-required">member_path: cluster_peer:sync_id/syncvd:name</span>
 <a id='label46' href="javascript:ContentClick('label47', 'label46');" onmouseover="ContentPreview('label47');" onmouseout="ContentUnpreview('label47');" title="click to collapse or expand..."> more... </a>
 <div id="label47" style="display:none">
 <table border="1">
 <tr>
 <td></td><td colspan="1">Supported Version Ranges</td>
 </tr>
 <tr>
 <td>syncvd</td>
 <td><code class="docutils literal notranslate">v7.2.1 -> 7.6.0 </code></td>
 </tr>
 </table>
 </div>
 </li>
                <ul class="ul-self">
                <li> <span class="li-head">name</span> - VDOM name. Source system.vdom.name. <span class="li-normal">type: str</span> <span class="li-required">required: true</span>
 <a id='label48' href="javascript:ContentClick('label49', 'label48');" onmouseover="ContentPreview('label49');" onmouseout="ContentUnpreview('label49');" title="click to collapse or expand..."> more... </a>
 <div id="label49" style="display:none">
 <table border="1">
 <tr>
 <td></td>
 <td colspan="1">Supported Version Ranges</td>
 </tr>
 <tr>
 <td>name</td>
 <td><code class="docutils literal notranslate">v7.2.1 -> 7.6.0 </code></td>
 </tr>
 </table>
 </div>
 </li>
                </ul>
            </ul>
        <li> <span class="li-head">encryption</span> - Enable/disable encryption when synchronizing sessions. <span class="li-normal">type: str</span> <span class="li-normal">choices: enable, disable</span>
 <a id='label50' href="javascript:ContentClick('label51', 'label50');" onmouseover="ContentPreview('label51');" onmouseout="ContentUnpreview('label51');" title="click to collapse or expand..."> more... </a>
 <div id="label51" style="display:none">
 <table border="1">
 <tr>
 <td></td>
 <td colspan="1">Supported Version Ranges</td>
 </tr>
 <tr>
 <td>encryption</td>
 <td><code class="docutils literal notranslate">v6.4.0 -> 7.6.0 </code></td>
 </tr>
 <tr>
 <td>[enable]</td>
 <td><code class="docutils literal notranslate">v6.4.0 -> 7.6.0</code></td>
 <tr>
 <td>[disable]</td>
 <td><code class="docutils literal notranslate">v6.4.0 -> 7.6.0</code></td>
 </table>
 </div>
 </li>
        <li> <span class="li-head">group_member_id</span> - Cluster member ID (0 - 15). <span class="li-normal">type: int</span>
 <a id='label52' href="javascript:ContentClick('label53', 'label52');" onmouseover="ContentPreview('label53');" onmouseout="ContentUnpreview('label53');" title="click to collapse or expand..."> more... </a>
 <div id="label53" style="display:none">
 <table border="1">
 <tr>
 <td></td>
 <td colspan="1">Supported Version Ranges</td>
 </tr>
 <tr>
 <td>group_member_id</td>
 <td><code class="docutils literal notranslate">v6.4.0 -> 7.6.0 </code></td>
 </tr>
 </table>
 </div>
 </li>
        <li> <span class="li-head">layer2_connection</span> - Indicate whether layer 2 connections are present among FGSP members. <span class="li-normal">type: str</span> <span class="li-normal">choices: available, unavailable</span>
 <a id='label54' href="javascript:ContentClick('label55', 'label54');" onmouseover="ContentPreview('label55');" onmouseout="ContentUnpreview('label55');" title="click to collapse or expand..."> more... </a>
 <div id="label55" style="display:none">
 <table border="1">
 <tr>
 <td></td>
 <td colspan="1">Supported Version Ranges</td>
 </tr>
 <tr>
 <td>layer2_connection</td>
 <td><code class="docutils literal notranslate">v6.4.0 -> 7.6.0 </code></td>
 </tr>
 <tr>
 <td>[available]</td>
 <td><code class="docutils literal notranslate">v6.4.0 -> 7.6.0</code></td>
 <tr>
 <td>[unavailable]</td>
 <td><code class="docutils literal notranslate">v6.4.0 -> 7.6.0</code></td>
 </table>
 </div>
 </li>
        <li> <span class="li-head">monitor_interface</span> - Configure a list of interfaces on which to monitor itself. Monitoring is performed on the status of the interface. <span class="li-normal">type: list</span> <span style="font-family:'Courier New'" class="li-required">member_path: monitor_interface:name</span>
 <a id='label56' href="javascript:ContentClick('label57', 'label56');" onmouseover="ContentPreview('label57');" onmouseout="ContentUnpreview('label57');" title="click to collapse or expand..."> more... </a>
 <div id="label57" style="display:none">
 <table border="1">
 <tr>
 <td></td><td colspan="1">Supported Version Ranges</td>
 </tr>
 <tr>
 <td>monitor_interface</td>
 <td><code class="docutils literal notranslate">v7.6.0 -> 7.6.0 </code></td>
 </tr>
 </table>
 </div>
 </li>
            <ul class="ul-self">
            <li> <span class="li-head">name</span> - Interface name. Source system.interface.name. <span class="li-normal">type: str</span> <span class="li-required">required: true</span>
 <a id='label58' href="javascript:ContentClick('label59', 'label58');" onmouseover="ContentPreview('label59');" onmouseout="ContentUnpreview('label59');" title="click to collapse or expand..."> more... </a>
 <div id="label59" style="display:none">
 <table border="1">
 <tr>
 <td></td>
 <td colspan="1">Supported Version Ranges</td>
 </tr>
 <tr>
 <td>name</td>
 <td><code class="docutils literal notranslate">v7.6.0 -> 7.6.0 </code></td>
 </tr>
 </table>
 </div>
 </li>
            </ul>
        <li> <span class="li-head">pingsvr_monitor_interface</span> - List of pingsvr monitor interface to check for remote IP monitoring. <span class="li-normal">type: list</span> <span style="font-family:'Courier New'" class="li-required">member_path: pingsvr_monitor_interface:name</span>
 <a id='label60' href="javascript:ContentClick('label61', 'label60');" onmouseover="ContentPreview('label61');" onmouseout="ContentUnpreview('label61');" title="click to collapse or expand..."> more... </a>
 <div id="label61" style="display:none">
 <table border="1">
 <tr>
 <td></td><td colspan="1">Supported Version Ranges</td>
 </tr>
 <tr>
 <td>pingsvr_monitor_interface</td>
 <td><code class="docutils literal notranslate">v7.6.0 -> 7.6.0 </code></td>
 </tr>
 </table>
 </div>
 </li>
            <ul class="ul-self">
            <li> <span class="li-head">name</span> - Interface name. Source system.interface.name. <span class="li-normal">type: str</span> <span class="li-required">required: true</span>
 <a id='label62' href="javascript:ContentClick('label63', 'label62');" onmouseover="ContentPreview('label63');" onmouseout="ContentUnpreview('label63');" title="click to collapse or expand..."> more... </a>
 <div id="label63" style="display:none">
 <table border="1">
 <tr>
 <td></td>
 <td colspan="1">Supported Version Ranges</td>
 </tr>
 <tr>
 <td>name</td>
 <td><code class="docutils literal notranslate">v7.6.0 -> 7.6.0 </code></td>
 </tr>
 </table>
 </div>
 </li>
            </ul>
        <li> <span class="li-head">psksecret</span> - Pre-shared secret for session synchronization (ASCII string or hexadecimal encoded with a leading 0x). <span class="li-normal">type: str</span>
 <a id='label64' href="javascript:ContentClick('label65', 'label64');" onmouseover="ContentPreview('label65');" onmouseout="ContentUnpreview('label65');" title="click to collapse or expand..."> more... </a>
 <div id="label65" style="display:none">
 <table border="1">
 <tr>
 <td></td>
 <td colspan="1">Supported Version Ranges</td>
 </tr>
 <tr>
 <td>psksecret</td>
 <td><code class="docutils literal notranslate">v6.4.0 -> 7.6.0 </code></td>
 </tr>
 </table>
 </div>
 </li>
        <li> <span class="li-head">session_sync_dev</span> - Offload session-sync process to kernel and sync sessions using connected interface(s) directly. Source system.interface.name. <span class="li-normal">type: list</span> </li>
        <li> <span class="li-head">standalone_group_id</span> - Cluster group ID (0 - 255). Must be the same for all members. <span class="li-normal">type: int</span>
 <a id='label66' href="javascript:ContentClick('label67', 'label66');" onmouseover="ContentPreview('label67');" onmouseout="ContentUnpreview('label67');" title="click to collapse or expand..."> more... </a>
 <div id="label67" style="display:none">
 <table border="1">
 <tr>
 <td></td>
 <td colspan="1">Supported Version Ranges</td>
 </tr>
 <tr>
 <td>standalone_group_id</td>
 <td><code class="docutils literal notranslate">v6.4.0 -> 7.6.0 </code></td>
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
    
    - name: Configure FortiGate Session Life Support Protocol (FGSP) cluster attributes.
      fortinet.fortios.fortios_system_standalone_cluster:
          vdom: "{{ vdom }}"
          system_standalone_cluster:
              asymmetric_traffic_control: "cps-preferred"
              cluster_peer:
                  -
                      down_intfs_before_sess_sync:
                          -
                              name: "default_name_6 (source system.interface.name)"
                      hb_interval: "2"
                      hb_lost_threshold: "10"
                      ipsec_tunnel_sync: "enable"
                      peerip: "<your_own_value>"
                      peervd: "<your_own_value> (source system.vdom.name)"
                      secondary_add_ipsec_routes: "enable"
                      session_sync_filter:
                          custom_service:
                              -
                                  dst_port_range: "<your_own_value>"
                                  id: "16"
                                  src_port_range: "<your_own_value>"
                          dstaddr: "<your_own_value>"
                          dstaddr6: "<your_own_value>"
                          dstintf: "<your_own_value> (source system.interface.name)"
                          srcaddr: "<your_own_value>"
                          srcaddr6: "<your_own_value>"
                          srcintf: "<your_own_value> (source system.interface.name)"
                      sync_id: "<you_own_value>"
                      syncvd:
                          -
                              name: "default_name_26 (source system.vdom.name)"
              encryption: "enable"
              group_member_id: "0"
              layer2_connection: "available"
              monitor_interface:
                  -
                      name: "default_name_31 (source system.interface.name)"
              pingsvr_monitor_interface:
                  -
                      name: "default_name_33 (source system.interface.name)"
              psksecret: "<your_own_value>"
              session_sync_dev: "<your_own_value> (source system.interface.name)"
              standalone_group_id: "0"


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
