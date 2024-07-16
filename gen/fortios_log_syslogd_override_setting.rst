:source: fortios_log_syslogd_override_setting.py

:orphan:

.. fortios_log_syslogd_override_setting:

fortios_log_syslogd_override_setting -- Override settings for remote syslog server in Fortinet's FortiOS and FortiGate.
+++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++

.. versionadded:: 2.0.0

.. contents::
   :local:
   :depth: 1


Synopsis
--------
- This module is able to configure a FortiGate or FortiOS (FOS) device by allowing the user to set and modify log_syslogd feature and override_setting category. Examples include all parameters and values need to be adjusted to datasources before usage. Tested with FOS v6.0.0



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
    <li> <span class="li-head">log_syslogd_override_setting</span> - Override settings for remote syslog server. <span class="li-normal">type: dict</span>
 <a id='label0' href="javascript:ContentClick('label1', 'label0');" onmouseover="ContentPreview('label1');" onmouseout="ContentUnpreview('label1');" title="click to collapse or expand..."> more... </a>
 <div id="label1" style="display:none">
 <table border="1">
 <tr>
 <td></td><td colspan="1">Supported Version Ranges</td>
 </tr>
 <tr>
 <td>log_syslogd_override_setting</td>
 <td><code class="docutils literal notranslate">v6.0.0 -> 7.4.4 </code></td>
 </tr>
 </table>
 </div>
 </li>
        <ul class="ul-self">
        <li> <span class="li-head">certificate</span> - Certificate used to communicate with Syslog server. Source certificate.local.name. <span class="li-normal">type: str</span>
 <a id='label2' href="javascript:ContentClick('label3', 'label2');" onmouseover="ContentPreview('label3');" onmouseout="ContentUnpreview('label3');" title="click to collapse or expand..."> more... </a>
 <div id="label3" style="display:none">
 <table border="1">
 <tr>
 <td></td>
 <td colspan="1">Supported Version Ranges</td>
 </tr>
 <tr>
 <td>certificate</td>
 <td><code class="docutils literal notranslate">v6.0.0 -> 7.4.4 </code></td>
 </tr>
 </table>
 </div>
 </li>
        <li> <span class="li-head">custom_field_name</span> - Custom field name for CEF format logging. <span class="li-normal">type: list</span> <span style="font-family:'Courier New'" class="li-required">member_path: custom_field_name:id</span>
 <a id='label4' href="javascript:ContentClick('label5', 'label4');" onmouseover="ContentPreview('label5');" onmouseout="ContentUnpreview('label5');" title="click to collapse or expand..."> more... </a>
 <div id="label5" style="display:none">
 <table border="1">
 <tr>
 <td></td><td colspan="1">Supported Version Ranges</td>
 </tr>
 <tr>
 <td>custom_field_name</td>
 <td><code class="docutils literal notranslate">v6.0.0 -> 7.4.4 </code></td>
 </tr>
 </table>
 </div>
 </li>
            <ul class="ul-self">
            <li> <span class="li-head">custom</span> - Field custom name [A-Za-z0-9_]. <span class="li-normal">type: str</span>
 <a id='label6' href="javascript:ContentClick('label7', 'label6');" onmouseover="ContentPreview('label7');" onmouseout="ContentUnpreview('label7');" title="click to collapse or expand..."> more... </a>
 <div id="label7" style="display:none">
 <table border="1">
 <tr>
 <td></td>
 <td colspan="1">Supported Version Ranges</td>
 </tr>
 <tr>
 <td>custom</td>
 <td><code class="docutils literal notranslate">v6.0.0 -> 7.4.4 </code></td>
 </tr>
 </table>
 </div>
 </li>
            <li> <span class="li-head">id</span> - Entry ID. see <a href='#notes'>Notes</a>. <span class="li-normal">type: int</span> <span class="li-required">required: true</span>
 <a id='label8' href="javascript:ContentClick('label9', 'label8');" onmouseover="ContentPreview('label9');" onmouseout="ContentUnpreview('label9');" title="click to collapse or expand..."> more... </a>
 <div id="label9" style="display:none">
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
            <li> <span class="li-head">name</span> - Field name [A-Za-z0-9_]. <span class="li-normal">type: str</span>
 <a id='label10' href="javascript:ContentClick('label11', 'label10');" onmouseover="ContentPreview('label11');" onmouseout="ContentUnpreview('label11');" title="click to collapse or expand..."> more... </a>
 <div id="label11" style="display:none">
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
            </ul>
        <li> <span class="li-head">enc_algorithm</span> - Enable/disable reliable syslogging with TLS encryption. <span class="li-normal">type: str</span> <span class="li-normal">choices: high-medium, high, low, disable</span>
 <a id='label12' href="javascript:ContentClick('label13', 'label12');" onmouseover="ContentPreview('label13');" onmouseout="ContentUnpreview('label13');" title="click to collapse or expand..."> more... </a>
 <div id="label13" style="display:none">
 <table border="1">
 <tr>
 <td></td>
 <td colspan="1">Supported Version Ranges</td>
 </tr>
 <tr>
 <td>enc_algorithm</td>
 <td><code class="docutils literal notranslate">v6.0.0 -> 7.4.4 </code></td>
 </tr>
 <tr>
 <td>[high-medium]</td>
 <td><code class="docutils literal notranslate">v6.0.0 -> 7.4.4</code></td>
 <tr>
 <td>[high]</td>
 <td><code class="docutils literal notranslate">v6.0.0 -> 7.4.4</code></td>
 <tr>
 <td>[low]</td>
 <td><code class="docutils literal notranslate">v6.0.0 -> 7.4.4</code></td>
 <tr>
 <td>[disable]</td>
 <td><code class="docutils literal notranslate">v6.0.0 -> 7.4.4</code></td>
 </table>
 </div>
 </li>
        <li> <span class="li-head">facility</span> - Remote syslog facility. <span class="li-normal">type: str</span> <span class="li-normal">choices: kernel, user, mail, daemon, auth, syslog, lpr, news, uucp, cron, authpriv, ftp, ntp, audit, alert, clock, local0, local1, local2, local3, local4, local5, local6, local7</span>
 <a id='label14' href="javascript:ContentClick('label15', 'label14');" onmouseover="ContentPreview('label15');" onmouseout="ContentUnpreview('label15');" title="click to collapse or expand..."> more... </a>
 <div id="label15" style="display:none">
 <table border="1">
 <tr>
 <td></td>
 <td colspan="1">Supported Version Ranges</td>
 </tr>
 <tr>
 <td>facility</td>
 <td><code class="docutils literal notranslate">v6.0.0 -> 7.4.4 </code></td>
 </tr>
 <tr>
 <td>[kernel]</td>
 <td><code class="docutils literal notranslate">v6.0.0 -> 7.4.4</code></td>
 <tr>
 <td>[user]</td>
 <td><code class="docutils literal notranslate">v6.0.0 -> 7.4.4</code></td>
 <tr>
 <td>[mail]</td>
 <td><code class="docutils literal notranslate">v6.0.0 -> 7.4.4</code></td>
 <tr>
 <td>[daemon]</td>
 <td><code class="docutils literal notranslate">v6.0.0 -> 7.4.4</code></td>
 <tr>
 <td>[auth]</td>
 <td><code class="docutils literal notranslate">v6.0.0 -> 7.4.4</code></td>
 <tr>
 <td>[syslog]</td>
 <td><code class="docutils literal notranslate">v6.0.0 -> 7.4.4</code></td>
 <tr>
 <td>[lpr]</td>
 <td><code class="docutils literal notranslate">v6.0.0 -> 7.4.4</code></td>
 <tr>
 <td>[news]</td>
 <td><code class="docutils literal notranslate">v6.0.0 -> 7.4.4</code></td>
 <tr>
 <td>[uucp]</td>
 <td><code class="docutils literal notranslate">v6.0.0 -> 7.4.4</code></td>
 <tr>
 <td>[cron]</td>
 <td><code class="docutils literal notranslate">v6.0.0 -> 7.4.4</code></td>
 <tr>
 <td>[authpriv]</td>
 <td><code class="docutils literal notranslate">v6.0.0 -> 7.4.4</code></td>
 <tr>
 <td>[ftp]</td>
 <td><code class="docutils literal notranslate">v6.0.0 -> 7.4.4</code></td>
 <tr>
 <td>[ntp]</td>
 <td><code class="docutils literal notranslate">v6.0.0 -> 7.4.4</code></td>
 <tr>
 <td>[audit]</td>
 <td><code class="docutils literal notranslate">v6.0.0 -> 7.4.4</code></td>
 <tr>
 <td>[alert]</td>
 <td><code class="docutils literal notranslate">v6.0.0 -> 7.4.4</code></td>
 <tr>
 <td>[clock]</td>
 <td><code class="docutils literal notranslate">v6.0.0 -> 7.4.4</code></td>
 <tr>
 <td>[local0]</td>
 <td><code class="docutils literal notranslate">v6.0.0 -> 7.4.4</code></td>
 <tr>
 <td>[local1]</td>
 <td><code class="docutils literal notranslate">v6.0.0 -> 7.4.4</code></td>
 <tr>
 <td>[local2]</td>
 <td><code class="docutils literal notranslate">v6.0.0 -> 7.4.4</code></td>
 <tr>
 <td>[local3]</td>
 <td><code class="docutils literal notranslate">v6.0.0 -> 7.4.4</code></td>
 <tr>
 <td>[local4]</td>
 <td><code class="docutils literal notranslate">v6.0.0 -> 7.4.4</code></td>
 <tr>
 <td>[local5]</td>
 <td><code class="docutils literal notranslate">v6.0.0 -> 7.4.4</code></td>
 <tr>
 <td>[local6]</td>
 <td><code class="docutils literal notranslate">v6.0.0 -> 7.4.4</code></td>
 <tr>
 <td>[local7]</td>
 <td><code class="docutils literal notranslate">v6.0.0 -> 7.4.4</code></td>
 </table>
 </div>
 </li>
        <li> <span class="li-head">format</span> - Log format. <span class="li-normal">type: str</span> <span class="li-normal">choices: default, csv, cef, rfc5424, json</span>
 <a id='label16' href="javascript:ContentClick('label17', 'label16');" onmouseover="ContentPreview('label17');" onmouseout="ContentUnpreview('label17');" title="click to collapse or expand..."> more... </a>
 <div id="label17" style="display:none">
 <table border="1">
 <tr>
 <td></td>
 <td colspan="1">Supported Version Ranges</td>
 </tr>
 <tr>
 <td>format</td>
 <td><code class="docutils literal notranslate">v6.0.0 -> 7.4.4 </code></td>
 </tr>
 <tr>
 <td>[default]</td>
 <td><code class="docutils literal notranslate">v6.0.0 -> 7.4.4</code></td>
 <tr>
 <td>[csv]</td>
 <td><code class="docutils literal notranslate">v6.0.0 -> 7.4.4</code></td>
 <tr>
 <td>[cef]</td>
 <td><code class="docutils literal notranslate">v6.0.0 -> 7.4.4</code></td>
 <tr>
 <td>[rfc5424]</td>
 <td><code class="docutils literal notranslate">v7.0.0 -> 7.4.4</code></td>
 </tr>
 <tr>
 <td>[json]</td>
 <td><code class="docutils literal notranslate">v7.4.1 -> 7.4.4</code></td>
 </tr>
 </table>
 </div>
 </li>
        <li> <span class="li-head">interface</span> - Specify outgoing interface to reach server. Source system.interface.name. <span class="li-normal">type: str</span>
 <a id='label18' href="javascript:ContentClick('label19', 'label18');" onmouseover="ContentPreview('label19');" onmouseout="ContentUnpreview('label19');" title="click to collapse or expand..."> more... </a>
 <div id="label19" style="display:none">
 <table border="1">
 <tr>
 <td></td>
 <td colspan="2">Supported Version Ranges</td>
 </tr>
 <tr>
 <td>interface</td>
 <td><code class="docutils literal notranslate">v6.2.7 -> v6.4.0 </code></td>
 <td><code class="docutils literal notranslate">v6.4.4 -> 7.4.4 </code></td>
 </tr>
 </table>
 </div>
 </li>
        <li> <span class="li-head">interface_select_method</span> - Specify how to select outgoing interface to reach server. <span class="li-normal">type: str</span> <span class="li-normal">choices: auto, sdwan, specify</span>
 <a id='label20' href="javascript:ContentClick('label21', 'label20');" onmouseover="ContentPreview('label21');" onmouseout="ContentUnpreview('label21');" title="click to collapse or expand..."> more... </a>
 <div id="label21" style="display:none">
 <table border="1">
 <tr>
 <td></td>
 <td colspan="2">Supported Version Ranges</td>
 </tr>
 <tr>
 <td>interface_select_method</td>
 <td><code class="docutils literal notranslate">v6.2.7 -> v6.4.0 </code></td>
 <td><code class="docutils literal notranslate">v6.4.4 -> 7.4.4 </code></td>
 </tr>
 <tr>
 <td>[auto]</td>
 <td><code class="docutils literal notranslate">v6.2.7 -> v6.4.0</code></td>
 <tr>
 <td>[sdwan]</td>
 <td><code class="docutils literal notranslate">v6.2.7 -> v6.4.0</code></td>
 <tr>
 <td>[specify]</td>
 <td><code class="docutils literal notranslate">v6.2.7 -> v6.4.0</code></td>
 </table>
 </div>
 </li>
        <li> <span class="li-head">max_log_rate</span> - Syslog maximum log rate in MBps (0 = unlimited). <span class="li-normal">type: int</span>
 <a id='label22' href="javascript:ContentClick('label23', 'label22');" onmouseover="ContentPreview('label23');" onmouseout="ContentUnpreview('label23');" title="click to collapse or expand..."> more... </a>
 <div id="label23" style="display:none">
 <table border="1">
 <tr>
 <td></td>
 <td colspan="1">Supported Version Ranges</td>
 </tr>
 <tr>
 <td>max_log_rate</td>
 <td><code class="docutils literal notranslate">v6.2.0 -> 7.4.4 </code></td>
 </tr>
 </table>
 </div>
 </li>
        <li> <span class="li-head">mode</span> - Remote syslog logging over UDP/Reliable TCP. <span class="li-normal">type: str</span> <span class="li-normal">choices: udp, legacy-reliable, reliable</span>
 <a id='label24' href="javascript:ContentClick('label25', 'label24');" onmouseover="ContentPreview('label25');" onmouseout="ContentUnpreview('label25');" title="click to collapse or expand..."> more... </a>
 <div id="label25" style="display:none">
 <table border="1">
 <tr>
 <td></td>
 <td colspan="1">Supported Version Ranges</td>
 </tr>
 <tr>
 <td>mode</td>
 <td><code class="docutils literal notranslate">v6.0.0 -> 7.4.4 </code></td>
 </tr>
 <tr>
 <td>[udp]</td>
 <td><code class="docutils literal notranslate">v6.0.0 -> 7.4.4</code></td>
 <tr>
 <td>[legacy-reliable]</td>
 <td><code class="docutils literal notranslate">v6.0.0 -> 7.4.4</code></td>
 <tr>
 <td>[reliable]</td>
 <td><code class="docutils literal notranslate">v6.0.0 -> 7.4.4</code></td>
 </table>
 </div>
 </li>
        <li> <span class="li-head">override</span> - Enable/disable override syslog settings. <span class="li-normal">type: str</span> <span class="li-normal">choices: enable, disable</span>
 <a id='label26' href="javascript:ContentClick('label27', 'label26');" onmouseover="ContentPreview('label27');" onmouseout="ContentUnpreview('label27');" title="click to collapse or expand..."> more... </a>
 <div id="label27" style="display:none">
 <table border="1">
 <tr>
 <td></td>
 <td colspan="2">Supported Version Ranges</td>
 </tr>
 <tr>
 <td>override</td>
 <td><code class="docutils literal notranslate">v6.0.0 -> v6.0.11 </code></td>
 <td><code class="docutils literal notranslate">v6.2.3 -> v6.2.3 </code></td>
 </tr>
 <tr>
 <td>[enable]</td>
 <td><code class="docutils literal notranslate">v6.0.0 -> v6.0.11</code></td>
 <tr>
 <td>[disable]</td>
 <td><code class="docutils literal notranslate">v6.0.0 -> v6.0.11</code></td>
 </table>
 </div>
 </li>
        <li> <span class="li-head">port</span> - Server listen port. <span class="li-normal">type: int</span>
 <a id='label28' href="javascript:ContentClick('label29', 'label28');" onmouseover="ContentPreview('label29');" onmouseout="ContentUnpreview('label29');" title="click to collapse or expand..."> more... </a>
 <div id="label29" style="display:none">
 <table border="1">
 <tr>
 <td></td>
 <td colspan="1">Supported Version Ranges</td>
 </tr>
 <tr>
 <td>port</td>
 <td><code class="docutils literal notranslate">v6.0.0 -> 7.4.4 </code></td>
 </tr>
 </table>
 </div>
 </li>
        <li> <span class="li-head">priority</span> - Set log transmission priority. <span class="li-normal">type: str</span> <span class="li-normal">choices: default, low</span>
 <a id='label30' href="javascript:ContentClick('label31', 'label30');" onmouseover="ContentPreview('label31');" onmouseout="ContentUnpreview('label31');" title="click to collapse or expand..."> more... </a>
 <div id="label31" style="display:none">
 <table border="1">
 <tr>
 <td></td>
 <td colspan="1">Supported Version Ranges</td>
 </tr>
 <tr>
 <td>priority</td>
 <td><code class="docutils literal notranslate">v6.2.0 -> 7.4.4 </code></td>
 </tr>
 <tr>
 <td>[default]</td>
 <td><code class="docutils literal notranslate">v6.2.0 -> 7.4.4</code></td>
 <tr>
 <td>[low]</td>
 <td><code class="docutils literal notranslate">v6.2.0 -> 7.4.4</code></td>
 </table>
 </div>
 </li>
        <li> <span class="li-head">server</span> - Address of remote syslog server. <span class="li-normal">type: str</span>
 <a id='label32' href="javascript:ContentClick('label33', 'label32');" onmouseover="ContentPreview('label33');" onmouseout="ContentUnpreview('label33');" title="click to collapse or expand..."> more... </a>
 <div id="label33" style="display:none">
 <table border="1">
 <tr>
 <td></td>
 <td colspan="1">Supported Version Ranges</td>
 </tr>
 <tr>
 <td>server</td>
 <td><code class="docutils literal notranslate">v6.0.0 -> 7.4.4 </code></td>
 </tr>
 </table>
 </div>
 </li>
        <li> <span class="li-head">source_ip</span> - Source IP address of syslog. <span class="li-normal">type: str</span>
 <a id='label34' href="javascript:ContentClick('label35', 'label34');" onmouseover="ContentPreview('label35');" onmouseout="ContentUnpreview('label35');" title="click to collapse or expand..."> more... </a>
 <div id="label35" style="display:none">
 <table border="1">
 <tr>
 <td></td>
 <td colspan="1">Supported Version Ranges</td>
 </tr>
 <tr>
 <td>source_ip</td>
 <td><code class="docutils literal notranslate">v6.0.0 -> 7.4.4 </code></td>
 </tr>
 </table>
 </div>
 </li>
        <li> <span class="li-head">ssl_min_proto_version</span> - Minimum supported protocol version for SSL/TLS connections . <span class="li-normal">type: str</span> <span class="li-normal">choices: default, SSLv3, TLSv1, TLSv1-1, TLSv1-2, TLSv1-3</span>
 <a id='label36' href="javascript:ContentClick('label37', 'label36');" onmouseover="ContentPreview('label37');" onmouseout="ContentUnpreview('label37');" title="click to collapse or expand..."> more... </a>
 <div id="label37" style="display:none">
 <table border="1">
 <tr>
 <td></td>
 <td colspan="1">Supported Version Ranges</td>
 </tr>
 <tr>
 <td>ssl_min_proto_version</td>
 <td><code class="docutils literal notranslate">v6.0.0 -> 7.4.4 </code></td>
 </tr>
 <tr>
 <td>[default]</td>
 <td><code class="docutils literal notranslate">v6.0.0 -> 7.4.4</code></td>
 <tr>
 <td>[SSLv3]</td>
 <td><code class="docutils literal notranslate">v6.0.0 -> 7.4.4</code></td>
 <tr>
 <td>[TLSv1]</td>
 <td><code class="docutils literal notranslate">v6.0.0 -> 7.4.4</code></td>
 <tr>
 <td>[TLSv1-1]</td>
 <td><code class="docutils literal notranslate">v6.0.0 -> 7.4.4</code></td>
 <tr>
 <td>[TLSv1-2]</td>
 <td><code class="docutils literal notranslate">v6.0.0 -> 7.4.4</code></td>
 <tr>
 <td>[TLSv1-3]</td>
 <td><code class="docutils literal notranslate">v7.4.1 -> 7.4.4</code></td>
 </tr>
 </table>
 </div>
 </li>
        <li> <span class="li-head">status</span> - Enable/disable remote syslog logging. <span class="li-normal">type: str</span> <span class="li-normal">choices: enable, disable</span>
 <a id='label38' href="javascript:ContentClick('label39', 'label38');" onmouseover="ContentPreview('label39');" onmouseout="ContentUnpreview('label39');" title="click to collapse or expand..."> more... </a>
 <div id="label39" style="display:none">
 <table border="1">
 <tr>
 <td></td>
 <td colspan="1">Supported Version Ranges</td>
 </tr>
 <tr>
 <td>status</td>
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
        <li> <span class="li-head">syslog_type</span> - Hidden setting index of Syslog. <span class="li-normal">type: int</span>
 <a id='label40' href="javascript:ContentClick('label41', 'label40');" onmouseover="ContentPreview('label41');" onmouseout="ContentUnpreview('label41');" title="click to collapse or expand..."> more... </a>
 <div id="label41" style="display:none">
 <table border="1">
 <tr>
 <td></td>
 <td colspan="1">Supported Version Ranges</td>
 </tr>
 <tr>
 <td>syslog_type</td>
 <td><code class="docutils literal notranslate">v6.2.3 -> v6.2.3 </code></td>
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
    
    - name: Override settings for remote syslog server.
      fortinet.fortios.fortios_log_syslogd_override_setting:
          vdom: "{{ vdom }}"
          log_syslogd_override_setting:
              certificate: "<your_own_value> (source certificate.local.name)"
              custom_field_name:
                  -
                      custom: "<your_own_value>"
                      id: "6"
                      name: "default_name_7"
              enc_algorithm: "high-medium"
              facility: "kernel"
              format: "default"
              interface: "<your_own_value> (source system.interface.name)"
              interface_select_method: "auto"
              max_log_rate: "0"
              mode: "udp"
              override: "enable"
              port: "514"
              priority: "default"
              server: "192.168.100.40"
              source_ip: "84.230.14.43"
              ssl_min_proto_version: "default"
              status: "enable"
              syslog_type: "2147483647"


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
