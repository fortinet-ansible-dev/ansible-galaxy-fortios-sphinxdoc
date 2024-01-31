:source: fortios_firewall_access_proxy6.py

:orphan:

.. fortios_firewall_access_proxy6:

fortios_firewall_access_proxy6 -- Configure IPv6 access proxy in Fortinet's FortiOS and FortiGate.
++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++

.. versionadded:: 2.0.0

.. contents::
   :local:
   :depth: 1


Synopsis
--------
- This module is able to configure a FortiGate or FortiOS (FOS) device by allowing the user to set and modify firewall feature and access_proxy6 category. Examples include all parameters and values need to be adjusted to datasources before usage. Tested with FOS v6.0.0



Requirements
------------
The below requirements are needed on the host that executes this module.

- ansible>=2.14


Tips
----
Using member operation to add an element to an existing object.

FortiOS Version Compatibility
-----------------------------


.. raw:: html

 <br>
 <table border="1">
 <tr>
 <td></td><td colspan="1">Supported Version Ranges</td>
 </tr>
 <tr>
 <td>fortios_firewall_access_proxy6</td>
 <td><code class="docutils literal notranslate">v7.0.1 -> latest </code></td>
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
    <li> <span class="li-head">state</span> - Indicates whether to create or remove the object. <span class="li-normal">type: str</span> <span class="li-required">required: true</span> <span class="li-normal">choices: present, absent</span> </li>
    <li> <span class="li-head">firewall_access_proxy6</span> - Configure IPv6 access proxy. <span class="li-normal">type: dict</span>
 <a id='label0' href="javascript:ContentClick('label1', 'label0');" onmouseover="ContentPreview('label1');" onmouseout="ContentUnpreview('label1');" title="click to collapse or expand..."> more... </a>
 <div id="label1" style="display:none">
 <table border="1">
 <tr>
 <td></td><td colspan="1">Supported Version Ranges</td>
 </tr>
 <tr>
 <td>firewall_access_proxy6</td>
 <td><code class="docutils literal notranslate">v7.0.1 -> latest </code></td>
 </tr>
 </table>
 </div>
 </li>
        <ul class="ul-self">
        <li> <span class="li-head">add_vhost_domain_to_dnsdb</span> - Enable/disable adding vhost/domain to dnsdb for ztna dox tunnel. <span class="li-normal">type: str</span> <span class="li-normal">choices: enable, disable</span>
 <a id='label2' href="javascript:ContentClick('label3', 'label2');" onmouseover="ContentPreview('label3');" onmouseout="ContentUnpreview('label3');" title="click to collapse or expand..."> more... </a>
 <div id="label3" style="display:none">
 <table border="1">
 <tr>
 <td></td>
 <td colspan="1">Supported Version Ranges</td>
 </tr>
 <tr>
 <td>add_vhost_domain_to_dnsdb</td>
 <td><code class="docutils literal notranslate">v7.2.1 -> latest </code></td>
 </tr>
 <tr>
 <td>[enable]</td>
 <td><code class="docutils literal notranslate">v6.0.0 -> latest</code></td> <tr>
 <td>[disable]</td>
 <td><code class="docutils literal notranslate">v6.0.0 -> latest</code></td> </table>
 </div>
 </li>
        <li> <span class="li-head">api_gateway</span> - Set IPv4 API Gateway. <span class="li-normal">type: list</span> <span style="font-family:'Courier New'" class="li-required">member_path: api_gateway:id</span>
 <a id='label4' href="javascript:ContentClick('label5', 'label4');" onmouseover="ContentPreview('label5');" onmouseout="ContentUnpreview('label5');" title="click to collapse or expand..."> more... </a>
 <div id="label5" style="display:none">
 <table border="1">
 <tr>
 <td></td><td colspan="1">Supported Version Ranges</td>
 </tr>
 <tr>
 <td>api_gateway</td>
 <td><code class="docutils literal notranslate">v7.0.1 -> latest </code></td>
 </tr>
 </table>
 </div>
 </li>
            <ul class="ul-self">
            <li> <span class="li-head">application</span> - SaaS application controlled by this Access Proxy. <span class="li-normal">type: list</span> <span style="font-family:'Courier New'" class="li-required">member_path: api_gateway:id/application:name</span>
 <a id='label6' href="javascript:ContentClick('label7', 'label6');" onmouseover="ContentPreview('label7');" onmouseout="ContentUnpreview('label7');" title="click to collapse or expand..."> more... </a>
 <div id="label7" style="display:none">
 <table border="1">
 <tr>
 <td></td><td colspan="1">Supported Version Ranges</td>
 </tr>
 <tr>
 <td>application</td>
 <td><code class="docutils literal notranslate">v7.2.1 -> latest </code></td>
 </tr>
 </table>
 </div>
 </li>
                <ul class="ul-self">
                <li> <span class="li-head">name</span> - SaaS application name. <span class="li-normal">type: str</span> <span class="li-required">required: true</span>
 <a id='label8' href="javascript:ContentClick('label9', 'label8');" onmouseover="ContentPreview('label9');" onmouseout="ContentUnpreview('label9');" title="click to collapse or expand..."> more... </a>
 <div id="label9" style="display:none">
 <table border="1">
 <tr>
 <td></td>
 <td colspan="1">Supported Version Ranges</td>
 </tr>
 <tr>
 <td>name</td>
 <td><code class="docutils literal notranslate">v7.2.1 -> latest </code></td>
 </tr>
 </table>
 </div>
 </li>
                </ul>
            <li> <span class="li-head">h2_support</span> - HTTP2 support, default=Enable. <span class="li-normal">type: str</span> <span class="li-normal">choices: enable, disable</span>
 <a id='label10' href="javascript:ContentClick('label11', 'label10');" onmouseover="ContentPreview('label11');" onmouseout="ContentUnpreview('label11');" title="click to collapse or expand..."> more... </a>
 <div id="label11" style="display:none">
 <table border="1">
 <tr>
 <td></td>
 <td colspan="1">Supported Version Ranges</td>
 </tr>
 <tr>
 <td>h2_support</td>
 <td><code class="docutils literal notranslate">v7.4.1 -> latest </code></td>
 </tr>
 <tr>
 <td>[enable]</td>
 <td><code class="docutils literal notranslate">v6.0.0 -> latest</code></td> <tr>
 <td>[disable]</td>
 <td><code class="docutils literal notranslate">v6.0.0 -> latest</code></td> </table>
 </div>
 </li>
            <li> <span class="li-head">h3_support</span> - HTTP3/QUIC support, default=Disable. <span class="li-normal">type: str</span> <span class="li-normal">choices: enable, disable</span>
 <a id='label12' href="javascript:ContentClick('label13', 'label12');" onmouseover="ContentPreview('label13');" onmouseout="ContentUnpreview('label13');" title="click to collapse or expand..."> more... </a>
 <div id="label13" style="display:none">
 <table border="1">
 <tr>
 <td></td>
 <td colspan="1">Supported Version Ranges</td>
 </tr>
 <tr>
 <td>h3_support</td>
 <td><code class="docutils literal notranslate">v7.4.1 -> latest </code></td>
 </tr>
 <tr>
 <td>[enable]</td>
 <td><code class="docutils literal notranslate">v6.0.0 -> latest</code></td> <tr>
 <td>[disable]</td>
 <td><code class="docutils literal notranslate">v6.0.0 -> latest</code></td> </table>
 </div>
 </li>
            <li> <span class="li-head">http_cookie_age</span> - Time in minutes that client web browsers should keep a cookie. Default is 60 minutes. 0 = no time limit. <span class="li-normal">type: int</span>
 <a id='label14' href="javascript:ContentClick('label15', 'label14');" onmouseover="ContentPreview('label15');" onmouseout="ContentUnpreview('label15');" title="click to collapse or expand..."> more... </a>
 <div id="label15" style="display:none">
 <table border="1">
 <tr>
 <td></td>
 <td colspan="1">Supported Version Ranges</td>
 </tr>
 <tr>
 <td>http_cookie_age</td>
 <td><code class="docutils literal notranslate">v7.0.1 -> latest </code></td>
 </tr>
 </table>
 </div>
 </li>
            <li> <span class="li-head">http_cookie_domain</span> - Domain that HTTP cookie persistence should apply to. <span class="li-normal">type: str</span>
 <a id='label16' href="javascript:ContentClick('label17', 'label16');" onmouseover="ContentPreview('label17');" onmouseout="ContentUnpreview('label17');" title="click to collapse or expand..."> more... </a>
 <div id="label17" style="display:none">
 <table border="1">
 <tr>
 <td></td>
 <td colspan="1">Supported Version Ranges</td>
 </tr>
 <tr>
 <td>http_cookie_domain</td>
 <td><code class="docutils literal notranslate">v7.0.1 -> latest </code></td>
 </tr>
 </table>
 </div>
 </li>
            <li> <span class="li-head">http_cookie_domain_from_host</span> - Enable/disable use of HTTP cookie domain from host field in HTTP. <span class="li-normal">type: str</span> <span class="li-normal">choices: disable, enable</span>
 <a id='label18' href="javascript:ContentClick('label19', 'label18');" onmouseover="ContentPreview('label19');" onmouseout="ContentUnpreview('label19');" title="click to collapse or expand..."> more... </a>
 <div id="label19" style="display:none">
 <table border="1">
 <tr>
 <td></td>
 <td colspan="1">Supported Version Ranges</td>
 </tr>
 <tr>
 <td>http_cookie_domain_from_host</td>
 <td><code class="docutils literal notranslate">v7.0.1 -> latest </code></td>
 </tr>
 <tr>
 <td>[disable]</td>
 <td><code class="docutils literal notranslate">v6.0.0 -> latest</code></td> <tr>
 <td>[enable]</td>
 <td><code class="docutils literal notranslate">v6.0.0 -> latest</code></td> </table>
 </div>
 </li>
            <li> <span class="li-head">http_cookie_generation</span> - Generation of HTTP cookie to be accepted. Changing invalidates all existing cookies. <span class="li-normal">type: int</span>
 <a id='label20' href="javascript:ContentClick('label21', 'label20');" onmouseover="ContentPreview('label21');" onmouseout="ContentUnpreview('label21');" title="click to collapse or expand..."> more... </a>
 <div id="label21" style="display:none">
 <table border="1">
 <tr>
 <td></td>
 <td colspan="1">Supported Version Ranges</td>
 </tr>
 <tr>
 <td>http_cookie_generation</td>
 <td><code class="docutils literal notranslate">v7.0.1 -> latest </code></td>
 </tr>
 </table>
 </div>
 </li>
            <li> <span class="li-head">http_cookie_path</span> - Limit HTTP cookie persistence to the specified path. <span class="li-normal">type: str</span>
 <a id='label22' href="javascript:ContentClick('label23', 'label22');" onmouseover="ContentPreview('label23');" onmouseout="ContentUnpreview('label23');" title="click to collapse or expand..."> more... </a>
 <div id="label23" style="display:none">
 <table border="1">
 <tr>
 <td></td>
 <td colspan="1">Supported Version Ranges</td>
 </tr>
 <tr>
 <td>http_cookie_path</td>
 <td><code class="docutils literal notranslate">v7.0.1 -> latest </code></td>
 </tr>
 </table>
 </div>
 </li>
            <li> <span class="li-head">http_cookie_share</span> - Control sharing of cookies across API Gateway. Use of same-ip means a cookie from one virtual server can be used by another. Disable stops cookie sharing. <span class="li-normal">type: str</span> <span class="li-normal">choices: disable, same-ip</span>
 <a id='label24' href="javascript:ContentClick('label25', 'label24');" onmouseover="ContentPreview('label25');" onmouseout="ContentUnpreview('label25');" title="click to collapse or expand..."> more... </a>
 <div id="label25" style="display:none">
 <table border="1">
 <tr>
 <td></td>
 <td colspan="1">Supported Version Ranges</td>
 </tr>
 <tr>
 <td>http_cookie_share</td>
 <td><code class="docutils literal notranslate">v7.0.1 -> latest </code></td>
 </tr>
 <tr>
 <td>[disable]</td>
 <td><code class="docutils literal notranslate">v6.0.0 -> latest</code></td> <tr>
 <td>[same-ip]</td>
 <td><code class="docutils literal notranslate">v6.0.0 -> latest</code></td> </table>
 </div>
 </li>
            <li> <span class="li-head">https_cookie_secure</span> - Enable/disable verification that inserted HTTPS cookies are secure. <span class="li-normal">type: str</span> <span class="li-normal">choices: disable, enable</span>
 <a id='label26' href="javascript:ContentClick('label27', 'label26');" onmouseover="ContentPreview('label27');" onmouseout="ContentUnpreview('label27');" title="click to collapse or expand..."> more... </a>
 <div id="label27" style="display:none">
 <table border="1">
 <tr>
 <td></td>
 <td colspan="1">Supported Version Ranges</td>
 </tr>
 <tr>
 <td>https_cookie_secure</td>
 <td><code class="docutils literal notranslate">v7.0.1 -> latest </code></td>
 </tr>
 <tr>
 <td>[disable]</td>
 <td><code class="docutils literal notranslate">v6.0.0 -> latest</code></td> <tr>
 <td>[enable]</td>
 <td><code class="docutils literal notranslate">v6.0.0 -> latest</code></td> </table>
 </div>
 </li>
            <li> <span class="li-head">id</span> - API Gateway ID. see <a href='#notes'>Notes</a>. <span class="li-normal">type: int</span> <span class="li-required">required: true</span>
 <a id='label28' href="javascript:ContentClick('label29', 'label28');" onmouseover="ContentPreview('label29');" onmouseout="ContentUnpreview('label29');" title="click to collapse or expand..."> more... </a>
 <div id="label29" style="display:none">
 <table border="1">
 <tr>
 <td></td>
 <td colspan="1">Supported Version Ranges</td>
 </tr>
 <tr>
 <td>id</td>
 <td><code class="docutils literal notranslate">v7.0.1 -> latest </code></td>
 </tr>
 </table>
 </div>
 </li>
            <li> <span class="li-head">ldb_method</span> - Method used to distribute sessions to real servers. <span class="li-normal">type: str</span> <span class="li-normal">choices: static, round-robin, weighted, first-alive, http-host</span>
 <a id='label30' href="javascript:ContentClick('label31', 'label30');" onmouseover="ContentPreview('label31');" onmouseout="ContentUnpreview('label31');" title="click to collapse or expand..."> more... </a>
 <div id="label31" style="display:none">
 <table border="1">
 <tr>
 <td></td>
 <td colspan="1">Supported Version Ranges</td>
 </tr>
 <tr>
 <td>ldb_method</td>
 <td><code class="docutils literal notranslate">v7.0.1 -> latest </code></td>
 </tr>
 <tr>
 <td>[static]</td>
 <td><code class="docutils literal notranslate">v6.0.0 -> latest</code></td> <tr>
 <td>[round-robin]</td>
 <td><code class="docutils literal notranslate">v6.0.0 -> latest</code></td> <tr>
 <td>[weighted]</td>
 <td><code class="docutils literal notranslate">v6.0.0 -> latest</code></td> <tr>
 <td>[first-alive]</td>
 <td><code class="docutils literal notranslate">v6.0.0 -> latest</code></td> <tr>
 <td>[http-host]</td>
 <td><code class="docutils literal notranslate">v6.0.0 -> latest</code></td> </table>
 </div>
 </li>
            <li> <span class="li-head">persistence</span> - Configure how to make sure that clients connect to the same server every time they make a request that is part of the same session. <span class="li-normal">type: str</span> <span class="li-normal">choices: none, http-cookie</span>
 <a id='label32' href="javascript:ContentClick('label33', 'label32');" onmouseover="ContentPreview('label33');" onmouseout="ContentUnpreview('label33');" title="click to collapse or expand..."> more... </a>
 <div id="label33" style="display:none">
 <table border="1">
 <tr>
 <td></td>
 <td colspan="1">Supported Version Ranges</td>
 </tr>
 <tr>
 <td>persistence</td>
 <td><code class="docutils literal notranslate">v7.0.1 -> latest </code></td>
 </tr>
 <tr>
 <td>[none]</td>
 <td><code class="docutils literal notranslate">v6.0.0 -> latest</code></td> <tr>
 <td>[http-cookie]</td>
 <td><code class="docutils literal notranslate">v6.0.0 -> latest</code></td> </table>
 </div>
 </li>
            <li> <span class="li-head">quic</span> - QUIC setting. <span class="li-normal">type: dict</span>
 <a id='label34' href="javascript:ContentClick('label35', 'label34');" onmouseover="ContentPreview('label35');" onmouseout="ContentUnpreview('label35');" title="click to collapse or expand..."> more... </a>
 <div id="label35" style="display:none">
 <table border="1">
 <tr>
 <td></td><td colspan="1">Supported Version Ranges</td>
 </tr>
 <tr>
 <td>quic</td>
 <td><code class="docutils literal notranslate">v7.4.1 -> latest </code></td>
 </tr>
 </table>
 </div>
 </li>
                <ul class="ul-self">
                <li> <span class="li-head">ack_delay_exponent</span> - ACK delay exponent (1 - 20). <span class="li-normal">type: int</span>
 <a id='label36' href="javascript:ContentClick('label37', 'label36');" onmouseover="ContentPreview('label37');" onmouseout="ContentUnpreview('label37');" title="click to collapse or expand..."> more... </a>
 <div id="label37" style="display:none">
 <table border="1">
 <tr>
 <td></td>
 <td colspan="1">Supported Version Ranges</td>
 </tr>
 <tr>
 <td>ack_delay_exponent</td>
 <td><code class="docutils literal notranslate">v7.4.1 -> latest </code></td>
 </tr>
 </table>
 </div>
 </li>
                <li> <span class="li-head">active_connection_id_limit</span> - Active connection ID limit (1 - 8). <span class="li-normal">type: int</span>
 <a id='label38' href="javascript:ContentClick('label39', 'label38');" onmouseover="ContentPreview('label39');" onmouseout="ContentUnpreview('label39');" title="click to collapse or expand..."> more... </a>
 <div id="label39" style="display:none">
 <table border="1">
 <tr>
 <td></td>
 <td colspan="1">Supported Version Ranges</td>
 </tr>
 <tr>
 <td>active_connection_id_limit</td>
 <td><code class="docutils literal notranslate">v7.4.1 -> latest </code></td>
 </tr>
 </table>
 </div>
 </li>
                <li> <span class="li-head">active_migration</span> - Enable/disable active migration . <span class="li-normal">type: str</span> <span class="li-normal">choices: enable, disable</span>
 <a id='label40' href="javascript:ContentClick('label41', 'label40');" onmouseover="ContentPreview('label41');" onmouseout="ContentUnpreview('label41');" title="click to collapse or expand..."> more... </a>
 <div id="label41" style="display:none">
 <table border="1">
 <tr>
 <td></td>
 <td colspan="1">Supported Version Ranges</td>
 </tr>
 <tr>
 <td>active_migration</td>
 <td><code class="docutils literal notranslate">v7.4.1 -> latest </code></td>
 </tr>
 <tr>
 <td>[enable]</td>
 <td><code class="docutils literal notranslate">v6.0.0 -> latest</code></td> <tr>
 <td>[disable]</td>
 <td><code class="docutils literal notranslate">v6.0.0 -> latest</code></td> </table>
 </div>
 </li>
                <li> <span class="li-head">grease_quic_bit</span> - Enable/disable grease QUIC bit . <span class="li-normal">type: str</span> <span class="li-normal">choices: enable, disable</span>
 <a id='label42' href="javascript:ContentClick('label43', 'label42');" onmouseover="ContentPreview('label43');" onmouseout="ContentUnpreview('label43');" title="click to collapse or expand..."> more... </a>
 <div id="label43" style="display:none">
 <table border="1">
 <tr>
 <td></td>
 <td colspan="1">Supported Version Ranges</td>
 </tr>
 <tr>
 <td>grease_quic_bit</td>
 <td><code class="docutils literal notranslate">v7.4.1 -> latest </code></td>
 </tr>
 <tr>
 <td>[enable]</td>
 <td><code class="docutils literal notranslate">v6.0.0 -> latest</code></td> <tr>
 <td>[disable]</td>
 <td><code class="docutils literal notranslate">v6.0.0 -> latest</code></td> </table>
 </div>
 </li>
                <li> <span class="li-head">max_ack_delay</span> - Maximum ACK delay in milliseconds (1 - 16383). <span class="li-normal">type: int</span>
 <a id='label44' href="javascript:ContentClick('label45', 'label44');" onmouseover="ContentPreview('label45');" onmouseout="ContentUnpreview('label45');" title="click to collapse or expand..."> more... </a>
 <div id="label45" style="display:none">
 <table border="1">
 <tr>
 <td></td>
 <td colspan="1">Supported Version Ranges</td>
 </tr>
 <tr>
 <td>max_ack_delay</td>
 <td><code class="docutils literal notranslate">v7.4.1 -> latest </code></td>
 </tr>
 </table>
 </div>
 </li>
                <li> <span class="li-head">max_datagram_frame_size</span> - Maximum datagram frame size in bytes (1 - 1500). <span class="li-normal">type: int</span>
 <a id='label46' href="javascript:ContentClick('label47', 'label46');" onmouseover="ContentPreview('label47');" onmouseout="ContentUnpreview('label47');" title="click to collapse or expand..."> more... </a>
 <div id="label47" style="display:none">
 <table border="1">
 <tr>
 <td></td>
 <td colspan="1">Supported Version Ranges</td>
 </tr>
 <tr>
 <td>max_datagram_frame_size</td>
 <td><code class="docutils literal notranslate">v7.4.1 -> latest </code></td>
 </tr>
 </table>
 </div>
 </li>
                <li> <span class="li-head">max_idle_timeout</span> - Maximum idle timeout milliseconds (1 - 60000). <span class="li-normal">type: int</span>
 <a id='label48' href="javascript:ContentClick('label49', 'label48');" onmouseover="ContentPreview('label49');" onmouseout="ContentUnpreview('label49');" title="click to collapse or expand..."> more... </a>
 <div id="label49" style="display:none">
 <table border="1">
 <tr>
 <td></td>
 <td colspan="1">Supported Version Ranges</td>
 </tr>
 <tr>
 <td>max_idle_timeout</td>
 <td><code class="docutils literal notranslate">v7.4.1 -> latest </code></td>
 </tr>
 </table>
 </div>
 </li>
                <li> <span class="li-head">max_udp_payload_size</span> - Maximum UDP payload size in bytes (1200 - 1500). <span class="li-normal">type: int</span>
 <a id='label50' href="javascript:ContentClick('label51', 'label50');" onmouseover="ContentPreview('label51');" onmouseout="ContentUnpreview('label51');" title="click to collapse or expand..."> more... </a>
 <div id="label51" style="display:none">
 <table border="1">
 <tr>
 <td></td>
 <td colspan="1">Supported Version Ranges</td>
 </tr>
 <tr>
 <td>max_udp_payload_size</td>
 <td><code class="docutils literal notranslate">v7.4.1 -> latest </code></td>
 </tr>
 </table>
 </div>
 </li>
                </ul>
            <li> <span class="li-head">realservers</span> - Select the real servers that this Access Proxy will distribute traffic to. <span class="li-normal">type: list</span> <span style="font-family:'Courier New'" class="li-required">member_path: api_gateway:id/realservers:id</span>
 <a id='label52' href="javascript:ContentClick('label53', 'label52');" onmouseover="ContentPreview('label53');" onmouseout="ContentUnpreview('label53');" title="click to collapse or expand..."> more... </a>
 <div id="label53" style="display:none">
 <table border="1">
 <tr>
 <td></td><td colspan="1">Supported Version Ranges</td>
 </tr>
 <tr>
 <td>realservers</td>
 <td><code class="docutils literal notranslate">v7.0.1 -> latest </code></td>
 </tr>
 </table>
 </div>
 </li>
                <ul class="ul-self">
                <li> <span class="li-head">addr_type</span> - Type of address. <span class="li-normal">type: str</span> <span class="li-normal">choices: ip, fqdn</span>
 <a id='label54' href="javascript:ContentClick('label55', 'label54');" onmouseover="ContentPreview('label55');" onmouseout="ContentUnpreview('label55');" title="click to collapse or expand..."> more... </a>
 <div id="label55" style="display:none">
 <table border="1">
 <tr>
 <td></td>
 <td colspan="1">Supported Version Ranges</td>
 </tr>
 <tr>
 <td>addr_type</td>
 <td><code class="docutils literal notranslate">v7.0.2 -> latest </code></td>
 </tr>
 <tr>
 <td>[ip]</td>
 <td><code class="docutils literal notranslate">v6.0.0 -> latest</code></td> <tr>
 <td>[fqdn]</td>
 <td><code class="docutils literal notranslate">v6.0.0 -> latest</code></td> </table>
 </div>
 </li>
                <li> <span class="li-head">address</span> - Address or address group of the real server. Source firewall.address.name firewall.addrgrp.name. <span class="li-normal">type: str</span>
 <a id='label56' href="javascript:ContentClick('label57', 'label56');" onmouseover="ContentPreview('label57');" onmouseout="ContentUnpreview('label57');" title="click to collapse or expand..."> more... </a>
 <div id="label57" style="display:none">
 <table border="1">
 <tr>
 <td></td>
 <td colspan="1">Supported Version Ranges</td>
 </tr>
 <tr>
 <td>address</td>
 <td><code class="docutils literal notranslate">v7.0.1 -> latest </code></td>
 </tr>
 </table>
 </div>
 </li>
                <li> <span class="li-head">domain</span> - Wildcard domain name of the real server. <span class="li-normal">type: str</span>
 <a id='label58' href="javascript:ContentClick('label59', 'label58');" onmouseover="ContentPreview('label59');" onmouseout="ContentUnpreview('label59');" title="click to collapse or expand..."> more... </a>
 <div id="label59" style="display:none">
 <table border="1">
 <tr>
 <td></td>
 <td colspan="1">Supported Version Ranges</td>
 </tr>
 <tr>
 <td>domain</td>
 <td><code class="docutils literal notranslate">v7.0.4 -> latest </code></td>
 </tr>
 </table>
 </div>
 </li>
                <li> <span class="li-head">external_auth</span> - Enable/disable use of external browser as user-agent for SAML user authentication. <span class="li-normal">type: str</span> <span class="li-normal">choices: enable, disable</span>
 <a id='label60' href="javascript:ContentClick('label61', 'label60');" onmouseover="ContentPreview('label61');" onmouseout="ContentUnpreview('label61');" title="click to collapse or expand..."> more... </a>
 <div id="label61" style="display:none">
 <table border="1">
 <tr>
 <td></td>
 <td colspan="1">Supported Version Ranges</td>
 </tr>
 <tr>
 <td>external_auth</td>
 <td><code class="docutils literal notranslate">v7.4.0 -> latest </code></td>
 </tr>
 <tr>
 <td>[enable]</td>
 <td><code class="docutils literal notranslate">v6.0.0 -> latest</code></td> <tr>
 <td>[disable]</td>
 <td><code class="docutils literal notranslate">v6.0.0 -> latest</code></td> </table>
 </div>
 </li>
                <li> <span class="li-head">health_check</span> - Enable to check the responsiveness of the real server before forwarding traffic. <span class="li-normal">type: str</span> <span class="li-normal">choices: disable, enable</span>
 <a id='label62' href="javascript:ContentClick('label63', 'label62');" onmouseover="ContentPreview('label63');" onmouseout="ContentUnpreview('label63');" title="click to collapse or expand..."> more... </a>
 <div id="label63" style="display:none">
 <table border="1">
 <tr>
 <td></td>
 <td colspan="1">Supported Version Ranges</td>
 </tr>
 <tr>
 <td>health_check</td>
 <td><code class="docutils literal notranslate">v7.0.1 -> latest </code></td>
 </tr>
 <tr>
 <td>[disable]</td>
 <td><code class="docutils literal notranslate">v6.0.0 -> latest</code></td> <tr>
 <td>[enable]</td>
 <td><code class="docutils literal notranslate">v6.0.0 -> latest</code></td> </table>
 </div>
 </li>
                <li> <span class="li-head">health_check_proto</span> - Protocol of the health check monitor to use when polling to determine server"s connectivity status. <span class="li-normal">type: str</span> <span class="li-normal">choices: ping, http, tcp-connect</span>
 <a id='label64' href="javascript:ContentClick('label65', 'label64');" onmouseover="ContentPreview('label65');" onmouseout="ContentUnpreview('label65');" title="click to collapse or expand..."> more... </a>
 <div id="label65" style="display:none">
 <table border="1">
 <tr>
 <td></td>
 <td colspan="1">Supported Version Ranges</td>
 </tr>
 <tr>
 <td>health_check_proto</td>
 <td><code class="docutils literal notranslate">v7.0.1 -> latest </code></td>
 </tr>
 <tr>
 <td>[ping]</td>
 <td><code class="docutils literal notranslate">v6.0.0 -> latest</code></td> <tr>
 <td>[http]</td>
 <td><code class="docutils literal notranslate">v6.0.0 -> latest</code></td> <tr>
 <td>[tcp-connect]</td>
 <td><code class="docutils literal notranslate">v6.0.0 -> latest</code></td> </table>
 </div>
 </li>
                <li> <span class="li-head">holddown_interval</span> - Enable/disable holddown timer. Server will be considered active and reachable once the holddown period has expired (30 seconds). <span class="li-normal">type: str</span> <span class="li-normal">choices: enable, disable</span>
 <a id='label66' href="javascript:ContentClick('label67', 'label66');" onmouseover="ContentPreview('label67');" onmouseout="ContentUnpreview('label67');" title="click to collapse or expand..."> more... </a>
 <div id="label67" style="display:none">
 <table border="1">
 <tr>
 <td></td>
 <td colspan="1">Supported Version Ranges</td>
 </tr>
 <tr>
 <td>holddown_interval</td>
 <td><code class="docutils literal notranslate">v7.0.1 -> latest </code></td>
 </tr>
 <tr>
 <td>[enable]</td>
 <td><code class="docutils literal notranslate">v6.0.0 -> latest</code></td> <tr>
 <td>[disable]</td>
 <td><code class="docutils literal notranslate">v6.0.0 -> latest</code></td> </table>
 </div>
 </li>
                <li> <span class="li-head">http_host</span> - HTTP server domain name in HTTP header. <span class="li-normal">type: str</span>
 <a id='label68' href="javascript:ContentClick('label69', 'label68');" onmouseover="ContentPreview('label69');" onmouseout="ContentUnpreview('label69');" title="click to collapse or expand..."> more... </a>
 <div id="label69" style="display:none">
 <table border="1">
 <tr>
 <td></td>
 <td colspan="1">Supported Version Ranges</td>
 </tr>
 <tr>
 <td>http_host</td>
 <td><code class="docutils literal notranslate">v7.0.1 -> latest </code></td>
 </tr>
 </table>
 </div>
 </li>
                <li> <span class="li-head">id</span> - Real server ID. see <a href='#notes'>Notes</a>. <span class="li-normal">type: int</span> <span class="li-required">required: true</span>
 <a id='label70' href="javascript:ContentClick('label71', 'label70');" onmouseover="ContentPreview('label71');" onmouseout="ContentUnpreview('label71');" title="click to collapse or expand..."> more... </a>
 <div id="label71" style="display:none">
 <table border="1">
 <tr>
 <td></td>
 <td colspan="1">Supported Version Ranges</td>
 </tr>
 <tr>
 <td>id</td>
 <td><code class="docutils literal notranslate">v7.0.1 -> latest </code></td>
 </tr>
 </table>
 </div>
 </li>
                <li> <span class="li-head">ip</span> - IP address of the real server. <span class="li-normal">type: str</span>
 <a id='label72' href="javascript:ContentClick('label73', 'label72');" onmouseover="ContentPreview('label73');" onmouseout="ContentUnpreview('label73');" title="click to collapse or expand..."> more... </a>
 <div id="label73" style="display:none">
 <table border="1">
 <tr>
 <td></td>
 <td colspan="1">Supported Version Ranges</td>
 </tr>
 <tr>
 <td>ip</td>
 <td><code class="docutils literal notranslate">v7.0.1 -> latest </code></td>
 </tr>
 </table>
 </div>
 </li>
                <li> <span class="li-head">mappedport</span> - Port for communicating with the real server. <span class="li-normal">type: str</span>
 <a id='label74' href="javascript:ContentClick('label75', 'label74');" onmouseover="ContentPreview('label75');" onmouseout="ContentUnpreview('label75');" title="click to collapse or expand..."> more... </a>
 <div id="label75" style="display:none">
 <table border="1">
 <tr>
 <td></td>
 <td colspan="1">Supported Version Ranges</td>
 </tr>
 <tr>
 <td>mappedport</td>
 <td><code class="docutils literal notranslate">v7.0.1 -> latest </code></td>
 </tr>
 </table>
 </div>
 </li>
                <li> <span class="li-head">port</span> - Port for communicating with the real server. <span class="li-normal">type: int</span>
 <a id='label76' href="javascript:ContentClick('label77', 'label76');" onmouseover="ContentPreview('label77');" onmouseout="ContentUnpreview('label77');" title="click to collapse or expand..."> more... </a>
 <div id="label77" style="display:none">
 <table border="1">
 <tr>
 <td></td>
 <td colspan="1">Supported Version Ranges</td>
 </tr>
 <tr>
 <td>port</td>
 <td><code class="docutils literal notranslate">v7.0.1 -> latest </code></td>
 </tr>
 </table>
 </div>
 </li>
                <li> <span class="li-head">ssh_client_cert</span> - Set access-proxy SSH client certificate profile. Source firewall.access-proxy-ssh-client-cert.name. <span class="li-normal">type: str</span>
 <a id='label78' href="javascript:ContentClick('label79', 'label78');" onmouseover="ContentPreview('label79');" onmouseout="ContentUnpreview('label79');" title="click to collapse or expand..."> more... </a>
 <div id="label79" style="display:none">
 <table border="1">
 <tr>
 <td></td>
 <td colspan="1">Supported Version Ranges</td>
 </tr>
 <tr>
 <td>ssh_client_cert</td>
 <td><code class="docutils literal notranslate">v7.0.1 -> latest </code></td>
 </tr>
 </table>
 </div>
 </li>
                <li> <span class="li-head">ssh_host_key</span> - One or more server host key. <span class="li-normal">type: list</span> <span style="font-family:'Courier New'" class="li-required">member_path: api_gateway:id/realservers:id/ssh_host_key:name</span>
 <a id='label80' href="javascript:ContentClick('label81', 'label80');" onmouseover="ContentPreview('label81');" onmouseout="ContentUnpreview('label81');" title="click to collapse or expand..."> more... </a>
 <div id="label81" style="display:none">
 <table border="1">
 <tr>
 <td></td><td colspan="1">Supported Version Ranges</td>
 </tr>
 <tr>
 <td>ssh_host_key</td>
 <td><code class="docutils literal notranslate">v7.0.1 -> latest </code></td>
 </tr>
 </table>
 </div>
 </li>
                    <ul class="ul-self">
                    <li> <span class="li-head">name</span> - Server host key name. Source firewall.ssh.host-key.name. <span class="li-normal">type: str</span> <span class="li-required">required: true</span>
 <a id='label82' href="javascript:ContentClick('label83', 'label82');" onmouseover="ContentPreview('label83');" onmouseout="ContentUnpreview('label83');" title="click to collapse or expand..."> more... </a>
 <div id="label83" style="display:none">
 <table border="1">
 <tr>
 <td></td>
 <td colspan="1">Supported Version Ranges</td>
 </tr>
 <tr>
 <td>name</td>
 <td><code class="docutils literal notranslate">v7.0.1 -> latest </code></td>
 </tr>
 </table>
 </div>
 </li>
                    </ul>
                <li> <span class="li-head">ssh_host_key_validation</span> - Enable/disable SSH real server host key validation. <span class="li-normal">type: str</span> <span class="li-normal">choices: disable, enable</span>
 <a id='label84' href="javascript:ContentClick('label85', 'label84');" onmouseover="ContentPreview('label85');" onmouseout="ContentUnpreview('label85');" title="click to collapse or expand..."> more... </a>
 <div id="label85" style="display:none">
 <table border="1">
 <tr>
 <td></td>
 <td colspan="1">Supported Version Ranges</td>
 </tr>
 <tr>
 <td>ssh_host_key_validation</td>
 <td><code class="docutils literal notranslate">v7.0.1 -> latest </code></td>
 </tr>
 <tr>
 <td>[disable]</td>
 <td><code class="docutils literal notranslate">v6.0.0 -> latest</code></td> <tr>
 <td>[enable]</td>
 <td><code class="docutils literal notranslate">v6.0.0 -> latest</code></td> </table>
 </div>
 </li>
                <li> <span class="li-head">status</span> - Set the status of the real server to active so that it can accept traffic, or on standby or disabled so no traffic is sent. <span class="li-normal">type: str</span> <span class="li-normal">choices: active, standby, disable</span>
 <a id='label86' href="javascript:ContentClick('label87', 'label86');" onmouseover="ContentPreview('label87');" onmouseout="ContentUnpreview('label87');" title="click to collapse or expand..."> more... </a>
 <div id="label87" style="display:none">
 <table border="1">
 <tr>
 <td></td>
 <td colspan="1">Supported Version Ranges</td>
 </tr>
 <tr>
 <td>status</td>
 <td><code class="docutils literal notranslate">v7.0.1 -> latest </code></td>
 </tr>
 <tr>
 <td>[active]</td>
 <td><code class="docutils literal notranslate">v6.0.0 -> latest</code></td> <tr>
 <td>[standby]</td>
 <td><code class="docutils literal notranslate">v6.0.0 -> latest</code></td> <tr>
 <td>[disable]</td>
 <td><code class="docutils literal notranslate">v6.0.0 -> latest</code></td> </table>
 </div>
 </li>
                <li> <span class="li-head">translate_host</span> - Enable/disable translation of hostname/IP from virtual server to real server. <span class="li-normal">type: str</span> <span class="li-normal">choices: enable, disable</span>
 <a id='label88' href="javascript:ContentClick('label89', 'label88');" onmouseover="ContentPreview('label89');" onmouseout="ContentUnpreview('label89');" title="click to collapse or expand..."> more... </a>
 <div id="label89" style="display:none">
 <table border="1">
 <tr>
 <td></td>
 <td colspan="1">Supported Version Ranges</td>
 </tr>
 <tr>
 <td>translate_host</td>
 <td><code class="docutils literal notranslate">v7.2.4 -> latest </code></td>
 </tr>
 <tr>
 <td>[enable]</td>
 <td><code class="docutils literal notranslate">v6.0.0 -> latest</code></td> <tr>
 <td>[disable]</td>
 <td><code class="docutils literal notranslate">v6.0.0 -> latest</code></td> </table>
 </div>
 </li>
                <li> <span class="li-head">tunnel_encryption</span> - Tunnel encryption. <span class="li-normal">type: str</span> <span class="li-normal">choices: enable, disable</span>
 <a id='label90' href="javascript:ContentClick('label91', 'label90');" onmouseover="ContentPreview('label91');" onmouseout="ContentUnpreview('label91');" title="click to collapse or expand..."> more... </a>
 <div id="label91" style="display:none">
 <table border="1">
 <tr>
 <td></td>
 <td colspan="1">Supported Version Ranges</td>
 </tr>
 <tr>
 <td>tunnel_encryption</td>
 <td><code class="docutils literal notranslate">v7.4.0 -> latest </code></td>
 </tr>
 <tr>
 <td>[enable]</td>
 <td><code class="docutils literal notranslate">v6.0.0 -> latest</code></td> <tr>
 <td>[disable]</td>
 <td><code class="docutils literal notranslate">v6.0.0 -> latest</code></td> </table>
 </div>
 </li>
                <li> <span class="li-head">type</span> - TCP forwarding server type. <span class="li-normal">type: str</span> <span class="li-normal">choices: tcp-forwarding, ssh</span>
 <a id='label92' href="javascript:ContentClick('label93', 'label92');" onmouseover="ContentPreview('label93');" onmouseout="ContentUnpreview('label93');" title="click to collapse or expand..."> more... </a>
 <div id="label93" style="display:none">
 <table border="1">
 <tr>
 <td></td>
 <td colspan="1">Supported Version Ranges</td>
 </tr>
 <tr>
 <td>type</td>
 <td><code class="docutils literal notranslate">v7.0.1 -> latest </code></td>
 </tr>
 <tr>
 <td>[tcp-forwarding]</td>
 <td><code class="docutils literal notranslate">v6.0.0 -> latest</code></td> <tr>
 <td>[ssh]</td>
 <td><code class="docutils literal notranslate">v6.0.0 -> latest</code></td> </table>
 </div>
 </li>
                <li> <span class="li-head">weight</span> - Weight of the real server. If weighted load balancing is enabled, the server with the highest weight gets more connections. <span class="li-normal">type: int</span>
 <a id='label94' href="javascript:ContentClick('label95', 'label94');" onmouseover="ContentPreview('label95');" onmouseout="ContentUnpreview('label95');" title="click to collapse or expand..."> more... </a>
 <div id="label95" style="display:none">
 <table border="1">
 <tr>
 <td></td>
 <td colspan="1">Supported Version Ranges</td>
 </tr>
 <tr>
 <td>weight</td>
 <td><code class="docutils literal notranslate">v7.0.1 -> latest </code></td>
 </tr>
 </table>
 </div>
 </li>
                </ul>
            <li> <span class="li-head">saml_redirect</span> - Enable/disable SAML redirection after successful authentication. <span class="li-normal">type: str</span> <span class="li-normal">choices: disable, enable</span>
 <a id='label96' href="javascript:ContentClick('label97', 'label96');" onmouseover="ContentPreview('label97');" onmouseout="ContentUnpreview('label97');" title="click to collapse or expand..."> more... </a>
 <div id="label97" style="display:none">
 <table border="1">
 <tr>
 <td></td>
 <td colspan="1">Supported Version Ranges</td>
 </tr>
 <tr>
 <td>saml_redirect</td>
 <td><code class="docutils literal notranslate">v7.0.2 -> latest </code></td>
 </tr>
 <tr>
 <td>[disable]</td>
 <td><code class="docutils literal notranslate">v6.0.0 -> latest</code></td> <tr>
 <td>[enable]</td>
 <td><code class="docutils literal notranslate">v6.0.0 -> latest</code></td> </table>
 </div>
 </li>
            <li> <span class="li-head">saml_server</span> - SAML service provider configuration for VIP authentication. Source user.saml.name. <span class="li-normal">type: str</span>
 <a id='label98' href="javascript:ContentClick('label99', 'label98');" onmouseover="ContentPreview('label99');" onmouseout="ContentUnpreview('label99');" title="click to collapse or expand..."> more... </a>
 <div id="label99" style="display:none">
 <table border="1">
 <tr>
 <td></td>
 <td colspan="1">Supported Version Ranges</td>
 </tr>
 <tr>
 <td>saml_server</td>
 <td><code class="docutils literal notranslate">v7.0.1 -> latest </code></td>
 </tr>
 </table>
 </div>
 </li>
            <li> <span class="li-head">service</span> - Service. <span class="li-normal">type: str</span> <span class="li-normal">choices: http, https, tcp-forwarding, samlsp, web-portal, saas</span>
 <a id='label100' href="javascript:ContentClick('label101', 'label100');" onmouseover="ContentPreview('label101');" onmouseout="ContentUnpreview('label101');" title="click to collapse or expand..."> more... </a>
 <div id="label101" style="display:none">
 <table border="1">
 <tr>
 <td></td>
 <td colspan="1">Supported Version Ranges</td>
 </tr>
 <tr>
 <td>service</td>
 <td><code class="docutils literal notranslate">v7.0.1 -> latest </code></td>
 </tr>
 <tr>
 <td>[http]</td>
 <td><code class="docutils literal notranslate">v6.0.0 -> latest</code></td> <tr>
 <td>[https]</td>
 <td><code class="docutils literal notranslate">v6.0.0 -> latest</code></td> <tr>
 <td>[tcp-forwarding]</td>
 <td><code class="docutils literal notranslate">v6.0.0 -> latest</code></td> <tr>
 <td>[samlsp]</td>
 <td><code class="docutils literal notranslate">v6.0.0 -> latest</code></td> <tr>
 <td>[web-portal]</td>
 <td><code class="docutils literal notranslate">v7.0.4 -> latest</code></td>
 </tr>
 <tr>
 <td>[saas]</td>
 <td><code class="docutils literal notranslate">v7.2.1 -> latest</code></td>
 </tr>
 </table>
 </div>
 </li>
            <li> <span class="li-head">ssl_algorithm</span> - Permitted encryption algorithms for the server side of SSL full mode sessions according to encryption strength. <span class="li-normal">type: str</span> <span class="li-normal">choices: high, medium, low</span>
 <a id='label102' href="javascript:ContentClick('label103', 'label102');" onmouseover="ContentPreview('label103');" onmouseout="ContentUnpreview('label103');" title="click to collapse or expand..."> more... </a>
 <div id="label103" style="display:none">
 <table border="1">
 <tr>
 <td></td>
 <td colspan="1">Supported Version Ranges</td>
 </tr>
 <tr>
 <td>ssl_algorithm</td>
 <td><code class="docutils literal notranslate">v7.0.1 -> latest </code></td>
 </tr>
 <tr>
 <td>[high]</td>
 <td><code class="docutils literal notranslate">v6.0.0 -> latest</code></td> <tr>
 <td>[medium]</td>
 <td><code class="docutils literal notranslate">v6.0.0 -> latest</code></td> <tr>
 <td>[low]</td>
 <td><code class="docutils literal notranslate">v6.0.0 -> latest</code></td> </table>
 </div>
 </li>
            <li> <span class="li-head">ssl_cipher_suites</span> - SSL/TLS cipher suites to offer to a server, ordered by priority. <span class="li-normal">type: list</span> <span style="font-family:'Courier New'" class="li-required">member_path: api_gateway:id/ssl_cipher_suites:priority</span>
 <a id='label104' href="javascript:ContentClick('label105', 'label104');" onmouseover="ContentPreview('label105');" onmouseout="ContentUnpreview('label105');" title="click to collapse or expand..."> more... </a>
 <div id="label105" style="display:none">
 <table border="1">
 <tr>
 <td></td><td colspan="1">Supported Version Ranges</td>
 </tr>
 <tr>
 <td>ssl_cipher_suites</td>
 <td><code class="docutils literal notranslate">v7.0.1 -> latest </code></td>
 </tr>
 </table>
 </div>
 </li>
                <ul class="ul-self">
                <li> <span class="li-head">cipher</span> - Cipher suite name. <span class="li-normal">type: str</span> <span class="li-normal">choices: TLS-AES-128-GCM-SHA256, TLS-AES-256-GCM-SHA384, TLS-CHACHA20-POLY1305-SHA256, TLS-ECDHE-RSA-WITH-CHACHA20-POLY1305-SHA256, TLS-ECDHE-ECDSA-WITH-CHACHA20-POLY1305-SHA256, TLS-DHE-RSA-WITH-CHACHA20-POLY1305-SHA256, TLS-DHE-RSA-WITH-AES-128-CBC-SHA, TLS-DHE-RSA-WITH-AES-256-CBC-SHA, TLS-DHE-RSA-WITH-AES-128-CBC-SHA256, TLS-DHE-RSA-WITH-AES-128-GCM-SHA256, TLS-DHE-RSA-WITH-AES-256-CBC-SHA256, TLS-DHE-RSA-WITH-AES-256-GCM-SHA384, TLS-DHE-DSS-WITH-AES-128-CBC-SHA, TLS-DHE-DSS-WITH-AES-256-CBC-SHA, TLS-DHE-DSS-WITH-AES-128-CBC-SHA256, TLS-DHE-DSS-WITH-AES-128-GCM-SHA256, TLS-DHE-DSS-WITH-AES-256-CBC-SHA256, TLS-DHE-DSS-WITH-AES-256-GCM-SHA384, TLS-ECDHE-RSA-WITH-AES-128-CBC-SHA, TLS-ECDHE-RSA-WITH-AES-128-CBC-SHA256, TLS-ECDHE-RSA-WITH-AES-128-GCM-SHA256, TLS-ECDHE-RSA-WITH-AES-256-CBC-SHA, TLS-ECDHE-RSA-WITH-AES-256-CBC-SHA384, TLS-ECDHE-RSA-WITH-AES-256-GCM-SHA384, TLS-ECDHE-ECDSA-WITH-AES-128-CBC-SHA, TLS-ECDHE-ECDSA-WITH-AES-128-CBC-SHA256, TLS-ECDHE-ECDSA-WITH-AES-128-GCM-SHA256, TLS-ECDHE-ECDSA-WITH-AES-256-CBC-SHA, TLS-ECDHE-ECDSA-WITH-AES-256-CBC-SHA384, TLS-ECDHE-ECDSA-WITH-AES-256-GCM-SHA384, TLS-RSA-WITH-AES-128-CBC-SHA, TLS-RSA-WITH-AES-256-CBC-SHA, TLS-RSA-WITH-AES-128-CBC-SHA256, TLS-RSA-WITH-AES-128-GCM-SHA256, TLS-RSA-WITH-AES-256-CBC-SHA256, TLS-RSA-WITH-AES-256-GCM-SHA384, TLS-RSA-WITH-CAMELLIA-128-CBC-SHA, TLS-RSA-WITH-CAMELLIA-256-CBC-SHA, TLS-RSA-WITH-CAMELLIA-128-CBC-SHA256, TLS-RSA-WITH-CAMELLIA-256-CBC-SHA256, TLS-DHE-RSA-WITH-3DES-EDE-CBC-SHA, TLS-DHE-RSA-WITH-CAMELLIA-128-CBC-SHA, TLS-DHE-DSS-WITH-CAMELLIA-128-CBC-SHA, TLS-DHE-RSA-WITH-CAMELLIA-256-CBC-SHA, TLS-DHE-DSS-WITH-CAMELLIA-256-CBC-SHA, TLS-DHE-RSA-WITH-CAMELLIA-128-CBC-SHA256, TLS-DHE-DSS-WITH-CAMELLIA-128-CBC-SHA256, TLS-DHE-RSA-WITH-CAMELLIA-256-CBC-SHA256, TLS-DHE-DSS-WITH-CAMELLIA-256-CBC-SHA256, TLS-DHE-RSA-WITH-SEED-CBC-SHA, TLS-DHE-DSS-WITH-SEED-CBC-SHA, TLS-DHE-RSA-WITH-ARIA-128-CBC-SHA256, TLS-DHE-RSA-WITH-ARIA-256-CBC-SHA384, TLS-DHE-DSS-WITH-ARIA-128-CBC-SHA256, TLS-DHE-DSS-WITH-ARIA-256-CBC-SHA384, TLS-RSA-WITH-SEED-CBC-SHA, TLS-RSA-WITH-ARIA-128-CBC-SHA256, TLS-RSA-WITH-ARIA-256-CBC-SHA384, TLS-ECDHE-RSA-WITH-ARIA-128-CBC-SHA256, TLS-ECDHE-RSA-WITH-ARIA-256-CBC-SHA384, TLS-ECDHE-ECDSA-WITH-ARIA-128-CBC-SHA256, TLS-ECDHE-ECDSA-WITH-ARIA-256-CBC-SHA384, TLS-ECDHE-RSA-WITH-RC4-128-SHA, TLS-ECDHE-RSA-WITH-3DES-EDE-CBC-SHA, TLS-DHE-DSS-WITH-3DES-EDE-CBC-SHA, TLS-RSA-WITH-3DES-EDE-CBC-SHA, TLS-RSA-WITH-RC4-128-MD5, TLS-RSA-WITH-RC4-128-SHA, TLS-DHE-RSA-WITH-DES-CBC-SHA, TLS-DHE-DSS-WITH-DES-CBC-SHA, TLS-RSA-WITH-DES-CBC-SHA</span>
 <a id='label106' href="javascript:ContentClick('label107', 'label106');" onmouseover="ContentPreview('label107');" onmouseout="ContentUnpreview('label107');" title="click to collapse or expand..."> more... </a>
 <div id="label107" style="display:none">
 <table border="1">
 <tr>
 <td></td>
 <td colspan="1">Supported Version Ranges</td>
 </tr>
 <tr>
 <td>cipher</td>
 <td><code class="docutils literal notranslate">v7.0.1 -> latest </code></td>
 </tr>
 <tr>
 <td>[TLS-AES-128-GCM-SHA256]</td>
 <td><code class="docutils literal notranslate">v6.0.0 -> latest</code></td> <tr>
 <td>[TLS-AES-256-GCM-SHA384]</td>
 <td><code class="docutils literal notranslate">v6.0.0 -> latest</code></td> <tr>
 <td>[TLS-CHACHA20-POLY1305-SHA256]</td>
 <td><code class="docutils literal notranslate">v6.0.0 -> latest</code></td> <tr>
 <td>[TLS-ECDHE-RSA-WITH-CHACHA20-POLY1305-SHA256]</td>
 <td><code class="docutils literal notranslate">v6.0.0 -> latest</code></td> <tr>
 <td>[TLS-ECDHE-ECDSA-WITH-CHACHA20-POLY1305-SHA256]</td>
 <td><code class="docutils literal notranslate">v6.0.0 -> latest</code></td> <tr>
 <td>[TLS-DHE-RSA-WITH-CHACHA20-POLY1305-SHA256]</td>
 <td><code class="docutils literal notranslate">v6.0.0 -> latest</code></td> <tr>
 <td>[TLS-DHE-RSA-WITH-AES-128-CBC-SHA]</td>
 <td><code class="docutils literal notranslate">v6.0.0 -> latest</code></td> <tr>
 <td>[TLS-DHE-RSA-WITH-AES-256-CBC-SHA]</td>
 <td><code class="docutils literal notranslate">v6.0.0 -> latest</code></td> <tr>
 <td>[TLS-DHE-RSA-WITH-AES-128-CBC-SHA256]</td>
 <td><code class="docutils literal notranslate">v6.0.0 -> latest</code></td> <tr>
 <td>[TLS-DHE-RSA-WITH-AES-128-GCM-SHA256]</td>
 <td><code class="docutils literal notranslate">v6.0.0 -> latest</code></td> <tr>
 <td>[TLS-DHE-RSA-WITH-AES-256-CBC-SHA256]</td>
 <td><code class="docutils literal notranslate">v6.0.0 -> latest</code></td> <tr>
 <td>[TLS-DHE-RSA-WITH-AES-256-GCM-SHA384]</td>
 <td><code class="docutils literal notranslate">v6.0.0 -> latest</code></td> <tr>
 <td>[TLS-DHE-DSS-WITH-AES-128-CBC-SHA]</td>
 <td><code class="docutils literal notranslate">v6.0.0 -> latest</code></td> <tr>
 <td>[TLS-DHE-DSS-WITH-AES-256-CBC-SHA]</td>
 <td><code class="docutils literal notranslate">v6.0.0 -> latest</code></td> <tr>
 <td>[TLS-DHE-DSS-WITH-AES-128-CBC-SHA256]</td>
 <td><code class="docutils literal notranslate">v6.0.0 -> latest</code></td> <tr>
 <td>[TLS-DHE-DSS-WITH-AES-128-GCM-SHA256]</td>
 <td><code class="docutils literal notranslate">v6.0.0 -> latest</code></td> <tr>
 <td>[TLS-DHE-DSS-WITH-AES-256-CBC-SHA256]</td>
 <td><code class="docutils literal notranslate">v6.0.0 -> latest</code></td> <tr>
 <td>[TLS-DHE-DSS-WITH-AES-256-GCM-SHA384]</td>
 <td><code class="docutils literal notranslate">v6.0.0 -> latest</code></td> <tr>
 <td>[TLS-ECDHE-RSA-WITH-AES-128-CBC-SHA]</td>
 <td><code class="docutils literal notranslate">v6.0.0 -> latest</code></td> <tr>
 <td>[TLS-ECDHE-RSA-WITH-AES-128-CBC-SHA256]</td>
 <td><code class="docutils literal notranslate">v6.0.0 -> latest</code></td> <tr>
 <td>[TLS-ECDHE-RSA-WITH-AES-128-GCM-SHA256]</td>
 <td><code class="docutils literal notranslate">v6.0.0 -> latest</code></td> <tr>
 <td>[TLS-ECDHE-RSA-WITH-AES-256-CBC-SHA]</td>
 <td><code class="docutils literal notranslate">v6.0.0 -> latest</code></td> <tr>
 <td>[TLS-ECDHE-RSA-WITH-AES-256-CBC-SHA384]</td>
 <td><code class="docutils literal notranslate">v6.0.0 -> latest</code></td> <tr>
 <td>[TLS-ECDHE-RSA-WITH-AES-256-GCM-SHA384]</td>
 <td><code class="docutils literal notranslate">v6.0.0 -> latest</code></td> <tr>
 <td>[TLS-ECDHE-ECDSA-WITH-AES-128-CBC-SHA]</td>
 <td><code class="docutils literal notranslate">v6.0.0 -> latest</code></td> <tr>
 <td>[TLS-ECDHE-ECDSA-WITH-AES-128-CBC-SHA256]</td>
 <td><code class="docutils literal notranslate">v6.0.0 -> latest</code></td> <tr>
 <td>[TLS-ECDHE-ECDSA-WITH-AES-128-GCM-SHA256]</td>
 <td><code class="docutils literal notranslate">v6.0.0 -> latest</code></td> <tr>
 <td>[TLS-ECDHE-ECDSA-WITH-AES-256-CBC-SHA]</td>
 <td><code class="docutils literal notranslate">v6.0.0 -> latest</code></td> <tr>
 <td>[TLS-ECDHE-ECDSA-WITH-AES-256-CBC-SHA384]</td>
 <td><code class="docutils literal notranslate">v6.0.0 -> latest</code></td> <tr>
 <td>[TLS-ECDHE-ECDSA-WITH-AES-256-GCM-SHA384]</td>
 <td><code class="docutils literal notranslate">v6.0.0 -> latest</code></td> <tr>
 <td>[TLS-RSA-WITH-AES-128-CBC-SHA]</td>
 <td><code class="docutils literal notranslate">v6.0.0 -> latest</code></td> <tr>
 <td>[TLS-RSA-WITH-AES-256-CBC-SHA]</td>
 <td><code class="docutils literal notranslate">v6.0.0 -> latest</code></td> <tr>
 <td>[TLS-RSA-WITH-AES-128-CBC-SHA256]</td>
 <td><code class="docutils literal notranslate">v6.0.0 -> latest</code></td> <tr>
 <td>[TLS-RSA-WITH-AES-128-GCM-SHA256]</td>
 <td><code class="docutils literal notranslate">v6.0.0 -> latest</code></td> <tr>
 <td>[TLS-RSA-WITH-AES-256-CBC-SHA256]</td>
 <td><code class="docutils literal notranslate">v6.0.0 -> latest</code></td> <tr>
 <td>[TLS-RSA-WITH-AES-256-GCM-SHA384]</td>
 <td><code class="docutils literal notranslate">v6.0.0 -> latest</code></td> <tr>
 <td>[TLS-RSA-WITH-CAMELLIA-128-CBC-SHA]</td>
 <td><code class="docutils literal notranslate">v6.0.0 -> latest</code></td> <tr>
 <td>[TLS-RSA-WITH-CAMELLIA-256-CBC-SHA]</td>
 <td><code class="docutils literal notranslate">v6.0.0 -> latest</code></td> <tr>
 <td>[TLS-RSA-WITH-CAMELLIA-128-CBC-SHA256]</td>
 <td><code class="docutils literal notranslate">v6.0.0 -> latest</code></td> <tr>
 <td>[TLS-RSA-WITH-CAMELLIA-256-CBC-SHA256]</td>
 <td><code class="docutils literal notranslate">v6.0.0 -> latest</code></td> <tr>
 <td>[TLS-DHE-RSA-WITH-3DES-EDE-CBC-SHA]</td>
 <td><code class="docutils literal notranslate">v6.0.0 -> latest</code></td> <tr>
 <td>[TLS-DHE-RSA-WITH-CAMELLIA-128-CBC-SHA]</td>
 <td><code class="docutils literal notranslate">v6.0.0 -> latest</code></td> <tr>
 <td>[TLS-DHE-DSS-WITH-CAMELLIA-128-CBC-SHA]</td>
 <td><code class="docutils literal notranslate">v6.0.0 -> latest</code></td> <tr>
 <td>[TLS-DHE-RSA-WITH-CAMELLIA-256-CBC-SHA]</td>
 <td><code class="docutils literal notranslate">v6.0.0 -> latest</code></td> <tr>
 <td>[TLS-DHE-DSS-WITH-CAMELLIA-256-CBC-SHA]</td>
 <td><code class="docutils literal notranslate">v6.0.0 -> latest</code></td> <tr>
 <td>[TLS-DHE-RSA-WITH-CAMELLIA-128-CBC-SHA256]</td>
 <td><code class="docutils literal notranslate">v6.0.0 -> latest</code></td> <tr>
 <td>[TLS-DHE-DSS-WITH-CAMELLIA-128-CBC-SHA256]</td>
 <td><code class="docutils literal notranslate">v6.0.0 -> latest</code></td> <tr>
 <td>[TLS-DHE-RSA-WITH-CAMELLIA-256-CBC-SHA256]</td>
 <td><code class="docutils literal notranslate">v6.0.0 -> latest</code></td> <tr>
 <td>[TLS-DHE-DSS-WITH-CAMELLIA-256-CBC-SHA256]</td>
 <td><code class="docutils literal notranslate">v6.0.0 -> latest</code></td> <tr>
 <td>[TLS-DHE-RSA-WITH-SEED-CBC-SHA]</td>
 <td><code class="docutils literal notranslate">v6.0.0 -> latest</code></td> <tr>
 <td>[TLS-DHE-DSS-WITH-SEED-CBC-SHA]</td>
 <td><code class="docutils literal notranslate">v6.0.0 -> latest</code></td> <tr>
 <td>[TLS-DHE-RSA-WITH-ARIA-128-CBC-SHA256]</td>
 <td><code class="docutils literal notranslate">v6.0.0 -> latest</code></td> <tr>
 <td>[TLS-DHE-RSA-WITH-ARIA-256-CBC-SHA384]</td>
 <td><code class="docutils literal notranslate">v6.0.0 -> latest</code></td> <tr>
 <td>[TLS-DHE-DSS-WITH-ARIA-128-CBC-SHA256]</td>
 <td><code class="docutils literal notranslate">v6.0.0 -> latest</code></td> <tr>
 <td>[TLS-DHE-DSS-WITH-ARIA-256-CBC-SHA384]</td>
 <td><code class="docutils literal notranslate">v6.0.0 -> latest</code></td> <tr>
 <td>[TLS-RSA-WITH-SEED-CBC-SHA]</td>
 <td><code class="docutils literal notranslate">v6.0.0 -> latest</code></td> <tr>
 <td>[TLS-RSA-WITH-ARIA-128-CBC-SHA256]</td>
 <td><code class="docutils literal notranslate">v6.0.0 -> latest</code></td> <tr>
 <td>[TLS-RSA-WITH-ARIA-256-CBC-SHA384]</td>
 <td><code class="docutils literal notranslate">v6.0.0 -> latest</code></td> <tr>
 <td>[TLS-ECDHE-RSA-WITH-ARIA-128-CBC-SHA256]</td>
 <td><code class="docutils literal notranslate">v6.0.0 -> latest</code></td> <tr>
 <td>[TLS-ECDHE-RSA-WITH-ARIA-256-CBC-SHA384]</td>
 <td><code class="docutils literal notranslate">v6.0.0 -> latest</code></td> <tr>
 <td>[TLS-ECDHE-ECDSA-WITH-ARIA-128-CBC-SHA256]</td>
 <td><code class="docutils literal notranslate">v6.0.0 -> latest</code></td> <tr>
 <td>[TLS-ECDHE-ECDSA-WITH-ARIA-256-CBC-SHA384]</td>
 <td><code class="docutils literal notranslate">v6.0.0 -> latest</code></td> <tr>
 <td>[TLS-ECDHE-RSA-WITH-RC4-128-SHA]</td>
 <td><code class="docutils literal notranslate">v6.0.0 -> latest</code></td> <tr>
 <td>[TLS-ECDHE-RSA-WITH-3DES-EDE-CBC-SHA]</td>
 <td><code class="docutils literal notranslate">v6.0.0 -> latest</code></td> <tr>
 <td>[TLS-DHE-DSS-WITH-3DES-EDE-CBC-SHA]</td>
 <td><code class="docutils literal notranslate">v6.0.0 -> latest</code></td> <tr>
 <td>[TLS-RSA-WITH-3DES-EDE-CBC-SHA]</td>
 <td><code class="docutils literal notranslate">v6.0.0 -> latest</code></td> <tr>
 <td>[TLS-RSA-WITH-RC4-128-MD5]</td>
 <td><code class="docutils literal notranslate">v6.0.0 -> latest</code></td> <tr>
 <td>[TLS-RSA-WITH-RC4-128-SHA]</td>
 <td><code class="docutils literal notranslate">v6.0.0 -> latest</code></td> <tr>
 <td>[TLS-DHE-RSA-WITH-DES-CBC-SHA]</td>
 <td><code class="docutils literal notranslate">v6.0.0 -> latest</code></td> <tr>
 <td>[TLS-DHE-DSS-WITH-DES-CBC-SHA]</td>
 <td><code class="docutils literal notranslate">v6.0.0 -> latest</code></td> <tr>
 <td>[TLS-RSA-WITH-DES-CBC-SHA]</td>
 <td><code class="docutils literal notranslate">v6.0.0 -> latest</code></td> </table>
 </div>
 </li>
                <li> <span class="li-head">priority</span> - SSL/TLS cipher suites priority. see <a href='#notes'>Notes</a>. <span class="li-normal">type: int</span> <span class="li-required">required: true</span>
 <a id='label108' href="javascript:ContentClick('label109', 'label108');" onmouseover="ContentPreview('label109');" onmouseout="ContentUnpreview('label109');" title="click to collapse or expand..."> more... </a>
 <div id="label109" style="display:none">
 <table border="1">
 <tr>
 <td></td>
 <td colspan="1">Supported Version Ranges</td>
 </tr>
 <tr>
 <td>priority</td>
 <td><code class="docutils literal notranslate">v7.0.1 -> latest </code></td>
 </tr>
 </table>
 </div>
 </li>
                <li> <span class="li-head">versions</span> - SSL/TLS versions that the cipher suite can be used with. <span class="li-normal">type: list</span> <span class="li-normal">choices: tls-1.0, tls-1.1, tls-1.2, tls-1.3</span>
 <a id='label110' href="javascript:ContentClick('label111', 'label110');" onmouseover="ContentPreview('label111');" onmouseout="ContentUnpreview('label111');" title="click to collapse or expand..."> more... </a>
 <div id="label111" style="display:none">
 <table border="1">
 <tr>
 <td></td>
 <td colspan="1">Supported Version Ranges</td>
 </tr>
 <tr>
 <td>versions</td>
 <td><code class="docutils literal notranslate">v7.0.1 -> latest </code></td>
 </tr>
 <tr>
 <td>[tls-1.0]</td>
 <td><code class="docutils literal notranslate">v6.0.0 -> latest</code></td> <tr>
 <td>[tls-1.1]</td>
 <td><code class="docutils literal notranslate">v6.0.0 -> latest</code></td> <tr>
 <td>[tls-1.2]</td>
 <td><code class="docutils literal notranslate">v6.0.0 -> latest</code></td> <tr>
 <td>[tls-1.3]</td>
 <td><code class="docutils literal notranslate">v6.0.0 -> latest</code></td> </table>
 </div>
 </li>
                </ul>
            <li> <span class="li-head">ssl_dh_bits</span> - Number of bits to use in the Diffie-Hellman exchange for RSA encryption of SSL sessions. <span class="li-normal">type: str</span> <span class="li-normal">choices: 768, 1024, 1536, 2048, 3072, 4096</span>
 <a id='label112' href="javascript:ContentClick('label113', 'label112');" onmouseover="ContentPreview('label113');" onmouseout="ContentUnpreview('label113');" title="click to collapse or expand..."> more... </a>
 <div id="label113" style="display:none">
 <table border="1">
 <tr>
 <td></td>
 <td colspan="1">Supported Version Ranges</td>
 </tr>
 <tr>
 <td>ssl_dh_bits</td>
 <td><code class="docutils literal notranslate">v7.0.1 -> latest </code></td>
 </tr>
 <tr>
 <td>[768]</td>
 <td><code class="docutils literal notranslate">v6.0.0 -> latest</code></td> <tr>
 <td>[1024]</td>
 <td><code class="docutils literal notranslate">v6.0.0 -> latest</code></td> <tr>
 <td>[1536]</td>
 <td><code class="docutils literal notranslate">v6.0.0 -> latest</code></td> <tr>
 <td>[2048]</td>
 <td><code class="docutils literal notranslate">v6.0.0 -> latest</code></td> <tr>
 <td>[3072]</td>
 <td><code class="docutils literal notranslate">v6.0.0 -> latest</code></td> <tr>
 <td>[4096]</td>
 <td><code class="docutils literal notranslate">v6.0.0 -> latest</code></td> </table>
 </div>
 </li>
            <li> <span class="li-head">ssl_max_version</span> - Highest SSL/TLS version acceptable from a server. <span class="li-normal">type: str</span> <span class="li-normal">choices: tls-1.0, tls-1.1, tls-1.2, tls-1.3</span>
 <a id='label114' href="javascript:ContentClick('label115', 'label114');" onmouseover="ContentPreview('label115');" onmouseout="ContentUnpreview('label115');" title="click to collapse or expand..."> more... </a>
 <div id="label115" style="display:none">
 <table border="1">
 <tr>
 <td></td>
 <td colspan="1">Supported Version Ranges</td>
 </tr>
 <tr>
 <td>ssl_max_version</td>
 <td><code class="docutils literal notranslate">v7.0.1 -> latest </code></td>
 </tr>
 <tr>
 <td>[tls-1.0]</td>
 <td><code class="docutils literal notranslate">v6.0.0 -> latest</code></td> <tr>
 <td>[tls-1.1]</td>
 <td><code class="docutils literal notranslate">v6.0.0 -> latest</code></td> <tr>
 <td>[tls-1.2]</td>
 <td><code class="docutils literal notranslate">v6.0.0 -> latest</code></td> <tr>
 <td>[tls-1.3]</td>
 <td><code class="docutils literal notranslate">v6.0.0 -> latest</code></td> </table>
 </div>
 </li>
            <li> <span class="li-head">ssl_min_version</span> - Lowest SSL/TLS version acceptable from a server. <span class="li-normal">type: str</span> <span class="li-normal">choices: tls-1.0, tls-1.1, tls-1.2, tls-1.3</span>
 <a id='label116' href="javascript:ContentClick('label117', 'label116');" onmouseover="ContentPreview('label117');" onmouseout="ContentUnpreview('label117');" title="click to collapse or expand..."> more... </a>
 <div id="label117" style="display:none">
 <table border="1">
 <tr>
 <td></td>
 <td colspan="1">Supported Version Ranges</td>
 </tr>
 <tr>
 <td>ssl_min_version</td>
 <td><code class="docutils literal notranslate">v7.0.1 -> latest </code></td>
 </tr>
 <tr>
 <td>[tls-1.0]</td>
 <td><code class="docutils literal notranslate">v6.0.0 -> latest</code></td> <tr>
 <td>[tls-1.1]</td>
 <td><code class="docutils literal notranslate">v6.0.0 -> latest</code></td> <tr>
 <td>[tls-1.2]</td>
 <td><code class="docutils literal notranslate">v6.0.0 -> latest</code></td> <tr>
 <td>[tls-1.3]</td>
 <td><code class="docutils literal notranslate">v6.0.0 -> latest</code></td> </table>
 </div>
 </li>
            <li> <span class="li-head">ssl_renegotiation</span> - Enable/disable secure renegotiation to comply with RFC 5746. <span class="li-normal">type: str</span> <span class="li-normal">choices: enable, disable</span>
 <a id='label118' href="javascript:ContentClick('label119', 'label118');" onmouseover="ContentPreview('label119');" onmouseout="ContentUnpreview('label119');" title="click to collapse or expand..."> more... </a>
 <div id="label119" style="display:none">
 <table border="1">
 <tr>
 <td></td>
 <td colspan="1">Supported Version Ranges</td>
 </tr>
 <tr>
 <td>ssl_renegotiation</td>
 <td><code class="docutils literal notranslate">v7.2.4 -> latest </code></td>
 </tr>
 <tr>
 <td>[enable]</td>
 <td><code class="docutils literal notranslate">v6.0.0 -> latest</code></td> <tr>
 <td>[disable]</td>
 <td><code class="docutils literal notranslate">v6.0.0 -> latest</code></td> </table>
 </div>
 </li>
            <li> <span class="li-head">ssl_vpn_web_portal</span> - SSL-VPN web portal. Source vpn.ssl.web.portal.name. <span class="li-normal">type: str</span>
 <a id='label120' href="javascript:ContentClick('label121', 'label120');" onmouseover="ContentPreview('label121');" onmouseout="ContentUnpreview('label121');" title="click to collapse or expand..."> more... </a>
 <div id="label121" style="display:none">
 <table border="1">
 <tr>
 <td></td>
 <td colspan="1">Supported Version Ranges</td>
 </tr>
 <tr>
 <td>ssl_vpn_web_portal</td>
 <td><code class="docutils literal notranslate">v7.0.4 -> latest </code></td>
 </tr>
 </table>
 </div>
 </li>
            <li> <span class="li-head">url_map</span> - URL pattern to match. <span class="li-normal">type: str</span>
 <a id='label122' href="javascript:ContentClick('label123', 'label122');" onmouseover="ContentPreview('label123');" onmouseout="ContentUnpreview('label123');" title="click to collapse or expand..."> more... </a>
 <div id="label123" style="display:none">
 <table border="1">
 <tr>
 <td></td>
 <td colspan="1">Supported Version Ranges</td>
 </tr>
 <tr>
 <td>url_map</td>
 <td><code class="docutils literal notranslate">v7.0.1 -> latest </code></td>
 </tr>
 </table>
 </div>
 </li>
            <li> <span class="li-head">url_map_type</span> - Type of url-map. <span class="li-normal">type: str</span> <span class="li-normal">choices: sub-string, wildcard, regex</span>
 <a id='label124' href="javascript:ContentClick('label125', 'label124');" onmouseover="ContentPreview('label125');" onmouseout="ContentUnpreview('label125');" title="click to collapse or expand..."> more... </a>
 <div id="label125" style="display:none">
 <table border="1">
 <tr>
 <td></td>
 <td colspan="1">Supported Version Ranges</td>
 </tr>
 <tr>
 <td>url_map_type</td>
 <td><code class="docutils literal notranslate">v7.0.1 -> latest </code></td>
 </tr>
 <tr>
 <td>[sub-string]</td>
 <td><code class="docutils literal notranslate">v6.0.0 -> latest</code></td> <tr>
 <td>[wildcard]</td>
 <td><code class="docutils literal notranslate">v6.0.0 -> latest</code></td> <tr>
 <td>[regex]</td>
 <td><code class="docutils literal notranslate">v6.0.0 -> latest</code></td> </table>
 </div>
 </li>
            <li> <span class="li-head">virtual_host</span> - Virtual host. Source firewall.access-proxy-virtual-host.name. <span class="li-normal">type: str</span>
 <a id='label126' href="javascript:ContentClick('label127', 'label126');" onmouseover="ContentPreview('label127');" onmouseout="ContentUnpreview('label127');" title="click to collapse or expand..."> more... </a>
 <div id="label127" style="display:none">
 <table border="1">
 <tr>
 <td></td>
 <td colspan="1">Supported Version Ranges</td>
 </tr>
 <tr>
 <td>virtual_host</td>
 <td><code class="docutils literal notranslate">v7.0.1 -> latest </code></td>
 </tr>
 </table>
 </div>
 </li>
            </ul>
        <li> <span class="li-head">api_gateway6</span> - Set IPv6 API Gateway. <span class="li-normal">type: list</span> <span style="font-family:'Courier New'" class="li-required">member_path: api_gateway6:id</span>
 <a id='label128' href="javascript:ContentClick('label129', 'label128');" onmouseover="ContentPreview('label129');" onmouseout="ContentUnpreview('label129');" title="click to collapse or expand..."> more... </a>
 <div id="label129" style="display:none">
 <table border="1">
 <tr>
 <td></td><td colspan="1">Supported Version Ranges</td>
 </tr>
 <tr>
 <td>api_gateway6</td>
 <td><code class="docutils literal notranslate">v7.0.1 -> latest </code></td>
 </tr>
 </table>
 </div>
 </li>
            <ul class="ul-self">
            <li> <span class="li-head">application</span> - SaaS application controlled by this Access Proxy. <span class="li-normal">type: list</span> <span style="font-family:'Courier New'" class="li-required">member_path: api_gateway6:id/application:name</span>
 <a id='label130' href="javascript:ContentClick('label131', 'label130');" onmouseover="ContentPreview('label131');" onmouseout="ContentUnpreview('label131');" title="click to collapse or expand..."> more... </a>
 <div id="label131" style="display:none">
 <table border="1">
 <tr>
 <td></td><td colspan="1">Supported Version Ranges</td>
 </tr>
 <tr>
 <td>application</td>
 <td><code class="docutils literal notranslate">v7.2.1 -> latest </code></td>
 </tr>
 </table>
 </div>
 </li>
                <ul class="ul-self">
                <li> <span class="li-head">name</span> - SaaS application name. <span class="li-normal">type: str</span> <span class="li-required">required: true</span>
 <a id='label132' href="javascript:ContentClick('label133', 'label132');" onmouseover="ContentPreview('label133');" onmouseout="ContentUnpreview('label133');" title="click to collapse or expand..."> more... </a>
 <div id="label133" style="display:none">
 <table border="1">
 <tr>
 <td></td>
 <td colspan="1">Supported Version Ranges</td>
 </tr>
 <tr>
 <td>name</td>
 <td><code class="docutils literal notranslate">v7.2.1 -> latest </code></td>
 </tr>
 </table>
 </div>
 </li>
                </ul>
            <li> <span class="li-head">h2_support</span> - HTTP2 support, default=Enable. <span class="li-normal">type: str</span> <span class="li-normal">choices: enable, disable</span>
 <a id='label134' href="javascript:ContentClick('label135', 'label134');" onmouseover="ContentPreview('label135');" onmouseout="ContentUnpreview('label135');" title="click to collapse or expand..."> more... </a>
 <div id="label135" style="display:none">
 <table border="1">
 <tr>
 <td></td>
 <td colspan="1">Supported Version Ranges</td>
 </tr>
 <tr>
 <td>h2_support</td>
 <td><code class="docutils literal notranslate">v7.4.1 -> latest </code></td>
 </tr>
 <tr>
 <td>[enable]</td>
 <td><code class="docutils literal notranslate">v6.0.0 -> latest</code></td> <tr>
 <td>[disable]</td>
 <td><code class="docutils literal notranslate">v6.0.0 -> latest</code></td> </table>
 </div>
 </li>
            <li> <span class="li-head">h3_support</span> - HTTP3/QUIC support, default=Disable. <span class="li-normal">type: str</span> <span class="li-normal">choices: enable, disable</span>
 <a id='label136' href="javascript:ContentClick('label137', 'label136');" onmouseover="ContentPreview('label137');" onmouseout="ContentUnpreview('label137');" title="click to collapse or expand..."> more... </a>
 <div id="label137" style="display:none">
 <table border="1">
 <tr>
 <td></td>
 <td colspan="1">Supported Version Ranges</td>
 </tr>
 <tr>
 <td>h3_support</td>
 <td><code class="docutils literal notranslate">v7.4.1 -> latest </code></td>
 </tr>
 <tr>
 <td>[enable]</td>
 <td><code class="docutils literal notranslate">v6.0.0 -> latest</code></td> <tr>
 <td>[disable]</td>
 <td><code class="docutils literal notranslate">v6.0.0 -> latest</code></td> </table>
 </div>
 </li>
            <li> <span class="li-head">http_cookie_age</span> - Time in minutes that client web browsers should keep a cookie. Default is 60 minutes. 0 = no time limit. <span class="li-normal">type: int</span>
 <a id='label138' href="javascript:ContentClick('label139', 'label138');" onmouseover="ContentPreview('label139');" onmouseout="ContentUnpreview('label139');" title="click to collapse or expand..."> more... </a>
 <div id="label139" style="display:none">
 <table border="1">
 <tr>
 <td></td>
 <td colspan="1">Supported Version Ranges</td>
 </tr>
 <tr>
 <td>http_cookie_age</td>
 <td><code class="docutils literal notranslate">v7.0.1 -> latest </code></td>
 </tr>
 </table>
 </div>
 </li>
            <li> <span class="li-head">http_cookie_domain</span> - Domain that HTTP cookie persistence should apply to. <span class="li-normal">type: str</span>
 <a id='label140' href="javascript:ContentClick('label141', 'label140');" onmouseover="ContentPreview('label141');" onmouseout="ContentUnpreview('label141');" title="click to collapse or expand..."> more... </a>
 <div id="label141" style="display:none">
 <table border="1">
 <tr>
 <td></td>
 <td colspan="1">Supported Version Ranges</td>
 </tr>
 <tr>
 <td>http_cookie_domain</td>
 <td><code class="docutils literal notranslate">v7.0.1 -> latest </code></td>
 </tr>
 </table>
 </div>
 </li>
            <li> <span class="li-head">http_cookie_domain_from_host</span> - Enable/disable use of HTTP cookie domain from host field in HTTP. <span class="li-normal">type: str</span> <span class="li-normal">choices: disable, enable</span>
 <a id='label142' href="javascript:ContentClick('label143', 'label142');" onmouseover="ContentPreview('label143');" onmouseout="ContentUnpreview('label143');" title="click to collapse or expand..."> more... </a>
 <div id="label143" style="display:none">
 <table border="1">
 <tr>
 <td></td>
 <td colspan="1">Supported Version Ranges</td>
 </tr>
 <tr>
 <td>http_cookie_domain_from_host</td>
 <td><code class="docutils literal notranslate">v7.0.1 -> latest </code></td>
 </tr>
 <tr>
 <td>[disable]</td>
 <td><code class="docutils literal notranslate">v6.0.0 -> latest</code></td> <tr>
 <td>[enable]</td>
 <td><code class="docutils literal notranslate">v6.0.0 -> latest</code></td> </table>
 </div>
 </li>
            <li> <span class="li-head">http_cookie_generation</span> - Generation of HTTP cookie to be accepted. Changing invalidates all existing cookies. <span class="li-normal">type: int</span>
 <a id='label144' href="javascript:ContentClick('label145', 'label144');" onmouseover="ContentPreview('label145');" onmouseout="ContentUnpreview('label145');" title="click to collapse or expand..."> more... </a>
 <div id="label145" style="display:none">
 <table border="1">
 <tr>
 <td></td>
 <td colspan="1">Supported Version Ranges</td>
 </tr>
 <tr>
 <td>http_cookie_generation</td>
 <td><code class="docutils literal notranslate">v7.0.1 -> latest </code></td>
 </tr>
 </table>
 </div>
 </li>
            <li> <span class="li-head">http_cookie_path</span> - Limit HTTP cookie persistence to the specified path. <span class="li-normal">type: str</span>
 <a id='label146' href="javascript:ContentClick('label147', 'label146');" onmouseover="ContentPreview('label147');" onmouseout="ContentUnpreview('label147');" title="click to collapse or expand..."> more... </a>
 <div id="label147" style="display:none">
 <table border="1">
 <tr>
 <td></td>
 <td colspan="1">Supported Version Ranges</td>
 </tr>
 <tr>
 <td>http_cookie_path</td>
 <td><code class="docutils literal notranslate">v7.0.1 -> latest </code></td>
 </tr>
 </table>
 </div>
 </li>
            <li> <span class="li-head">http_cookie_share</span> - Control sharing of cookies across API Gateway. Use of same-ip means a cookie from one virtual server can be used by another. Disable stops cookie sharing. <span class="li-normal">type: str</span> <span class="li-normal">choices: disable, same-ip</span>
 <a id='label148' href="javascript:ContentClick('label149', 'label148');" onmouseover="ContentPreview('label149');" onmouseout="ContentUnpreview('label149');" title="click to collapse or expand..."> more... </a>
 <div id="label149" style="display:none">
 <table border="1">
 <tr>
 <td></td>
 <td colspan="1">Supported Version Ranges</td>
 </tr>
 <tr>
 <td>http_cookie_share</td>
 <td><code class="docutils literal notranslate">v7.0.1 -> latest </code></td>
 </tr>
 <tr>
 <td>[disable]</td>
 <td><code class="docutils literal notranslate">v6.0.0 -> latest</code></td> <tr>
 <td>[same-ip]</td>
 <td><code class="docutils literal notranslate">v6.0.0 -> latest</code></td> </table>
 </div>
 </li>
            <li> <span class="li-head">https_cookie_secure</span> - Enable/disable verification that inserted HTTPS cookies are secure. <span class="li-normal">type: str</span> <span class="li-normal">choices: disable, enable</span>
 <a id='label150' href="javascript:ContentClick('label151', 'label150');" onmouseover="ContentPreview('label151');" onmouseout="ContentUnpreview('label151');" title="click to collapse or expand..."> more... </a>
 <div id="label151" style="display:none">
 <table border="1">
 <tr>
 <td></td>
 <td colspan="1">Supported Version Ranges</td>
 </tr>
 <tr>
 <td>https_cookie_secure</td>
 <td><code class="docutils literal notranslate">v7.0.1 -> latest </code></td>
 </tr>
 <tr>
 <td>[disable]</td>
 <td><code class="docutils literal notranslate">v6.0.0 -> latest</code></td> <tr>
 <td>[enable]</td>
 <td><code class="docutils literal notranslate">v6.0.0 -> latest</code></td> </table>
 </div>
 </li>
            <li> <span class="li-head">id</span> - API Gateway ID. see <a href='#notes'>Notes</a>. <span class="li-normal">type: int</span> <span class="li-required">required: true</span>
 <a id='label152' href="javascript:ContentClick('label153', 'label152');" onmouseover="ContentPreview('label153');" onmouseout="ContentUnpreview('label153');" title="click to collapse or expand..."> more... </a>
 <div id="label153" style="display:none">
 <table border="1">
 <tr>
 <td></td>
 <td colspan="1">Supported Version Ranges</td>
 </tr>
 <tr>
 <td>id</td>
 <td><code class="docutils literal notranslate">v7.0.1 -> latest </code></td>
 </tr>
 </table>
 </div>
 </li>
            <li> <span class="li-head">ldb_method</span> - Method used to distribute sessions to real servers. <span class="li-normal">type: str</span> <span class="li-normal">choices: static, round-robin, weighted, first-alive, http-host</span>
 <a id='label154' href="javascript:ContentClick('label155', 'label154');" onmouseover="ContentPreview('label155');" onmouseout="ContentUnpreview('label155');" title="click to collapse or expand..."> more... </a>
 <div id="label155" style="display:none">
 <table border="1">
 <tr>
 <td></td>
 <td colspan="1">Supported Version Ranges</td>
 </tr>
 <tr>
 <td>ldb_method</td>
 <td><code class="docutils literal notranslate">v7.0.1 -> latest </code></td>
 </tr>
 <tr>
 <td>[static]</td>
 <td><code class="docutils literal notranslate">v6.0.0 -> latest</code></td> <tr>
 <td>[round-robin]</td>
 <td><code class="docutils literal notranslate">v6.0.0 -> latest</code></td> <tr>
 <td>[weighted]</td>
 <td><code class="docutils literal notranslate">v6.0.0 -> latest</code></td> <tr>
 <td>[first-alive]</td>
 <td><code class="docutils literal notranslate">v6.0.0 -> latest</code></td> <tr>
 <td>[http-host]</td>
 <td><code class="docutils literal notranslate">v6.0.0 -> latest</code></td> </table>
 </div>
 </li>
            <li> <span class="li-head">persistence</span> - Configure how to make sure that clients connect to the same server every time they make a request that is part of the same session. <span class="li-normal">type: str</span> <span class="li-normal">choices: none, http-cookie</span>
 <a id='label156' href="javascript:ContentClick('label157', 'label156');" onmouseover="ContentPreview('label157');" onmouseout="ContentUnpreview('label157');" title="click to collapse or expand..."> more... </a>
 <div id="label157" style="display:none">
 <table border="1">
 <tr>
 <td></td>
 <td colspan="1">Supported Version Ranges</td>
 </tr>
 <tr>
 <td>persistence</td>
 <td><code class="docutils literal notranslate">v7.0.1 -> latest </code></td>
 </tr>
 <tr>
 <td>[none]</td>
 <td><code class="docutils literal notranslate">v6.0.0 -> latest</code></td> <tr>
 <td>[http-cookie]</td>
 <td><code class="docutils literal notranslate">v6.0.0 -> latest</code></td> </table>
 </div>
 </li>
            <li> <span class="li-head">quic</span> - QUIC setting. <span class="li-normal">type: dict</span>
 <a id='label158' href="javascript:ContentClick('label159', 'label158');" onmouseover="ContentPreview('label159');" onmouseout="ContentUnpreview('label159');" title="click to collapse or expand..."> more... </a>
 <div id="label159" style="display:none">
 <table border="1">
 <tr>
 <td></td><td colspan="1">Supported Version Ranges</td>
 </tr>
 <tr>
 <td>quic</td>
 <td><code class="docutils literal notranslate">v7.4.1 -> latest </code></td>
 </tr>
 </table>
 </div>
 </li>
                <ul class="ul-self">
                <li> <span class="li-head">ack_delay_exponent</span> - ACK delay exponent (1 - 20). <span class="li-normal">type: int</span>
 <a id='label160' href="javascript:ContentClick('label161', 'label160');" onmouseover="ContentPreview('label161');" onmouseout="ContentUnpreview('label161');" title="click to collapse or expand..."> more... </a>
 <div id="label161" style="display:none">
 <table border="1">
 <tr>
 <td></td>
 <td colspan="1">Supported Version Ranges</td>
 </tr>
 <tr>
 <td>ack_delay_exponent</td>
 <td><code class="docutils literal notranslate">v7.4.1 -> latest </code></td>
 </tr>
 </table>
 </div>
 </li>
                <li> <span class="li-head">active_connection_id_limit</span> - Active connection ID limit (1 - 8). <span class="li-normal">type: int</span>
 <a id='label162' href="javascript:ContentClick('label163', 'label162');" onmouseover="ContentPreview('label163');" onmouseout="ContentUnpreview('label163');" title="click to collapse or expand..."> more... </a>
 <div id="label163" style="display:none">
 <table border="1">
 <tr>
 <td></td>
 <td colspan="1">Supported Version Ranges</td>
 </tr>
 <tr>
 <td>active_connection_id_limit</td>
 <td><code class="docutils literal notranslate">v7.4.1 -> latest </code></td>
 </tr>
 </table>
 </div>
 </li>
                <li> <span class="li-head">active_migration</span> - Enable/disable active migration . <span class="li-normal">type: str</span> <span class="li-normal">choices: enable, disable</span>
 <a id='label164' href="javascript:ContentClick('label165', 'label164');" onmouseover="ContentPreview('label165');" onmouseout="ContentUnpreview('label165');" title="click to collapse or expand..."> more... </a>
 <div id="label165" style="display:none">
 <table border="1">
 <tr>
 <td></td>
 <td colspan="1">Supported Version Ranges</td>
 </tr>
 <tr>
 <td>active_migration</td>
 <td><code class="docutils literal notranslate">v7.4.1 -> latest </code></td>
 </tr>
 <tr>
 <td>[enable]</td>
 <td><code class="docutils literal notranslate">v6.0.0 -> latest</code></td> <tr>
 <td>[disable]</td>
 <td><code class="docutils literal notranslate">v6.0.0 -> latest</code></td> </table>
 </div>
 </li>
                <li> <span class="li-head">grease_quic_bit</span> - Enable/disable grease QUIC bit . <span class="li-normal">type: str</span> <span class="li-normal">choices: enable, disable</span>
 <a id='label166' href="javascript:ContentClick('label167', 'label166');" onmouseover="ContentPreview('label167');" onmouseout="ContentUnpreview('label167');" title="click to collapse or expand..."> more... </a>
 <div id="label167" style="display:none">
 <table border="1">
 <tr>
 <td></td>
 <td colspan="1">Supported Version Ranges</td>
 </tr>
 <tr>
 <td>grease_quic_bit</td>
 <td><code class="docutils literal notranslate">v7.4.1 -> latest </code></td>
 </tr>
 <tr>
 <td>[enable]</td>
 <td><code class="docutils literal notranslate">v6.0.0 -> latest</code></td> <tr>
 <td>[disable]</td>
 <td><code class="docutils literal notranslate">v6.0.0 -> latest</code></td> </table>
 </div>
 </li>
                <li> <span class="li-head">max_ack_delay</span> - Maximum ACK delay in milliseconds (1 - 16383). <span class="li-normal">type: int</span>
 <a id='label168' href="javascript:ContentClick('label169', 'label168');" onmouseover="ContentPreview('label169');" onmouseout="ContentUnpreview('label169');" title="click to collapse or expand..."> more... </a>
 <div id="label169" style="display:none">
 <table border="1">
 <tr>
 <td></td>
 <td colspan="1">Supported Version Ranges</td>
 </tr>
 <tr>
 <td>max_ack_delay</td>
 <td><code class="docutils literal notranslate">v7.4.1 -> latest </code></td>
 </tr>
 </table>
 </div>
 </li>
                <li> <span class="li-head">max_datagram_frame_size</span> - Maximum datagram frame size in bytes (1 - 1500). <span class="li-normal">type: int</span>
 <a id='label170' href="javascript:ContentClick('label171', 'label170');" onmouseover="ContentPreview('label171');" onmouseout="ContentUnpreview('label171');" title="click to collapse or expand..."> more... </a>
 <div id="label171" style="display:none">
 <table border="1">
 <tr>
 <td></td>
 <td colspan="1">Supported Version Ranges</td>
 </tr>
 <tr>
 <td>max_datagram_frame_size</td>
 <td><code class="docutils literal notranslate">v7.4.1 -> latest </code></td>
 </tr>
 </table>
 </div>
 </li>
                <li> <span class="li-head">max_idle_timeout</span> - Maximum idle timeout milliseconds (1 - 60000). <span class="li-normal">type: int</span>
 <a id='label172' href="javascript:ContentClick('label173', 'label172');" onmouseover="ContentPreview('label173');" onmouseout="ContentUnpreview('label173');" title="click to collapse or expand..."> more... </a>
 <div id="label173" style="display:none">
 <table border="1">
 <tr>
 <td></td>
 <td colspan="1">Supported Version Ranges</td>
 </tr>
 <tr>
 <td>max_idle_timeout</td>
 <td><code class="docutils literal notranslate">v7.4.1 -> latest </code></td>
 </tr>
 </table>
 </div>
 </li>
                <li> <span class="li-head">max_udp_payload_size</span> - Maximum UDP payload size in bytes (1200 - 1500). <span class="li-normal">type: int</span>
 <a id='label174' href="javascript:ContentClick('label175', 'label174');" onmouseover="ContentPreview('label175');" onmouseout="ContentUnpreview('label175');" title="click to collapse or expand..."> more... </a>
 <div id="label175" style="display:none">
 <table border="1">
 <tr>
 <td></td>
 <td colspan="1">Supported Version Ranges</td>
 </tr>
 <tr>
 <td>max_udp_payload_size</td>
 <td><code class="docutils literal notranslate">v7.4.1 -> latest </code></td>
 </tr>
 </table>
 </div>
 </li>
                </ul>
            <li> <span class="li-head">realservers</span> - Select the real servers that this Access Proxy will distribute traffic to. <span class="li-normal">type: list</span> <span style="font-family:'Courier New'" class="li-required">member_path: api_gateway6:id/realservers:id</span>
 <a id='label176' href="javascript:ContentClick('label177', 'label176');" onmouseover="ContentPreview('label177');" onmouseout="ContentUnpreview('label177');" title="click to collapse or expand..."> more... </a>
 <div id="label177" style="display:none">
 <table border="1">
 <tr>
 <td></td><td colspan="1">Supported Version Ranges</td>
 </tr>
 <tr>
 <td>realservers</td>
 <td><code class="docutils literal notranslate">v7.0.1 -> latest </code></td>
 </tr>
 </table>
 </div>
 </li>
                <ul class="ul-self">
                <li> <span class="li-head">addr_type</span> - Type of address. <span class="li-normal">type: str</span> <span class="li-normal">choices: ip, fqdn</span>
 <a id='label178' href="javascript:ContentClick('label179', 'label178');" onmouseover="ContentPreview('label179');" onmouseout="ContentUnpreview('label179');" title="click to collapse or expand..."> more... </a>
 <div id="label179" style="display:none">
 <table border="1">
 <tr>
 <td></td>
 <td colspan="1">Supported Version Ranges</td>
 </tr>
 <tr>
 <td>addr_type</td>
 <td><code class="docutils literal notranslate">v7.0.2 -> latest </code></td>
 </tr>
 <tr>
 <td>[ip]</td>
 <td><code class="docutils literal notranslate">v6.0.0 -> latest</code></td> <tr>
 <td>[fqdn]</td>
 <td><code class="docutils literal notranslate">v6.0.0 -> latest</code></td> </table>
 </div>
 </li>
                <li> <span class="li-head">address</span> - Address or address group of the real server. Source firewall.address6.name firewall.addrgrp6.name. <span class="li-normal">type: str</span>
 <a id='label180' href="javascript:ContentClick('label181', 'label180');" onmouseover="ContentPreview('label181');" onmouseout="ContentUnpreview('label181');" title="click to collapse or expand..."> more... </a>
 <div id="label181" style="display:none">
 <table border="1">
 <tr>
 <td></td>
 <td colspan="1">Supported Version Ranges</td>
 </tr>
 <tr>
 <td>address</td>
 <td><code class="docutils literal notranslate">v7.0.1 -> latest </code></td>
 </tr>
 </table>
 </div>
 </li>
                <li> <span class="li-head">domain</span> - Wildcard domain name of the real server. <span class="li-normal">type: str</span>
 <a id='label182' href="javascript:ContentClick('label183', 'label182');" onmouseover="ContentPreview('label183');" onmouseout="ContentUnpreview('label183');" title="click to collapse or expand..."> more... </a>
 <div id="label183" style="display:none">
 <table border="1">
 <tr>
 <td></td>
 <td colspan="1">Supported Version Ranges</td>
 </tr>
 <tr>
 <td>domain</td>
 <td><code class="docutils literal notranslate">v7.0.4 -> latest </code></td>
 </tr>
 </table>
 </div>
 </li>
                <li> <span class="li-head">external_auth</span> - Enable/disable use of external browser as user-agent for SAML user authentication. <span class="li-normal">type: str</span> <span class="li-normal">choices: enable, disable</span>
 <a id='label184' href="javascript:ContentClick('label185', 'label184');" onmouseover="ContentPreview('label185');" onmouseout="ContentUnpreview('label185');" title="click to collapse or expand..."> more... </a>
 <div id="label185" style="display:none">
 <table border="1">
 <tr>
 <td></td>
 <td colspan="1">Supported Version Ranges</td>
 </tr>
 <tr>
 <td>external_auth</td>
 <td><code class="docutils literal notranslate">v7.4.0 -> latest </code></td>
 </tr>
 <tr>
 <td>[enable]</td>
 <td><code class="docutils literal notranslate">v6.0.0 -> latest</code></td> <tr>
 <td>[disable]</td>
 <td><code class="docutils literal notranslate">v6.0.0 -> latest</code></td> </table>
 </div>
 </li>
                <li> <span class="li-head">health_check</span> - Enable to check the responsiveness of the real server before forwarding traffic. <span class="li-normal">type: str</span> <span class="li-normal">choices: disable, enable</span>
 <a id='label186' href="javascript:ContentClick('label187', 'label186');" onmouseover="ContentPreview('label187');" onmouseout="ContentUnpreview('label187');" title="click to collapse or expand..."> more... </a>
 <div id="label187" style="display:none">
 <table border="1">
 <tr>
 <td></td>
 <td colspan="1">Supported Version Ranges</td>
 </tr>
 <tr>
 <td>health_check</td>
 <td><code class="docutils literal notranslate">v7.0.1 -> latest </code></td>
 </tr>
 <tr>
 <td>[disable]</td>
 <td><code class="docutils literal notranslate">v6.0.0 -> latest</code></td> <tr>
 <td>[enable]</td>
 <td><code class="docutils literal notranslate">v6.0.0 -> latest</code></td> </table>
 </div>
 </li>
                <li> <span class="li-head">health_check_proto</span> - Protocol of the health check monitor to use when polling to determine server"s connectivity status. <span class="li-normal">type: str</span> <span class="li-normal">choices: ping, http, tcp-connect</span>
 <a id='label188' href="javascript:ContentClick('label189', 'label188');" onmouseover="ContentPreview('label189');" onmouseout="ContentUnpreview('label189');" title="click to collapse or expand..."> more... </a>
 <div id="label189" style="display:none">
 <table border="1">
 <tr>
 <td></td>
 <td colspan="1">Supported Version Ranges</td>
 </tr>
 <tr>
 <td>health_check_proto</td>
 <td><code class="docutils literal notranslate">v7.0.1 -> latest </code></td>
 </tr>
 <tr>
 <td>[ping]</td>
 <td><code class="docutils literal notranslate">v6.0.0 -> latest</code></td> <tr>
 <td>[http]</td>
 <td><code class="docutils literal notranslate">v6.0.0 -> latest</code></td> <tr>
 <td>[tcp-connect]</td>
 <td><code class="docutils literal notranslate">v6.0.0 -> latest</code></td> </table>
 </div>
 </li>
                <li> <span class="li-head">holddown_interval</span> - Enable/disable holddown timer. Server will be considered active and reachable once the holddown period has expired (30 seconds). <span class="li-normal">type: str</span> <span class="li-normal">choices: enable, disable</span>
 <a id='label190' href="javascript:ContentClick('label191', 'label190');" onmouseover="ContentPreview('label191');" onmouseout="ContentUnpreview('label191');" title="click to collapse or expand..."> more... </a>
 <div id="label191" style="display:none">
 <table border="1">
 <tr>
 <td></td>
 <td colspan="1">Supported Version Ranges</td>
 </tr>
 <tr>
 <td>holddown_interval</td>
 <td><code class="docutils literal notranslate">v7.0.1 -> latest </code></td>
 </tr>
 <tr>
 <td>[enable]</td>
 <td><code class="docutils literal notranslate">v6.0.0 -> latest</code></td> <tr>
 <td>[disable]</td>
 <td><code class="docutils literal notranslate">v6.0.0 -> latest</code></td> </table>
 </div>
 </li>
                <li> <span class="li-head">http_host</span> - HTTP server domain name in HTTP header. <span class="li-normal">type: str</span>
 <a id='label192' href="javascript:ContentClick('label193', 'label192');" onmouseover="ContentPreview('label193');" onmouseout="ContentUnpreview('label193');" title="click to collapse or expand..."> more... </a>
 <div id="label193" style="display:none">
 <table border="1">
 <tr>
 <td></td>
 <td colspan="1">Supported Version Ranges</td>
 </tr>
 <tr>
 <td>http_host</td>
 <td><code class="docutils literal notranslate">v7.0.1 -> latest </code></td>
 </tr>
 </table>
 </div>
 </li>
                <li> <span class="li-head">id</span> - Real server ID. see <a href='#notes'>Notes</a>. <span class="li-normal">type: int</span> <span class="li-required">required: true</span>
 <a id='label194' href="javascript:ContentClick('label195', 'label194');" onmouseover="ContentPreview('label195');" onmouseout="ContentUnpreview('label195');" title="click to collapse or expand..."> more... </a>
 <div id="label195" style="display:none">
 <table border="1">
 <tr>
 <td></td>
 <td colspan="1">Supported Version Ranges</td>
 </tr>
 <tr>
 <td>id</td>
 <td><code class="docutils literal notranslate">v7.0.1 -> latest </code></td>
 </tr>
 </table>
 </div>
 </li>
                <li> <span class="li-head">ip</span> - IPv6 address of the real server. <span class="li-normal">type: str</span>
 <a id='label196' href="javascript:ContentClick('label197', 'label196');" onmouseover="ContentPreview('label197');" onmouseout="ContentUnpreview('label197');" title="click to collapse or expand..."> more... </a>
 <div id="label197" style="display:none">
 <table border="1">
 <tr>
 <td></td>
 <td colspan="1">Supported Version Ranges</td>
 </tr>
 <tr>
 <td>ip</td>
 <td><code class="docutils literal notranslate">v7.0.1 -> latest </code></td>
 </tr>
 </table>
 </div>
 </li>
                <li> <span class="li-head">mappedport</span> - Port for communicating with the real server. <span class="li-normal">type: str</span>
 <a id='label198' href="javascript:ContentClick('label199', 'label198');" onmouseover="ContentPreview('label199');" onmouseout="ContentUnpreview('label199');" title="click to collapse or expand..."> more... </a>
 <div id="label199" style="display:none">
 <table border="1">
 <tr>
 <td></td>
 <td colspan="1">Supported Version Ranges</td>
 </tr>
 <tr>
 <td>mappedport</td>
 <td><code class="docutils literal notranslate">v7.0.1 -> latest </code></td>
 </tr>
 </table>
 </div>
 </li>
                <li> <span class="li-head">port</span> - Port for communicating with the real server. <span class="li-normal">type: int</span>
 <a id='label200' href="javascript:ContentClick('label201', 'label200');" onmouseover="ContentPreview('label201');" onmouseout="ContentUnpreview('label201');" title="click to collapse or expand..."> more... </a>
 <div id="label201" style="display:none">
 <table border="1">
 <tr>
 <td></td>
 <td colspan="1">Supported Version Ranges</td>
 </tr>
 <tr>
 <td>port</td>
 <td><code class="docutils literal notranslate">v7.0.1 -> latest </code></td>
 </tr>
 </table>
 </div>
 </li>
                <li> <span class="li-head">ssh_client_cert</span> - Set access-proxy SSH client certificate profile. Source firewall.access-proxy-ssh-client-cert.name. <span class="li-normal">type: str</span>
 <a id='label202' href="javascript:ContentClick('label203', 'label202');" onmouseover="ContentPreview('label203');" onmouseout="ContentUnpreview('label203');" title="click to collapse or expand..."> more... </a>
 <div id="label203" style="display:none">
 <table border="1">
 <tr>
 <td></td>
 <td colspan="1">Supported Version Ranges</td>
 </tr>
 <tr>
 <td>ssh_client_cert</td>
 <td><code class="docutils literal notranslate">v7.0.1 -> latest </code></td>
 </tr>
 </table>
 </div>
 </li>
                <li> <span class="li-head">ssh_host_key</span> - One or more server host key. <span class="li-normal">type: list</span> <span style="font-family:'Courier New'" class="li-required">member_path: api_gateway6:id/realservers:id/ssh_host_key:name</span>
 <a id='label204' href="javascript:ContentClick('label205', 'label204');" onmouseover="ContentPreview('label205');" onmouseout="ContentUnpreview('label205');" title="click to collapse or expand..."> more... </a>
 <div id="label205" style="display:none">
 <table border="1">
 <tr>
 <td></td><td colspan="1">Supported Version Ranges</td>
 </tr>
 <tr>
 <td>ssh_host_key</td>
 <td><code class="docutils literal notranslate">v7.0.1 -> latest </code></td>
 </tr>
 </table>
 </div>
 </li>
                    <ul class="ul-self">
                    <li> <span class="li-head">name</span> - Server host key name. Source firewall.ssh.host-key.name. <span class="li-normal">type: str</span> <span class="li-required">required: true</span>
 <a id='label206' href="javascript:ContentClick('label207', 'label206');" onmouseover="ContentPreview('label207');" onmouseout="ContentUnpreview('label207');" title="click to collapse or expand..."> more... </a>
 <div id="label207" style="display:none">
 <table border="1">
 <tr>
 <td></td>
 <td colspan="1">Supported Version Ranges</td>
 </tr>
 <tr>
 <td>name</td>
 <td><code class="docutils literal notranslate">v7.0.1 -> latest </code></td>
 </tr>
 </table>
 </div>
 </li>
                    </ul>
                <li> <span class="li-head">ssh_host_key_validation</span> - Enable/disable SSH real server host key validation. <span class="li-normal">type: str</span> <span class="li-normal">choices: disable, enable</span>
 <a id='label208' href="javascript:ContentClick('label209', 'label208');" onmouseover="ContentPreview('label209');" onmouseout="ContentUnpreview('label209');" title="click to collapse or expand..."> more... </a>
 <div id="label209" style="display:none">
 <table border="1">
 <tr>
 <td></td>
 <td colspan="1">Supported Version Ranges</td>
 </tr>
 <tr>
 <td>ssh_host_key_validation</td>
 <td><code class="docutils literal notranslate">v7.0.1 -> latest </code></td>
 </tr>
 <tr>
 <td>[disable]</td>
 <td><code class="docutils literal notranslate">v6.0.0 -> latest</code></td> <tr>
 <td>[enable]</td>
 <td><code class="docutils literal notranslate">v6.0.0 -> latest</code></td> </table>
 </div>
 </li>
                <li> <span class="li-head">status</span> - Set the status of the real server to active so that it can accept traffic, or on standby or disabled so no traffic is sent. <span class="li-normal">type: str</span> <span class="li-normal">choices: active, standby, disable</span>
 <a id='label210' href="javascript:ContentClick('label211', 'label210');" onmouseover="ContentPreview('label211');" onmouseout="ContentUnpreview('label211');" title="click to collapse or expand..."> more... </a>
 <div id="label211" style="display:none">
 <table border="1">
 <tr>
 <td></td>
 <td colspan="1">Supported Version Ranges</td>
 </tr>
 <tr>
 <td>status</td>
 <td><code class="docutils literal notranslate">v7.0.1 -> latest </code></td>
 </tr>
 <tr>
 <td>[active]</td>
 <td><code class="docutils literal notranslate">v6.0.0 -> latest</code></td> <tr>
 <td>[standby]</td>
 <td><code class="docutils literal notranslate">v6.0.0 -> latest</code></td> <tr>
 <td>[disable]</td>
 <td><code class="docutils literal notranslate">v6.0.0 -> latest</code></td> </table>
 </div>
 </li>
                <li> <span class="li-head">translate_host</span> - Enable/disable translation of hostname/IP from virtual server to real server. <span class="li-normal">type: str</span> <span class="li-normal">choices: enable, disable</span>
 <a id='label212' href="javascript:ContentClick('label213', 'label212');" onmouseover="ContentPreview('label213');" onmouseout="ContentUnpreview('label213');" title="click to collapse or expand..."> more... </a>
 <div id="label213" style="display:none">
 <table border="1">
 <tr>
 <td></td>
 <td colspan="1">Supported Version Ranges</td>
 </tr>
 <tr>
 <td>translate_host</td>
 <td><code class="docutils literal notranslate">v7.2.4 -> latest </code></td>
 </tr>
 <tr>
 <td>[enable]</td>
 <td><code class="docutils literal notranslate">v6.0.0 -> latest</code></td> <tr>
 <td>[disable]</td>
 <td><code class="docutils literal notranslate">v6.0.0 -> latest</code></td> </table>
 </div>
 </li>
                <li> <span class="li-head">tunnel_encryption</span> - Tunnel encryption. <span class="li-normal">type: str</span> <span class="li-normal">choices: enable, disable</span>
 <a id='label214' href="javascript:ContentClick('label215', 'label214');" onmouseover="ContentPreview('label215');" onmouseout="ContentUnpreview('label215');" title="click to collapse or expand..."> more... </a>
 <div id="label215" style="display:none">
 <table border="1">
 <tr>
 <td></td>
 <td colspan="1">Supported Version Ranges</td>
 </tr>
 <tr>
 <td>tunnel_encryption</td>
 <td><code class="docutils literal notranslate">v7.4.0 -> latest </code></td>
 </tr>
 <tr>
 <td>[enable]</td>
 <td><code class="docutils literal notranslate">v6.0.0 -> latest</code></td> <tr>
 <td>[disable]</td>
 <td><code class="docutils literal notranslate">v6.0.0 -> latest</code></td> </table>
 </div>
 </li>
                <li> <span class="li-head">type</span> - TCP forwarding server type. <span class="li-normal">type: str</span> <span class="li-normal">choices: tcp-forwarding, ssh</span>
 <a id='label216' href="javascript:ContentClick('label217', 'label216');" onmouseover="ContentPreview('label217');" onmouseout="ContentUnpreview('label217');" title="click to collapse or expand..."> more... </a>
 <div id="label217" style="display:none">
 <table border="1">
 <tr>
 <td></td>
 <td colspan="1">Supported Version Ranges</td>
 </tr>
 <tr>
 <td>type</td>
 <td><code class="docutils literal notranslate">v7.0.1 -> latest </code></td>
 </tr>
 <tr>
 <td>[tcp-forwarding]</td>
 <td><code class="docutils literal notranslate">v6.0.0 -> latest</code></td> <tr>
 <td>[ssh]</td>
 <td><code class="docutils literal notranslate">v6.0.0 -> latest</code></td> </table>
 </div>
 </li>
                <li> <span class="li-head">weight</span> - Weight of the real server. If weighted load balancing is enabled, the server with the highest weight gets more connections. <span class="li-normal">type: int</span>
 <a id='label218' href="javascript:ContentClick('label219', 'label218');" onmouseover="ContentPreview('label219');" onmouseout="ContentUnpreview('label219');" title="click to collapse or expand..."> more... </a>
 <div id="label219" style="display:none">
 <table border="1">
 <tr>
 <td></td>
 <td colspan="1">Supported Version Ranges</td>
 </tr>
 <tr>
 <td>weight</td>
 <td><code class="docutils literal notranslate">v7.0.1 -> latest </code></td>
 </tr>
 </table>
 </div>
 </li>
                </ul>
            <li> <span class="li-head">saml_redirect</span> - Enable/disable SAML redirection after successful authentication. <span class="li-normal">type: str</span> <span class="li-normal">choices: disable, enable</span>
 <a id='label220' href="javascript:ContentClick('label221', 'label220');" onmouseover="ContentPreview('label221');" onmouseout="ContentUnpreview('label221');" title="click to collapse or expand..."> more... </a>
 <div id="label221" style="display:none">
 <table border="1">
 <tr>
 <td></td>
 <td colspan="1">Supported Version Ranges</td>
 </tr>
 <tr>
 <td>saml_redirect</td>
 <td><code class="docutils literal notranslate">v7.0.2 -> latest </code></td>
 </tr>
 <tr>
 <td>[disable]</td>
 <td><code class="docutils literal notranslate">v6.0.0 -> latest</code></td> <tr>
 <td>[enable]</td>
 <td><code class="docutils literal notranslate">v6.0.0 -> latest</code></td> </table>
 </div>
 </li>
            <li> <span class="li-head">saml_server</span> - SAML service provider configuration for VIP authentication. Source user.saml.name. <span class="li-normal">type: str</span>
 <a id='label222' href="javascript:ContentClick('label223', 'label222');" onmouseover="ContentPreview('label223');" onmouseout="ContentUnpreview('label223');" title="click to collapse or expand..."> more... </a>
 <div id="label223" style="display:none">
 <table border="1">
 <tr>
 <td></td>
 <td colspan="1">Supported Version Ranges</td>
 </tr>
 <tr>
 <td>saml_server</td>
 <td><code class="docutils literal notranslate">v7.0.1 -> latest </code></td>
 </tr>
 </table>
 </div>
 </li>
            <li> <span class="li-head">service</span> - Service. <span class="li-normal">type: str</span> <span class="li-normal">choices: http, https, tcp-forwarding, samlsp, web-portal, saas</span>
 <a id='label224' href="javascript:ContentClick('label225', 'label224');" onmouseover="ContentPreview('label225');" onmouseout="ContentUnpreview('label225');" title="click to collapse or expand..."> more... </a>
 <div id="label225" style="display:none">
 <table border="1">
 <tr>
 <td></td>
 <td colspan="1">Supported Version Ranges</td>
 </tr>
 <tr>
 <td>service</td>
 <td><code class="docutils literal notranslate">v7.0.1 -> latest </code></td>
 </tr>
 <tr>
 <td>[http]</td>
 <td><code class="docutils literal notranslate">v6.0.0 -> latest</code></td> <tr>
 <td>[https]</td>
 <td><code class="docutils literal notranslate">v6.0.0 -> latest</code></td> <tr>
 <td>[tcp-forwarding]</td>
 <td><code class="docutils literal notranslate">v6.0.0 -> latest</code></td> <tr>
 <td>[samlsp]</td>
 <td><code class="docutils literal notranslate">v6.0.0 -> latest</code></td> <tr>
 <td>[web-portal]</td>
 <td><code class="docutils literal notranslate">v7.0.4 -> latest</code></td>
 </tr>
 <tr>
 <td>[saas]</td>
 <td><code class="docutils literal notranslate">v7.2.1 -> latest</code></td>
 </tr>
 </table>
 </div>
 </li>
            <li> <span class="li-head">ssl_algorithm</span> - Permitted encryption algorithms for the server side of SSL full mode sessions according to encryption strength. <span class="li-normal">type: str</span> <span class="li-normal">choices: high, medium, low</span>
 <a id='label226' href="javascript:ContentClick('label227', 'label226');" onmouseover="ContentPreview('label227');" onmouseout="ContentUnpreview('label227');" title="click to collapse or expand..."> more... </a>
 <div id="label227" style="display:none">
 <table border="1">
 <tr>
 <td></td>
 <td colspan="1">Supported Version Ranges</td>
 </tr>
 <tr>
 <td>ssl_algorithm</td>
 <td><code class="docutils literal notranslate">v7.0.1 -> latest </code></td>
 </tr>
 <tr>
 <td>[high]</td>
 <td><code class="docutils literal notranslate">v6.0.0 -> latest</code></td> <tr>
 <td>[medium]</td>
 <td><code class="docutils literal notranslate">v6.0.0 -> latest</code></td> <tr>
 <td>[low]</td>
 <td><code class="docutils literal notranslate">v6.0.0 -> latest</code></td> </table>
 </div>
 </li>
            <li> <span class="li-head">ssl_cipher_suites</span> - SSL/TLS cipher suites to offer to a server, ordered by priority. <span class="li-normal">type: list</span> <span style="font-family:'Courier New'" class="li-required">member_path: api_gateway6:id/ssl_cipher_suites:priority</span>
 <a id='label228' href="javascript:ContentClick('label229', 'label228');" onmouseover="ContentPreview('label229');" onmouseout="ContentUnpreview('label229');" title="click to collapse or expand..."> more... </a>
 <div id="label229" style="display:none">
 <table border="1">
 <tr>
 <td></td><td colspan="1">Supported Version Ranges</td>
 </tr>
 <tr>
 <td>ssl_cipher_suites</td>
 <td><code class="docutils literal notranslate">v7.0.1 -> latest </code></td>
 </tr>
 </table>
 </div>
 </li>
                <ul class="ul-self">
                <li> <span class="li-head">cipher</span> - Cipher suite name. <span class="li-normal">type: str</span> <span class="li-normal">choices: TLS-AES-128-GCM-SHA256, TLS-AES-256-GCM-SHA384, TLS-CHACHA20-POLY1305-SHA256, TLS-ECDHE-RSA-WITH-CHACHA20-POLY1305-SHA256, TLS-ECDHE-ECDSA-WITH-CHACHA20-POLY1305-SHA256, TLS-DHE-RSA-WITH-CHACHA20-POLY1305-SHA256, TLS-DHE-RSA-WITH-AES-128-CBC-SHA, TLS-DHE-RSA-WITH-AES-256-CBC-SHA, TLS-DHE-RSA-WITH-AES-128-CBC-SHA256, TLS-DHE-RSA-WITH-AES-128-GCM-SHA256, TLS-DHE-RSA-WITH-AES-256-CBC-SHA256, TLS-DHE-RSA-WITH-AES-256-GCM-SHA384, TLS-DHE-DSS-WITH-AES-128-CBC-SHA, TLS-DHE-DSS-WITH-AES-256-CBC-SHA, TLS-DHE-DSS-WITH-AES-128-CBC-SHA256, TLS-DHE-DSS-WITH-AES-128-GCM-SHA256, TLS-DHE-DSS-WITH-AES-256-CBC-SHA256, TLS-DHE-DSS-WITH-AES-256-GCM-SHA384, TLS-ECDHE-RSA-WITH-AES-128-CBC-SHA, TLS-ECDHE-RSA-WITH-AES-128-CBC-SHA256, TLS-ECDHE-RSA-WITH-AES-128-GCM-SHA256, TLS-ECDHE-RSA-WITH-AES-256-CBC-SHA, TLS-ECDHE-RSA-WITH-AES-256-CBC-SHA384, TLS-ECDHE-RSA-WITH-AES-256-GCM-SHA384, TLS-ECDHE-ECDSA-WITH-AES-128-CBC-SHA, TLS-ECDHE-ECDSA-WITH-AES-128-CBC-SHA256, TLS-ECDHE-ECDSA-WITH-AES-128-GCM-SHA256, TLS-ECDHE-ECDSA-WITH-AES-256-CBC-SHA, TLS-ECDHE-ECDSA-WITH-AES-256-CBC-SHA384, TLS-ECDHE-ECDSA-WITH-AES-256-GCM-SHA384, TLS-RSA-WITH-AES-128-CBC-SHA, TLS-RSA-WITH-AES-256-CBC-SHA, TLS-RSA-WITH-AES-128-CBC-SHA256, TLS-RSA-WITH-AES-128-GCM-SHA256, TLS-RSA-WITH-AES-256-CBC-SHA256, TLS-RSA-WITH-AES-256-GCM-SHA384, TLS-RSA-WITH-CAMELLIA-128-CBC-SHA, TLS-RSA-WITH-CAMELLIA-256-CBC-SHA, TLS-RSA-WITH-CAMELLIA-128-CBC-SHA256, TLS-RSA-WITH-CAMELLIA-256-CBC-SHA256, TLS-DHE-RSA-WITH-3DES-EDE-CBC-SHA, TLS-DHE-RSA-WITH-CAMELLIA-128-CBC-SHA, TLS-DHE-DSS-WITH-CAMELLIA-128-CBC-SHA, TLS-DHE-RSA-WITH-CAMELLIA-256-CBC-SHA, TLS-DHE-DSS-WITH-CAMELLIA-256-CBC-SHA, TLS-DHE-RSA-WITH-CAMELLIA-128-CBC-SHA256, TLS-DHE-DSS-WITH-CAMELLIA-128-CBC-SHA256, TLS-DHE-RSA-WITH-CAMELLIA-256-CBC-SHA256, TLS-DHE-DSS-WITH-CAMELLIA-256-CBC-SHA256, TLS-DHE-RSA-WITH-SEED-CBC-SHA, TLS-DHE-DSS-WITH-SEED-CBC-SHA, TLS-DHE-RSA-WITH-ARIA-128-CBC-SHA256, TLS-DHE-RSA-WITH-ARIA-256-CBC-SHA384, TLS-DHE-DSS-WITH-ARIA-128-CBC-SHA256, TLS-DHE-DSS-WITH-ARIA-256-CBC-SHA384, TLS-RSA-WITH-SEED-CBC-SHA, TLS-RSA-WITH-ARIA-128-CBC-SHA256, TLS-RSA-WITH-ARIA-256-CBC-SHA384, TLS-ECDHE-RSA-WITH-ARIA-128-CBC-SHA256, TLS-ECDHE-RSA-WITH-ARIA-256-CBC-SHA384, TLS-ECDHE-ECDSA-WITH-ARIA-128-CBC-SHA256, TLS-ECDHE-ECDSA-WITH-ARIA-256-CBC-SHA384, TLS-ECDHE-RSA-WITH-RC4-128-SHA, TLS-ECDHE-RSA-WITH-3DES-EDE-CBC-SHA, TLS-DHE-DSS-WITH-3DES-EDE-CBC-SHA, TLS-RSA-WITH-3DES-EDE-CBC-SHA, TLS-RSA-WITH-RC4-128-MD5, TLS-RSA-WITH-RC4-128-SHA, TLS-DHE-RSA-WITH-DES-CBC-SHA, TLS-DHE-DSS-WITH-DES-CBC-SHA, TLS-RSA-WITH-DES-CBC-SHA</span>
 <a id='label230' href="javascript:ContentClick('label231', 'label230');" onmouseover="ContentPreview('label231');" onmouseout="ContentUnpreview('label231');" title="click to collapse or expand..."> more... </a>
 <div id="label231" style="display:none">
 <table border="1">
 <tr>
 <td></td>
 <td colspan="1">Supported Version Ranges</td>
 </tr>
 <tr>
 <td>cipher</td>
 <td><code class="docutils literal notranslate">v7.0.1 -> latest </code></td>
 </tr>
 <tr>
 <td>[TLS-AES-128-GCM-SHA256]</td>
 <td><code class="docutils literal notranslate">v6.0.0 -> latest</code></td> <tr>
 <td>[TLS-AES-256-GCM-SHA384]</td>
 <td><code class="docutils literal notranslate">v6.0.0 -> latest</code></td> <tr>
 <td>[TLS-CHACHA20-POLY1305-SHA256]</td>
 <td><code class="docutils literal notranslate">v6.0.0 -> latest</code></td> <tr>
 <td>[TLS-ECDHE-RSA-WITH-CHACHA20-POLY1305-SHA256]</td>
 <td><code class="docutils literal notranslate">v6.0.0 -> latest</code></td> <tr>
 <td>[TLS-ECDHE-ECDSA-WITH-CHACHA20-POLY1305-SHA256]</td>
 <td><code class="docutils literal notranslate">v6.0.0 -> latest</code></td> <tr>
 <td>[TLS-DHE-RSA-WITH-CHACHA20-POLY1305-SHA256]</td>
 <td><code class="docutils literal notranslate">v6.0.0 -> latest</code></td> <tr>
 <td>[TLS-DHE-RSA-WITH-AES-128-CBC-SHA]</td>
 <td><code class="docutils literal notranslate">v6.0.0 -> latest</code></td> <tr>
 <td>[TLS-DHE-RSA-WITH-AES-256-CBC-SHA]</td>
 <td><code class="docutils literal notranslate">v6.0.0 -> latest</code></td> <tr>
 <td>[TLS-DHE-RSA-WITH-AES-128-CBC-SHA256]</td>
 <td><code class="docutils literal notranslate">v6.0.0 -> latest</code></td> <tr>
 <td>[TLS-DHE-RSA-WITH-AES-128-GCM-SHA256]</td>
 <td><code class="docutils literal notranslate">v6.0.0 -> latest</code></td> <tr>
 <td>[TLS-DHE-RSA-WITH-AES-256-CBC-SHA256]</td>
 <td><code class="docutils literal notranslate">v6.0.0 -> latest</code></td> <tr>
 <td>[TLS-DHE-RSA-WITH-AES-256-GCM-SHA384]</td>
 <td><code class="docutils literal notranslate">v6.0.0 -> latest</code></td> <tr>
 <td>[TLS-DHE-DSS-WITH-AES-128-CBC-SHA]</td>
 <td><code class="docutils literal notranslate">v6.0.0 -> latest</code></td> <tr>
 <td>[TLS-DHE-DSS-WITH-AES-256-CBC-SHA]</td>
 <td><code class="docutils literal notranslate">v6.0.0 -> latest</code></td> <tr>
 <td>[TLS-DHE-DSS-WITH-AES-128-CBC-SHA256]</td>
 <td><code class="docutils literal notranslate">v6.0.0 -> latest</code></td> <tr>
 <td>[TLS-DHE-DSS-WITH-AES-128-GCM-SHA256]</td>
 <td><code class="docutils literal notranslate">v6.0.0 -> latest</code></td> <tr>
 <td>[TLS-DHE-DSS-WITH-AES-256-CBC-SHA256]</td>
 <td><code class="docutils literal notranslate">v6.0.0 -> latest</code></td> <tr>
 <td>[TLS-DHE-DSS-WITH-AES-256-GCM-SHA384]</td>
 <td><code class="docutils literal notranslate">v6.0.0 -> latest</code></td> <tr>
 <td>[TLS-ECDHE-RSA-WITH-AES-128-CBC-SHA]</td>
 <td><code class="docutils literal notranslate">v6.0.0 -> latest</code></td> <tr>
 <td>[TLS-ECDHE-RSA-WITH-AES-128-CBC-SHA256]</td>
 <td><code class="docutils literal notranslate">v6.0.0 -> latest</code></td> <tr>
 <td>[TLS-ECDHE-RSA-WITH-AES-128-GCM-SHA256]</td>
 <td><code class="docutils literal notranslate">v6.0.0 -> latest</code></td> <tr>
 <td>[TLS-ECDHE-RSA-WITH-AES-256-CBC-SHA]</td>
 <td><code class="docutils literal notranslate">v6.0.0 -> latest</code></td> <tr>
 <td>[TLS-ECDHE-RSA-WITH-AES-256-CBC-SHA384]</td>
 <td><code class="docutils literal notranslate">v6.0.0 -> latest</code></td> <tr>
 <td>[TLS-ECDHE-RSA-WITH-AES-256-GCM-SHA384]</td>
 <td><code class="docutils literal notranslate">v6.0.0 -> latest</code></td> <tr>
 <td>[TLS-ECDHE-ECDSA-WITH-AES-128-CBC-SHA]</td>
 <td><code class="docutils literal notranslate">v6.0.0 -> latest</code></td> <tr>
 <td>[TLS-ECDHE-ECDSA-WITH-AES-128-CBC-SHA256]</td>
 <td><code class="docutils literal notranslate">v6.0.0 -> latest</code></td> <tr>
 <td>[TLS-ECDHE-ECDSA-WITH-AES-128-GCM-SHA256]</td>
 <td><code class="docutils literal notranslate">v6.0.0 -> latest</code></td> <tr>
 <td>[TLS-ECDHE-ECDSA-WITH-AES-256-CBC-SHA]</td>
 <td><code class="docutils literal notranslate">v6.0.0 -> latest</code></td> <tr>
 <td>[TLS-ECDHE-ECDSA-WITH-AES-256-CBC-SHA384]</td>
 <td><code class="docutils literal notranslate">v6.0.0 -> latest</code></td> <tr>
 <td>[TLS-ECDHE-ECDSA-WITH-AES-256-GCM-SHA384]</td>
 <td><code class="docutils literal notranslate">v6.0.0 -> latest</code></td> <tr>
 <td>[TLS-RSA-WITH-AES-128-CBC-SHA]</td>
 <td><code class="docutils literal notranslate">v6.0.0 -> latest</code></td> <tr>
 <td>[TLS-RSA-WITH-AES-256-CBC-SHA]</td>
 <td><code class="docutils literal notranslate">v6.0.0 -> latest</code></td> <tr>
 <td>[TLS-RSA-WITH-AES-128-CBC-SHA256]</td>
 <td><code class="docutils literal notranslate">v6.0.0 -> latest</code></td> <tr>
 <td>[TLS-RSA-WITH-AES-128-GCM-SHA256]</td>
 <td><code class="docutils literal notranslate">v6.0.0 -> latest</code></td> <tr>
 <td>[TLS-RSA-WITH-AES-256-CBC-SHA256]</td>
 <td><code class="docutils literal notranslate">v6.0.0 -> latest</code></td> <tr>
 <td>[TLS-RSA-WITH-AES-256-GCM-SHA384]</td>
 <td><code class="docutils literal notranslate">v6.0.0 -> latest</code></td> <tr>
 <td>[TLS-RSA-WITH-CAMELLIA-128-CBC-SHA]</td>
 <td><code class="docutils literal notranslate">v6.0.0 -> latest</code></td> <tr>
 <td>[TLS-RSA-WITH-CAMELLIA-256-CBC-SHA]</td>
 <td><code class="docutils literal notranslate">v6.0.0 -> latest</code></td> <tr>
 <td>[TLS-RSA-WITH-CAMELLIA-128-CBC-SHA256]</td>
 <td><code class="docutils literal notranslate">v6.0.0 -> latest</code></td> <tr>
 <td>[TLS-RSA-WITH-CAMELLIA-256-CBC-SHA256]</td>
 <td><code class="docutils literal notranslate">v6.0.0 -> latest</code></td> <tr>
 <td>[TLS-DHE-RSA-WITH-3DES-EDE-CBC-SHA]</td>
 <td><code class="docutils literal notranslate">v6.0.0 -> latest</code></td> <tr>
 <td>[TLS-DHE-RSA-WITH-CAMELLIA-128-CBC-SHA]</td>
 <td><code class="docutils literal notranslate">v6.0.0 -> latest</code></td> <tr>
 <td>[TLS-DHE-DSS-WITH-CAMELLIA-128-CBC-SHA]</td>
 <td><code class="docutils literal notranslate">v6.0.0 -> latest</code></td> <tr>
 <td>[TLS-DHE-RSA-WITH-CAMELLIA-256-CBC-SHA]</td>
 <td><code class="docutils literal notranslate">v6.0.0 -> latest</code></td> <tr>
 <td>[TLS-DHE-DSS-WITH-CAMELLIA-256-CBC-SHA]</td>
 <td><code class="docutils literal notranslate">v6.0.0 -> latest</code></td> <tr>
 <td>[TLS-DHE-RSA-WITH-CAMELLIA-128-CBC-SHA256]</td>
 <td><code class="docutils literal notranslate">v6.0.0 -> latest</code></td> <tr>
 <td>[TLS-DHE-DSS-WITH-CAMELLIA-128-CBC-SHA256]</td>
 <td><code class="docutils literal notranslate">v6.0.0 -> latest</code></td> <tr>
 <td>[TLS-DHE-RSA-WITH-CAMELLIA-256-CBC-SHA256]</td>
 <td><code class="docutils literal notranslate">v6.0.0 -> latest</code></td> <tr>
 <td>[TLS-DHE-DSS-WITH-CAMELLIA-256-CBC-SHA256]</td>
 <td><code class="docutils literal notranslate">v6.0.0 -> latest</code></td> <tr>
 <td>[TLS-DHE-RSA-WITH-SEED-CBC-SHA]</td>
 <td><code class="docutils literal notranslate">v6.0.0 -> latest</code></td> <tr>
 <td>[TLS-DHE-DSS-WITH-SEED-CBC-SHA]</td>
 <td><code class="docutils literal notranslate">v6.0.0 -> latest</code></td> <tr>
 <td>[TLS-DHE-RSA-WITH-ARIA-128-CBC-SHA256]</td>
 <td><code class="docutils literal notranslate">v6.0.0 -> latest</code></td> <tr>
 <td>[TLS-DHE-RSA-WITH-ARIA-256-CBC-SHA384]</td>
 <td><code class="docutils literal notranslate">v6.0.0 -> latest</code></td> <tr>
 <td>[TLS-DHE-DSS-WITH-ARIA-128-CBC-SHA256]</td>
 <td><code class="docutils literal notranslate">v6.0.0 -> latest</code></td> <tr>
 <td>[TLS-DHE-DSS-WITH-ARIA-256-CBC-SHA384]</td>
 <td><code class="docutils literal notranslate">v6.0.0 -> latest</code></td> <tr>
 <td>[TLS-RSA-WITH-SEED-CBC-SHA]</td>
 <td><code class="docutils literal notranslate">v6.0.0 -> latest</code></td> <tr>
 <td>[TLS-RSA-WITH-ARIA-128-CBC-SHA256]</td>
 <td><code class="docutils literal notranslate">v6.0.0 -> latest</code></td> <tr>
 <td>[TLS-RSA-WITH-ARIA-256-CBC-SHA384]</td>
 <td><code class="docutils literal notranslate">v6.0.0 -> latest</code></td> <tr>
 <td>[TLS-ECDHE-RSA-WITH-ARIA-128-CBC-SHA256]</td>
 <td><code class="docutils literal notranslate">v6.0.0 -> latest</code></td> <tr>
 <td>[TLS-ECDHE-RSA-WITH-ARIA-256-CBC-SHA384]</td>
 <td><code class="docutils literal notranslate">v6.0.0 -> latest</code></td> <tr>
 <td>[TLS-ECDHE-ECDSA-WITH-ARIA-128-CBC-SHA256]</td>
 <td><code class="docutils literal notranslate">v6.0.0 -> latest</code></td> <tr>
 <td>[TLS-ECDHE-ECDSA-WITH-ARIA-256-CBC-SHA384]</td>
 <td><code class="docutils literal notranslate">v6.0.0 -> latest</code></td> <tr>
 <td>[TLS-ECDHE-RSA-WITH-RC4-128-SHA]</td>
 <td><code class="docutils literal notranslate">v6.0.0 -> latest</code></td> <tr>
 <td>[TLS-ECDHE-RSA-WITH-3DES-EDE-CBC-SHA]</td>
 <td><code class="docutils literal notranslate">v6.0.0 -> latest</code></td> <tr>
 <td>[TLS-DHE-DSS-WITH-3DES-EDE-CBC-SHA]</td>
 <td><code class="docutils literal notranslate">v6.0.0 -> latest</code></td> <tr>
 <td>[TLS-RSA-WITH-3DES-EDE-CBC-SHA]</td>
 <td><code class="docutils literal notranslate">v6.0.0 -> latest</code></td> <tr>
 <td>[TLS-RSA-WITH-RC4-128-MD5]</td>
 <td><code class="docutils literal notranslate">v6.0.0 -> latest</code></td> <tr>
 <td>[TLS-RSA-WITH-RC4-128-SHA]</td>
 <td><code class="docutils literal notranslate">v6.0.0 -> latest</code></td> <tr>
 <td>[TLS-DHE-RSA-WITH-DES-CBC-SHA]</td>
 <td><code class="docutils literal notranslate">v6.0.0 -> latest</code></td> <tr>
 <td>[TLS-DHE-DSS-WITH-DES-CBC-SHA]</td>
 <td><code class="docutils literal notranslate">v6.0.0 -> latest</code></td> <tr>
 <td>[TLS-RSA-WITH-DES-CBC-SHA]</td>
 <td><code class="docutils literal notranslate">v6.0.0 -> latest</code></td> </table>
 </div>
 </li>
                <li> <span class="li-head">priority</span> - SSL/TLS cipher suites priority. see <a href='#notes'>Notes</a>. <span class="li-normal">type: int</span> <span class="li-required">required: true</span>
 <a id='label232' href="javascript:ContentClick('label233', 'label232');" onmouseover="ContentPreview('label233');" onmouseout="ContentUnpreview('label233');" title="click to collapse or expand..."> more... </a>
 <div id="label233" style="display:none">
 <table border="1">
 <tr>
 <td></td>
 <td colspan="1">Supported Version Ranges</td>
 </tr>
 <tr>
 <td>priority</td>
 <td><code class="docutils literal notranslate">v7.0.1 -> latest </code></td>
 </tr>
 </table>
 </div>
 </li>
                <li> <span class="li-head">versions</span> - SSL/TLS versions that the cipher suite can be used with. <span class="li-normal">type: list</span> <span class="li-normal">choices: tls-1.0, tls-1.1, tls-1.2, tls-1.3</span>
 <a id='label234' href="javascript:ContentClick('label235', 'label234');" onmouseover="ContentPreview('label235');" onmouseout="ContentUnpreview('label235');" title="click to collapse or expand..."> more... </a>
 <div id="label235" style="display:none">
 <table border="1">
 <tr>
 <td></td>
 <td colspan="1">Supported Version Ranges</td>
 </tr>
 <tr>
 <td>versions</td>
 <td><code class="docutils literal notranslate">v7.0.1 -> latest </code></td>
 </tr>
 <tr>
 <td>[tls-1.0]</td>
 <td><code class="docutils literal notranslate">v6.0.0 -> latest</code></td> <tr>
 <td>[tls-1.1]</td>
 <td><code class="docutils literal notranslate">v6.0.0 -> latest</code></td> <tr>
 <td>[tls-1.2]</td>
 <td><code class="docutils literal notranslate">v6.0.0 -> latest</code></td> <tr>
 <td>[tls-1.3]</td>
 <td><code class="docutils literal notranslate">v6.0.0 -> latest</code></td> </table>
 </div>
 </li>
                </ul>
            <li> <span class="li-head">ssl_dh_bits</span> - Number of bits to use in the Diffie-Hellman exchange for RSA encryption of SSL sessions. <span class="li-normal">type: str</span> <span class="li-normal">choices: 768, 1024, 1536, 2048, 3072, 4096</span>
 <a id='label236' href="javascript:ContentClick('label237', 'label236');" onmouseover="ContentPreview('label237');" onmouseout="ContentUnpreview('label237');" title="click to collapse or expand..."> more... </a>
 <div id="label237" style="display:none">
 <table border="1">
 <tr>
 <td></td>
 <td colspan="1">Supported Version Ranges</td>
 </tr>
 <tr>
 <td>ssl_dh_bits</td>
 <td><code class="docutils literal notranslate">v7.0.1 -> latest </code></td>
 </tr>
 <tr>
 <td>[768]</td>
 <td><code class="docutils literal notranslate">v6.0.0 -> latest</code></td> <tr>
 <td>[1024]</td>
 <td><code class="docutils literal notranslate">v6.0.0 -> latest</code></td> <tr>
 <td>[1536]</td>
 <td><code class="docutils literal notranslate">v6.0.0 -> latest</code></td> <tr>
 <td>[2048]</td>
 <td><code class="docutils literal notranslate">v6.0.0 -> latest</code></td> <tr>
 <td>[3072]</td>
 <td><code class="docutils literal notranslate">v6.0.0 -> latest</code></td> <tr>
 <td>[4096]</td>
 <td><code class="docutils literal notranslate">v6.0.0 -> latest</code></td> </table>
 </div>
 </li>
            <li> <span class="li-head">ssl_max_version</span> - Highest SSL/TLS version acceptable from a server. <span class="li-normal">type: str</span> <span class="li-normal">choices: tls-1.0, tls-1.1, tls-1.2, tls-1.3</span>
 <a id='label238' href="javascript:ContentClick('label239', 'label238');" onmouseover="ContentPreview('label239');" onmouseout="ContentUnpreview('label239');" title="click to collapse or expand..."> more... </a>
 <div id="label239" style="display:none">
 <table border="1">
 <tr>
 <td></td>
 <td colspan="1">Supported Version Ranges</td>
 </tr>
 <tr>
 <td>ssl_max_version</td>
 <td><code class="docutils literal notranslate">v7.0.1 -> latest </code></td>
 </tr>
 <tr>
 <td>[tls-1.0]</td>
 <td><code class="docutils literal notranslate">v6.0.0 -> latest</code></td> <tr>
 <td>[tls-1.1]</td>
 <td><code class="docutils literal notranslate">v6.0.0 -> latest</code></td> <tr>
 <td>[tls-1.2]</td>
 <td><code class="docutils literal notranslate">v6.0.0 -> latest</code></td> <tr>
 <td>[tls-1.3]</td>
 <td><code class="docutils literal notranslate">v6.0.0 -> latest</code></td> </table>
 </div>
 </li>
            <li> <span class="li-head">ssl_min_version</span> - Lowest SSL/TLS version acceptable from a server. <span class="li-normal">type: str</span> <span class="li-normal">choices: tls-1.0, tls-1.1, tls-1.2, tls-1.3</span>
 <a id='label240' href="javascript:ContentClick('label241', 'label240');" onmouseover="ContentPreview('label241');" onmouseout="ContentUnpreview('label241');" title="click to collapse or expand..."> more... </a>
 <div id="label241" style="display:none">
 <table border="1">
 <tr>
 <td></td>
 <td colspan="1">Supported Version Ranges</td>
 </tr>
 <tr>
 <td>ssl_min_version</td>
 <td><code class="docutils literal notranslate">v7.0.1 -> latest </code></td>
 </tr>
 <tr>
 <td>[tls-1.0]</td>
 <td><code class="docutils literal notranslate">v6.0.0 -> latest</code></td> <tr>
 <td>[tls-1.1]</td>
 <td><code class="docutils literal notranslate">v6.0.0 -> latest</code></td> <tr>
 <td>[tls-1.2]</td>
 <td><code class="docutils literal notranslate">v6.0.0 -> latest</code></td> <tr>
 <td>[tls-1.3]</td>
 <td><code class="docutils literal notranslate">v6.0.0 -> latest</code></td> </table>
 </div>
 </li>
            <li> <span class="li-head">ssl_renegotiation</span> - Enable/disable secure renegotiation to comply with RFC 5746. <span class="li-normal">type: str</span> <span class="li-normal">choices: enable, disable</span>
 <a id='label242' href="javascript:ContentClick('label243', 'label242');" onmouseover="ContentPreview('label243');" onmouseout="ContentUnpreview('label243');" title="click to collapse or expand..."> more... </a>
 <div id="label243" style="display:none">
 <table border="1">
 <tr>
 <td></td>
 <td colspan="1">Supported Version Ranges</td>
 </tr>
 <tr>
 <td>ssl_renegotiation</td>
 <td><code class="docutils literal notranslate">v7.2.4 -> latest </code></td>
 </tr>
 <tr>
 <td>[enable]</td>
 <td><code class="docutils literal notranslate">v6.0.0 -> latest</code></td> <tr>
 <td>[disable]</td>
 <td><code class="docutils literal notranslate">v6.0.0 -> latest</code></td> </table>
 </div>
 </li>
            <li> <span class="li-head">ssl_vpn_web_portal</span> - SSL-VPN web portal. Source vpn.ssl.web.portal.name. <span class="li-normal">type: str</span>
 <a id='label244' href="javascript:ContentClick('label245', 'label244');" onmouseover="ContentPreview('label245');" onmouseout="ContentUnpreview('label245');" title="click to collapse or expand..."> more... </a>
 <div id="label245" style="display:none">
 <table border="1">
 <tr>
 <td></td>
 <td colspan="1">Supported Version Ranges</td>
 </tr>
 <tr>
 <td>ssl_vpn_web_portal</td>
 <td><code class="docutils literal notranslate">v7.0.4 -> latest </code></td>
 </tr>
 </table>
 </div>
 </li>
            <li> <span class="li-head">url_map</span> - URL pattern to match. <span class="li-normal">type: str</span>
 <a id='label246' href="javascript:ContentClick('label247', 'label246');" onmouseover="ContentPreview('label247');" onmouseout="ContentUnpreview('label247');" title="click to collapse or expand..."> more... </a>
 <div id="label247" style="display:none">
 <table border="1">
 <tr>
 <td></td>
 <td colspan="1">Supported Version Ranges</td>
 </tr>
 <tr>
 <td>url_map</td>
 <td><code class="docutils literal notranslate">v7.0.1 -> latest </code></td>
 </tr>
 </table>
 </div>
 </li>
            <li> <span class="li-head">url_map_type</span> - Type of url-map. <span class="li-normal">type: str</span> <span class="li-normal">choices: sub-string, wildcard, regex</span>
 <a id='label248' href="javascript:ContentClick('label249', 'label248');" onmouseover="ContentPreview('label249');" onmouseout="ContentUnpreview('label249');" title="click to collapse or expand..."> more... </a>
 <div id="label249" style="display:none">
 <table border="1">
 <tr>
 <td></td>
 <td colspan="1">Supported Version Ranges</td>
 </tr>
 <tr>
 <td>url_map_type</td>
 <td><code class="docutils literal notranslate">v7.0.1 -> latest </code></td>
 </tr>
 <tr>
 <td>[sub-string]</td>
 <td><code class="docutils literal notranslate">v6.0.0 -> latest</code></td> <tr>
 <td>[wildcard]</td>
 <td><code class="docutils literal notranslate">v6.0.0 -> latest</code></td> <tr>
 <td>[regex]</td>
 <td><code class="docutils literal notranslate">v6.0.0 -> latest</code></td> </table>
 </div>
 </li>
            <li> <span class="li-head">virtual_host</span> - Virtual host. Source firewall.access-proxy-virtual-host.name. <span class="li-normal">type: str</span>
 <a id='label250' href="javascript:ContentClick('label251', 'label250');" onmouseover="ContentPreview('label251');" onmouseout="ContentUnpreview('label251');" title="click to collapse or expand..."> more... </a>
 <div id="label251" style="display:none">
 <table border="1">
 <tr>
 <td></td>
 <td colspan="1">Supported Version Ranges</td>
 </tr>
 <tr>
 <td>virtual_host</td>
 <td><code class="docutils literal notranslate">v7.0.1 -> latest </code></td>
 </tr>
 </table>
 </div>
 </li>
            </ul>
        <li> <span class="li-head">auth_portal</span> - Enable/disable authentication portal. <span class="li-normal">type: str</span> <span class="li-normal">choices: disable, enable</span>
 <a id='label252' href="javascript:ContentClick('label253', 'label252');" onmouseover="ContentPreview('label253');" onmouseout="ContentUnpreview('label253');" title="click to collapse or expand..."> more... </a>
 <div id="label253" style="display:none">
 <table border="1">
 <tr>
 <td></td>
 <td colspan="1">Supported Version Ranges</td>
 </tr>
 <tr>
 <td>auth_portal</td>
 <td><code class="docutils literal notranslate">v7.0.4 -> latest </code></td>
 </tr>
 <tr>
 <td>[disable]</td>
 <td><code class="docutils literal notranslate">v6.0.0 -> latest</code></td> <tr>
 <td>[enable]</td>
 <td><code class="docutils literal notranslate">v6.0.0 -> latest</code></td> </table>
 </div>
 </li>
        <li> <span class="li-head">auth_virtual_host</span> - Virtual host for authentication portal. Source firewall.access-proxy-virtual-host.name. <span class="li-normal">type: str</span>
 <a id='label254' href="javascript:ContentClick('label255', 'label254');" onmouseover="ContentPreview('label255');" onmouseout="ContentUnpreview('label255');" title="click to collapse or expand..."> more... </a>
 <div id="label255" style="display:none">
 <table border="1">
 <tr>
 <td></td>
 <td colspan="1">Supported Version Ranges</td>
 </tr>
 <tr>
 <td>auth_virtual_host</td>
 <td><code class="docutils literal notranslate">v7.0.4 -> latest </code></td>
 </tr>
 </table>
 </div>
 </li>
        <li> <span class="li-head">client_cert</span> - Enable/disable to request client certificate. <span class="li-normal">type: str</span> <span class="li-normal">choices: disable, enable</span>
 <a id='label256' href="javascript:ContentClick('label257', 'label256');" onmouseover="ContentPreview('label257');" onmouseout="ContentUnpreview('label257');" title="click to collapse or expand..."> more... </a>
 <div id="label257" style="display:none">
 <table border="1">
 <tr>
 <td></td>
 <td colspan="1">Supported Version Ranges</td>
 </tr>
 <tr>
 <td>client_cert</td>
 <td><code class="docutils literal notranslate">v7.0.1 -> latest </code></td>
 </tr>
 <tr>
 <td>[disable]</td>
 <td><code class="docutils literal notranslate">v6.0.0 -> latest</code></td> <tr>
 <td>[enable]</td>
 <td><code class="docutils literal notranslate">v6.0.0 -> latest</code></td> </table>
 </div>
 </li>
        <li> <span class="li-head">decrypted_traffic_mirror</span> - Decrypted traffic mirror. Source firewall.decrypted-traffic-mirror.name. <span class="li-normal">type: str</span>
 <a id='label258' href="javascript:ContentClick('label259', 'label258');" onmouseover="ContentPreview('label259');" onmouseout="ContentUnpreview('label259');" title="click to collapse or expand..."> more... </a>
 <div id="label259" style="display:none">
 <table border="1">
 <tr>
 <td></td>
 <td colspan="1">Supported Version Ranges</td>
 </tr>
 <tr>
 <td>decrypted_traffic_mirror</td>
 <td><code class="docutils literal notranslate">v7.0.2 -> latest </code></td>
 </tr>
 </table>
 </div>
 </li>
        <li> <span class="li-head">empty_cert_action</span> - Action of an empty client certificate. <span class="li-normal">type: str</span> <span class="li-normal">choices: accept, block, accept-unmanageable</span>
 <a id='label260' href="javascript:ContentClick('label261', 'label260');" onmouseover="ContentPreview('label261');" onmouseout="ContentUnpreview('label261');" title="click to collapse or expand..."> more... </a>
 <div id="label261" style="display:none">
 <table border="1">
 <tr>
 <td></td>
 <td colspan="1">Supported Version Ranges</td>
 </tr>
 <tr>
 <td>empty_cert_action</td>
 <td><code class="docutils literal notranslate">v7.0.1 -> latest </code></td>
 </tr>
 <tr>
 <td>[accept]</td>
 <td><code class="docutils literal notranslate">v6.0.0 -> latest</code></td> <tr>
 <td>[block]</td>
 <td><code class="docutils literal notranslate">v6.0.0 -> latest</code></td> <tr>
 <td>[accept-unmanageable]</td>
 <td><code class="docutils literal notranslate">v7.2.1 -> latest</code></td>
 </tr>
 </table>
 </div>
 </li>
        <li> <span class="li-head">http_supported_max_version</span> - Maximum supported HTTP versions. default = HTTP2 <span class="li-normal">type: str</span> <span class="li-normal">choices: http1, http2</span>
 <a id='label262' href="javascript:ContentClick('label263', 'label262');" onmouseover="ContentPreview('label263');" onmouseout="ContentUnpreview('label263');" title="click to collapse or expand..."> more... </a>
 <div id="label263" style="display:none">
 <table border="1">
 <tr>
 <td></td>
 <td colspan="1">Supported Version Ranges</td>
 </tr>
 <tr>
 <td>http_supported_max_version</td>
 <td><code class="docutils literal notranslate">v7.2.4 -> v7.4.0 </code></td>
 </tr>
 <tr>
 <td>[http1]</td>
 <td><code class="docutils literal notranslate">v6.0.0 -> latest</code></td> <tr>
 <td>[http2]</td>
 <td><code class="docutils literal notranslate">v6.0.0 -> latest</code></td> </table>
 </div>
 </li>
        <li> <span class="li-head">log_blocked_traffic</span> - Enable/disable logging of blocked traffic. <span class="li-normal">type: str</span> <span class="li-normal">choices: enable, disable</span>
 <a id='label264' href="javascript:ContentClick('label265', 'label264');" onmouseover="ContentPreview('label265');" onmouseout="ContentUnpreview('label265');" title="click to collapse or expand..."> more... </a>
 <div id="label265" style="display:none">
 <table border="1">
 <tr>
 <td></td>
 <td colspan="1">Supported Version Ranges</td>
 </tr>
 <tr>
 <td>log_blocked_traffic</td>
 <td><code class="docutils literal notranslate">v7.0.2 -> latest </code></td>
 </tr>
 <tr>
 <td>[enable]</td>
 <td><code class="docutils literal notranslate">v6.0.0 -> latest</code></td> <tr>
 <td>[disable]</td>
 <td><code class="docutils literal notranslate">v6.0.0 -> latest</code></td> </table>
 </div>
 </li>
        <li> <span class="li-head">name</span> - Access Proxy name. <span class="li-normal">type: str</span> <span class="li-required">required: true</span>
 <a id='label266' href="javascript:ContentClick('label267', 'label266');" onmouseover="ContentPreview('label267');" onmouseout="ContentUnpreview('label267');" title="click to collapse or expand..."> more... </a>
 <div id="label267" style="display:none">
 <table border="1">
 <tr>
 <td></td>
 <td colspan="1">Supported Version Ranges</td>
 </tr>
 <tr>
 <td>name</td>
 <td><code class="docutils literal notranslate">v7.0.1 -> latest </code></td>
 </tr>
 </table>
 </div>
 </li>
        <li> <span class="li-head">svr_pool_multiplex</span> - Enable/disable server pool multiplexing. Share connected server in HTTP, HTTPS, and web-portal api-gateway. <span class="li-normal">type: str</span> <span class="li-normal">choices: enable, disable</span>
 <a id='label268' href="javascript:ContentClick('label269', 'label268');" onmouseover="ContentPreview('label269');" onmouseout="ContentUnpreview('label269');" title="click to collapse or expand..."> more... </a>
 <div id="label269" style="display:none">
 <table border="1">
 <tr>
 <td></td>
 <td colspan="1">Supported Version Ranges</td>
 </tr>
 <tr>
 <td>svr_pool_multiplex</td>
 <td><code class="docutils literal notranslate">v7.2.4 -> latest </code></td>
 </tr>
 <tr>
 <td>[enable]</td>
 <td><code class="docutils literal notranslate">v6.0.0 -> latest</code></td> <tr>
 <td>[disable]</td>
 <td><code class="docutils literal notranslate">v6.0.0 -> latest</code></td> </table>
 </div>
 </li>
        <li> <span class="li-head">svr_pool_server_max_concurrent_request</span> - Maximum number of concurrent requests that servers in server pool could handle . <span class="li-normal">type: int</span>
 <a id='label270' href="javascript:ContentClick('label271', 'label270');" onmouseover="ContentPreview('label271');" onmouseout="ContentUnpreview('label271');" title="click to collapse or expand..."> more... </a>
 <div id="label271" style="display:none">
 <table border="1">
 <tr>
 <td></td>
 <td colspan="1">Supported Version Ranges</td>
 </tr>
 <tr>
 <td>svr_pool_server_max_concurrent_request</td>
 <td><code class="docutils literal notranslate">v7.4.1 -> latest </code></td>
 </tr>
 </table>
 </div>
 </li>
        <li> <span class="li-head">svr_pool_server_max_request</span> - Maximum number of requests that servers in server pool handle before disconnecting . <span class="li-normal">type: int</span>
 <a id='label272' href="javascript:ContentClick('label273', 'label272');" onmouseover="ContentPreview('label273');" onmouseout="ContentUnpreview('label273');" title="click to collapse or expand..."> more... </a>
 <div id="label273" style="display:none">
 <table border="1">
 <tr>
 <td></td>
 <td colspan="1">Supported Version Ranges</td>
 </tr>
 <tr>
 <td>svr_pool_server_max_request</td>
 <td><code class="docutils literal notranslate">v7.2.4 -> latest </code></td>
 </tr>
 </table>
 </div>
 </li>
        <li> <span class="li-head">svr_pool_ttl</span> - Time-to-live in the server pool for idle connections to servers. <span class="li-normal">type: int</span>
 <a id='label274' href="javascript:ContentClick('label275', 'label274');" onmouseover="ContentPreview('label275');" onmouseout="ContentUnpreview('label275');" title="click to collapse or expand..."> more... </a>
 <div id="label275" style="display:none">
 <table border="1">
 <tr>
 <td></td>
 <td colspan="1">Supported Version Ranges</td>
 </tr>
 <tr>
 <td>svr_pool_ttl</td>
 <td><code class="docutils literal notranslate">v7.2.4 -> latest </code></td>
 </tr>
 </table>
 </div>
 </li>
        <li> <span class="li-head">user_agent_detect</span> - Enable/disable to detect device type by HTTP user-agent if no client certificate provided. <span class="li-normal">type: str</span> <span class="li-normal">choices: disable, enable</span>
 <a id='label276' href="javascript:ContentClick('label277', 'label276');" onmouseover="ContentPreview('label277');" onmouseout="ContentUnpreview('label277');" title="click to collapse or expand..."> more... </a>
 <div id="label277" style="display:none">
 <table border="1">
 <tr>
 <td></td>
 <td colspan="1">Supported Version Ranges</td>
 </tr>
 <tr>
 <td>user_agent_detect</td>
 <td><code class="docutils literal notranslate">v7.2.1 -> latest </code></td>
 </tr>
 <tr>
 <td>[disable]</td>
 <td><code class="docutils literal notranslate">v6.0.0 -> latest</code></td> <tr>
 <td>[enable]</td>
 <td><code class="docutils literal notranslate">v6.0.0 -> latest</code></td> </table>
 </div>
 </li>
        <li> <span class="li-head">vip</span> - Virtual IP name. Source firewall.vip6.name. <span class="li-normal">type: str</span>
 <a id='label278' href="javascript:ContentClick('label279', 'label278');" onmouseover="ContentPreview('label279');" onmouseout="ContentUnpreview('label279');" title="click to collapse or expand..."> more... </a>
 <div id="label279" style="display:none">
 <table border="1">
 <tr>
 <td></td>
 <td colspan="1">Supported Version Ranges</td>
 </tr>
 <tr>
 <td>vip</td>
 <td><code class="docutils literal notranslate">v7.0.1 -> latest </code></td>
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
    
    - name: Configure IPv6 access proxy.
      fortinet.fortios.fortios_firewall_access_proxy6:
          vdom: "{{ vdom }}"
          state: "present"
          access_token: "<your_own_value>"
          firewall_access_proxy6:
              add_vhost_domain_to_dnsdb: "enable"
              api_gateway:
                  -
                      application:
                          -
                              name: "default_name_6"
                      h2_support: "enable"
                      h3_support: "enable"
                      http_cookie_age: "60"
                      http_cookie_domain: "<your_own_value>"
                      http_cookie_domain_from_host: "disable"
                      http_cookie_generation: "0"
                      http_cookie_path: "<your_own_value>"
                      http_cookie_share: "disable"
                      https_cookie_secure: "disable"
                      id: "16"
                      ldb_method: "static"
                      persistence: "none"
                      quic:
                          ack_delay_exponent: "3"
                          active_connection_id_limit: "2"
                          active_migration: "enable"
                          grease_quic_bit: "enable"
                          max_ack_delay: "25"
                          max_datagram_frame_size: "1500"
                          max_idle_timeout: "30000"
                          max_udp_payload_size: "1500"
                      realservers:
                          -
                              addr_type: "ip"
                              address: "<your_own_value> (source firewall.address.name firewall.addrgrp.name)"
                              domain: "<your_own_value>"
                              external_auth: "enable"
                              health_check: "disable"
                              health_check_proto: "ping"
                              holddown_interval: "enable"
                              http_host: "myhostname"
                              id: "37"
                              ip: "<your_own_value>"
                              mappedport: "<your_own_value>"
                              port: "443"
                              ssh_client_cert: "<your_own_value> (source firewall.access-proxy-ssh-client-cert.name)"
                              ssh_host_key:
                                  -
                                      name: "default_name_43 (source firewall.ssh.host-key.name)"
                              ssh_host_key_validation: "disable"
                              status: "active"
                              translate_host: "enable"
                              tunnel_encryption: "enable"
                              type: "tcp-forwarding"
                              weight: "1"
                      saml_redirect: "disable"
                      saml_server: "<your_own_value> (source user.saml.name)"
                      service: "http"
                      ssl_algorithm: "high"
                      ssl_cipher_suites:
                          -
                              cipher: "TLS-AES-128-GCM-SHA256"
                              priority: "<you_own_value>"
                              versions: "tls-1.0"
                      ssl_dh_bits: "768"
                      ssl_max_version: "tls-1.0"
                      ssl_min_version: "tls-1.0"
                      ssl_renegotiation: "enable"
                      ssl_vpn_web_portal: "<your_own_value> (source vpn.ssl.web.portal.name)"
                      url_map: "<your_own_value>"
                      url_map_type: "sub-string"
                      virtual_host: "myhostname (source firewall.access-proxy-virtual-host.name)"
              api_gateway6:
                  -
                      application:
                          -
                              name: "default_name_68"
                      h2_support: "enable"
                      h3_support: "enable"
                      http_cookie_age: "60"
                      http_cookie_domain: "<your_own_value>"
                      http_cookie_domain_from_host: "disable"
                      http_cookie_generation: "0"
                      http_cookie_path: "<your_own_value>"
                      http_cookie_share: "disable"
                      https_cookie_secure: "disable"
                      id: "78"
                      ldb_method: "static"
                      persistence: "none"
                      quic:
                          ack_delay_exponent: "3"
                          active_connection_id_limit: "2"
                          active_migration: "enable"
                          grease_quic_bit: "enable"
                          max_ack_delay: "25"
                          max_datagram_frame_size: "1500"
                          max_idle_timeout: "30000"
                          max_udp_payload_size: "1500"
                      realservers:
                          -
                              addr_type: "ip"
                              address: "<your_own_value> (source firewall.address6.name firewall.addrgrp6.name)"
                              domain: "<your_own_value>"
                              external_auth: "enable"
                              health_check: "disable"
                              health_check_proto: "ping"
                              holddown_interval: "enable"
                              http_host: "myhostname"
                              id: "99"
                              ip: "<your_own_value>"
                              mappedport: "<your_own_value>"
                              port: "443"
                              ssh_client_cert: "<your_own_value> (source firewall.access-proxy-ssh-client-cert.name)"
                              ssh_host_key:
                                  -
                                      name: "default_name_105 (source firewall.ssh.host-key.name)"
                              ssh_host_key_validation: "disable"
                              status: "active"
                              translate_host: "enable"
                              tunnel_encryption: "enable"
                              type: "tcp-forwarding"
                              weight: "1"
                      saml_redirect: "disable"
                      saml_server: "<your_own_value> (source user.saml.name)"
                      service: "http"
                      ssl_algorithm: "high"
                      ssl_cipher_suites:
                          -
                              cipher: "TLS-AES-128-GCM-SHA256"
                              priority: "<you_own_value>"
                              versions: "tls-1.0"
                      ssl_dh_bits: "768"
                      ssl_max_version: "tls-1.0"
                      ssl_min_version: "tls-1.0"
                      ssl_renegotiation: "enable"
                      ssl_vpn_web_portal: "<your_own_value> (source vpn.ssl.web.portal.name)"
                      url_map: "<your_own_value>"
                      url_map_type: "sub-string"
                      virtual_host: "myhostname (source firewall.access-proxy-virtual-host.name)"
              auth_portal: "disable"
              auth_virtual_host: "myhostname (source firewall.access-proxy-virtual-host.name)"
              client_cert: "disable"
              decrypted_traffic_mirror: "<your_own_value> (source firewall.decrypted-traffic-mirror.name)"
              empty_cert_action: "accept"
              http_supported_max_version: "http1"
              log_blocked_traffic: "enable"
              name: "default_name_135"
              svr_pool_multiplex: "enable"
              svr_pool_server_max_concurrent_request: "0"
              svr_pool_server_max_request: "0"
              svr_pool_ttl: "15"
              user_agent_detect: "disable"
              vip: "<your_own_value> (source firewall.vip6.name)"


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
