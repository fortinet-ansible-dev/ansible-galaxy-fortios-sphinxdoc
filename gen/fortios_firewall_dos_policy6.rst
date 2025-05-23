:source: fortios_firewall_dos_policy6.py

:orphan:

.. fortios_firewall_dos_policy6:

fortios_firewall_dos_policy6 -- Configure IPv6 DoS policies in Fortinet's FortiOS and FortiGate.
++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++

.. versionadded:: 2.0.0

.. contents::
   :local:
   :depth: 1


Synopsis
--------
- This module is able to configure a FortiGate or FortiOS (FOS) device by allowing the user to set and modify firewall feature and dos_policy6 category. Examples include all parameters and values need to be adjusted to datasources before usage. Tested with FOS v6.0.0



Requirements
------------
The below requirements are needed on the host that executes this module.

- ansible>=2.15


Tips
----
Using member operation to add an element to an existing object.

FortiOS Version Compatibility
-----------------------------
Supported Version Ranges: v6.0.0 -> v7.6.2


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
    <li> <span class="li-head">firewall_dos_policy6</span> - Configure IPv6 DoS policies. <span class="li-normal">type: dict</span>
 <a id='label0' href="javascript:ContentClick('label1', 'label0');" onmouseover="ContentPreview('label1');" onmouseout="ContentUnpreview('label1');" title="click to collapse or expand..."> more... </a>
 <div id="label1" style="display:none">
 <table border="1">
 <tr>
 <td></td><td colspan="1">Supported Version Ranges</td>
 </tr>
 <tr>
 <td>firewall_dos_policy6</td>
 <td><code class="docutils literal notranslate">v6.0.0 -> 7.6.2 </code></td>
 </tr>
 </table>
 </div>
 </li>
        <ul class="ul-self">
        <li> <span class="li-head">anomaly</span> - Anomaly name. <span class="li-normal">type: list</span> <span style="font-family:'Courier New'" class="li-required">member_path: anomaly:name</span>
 <a id='label2' href="javascript:ContentClick('label3', 'label2');" onmouseover="ContentPreview('label3');" onmouseout="ContentUnpreview('label3');" title="click to collapse or expand..."> more... </a>
 <div id="label3" style="display:none">
 <table border="1">
 <tr>
 <td></td><td colspan="1">Supported Version Ranges</td>
 </tr>
 <tr>
 <td>anomaly</td>
 <td><code class="docutils literal notranslate">v6.0.0 -> 7.6.2 </code></td>
 </tr>
 </table>
 </div>
 </li>
            <ul class="ul-self">
            <li> <span class="li-head">action</span> - Action taken when the threshold is reached. <span class="li-normal">type: str</span> <span class="li-normal">choices: pass, block, proxy</span>
 <a id='label4' href="javascript:ContentClick('label5', 'label4');" onmouseover="ContentPreview('label5');" onmouseout="ContentUnpreview('label5');" title="click to collapse or expand..."> more... </a>
 <div id="label5" style="display:none">
 <table border="1">
 <tr>
 <td></td>
 <td colspan="1">Supported Version Ranges</td>
 </tr>
 <tr>
 <td>action</td>
 <td><code class="docutils literal notranslate">v6.0.0 -> 7.6.2 </code></td>
 </tr>
 <tr>
 <td>[pass]</td>
 <td><code class="docutils literal notranslate">v6.0.0 -> 7.6.2</code></td>
 <tr>
 <td>[block]</td>
 <td><code class="docutils literal notranslate">v6.0.0 -> 7.6.2</code></td>
 <tr>
 <td>[proxy]</td>
 <td><code class="docutils literal notranslate">v6.0.0 -> 7.6.2</code></td>
 </table>
 </div>
 </li>
            <li> <span class="li-head">log</span> - Enable/disable anomaly logging. <span class="li-normal">type: str</span> <span class="li-normal">choices: enable, disable</span>
 <a id='label6' href="javascript:ContentClick('label7', 'label6');" onmouseover="ContentPreview('label7');" onmouseout="ContentUnpreview('label7');" title="click to collapse or expand..."> more... </a>
 <div id="label7" style="display:none">
 <table border="1">
 <tr>
 <td></td>
 <td colspan="1">Supported Version Ranges</td>
 </tr>
 <tr>
 <td>log</td>
 <td><code class="docutils literal notranslate">v6.0.0 -> 7.6.2 </code></td>
 </tr>
 <tr>
 <td>[enable]</td>
 <td><code class="docutils literal notranslate">v6.0.0 -> 7.6.2</code></td>
 <tr>
 <td>[disable]</td>
 <td><code class="docutils literal notranslate">v6.0.0 -> 7.6.2</code></td>
 </table>
 </div>
 </li>
            <li> <span class="li-head">name</span> - Anomaly name. <span class="li-normal">type: str</span> <span class="li-required">required: true</span>
 <a id='label8' href="javascript:ContentClick('label9', 'label8');" onmouseover="ContentPreview('label9');" onmouseout="ContentUnpreview('label9');" title="click to collapse or expand..."> more... </a>
 <div id="label9" style="display:none">
 <table border="1">
 <tr>
 <td></td>
 <td colspan="1">Supported Version Ranges</td>
 </tr>
 <tr>
 <td>name</td>
 <td><code class="docutils literal notranslate">v6.0.0 -> 7.6.2 </code></td>
 </tr>
 </table>
 </div>
 </li>
            <li> <span class="li-head">quarantine</span> - Quarantine method. <span class="li-normal">type: str</span> <span class="li-normal">choices: none, attacker</span>
 <a id='label10' href="javascript:ContentClick('label11', 'label10');" onmouseover="ContentPreview('label11');" onmouseout="ContentUnpreview('label11');" title="click to collapse or expand..."> more... </a>
 <div id="label11" style="display:none">
 <table border="1">
 <tr>
 <td></td>
 <td colspan="1">Supported Version Ranges</td>
 </tr>
 <tr>
 <td>quarantine</td>
 <td><code class="docutils literal notranslate">v6.0.0 -> 7.6.2 </code></td>
 </tr>
 <tr>
 <td>[none]</td>
 <td><code class="docutils literal notranslate">v6.0.0 -> 7.6.2</code></td>
 <tr>
 <td>[attacker]</td>
 <td><code class="docutils literal notranslate">v6.0.0 -> 7.6.2</code></td>
 </table>
 </div>
 </li>
            <li> <span class="li-head">quarantine_expiry</span> - Duration of quarantine. (Format <span class="li-normal">type: str</span>
 <a id='label12' href="javascript:ContentClick('label13', 'label12');" onmouseover="ContentPreview('label13');" onmouseout="ContentUnpreview('label13');" title="click to collapse or expand..."> more... </a>
 <div id="label13" style="display:none">
 <table border="1">
 <tr>
 <td></td>
 <td colspan="1">Supported Version Ranges</td>
 </tr>
 <tr>
 <td>quarantine_expiry</td>
 <td><code class="docutils literal notranslate">v6.0.0 -> 7.6.2 </code></td>
 </tr>
 </table>
 </div>
 </li>
            <li> <span class="li-head">quarantine_log</span> - Enable/disable quarantine logging. <span class="li-normal">type: str</span> <span class="li-normal">choices: disable, enable</span>
 <a id='label14' href="javascript:ContentClick('label15', 'label14');" onmouseover="ContentPreview('label15');" onmouseout="ContentUnpreview('label15');" title="click to collapse or expand..."> more... </a>
 <div id="label15" style="display:none">
 <table border="1">
 <tr>
 <td></td>
 <td colspan="1">Supported Version Ranges</td>
 </tr>
 <tr>
 <td>quarantine_log</td>
 <td><code class="docutils literal notranslate">v6.0.0 -> 7.6.2 </code></td>
 </tr>
 <tr>
 <td>[disable]</td>
 <td><code class="docutils literal notranslate">v6.0.0 -> 7.6.2</code></td>
 <tr>
 <td>[enable]</td>
 <td><code class="docutils literal notranslate">v6.0.0 -> 7.6.2</code></td>
 </table>
 </div>
 </li>
            <li> <span class="li-head">status</span> - Enable/disable this anomaly. <span class="li-normal">type: str</span> <span class="li-normal">choices: disable, enable</span>
 <a id='label16' href="javascript:ContentClick('label17', 'label16');" onmouseover="ContentPreview('label17');" onmouseout="ContentUnpreview('label17');" title="click to collapse or expand..."> more... </a>
 <div id="label17" style="display:none">
 <table border="1">
 <tr>
 <td></td>
 <td colspan="1">Supported Version Ranges</td>
 </tr>
 <tr>
 <td>status</td>
 <td><code class="docutils literal notranslate">v6.0.0 -> 7.6.2 </code></td>
 </tr>
 <tr>
 <td>[disable]</td>
 <td><code class="docutils literal notranslate">v6.0.0 -> 7.6.2</code></td>
 <tr>
 <td>[enable]</td>
 <td><code class="docutils literal notranslate">v6.0.0 -> 7.6.2</code></td>
 </table>
 </div>
 </li>
            <li> <span class="li-head">synproxy_tcp_mss</span> - Determine TCP maximum segment size (MSS) value for packets replied by syn proxy module. <span class="li-normal">type: str</span> <span class="li-normal">choices: 0, 256, 512, 1024, 1300, 1360, 1460, 1500</span>
 <a id='label18' href="javascript:ContentClick('label19', 'label18');" onmouseover="ContentPreview('label19');" onmouseout="ContentUnpreview('label19');" title="click to collapse or expand..."> more... </a>
 <div id="label19" style="display:none">
 <table border="1">
 <tr>
 <td></td>
 <td colspan="1">Supported Version Ranges</td>
 </tr>
 <tr>
 <td>synproxy_tcp_mss</td>
 <td><code class="docutils literal notranslate">v7.4.2 -> v7.4.2 </code></td>
 </tr>
 <tr>
 <td>[0]</td>
 <td><code class="docutils literal notranslate">v7.4.2 -> v7.4.2</code></td>
 <tr>
 <td>[256]</td>
 <td><code class="docutils literal notranslate">v7.4.2 -> v7.4.2</code></td>
 <tr>
 <td>[512]</td>
 <td><code class="docutils literal notranslate">v7.4.2 -> v7.4.2</code></td>
 <tr>
 <td>[1024]</td>
 <td><code class="docutils literal notranslate">v7.4.2 -> v7.4.2</code></td>
 <tr>
 <td>[1300]</td>
 <td><code class="docutils literal notranslate">v7.4.2 -> v7.4.2</code></td>
 <tr>
 <td>[1360]</td>
 <td><code class="docutils literal notranslate">v7.4.2 -> v7.4.2</code></td>
 <tr>
 <td>[1460]</td>
 <td><code class="docutils literal notranslate">v7.4.2 -> v7.4.2</code></td>
 <tr>
 <td>[1500]</td>
 <td><code class="docutils literal notranslate">v7.4.2 -> v7.4.2</code></td>
 </table>
 </div>
 </li>
            <li> <span class="li-head">synproxy_tcp_sack</span> - enable/disable TCP selective acknowledage (SACK) for packets replied by syn proxy module. <span class="li-normal">type: str</span> <span class="li-normal">choices: enable, disable</span>
 <a id='label20' href="javascript:ContentClick('label21', 'label20');" onmouseover="ContentPreview('label21');" onmouseout="ContentUnpreview('label21');" title="click to collapse or expand..."> more... </a>
 <div id="label21" style="display:none">
 <table border="1">
 <tr>
 <td></td>
 <td colspan="1">Supported Version Ranges</td>
 </tr>
 <tr>
 <td>synproxy_tcp_sack</td>
 <td><code class="docutils literal notranslate">v7.4.2 -> v7.4.2 </code></td>
 </tr>
 <tr>
 <td>[enable]</td>
 <td><code class="docutils literal notranslate">v7.4.2 -> v7.4.2</code></td>
 <tr>
 <td>[disable]</td>
 <td><code class="docutils literal notranslate">v7.4.2 -> v7.4.2</code></td>
 </table>
 </div>
 </li>
            <li> <span class="li-head">synproxy_tcp_timestamp</span> - enable/disable TCP timestamp option for packets replied by syn proxy module. <span class="li-normal">type: str</span> <span class="li-normal">choices: enable, disable</span>
 <a id='label22' href="javascript:ContentClick('label23', 'label22');" onmouseover="ContentPreview('label23');" onmouseout="ContentUnpreview('label23');" title="click to collapse or expand..."> more... </a>
 <div id="label23" style="display:none">
 <table border="1">
 <tr>
 <td></td>
 <td colspan="1">Supported Version Ranges</td>
 </tr>
 <tr>
 <td>synproxy_tcp_timestamp</td>
 <td><code class="docutils literal notranslate">v7.4.2 -> v7.4.2 </code></td>
 </tr>
 <tr>
 <td>[enable]</td>
 <td><code class="docutils literal notranslate">v7.4.2 -> v7.4.2</code></td>
 <tr>
 <td>[disable]</td>
 <td><code class="docutils literal notranslate">v7.4.2 -> v7.4.2</code></td>
 </table>
 </div>
 </li>
            <li> <span class="li-head">synproxy_tcp_window</span> - Determine TCP Window size for packets replied by syn proxy module. <span class="li-normal">type: str</span> <span class="li-normal">choices: 4096, 8192, 16384, 32768</span>
 <a id='label24' href="javascript:ContentClick('label25', 'label24');" onmouseover="ContentPreview('label25');" onmouseout="ContentUnpreview('label25');" title="click to collapse or expand..."> more... </a>
 <div id="label25" style="display:none">
 <table border="1">
 <tr>
 <td></td>
 <td colspan="1">Supported Version Ranges</td>
 </tr>
 <tr>
 <td>synproxy_tcp_window</td>
 <td><code class="docutils literal notranslate">v7.4.2 -> v7.4.2 </code></td>
 </tr>
 <tr>
 <td>[4096]</td>
 <td><code class="docutils literal notranslate">v7.4.2 -> v7.4.2</code></td>
 <tr>
 <td>[8192]</td>
 <td><code class="docutils literal notranslate">v7.4.2 -> v7.4.2</code></td>
 <tr>
 <td>[16384]</td>
 <td><code class="docutils literal notranslate">v7.4.2 -> v7.4.2</code></td>
 <tr>
 <td>[32768]</td>
 <td><code class="docutils literal notranslate">v7.4.2 -> v7.4.2</code></td>
 </table>
 </div>
 </li>
            <li> <span class="li-head">synproxy_tcp_windowscale</span> - Determine TCP window scale option value for packets replied by syn proxy module. <span class="li-normal">type: str</span> <span class="li-normal">choices: 0, 1, 2, 3, 4, 5, 6, 7, 8, 9, 10, 11, 12, 13, 14</span>
 <a id='label26' href="javascript:ContentClick('label27', 'label26');" onmouseover="ContentPreview('label27');" onmouseout="ContentUnpreview('label27');" title="click to collapse or expand..."> more... </a>
 <div id="label27" style="display:none">
 <table border="1">
 <tr>
 <td></td>
 <td colspan="1">Supported Version Ranges</td>
 </tr>
 <tr>
 <td>synproxy_tcp_windowscale</td>
 <td><code class="docutils literal notranslate">v7.4.2 -> v7.4.2 </code></td>
 </tr>
 <tr>
 <td>[0]</td>
 <td><code class="docutils literal notranslate">v7.4.2 -> v7.4.2</code></td>
 <tr>
 <td>[1]</td>
 <td><code class="docutils literal notranslate">v7.4.2 -> v7.4.2</code></td>
 <tr>
 <td>[2]</td>
 <td><code class="docutils literal notranslate">v7.4.2 -> v7.4.2</code></td>
 <tr>
 <td>[3]</td>
 <td><code class="docutils literal notranslate">v7.4.2 -> v7.4.2</code></td>
 <tr>
 <td>[4]</td>
 <td><code class="docutils literal notranslate">v7.4.2 -> v7.4.2</code></td>
 <tr>
 <td>[5]</td>
 <td><code class="docutils literal notranslate">v7.4.2 -> v7.4.2</code></td>
 <tr>
 <td>[6]</td>
 <td><code class="docutils literal notranslate">v7.4.2 -> v7.4.2</code></td>
 <tr>
 <td>[7]</td>
 <td><code class="docutils literal notranslate">v7.4.2 -> v7.4.2</code></td>
 <tr>
 <td>[8]</td>
 <td><code class="docutils literal notranslate">v7.4.2 -> v7.4.2</code></td>
 <tr>
 <td>[9]</td>
 <td><code class="docutils literal notranslate">v7.4.2 -> v7.4.2</code></td>
 <tr>
 <td>[10]</td>
 <td><code class="docutils literal notranslate">v7.4.2 -> v7.4.2</code></td>
 <tr>
 <td>[11]</td>
 <td><code class="docutils literal notranslate">v7.4.2 -> v7.4.2</code></td>
 <tr>
 <td>[12]</td>
 <td><code class="docutils literal notranslate">v7.4.2 -> v7.4.2</code></td>
 <tr>
 <td>[13]</td>
 <td><code class="docutils literal notranslate">v7.4.2 -> v7.4.2</code></td>
 <tr>
 <td>[14]</td>
 <td><code class="docutils literal notranslate">v7.4.2 -> v7.4.2</code></td>
 </table>
 </div>
 </li>
            <li> <span class="li-head">synproxy_tos</span> - Determine TCP differentiated services code point value (type of service). <span class="li-normal">type: str</span> <span class="li-normal">choices: 0, 10, 12, 14, 18, 20, 22, 26, 28, 30, 34, 36, 38, 40, 46, 255</span>
 <a id='label28' href="javascript:ContentClick('label29', 'label28');" onmouseover="ContentPreview('label29');" onmouseout="ContentUnpreview('label29');" title="click to collapse or expand..."> more... </a>
 <div id="label29" style="display:none">
 <table border="1">
 <tr>
 <td></td>
 <td colspan="1">Supported Version Ranges</td>
 </tr>
 <tr>
 <td>synproxy_tos</td>
 <td><code class="docutils literal notranslate">v7.4.2 -> v7.4.2 </code></td>
 </tr>
 <tr>
 <td>[0]</td>
 <td><code class="docutils literal notranslate">v7.4.2 -> v7.4.2</code></td>
 <tr>
 <td>[10]</td>
 <td><code class="docutils literal notranslate">v7.4.2 -> v7.4.2</code></td>
 <tr>
 <td>[12]</td>
 <td><code class="docutils literal notranslate">v7.4.2 -> v7.4.2</code></td>
 <tr>
 <td>[14]</td>
 <td><code class="docutils literal notranslate">v7.4.2 -> v7.4.2</code></td>
 <tr>
 <td>[18]</td>
 <td><code class="docutils literal notranslate">v7.4.2 -> v7.4.2</code></td>
 <tr>
 <td>[20]</td>
 <td><code class="docutils literal notranslate">v7.4.2 -> v7.4.2</code></td>
 <tr>
 <td>[22]</td>
 <td><code class="docutils literal notranslate">v7.4.2 -> v7.4.2</code></td>
 <tr>
 <td>[26]</td>
 <td><code class="docutils literal notranslate">v7.4.2 -> v7.4.2</code></td>
 <tr>
 <td>[28]</td>
 <td><code class="docutils literal notranslate">v7.4.2 -> v7.4.2</code></td>
 <tr>
 <td>[30]</td>
 <td><code class="docutils literal notranslate">v7.4.2 -> v7.4.2</code></td>
 <tr>
 <td>[34]</td>
 <td><code class="docutils literal notranslate">v7.4.2 -> v7.4.2</code></td>
 <tr>
 <td>[36]</td>
 <td><code class="docutils literal notranslate">v7.4.2 -> v7.4.2</code></td>
 <tr>
 <td>[38]</td>
 <td><code class="docutils literal notranslate">v7.4.2 -> v7.4.2</code></td>
 <tr>
 <td>[40]</td>
 <td><code class="docutils literal notranslate">v7.4.2 -> v7.4.2</code></td>
 <tr>
 <td>[46]</td>
 <td><code class="docutils literal notranslate">v7.4.2 -> v7.4.2</code></td>
 <tr>
 <td>[255]</td>
 <td><code class="docutils literal notranslate">v7.4.2 -> v7.4.2</code></td>
 </table>
 </div>
 </li>
            <li> <span class="li-head">synproxy_ttl</span> - Determine Time to live (TTL) value for packets replied by syn proxy module. <span class="li-normal">type: str</span> <span class="li-normal">choices: 32, 64, 128, 255</span>
 <a id='label30' href="javascript:ContentClick('label31', 'label30');" onmouseover="ContentPreview('label31');" onmouseout="ContentUnpreview('label31');" title="click to collapse or expand..."> more... </a>
 <div id="label31" style="display:none">
 <table border="1">
 <tr>
 <td></td>
 <td colspan="1">Supported Version Ranges</td>
 </tr>
 <tr>
 <td>synproxy_ttl</td>
 <td><code class="docutils literal notranslate">v7.4.2 -> v7.4.2 </code></td>
 </tr>
 <tr>
 <td>[32]</td>
 <td><code class="docutils literal notranslate">v7.4.2 -> v7.4.2</code></td>
 <tr>
 <td>[64]</td>
 <td><code class="docutils literal notranslate">v7.4.2 -> v7.4.2</code></td>
 <tr>
 <td>[128]</td>
 <td><code class="docutils literal notranslate">v7.4.2 -> v7.4.2</code></td>
 <tr>
 <td>[255]</td>
 <td><code class="docutils literal notranslate">v7.4.2 -> v7.4.2</code></td>
 </table>
 </div>
 </li>
            <li> <span class="li-head">threshold</span> - Anomaly threshold. Number of detected instances (packets per second or concurrent session number) that triggers the anomaly action. <span class="li-normal">type: int</span>
 <a id='label32' href="javascript:ContentClick('label33', 'label32');" onmouseover="ContentPreview('label33');" onmouseout="ContentUnpreview('label33');" title="click to collapse or expand..."> more... </a>
 <div id="label33" style="display:none">
 <table border="1">
 <tr>
 <td></td>
 <td colspan="1">Supported Version Ranges</td>
 </tr>
 <tr>
 <td>threshold</td>
 <td><code class="docutils literal notranslate">v6.0.0 -> 7.6.2 </code></td>
 </tr>
 </table>
 </div>
 </li>
            <li> <span class="li-head">threshold_default</span> - Number of detected instances per minute which triggers action (1 - 2147483647). Note that each anomaly has a different threshold value assigned to it. <span class="li-normal">type: int</span>
 <a id='label34' href="javascript:ContentClick('label35', 'label34');" onmouseover="ContentPreview('label35');" onmouseout="ContentUnpreview('label35');" title="click to collapse or expand..."> more... </a>
 <div id="label35" style="display:none">
 <table border="1">
 <tr>
 <td></td>
 <td colspan="2">Supported Version Ranges</td>
 </tr>
 <tr>
 <td>threshold_default</td>
 <td><code class="docutils literal notranslate">v6.0.0 -> v7.0.5 </code></td>
 <td><code class="docutils literal notranslate">v7.2.0 -> v7.2.0 </code></td>
 </tr>
 </table>
 </div>
 </li>
            </ul>
        <li> <span class="li-head">comments</span> - Comment. <span class="li-normal">type: str</span>
 <a id='label36' href="javascript:ContentClick('label37', 'label36');" onmouseover="ContentPreview('label37');" onmouseout="ContentUnpreview('label37');" title="click to collapse or expand..."> more... </a>
 <div id="label37" style="display:none">
 <table border="1">
 <tr>
 <td></td>
 <td colspan="1">Supported Version Ranges</td>
 </tr>
 <tr>
 <td>comments</td>
 <td><code class="docutils literal notranslate">v6.0.0 -> 7.6.2 </code></td>
 </tr>
 </table>
 </div>
 </li>
        <li> <span class="li-head">dstaddr</span> - Destination address name from available addresses. <span class="li-normal">type: list</span> <span style="font-family:'Courier New'" class="li-required">member_path: dstaddr:name</span>
 <a id='label38' href="javascript:ContentClick('label39', 'label38');" onmouseover="ContentPreview('label39');" onmouseout="ContentUnpreview('label39');" title="click to collapse or expand..."> more... </a>
 <div id="label39" style="display:none">
 <table border="1">
 <tr>
 <td></td><td colspan="1">Supported Version Ranges</td>
 </tr>
 <tr>
 <td>dstaddr</td>
 <td><code class="docutils literal notranslate">v6.0.0 -> 7.6.2 </code></td>
 </tr>
 </table>
 </div>
 </li>
            <ul class="ul-self">
            <li> <span class="li-head">name</span> - Address name. Source firewall.address6.name firewall.addrgrp6.name. <span class="li-normal">type: str</span> <span class="li-required">required: true</span>
 <a id='label40' href="javascript:ContentClick('label41', 'label40');" onmouseover="ContentPreview('label41');" onmouseout="ContentUnpreview('label41');" title="click to collapse or expand..."> more... </a>
 <div id="label41" style="display:none">
 <table border="1">
 <tr>
 <td></td>
 <td colspan="1">Supported Version Ranges</td>
 </tr>
 <tr>
 <td>name</td>
 <td><code class="docutils literal notranslate">v6.0.0 -> 7.6.2 </code></td>
 </tr>
 </table>
 </div>
 </li>
            </ul>
        <li> <span class="li-head">interface</span> - Incoming interface name from available interfaces. Source system.zone.name system.sdwan.zone.name system.interface.name. <span class="li-normal">type: str</span>
 <a id='label42' href="javascript:ContentClick('label43', 'label42');" onmouseover="ContentPreview('label43');" onmouseout="ContentUnpreview('label43');" title="click to collapse or expand..."> more... </a>
 <div id="label43" style="display:none">
 <table border="1">
 <tr>
 <td></td>
 <td colspan="1">Supported Version Ranges</td>
 </tr>
 <tr>
 <td>interface</td>
 <td><code class="docutils literal notranslate">v6.0.0 -> 7.6.2 </code></td>
 </tr>
 </table>
 </div>
 </li>
        <li> <span class="li-head">name</span> - Policy name. <span class="li-normal">type: str</span>
 <a id='label44' href="javascript:ContentClick('label45', 'label44');" onmouseover="ContentPreview('label45');" onmouseout="ContentUnpreview('label45');" title="click to collapse or expand..."> more... </a>
 <div id="label45" style="display:none">
 <table border="1">
 <tr>
 <td></td>
 <td colspan="2">Supported Version Ranges</td>
 </tr>
 <tr>
 <td>name</td>
 <td><code class="docutils literal notranslate">v6.4.0 -> v6.4.0 </code></td>
 <td><code class="docutils literal notranslate">v6.4.4 -> 7.6.2 </code></td>
 </tr>
 </table>
 </div>
 </li>
        <li> <span class="li-head">policyid</span> - Policy ID. see <a href='#notes'>Notes</a>. <span class="li-normal">type: int</span> <span class="li-required">required: true</span>
 <a id='label46' href="javascript:ContentClick('label47', 'label46');" onmouseover="ContentPreview('label47');" onmouseout="ContentUnpreview('label47');" title="click to collapse or expand..."> more... </a>
 <div id="label47" style="display:none">
 <table border="1">
 <tr>
 <td></td>
 <td colspan="1">Supported Version Ranges</td>
 </tr>
 <tr>
 <td>policyid</td>
 <td><code class="docutils literal notranslate">v6.0.0 -> 7.6.2 </code></td>
 </tr>
 </table>
 </div>
 </li>
        <li> <span class="li-head">service</span> - Service object from available options. <span class="li-normal">type: list</span> <span style="font-family:'Courier New'" class="li-required">member_path: service:name</span>
 <a id='label48' href="javascript:ContentClick('label49', 'label48');" onmouseover="ContentPreview('label49');" onmouseout="ContentUnpreview('label49');" title="click to collapse or expand..."> more... </a>
 <div id="label49" style="display:none">
 <table border="1">
 <tr>
 <td></td><td colspan="1">Supported Version Ranges</td>
 </tr>
 <tr>
 <td>service</td>
 <td><code class="docutils literal notranslate">v6.0.0 -> 7.6.2 </code></td>
 </tr>
 </table>
 </div>
 </li>
            <ul class="ul-self">
            <li> <span class="li-head">name</span> - Service name. Source firewall.service.custom.name firewall.service.group.name. <span class="li-normal">type: str</span> <span class="li-required">required: true</span>
 <a id='label50' href="javascript:ContentClick('label51', 'label50');" onmouseover="ContentPreview('label51');" onmouseout="ContentUnpreview('label51');" title="click to collapse or expand..."> more... </a>
 <div id="label51" style="display:none">
 <table border="1">
 <tr>
 <td></td>
 <td colspan="1">Supported Version Ranges</td>
 </tr>
 <tr>
 <td>name</td>
 <td><code class="docutils literal notranslate">v6.0.0 -> 7.6.2 </code></td>
 </tr>
 </table>
 </div>
 </li>
            </ul>
        <li> <span class="li-head">srcaddr</span> - Source address name from available addresses. <span class="li-normal">type: list</span> <span style="font-family:'Courier New'" class="li-required">member_path: srcaddr:name</span>
 <a id='label52' href="javascript:ContentClick('label53', 'label52');" onmouseover="ContentPreview('label53');" onmouseout="ContentUnpreview('label53');" title="click to collapse or expand..."> more... </a>
 <div id="label53" style="display:none">
 <table border="1">
 <tr>
 <td></td><td colspan="1">Supported Version Ranges</td>
 </tr>
 <tr>
 <td>srcaddr</td>
 <td><code class="docutils literal notranslate">v6.0.0 -> 7.6.2 </code></td>
 </tr>
 </table>
 </div>
 </li>
            <ul class="ul-self">
            <li> <span class="li-head">name</span> - Address name. Source firewall.address6.name firewall.addrgrp6.name. <span class="li-normal">type: str</span> <span class="li-required">required: true</span>
 <a id='label54' href="javascript:ContentClick('label55', 'label54');" onmouseover="ContentPreview('label55');" onmouseout="ContentUnpreview('label55');" title="click to collapse or expand..."> more... </a>
 <div id="label55" style="display:none">
 <table border="1">
 <tr>
 <td></td>
 <td colspan="1">Supported Version Ranges</td>
 </tr>
 <tr>
 <td>name</td>
 <td><code class="docutils literal notranslate">v6.0.0 -> 7.6.2 </code></td>
 </tr>
 </table>
 </div>
 </li>
            </ul>
        <li> <span class="li-head">status</span> - Enable/disable this policy. <span class="li-normal">type: str</span> <span class="li-normal">choices: enable, disable</span>
 <a id='label56' href="javascript:ContentClick('label57', 'label56');" onmouseover="ContentPreview('label57');" onmouseout="ContentUnpreview('label57');" title="click to collapse or expand..."> more... </a>
 <div id="label57" style="display:none">
 <table border="1">
 <tr>
 <td></td>
 <td colspan="1">Supported Version Ranges</td>
 </tr>
 <tr>
 <td>status</td>
 <td><code class="docutils literal notranslate">v6.0.0 -> 7.6.2 </code></td>
 </tr>
 <tr>
 <td>[enable]</td>
 <td><code class="docutils literal notranslate">v6.0.0 -> 7.6.2</code></td>
 <tr>
 <td>[disable]</td>
 <td><code class="docutils literal notranslate">v6.0.0 -> 7.6.2</code></td>
 </table>
 </div>
 </li>
        </ul>
    </ul>


Notes
-----

.. note::

   - We highly recommend using your own value as the policyid instead of 0, while '0' is a special placeholder that allows the backend to assign the latest available number for the object, it does have limitations. Please find more details in Q&A.

   - Legacy fortiosapi has been deprecated, httpapi is the preferred way to run playbooks

   - The module supports check_mode.



Examples
--------

.. code-block:: yaml+jinja
    
    - name: Configure IPv6 DoS policies.
      fortinet.fortios.fortios_firewall_dos_policy6:
          vdom: "{{ vdom }}"
          state: "present"
          access_token: "<your_own_value>"
          firewall_dos_policy6:
              anomaly:
                  -
                      action: "pass"
                      log: "enable"
                      name: "default_name_6"
                      quarantine: "none"
                      quarantine_expiry: "<your_own_value>"
                      quarantine_log: "disable"
                      status: "disable"
                      synproxy_tcp_mss: "0"
                      synproxy_tcp_sack: "enable"
                      synproxy_tcp_timestamp: "enable"
                      synproxy_tcp_window: "4096"
                      synproxy_tcp_windowscale: "0"
                      synproxy_tos: "0"
                      synproxy_ttl: "32"
                      threshold: "0"
                      threshold_default: "0"
              comments: "<your_own_value>"
              dstaddr:
                  -
                      name: "default_name_22 (source firewall.address6.name firewall.addrgrp6.name)"
              interface: "<your_own_value> (source system.zone.name system.sdwan.zone.name system.interface.name)"
              name: "default_name_24"
              policyid: "<you_own_value>"
              service:
                  -
                      name: "default_name_27 (source firewall.service.custom.name firewall.service.group.name)"
              srcaddr:
                  -
                      name: "default_name_29 (source firewall.address6.name firewall.addrgrp6.name)"
              status: "enable"


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
