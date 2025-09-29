:source: fortios_gtp_message_filter_v2.py

:orphan:

.. fortios_gtp_message_filter_v2:

fortios_gtp_message_filter_v2 -- Message filter for GTPv2 messages in Fortinet's FortiOS and FortiGate.
+++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++

.. versionadded:: 2.0.0

.. contents::
   :local:
   :depth: 1


Synopsis
--------
- This module is able to configure a FortiGate or FortiOS (FOS) device by allowing the user to set and modify gtp feature and message_filter_v2 category. Examples include all parameters and values need to be adjusted to datasources before usage. Tested with FOS v6.0.0



Requirements
------------
The below requirements are needed on the host that executes this module.

- ansible>=2.15


Tips
----
Using member operation to add an element to an existing object.

FortiOS Version Compatibility
-----------------------------
Supported Version Ranges: v6.0.0 -> v7.0.8, v7.2.0 -> v7.2.4, v7.4.3 -> v7.6.4


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
    <li> <span class="li-head">gtp_message_filter_v2</span> - Message filter for GTPv2 messages. <span class="li-normal">type: dict</span>
 <a id='label0' href="javascript:ContentClick('label1', 'label0');" onmouseover="ContentPreview('label1');" onmouseout="ContentUnpreview('label1');" title="click to collapse or expand..."> more... </a>
 <div id="label1" style="display:none">
 <table border="1">
 <tr>
 <td></td><td colspan="3">Supported Version Ranges</td>
 </tr>
 <tr>
 <td>gtp_message_filter_v2</td>
 <td><code class="docutils literal notranslate">v6.0.0 -> v7.0.8 </code></td>
 <td><code class="docutils literal notranslate">v7.2.0 -> v7.2.4 </code></td>
 <td><code class="docutils literal notranslate">v7.4.3 -> 7.6.4 </code></td>
 </tr>
 </table>
 </div>
 </li>
        <ul class="ul-self">
        <li> <span class="li-head">alert_mme_notif_ack</span> - Alert MME notification/acknowledge (notif 153, ack 154). <span class="li-normal">type: str</span> <span class="li-normal">choices: allow, deny</span>
 <a id='label2' href="javascript:ContentClick('label3', 'label2');" onmouseover="ContentPreview('label3');" onmouseout="ContentUnpreview('label3');" title="click to collapse or expand..."> more... </a>
 <div id="label3" style="display:none">
 <table border="1">
 <tr>
 <td></td>
 <td colspan="2">Supported Version Ranges</td>
 </tr>
 <tr>
 <td>alert_mme_notif_ack</td>
 <td><code class="docutils literal notranslate">v7.2.1 -> v7.2.4 </code></td>
 <td><code class="docutils literal notranslate">v7.4.3 -> 7.6.4 </code></td>
 </tr>
 <tr>
 <td>[allow]</td>
 <td><code class="docutils literal notranslate">v7.2.1 -> v7.2.4</code></td>
 <tr>
 <td>[deny]</td>
 <td><code class="docutils literal notranslate">v7.2.1 -> v7.2.4</code></td>
 </table>
 </div>
 </li>
        <li> <span class="li-head">bearer_resource_cmd_fail</span> - Bearer resource (command 68, failure indication 69). <span class="li-normal">type: str</span> <span class="li-normal">choices: allow, deny</span>
 <a id='label4' href="javascript:ContentClick('label5', 'label4');" onmouseover="ContentPreview('label5');" onmouseout="ContentUnpreview('label5');" title="click to collapse or expand..."> more... </a>
 <div id="label5" style="display:none">
 <table border="1">
 <tr>
 <td></td>
 <td colspan="3">Supported Version Ranges</td>
 </tr>
 <tr>
 <td>bearer_resource_cmd_fail</td>
 <td><code class="docutils literal notranslate">v6.0.0 -> v7.0.8 </code></td>
 <td><code class="docutils literal notranslate">v7.2.0 -> v7.2.4 </code></td>
 <td><code class="docutils literal notranslate">v7.4.3 -> 7.6.4 </code></td>
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
        <li> <span class="li-head">change_notification</span> - Change notification (req 38, resp 39). <span class="li-normal">type: str</span> <span class="li-normal">choices: allow, deny</span>
 <a id='label6' href="javascript:ContentClick('label7', 'label6');" onmouseover="ContentPreview('label7');" onmouseout="ContentUnpreview('label7');" title="click to collapse or expand..."> more... </a>
 <div id="label7" style="display:none">
 <table border="1">
 <tr>
 <td></td>
 <td colspan="3">Supported Version Ranges</td>
 </tr>
 <tr>
 <td>change_notification</td>
 <td><code class="docutils literal notranslate">v6.0.0 -> v7.0.8 </code></td>
 <td><code class="docutils literal notranslate">v7.2.0 -> v7.2.4 </code></td>
 <td><code class="docutils literal notranslate">v7.4.3 -> 7.6.4 </code></td>
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
        <li> <span class="li-head">configuration_transfer_tunnel</span> - Configuration transfer tunnel (141). <span class="li-normal">type: str</span> <span class="li-normal">choices: allow, deny</span>
 <a id='label8' href="javascript:ContentClick('label9', 'label8');" onmouseover="ContentPreview('label9');" onmouseout="ContentUnpreview('label9');" title="click to collapse or expand..."> more... </a>
 <div id="label9" style="display:none">
 <table border="1">
 <tr>
 <td></td>
 <td colspan="2">Supported Version Ranges</td>
 </tr>
 <tr>
 <td>configuration_transfer_tunnel</td>
 <td><code class="docutils literal notranslate">v7.2.1 -> v7.2.4 </code></td>
 <td><code class="docutils literal notranslate">v7.4.3 -> 7.6.4 </code></td>
 </tr>
 <tr>
 <td>[allow]</td>
 <td><code class="docutils literal notranslate">v7.2.1 -> v7.2.4</code></td>
 <tr>
 <td>[deny]</td>
 <td><code class="docutils literal notranslate">v7.2.1 -> v7.2.4</code></td>
 </table>
 </div>
 </li>
        <li> <span class="li-head">context_req_res_ack</span> - Context request/response/acknowledge (req 130, resp 131, ack 132). <span class="li-normal">type: str</span> <span class="li-normal">choices: allow, deny</span>
 <a id='label10' href="javascript:ContentClick('label11', 'label10');" onmouseover="ContentPreview('label11');" onmouseout="ContentUnpreview('label11');" title="click to collapse or expand..."> more... </a>
 <div id="label11" style="display:none">
 <table border="1">
 <tr>
 <td></td>
 <td colspan="3">Supported Version Ranges</td>
 </tr>
 <tr>
 <td>context_req_res_ack</td>
 <td><code class="docutils literal notranslate">v7.0.2 -> v7.0.8 </code></td>
 <td><code class="docutils literal notranslate">v7.2.0 -> v7.2.4 </code></td>
 <td><code class="docutils literal notranslate">v7.4.3 -> 7.6.4 </code></td>
 </tr>
 <tr>
 <td>[allow]</td>
 <td><code class="docutils literal notranslate">v7.0.2 -> v7.0.8</code></td>
 <tr>
 <td>[deny]</td>
 <td><code class="docutils literal notranslate">v7.0.2 -> v7.0.8</code></td>
 </table>
 </div>
 </li>
        <li> <span class="li-head">create_bearer</span> - Create bearer (req 95, resp 96). <span class="li-normal">type: str</span> <span class="li-normal">choices: allow, deny</span>
 <a id='label12' href="javascript:ContentClick('label13', 'label12');" onmouseover="ContentPreview('label13');" onmouseout="ContentUnpreview('label13');" title="click to collapse or expand..."> more... </a>
 <div id="label13" style="display:none">
 <table border="1">
 <tr>
 <td></td>
 <td colspan="3">Supported Version Ranges</td>
 </tr>
 <tr>
 <td>create_bearer</td>
 <td><code class="docutils literal notranslate">v6.0.0 -> v7.0.8 </code></td>
 <td><code class="docutils literal notranslate">v7.2.0 -> v7.2.4 </code></td>
 <td><code class="docutils literal notranslate">v7.4.3 -> 7.6.4 </code></td>
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
        <li> <span class="li-head">create_forwarding_tunnel_req_resp</span> - Create forwarding tunnel request/response (req 160, resp 161). <span class="li-normal">type: str</span> <span class="li-normal">choices: allow, deny</span>
 <a id='label14' href="javascript:ContentClick('label15', 'label14');" onmouseover="ContentPreview('label15');" onmouseout="ContentUnpreview('label15');" title="click to collapse or expand..."> more... </a>
 <div id="label15" style="display:none">
 <table border="1">
 <tr>
 <td></td>
 <td colspan="2">Supported Version Ranges</td>
 </tr>
 <tr>
 <td>create_forwarding_tunnel_req_resp</td>
 <td><code class="docutils literal notranslate">v7.2.1 -> v7.2.4 </code></td>
 <td><code class="docutils literal notranslate">v7.4.3 -> 7.6.4 </code></td>
 </tr>
 <tr>
 <td>[allow]</td>
 <td><code class="docutils literal notranslate">v7.2.1 -> v7.2.4</code></td>
 <tr>
 <td>[deny]</td>
 <td><code class="docutils literal notranslate">v7.2.1 -> v7.2.4</code></td>
 </table>
 </div>
 </li>
        <li> <span class="li-head">create_indirect_forwarding_tunnel_req_resp</span> - Create indirect data forwarding tunnel request/response (req 166, resp 167). <span class="li-normal">type: str</span> <span class="li-normal">choices: allow, deny</span>
 <a id='label16' href="javascript:ContentClick('label17', 'label16');" onmouseover="ContentPreview('label17');" onmouseout="ContentUnpreview('label17');" title="click to collapse or expand..."> more... </a>
 <div id="label17" style="display:none">
 <table border="1">
 <tr>
 <td></td>
 <td colspan="2">Supported Version Ranges</td>
 </tr>
 <tr>
 <td>create_indirect_forwarding_tunnel_req_resp</td>
 <td><code class="docutils literal notranslate">v7.2.1 -> v7.2.4 </code></td>
 <td><code class="docutils literal notranslate">v7.4.3 -> 7.6.4 </code></td>
 </tr>
 <tr>
 <td>[allow]</td>
 <td><code class="docutils literal notranslate">v7.2.1 -> v7.2.4</code></td>
 <tr>
 <td>[deny]</td>
 <td><code class="docutils literal notranslate">v7.2.1 -> v7.2.4</code></td>
 </table>
 </div>
 </li>
        <li> <span class="li-head">create_session</span> - Create session (req 32, resp 33). <span class="li-normal">type: str</span> <span class="li-normal">choices: allow, deny</span>
 <a id='label18' href="javascript:ContentClick('label19', 'label18');" onmouseover="ContentPreview('label19');" onmouseout="ContentUnpreview('label19');" title="click to collapse or expand..."> more... </a>
 <div id="label19" style="display:none">
 <table border="1">
 <tr>
 <td></td>
 <td colspan="3">Supported Version Ranges</td>
 </tr>
 <tr>
 <td>create_session</td>
 <td><code class="docutils literal notranslate">v6.0.0 -> v7.0.8 </code></td>
 <td><code class="docutils literal notranslate">v7.2.0 -> v7.2.4 </code></td>
 <td><code class="docutils literal notranslate">v7.4.3 -> 7.6.4 </code></td>
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
        <li> <span class="li-head">cs_paging</span> - CS paging indication (151) <span class="li-normal">type: str</span> <span class="li-normal">choices: allow, deny</span>
 <a id='label20' href="javascript:ContentClick('label21', 'label20');" onmouseover="ContentPreview('label21');" onmouseout="ContentUnpreview('label21');" title="click to collapse or expand..."> more... </a>
 <div id="label21" style="display:none">
 <table border="1">
 <tr>
 <td></td>
 <td colspan="2">Supported Version Ranges</td>
 </tr>
 <tr>
 <td>cs_paging</td>
 <td><code class="docutils literal notranslate">v7.2.1 -> v7.2.4 </code></td>
 <td><code class="docutils literal notranslate">v7.4.3 -> 7.6.4 </code></td>
 </tr>
 <tr>
 <td>[allow]</td>
 <td><code class="docutils literal notranslate">v7.2.1 -> v7.2.4</code></td>
 <tr>
 <td>[deny]</td>
 <td><code class="docutils literal notranslate">v7.2.1 -> v7.2.4</code></td>
 </table>
 </div>
 </li>
        <li> <span class="li-head">delete_bearer_cmd_fail</span> - Delete bearer (command 66, failure indication 67). <span class="li-normal">type: str</span> <span class="li-normal">choices: allow, deny</span>
 <a id='label22' href="javascript:ContentClick('label23', 'label22');" onmouseover="ContentPreview('label23');" onmouseout="ContentUnpreview('label23');" title="click to collapse or expand..."> more... </a>
 <div id="label23" style="display:none">
 <table border="1">
 <tr>
 <td></td>
 <td colspan="3">Supported Version Ranges</td>
 </tr>
 <tr>
 <td>delete_bearer_cmd_fail</td>
 <td><code class="docutils literal notranslate">v6.0.0 -> v7.0.8 </code></td>
 <td><code class="docutils literal notranslate">v7.2.0 -> v7.2.4 </code></td>
 <td><code class="docutils literal notranslate">v7.4.3 -> 7.6.4 </code></td>
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
        <li> <span class="li-head">delete_bearer_req_resp</span> - Delete bearer (req 99, resp 100). <span class="li-normal">type: str</span> <span class="li-normal">choices: allow, deny</span>
 <a id='label24' href="javascript:ContentClick('label25', 'label24');" onmouseover="ContentPreview('label25');" onmouseout="ContentUnpreview('label25');" title="click to collapse or expand..."> more... </a>
 <div id="label25" style="display:none">
 <table border="1">
 <tr>
 <td></td>
 <td colspan="3">Supported Version Ranges</td>
 </tr>
 <tr>
 <td>delete_bearer_req_resp</td>
 <td><code class="docutils literal notranslate">v6.0.0 -> v7.0.8 </code></td>
 <td><code class="docutils literal notranslate">v7.2.0 -> v7.2.4 </code></td>
 <td><code class="docutils literal notranslate">v7.4.3 -> 7.6.4 </code></td>
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
        <li> <span class="li-head">delete_indirect_forwarding_tunnel_req_resp</span> - Delete indirect data forwarding tunnel request/response (req 168, resp 169). <span class="li-normal">type: str</span> <span class="li-normal">choices: allow, deny</span>
 <a id='label26' href="javascript:ContentClick('label27', 'label26');" onmouseover="ContentPreview('label27');" onmouseout="ContentUnpreview('label27');" title="click to collapse or expand..."> more... </a>
 <div id="label27" style="display:none">
 <table border="1">
 <tr>
 <td></td>
 <td colspan="2">Supported Version Ranges</td>
 </tr>
 <tr>
 <td>delete_indirect_forwarding_tunnel_req_resp</td>
 <td><code class="docutils literal notranslate">v7.2.1 -> v7.2.4 </code></td>
 <td><code class="docutils literal notranslate">v7.4.3 -> 7.6.4 </code></td>
 </tr>
 <tr>
 <td>[allow]</td>
 <td><code class="docutils literal notranslate">v7.2.1 -> v7.2.4</code></td>
 <tr>
 <td>[deny]</td>
 <td><code class="docutils literal notranslate">v7.2.1 -> v7.2.4</code></td>
 </table>
 </div>
 </li>
        <li> <span class="li-head">delete_pdn_connection_set</span> - Delete PDN connection set (req 101, resp 102). <span class="li-normal">type: str</span> <span class="li-normal">choices: allow, deny</span>
 <a id='label28' href="javascript:ContentClick('label29', 'label28');" onmouseover="ContentPreview('label29');" onmouseout="ContentUnpreview('label29');" title="click to collapse or expand..."> more... </a>
 <div id="label29" style="display:none">
 <table border="1">
 <tr>
 <td></td>
 <td colspan="3">Supported Version Ranges</td>
 </tr>
 <tr>
 <td>delete_pdn_connection_set</td>
 <td><code class="docutils literal notranslate">v6.0.0 -> v7.0.8 </code></td>
 <td><code class="docutils literal notranslate">v7.2.0 -> v7.2.4 </code></td>
 <td><code class="docutils literal notranslate">v7.4.3 -> 7.6.4 </code></td>
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
        <li> <span class="li-head">delete_session</span> - Delete session (req 36, resp 37). <span class="li-normal">type: str</span> <span class="li-normal">choices: allow, deny</span>
 <a id='label30' href="javascript:ContentClick('label31', 'label30');" onmouseover="ContentPreview('label31');" onmouseout="ContentUnpreview('label31');" title="click to collapse or expand..."> more... </a>
 <div id="label31" style="display:none">
 <table border="1">
 <tr>
 <td></td>
 <td colspan="3">Supported Version Ranges</td>
 </tr>
 <tr>
 <td>delete_session</td>
 <td><code class="docutils literal notranslate">v6.0.0 -> v7.0.8 </code></td>
 <td><code class="docutils literal notranslate">v7.2.0 -> v7.2.4 </code></td>
 <td><code class="docutils literal notranslate">v7.4.3 -> 7.6.4 </code></td>
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
        <li> <span class="li-head">detach_notif_ack</span> - Detach notification/acknowledge (notif 149, ack 150). <span class="li-normal">type: str</span> <span class="li-normal">choices: allow, deny</span>
 <a id='label32' href="javascript:ContentClick('label33', 'label32');" onmouseover="ContentPreview('label33');" onmouseout="ContentUnpreview('label33');" title="click to collapse or expand..."> more... </a>
 <div id="label33" style="display:none">
 <table border="1">
 <tr>
 <td></td>
 <td colspan="2">Supported Version Ranges</td>
 </tr>
 <tr>
 <td>detach_notif_ack</td>
 <td><code class="docutils literal notranslate">v7.2.1 -> v7.2.4 </code></td>
 <td><code class="docutils literal notranslate">v7.4.3 -> 7.6.4 </code></td>
 </tr>
 <tr>
 <td>[allow]</td>
 <td><code class="docutils literal notranslate">v7.2.1 -> v7.2.4</code></td>
 <tr>
 <td>[deny]</td>
 <td><code class="docutils literal notranslate">v7.2.1 -> v7.2.4</code></td>
 </table>
 </div>
 </li>
        <li> <span class="li-head">dlink_data_notif_ack</span> - Downlink data notification/acknowledge (notif 176, ack 177). <span class="li-normal">type: str</span> <span class="li-normal">choices: allow, deny</span>
 <a id='label34' href="javascript:ContentClick('label35', 'label34');" onmouseover="ContentPreview('label35');" onmouseout="ContentUnpreview('label35');" title="click to collapse or expand..."> more... </a>
 <div id="label35" style="display:none">
 <table border="1">
 <tr>
 <td></td>
 <td colspan="2">Supported Version Ranges</td>
 </tr>
 <tr>
 <td>dlink_data_notif_ack</td>
 <td><code class="docutils literal notranslate">v7.2.1 -> v7.2.4 </code></td>
 <td><code class="docutils literal notranslate">v7.4.3 -> 7.6.4 </code></td>
 </tr>
 <tr>
 <td>[allow]</td>
 <td><code class="docutils literal notranslate">v7.2.1 -> v7.2.4</code></td>
 <tr>
 <td>[deny]</td>
 <td><code class="docutils literal notranslate">v7.2.1 -> v7.2.4</code></td>
 </table>
 </div>
 </li>
        <li> <span class="li-head">dlink_notif_failure</span> - Downlink data notification failure indication (70). <span class="li-normal">type: str</span> <span class="li-normal">choices: allow, deny</span>
 <a id='label36' href="javascript:ContentClick('label37', 'label36');" onmouseover="ContentPreview('label37');" onmouseout="ContentUnpreview('label37');" title="click to collapse or expand..."> more... </a>
 <div id="label37" style="display:none">
 <table border="1">
 <tr>
 <td></td>
 <td colspan="2">Supported Version Ranges</td>
 </tr>
 <tr>
 <td>dlink_notif_failure</td>
 <td><code class="docutils literal notranslate">v7.2.1 -> v7.2.4 </code></td>
 <td><code class="docutils literal notranslate">v7.4.3 -> 7.6.4 </code></td>
 </tr>
 <tr>
 <td>[allow]</td>
 <td><code class="docutils literal notranslate">v7.2.1 -> v7.2.4</code></td>
 <tr>
 <td>[deny]</td>
 <td><code class="docutils literal notranslate">v7.2.1 -> v7.2.4</code></td>
 </table>
 </div>
 </li>
        <li> <span class="li-head">echo</span> - Echo (req 1, resp 2). <span class="li-normal">type: str</span> <span class="li-normal">choices: allow, deny</span>
 <a id='label38' href="javascript:ContentClick('label39', 'label38');" onmouseover="ContentPreview('label39');" onmouseout="ContentUnpreview('label39');" title="click to collapse or expand..."> more... </a>
 <div id="label39" style="display:none">
 <table border="1">
 <tr>
 <td></td>
 <td colspan="3">Supported Version Ranges</td>
 </tr>
 <tr>
 <td>echo</td>
 <td><code class="docutils literal notranslate">v6.0.0 -> v7.0.8 </code></td>
 <td><code class="docutils literal notranslate">v7.2.0 -> v7.2.4 </code></td>
 <td><code class="docutils literal notranslate">v7.4.3 -> 7.6.4 </code></td>
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
        <li> <span class="li-head">forward_access_notif_ack</span> - Forward access context notification/acknowledge (notif 137, ack 138). <span class="li-normal">type: str</span> <span class="li-normal">choices: allow, deny</span>
 <a id='label40' href="javascript:ContentClick('label41', 'label40');" onmouseover="ContentPreview('label41');" onmouseout="ContentUnpreview('label41');" title="click to collapse or expand..."> more... </a>
 <div id="label41" style="display:none">
 <table border="1">
 <tr>
 <td></td>
 <td colspan="2">Supported Version Ranges</td>
 </tr>
 <tr>
 <td>forward_access_notif_ack</td>
 <td><code class="docutils literal notranslate">v7.2.1 -> v7.2.4 </code></td>
 <td><code class="docutils literal notranslate">v7.4.3 -> 7.6.4 </code></td>
 </tr>
 <tr>
 <td>[allow]</td>
 <td><code class="docutils literal notranslate">v7.2.1 -> v7.2.4</code></td>
 <tr>
 <td>[deny]</td>
 <td><code class="docutils literal notranslate">v7.2.1 -> v7.2.4</code></td>
 </table>
 </div>
 </li>
        <li> <span class="li-head">forward_relocation_cmp_notif_ack</span> - Forward relocation complete notification/acknowledge (notif 135, ack 136). <span class="li-normal">type: str</span> <span class="li-normal">choices: allow, deny</span>
 <a id='label42' href="javascript:ContentClick('label43', 'label42');" onmouseover="ContentPreview('label43');" onmouseout="ContentUnpreview('label43');" title="click to collapse or expand..."> more... </a>
 <div id="label43" style="display:none">
 <table border="1">
 <tr>
 <td></td>
 <td colspan="3">Supported Version Ranges</td>
 </tr>
 <tr>
 <td>forward_relocation_cmp_notif_ack</td>
 <td><code class="docutils literal notranslate">v7.0.2 -> v7.0.8 </code></td>
 <td><code class="docutils literal notranslate">v7.2.0 -> v7.2.4 </code></td>
 <td><code class="docutils literal notranslate">v7.4.3 -> 7.6.4 </code></td>
 </tr>
 <tr>
 <td>[allow]</td>
 <td><code class="docutils literal notranslate">v7.0.2 -> v7.0.8</code></td>
 <tr>
 <td>[deny]</td>
 <td><code class="docutils literal notranslate">v7.0.2 -> v7.0.8</code></td>
 </table>
 </div>
 </li>
        <li> <span class="li-head">forward_relocation_req_res</span> - Forward relocation request/response (req 133, resp 134). <span class="li-normal">type: str</span> <span class="li-normal">choices: allow, deny</span>
 <a id='label44' href="javascript:ContentClick('label45', 'label44');" onmouseover="ContentPreview('label45');" onmouseout="ContentUnpreview('label45');" title="click to collapse or expand..."> more... </a>
 <div id="label45" style="display:none">
 <table border="1">
 <tr>
 <td></td>
 <td colspan="3">Supported Version Ranges</td>
 </tr>
 <tr>
 <td>forward_relocation_req_res</td>
 <td><code class="docutils literal notranslate">v7.0.2 -> v7.0.8 </code></td>
 <td><code class="docutils literal notranslate">v7.2.0 -> v7.2.4 </code></td>
 <td><code class="docutils literal notranslate">v7.4.3 -> 7.6.4 </code></td>
 </tr>
 <tr>
 <td>[allow]</td>
 <td><code class="docutils literal notranslate">v7.0.2 -> v7.0.8</code></td>
 <tr>
 <td>[deny]</td>
 <td><code class="docutils literal notranslate">v7.0.2 -> v7.0.8</code></td>
 </table>
 </div>
 </li>
        <li> <span class="li-head">identification_req_resp</span> - Identification request/response (req 128, resp 129). <span class="li-normal">type: str</span> <span class="li-normal">choices: allow, deny</span>
 <a id='label46' href="javascript:ContentClick('label47', 'label46');" onmouseover="ContentPreview('label47');" onmouseout="ContentUnpreview('label47');" title="click to collapse or expand..."> more... </a>
 <div id="label47" style="display:none">
 <table border="1">
 <tr>
 <td></td>
 <td colspan="2">Supported Version Ranges</td>
 </tr>
 <tr>
 <td>identification_req_resp</td>
 <td><code class="docutils literal notranslate">v7.2.1 -> v7.2.4 </code></td>
 <td><code class="docutils literal notranslate">v7.4.3 -> 7.6.4 </code></td>
 </tr>
 <tr>
 <td>[allow]</td>
 <td><code class="docutils literal notranslate">v7.2.1 -> v7.2.4</code></td>
 <tr>
 <td>[deny]</td>
 <td><code class="docutils literal notranslate">v7.2.1 -> v7.2.4</code></td>
 </table>
 </div>
 </li>
        <li> <span class="li-head">isr_status</span> - ISR status indication (157). <span class="li-normal">type: str</span> <span class="li-normal">choices: allow, deny</span>
 <a id='label48' href="javascript:ContentClick('label49', 'label48');" onmouseover="ContentPreview('label49');" onmouseout="ContentUnpreview('label49');" title="click to collapse or expand..."> more... </a>
 <div id="label49" style="display:none">
 <table border="1">
 <tr>
 <td></td>
 <td colspan="2">Supported Version Ranges</td>
 </tr>
 <tr>
 <td>isr_status</td>
 <td><code class="docutils literal notranslate">v7.2.1 -> v7.2.4 </code></td>
 <td><code class="docutils literal notranslate">v7.4.3 -> 7.6.4 </code></td>
 </tr>
 <tr>
 <td>[allow]</td>
 <td><code class="docutils literal notranslate">v7.2.1 -> v7.2.4</code></td>
 <tr>
 <td>[deny]</td>
 <td><code class="docutils literal notranslate">v7.2.1 -> v7.2.4</code></td>
 </table>
 </div>
 </li>
        <li> <span class="li-head">mbms_session_start_req_resp</span> - MBMS session start request/response (req 231, resp 232). <span class="li-normal">type: str</span> <span class="li-normal">choices: allow, deny</span>
 <a id='label50' href="javascript:ContentClick('label51', 'label50');" onmouseover="ContentPreview('label51');" onmouseout="ContentUnpreview('label51');" title="click to collapse or expand..."> more... </a>
 <div id="label51" style="display:none">
 <table border="1">
 <tr>
 <td></td>
 <td colspan="2">Supported Version Ranges</td>
 </tr>
 <tr>
 <td>mbms_session_start_req_resp</td>
 <td><code class="docutils literal notranslate">v7.2.1 -> v7.2.4 </code></td>
 <td><code class="docutils literal notranslate">v7.4.3 -> 7.6.4 </code></td>
 </tr>
 <tr>
 <td>[allow]</td>
 <td><code class="docutils literal notranslate">v7.2.1 -> v7.2.4</code></td>
 <tr>
 <td>[deny]</td>
 <td><code class="docutils literal notranslate">v7.2.1 -> v7.2.4</code></td>
 </table>
 </div>
 </li>
        <li> <span class="li-head">mbms_session_stop_req_resp</span> - MBMS session stop request/response (req 235, resp 236). <span class="li-normal">type: str</span> <span class="li-normal">choices: allow, deny</span>
 <a id='label52' href="javascript:ContentClick('label53', 'label52');" onmouseover="ContentPreview('label53');" onmouseout="ContentUnpreview('label53');" title="click to collapse or expand..."> more... </a>
 <div id="label53" style="display:none">
 <table border="1">
 <tr>
 <td></td>
 <td colspan="2">Supported Version Ranges</td>
 </tr>
 <tr>
 <td>mbms_session_stop_req_resp</td>
 <td><code class="docutils literal notranslate">v7.2.1 -> v7.2.4 </code></td>
 <td><code class="docutils literal notranslate">v7.4.3 -> 7.6.4 </code></td>
 </tr>
 <tr>
 <td>[allow]</td>
 <td><code class="docutils literal notranslate">v7.2.1 -> v7.2.4</code></td>
 <tr>
 <td>[deny]</td>
 <td><code class="docutils literal notranslate">v7.2.1 -> v7.2.4</code></td>
 </table>
 </div>
 </li>
        <li> <span class="li-head">mbms_session_update_req_resp</span> - MBMS session update request/response (req 233, resp 234). <span class="li-normal">type: str</span> <span class="li-normal">choices: allow, deny</span>
 <a id='label54' href="javascript:ContentClick('label55', 'label54');" onmouseover="ContentPreview('label55');" onmouseout="ContentUnpreview('label55');" title="click to collapse or expand..."> more... </a>
 <div id="label55" style="display:none">
 <table border="1">
 <tr>
 <td></td>
 <td colspan="2">Supported Version Ranges</td>
 </tr>
 <tr>
 <td>mbms_session_update_req_resp</td>
 <td><code class="docutils literal notranslate">v7.2.1 -> v7.2.4 </code></td>
 <td><code class="docutils literal notranslate">v7.4.3 -> 7.6.4 </code></td>
 </tr>
 <tr>
 <td>[allow]</td>
 <td><code class="docutils literal notranslate">v7.2.1 -> v7.2.4</code></td>
 <tr>
 <td>[deny]</td>
 <td><code class="docutils literal notranslate">v7.2.1 -> v7.2.4</code></td>
 </table>
 </div>
 </li>
        <li> <span class="li-head">modify_access_req_resp</span> - Modify access bearers request/response (req 211, resp 212). <span class="li-normal">type: str</span> <span class="li-normal">choices: allow, deny</span>
 <a id='label56' href="javascript:ContentClick('label57', 'label56');" onmouseover="ContentPreview('label57');" onmouseout="ContentUnpreview('label57');" title="click to collapse or expand..."> more... </a>
 <div id="label57" style="display:none">
 <table border="1">
 <tr>
 <td></td>
 <td colspan="2">Supported Version Ranges</td>
 </tr>
 <tr>
 <td>modify_access_req_resp</td>
 <td><code class="docutils literal notranslate">v7.2.1 -> v7.2.4 </code></td>
 <td><code class="docutils literal notranslate">v7.4.3 -> 7.6.4 </code></td>
 </tr>
 <tr>
 <td>[allow]</td>
 <td><code class="docutils literal notranslate">v7.2.1 -> v7.2.4</code></td>
 <tr>
 <td>[deny]</td>
 <td><code class="docutils literal notranslate">v7.2.1 -> v7.2.4</code></td>
 </table>
 </div>
 </li>
        <li> <span class="li-head">modify_bearer_cmd_fail</span> - Modify bearer (command 64 , failure indication 65). <span class="li-normal">type: str</span> <span class="li-normal">choices: allow, deny</span>
 <a id='label58' href="javascript:ContentClick('label59', 'label58');" onmouseover="ContentPreview('label59');" onmouseout="ContentUnpreview('label59');" title="click to collapse or expand..."> more... </a>
 <div id="label59" style="display:none">
 <table border="1">
 <tr>
 <td></td>
 <td colspan="3">Supported Version Ranges</td>
 </tr>
 <tr>
 <td>modify_bearer_cmd_fail</td>
 <td><code class="docutils literal notranslate">v6.0.0 -> v7.0.8 </code></td>
 <td><code class="docutils literal notranslate">v7.2.0 -> v7.2.4 </code></td>
 <td><code class="docutils literal notranslate">v7.4.3 -> 7.6.4 </code></td>
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
        <li> <span class="li-head">modify_bearer_req_resp</span> - Modify bearer (req 34, resp 35). <span class="li-normal">type: str</span> <span class="li-normal">choices: allow, deny</span>
 <a id='label60' href="javascript:ContentClick('label61', 'label60');" onmouseover="ContentPreview('label61');" onmouseout="ContentUnpreview('label61');" title="click to collapse or expand..."> more... </a>
 <div id="label61" style="display:none">
 <table border="1">
 <tr>
 <td></td>
 <td colspan="3">Supported Version Ranges</td>
 </tr>
 <tr>
 <td>modify_bearer_req_resp</td>
 <td><code class="docutils literal notranslate">v6.0.0 -> v7.0.8 </code></td>
 <td><code class="docutils literal notranslate">v7.2.0 -> v7.2.4 </code></td>
 <td><code class="docutils literal notranslate">v7.4.3 -> 7.6.4 </code></td>
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
        <li> <span class="li-head">name</span> - Message filter name. <span class="li-normal">type: str</span> <span class="li-required">required: true</span>
 <a id='label62' href="javascript:ContentClick('label63', 'label62');" onmouseover="ContentPreview('label63');" onmouseout="ContentUnpreview('label63');" title="click to collapse or expand..."> more... </a>
 <div id="label63" style="display:none">
 <table border="1">
 <tr>
 <td></td>
 <td colspan="3">Supported Version Ranges</td>
 </tr>
 <tr>
 <td>name</td>
 <td><code class="docutils literal notranslate">v6.0.0 -> v7.0.8 </code></td>
 <td><code class="docutils literal notranslate">v7.2.0 -> v7.2.4 </code></td>
 <td><code class="docutils literal notranslate">v7.4.3 -> 7.6.4 </code></td>
 </tr>
 </table>
 </div>
 </li>
        <li> <span class="li-head">pgw_dlink_notif_ack</span> - PGW downlink triggering notification/acknowledge (notif 103, ack 104). <span class="li-normal">type: str</span> <span class="li-normal">choices: allow, deny</span>
 <a id='label64' href="javascript:ContentClick('label65', 'label64');" onmouseover="ContentPreview('label65');" onmouseout="ContentUnpreview('label65');" title="click to collapse or expand..."> more... </a>
 <div id="label65" style="display:none">
 <table border="1">
 <tr>
 <td></td>
 <td colspan="2">Supported Version Ranges</td>
 </tr>
 <tr>
 <td>pgw_dlink_notif_ack</td>
 <td><code class="docutils literal notranslate">v7.2.1 -> v7.2.4 </code></td>
 <td><code class="docutils literal notranslate">v7.4.3 -> 7.6.4 </code></td>
 </tr>
 <tr>
 <td>[allow]</td>
 <td><code class="docutils literal notranslate">v7.2.1 -> v7.2.4</code></td>
 <tr>
 <td>[deny]</td>
 <td><code class="docutils literal notranslate">v7.2.1 -> v7.2.4</code></td>
 </table>
 </div>
 </li>
        <li> <span class="li-head">pgw_restart_notif_ack</span> - PGW restart notification/acknowledge (notif 179, ack 180). <span class="li-normal">type: str</span> <span class="li-normal">choices: allow, deny</span>
 <a id='label66' href="javascript:ContentClick('label67', 'label66');" onmouseover="ContentPreview('label67');" onmouseout="ContentUnpreview('label67');" title="click to collapse or expand..."> more... </a>
 <div id="label67" style="display:none">
 <table border="1">
 <tr>
 <td></td>
 <td colspan="2">Supported Version Ranges</td>
 </tr>
 <tr>
 <td>pgw_restart_notif_ack</td>
 <td><code class="docutils literal notranslate">v7.2.1 -> v7.2.4 </code></td>
 <td><code class="docutils literal notranslate">v7.4.3 -> 7.6.4 </code></td>
 </tr>
 <tr>
 <td>[allow]</td>
 <td><code class="docutils literal notranslate">v7.2.1 -> v7.2.4</code></td>
 <tr>
 <td>[deny]</td>
 <td><code class="docutils literal notranslate">v7.2.1 -> v7.2.4</code></td>
 </table>
 </div>
 </li>
        <li> <span class="li-head">ran_info_relay</span> - RAN information relay (152). <span class="li-normal">type: str</span> <span class="li-normal">choices: allow, deny</span>
 <a id='label68' href="javascript:ContentClick('label69', 'label68');" onmouseover="ContentPreview('label69');" onmouseout="ContentUnpreview('label69');" title="click to collapse or expand..."> more... </a>
 <div id="label69" style="display:none">
 <table border="1">
 <tr>
 <td></td>
 <td colspan="2">Supported Version Ranges</td>
 </tr>
 <tr>
 <td>ran_info_relay</td>
 <td><code class="docutils literal notranslate">v7.2.1 -> v7.2.4 </code></td>
 <td><code class="docutils literal notranslate">v7.4.3 -> 7.6.4 </code></td>
 </tr>
 <tr>
 <td>[allow]</td>
 <td><code class="docutils literal notranslate">v7.2.1 -> v7.2.4</code></td>
 <tr>
 <td>[deny]</td>
 <td><code class="docutils literal notranslate">v7.2.1 -> v7.2.4</code></td>
 </table>
 </div>
 </li>
        <li> <span class="li-head">release_access_bearer_req_resp</span> - Release access bearers request/response (req 170, resp 171). <span class="li-normal">type: str</span> <span class="li-normal">choices: allow, deny</span>
 <a id='label70' href="javascript:ContentClick('label71', 'label70');" onmouseover="ContentPreview('label71');" onmouseout="ContentUnpreview('label71');" title="click to collapse or expand..."> more... </a>
 <div id="label71" style="display:none">
 <table border="1">
 <tr>
 <td></td>
 <td colspan="2">Supported Version Ranges</td>
 </tr>
 <tr>
 <td>release_access_bearer_req_resp</td>
 <td><code class="docutils literal notranslate">v7.2.1 -> v7.2.4 </code></td>
 <td><code class="docutils literal notranslate">v7.4.3 -> 7.6.4 </code></td>
 </tr>
 <tr>
 <td>[allow]</td>
 <td><code class="docutils literal notranslate">v7.2.1 -> v7.2.4</code></td>
 <tr>
 <td>[deny]</td>
 <td><code class="docutils literal notranslate">v7.2.1 -> v7.2.4</code></td>
 </table>
 </div>
 </li>
        <li> <span class="li-head">relocation_cancel_req_resp</span> - Relocation cancel request/response (req 139, resp 140). <span class="li-normal">type: str</span> <span class="li-normal">choices: allow, deny</span>
 <a id='label72' href="javascript:ContentClick('label73', 'label72');" onmouseover="ContentPreview('label73');" onmouseout="ContentUnpreview('label73');" title="click to collapse or expand..."> more... </a>
 <div id="label73" style="display:none">
 <table border="1">
 <tr>
 <td></td>
 <td colspan="2">Supported Version Ranges</td>
 </tr>
 <tr>
 <td>relocation_cancel_req_resp</td>
 <td><code class="docutils literal notranslate">v7.2.1 -> v7.2.4 </code></td>
 <td><code class="docutils literal notranslate">v7.4.3 -> 7.6.4 </code></td>
 </tr>
 <tr>
 <td>[allow]</td>
 <td><code class="docutils literal notranslate">v7.2.1 -> v7.2.4</code></td>
 <tr>
 <td>[deny]</td>
 <td><code class="docutils literal notranslate">v7.2.1 -> v7.2.4</code></td>
 </table>
 </div>
 </li>
        <li> <span class="li-head">remote_ue_report_notif_ack</span> - Remote UE report notification/acknowledge (notif 40, ack 41). <span class="li-normal">type: str</span> <span class="li-normal">choices: allow, deny</span>
 <a id='label74' href="javascript:ContentClick('label75', 'label74');" onmouseover="ContentPreview('label75');" onmouseout="ContentUnpreview('label75');" title="click to collapse or expand..."> more... </a>
 <div id="label75" style="display:none">
 <table border="1">
 <tr>
 <td></td>
 <td colspan="2">Supported Version Ranges</td>
 </tr>
 <tr>
 <td>remote_ue_report_notif_ack</td>
 <td><code class="docutils literal notranslate">v7.2.1 -> v7.2.4 </code></td>
 <td><code class="docutils literal notranslate">v7.4.3 -> 7.6.4 </code></td>
 </tr>
 <tr>
 <td>[allow]</td>
 <td><code class="docutils literal notranslate">v7.2.1 -> v7.2.4</code></td>
 <tr>
 <td>[deny]</td>
 <td><code class="docutils literal notranslate">v7.2.1 -> v7.2.4</code></td>
 </table>
 </div>
 </li>
        <li> <span class="li-head">reserved_for_earlier_version</span> - Reserved for earlier version of the GTP specification (178). <span class="li-normal">type: str</span> <span class="li-normal">choices: allow, deny</span>
 <a id='label76' href="javascript:ContentClick('label77', 'label76');" onmouseover="ContentPreview('label77');" onmouseout="ContentUnpreview('label77');" title="click to collapse or expand..."> more... </a>
 <div id="label77" style="display:none">
 <table border="1">
 <tr>
 <td></td>
 <td colspan="2">Supported Version Ranges</td>
 </tr>
 <tr>
 <td>reserved_for_earlier_version</td>
 <td><code class="docutils literal notranslate">v7.2.1 -> v7.2.4 </code></td>
 <td><code class="docutils literal notranslate">v7.4.3 -> 7.6.4 </code></td>
 </tr>
 <tr>
 <td>[allow]</td>
 <td><code class="docutils literal notranslate">v7.2.1 -> v7.2.4</code></td>
 <tr>
 <td>[deny]</td>
 <td><code class="docutils literal notranslate">v7.2.1 -> v7.2.4</code></td>
 </table>
 </div>
 </li>
        <li> <span class="li-head">resume</span> - Resume (notify 164 , ack 165). <span class="li-normal">type: str</span> <span class="li-normal">choices: allow, deny</span>
 <a id='label78' href="javascript:ContentClick('label79', 'label78');" onmouseover="ContentPreview('label79');" onmouseout="ContentUnpreview('label79');" title="click to collapse or expand..."> more... </a>
 <div id="label79" style="display:none">
 <table border="1">
 <tr>
 <td></td>
 <td colspan="3">Supported Version Ranges</td>
 </tr>
 <tr>
 <td>resume</td>
 <td><code class="docutils literal notranslate">v6.0.0 -> v7.0.8 </code></td>
 <td><code class="docutils literal notranslate">v7.2.0 -> v7.2.4 </code></td>
 <td><code class="docutils literal notranslate">v7.4.3 -> 7.6.4 </code></td>
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
        <li> <span class="li-head">stop_paging_indication</span> - Stop Paging Indication (73). <span class="li-normal">type: str</span> <span class="li-normal">choices: allow, deny</span>
 <a id='label80' href="javascript:ContentClick('label81', 'label80');" onmouseover="ContentPreview('label81');" onmouseout="ContentUnpreview('label81');" title="click to collapse or expand..."> more... </a>
 <div id="label81" style="display:none">
 <table border="1">
 <tr>
 <td></td>
 <td colspan="2">Supported Version Ranges</td>
 </tr>
 <tr>
 <td>stop_paging_indication</td>
 <td><code class="docutils literal notranslate">v7.2.1 -> v7.2.4 </code></td>
 <td><code class="docutils literal notranslate">v7.4.3 -> 7.6.4 </code></td>
 </tr>
 <tr>
 <td>[allow]</td>
 <td><code class="docutils literal notranslate">v7.2.1 -> v7.2.4</code></td>
 <tr>
 <td>[deny]</td>
 <td><code class="docutils literal notranslate">v7.2.1 -> v7.2.4</code></td>
 </table>
 </div>
 </li>
        <li> <span class="li-head">suspend</span> - Suspend (notify 162, ack 163). <span class="li-normal">type: str</span> <span class="li-normal">choices: allow, deny</span>
 <a id='label82' href="javascript:ContentClick('label83', 'label82');" onmouseover="ContentPreview('label83');" onmouseout="ContentUnpreview('label83');" title="click to collapse or expand..."> more... </a>
 <div id="label83" style="display:none">
 <table border="1">
 <tr>
 <td></td>
 <td colspan="3">Supported Version Ranges</td>
 </tr>
 <tr>
 <td>suspend</td>
 <td><code class="docutils literal notranslate">v6.0.0 -> v7.0.8 </code></td>
 <td><code class="docutils literal notranslate">v7.2.0 -> v7.2.4 </code></td>
 <td><code class="docutils literal notranslate">v7.4.3 -> 7.6.4 </code></td>
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
        <li> <span class="li-head">trace_session</span> - Trace session (activation 71, deactivation 72). <span class="li-normal">type: str</span> <span class="li-normal">choices: allow, deny</span>
 <a id='label84' href="javascript:ContentClick('label85', 'label84');" onmouseover="ContentPreview('label85');" onmouseout="ContentUnpreview('label85');" title="click to collapse or expand..."> more... </a>
 <div id="label85" style="display:none">
 <table border="1">
 <tr>
 <td></td>
 <td colspan="3">Supported Version Ranges</td>
 </tr>
 <tr>
 <td>trace_session</td>
 <td><code class="docutils literal notranslate">v6.0.0 -> v7.0.8 </code></td>
 <td><code class="docutils literal notranslate">v7.2.0 -> v7.2.4 </code></td>
 <td><code class="docutils literal notranslate">v7.4.3 -> 7.6.4 </code></td>
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
        <li> <span class="li-head">ue_activity_notif_ack</span> - UE activity notification/acknowledge (notif 155, ack 156). <span class="li-normal">type: str</span> <span class="li-normal">choices: allow, deny</span>
 <a id='label86' href="javascript:ContentClick('label87', 'label86');" onmouseover="ContentPreview('label87');" onmouseout="ContentUnpreview('label87');" title="click to collapse or expand..."> more... </a>
 <div id="label87" style="display:none">
 <table border="1">
 <tr>
 <td></td>
 <td colspan="2">Supported Version Ranges</td>
 </tr>
 <tr>
 <td>ue_activity_notif_ack</td>
 <td><code class="docutils literal notranslate">v7.2.1 -> v7.2.4 </code></td>
 <td><code class="docutils literal notranslate">v7.4.3 -> 7.6.4 </code></td>
 </tr>
 <tr>
 <td>[allow]</td>
 <td><code class="docutils literal notranslate">v7.2.1 -> v7.2.4</code></td>
 <tr>
 <td>[deny]</td>
 <td><code class="docutils literal notranslate">v7.2.1 -> v7.2.4</code></td>
 </table>
 </div>
 </li>
        <li> <span class="li-head">ue_registration_query_req_resp</span> - UE registration query request/response (req 158, resp 159). <span class="li-normal">type: str</span> <span class="li-normal">choices: allow, deny</span>
 <a id='label88' href="javascript:ContentClick('label89', 'label88');" onmouseover="ContentPreview('label89');" onmouseout="ContentUnpreview('label89');" title="click to collapse or expand..."> more... </a>
 <div id="label89" style="display:none">
 <table border="1">
 <tr>
 <td></td>
 <td colspan="2">Supported Version Ranges</td>
 </tr>
 <tr>
 <td>ue_registration_query_req_resp</td>
 <td><code class="docutils literal notranslate">v7.2.1 -> v7.2.4 </code></td>
 <td><code class="docutils literal notranslate">v7.4.3 -> 7.6.4 </code></td>
 </tr>
 <tr>
 <td>[allow]</td>
 <td><code class="docutils literal notranslate">v7.2.1 -> v7.2.4</code></td>
 <tr>
 <td>[deny]</td>
 <td><code class="docutils literal notranslate">v7.2.1 -> v7.2.4</code></td>
 </table>
 </div>
 </li>
        <li> <span class="li-head">unknown_message</span> - Allow or Deny unknown messages. <span class="li-normal">type: str</span> <span class="li-normal">choices: allow, deny</span>
 <a id='label90' href="javascript:ContentClick('label91', 'label90');" onmouseover="ContentPreview('label91');" onmouseout="ContentUnpreview('label91');" title="click to collapse or expand..."> more... </a>
 <div id="label91" style="display:none">
 <table border="1">
 <tr>
 <td></td>
 <td colspan="3">Supported Version Ranges</td>
 </tr>
 <tr>
 <td>unknown_message</td>
 <td><code class="docutils literal notranslate">v6.0.0 -> v7.0.8 </code></td>
 <td><code class="docutils literal notranslate">v7.2.0 -> v7.2.4 </code></td>
 <td><code class="docutils literal notranslate">v7.4.3 -> 7.6.4 </code></td>
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
        <li> <span class="li-head">unknown_message_white_list</span> - White list (to allow) of unknown messages. <span class="li-normal">type: list</span> <span style="font-family:'Courier New'" class="li-required">member_path: unknown_message_white_list:id</span>
 <a id='label92' href="javascript:ContentClick('label93', 'label92');" onmouseover="ContentPreview('label93');" onmouseout="ContentUnpreview('label93');" title="click to collapse or expand..."> more... </a>
 <div id="label93" style="display:none">
 <table border="1">
 <tr>
 <td></td><td colspan="3">Supported Version Ranges</td>
 </tr>
 <tr>
 <td>unknown_message_white_list</td>
 <td><code class="docutils literal notranslate">v6.0.0 -> v7.0.8 </code></td>
 <td><code class="docutils literal notranslate">v7.2.0 -> v7.2.4 </code></td>
 <td><code class="docutils literal notranslate">v7.4.3 -> 7.6.4 </code></td>
 </tr>
 </table>
 </div>
 </li>
            <ul class="ul-self">
            <li> <span class="li-head">id</span> - Message IDs. see <a href='#notes'>Notes</a>. <span class="li-normal">type: int</span> <span class="li-required">required: true</span>
 <a id='label94' href="javascript:ContentClick('label95', 'label94');" onmouseover="ContentPreview('label95');" onmouseout="ContentUnpreview('label95');" title="click to collapse or expand..."> more... </a>
 <div id="label95" style="display:none">
 <table border="1">
 <tr>
 <td></td>
 <td colspan="3">Supported Version Ranges</td>
 </tr>
 <tr>
 <td>id</td>
 <td><code class="docutils literal notranslate">v6.0.0 -> v7.0.8 </code></td>
 <td><code class="docutils literal notranslate">v7.2.0 -> v7.2.4 </code></td>
 <td><code class="docutils literal notranslate">v7.4.3 -> 7.6.4 </code></td>
 </tr>
 </table>
 </div>
 </li>
            </ul>
        <li> <span class="li-head">update_bearer</span> - Update bearer (req 97, resp 98). <span class="li-normal">type: str</span> <span class="li-normal">choices: allow, deny</span>
 <a id='label96' href="javascript:ContentClick('label97', 'label96');" onmouseover="ContentPreview('label97');" onmouseout="ContentUnpreview('label97');" title="click to collapse or expand..."> more... </a>
 <div id="label97" style="display:none">
 <table border="1">
 <tr>
 <td></td>
 <td colspan="3">Supported Version Ranges</td>
 </tr>
 <tr>
 <td>update_bearer</td>
 <td><code class="docutils literal notranslate">v6.0.0 -> v7.0.8 </code></td>
 <td><code class="docutils literal notranslate">v7.2.0 -> v7.2.4 </code></td>
 <td><code class="docutils literal notranslate">v7.4.3 -> 7.6.4 </code></td>
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
        <li> <span class="li-head">update_pdn_connection_set</span> - Update PDN connection set (req 200, resp 201). <span class="li-normal">type: str</span> <span class="li-normal">choices: allow, deny</span>
 <a id='label98' href="javascript:ContentClick('label99', 'label98');" onmouseover="ContentPreview('label99');" onmouseout="ContentUnpreview('label99');" title="click to collapse or expand..."> more... </a>
 <div id="label99" style="display:none">
 <table border="1">
 <tr>
 <td></td>
 <td colspan="3">Supported Version Ranges</td>
 </tr>
 <tr>
 <td>update_pdn_connection_set</td>
 <td><code class="docutils literal notranslate">v6.0.0 -> v7.0.8 </code></td>
 <td><code class="docutils literal notranslate">v7.2.0 -> v7.2.4 </code></td>
 <td><code class="docutils literal notranslate">v7.4.3 -> 7.6.4 </code></td>
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
        <li> <span class="li-head">version_not_support</span> - Version not supported (3). <span class="li-normal">type: str</span> <span class="li-normal">choices: allow, deny</span>
 <a id='label100' href="javascript:ContentClick('label101', 'label100');" onmouseover="ContentPreview('label101');" onmouseout="ContentUnpreview('label101');" title="click to collapse or expand..."> more... </a>
 <div id="label101" style="display:none">
 <table border="1">
 <tr>
 <td></td>
 <td colspan="3">Supported Version Ranges</td>
 </tr>
 <tr>
 <td>version_not_support</td>
 <td><code class="docutils literal notranslate">v6.0.0 -> v7.0.8 </code></td>
 <td><code class="docutils literal notranslate">v7.2.0 -> v7.2.4 </code></td>
 <td><code class="docutils literal notranslate">v7.4.3 -> 7.6.4 </code></td>
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
    
    - name: Message filter for GTPv2 messages.
      fortinet.fortios.fortios_gtp_message_filter_v2:
          vdom: "{{ vdom }}"
          state: "present"
          access_token: "<your_own_value>"
          gtp_message_filter_v2:
              alert_mme_notif_ack: "allow"
              bearer_resource_cmd_fail: "allow"
              change_notification: "allow"
              configuration_transfer_tunnel: "allow"
              context_req_res_ack: "allow"
              create_bearer: "allow"
              create_forwarding_tunnel_req_resp: "allow"
              create_indirect_forwarding_tunnel_req_resp: "allow"
              create_session: "allow"
              cs_paging: "allow"
              delete_bearer_cmd_fail: "allow"
              delete_bearer_req_resp: "allow"
              delete_indirect_forwarding_tunnel_req_resp: "allow"
              delete_pdn_connection_set: "allow"
              delete_session: "allow"
              detach_notif_ack: "allow"
              dlink_data_notif_ack: "allow"
              dlink_notif_failure: "allow"
              echo: "allow"
              forward_access_notif_ack: "allow"
              forward_relocation_cmp_notif_ack: "allow"
              forward_relocation_req_res: "allow"
              identification_req_resp: "allow"
              isr_status: "allow"
              mbms_session_start_req_resp: "allow"
              mbms_session_stop_req_resp: "allow"
              mbms_session_update_req_resp: "allow"
              modify_access_req_resp: "allow"
              modify_bearer_cmd_fail: "allow"
              modify_bearer_req_resp: "allow"
              name: "default_name_33"
              pgw_dlink_notif_ack: "allow"
              pgw_restart_notif_ack: "allow"
              ran_info_relay: "allow"
              release_access_bearer_req_resp: "allow"
              relocation_cancel_req_resp: "allow"
              remote_ue_report_notif_ack: "allow"
              reserved_for_earlier_version: "allow"
              resume: "allow"
              stop_paging_indication: "allow"
              suspend: "allow"
              trace_session: "allow"
              ue_activity_notif_ack: "allow"
              ue_registration_query_req_resp: "allow"
              unknown_message: "allow"
              unknown_message_white_list:
                  -
                      id: "49"
              update_bearer: "allow"
              update_pdn_connection_set: "allow"
              version_not_support: "allow"


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
