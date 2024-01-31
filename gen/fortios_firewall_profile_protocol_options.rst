:source: fortios_firewall_profile_protocol_options.py

:orphan:

.. fortios_firewall_profile_protocol_options:

fortios_firewall_profile_protocol_options -- Configure protocol options in Fortinet's FortiOS and FortiGate.
++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++

.. versionadded:: 2.0.0

.. contents::
   :local:
   :depth: 1


Synopsis
--------
- This module is able to configure a FortiGate or FortiOS (FOS) device by allowing the user to set and modify firewall feature and profile_protocol_options category. Examples include all parameters and values need to be adjusted to datasources before usage. Tested with FOS v6.0.0



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
 <td>fortios_firewall_profile_protocol_options</td>
 <td><code class="docutils literal notranslate">v6.0.0 -> latest </code></td>
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
    <li> <span class="li-head">firewall_profile_protocol_options</span> - Configure protocol options. <span class="li-normal">type: dict</span>
 <a id='label0' href="javascript:ContentClick('label1', 'label0');" onmouseover="ContentPreview('label1');" onmouseout="ContentUnpreview('label1');" title="click to collapse or expand..."> more... </a>
 <div id="label1" style="display:none">
 <table border="1">
 <tr>
 <td></td><td colspan="1">Supported Version Ranges</td>
 </tr>
 <tr>
 <td>firewall_profile_protocol_options</td>
 <td><code class="docutils literal notranslate">v6.0.0 -> latest </code></td>
 </tr>
 </table>
 </div>
 </li>
        <ul class="ul-self">
        <li> <span class="li-head">cifs</span> - Configure CIFS protocol options. <span class="li-normal">type: dict</span>
 <a id='label2' href="javascript:ContentClick('label3', 'label2');" onmouseover="ContentPreview('label3');" onmouseout="ContentUnpreview('label3');" title="click to collapse or expand..."> more... </a>
 <div id="label3" style="display:none">
 <table border="1">
 <tr>
 <td></td><td colspan="1">Supported Version Ranges</td>
 </tr>
 <tr>
 <td>cifs</td>
 <td><code class="docutils literal notranslate">v6.2.0 -> latest </code></td>
 </tr>
 </table>
 </div>
 </li>
            <ul class="ul-self">
            <li> <span class="li-head">domain_controller</span> - Domain for which to decrypt CIFS traffic. Source user.domain-controller.name credential-store.domain-controller.server-name. <span class="li-normal">type: str</span>
 <a id='label4' href="javascript:ContentClick('label5', 'label4');" onmouseover="ContentPreview('label5');" onmouseout="ContentUnpreview('label5');" title="click to collapse or expand..."> more... </a>
 <div id="label5" style="display:none">
 <table border="1">
 <tr>
 <td></td>
 <td colspan="2">Supported Version Ranges</td>
 </tr>
 <tr>
 <td>domain_controller</td>
 <td><code class="docutils literal notranslate">v6.4.0 -> v6.4.0 </code></td>
 <td><code class="docutils literal notranslate">v6.4.4 -> latest </code></td>
 </tr>
 </table>
 </div>
 </li>
            <li> <span class="li-head">options</span> - One or more options that can be applied to the session. <span class="li-normal">type: list</span> <span class="li-normal">choices: oversize</span>
 <a id='label6' href="javascript:ContentClick('label7', 'label6');" onmouseover="ContentPreview('label7');" onmouseout="ContentUnpreview('label7');" title="click to collapse or expand..."> more... </a>
 <div id="label7" style="display:none">
 <table border="1">
 <tr>
 <td></td>
 <td colspan="1">Supported Version Ranges</td>
 </tr>
 <tr>
 <td>options</td>
 <td><code class="docutils literal notranslate">v6.4.0 -> latest </code></td>
 </tr>
 <tr>
 <td>[oversize]</td>
 <td><code class="docutils literal notranslate">v6.0.0 -> latest</code></td> </table>
 </div>
 </li>
            <li> <span class="li-head">oversize_limit</span> - Maximum in-memory file size that can be scanned (MB). <span class="li-normal">type: int</span>
 <a id='label8' href="javascript:ContentClick('label9', 'label8');" onmouseover="ContentPreview('label9');" onmouseout="ContentUnpreview('label9');" title="click to collapse or expand..."> more... </a>
 <div id="label9" style="display:none">
 <table border="1">
 <tr>
 <td></td>
 <td colspan="1">Supported Version Ranges</td>
 </tr>
 <tr>
 <td>oversize_limit</td>
 <td><code class="docutils literal notranslate">v6.4.0 -> latest </code></td>
 </tr>
 </table>
 </div>
 </li>
            <li> <span class="li-head">ports</span> - Ports to scan for content (1 - 65535). <span class="li-normal">type: list</span> </li>
            <li> <span class="li-head">scan_bzip2</span> - Enable/disable scanning of BZip2 compressed files. <span class="li-normal">type: str</span> <span class="li-normal">choices: enable, disable</span>
 <a id='label10' href="javascript:ContentClick('label11', 'label10');" onmouseover="ContentPreview('label11');" onmouseout="ContentUnpreview('label11');" title="click to collapse or expand..."> more... </a>
 <div id="label11" style="display:none">
 <table border="1">
 <tr>
 <td></td>
 <td colspan="1">Supported Version Ranges</td>
 </tr>
 <tr>
 <td>scan_bzip2</td>
 <td><code class="docutils literal notranslate">v6.4.0 -> latest </code></td>
 </tr>
 <tr>
 <td>[enable]</td>
 <td><code class="docutils literal notranslate">v6.0.0 -> latest</code></td> <tr>
 <td>[disable]</td>
 <td><code class="docutils literal notranslate">v6.0.0 -> latest</code></td> </table>
 </div>
 </li>
            <li> <span class="li-head">server_credential_type</span> - CIFS server credential type. <span class="li-normal">type: str</span> <span class="li-normal">choices: none, credential-replication, credential-keytab</span>
 <a id='label12' href="javascript:ContentClick('label13', 'label12');" onmouseover="ContentPreview('label13');" onmouseout="ContentUnpreview('label13');" title="click to collapse or expand..."> more... </a>
 <div id="label13" style="display:none">
 <table border="1">
 <tr>
 <td></td>
 <td colspan="2">Supported Version Ranges</td>
 </tr>
 <tr>
 <td>server_credential_type</td>
 <td><code class="docutils literal notranslate">v6.2.7 -> v6.4.0 </code></td>
 <td><code class="docutils literal notranslate">v6.4.4 -> latest </code></td>
 </tr>
 <tr>
 <td>[none]</td>
 <td><code class="docutils literal notranslate">v6.0.0 -> latest</code></td> <tr>
 <td>[credential-replication]</td>
 <td><code class="docutils literal notranslate">v6.0.0 -> latest</code></td> <tr>
 <td>[credential-keytab]</td>
 <td><code class="docutils literal notranslate">v6.0.0 -> latest</code></td> </table>
 </div>
 </li>
            <li> <span class="li-head">server_keytab</span> - Server keytab. <span class="li-normal">type: list</span> <span style="font-family:'Courier New'" class="li-required">member_path: cifs/server_keytab:principal</span>
 <a id='label14' href="javascript:ContentClick('label15', 'label14');" onmouseover="ContentPreview('label15');" onmouseout="ContentUnpreview('label15');" title="click to collapse or expand..."> more... </a>
 <div id="label15" style="display:none">
 <table border="1">
 <tr>
 <td></td><td colspan="2">Supported Version Ranges</td>
 </tr>
 <tr>
 <td>server_keytab</td>
 <td><code class="docutils literal notranslate">v6.2.7 -> v6.4.0 </code></td>
 <td><code class="docutils literal notranslate">v6.4.4 -> latest </code></td>
 </tr>
 </table>
 </div>
 </li>
                <ul class="ul-self">
                <li> <span class="li-head">keytab</span> - Base64 encoded keytab file containing credential of the server. <span class="li-normal">type: str</span>
 <a id='label16' href="javascript:ContentClick('label17', 'label16');" onmouseover="ContentPreview('label17');" onmouseout="ContentUnpreview('label17');" title="click to collapse or expand..."> more... </a>
 <div id="label17" style="display:none">
 <table border="1">
 <tr>
 <td></td>
 <td colspan="2">Supported Version Ranges</td>
 </tr>
 <tr>
 <td>keytab</td>
 <td><code class="docutils literal notranslate">v6.2.7 -> v6.4.0 </code></td>
 <td><code class="docutils literal notranslate">v6.4.4 -> latest </code></td>
 </tr>
 </table>
 </div>
 </li>
                <li> <span class="li-head">principal</span> - Service principal. For example, host/cifsserver.example.com@example.com. <span class="li-normal">type: str</span> <span class="li-required">required: true</span>
 <a id='label18' href="javascript:ContentClick('label19', 'label18');" onmouseover="ContentPreview('label19');" onmouseout="ContentUnpreview('label19');" title="click to collapse or expand..."> more... </a>
 <div id="label19" style="display:none">
 <table border="1">
 <tr>
 <td></td>
 <td colspan="2">Supported Version Ranges</td>
 </tr>
 <tr>
 <td>principal</td>
 <td><code class="docutils literal notranslate">v6.2.7 -> v6.4.0 </code></td>
 <td><code class="docutils literal notranslate">v6.4.4 -> latest </code></td>
 </tr>
 </table>
 </div>
 </li>
                </ul>
            <li> <span class="li-head">status</span> - Enable/disable the active status of scanning for this protocol. <span class="li-normal">type: str</span> <span class="li-normal">choices: enable, disable</span>
 <a id='label20' href="javascript:ContentClick('label21', 'label20');" onmouseover="ContentPreview('label21');" onmouseout="ContentUnpreview('label21');" title="click to collapse or expand..."> more... </a>
 <div id="label21" style="display:none">
 <table border="1">
 <tr>
 <td></td>
 <td colspan="1">Supported Version Ranges</td>
 </tr>
 <tr>
 <td>status</td>
 <td><code class="docutils literal notranslate">v6.2.0 -> latest </code></td>
 </tr>
 <tr>
 <td>[enable]</td>
 <td><code class="docutils literal notranslate">v6.0.0 -> latest</code></td> <tr>
 <td>[disable]</td>
 <td><code class="docutils literal notranslate">v6.0.0 -> latest</code></td> </table>
 </div>
 </li>
            <li> <span class="li-head">tcp_window_maximum</span> - Maximum dynamic TCP window size. <span class="li-normal">type: int</span>
 <a id='label22' href="javascript:ContentClick('label23', 'label22');" onmouseover="ContentPreview('label23');" onmouseout="ContentUnpreview('label23');" title="click to collapse or expand..."> more... </a>
 <div id="label23" style="display:none">
 <table border="1">
 <tr>
 <td></td>
 <td colspan="1">Supported Version Ranges</td>
 </tr>
 <tr>
 <td>tcp_window_maximum</td>
 <td><code class="docutils literal notranslate">v6.4.0 -> latest </code></td>
 </tr>
 </table>
 </div>
 </li>
            <li> <span class="li-head">tcp_window_minimum</span> - Minimum dynamic TCP window size. <span class="li-normal">type: int</span>
 <a id='label24' href="javascript:ContentClick('label25', 'label24');" onmouseover="ContentPreview('label25');" onmouseout="ContentUnpreview('label25');" title="click to collapse or expand..."> more... </a>
 <div id="label25" style="display:none">
 <table border="1">
 <tr>
 <td></td>
 <td colspan="1">Supported Version Ranges</td>
 </tr>
 <tr>
 <td>tcp_window_minimum</td>
 <td><code class="docutils literal notranslate">v6.4.0 -> latest </code></td>
 </tr>
 </table>
 </div>
 </li>
            <li> <span class="li-head">tcp_window_size</span> - Set TCP static window size. <span class="li-normal">type: int</span>
 <a id='label26' href="javascript:ContentClick('label27', 'label26');" onmouseover="ContentPreview('label27');" onmouseout="ContentUnpreview('label27');" title="click to collapse or expand..."> more... </a>
 <div id="label27" style="display:none">
 <table border="1">
 <tr>
 <td></td>
 <td colspan="1">Supported Version Ranges</td>
 </tr>
 <tr>
 <td>tcp_window_size</td>
 <td><code class="docutils literal notranslate">v6.4.0 -> latest </code></td>
 </tr>
 </table>
 </div>
 </li>
            <li> <span class="li-head">tcp_window_type</span> - TCP window type to use for this protocol. <span class="li-normal">type: str</span> <span class="li-normal">choices: auto-tuning, system, static, dynamic</span>
 <a id='label28' href="javascript:ContentClick('label29', 'label28');" onmouseover="ContentPreview('label29');" onmouseout="ContentUnpreview('label29');" title="click to collapse or expand..."> more... </a>
 <div id="label29" style="display:none">
 <table border="1">
 <tr>
 <td></td>
 <td colspan="1">Supported Version Ranges</td>
 </tr>
 <tr>
 <td>tcp_window_type</td>
 <td><code class="docutils literal notranslate">v6.4.0 -> latest </code></td>
 </tr>
 <tr>
 <td>[auto-tuning]</td>
 <td><code class="docutils literal notranslate">v7.0.4 -> latest</code></td>
 </tr>
 <tr>
 <td>[system]</td>
 <td><code class="docutils literal notranslate">v6.0.0 -> latest</code></td> <tr>
 <td>[static]</td>
 <td><code class="docutils literal notranslate">v6.0.0 -> latest</code></td> <tr>
 <td>[dynamic]</td>
 <td><code class="docutils literal notranslate">v6.0.0 -> latest</code></td> </table>
 </div>
 </li>
            <li> <span class="li-head">uncompressed_nest_limit</span> - Maximum nested levels of compression that can be uncompressed and scanned (2 - 100). <span class="li-normal">type: int</span>
 <a id='label30' href="javascript:ContentClick('label31', 'label30');" onmouseover="ContentPreview('label31');" onmouseout="ContentUnpreview('label31');" title="click to collapse or expand..."> more... </a>
 <div id="label31" style="display:none">
 <table border="1">
 <tr>
 <td></td>
 <td colspan="1">Supported Version Ranges</td>
 </tr>
 <tr>
 <td>uncompressed_nest_limit</td>
 <td><code class="docutils literal notranslate">v6.4.0 -> latest </code></td>
 </tr>
 </table>
 </div>
 </li>
            <li> <span class="li-head">uncompressed_oversize_limit</span> - Maximum in-memory uncompressed file size that can be scanned. <span class="li-normal">type: int</span>
 <a id='label32' href="javascript:ContentClick('label33', 'label32');" onmouseover="ContentPreview('label33');" onmouseout="ContentUnpreview('label33');" title="click to collapse or expand..."> more... </a>
 <div id="label33" style="display:none">
 <table border="1">
 <tr>
 <td></td>
 <td colspan="1">Supported Version Ranges</td>
 </tr>
 <tr>
 <td>uncompressed_oversize_limit</td>
 <td><code class="docutils literal notranslate">v6.4.0 -> latest </code></td>
 </tr>
 </table>
 </div>
 </li>
            </ul>
        <li> <span class="li-head">comment</span> - Optional comments. <span class="li-normal">type: str</span>
 <a id='label34' href="javascript:ContentClick('label35', 'label34');" onmouseover="ContentPreview('label35');" onmouseout="ContentUnpreview('label35');" title="click to collapse or expand..."> more... </a>
 <div id="label35" style="display:none">
 <table border="1">
 <tr>
 <td></td>
 <td colspan="1">Supported Version Ranges</td>
 </tr>
 <tr>
 <td>comment</td>
 <td><code class="docutils literal notranslate">v6.0.0 -> latest </code></td>
 </tr>
 </table>
 </div>
 </li>
        <li> <span class="li-head">dns</span> - Configure DNS protocol options. <span class="li-normal">type: dict</span>
 <a id='label36' href="javascript:ContentClick('label37', 'label36');" onmouseover="ContentPreview('label37');" onmouseout="ContentUnpreview('label37');" title="click to collapse or expand..."> more... </a>
 <div id="label37" style="display:none">
 <table border="1">
 <tr>
 <td></td><td colspan="1">Supported Version Ranges</td>
 </tr>
 <tr>
 <td>dns</td>
 <td><code class="docutils literal notranslate">v6.0.0 -> latest </code></td>
 </tr>
 </table>
 </div>
 </li>
            <ul class="ul-self">
            <li> <span class="li-head">ports</span> - Ports to scan for content (1 - 65535). <span class="li-normal">type: list</span> </li>
            <li> <span class="li-head">status</span> - Enable/disable the active status of scanning for this protocol. <span class="li-normal">type: str</span> <span class="li-normal">choices: enable, disable</span>
 <a id='label38' href="javascript:ContentClick('label39', 'label38');" onmouseover="ContentPreview('label39');" onmouseout="ContentUnpreview('label39');" title="click to collapse or expand..."> more... </a>
 <div id="label39" style="display:none">
 <table border="1">
 <tr>
 <td></td>
 <td colspan="1">Supported Version Ranges</td>
 </tr>
 <tr>
 <td>status</td>
 <td><code class="docutils literal notranslate">v6.0.0 -> latest </code></td>
 </tr>
 <tr>
 <td>[enable]</td>
 <td><code class="docutils literal notranslate">v6.0.0 -> latest</code></td> <tr>
 <td>[disable]</td>
 <td><code class="docutils literal notranslate">v6.0.0 -> latest</code></td> </table>
 </div>
 </li>
            </ul>
        <li> <span class="li-head">ftp</span> - Configure FTP protocol options. <span class="li-normal">type: dict</span>
 <a id='label40' href="javascript:ContentClick('label41', 'label40');" onmouseover="ContentPreview('label41');" onmouseout="ContentUnpreview('label41');" title="click to collapse or expand..."> more... </a>
 <div id="label41" style="display:none">
 <table border="1">
 <tr>
 <td></td><td colspan="1">Supported Version Ranges</td>
 </tr>
 <tr>
 <td>ftp</td>
 <td><code class="docutils literal notranslate">v6.0.0 -> latest </code></td>
 </tr>
 </table>
 </div>
 </li>
            <ul class="ul-self">
            <li> <span class="li-head">comfort_amount</span> - Number of bytes to send in each transmission for client comforting (bytes). <span class="li-normal">type: int</span>
 <a id='label42' href="javascript:ContentClick('label43', 'label42');" onmouseover="ContentPreview('label43');" onmouseout="ContentUnpreview('label43');" title="click to collapse or expand..."> more... </a>
 <div id="label43" style="display:none">
 <table border="1">
 <tr>
 <td></td>
 <td colspan="1">Supported Version Ranges</td>
 </tr>
 <tr>
 <td>comfort_amount</td>
 <td><code class="docutils literal notranslate">v6.0.0 -> latest </code></td>
 </tr>
 </table>
 </div>
 </li>
            <li> <span class="li-head">comfort_interval</span> - Interval between successive transmissions of data for client comforting (seconds). <span class="li-normal">type: int</span>
 <a id='label44' href="javascript:ContentClick('label45', 'label44');" onmouseover="ContentPreview('label45');" onmouseout="ContentUnpreview('label45');" title="click to collapse or expand..."> more... </a>
 <div id="label45" style="display:none">
 <table border="1">
 <tr>
 <td></td>
 <td colspan="1">Supported Version Ranges</td>
 </tr>
 <tr>
 <td>comfort_interval</td>
 <td><code class="docutils literal notranslate">v6.0.0 -> latest </code></td>
 </tr>
 </table>
 </div>
 </li>
            <li> <span class="li-head">explicit_ftp_tls</span> - Enable/disable FTP redirection for explicit FTPS. <span class="li-normal">type: str</span> <span class="li-normal">choices: enable, disable</span>
 <a id='label46' href="javascript:ContentClick('label47', 'label46');" onmouseover="ContentPreview('label47');" onmouseout="ContentUnpreview('label47');" title="click to collapse or expand..."> more... </a>
 <div id="label47" style="display:none">
 <table border="1">
 <tr>
 <td></td>
 <td colspan="2">Supported Version Ranges</td>
 </tr>
 <tr>
 <td>explicit_ftp_tls</td>
 <td><code class="docutils literal notranslate">v7.0.8 -> v7.0.12 </code></td>
 <td><code class="docutils literal notranslate">v7.2.1 -> latest </code></td>
 </tr>
 <tr>
 <td>[enable]</td>
 <td><code class="docutils literal notranslate">v6.0.0 -> latest</code></td> <tr>
 <td>[disable]</td>
 <td><code class="docutils literal notranslate">v6.0.0 -> latest</code></td> </table>
 </div>
 </li>
            <li> <span class="li-head">inspect_all</span> - Enable/disable the inspection of all ports for the protocol. <span class="li-normal">type: str</span> <span class="li-normal">choices: enable, disable</span>
 <a id='label48' href="javascript:ContentClick('label49', 'label48');" onmouseover="ContentPreview('label49');" onmouseout="ContentUnpreview('label49');" title="click to collapse or expand..."> more... </a>
 <div id="label49" style="display:none">
 <table border="1">
 <tr>
 <td></td>
 <td colspan="1">Supported Version Ranges</td>
 </tr>
 <tr>
 <td>inspect_all</td>
 <td><code class="docutils literal notranslate">v6.0.0 -> latest </code></td>
 </tr>
 <tr>
 <td>[enable]</td>
 <td><code class="docutils literal notranslate">v6.0.0 -> latest</code></td> <tr>
 <td>[disable]</td>
 <td><code class="docutils literal notranslate">v6.0.0 -> latest</code></td> </table>
 </div>
 </li>
            <li> <span class="li-head">options</span> - One or more options that can be applied to the session. <span class="li-normal">type: list</span> <span class="li-normal">choices: clientcomfort, oversize, splice, bypass-rest-command, bypass-mode-command</span>
 <a id='label50' href="javascript:ContentClick('label51', 'label50');" onmouseover="ContentPreview('label51');" onmouseout="ContentUnpreview('label51');" title="click to collapse or expand..."> more... </a>
 <div id="label51" style="display:none">
 <table border="1">
 <tr>
 <td></td>
 <td colspan="1">Supported Version Ranges</td>
 </tr>
 <tr>
 <td>options</td>
 <td><code class="docutils literal notranslate">v6.0.0 -> latest </code></td>
 </tr>
 <tr>
 <td>[clientcomfort]</td>
 <td><code class="docutils literal notranslate">v6.0.0 -> latest</code></td> <tr>
 <td>[oversize]</td>
 <td><code class="docutils literal notranslate">v6.0.0 -> latest</code></td> <tr>
 <td>[splice]</td>
 <td><code class="docutils literal notranslate">v6.0.0 -> latest</code></td> <tr>
 <td>[bypass-rest-command]</td>
 <td><code class="docutils literal notranslate">v6.0.0 -> latest</code></td> <tr>
 <td>[bypass-mode-command]</td>
 <td><code class="docutils literal notranslate">v6.0.0 -> latest</code></td> </table>
 </div>
 </li>
            <li> <span class="li-head">oversize_limit</span> - Maximum in-memory file size that can be scanned (MB). <span class="li-normal">type: int</span>
 <a id='label52' href="javascript:ContentClick('label53', 'label52');" onmouseover="ContentPreview('label53');" onmouseout="ContentUnpreview('label53');" title="click to collapse or expand..."> more... </a>
 <div id="label53" style="display:none">
 <table border="1">
 <tr>
 <td></td>
 <td colspan="1">Supported Version Ranges</td>
 </tr>
 <tr>
 <td>oversize_limit</td>
 <td><code class="docutils literal notranslate">v6.0.0 -> latest </code></td>
 </tr>
 </table>
 </div>
 </li>
            <li> <span class="li-head">ports</span> - Ports to scan for content (1 - 65535). <span class="li-normal">type: list</span> </li>
            <li> <span class="li-head">scan_bzip2</span> - Enable/disable scanning of BZip2 compressed files. <span class="li-normal">type: str</span> <span class="li-normal">choices: enable, disable</span>
 <a id='label54' href="javascript:ContentClick('label55', 'label54');" onmouseover="ContentPreview('label55');" onmouseout="ContentUnpreview('label55');" title="click to collapse or expand..."> more... </a>
 <div id="label55" style="display:none">
 <table border="1">
 <tr>
 <td></td>
 <td colspan="1">Supported Version Ranges</td>
 </tr>
 <tr>
 <td>scan_bzip2</td>
 <td><code class="docutils literal notranslate">v6.0.0 -> latest </code></td>
 </tr>
 <tr>
 <td>[enable]</td>
 <td><code class="docutils literal notranslate">v6.0.0 -> latest</code></td> <tr>
 <td>[disable]</td>
 <td><code class="docutils literal notranslate">v6.0.0 -> latest</code></td> </table>
 </div>
 </li>
            <li> <span class="li-head">ssl_offloaded</span> - SSL decryption and encryption performed by an external device. <span class="li-normal">type: str</span> <span class="li-normal">choices: no, yes</span>
 <a id='label56' href="javascript:ContentClick('label57', 'label56');" onmouseover="ContentPreview('label57');" onmouseout="ContentUnpreview('label57');" title="click to collapse or expand..."> more... </a>
 <div id="label57" style="display:none">
 <table border="1">
 <tr>
 <td></td>
 <td colspan="1">Supported Version Ranges</td>
 </tr>
 <tr>
 <td>ssl_offloaded</td>
 <td><code class="docutils literal notranslate">v6.2.0 -> latest </code></td>
 </tr>
 <tr>
 <td>[no]</td>
 <td><code class="docutils literal notranslate">v6.0.0 -> latest</code></td> <tr>
 <td>[yes]</td>
 <td><code class="docutils literal notranslate">v6.0.0 -> latest</code></td> </table>
 </div>
 </li>
            <li> <span class="li-head">status</span> - Enable/disable the active status of scanning for this protocol. <span class="li-normal">type: str</span> <span class="li-normal">choices: enable, disable</span>
 <a id='label58' href="javascript:ContentClick('label59', 'label58');" onmouseover="ContentPreview('label59');" onmouseout="ContentUnpreview('label59');" title="click to collapse or expand..."> more... </a>
 <div id="label59" style="display:none">
 <table border="1">
 <tr>
 <td></td>
 <td colspan="1">Supported Version Ranges</td>
 </tr>
 <tr>
 <td>status</td>
 <td><code class="docutils literal notranslate">v6.0.0 -> latest </code></td>
 </tr>
 <tr>
 <td>[enable]</td>
 <td><code class="docutils literal notranslate">v6.0.0 -> latest</code></td> <tr>
 <td>[disable]</td>
 <td><code class="docutils literal notranslate">v6.0.0 -> latest</code></td> </table>
 </div>
 </li>
            <li> <span class="li-head">stream_based_uncompressed_limit</span> - Maximum stream-based uncompressed data size that will be scanned in megabytes. Stream-based uncompression used only under certain conditions (unlimited = 0). <span class="li-normal">type: int</span>
 <a id='label60' href="javascript:ContentClick('label61', 'label60');" onmouseover="ContentPreview('label61');" onmouseout="ContentUnpreview('label61');" title="click to collapse or expand..."> more... </a>
 <div id="label61" style="display:none">
 <table border="1">
 <tr>
 <td></td>
 <td colspan="1">Supported Version Ranges</td>
 </tr>
 <tr>
 <td>stream_based_uncompressed_limit</td>
 <td><code class="docutils literal notranslate">v7.0.0 -> latest </code></td>
 </tr>
 </table>
 </div>
 </li>
            <li> <span class="li-head">tcp_window_maximum</span> - Maximum dynamic TCP window size. <span class="li-normal">type: int</span>
 <a id='label62' href="javascript:ContentClick('label63', 'label62');" onmouseover="ContentPreview('label63');" onmouseout="ContentUnpreview('label63');" title="click to collapse or expand..."> more... </a>
 <div id="label63" style="display:none">
 <table border="1">
 <tr>
 <td></td>
 <td colspan="1">Supported Version Ranges</td>
 </tr>
 <tr>
 <td>tcp_window_maximum</td>
 <td><code class="docutils literal notranslate">v7.0.0 -> latest </code></td>
 </tr>
 </table>
 </div>
 </li>
            <li> <span class="li-head">tcp_window_minimum</span> - Minimum dynamic TCP window size. <span class="li-normal">type: int</span>
 <a id='label64' href="javascript:ContentClick('label65', 'label64');" onmouseover="ContentPreview('label65');" onmouseout="ContentUnpreview('label65');" title="click to collapse or expand..."> more... </a>
 <div id="label65" style="display:none">
 <table border="1">
 <tr>
 <td></td>
 <td colspan="1">Supported Version Ranges</td>
 </tr>
 <tr>
 <td>tcp_window_minimum</td>
 <td><code class="docutils literal notranslate">v7.0.0 -> latest </code></td>
 </tr>
 </table>
 </div>
 </li>
            <li> <span class="li-head">tcp_window_size</span> - Set TCP static window size. <span class="li-normal">type: int</span>
 <a id='label66' href="javascript:ContentClick('label67', 'label66');" onmouseover="ContentPreview('label67');" onmouseout="ContentUnpreview('label67');" title="click to collapse or expand..."> more... </a>
 <div id="label67" style="display:none">
 <table border="1">
 <tr>
 <td></td>
 <td colspan="1">Supported Version Ranges</td>
 </tr>
 <tr>
 <td>tcp_window_size</td>
 <td><code class="docutils literal notranslate">v7.0.0 -> latest </code></td>
 </tr>
 </table>
 </div>
 </li>
            <li> <span class="li-head">tcp_window_type</span> - TCP window type to use for this protocol. <span class="li-normal">type: str</span> <span class="li-normal">choices: auto-tuning, system, static, dynamic</span>
 <a id='label68' href="javascript:ContentClick('label69', 'label68');" onmouseover="ContentPreview('label69');" onmouseout="ContentUnpreview('label69');" title="click to collapse or expand..."> more... </a>
 <div id="label69" style="display:none">
 <table border="1">
 <tr>
 <td></td>
 <td colspan="1">Supported Version Ranges</td>
 </tr>
 <tr>
 <td>tcp_window_type</td>
 <td><code class="docutils literal notranslate">v7.0.0 -> latest </code></td>
 </tr>
 <tr>
 <td>[auto-tuning]</td>
 <td><code class="docutils literal notranslate">v7.0.4 -> latest</code></td>
 </tr>
 <tr>
 <td>[system]</td>
 <td><code class="docutils literal notranslate">v6.0.0 -> latest</code></td> <tr>
 <td>[static]</td>
 <td><code class="docutils literal notranslate">v6.0.0 -> latest</code></td> <tr>
 <td>[dynamic]</td>
 <td><code class="docutils literal notranslate">v6.0.0 -> latest</code></td> </table>
 </div>
 </li>
            <li> <span class="li-head">uncompressed_nest_limit</span> - Maximum nested levels of compression that can be uncompressed and scanned (2 - 100). <span class="li-normal">type: int</span>
 <a id='label70' href="javascript:ContentClick('label71', 'label70');" onmouseover="ContentPreview('label71');" onmouseout="ContentUnpreview('label71');" title="click to collapse or expand..."> more... </a>
 <div id="label71" style="display:none">
 <table border="1">
 <tr>
 <td></td>
 <td colspan="1">Supported Version Ranges</td>
 </tr>
 <tr>
 <td>uncompressed_nest_limit</td>
 <td><code class="docutils literal notranslate">v6.0.0 -> latest </code></td>
 </tr>
 </table>
 </div>
 </li>
            <li> <span class="li-head">uncompressed_oversize_limit</span> - Maximum in-memory uncompressed file size that can be scanned. <span class="li-normal">type: int</span>
 <a id='label72' href="javascript:ContentClick('label73', 'label72');" onmouseover="ContentPreview('label73');" onmouseout="ContentUnpreview('label73');" title="click to collapse or expand..."> more... </a>
 <div id="label73" style="display:none">
 <table border="1">
 <tr>
 <td></td>
 <td colspan="1">Supported Version Ranges</td>
 </tr>
 <tr>
 <td>uncompressed_oversize_limit</td>
 <td><code class="docutils literal notranslate">v6.0.0 -> latest </code></td>
 </tr>
 </table>
 </div>
 </li>
            </ul>
        <li> <span class="li-head">http</span> - Configure HTTP protocol options. <span class="li-normal">type: dict</span>
 <a id='label74' href="javascript:ContentClick('label75', 'label74');" onmouseover="ContentPreview('label75');" onmouseout="ContentUnpreview('label75');" title="click to collapse or expand..."> more... </a>
 <div id="label75" style="display:none">
 <table border="1">
 <tr>
 <td></td><td colspan="1">Supported Version Ranges</td>
 </tr>
 <tr>
 <td>http</td>
 <td><code class="docutils literal notranslate">v6.0.0 -> latest </code></td>
 </tr>
 </table>
 </div>
 </li>
            <ul class="ul-self">
            <li> <span class="li-head">address_ip_rating</span> - Enable/disable IP based URL rating. <span class="li-normal">type: str</span> <span class="li-normal">choices: enable, disable</span>
 <a id='label76' href="javascript:ContentClick('label77', 'label76');" onmouseover="ContentPreview('label77');" onmouseout="ContentUnpreview('label77');" title="click to collapse or expand..."> more... </a>
 <div id="label77" style="display:none">
 <table border="1">
 <tr>
 <td></td>
 <td colspan="1">Supported Version Ranges</td>
 </tr>
 <tr>
 <td>address_ip_rating</td>
 <td><code class="docutils literal notranslate">v7.0.6 -> latest </code></td>
 </tr>
 <tr>
 <td>[enable]</td>
 <td><code class="docutils literal notranslate">v6.0.0 -> latest</code></td> <tr>
 <td>[disable]</td>
 <td><code class="docutils literal notranslate">v6.0.0 -> latest</code></td> </table>
 </div>
 </li>
            <li> <span class="li-head">block_page_status_code</span> - Code number returned for blocked HTTP pages (non-FortiGuard only) (100 - 599). <span class="li-normal">type: int</span>
 <a id='label78' href="javascript:ContentClick('label79', 'label78');" onmouseover="ContentPreview('label79');" onmouseout="ContentUnpreview('label79');" title="click to collapse or expand..."> more... </a>
 <div id="label79" style="display:none">
 <table border="1">
 <tr>
 <td></td>
 <td colspan="1">Supported Version Ranges</td>
 </tr>
 <tr>
 <td>block_page_status_code</td>
 <td><code class="docutils literal notranslate">v6.0.0 -> latest </code></td>
 </tr>
 </table>
 </div>
 </li>
            <li> <span class="li-head">comfort_amount</span> - Number of bytes to send in each transmission for client comforting (bytes). <span class="li-normal">type: int</span>
 <a id='label80' href="javascript:ContentClick('label81', 'label80');" onmouseover="ContentPreview('label81');" onmouseout="ContentUnpreview('label81');" title="click to collapse or expand..."> more... </a>
 <div id="label81" style="display:none">
 <table border="1">
 <tr>
 <td></td>
 <td colspan="1">Supported Version Ranges</td>
 </tr>
 <tr>
 <td>comfort_amount</td>
 <td><code class="docutils literal notranslate">v6.0.0 -> latest </code></td>
 </tr>
 </table>
 </div>
 </li>
            <li> <span class="li-head">comfort_interval</span> - Interval between successive transmissions of data for client comforting (seconds). <span class="li-normal">type: int</span>
 <a id='label82' href="javascript:ContentClick('label83', 'label82');" onmouseover="ContentPreview('label83');" onmouseout="ContentUnpreview('label83');" title="click to collapse or expand..."> more... </a>
 <div id="label83" style="display:none">
 <table border="1">
 <tr>
 <td></td>
 <td colspan="1">Supported Version Ranges</td>
 </tr>
 <tr>
 <td>comfort_interval</td>
 <td><code class="docutils literal notranslate">v6.0.0 -> latest </code></td>
 </tr>
 </table>
 </div>
 </li>
            <li> <span class="li-head">fortinet_bar</span> - Enable/disable Fortinet bar on HTML content. <span class="li-normal">type: str</span> <span class="li-normal">choices: enable, disable</span>
 <a id='label84' href="javascript:ContentClick('label85', 'label84');" onmouseover="ContentPreview('label85');" onmouseout="ContentUnpreview('label85');" title="click to collapse or expand..."> more... </a>
 <div id="label85" style="display:none">
 <table border="1">
 <tr>
 <td></td>
 <td colspan="2">Supported Version Ranges</td>
 </tr>
 <tr>
 <td>fortinet_bar</td>
 <td><code class="docutils literal notranslate">v6.0.0 -> v6.2.7 </code></td>
 <td><code class="docutils literal notranslate">v6.4.1 -> v6.4.1 </code></td>
 </tr>
 <tr>
 <td>[enable]</td>
 <td><code class="docutils literal notranslate">v6.0.0 -> latest</code></td> <tr>
 <td>[disable]</td>
 <td><code class="docutils literal notranslate">v6.0.0 -> latest</code></td> </table>
 </div>
 </li>
            <li> <span class="li-head">fortinet_bar_port</span> - Port for use by Fortinet Bar (1 - 65535). <span class="li-normal">type: int</span>
 <a id='label86' href="javascript:ContentClick('label87', 'label86');" onmouseover="ContentPreview('label87');" onmouseout="ContentUnpreview('label87');" title="click to collapse or expand..."> more... </a>
 <div id="label87" style="display:none">
 <table border="1">
 <tr>
 <td></td>
 <td colspan="2">Supported Version Ranges</td>
 </tr>
 <tr>
 <td>fortinet_bar_port</td>
 <td><code class="docutils literal notranslate">v6.0.0 -> v6.2.7 </code></td>
 <td><code class="docutils literal notranslate">v6.4.1 -> v6.4.1 </code></td>
 </tr>
 </table>
 </div>
 </li>
            <li> <span class="li-head">h2c</span> - Enable/disable h2c HTTP connection upgrade. <span class="li-normal">type: str</span> <span class="li-normal">choices: enable, disable</span>
 <a id='label88' href="javascript:ContentClick('label89', 'label88');" onmouseover="ContentPreview('label89');" onmouseout="ContentUnpreview('label89');" title="click to collapse or expand..."> more... </a>
 <div id="label89" style="display:none">
 <table border="1">
 <tr>
 <td></td>
 <td colspan="1">Supported Version Ranges</td>
 </tr>
 <tr>
 <td>h2c</td>
 <td><code class="docutils literal notranslate">v7.2.0 -> latest </code></td>
 </tr>
 <tr>
 <td>[enable]</td>
 <td><code class="docutils literal notranslate">v6.0.0 -> latest</code></td> <tr>
 <td>[disable]</td>
 <td><code class="docutils literal notranslate">v6.0.0 -> latest</code></td> </table>
 </div>
 </li>
            <li> <span class="li-head">http_policy</span> - Enable/disable HTTP policy check. <span class="li-normal">type: str</span> <span class="li-normal">choices: disable, enable</span>
 <a id='label90' href="javascript:ContentClick('label91', 'label90');" onmouseover="ContentPreview('label91');" onmouseout="ContentUnpreview('label91');" title="click to collapse or expand..."> more... </a>
 <div id="label91" style="display:none">
 <table border="1">
 <tr>
 <td></td>
 <td colspan="1">Supported Version Ranges</td>
 </tr>
 <tr>
 <td>http_policy</td>
 <td><code class="docutils literal notranslate">v6.0.0 -> v6.0.11 </code></td>
 </tr>
 <tr>
 <td>[disable]</td>
 <td><code class="docutils literal notranslate">v6.0.0 -> latest</code></td> <tr>
 <td>[enable]</td>
 <td><code class="docutils literal notranslate">v6.0.0 -> latest</code></td> </table>
 </div>
 </li>
            <li> <span class="li-head">inspect_all</span> - Enable/disable the inspection of all ports for the protocol. <span class="li-normal">type: str</span> <span class="li-normal">choices: enable, disable</span>
 <a id='label92' href="javascript:ContentClick('label93', 'label92');" onmouseover="ContentPreview('label93');" onmouseout="ContentUnpreview('label93');" title="click to collapse or expand..."> more... </a>
 <div id="label93" style="display:none">
 <table border="1">
 <tr>
 <td></td>
 <td colspan="1">Supported Version Ranges</td>
 </tr>
 <tr>
 <td>inspect_all</td>
 <td><code class="docutils literal notranslate">v6.0.0 -> latest </code></td>
 </tr>
 <tr>
 <td>[enable]</td>
 <td><code class="docutils literal notranslate">v6.0.0 -> latest</code></td> <tr>
 <td>[disable]</td>
 <td><code class="docutils literal notranslate">v6.0.0 -> latest</code></td> </table>
 </div>
 </li>
            <li> <span class="li-head">options</span> - One or more options that can be applied to the session. <span class="li-normal">type: list</span> <span class="li-normal">choices: clientcomfort, servercomfort, oversize, chunkedbypass</span>
 <a id='label94' href="javascript:ContentClick('label95', 'label94');" onmouseover="ContentPreview('label95');" onmouseout="ContentUnpreview('label95');" title="click to collapse or expand..."> more... </a>
 <div id="label95" style="display:none">
 <table border="1">
 <tr>
 <td></td>
 <td colspan="1">Supported Version Ranges</td>
 </tr>
 <tr>
 <td>options</td>
 <td><code class="docutils literal notranslate">v6.0.0 -> latest </code></td>
 </tr>
 <tr>
 <td>[clientcomfort]</td>
 <td><code class="docutils literal notranslate">v6.0.0 -> latest</code></td> <tr>
 <td>[servercomfort]</td>
 <td><code class="docutils literal notranslate">v6.0.0 -> latest</code></td> <tr>
 <td>[oversize]</td>
 <td><code class="docutils literal notranslate">v6.0.0 -> latest</code></td> <tr>
 <td>[chunkedbypass]</td>
 <td><code class="docutils literal notranslate">v6.0.0 -> latest</code></td> </table>
 </div>
 </li>
            <li> <span class="li-head">oversize_limit</span> - Maximum in-memory file size that can be scanned (MB). <span class="li-normal">type: int</span>
 <a id='label96' href="javascript:ContentClick('label97', 'label96');" onmouseover="ContentPreview('label97');" onmouseout="ContentUnpreview('label97');" title="click to collapse or expand..."> more... </a>
 <div id="label97" style="display:none">
 <table border="1">
 <tr>
 <td></td>
 <td colspan="1">Supported Version Ranges</td>
 </tr>
 <tr>
 <td>oversize_limit</td>
 <td><code class="docutils literal notranslate">v6.0.0 -> latest </code></td>
 </tr>
 </table>
 </div>
 </li>
            <li> <span class="li-head">ports</span> - Ports to scan for content (1 - 65535). <span class="li-normal">type: list</span> </li>
            <li> <span class="li-head">post_lang</span> - ID codes for character sets to be used to convert to UTF-8 for banned words and DLP on HTTP posts (maximum of 5 character sets). <span class="li-normal">type: list</span> <span class="li-normal">choices: jisx0201, jisx0208, jisx0212, gb2312, ksc5601-ex, euc-jp, sjis, iso2022-jp, iso2022-jp-1, iso2022-jp-2, euc-cn, ces-gbk, hz, ces-big5, euc-kr, iso2022-jp-3, iso8859-1, tis620, cp874, cp1252, cp1251</span>
 <a id='label98' href="javascript:ContentClick('label99', 'label98');" onmouseover="ContentPreview('label99');" onmouseout="ContentUnpreview('label99');" title="click to collapse or expand..."> more... </a>
 <div id="label99" style="display:none">
 <table border="1">
 <tr>
 <td></td>
 <td colspan="1">Supported Version Ranges</td>
 </tr>
 <tr>
 <td>post_lang</td>
 <td><code class="docutils literal notranslate">v6.0.0 -> latest </code></td>
 </tr>
 <tr>
 <td>[jisx0201]</td>
 <td><code class="docutils literal notranslate">v6.0.0 -> latest</code></td> <tr>
 <td>[jisx0208]</td>
 <td><code class="docutils literal notranslate">v6.0.0 -> latest</code></td> <tr>
 <td>[jisx0212]</td>
 <td><code class="docutils literal notranslate">v6.0.0 -> latest</code></td> <tr>
 <td>[gb2312]</td>
 <td><code class="docutils literal notranslate">v6.0.0 -> latest</code></td> <tr>
 <td>[ksc5601-ex]</td>
 <td><code class="docutils literal notranslate">v6.0.0 -> latest</code></td> <tr>
 <td>[euc-jp]</td>
 <td><code class="docutils literal notranslate">v6.0.0 -> latest</code></td> <tr>
 <td>[sjis]</td>
 <td><code class="docutils literal notranslate">v6.0.0 -> latest</code></td> <tr>
 <td>[iso2022-jp]</td>
 <td><code class="docutils literal notranslate">v6.0.0 -> latest</code></td> <tr>
 <td>[iso2022-jp-1]</td>
 <td><code class="docutils literal notranslate">v6.0.0 -> latest</code></td> <tr>
 <td>[iso2022-jp-2]</td>
 <td><code class="docutils literal notranslate">v6.0.0 -> latest</code></td> <tr>
 <td>[euc-cn]</td>
 <td><code class="docutils literal notranslate">v6.0.0 -> latest</code></td> <tr>
 <td>[ces-gbk]</td>
 <td><code class="docutils literal notranslate">v6.0.0 -> latest</code></td> <tr>
 <td>[hz]</td>
 <td><code class="docutils literal notranslate">v6.0.0 -> latest</code></td> <tr>
 <td>[ces-big5]</td>
 <td><code class="docutils literal notranslate">v6.0.0 -> latest</code></td> <tr>
 <td>[euc-kr]</td>
 <td><code class="docutils literal notranslate">v6.0.0 -> latest</code></td> <tr>
 <td>[iso2022-jp-3]</td>
 <td><code class="docutils literal notranslate">v6.0.0 -> latest</code></td> <tr>
 <td>[iso8859-1]</td>
 <td><code class="docutils literal notranslate">v6.0.0 -> latest</code></td> <tr>
 <td>[tis620]</td>
 <td><code class="docutils literal notranslate">v6.0.0 -> latest</code></td> <tr>
 <td>[cp874]</td>
 <td><code class="docutils literal notranslate">v6.0.0 -> latest</code></td> <tr>
 <td>[cp1252]</td>
 <td><code class="docutils literal notranslate">v6.0.0 -> latest</code></td> <tr>
 <td>[cp1251]</td>
 <td><code class="docutils literal notranslate">v6.0.0 -> latest</code></td> </table>
 </div>
 </li>
            <li> <span class="li-head">proxy_after_tcp_handshake</span> - Proxy traffic after the TCP 3-way handshake has been established (not before). <span class="li-normal">type: str</span> <span class="li-normal">choices: enable, disable</span>
 <a id='label100' href="javascript:ContentClick('label101', 'label100');" onmouseover="ContentPreview('label101');" onmouseout="ContentUnpreview('label101');" title="click to collapse or expand..."> more... </a>
 <div id="label101" style="display:none">
 <table border="1">
 <tr>
 <td></td>
 <td colspan="1">Supported Version Ranges</td>
 </tr>
 <tr>
 <td>proxy_after_tcp_handshake</td>
 <td><code class="docutils literal notranslate">v6.4.0 -> latest </code></td>
 </tr>
 <tr>
 <td>[enable]</td>
 <td><code class="docutils literal notranslate">v6.0.0 -> latest</code></td> <tr>
 <td>[disable]</td>
 <td><code class="docutils literal notranslate">v6.0.0 -> latest</code></td> </table>
 </div>
 </li>
            <li> <span class="li-head">range_block</span> - Enable/disable blocking of partial downloads. <span class="li-normal">type: str</span> <span class="li-normal">choices: disable, enable</span>
 <a id='label102' href="javascript:ContentClick('label103', 'label102');" onmouseover="ContentPreview('label103');" onmouseout="ContentUnpreview('label103');" title="click to collapse or expand..."> more... </a>
 <div id="label103" style="display:none">
 <table border="1">
 <tr>
 <td></td>
 <td colspan="1">Supported Version Ranges</td>
 </tr>
 <tr>
 <td>range_block</td>
 <td><code class="docutils literal notranslate">v6.0.0 -> latest </code></td>
 </tr>
 <tr>
 <td>[disable]</td>
 <td><code class="docutils literal notranslate">v6.0.0 -> latest</code></td> <tr>
 <td>[enable]</td>
 <td><code class="docutils literal notranslate">v6.0.0 -> latest</code></td> </table>
 </div>
 </li>
            <li> <span class="li-head">retry_count</span> - Number of attempts to retry HTTP connection (0 - 100). <span class="li-normal">type: int</span>
 <a id='label104' href="javascript:ContentClick('label105', 'label104');" onmouseover="ContentPreview('label105');" onmouseout="ContentUnpreview('label105');" title="click to collapse or expand..."> more... </a>
 <div id="label105" style="display:none">
 <table border="1">
 <tr>
 <td></td>
 <td colspan="1">Supported Version Ranges</td>
 </tr>
 <tr>
 <td>retry_count</td>
 <td><code class="docutils literal notranslate">v6.0.0 -> latest </code></td>
 </tr>
 </table>
 </div>
 </li>
            <li> <span class="li-head">scan_bzip2</span> - Enable/disable scanning of BZip2 compressed files. <span class="li-normal">type: str</span> <span class="li-normal">choices: enable, disable</span>
 <a id='label106' href="javascript:ContentClick('label107', 'label106');" onmouseover="ContentPreview('label107');" onmouseout="ContentUnpreview('label107');" title="click to collapse or expand..."> more... </a>
 <div id="label107" style="display:none">
 <table border="1">
 <tr>
 <td></td>
 <td colspan="1">Supported Version Ranges</td>
 </tr>
 <tr>
 <td>scan_bzip2</td>
 <td><code class="docutils literal notranslate">v6.0.0 -> latest </code></td>
 </tr>
 <tr>
 <td>[enable]</td>
 <td><code class="docutils literal notranslate">v6.0.0 -> latest</code></td> <tr>
 <td>[disable]</td>
 <td><code class="docutils literal notranslate">v6.0.0 -> latest</code></td> </table>
 </div>
 </li>
            <li> <span class="li-head">ssl_offloaded</span> - SSL decryption and encryption performed by an external device. <span class="li-normal">type: str</span> <span class="li-normal">choices: no, yes</span>
 <a id='label108' href="javascript:ContentClick('label109', 'label108');" onmouseover="ContentPreview('label109');" onmouseout="ContentUnpreview('label109');" title="click to collapse or expand..."> more... </a>
 <div id="label109" style="display:none">
 <table border="1">
 <tr>
 <td></td>
 <td colspan="1">Supported Version Ranges</td>
 </tr>
 <tr>
 <td>ssl_offloaded</td>
 <td><code class="docutils literal notranslate">v6.2.0 -> latest </code></td>
 </tr>
 <tr>
 <td>[no]</td>
 <td><code class="docutils literal notranslate">v6.0.0 -> latest</code></td> <tr>
 <td>[yes]</td>
 <td><code class="docutils literal notranslate">v6.0.0 -> latest</code></td> </table>
 </div>
 </li>
            <li> <span class="li-head">status</span> - Enable/disable the active status of scanning for this protocol. <span class="li-normal">type: str</span> <span class="li-normal">choices: enable, disable</span>
 <a id='label110' href="javascript:ContentClick('label111', 'label110');" onmouseover="ContentPreview('label111');" onmouseout="ContentUnpreview('label111');" title="click to collapse or expand..."> more... </a>
 <div id="label111" style="display:none">
 <table border="1">
 <tr>
 <td></td>
 <td colspan="1">Supported Version Ranges</td>
 </tr>
 <tr>
 <td>status</td>
 <td><code class="docutils literal notranslate">v6.0.0 -> latest </code></td>
 </tr>
 <tr>
 <td>[enable]</td>
 <td><code class="docutils literal notranslate">v6.0.0 -> latest</code></td> <tr>
 <td>[disable]</td>
 <td><code class="docutils literal notranslate">v6.0.0 -> latest</code></td> </table>
 </div>
 </li>
            <li> <span class="li-head">stream_based_uncompressed_limit</span> - Maximum stream-based uncompressed data size that will be scanned in megabytes. Stream-based uncompression used only under certain conditions (unlimited = 0). <span class="li-normal">type: int</span>
 <a id='label112' href="javascript:ContentClick('label113', 'label112');" onmouseover="ContentPreview('label113');" onmouseout="ContentUnpreview('label113');" title="click to collapse or expand..."> more... </a>
 <div id="label113" style="display:none">
 <table border="1">
 <tr>
 <td></td>
 <td colspan="1">Supported Version Ranges</td>
 </tr>
 <tr>
 <td>stream_based_uncompressed_limit</td>
 <td><code class="docutils literal notranslate">v6.2.0 -> latest </code></td>
 </tr>
 </table>
 </div>
 </li>
            <li> <span class="li-head">streaming_content_bypass</span> - Enable/disable bypassing of streaming content from buffering. <span class="li-normal">type: str</span> <span class="li-normal">choices: enable, disable</span>
 <a id='label114' href="javascript:ContentClick('label115', 'label114');" onmouseover="ContentPreview('label115');" onmouseout="ContentUnpreview('label115');" title="click to collapse or expand..."> more... </a>
 <div id="label115" style="display:none">
 <table border="1">
 <tr>
 <td></td>
 <td colspan="1">Supported Version Ranges</td>
 </tr>
 <tr>
 <td>streaming_content_bypass</td>
 <td><code class="docutils literal notranslate">v6.0.0 -> latest </code></td>
 </tr>
 <tr>
 <td>[enable]</td>
 <td><code class="docutils literal notranslate">v6.0.0 -> latest</code></td> <tr>
 <td>[disable]</td>
 <td><code class="docutils literal notranslate">v6.0.0 -> latest</code></td> </table>
 </div>
 </li>
            <li> <span class="li-head">strip_x_forwarded_for</span> - Enable/disable stripping of HTTP X-Forwarded-For header. <span class="li-normal">type: str</span> <span class="li-normal">choices: disable, enable</span>
 <a id='label116' href="javascript:ContentClick('label117', 'label116');" onmouseover="ContentPreview('label117');" onmouseout="ContentUnpreview('label117');" title="click to collapse or expand..."> more... </a>
 <div id="label117" style="display:none">
 <table border="1">
 <tr>
 <td></td>
 <td colspan="1">Supported Version Ranges</td>
 </tr>
 <tr>
 <td>strip_x_forwarded_for</td>
 <td><code class="docutils literal notranslate">v6.0.0 -> latest </code></td>
 </tr>
 <tr>
 <td>[disable]</td>
 <td><code class="docutils literal notranslate">v6.0.0 -> latest</code></td> <tr>
 <td>[enable]</td>
 <td><code class="docutils literal notranslate">v6.0.0 -> latest</code></td> </table>
 </div>
 </li>
            <li> <span class="li-head">switching_protocols</span> - Bypass from scanning, or block a connection that attempts to switch protocol. <span class="li-normal">type: str</span> <span class="li-normal">choices: bypass, block</span>
 <a id='label118' href="javascript:ContentClick('label119', 'label118');" onmouseover="ContentPreview('label119');" onmouseout="ContentUnpreview('label119');" title="click to collapse or expand..."> more... </a>
 <div id="label119" style="display:none">
 <table border="1">
 <tr>
 <td></td>
 <td colspan="1">Supported Version Ranges</td>
 </tr>
 <tr>
 <td>switching_protocols</td>
 <td><code class="docutils literal notranslate">v6.0.0 -> latest </code></td>
 </tr>
 <tr>
 <td>[bypass]</td>
 <td><code class="docutils literal notranslate">v6.0.0 -> latest</code></td> <tr>
 <td>[block]</td>
 <td><code class="docutils literal notranslate">v6.0.0 -> latest</code></td> </table>
 </div>
 </li>
            <li> <span class="li-head">tcp_window_maximum</span> - Maximum dynamic TCP window size. <span class="li-normal">type: int</span>
 <a id='label120' href="javascript:ContentClick('label121', 'label120');" onmouseover="ContentPreview('label121');" onmouseout="ContentUnpreview('label121');" title="click to collapse or expand..."> more... </a>
 <div id="label121" style="display:none">
 <table border="1">
 <tr>
 <td></td>
 <td colspan="1">Supported Version Ranges</td>
 </tr>
 <tr>
 <td>tcp_window_maximum</td>
 <td><code class="docutils literal notranslate">v6.2.0 -> latest </code></td>
 </tr>
 </table>
 </div>
 </li>
            <li> <span class="li-head">tcp_window_minimum</span> - Minimum dynamic TCP window size. <span class="li-normal">type: int</span>
 <a id='label122' href="javascript:ContentClick('label123', 'label122');" onmouseover="ContentPreview('label123');" onmouseout="ContentUnpreview('label123');" title="click to collapse or expand..."> more... </a>
 <div id="label123" style="display:none">
 <table border="1">
 <tr>
 <td></td>
 <td colspan="1">Supported Version Ranges</td>
 </tr>
 <tr>
 <td>tcp_window_minimum</td>
 <td><code class="docutils literal notranslate">v6.2.0 -> latest </code></td>
 </tr>
 </table>
 </div>
 </li>
            <li> <span class="li-head">tcp_window_size</span> - Set TCP static window size. <span class="li-normal">type: int</span>
 <a id='label124' href="javascript:ContentClick('label125', 'label124');" onmouseover="ContentPreview('label125');" onmouseout="ContentUnpreview('label125');" title="click to collapse or expand..."> more... </a>
 <div id="label125" style="display:none">
 <table border="1">
 <tr>
 <td></td>
 <td colspan="1">Supported Version Ranges</td>
 </tr>
 <tr>
 <td>tcp_window_size</td>
 <td><code class="docutils literal notranslate">v6.2.0 -> latest </code></td>
 </tr>
 </table>
 </div>
 </li>
            <li> <span class="li-head">tcp_window_type</span> - TCP window type to use for this protocol. <span class="li-normal">type: str</span> <span class="li-normal">choices: auto-tuning, system, static, dynamic</span>
 <a id='label126' href="javascript:ContentClick('label127', 'label126');" onmouseover="ContentPreview('label127');" onmouseout="ContentUnpreview('label127');" title="click to collapse or expand..."> more... </a>
 <div id="label127" style="display:none">
 <table border="1">
 <tr>
 <td></td>
 <td colspan="1">Supported Version Ranges</td>
 </tr>
 <tr>
 <td>tcp_window_type</td>
 <td><code class="docutils literal notranslate">v6.2.0 -> latest </code></td>
 </tr>
 <tr>
 <td>[auto-tuning]</td>
 <td><code class="docutils literal notranslate">v7.0.4 -> latest</code></td>
 </tr>
 <tr>
 <td>[system]</td>
 <td><code class="docutils literal notranslate">v6.0.0 -> latest</code></td> <tr>
 <td>[static]</td>
 <td><code class="docutils literal notranslate">v6.0.0 -> latest</code></td> <tr>
 <td>[dynamic]</td>
 <td><code class="docutils literal notranslate">v6.0.0 -> latest</code></td> </table>
 </div>
 </li>
            <li> <span class="li-head">tunnel_non_http</span> - Configure how to process non-HTTP traffic when a profile configured for HTTP traffic accepts a non-HTTP session. Can occur if an application sends non-HTTP traffic using an HTTP destination port. <span class="li-normal">type: str</span> <span class="li-normal">choices: enable, disable</span>
 <a id='label128' href="javascript:ContentClick('label129', 'label128');" onmouseover="ContentPreview('label129');" onmouseout="ContentUnpreview('label129');" title="click to collapse or expand..."> more... </a>
 <div id="label129" style="display:none">
 <table border="1">
 <tr>
 <td></td>
 <td colspan="1">Supported Version Ranges</td>
 </tr>
 <tr>
 <td>tunnel_non_http</td>
 <td><code class="docutils literal notranslate">v6.4.0 -> latest </code></td>
 </tr>
 <tr>
 <td>[enable]</td>
 <td><code class="docutils literal notranslate">v6.0.0 -> latest</code></td> <tr>
 <td>[disable]</td>
 <td><code class="docutils literal notranslate">v6.0.0 -> latest</code></td> </table>
 </div>
 </li>
            <li> <span class="li-head">uncompressed_nest_limit</span> - Maximum nested levels of compression that can be uncompressed and scanned (2 - 100). <span class="li-normal">type: int</span>
 <a id='label130' href="javascript:ContentClick('label131', 'label130');" onmouseover="ContentPreview('label131');" onmouseout="ContentUnpreview('label131');" title="click to collapse or expand..."> more... </a>
 <div id="label131" style="display:none">
 <table border="1">
 <tr>
 <td></td>
 <td colspan="1">Supported Version Ranges</td>
 </tr>
 <tr>
 <td>uncompressed_nest_limit</td>
 <td><code class="docutils literal notranslate">v6.0.0 -> latest </code></td>
 </tr>
 </table>
 </div>
 </li>
            <li> <span class="li-head">uncompressed_oversize_limit</span> - Maximum in-memory uncompressed file size that can be scanned. <span class="li-normal">type: int</span>
 <a id='label132' href="javascript:ContentClick('label133', 'label132');" onmouseover="ContentPreview('label133');" onmouseout="ContentUnpreview('label133');" title="click to collapse or expand..."> more... </a>
 <div id="label133" style="display:none">
 <table border="1">
 <tr>
 <td></td>
 <td colspan="1">Supported Version Ranges</td>
 </tr>
 <tr>
 <td>uncompressed_oversize_limit</td>
 <td><code class="docutils literal notranslate">v6.0.0 -> latest </code></td>
 </tr>
 </table>
 </div>
 </li>
            <li> <span class="li-head">unknown_content_encoding</span> - Configure the action the FortiGate unit will take on unknown content-encoding. <span class="li-normal">type: str</span> <span class="li-normal">choices: block, inspect, bypass</span>
 <a id='label134' href="javascript:ContentClick('label135', 'label134');" onmouseover="ContentPreview('label135');" onmouseout="ContentUnpreview('label135');" title="click to collapse or expand..."> more... </a>
 <div id="label135" style="display:none">
 <table border="1">
 <tr>
 <td></td>
 <td colspan="1">Supported Version Ranges</td>
 </tr>
 <tr>
 <td>unknown_content_encoding</td>
 <td><code class="docutils literal notranslate">v7.2.4 -> latest </code></td>
 </tr>
 <tr>
 <td>[block]</td>
 <td><code class="docutils literal notranslate">v6.0.0 -> latest</code></td> <tr>
 <td>[inspect]</td>
 <td><code class="docutils literal notranslate">v6.0.0 -> latest</code></td> <tr>
 <td>[bypass]</td>
 <td><code class="docutils literal notranslate">v6.0.0 -> latest</code></td> </table>
 </div>
 </li>
            <li> <span class="li-head">unknown_http_version</span> - How to handle HTTP sessions that do not comply with HTTP 0.9, 1.0, or 1.1. <span class="li-normal">type: str</span> <span class="li-normal">choices: reject, tunnel, best-effort</span>
 <a id='label136' href="javascript:ContentClick('label137', 'label136');" onmouseover="ContentPreview('label137');" onmouseout="ContentUnpreview('label137');" title="click to collapse or expand..."> more... </a>
 <div id="label137" style="display:none">
 <table border="1">
 <tr>
 <td></td>
 <td colspan="1">Supported Version Ranges</td>
 </tr>
 <tr>
 <td>unknown_http_version</td>
 <td><code class="docutils literal notranslate">v6.4.0 -> latest </code></td>
 </tr>
 <tr>
 <td>[reject]</td>
 <td><code class="docutils literal notranslate">v6.0.0 -> latest</code></td> <tr>
 <td>[tunnel]</td>
 <td><code class="docutils literal notranslate">v6.0.0 -> latest</code></td> <tr>
 <td>[best-effort]</td>
 <td><code class="docutils literal notranslate">v6.0.0 -> latest</code></td> </table>
 </div>
 </li>
            <li> <span class="li-head">verify_dns_for_policy_matching</span> - Enable/disable verification of DNS for policy matching. <span class="li-normal">type: str</span> <span class="li-normal">choices: enable, disable</span>
 <a id='label138' href="javascript:ContentClick('label139', 'label138');" onmouseover="ContentPreview('label139');" onmouseout="ContentUnpreview('label139');" title="click to collapse or expand..."> more... </a>
 <div id="label139" style="display:none">
 <table border="1">
 <tr>
 <td></td>
 <td colspan="1">Supported Version Ranges</td>
 </tr>
 <tr>
 <td>verify_dns_for_policy_matching</td>
 <td><code class="docutils literal notranslate">v7.2.1 -> latest </code></td>
 </tr>
 <tr>
 <td>[enable]</td>
 <td><code class="docutils literal notranslate">v6.0.0 -> latest</code></td> <tr>
 <td>[disable]</td>
 <td><code class="docutils literal notranslate">v6.0.0 -> latest</code></td> </table>
 </div>
 </li>
            </ul>
        <li> <span class="li-head">imap</span> - Configure IMAP protocol options. <span class="li-normal">type: dict</span>
 <a id='label140' href="javascript:ContentClick('label141', 'label140');" onmouseover="ContentPreview('label141');" onmouseout="ContentUnpreview('label141');" title="click to collapse or expand..."> more... </a>
 <div id="label141" style="display:none">
 <table border="1">
 <tr>
 <td></td><td colspan="1">Supported Version Ranges</td>
 </tr>
 <tr>
 <td>imap</td>
 <td><code class="docutils literal notranslate">v6.0.0 -> latest </code></td>
 </tr>
 </table>
 </div>
 </li>
            <ul class="ul-self">
            <li> <span class="li-head">inspect_all</span> - Enable/disable the inspection of all ports for the protocol. <span class="li-normal">type: str</span> <span class="li-normal">choices: enable, disable</span>
 <a id='label142' href="javascript:ContentClick('label143', 'label142');" onmouseover="ContentPreview('label143');" onmouseout="ContentUnpreview('label143');" title="click to collapse or expand..."> more... </a>
 <div id="label143" style="display:none">
 <table border="1">
 <tr>
 <td></td>
 <td colspan="1">Supported Version Ranges</td>
 </tr>
 <tr>
 <td>inspect_all</td>
 <td><code class="docutils literal notranslate">v6.0.0 -> latest </code></td>
 </tr>
 <tr>
 <td>[enable]</td>
 <td><code class="docutils literal notranslate">v6.0.0 -> latest</code></td> <tr>
 <td>[disable]</td>
 <td><code class="docutils literal notranslate">v6.0.0 -> latest</code></td> </table>
 </div>
 </li>
            <li> <span class="li-head">options</span> - One or more options that can be applied to the session. <span class="li-normal">type: list</span> <span class="li-normal">choices: fragmail, oversize</span>
 <a id='label144' href="javascript:ContentClick('label145', 'label144');" onmouseover="ContentPreview('label145');" onmouseout="ContentUnpreview('label145');" title="click to collapse or expand..."> more... </a>
 <div id="label145" style="display:none">
 <table border="1">
 <tr>
 <td></td>
 <td colspan="1">Supported Version Ranges</td>
 </tr>
 <tr>
 <td>options</td>
 <td><code class="docutils literal notranslate">v6.0.0 -> latest </code></td>
 </tr>
 <tr>
 <td>[fragmail]</td>
 <td><code class="docutils literal notranslate">v6.0.0 -> latest</code></td> <tr>
 <td>[oversize]</td>
 <td><code class="docutils literal notranslate">v6.0.0 -> latest</code></td> </table>
 </div>
 </li>
            <li> <span class="li-head">oversize_limit</span> - Maximum in-memory file size that can be scanned (MB). <span class="li-normal">type: int</span>
 <a id='label146' href="javascript:ContentClick('label147', 'label146');" onmouseover="ContentPreview('label147');" onmouseout="ContentUnpreview('label147');" title="click to collapse or expand..."> more... </a>
 <div id="label147" style="display:none">
 <table border="1">
 <tr>
 <td></td>
 <td colspan="1">Supported Version Ranges</td>
 </tr>
 <tr>
 <td>oversize_limit</td>
 <td><code class="docutils literal notranslate">v6.0.0 -> latest </code></td>
 </tr>
 </table>
 </div>
 </li>
            <li> <span class="li-head">ports</span> - Ports to scan for content (1 - 65535). <span class="li-normal">type: list</span> </li>
            <li> <span class="li-head">proxy_after_tcp_handshake</span> - Proxy traffic after the TCP 3-way handshake has been established (not before). <span class="li-normal">type: str</span> <span class="li-normal">choices: enable, disable</span>
 <a id='label148' href="javascript:ContentClick('label149', 'label148');" onmouseover="ContentPreview('label149');" onmouseout="ContentUnpreview('label149');" title="click to collapse or expand..."> more... </a>
 <div id="label149" style="display:none">
 <table border="1">
 <tr>
 <td></td>
 <td colspan="1">Supported Version Ranges</td>
 </tr>
 <tr>
 <td>proxy_after_tcp_handshake</td>
 <td><code class="docutils literal notranslate">v6.4.0 -> latest </code></td>
 </tr>
 <tr>
 <td>[enable]</td>
 <td><code class="docutils literal notranslate">v6.0.0 -> latest</code></td> <tr>
 <td>[disable]</td>
 <td><code class="docutils literal notranslate">v6.0.0 -> latest</code></td> </table>
 </div>
 </li>
            <li> <span class="li-head">scan_bzip2</span> - Enable/disable scanning of BZip2 compressed files. <span class="li-normal">type: str</span> <span class="li-normal">choices: enable, disable</span>
 <a id='label150' href="javascript:ContentClick('label151', 'label150');" onmouseover="ContentPreview('label151');" onmouseout="ContentUnpreview('label151');" title="click to collapse or expand..."> more... </a>
 <div id="label151" style="display:none">
 <table border="1">
 <tr>
 <td></td>
 <td colspan="1">Supported Version Ranges</td>
 </tr>
 <tr>
 <td>scan_bzip2</td>
 <td><code class="docutils literal notranslate">v6.0.0 -> latest </code></td>
 </tr>
 <tr>
 <td>[enable]</td>
 <td><code class="docutils literal notranslate">v6.0.0 -> latest</code></td> <tr>
 <td>[disable]</td>
 <td><code class="docutils literal notranslate">v6.0.0 -> latest</code></td> </table>
 </div>
 </li>
            <li> <span class="li-head">ssl_offloaded</span> - SSL decryption and encryption performed by an external device. <span class="li-normal">type: str</span> <span class="li-normal">choices: no, yes</span>
 <a id='label152' href="javascript:ContentClick('label153', 'label152');" onmouseover="ContentPreview('label153');" onmouseout="ContentUnpreview('label153');" title="click to collapse or expand..."> more... </a>
 <div id="label153" style="display:none">
 <table border="1">
 <tr>
 <td></td>
 <td colspan="1">Supported Version Ranges</td>
 </tr>
 <tr>
 <td>ssl_offloaded</td>
 <td><code class="docutils literal notranslate">v6.2.0 -> latest </code></td>
 </tr>
 <tr>
 <td>[no]</td>
 <td><code class="docutils literal notranslate">v6.0.0 -> latest</code></td> <tr>
 <td>[yes]</td>
 <td><code class="docutils literal notranslate">v6.0.0 -> latest</code></td> </table>
 </div>
 </li>
            <li> <span class="li-head">status</span> - Enable/disable the active status of scanning for this protocol. <span class="li-normal">type: str</span> <span class="li-normal">choices: enable, disable</span>
 <a id='label154' href="javascript:ContentClick('label155', 'label154');" onmouseover="ContentPreview('label155');" onmouseout="ContentUnpreview('label155');" title="click to collapse or expand..."> more... </a>
 <div id="label155" style="display:none">
 <table border="1">
 <tr>
 <td></td>
 <td colspan="1">Supported Version Ranges</td>
 </tr>
 <tr>
 <td>status</td>
 <td><code class="docutils literal notranslate">v6.0.0 -> latest </code></td>
 </tr>
 <tr>
 <td>[enable]</td>
 <td><code class="docutils literal notranslate">v6.0.0 -> latest</code></td> <tr>
 <td>[disable]</td>
 <td><code class="docutils literal notranslate">v6.0.0 -> latest</code></td> </table>
 </div>
 </li>
            <li> <span class="li-head">uncompressed_nest_limit</span> - Maximum nested levels of compression that can be uncompressed and scanned (2 - 100). <span class="li-normal">type: int</span>
 <a id='label156' href="javascript:ContentClick('label157', 'label156');" onmouseover="ContentPreview('label157');" onmouseout="ContentUnpreview('label157');" title="click to collapse or expand..."> more... </a>
 <div id="label157" style="display:none">
 <table border="1">
 <tr>
 <td></td>
 <td colspan="1">Supported Version Ranges</td>
 </tr>
 <tr>
 <td>uncompressed_nest_limit</td>
 <td><code class="docutils literal notranslate">v6.0.0 -> latest </code></td>
 </tr>
 </table>
 </div>
 </li>
            <li> <span class="li-head">uncompressed_oversize_limit</span> - Maximum in-memory uncompressed file size that can be scanned. <span class="li-normal">type: int</span>
 <a id='label158' href="javascript:ContentClick('label159', 'label158');" onmouseover="ContentPreview('label159');" onmouseout="ContentUnpreview('label159');" title="click to collapse or expand..."> more... </a>
 <div id="label159" style="display:none">
 <table border="1">
 <tr>
 <td></td>
 <td colspan="1">Supported Version Ranges</td>
 </tr>
 <tr>
 <td>uncompressed_oversize_limit</td>
 <td><code class="docutils literal notranslate">v6.0.0 -> latest </code></td>
 </tr>
 </table>
 </div>
 </li>
            </ul>
        <li> <span class="li-head">mail_signature</span> - Configure Mail signature. <span class="li-normal">type: dict</span>
 <a id='label160' href="javascript:ContentClick('label161', 'label160');" onmouseover="ContentPreview('label161');" onmouseout="ContentUnpreview('label161');" title="click to collapse or expand..."> more... </a>
 <div id="label161" style="display:none">
 <table border="1">
 <tr>
 <td></td><td colspan="1">Supported Version Ranges</td>
 </tr>
 <tr>
 <td>mail_signature</td>
 <td><code class="docutils literal notranslate">v6.0.0 -> latest </code></td>
 </tr>
 </table>
 </div>
 </li>
            <ul class="ul-self">
            <li> <span class="li-head">signature</span> - Email signature to be added to outgoing email (if the signature contains spaces, enclose with quotation marks). <span class="li-normal">type: str</span>
 <a id='label162' href="javascript:ContentClick('label163', 'label162');" onmouseover="ContentPreview('label163');" onmouseout="ContentUnpreview('label163');" title="click to collapse or expand..."> more... </a>
 <div id="label163" style="display:none">
 <table border="1">
 <tr>
 <td></td>
 <td colspan="1">Supported Version Ranges</td>
 </tr>
 <tr>
 <td>signature</td>
 <td><code class="docutils literal notranslate">v6.0.0 -> latest </code></td>
 </tr>
 </table>
 </div>
 </li>
            <li> <span class="li-head">status</span> - Enable/disable adding an email signature to SMTP email messages as they pass through the FortiGate. <span class="li-normal">type: str</span> <span class="li-normal">choices: disable, enable</span>
 <a id='label164' href="javascript:ContentClick('label165', 'label164');" onmouseover="ContentPreview('label165');" onmouseout="ContentUnpreview('label165');" title="click to collapse or expand..."> more... </a>
 <div id="label165" style="display:none">
 <table border="1">
 <tr>
 <td></td>
 <td colspan="1">Supported Version Ranges</td>
 </tr>
 <tr>
 <td>status</td>
 <td><code class="docutils literal notranslate">v6.0.0 -> latest </code></td>
 </tr>
 <tr>
 <td>[disable]</td>
 <td><code class="docutils literal notranslate">v6.0.0 -> latest</code></td> <tr>
 <td>[enable]</td>
 <td><code class="docutils literal notranslate">v6.0.0 -> latest</code></td> </table>
 </div>
 </li>
            </ul>
        <li> <span class="li-head">mapi</span> - Configure MAPI protocol options. <span class="li-normal">type: dict</span>
 <a id='label166' href="javascript:ContentClick('label167', 'label166');" onmouseover="ContentPreview('label167');" onmouseout="ContentUnpreview('label167');" title="click to collapse or expand..."> more... </a>
 <div id="label167" style="display:none">
 <table border="1">
 <tr>
 <td></td><td colspan="1">Supported Version Ranges</td>
 </tr>
 <tr>
 <td>mapi</td>
 <td><code class="docutils literal notranslate">v6.0.0 -> latest </code></td>
 </tr>
 </table>
 </div>
 </li>
            <ul class="ul-self">
            <li> <span class="li-head">options</span> - One or more options that can be applied to the session. <span class="li-normal">type: list</span> <span class="li-normal">choices: fragmail, oversize</span>
 <a id='label168' href="javascript:ContentClick('label169', 'label168');" onmouseover="ContentPreview('label169');" onmouseout="ContentUnpreview('label169');" title="click to collapse or expand..."> more... </a>
 <div id="label169" style="display:none">
 <table border="1">
 <tr>
 <td></td>
 <td colspan="1">Supported Version Ranges</td>
 </tr>
 <tr>
 <td>options</td>
 <td><code class="docutils literal notranslate">v6.0.0 -> latest </code></td>
 </tr>
 <tr>
 <td>[fragmail]</td>
 <td><code class="docutils literal notranslate">v6.0.0 -> latest</code></td> <tr>
 <td>[oversize]</td>
 <td><code class="docutils literal notranslate">v6.0.0 -> latest</code></td> </table>
 </div>
 </li>
            <li> <span class="li-head">oversize_limit</span> - Maximum in-memory file size that can be scanned (MB). <span class="li-normal">type: int</span>
 <a id='label170' href="javascript:ContentClick('label171', 'label170');" onmouseover="ContentPreview('label171');" onmouseout="ContentUnpreview('label171');" title="click to collapse or expand..."> more... </a>
 <div id="label171" style="display:none">
 <table border="1">
 <tr>
 <td></td>
 <td colspan="1">Supported Version Ranges</td>
 </tr>
 <tr>
 <td>oversize_limit</td>
 <td><code class="docutils literal notranslate">v6.0.0 -> latest </code></td>
 </tr>
 </table>
 </div>
 </li>
            <li> <span class="li-head">ports</span> - Ports to scan for content (1 - 65535). <span class="li-normal">type: list</span> </li>
            <li> <span class="li-head">scan_bzip2</span> - Enable/disable scanning of BZip2 compressed files. <span class="li-normal">type: str</span> <span class="li-normal">choices: enable, disable</span>
 <a id='label172' href="javascript:ContentClick('label173', 'label172');" onmouseover="ContentPreview('label173');" onmouseout="ContentUnpreview('label173');" title="click to collapse or expand..."> more... </a>
 <div id="label173" style="display:none">
 <table border="1">
 <tr>
 <td></td>
 <td colspan="1">Supported Version Ranges</td>
 </tr>
 <tr>
 <td>scan_bzip2</td>
 <td><code class="docutils literal notranslate">v6.0.0 -> latest </code></td>
 </tr>
 <tr>
 <td>[enable]</td>
 <td><code class="docutils literal notranslate">v6.0.0 -> latest</code></td> <tr>
 <td>[disable]</td>
 <td><code class="docutils literal notranslate">v6.0.0 -> latest</code></td> </table>
 </div>
 </li>
            <li> <span class="li-head">status</span> - Enable/disable the active status of scanning for this protocol. <span class="li-normal">type: str</span> <span class="li-normal">choices: enable, disable</span>
 <a id='label174' href="javascript:ContentClick('label175', 'label174');" onmouseover="ContentPreview('label175');" onmouseout="ContentUnpreview('label175');" title="click to collapse or expand..."> more... </a>
 <div id="label175" style="display:none">
 <table border="1">
 <tr>
 <td></td>
 <td colspan="1">Supported Version Ranges</td>
 </tr>
 <tr>
 <td>status</td>
 <td><code class="docutils literal notranslate">v6.0.0 -> latest </code></td>
 </tr>
 <tr>
 <td>[enable]</td>
 <td><code class="docutils literal notranslate">v6.0.0 -> latest</code></td> <tr>
 <td>[disable]</td>
 <td><code class="docutils literal notranslate">v6.0.0 -> latest</code></td> </table>
 </div>
 </li>
            <li> <span class="li-head">uncompressed_nest_limit</span> - Maximum nested levels of compression that can be uncompressed and scanned (2 - 100). <span class="li-normal">type: int</span>
 <a id='label176' href="javascript:ContentClick('label177', 'label176');" onmouseover="ContentPreview('label177');" onmouseout="ContentUnpreview('label177');" title="click to collapse or expand..."> more... </a>
 <div id="label177" style="display:none">
 <table border="1">
 <tr>
 <td></td>
 <td colspan="1">Supported Version Ranges</td>
 </tr>
 <tr>
 <td>uncompressed_nest_limit</td>
 <td><code class="docutils literal notranslate">v6.0.0 -> latest </code></td>
 </tr>
 </table>
 </div>
 </li>
            <li> <span class="li-head">uncompressed_oversize_limit</span> - Maximum in-memory uncompressed file size that can be scanned. <span class="li-normal">type: int</span>
 <a id='label178' href="javascript:ContentClick('label179', 'label178');" onmouseover="ContentPreview('label179');" onmouseout="ContentUnpreview('label179');" title="click to collapse or expand..."> more... </a>
 <div id="label179" style="display:none">
 <table border="1">
 <tr>
 <td></td>
 <td colspan="1">Supported Version Ranges</td>
 </tr>
 <tr>
 <td>uncompressed_oversize_limit</td>
 <td><code class="docutils literal notranslate">v6.0.0 -> latest </code></td>
 </tr>
 </table>
 </div>
 </li>
            </ul>
        <li> <span class="li-head">name</span> - Name. <span class="li-normal">type: str</span> <span class="li-required">required: true</span>
 <a id='label180' href="javascript:ContentClick('label181', 'label180');" onmouseover="ContentPreview('label181');" onmouseout="ContentUnpreview('label181');" title="click to collapse or expand..."> more... </a>
 <div id="label181" style="display:none">
 <table border="1">
 <tr>
 <td></td>
 <td colspan="1">Supported Version Ranges</td>
 </tr>
 <tr>
 <td>name</td>
 <td><code class="docutils literal notranslate">v6.0.0 -> latest </code></td>
 </tr>
 </table>
 </div>
 </li>
        <li> <span class="li-head">nntp</span> - Configure NNTP protocol options. <span class="li-normal">type: dict</span>
 <a id='label182' href="javascript:ContentClick('label183', 'label182');" onmouseover="ContentPreview('label183');" onmouseout="ContentUnpreview('label183');" title="click to collapse or expand..."> more... </a>
 <div id="label183" style="display:none">
 <table border="1">
 <tr>
 <td></td><td colspan="1">Supported Version Ranges</td>
 </tr>
 <tr>
 <td>nntp</td>
 <td><code class="docutils literal notranslate">v6.0.0 -> latest </code></td>
 </tr>
 </table>
 </div>
 </li>
            <ul class="ul-self">
            <li> <span class="li-head">inspect_all</span> - Enable/disable the inspection of all ports for the protocol. <span class="li-normal">type: str</span> <span class="li-normal">choices: enable, disable</span>
 <a id='label184' href="javascript:ContentClick('label185', 'label184');" onmouseover="ContentPreview('label185');" onmouseout="ContentUnpreview('label185');" title="click to collapse or expand..."> more... </a>
 <div id="label185" style="display:none">
 <table border="1">
 <tr>
 <td></td>
 <td colspan="1">Supported Version Ranges</td>
 </tr>
 <tr>
 <td>inspect_all</td>
 <td><code class="docutils literal notranslate">v6.0.0 -> latest </code></td>
 </tr>
 <tr>
 <td>[enable]</td>
 <td><code class="docutils literal notranslate">v6.0.0 -> latest</code></td> <tr>
 <td>[disable]</td>
 <td><code class="docutils literal notranslate">v6.0.0 -> latest</code></td> </table>
 </div>
 </li>
            <li> <span class="li-head">options</span> - One or more options that can be applied to the session. <span class="li-normal">type: list</span> <span class="li-normal">choices: oversize, splice</span>
 <a id='label186' href="javascript:ContentClick('label187', 'label186');" onmouseover="ContentPreview('label187');" onmouseout="ContentUnpreview('label187');" title="click to collapse or expand..."> more... </a>
 <div id="label187" style="display:none">
 <table border="1">
 <tr>
 <td></td>
 <td colspan="1">Supported Version Ranges</td>
 </tr>
 <tr>
 <td>options</td>
 <td><code class="docutils literal notranslate">v6.0.0 -> latest </code></td>
 </tr>
 <tr>
 <td>[oversize]</td>
 <td><code class="docutils literal notranslate">v6.0.0 -> latest</code></td> <tr>
 <td>[splice]</td>
 <td><code class="docutils literal notranslate">v6.0.0 -> latest</code></td> </table>
 </div>
 </li>
            <li> <span class="li-head">oversize_limit</span> - Maximum in-memory file size that can be scanned (MB). <span class="li-normal">type: int</span>
 <a id='label188' href="javascript:ContentClick('label189', 'label188');" onmouseover="ContentPreview('label189');" onmouseout="ContentUnpreview('label189');" title="click to collapse or expand..."> more... </a>
 <div id="label189" style="display:none">
 <table border="1">
 <tr>
 <td></td>
 <td colspan="1">Supported Version Ranges</td>
 </tr>
 <tr>
 <td>oversize_limit</td>
 <td><code class="docutils literal notranslate">v6.0.0 -> latest </code></td>
 </tr>
 </table>
 </div>
 </li>
            <li> <span class="li-head">ports</span> - Ports to scan for content (1 - 65535). <span class="li-normal">type: list</span> </li>
            <li> <span class="li-head">proxy_after_tcp_handshake</span> - Proxy traffic after the TCP 3-way handshake has been established (not before). <span class="li-normal">type: str</span> <span class="li-normal">choices: enable, disable</span>
 <a id='label190' href="javascript:ContentClick('label191', 'label190');" onmouseover="ContentPreview('label191');" onmouseout="ContentUnpreview('label191');" title="click to collapse or expand..."> more... </a>
 <div id="label191" style="display:none">
 <table border="1">
 <tr>
 <td></td>
 <td colspan="1">Supported Version Ranges</td>
 </tr>
 <tr>
 <td>proxy_after_tcp_handshake</td>
 <td><code class="docutils literal notranslate">v6.4.0 -> latest </code></td>
 </tr>
 <tr>
 <td>[enable]</td>
 <td><code class="docutils literal notranslate">v6.0.0 -> latest</code></td> <tr>
 <td>[disable]</td>
 <td><code class="docutils literal notranslate">v6.0.0 -> latest</code></td> </table>
 </div>
 </li>
            <li> <span class="li-head">scan_bzip2</span> - Enable/disable scanning of BZip2 compressed files. <span class="li-normal">type: str</span> <span class="li-normal">choices: enable, disable</span>
 <a id='label192' href="javascript:ContentClick('label193', 'label192');" onmouseover="ContentPreview('label193');" onmouseout="ContentUnpreview('label193');" title="click to collapse or expand..."> more... </a>
 <div id="label193" style="display:none">
 <table border="1">
 <tr>
 <td></td>
 <td colspan="1">Supported Version Ranges</td>
 </tr>
 <tr>
 <td>scan_bzip2</td>
 <td><code class="docutils literal notranslate">v6.0.0 -> latest </code></td>
 </tr>
 <tr>
 <td>[enable]</td>
 <td><code class="docutils literal notranslate">v6.0.0 -> latest</code></td> <tr>
 <td>[disable]</td>
 <td><code class="docutils literal notranslate">v6.0.0 -> latest</code></td> </table>
 </div>
 </li>
            <li> <span class="li-head">status</span> - Enable/disable the active status of scanning for this protocol. <span class="li-normal">type: str</span> <span class="li-normal">choices: enable, disable</span>
 <a id='label194' href="javascript:ContentClick('label195', 'label194');" onmouseover="ContentPreview('label195');" onmouseout="ContentUnpreview('label195');" title="click to collapse or expand..."> more... </a>
 <div id="label195" style="display:none">
 <table border="1">
 <tr>
 <td></td>
 <td colspan="1">Supported Version Ranges</td>
 </tr>
 <tr>
 <td>status</td>
 <td><code class="docutils literal notranslate">v6.0.0 -> latest </code></td>
 </tr>
 <tr>
 <td>[enable]</td>
 <td><code class="docutils literal notranslate">v6.0.0 -> latest</code></td> <tr>
 <td>[disable]</td>
 <td><code class="docutils literal notranslate">v6.0.0 -> latest</code></td> </table>
 </div>
 </li>
            <li> <span class="li-head">uncompressed_nest_limit</span> - Maximum nested levels of compression that can be uncompressed and scanned (2 - 100). <span class="li-normal">type: int</span>
 <a id='label196' href="javascript:ContentClick('label197', 'label196');" onmouseover="ContentPreview('label197');" onmouseout="ContentUnpreview('label197');" title="click to collapse or expand..."> more... </a>
 <div id="label197" style="display:none">
 <table border="1">
 <tr>
 <td></td>
 <td colspan="1">Supported Version Ranges</td>
 </tr>
 <tr>
 <td>uncompressed_nest_limit</td>
 <td><code class="docutils literal notranslate">v6.0.0 -> latest </code></td>
 </tr>
 </table>
 </div>
 </li>
            <li> <span class="li-head">uncompressed_oversize_limit</span> - Maximum in-memory uncompressed file size that can be scanned. <span class="li-normal">type: int</span>
 <a id='label198' href="javascript:ContentClick('label199', 'label198');" onmouseover="ContentPreview('label199');" onmouseout="ContentUnpreview('label199');" title="click to collapse or expand..."> more... </a>
 <div id="label199" style="display:none">
 <table border="1">
 <tr>
 <td></td>
 <td colspan="1">Supported Version Ranges</td>
 </tr>
 <tr>
 <td>uncompressed_oversize_limit</td>
 <td><code class="docutils literal notranslate">v6.0.0 -> latest </code></td>
 </tr>
 </table>
 </div>
 </li>
            </ul>
        <li> <span class="li-head">oversize_log</span> - Enable/disable logging for antivirus oversize file blocking. <span class="li-normal">type: str</span> <span class="li-normal">choices: disable, enable</span>
 <a id='label200' href="javascript:ContentClick('label201', 'label200');" onmouseover="ContentPreview('label201');" onmouseout="ContentUnpreview('label201');" title="click to collapse or expand..."> more... </a>
 <div id="label201" style="display:none">
 <table border="1">
 <tr>
 <td></td>
 <td colspan="1">Supported Version Ranges</td>
 </tr>
 <tr>
 <td>oversize_log</td>
 <td><code class="docutils literal notranslate">v6.0.0 -> latest </code></td>
 </tr>
 <tr>
 <td>[disable]</td>
 <td><code class="docutils literal notranslate">v6.0.0 -> latest</code></td> <tr>
 <td>[enable]</td>
 <td><code class="docutils literal notranslate">v6.0.0 -> latest</code></td> </table>
 </div>
 </li>
        <li> <span class="li-head">pop3</span> - Configure POP3 protocol options. <span class="li-normal">type: dict</span>
 <a id='label202' href="javascript:ContentClick('label203', 'label202');" onmouseover="ContentPreview('label203');" onmouseout="ContentUnpreview('label203');" title="click to collapse or expand..."> more... </a>
 <div id="label203" style="display:none">
 <table border="1">
 <tr>
 <td></td><td colspan="1">Supported Version Ranges</td>
 </tr>
 <tr>
 <td>pop3</td>
 <td><code class="docutils literal notranslate">v6.0.0 -> latest </code></td>
 </tr>
 </table>
 </div>
 </li>
            <ul class="ul-self">
            <li> <span class="li-head">inspect_all</span> - Enable/disable the inspection of all ports for the protocol. <span class="li-normal">type: str</span> <span class="li-normal">choices: enable, disable</span>
 <a id='label204' href="javascript:ContentClick('label205', 'label204');" onmouseover="ContentPreview('label205');" onmouseout="ContentUnpreview('label205');" title="click to collapse or expand..."> more... </a>
 <div id="label205" style="display:none">
 <table border="1">
 <tr>
 <td></td>
 <td colspan="1">Supported Version Ranges</td>
 </tr>
 <tr>
 <td>inspect_all</td>
 <td><code class="docutils literal notranslate">v6.0.0 -> latest </code></td>
 </tr>
 <tr>
 <td>[enable]</td>
 <td><code class="docutils literal notranslate">v6.0.0 -> latest</code></td> <tr>
 <td>[disable]</td>
 <td><code class="docutils literal notranslate">v6.0.0 -> latest</code></td> </table>
 </div>
 </li>
            <li> <span class="li-head">options</span> - One or more options that can be applied to the session. <span class="li-normal">type: list</span> <span class="li-normal">choices: fragmail, oversize</span>
 <a id='label206' href="javascript:ContentClick('label207', 'label206');" onmouseover="ContentPreview('label207');" onmouseout="ContentUnpreview('label207');" title="click to collapse or expand..."> more... </a>
 <div id="label207" style="display:none">
 <table border="1">
 <tr>
 <td></td>
 <td colspan="1">Supported Version Ranges</td>
 </tr>
 <tr>
 <td>options</td>
 <td><code class="docutils literal notranslate">v6.0.0 -> latest </code></td>
 </tr>
 <tr>
 <td>[fragmail]</td>
 <td><code class="docutils literal notranslate">v6.0.0 -> latest</code></td> <tr>
 <td>[oversize]</td>
 <td><code class="docutils literal notranslate">v6.0.0 -> latest</code></td> </table>
 </div>
 </li>
            <li> <span class="li-head">oversize_limit</span> - Maximum in-memory file size that can be scanned (MB). <span class="li-normal">type: int</span>
 <a id='label208' href="javascript:ContentClick('label209', 'label208');" onmouseover="ContentPreview('label209');" onmouseout="ContentUnpreview('label209');" title="click to collapse or expand..."> more... </a>
 <div id="label209" style="display:none">
 <table border="1">
 <tr>
 <td></td>
 <td colspan="1">Supported Version Ranges</td>
 </tr>
 <tr>
 <td>oversize_limit</td>
 <td><code class="docutils literal notranslate">v6.0.0 -> latest </code></td>
 </tr>
 </table>
 </div>
 </li>
            <li> <span class="li-head">ports</span> - Ports to scan for content (1 - 65535). <span class="li-normal">type: list</span> </li>
            <li> <span class="li-head">proxy_after_tcp_handshake</span> - Proxy traffic after the TCP 3-way handshake has been established (not before). <span class="li-normal">type: str</span> <span class="li-normal">choices: enable, disable</span>
 <a id='label210' href="javascript:ContentClick('label211', 'label210');" onmouseover="ContentPreview('label211');" onmouseout="ContentUnpreview('label211');" title="click to collapse or expand..."> more... </a>
 <div id="label211" style="display:none">
 <table border="1">
 <tr>
 <td></td>
 <td colspan="1">Supported Version Ranges</td>
 </tr>
 <tr>
 <td>proxy_after_tcp_handshake</td>
 <td><code class="docutils literal notranslate">v6.4.0 -> latest </code></td>
 </tr>
 <tr>
 <td>[enable]</td>
 <td><code class="docutils literal notranslate">v6.0.0 -> latest</code></td> <tr>
 <td>[disable]</td>
 <td><code class="docutils literal notranslate">v6.0.0 -> latest</code></td> </table>
 </div>
 </li>
            <li> <span class="li-head">scan_bzip2</span> - Enable/disable scanning of BZip2 compressed files. <span class="li-normal">type: str</span> <span class="li-normal">choices: enable, disable</span>
 <a id='label212' href="javascript:ContentClick('label213', 'label212');" onmouseover="ContentPreview('label213');" onmouseout="ContentUnpreview('label213');" title="click to collapse or expand..."> more... </a>
 <div id="label213" style="display:none">
 <table border="1">
 <tr>
 <td></td>
 <td colspan="1">Supported Version Ranges</td>
 </tr>
 <tr>
 <td>scan_bzip2</td>
 <td><code class="docutils literal notranslate">v6.0.0 -> latest </code></td>
 </tr>
 <tr>
 <td>[enable]</td>
 <td><code class="docutils literal notranslate">v6.0.0 -> latest</code></td> <tr>
 <td>[disable]</td>
 <td><code class="docutils literal notranslate">v6.0.0 -> latest</code></td> </table>
 </div>
 </li>
            <li> <span class="li-head">ssl_offloaded</span> - SSL decryption and encryption performed by an external device. <span class="li-normal">type: str</span> <span class="li-normal">choices: no, yes</span>
 <a id='label214' href="javascript:ContentClick('label215', 'label214');" onmouseover="ContentPreview('label215');" onmouseout="ContentUnpreview('label215');" title="click to collapse or expand..."> more... </a>
 <div id="label215" style="display:none">
 <table border="1">
 <tr>
 <td></td>
 <td colspan="1">Supported Version Ranges</td>
 </tr>
 <tr>
 <td>ssl_offloaded</td>
 <td><code class="docutils literal notranslate">v6.2.0 -> latest </code></td>
 </tr>
 <tr>
 <td>[no]</td>
 <td><code class="docutils literal notranslate">v6.0.0 -> latest</code></td> <tr>
 <td>[yes]</td>
 <td><code class="docutils literal notranslate">v6.0.0 -> latest</code></td> </table>
 </div>
 </li>
            <li> <span class="li-head">status</span> - Enable/disable the active status of scanning for this protocol. <span class="li-normal">type: str</span> <span class="li-normal">choices: enable, disable</span>
 <a id='label216' href="javascript:ContentClick('label217', 'label216');" onmouseover="ContentPreview('label217');" onmouseout="ContentUnpreview('label217');" title="click to collapse or expand..."> more... </a>
 <div id="label217" style="display:none">
 <table border="1">
 <tr>
 <td></td>
 <td colspan="1">Supported Version Ranges</td>
 </tr>
 <tr>
 <td>status</td>
 <td><code class="docutils literal notranslate">v6.0.0 -> latest </code></td>
 </tr>
 <tr>
 <td>[enable]</td>
 <td><code class="docutils literal notranslate">v6.0.0 -> latest</code></td> <tr>
 <td>[disable]</td>
 <td><code class="docutils literal notranslate">v6.0.0 -> latest</code></td> </table>
 </div>
 </li>
            <li> <span class="li-head">uncompressed_nest_limit</span> - Maximum nested levels of compression that can be uncompressed and scanned (2 - 100). <span class="li-normal">type: int</span>
 <a id='label218' href="javascript:ContentClick('label219', 'label218');" onmouseover="ContentPreview('label219');" onmouseout="ContentUnpreview('label219');" title="click to collapse or expand..."> more... </a>
 <div id="label219" style="display:none">
 <table border="1">
 <tr>
 <td></td>
 <td colspan="1">Supported Version Ranges</td>
 </tr>
 <tr>
 <td>uncompressed_nest_limit</td>
 <td><code class="docutils literal notranslate">v6.0.0 -> latest </code></td>
 </tr>
 </table>
 </div>
 </li>
            <li> <span class="li-head">uncompressed_oversize_limit</span> - Maximum in-memory uncompressed file size that can be scanned. <span class="li-normal">type: int</span>
 <a id='label220' href="javascript:ContentClick('label221', 'label220');" onmouseover="ContentPreview('label221');" onmouseout="ContentUnpreview('label221');" title="click to collapse or expand..."> more... </a>
 <div id="label221" style="display:none">
 <table border="1">
 <tr>
 <td></td>
 <td colspan="1">Supported Version Ranges</td>
 </tr>
 <tr>
 <td>uncompressed_oversize_limit</td>
 <td><code class="docutils literal notranslate">v6.0.0 -> latest </code></td>
 </tr>
 </table>
 </div>
 </li>
            </ul>
        <li> <span class="li-head">replacemsg_group</span> - Name of the replacement message group to be used. Source system.replacemsg-group.name. <span class="li-normal">type: str</span>
 <a id='label222' href="javascript:ContentClick('label223', 'label222');" onmouseover="ContentPreview('label223');" onmouseout="ContentUnpreview('label223');" title="click to collapse or expand..."> more... </a>
 <div id="label223" style="display:none">
 <table border="1">
 <tr>
 <td></td>
 <td colspan="1">Supported Version Ranges</td>
 </tr>
 <tr>
 <td>replacemsg_group</td>
 <td><code class="docutils literal notranslate">v6.0.0 -> latest </code></td>
 </tr>
 </table>
 </div>
 </li>
        <li> <span class="li-head">rpc_over_http</span> - Enable/disable inspection of RPC over HTTP. <span class="li-normal">type: str</span> <span class="li-normal">choices: enable, disable</span>
 <a id='label224' href="javascript:ContentClick('label225', 'label224');" onmouseover="ContentPreview('label225');" onmouseout="ContentUnpreview('label225');" title="click to collapse or expand..."> more... </a>
 <div id="label225" style="display:none">
 <table border="1">
 <tr>
 <td></td>
 <td colspan="1">Supported Version Ranges</td>
 </tr>
 <tr>
 <td>rpc_over_http</td>
 <td><code class="docutils literal notranslate">v6.0.0 -> latest </code></td>
 </tr>
 <tr>
 <td>[enable]</td>
 <td><code class="docutils literal notranslate">v6.0.0 -> latest</code></td> <tr>
 <td>[disable]</td>
 <td><code class="docutils literal notranslate">v6.0.0 -> latest</code></td> </table>
 </div>
 </li>
        <li> <span class="li-head">smtp</span> - Configure SMTP protocol options. <span class="li-normal">type: dict</span>
 <a id='label226' href="javascript:ContentClick('label227', 'label226');" onmouseover="ContentPreview('label227');" onmouseout="ContentUnpreview('label227');" title="click to collapse or expand..."> more... </a>
 <div id="label227" style="display:none">
 <table border="1">
 <tr>
 <td></td><td colspan="1">Supported Version Ranges</td>
 </tr>
 <tr>
 <td>smtp</td>
 <td><code class="docutils literal notranslate">v6.0.0 -> latest </code></td>
 </tr>
 </table>
 </div>
 </li>
            <ul class="ul-self">
            <li> <span class="li-head">inspect_all</span> - Enable/disable the inspection of all ports for the protocol. <span class="li-normal">type: str</span> <span class="li-normal">choices: enable, disable</span>
 <a id='label228' href="javascript:ContentClick('label229', 'label228');" onmouseover="ContentPreview('label229');" onmouseout="ContentUnpreview('label229');" title="click to collapse or expand..."> more... </a>
 <div id="label229" style="display:none">
 <table border="1">
 <tr>
 <td></td>
 <td colspan="1">Supported Version Ranges</td>
 </tr>
 <tr>
 <td>inspect_all</td>
 <td><code class="docutils literal notranslate">v6.0.0 -> latest </code></td>
 </tr>
 <tr>
 <td>[enable]</td>
 <td><code class="docutils literal notranslate">v6.0.0 -> latest</code></td> <tr>
 <td>[disable]</td>
 <td><code class="docutils literal notranslate">v6.0.0 -> latest</code></td> </table>
 </div>
 </li>
            <li> <span class="li-head">options</span> - One or more options that can be applied to the session. <span class="li-normal">type: list</span> <span class="li-normal">choices: fragmail, oversize, splice</span>
 <a id='label230' href="javascript:ContentClick('label231', 'label230');" onmouseover="ContentPreview('label231');" onmouseout="ContentUnpreview('label231');" title="click to collapse or expand..."> more... </a>
 <div id="label231" style="display:none">
 <table border="1">
 <tr>
 <td></td>
 <td colspan="1">Supported Version Ranges</td>
 </tr>
 <tr>
 <td>options</td>
 <td><code class="docutils literal notranslate">v6.0.0 -> latest </code></td>
 </tr>
 <tr>
 <td>[fragmail]</td>
 <td><code class="docutils literal notranslate">v6.0.0 -> latest</code></td> <tr>
 <td>[oversize]</td>
 <td><code class="docutils literal notranslate">v6.0.0 -> latest</code></td> <tr>
 <td>[splice]</td>
 <td><code class="docutils literal notranslate">v6.0.0 -> latest</code></td> </table>
 </div>
 </li>
            <li> <span class="li-head">oversize_limit</span> - Maximum in-memory file size that can be scanned (MB). <span class="li-normal">type: int</span>
 <a id='label232' href="javascript:ContentClick('label233', 'label232');" onmouseover="ContentPreview('label233');" onmouseout="ContentUnpreview('label233');" title="click to collapse or expand..."> more... </a>
 <div id="label233" style="display:none">
 <table border="1">
 <tr>
 <td></td>
 <td colspan="1">Supported Version Ranges</td>
 </tr>
 <tr>
 <td>oversize_limit</td>
 <td><code class="docutils literal notranslate">v6.0.0 -> latest </code></td>
 </tr>
 </table>
 </div>
 </li>
            <li> <span class="li-head">ports</span> - Ports to scan for content (1 - 65535). <span class="li-normal">type: list</span> </li>
            <li> <span class="li-head">proxy_after_tcp_handshake</span> - Proxy traffic after the TCP 3-way handshake has been established (not before). <span class="li-normal">type: str</span> <span class="li-normal">choices: enable, disable</span>
 <a id='label234' href="javascript:ContentClick('label235', 'label234');" onmouseover="ContentPreview('label235');" onmouseout="ContentUnpreview('label235');" title="click to collapse or expand..."> more... </a>
 <div id="label235" style="display:none">
 <table border="1">
 <tr>
 <td></td>
 <td colspan="1">Supported Version Ranges</td>
 </tr>
 <tr>
 <td>proxy_after_tcp_handshake</td>
 <td><code class="docutils literal notranslate">v6.4.0 -> latest </code></td>
 </tr>
 <tr>
 <td>[enable]</td>
 <td><code class="docutils literal notranslate">v6.0.0 -> latest</code></td> <tr>
 <td>[disable]</td>
 <td><code class="docutils literal notranslate">v6.0.0 -> latest</code></td> </table>
 </div>
 </li>
            <li> <span class="li-head">scan_bzip2</span> - Enable/disable scanning of BZip2 compressed files. <span class="li-normal">type: str</span> <span class="li-normal">choices: enable, disable</span>
 <a id='label236' href="javascript:ContentClick('label237', 'label236');" onmouseover="ContentPreview('label237');" onmouseout="ContentUnpreview('label237');" title="click to collapse or expand..."> more... </a>
 <div id="label237" style="display:none">
 <table border="1">
 <tr>
 <td></td>
 <td colspan="1">Supported Version Ranges</td>
 </tr>
 <tr>
 <td>scan_bzip2</td>
 <td><code class="docutils literal notranslate">v6.0.0 -> latest </code></td>
 </tr>
 <tr>
 <td>[enable]</td>
 <td><code class="docutils literal notranslate">v6.0.0 -> latest</code></td> <tr>
 <td>[disable]</td>
 <td><code class="docutils literal notranslate">v6.0.0 -> latest</code></td> </table>
 </div>
 </li>
            <li> <span class="li-head">server_busy</span> - Enable/disable SMTP server busy when server not available. <span class="li-normal">type: str</span> <span class="li-normal">choices: enable, disable</span>
 <a id='label238' href="javascript:ContentClick('label239', 'label238');" onmouseover="ContentPreview('label239');" onmouseout="ContentUnpreview('label239');" title="click to collapse or expand..."> more... </a>
 <div id="label239" style="display:none">
 <table border="1">
 <tr>
 <td></td>
 <td colspan="1">Supported Version Ranges</td>
 </tr>
 <tr>
 <td>server_busy</td>
 <td><code class="docutils literal notranslate">v6.0.0 -> latest </code></td>
 </tr>
 <tr>
 <td>[enable]</td>
 <td><code class="docutils literal notranslate">v6.0.0 -> latest</code></td> <tr>
 <td>[disable]</td>
 <td><code class="docutils literal notranslate">v6.0.0 -> latest</code></td> </table>
 </div>
 </li>
            <li> <span class="li-head">ssl_offloaded</span> - SSL decryption and encryption performed by an external device. <span class="li-normal">type: str</span> <span class="li-normal">choices: no, yes</span>
 <a id='label240' href="javascript:ContentClick('label241', 'label240');" onmouseover="ContentPreview('label241');" onmouseout="ContentUnpreview('label241');" title="click to collapse or expand..."> more... </a>
 <div id="label241" style="display:none">
 <table border="1">
 <tr>
 <td></td>
 <td colspan="1">Supported Version Ranges</td>
 </tr>
 <tr>
 <td>ssl_offloaded</td>
 <td><code class="docutils literal notranslate">v6.2.0 -> latest </code></td>
 </tr>
 <tr>
 <td>[no]</td>
 <td><code class="docutils literal notranslate">v6.0.0 -> latest</code></td> <tr>
 <td>[yes]</td>
 <td><code class="docutils literal notranslate">v6.0.0 -> latest</code></td> </table>
 </div>
 </li>
            <li> <span class="li-head">status</span> - Enable/disable the active status of scanning for this protocol. <span class="li-normal">type: str</span> <span class="li-normal">choices: enable, disable</span>
 <a id='label242' href="javascript:ContentClick('label243', 'label242');" onmouseover="ContentPreview('label243');" onmouseout="ContentUnpreview('label243');" title="click to collapse or expand..."> more... </a>
 <div id="label243" style="display:none">
 <table border="1">
 <tr>
 <td></td>
 <td colspan="1">Supported Version Ranges</td>
 </tr>
 <tr>
 <td>status</td>
 <td><code class="docutils literal notranslate">v6.0.0 -> latest </code></td>
 </tr>
 <tr>
 <td>[enable]</td>
 <td><code class="docutils literal notranslate">v6.0.0 -> latest</code></td> <tr>
 <td>[disable]</td>
 <td><code class="docutils literal notranslate">v6.0.0 -> latest</code></td> </table>
 </div>
 </li>
            <li> <span class="li-head">uncompressed_nest_limit</span> - Maximum nested levels of compression that can be uncompressed and scanned (2 - 100). <span class="li-normal">type: int</span>
 <a id='label244' href="javascript:ContentClick('label245', 'label244');" onmouseover="ContentPreview('label245');" onmouseout="ContentUnpreview('label245');" title="click to collapse or expand..."> more... </a>
 <div id="label245" style="display:none">
 <table border="1">
 <tr>
 <td></td>
 <td colspan="1">Supported Version Ranges</td>
 </tr>
 <tr>
 <td>uncompressed_nest_limit</td>
 <td><code class="docutils literal notranslate">v6.0.0 -> latest </code></td>
 </tr>
 </table>
 </div>
 </li>
            <li> <span class="li-head">uncompressed_oversize_limit</span> - Maximum in-memory uncompressed file size that can be scanned. <span class="li-normal">type: int</span>
 <a id='label246' href="javascript:ContentClick('label247', 'label246');" onmouseover="ContentPreview('label247');" onmouseout="ContentUnpreview('label247');" title="click to collapse or expand..."> more... </a>
 <div id="label247" style="display:none">
 <table border="1">
 <tr>
 <td></td>
 <td colspan="1">Supported Version Ranges</td>
 </tr>
 <tr>
 <td>uncompressed_oversize_limit</td>
 <td><code class="docutils literal notranslate">v6.0.0 -> latest </code></td>
 </tr>
 </table>
 </div>
 </li>
            </ul>
        <li> <span class="li-head">ssh</span> - Configure SFTP and SCP protocol options. <span class="li-normal">type: dict</span>
 <a id='label248' href="javascript:ContentClick('label249', 'label248');" onmouseover="ContentPreview('label249');" onmouseout="ContentUnpreview('label249');" title="click to collapse or expand..."> more... </a>
 <div id="label249" style="display:none">
 <table border="1">
 <tr>
 <td></td><td colspan="1">Supported Version Ranges</td>
 </tr>
 <tr>
 <td>ssh</td>
 <td><code class="docutils literal notranslate">v6.2.0 -> latest </code></td>
 </tr>
 </table>
 </div>
 </li>
            <ul class="ul-self">
            <li> <span class="li-head">comfort_amount</span> - Number of bytes to send in each transmission for client comforting (bytes). <span class="li-normal">type: int</span>
 <a id='label250' href="javascript:ContentClick('label251', 'label250');" onmouseover="ContentPreview('label251');" onmouseout="ContentUnpreview('label251');" title="click to collapse or expand..."> more... </a>
 <div id="label251" style="display:none">
 <table border="1">
 <tr>
 <td></td>
 <td colspan="1">Supported Version Ranges</td>
 </tr>
 <tr>
 <td>comfort_amount</td>
 <td><code class="docutils literal notranslate">v6.2.0 -> latest </code></td>
 </tr>
 </table>
 </div>
 </li>
            <li> <span class="li-head">comfort_interval</span> - Interval between successive transmissions of data for client comforting (seconds). <span class="li-normal">type: int</span>
 <a id='label252' href="javascript:ContentClick('label253', 'label252');" onmouseover="ContentPreview('label253');" onmouseout="ContentUnpreview('label253');" title="click to collapse or expand..."> more... </a>
 <div id="label253" style="display:none">
 <table border="1">
 <tr>
 <td></td>
 <td colspan="1">Supported Version Ranges</td>
 </tr>
 <tr>
 <td>comfort_interval</td>
 <td><code class="docutils literal notranslate">v6.2.0 -> latest </code></td>
 </tr>
 </table>
 </div>
 </li>
            <li> <span class="li-head">options</span> - One or more options that can be applied to the session. <span class="li-normal">type: list</span> <span class="li-normal">choices: oversize, clientcomfort, servercomfort</span>
 <a id='label254' href="javascript:ContentClick('label255', 'label254');" onmouseover="ContentPreview('label255');" onmouseout="ContentUnpreview('label255');" title="click to collapse or expand..."> more... </a>
 <div id="label255" style="display:none">
 <table border="1">
 <tr>
 <td></td>
 <td colspan="1">Supported Version Ranges</td>
 </tr>
 <tr>
 <td>options</td>
 <td><code class="docutils literal notranslate">v6.2.0 -> latest </code></td>
 </tr>
 <tr>
 <td>[oversize]</td>
 <td><code class="docutils literal notranslate">v6.0.0 -> latest</code></td> <tr>
 <td>[clientcomfort]</td>
 <td><code class="docutils literal notranslate">v6.0.0 -> latest</code></td> <tr>
 <td>[servercomfort]</td>
 <td><code class="docutils literal notranslate">v6.0.0 -> latest</code></td> </table>
 </div>
 </li>
            <li> <span class="li-head">oversize_limit</span> - Maximum in-memory file size that can be scanned (MB). <span class="li-normal">type: int</span>
 <a id='label256' href="javascript:ContentClick('label257', 'label256');" onmouseover="ContentPreview('label257');" onmouseout="ContentUnpreview('label257');" title="click to collapse or expand..."> more... </a>
 <div id="label257" style="display:none">
 <table border="1">
 <tr>
 <td></td>
 <td colspan="1">Supported Version Ranges</td>
 </tr>
 <tr>
 <td>oversize_limit</td>
 <td><code class="docutils literal notranslate">v6.2.0 -> latest </code></td>
 </tr>
 </table>
 </div>
 </li>
            <li> <span class="li-head">scan_bzip2</span> - Enable/disable scanning of BZip2 compressed files. <span class="li-normal">type: str</span> <span class="li-normal">choices: enable, disable</span>
 <a id='label258' href="javascript:ContentClick('label259', 'label258');" onmouseover="ContentPreview('label259');" onmouseout="ContentUnpreview('label259');" title="click to collapse or expand..."> more... </a>
 <div id="label259" style="display:none">
 <table border="1">
 <tr>
 <td></td>
 <td colspan="1">Supported Version Ranges</td>
 </tr>
 <tr>
 <td>scan_bzip2</td>
 <td><code class="docutils literal notranslate">v6.2.0 -> latest </code></td>
 </tr>
 <tr>
 <td>[enable]</td>
 <td><code class="docutils literal notranslate">v6.0.0 -> latest</code></td> <tr>
 <td>[disable]</td>
 <td><code class="docutils literal notranslate">v6.0.0 -> latest</code></td> </table>
 </div>
 </li>
            <li> <span class="li-head">ssl_offloaded</span> - SSL decryption and encryption performed by an external device. <span class="li-normal">type: str</span> <span class="li-normal">choices: no, yes</span>
 <a id='label260' href="javascript:ContentClick('label261', 'label260');" onmouseover="ContentPreview('label261');" onmouseout="ContentUnpreview('label261');" title="click to collapse or expand..."> more... </a>
 <div id="label261" style="display:none">
 <table border="1">
 <tr>
 <td></td>
 <td colspan="1">Supported Version Ranges</td>
 </tr>
 <tr>
 <td>ssl_offloaded</td>
 <td><code class="docutils literal notranslate">v7.0.0 -> latest </code></td>
 </tr>
 <tr>
 <td>[no]</td>
 <td><code class="docutils literal notranslate">v6.0.0 -> latest</code></td> <tr>
 <td>[yes]</td>
 <td><code class="docutils literal notranslate">v6.0.0 -> latest</code></td> </table>
 </div>
 </li>
            <li> <span class="li-head">stream_based_uncompressed_limit</span> - Maximum stream-based uncompressed data size that will be scanned in megabytes. Stream-based uncompression used only under certain conditions (unlimited = 0). <span class="li-normal">type: int</span>
 <a id='label262' href="javascript:ContentClick('label263', 'label262');" onmouseover="ContentPreview('label263');" onmouseout="ContentUnpreview('label263');" title="click to collapse or expand..."> more... </a>
 <div id="label263" style="display:none">
 <table border="1">
 <tr>
 <td></td>
 <td colspan="1">Supported Version Ranges</td>
 </tr>
 <tr>
 <td>stream_based_uncompressed_limit</td>
 <td><code class="docutils literal notranslate">v7.0.0 -> latest </code></td>
 </tr>
 </table>
 </div>
 </li>
            <li> <span class="li-head">tcp_window_maximum</span> - Maximum dynamic TCP window size. <span class="li-normal">type: int</span>
 <a id='label264' href="javascript:ContentClick('label265', 'label264');" onmouseover="ContentPreview('label265');" onmouseout="ContentUnpreview('label265');" title="click to collapse or expand..."> more... </a>
 <div id="label265" style="display:none">
 <table border="1">
 <tr>
 <td></td>
 <td colspan="1">Supported Version Ranges</td>
 </tr>
 <tr>
 <td>tcp_window_maximum</td>
 <td><code class="docutils literal notranslate">v7.0.0 -> latest </code></td>
 </tr>
 </table>
 </div>
 </li>
            <li> <span class="li-head">tcp_window_minimum</span> - Minimum dynamic TCP window size. <span class="li-normal">type: int</span>
 <a id='label266' href="javascript:ContentClick('label267', 'label266');" onmouseover="ContentPreview('label267');" onmouseout="ContentUnpreview('label267');" title="click to collapse or expand..."> more... </a>
 <div id="label267" style="display:none">
 <table border="1">
 <tr>
 <td></td>
 <td colspan="1">Supported Version Ranges</td>
 </tr>
 <tr>
 <td>tcp_window_minimum</td>
 <td><code class="docutils literal notranslate">v7.0.0 -> latest </code></td>
 </tr>
 </table>
 </div>
 </li>
            <li> <span class="li-head">tcp_window_size</span> - Set TCP static window size. <span class="li-normal">type: int</span>
 <a id='label268' href="javascript:ContentClick('label269', 'label268');" onmouseover="ContentPreview('label269');" onmouseout="ContentUnpreview('label269');" title="click to collapse or expand..."> more... </a>
 <div id="label269" style="display:none">
 <table border="1">
 <tr>
 <td></td>
 <td colspan="1">Supported Version Ranges</td>
 </tr>
 <tr>
 <td>tcp_window_size</td>
 <td><code class="docutils literal notranslate">v7.0.0 -> latest </code></td>
 </tr>
 </table>
 </div>
 </li>
            <li> <span class="li-head">tcp_window_type</span> - TCP window type to use for this protocol. <span class="li-normal">type: str</span> <span class="li-normal">choices: auto-tuning, system, static, dynamic</span>
 <a id='label270' href="javascript:ContentClick('label271', 'label270');" onmouseover="ContentPreview('label271');" onmouseout="ContentUnpreview('label271');" title="click to collapse or expand..."> more... </a>
 <div id="label271" style="display:none">
 <table border="1">
 <tr>
 <td></td>
 <td colspan="1">Supported Version Ranges</td>
 </tr>
 <tr>
 <td>tcp_window_type</td>
 <td><code class="docutils literal notranslate">v7.0.0 -> latest </code></td>
 </tr>
 <tr>
 <td>[auto-tuning]</td>
 <td><code class="docutils literal notranslate">v7.0.4 -> latest</code></td>
 </tr>
 <tr>
 <td>[system]</td>
 <td><code class="docutils literal notranslate">v6.0.0 -> latest</code></td> <tr>
 <td>[static]</td>
 <td><code class="docutils literal notranslate">v6.0.0 -> latest</code></td> <tr>
 <td>[dynamic]</td>
 <td><code class="docutils literal notranslate">v6.0.0 -> latest</code></td> </table>
 </div>
 </li>
            <li> <span class="li-head">uncompressed_nest_limit</span> - Maximum nested levels of compression that can be uncompressed and scanned (2 - 100). <span class="li-normal">type: int</span>
 <a id='label272' href="javascript:ContentClick('label273', 'label272');" onmouseover="ContentPreview('label273');" onmouseout="ContentUnpreview('label273');" title="click to collapse or expand..."> more... </a>
 <div id="label273" style="display:none">
 <table border="1">
 <tr>
 <td></td>
 <td colspan="1">Supported Version Ranges</td>
 </tr>
 <tr>
 <td>uncompressed_nest_limit</td>
 <td><code class="docutils literal notranslate">v6.2.0 -> latest </code></td>
 </tr>
 </table>
 </div>
 </li>
            <li> <span class="li-head">uncompressed_oversize_limit</span> - Maximum in-memory uncompressed file size that can be scanned. <span class="li-normal">type: int</span>
 <a id='label274' href="javascript:ContentClick('label275', 'label274');" onmouseover="ContentPreview('label275');" onmouseout="ContentUnpreview('label275');" title="click to collapse or expand..."> more... </a>
 <div id="label275" style="display:none">
 <table border="1">
 <tr>
 <td></td>
 <td colspan="1">Supported Version Ranges</td>
 </tr>
 <tr>
 <td>uncompressed_oversize_limit</td>
 <td><code class="docutils literal notranslate">v6.2.0 -> latest </code></td>
 </tr>
 </table>
 </div>
 </li>
            </ul>
        <li> <span class="li-head">switching_protocols_log</span> - Enable/disable logging for HTTP/HTTPS switching protocols. <span class="li-normal">type: str</span> <span class="li-normal">choices: disable, enable</span>
 <a id='label276' href="javascript:ContentClick('label277', 'label276');" onmouseover="ContentPreview('label277');" onmouseout="ContentUnpreview('label277');" title="click to collapse or expand..."> more... </a>
 <div id="label277" style="display:none">
 <table border="1">
 <tr>
 <td></td>
 <td colspan="1">Supported Version Ranges</td>
 </tr>
 <tr>
 <td>switching_protocols_log</td>
 <td><code class="docutils literal notranslate">v6.0.0 -> latest </code></td>
 </tr>
 <tr>
 <td>[disable]</td>
 <td><code class="docutils literal notranslate">v6.0.0 -> latest</code></td> <tr>
 <td>[enable]</td>
 <td><code class="docutils literal notranslate">v6.0.0 -> latest</code></td> </table>
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
    
    - name: Configure protocol options.
      fortinet.fortios.fortios_firewall_profile_protocol_options:
          vdom: "{{ vdom }}"
          state: "present"
          access_token: "<your_own_value>"
          firewall_profile_protocol_options:
              cifs:
                  domain_controller: "<your_own_value> (source user.domain-controller.name credential-store.domain-controller.server-name)"
                  options: "oversize"
                  oversize_limit: "10"
                  ports: "<your_own_value>"
                  scan_bzip2: "enable"
                  server_credential_type: "none"
                  server_keytab:
                      -
                          keytab: "<your_own_value>"
                          principal: "<your_own_value>"
                  status: "enable"
                  tcp_window_maximum: "8388608"
                  tcp_window_minimum: "131072"
                  tcp_window_size: "262144"
                  tcp_window_type: "auto-tuning"
                  uncompressed_nest_limit: "12"
                  uncompressed_oversize_limit: "10"
              comment: "Optional comments."
              dns:
                  ports: "<your_own_value>"
                  status: "enable"
              ftp:
                  comfort_amount: "1"
                  comfort_interval: "10"
                  explicit_ftp_tls: "enable"
                  inspect_all: "enable"
                  options: "clientcomfort"
                  oversize_limit: "10"
                  ports: "<your_own_value>"
                  scan_bzip2: "enable"
                  ssl_offloaded: "no"
                  status: "enable"
                  stream_based_uncompressed_limit: "0"
                  tcp_window_maximum: "8388608"
                  tcp_window_minimum: "131072"
                  tcp_window_size: "262144"
                  tcp_window_type: "auto-tuning"
                  uncompressed_nest_limit: "12"
                  uncompressed_oversize_limit: "10"
              http:
                  address_ip_rating: "enable"
                  block_page_status_code: "403"
                  comfort_amount: "1"
                  comfort_interval: "10"
                  fortinet_bar: "enable"
                  fortinet_bar_port: "32767"
                  h2c: "enable"
                  http_policy: "disable"
                  inspect_all: "enable"
                  options: "clientcomfort"
                  oversize_limit: "10"
                  ports: "<your_own_value>"
                  post_lang: "jisx0201"
                  proxy_after_tcp_handshake: "enable"
                  range_block: "disable"
                  retry_count: "0"
                  scan_bzip2: "enable"
                  ssl_offloaded: "no"
                  status: "enable"
                  stream_based_uncompressed_limit: "0"
                  streaming_content_bypass: "enable"
                  strip_x_forwarded_for: "disable"
                  switching_protocols: "bypass"
                  tcp_window_maximum: "8388608"
                  tcp_window_minimum: "131072"
                  tcp_window_size: "262144"
                  tcp_window_type: "auto-tuning"
                  tunnel_non_http: "enable"
                  uncompressed_nest_limit: "12"
                  uncompressed_oversize_limit: "10"
                  unknown_content_encoding: "block"
                  unknown_http_version: "reject"
                  verify_dns_for_policy_matching: "enable"
              imap:
                  inspect_all: "enable"
                  options: "fragmail"
                  oversize_limit: "10"
                  ports: "<your_own_value>"
                  proxy_after_tcp_handshake: "enable"
                  scan_bzip2: "enable"
                  ssl_offloaded: "no"
                  status: "enable"
                  uncompressed_nest_limit: "12"
                  uncompressed_oversize_limit: "10"
              mail_signature:
                  signature: "<your_own_value>"
                  status: "disable"
              mapi:
                  options: "fragmail"
                  oversize_limit: "10"
                  ports: "<your_own_value>"
                  scan_bzip2: "enable"
                  status: "enable"
                  uncompressed_nest_limit: "12"
                  uncompressed_oversize_limit: "10"
              name: "default_name_98"
              nntp:
                  inspect_all: "enable"
                  options: "oversize"
                  oversize_limit: "10"
                  ports: "<your_own_value>"
                  proxy_after_tcp_handshake: "enable"
                  scan_bzip2: "enable"
                  status: "enable"
                  uncompressed_nest_limit: "12"
                  uncompressed_oversize_limit: "10"
              oversize_log: "disable"
              pop3:
                  inspect_all: "enable"
                  options: "fragmail"
                  oversize_limit: "10"
                  ports: "<your_own_value>"
                  proxy_after_tcp_handshake: "enable"
                  scan_bzip2: "enable"
                  ssl_offloaded: "no"
                  status: "enable"
                  uncompressed_nest_limit: "12"
                  uncompressed_oversize_limit: "10"
              replacemsg_group: "<your_own_value> (source system.replacemsg-group.name)"
              rpc_over_http: "enable"
              smtp:
                  inspect_all: "enable"
                  options: "fragmail"
                  oversize_limit: "10"
                  ports: "<your_own_value>"
                  proxy_after_tcp_handshake: "enable"
                  scan_bzip2: "enable"
                  server_busy: "enable"
                  ssl_offloaded: "no"
                  status: "enable"
                  uncompressed_nest_limit: "12"
                  uncompressed_oversize_limit: "10"
              ssh:
                  comfort_amount: "1"
                  comfort_interval: "10"
                  options: "oversize"
                  oversize_limit: "10"
                  scan_bzip2: "enable"
                  ssl_offloaded: "no"
                  stream_based_uncompressed_limit: "0"
                  tcp_window_maximum: "8388608"
                  tcp_window_minimum: "131072"
                  tcp_window_size: "262144"
                  tcp_window_type: "auto-tuning"
                  uncompressed_nest_limit: "12"
                  uncompressed_oversize_limit: "10"
              switching_protocols_log: "disable"


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
