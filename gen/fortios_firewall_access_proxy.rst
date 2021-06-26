:source: fortios_firewall_access_proxy.py

:orphan:

.. fortios_firewall_access_proxy:

fortios_firewall_access_proxy -- Configure Access Proxy in Fortinet's FortiOS and FortiGate.
++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++

.. versionadded:: 2.10

.. contents::
   :local:
   :depth: 1


Synopsis
--------
- This module is able to configure a FortiGate or FortiOS (FOS) device by allowing the user to set and modify firewall feature and access_proxy category. Examples include all parameters and values need to be adjusted to datasources before usage. Tested with FOS v6.0.0



Requirements
------------
The below requirements are needed on the host that executes this module.

- ansible>=2.9.0


FortiOS Version Compatibility
-----------------------------


.. raw:: html

 <br>
 <table>
 <tr>
 <td></td>
 <td><code class="docutils literal notranslate">v7.0.0 </code></td>
 </tr>
 <tr>
 <td>fortios_firewall_access_proxy</td>
 <td>yes</td>
 </tr>
 </table>
 <p>



Parameters
----------


.. raw:: html

    <ul>
    <li> <span class="li-head">access_token</span> - Token-based authentication. Generated from GUI of Fortigate. <span class="li-normal">type: str</span> <span class="li-required">required: False</span> </li>
    <li> <span class="li-head">enable_log</span> - Enable/Disable logging for task. <span class="li-normal">type: bool</span> <span class="li-required">required: False</span> <span class="li-normal">default: False</span> </li>
    <li> <span class="li-head">vdom</span> - Virtual domain, among those defined previously. A vdom is a virtual instance of the FortiGate that can be configured and used as a different unit. <span class="li-normal">type: str</span> <span class="li-normal">default: root</span> </li>
    <li> <span class="li-head">state</span> - Indicates whether to create or remove the object. <span class="li-normal">type: str</span> <span class="li-required">required: True</span> <span class="li-normal">choices: present, absent</span> </li>
    <li> <span class="li-head">firewall_access_proxy</span> - Configure Access Proxy. <span class="li-normal">type: dict</span>
 <a id='label0' href="javascript:ContentClick('label1', 'label0');" onmouseover="ContentPreview('label1');" onmouseout="ContentUnpreview('label1');" title="click to collapse or expand..."> more... </a>
 <div id="label1" style="display:none">
 <table border="1">
 <tr>
 <td></td>
 <td><code class="docutils literal notranslate">v7.0.0 </code></td>
 </tr>
 <tr>
 <td>firewall_access_proxy</td>
 <td>yes</td>
 </tr>
 </table>
 </div>
 </li>
        <ul class="ul-self">
        <li> <span class="li-head">api_gateway</span> - Set API Gateway. <span class="li-normal">type: list</span>
 <a id='label2' href="javascript:ContentClick('label3', 'label2');" onmouseover="ContentPreview('label3');" onmouseout="ContentUnpreview('label3');" title="click to collapse or expand..."> more... </a>
 <div id="label3" style="display:none">
 <table border="1">
 <tr>
 <td></td>
 <td><code class="docutils literal notranslate">v7.0.0 </code></td>
 </tr>
 <tr>
 <td>api_gateway</td>
 <td>yes</td>
 </tr>
 </table>
 </div>
 </li>
            <ul class="ul-self">
            <li> <span class="li-head">http_cookie_age</span> - Time in minutes that client web browsers should keep a cookie. Default is 60 minutes. 0 = no time limit. <span class="li-normal">type: int</span>
 <a id='label4' href="javascript:ContentClick('label5', 'label4');" onmouseover="ContentPreview('label5');" onmouseout="ContentUnpreview('label5');" title="click to collapse or expand..."> more... </a>
 <div id="label5" style="display:none">
 <table border="1">
 <tr>
 <td></td>
 <td><code class="docutils literal notranslate">v7.0.0 </code></td>
 </tr>
 <tr>
 <td>http_cookie_age</td>
 <td>yes</td>
 </tr>
 </table>
 </div>
 </li>
            <li> <span class="li-head">http_cookie_domain</span> - Domain that HTTP cookie persistence should apply to. <span class="li-normal">type: str</span>
 <a id='label6' href="javascript:ContentClick('label7', 'label6');" onmouseover="ContentPreview('label7');" onmouseout="ContentUnpreview('label7');" title="click to collapse or expand..."> more... </a>
 <div id="label7" style="display:none">
 <table border="1">
 <tr>
 <td></td>
 <td><code class="docutils literal notranslate">v7.0.0 </code></td>
 </tr>
 <tr>
 <td>http_cookie_domain</td>
 <td>yes</td>
 </tr>
 </table>
 </div>
 </li>
            <li> <span class="li-head">http_cookie_domain_from_host</span> - Enable/disable use of HTTP cookie domain from host field in HTTP. <span class="li-normal">type: str</span> <span class="li-normal">choices: disable, enable</span>
 <a id='label8' href="javascript:ContentClick('label9', 'label8');" onmouseover="ContentPreview('label9');" onmouseout="ContentUnpreview('label9');" title="click to collapse or expand..."> more... </a>
 <div id="label9" style="display:none">
 <table border="1">
 <tr>
 <td></td>
 <td><code class="docutils literal notranslate">v7.0.0 </code></td>
 </tr>
 <tr>
 <td>http_cookie_domain_from_host</td>
 <td>yes</td>
 </tr>
 <tr>
 <td>[disable]</td>
 <td>yes</td>
 </tr>
 <tr>
 <td>[enable]</td>
 <td>yes</td>
 </tr>
 </table>
 </div>
 </li>
            <li> <span class="li-head">http_cookie_generation</span> - Generation of HTTP cookie to be accepted. Changing invalidates all existing cookies. <span class="li-normal">type: int</span>
 <a id='label10' href="javascript:ContentClick('label11', 'label10');" onmouseover="ContentPreview('label11');" onmouseout="ContentUnpreview('label11');" title="click to collapse or expand..."> more... </a>
 <div id="label11" style="display:none">
 <table border="1">
 <tr>
 <td></td>
 <td><code class="docutils literal notranslate">v7.0.0 </code></td>
 </tr>
 <tr>
 <td>http_cookie_generation</td>
 <td>yes</td>
 </tr>
 </table>
 </div>
 </li>
            <li> <span class="li-head">http_cookie_path</span> - Limit HTTP cookie persistence to the specified path. <span class="li-normal">type: str</span>
 <a id='label12' href="javascript:ContentClick('label13', 'label12');" onmouseover="ContentPreview('label13');" onmouseout="ContentUnpreview('label13');" title="click to collapse or expand..."> more... </a>
 <div id="label13" style="display:none">
 <table border="1">
 <tr>
 <td></td>
 <td><code class="docutils literal notranslate">v7.0.0 </code></td>
 </tr>
 <tr>
 <td>http_cookie_path</td>
 <td>yes</td>
 </tr>
 </table>
 </div>
 </li>
            <li> <span class="li-head">http_cookie_share</span> - Control sharing of cookies across API Gateway. same-ip means a cookie from one virtual server can be used by another. Disable stops cookie sharing. <span class="li-normal">type: str</span> <span class="li-normal">choices: disable, same-ip</span>
 <a id='label14' href="javascript:ContentClick('label15', 'label14');" onmouseover="ContentPreview('label15');" onmouseout="ContentUnpreview('label15');" title="click to collapse or expand..."> more... </a>
 <div id="label15" style="display:none">
 <table border="1">
 <tr>
 <td></td>
 <td><code class="docutils literal notranslate">v7.0.0 </code></td>
 </tr>
 <tr>
 <td>http_cookie_share</td>
 <td>yes</td>
 </tr>
 <tr>
 <td>[disable]</td>
 <td>yes</td>
 </tr>
 <tr>
 <td>[same-ip]</td>
 <td>yes</td>
 </tr>
 </table>
 </div>
 </li>
            <li> <span class="li-head">https_cookie_secure</span> - Enable/disable verification that inserted HTTPS cookies are secure. <span class="li-normal">type: str</span> <span class="li-normal">choices: disable, enable</span>
 <a id='label16' href="javascript:ContentClick('label17', 'label16');" onmouseover="ContentPreview('label17');" onmouseout="ContentUnpreview('label17');" title="click to collapse or expand..."> more... </a>
 <div id="label17" style="display:none">
 <table border="1">
 <tr>
 <td></td>
 <td><code class="docutils literal notranslate">v7.0.0 </code></td>
 </tr>
 <tr>
 <td>https_cookie_secure</td>
 <td>yes</td>
 </tr>
 <tr>
 <td>[disable]</td>
 <td>yes</td>
 </tr>
 <tr>
 <td>[enable]</td>
 <td>yes</td>
 </tr>
 </table>
 </div>
 </li>
            <li> <span class="li-head">id</span> - API Gateway ID. <span class="li-normal">type: int</span> <span class="li-required">required: True</span>
 <a id='label18' href="javascript:ContentClick('label19', 'label18');" onmouseover="ContentPreview('label19');" onmouseout="ContentUnpreview('label19');" title="click to collapse or expand..."> more... </a>
 <div id="label19" style="display:none">
 <table border="1">
 <tr>
 <td></td>
 <td><code class="docutils literal notranslate">v7.0.0 </code></td>
 </tr>
 <tr>
 <td>id</td>
 <td>yes</td>
 </tr>
 </table>
 </div>
 </li>
            <li> <span class="li-head">ldb_method</span> - Method used to distribute sessions to real servers. <span class="li-normal">type: str</span> <span class="li-normal">choices: static, round-robin, weighted, least-session, least-rtt, first-alive, http-host</span>
 <a id='label20' href="javascript:ContentClick('label21', 'label20');" onmouseover="ContentPreview('label21');" onmouseout="ContentUnpreview('label21');" title="click to collapse or expand..."> more... </a>
 <div id="label21" style="display:none">
 <table border="1">
 <tr>
 <td></td>
 <td><code class="docutils literal notranslate">v7.0.0 </code></td>
 </tr>
 <tr>
 <td>ldb_method</td>
 <td>yes</td>
 </tr>
 <tr>
 <td>[static]</td>
 <td>yes</td>
 </tr>
 <tr>
 <td>[round-robin]</td>
 <td>yes</td>
 </tr>
 <tr>
 <td>[weighted]</td>
 <td>yes</td>
 </tr>
 <tr>
 <td>[least-session]</td>
 <td>yes</td>
 </tr>
 <tr>
 <td>[least-rtt]</td>
 <td>yes</td>
 </tr>
 <tr>
 <td>[first-alive]</td>
 <td>yes</td>
 </tr>
 <tr>
 <td>[http-host]</td>
 <td>yes</td>
 </tr>
 </table>
 </div>
 </li>
            <li> <span class="li-head">persistence</span> - Configure how to make sure that clients connect to the same server every time they make a request that is part of the same session. <span class="li-normal">type: str</span> <span class="li-normal">choices: none, http-cookie</span>
 <a id='label22' href="javascript:ContentClick('label23', 'label22');" onmouseover="ContentPreview('label23');" onmouseout="ContentUnpreview('label23');" title="click to collapse or expand..."> more... </a>
 <div id="label23" style="display:none">
 <table border="1">
 <tr>
 <td></td>
 <td><code class="docutils literal notranslate">v7.0.0 </code></td>
 </tr>
 <tr>
 <td>persistence</td>
 <td>yes</td>
 </tr>
 <tr>
 <td>[none]</td>
 <td>yes</td>
 </tr>
 <tr>
 <td>[http-cookie]</td>
 <td>yes</td>
 </tr>
 </table>
 </div>
 </li>
            <li> <span class="li-head">realservers</span> - Select the real servers that this Access Proxy will distribute traffic to. <span class="li-normal">type: list</span>
 <a id='label24' href="javascript:ContentClick('label25', 'label24');" onmouseover="ContentPreview('label25');" onmouseout="ContentUnpreview('label25');" title="click to collapse or expand..."> more... </a>
 <div id="label25" style="display:none">
 <table border="1">
 <tr>
 <td></td>
 <td><code class="docutils literal notranslate">v7.0.0 </code></td>
 </tr>
 <tr>
 <td>realservers</td>
 <td>yes</td>
 </tr>
 </table>
 </div>
 </li>
                <ul class="ul-self">
                <li> <span class="li-head">address</span> - Address or address group of the real server. Source firewall.address.name firewall.addrgrp.name. <span class="li-normal">type: str</span>
 <a id='label26' href="javascript:ContentClick('label27', 'label26');" onmouseover="ContentPreview('label27');" onmouseout="ContentUnpreview('label27');" title="click to collapse or expand..."> more... </a>
 <div id="label27" style="display:none">
 <table border="1">
 <tr>
 <td></td>
 <td><code class="docutils literal notranslate">v7.0.0 </code></td>
 </tr>
 <tr>
 <td>address</td>
 <td>yes</td>
 </tr>
 </table>
 </div>
 </li>
                <li> <span class="li-head">health_check</span> - Enable to check the responsiveness of the real server before forwarding traffic. <span class="li-normal">type: str</span> <span class="li-normal">choices: disable, enable</span>
 <a id='label28' href="javascript:ContentClick('label29', 'label28');" onmouseover="ContentPreview('label29');" onmouseout="ContentUnpreview('label29');" title="click to collapse or expand..."> more... </a>
 <div id="label29" style="display:none">
 <table border="1">
 <tr>
 <td></td>
 <td><code class="docutils literal notranslate">v7.0.0 </code></td>
 </tr>
 <tr>
 <td>health_check</td>
 <td>yes</td>
 </tr>
 <tr>
 <td>[disable]</td>
 <td>yes</td>
 </tr>
 <tr>
 <td>[enable]</td>
 <td>yes</td>
 </tr>
 </table>
 </div>
 </li>
                <li> <span class="li-head">health_check_proto</span> - Protocol of the health check monitor to use when polling to determine server"s connectivity status. <span class="li-normal">type: str</span> <span class="li-normal">choices: ping, http, tcp-connect</span>
 <a id='label30' href="javascript:ContentClick('label31', 'label30');" onmouseover="ContentPreview('label31');" onmouseout="ContentUnpreview('label31');" title="click to collapse or expand..."> more... </a>
 <div id="label31" style="display:none">
 <table border="1">
 <tr>
 <td></td>
 <td><code class="docutils literal notranslate">v7.0.0 </code></td>
 </tr>
 <tr>
 <td>health_check_proto</td>
 <td>yes</td>
 </tr>
 <tr>
 <td>[ping]</td>
 <td>yes</td>
 </tr>
 <tr>
 <td>[http]</td>
 <td>yes</td>
 </tr>
 <tr>
 <td>[tcp-connect]</td>
 <td>yes</td>
 </tr>
 </table>
 </div>
 </li>
                <li> <span class="li-head">http_host</span> - HTTP server domain name in HTTP header. <span class="li-normal">type: str</span>
 <a id='label32' href="javascript:ContentClick('label33', 'label32');" onmouseover="ContentPreview('label33');" onmouseout="ContentUnpreview('label33');" title="click to collapse or expand..."> more... </a>
 <div id="label33" style="display:none">
 <table border="1">
 <tr>
 <td></td>
 <td><code class="docutils literal notranslate">v7.0.0 </code></td>
 </tr>
 <tr>
 <td>http_host</td>
 <td>yes</td>
 </tr>
 </table>
 </div>
 </li>
                <li> <span class="li-head">id</span> - Real server ID. <span class="li-normal">type: int</span> <span class="li-required">required: True</span>
 <a id='label34' href="javascript:ContentClick('label35', 'label34');" onmouseover="ContentPreview('label35');" onmouseout="ContentUnpreview('label35');" title="click to collapse or expand..."> more... </a>
 <div id="label35" style="display:none">
 <table border="1">
 <tr>
 <td></td>
 <td><code class="docutils literal notranslate">v7.0.0 </code></td>
 </tr>
 <tr>
 <td>id</td>
 <td>yes</td>
 </tr>
 </table>
 </div>
 </li>
                <li> <span class="li-head">ip</span> - IP address of the real server. <span class="li-normal">type: str</span>
 <a id='label36' href="javascript:ContentClick('label37', 'label36');" onmouseover="ContentPreview('label37');" onmouseout="ContentUnpreview('label37');" title="click to collapse or expand..."> more... </a>
 <div id="label37" style="display:none">
 <table border="1">
 <tr>
 <td></td>
 <td><code class="docutils literal notranslate">v7.0.0 </code></td>
 </tr>
 <tr>
 <td>ip</td>
 <td>yes</td>
 </tr>
 </table>
 </div>
 </li>
                <li> <span class="li-head">mappedport</span> - Port for communicating with the real server. <span class="li-normal">type: str</span>
 <a id='label38' href="javascript:ContentClick('label39', 'label38');" onmouseover="ContentPreview('label39');" onmouseout="ContentUnpreview('label39');" title="click to collapse or expand..."> more... </a>
 <div id="label39" style="display:none">
 <table border="1">
 <tr>
 <td></td>
 <td><code class="docutils literal notranslate">v7.0.0 </code></td>
 </tr>
 <tr>
 <td>mappedport</td>
 <td>yes</td>
 </tr>
 </table>
 </div>
 </li>
                <li> <span class="li-head">port</span> - Port for communicating with the real server. <span class="li-normal">type: int</span>
 <a id='label40' href="javascript:ContentClick('label41', 'label40');" onmouseover="ContentPreview('label41');" onmouseout="ContentUnpreview('label41');" title="click to collapse or expand..."> more... </a>
 <div id="label41" style="display:none">
 <table border="1">
 <tr>
 <td></td>
 <td><code class="docutils literal notranslate">v7.0.0 </code></td>
 </tr>
 <tr>
 <td>port</td>
 <td>yes</td>
 </tr>
 </table>
 </div>
 </li>
                <li> <span class="li-head">status</span> - Set the status of the real server to active so that it can accept traffic, or on standby or disabled so no traffic is sent. <span class="li-normal">type: str</span> <span class="li-normal">choices: active, standby, disable</span>
 <a id='label42' href="javascript:ContentClick('label43', 'label42');" onmouseover="ContentPreview('label43');" onmouseout="ContentUnpreview('label43');" title="click to collapse or expand..."> more... </a>
 <div id="label43" style="display:none">
 <table border="1">
 <tr>
 <td></td>
 <td><code class="docutils literal notranslate">v7.0.0 </code></td>
 </tr>
 <tr>
 <td>status</td>
 <td>yes</td>
 </tr>
 <tr>
 <td>[active]</td>
 <td>yes</td>
 </tr>
 <tr>
 <td>[standby]</td>
 <td>yes</td>
 </tr>
 <tr>
 <td>[disable]</td>
 <td>yes</td>
 </tr>
 </table>
 </div>
 </li>
                <li> <span class="li-head">weight</span> - Weight of the real server. If weighted load balancing is enabled, the server with the highest weight gets more connections. <span class="li-normal">type: int</span>
 <a id='label44' href="javascript:ContentClick('label45', 'label44');" onmouseover="ContentPreview('label45');" onmouseout="ContentUnpreview('label45');" title="click to collapse or expand..."> more... </a>
 <div id="label45" style="display:none">
 <table border="1">
 <tr>
 <td></td>
 <td><code class="docutils literal notranslate">v7.0.0 </code></td>
 </tr>
 <tr>
 <td>weight</td>
 <td>yes</td>
 </tr>
 </table>
 </div>
 </li>
                </ul>
            <li> <span class="li-head">saml_server</span> - SAML service provider configuration for VIP authentication. Source user.saml.name. <span class="li-normal">type: str</span>
 <a id='label46' href="javascript:ContentClick('label47', 'label46');" onmouseover="ContentPreview('label47');" onmouseout="ContentUnpreview('label47');" title="click to collapse or expand..."> more... </a>
 <div id="label47" style="display:none">
 <table border="1">
 <tr>
 <td></td>
 <td><code class="docutils literal notranslate">v7.0.0 </code></td>
 </tr>
 <tr>
 <td>saml_server</td>
 <td>yes</td>
 </tr>
 </table>
 </div>
 </li>
            <li> <span class="li-head">service</span> - Service. <span class="li-normal">type: str</span> <span class="li-normal">choices: http, https, tcp-forwarding, samlsp</span>
 <a id='label48' href="javascript:ContentClick('label49', 'label48');" onmouseover="ContentPreview('label49');" onmouseout="ContentUnpreview('label49');" title="click to collapse or expand..."> more... </a>
 <div id="label49" style="display:none">
 <table border="1">
 <tr>
 <td></td>
 <td><code class="docutils literal notranslate">v7.0.0 </code></td>
 </tr>
 <tr>
 <td>service</td>
 <td>yes</td>
 </tr>
 <tr>
 <td>[http]</td>
 <td>yes</td>
 </tr>
 <tr>
 <td>[https]</td>
 <td>yes</td>
 </tr>
 <tr>
 <td>[tcp-forwarding]</td>
 <td>yes</td>
 </tr>
 <tr>
 <td>[samlsp]</td>
 <td>yes</td>
 </tr>
 </table>
 </div>
 </li>
            <li> <span class="li-head">ssl_algorithm</span> - Permitted encryption algorithms for the server side of SSL full mode sessions according to encryption strength. <span class="li-normal">type: str</span> <span class="li-normal">choices: high, medium, low, custom</span>
 <a id='label50' href="javascript:ContentClick('label51', 'label50');" onmouseover="ContentPreview('label51');" onmouseout="ContentUnpreview('label51');" title="click to collapse or expand..."> more... </a>
 <div id="label51" style="display:none">
 <table border="1">
 <tr>
 <td></td>
 <td><code class="docutils literal notranslate">v7.0.0 </code></td>
 </tr>
 <tr>
 <td>ssl_algorithm</td>
 <td>yes</td>
 </tr>
 <tr>
 <td>[high]</td>
 <td>yes</td>
 </tr>
 <tr>
 <td>[medium]</td>
 <td>yes</td>
 </tr>
 <tr>
 <td>[low]</td>
 <td>yes</td>
 </tr>
 <tr>
 <td>[custom]</td>
 <td>yes</td>
 </tr>
 </table>
 </div>
 </li>
            <li> <span class="li-head">ssl_cipher_suites</span> - SSL/TLS cipher suites to offer to a server, ordered by priority. <span class="li-normal">type: list</span>
 <a id='label52' href="javascript:ContentClick('label53', 'label52');" onmouseover="ContentPreview('label53');" onmouseout="ContentUnpreview('label53');" title="click to collapse or expand..."> more... </a>
 <div id="label53" style="display:none">
 <table border="1">
 <tr>
 <td></td>
 <td><code class="docutils literal notranslate">v7.0.0 </code></td>
 </tr>
 <tr>
 <td>ssl_cipher_suites</td>
 <td>yes</td>
 </tr>
 </table>
 </div>
 </li>
                <ul class="ul-self">
                <li> <span class="li-head">cipher</span> - Cipher suite name. <span class="li-normal">type: str</span> <span class="li-normal">choices: TLS-AES-128-GCM-SHA256, TLS-AES-256-GCM-SHA384, TLS-CHACHA20-POLY1305-SHA256, TLS-ECDHE-RSA-WITH-CHACHA20-POLY1305-SHA256, TLS-ECDHE-ECDSA-WITH-CHACHA20-POLY1305-SHA256, TLS-DHE-RSA-WITH-CHACHA20-POLY1305-SHA256, TLS-DHE-RSA-WITH-AES-128-CBC-SHA, TLS-DHE-RSA-WITH-AES-256-CBC-SHA, TLS-DHE-RSA-WITH-AES-128-CBC-SHA256, TLS-DHE-RSA-WITH-AES-128-GCM-SHA256, TLS-DHE-RSA-WITH-AES-256-CBC-SHA256, TLS-DHE-RSA-WITH-AES-256-GCM-SHA384, TLS-DHE-DSS-WITH-AES-128-CBC-SHA, TLS-DHE-DSS-WITH-AES-256-CBC-SHA, TLS-DHE-DSS-WITH-AES-128-CBC-SHA256, TLS-DHE-DSS-WITH-AES-128-GCM-SHA256, TLS-DHE-DSS-WITH-AES-256-CBC-SHA256, TLS-DHE-DSS-WITH-AES-256-GCM-SHA384, TLS-ECDHE-RSA-WITH-AES-128-CBC-SHA, TLS-ECDHE-RSA-WITH-AES-128-CBC-SHA256, TLS-ECDHE-RSA-WITH-AES-128-GCM-SHA256, TLS-ECDHE-RSA-WITH-AES-256-CBC-SHA, TLS-ECDHE-RSA-WITH-AES-256-CBC-SHA384, TLS-ECDHE-RSA-WITH-AES-256-GCM-SHA384, TLS-ECDHE-ECDSA-WITH-AES-128-CBC-SHA, TLS-ECDHE-ECDSA-WITH-AES-128-CBC-SHA256, TLS-ECDHE-ECDSA-WITH-AES-128-GCM-SHA256, TLS-ECDHE-ECDSA-WITH-AES-256-CBC-SHA384, TLS-ECDHE-ECDSA-WITH-AES-256-GCM-SHA384, TLS-RSA-WITH-AES-128-CBC-SHA, TLS-RSA-WITH-AES-256-CBC-SHA, TLS-RSA-WITH-AES-128-CBC-SHA256, TLS-RSA-WITH-AES-128-GCM-SHA256, TLS-RSA-WITH-AES-256-CBC-SHA256, TLS-RSA-WITH-AES-256-GCM-SHA384, TLS-RSA-WITH-CAMELLIA-128-CBC-SHA, TLS-RSA-WITH-CAMELLIA-256-CBC-SHA, TLS-RSA-WITH-CAMELLIA-128-CBC-SHA256, TLS-RSA-WITH-CAMELLIA-256-CBC-SHA256, TLS-DHE-RSA-WITH-3DES-EDE-CBC-SHA, TLS-DHE-RSA-WITH-CAMELLIA-128-CBC-SHA, TLS-DHE-DSS-WITH-CAMELLIA-128-CBC-SHA, TLS-DHE-RSA-WITH-CAMELLIA-256-CBC-SHA, TLS-DHE-DSS-WITH-CAMELLIA-256-CBC-SHA, TLS-DHE-RSA-WITH-CAMELLIA-128-CBC-SHA256, TLS-DHE-DSS-WITH-CAMELLIA-128-CBC-SHA256, TLS-DHE-RSA-WITH-CAMELLIA-256-CBC-SHA256, TLS-DHE-DSS-WITH-CAMELLIA-256-CBC-SHA256, TLS-DHE-RSA-WITH-SEED-CBC-SHA, TLS-DHE-DSS-WITH-SEED-CBC-SHA, TLS-DHE-RSA-WITH-ARIA-128-CBC-SHA256, TLS-DHE-RSA-WITH-ARIA-256-CBC-SHA384, TLS-DHE-DSS-WITH-ARIA-128-CBC-SHA256, TLS-DHE-DSS-WITH-ARIA-256-CBC-SHA384, TLS-RSA-WITH-SEED-CBC-SHA, TLS-RSA-WITH-ARIA-128-CBC-SHA256, TLS-RSA-WITH-ARIA-256-CBC-SHA384, TLS-ECDHE-RSA-WITH-ARIA-128-CBC-SHA256, TLS-ECDHE-RSA-WITH-ARIA-256-CBC-SHA384, TLS-ECDHE-ECDSA-WITH-ARIA-128-CBC-SHA256, TLS-ECDHE-ECDSA-WITH-ARIA-256-CBC-SHA384, TLS-ECDHE-RSA-WITH-RC4-128-SHA, TLS-ECDHE-RSA-WITH-3DES-EDE-CBC-SHA, TLS-DHE-DSS-WITH-3DES-EDE-CBC-SHA, TLS-RSA-WITH-3DES-EDE-CBC-SHA, TLS-RSA-WITH-RC4-128-MD5, TLS-RSA-WITH-RC4-128-SHA, TLS-DHE-RSA-WITH-DES-CBC-SHA, TLS-DHE-DSS-WITH-DES-CBC-SHA, TLS-RSA-WITH-DES-CBC-SHA</span>
 <a id='label54' href="javascript:ContentClick('label55', 'label54');" onmouseover="ContentPreview('label55');" onmouseout="ContentUnpreview('label55');" title="click to collapse or expand..."> more... </a>
 <div id="label55" style="display:none">
 <table border="1">
 <tr>
 <td></td>
 <td><code class="docutils literal notranslate">v7.0.0 </code></td>
 </tr>
 <tr>
 <td>cipher</td>
 <td>yes</td>
 </tr>
 <tr>
 <td>[TLS-AES-128-GCM-SHA256]</td>
 <td>yes</td>
 </tr>
 <tr>
 <td>[TLS-AES-256-GCM-SHA384]</td>
 <td>yes</td>
 </tr>
 <tr>
 <td>[TLS-CHACHA20-POLY1305-SHA256]</td>
 <td>yes</td>
 </tr>
 <tr>
 <td>[TLS-ECDHE-RSA-WITH-CHACHA20-POLY1305-SHA256]</td>
 <td>yes</td>
 </tr>
 <tr>
 <td>[TLS-ECDHE-ECDSA-WITH-CHACHA20-POLY1305-SHA256]</td>
 <td>yes</td>
 </tr>
 <tr>
 <td>[TLS-DHE-RSA-WITH-CHACHA20-POLY1305-SHA256]</td>
 <td>yes</td>
 </tr>
 <tr>
 <td>[TLS-DHE-RSA-WITH-AES-128-CBC-SHA]</td>
 <td>yes</td>
 </tr>
 <tr>
 <td>[TLS-DHE-RSA-WITH-AES-256-CBC-SHA]</td>
 <td>yes</td>
 </tr>
 <tr>
 <td>[TLS-DHE-RSA-WITH-AES-128-CBC-SHA256]</td>
 <td>yes</td>
 </tr>
 <tr>
 <td>[TLS-DHE-RSA-WITH-AES-128-GCM-SHA256]</td>
 <td>yes</td>
 </tr>
 <tr>
 <td>[TLS-DHE-RSA-WITH-AES-256-CBC-SHA256]</td>
 <td>yes</td>
 </tr>
 <tr>
 <td>[TLS-DHE-RSA-WITH-AES-256-GCM-SHA384]</td>
 <td>yes</td>
 </tr>
 <tr>
 <td>[TLS-DHE-DSS-WITH-AES-128-CBC-SHA]</td>
 <td>yes</td>
 </tr>
 <tr>
 <td>[TLS-DHE-DSS-WITH-AES-256-CBC-SHA]</td>
 <td>yes</td>
 </tr>
 <tr>
 <td>[TLS-DHE-DSS-WITH-AES-128-CBC-SHA256]</td>
 <td>yes</td>
 </tr>
 <tr>
 <td>[TLS-DHE-DSS-WITH-AES-128-GCM-SHA256]</td>
 <td>yes</td>
 </tr>
 <tr>
 <td>[TLS-DHE-DSS-WITH-AES-256-CBC-SHA256]</td>
 <td>yes</td>
 </tr>
 <tr>
 <td>[TLS-DHE-DSS-WITH-AES-256-GCM-SHA384]</td>
 <td>yes</td>
 </tr>
 <tr>
 <td>[TLS-ECDHE-RSA-WITH-AES-128-CBC-SHA]</td>
 <td>yes</td>
 </tr>
 <tr>
 <td>[TLS-ECDHE-RSA-WITH-AES-128-CBC-SHA256]</td>
 <td>yes</td>
 </tr>
 <tr>
 <td>[TLS-ECDHE-RSA-WITH-AES-128-GCM-SHA256]</td>
 <td>yes</td>
 </tr>
 <tr>
 <td>[TLS-ECDHE-RSA-WITH-AES-256-CBC-SHA]</td>
 <td>yes</td>
 </tr>
 <tr>
 <td>[TLS-ECDHE-RSA-WITH-AES-256-CBC-SHA384]</td>
 <td>yes</td>
 </tr>
 <tr>
 <td>[TLS-ECDHE-RSA-WITH-AES-256-GCM-SHA384]</td>
 <td>yes</td>
 </tr>
 <tr>
 <td>[TLS-ECDHE-ECDSA-WITH-AES-128-CBC-SHA]</td>
 <td>yes</td>
 </tr>
 <tr>
 <td>[TLS-ECDHE-ECDSA-WITH-AES-128-CBC-SHA256]</td>
 <td>yes</td>
 </tr>
 <tr>
 <td>[TLS-ECDHE-ECDSA-WITH-AES-128-GCM-SHA256]</td>
 <td>yes</td>
 </tr>
 <tr>
 <td>[TLS-ECDHE-ECDSA-WITH-AES-256-CBC-SHA384]</td>
 <td>yes</td>
 </tr>
 <tr>
 <td>[TLS-ECDHE-ECDSA-WITH-AES-256-GCM-SHA384]</td>
 <td>yes</td>
 </tr>
 <tr>
 <td>[TLS-RSA-WITH-AES-128-CBC-SHA]</td>
 <td>yes</td>
 </tr>
 <tr>
 <td>[TLS-RSA-WITH-AES-256-CBC-SHA]</td>
 <td>yes</td>
 </tr>
 <tr>
 <td>[TLS-RSA-WITH-AES-128-CBC-SHA256]</td>
 <td>yes</td>
 </tr>
 <tr>
 <td>[TLS-RSA-WITH-AES-128-GCM-SHA256]</td>
 <td>yes</td>
 </tr>
 <tr>
 <td>[TLS-RSA-WITH-AES-256-CBC-SHA256]</td>
 <td>yes</td>
 </tr>
 <tr>
 <td>[TLS-RSA-WITH-AES-256-GCM-SHA384]</td>
 <td>yes</td>
 </tr>
 <tr>
 <td>[TLS-RSA-WITH-CAMELLIA-128-CBC-SHA]</td>
 <td>yes</td>
 </tr>
 <tr>
 <td>[TLS-RSA-WITH-CAMELLIA-256-CBC-SHA]</td>
 <td>yes</td>
 </tr>
 <tr>
 <td>[TLS-RSA-WITH-CAMELLIA-128-CBC-SHA256]</td>
 <td>yes</td>
 </tr>
 <tr>
 <td>[TLS-RSA-WITH-CAMELLIA-256-CBC-SHA256]</td>
 <td>yes</td>
 </tr>
 <tr>
 <td>[TLS-DHE-RSA-WITH-3DES-EDE-CBC-SHA]</td>
 <td>yes</td>
 </tr>
 <tr>
 <td>[TLS-DHE-RSA-WITH-CAMELLIA-128-CBC-SHA]</td>
 <td>yes</td>
 </tr>
 <tr>
 <td>[TLS-DHE-DSS-WITH-CAMELLIA-128-CBC-SHA]</td>
 <td>yes</td>
 </tr>
 <tr>
 <td>[TLS-DHE-RSA-WITH-CAMELLIA-256-CBC-SHA]</td>
 <td>yes</td>
 </tr>
 <tr>
 <td>[TLS-DHE-DSS-WITH-CAMELLIA-256-CBC-SHA]</td>
 <td>yes</td>
 </tr>
 <tr>
 <td>[TLS-DHE-RSA-WITH-CAMELLIA-128-CBC-SHA256]</td>
 <td>yes</td>
 </tr>
 <tr>
 <td>[TLS-DHE-DSS-WITH-CAMELLIA-128-CBC-SHA256]</td>
 <td>yes</td>
 </tr>
 <tr>
 <td>[TLS-DHE-RSA-WITH-CAMELLIA-256-CBC-SHA256]</td>
 <td>yes</td>
 </tr>
 <tr>
 <td>[TLS-DHE-DSS-WITH-CAMELLIA-256-CBC-SHA256]</td>
 <td>yes</td>
 </tr>
 <tr>
 <td>[TLS-DHE-RSA-WITH-SEED-CBC-SHA]</td>
 <td>yes</td>
 </tr>
 <tr>
 <td>[TLS-DHE-DSS-WITH-SEED-CBC-SHA]</td>
 <td>yes</td>
 </tr>
 <tr>
 <td>[TLS-DHE-RSA-WITH-ARIA-128-CBC-SHA256]</td>
 <td>yes</td>
 </tr>
 <tr>
 <td>[TLS-DHE-RSA-WITH-ARIA-256-CBC-SHA384]</td>
 <td>yes</td>
 </tr>
 <tr>
 <td>[TLS-DHE-DSS-WITH-ARIA-128-CBC-SHA256]</td>
 <td>yes</td>
 </tr>
 <tr>
 <td>[TLS-DHE-DSS-WITH-ARIA-256-CBC-SHA384]</td>
 <td>yes</td>
 </tr>
 <tr>
 <td>[TLS-RSA-WITH-SEED-CBC-SHA]</td>
 <td>yes</td>
 </tr>
 <tr>
 <td>[TLS-RSA-WITH-ARIA-128-CBC-SHA256]</td>
 <td>yes</td>
 </tr>
 <tr>
 <td>[TLS-RSA-WITH-ARIA-256-CBC-SHA384]</td>
 <td>yes</td>
 </tr>
 <tr>
 <td>[TLS-ECDHE-RSA-WITH-ARIA-128-CBC-SHA256]</td>
 <td>yes</td>
 </tr>
 <tr>
 <td>[TLS-ECDHE-RSA-WITH-ARIA-256-CBC-SHA384]</td>
 <td>yes</td>
 </tr>
 <tr>
 <td>[TLS-ECDHE-ECDSA-WITH-ARIA-128-CBC-SHA256]</td>
 <td>yes</td>
 </tr>
 <tr>
 <td>[TLS-ECDHE-ECDSA-WITH-ARIA-256-CBC-SHA384]</td>
 <td>yes</td>
 </tr>
 <tr>
 <td>[TLS-ECDHE-RSA-WITH-RC4-128-SHA]</td>
 <td>yes</td>
 </tr>
 <tr>
 <td>[TLS-ECDHE-RSA-WITH-3DES-EDE-CBC-SHA]</td>
 <td>yes</td>
 </tr>
 <tr>
 <td>[TLS-DHE-DSS-WITH-3DES-EDE-CBC-SHA]</td>
 <td>yes</td>
 </tr>
 <tr>
 <td>[TLS-RSA-WITH-3DES-EDE-CBC-SHA]</td>
 <td>yes</td>
 </tr>
 <tr>
 <td>[TLS-RSA-WITH-RC4-128-MD5]</td>
 <td>yes</td>
 </tr>
 <tr>
 <td>[TLS-RSA-WITH-RC4-128-SHA]</td>
 <td>yes</td>
 </tr>
 <tr>
 <td>[TLS-DHE-RSA-WITH-DES-CBC-SHA]</td>
 <td>yes</td>
 </tr>
 <tr>
 <td>[TLS-DHE-DSS-WITH-DES-CBC-SHA]</td>
 <td>yes</td>
 </tr>
 <tr>
 <td>[TLS-RSA-WITH-DES-CBC-SHA]</td>
 <td>yes</td>
 </tr>
 </table>
 </div>
 </li>
                <li> <span class="li-head">priority</span> - SSL/TLS cipher suites priority. <span class="li-normal">type: int</span> <span class="li-required">required: True</span>
 <a id='label56' href="javascript:ContentClick('label57', 'label56');" onmouseover="ContentPreview('label57');" onmouseout="ContentUnpreview('label57');" title="click to collapse or expand..."> more... </a>
 <div id="label57" style="display:none">
 <table border="1">
 <tr>
 <td></td>
 <td><code class="docutils literal notranslate">v7.0.0 </code></td>
 </tr>
 <tr>
 <td>priority</td>
 <td>yes</td>
 </tr>
 </table>
 </div>
 </li>
                <li> <span class="li-head">versions</span> - SSL/TLS versions that the cipher suite can be used with. <span class="li-normal">type: str</span> <span class="li-normal">choices: tls-1.0, tls-1.1, tls-1.2, tls-1.3</span>
 <a id='label58' href="javascript:ContentClick('label59', 'label58');" onmouseover="ContentPreview('label59');" onmouseout="ContentUnpreview('label59');" title="click to collapse or expand..."> more... </a>
 <div id="label59" style="display:none">
 <table border="1">
 <tr>
 <td></td>
 <td><code class="docutils literal notranslate">v7.0.0 </code></td>
 </tr>
 <tr>
 <td>versions</td>
 <td>yes</td>
 </tr>
 <tr>
 <td>[tls-1.0]</td>
 <td>yes</td>
 </tr>
 <tr>
 <td>[tls-1.1]</td>
 <td>yes</td>
 </tr>
 <tr>
 <td>[tls-1.2]</td>
 <td>yes</td>
 </tr>
 <tr>
 <td>[tls-1.3]</td>
 <td>yes</td>
 </tr>
 </table>
 </div>
 </li>
                </ul>
            <li> <span class="li-head">ssl_dh_bits</span> - Number of bits to use in the Diffie-Hellman exchange for RSA encryption of SSL sessions. <span class="li-normal">type: str</span> <span class="li-normal">choices: 768, 1024, 1536, 2048, 3072, 4096</span>
 <a id='label60' href="javascript:ContentClick('label61', 'label60');" onmouseover="ContentPreview('label61');" onmouseout="ContentUnpreview('label61');" title="click to collapse or expand..."> more... </a>
 <div id="label61" style="display:none">
 <table border="1">
 <tr>
 <td></td>
 <td><code class="docutils literal notranslate">v7.0.0 </code></td>
 </tr>
 <tr>
 <td>ssl_dh_bits</td>
 <td>yes</td>
 </tr>
 <tr>
 <td>[768]</td>
 <td>yes</td>
 </tr>
 <tr>
 <td>[1024]</td>
 <td>yes</td>
 </tr>
 <tr>
 <td>[1536]</td>
 <td>yes</td>
 </tr>
 <tr>
 <td>[2048]</td>
 <td>yes</td>
 </tr>
 <tr>
 <td>[3072]</td>
 <td>yes</td>
 </tr>
 <tr>
 <td>[4096]</td>
 <td>yes</td>
 </tr>
 </table>
 </div>
 </li>
            <li> <span class="li-head">ssl_max_version</span> - Highest SSL/TLS version acceptable from a server. <span class="li-normal">type: str</span> <span class="li-normal">choices: tls-1.0, tls-1.1, tls-1.2, tls-1.3</span>
 <a id='label62' href="javascript:ContentClick('label63', 'label62');" onmouseover="ContentPreview('label63');" onmouseout="ContentUnpreview('label63');" title="click to collapse or expand..."> more... </a>
 <div id="label63" style="display:none">
 <table border="1">
 <tr>
 <td></td>
 <td><code class="docutils literal notranslate">v7.0.0 </code></td>
 </tr>
 <tr>
 <td>ssl_max_version</td>
 <td>yes</td>
 </tr>
 <tr>
 <td>[tls-1.0]</td>
 <td>yes</td>
 </tr>
 <tr>
 <td>[tls-1.1]</td>
 <td>yes</td>
 </tr>
 <tr>
 <td>[tls-1.2]</td>
 <td>yes</td>
 </tr>
 <tr>
 <td>[tls-1.3]</td>
 <td>yes</td>
 </tr>
 </table>
 </div>
 </li>
            <li> <span class="li-head">ssl_min_version</span> - Lowest SSL/TLS version acceptable from a server. <span class="li-normal">type: str</span> <span class="li-normal">choices: tls-1.0, tls-1.1, tls-1.2, tls-1.3</span>
 <a id='label64' href="javascript:ContentClick('label65', 'label64');" onmouseover="ContentPreview('label65');" onmouseout="ContentUnpreview('label65');" title="click to collapse or expand..."> more... </a>
 <div id="label65" style="display:none">
 <table border="1">
 <tr>
 <td></td>
 <td><code class="docutils literal notranslate">v7.0.0 </code></td>
 </tr>
 <tr>
 <td>ssl_min_version</td>
 <td>yes</td>
 </tr>
 <tr>
 <td>[tls-1.0]</td>
 <td>yes</td>
 </tr>
 <tr>
 <td>[tls-1.1]</td>
 <td>yes</td>
 </tr>
 <tr>
 <td>[tls-1.2]</td>
 <td>yes</td>
 </tr>
 <tr>
 <td>[tls-1.3]</td>
 <td>yes</td>
 </tr>
 </table>
 </div>
 </li>
            <li> <span class="li-head">url_map</span> - URL pattern to match. <span class="li-normal">type: str</span>
 <a id='label66' href="javascript:ContentClick('label67', 'label66');" onmouseover="ContentPreview('label67');" onmouseout="ContentUnpreview('label67');" title="click to collapse or expand..."> more... </a>
 <div id="label67" style="display:none">
 <table border="1">
 <tr>
 <td></td>
 <td><code class="docutils literal notranslate">v7.0.0 </code></td>
 </tr>
 <tr>
 <td>url_map</td>
 <td>yes</td>
 </tr>
 </table>
 </div>
 </li>
            <li> <span class="li-head">url_map_type</span> - Type of url-map. <span class="li-normal">type: str</span> <span class="li-normal">choices: sub-string, wildcard, regex</span>
 <a id='label68' href="javascript:ContentClick('label69', 'label68');" onmouseover="ContentPreview('label69');" onmouseout="ContentUnpreview('label69');" title="click to collapse or expand..."> more... </a>
 <div id="label69" style="display:none">
 <table border="1">
 <tr>
 <td></td>
 <td><code class="docutils literal notranslate">v7.0.0 </code></td>
 </tr>
 <tr>
 <td>url_map_type</td>
 <td>yes</td>
 </tr>
 <tr>
 <td>[sub-string]</td>
 <td>yes</td>
 </tr>
 <tr>
 <td>[wildcard]</td>
 <td>yes</td>
 </tr>
 <tr>
 <td>[regex]</td>
 <td>yes</td>
 </tr>
 </table>
 </div>
 </li>
            <li> <span class="li-head">virtual_host</span> - Virtual host. Source firewall.access-proxy-virtual-host.name. <span class="li-normal">type: str</span>
 <a id='label70' href="javascript:ContentClick('label71', 'label70');" onmouseover="ContentPreview('label71');" onmouseout="ContentUnpreview('label71');" title="click to collapse or expand..."> more... </a>
 <div id="label71" style="display:none">
 <table border="1">
 <tr>
 <td></td>
 <td><code class="docutils literal notranslate">v7.0.0 </code></td>
 </tr>
 <tr>
 <td>virtual_host</td>
 <td>yes</td>
 </tr>
 </table>
 </div>
 </li>
            </ul>
        <li> <span class="li-head">client_cert</span> - Enable/disable to request client certificate. <span class="li-normal">type: str</span> <span class="li-normal">choices: disable, enable</span>
 <a id='label72' href="javascript:ContentClick('label73', 'label72');" onmouseover="ContentPreview('label73');" onmouseout="ContentUnpreview('label73');" title="click to collapse or expand..."> more... </a>
 <div id="label73" style="display:none">
 <table border="1">
 <tr>
 <td></td>
 <td><code class="docutils literal notranslate">v7.0.0 </code></td>
 </tr>
 <tr>
 <td>client_cert</td>
 <td>yes</td>
 </tr>
 <tr>
 <td>[disable]</td>
 <td>yes</td>
 </tr>
 <tr>
 <td>[enable]</td>
 <td>yes</td>
 </tr>
 </table>
 </div>
 </li>
        <li> <span class="li-head">empty_cert_action</span> - Action of an empty client certificate. <span class="li-normal">type: str</span> <span class="li-normal">choices: accept, block</span>
 <a id='label74' href="javascript:ContentClick('label75', 'label74');" onmouseover="ContentPreview('label75');" onmouseout="ContentUnpreview('label75');" title="click to collapse or expand..."> more... </a>
 <div id="label75" style="display:none">
 <table border="1">
 <tr>
 <td></td>
 <td><code class="docutils literal notranslate">v7.0.0 </code></td>
 </tr>
 <tr>
 <td>empty_cert_action</td>
 <td>yes</td>
 </tr>
 <tr>
 <td>[accept]</td>
 <td>yes</td>
 </tr>
 <tr>
 <td>[block]</td>
 <td>yes</td>
 </tr>
 </table>
 </div>
 </li>
        <li> <span class="li-head">ldb_method</span> - Method used to distribute sessions to SSL real servers. <span class="li-normal">type: str</span> <span class="li-normal">choices: static, round-robin, weighted, least-session, least-rtt, first-alive</span>
 <a id='label76' href="javascript:ContentClick('label77', 'label76');" onmouseover="ContentPreview('label77');" onmouseout="ContentUnpreview('label77');" title="click to collapse or expand..."> more... </a>
 <div id="label77" style="display:none">
 <table border="1">
 <tr>
 <td></td>
 <td><code class="docutils literal notranslate">v7.0.0 </code></td>
 </tr>
 <tr>
 <td>ldb_method</td>
 <td>yes</td>
 </tr>
 <tr>
 <td>[static]</td>
 <td>yes</td>
 </tr>
 <tr>
 <td>[round-robin]</td>
 <td>yes</td>
 </tr>
 <tr>
 <td>[weighted]</td>
 <td>yes</td>
 </tr>
 <tr>
 <td>[least-session]</td>
 <td>yes</td>
 </tr>
 <tr>
 <td>[least-rtt]</td>
 <td>yes</td>
 </tr>
 <tr>
 <td>[first-alive]</td>
 <td>yes</td>
 </tr>
 </table>
 </div>
 </li>
        <li> <span class="li-head">name</span> - Access Proxy name. <span class="li-normal">type: str</span> <span class="li-required">required: True</span>
 <a id='label78' href="javascript:ContentClick('label79', 'label78');" onmouseover="ContentPreview('label79');" onmouseout="ContentUnpreview('label79');" title="click to collapse or expand..."> more... </a>
 <div id="label79" style="display:none">
 <table border="1">
 <tr>
 <td></td>
 <td><code class="docutils literal notranslate">v7.0.0 </code></td>
 </tr>
 <tr>
 <td>name</td>
 <td>yes</td>
 </tr>
 </table>
 </div>
 </li>
        <li> <span class="li-head">realservers</span> - Select the SSL real servers that this Access Proxy will distribute traffic to. <span class="li-normal">type: list</span>
 <a id='label80' href="javascript:ContentClick('label81', 'label80');" onmouseover="ContentPreview('label81');" onmouseout="ContentUnpreview('label81');" title="click to collapse or expand..."> more... </a>
 <div id="label81" style="display:none">
 <table border="1">
 <tr>
 <td></td>
 <td><code class="docutils literal notranslate">v7.0.0 </code></td>
 </tr>
 <tr>
 <td>realservers</td>
 <td>yes</td>
 </tr>
 </table>
 </div>
 </li>
            <ul class="ul-self">
            <li> <span class="li-head">id</span> - Real server ID. <span class="li-normal">type: int</span> <span class="li-required">required: True</span>
 <a id='label82' href="javascript:ContentClick('label83', 'label82');" onmouseover="ContentPreview('label83');" onmouseout="ContentUnpreview('label83');" title="click to collapse or expand..."> more... </a>
 <div id="label83" style="display:none">
 <table border="1">
 <tr>
 <td></td>
 <td><code class="docutils literal notranslate">v7.0.0 </code></td>
 </tr>
 <tr>
 <td>id</td>
 <td>yes</td>
 </tr>
 </table>
 </div>
 </li>
            <li> <span class="li-head">ip</span> - IP address of the real server. <span class="li-normal">type: str</span>
 <a id='label84' href="javascript:ContentClick('label85', 'label84');" onmouseover="ContentPreview('label85');" onmouseout="ContentUnpreview('label85');" title="click to collapse or expand..."> more... </a>
 <div id="label85" style="display:none">
 <table border="1">
 <tr>
 <td></td>
 <td><code class="docutils literal notranslate">v7.0.0 </code></td>
 </tr>
 <tr>
 <td>ip</td>
 <td>yes</td>
 </tr>
 </table>
 </div>
 </li>
            <li> <span class="li-head">port</span> - Port for communicating with the real server. <span class="li-normal">type: int</span>
 <a id='label86' href="javascript:ContentClick('label87', 'label86');" onmouseover="ContentPreview('label87');" onmouseout="ContentUnpreview('label87');" title="click to collapse or expand..."> more... </a>
 <div id="label87" style="display:none">
 <table border="1">
 <tr>
 <td></td>
 <td><code class="docutils literal notranslate">v7.0.0 </code></td>
 </tr>
 <tr>
 <td>port</td>
 <td>yes</td>
 </tr>
 </table>
 </div>
 </li>
            <li> <span class="li-head">status</span> - Set the status of the real server to active so that it can accept traffic, or on standby or disabled so no traffic is sent. <span class="li-normal">type: str</span> <span class="li-normal">choices: active, standby, disable</span>
 <a id='label88' href="javascript:ContentClick('label89', 'label88');" onmouseover="ContentPreview('label89');" onmouseout="ContentUnpreview('label89');" title="click to collapse or expand..."> more... </a>
 <div id="label89" style="display:none">
 <table border="1">
 <tr>
 <td></td>
 <td><code class="docutils literal notranslate">v7.0.0 </code></td>
 </tr>
 <tr>
 <td>status</td>
 <td>yes</td>
 </tr>
 <tr>
 <td>[active]</td>
 <td>yes</td>
 </tr>
 <tr>
 <td>[standby]</td>
 <td>yes</td>
 </tr>
 <tr>
 <td>[disable]</td>
 <td>yes</td>
 </tr>
 </table>
 </div>
 </li>
            <li> <span class="li-head">weight</span> - Weight of the real server. If weighted load balancing is enabled, the server with the highest weight gets more connections. <span class="li-normal">type: int</span>
 <a id='label90' href="javascript:ContentClick('label91', 'label90');" onmouseover="ContentPreview('label91');" onmouseout="ContentUnpreview('label91');" title="click to collapse or expand..."> more... </a>
 <div id="label91" style="display:none">
 <table border="1">
 <tr>
 <td></td>
 <td><code class="docutils literal notranslate">v7.0.0 </code></td>
 </tr>
 <tr>
 <td>weight</td>
 <td>yes</td>
 </tr>
 </table>
 </div>
 </li>
            </ul>
        <li> <span class="li-head">server_pubkey_auth</span> - Enable/disable SSH real server public key authentication. <span class="li-normal">type: str</span> <span class="li-normal">choices: disable, enable</span>
 <a id='label92' href="javascript:ContentClick('label93', 'label92');" onmouseover="ContentPreview('label93');" onmouseout="ContentUnpreview('label93');" title="click to collapse or expand..."> more... </a>
 <div id="label93" style="display:none">
 <table border="1">
 <tr>
 <td></td>
 <td><code class="docutils literal notranslate">v7.0.0 </code></td>
 </tr>
 <tr>
 <td>server_pubkey_auth</td>
 <td>yes</td>
 </tr>
 <tr>
 <td>[disable]</td>
 <td>yes</td>
 </tr>
 <tr>
 <td>[enable]</td>
 <td>yes</td>
 </tr>
 </table>
 </div>
 </li>
        <li> <span class="li-head">server_pubkey_auth_settings</span> - Server SSH public key authentication settings. <span class="li-normal">type: dict</span>
 <a id='label94' href="javascript:ContentClick('label95', 'label94');" onmouseover="ContentPreview('label95');" onmouseout="ContentUnpreview('label95');" title="click to collapse or expand..."> more... </a>
 <div id="label95" style="display:none">
 <table border="1">
 <tr>
 <td></td>
 <td><code class="docutils literal notranslate">v7.0.0 </code></td>
 </tr>
 <tr>
 <td>server_pubkey_auth_settings</td>
 <td>yes</td>
 </tr>
 </table>
 </div>
 </li>
            <ul class="ul-self">
            <li> <span class="li-head">auth_ca</span> - Name of the SSH server public key authentication CA. Source firewall.ssh.local-ca.name. <span class="li-normal">type: str</span>
 <a id='label96' href="javascript:ContentClick('label97', 'label96');" onmouseover="ContentPreview('label97');" onmouseout="ContentUnpreview('label97');" title="click to collapse or expand..."> more... </a>
 <div id="label97" style="display:none">
 <table border="1">
 <tr>
 <td></td>
 <td><code class="docutils literal notranslate">v7.0.0 </code></td>
 </tr>
 <tr>
 <td>auth_ca</td>
 <td>yes</td>
 </tr>
 </table>
 </div>
 </li>
            <li> <span class="li-head">cert_extension</span> - Configure certificate extension for user certificate. <span class="li-normal">type: list</span>
 <a id='label98' href="javascript:ContentClick('label99', 'label98');" onmouseover="ContentPreview('label99');" onmouseout="ContentUnpreview('label99');" title="click to collapse or expand..."> more... </a>
 <div id="label99" style="display:none">
 <table border="1">
 <tr>
 <td></td>
 <td><code class="docutils literal notranslate">v7.0.0 </code></td>
 </tr>
 <tr>
 <td>cert_extension</td>
 <td>yes</td>
 </tr>
 </table>
 </div>
 </li>
                <ul class="ul-self">
                <li> <span class="li-head">critical</span> - Critical option. <span class="li-normal">type: str</span> <span class="li-normal">choices: False, True</span>
 <a id='label100' href="javascript:ContentClick('label101', 'label100');" onmouseover="ContentPreview('label101');" onmouseout="ContentUnpreview('label101');" title="click to collapse or expand..."> more... </a>
 <div id="label101" style="display:none">
 <table border="1">
 <tr>
 <td></td>
 <td><code class="docutils literal notranslate">v7.0.0 </code></td>
 </tr>
 <tr>
 <td>critical</td>
 <td>yes</td>
 </tr>
 <tr>
 <td>[no]</td>
 <td>yes</td>
 </tr>
 <tr>
 <td>[yes]</td>
 <td>yes</td>
 </tr>
 </table>
 </div>
 </li>
                <li> <span class="li-head">data</span> - Name of certificate extension. <span class="li-normal">type: str</span>
 <a id='label102' href="javascript:ContentClick('label103', 'label102');" onmouseover="ContentPreview('label103');" onmouseout="ContentUnpreview('label103');" title="click to collapse or expand..."> more... </a>
 <div id="label103" style="display:none">
 <table border="1">
 <tr>
 <td></td>
 <td><code class="docutils literal notranslate">v7.0.0 </code></td>
 </tr>
 <tr>
 <td>data</td>
 <td>yes</td>
 </tr>
 </table>
 </div>
 </li>
                <li> <span class="li-head">name</span> - Name of certificate extension. <span class="li-normal">type: str</span> <span class="li-required">required: True</span>
 <a id='label104' href="javascript:ContentClick('label105', 'label104');" onmouseover="ContentPreview('label105');" onmouseout="ContentUnpreview('label105');" title="click to collapse or expand..."> more... </a>
 <div id="label105" style="display:none">
 <table border="1">
 <tr>
 <td></td>
 <td><code class="docutils literal notranslate">v7.0.0 </code></td>
 </tr>
 <tr>
 <td>name</td>
 <td>yes</td>
 </tr>
 </table>
 </div>
 </li>
                <li> <span class="li-head">type</span> - Type of certificate extension. <span class="li-normal">type: str</span> <span class="li-normal">choices: fixed, user</span>
 <a id='label106' href="javascript:ContentClick('label107', 'label106');" onmouseover="ContentPreview('label107');" onmouseout="ContentUnpreview('label107');" title="click to collapse or expand..."> more... </a>
 <div id="label107" style="display:none">
 <table border="1">
 <tr>
 <td></td>
 <td><code class="docutils literal notranslate">v7.0.0 </code></td>
 </tr>
 <tr>
 <td>type</td>
 <td>yes</td>
 </tr>
 <tr>
 <td>[fixed]</td>
 <td>yes</td>
 </tr>
 <tr>
 <td>[user]</td>
 <td>yes</td>
 </tr>
 </table>
 </div>
 </li>
                </ul>
            <li> <span class="li-head">permit_agent_forwarding</span> - Enable/disable appending permit-agent-forwarding certificate extension. <span class="li-normal">type: str</span> <span class="li-normal">choices: enable, disable</span>
 <a id='label108' href="javascript:ContentClick('label109', 'label108');" onmouseover="ContentPreview('label109');" onmouseout="ContentUnpreview('label109');" title="click to collapse or expand..."> more... </a>
 <div id="label109" style="display:none">
 <table border="1">
 <tr>
 <td></td>
 <td><code class="docutils literal notranslate">v7.0.0 </code></td>
 </tr>
 <tr>
 <td>permit_agent_forwarding</td>
 <td>yes</td>
 </tr>
 <tr>
 <td>[enable]</td>
 <td>yes</td>
 </tr>
 <tr>
 <td>[disable]</td>
 <td>yes</td>
 </tr>
 </table>
 </div>
 </li>
            <li> <span class="li-head">permit_port_forwarding</span> - Enable/disable appending permit-port-forwarding certificate extension. <span class="li-normal">type: str</span> <span class="li-normal">choices: enable, disable</span>
 <a id='label110' href="javascript:ContentClick('label111', 'label110');" onmouseover="ContentPreview('label111');" onmouseout="ContentUnpreview('label111');" title="click to collapse or expand..."> more... </a>
 <div id="label111" style="display:none">
 <table border="1">
 <tr>
 <td></td>
 <td><code class="docutils literal notranslate">v7.0.0 </code></td>
 </tr>
 <tr>
 <td>permit_port_forwarding</td>
 <td>yes</td>
 </tr>
 <tr>
 <td>[enable]</td>
 <td>yes</td>
 </tr>
 <tr>
 <td>[disable]</td>
 <td>yes</td>
 </tr>
 </table>
 </div>
 </li>
            <li> <span class="li-head">permit_pty</span> - Enable/disable appending permit-pty certificate extension. <span class="li-normal">type: str</span> <span class="li-normal">choices: enable, disable</span>
 <a id='label112' href="javascript:ContentClick('label113', 'label112');" onmouseover="ContentPreview('label113');" onmouseout="ContentUnpreview('label113');" title="click to collapse or expand..."> more... </a>
 <div id="label113" style="display:none">
 <table border="1">
 <tr>
 <td></td>
 <td><code class="docutils literal notranslate">v7.0.0 </code></td>
 </tr>
 <tr>
 <td>permit_pty</td>
 <td>yes</td>
 </tr>
 <tr>
 <td>[enable]</td>
 <td>yes</td>
 </tr>
 <tr>
 <td>[disable]</td>
 <td>yes</td>
 </tr>
 </table>
 </div>
 </li>
            <li> <span class="li-head">permit_user_rc</span> - Enable/disable appending permit-user-rc certificate extension. <span class="li-normal">type: str</span> <span class="li-normal">choices: enable, disable</span>
 <a id='label114' href="javascript:ContentClick('label115', 'label114');" onmouseover="ContentPreview('label115');" onmouseout="ContentUnpreview('label115');" title="click to collapse or expand..."> more... </a>
 <div id="label115" style="display:none">
 <table border="1">
 <tr>
 <td></td>
 <td><code class="docutils literal notranslate">v7.0.0 </code></td>
 </tr>
 <tr>
 <td>permit_user_rc</td>
 <td>yes</td>
 </tr>
 <tr>
 <td>[enable]</td>
 <td>yes</td>
 </tr>
 <tr>
 <td>[disable]</td>
 <td>yes</td>
 </tr>
 </table>
 </div>
 </li>
            <li> <span class="li-head">permit_x11_forwarding</span> - Enable/disable appending permit-x11-forwarding certificate extension. <span class="li-normal">type: str</span> <span class="li-normal">choices: enable, disable</span>
 <a id='label116' href="javascript:ContentClick('label117', 'label116');" onmouseover="ContentPreview('label117');" onmouseout="ContentUnpreview('label117');" title="click to collapse or expand..."> more... </a>
 <div id="label117" style="display:none">
 <table border="1">
 <tr>
 <td></td>
 <td><code class="docutils literal notranslate">v7.0.0 </code></td>
 </tr>
 <tr>
 <td>permit_x11_forwarding</td>
 <td>yes</td>
 </tr>
 <tr>
 <td>[enable]</td>
 <td>yes</td>
 </tr>
 <tr>
 <td>[disable]</td>
 <td>yes</td>
 </tr>
 </table>
 </div>
 </li>
            <li> <span class="li-head">source_address</span> - Enable/disable appending source-address certificate critical option. This option ensure certificate only accepted from FortiGate source address. <span class="li-normal">type: str</span> <span class="li-normal">choices: enable, disable</span>
 <a id='label118' href="javascript:ContentClick('label119', 'label118');" onmouseover="ContentPreview('label119');" onmouseout="ContentUnpreview('label119');" title="click to collapse or expand..."> more... </a>
 <div id="label119" style="display:none">
 <table border="1">
 <tr>
 <td></td>
 <td><code class="docutils literal notranslate">v7.0.0 </code></td>
 </tr>
 <tr>
 <td>source_address</td>
 <td>yes</td>
 </tr>
 <tr>
 <td>[enable]</td>
 <td>yes</td>
 </tr>
 <tr>
 <td>[disable]</td>
 <td>yes</td>
 </tr>
 </table>
 </div>
 </li>
            </ul>
        <li> <span class="li-head">vip</span> - Virtual IP name. Source firewall.vip.name. <span class="li-normal">type: str</span>
 <a id='label120' href="javascript:ContentClick('label121', 'label120');" onmouseover="ContentPreview('label121');" onmouseout="ContentUnpreview('label121');" title="click to collapse or expand..."> more... </a>
 <div id="label121" style="display:none">
 <table border="1">
 <tr>
 <td></td>
 <td><code class="docutils literal notranslate">v7.0.0 </code></td>
 </tr>
 <tr>
 <td>vip</td>
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
      - name: Configure Access Proxy.
        fortios_firewall_access_proxy:
          vdom:  "{{ vdom }}"
          state: "present"
          access_token: "<your_own_value>"
          firewall_access_proxy:
            api_gateway:
             -
                http_cookie_age: "4"
                http_cookie_domain: "<your_own_value>"
                http_cookie_domain_from_host: "disable"
                http_cookie_generation: "7"
                http_cookie_path: "<your_own_value>"
                http_cookie_share: "disable"
                https_cookie_secure: "disable"
                id:  "11"
                ldb_method: "static"
                persistence: "none"
                realservers:
                 -
                    address: "<your_own_value> (source firewall.address.name firewall.addrgrp.name)"
                    health_check: "disable"
                    health_check_proto: "ping"
                    http_host: "myhostname"
                    id:  "19"
                    ip: "<your_own_value>"
                    mappedport: "<your_own_value>"
                    port: "22"
                    status: "active"
                    weight: "24"
                saml_server: "<your_own_value> (source user.saml.name)"
                service: "http"
                ssl_algorithm: "high"
                ssl_cipher_suites:
                 -
                    cipher: "TLS-AES-128-GCM-SHA256"
                    priority: "30"
                    versions: "tls-1.0"
                ssl_dh_bits: "768"
                ssl_max_version: "tls-1.0"
                ssl_min_version: "tls-1.0"
                url_map: "<your_own_value>"
                url_map_type: "sub-string"
                virtual_host: "myhostname (source firewall.access-proxy-virtual-host.name)"
            client_cert: "disable"
            empty_cert_action: "accept"
            ldb_method: "static"
            name: "default_name_41"
            realservers:
             -
                id:  "43"
                ip: "<your_own_value>"
                port: "45"
                status: "active"
                weight: "47"
            server_pubkey_auth: "disable"
            server_pubkey_auth_settings:
                auth_ca: "<your_own_value> (source firewall.ssh.local-ca.name)"
                cert_extension:
                 -
                    critical: "no"
                    data: "<your_own_value>"
                    name: "default_name_54"
                    type: "fixed"
                permit_agent_forwarding: "enable"
                permit_port_forwarding: "enable"
                permit_pty: "enable"
                permit_user_rc: "enable"
                permit_x11_forwarding: "enable"
                source_address: "enable"
            vip: "<your_own_value> (source firewall.vip.name)"
    


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
