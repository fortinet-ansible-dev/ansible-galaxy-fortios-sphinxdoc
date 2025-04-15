:source: fortios_ztna_traffic_forward_proxy.py

:orphan:

.. fortios_ztna_traffic_forward_proxy:

fortios_ztna_traffic_forward_proxy -- Configure ZTNA traffic forward proxy in Fortinet's FortiOS and FortiGate.
+++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++

.. versionadded:: 2.0.0

.. contents::
   :local:
   :depth: 1


Synopsis
--------
- This module is able to configure a FortiGate or FortiOS (FOS) device by allowing the user to set and modify ztna feature and traffic_forward_proxy category. Examples include all parameters and values need to be adjusted to datasources before usage. Tested with FOS v6.0.0



Requirements
------------
The below requirements are needed on the host that executes this module.

- ansible>=2.15


Tips
----
Using member operation to add an element to an existing object.

FortiOS Version Compatibility
-----------------------------
Supported Version Ranges: v7.6.0 -> v7.6.2


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
    <li> <span class="li-head">ztna_traffic_forward_proxy</span> - Configure ZTNA traffic forward proxy. <span class="li-normal">type: dict</span>
 <a id='label0' href="javascript:ContentClick('label1', 'label0');" onmouseover="ContentPreview('label1');" onmouseout="ContentUnpreview('label1');" title="click to collapse or expand..."> more... </a>
 <div id="label1" style="display:none">
 <table border="1">
 <tr>
 <td></td><td colspan="1">Supported Version Ranges</td>
 </tr>
 <tr>
 <td>ztna_traffic_forward_proxy</td>
 <td><code class="docutils literal notranslate">v7.6.0 -> 7.6.2 </code></td>
 </tr>
 </table>
 </div>
 </li>
        <ul class="ul-self">
        <li> <span class="li-head">auth_portal</span> - Enable/disable authentication portal. <span class="li-normal">type: str</span> <span class="li-normal">choices: disable, enable</span>
 <a id='label2' href="javascript:ContentClick('label3', 'label2');" onmouseover="ContentPreview('label3');" onmouseout="ContentUnpreview('label3');" title="click to collapse or expand..."> more... </a>
 <div id="label3" style="display:none">
 <table border="1">
 <tr>
 <td></td>
 <td colspan="1">Supported Version Ranges</td>
 </tr>
 <tr>
 <td>auth_portal</td>
 <td><code class="docutils literal notranslate">v7.6.0 -> 7.6.2 </code></td>
 </tr>
 <tr>
 <td>[disable]</td>
 <td><code class="docutils literal notranslate">v7.6.0 -> 7.6.2</code></td>
 <tr>
 <td>[enable]</td>
 <td><code class="docutils literal notranslate">v7.6.0 -> 7.6.2</code></td>
 </table>
 </div>
 </li>
        <li> <span class="li-head">auth_virtual_host</span> - Virtual host for authentication portal. Source firewall.access-proxy-virtual-host.name. <span class="li-normal">type: str</span>
 <a id='label4' href="javascript:ContentClick('label5', 'label4');" onmouseover="ContentPreview('label5');" onmouseout="ContentUnpreview('label5');" title="click to collapse or expand..."> more... </a>
 <div id="label5" style="display:none">
 <table border="1">
 <tr>
 <td></td>
 <td colspan="1">Supported Version Ranges</td>
 </tr>
 <tr>
 <td>auth_virtual_host</td>
 <td><code class="docutils literal notranslate">v7.6.1 -> 7.6.2 </code></td>
 </tr>
 </table>
 </div>
 </li>
        <li> <span class="li-head">client_cert</span> - Enable/disable to request client certificate. <span class="li-normal">type: str</span> <span class="li-normal">choices: disable, enable</span>
 <a id='label6' href="javascript:ContentClick('label7', 'label6');" onmouseover="ContentPreview('label7');" onmouseout="ContentUnpreview('label7');" title="click to collapse or expand..."> more... </a>
 <div id="label7" style="display:none">
 <table border="1">
 <tr>
 <td></td>
 <td colspan="1">Supported Version Ranges</td>
 </tr>
 <tr>
 <td>client_cert</td>
 <td><code class="docutils literal notranslate">v7.6.0 -> v7.6.0 </code></td>
 </tr>
 <tr>
 <td>[disable]</td>
 <td><code class="docutils literal notranslate">v7.6.0 -> v7.6.0</code></td>
 <tr>
 <td>[enable]</td>
 <td><code class="docutils literal notranslate">v7.6.0 -> v7.6.0</code></td>
 </table>
 </div>
 </li>
        <li> <span class="li-head">comment</span> - Comment. <span class="li-normal">type: str</span>
 <a id='label8' href="javascript:ContentClick('label9', 'label8');" onmouseover="ContentPreview('label9');" onmouseout="ContentUnpreview('label9');" title="click to collapse or expand..."> more... </a>
 <div id="label9" style="display:none">
 <table border="1">
 <tr>
 <td></td>
 <td colspan="1">Supported Version Ranges</td>
 </tr>
 <tr>
 <td>comment</td>
 <td><code class="docutils literal notranslate">v7.6.0 -> v7.6.0 </code></td>
 </tr>
 </table>
 </div>
 </li>
        <li> <span class="li-head">decrypted_traffic_mirror</span> - Decrypted traffic mirror. Source firewall.decrypted-traffic-mirror.name. <span class="li-normal">type: str</span>
 <a id='label10' href="javascript:ContentClick('label11', 'label10');" onmouseover="ContentPreview('label11');" onmouseout="ContentUnpreview('label11');" title="click to collapse or expand..."> more... </a>
 <div id="label11" style="display:none">
 <table border="1">
 <tr>
 <td></td>
 <td colspan="1">Supported Version Ranges</td>
 </tr>
 <tr>
 <td>decrypted_traffic_mirror</td>
 <td><code class="docutils literal notranslate">v7.6.1 -> 7.6.2 </code></td>
 </tr>
 </table>
 </div>
 </li>
        <li> <span class="li-head">empty_cert_action</span> - Action of an empty client certificate. <span class="li-normal">type: str</span> <span class="li-normal">choices: accept, block, accept-unmanageable</span>
 <a id='label12' href="javascript:ContentClick('label13', 'label12');" onmouseover="ContentPreview('label13');" onmouseout="ContentUnpreview('label13');" title="click to collapse or expand..."> more... </a>
 <div id="label13" style="display:none">
 <table border="1">
 <tr>
 <td></td>
 <td colspan="1">Supported Version Ranges</td>
 </tr>
 <tr>
 <td>empty_cert_action</td>
 <td><code class="docutils literal notranslate">v7.6.0 -> v7.6.0 </code></td>
 </tr>
 <tr>
 <td>[accept]</td>
 <td><code class="docutils literal notranslate">v7.6.0 -> v7.6.0</code></td>
 <tr>
 <td>[block]</td>
 <td><code class="docutils literal notranslate">v7.6.0 -> v7.6.0</code></td>
 <tr>
 <td>[accept-unmanageable]</td>
 <td><code class="docutils literal notranslate">v7.6.0 -> v7.6.0</code></td>
 </table>
 </div>
 </li>
        <li> <span class="li-head">h3_support</span> - Enable/disable HTTP3/QUIC support . <span class="li-normal">type: str</span> <span class="li-normal">choices: enable, disable</span>
 <a id='label14' href="javascript:ContentClick('label15', 'label14');" onmouseover="ContentPreview('label15');" onmouseout="ContentUnpreview('label15');" title="click to collapse or expand..."> more... </a>
 <div id="label15" style="display:none">
 <table border="1">
 <tr>
 <td></td>
 <td colspan="1">Supported Version Ranges</td>
 </tr>
 <tr>
 <td>h3_support</td>
 <td><code class="docutils literal notranslate">v7.6.0 -> v7.6.0 </code></td>
 </tr>
 <tr>
 <td>[enable]</td>
 <td><code class="docutils literal notranslate">v7.6.0 -> v7.6.0</code></td>
 <tr>
 <td>[disable]</td>
 <td><code class="docutils literal notranslate">v7.6.0 -> v7.6.0</code></td>
 </table>
 </div>
 </li>
        <li> <span class="li-head">host</span> - Virtual or real host name. Source firewall.access-proxy-virtual-host.name. <span class="li-normal">type: str</span>
 <a id='label16' href="javascript:ContentClick('label17', 'label16');" onmouseover="ContentPreview('label17');" onmouseout="ContentUnpreview('label17');" title="click to collapse or expand..."> more... </a>
 <div id="label17" style="display:none">
 <table border="1">
 <tr>
 <td></td>
 <td colspan="1">Supported Version Ranges</td>
 </tr>
 <tr>
 <td>host</td>
 <td><code class="docutils literal notranslate">v7.6.1 -> 7.6.2 </code></td>
 </tr>
 </table>
 </div>
 </li>
        <li> <span class="li-head">interface</span> - interface name Source system.interface.name. <span class="li-normal">type: str</span>
 <a id='label18' href="javascript:ContentClick('label19', 'label18');" onmouseover="ContentPreview('label19');" onmouseout="ContentUnpreview('label19');" title="click to collapse or expand..."> more... </a>
 <div id="label19" style="display:none">
 <table border="1">
 <tr>
 <td></td>
 <td colspan="1">Supported Version Ranges</td>
 </tr>
 <tr>
 <td>interface</td>
 <td><code class="docutils literal notranslate">v7.6.0 -> v7.6.0 </code></td>
 </tr>
 </table>
 </div>
 </li>
        <li> <span class="li-head">log_blocked_traffic</span> - Enable/disable logging of blocked traffic. <span class="li-normal">type: str</span> <span class="li-normal">choices: disable, enable</span>
 <a id='label20' href="javascript:ContentClick('label21', 'label20');" onmouseover="ContentPreview('label21');" onmouseout="ContentUnpreview('label21');" title="click to collapse or expand..."> more... </a>
 <div id="label21" style="display:none">
 <table border="1">
 <tr>
 <td></td>
 <td colspan="1">Supported Version Ranges</td>
 </tr>
 <tr>
 <td>log_blocked_traffic</td>
 <td><code class="docutils literal notranslate">v7.6.0 -> 7.6.2 </code></td>
 </tr>
 <tr>
 <td>[disable]</td>
 <td><code class="docutils literal notranslate">v7.6.0 -> 7.6.2</code></td>
 <tr>
 <td>[enable]</td>
 <td><code class="docutils literal notranslate">v7.6.0 -> 7.6.2</code></td>
 </table>
 </div>
 </li>
        <li> <span class="li-head">name</span> - ZTNA proxy name. <span class="li-normal">type: str</span> <span class="li-required">required: true</span>
 <a id='label22' href="javascript:ContentClick('label23', 'label22');" onmouseover="ContentPreview('label23');" onmouseout="ContentUnpreview('label23');" title="click to collapse or expand..."> more... </a>
 <div id="label23" style="display:none">
 <table border="1">
 <tr>
 <td></td>
 <td colspan="1">Supported Version Ranges</td>
 </tr>
 <tr>
 <td>name</td>
 <td><code class="docutils literal notranslate">v7.6.0 -> 7.6.2 </code></td>
 </tr>
 </table>
 </div>
 </li>
        <li> <span class="li-head">port</span> - Accept incoming traffic on one or more ports (0 - 65535). <span class="li-normal">type: str</span>
 <a id='label24' href="javascript:ContentClick('label25', 'label24');" onmouseover="ContentPreview('label25');" onmouseout="ContentUnpreview('label25');" title="click to collapse or expand..."> more... </a>
 <div id="label25" style="display:none">
 <table border="1">
 <tr>
 <td></td>
 <td colspan="1">Supported Version Ranges</td>
 </tr>
 <tr>
 <td>port</td>
 <td><code class="docutils literal notranslate">v7.6.0 -> v7.6.0 </code></td>
 </tr>
 </table>
 </div>
 </li>
        <li> <span class="li-head">quic</span> - QUIC setting. <span class="li-normal">type: dict</span>
 <a id='label26' href="javascript:ContentClick('label27', 'label26');" onmouseover="ContentPreview('label27');" onmouseout="ContentUnpreview('label27');" title="click to collapse or expand..."> more... </a>
 <div id="label27" style="display:none">
 <table border="1">
 <tr>
 <td></td><td colspan="1">Supported Version Ranges</td>
 </tr>
 <tr>
 <td>quic</td>
 <td><code class="docutils literal notranslate">v7.6.0 -> v7.6.0 </code></td>
 </tr>
 </table>
 </div>
 </li>
            <ul class="ul-self">
            <li> <span class="li-head">ack_delay_exponent</span> - ACK delay exponent (1 - 20). <span class="li-normal">type: int</span>
 <a id='label28' href="javascript:ContentClick('label29', 'label28');" onmouseover="ContentPreview('label29');" onmouseout="ContentUnpreview('label29');" title="click to collapse or expand..."> more... </a>
 <div id="label29" style="display:none">
 <table border="1">
 <tr>
 <td></td>
 <td colspan="1">Supported Version Ranges</td>
 </tr>
 <tr>
 <td>ack_delay_exponent</td>
 <td><code class="docutils literal notranslate">v7.6.0 -> v7.6.0 </code></td>
 </tr>
 </table>
 </div>
 </li>
            <li> <span class="li-head">active_connection_id_limit</span> - Active connection ID limit (1 - 8). <span class="li-normal">type: int</span>
 <a id='label30' href="javascript:ContentClick('label31', 'label30');" onmouseover="ContentPreview('label31');" onmouseout="ContentUnpreview('label31');" title="click to collapse or expand..."> more... </a>
 <div id="label31" style="display:none">
 <table border="1">
 <tr>
 <td></td>
 <td colspan="1">Supported Version Ranges</td>
 </tr>
 <tr>
 <td>active_connection_id_limit</td>
 <td><code class="docutils literal notranslate">v7.6.0 -> v7.6.0 </code></td>
 </tr>
 </table>
 </div>
 </li>
            <li> <span class="li-head">active_migration</span> - Enable/disable active migration . <span class="li-normal">type: str</span> <span class="li-normal">choices: enable, disable</span>
 <a id='label32' href="javascript:ContentClick('label33', 'label32');" onmouseover="ContentPreview('label33');" onmouseout="ContentUnpreview('label33');" title="click to collapse or expand..."> more... </a>
 <div id="label33" style="display:none">
 <table border="1">
 <tr>
 <td></td>
 <td colspan="1">Supported Version Ranges</td>
 </tr>
 <tr>
 <td>active_migration</td>
 <td><code class="docutils literal notranslate">v7.6.0 -> v7.6.0 </code></td>
 </tr>
 <tr>
 <td>[enable]</td>
 <td><code class="docutils literal notranslate">v7.6.0 -> v7.6.0</code></td>
 <tr>
 <td>[disable]</td>
 <td><code class="docutils literal notranslate">v7.6.0 -> v7.6.0</code></td>
 </table>
 </div>
 </li>
            <li> <span class="li-head">grease_quic_bit</span> - Enable/disable grease QUIC bit . <span class="li-normal">type: str</span> <span class="li-normal">choices: enable, disable</span>
 <a id='label34' href="javascript:ContentClick('label35', 'label34');" onmouseover="ContentPreview('label35');" onmouseout="ContentUnpreview('label35');" title="click to collapse or expand..."> more... </a>
 <div id="label35" style="display:none">
 <table border="1">
 <tr>
 <td></td>
 <td colspan="1">Supported Version Ranges</td>
 </tr>
 <tr>
 <td>grease_quic_bit</td>
 <td><code class="docutils literal notranslate">v7.6.0 -> v7.6.0 </code></td>
 </tr>
 <tr>
 <td>[enable]</td>
 <td><code class="docutils literal notranslate">v7.6.0 -> v7.6.0</code></td>
 <tr>
 <td>[disable]</td>
 <td><code class="docutils literal notranslate">v7.6.0 -> v7.6.0</code></td>
 </table>
 </div>
 </li>
            <li> <span class="li-head">max_ack_delay</span> - Maximum ACK delay in milliseconds (1 - 16383). <span class="li-normal">type: int</span>
 <a id='label36' href="javascript:ContentClick('label37', 'label36');" onmouseover="ContentPreview('label37');" onmouseout="ContentUnpreview('label37');" title="click to collapse or expand..."> more... </a>
 <div id="label37" style="display:none">
 <table border="1">
 <tr>
 <td></td>
 <td colspan="1">Supported Version Ranges</td>
 </tr>
 <tr>
 <td>max_ack_delay</td>
 <td><code class="docutils literal notranslate">v7.6.0 -> v7.6.0 </code></td>
 </tr>
 </table>
 </div>
 </li>
            <li> <span class="li-head">max_datagram_frame_size</span> - Maximum datagram frame size in bytes (1 - 1500). <span class="li-normal">type: int</span>
 <a id='label38' href="javascript:ContentClick('label39', 'label38');" onmouseover="ContentPreview('label39');" onmouseout="ContentUnpreview('label39');" title="click to collapse or expand..."> more... </a>
 <div id="label39" style="display:none">
 <table border="1">
 <tr>
 <td></td>
 <td colspan="1">Supported Version Ranges</td>
 </tr>
 <tr>
 <td>max_datagram_frame_size</td>
 <td><code class="docutils literal notranslate">v7.6.0 -> v7.6.0 </code></td>
 </tr>
 </table>
 </div>
 </li>
            <li> <span class="li-head">max_idle_timeout</span> - Maximum idle timeout milliseconds (1 - 60000). <span class="li-normal">type: int</span>
 <a id='label40' href="javascript:ContentClick('label41', 'label40');" onmouseover="ContentPreview('label41');" onmouseout="ContentUnpreview('label41');" title="click to collapse or expand..."> more... </a>
 <div id="label41" style="display:none">
 <table border="1">
 <tr>
 <td></td>
 <td colspan="1">Supported Version Ranges</td>
 </tr>
 <tr>
 <td>max_idle_timeout</td>
 <td><code class="docutils literal notranslate">v7.6.0 -> v7.6.0 </code></td>
 </tr>
 </table>
 </div>
 </li>
            <li> <span class="li-head">max_udp_payload_size</span> - Maximum UDP payload size in bytes (1200 - 1500). <span class="li-normal">type: int</span>
 <a id='label42' href="javascript:ContentClick('label43', 'label42');" onmouseover="ContentPreview('label43');" onmouseout="ContentUnpreview('label43');" title="click to collapse or expand..."> more... </a>
 <div id="label43" style="display:none">
 <table border="1">
 <tr>
 <td></td>
 <td colspan="1">Supported Version Ranges</td>
 </tr>
 <tr>
 <td>max_udp_payload_size</td>
 <td><code class="docutils literal notranslate">v7.6.0 -> v7.6.0 </code></td>
 </tr>
 </table>
 </div>
 </li>
            </ul>
        <li> <span class="li-head">ssl_accept_ffdhe_groups</span> - Enable/disable FFDHE cipher suite for SSL key exchange. <span class="li-normal">type: str</span> <span class="li-normal">choices: enable, disable</span>
 <a id='label44' href="javascript:ContentClick('label45', 'label44');" onmouseover="ContentPreview('label45');" onmouseout="ContentUnpreview('label45');" title="click to collapse or expand..."> more... </a>
 <div id="label45" style="display:none">
 <table border="1">
 <tr>
 <td></td>
 <td colspan="1">Supported Version Ranges</td>
 </tr>
 <tr>
 <td>ssl_accept_ffdhe_groups</td>
 <td><code class="docutils literal notranslate">v7.6.0 -> v7.6.0 </code></td>
 </tr>
 <tr>
 <td>[enable]</td>
 <td><code class="docutils literal notranslate">v7.6.0 -> v7.6.0</code></td>
 <tr>
 <td>[disable]</td>
 <td><code class="docutils literal notranslate">v7.6.0 -> v7.6.0</code></td>
 </table>
 </div>
 </li>
        <li> <span class="li-head">ssl_algorithm</span> - Permitted encryption algorithms for SSL sessions according to encryption strength. <span class="li-normal">type: str</span> <span class="li-normal">choices: high, medium, low, custom</span>
 <a id='label46' href="javascript:ContentClick('label47', 'label46');" onmouseover="ContentPreview('label47');" onmouseout="ContentUnpreview('label47');" title="click to collapse or expand..."> more... </a>
 <div id="label47" style="display:none">
 <table border="1">
 <tr>
 <td></td>
 <td colspan="1">Supported Version Ranges</td>
 </tr>
 <tr>
 <td>ssl_algorithm</td>
 <td><code class="docutils literal notranslate">v7.6.0 -> v7.6.0 </code></td>
 </tr>
 <tr>
 <td>[high]</td>
 <td><code class="docutils literal notranslate">v7.6.0 -> v7.6.0</code></td>
 <tr>
 <td>[medium]</td>
 <td><code class="docutils literal notranslate">v7.6.0 -> v7.6.0</code></td>
 <tr>
 <td>[low]</td>
 <td><code class="docutils literal notranslate">v7.6.0 -> v7.6.0</code></td>
 <tr>
 <td>[custom]</td>
 <td><code class="docutils literal notranslate">v7.6.0 -> v7.6.0</code></td>
 </table>
 </div>
 </li>
        <li> <span class="li-head">ssl_certificate</span> - Name of the certificate to use for SSL handshake. <span class="li-normal">type: list</span> <span style="font-family:'Courier New'" class="li-required">member_path: ssl_certificate:name</span>
 <a id='label48' href="javascript:ContentClick('label49', 'label48');" onmouseover="ContentPreview('label49');" onmouseout="ContentUnpreview('label49');" title="click to collapse or expand..."> more... </a>
 <div id="label49" style="display:none">
 <table border="1">
 <tr>
 <td></td><td colspan="1">Supported Version Ranges</td>
 </tr>
 <tr>
 <td>ssl_certificate</td>
 <td><code class="docutils literal notranslate">v7.6.0 -> v7.6.0 </code></td>
 </tr>
 </table>
 </div>
 </li>
            <ul class="ul-self">
            <li> <span class="li-head">name</span> - Certificate list. Source vpn.certificate.local.name. <span class="li-normal">type: str</span> <span class="li-required">required: true</span>
 <a id='label50' href="javascript:ContentClick('label51', 'label50');" onmouseover="ContentPreview('label51');" onmouseout="ContentUnpreview('label51');" title="click to collapse or expand..."> more... </a>
 <div id="label51" style="display:none">
 <table border="1">
 <tr>
 <td></td>
 <td colspan="1">Supported Version Ranges</td>
 </tr>
 <tr>
 <td>name</td>
 <td><code class="docutils literal notranslate">v7.6.0 -> v7.6.0 </code></td>
 </tr>
 </table>
 </div>
 </li>
            </ul>
        <li> <span class="li-head">ssl_cipher_suites</span> - SSL/TLS cipher suites acceptable from a client, ordered by priority. <span class="li-normal">type: list</span> <span style="font-family:'Courier New'" class="li-required">member_path: ssl_cipher_suites:priority</span>
 <a id='label52' href="javascript:ContentClick('label53', 'label52');" onmouseover="ContentPreview('label53');" onmouseout="ContentUnpreview('label53');" title="click to collapse or expand..."> more... </a>
 <div id="label53" style="display:none">
 <table border="1">
 <tr>
 <td></td><td colspan="1">Supported Version Ranges</td>
 </tr>
 <tr>
 <td>ssl_cipher_suites</td>
 <td><code class="docutils literal notranslate">v7.6.0 -> v7.6.0 </code></td>
 </tr>
 </table>
 </div>
 </li>
            <ul class="ul-self">
            <li> <span class="li-head">cipher</span> - Cipher suite name. <span class="li-normal">type: str</span> <span class="li-normal">choices: TLS-AES-128-GCM-SHA256, TLS-AES-256-GCM-SHA384, TLS-CHACHA20-POLY1305-SHA256, TLS-ECDHE-RSA-WITH-CHACHA20-POLY1305-SHA256, TLS-ECDHE-ECDSA-WITH-CHACHA20-POLY1305-SHA256, TLS-DHE-RSA-WITH-CHACHA20-POLY1305-SHA256, TLS-DHE-RSA-WITH-AES-128-CBC-SHA, TLS-DHE-RSA-WITH-AES-256-CBC-SHA, TLS-DHE-RSA-WITH-AES-128-CBC-SHA256, TLS-DHE-RSA-WITH-AES-128-GCM-SHA256, TLS-DHE-RSA-WITH-AES-256-CBC-SHA256, TLS-DHE-RSA-WITH-AES-256-GCM-SHA384, TLS-DHE-DSS-WITH-AES-128-CBC-SHA, TLS-DHE-DSS-WITH-AES-256-CBC-SHA, TLS-DHE-DSS-WITH-AES-128-CBC-SHA256, TLS-DHE-DSS-WITH-AES-128-GCM-SHA256, TLS-DHE-DSS-WITH-AES-256-CBC-SHA256, TLS-DHE-DSS-WITH-AES-256-GCM-SHA384, TLS-ECDHE-RSA-WITH-AES-128-CBC-SHA, TLS-ECDHE-RSA-WITH-AES-128-CBC-SHA256, TLS-ECDHE-RSA-WITH-AES-128-GCM-SHA256, TLS-ECDHE-RSA-WITH-AES-256-CBC-SHA, TLS-ECDHE-RSA-WITH-AES-256-CBC-SHA384, TLS-ECDHE-RSA-WITH-AES-256-GCM-SHA384, TLS-ECDHE-ECDSA-WITH-AES-128-CBC-SHA, TLS-ECDHE-ECDSA-WITH-AES-128-CBC-SHA256, TLS-ECDHE-ECDSA-WITH-AES-128-GCM-SHA256, TLS-ECDHE-ECDSA-WITH-AES-256-CBC-SHA, TLS-ECDHE-ECDSA-WITH-AES-256-CBC-SHA384, TLS-ECDHE-ECDSA-WITH-AES-256-GCM-SHA384, TLS-RSA-WITH-AES-128-CBC-SHA, TLS-RSA-WITH-AES-256-CBC-SHA, TLS-RSA-WITH-AES-128-CBC-SHA256, TLS-RSA-WITH-AES-128-GCM-SHA256, TLS-RSA-WITH-AES-256-CBC-SHA256, TLS-RSA-WITH-AES-256-GCM-SHA384, TLS-RSA-WITH-CAMELLIA-128-CBC-SHA, TLS-RSA-WITH-CAMELLIA-256-CBC-SHA, TLS-RSA-WITH-CAMELLIA-128-CBC-SHA256, TLS-RSA-WITH-CAMELLIA-256-CBC-SHA256, TLS-DHE-RSA-WITH-3DES-EDE-CBC-SHA, TLS-DHE-RSA-WITH-CAMELLIA-128-CBC-SHA, TLS-DHE-DSS-WITH-CAMELLIA-128-CBC-SHA, TLS-DHE-RSA-WITH-CAMELLIA-256-CBC-SHA, TLS-DHE-DSS-WITH-CAMELLIA-256-CBC-SHA, TLS-DHE-RSA-WITH-CAMELLIA-128-CBC-SHA256, TLS-DHE-DSS-WITH-CAMELLIA-128-CBC-SHA256, TLS-DHE-RSA-WITH-CAMELLIA-256-CBC-SHA256, TLS-DHE-DSS-WITH-CAMELLIA-256-CBC-SHA256, TLS-DHE-RSA-WITH-SEED-CBC-SHA, TLS-DHE-DSS-WITH-SEED-CBC-SHA, TLS-DHE-RSA-WITH-ARIA-128-CBC-SHA256, TLS-DHE-RSA-WITH-ARIA-256-CBC-SHA384, TLS-DHE-DSS-WITH-ARIA-128-CBC-SHA256, TLS-DHE-DSS-WITH-ARIA-256-CBC-SHA384, TLS-RSA-WITH-SEED-CBC-SHA, TLS-RSA-WITH-ARIA-128-CBC-SHA256, TLS-RSA-WITH-ARIA-256-CBC-SHA384, TLS-ECDHE-RSA-WITH-ARIA-128-CBC-SHA256, TLS-ECDHE-RSA-WITH-ARIA-256-CBC-SHA384, TLS-ECDHE-ECDSA-WITH-ARIA-128-CBC-SHA256, TLS-ECDHE-ECDSA-WITH-ARIA-256-CBC-SHA384, TLS-ECDHE-RSA-WITH-RC4-128-SHA, TLS-ECDHE-RSA-WITH-3DES-EDE-CBC-SHA, TLS-DHE-DSS-WITH-3DES-EDE-CBC-SHA, TLS-RSA-WITH-3DES-EDE-CBC-SHA, TLS-RSA-WITH-RC4-128-MD5, TLS-RSA-WITH-RC4-128-SHA, TLS-DHE-RSA-WITH-DES-CBC-SHA, TLS-DHE-DSS-WITH-DES-CBC-SHA, TLS-RSA-WITH-DES-CBC-SHA</span>
 <a id='label54' href="javascript:ContentClick('label55', 'label54');" onmouseover="ContentPreview('label55');" onmouseout="ContentUnpreview('label55');" title="click to collapse or expand..."> more... </a>
 <div id="label55" style="display:none">
 <table border="1">
 <tr>
 <td></td>
 <td colspan="1">Supported Version Ranges</td>
 </tr>
 <tr>
 <td>cipher</td>
 <td><code class="docutils literal notranslate">v7.6.0 -> v7.6.0 </code></td>
 </tr>
 <tr>
 <td>[TLS-AES-128-GCM-SHA256]</td>
 <td><code class="docutils literal notranslate">v7.6.0 -> v7.6.0</code></td>
 <tr>
 <td>[TLS-AES-256-GCM-SHA384]</td>
 <td><code class="docutils literal notranslate">v7.6.0 -> v7.6.0</code></td>
 <tr>
 <td>[TLS-CHACHA20-POLY1305-SHA256]</td>
 <td><code class="docutils literal notranslate">v7.6.0 -> v7.6.0</code></td>
 <tr>
 <td>[TLS-ECDHE-RSA-WITH-CHACHA20-POLY1305-SHA256]</td>
 <td><code class="docutils literal notranslate">v7.6.0 -> v7.6.0</code></td>
 <tr>
 <td>[TLS-ECDHE-ECDSA-WITH-CHACHA20-POLY1305-SHA256]</td>
 <td><code class="docutils literal notranslate">v7.6.0 -> v7.6.0</code></td>
 <tr>
 <td>[TLS-DHE-RSA-WITH-CHACHA20-POLY1305-SHA256]</td>
 <td><code class="docutils literal notranslate">v7.6.0 -> v7.6.0</code></td>
 <tr>
 <td>[TLS-DHE-RSA-WITH-AES-128-CBC-SHA]</td>
 <td><code class="docutils literal notranslate">v7.6.0 -> v7.6.0</code></td>
 <tr>
 <td>[TLS-DHE-RSA-WITH-AES-256-CBC-SHA]</td>
 <td><code class="docutils literal notranslate">v7.6.0 -> v7.6.0</code></td>
 <tr>
 <td>[TLS-DHE-RSA-WITH-AES-128-CBC-SHA256]</td>
 <td><code class="docutils literal notranslate">v7.6.0 -> v7.6.0</code></td>
 <tr>
 <td>[TLS-DHE-RSA-WITH-AES-128-GCM-SHA256]</td>
 <td><code class="docutils literal notranslate">v7.6.0 -> v7.6.0</code></td>
 <tr>
 <td>[TLS-DHE-RSA-WITH-AES-256-CBC-SHA256]</td>
 <td><code class="docutils literal notranslate">v7.6.0 -> v7.6.0</code></td>
 <tr>
 <td>[TLS-DHE-RSA-WITH-AES-256-GCM-SHA384]</td>
 <td><code class="docutils literal notranslate">v7.6.0 -> v7.6.0</code></td>
 <tr>
 <td>[TLS-DHE-DSS-WITH-AES-128-CBC-SHA]</td>
 <td><code class="docutils literal notranslate">v7.6.0 -> v7.6.0</code></td>
 <tr>
 <td>[TLS-DHE-DSS-WITH-AES-256-CBC-SHA]</td>
 <td><code class="docutils literal notranslate">v7.6.0 -> v7.6.0</code></td>
 <tr>
 <td>[TLS-DHE-DSS-WITH-AES-128-CBC-SHA256]</td>
 <td><code class="docutils literal notranslate">v7.6.0 -> v7.6.0</code></td>
 <tr>
 <td>[TLS-DHE-DSS-WITH-AES-128-GCM-SHA256]</td>
 <td><code class="docutils literal notranslate">v7.6.0 -> v7.6.0</code></td>
 <tr>
 <td>[TLS-DHE-DSS-WITH-AES-256-CBC-SHA256]</td>
 <td><code class="docutils literal notranslate">v7.6.0 -> v7.6.0</code></td>
 <tr>
 <td>[TLS-DHE-DSS-WITH-AES-256-GCM-SHA384]</td>
 <td><code class="docutils literal notranslate">v7.6.0 -> v7.6.0</code></td>
 <tr>
 <td>[TLS-ECDHE-RSA-WITH-AES-128-CBC-SHA]</td>
 <td><code class="docutils literal notranslate">v7.6.0 -> v7.6.0</code></td>
 <tr>
 <td>[TLS-ECDHE-RSA-WITH-AES-128-CBC-SHA256]</td>
 <td><code class="docutils literal notranslate">v7.6.0 -> v7.6.0</code></td>
 <tr>
 <td>[TLS-ECDHE-RSA-WITH-AES-128-GCM-SHA256]</td>
 <td><code class="docutils literal notranslate">v7.6.0 -> v7.6.0</code></td>
 <tr>
 <td>[TLS-ECDHE-RSA-WITH-AES-256-CBC-SHA]</td>
 <td><code class="docutils literal notranslate">v7.6.0 -> v7.6.0</code></td>
 <tr>
 <td>[TLS-ECDHE-RSA-WITH-AES-256-CBC-SHA384]</td>
 <td><code class="docutils literal notranslate">v7.6.0 -> v7.6.0</code></td>
 <tr>
 <td>[TLS-ECDHE-RSA-WITH-AES-256-GCM-SHA384]</td>
 <td><code class="docutils literal notranslate">v7.6.0 -> v7.6.0</code></td>
 <tr>
 <td>[TLS-ECDHE-ECDSA-WITH-AES-128-CBC-SHA]</td>
 <td><code class="docutils literal notranslate">v7.6.0 -> v7.6.0</code></td>
 <tr>
 <td>[TLS-ECDHE-ECDSA-WITH-AES-128-CBC-SHA256]</td>
 <td><code class="docutils literal notranslate">v7.6.0 -> v7.6.0</code></td>
 <tr>
 <td>[TLS-ECDHE-ECDSA-WITH-AES-128-GCM-SHA256]</td>
 <td><code class="docutils literal notranslate">v7.6.0 -> v7.6.0</code></td>
 <tr>
 <td>[TLS-ECDHE-ECDSA-WITH-AES-256-CBC-SHA]</td>
 <td><code class="docutils literal notranslate">v7.6.0 -> v7.6.0</code></td>
 <tr>
 <td>[TLS-ECDHE-ECDSA-WITH-AES-256-CBC-SHA384]</td>
 <td><code class="docutils literal notranslate">v7.6.0 -> v7.6.0</code></td>
 <tr>
 <td>[TLS-ECDHE-ECDSA-WITH-AES-256-GCM-SHA384]</td>
 <td><code class="docutils literal notranslate">v7.6.0 -> v7.6.0</code></td>
 <tr>
 <td>[TLS-RSA-WITH-AES-128-CBC-SHA]</td>
 <td><code class="docutils literal notranslate">v7.6.0 -> v7.6.0</code></td>
 <tr>
 <td>[TLS-RSA-WITH-AES-256-CBC-SHA]</td>
 <td><code class="docutils literal notranslate">v7.6.0 -> v7.6.0</code></td>
 <tr>
 <td>[TLS-RSA-WITH-AES-128-CBC-SHA256]</td>
 <td><code class="docutils literal notranslate">v7.6.0 -> v7.6.0</code></td>
 <tr>
 <td>[TLS-RSA-WITH-AES-128-GCM-SHA256]</td>
 <td><code class="docutils literal notranslate">v7.6.0 -> v7.6.0</code></td>
 <tr>
 <td>[TLS-RSA-WITH-AES-256-CBC-SHA256]</td>
 <td><code class="docutils literal notranslate">v7.6.0 -> v7.6.0</code></td>
 <tr>
 <td>[TLS-RSA-WITH-AES-256-GCM-SHA384]</td>
 <td><code class="docutils literal notranslate">v7.6.0 -> v7.6.0</code></td>
 <tr>
 <td>[TLS-RSA-WITH-CAMELLIA-128-CBC-SHA]</td>
 <td><code class="docutils literal notranslate">v7.6.0 -> v7.6.0</code></td>
 <tr>
 <td>[TLS-RSA-WITH-CAMELLIA-256-CBC-SHA]</td>
 <td><code class="docutils literal notranslate">v7.6.0 -> v7.6.0</code></td>
 <tr>
 <td>[TLS-RSA-WITH-CAMELLIA-128-CBC-SHA256]</td>
 <td><code class="docutils literal notranslate">v7.6.0 -> v7.6.0</code></td>
 <tr>
 <td>[TLS-RSA-WITH-CAMELLIA-256-CBC-SHA256]</td>
 <td><code class="docutils literal notranslate">v7.6.0 -> v7.6.0</code></td>
 <tr>
 <td>[TLS-DHE-RSA-WITH-3DES-EDE-CBC-SHA]</td>
 <td><code class="docutils literal notranslate">v7.6.0 -> v7.6.0</code></td>
 <tr>
 <td>[TLS-DHE-RSA-WITH-CAMELLIA-128-CBC-SHA]</td>
 <td><code class="docutils literal notranslate">v7.6.0 -> v7.6.0</code></td>
 <tr>
 <td>[TLS-DHE-DSS-WITH-CAMELLIA-128-CBC-SHA]</td>
 <td><code class="docutils literal notranslate">v7.6.0 -> v7.6.0</code></td>
 <tr>
 <td>[TLS-DHE-RSA-WITH-CAMELLIA-256-CBC-SHA]</td>
 <td><code class="docutils literal notranslate">v7.6.0 -> v7.6.0</code></td>
 <tr>
 <td>[TLS-DHE-DSS-WITH-CAMELLIA-256-CBC-SHA]</td>
 <td><code class="docutils literal notranslate">v7.6.0 -> v7.6.0</code></td>
 <tr>
 <td>[TLS-DHE-RSA-WITH-CAMELLIA-128-CBC-SHA256]</td>
 <td><code class="docutils literal notranslate">v7.6.0 -> v7.6.0</code></td>
 <tr>
 <td>[TLS-DHE-DSS-WITH-CAMELLIA-128-CBC-SHA256]</td>
 <td><code class="docutils literal notranslate">v7.6.0 -> v7.6.0</code></td>
 <tr>
 <td>[TLS-DHE-RSA-WITH-CAMELLIA-256-CBC-SHA256]</td>
 <td><code class="docutils literal notranslate">v7.6.0 -> v7.6.0</code></td>
 <tr>
 <td>[TLS-DHE-DSS-WITH-CAMELLIA-256-CBC-SHA256]</td>
 <td><code class="docutils literal notranslate">v7.6.0 -> v7.6.0</code></td>
 <tr>
 <td>[TLS-DHE-RSA-WITH-SEED-CBC-SHA]</td>
 <td><code class="docutils literal notranslate">v7.6.0 -> v7.6.0</code></td>
 <tr>
 <td>[TLS-DHE-DSS-WITH-SEED-CBC-SHA]</td>
 <td><code class="docutils literal notranslate">v7.6.0 -> v7.6.0</code></td>
 <tr>
 <td>[TLS-DHE-RSA-WITH-ARIA-128-CBC-SHA256]</td>
 <td><code class="docutils literal notranslate">v7.6.0 -> v7.6.0</code></td>
 <tr>
 <td>[TLS-DHE-RSA-WITH-ARIA-256-CBC-SHA384]</td>
 <td><code class="docutils literal notranslate">v7.6.0 -> v7.6.0</code></td>
 <tr>
 <td>[TLS-DHE-DSS-WITH-ARIA-128-CBC-SHA256]</td>
 <td><code class="docutils literal notranslate">v7.6.0 -> v7.6.0</code></td>
 <tr>
 <td>[TLS-DHE-DSS-WITH-ARIA-256-CBC-SHA384]</td>
 <td><code class="docutils literal notranslate">v7.6.0 -> v7.6.0</code></td>
 <tr>
 <td>[TLS-RSA-WITH-SEED-CBC-SHA]</td>
 <td><code class="docutils literal notranslate">v7.6.0 -> v7.6.0</code></td>
 <tr>
 <td>[TLS-RSA-WITH-ARIA-128-CBC-SHA256]</td>
 <td><code class="docutils literal notranslate">v7.6.0 -> v7.6.0</code></td>
 <tr>
 <td>[TLS-RSA-WITH-ARIA-256-CBC-SHA384]</td>
 <td><code class="docutils literal notranslate">v7.6.0 -> v7.6.0</code></td>
 <tr>
 <td>[TLS-ECDHE-RSA-WITH-ARIA-128-CBC-SHA256]</td>
 <td><code class="docutils literal notranslate">v7.6.0 -> v7.6.0</code></td>
 <tr>
 <td>[TLS-ECDHE-RSA-WITH-ARIA-256-CBC-SHA384]</td>
 <td><code class="docutils literal notranslate">v7.6.0 -> v7.6.0</code></td>
 <tr>
 <td>[TLS-ECDHE-ECDSA-WITH-ARIA-128-CBC-SHA256]</td>
 <td><code class="docutils literal notranslate">v7.6.0 -> v7.6.0</code></td>
 <tr>
 <td>[TLS-ECDHE-ECDSA-WITH-ARIA-256-CBC-SHA384]</td>
 <td><code class="docutils literal notranslate">v7.6.0 -> v7.6.0</code></td>
 <tr>
 <td>[TLS-ECDHE-RSA-WITH-RC4-128-SHA]</td>
 <td><code class="docutils literal notranslate">v7.6.0 -> v7.6.0</code></td>
 <tr>
 <td>[TLS-ECDHE-RSA-WITH-3DES-EDE-CBC-SHA]</td>
 <td><code class="docutils literal notranslate">v7.6.0 -> v7.6.0</code></td>
 <tr>
 <td>[TLS-DHE-DSS-WITH-3DES-EDE-CBC-SHA]</td>
 <td><code class="docutils literal notranslate">v7.6.0 -> v7.6.0</code></td>
 <tr>
 <td>[TLS-RSA-WITH-3DES-EDE-CBC-SHA]</td>
 <td><code class="docutils literal notranslate">v7.6.0 -> v7.6.0</code></td>
 <tr>
 <td>[TLS-RSA-WITH-RC4-128-MD5]</td>
 <td><code class="docutils literal notranslate">v7.6.0 -> v7.6.0</code></td>
 <tr>
 <td>[TLS-RSA-WITH-RC4-128-SHA]</td>
 <td><code class="docutils literal notranslate">v7.6.0 -> v7.6.0</code></td>
 <tr>
 <td>[TLS-DHE-RSA-WITH-DES-CBC-SHA]</td>
 <td><code class="docutils literal notranslate">v7.6.0 -> v7.6.0</code></td>
 <tr>
 <td>[TLS-DHE-DSS-WITH-DES-CBC-SHA]</td>
 <td><code class="docutils literal notranslate">v7.6.0 -> v7.6.0</code></td>
 <tr>
 <td>[TLS-RSA-WITH-DES-CBC-SHA]</td>
 <td><code class="docutils literal notranslate">v7.6.0 -> v7.6.0</code></td>
 </table>
 </div>
 </li>
            <li> <span class="li-head">priority</span> - SSL/TLS cipher suites priority. see <a href='#notes'>Notes</a>. <span class="li-normal">type: int</span> <span class="li-required">required: true</span>
 <a id='label56' href="javascript:ContentClick('label57', 'label56');" onmouseover="ContentPreview('label57');" onmouseout="ContentUnpreview('label57');" title="click to collapse or expand..."> more... </a>
 <div id="label57" style="display:none">
 <table border="1">
 <tr>
 <td></td>
 <td colspan="1">Supported Version Ranges</td>
 </tr>
 <tr>
 <td>priority</td>
 <td><code class="docutils literal notranslate">v7.6.0 -> v7.6.0 </code></td>
 </tr>
 </table>
 </div>
 </li>
            <li> <span class="li-head">versions</span> - SSL/TLS versions that the cipher suite can be used with. <span class="li-normal">type: list</span> <span class="li-normal">choices: ssl-3.0, tls-1.0, tls-1.1, tls-1.2, tls-1.3</span>
 <a id='label58' href="javascript:ContentClick('label59', 'label58');" onmouseover="ContentPreview('label59');" onmouseout="ContentUnpreview('label59');" title="click to collapse or expand..."> more... </a>
 <div id="label59" style="display:none">
 <table border="1">
 <tr>
 <td></td>
 <td colspan="1">Supported Version Ranges</td>
 </tr>
 <tr>
 <td>versions</td>
 <td><code class="docutils literal notranslate">v7.6.0 -> v7.6.0 </code></td>
 </tr>
 <tr>
 <td>[ssl-3.0]</td>
 <td><code class="docutils literal notranslate">v7.6.0 -> v7.6.0</code></td>
 <tr>
 <td>[tls-1.0]</td>
 <td><code class="docutils literal notranslate">v7.6.0 -> v7.6.0</code></td>
 <tr>
 <td>[tls-1.1]</td>
 <td><code class="docutils literal notranslate">v7.6.0 -> v7.6.0</code></td>
 <tr>
 <td>[tls-1.2]</td>
 <td><code class="docutils literal notranslate">v7.6.0 -> v7.6.0</code></td>
 <tr>
 <td>[tls-1.3]</td>
 <td><code class="docutils literal notranslate">v7.6.0 -> v7.6.0</code></td>
 </table>
 </div>
 </li>
            </ul>
        <li> <span class="li-head">ssl_client_fallback</span> - Enable/disable support for preventing Downgrade Attacks on client connections (RFC 7507). <span class="li-normal">type: str</span> <span class="li-normal">choices: disable, enable</span>
 <a id='label60' href="javascript:ContentClick('label61', 'label60');" onmouseover="ContentPreview('label61');" onmouseout="ContentUnpreview('label61');" title="click to collapse or expand..."> more... </a>
 <div id="label61" style="display:none">
 <table border="1">
 <tr>
 <td></td>
 <td colspan="1">Supported Version Ranges</td>
 </tr>
 <tr>
 <td>ssl_client_fallback</td>
 <td><code class="docutils literal notranslate">v7.6.0 -> v7.6.0 </code></td>
 </tr>
 <tr>
 <td>[disable]</td>
 <td><code class="docutils literal notranslate">v7.6.0 -> v7.6.0</code></td>
 <tr>
 <td>[enable]</td>
 <td><code class="docutils literal notranslate">v7.6.0 -> v7.6.0</code></td>
 </table>
 </div>
 </li>
        <li> <span class="li-head">ssl_client_rekey_count</span> - Maximum length of data in MB before triggering a client rekey (0 = disable). <span class="li-normal">type: int</span>
 <a id='label62' href="javascript:ContentClick('label63', 'label62');" onmouseover="ContentPreview('label63');" onmouseout="ContentUnpreview('label63');" title="click to collapse or expand..."> more... </a>
 <div id="label63" style="display:none">
 <table border="1">
 <tr>
 <td></td>
 <td colspan="1">Supported Version Ranges</td>
 </tr>
 <tr>
 <td>ssl_client_rekey_count</td>
 <td><code class="docutils literal notranslate">v7.6.0 -> v7.6.0 </code></td>
 </tr>
 </table>
 </div>
 </li>
        <li> <span class="li-head">ssl_client_renegotiation</span> - Allow, deny, or require secure renegotiation of client sessions to comply with RFC 5746. <span class="li-normal">type: str</span> <span class="li-normal">choices: allow, deny, secure</span>
 <a id='label64' href="javascript:ContentClick('label65', 'label64');" onmouseover="ContentPreview('label65');" onmouseout="ContentUnpreview('label65');" title="click to collapse or expand..."> more... </a>
 <div id="label65" style="display:none">
 <table border="1">
 <tr>
 <td></td>
 <td colspan="1">Supported Version Ranges</td>
 </tr>
 <tr>
 <td>ssl_client_renegotiation</td>
 <td><code class="docutils literal notranslate">v7.6.0 -> v7.6.0 </code></td>
 </tr>
 <tr>
 <td>[allow]</td>
 <td><code class="docutils literal notranslate">v7.6.0 -> v7.6.0</code></td>
 <tr>
 <td>[deny]</td>
 <td><code class="docutils literal notranslate">v7.6.0 -> v7.6.0</code></td>
 <tr>
 <td>[secure]</td>
 <td><code class="docutils literal notranslate">v7.6.0 -> v7.6.0</code></td>
 </table>
 </div>
 </li>
        <li> <span class="li-head">ssl_client_session_state_max</span> - Maximum number of client to FortiProxy SSL session states to keep. <span class="li-normal">type: int</span>
 <a id='label66' href="javascript:ContentClick('label67', 'label66');" onmouseover="ContentPreview('label67');" onmouseout="ContentUnpreview('label67');" title="click to collapse or expand..."> more... </a>
 <div id="label67" style="display:none">
 <table border="1">
 <tr>
 <td></td>
 <td colspan="1">Supported Version Ranges</td>
 </tr>
 <tr>
 <td>ssl_client_session_state_max</td>
 <td><code class="docutils literal notranslate">v7.6.0 -> v7.6.0 </code></td>
 </tr>
 </table>
 </div>
 </li>
        <li> <span class="li-head">ssl_client_session_state_timeout</span> - Number of minutes to keep client to FortiProxy SSL session state. <span class="li-normal">type: int</span>
 <a id='label68' href="javascript:ContentClick('label69', 'label68');" onmouseover="ContentPreview('label69');" onmouseout="ContentUnpreview('label69');" title="click to collapse or expand..."> more... </a>
 <div id="label69" style="display:none">
 <table border="1">
 <tr>
 <td></td>
 <td colspan="1">Supported Version Ranges</td>
 </tr>
 <tr>
 <td>ssl_client_session_state_timeout</td>
 <td><code class="docutils literal notranslate">v7.6.0 -> v7.6.0 </code></td>
 </tr>
 </table>
 </div>
 </li>
        <li> <span class="li-head">ssl_client_session_state_type</span> - How to expire SSL sessions for the segment of the SSL connection between the client and the FortiGate. <span class="li-normal">type: str</span> <span class="li-normal">choices: disable, time, count, both</span>
 <a id='label70' href="javascript:ContentClick('label71', 'label70');" onmouseover="ContentPreview('label71');" onmouseout="ContentUnpreview('label71');" title="click to collapse or expand..."> more... </a>
 <div id="label71" style="display:none">
 <table border="1">
 <tr>
 <td></td>
 <td colspan="1">Supported Version Ranges</td>
 </tr>
 <tr>
 <td>ssl_client_session_state_type</td>
 <td><code class="docutils literal notranslate">v7.6.0 -> v7.6.0 </code></td>
 </tr>
 <tr>
 <td>[disable]</td>
 <td><code class="docutils literal notranslate">v7.6.0 -> v7.6.0</code></td>
 <tr>
 <td>[time]</td>
 <td><code class="docutils literal notranslate">v7.6.0 -> v7.6.0</code></td>
 <tr>
 <td>[count]</td>
 <td><code class="docutils literal notranslate">v7.6.0 -> v7.6.0</code></td>
 <tr>
 <td>[both]</td>
 <td><code class="docutils literal notranslate">v7.6.0 -> v7.6.0</code></td>
 </table>
 </div>
 </li>
        <li> <span class="li-head">ssl_dh_bits</span> - Bit-size of Diffie-Hellman (DH) prime used in DHE-RSA negotiation . <span class="li-normal">type: str</span> <span class="li-normal">choices: 768, 1024, 1536, 2048, 3072, 4096</span>
 <a id='label72' href="javascript:ContentClick('label73', 'label72');" onmouseover="ContentPreview('label73');" onmouseout="ContentUnpreview('label73');" title="click to collapse or expand..."> more... </a>
 <div id="label73" style="display:none">
 <table border="1">
 <tr>
 <td></td>
 <td colspan="1">Supported Version Ranges</td>
 </tr>
 <tr>
 <td>ssl_dh_bits</td>
 <td><code class="docutils literal notranslate">v7.6.0 -> v7.6.0 </code></td>
 </tr>
 <tr>
 <td>[768]</td>
 <td><code class="docutils literal notranslate">v7.6.0 -> v7.6.0</code></td>
 <tr>
 <td>[1024]</td>
 <td><code class="docutils literal notranslate">v7.6.0 -> v7.6.0</code></td>
 <tr>
 <td>[1536]</td>
 <td><code class="docutils literal notranslate">v7.6.0 -> v7.6.0</code></td>
 <tr>
 <td>[2048]</td>
 <td><code class="docutils literal notranslate">v7.6.0 -> v7.6.0</code></td>
 <tr>
 <td>[3072]</td>
 <td><code class="docutils literal notranslate">v7.6.0 -> v7.6.0</code></td>
 <tr>
 <td>[4096]</td>
 <td><code class="docutils literal notranslate">v7.6.0 -> v7.6.0</code></td>
 </table>
 </div>
 </li>
        <li> <span class="li-head">ssl_hpkp</span> - Enable/disable including HPKP header in response. <span class="li-normal">type: str</span> <span class="li-normal">choices: disable, enable, report-only</span>
 <a id='label74' href="javascript:ContentClick('label75', 'label74');" onmouseover="ContentPreview('label75');" onmouseout="ContentUnpreview('label75');" title="click to collapse or expand..."> more... </a>
 <div id="label75" style="display:none">
 <table border="1">
 <tr>
 <td></td>
 <td colspan="1">Supported Version Ranges</td>
 </tr>
 <tr>
 <td>ssl_hpkp</td>
 <td><code class="docutils literal notranslate">v7.6.0 -> v7.6.0 </code></td>
 </tr>
 <tr>
 <td>[disable]</td>
 <td><code class="docutils literal notranslate">v7.6.0 -> v7.6.0</code></td>
 <tr>
 <td>[enable]</td>
 <td><code class="docutils literal notranslate">v7.6.0 -> v7.6.0</code></td>
 <tr>
 <td>[report-only]</td>
 <td><code class="docutils literal notranslate">v7.6.0 -> v7.6.0</code></td>
 </table>
 </div>
 </li>
        <li> <span class="li-head">ssl_hpkp_age</span> - Number of seconds the client should honor the HPKP setting. <span class="li-normal">type: int</span>
 <a id='label76' href="javascript:ContentClick('label77', 'label76');" onmouseover="ContentPreview('label77');" onmouseout="ContentUnpreview('label77');" title="click to collapse or expand..."> more... </a>
 <div id="label77" style="display:none">
 <table border="1">
 <tr>
 <td></td>
 <td colspan="1">Supported Version Ranges</td>
 </tr>
 <tr>
 <td>ssl_hpkp_age</td>
 <td><code class="docutils literal notranslate">v7.6.0 -> v7.6.0 </code></td>
 </tr>
 </table>
 </div>
 </li>
        <li> <span class="li-head">ssl_hpkp_backup</span> - Certificate to generate backup HPKP pin from. Source vpn.certificate.local.name vpn.certificate.ca.name. <span class="li-normal">type: str</span>
 <a id='label78' href="javascript:ContentClick('label79', 'label78');" onmouseover="ContentPreview('label79');" onmouseout="ContentUnpreview('label79');" title="click to collapse or expand..."> more... </a>
 <div id="label79" style="display:none">
 <table border="1">
 <tr>
 <td></td>
 <td colspan="1">Supported Version Ranges</td>
 </tr>
 <tr>
 <td>ssl_hpkp_backup</td>
 <td><code class="docutils literal notranslate">v7.6.0 -> v7.6.0 </code></td>
 </tr>
 </table>
 </div>
 </li>
        <li> <span class="li-head">ssl_hpkp_include_subdomains</span> - Indicate that HPKP header applies to all subdomains. <span class="li-normal">type: str</span> <span class="li-normal">choices: disable, enable</span>
 <a id='label80' href="javascript:ContentClick('label81', 'label80');" onmouseover="ContentPreview('label81');" onmouseout="ContentUnpreview('label81');" title="click to collapse or expand..."> more... </a>
 <div id="label81" style="display:none">
 <table border="1">
 <tr>
 <td></td>
 <td colspan="1">Supported Version Ranges</td>
 </tr>
 <tr>
 <td>ssl_hpkp_include_subdomains</td>
 <td><code class="docutils literal notranslate">v7.6.0 -> v7.6.0 </code></td>
 </tr>
 <tr>
 <td>[disable]</td>
 <td><code class="docutils literal notranslate">v7.6.0 -> v7.6.0</code></td>
 <tr>
 <td>[enable]</td>
 <td><code class="docutils literal notranslate">v7.6.0 -> v7.6.0</code></td>
 </table>
 </div>
 </li>
        <li> <span class="li-head">ssl_hpkp_primary</span> - Certificate to generate primary HPKP pin from. Source vpn.certificate.local.name vpn.certificate.ca.name. <span class="li-normal">type: str</span>
 <a id='label82' href="javascript:ContentClick('label83', 'label82');" onmouseover="ContentPreview('label83');" onmouseout="ContentUnpreview('label83');" title="click to collapse or expand..."> more... </a>
 <div id="label83" style="display:none">
 <table border="1">
 <tr>
 <td></td>
 <td colspan="1">Supported Version Ranges</td>
 </tr>
 <tr>
 <td>ssl_hpkp_primary</td>
 <td><code class="docutils literal notranslate">v7.6.0 -> v7.6.0 </code></td>
 </tr>
 </table>
 </div>
 </li>
        <li> <span class="li-head">ssl_hpkp_report_uri</span> - URL to report HPKP violations to. <span class="li-normal">type: str</span>
 <a id='label84' href="javascript:ContentClick('label85', 'label84');" onmouseover="ContentPreview('label85');" onmouseout="ContentUnpreview('label85');" title="click to collapse or expand..."> more... </a>
 <div id="label85" style="display:none">
 <table border="1">
 <tr>
 <td></td>
 <td colspan="1">Supported Version Ranges</td>
 </tr>
 <tr>
 <td>ssl_hpkp_report_uri</td>
 <td><code class="docutils literal notranslate">v7.6.0 -> v7.6.0 </code></td>
 </tr>
 </table>
 </div>
 </li>
        <li> <span class="li-head">ssl_hsts</span> - Enable/disable including HSTS header in response. <span class="li-normal">type: str</span> <span class="li-normal">choices: disable, enable</span>
 <a id='label86' href="javascript:ContentClick('label87', 'label86');" onmouseover="ContentPreview('label87');" onmouseout="ContentUnpreview('label87');" title="click to collapse or expand..."> more... </a>
 <div id="label87" style="display:none">
 <table border="1">
 <tr>
 <td></td>
 <td colspan="1">Supported Version Ranges</td>
 </tr>
 <tr>
 <td>ssl_hsts</td>
 <td><code class="docutils literal notranslate">v7.6.0 -> v7.6.0 </code></td>
 </tr>
 <tr>
 <td>[disable]</td>
 <td><code class="docutils literal notranslate">v7.6.0 -> v7.6.0</code></td>
 <tr>
 <td>[enable]</td>
 <td><code class="docutils literal notranslate">v7.6.0 -> v7.6.0</code></td>
 </table>
 </div>
 </li>
        <li> <span class="li-head">ssl_hsts_age</span> - Number of seconds the client should honor the HSTS setting. <span class="li-normal">type: int</span>
 <a id='label88' href="javascript:ContentClick('label89', 'label88');" onmouseover="ContentPreview('label89');" onmouseout="ContentUnpreview('label89');" title="click to collapse or expand..."> more... </a>
 <div id="label89" style="display:none">
 <table border="1">
 <tr>
 <td></td>
 <td colspan="1">Supported Version Ranges</td>
 </tr>
 <tr>
 <td>ssl_hsts_age</td>
 <td><code class="docutils literal notranslate">v7.6.0 -> v7.6.0 </code></td>
 </tr>
 </table>
 </div>
 </li>
        <li> <span class="li-head">ssl_hsts_include_subdomains</span> - Indicate that HSTS header applies to all subdomains. <span class="li-normal">type: str</span> <span class="li-normal">choices: disable, enable</span>
 <a id='label90' href="javascript:ContentClick('label91', 'label90');" onmouseover="ContentPreview('label91');" onmouseout="ContentUnpreview('label91');" title="click to collapse or expand..."> more... </a>
 <div id="label91" style="display:none">
 <table border="1">
 <tr>
 <td></td>
 <td colspan="1">Supported Version Ranges</td>
 </tr>
 <tr>
 <td>ssl_hsts_include_subdomains</td>
 <td><code class="docutils literal notranslate">v7.6.0 -> v7.6.0 </code></td>
 </tr>
 <tr>
 <td>[disable]</td>
 <td><code class="docutils literal notranslate">v7.6.0 -> v7.6.0</code></td>
 <tr>
 <td>[enable]</td>
 <td><code class="docutils literal notranslate">v7.6.0 -> v7.6.0</code></td>
 </table>
 </div>
 </li>
        <li> <span class="li-head">ssl_http_location_conversion</span> - Enable to replace HTTP with HTTPS in the reply"s Location HTTP header field. <span class="li-normal">type: str</span> <span class="li-normal">choices: enable, disable</span>
 <a id='label92' href="javascript:ContentClick('label93', 'label92');" onmouseover="ContentPreview('label93');" onmouseout="ContentUnpreview('label93');" title="click to collapse or expand..."> more... </a>
 <div id="label93" style="display:none">
 <table border="1">
 <tr>
 <td></td>
 <td colspan="1">Supported Version Ranges</td>
 </tr>
 <tr>
 <td>ssl_http_location_conversion</td>
 <td><code class="docutils literal notranslate">v7.6.0 -> v7.6.0 </code></td>
 </tr>
 <tr>
 <td>[enable]</td>
 <td><code class="docutils literal notranslate">v7.6.0 -> v7.6.0</code></td>
 <tr>
 <td>[disable]</td>
 <td><code class="docutils literal notranslate">v7.6.0 -> v7.6.0</code></td>
 </table>
 </div>
 </li>
        <li> <span class="li-head">ssl_http_match_host</span> - Enable/disable HTTP host matching for location conversion. <span class="li-normal">type: str</span> <span class="li-normal">choices: enable, disable</span>
 <a id='label94' href="javascript:ContentClick('label95', 'label94');" onmouseover="ContentPreview('label95');" onmouseout="ContentUnpreview('label95');" title="click to collapse or expand..."> more... </a>
 <div id="label95" style="display:none">
 <table border="1">
 <tr>
 <td></td>
 <td colspan="1">Supported Version Ranges</td>
 </tr>
 <tr>
 <td>ssl_http_match_host</td>
 <td><code class="docutils literal notranslate">v7.6.0 -> v7.6.0 </code></td>
 </tr>
 <tr>
 <td>[enable]</td>
 <td><code class="docutils literal notranslate">v7.6.0 -> v7.6.0</code></td>
 <tr>
 <td>[disable]</td>
 <td><code class="docutils literal notranslate">v7.6.0 -> v7.6.0</code></td>
 </table>
 </div>
 </li>
        <li> <span class="li-head">ssl_max_version</span> - Highest SSL/TLS version acceptable from a client. <span class="li-normal">type: str</span> <span class="li-normal">choices: ssl-3.0, tls-1.0, tls-1.1, tls-1.2, tls-1.3</span>
 <a id='label96' href="javascript:ContentClick('label97', 'label96');" onmouseover="ContentPreview('label97');" onmouseout="ContentUnpreview('label97');" title="click to collapse or expand..."> more... </a>
 <div id="label97" style="display:none">
 <table border="1">
 <tr>
 <td></td>
 <td colspan="1">Supported Version Ranges</td>
 </tr>
 <tr>
 <td>ssl_max_version</td>
 <td><code class="docutils literal notranslate">v7.6.0 -> v7.6.0 </code></td>
 </tr>
 <tr>
 <td>[ssl-3.0]</td>
 <td><code class="docutils literal notranslate">v7.6.0 -> v7.6.0</code></td>
 <tr>
 <td>[tls-1.0]</td>
 <td><code class="docutils literal notranslate">v7.6.0 -> v7.6.0</code></td>
 <tr>
 <td>[tls-1.1]</td>
 <td><code class="docutils literal notranslate">v7.6.0 -> v7.6.0</code></td>
 <tr>
 <td>[tls-1.2]</td>
 <td><code class="docutils literal notranslate">v7.6.0 -> v7.6.0</code></td>
 <tr>
 <td>[tls-1.3]</td>
 <td><code class="docutils literal notranslate">v7.6.0 -> v7.6.0</code></td>
 </table>
 </div>
 </li>
        <li> <span class="li-head">ssl_min_version</span> - Lowest SSL/TLS version acceptable from a client. <span class="li-normal">type: str</span> <span class="li-normal">choices: ssl-3.0, tls-1.0, tls-1.1, tls-1.2, tls-1.3</span>
 <a id='label98' href="javascript:ContentClick('label99', 'label98');" onmouseover="ContentPreview('label99');" onmouseout="ContentUnpreview('label99');" title="click to collapse or expand..."> more... </a>
 <div id="label99" style="display:none">
 <table border="1">
 <tr>
 <td></td>
 <td colspan="1">Supported Version Ranges</td>
 </tr>
 <tr>
 <td>ssl_min_version</td>
 <td><code class="docutils literal notranslate">v7.6.0 -> v7.6.0 </code></td>
 </tr>
 <tr>
 <td>[ssl-3.0]</td>
 <td><code class="docutils literal notranslate">v7.6.0 -> v7.6.0</code></td>
 <tr>
 <td>[tls-1.0]</td>
 <td><code class="docutils literal notranslate">v7.6.0 -> v7.6.0</code></td>
 <tr>
 <td>[tls-1.1]</td>
 <td><code class="docutils literal notranslate">v7.6.0 -> v7.6.0</code></td>
 <tr>
 <td>[tls-1.2]</td>
 <td><code class="docutils literal notranslate">v7.6.0 -> v7.6.0</code></td>
 <tr>
 <td>[tls-1.3]</td>
 <td><code class="docutils literal notranslate">v7.6.0 -> v7.6.0</code></td>
 </table>
 </div>
 </li>
        <li> <span class="li-head">ssl_mode</span> - Apply SSL offloading between the client and the FortiGate (half) or from the client to the FortiGate and from the FortiGate to the server (full). <span class="li-normal">type: str</span> <span class="li-normal">choices: half, full</span>
 <a id='label100' href="javascript:ContentClick('label101', 'label100');" onmouseover="ContentPreview('label101');" onmouseout="ContentUnpreview('label101');" title="click to collapse or expand..."> more... </a>
 <div id="label101" style="display:none">
 <table border="1">
 <tr>
 <td></td>
 <td colspan="1">Supported Version Ranges</td>
 </tr>
 <tr>
 <td>ssl_mode</td>
 <td><code class="docutils literal notranslate">v7.6.0 -> v7.6.0 </code></td>
 </tr>
 <tr>
 <td>[half]</td>
 <td><code class="docutils literal notranslate">v7.6.0 -> v7.6.0</code></td>
 <tr>
 <td>[full]</td>
 <td><code class="docutils literal notranslate">v7.6.0 -> v7.6.0</code></td>
 </table>
 </div>
 </li>
        <li> <span class="li-head">ssl_pfs</span> - Select the cipher suites that can be used for SSL perfect forward secrecy (PFS). Applies to both client and server sessions. <span class="li-normal">type: str</span> <span class="li-normal">choices: require, deny, allow</span>
 <a id='label102' href="javascript:ContentClick('label103', 'label102');" onmouseover="ContentPreview('label103');" onmouseout="ContentUnpreview('label103');" title="click to collapse or expand..."> more... </a>
 <div id="label103" style="display:none">
 <table border="1">
 <tr>
 <td></td>
 <td colspan="1">Supported Version Ranges</td>
 </tr>
 <tr>
 <td>ssl_pfs</td>
 <td><code class="docutils literal notranslate">v7.6.0 -> v7.6.0 </code></td>
 </tr>
 <tr>
 <td>[require]</td>
 <td><code class="docutils literal notranslate">v7.6.0 -> v7.6.0</code></td>
 <tr>
 <td>[deny]</td>
 <td><code class="docutils literal notranslate">v7.6.0 -> v7.6.0</code></td>
 <tr>
 <td>[allow]</td>
 <td><code class="docutils literal notranslate">v7.6.0 -> v7.6.0</code></td>
 </table>
 </div>
 </li>
        <li> <span class="li-head">ssl_send_empty_frags</span> - Enable/disable sending empty fragments to avoid CBC IV attacks (SSL 3.0 & TLS 1.0 only). May need to be disabled for compatibility with older systems. <span class="li-normal">type: str</span> <span class="li-normal">choices: enable, disable</span>
 <a id='label104' href="javascript:ContentClick('label105', 'label104');" onmouseover="ContentPreview('label105');" onmouseout="ContentUnpreview('label105');" title="click to collapse or expand..."> more... </a>
 <div id="label105" style="display:none">
 <table border="1">
 <tr>
 <td></td>
 <td colspan="1">Supported Version Ranges</td>
 </tr>
 <tr>
 <td>ssl_send_empty_frags</td>
 <td><code class="docutils literal notranslate">v7.6.0 -> v7.6.0 </code></td>
 </tr>
 <tr>
 <td>[enable]</td>
 <td><code class="docutils literal notranslate">v7.6.0 -> v7.6.0</code></td>
 <tr>
 <td>[disable]</td>
 <td><code class="docutils literal notranslate">v7.6.0 -> v7.6.0</code></td>
 </table>
 </div>
 </li>
        <li> <span class="li-head">ssl_server_algorithm</span> - Permitted encryption algorithms for the server side of SSL full mode sessions according to encryption strength. <span class="li-normal">type: str</span> <span class="li-normal">choices: high, medium, low, custom, client</span>
 <a id='label106' href="javascript:ContentClick('label107', 'label106');" onmouseover="ContentPreview('label107');" onmouseout="ContentUnpreview('label107');" title="click to collapse or expand..."> more... </a>
 <div id="label107" style="display:none">
 <table border="1">
 <tr>
 <td></td>
 <td colspan="1">Supported Version Ranges</td>
 </tr>
 <tr>
 <td>ssl_server_algorithm</td>
 <td><code class="docutils literal notranslate">v7.6.0 -> v7.6.0 </code></td>
 </tr>
 <tr>
 <td>[high]</td>
 <td><code class="docutils literal notranslate">v7.6.0 -> v7.6.0</code></td>
 <tr>
 <td>[medium]</td>
 <td><code class="docutils literal notranslate">v7.6.0 -> v7.6.0</code></td>
 <tr>
 <td>[low]</td>
 <td><code class="docutils literal notranslate">v7.6.0 -> v7.6.0</code></td>
 <tr>
 <td>[custom]</td>
 <td><code class="docutils literal notranslate">v7.6.0 -> v7.6.0</code></td>
 <tr>
 <td>[client]</td>
 <td><code class="docutils literal notranslate">v7.6.0 -> v7.6.0</code></td>
 </table>
 </div>
 </li>
        <li> <span class="li-head">ssl_server_cipher_suites</span> - SSL/TLS cipher suites to offer to a server, ordered by priority. <span class="li-normal">type: list</span> <span style="font-family:'Courier New'" class="li-required">member_path: ssl_server_cipher_suites:priority</span>
 <a id='label108' href="javascript:ContentClick('label109', 'label108');" onmouseover="ContentPreview('label109');" onmouseout="ContentUnpreview('label109');" title="click to collapse or expand..."> more... </a>
 <div id="label109" style="display:none">
 <table border="1">
 <tr>
 <td></td><td colspan="1">Supported Version Ranges</td>
 </tr>
 <tr>
 <td>ssl_server_cipher_suites</td>
 <td><code class="docutils literal notranslate">v7.6.0 -> v7.6.0 </code></td>
 </tr>
 </table>
 </div>
 </li>
            <ul class="ul-self">
            <li> <span class="li-head">cipher</span> - Cipher suite name. <span class="li-normal">type: str</span> <span class="li-normal">choices: TLS-AES-128-GCM-SHA256, TLS-AES-256-GCM-SHA384, TLS-CHACHA20-POLY1305-SHA256, TLS-ECDHE-RSA-WITH-CHACHA20-POLY1305-SHA256, TLS-ECDHE-ECDSA-WITH-CHACHA20-POLY1305-SHA256, TLS-DHE-RSA-WITH-CHACHA20-POLY1305-SHA256, TLS-DHE-RSA-WITH-AES-128-CBC-SHA, TLS-DHE-RSA-WITH-AES-256-CBC-SHA, TLS-DHE-RSA-WITH-AES-128-CBC-SHA256, TLS-DHE-RSA-WITH-AES-128-GCM-SHA256, TLS-DHE-RSA-WITH-AES-256-CBC-SHA256, TLS-DHE-RSA-WITH-AES-256-GCM-SHA384, TLS-DHE-DSS-WITH-AES-128-CBC-SHA, TLS-DHE-DSS-WITH-AES-256-CBC-SHA, TLS-DHE-DSS-WITH-AES-128-CBC-SHA256, TLS-DHE-DSS-WITH-AES-128-GCM-SHA256, TLS-DHE-DSS-WITH-AES-256-CBC-SHA256, TLS-DHE-DSS-WITH-AES-256-GCM-SHA384, TLS-ECDHE-RSA-WITH-AES-128-CBC-SHA, TLS-ECDHE-RSA-WITH-AES-128-CBC-SHA256, TLS-ECDHE-RSA-WITH-AES-128-GCM-SHA256, TLS-ECDHE-RSA-WITH-AES-256-CBC-SHA, TLS-ECDHE-RSA-WITH-AES-256-CBC-SHA384, TLS-ECDHE-RSA-WITH-AES-256-GCM-SHA384, TLS-ECDHE-ECDSA-WITH-AES-128-CBC-SHA, TLS-ECDHE-ECDSA-WITH-AES-128-CBC-SHA256, TLS-ECDHE-ECDSA-WITH-AES-128-GCM-SHA256, TLS-ECDHE-ECDSA-WITH-AES-256-CBC-SHA, TLS-ECDHE-ECDSA-WITH-AES-256-CBC-SHA384, TLS-ECDHE-ECDSA-WITH-AES-256-GCM-SHA384, TLS-RSA-WITH-AES-128-CBC-SHA, TLS-RSA-WITH-AES-256-CBC-SHA, TLS-RSA-WITH-AES-128-CBC-SHA256, TLS-RSA-WITH-AES-128-GCM-SHA256, TLS-RSA-WITH-AES-256-CBC-SHA256, TLS-RSA-WITH-AES-256-GCM-SHA384, TLS-RSA-WITH-CAMELLIA-128-CBC-SHA, TLS-RSA-WITH-CAMELLIA-256-CBC-SHA, TLS-RSA-WITH-CAMELLIA-128-CBC-SHA256, TLS-RSA-WITH-CAMELLIA-256-CBC-SHA256, TLS-DHE-RSA-WITH-3DES-EDE-CBC-SHA, TLS-DHE-RSA-WITH-CAMELLIA-128-CBC-SHA, TLS-DHE-DSS-WITH-CAMELLIA-128-CBC-SHA, TLS-DHE-RSA-WITH-CAMELLIA-256-CBC-SHA, TLS-DHE-DSS-WITH-CAMELLIA-256-CBC-SHA, TLS-DHE-RSA-WITH-CAMELLIA-128-CBC-SHA256, TLS-DHE-DSS-WITH-CAMELLIA-128-CBC-SHA256, TLS-DHE-RSA-WITH-CAMELLIA-256-CBC-SHA256, TLS-DHE-DSS-WITH-CAMELLIA-256-CBC-SHA256, TLS-DHE-RSA-WITH-SEED-CBC-SHA, TLS-DHE-DSS-WITH-SEED-CBC-SHA, TLS-DHE-RSA-WITH-ARIA-128-CBC-SHA256, TLS-DHE-RSA-WITH-ARIA-256-CBC-SHA384, TLS-DHE-DSS-WITH-ARIA-128-CBC-SHA256, TLS-DHE-DSS-WITH-ARIA-256-CBC-SHA384, TLS-RSA-WITH-SEED-CBC-SHA, TLS-RSA-WITH-ARIA-128-CBC-SHA256, TLS-RSA-WITH-ARIA-256-CBC-SHA384, TLS-ECDHE-RSA-WITH-ARIA-128-CBC-SHA256, TLS-ECDHE-RSA-WITH-ARIA-256-CBC-SHA384, TLS-ECDHE-ECDSA-WITH-ARIA-128-CBC-SHA256, TLS-ECDHE-ECDSA-WITH-ARIA-256-CBC-SHA384, TLS-ECDHE-RSA-WITH-RC4-128-SHA, TLS-ECDHE-RSA-WITH-3DES-EDE-CBC-SHA, TLS-DHE-DSS-WITH-3DES-EDE-CBC-SHA, TLS-RSA-WITH-3DES-EDE-CBC-SHA, TLS-RSA-WITH-RC4-128-MD5, TLS-RSA-WITH-RC4-128-SHA, TLS-DHE-RSA-WITH-DES-CBC-SHA, TLS-DHE-DSS-WITH-DES-CBC-SHA, TLS-RSA-WITH-DES-CBC-SHA</span>
 <a id='label110' href="javascript:ContentClick('label111', 'label110');" onmouseover="ContentPreview('label111');" onmouseout="ContentUnpreview('label111');" title="click to collapse or expand..."> more... </a>
 <div id="label111" style="display:none">
 <table border="1">
 <tr>
 <td></td>
 <td colspan="1">Supported Version Ranges</td>
 </tr>
 <tr>
 <td>cipher</td>
 <td><code class="docutils literal notranslate">v7.6.0 -> v7.6.0 </code></td>
 </tr>
 <tr>
 <td>[TLS-AES-128-GCM-SHA256]</td>
 <td><code class="docutils literal notranslate">v7.6.0 -> v7.6.0</code></td>
 <tr>
 <td>[TLS-AES-256-GCM-SHA384]</td>
 <td><code class="docutils literal notranslate">v7.6.0 -> v7.6.0</code></td>
 <tr>
 <td>[TLS-CHACHA20-POLY1305-SHA256]</td>
 <td><code class="docutils literal notranslate">v7.6.0 -> v7.6.0</code></td>
 <tr>
 <td>[TLS-ECDHE-RSA-WITH-CHACHA20-POLY1305-SHA256]</td>
 <td><code class="docutils literal notranslate">v7.6.0 -> v7.6.0</code></td>
 <tr>
 <td>[TLS-ECDHE-ECDSA-WITH-CHACHA20-POLY1305-SHA256]</td>
 <td><code class="docutils literal notranslate">v7.6.0 -> v7.6.0</code></td>
 <tr>
 <td>[TLS-DHE-RSA-WITH-CHACHA20-POLY1305-SHA256]</td>
 <td><code class="docutils literal notranslate">v7.6.0 -> v7.6.0</code></td>
 <tr>
 <td>[TLS-DHE-RSA-WITH-AES-128-CBC-SHA]</td>
 <td><code class="docutils literal notranslate">v7.6.0 -> v7.6.0</code></td>
 <tr>
 <td>[TLS-DHE-RSA-WITH-AES-256-CBC-SHA]</td>
 <td><code class="docutils literal notranslate">v7.6.0 -> v7.6.0</code></td>
 <tr>
 <td>[TLS-DHE-RSA-WITH-AES-128-CBC-SHA256]</td>
 <td><code class="docutils literal notranslate">v7.6.0 -> v7.6.0</code></td>
 <tr>
 <td>[TLS-DHE-RSA-WITH-AES-128-GCM-SHA256]</td>
 <td><code class="docutils literal notranslate">v7.6.0 -> v7.6.0</code></td>
 <tr>
 <td>[TLS-DHE-RSA-WITH-AES-256-CBC-SHA256]</td>
 <td><code class="docutils literal notranslate">v7.6.0 -> v7.6.0</code></td>
 <tr>
 <td>[TLS-DHE-RSA-WITH-AES-256-GCM-SHA384]</td>
 <td><code class="docutils literal notranslate">v7.6.0 -> v7.6.0</code></td>
 <tr>
 <td>[TLS-DHE-DSS-WITH-AES-128-CBC-SHA]</td>
 <td><code class="docutils literal notranslate">v7.6.0 -> v7.6.0</code></td>
 <tr>
 <td>[TLS-DHE-DSS-WITH-AES-256-CBC-SHA]</td>
 <td><code class="docutils literal notranslate">v7.6.0 -> v7.6.0</code></td>
 <tr>
 <td>[TLS-DHE-DSS-WITH-AES-128-CBC-SHA256]</td>
 <td><code class="docutils literal notranslate">v7.6.0 -> v7.6.0</code></td>
 <tr>
 <td>[TLS-DHE-DSS-WITH-AES-128-GCM-SHA256]</td>
 <td><code class="docutils literal notranslate">v7.6.0 -> v7.6.0</code></td>
 <tr>
 <td>[TLS-DHE-DSS-WITH-AES-256-CBC-SHA256]</td>
 <td><code class="docutils literal notranslate">v7.6.0 -> v7.6.0</code></td>
 <tr>
 <td>[TLS-DHE-DSS-WITH-AES-256-GCM-SHA384]</td>
 <td><code class="docutils literal notranslate">v7.6.0 -> v7.6.0</code></td>
 <tr>
 <td>[TLS-ECDHE-RSA-WITH-AES-128-CBC-SHA]</td>
 <td><code class="docutils literal notranslate">v7.6.0 -> v7.6.0</code></td>
 <tr>
 <td>[TLS-ECDHE-RSA-WITH-AES-128-CBC-SHA256]</td>
 <td><code class="docutils literal notranslate">v7.6.0 -> v7.6.0</code></td>
 <tr>
 <td>[TLS-ECDHE-RSA-WITH-AES-128-GCM-SHA256]</td>
 <td><code class="docutils literal notranslate">v7.6.0 -> v7.6.0</code></td>
 <tr>
 <td>[TLS-ECDHE-RSA-WITH-AES-256-CBC-SHA]</td>
 <td><code class="docutils literal notranslate">v7.6.0 -> v7.6.0</code></td>
 <tr>
 <td>[TLS-ECDHE-RSA-WITH-AES-256-CBC-SHA384]</td>
 <td><code class="docutils literal notranslate">v7.6.0 -> v7.6.0</code></td>
 <tr>
 <td>[TLS-ECDHE-RSA-WITH-AES-256-GCM-SHA384]</td>
 <td><code class="docutils literal notranslate">v7.6.0 -> v7.6.0</code></td>
 <tr>
 <td>[TLS-ECDHE-ECDSA-WITH-AES-128-CBC-SHA]</td>
 <td><code class="docutils literal notranslate">v7.6.0 -> v7.6.0</code></td>
 <tr>
 <td>[TLS-ECDHE-ECDSA-WITH-AES-128-CBC-SHA256]</td>
 <td><code class="docutils literal notranslate">v7.6.0 -> v7.6.0</code></td>
 <tr>
 <td>[TLS-ECDHE-ECDSA-WITH-AES-128-GCM-SHA256]</td>
 <td><code class="docutils literal notranslate">v7.6.0 -> v7.6.0</code></td>
 <tr>
 <td>[TLS-ECDHE-ECDSA-WITH-AES-256-CBC-SHA]</td>
 <td><code class="docutils literal notranslate">v7.6.0 -> v7.6.0</code></td>
 <tr>
 <td>[TLS-ECDHE-ECDSA-WITH-AES-256-CBC-SHA384]</td>
 <td><code class="docutils literal notranslate">v7.6.0 -> v7.6.0</code></td>
 <tr>
 <td>[TLS-ECDHE-ECDSA-WITH-AES-256-GCM-SHA384]</td>
 <td><code class="docutils literal notranslate">v7.6.0 -> v7.6.0</code></td>
 <tr>
 <td>[TLS-RSA-WITH-AES-128-CBC-SHA]</td>
 <td><code class="docutils literal notranslate">v7.6.0 -> v7.6.0</code></td>
 <tr>
 <td>[TLS-RSA-WITH-AES-256-CBC-SHA]</td>
 <td><code class="docutils literal notranslate">v7.6.0 -> v7.6.0</code></td>
 <tr>
 <td>[TLS-RSA-WITH-AES-128-CBC-SHA256]</td>
 <td><code class="docutils literal notranslate">v7.6.0 -> v7.6.0</code></td>
 <tr>
 <td>[TLS-RSA-WITH-AES-128-GCM-SHA256]</td>
 <td><code class="docutils literal notranslate">v7.6.0 -> v7.6.0</code></td>
 <tr>
 <td>[TLS-RSA-WITH-AES-256-CBC-SHA256]</td>
 <td><code class="docutils literal notranslate">v7.6.0 -> v7.6.0</code></td>
 <tr>
 <td>[TLS-RSA-WITH-AES-256-GCM-SHA384]</td>
 <td><code class="docutils literal notranslate">v7.6.0 -> v7.6.0</code></td>
 <tr>
 <td>[TLS-RSA-WITH-CAMELLIA-128-CBC-SHA]</td>
 <td><code class="docutils literal notranslate">v7.6.0 -> v7.6.0</code></td>
 <tr>
 <td>[TLS-RSA-WITH-CAMELLIA-256-CBC-SHA]</td>
 <td><code class="docutils literal notranslate">v7.6.0 -> v7.6.0</code></td>
 <tr>
 <td>[TLS-RSA-WITH-CAMELLIA-128-CBC-SHA256]</td>
 <td><code class="docutils literal notranslate">v7.6.0 -> v7.6.0</code></td>
 <tr>
 <td>[TLS-RSA-WITH-CAMELLIA-256-CBC-SHA256]</td>
 <td><code class="docutils literal notranslate">v7.6.0 -> v7.6.0</code></td>
 <tr>
 <td>[TLS-DHE-RSA-WITH-3DES-EDE-CBC-SHA]</td>
 <td><code class="docutils literal notranslate">v7.6.0 -> v7.6.0</code></td>
 <tr>
 <td>[TLS-DHE-RSA-WITH-CAMELLIA-128-CBC-SHA]</td>
 <td><code class="docutils literal notranslate">v7.6.0 -> v7.6.0</code></td>
 <tr>
 <td>[TLS-DHE-DSS-WITH-CAMELLIA-128-CBC-SHA]</td>
 <td><code class="docutils literal notranslate">v7.6.0 -> v7.6.0</code></td>
 <tr>
 <td>[TLS-DHE-RSA-WITH-CAMELLIA-256-CBC-SHA]</td>
 <td><code class="docutils literal notranslate">v7.6.0 -> v7.6.0</code></td>
 <tr>
 <td>[TLS-DHE-DSS-WITH-CAMELLIA-256-CBC-SHA]</td>
 <td><code class="docutils literal notranslate">v7.6.0 -> v7.6.0</code></td>
 <tr>
 <td>[TLS-DHE-RSA-WITH-CAMELLIA-128-CBC-SHA256]</td>
 <td><code class="docutils literal notranslate">v7.6.0 -> v7.6.0</code></td>
 <tr>
 <td>[TLS-DHE-DSS-WITH-CAMELLIA-128-CBC-SHA256]</td>
 <td><code class="docutils literal notranslate">v7.6.0 -> v7.6.0</code></td>
 <tr>
 <td>[TLS-DHE-RSA-WITH-CAMELLIA-256-CBC-SHA256]</td>
 <td><code class="docutils literal notranslate">v7.6.0 -> v7.6.0</code></td>
 <tr>
 <td>[TLS-DHE-DSS-WITH-CAMELLIA-256-CBC-SHA256]</td>
 <td><code class="docutils literal notranslate">v7.6.0 -> v7.6.0</code></td>
 <tr>
 <td>[TLS-DHE-RSA-WITH-SEED-CBC-SHA]</td>
 <td><code class="docutils literal notranslate">v7.6.0 -> v7.6.0</code></td>
 <tr>
 <td>[TLS-DHE-DSS-WITH-SEED-CBC-SHA]</td>
 <td><code class="docutils literal notranslate">v7.6.0 -> v7.6.0</code></td>
 <tr>
 <td>[TLS-DHE-RSA-WITH-ARIA-128-CBC-SHA256]</td>
 <td><code class="docutils literal notranslate">v7.6.0 -> v7.6.0</code></td>
 <tr>
 <td>[TLS-DHE-RSA-WITH-ARIA-256-CBC-SHA384]</td>
 <td><code class="docutils literal notranslate">v7.6.0 -> v7.6.0</code></td>
 <tr>
 <td>[TLS-DHE-DSS-WITH-ARIA-128-CBC-SHA256]</td>
 <td><code class="docutils literal notranslate">v7.6.0 -> v7.6.0</code></td>
 <tr>
 <td>[TLS-DHE-DSS-WITH-ARIA-256-CBC-SHA384]</td>
 <td><code class="docutils literal notranslate">v7.6.0 -> v7.6.0</code></td>
 <tr>
 <td>[TLS-RSA-WITH-SEED-CBC-SHA]</td>
 <td><code class="docutils literal notranslate">v7.6.0 -> v7.6.0</code></td>
 <tr>
 <td>[TLS-RSA-WITH-ARIA-128-CBC-SHA256]</td>
 <td><code class="docutils literal notranslate">v7.6.0 -> v7.6.0</code></td>
 <tr>
 <td>[TLS-RSA-WITH-ARIA-256-CBC-SHA384]</td>
 <td><code class="docutils literal notranslate">v7.6.0 -> v7.6.0</code></td>
 <tr>
 <td>[TLS-ECDHE-RSA-WITH-ARIA-128-CBC-SHA256]</td>
 <td><code class="docutils literal notranslate">v7.6.0 -> v7.6.0</code></td>
 <tr>
 <td>[TLS-ECDHE-RSA-WITH-ARIA-256-CBC-SHA384]</td>
 <td><code class="docutils literal notranslate">v7.6.0 -> v7.6.0</code></td>
 <tr>
 <td>[TLS-ECDHE-ECDSA-WITH-ARIA-128-CBC-SHA256]</td>
 <td><code class="docutils literal notranslate">v7.6.0 -> v7.6.0</code></td>
 <tr>
 <td>[TLS-ECDHE-ECDSA-WITH-ARIA-256-CBC-SHA384]</td>
 <td><code class="docutils literal notranslate">v7.6.0 -> v7.6.0</code></td>
 <tr>
 <td>[TLS-ECDHE-RSA-WITH-RC4-128-SHA]</td>
 <td><code class="docutils literal notranslate">v7.6.0 -> v7.6.0</code></td>
 <tr>
 <td>[TLS-ECDHE-RSA-WITH-3DES-EDE-CBC-SHA]</td>
 <td><code class="docutils literal notranslate">v7.6.0 -> v7.6.0</code></td>
 <tr>
 <td>[TLS-DHE-DSS-WITH-3DES-EDE-CBC-SHA]</td>
 <td><code class="docutils literal notranslate">v7.6.0 -> v7.6.0</code></td>
 <tr>
 <td>[TLS-RSA-WITH-3DES-EDE-CBC-SHA]</td>
 <td><code class="docutils literal notranslate">v7.6.0 -> v7.6.0</code></td>
 <tr>
 <td>[TLS-RSA-WITH-RC4-128-MD5]</td>
 <td><code class="docutils literal notranslate">v7.6.0 -> v7.6.0</code></td>
 <tr>
 <td>[TLS-RSA-WITH-RC4-128-SHA]</td>
 <td><code class="docutils literal notranslate">v7.6.0 -> v7.6.0</code></td>
 <tr>
 <td>[TLS-DHE-RSA-WITH-DES-CBC-SHA]</td>
 <td><code class="docutils literal notranslate">v7.6.0 -> v7.6.0</code></td>
 <tr>
 <td>[TLS-DHE-DSS-WITH-DES-CBC-SHA]</td>
 <td><code class="docutils literal notranslate">v7.6.0 -> v7.6.0</code></td>
 <tr>
 <td>[TLS-RSA-WITH-DES-CBC-SHA]</td>
 <td><code class="docutils literal notranslate">v7.6.0 -> v7.6.0</code></td>
 </table>
 </div>
 </li>
            <li> <span class="li-head">priority</span> - SSL/TLS cipher suites priority. see <a href='#notes'>Notes</a>. <span class="li-normal">type: int</span> <span class="li-required">required: true</span>
 <a id='label112' href="javascript:ContentClick('label113', 'label112');" onmouseover="ContentPreview('label113');" onmouseout="ContentUnpreview('label113');" title="click to collapse or expand..."> more... </a>
 <div id="label113" style="display:none">
 <table border="1">
 <tr>
 <td></td>
 <td colspan="1">Supported Version Ranges</td>
 </tr>
 <tr>
 <td>priority</td>
 <td><code class="docutils literal notranslate">v7.6.0 -> v7.6.0 </code></td>
 </tr>
 </table>
 </div>
 </li>
            <li> <span class="li-head">versions</span> - SSL/TLS versions that the cipher suite can be used with. <span class="li-normal">type: list</span> <span class="li-normal">choices: ssl-3.0, tls-1.0, tls-1.1, tls-1.2, tls-1.3</span>
 <a id='label114' href="javascript:ContentClick('label115', 'label114');" onmouseover="ContentPreview('label115');" onmouseout="ContentUnpreview('label115');" title="click to collapse or expand..."> more... </a>
 <div id="label115" style="display:none">
 <table border="1">
 <tr>
 <td></td>
 <td colspan="1">Supported Version Ranges</td>
 </tr>
 <tr>
 <td>versions</td>
 <td><code class="docutils literal notranslate">v7.6.0 -> v7.6.0 </code></td>
 </tr>
 <tr>
 <td>[ssl-3.0]</td>
 <td><code class="docutils literal notranslate">v7.6.0 -> v7.6.0</code></td>
 <tr>
 <td>[tls-1.0]</td>
 <td><code class="docutils literal notranslate">v7.6.0 -> v7.6.0</code></td>
 <tr>
 <td>[tls-1.1]</td>
 <td><code class="docutils literal notranslate">v7.6.0 -> v7.6.0</code></td>
 <tr>
 <td>[tls-1.2]</td>
 <td><code class="docutils literal notranslate">v7.6.0 -> v7.6.0</code></td>
 <tr>
 <td>[tls-1.3]</td>
 <td><code class="docutils literal notranslate">v7.6.0 -> v7.6.0</code></td>
 </table>
 </div>
 </li>
            </ul>
        <li> <span class="li-head">ssl_server_max_version</span> - Highest SSL/TLS version acceptable from a server. Use the client setting by default. <span class="li-normal">type: str</span> <span class="li-normal">choices: ssl-3.0, tls-1.0, tls-1.1, tls-1.2, tls-1.3, client</span>
 <a id='label116' href="javascript:ContentClick('label117', 'label116');" onmouseover="ContentPreview('label117');" onmouseout="ContentUnpreview('label117');" title="click to collapse or expand..."> more... </a>
 <div id="label117" style="display:none">
 <table border="1">
 <tr>
 <td></td>
 <td colspan="1">Supported Version Ranges</td>
 </tr>
 <tr>
 <td>ssl_server_max_version</td>
 <td><code class="docutils literal notranslate">v7.6.0 -> v7.6.0 </code></td>
 </tr>
 <tr>
 <td>[ssl-3.0]</td>
 <td><code class="docutils literal notranslate">v7.6.0 -> v7.6.0</code></td>
 <tr>
 <td>[tls-1.0]</td>
 <td><code class="docutils literal notranslate">v7.6.0 -> v7.6.0</code></td>
 <tr>
 <td>[tls-1.1]</td>
 <td><code class="docutils literal notranslate">v7.6.0 -> v7.6.0</code></td>
 <tr>
 <td>[tls-1.2]</td>
 <td><code class="docutils literal notranslate">v7.6.0 -> v7.6.0</code></td>
 <tr>
 <td>[tls-1.3]</td>
 <td><code class="docutils literal notranslate">v7.6.0 -> v7.6.0</code></td>
 <tr>
 <td>[client]</td>
 <td><code class="docutils literal notranslate">v7.6.0 -> v7.6.0</code></td>
 </table>
 </div>
 </li>
        <li> <span class="li-head">ssl_server_min_version</span> - Lowest SSL/TLS version acceptable from a server. Use the client setting by default. <span class="li-normal">type: str</span> <span class="li-normal">choices: ssl-3.0, tls-1.0, tls-1.1, tls-1.2, tls-1.3, client</span>
 <a id='label118' href="javascript:ContentClick('label119', 'label118');" onmouseover="ContentPreview('label119');" onmouseout="ContentUnpreview('label119');" title="click to collapse or expand..."> more... </a>
 <div id="label119" style="display:none">
 <table border="1">
 <tr>
 <td></td>
 <td colspan="1">Supported Version Ranges</td>
 </tr>
 <tr>
 <td>ssl_server_min_version</td>
 <td><code class="docutils literal notranslate">v7.6.0 -> v7.6.0 </code></td>
 </tr>
 <tr>
 <td>[ssl-3.0]</td>
 <td><code class="docutils literal notranslate">v7.6.0 -> v7.6.0</code></td>
 <tr>
 <td>[tls-1.0]</td>
 <td><code class="docutils literal notranslate">v7.6.0 -> v7.6.0</code></td>
 <tr>
 <td>[tls-1.1]</td>
 <td><code class="docutils literal notranslate">v7.6.0 -> v7.6.0</code></td>
 <tr>
 <td>[tls-1.2]</td>
 <td><code class="docutils literal notranslate">v7.6.0 -> v7.6.0</code></td>
 <tr>
 <td>[tls-1.3]</td>
 <td><code class="docutils literal notranslate">v7.6.0 -> v7.6.0</code></td>
 <tr>
 <td>[client]</td>
 <td><code class="docutils literal notranslate">v7.6.0 -> v7.6.0</code></td>
 </table>
 </div>
 </li>
        <li> <span class="li-head">ssl_server_renegotiation</span> - Enable/disable secure renegotiation to comply with RFC 5746. <span class="li-normal">type: str</span> <span class="li-normal">choices: enable, disable</span>
 <a id='label120' href="javascript:ContentClick('label121', 'label120');" onmouseover="ContentPreview('label121');" onmouseout="ContentUnpreview('label121');" title="click to collapse or expand..."> more... </a>
 <div id="label121" style="display:none">
 <table border="1">
 <tr>
 <td></td>
 <td colspan="1">Supported Version Ranges</td>
 </tr>
 <tr>
 <td>ssl_server_renegotiation</td>
 <td><code class="docutils literal notranslate">v7.6.0 -> v7.6.0 </code></td>
 </tr>
 <tr>
 <td>[enable]</td>
 <td><code class="docutils literal notranslate">v7.6.0 -> v7.6.0</code></td>
 <tr>
 <td>[disable]</td>
 <td><code class="docutils literal notranslate">v7.6.0 -> v7.6.0</code></td>
 </table>
 </div>
 </li>
        <li> <span class="li-head">ssl_server_session_state_max</span> - Maximum number of FortiGate to Server SSL session states to keep. <span class="li-normal">type: int</span>
 <a id='label122' href="javascript:ContentClick('label123', 'label122');" onmouseover="ContentPreview('label123');" onmouseout="ContentUnpreview('label123');" title="click to collapse or expand..."> more... </a>
 <div id="label123" style="display:none">
 <table border="1">
 <tr>
 <td></td>
 <td colspan="1">Supported Version Ranges</td>
 </tr>
 <tr>
 <td>ssl_server_session_state_max</td>
 <td><code class="docutils literal notranslate">v7.6.0 -> v7.6.0 </code></td>
 </tr>
 </table>
 </div>
 </li>
        <li> <span class="li-head">ssl_server_session_state_timeout</span> - Number of minutes to keep FortiGate to Server SSL session state. <span class="li-normal">type: int</span>
 <a id='label124' href="javascript:ContentClick('label125', 'label124');" onmouseover="ContentPreview('label125');" onmouseout="ContentUnpreview('label125');" title="click to collapse or expand..."> more... </a>
 <div id="label125" style="display:none">
 <table border="1">
 <tr>
 <td></td>
 <td colspan="1">Supported Version Ranges</td>
 </tr>
 <tr>
 <td>ssl_server_session_state_timeout</td>
 <td><code class="docutils literal notranslate">v7.6.0 -> v7.6.0 </code></td>
 </tr>
 </table>
 </div>
 </li>
        <li> <span class="li-head">ssl_server_session_state_type</span> - How to expire SSL sessions for the segment of the SSL connection between the server and the FortiGate. <span class="li-normal">type: str</span> <span class="li-normal">choices: disable, time, count, both</span>
 <a id='label126' href="javascript:ContentClick('label127', 'label126');" onmouseover="ContentPreview('label127');" onmouseout="ContentUnpreview('label127');" title="click to collapse or expand..."> more... </a>
 <div id="label127" style="display:none">
 <table border="1">
 <tr>
 <td></td>
 <td colspan="1">Supported Version Ranges</td>
 </tr>
 <tr>
 <td>ssl_server_session_state_type</td>
 <td><code class="docutils literal notranslate">v7.6.0 -> v7.6.0 </code></td>
 </tr>
 <tr>
 <td>[disable]</td>
 <td><code class="docutils literal notranslate">v7.6.0 -> v7.6.0</code></td>
 <tr>
 <td>[time]</td>
 <td><code class="docutils literal notranslate">v7.6.0 -> v7.6.0</code></td>
 <tr>
 <td>[count]</td>
 <td><code class="docutils literal notranslate">v7.6.0 -> v7.6.0</code></td>
 <tr>
 <td>[both]</td>
 <td><code class="docutils literal notranslate">v7.6.0 -> v7.6.0</code></td>
 </table>
 </div>
 </li>
        <li> <span class="li-head">status</span> - Enable/disable the traffic forward proxy for ZTNA traffic. <span class="li-normal">type: str</span> <span class="li-normal">choices: enable, disable</span>
 <a id='label128' href="javascript:ContentClick('label129', 'label128');" onmouseover="ContentPreview('label129');" onmouseout="ContentUnpreview('label129');" title="click to collapse or expand..."> more... </a>
 <div id="label129" style="display:none">
 <table border="1">
 <tr>
 <td></td>
 <td colspan="1">Supported Version Ranges</td>
 </tr>
 <tr>
 <td>status</td>
 <td><code class="docutils literal notranslate">v7.6.0 -> v7.6.0 </code></td>
 </tr>
 <tr>
 <td>[enable]</td>
 <td><code class="docutils literal notranslate">v7.6.0 -> v7.6.0</code></td>
 <tr>
 <td>[disable]</td>
 <td><code class="docutils literal notranslate">v7.6.0 -> v7.6.0</code></td>
 </table>
 </div>
 </li>
        <li> <span class="li-head">svr_pool_multiplex</span> - Enable/disable server pool multiplexing. Share connected server in HTTP, HTTPS, and web-portal api-gateway. <span class="li-normal">type: str</span> <span class="li-normal">choices: enable, disable</span>
 <a id='label130' href="javascript:ContentClick('label131', 'label130');" onmouseover="ContentPreview('label131');" onmouseout="ContentUnpreview('label131');" title="click to collapse or expand..."> more... </a>
 <div id="label131" style="display:none">
 <table border="1">
 <tr>
 <td></td>
 <td colspan="1">Supported Version Ranges</td>
 </tr>
 <tr>
 <td>svr_pool_multiplex</td>
 <td><code class="docutils literal notranslate">v7.6.0 -> v7.6.0 </code></td>
 </tr>
 <tr>
 <td>[enable]</td>
 <td><code class="docutils literal notranslate">v7.6.0 -> v7.6.0</code></td>
 <tr>
 <td>[disable]</td>
 <td><code class="docutils literal notranslate">v7.6.0 -> v7.6.0</code></td>
 </table>
 </div>
 </li>
        <li> <span class="li-head">svr_pool_server_max_concurrent_request</span> - Maximum number of concurrent requests that servers in server pool could handle . <span class="li-normal">type: int</span>
 <a id='label132' href="javascript:ContentClick('label133', 'label132');" onmouseover="ContentPreview('label133');" onmouseout="ContentUnpreview('label133');" title="click to collapse or expand..."> more... </a>
 <div id="label133" style="display:none">
 <table border="1">
 <tr>
 <td></td>
 <td colspan="1">Supported Version Ranges</td>
 </tr>
 <tr>
 <td>svr_pool_server_max_concurrent_request</td>
 <td><code class="docutils literal notranslate">v7.6.0 -> v7.6.0 </code></td>
 </tr>
 </table>
 </div>
 </li>
        <li> <span class="li-head">svr_pool_server_max_request</span> - Maximum number of requests that servers in server pool handle before disconnecting . <span class="li-normal">type: int</span>
 <a id='label134' href="javascript:ContentClick('label135', 'label134');" onmouseover="ContentPreview('label135');" onmouseout="ContentUnpreview('label135');" title="click to collapse or expand..."> more... </a>
 <div id="label135" style="display:none">
 <table border="1">
 <tr>
 <td></td>
 <td colspan="1">Supported Version Ranges</td>
 </tr>
 <tr>
 <td>svr_pool_server_max_request</td>
 <td><code class="docutils literal notranslate">v7.6.0 -> v7.6.0 </code></td>
 </tr>
 </table>
 </div>
 </li>
        <li> <span class="li-head">svr_pool_ttl</span> - Time-to-live in the server pool for idle connections to servers. <span class="li-normal">type: int</span>
 <a id='label136' href="javascript:ContentClick('label137', 'label136');" onmouseover="ContentPreview('label137');" onmouseout="ContentUnpreview('label137');" title="click to collapse or expand..."> more... </a>
 <div id="label137" style="display:none">
 <table border="1">
 <tr>
 <td></td>
 <td colspan="1">Supported Version Ranges</td>
 </tr>
 <tr>
 <td>svr_pool_ttl</td>
 <td><code class="docutils literal notranslate">v7.6.0 -> v7.6.0 </code></td>
 </tr>
 </table>
 </div>
 </li>
        <li> <span class="li-head">user_agent_detect</span> - Enable/disable to detect device type by HTTP user-agent if no client certificate provided. <span class="li-normal">type: str</span> <span class="li-normal">choices: disable, enable</span>
 <a id='label138' href="javascript:ContentClick('label139', 'label138');" onmouseover="ContentPreview('label139');" onmouseout="ContentUnpreview('label139');" title="click to collapse or expand..."> more... </a>
 <div id="label139" style="display:none">
 <table border="1">
 <tr>
 <td></td>
 <td colspan="1">Supported Version Ranges</td>
 </tr>
 <tr>
 <td>user_agent_detect</td>
 <td><code class="docutils literal notranslate">v7.6.0 -> v7.6.0 </code></td>
 </tr>
 <tr>
 <td>[disable]</td>
 <td><code class="docutils literal notranslate">v7.6.0 -> v7.6.0</code></td>
 <tr>
 <td>[enable]</td>
 <td><code class="docutils literal notranslate">v7.6.0 -> v7.6.0</code></td>
 </table>
 </div>
 </li>
        <li> <span class="li-head">vip</span> - Virtual IP name. Source firewall.vip.name. <span class="li-normal">type: str</span>
 <a id='label140' href="javascript:ContentClick('label141', 'label140');" onmouseover="ContentPreview('label141');" onmouseout="ContentUnpreview('label141');" title="click to collapse or expand..."> more... </a>
 <div id="label141" style="display:none">
 <table border="1">
 <tr>
 <td></td>
 <td colspan="1">Supported Version Ranges</td>
 </tr>
 <tr>
 <td>vip</td>
 <td><code class="docutils literal notranslate">v7.6.1 -> 7.6.2 </code></td>
 </tr>
 </table>
 </div>
 </li>
        <li> <span class="li-head">vip6</span> - Virtual IPv6 name. Source firewall.vip6.name. <span class="li-normal">type: str</span>
 <a id='label142' href="javascript:ContentClick('label143', 'label142');" onmouseover="ContentPreview('label143');" onmouseout="ContentUnpreview('label143');" title="click to collapse or expand..."> more... </a>
 <div id="label143" style="display:none">
 <table border="1">
 <tr>
 <td></td>
 <td colspan="1">Supported Version Ranges</td>
 </tr>
 <tr>
 <td>vip6</td>
 <td><code class="docutils literal notranslate">v7.6.1 -> 7.6.2 </code></td>
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
    
    - name: Configure ZTNA traffic forward proxy.
      fortinet.fortios.fortios_ztna_traffic_forward_proxy:
          vdom: "{{ vdom }}"
          state: "present"
          access_token: "<your_own_value>"
          ztna_traffic_forward_proxy:
              auth_portal: "disable"
              auth_virtual_host: "myhostname (source firewall.access-proxy-virtual-host.name)"
              client_cert: "disable"
              comment: "Comment."
              decrypted_traffic_mirror: "<your_own_value> (source firewall.decrypted-traffic-mirror.name)"
              empty_cert_action: "accept"
              h3_support: "enable"
              host: "myhostname (source firewall.access-proxy-virtual-host.name)"
              interface: "<your_own_value> (source system.interface.name)"
              log_blocked_traffic: "disable"
              name: "default_name_13"
              port: "<your_own_value>"
              quic:
                  ack_delay_exponent: "3"
                  active_connection_id_limit: "2"
                  active_migration: "enable"
                  grease_quic_bit: "enable"
                  max_ack_delay: "25"
                  max_datagram_frame_size: "1500"
                  max_idle_timeout: "30000"
                  max_udp_payload_size: "1500"
              ssl_accept_ffdhe_groups: "enable"
              ssl_algorithm: "high"
              ssl_certificate:
                  -
                      name: "default_name_27 (source vpn.certificate.local.name)"
              ssl_cipher_suites:
                  -
                      cipher: "TLS-AES-128-GCM-SHA256"
                      priority: "<you_own_value>"
                      versions: "ssl-3.0"
              ssl_client_fallback: "disable"
              ssl_client_rekey_count: "0"
              ssl_client_renegotiation: "allow"
              ssl_client_session_state_max: "1000"
              ssl_client_session_state_timeout: "30"
              ssl_client_session_state_type: "disable"
              ssl_dh_bits: "768"
              ssl_hpkp: "disable"
              ssl_hpkp_age: "5184000"
              ssl_hpkp_backup: "<your_own_value> (source vpn.certificate.local.name vpn.certificate.ca.name)"
              ssl_hpkp_include_subdomains: "disable"
              ssl_hpkp_primary: "<your_own_value> (source vpn.certificate.local.name vpn.certificate.ca.name)"
              ssl_hpkp_report_uri: "<your_own_value>"
              ssl_hsts: "disable"
              ssl_hsts_age: "5184000"
              ssl_hsts_include_subdomains: "disable"
              ssl_http_location_conversion: "enable"
              ssl_http_match_host: "enable"
              ssl_max_version: "ssl-3.0"
              ssl_min_version: "ssl-3.0"
              ssl_mode: "half"
              ssl_pfs: "require"
              ssl_send_empty_frags: "enable"
              ssl_server_algorithm: "high"
              ssl_server_cipher_suites:
                  -
                      cipher: "TLS-AES-128-GCM-SHA256"
                      priority: "<you_own_value>"
                      versions: "ssl-3.0"
              ssl_server_max_version: "ssl-3.0"
              ssl_server_min_version: "ssl-3.0"
              ssl_server_renegotiation: "enable"
              ssl_server_session_state_max: "100"
              ssl_server_session_state_timeout: "60"
              ssl_server_session_state_type: "disable"
              status: "enable"
              svr_pool_multiplex: "enable"
              svr_pool_server_max_concurrent_request: "0"
              svr_pool_server_max_request: "0"
              svr_pool_ttl: "15"
              user_agent_detect: "disable"
              vip: "<your_own_value> (source firewall.vip.name)"
              vip6: "<your_own_value> (source firewall.vip6.name)"


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
