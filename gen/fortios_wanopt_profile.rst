:source: fortios_wanopt_profile.py

:orphan:

.. fortios_wanopt_profile:

fortios_wanopt_profile -- Configure WAN optimization profiles in Fortinet's FortiOS and FortiGate.
++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++

.. versionadded:: 2.0.0

.. contents::
   :local:
   :depth: 1


Synopsis
--------
- This module is able to configure a FortiGate or FortiOS (FOS) device by allowing the user to set and modify wanopt feature and profile category. Examples include all parameters and values need to be adjusted to datasources before usage. Tested with FOS v6.0.0



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
 <td>fortios_wanopt_profile</td>
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
    <li> <span class="li-head">wanopt_profile</span> - Configure WAN optimization profiles. <span class="li-normal">type: dict</span>
 <a id='label0' href="javascript:ContentClick('label1', 'label0');" onmouseover="ContentPreview('label1');" onmouseout="ContentUnpreview('label1');" title="click to collapse or expand..."> more... </a>
 <div id="label1" style="display:none">
 <table border="1">
 <tr>
 <td></td><td colspan="1">Supported Version Ranges</td>
 </tr>
 <tr>
 <td>wanopt_profile</td>
 <td><code class="docutils literal notranslate">v6.0.0 -> latest </code></td>
 </tr>
 </table>
 </div>
 </li>
        <ul class="ul-self">
        <li> <span class="li-head">auth_group</span> - Optionally add an authentication group to restrict access to the WAN Optimization tunnel to peers in the authentication group. Source wanopt.auth-group.name. <span class="li-normal">type: str</span>
 <a id='label2' href="javascript:ContentClick('label3', 'label2');" onmouseover="ContentPreview('label3');" onmouseout="ContentUnpreview('label3');" title="click to collapse or expand..."> more... </a>
 <div id="label3" style="display:none">
 <table border="1">
 <tr>
 <td></td>
 <td colspan="1">Supported Version Ranges</td>
 </tr>
 <tr>
 <td>auth_group</td>
 <td><code class="docutils literal notranslate">v6.0.0 -> latest </code></td>
 </tr>
 </table>
 </div>
 </li>
        <li> <span class="li-head">cifs</span> - Enable/disable CIFS (Windows sharing) WAN Optimization and configure CIFS WAN Optimization features. <span class="li-normal">type: dict</span>
 <a id='label4' href="javascript:ContentClick('label5', 'label4');" onmouseover="ContentPreview('label5');" onmouseout="ContentUnpreview('label5');" title="click to collapse or expand..."> more... </a>
 <div id="label5" style="display:none">
 <table border="1">
 <tr>
 <td></td><td colspan="1">Supported Version Ranges</td>
 </tr>
 <tr>
 <td>cifs</td>
 <td><code class="docutils literal notranslate">v6.0.0 -> latest </code></td>
 </tr>
 </table>
 </div>
 </li>
            <ul class="ul-self">
            <li> <span class="li-head">byte_caching</span> - Enable/disable byte-caching. Byte caching reduces the amount of traffic by caching file data sent across the WAN and in future serving if from the cache. <span class="li-normal">type: str</span> <span class="li-normal">choices: enable, disable</span>
 <a id='label6' href="javascript:ContentClick('label7', 'label6');" onmouseover="ContentPreview('label7');" onmouseout="ContentUnpreview('label7');" title="click to collapse or expand..."> more... </a>
 <div id="label7" style="display:none">
 <table border="1">
 <tr>
 <td></td>
 <td colspan="1">Supported Version Ranges</td>
 </tr>
 <tr>
 <td>byte_caching</td>
 <td><code class="docutils literal notranslate">v6.0.0 -> latest </code></td>
 </tr>
 <tr>
 <td>[enable]</td>
 <td><code class="docutils literal notranslate">v6.0.0 -> latest</code></td> <tr>
 <td>[disable]</td>
 <td><code class="docutils literal notranslate">v6.0.0 -> latest</code></td> </table>
 </div>
 </li>
            <li> <span class="li-head">log_traffic</span> - Enable/disable logging. <span class="li-normal">type: str</span> <span class="li-normal">choices: enable, disable</span>
 <a id='label8' href="javascript:ContentClick('label9', 'label8');" onmouseover="ContentPreview('label9');" onmouseout="ContentUnpreview('label9');" title="click to collapse or expand..."> more... </a>
 <div id="label9" style="display:none">
 <table border="1">
 <tr>
 <td></td>
 <td colspan="1">Supported Version Ranges</td>
 </tr>
 <tr>
 <td>log_traffic</td>
 <td><code class="docutils literal notranslate">v6.0.0 -> v7.2.2 </code></td>
 </tr>
 <tr>
 <td>[enable]</td>
 <td><code class="docutils literal notranslate">v6.0.0 -> latest</code></td> <tr>
 <td>[disable]</td>
 <td><code class="docutils literal notranslate">v6.0.0 -> latest</code></td> </table>
 </div>
 </li>
            <li> <span class="li-head">port</span> - Single port number or port number range for CIFS. Only packets with a destination port number that matches this port number or range are accepted by this profile. <span class="li-normal">type: int</span>
 <a id='label10' href="javascript:ContentClick('label11', 'label10');" onmouseover="ContentPreview('label11');" onmouseout="ContentUnpreview('label11');" title="click to collapse or expand..."> more... </a>
 <div id="label11" style="display:none">
 <table border="1">
 <tr>
 <td></td>
 <td colspan="1">Supported Version Ranges</td>
 </tr>
 <tr>
 <td>port</td>
 <td><code class="docutils literal notranslate">v6.0.0 -> v6.2.7 </code></td>
 </tr>
 </table>
 </div>
 </li>
            <li> <span class="li-head">prefer_chunking</span> - Select dynamic or fixed-size data chunking for WAN Optimization. <span class="li-normal">type: str</span> <span class="li-normal">choices: dynamic, fix</span>
 <a id='label12' href="javascript:ContentClick('label13', 'label12');" onmouseover="ContentPreview('label13');" onmouseout="ContentUnpreview('label13');" title="click to collapse or expand..."> more... </a>
 <div id="label13" style="display:none">
 <table border="1">
 <tr>
 <td></td>
 <td colspan="1">Supported Version Ranges</td>
 </tr>
 <tr>
 <td>prefer_chunking</td>
 <td><code class="docutils literal notranslate">v6.0.0 -> latest </code></td>
 </tr>
 <tr>
 <td>[dynamic]</td>
 <td><code class="docutils literal notranslate">v6.0.0 -> latest</code></td> <tr>
 <td>[fix]</td>
 <td><code class="docutils literal notranslate">v6.0.0 -> latest</code></td> </table>
 </div>
 </li>
            <li> <span class="li-head">protocol_opt</span> - Select protocol specific optimization or generic TCP optimization. <span class="li-normal">type: str</span> <span class="li-normal">choices: protocol, tcp</span>
 <a id='label14' href="javascript:ContentClick('label15', 'label14');" onmouseover="ContentPreview('label15');" onmouseout="ContentUnpreview('label15');" title="click to collapse or expand..."> more... </a>
 <div id="label15" style="display:none">
 <table border="1">
 <tr>
 <td></td>
 <td colspan="1">Supported Version Ranges</td>
 </tr>
 <tr>
 <td>protocol_opt</td>
 <td><code class="docutils literal notranslate">v6.4.0 -> latest </code></td>
 </tr>
 <tr>
 <td>[protocol]</td>
 <td><code class="docutils literal notranslate">v6.0.0 -> latest</code></td> <tr>
 <td>[tcp]</td>
 <td><code class="docutils literal notranslate">v6.0.0 -> latest</code></td> </table>
 </div>
 </li>
            <li> <span class="li-head">secure_tunnel</span> - Enable/disable securing the WAN Opt tunnel using SSL. Secure and non-secure tunnels use the same TCP port (7810). <span class="li-normal">type: str</span> <span class="li-normal">choices: enable, disable</span>
 <a id='label16' href="javascript:ContentClick('label17', 'label16');" onmouseover="ContentPreview('label17');" onmouseout="ContentUnpreview('label17');" title="click to collapse or expand..."> more... </a>
 <div id="label17" style="display:none">
 <table border="1">
 <tr>
 <td></td>
 <td colspan="1">Supported Version Ranges</td>
 </tr>
 <tr>
 <td>secure_tunnel</td>
 <td><code class="docutils literal notranslate">v6.0.0 -> latest </code></td>
 </tr>
 <tr>
 <td>[enable]</td>
 <td><code class="docutils literal notranslate">v6.0.0 -> latest</code></td> <tr>
 <td>[disable]</td>
 <td><code class="docutils literal notranslate">v6.0.0 -> latest</code></td> </table>
 </div>
 </li>
            <li> <span class="li-head">status</span> - Enable/disable WAN Optimization. <span class="li-normal">type: str</span> <span class="li-normal">choices: enable, disable</span>
 <a id='label18' href="javascript:ContentClick('label19', 'label18');" onmouseover="ContentPreview('label19');" onmouseout="ContentUnpreview('label19');" title="click to collapse or expand..."> more... </a>
 <div id="label19" style="display:none">
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
            <li> <span class="li-head">tunnel_sharing</span> - Tunnel sharing mode for aggressive/non-aggressive and/or interactive/non-interactive protocols. <span class="li-normal">type: str</span> <span class="li-normal">choices: shared, express-shared, private</span>
 <a id='label20' href="javascript:ContentClick('label21', 'label20');" onmouseover="ContentPreview('label21');" onmouseout="ContentUnpreview('label21');" title="click to collapse or expand..."> more... </a>
 <div id="label21" style="display:none">
 <table border="1">
 <tr>
 <td></td>
 <td colspan="1">Supported Version Ranges</td>
 </tr>
 <tr>
 <td>tunnel_sharing</td>
 <td><code class="docutils literal notranslate">v6.0.0 -> latest </code></td>
 </tr>
 <tr>
 <td>[shared]</td>
 <td><code class="docutils literal notranslate">v6.0.0 -> latest</code></td> <tr>
 <td>[express-shared]</td>
 <td><code class="docutils literal notranslate">v6.0.0 -> latest</code></td> <tr>
 <td>[private]</td>
 <td><code class="docutils literal notranslate">v6.0.0 -> latest</code></td> </table>
 </div>
 </li>
            </ul>
        <li> <span class="li-head">comments</span> - Comment. <span class="li-normal">type: str</span>
 <a id='label22' href="javascript:ContentClick('label23', 'label22');" onmouseover="ContentPreview('label23');" onmouseout="ContentUnpreview('label23');" title="click to collapse or expand..."> more... </a>
 <div id="label23" style="display:none">
 <table border="1">
 <tr>
 <td></td>
 <td colspan="1">Supported Version Ranges</td>
 </tr>
 <tr>
 <td>comments</td>
 <td><code class="docutils literal notranslate">v6.0.0 -> latest </code></td>
 </tr>
 </table>
 </div>
 </li>
        <li> <span class="li-head">ftp</span> - Enable/disable FTP WAN Optimization and configure FTP WAN Optimization features. <span class="li-normal">type: dict</span>
 <a id='label24' href="javascript:ContentClick('label25', 'label24');" onmouseover="ContentPreview('label25');" onmouseout="ContentUnpreview('label25');" title="click to collapse or expand..."> more... </a>
 <div id="label25" style="display:none">
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
            <li> <span class="li-head">byte_caching</span> - Enable/disable byte-caching. Byte caching reduces the amount of traffic by caching file data sent across the WAN and in future serving if from the cache. <span class="li-normal">type: str</span> <span class="li-normal">choices: enable, disable</span>
 <a id='label26' href="javascript:ContentClick('label27', 'label26');" onmouseover="ContentPreview('label27');" onmouseout="ContentUnpreview('label27');" title="click to collapse or expand..."> more... </a>
 <div id="label27" style="display:none">
 <table border="1">
 <tr>
 <td></td>
 <td colspan="1">Supported Version Ranges</td>
 </tr>
 <tr>
 <td>byte_caching</td>
 <td><code class="docutils literal notranslate">v6.0.0 -> latest </code></td>
 </tr>
 <tr>
 <td>[enable]</td>
 <td><code class="docutils literal notranslate">v6.0.0 -> latest</code></td> <tr>
 <td>[disable]</td>
 <td><code class="docutils literal notranslate">v6.0.0 -> latest</code></td> </table>
 </div>
 </li>
            <li> <span class="li-head">log_traffic</span> - Enable/disable logging. <span class="li-normal">type: str</span> <span class="li-normal">choices: enable, disable</span>
 <a id='label28' href="javascript:ContentClick('label29', 'label28');" onmouseover="ContentPreview('label29');" onmouseout="ContentUnpreview('label29');" title="click to collapse or expand..."> more... </a>
 <div id="label29" style="display:none">
 <table border="1">
 <tr>
 <td></td>
 <td colspan="1">Supported Version Ranges</td>
 </tr>
 <tr>
 <td>log_traffic</td>
 <td><code class="docutils literal notranslate">v6.0.0 -> v7.2.2 </code></td>
 </tr>
 <tr>
 <td>[enable]</td>
 <td><code class="docutils literal notranslate">v6.0.0 -> latest</code></td> <tr>
 <td>[disable]</td>
 <td><code class="docutils literal notranslate">v6.0.0 -> latest</code></td> </table>
 </div>
 </li>
            <li> <span class="li-head">port</span> - Single port number or port number range for FTP. Only packets with a destination port number that matches this port number or range are accepted by this profile. <span class="li-normal">type: int</span>
 <a id='label30' href="javascript:ContentClick('label31', 'label30');" onmouseover="ContentPreview('label31');" onmouseout="ContentUnpreview('label31');" title="click to collapse or expand..."> more... </a>
 <div id="label31" style="display:none">
 <table border="1">
 <tr>
 <td></td>
 <td colspan="1">Supported Version Ranges</td>
 </tr>
 <tr>
 <td>port</td>
 <td><code class="docutils literal notranslate">v6.0.0 -> v6.2.7 </code></td>
 </tr>
 </table>
 </div>
 </li>
            <li> <span class="li-head">prefer_chunking</span> - Select dynamic or fixed-size data chunking for WAN Optimization. <span class="li-normal">type: str</span> <span class="li-normal">choices: dynamic, fix</span>
 <a id='label32' href="javascript:ContentClick('label33', 'label32');" onmouseover="ContentPreview('label33');" onmouseout="ContentUnpreview('label33');" title="click to collapse or expand..."> more... </a>
 <div id="label33" style="display:none">
 <table border="1">
 <tr>
 <td></td>
 <td colspan="1">Supported Version Ranges</td>
 </tr>
 <tr>
 <td>prefer_chunking</td>
 <td><code class="docutils literal notranslate">v6.0.0 -> latest </code></td>
 </tr>
 <tr>
 <td>[dynamic]</td>
 <td><code class="docutils literal notranslate">v6.0.0 -> latest</code></td> <tr>
 <td>[fix]</td>
 <td><code class="docutils literal notranslate">v6.0.0 -> latest</code></td> </table>
 </div>
 </li>
            <li> <span class="li-head">protocol_opt</span> - Select protocol specific optimization or generic TCP optimization. <span class="li-normal">type: str</span> <span class="li-normal">choices: protocol, tcp</span>
 <a id='label34' href="javascript:ContentClick('label35', 'label34');" onmouseover="ContentPreview('label35');" onmouseout="ContentUnpreview('label35');" title="click to collapse or expand..."> more... </a>
 <div id="label35" style="display:none">
 <table border="1">
 <tr>
 <td></td>
 <td colspan="1">Supported Version Ranges</td>
 </tr>
 <tr>
 <td>protocol_opt</td>
 <td><code class="docutils literal notranslate">v6.4.0 -> latest </code></td>
 </tr>
 <tr>
 <td>[protocol]</td>
 <td><code class="docutils literal notranslate">v6.0.0 -> latest</code></td> <tr>
 <td>[tcp]</td>
 <td><code class="docutils literal notranslate">v6.0.0 -> latest</code></td> </table>
 </div>
 </li>
            <li> <span class="li-head">secure_tunnel</span> - Enable/disable securing the WAN Opt tunnel using SSL. Secure and non-secure tunnels use the same TCP port (7810). <span class="li-normal">type: str</span> <span class="li-normal">choices: enable, disable</span>
 <a id='label36' href="javascript:ContentClick('label37', 'label36');" onmouseover="ContentPreview('label37');" onmouseout="ContentUnpreview('label37');" title="click to collapse or expand..."> more... </a>
 <div id="label37" style="display:none">
 <table border="1">
 <tr>
 <td></td>
 <td colspan="1">Supported Version Ranges</td>
 </tr>
 <tr>
 <td>secure_tunnel</td>
 <td><code class="docutils literal notranslate">v6.0.0 -> latest </code></td>
 </tr>
 <tr>
 <td>[enable]</td>
 <td><code class="docutils literal notranslate">v6.0.0 -> latest</code></td> <tr>
 <td>[disable]</td>
 <td><code class="docutils literal notranslate">v6.0.0 -> latest</code></td> </table>
 </div>
 </li>
            <li> <span class="li-head">ssl</span> - Enable/disable SSL/TLS offloading (hardware acceleration) for traffic in this tunnel. <span class="li-normal">type: str</span> <span class="li-normal">choices: enable, disable</span>
 <a id='label38' href="javascript:ContentClick('label39', 'label38');" onmouseover="ContentPreview('label39');" onmouseout="ContentUnpreview('label39');" title="click to collapse or expand..."> more... </a>
 <div id="label39" style="display:none">
 <table border="1">
 <tr>
 <td></td>
 <td colspan="1">Supported Version Ranges</td>
 </tr>
 <tr>
 <td>ssl</td>
 <td><code class="docutils literal notranslate">v6.4.0 -> v7.2.2 </code></td>
 </tr>
 <tr>
 <td>[enable]</td>
 <td><code class="docutils literal notranslate">v6.0.0 -> latest</code></td> <tr>
 <td>[disable]</td>
 <td><code class="docutils literal notranslate">v6.0.0 -> latest</code></td> </table>
 </div>
 </li>
            <li> <span class="li-head">status</span> - Enable/disable WAN Optimization. <span class="li-normal">type: str</span> <span class="li-normal">choices: enable, disable</span>
 <a id='label40' href="javascript:ContentClick('label41', 'label40');" onmouseover="ContentPreview('label41');" onmouseout="ContentUnpreview('label41');" title="click to collapse or expand..."> more... </a>
 <div id="label41" style="display:none">
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
            <li> <span class="li-head">tunnel_sharing</span> - Tunnel sharing mode for aggressive/non-aggressive and/or interactive/non-interactive protocols. <span class="li-normal">type: str</span> <span class="li-normal">choices: shared, express-shared, private</span>
 <a id='label42' href="javascript:ContentClick('label43', 'label42');" onmouseover="ContentPreview('label43');" onmouseout="ContentUnpreview('label43');" title="click to collapse or expand..."> more... </a>
 <div id="label43" style="display:none">
 <table border="1">
 <tr>
 <td></td>
 <td colspan="1">Supported Version Ranges</td>
 </tr>
 <tr>
 <td>tunnel_sharing</td>
 <td><code class="docutils literal notranslate">v6.0.0 -> latest </code></td>
 </tr>
 <tr>
 <td>[shared]</td>
 <td><code class="docutils literal notranslate">v6.0.0 -> latest</code></td> <tr>
 <td>[express-shared]</td>
 <td><code class="docutils literal notranslate">v6.0.0 -> latest</code></td> <tr>
 <td>[private]</td>
 <td><code class="docutils literal notranslate">v6.0.0 -> latest</code></td> </table>
 </div>
 </li>
            </ul>
        <li> <span class="li-head">http</span> - Enable/disable HTTP WAN Optimization and configure HTTP WAN Optimization features. <span class="li-normal">type: dict</span>
 <a id='label44' href="javascript:ContentClick('label45', 'label44');" onmouseover="ContentPreview('label45');" onmouseout="ContentUnpreview('label45');" title="click to collapse or expand..."> more... </a>
 <div id="label45" style="display:none">
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
            <li> <span class="li-head">byte_caching</span> - Enable/disable byte-caching. Byte caching reduces the amount of traffic by caching file data sent across the WAN and in future serving if from the cache. <span class="li-normal">type: str</span> <span class="li-normal">choices: enable, disable</span>
 <a id='label46' href="javascript:ContentClick('label47', 'label46');" onmouseover="ContentPreview('label47');" onmouseout="ContentUnpreview('label47');" title="click to collapse or expand..."> more... </a>
 <div id="label47" style="display:none">
 <table border="1">
 <tr>
 <td></td>
 <td colspan="1">Supported Version Ranges</td>
 </tr>
 <tr>
 <td>byte_caching</td>
 <td><code class="docutils literal notranslate">v6.0.0 -> latest </code></td>
 </tr>
 <tr>
 <td>[enable]</td>
 <td><code class="docutils literal notranslate">v6.0.0 -> latest</code></td> <tr>
 <td>[disable]</td>
 <td><code class="docutils literal notranslate">v6.0.0 -> latest</code></td> </table>
 </div>
 </li>
            <li> <span class="li-head">log_traffic</span> - Enable/disable logging. <span class="li-normal">type: str</span> <span class="li-normal">choices: enable, disable</span>
 <a id='label48' href="javascript:ContentClick('label49', 'label48');" onmouseover="ContentPreview('label49');" onmouseout="ContentUnpreview('label49');" title="click to collapse or expand..."> more... </a>
 <div id="label49" style="display:none">
 <table border="1">
 <tr>
 <td></td>
 <td colspan="1">Supported Version Ranges</td>
 </tr>
 <tr>
 <td>log_traffic</td>
 <td><code class="docutils literal notranslate">v6.0.0 -> v7.2.2 </code></td>
 </tr>
 <tr>
 <td>[enable]</td>
 <td><code class="docutils literal notranslate">v6.0.0 -> latest</code></td> <tr>
 <td>[disable]</td>
 <td><code class="docutils literal notranslate">v6.0.0 -> latest</code></td> </table>
 </div>
 </li>
            <li> <span class="li-head">port</span> - Single port number or port number range for HTTP. Only packets with a destination port number that matches this port number or range are accepted by this profile. <span class="li-normal">type: int</span>
 <a id='label50' href="javascript:ContentClick('label51', 'label50');" onmouseover="ContentPreview('label51');" onmouseout="ContentUnpreview('label51');" title="click to collapse or expand..."> more... </a>
 <div id="label51" style="display:none">
 <table border="1">
 <tr>
 <td></td>
 <td colspan="1">Supported Version Ranges</td>
 </tr>
 <tr>
 <td>port</td>
 <td><code class="docutils literal notranslate">v6.0.0 -> v6.2.7 </code></td>
 </tr>
 </table>
 </div>
 </li>
            <li> <span class="li-head">prefer_chunking</span> - Select dynamic or fixed-size data chunking for WAN Optimization. <span class="li-normal">type: str</span> <span class="li-normal">choices: dynamic, fix</span>
 <a id='label52' href="javascript:ContentClick('label53', 'label52');" onmouseover="ContentPreview('label53');" onmouseout="ContentUnpreview('label53');" title="click to collapse or expand..."> more... </a>
 <div id="label53" style="display:none">
 <table border="1">
 <tr>
 <td></td>
 <td colspan="1">Supported Version Ranges</td>
 </tr>
 <tr>
 <td>prefer_chunking</td>
 <td><code class="docutils literal notranslate">v6.0.0 -> latest </code></td>
 </tr>
 <tr>
 <td>[dynamic]</td>
 <td><code class="docutils literal notranslate">v6.0.0 -> latest</code></td> <tr>
 <td>[fix]</td>
 <td><code class="docutils literal notranslate">v6.0.0 -> latest</code></td> </table>
 </div>
 </li>
            <li> <span class="li-head">protocol_opt</span> - Select protocol specific optimization or generic TCP optimization. <span class="li-normal">type: str</span> <span class="li-normal">choices: protocol, tcp</span>
 <a id='label54' href="javascript:ContentClick('label55', 'label54');" onmouseover="ContentPreview('label55');" onmouseout="ContentUnpreview('label55');" title="click to collapse or expand..."> more... </a>
 <div id="label55" style="display:none">
 <table border="1">
 <tr>
 <td></td>
 <td colspan="1">Supported Version Ranges</td>
 </tr>
 <tr>
 <td>protocol_opt</td>
 <td><code class="docutils literal notranslate">v6.4.0 -> latest </code></td>
 </tr>
 <tr>
 <td>[protocol]</td>
 <td><code class="docutils literal notranslate">v6.0.0 -> latest</code></td> <tr>
 <td>[tcp]</td>
 <td><code class="docutils literal notranslate">v6.0.0 -> latest</code></td> </table>
 </div>
 </li>
            <li> <span class="li-head">secure_tunnel</span> - Enable/disable securing the WAN Opt tunnel using SSL. Secure and non-secure tunnels use the same TCP port (7810). <span class="li-normal">type: str</span> <span class="li-normal">choices: enable, disable</span>
 <a id='label56' href="javascript:ContentClick('label57', 'label56');" onmouseover="ContentPreview('label57');" onmouseout="ContentUnpreview('label57');" title="click to collapse or expand..."> more... </a>
 <div id="label57" style="display:none">
 <table border="1">
 <tr>
 <td></td>
 <td colspan="1">Supported Version Ranges</td>
 </tr>
 <tr>
 <td>secure_tunnel</td>
 <td><code class="docutils literal notranslate">v6.0.0 -> latest </code></td>
 </tr>
 <tr>
 <td>[enable]</td>
 <td><code class="docutils literal notranslate">v6.0.0 -> latest</code></td> <tr>
 <td>[disable]</td>
 <td><code class="docutils literal notranslate">v6.0.0 -> latest</code></td> </table>
 </div>
 </li>
            <li> <span class="li-head">ssl</span> - Enable/disable SSL/TLS offloading (hardware acceleration) for traffic in this tunnel. <span class="li-normal">type: str</span> <span class="li-normal">choices: enable, disable</span>
 <a id='label58' href="javascript:ContentClick('label59', 'label58');" onmouseover="ContentPreview('label59');" onmouseout="ContentUnpreview('label59');" title="click to collapse or expand..."> more... </a>
 <div id="label59" style="display:none">
 <table border="1">
 <tr>
 <td></td>
 <td colspan="1">Supported Version Ranges</td>
 </tr>
 <tr>
 <td>ssl</td>
 <td><code class="docutils literal notranslate">v6.0.0 -> latest </code></td>
 </tr>
 <tr>
 <td>[enable]</td>
 <td><code class="docutils literal notranslate">v6.0.0 -> latest</code></td> <tr>
 <td>[disable]</td>
 <td><code class="docutils literal notranslate">v6.0.0 -> latest</code></td> </table>
 </div>
 </li>
            <li> <span class="li-head">ssl_port</span> - Port on which to expect HTTPS traffic for SSL/TLS offloading. <span class="li-normal">type: int</span>
 <a id='label60' href="javascript:ContentClick('label61', 'label60');" onmouseover="ContentPreview('label61');" onmouseout="ContentUnpreview('label61');" title="click to collapse or expand..."> more... </a>
 <div id="label61" style="display:none">
 <table border="1">
 <tr>
 <td></td>
 <td colspan="1">Supported Version Ranges</td>
 </tr>
 <tr>
 <td>ssl_port</td>
 <td><code class="docutils literal notranslate">v6.0.0 -> v6.2.7 </code></td>
 </tr>
 </table>
 </div>
 </li>
            <li> <span class="li-head">status</span> - Enable/disable WAN Optimization. <span class="li-normal">type: str</span> <span class="li-normal">choices: enable, disable</span>
 <a id='label62' href="javascript:ContentClick('label63', 'label62');" onmouseover="ContentPreview('label63');" onmouseout="ContentUnpreview('label63');" title="click to collapse or expand..."> more... </a>
 <div id="label63" style="display:none">
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
            <li> <span class="li-head">tunnel_non_http</span> - Configure how to process non-HTTP traffic when a profile configured for HTTP traffic accepts a non-HTTP session. Can occur if an application sends non-HTTP traffic using an HTTP destination port. <span class="li-normal">type: str</span> <span class="li-normal">choices: enable, disable</span>
 <a id='label64' href="javascript:ContentClick('label65', 'label64');" onmouseover="ContentPreview('label65');" onmouseout="ContentUnpreview('label65');" title="click to collapse or expand..."> more... </a>
 <div id="label65" style="display:none">
 <table border="1">
 <tr>
 <td></td>
 <td colspan="1">Supported Version Ranges</td>
 </tr>
 <tr>
 <td>tunnel_non_http</td>
 <td><code class="docutils literal notranslate">v6.0.0 -> v6.2.7 </code></td>
 </tr>
 <tr>
 <td>[enable]</td>
 <td><code class="docutils literal notranslate">v6.0.0 -> latest</code></td> <tr>
 <td>[disable]</td>
 <td><code class="docutils literal notranslate">v6.0.0 -> latest</code></td> </table>
 </div>
 </li>
            <li> <span class="li-head">tunnel_sharing</span> - Tunnel sharing mode for aggressive/non-aggressive and/or interactive/non-interactive protocols. <span class="li-normal">type: str</span> <span class="li-normal">choices: shared, express-shared, private</span>
 <a id='label66' href="javascript:ContentClick('label67', 'label66');" onmouseover="ContentPreview('label67');" onmouseout="ContentUnpreview('label67');" title="click to collapse or expand..."> more... </a>
 <div id="label67" style="display:none">
 <table border="1">
 <tr>
 <td></td>
 <td colspan="1">Supported Version Ranges</td>
 </tr>
 <tr>
 <td>tunnel_sharing</td>
 <td><code class="docutils literal notranslate">v6.0.0 -> latest </code></td>
 </tr>
 <tr>
 <td>[shared]</td>
 <td><code class="docutils literal notranslate">v6.0.0 -> latest</code></td> <tr>
 <td>[express-shared]</td>
 <td><code class="docutils literal notranslate">v6.0.0 -> latest</code></td> <tr>
 <td>[private]</td>
 <td><code class="docutils literal notranslate">v6.0.0 -> latest</code></td> </table>
 </div>
 </li>
            <li> <span class="li-head">unknown_http_version</span> - How to handle HTTP sessions that do not comply with HTTP 0.9, 1.0, or 1.1. <span class="li-normal">type: str</span> <span class="li-normal">choices: reject, tunnel, best-effort</span>
 <a id='label68' href="javascript:ContentClick('label69', 'label68');" onmouseover="ContentPreview('label69');" onmouseout="ContentUnpreview('label69');" title="click to collapse or expand..."> more... </a>
 <div id="label69" style="display:none">
 <table border="1">
 <tr>
 <td></td>
 <td colspan="1">Supported Version Ranges</td>
 </tr>
 <tr>
 <td>unknown_http_version</td>
 <td><code class="docutils literal notranslate">v6.0.0 -> v6.2.7 </code></td>
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
            </ul>
        <li> <span class="li-head">mapi</span> - Enable/disable MAPI email WAN Optimization and configure MAPI WAN Optimization features. <span class="li-normal">type: dict</span>
 <a id='label70' href="javascript:ContentClick('label71', 'label70');" onmouseover="ContentPreview('label71');" onmouseout="ContentUnpreview('label71');" title="click to collapse or expand..."> more... </a>
 <div id="label71" style="display:none">
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
            <li> <span class="li-head">byte_caching</span> - Enable/disable byte-caching. Byte caching reduces the amount of traffic by caching file data sent across the WAN and in future serving if from the cache. <span class="li-normal">type: str</span> <span class="li-normal">choices: enable, disable</span>
 <a id='label72' href="javascript:ContentClick('label73', 'label72');" onmouseover="ContentPreview('label73');" onmouseout="ContentUnpreview('label73');" title="click to collapse or expand..."> more... </a>
 <div id="label73" style="display:none">
 <table border="1">
 <tr>
 <td></td>
 <td colspan="1">Supported Version Ranges</td>
 </tr>
 <tr>
 <td>byte_caching</td>
 <td><code class="docutils literal notranslate">v6.0.0 -> latest </code></td>
 </tr>
 <tr>
 <td>[enable]</td>
 <td><code class="docutils literal notranslate">v6.0.0 -> latest</code></td> <tr>
 <td>[disable]</td>
 <td><code class="docutils literal notranslate">v6.0.0 -> latest</code></td> </table>
 </div>
 </li>
            <li> <span class="li-head">log_traffic</span> - Enable/disable logging. <span class="li-normal">type: str</span> <span class="li-normal">choices: enable, disable</span>
 <a id='label74' href="javascript:ContentClick('label75', 'label74');" onmouseover="ContentPreview('label75');" onmouseout="ContentUnpreview('label75');" title="click to collapse or expand..."> more... </a>
 <div id="label75" style="display:none">
 <table border="1">
 <tr>
 <td></td>
 <td colspan="1">Supported Version Ranges</td>
 </tr>
 <tr>
 <td>log_traffic</td>
 <td><code class="docutils literal notranslate">v6.0.0 -> v7.2.2 </code></td>
 </tr>
 <tr>
 <td>[enable]</td>
 <td><code class="docutils literal notranslate">v6.0.0 -> latest</code></td> <tr>
 <td>[disable]</td>
 <td><code class="docutils literal notranslate">v6.0.0 -> latest</code></td> </table>
 </div>
 </li>
            <li> <span class="li-head">port</span> - Single port number or port number range for MAPI. Only packets with a destination port number that matches this port number or range are accepted by this profile. <span class="li-normal">type: int</span>
 <a id='label76' href="javascript:ContentClick('label77', 'label76');" onmouseover="ContentPreview('label77');" onmouseout="ContentUnpreview('label77');" title="click to collapse or expand..."> more... </a>
 <div id="label77" style="display:none">
 <table border="1">
 <tr>
 <td></td>
 <td colspan="1">Supported Version Ranges</td>
 </tr>
 <tr>
 <td>port</td>
 <td><code class="docutils literal notranslate">v6.0.0 -> v6.2.7 </code></td>
 </tr>
 </table>
 </div>
 </li>
            <li> <span class="li-head">secure_tunnel</span> - Enable/disable securing the WAN Opt tunnel using SSL. Secure and non-secure tunnels use the same TCP port (7810). <span class="li-normal">type: str</span> <span class="li-normal">choices: enable, disable</span>
 <a id='label78' href="javascript:ContentClick('label79', 'label78');" onmouseover="ContentPreview('label79');" onmouseout="ContentUnpreview('label79');" title="click to collapse or expand..."> more... </a>
 <div id="label79" style="display:none">
 <table border="1">
 <tr>
 <td></td>
 <td colspan="1">Supported Version Ranges</td>
 </tr>
 <tr>
 <td>secure_tunnel</td>
 <td><code class="docutils literal notranslate">v6.0.0 -> latest </code></td>
 </tr>
 <tr>
 <td>[enable]</td>
 <td><code class="docutils literal notranslate">v6.0.0 -> latest</code></td> <tr>
 <td>[disable]</td>
 <td><code class="docutils literal notranslate">v6.0.0 -> latest</code></td> </table>
 </div>
 </li>
            <li> <span class="li-head">status</span> - Enable/disable WAN Optimization. <span class="li-normal">type: str</span> <span class="li-normal">choices: enable, disable</span>
 <a id='label80' href="javascript:ContentClick('label81', 'label80');" onmouseover="ContentPreview('label81');" onmouseout="ContentUnpreview('label81');" title="click to collapse or expand..."> more... </a>
 <div id="label81" style="display:none">
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
            <li> <span class="li-head">tunnel_sharing</span> - Tunnel sharing mode for aggressive/non-aggressive and/or interactive/non-interactive protocols. <span class="li-normal">type: str</span> <span class="li-normal">choices: shared, express-shared, private</span>
 <a id='label82' href="javascript:ContentClick('label83', 'label82');" onmouseover="ContentPreview('label83');" onmouseout="ContentUnpreview('label83');" title="click to collapse or expand..."> more... </a>
 <div id="label83" style="display:none">
 <table border="1">
 <tr>
 <td></td>
 <td colspan="1">Supported Version Ranges</td>
 </tr>
 <tr>
 <td>tunnel_sharing</td>
 <td><code class="docutils literal notranslate">v6.0.0 -> latest </code></td>
 </tr>
 <tr>
 <td>[shared]</td>
 <td><code class="docutils literal notranslate">v6.0.0 -> latest</code></td> <tr>
 <td>[express-shared]</td>
 <td><code class="docutils literal notranslate">v6.0.0 -> latest</code></td> <tr>
 <td>[private]</td>
 <td><code class="docutils literal notranslate">v6.0.0 -> latest</code></td> </table>
 </div>
 </li>
            </ul>
        <li> <span class="li-head">name</span> - Profile name. <span class="li-normal">type: str</span> <span class="li-required">required: true</span>
 <a id='label84' href="javascript:ContentClick('label85', 'label84');" onmouseover="ContentPreview('label85');" onmouseout="ContentUnpreview('label85');" title="click to collapse or expand..."> more... </a>
 <div id="label85" style="display:none">
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
        <li> <span class="li-head">tcp</span> - Enable/disable TCP WAN Optimization and configure TCP WAN Optimization features. <span class="li-normal">type: dict</span>
 <a id='label86' href="javascript:ContentClick('label87', 'label86');" onmouseover="ContentPreview('label87');" onmouseout="ContentUnpreview('label87');" title="click to collapse or expand..."> more... </a>
 <div id="label87" style="display:none">
 <table border="1">
 <tr>
 <td></td><td colspan="1">Supported Version Ranges</td>
 </tr>
 <tr>
 <td>tcp</td>
 <td><code class="docutils literal notranslate">v6.0.0 -> latest </code></td>
 </tr>
 </table>
 </div>
 </li>
            <ul class="ul-self">
            <li> <span class="li-head">byte_caching</span> - Enable/disable byte-caching. Byte caching reduces the amount of traffic by caching file data sent across the WAN and in future serving if from the cache. <span class="li-normal">type: str</span> <span class="li-normal">choices: enable, disable</span>
 <a id='label88' href="javascript:ContentClick('label89', 'label88');" onmouseover="ContentPreview('label89');" onmouseout="ContentUnpreview('label89');" title="click to collapse or expand..."> more... </a>
 <div id="label89" style="display:none">
 <table border="1">
 <tr>
 <td></td>
 <td colspan="1">Supported Version Ranges</td>
 </tr>
 <tr>
 <td>byte_caching</td>
 <td><code class="docutils literal notranslate">v6.0.0 -> latest </code></td>
 </tr>
 <tr>
 <td>[enable]</td>
 <td><code class="docutils literal notranslate">v6.0.0 -> latest</code></td> <tr>
 <td>[disable]</td>
 <td><code class="docutils literal notranslate">v6.0.0 -> latest</code></td> </table>
 </div>
 </li>
            <li> <span class="li-head">byte_caching_opt</span> - Select whether TCP byte-caching uses system memory only or both memory and disk space. <span class="li-normal">type: str</span> <span class="li-normal">choices: mem-only, mem-disk</span>
 <a id='label90' href="javascript:ContentClick('label91', 'label90');" onmouseover="ContentPreview('label91');" onmouseout="ContentUnpreview('label91');" title="click to collapse or expand..."> more... </a>
 <div id="label91" style="display:none">
 <table border="1">
 <tr>
 <td></td>
 <td colspan="1">Supported Version Ranges</td>
 </tr>
 <tr>
 <td>byte_caching_opt</td>
 <td><code class="docutils literal notranslate">v6.0.0 -> latest </code></td>
 </tr>
 <tr>
 <td>[mem-only]</td>
 <td><code class="docutils literal notranslate">v6.0.0 -> latest</code></td> <tr>
 <td>[mem-disk]</td>
 <td><code class="docutils literal notranslate">v6.0.0 -> latest</code></td> </table>
 </div>
 </li>
            <li> <span class="li-head">log_traffic</span> - Enable/disable logging. <span class="li-normal">type: str</span> <span class="li-normal">choices: enable, disable</span>
 <a id='label92' href="javascript:ContentClick('label93', 'label92');" onmouseover="ContentPreview('label93');" onmouseout="ContentUnpreview('label93');" title="click to collapse or expand..."> more... </a>
 <div id="label93" style="display:none">
 <table border="1">
 <tr>
 <td></td>
 <td colspan="1">Supported Version Ranges</td>
 </tr>
 <tr>
 <td>log_traffic</td>
 <td><code class="docutils literal notranslate">v6.0.0 -> v7.2.2 </code></td>
 </tr>
 <tr>
 <td>[enable]</td>
 <td><code class="docutils literal notranslate">v6.0.0 -> latest</code></td> <tr>
 <td>[disable]</td>
 <td><code class="docutils literal notranslate">v6.0.0 -> latest</code></td> </table>
 </div>
 </li>
            <li> <span class="li-head">port</span> - Port numbers or port number ranges for TCP. Only packets with a destination port number that matches this port number or range are accepted by this profile. <span class="li-normal">type: str</span>
 <a id='label94' href="javascript:ContentClick('label95', 'label94');" onmouseover="ContentPreview('label95');" onmouseout="ContentUnpreview('label95');" title="click to collapse or expand..."> more... </a>
 <div id="label95" style="display:none">
 <table border="1">
 <tr>
 <td></td>
 <td colspan="1">Supported Version Ranges</td>
 </tr>
 <tr>
 <td>port</td>
 <td><code class="docutils literal notranslate">v6.0.0 -> latest </code></td>
 </tr>
 </table>
 </div>
 </li>
            <li> <span class="li-head">secure_tunnel</span> - Enable/disable securing the WAN Opt tunnel using SSL. Secure and non-secure tunnels use the same TCP port (7810). <span class="li-normal">type: str</span> <span class="li-normal">choices: enable, disable</span>
 <a id='label96' href="javascript:ContentClick('label97', 'label96');" onmouseover="ContentPreview('label97');" onmouseout="ContentUnpreview('label97');" title="click to collapse or expand..."> more... </a>
 <div id="label97" style="display:none">
 <table border="1">
 <tr>
 <td></td>
 <td colspan="1">Supported Version Ranges</td>
 </tr>
 <tr>
 <td>secure_tunnel</td>
 <td><code class="docutils literal notranslate">v6.0.0 -> latest </code></td>
 </tr>
 <tr>
 <td>[enable]</td>
 <td><code class="docutils literal notranslate">v6.0.0 -> latest</code></td> <tr>
 <td>[disable]</td>
 <td><code class="docutils literal notranslate">v6.0.0 -> latest</code></td> </table>
 </div>
 </li>
            <li> <span class="li-head">ssl</span> - Enable/disable SSL/TLS offloading (hardware acceleration) for traffic in this tunnel. <span class="li-normal">type: str</span> <span class="li-normal">choices: enable, disable</span>
 <a id='label98' href="javascript:ContentClick('label99', 'label98');" onmouseover="ContentPreview('label99');" onmouseout="ContentUnpreview('label99');" title="click to collapse or expand..."> more... </a>
 <div id="label99" style="display:none">
 <table border="1">
 <tr>
 <td></td>
 <td colspan="1">Supported Version Ranges</td>
 </tr>
 <tr>
 <td>ssl</td>
 <td><code class="docutils literal notranslate">v6.0.0 -> latest </code></td>
 </tr>
 <tr>
 <td>[enable]</td>
 <td><code class="docutils literal notranslate">v6.0.0 -> latest</code></td> <tr>
 <td>[disable]</td>
 <td><code class="docutils literal notranslate">v6.0.0 -> latest</code></td> </table>
 </div>
 </li>
            <li> <span class="li-head">ssl_port</span> - Port numbers or port number ranges on which to expect HTTPS traffic for SSL/TLS offloading. <span class="li-normal">type: str</span>
 <a id='label100' href="javascript:ContentClick('label101', 'label100');" onmouseover="ContentPreview('label101');" onmouseout="ContentUnpreview('label101');" title="click to collapse or expand..."> more... </a>
 <div id="label101" style="display:none">
 <table border="1">
 <tr>
 <td></td>
 <td colspan="1">Supported Version Ranges</td>
 </tr>
 <tr>
 <td>ssl_port</td>
 <td><code class="docutils literal notranslate">v6.0.0 -> latest </code></td>
 </tr>
 </table>
 </div>
 </li>
            <li> <span class="li-head">status</span> - Enable/disable WAN Optimization. <span class="li-normal">type: str</span> <span class="li-normal">choices: enable, disable</span>
 <a id='label102' href="javascript:ContentClick('label103', 'label102');" onmouseover="ContentPreview('label103');" onmouseout="ContentUnpreview('label103');" title="click to collapse or expand..."> more... </a>
 <div id="label103" style="display:none">
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
            <li> <span class="li-head">tunnel_sharing</span> - Tunnel sharing mode for aggressive/non-aggressive and/or interactive/non-interactive protocols. <span class="li-normal">type: str</span> <span class="li-normal">choices: shared, express-shared, private</span>
 <a id='label104' href="javascript:ContentClick('label105', 'label104');" onmouseover="ContentPreview('label105');" onmouseout="ContentUnpreview('label105');" title="click to collapse or expand..."> more... </a>
 <div id="label105" style="display:none">
 <table border="1">
 <tr>
 <td></td>
 <td colspan="1">Supported Version Ranges</td>
 </tr>
 <tr>
 <td>tunnel_sharing</td>
 <td><code class="docutils literal notranslate">v6.0.0 -> latest </code></td>
 </tr>
 <tr>
 <td>[shared]</td>
 <td><code class="docutils literal notranslate">v6.0.0 -> latest</code></td> <tr>
 <td>[express-shared]</td>
 <td><code class="docutils literal notranslate">v6.0.0 -> latest</code></td> <tr>
 <td>[private]</td>
 <td><code class="docutils literal notranslate">v6.0.0 -> latest</code></td> </table>
 </div>
 </li>
            </ul>
        <li> <span class="li-head">transparent</span> - Enable/disable transparent mode. <span class="li-normal">type: str</span> <span class="li-normal">choices: enable, disable</span>
 <a id='label106' href="javascript:ContentClick('label107', 'label106');" onmouseover="ContentPreview('label107');" onmouseout="ContentUnpreview('label107');" title="click to collapse or expand..."> more... </a>
 <div id="label107" style="display:none">
 <table border="1">
 <tr>
 <td></td>
 <td colspan="1">Supported Version Ranges</td>
 </tr>
 <tr>
 <td>transparent</td>
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
    </ul>


Notes
-----

.. note::

   - Legacy fortiosapi has been deprecated, httpapi is the preferred way to run playbooks



Examples
--------

.. code-block:: yaml+jinja
    
    - name: Configure WAN optimization profiles.
      fortinet.fortios.fortios_wanopt_profile:
          vdom: "{{ vdom }}"
          state: "present"
          access_token: "<your_own_value>"
          wanopt_profile:
              auth_group: "<your_own_value> (source wanopt.auth-group.name)"
              cifs:
                  byte_caching: "enable"
                  log_traffic: "enable"
                  port: "32767"
                  prefer_chunking: "dynamic"
                  protocol_opt: "protocol"
                  secure_tunnel: "enable"
                  status: "enable"
                  tunnel_sharing: "shared"
              comments: "<your_own_value>"
              ftp:
                  byte_caching: "enable"
                  log_traffic: "enable"
                  port: "32767"
                  prefer_chunking: "dynamic"
                  protocol_opt: "protocol"
                  secure_tunnel: "enable"
                  ssl: "enable"
                  status: "enable"
                  tunnel_sharing: "shared"
              http:
                  byte_caching: "enable"
                  log_traffic: "enable"
                  port: "32767"
                  prefer_chunking: "dynamic"
                  protocol_opt: "protocol"
                  secure_tunnel: "enable"
                  ssl: "enable"
                  ssl_port: "32767"
                  status: "enable"
                  tunnel_non_http: "enable"
                  tunnel_sharing: "shared"
                  unknown_http_version: "reject"
              mapi:
                  byte_caching: "enable"
                  log_traffic: "enable"
                  port: "32767"
                  secure_tunnel: "enable"
                  status: "enable"
                  tunnel_sharing: "shared"
              name: "default_name_44"
              tcp:
                  byte_caching: "enable"
                  byte_caching_opt: "mem-only"
                  log_traffic: "enable"
                  port: "<your_own_value>"
                  secure_tunnel: "enable"
                  ssl: "enable"
                  ssl_port: "<your_own_value>"
                  status: "enable"
                  tunnel_sharing: "shared"
              transparent: "enable"


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
