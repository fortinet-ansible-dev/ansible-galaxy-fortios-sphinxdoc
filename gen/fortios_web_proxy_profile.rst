:source: fortios_web_proxy_profile.py

:orphan:

.. fortios_web_proxy_profile:

fortios_web_proxy_profile -- Configure web proxy profiles in Fortinet's FortiOS and FortiGate.
++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++

.. versionadded:: 2.0.0

.. contents::
   :local:
   :depth: 1


Synopsis
--------
- This module is able to configure a FortiGate or FortiOS (FOS) device by allowing the user to set and modify web_proxy feature and profile category. Examples include all parameters and values need to be adjusted to datasources before usage. Tested with FOS v6.0.0



Requirements
------------
The below requirements are needed on the host that executes this module.

- ansible>=2.15


Tips
----
Using member operation to add an element to an existing object.

FortiOS Version Compatibility
-----------------------------
Supported Version Ranges: v6.0.0 -> v7.4.4


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
    <li> <span class="li-head">web_proxy_profile</span> - Configure web proxy profiles. <span class="li-normal">type: dict</span>
 <a id='label0' href="javascript:ContentClick('label1', 'label0');" onmouseover="ContentPreview('label1');" onmouseout="ContentUnpreview('label1');" title="click to collapse or expand..."> more... </a>
 <div id="label1" style="display:none">
 <table border="1">
 <tr>
 <td></td><td colspan="1">Supported Version Ranges</td>
 </tr>
 <tr>
 <td>web_proxy_profile</td>
 <td><code class="docutils literal notranslate">v6.0.0 -> 7.4.4 </code></td>
 </tr>
 </table>
 </div>
 </li>
        <ul class="ul-self">
        <li> <span class="li-head">header_client_ip</span> - Action to take on the HTTP client-IP header in forwarded requests: forwards (pass), adds, or removes the HTTP header. <span class="li-normal">type: str</span> <span class="li-normal">choices: pass, add, remove</span>
 <a id='label2' href="javascript:ContentClick('label3', 'label2');" onmouseover="ContentPreview('label3');" onmouseout="ContentUnpreview('label3');" title="click to collapse or expand..."> more... </a>
 <div id="label3" style="display:none">
 <table border="1">
 <tr>
 <td></td>
 <td colspan="1">Supported Version Ranges</td>
 </tr>
 <tr>
 <td>header_client_ip</td>
 <td><code class="docutils literal notranslate">v6.0.0 -> 7.4.4 </code></td>
 </tr>
 <tr>
 <td>[pass]</td>
 <td><code class="docutils literal notranslate">v6.0.0 -> 7.4.4</code></td>
 <tr>
 <td>[add]</td>
 <td><code class="docutils literal notranslate">v6.0.0 -> 7.4.4</code></td>
 <tr>
 <td>[remove]</td>
 <td><code class="docutils literal notranslate">v6.0.0 -> 7.4.4</code></td>
 </table>
 </div>
 </li>
        <li> <span class="li-head">header_front_end_https</span> - Action to take on the HTTP front-end-HTTPS header in forwarded requests: forwards (pass), adds, or removes the HTTP header. <span class="li-normal">type: str</span> <span class="li-normal">choices: pass, add, remove</span>
 <a id='label4' href="javascript:ContentClick('label5', 'label4');" onmouseover="ContentPreview('label5');" onmouseout="ContentUnpreview('label5');" title="click to collapse or expand..."> more... </a>
 <div id="label5" style="display:none">
 <table border="1">
 <tr>
 <td></td>
 <td colspan="1">Supported Version Ranges</td>
 </tr>
 <tr>
 <td>header_front_end_https</td>
 <td><code class="docutils literal notranslate">v6.0.0 -> 7.4.4 </code></td>
 </tr>
 <tr>
 <td>[pass]</td>
 <td><code class="docutils literal notranslate">v6.0.0 -> 7.4.4</code></td>
 <tr>
 <td>[add]</td>
 <td><code class="docutils literal notranslate">v6.0.0 -> 7.4.4</code></td>
 <tr>
 <td>[remove]</td>
 <td><code class="docutils literal notranslate">v6.0.0 -> 7.4.4</code></td>
 </table>
 </div>
 </li>
        <li> <span class="li-head">header_via_request</span> - Action to take on the HTTP via header in forwarded requests: forwards (pass), adds, or removes the HTTP header. <span class="li-normal">type: str</span> <span class="li-normal">choices: pass, add, remove</span>
 <a id='label6' href="javascript:ContentClick('label7', 'label6');" onmouseover="ContentPreview('label7');" onmouseout="ContentUnpreview('label7');" title="click to collapse or expand..."> more... </a>
 <div id="label7" style="display:none">
 <table border="1">
 <tr>
 <td></td>
 <td colspan="1">Supported Version Ranges</td>
 </tr>
 <tr>
 <td>header_via_request</td>
 <td><code class="docutils literal notranslate">v6.0.0 -> 7.4.4 </code></td>
 </tr>
 <tr>
 <td>[pass]</td>
 <td><code class="docutils literal notranslate">v6.0.0 -> 7.4.4</code></td>
 <tr>
 <td>[add]</td>
 <td><code class="docutils literal notranslate">v6.0.0 -> 7.4.4</code></td>
 <tr>
 <td>[remove]</td>
 <td><code class="docutils literal notranslate">v6.0.0 -> 7.4.4</code></td>
 </table>
 </div>
 </li>
        <li> <span class="li-head">header_via_response</span> - Action to take on the HTTP via header in forwarded responses: forwards (pass), adds, or removes the HTTP header. <span class="li-normal">type: str</span> <span class="li-normal">choices: pass, add, remove</span>
 <a id='label8' href="javascript:ContentClick('label9', 'label8');" onmouseover="ContentPreview('label9');" onmouseout="ContentUnpreview('label9');" title="click to collapse or expand..."> more... </a>
 <div id="label9" style="display:none">
 <table border="1">
 <tr>
 <td></td>
 <td colspan="1">Supported Version Ranges</td>
 </tr>
 <tr>
 <td>header_via_response</td>
 <td><code class="docutils literal notranslate">v6.0.0 -> 7.4.4 </code></td>
 </tr>
 <tr>
 <td>[pass]</td>
 <td><code class="docutils literal notranslate">v6.0.0 -> 7.4.4</code></td>
 <tr>
 <td>[add]</td>
 <td><code class="docutils literal notranslate">v6.0.0 -> 7.4.4</code></td>
 <tr>
 <td>[remove]</td>
 <td><code class="docutils literal notranslate">v6.0.0 -> 7.4.4</code></td>
 </table>
 </div>
 </li>
        <li> <span class="li-head">header_x_authenticated_groups</span> - Action to take on the HTTP x-authenticated-groups header in forwarded requests: forwards (pass), adds, or removes the HTTP header. <span class="li-normal">type: str</span> <span class="li-normal">choices: pass, add, remove</span>
 <a id='label10' href="javascript:ContentClick('label11', 'label10');" onmouseover="ContentPreview('label11');" onmouseout="ContentUnpreview('label11');" title="click to collapse or expand..."> more... </a>
 <div id="label11" style="display:none">
 <table border="1">
 <tr>
 <td></td>
 <td colspan="1">Supported Version Ranges</td>
 </tr>
 <tr>
 <td>header_x_authenticated_groups</td>
 <td><code class="docutils literal notranslate">v6.0.0 -> 7.4.4 </code></td>
 </tr>
 <tr>
 <td>[pass]</td>
 <td><code class="docutils literal notranslate">v6.0.0 -> 7.4.4</code></td>
 <tr>
 <td>[add]</td>
 <td><code class="docutils literal notranslate">v6.0.0 -> 7.4.4</code></td>
 <tr>
 <td>[remove]</td>
 <td><code class="docutils literal notranslate">v6.0.0 -> 7.4.4</code></td>
 </table>
 </div>
 </li>
        <li> <span class="li-head">header_x_authenticated_user</span> - Action to take on the HTTP x-authenticated-user header in forwarded requests: forwards (pass), adds, or removes the HTTP header. <span class="li-normal">type: str</span> <span class="li-normal">choices: pass, add, remove</span>
 <a id='label12' href="javascript:ContentClick('label13', 'label12');" onmouseover="ContentPreview('label13');" onmouseout="ContentUnpreview('label13');" title="click to collapse or expand..."> more... </a>
 <div id="label13" style="display:none">
 <table border="1">
 <tr>
 <td></td>
 <td colspan="1">Supported Version Ranges</td>
 </tr>
 <tr>
 <td>header_x_authenticated_user</td>
 <td><code class="docutils literal notranslate">v6.0.0 -> 7.4.4 </code></td>
 </tr>
 <tr>
 <td>[pass]</td>
 <td><code class="docutils literal notranslate">v6.0.0 -> 7.4.4</code></td>
 <tr>
 <td>[add]</td>
 <td><code class="docutils literal notranslate">v6.0.0 -> 7.4.4</code></td>
 <tr>
 <td>[remove]</td>
 <td><code class="docutils literal notranslate">v6.0.0 -> 7.4.4</code></td>
 </table>
 </div>
 </li>
        <li> <span class="li-head">header_x_forwarded_client_cert</span> - Action to take on the HTTP x-forwarded-client-cert header in forwarded requests: forwards (pass), adds, or removes the HTTP header. <span class="li-normal">type: str</span> <span class="li-normal">choices: pass, add, remove</span>
 <a id='label14' href="javascript:ContentClick('label15', 'label14');" onmouseover="ContentPreview('label15');" onmouseout="ContentUnpreview('label15');" title="click to collapse or expand..."> more... </a>
 <div id="label15" style="display:none">
 <table border="1">
 <tr>
 <td></td>
 <td colspan="1">Supported Version Ranges</td>
 </tr>
 <tr>
 <td>header_x_forwarded_client_cert</td>
 <td><code class="docutils literal notranslate">v7.0.1 -> 7.4.4 </code></td>
 </tr>
 <tr>
 <td>[pass]</td>
 <td><code class="docutils literal notranslate">v7.0.1 -> 7.4.4</code></td>
 <tr>
 <td>[add]</td>
 <td><code class="docutils literal notranslate">v7.0.1 -> 7.4.4</code></td>
 <tr>
 <td>[remove]</td>
 <td><code class="docutils literal notranslate">v7.0.1 -> 7.4.4</code></td>
 </table>
 </div>
 </li>
        <li> <span class="li-head">header_x_forwarded_for</span> - Action to take on the HTTP x-forwarded-for header in forwarded requests: forwards (pass), adds, or removes the HTTP header. <span class="li-normal">type: str</span> <span class="li-normal">choices: pass, add, remove</span>
 <a id='label16' href="javascript:ContentClick('label17', 'label16');" onmouseover="ContentPreview('label17');" onmouseout="ContentUnpreview('label17');" title="click to collapse or expand..."> more... </a>
 <div id="label17" style="display:none">
 <table border="1">
 <tr>
 <td></td>
 <td colspan="1">Supported Version Ranges</td>
 </tr>
 <tr>
 <td>header_x_forwarded_for</td>
 <td><code class="docutils literal notranslate">v6.0.0 -> 7.4.4 </code></td>
 </tr>
 <tr>
 <td>[pass]</td>
 <td><code class="docutils literal notranslate">v6.0.0 -> 7.4.4</code></td>
 <tr>
 <td>[add]</td>
 <td><code class="docutils literal notranslate">v6.0.0 -> 7.4.4</code></td>
 <tr>
 <td>[remove]</td>
 <td><code class="docutils literal notranslate">v6.0.0 -> 7.4.4</code></td>
 </table>
 </div>
 </li>
        <li> <span class="li-head">headers</span> - Configure HTTP forwarded requests headers. <span class="li-normal">type: list</span> <span style="font-family:'Courier New'" class="li-required">member_path: headers:id</span>
 <a id='label18' href="javascript:ContentClick('label19', 'label18');" onmouseover="ContentPreview('label19');" onmouseout="ContentUnpreview('label19');" title="click to collapse or expand..."> more... </a>
 <div id="label19" style="display:none">
 <table border="1">
 <tr>
 <td></td><td colspan="1">Supported Version Ranges</td>
 </tr>
 <tr>
 <td>headers</td>
 <td><code class="docutils literal notranslate">v6.0.0 -> 7.4.4 </code></td>
 </tr>
 </table>
 </div>
 </li>
            <ul class="ul-self">
            <li> <span class="li-head">action</span> - Configure adding, removing, or logging of the HTTP header entry in HTTP requests and responses. <span class="li-normal">type: str</span> <span class="li-normal">choices: add-to-request, add-to-response, remove-from-request, remove-from-response, monitor-request, monitor-response</span>
 <a id='label20' href="javascript:ContentClick('label21', 'label20');" onmouseover="ContentPreview('label21');" onmouseout="ContentUnpreview('label21');" title="click to collapse or expand..."> more... </a>
 <div id="label21" style="display:none">
 <table border="1">
 <tr>
 <td></td>
 <td colspan="1">Supported Version Ranges</td>
 </tr>
 <tr>
 <td>action</td>
 <td><code class="docutils literal notranslate">v6.0.0 -> 7.4.4 </code></td>
 </tr>
 <tr>
 <td>[add-to-request]</td>
 <td><code class="docutils literal notranslate">v6.0.0 -> 7.4.4</code></td>
 <tr>
 <td>[add-to-response]</td>
 <td><code class="docutils literal notranslate">v6.0.0 -> 7.4.4</code></td>
 <tr>
 <td>[remove-from-request]</td>
 <td><code class="docutils literal notranslate">v6.0.0 -> 7.4.4</code></td>
 <tr>
 <td>[remove-from-response]</td>
 <td><code class="docutils literal notranslate">v6.0.0 -> 7.4.4</code></td>
 <tr>
 <td>[monitor-request]</td>
 <td><code class="docutils literal notranslate">v7.4.0 -> 7.4.4</code></td>
 </tr>
 <tr>
 <td>[monitor-response]</td>
 <td><code class="docutils literal notranslate">v7.4.0 -> 7.4.4</code></td>
 </tr>
 </table>
 </div>
 </li>
            <li> <span class="li-head">add_option</span> - Configure options to append content to existing HTTP header or add new HTTP header. <span class="li-normal">type: str</span> <span class="li-normal">choices: append, new-on-not-found, new</span>
 <a id='label22' href="javascript:ContentClick('label23', 'label22');" onmouseover="ContentPreview('label23');" onmouseout="ContentUnpreview('label23');" title="click to collapse or expand..."> more... </a>
 <div id="label23" style="display:none">
 <table border="1">
 <tr>
 <td></td>
 <td colspan="1">Supported Version Ranges</td>
 </tr>
 <tr>
 <td>add_option</td>
 <td><code class="docutils literal notranslate">v6.2.0 -> 7.4.4 </code></td>
 </tr>
 <tr>
 <td>[append]</td>
 <td><code class="docutils literal notranslate">v6.2.0 -> 7.4.4</code></td>
 <tr>
 <td>[new-on-not-found]</td>
 <td><code class="docutils literal notranslate">v6.2.0 -> 7.4.4</code></td>
 <tr>
 <td>[new]</td>
 <td><code class="docutils literal notranslate">v6.2.0 -> 7.4.4</code></td>
 </table>
 </div>
 </li>
            <li> <span class="li-head">base64_encoding</span> - Enable/disable use of base64 encoding of HTTP content. <span class="li-normal">type: str</span> <span class="li-normal">choices: disable, enable</span>
 <a id='label24' href="javascript:ContentClick('label25', 'label24');" onmouseover="ContentPreview('label25');" onmouseout="ContentUnpreview('label25');" title="click to collapse or expand..."> more... </a>
 <div id="label25" style="display:none">
 <table border="1">
 <tr>
 <td></td>
 <td colspan="1">Supported Version Ranges</td>
 </tr>
 <tr>
 <td>base64_encoding</td>
 <td><code class="docutils literal notranslate">v6.2.0 -> 7.4.4 </code></td>
 </tr>
 <tr>
 <td>[disable]</td>
 <td><code class="docutils literal notranslate">v6.2.0 -> 7.4.4</code></td>
 <tr>
 <td>[enable]</td>
 <td><code class="docutils literal notranslate">v6.2.0 -> 7.4.4</code></td>
 </table>
 </div>
 </li>
            <li> <span class="li-head">content</span> - HTTP header content. <span class="li-normal">type: str</span>
 <a id='label26' href="javascript:ContentClick('label27', 'label26');" onmouseover="ContentPreview('label27');" onmouseout="ContentUnpreview('label27');" title="click to collapse or expand..."> more... </a>
 <div id="label27" style="display:none">
 <table border="1">
 <tr>
 <td></td>
 <td colspan="1">Supported Version Ranges</td>
 </tr>
 <tr>
 <td>content</td>
 <td><code class="docutils literal notranslate">v6.0.0 -> 7.4.4 </code></td>
 </tr>
 </table>
 </div>
 </li>
            <li> <span class="li-head">dstaddr</span> - Destination address and address group names. <span class="li-normal">type: list</span> <span style="font-family:'Courier New'" class="li-required">member_path: headers:id/dstaddr:name</span>
 <a id='label28' href="javascript:ContentClick('label29', 'label28');" onmouseover="ContentPreview('label29');" onmouseout="ContentUnpreview('label29');" title="click to collapse or expand..."> more... </a>
 <div id="label29" style="display:none">
 <table border="1">
 <tr>
 <td></td><td colspan="1">Supported Version Ranges</td>
 </tr>
 <tr>
 <td>dstaddr</td>
 <td><code class="docutils literal notranslate">v6.2.0 -> 7.4.4 </code></td>
 </tr>
 </table>
 </div>
 </li>
                <ul class="ul-self">
                <li> <span class="li-head">name</span> - Address name. Source firewall.address.name firewall.addrgrp.name. <span class="li-normal">type: str</span> <span class="li-required">required: true</span>
 <a id='label30' href="javascript:ContentClick('label31', 'label30');" onmouseover="ContentPreview('label31');" onmouseout="ContentUnpreview('label31');" title="click to collapse or expand..."> more... </a>
 <div id="label31" style="display:none">
 <table border="1">
 <tr>
 <td></td>
 <td colspan="1">Supported Version Ranges</td>
 </tr>
 <tr>
 <td>name</td>
 <td><code class="docutils literal notranslate">v6.2.0 -> 7.4.4 </code></td>
 </tr>
 </table>
 </div>
 </li>
                </ul>
            <li> <span class="li-head">dstaddr6</span> - Destination address and address group names (IPv6). <span class="li-normal">type: list</span> <span style="font-family:'Courier New'" class="li-required">member_path: headers:id/dstaddr6:name</span>
 <a id='label32' href="javascript:ContentClick('label33', 'label32');" onmouseover="ContentPreview('label33');" onmouseout="ContentUnpreview('label33');" title="click to collapse or expand..."> more... </a>
 <div id="label33" style="display:none">
 <table border="1">
 <tr>
 <td></td><td colspan="1">Supported Version Ranges</td>
 </tr>
 <tr>
 <td>dstaddr6</td>
 <td><code class="docutils literal notranslate">v6.2.0 -> 7.4.4 </code></td>
 </tr>
 </table>
 </div>
 </li>
                <ul class="ul-self">
                <li> <span class="li-head">name</span> - Address name. Source firewall.address6.name firewall.addrgrp6.name. <span class="li-normal">type: str</span> <span class="li-required">required: true</span>
 <a id='label34' href="javascript:ContentClick('label35', 'label34');" onmouseover="ContentPreview('label35');" onmouseout="ContentUnpreview('label35');" title="click to collapse or expand..."> more... </a>
 <div id="label35" style="display:none">
 <table border="1">
 <tr>
 <td></td>
 <td colspan="1">Supported Version Ranges</td>
 </tr>
 <tr>
 <td>name</td>
 <td><code class="docutils literal notranslate">v6.2.0 -> 7.4.4 </code></td>
 </tr>
 </table>
 </div>
 </li>
                </ul>
            <li> <span class="li-head">id</span> - HTTP forwarded header id. see <a href='#notes'>Notes</a>. <span class="li-normal">type: int</span> <span class="li-required">required: true</span>
 <a id='label36' href="javascript:ContentClick('label37', 'label36');" onmouseover="ContentPreview('label37');" onmouseout="ContentUnpreview('label37');" title="click to collapse or expand..."> more... </a>
 <div id="label37" style="display:none">
 <table border="1">
 <tr>
 <td></td>
 <td colspan="1">Supported Version Ranges</td>
 </tr>
 <tr>
 <td>id</td>
 <td><code class="docutils literal notranslate">v6.0.0 -> 7.4.4 </code></td>
 </tr>
 </table>
 </div>
 </li>
            <li> <span class="li-head">name</span> - HTTP forwarded header name. <span class="li-normal">type: str</span>
 <a id='label38' href="javascript:ContentClick('label39', 'label38');" onmouseover="ContentPreview('label39');" onmouseout="ContentUnpreview('label39');" title="click to collapse or expand..."> more... </a>
 <div id="label39" style="display:none">
 <table border="1">
 <tr>
 <td></td>
 <td colspan="1">Supported Version Ranges</td>
 </tr>
 <tr>
 <td>name</td>
 <td><code class="docutils literal notranslate">v6.0.0 -> 7.4.4 </code></td>
 </tr>
 </table>
 </div>
 </li>
            <li> <span class="li-head">protocol</span> - Configure protocol(s) to take add-option action on (HTTP, HTTPS, or both). <span class="li-normal">type: list</span> <span class="li-normal">choices: https, http</span>
 <a id='label40' href="javascript:ContentClick('label41', 'label40');" onmouseover="ContentPreview('label41');" onmouseout="ContentUnpreview('label41');" title="click to collapse or expand..."> more... </a>
 <div id="label41" style="display:none">
 <table border="1">
 <tr>
 <td></td>
 <td colspan="1">Supported Version Ranges</td>
 </tr>
 <tr>
 <td>protocol</td>
 <td><code class="docutils literal notranslate">v6.2.0 -> 7.4.4 </code></td>
 </tr>
 <tr>
 <td>[https]</td>
 <td><code class="docutils literal notranslate">v6.2.0 -> 7.4.4</code></td>
 <tr>
 <td>[http]</td>
 <td><code class="docutils literal notranslate">v6.2.0 -> 7.4.4</code></td>
 </table>
 </div>
 </li>
            </ul>
        <li> <span class="li-head">log_header_change</span> - Enable/disable logging HTTP header changes. <span class="li-normal">type: str</span> <span class="li-normal">choices: enable, disable</span>
 <a id='label42' href="javascript:ContentClick('label43', 'label42');" onmouseover="ContentPreview('label43');" onmouseout="ContentUnpreview('label43');" title="click to collapse or expand..."> more... </a>
 <div id="label43" style="display:none">
 <table border="1">
 <tr>
 <td></td>
 <td colspan="1">Supported Version Ranges</td>
 </tr>
 <tr>
 <td>log_header_change</td>
 <td><code class="docutils literal notranslate">v6.0.0 -> 7.4.4 </code></td>
 </tr>
 <tr>
 <td>[enable]</td>
 <td><code class="docutils literal notranslate">v6.0.0 -> 7.4.4</code></td>
 <tr>
 <td>[disable]</td>
 <td><code class="docutils literal notranslate">v6.0.0 -> 7.4.4</code></td>
 </table>
 </div>
 </li>
        <li> <span class="li-head">name</span> - Profile name. <span class="li-normal">type: str</span> <span class="li-required">required: true</span>
 <a id='label44' href="javascript:ContentClick('label45', 'label44');" onmouseover="ContentPreview('label45');" onmouseout="ContentUnpreview('label45');" title="click to collapse or expand..."> more... </a>
 <div id="label45" style="display:none">
 <table border="1">
 <tr>
 <td></td>
 <td colspan="1">Supported Version Ranges</td>
 </tr>
 <tr>
 <td>name</td>
 <td><code class="docutils literal notranslate">v6.0.0 -> 7.4.4 </code></td>
 </tr>
 </table>
 </div>
 </li>
        <li> <span class="li-head">strip_encoding</span> - Enable/disable stripping unsupported encoding from the request header. <span class="li-normal">type: str</span> <span class="li-normal">choices: enable, disable</span>
 <a id='label46' href="javascript:ContentClick('label47', 'label46');" onmouseover="ContentPreview('label47');" onmouseout="ContentUnpreview('label47');" title="click to collapse or expand..."> more... </a>
 <div id="label47" style="display:none">
 <table border="1">
 <tr>
 <td></td>
 <td colspan="1">Supported Version Ranges</td>
 </tr>
 <tr>
 <td>strip_encoding</td>
 <td><code class="docutils literal notranslate">v6.0.0 -> 7.4.4 </code></td>
 </tr>
 <tr>
 <td>[enable]</td>
 <td><code class="docutils literal notranslate">v6.0.0 -> 7.4.4</code></td>
 <tr>
 <td>[disable]</td>
 <td><code class="docutils literal notranslate">v6.0.0 -> 7.4.4</code></td>
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
    
    - name: Configure web proxy profiles.
      fortinet.fortios.fortios_web_proxy_profile:
          vdom: "{{ vdom }}"
          state: "present"
          access_token: "<your_own_value>"
          web_proxy_profile:
              header_client_ip: "pass"
              header_front_end_https: "pass"
              header_via_request: "pass"
              header_via_response: "pass"
              header_x_authenticated_groups: "pass"
              header_x_authenticated_user: "pass"
              header_x_forwarded_client_cert: "pass"
              header_x_forwarded_for: "pass"
              headers:
                  -
                      action: "add-to-request"
                      add_option: "append"
                      base64_encoding: "disable"
                      content: "<your_own_value>"
                      dstaddr:
                          -
                              name: "default_name_17 (source firewall.address.name firewall.addrgrp.name)"
                      dstaddr6:
                          -
                              name: "default_name_19 (source firewall.address6.name firewall.addrgrp6.name)"
                      id: "20"
                      name: "default_name_21"
                      protocol: "https"
              log_header_change: "enable"
              name: "default_name_24"
              strip_encoding: "enable"


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
