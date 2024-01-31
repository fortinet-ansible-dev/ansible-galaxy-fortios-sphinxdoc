:source: fortios_vpn_ssl_web_portal.py

:orphan:

.. fortios_vpn_ssl_web_portal:

fortios_vpn_ssl_web_portal -- Portal in Fortinet's FortiOS and FortiGate.
+++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++

.. versionadded:: 2.0.0

.. contents::
   :local:
   :depth: 1


Synopsis
--------
- This module is able to configure a FortiGate or FortiOS (FOS) device by allowing the user to set and modify vpn_ssl_web feature and portal category. Examples include all parameters and values need to be adjusted to datasources before usage. Tested with FOS v6.0.0



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
 <td>fortios_vpn_ssl_web_portal</td>
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
    <li> <span class="li-head">vpn_ssl_web_portal</span> - Portal. <span class="li-normal">type: dict</span>
 <a id='label0' href="javascript:ContentClick('label1', 'label0');" onmouseover="ContentPreview('label1');" onmouseout="ContentUnpreview('label1');" title="click to collapse or expand..."> more... </a>
 <div id="label1" style="display:none">
 <table border="1">
 <tr>
 <td></td><td colspan="1">Supported Version Ranges</td>
 </tr>
 <tr>
 <td>vpn_ssl_web_portal</td>
 <td><code class="docutils literal notranslate">v6.0.0 -> latest </code></td>
 </tr>
 </table>
 </div>
 </li>
        <ul class="ul-self">
        <li> <span class="li-head">allow_user_access</span> - Allow user access to SSL-VPN applications. <span class="li-normal">type: list</span> <span class="li-normal">choices: web, ftp, smb, sftp, telnet, ssh, vnc, rdp, ping, citrix, portforward</span>
 <a id='label2' href="javascript:ContentClick('label3', 'label2');" onmouseover="ContentPreview('label3');" onmouseout="ContentUnpreview('label3');" title="click to collapse or expand..."> more... </a>
 <div id="label3" style="display:none">
 <table border="1">
 <tr>
 <td></td>
 <td colspan="1">Supported Version Ranges</td>
 </tr>
 <tr>
 <td>allow_user_access</td>
 <td><code class="docutils literal notranslate">v6.0.0 -> latest </code></td>
 </tr>
 <tr>
 <td>[web]</td>
 <td><code class="docutils literal notranslate">v6.0.0 -> latest</code></td> <tr>
 <td>[ftp]</td>
 <td><code class="docutils literal notranslate">v6.0.0 -> latest</code></td> <tr>
 <td>[smb]</td>
 <td><code class="docutils literal notranslate">v6.0.0 -> latest</code></td> <tr>
 <td>[sftp]</td>
 <td><code class="docutils literal notranslate">v6.2.0 -> latest</code></td>
 </tr>
 <tr>
 <td>[telnet]</td>
 <td><code class="docutils literal notranslate">v6.0.0 -> latest</code></td> <tr>
 <td>[ssh]</td>
 <td><code class="docutils literal notranslate">v6.0.0 -> latest</code></td> <tr>
 <td>[vnc]</td>
 <td><code class="docutils literal notranslate">v6.0.0 -> latest</code></td> <tr>
 <td>[rdp]</td>
 <td><code class="docutils literal notranslate">v6.0.0 -> latest</code></td> <tr>
 <td>[ping]</td>
 <td><code class="docutils literal notranslate">v6.0.0 -> latest</code></td> <tr>
 <td>[citrix]</td>
 <td><code class="docutils literal notranslate">v6.0.0 -> v7.0.0</code></td>
 </tr>
 <tr>
 <td>[portforward]</td>
 <td><code class="docutils literal notranslate">v6.0.0 -> v7.0.0</code></td>
 </tr>
 </table>
 </div>
 </li>
        <li> <span class="li-head">auto_connect</span> - Enable/disable automatic connect by client when system is up. <span class="li-normal">type: str</span> <span class="li-normal">choices: enable, disable</span>
 <a id='label4' href="javascript:ContentClick('label5', 'label4');" onmouseover="ContentPreview('label5');" onmouseout="ContentUnpreview('label5');" title="click to collapse or expand..."> more... </a>
 <div id="label5" style="display:none">
 <table border="1">
 <tr>
 <td></td>
 <td colspan="1">Supported Version Ranges</td>
 </tr>
 <tr>
 <td>auto_connect</td>
 <td><code class="docutils literal notranslate">v6.0.0 -> latest </code></td>
 </tr>
 <tr>
 <td>[enable]</td>
 <td><code class="docutils literal notranslate">v6.0.0 -> latest</code></td> <tr>
 <td>[disable]</td>
 <td><code class="docutils literal notranslate">v6.0.0 -> latest</code></td> </table>
 </div>
 </li>
        <li> <span class="li-head">bookmark_group</span> - Portal bookmark group. <span class="li-normal">type: list</span> <span style="font-family:'Courier New'" class="li-required">member_path: bookmark_group:name</span>
 <a id='label6' href="javascript:ContentClick('label7', 'label6');" onmouseover="ContentPreview('label7');" onmouseout="ContentUnpreview('label7');" title="click to collapse or expand..."> more... </a>
 <div id="label7" style="display:none">
 <table border="1">
 <tr>
 <td></td><td colspan="1">Supported Version Ranges</td>
 </tr>
 <tr>
 <td>bookmark_group</td>
 <td><code class="docutils literal notranslate">v6.0.0 -> latest </code></td>
 </tr>
 </table>
 </div>
 </li>
            <ul class="ul-self">
            <li> <span class="li-head">bookmarks</span> - Bookmark table. <span class="li-normal">type: list</span> <span style="font-family:'Courier New'" class="li-required">member_path: bookmark_group:name/bookmarks:name</span>
 <a id='label8' href="javascript:ContentClick('label9', 'label8');" onmouseover="ContentPreview('label9');" onmouseout="ContentUnpreview('label9');" title="click to collapse or expand..."> more... </a>
 <div id="label9" style="display:none">
 <table border="1">
 <tr>
 <td></td><td colspan="1">Supported Version Ranges</td>
 </tr>
 <tr>
 <td>bookmarks</td>
 <td><code class="docutils literal notranslate">v6.0.0 -> latest </code></td>
 </tr>
 </table>
 </div>
 </li>
                <ul class="ul-self">
                <li> <span class="li-head">additional_params</span> - Additional parameters. <span class="li-normal">type: str</span>
 <a id='label10' href="javascript:ContentClick('label11', 'label10');" onmouseover="ContentPreview('label11');" onmouseout="ContentUnpreview('label11');" title="click to collapse or expand..."> more... </a>
 <div id="label11" style="display:none">
 <table border="1">
 <tr>
 <td></td>
 <td colspan="1">Supported Version Ranges</td>
 </tr>
 <tr>
 <td>additional_params</td>
 <td><code class="docutils literal notranslate">v6.0.0 -> latest </code></td>
 </tr>
 </table>
 </div>
 </li>
                <li> <span class="li-head">apptype</span> - Application type. <span class="li-normal">type: str</span> <span class="li-normal">choices: ftp, rdp, sftp, smb, ssh, telnet, vnc, web, citrix, portforward</span>
 <a id='label12' href="javascript:ContentClick('label13', 'label12');" onmouseover="ContentPreview('label13');" onmouseout="ContentUnpreview('label13');" title="click to collapse or expand..."> more... </a>
 <div id="label13" style="display:none">
 <table border="1">
 <tr>
 <td></td>
 <td colspan="1">Supported Version Ranges</td>
 </tr>
 <tr>
 <td>apptype</td>
 <td><code class="docutils literal notranslate">v6.0.0 -> latest </code></td>
 </tr>
 <tr>
 <td>[ftp]</td>
 <td><code class="docutils literal notranslate">v6.0.0 -> latest</code></td> <tr>
 <td>[rdp]</td>
 <td><code class="docutils literal notranslate">v6.0.0 -> latest</code></td> <tr>
 <td>[sftp]</td>
 <td><code class="docutils literal notranslate">v6.2.0 -> latest</code></td>
 </tr>
 <tr>
 <td>[smb]</td>
 <td><code class="docutils literal notranslate">v6.0.0 -> latest</code></td> <tr>
 <td>[ssh]</td>
 <td><code class="docutils literal notranslate">v6.0.0 -> latest</code></td> <tr>
 <td>[telnet]</td>
 <td><code class="docutils literal notranslate">v6.0.0 -> latest</code></td> <tr>
 <td>[vnc]</td>
 <td><code class="docutils literal notranslate">v6.0.0 -> latest</code></td> <tr>
 <td>[web]</td>
 <td><code class="docutils literal notranslate">v6.0.0 -> latest</code></td> <tr>
 <td>[citrix]</td>
 <td><code class="docutils literal notranslate">v6.0.0 -> v6.0.11</code></td>
 </tr>
 <tr>
 <td>[portforward]</td>
 <td><code class="docutils literal notranslate">v6.0.0 -> v6.0.11</code></td>
 </tr>
 </table>
 </div>
 </li>
                <li> <span class="li-head">color_depth</span> - Color depth per pixel. <span class="li-normal">type: str</span> <span class="li-normal">choices: 32, 16, 8</span>
 <a id='label14' href="javascript:ContentClick('label15', 'label14');" onmouseover="ContentPreview('label15');" onmouseout="ContentUnpreview('label15');" title="click to collapse or expand..."> more... </a>
 <div id="label15" style="display:none">
 <table border="1">
 <tr>
 <td></td>
 <td colspan="1">Supported Version Ranges</td>
 </tr>
 <tr>
 <td>color_depth</td>
 <td><code class="docutils literal notranslate">v7.0.1 -> latest </code></td>
 </tr>
 <tr>
 <td>[32]</td>
 <td><code class="docutils literal notranslate">v6.0.0 -> latest</code></td> <tr>
 <td>[16]</td>
 <td><code class="docutils literal notranslate">v6.0.0 -> latest</code></td> <tr>
 <td>[8]</td>
 <td><code class="docutils literal notranslate">v6.0.0 -> latest</code></td> </table>
 </div>
 </li>
                <li> <span class="li-head">description</span> - Description. <span class="li-normal">type: str</span>
 <a id='label16' href="javascript:ContentClick('label17', 'label16');" onmouseover="ContentPreview('label17');" onmouseout="ContentUnpreview('label17');" title="click to collapse or expand..."> more... </a>
 <div id="label17" style="display:none">
 <table border="1">
 <tr>
 <td></td>
 <td colspan="1">Supported Version Ranges</td>
 </tr>
 <tr>
 <td>description</td>
 <td><code class="docutils literal notranslate">v6.0.0 -> latest </code></td>
 </tr>
 </table>
 </div>
 </li>
                <li> <span class="li-head">domain</span> - Login domain. <span class="li-normal">type: str</span>
 <a id='label18' href="javascript:ContentClick('label19', 'label18');" onmouseover="ContentPreview('label19');" onmouseout="ContentUnpreview('label19');" title="click to collapse or expand..."> more... </a>
 <div id="label19" style="display:none">
 <table border="1">
 <tr>
 <td></td>
 <td colspan="2">Supported Version Ranges</td>
 </tr>
 <tr>
 <td>domain</td>
 <td><code class="docutils literal notranslate">v6.4.0 -> v6.4.0 </code></td>
 <td><code class="docutils literal notranslate">v6.4.4 -> latest </code></td>
 </tr>
 </table>
 </div>
 </li>
                <li> <span class="li-head">folder</span> - Network shared file folder parameter. <span class="li-normal">type: str</span>
 <a id='label20' href="javascript:ContentClick('label21', 'label20');" onmouseover="ContentPreview('label21');" onmouseout="ContentUnpreview('label21');" title="click to collapse or expand..."> more... </a>
 <div id="label21" style="display:none">
 <table border="1">
 <tr>
 <td></td>
 <td colspan="1">Supported Version Ranges</td>
 </tr>
 <tr>
 <td>folder</td>
 <td><code class="docutils literal notranslate">v6.0.0 -> latest </code></td>
 </tr>
 </table>
 </div>
 </li>
                <li> <span class="li-head">form_data</span> - Form data. <span class="li-normal">type: list</span> <span style="font-family:'Courier New'" class="li-required">member_path: bookmark_group:name/bookmarks:name/form_data:name</span>
 <a id='label22' href="javascript:ContentClick('label23', 'label22');" onmouseover="ContentPreview('label23');" onmouseout="ContentUnpreview('label23');" title="click to collapse or expand..."> more... </a>
 <div id="label23" style="display:none">
 <table border="1">
 <tr>
 <td></td><td colspan="1">Supported Version Ranges</td>
 </tr>
 <tr>
 <td>form_data</td>
 <td><code class="docutils literal notranslate">v6.0.0 -> latest </code></td>
 </tr>
 </table>
 </div>
 </li>
                    <ul class="ul-self">
                    <li> <span class="li-head">name</span> - Name. <span class="li-normal">type: str</span> <span class="li-required">required: true</span>
 <a id='label24' href="javascript:ContentClick('label25', 'label24');" onmouseover="ContentPreview('label25');" onmouseout="ContentUnpreview('label25');" title="click to collapse or expand..."> more... </a>
 <div id="label25" style="display:none">
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
                    <li> <span class="li-head">value</span> - Value. <span class="li-normal">type: str</span>
 <a id='label26' href="javascript:ContentClick('label27', 'label26');" onmouseover="ContentPreview('label27');" onmouseout="ContentUnpreview('label27');" title="click to collapse or expand..."> more... </a>
 <div id="label27" style="display:none">
 <table border="1">
 <tr>
 <td></td>
 <td colspan="1">Supported Version Ranges</td>
 </tr>
 <tr>
 <td>value</td>
 <td><code class="docutils literal notranslate">v6.0.0 -> latest </code></td>
 </tr>
 </table>
 </div>
 </li>
                    </ul>
                <li> <span class="li-head">height</span> - Screen height (range from 0 - 65535). <span class="li-normal">type: int</span>
 <a id='label28' href="javascript:ContentClick('label29', 'label28');" onmouseover="ContentPreview('label29');" onmouseout="ContentUnpreview('label29');" title="click to collapse or expand..."> more... </a>
 <div id="label29" style="display:none">
 <table border="1">
 <tr>
 <td></td>
 <td colspan="1">Supported Version Ranges</td>
 </tr>
 <tr>
 <td>height</td>
 <td><code class="docutils literal notranslate">v7.0.4 -> latest </code></td>
 </tr>
 </table>
 </div>
 </li>
                <li> <span class="li-head">host</span> - Host name/IP parameter. <span class="li-normal">type: str</span>
 <a id='label30' href="javascript:ContentClick('label31', 'label30');" onmouseover="ContentPreview('label31');" onmouseout="ContentUnpreview('label31');" title="click to collapse or expand..."> more... </a>
 <div id="label31" style="display:none">
 <table border="1">
 <tr>
 <td></td>
 <td colspan="1">Supported Version Ranges</td>
 </tr>
 <tr>
 <td>host</td>
 <td><code class="docutils literal notranslate">v6.0.0 -> latest </code></td>
 </tr>
 </table>
 </div>
 </li>
                <li> <span class="li-head">keyboard_layout</span> - Keyboard layout. <span class="li-normal">type: str</span> <span class="li-normal">choices: ar-101, ar-102, ar-102-azerty, can-mul, cz, cz-qwerty, cz-pr, da, nl, de, de-ch, de-ibm, en-uk, en-uk-ext, en-us, en-us-dvorak, es, es-var, fi, fi-sami, fr, fr-apple, fr-ca, fr-ch, fr-be, hr, hu, hu-101, it, it-142, ja, ko, la-am, lt, lt-ibm, lt-std, lav-std, lav-leg, mk, mk-std, no, no-sami, pol-214, pol-pr, pt, pt-br, pt-br-abnt2, ru, ru-mne, ru-t, sl, sv, sv-sami, tuk, tur-f, tur-q, zh-sym-sg-us, zh-sym-us, zh-tr-hk, zh-tr-mo, zh-tr-us</span>
 <a id='label32' href="javascript:ContentClick('label33', 'label32');" onmouseover="ContentPreview('label33');" onmouseout="ContentUnpreview('label33');" title="click to collapse or expand..."> more... </a>
 <div id="label33" style="display:none">
 <table border="1">
 <tr>
 <td></td>
 <td colspan="1">Supported Version Ranges</td>
 </tr>
 <tr>
 <td>keyboard_layout</td>
 <td><code class="docutils literal notranslate">v7.0.1 -> latest </code></td>
 </tr>
 <tr>
 <td>[ar-101]</td>
 <td><code class="docutils literal notranslate">v6.0.0 -> latest</code></td> <tr>
 <td>[ar-102]</td>
 <td><code class="docutils literal notranslate">v6.0.0 -> latest</code></td> <tr>
 <td>[ar-102-azerty]</td>
 <td><code class="docutils literal notranslate">v6.0.0 -> latest</code></td> <tr>
 <td>[can-mul]</td>
 <td><code class="docutils literal notranslate">v6.0.0 -> latest</code></td> <tr>
 <td>[cz]</td>
 <td><code class="docutils literal notranslate">v6.0.0 -> latest</code></td> <tr>
 <td>[cz-qwerty]</td>
 <td><code class="docutils literal notranslate">v6.0.0 -> latest</code></td> <tr>
 <td>[cz-pr]</td>
 <td><code class="docutils literal notranslate">v6.0.0 -> latest</code></td> <tr>
 <td>[da]</td>
 <td><code class="docutils literal notranslate">v6.0.0 -> latest</code></td> <tr>
 <td>[nl]</td>
 <td><code class="docutils literal notranslate">v6.0.0 -> latest</code></td> <tr>
 <td>[de]</td>
 <td><code class="docutils literal notranslate">v6.0.0 -> latest</code></td> <tr>
 <td>[de-ch]</td>
 <td><code class="docutils literal notranslate">v6.0.0 -> latest</code></td> <tr>
 <td>[de-ibm]</td>
 <td><code class="docutils literal notranslate">v6.0.0 -> latest</code></td> <tr>
 <td>[en-uk]</td>
 <td><code class="docutils literal notranslate">v6.0.0 -> latest</code></td> <tr>
 <td>[en-uk-ext]</td>
 <td><code class="docutils literal notranslate">v6.0.0 -> latest</code></td> <tr>
 <td>[en-us]</td>
 <td><code class="docutils literal notranslate">v6.0.0 -> latest</code></td> <tr>
 <td>[en-us-dvorak]</td>
 <td><code class="docutils literal notranslate">v6.0.0 -> latest</code></td> <tr>
 <td>[es]</td>
 <td><code class="docutils literal notranslate">v6.0.0 -> latest</code></td> <tr>
 <td>[es-var]</td>
 <td><code class="docutils literal notranslate">v6.0.0 -> latest</code></td> <tr>
 <td>[fi]</td>
 <td><code class="docutils literal notranslate">v6.0.0 -> latest</code></td> <tr>
 <td>[fi-sami]</td>
 <td><code class="docutils literal notranslate">v6.0.0 -> latest</code></td> <tr>
 <td>[fr]</td>
 <td><code class="docutils literal notranslate">v6.0.0 -> latest</code></td> <tr>
 <td>[fr-apple]</td>
 <td><code class="docutils literal notranslate">v7.0.6 -> latest</code></td>
 </tr>
 <tr>
 <td>[fr-ca]</td>
 <td><code class="docutils literal notranslate">v6.0.0 -> latest</code></td> <tr>
 <td>[fr-ch]</td>
 <td><code class="docutils literal notranslate">v6.0.0 -> latest</code></td> <tr>
 <td>[fr-be]</td>
 <td><code class="docutils literal notranslate">v6.0.0 -> latest</code></td> <tr>
 <td>[hr]</td>
 <td><code class="docutils literal notranslate">v6.0.0 -> latest</code></td> <tr>
 <td>[hu]</td>
 <td><code class="docutils literal notranslate">v6.0.0 -> latest</code></td> <tr>
 <td>[hu-101]</td>
 <td><code class="docutils literal notranslate">v6.0.0 -> latest</code></td> <tr>
 <td>[it]</td>
 <td><code class="docutils literal notranslate">v6.0.0 -> latest</code></td> <tr>
 <td>[it-142]</td>
 <td><code class="docutils literal notranslate">v6.0.0 -> latest</code></td> <tr>
 <td>[ja]</td>
 <td><code class="docutils literal notranslate">v6.0.0 -> latest</code></td> <tr>
 <td>[ko]</td>
 <td><code class="docutils literal notranslate">v6.0.0 -> latest</code></td> <tr>
 <td>[la-am]</td>
 <td><code class="docutils literal notranslate">v7.4.1 -> latest</code></td>
 </tr>
 <tr>
 <td>[lt]</td>
 <td><code class="docutils literal notranslate">v6.0.0 -> latest</code></td> <tr>
 <td>[lt-ibm]</td>
 <td><code class="docutils literal notranslate">v6.0.0 -> latest</code></td> <tr>
 <td>[lt-std]</td>
 <td><code class="docutils literal notranslate">v6.0.0 -> latest</code></td> <tr>
 <td>[lav-std]</td>
 <td><code class="docutils literal notranslate">v6.0.0 -> latest</code></td> <tr>
 <td>[lav-leg]</td>
 <td><code class="docutils literal notranslate">v6.0.0 -> latest</code></td> <tr>
 <td>[mk]</td>
 <td><code class="docutils literal notranslate">v6.0.0 -> latest</code></td> <tr>
 <td>[mk-std]</td>
 <td><code class="docutils literal notranslate">v6.0.0 -> latest</code></td> <tr>
 <td>[no]</td>
 <td><code class="docutils literal notranslate">v6.0.0 -> latest</code></td> <tr>
 <td>[no-sami]</td>
 <td><code class="docutils literal notranslate">v6.0.0 -> latest</code></td> <tr>
 <td>[pol-214]</td>
 <td><code class="docutils literal notranslate">v6.0.0 -> latest</code></td> <tr>
 <td>[pol-pr]</td>
 <td><code class="docutils literal notranslate">v6.0.0 -> latest</code></td> <tr>
 <td>[pt]</td>
 <td><code class="docutils literal notranslate">v6.0.0 -> latest</code></td> <tr>
 <td>[pt-br]</td>
 <td><code class="docutils literal notranslate">v6.0.0 -> latest</code></td> <tr>
 <td>[pt-br-abnt2]</td>
 <td><code class="docutils literal notranslate">v6.0.0 -> latest</code></td> <tr>
 <td>[ru]</td>
 <td><code class="docutils literal notranslate">v6.0.0 -> latest</code></td> <tr>
 <td>[ru-mne]</td>
 <td><code class="docutils literal notranslate">v6.0.0 -> latest</code></td> <tr>
 <td>[ru-t]</td>
 <td><code class="docutils literal notranslate">v6.0.0 -> latest</code></td> <tr>
 <td>[sl]</td>
 <td><code class="docutils literal notranslate">v6.0.0 -> latest</code></td> <tr>
 <td>[sv]</td>
 <td><code class="docutils literal notranslate">v6.0.0 -> latest</code></td> <tr>
 <td>[sv-sami]</td>
 <td><code class="docutils literal notranslate">v6.0.0 -> latest</code></td> <tr>
 <td>[tuk]</td>
 <td><code class="docutils literal notranslate">v6.0.0 -> latest</code></td> <tr>
 <td>[tur-f]</td>
 <td><code class="docutils literal notranslate">v6.0.0 -> latest</code></td> <tr>
 <td>[tur-q]</td>
 <td><code class="docutils literal notranslate">v6.0.0 -> latest</code></td> <tr>
 <td>[zh-sym-sg-us]</td>
 <td><code class="docutils literal notranslate">v6.0.0 -> latest</code></td> <tr>
 <td>[zh-sym-us]</td>
 <td><code class="docutils literal notranslate">v6.0.0 -> latest</code></td> <tr>
 <td>[zh-tr-hk]</td>
 <td><code class="docutils literal notranslate">v6.0.0 -> latest</code></td> <tr>
 <td>[zh-tr-mo]</td>
 <td><code class="docutils literal notranslate">v6.0.0 -> latest</code></td> <tr>
 <td>[zh-tr-us]</td>
 <td><code class="docutils literal notranslate">v6.0.0 -> latest</code></td> </table>
 </div>
 </li>
                <li> <span class="li-head">listening_port</span> - Listening port (0 - 65535). <span class="li-normal">type: int</span>
 <a id='label34' href="javascript:ContentClick('label35', 'label34');" onmouseover="ContentPreview('label35');" onmouseout="ContentUnpreview('label35');" title="click to collapse or expand..."> more... </a>
 <div id="label35" style="display:none">
 <table border="1">
 <tr>
 <td></td>
 <td colspan="1">Supported Version Ranges</td>
 </tr>
 <tr>
 <td>listening_port</td>
 <td><code class="docutils literal notranslate">v6.0.0 -> v7.0.0 </code></td>
 </tr>
 </table>
 </div>
 </li>
                <li> <span class="li-head">load_balancing_info</span> - The load balancing information or cookie which should be provided to the connection broker. <span class="li-normal">type: str</span>
 <a id='label36' href="javascript:ContentClick('label37', 'label36');" onmouseover="ContentPreview('label37');" onmouseout="ContentUnpreview('label37');" title="click to collapse or expand..."> more... </a>
 <div id="label37" style="display:none">
 <table border="1">
 <tr>
 <td></td>
 <td colspan="1">Supported Version Ranges</td>
 </tr>
 <tr>
 <td>load_balancing_info</td>
 <td><code class="docutils literal notranslate">v6.0.0 -> latest </code></td>
 </tr>
 </table>
 </div>
 </li>
                <li> <span class="li-head">logon_password</span> - Logon password. <span class="li-normal">type: str</span>
 <a id='label38' href="javascript:ContentClick('label39', 'label38');" onmouseover="ContentPreview('label39');" onmouseout="ContentUnpreview('label39');" title="click to collapse or expand..."> more... </a>
 <div id="label39" style="display:none">
 <table border="1">
 <tr>
 <td></td>
 <td colspan="1">Supported Version Ranges</td>
 </tr>
 <tr>
 <td>logon_password</td>
 <td><code class="docutils literal notranslate">v6.0.0 -> latest </code></td>
 </tr>
 </table>
 </div>
 </li>
                <li> <span class="li-head">logon_user</span> - Logon user. <span class="li-normal">type: str</span>
 <a id='label40' href="javascript:ContentClick('label41', 'label40');" onmouseover="ContentPreview('label41');" onmouseout="ContentUnpreview('label41');" title="click to collapse or expand..."> more... </a>
 <div id="label41" style="display:none">
 <table border="1">
 <tr>
 <td></td>
 <td colspan="1">Supported Version Ranges</td>
 </tr>
 <tr>
 <td>logon_user</td>
 <td><code class="docutils literal notranslate">v6.0.0 -> latest </code></td>
 </tr>
 </table>
 </div>
 </li>
                <li> <span class="li-head">name</span> - Bookmark name. <span class="li-normal">type: str</span> <span class="li-required">required: true</span>
 <a id='label42' href="javascript:ContentClick('label43', 'label42');" onmouseover="ContentPreview('label43');" onmouseout="ContentUnpreview('label43');" title="click to collapse or expand..."> more... </a>
 <div id="label43" style="display:none">
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
                <li> <span class="li-head">port</span> - Remote port. <span class="li-normal">type: int</span>
 <a id='label44' href="javascript:ContentClick('label45', 'label44');" onmouseover="ContentPreview('label45');" onmouseout="ContentUnpreview('label45');" title="click to collapse or expand..."> more... </a>
 <div id="label45" style="display:none">
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
                <li> <span class="li-head">preconnection_blob</span> - An arbitrary string which identifies the RDP source. <span class="li-normal">type: str</span>
 <a id='label46' href="javascript:ContentClick('label47', 'label46');" onmouseover="ContentPreview('label47');" onmouseout="ContentUnpreview('label47');" title="click to collapse or expand..."> more... </a>
 <div id="label47" style="display:none">
 <table border="1">
 <tr>
 <td></td>
 <td colspan="1">Supported Version Ranges</td>
 </tr>
 <tr>
 <td>preconnection_blob</td>
 <td><code class="docutils literal notranslate">v6.0.0 -> latest </code></td>
 </tr>
 </table>
 </div>
 </li>
                <li> <span class="li-head">preconnection_id</span> - The numeric ID of the RDP source (0-4294967295). <span class="li-normal">type: int</span>
 <a id='label48' href="javascript:ContentClick('label49', 'label48');" onmouseover="ContentPreview('label49');" onmouseout="ContentUnpreview('label49');" title="click to collapse or expand..."> more... </a>
 <div id="label49" style="display:none">
 <table border="1">
 <tr>
 <td></td>
 <td colspan="1">Supported Version Ranges</td>
 </tr>
 <tr>
 <td>preconnection_id</td>
 <td><code class="docutils literal notranslate">v6.0.0 -> latest </code></td>
 </tr>
 </table>
 </div>
 </li>
                <li> <span class="li-head">remote_port</span> - Remote port (0 - 65535). <span class="li-normal">type: int</span>
 <a id='label50' href="javascript:ContentClick('label51', 'label50');" onmouseover="ContentPreview('label51');" onmouseout="ContentUnpreview('label51');" title="click to collapse or expand..."> more... </a>
 <div id="label51" style="display:none">
 <table border="1">
 <tr>
 <td></td>
 <td colspan="1">Supported Version Ranges</td>
 </tr>
 <tr>
 <td>remote_port</td>
 <td><code class="docutils literal notranslate">v6.0.0 -> v7.0.0 </code></td>
 </tr>
 </table>
 </div>
 </li>
                <li> <span class="li-head">restricted_admin</span> - Enable/disable restricted admin mode for RDP. <span class="li-normal">type: str</span> <span class="li-normal">choices: enable, disable</span>
 <a id='label52' href="javascript:ContentClick('label53', 'label52');" onmouseover="ContentPreview('label53');" onmouseout="ContentUnpreview('label53');" title="click to collapse or expand..."> more... </a>
 <div id="label53" style="display:none">
 <table border="1">
 <tr>
 <td></td>
 <td colspan="1">Supported Version Ranges</td>
 </tr>
 <tr>
 <td>restricted_admin</td>
 <td><code class="docutils literal notranslate">v7.0.1 -> latest </code></td>
 </tr>
 <tr>
 <td>[enable]</td>
 <td><code class="docutils literal notranslate">v6.0.0 -> latest</code></td> <tr>
 <td>[disable]</td>
 <td><code class="docutils literal notranslate">v6.0.0 -> latest</code></td> </table>
 </div>
 </li>
                <li> <span class="li-head">security</span> - Security mode for RDP connection . <span class="li-normal">type: str</span> <span class="li-normal">choices: any, rdp, nla, tls</span>
 <a id='label54' href="javascript:ContentClick('label55', 'label54');" onmouseover="ContentPreview('label55');" onmouseout="ContentUnpreview('label55');" title="click to collapse or expand..."> more... </a>
 <div id="label55" style="display:none">
 <table border="1">
 <tr>
 <td></td>
 <td colspan="1">Supported Version Ranges</td>
 </tr>
 <tr>
 <td>security</td>
 <td><code class="docutils literal notranslate">v6.0.0 -> latest </code></td>
 </tr>
 <tr>
 <td>[any]</td>
 <td><code class="docutils literal notranslate">v6.0.0 -> latest</code></td> <tr>
 <td>[rdp]</td>
 <td><code class="docutils literal notranslate">v6.0.0 -> latest</code></td> <tr>
 <td>[nla]</td>
 <td><code class="docutils literal notranslate">v6.0.0 -> latest</code></td> <tr>
 <td>[tls]</td>
 <td><code class="docutils literal notranslate">v6.0.0 -> latest</code></td> </table>
 </div>
 </li>
                <li> <span class="li-head">send_preconnection_id</span> - Enable/disable sending of preconnection ID. <span class="li-normal">type: str</span> <span class="li-normal">choices: enable, disable</span>
 <a id='label56' href="javascript:ContentClick('label57', 'label56');" onmouseover="ContentPreview('label57');" onmouseout="ContentUnpreview('label57');" title="click to collapse or expand..."> more... </a>
 <div id="label57" style="display:none">
 <table border="1">
 <tr>
 <td></td>
 <td colspan="1">Supported Version Ranges</td>
 </tr>
 <tr>
 <td>send_preconnection_id</td>
 <td><code class="docutils literal notranslate">v7.0.1 -> latest </code></td>
 </tr>
 <tr>
 <td>[enable]</td>
 <td><code class="docutils literal notranslate">v6.0.0 -> latest</code></td> <tr>
 <td>[disable]</td>
 <td><code class="docutils literal notranslate">v6.0.0 -> latest</code></td> </table>
 </div>
 </li>
                <li> <span class="li-head">server_layout</span> - Server side keyboard layout. <span class="li-normal">type: str</span> <span class="li-normal">choices: de-de-qwertz, en-gb-qwerty, en-us-qwerty, es-es-qwerty, fr-ca-qwerty, fr-fr-azerty, fr-ch-qwertz, it-it-qwerty, ja-jp-qwerty, pt-br-qwerty, sv-se-qwerty, tr-tr-qwerty, failsafe</span>
 <a id='label58' href="javascript:ContentClick('label59', 'label58');" onmouseover="ContentPreview('label59');" onmouseout="ContentUnpreview('label59');" title="click to collapse or expand..."> more... </a>
 <div id="label59" style="display:none">
 <table border="1">
 <tr>
 <td></td>
 <td colspan="1">Supported Version Ranges</td>
 </tr>
 <tr>
 <td>server_layout</td>
 <td><code class="docutils literal notranslate">v6.0.0 -> v7.0.0 </code></td>
 </tr>
 <tr>
 <td>[de-de-qwertz]</td>
 <td><code class="docutils literal notranslate">v6.0.0 -> latest</code></td> <tr>
 <td>[en-gb-qwerty]</td>
 <td><code class="docutils literal notranslate">v6.0.0 -> latest</code></td> <tr>
 <td>[en-us-qwerty]</td>
 <td><code class="docutils literal notranslate">v6.0.0 -> latest</code></td> <tr>
 <td>[es-es-qwerty]</td>
 <td><code class="docutils literal notranslate">v6.0.0 -> latest</code></td> <tr>
 <td>[fr-ca-qwerty]</td>
 <td><code class="docutils literal notranslate">v6.2.0 -> v7.0.0</code></td>
 </tr>
 <tr>
 <td>[fr-fr-azerty]</td>
 <td><code class="docutils literal notranslate">v6.0.0 -> latest</code></td> <tr>
 <td>[fr-ch-qwertz]</td>
 <td><code class="docutils literal notranslate">v6.0.0 -> latest</code></td> <tr>
 <td>[it-it-qwerty]</td>
 <td><code class="docutils literal notranslate">v6.0.0 -> latest</code></td> <tr>
 <td>[ja-jp-qwerty]</td>
 <td><code class="docutils literal notranslate">v6.0.0 -> latest</code></td> <tr>
 <td>[pt-br-qwerty]</td>
 <td><code class="docutils literal notranslate">v6.0.0 -> latest</code></td> <tr>
 <td>[sv-se-qwerty]</td>
 <td><code class="docutils literal notranslate">v6.0.0 -> latest</code></td> <tr>
 <td>[tr-tr-qwerty]</td>
 <td><code class="docutils literal notranslate">v6.0.0 -> latest</code></td> <tr>
 <td>[failsafe]</td>
 <td><code class="docutils literal notranslate">v6.0.0 -> latest</code></td> </table>
 </div>
 </li>
                <li> <span class="li-head">show_status_window</span> - Enable/disable showing of status window. <span class="li-normal">type: str</span> <span class="li-normal">choices: enable, disable</span>
 <a id='label60' href="javascript:ContentClick('label61', 'label60');" onmouseover="ContentPreview('label61');" onmouseout="ContentUnpreview('label61');" title="click to collapse or expand..."> more... </a>
 <div id="label61" style="display:none">
 <table border="1">
 <tr>
 <td></td>
 <td colspan="1">Supported Version Ranges</td>
 </tr>
 <tr>
 <td>show_status_window</td>
 <td><code class="docutils literal notranslate">v6.0.0 -> v7.0.0 </code></td>
 </tr>
 <tr>
 <td>[enable]</td>
 <td><code class="docutils literal notranslate">v6.0.0 -> latest</code></td> <tr>
 <td>[disable]</td>
 <td><code class="docutils literal notranslate">v6.0.0 -> latest</code></td> </table>
 </div>
 </li>
                <li> <span class="li-head">sso</span> - Single sign-on. <span class="li-normal">type: str</span> <span class="li-normal">choices: disable, static, auto</span>
 <a id='label62' href="javascript:ContentClick('label63', 'label62');" onmouseover="ContentPreview('label63');" onmouseout="ContentUnpreview('label63');" title="click to collapse or expand..."> more... </a>
 <div id="label63" style="display:none">
 <table border="1">
 <tr>
 <td></td>
 <td colspan="1">Supported Version Ranges</td>
 </tr>
 <tr>
 <td>sso</td>
 <td><code class="docutils literal notranslate">v6.0.0 -> latest </code></td>
 </tr>
 <tr>
 <td>[disable]</td>
 <td><code class="docutils literal notranslate">v6.0.0 -> latest</code></td> <tr>
 <td>[static]</td>
 <td><code class="docutils literal notranslate">v6.0.0 -> latest</code></td> <tr>
 <td>[auto]</td>
 <td><code class="docutils literal notranslate">v6.0.0 -> latest</code></td> </table>
 </div>
 </li>
                <li> <span class="li-head">sso_credential</span> - Single sign-on credentials. <span class="li-normal">type: str</span> <span class="li-normal">choices: sslvpn-login, alternative</span>
 <a id='label64' href="javascript:ContentClick('label65', 'label64');" onmouseover="ContentPreview('label65');" onmouseout="ContentUnpreview('label65');" title="click to collapse or expand..."> more... </a>
 <div id="label65" style="display:none">
 <table border="1">
 <tr>
 <td></td>
 <td colspan="1">Supported Version Ranges</td>
 </tr>
 <tr>
 <td>sso_credential</td>
 <td><code class="docutils literal notranslate">v6.0.0 -> latest </code></td>
 </tr>
 <tr>
 <td>[sslvpn-login]</td>
 <td><code class="docutils literal notranslate">v6.0.0 -> latest</code></td> <tr>
 <td>[alternative]</td>
 <td><code class="docutils literal notranslate">v6.0.0 -> latest</code></td> </table>
 </div>
 </li>
                <li> <span class="li-head">sso_credential_sent_once</span> - Single sign-on credentials are only sent once to remote server. <span class="li-normal">type: str</span> <span class="li-normal">choices: enable, disable</span>
 <a id='label66' href="javascript:ContentClick('label67', 'label66');" onmouseover="ContentPreview('label67');" onmouseout="ContentUnpreview('label67');" title="click to collapse or expand..."> more... </a>
 <div id="label67" style="display:none">
 <table border="1">
 <tr>
 <td></td>
 <td colspan="1">Supported Version Ranges</td>
 </tr>
 <tr>
 <td>sso_credential_sent_once</td>
 <td><code class="docutils literal notranslate">v6.0.0 -> latest </code></td>
 </tr>
 <tr>
 <td>[enable]</td>
 <td><code class="docutils literal notranslate">v6.0.0 -> latest</code></td> <tr>
 <td>[disable]</td>
 <td><code class="docutils literal notranslate">v6.0.0 -> latest</code></td> </table>
 </div>
 </li>
                <li> <span class="li-head">sso_password</span> - SSO password. <span class="li-normal">type: str</span>
 <a id='label68' href="javascript:ContentClick('label69', 'label68');" onmouseover="ContentPreview('label69');" onmouseout="ContentUnpreview('label69');" title="click to collapse or expand..."> more... </a>
 <div id="label69" style="display:none">
 <table border="1">
 <tr>
 <td></td>
 <td colspan="1">Supported Version Ranges</td>
 </tr>
 <tr>
 <td>sso_password</td>
 <td><code class="docutils literal notranslate">v6.0.0 -> latest </code></td>
 </tr>
 </table>
 </div>
 </li>
                <li> <span class="li-head">sso_username</span> - SSO user name. <span class="li-normal">type: str</span>
 <a id='label70' href="javascript:ContentClick('label71', 'label70');" onmouseover="ContentPreview('label71');" onmouseout="ContentUnpreview('label71');" title="click to collapse or expand..."> more... </a>
 <div id="label71" style="display:none">
 <table border="1">
 <tr>
 <td></td>
 <td colspan="1">Supported Version Ranges</td>
 </tr>
 <tr>
 <td>sso_username</td>
 <td><code class="docutils literal notranslate">v6.0.0 -> latest </code></td>
 </tr>
 </table>
 </div>
 </li>
                <li> <span class="li-head">url</span> - URL parameter. <span class="li-normal">type: str</span>
 <a id='label72' href="javascript:ContentClick('label73', 'label72');" onmouseover="ContentPreview('label73');" onmouseout="ContentUnpreview('label73');" title="click to collapse or expand..."> more... </a>
 <div id="label73" style="display:none">
 <table border="1">
 <tr>
 <td></td>
 <td colspan="1">Supported Version Ranges</td>
 </tr>
 <tr>
 <td>url</td>
 <td><code class="docutils literal notranslate">v6.0.0 -> latest </code></td>
 </tr>
 </table>
 </div>
 </li>
                <li> <span class="li-head">vnc_keyboard_layout</span> - Keyboard layout. <span class="li-normal">type: str</span> <span class="li-normal">choices: default, da, nl, en-uk, en-uk-ext, fi, fr, fr-be, fr-ca-mul, de, de-ch, it, it-142, pt, pt-br-abnt2, no, gd, es, sv, us-intl</span>
 <a id='label74' href="javascript:ContentClick('label75', 'label74');" onmouseover="ContentPreview('label75');" onmouseout="ContentUnpreview('label75');" title="click to collapse or expand..."> more... </a>
 <div id="label75" style="display:none">
 <table border="1">
 <tr>
 <td></td>
 <td colspan="1">Supported Version Ranges</td>
 </tr>
 <tr>
 <td>vnc_keyboard_layout</td>
 <td><code class="docutils literal notranslate">v7.2.4 -> latest </code></td>
 </tr>
 <tr>
 <td>[default]</td>
 <td><code class="docutils literal notranslate">v6.0.0 -> latest</code></td> <tr>
 <td>[da]</td>
 <td><code class="docutils literal notranslate">v6.0.0 -> latest</code></td> <tr>
 <td>[nl]</td>
 <td><code class="docutils literal notranslate">v6.0.0 -> latest</code></td> <tr>
 <td>[en-uk]</td>
 <td><code class="docutils literal notranslate">v6.0.0 -> latest</code></td> <tr>
 <td>[en-uk-ext]</td>
 <td><code class="docutils literal notranslate">v6.0.0 -> latest</code></td> <tr>
 <td>[fi]</td>
 <td><code class="docutils literal notranslate">v6.0.0 -> latest</code></td> <tr>
 <td>[fr]</td>
 <td><code class="docutils literal notranslate">v6.0.0 -> latest</code></td> <tr>
 <td>[fr-be]</td>
 <td><code class="docutils literal notranslate">v6.0.0 -> latest</code></td> <tr>
 <td>[fr-ca-mul]</td>
 <td><code class="docutils literal notranslate">v6.0.0 -> latest</code></td> <tr>
 <td>[de]</td>
 <td><code class="docutils literal notranslate">v6.0.0 -> latest</code></td> <tr>
 <td>[de-ch]</td>
 <td><code class="docutils literal notranslate">v6.0.0 -> latest</code></td> <tr>
 <td>[it]</td>
 <td><code class="docutils literal notranslate">v6.0.0 -> latest</code></td> <tr>
 <td>[it-142]</td>
 <td><code class="docutils literal notranslate">v6.0.0 -> latest</code></td> <tr>
 <td>[pt]</td>
 <td><code class="docutils literal notranslate">v6.0.0 -> latest</code></td> <tr>
 <td>[pt-br-abnt2]</td>
 <td><code class="docutils literal notranslate">v6.0.0 -> latest</code></td> <tr>
 <td>[no]</td>
 <td><code class="docutils literal notranslate">v6.0.0 -> latest</code></td> <tr>
 <td>[gd]</td>
 <td><code class="docutils literal notranslate">v6.0.0 -> latest</code></td> <tr>
 <td>[es]</td>
 <td><code class="docutils literal notranslate">v6.0.0 -> latest</code></td> <tr>
 <td>[sv]</td>
 <td><code class="docutils literal notranslate">v6.0.0 -> latest</code></td> <tr>
 <td>[us-intl]</td>
 <td><code class="docutils literal notranslate">v6.0.0 -> latest</code></td> </table>
 </div>
 </li>
                <li> <span class="li-head">width</span> - Screen width (range from 0 - 65535). <span class="li-normal">type: int</span>
 <a id='label76' href="javascript:ContentClick('label77', 'label76');" onmouseover="ContentPreview('label77');" onmouseout="ContentUnpreview('label77');" title="click to collapse or expand..."> more... </a>
 <div id="label77" style="display:none">
 <table border="1">
 <tr>
 <td></td>
 <td colspan="1">Supported Version Ranges</td>
 </tr>
 <tr>
 <td>width</td>
 <td><code class="docutils literal notranslate">v7.0.4 -> latest </code></td>
 </tr>
 </table>
 </div>
 </li>
                </ul>
            <li> <span class="li-head">name</span> - Bookmark group name. <span class="li-normal">type: str</span> <span class="li-required">required: true</span>
 <a id='label78' href="javascript:ContentClick('label79', 'label78');" onmouseover="ContentPreview('label79');" onmouseout="ContentUnpreview('label79');" title="click to collapse or expand..."> more... </a>
 <div id="label79" style="display:none">
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
            </ul>
        <li> <span class="li-head">client_src_range</span> - Allow client to add source range for the tunnel traffic. <span class="li-normal">type: str</span> <span class="li-normal">choices: enable, disable</span>
 <a id='label80' href="javascript:ContentClick('label81', 'label80');" onmouseover="ContentPreview('label81');" onmouseout="ContentUnpreview('label81');" title="click to collapse or expand..."> more... </a>
 <div id="label81" style="display:none">
 <table border="1">
 <tr>
 <td></td>
 <td colspan="1">Supported Version Ranges</td>
 </tr>
 <tr>
 <td>client_src_range</td>
 <td><code class="docutils literal notranslate">v7.2.4 -> latest </code></td>
 </tr>
 <tr>
 <td>[enable]</td>
 <td><code class="docutils literal notranslate">v6.0.0 -> latest</code></td> <tr>
 <td>[disable]</td>
 <td><code class="docutils literal notranslate">v6.0.0 -> latest</code></td> </table>
 </div>
 </li>
        <li> <span class="li-head">clipboard</span> - Enable to support RDP/VPC clipboard functionality. <span class="li-normal">type: str</span> <span class="li-normal">choices: enable, disable</span>
 <a id='label82' href="javascript:ContentClick('label83', 'label82');" onmouseover="ContentPreview('label83');" onmouseout="ContentUnpreview('label83');" title="click to collapse or expand..."> more... </a>
 <div id="label83" style="display:none">
 <table border="1">
 <tr>
 <td></td>
 <td colspan="1">Supported Version Ranges</td>
 </tr>
 <tr>
 <td>clipboard</td>
 <td><code class="docutils literal notranslate">v7.0.1 -> latest </code></td>
 </tr>
 <tr>
 <td>[enable]</td>
 <td><code class="docutils literal notranslate">v6.0.0 -> latest</code></td> <tr>
 <td>[disable]</td>
 <td><code class="docutils literal notranslate">v6.0.0 -> latest</code></td> </table>
 </div>
 </li>
        <li> <span class="li-head">custom_lang</span> - Change the web portal display language. Overrides config system global set language. You can use config system custom-language and execute system custom-language to add custom language files. Source system.custom-language.name. <span class="li-normal">type: str</span>
 <a id='label84' href="javascript:ContentClick('label85', 'label84');" onmouseover="ContentPreview('label85');" onmouseout="ContentUnpreview('label85');" title="click to collapse or expand..."> more... </a>
 <div id="label85" style="display:none">
 <table border="1">
 <tr>
 <td></td>
 <td colspan="1">Supported Version Ranges</td>
 </tr>
 <tr>
 <td>custom_lang</td>
 <td><code class="docutils literal notranslate">v6.0.0 -> latest </code></td>
 </tr>
 </table>
 </div>
 </li>
        <li> <span class="li-head">customize_forticlient_download_url</span> - Enable support of customized download URL for FortiClient. <span class="li-normal">type: str</span> <span class="li-normal">choices: enable, disable</span>
 <a id='label86' href="javascript:ContentClick('label87', 'label86');" onmouseover="ContentPreview('label87');" onmouseout="ContentUnpreview('label87');" title="click to collapse or expand..."> more... </a>
 <div id="label87" style="display:none">
 <table border="1">
 <tr>
 <td></td>
 <td colspan="1">Supported Version Ranges</td>
 </tr>
 <tr>
 <td>customize_forticlient_download_url</td>
 <td><code class="docutils literal notranslate">v6.0.0 -> latest </code></td>
 </tr>
 <tr>
 <td>[enable]</td>
 <td><code class="docutils literal notranslate">v6.0.0 -> latest</code></td> <tr>
 <td>[disable]</td>
 <td><code class="docutils literal notranslate">v6.0.0 -> latest</code></td> </table>
 </div>
 </li>
        <li> <span class="li-head">default_protocol</span> - Application type that is set by default. <span class="li-normal">type: str</span> <span class="li-normal">choices: web, ftp, telnet, smb, vnc, rdp, ssh, sftp</span>
 <a id='label88' href="javascript:ContentClick('label89', 'label88');" onmouseover="ContentPreview('label89');" onmouseout="ContentUnpreview('label89');" title="click to collapse or expand..."> more... </a>
 <div id="label89" style="display:none">
 <table border="1">
 <tr>
 <td></td>
 <td colspan="1">Supported Version Ranges</td>
 </tr>
 <tr>
 <td>default_protocol</td>
 <td><code class="docutils literal notranslate">v7.4.1 -> latest </code></td>
 </tr>
 <tr>
 <td>[web]</td>
 <td><code class="docutils literal notranslate">v6.0.0 -> latest</code></td> <tr>
 <td>[ftp]</td>
 <td><code class="docutils literal notranslate">v6.0.0 -> latest</code></td> <tr>
 <td>[telnet]</td>
 <td><code class="docutils literal notranslate">v6.0.0 -> latest</code></td> <tr>
 <td>[smb]</td>
 <td><code class="docutils literal notranslate">v6.0.0 -> latest</code></td> <tr>
 <td>[vnc]</td>
 <td><code class="docutils literal notranslate">v6.0.0 -> latest</code></td> <tr>
 <td>[rdp]</td>
 <td><code class="docutils literal notranslate">v6.0.0 -> latest</code></td> <tr>
 <td>[ssh]</td>
 <td><code class="docutils literal notranslate">v6.0.0 -> latest</code></td> <tr>
 <td>[sftp]</td>
 <td><code class="docutils literal notranslate">v6.0.0 -> latest</code></td> </table>
 </div>
 </li>
        <li> <span class="li-head">default_window_height</span> - Screen height (range from 0 - 65535). <span class="li-normal">type: int</span>
 <a id='label90' href="javascript:ContentClick('label91', 'label90');" onmouseover="ContentPreview('label91');" onmouseout="ContentUnpreview('label91');" title="click to collapse or expand..."> more... </a>
 <div id="label91" style="display:none">
 <table border="1">
 <tr>
 <td></td>
 <td colspan="1">Supported Version Ranges</td>
 </tr>
 <tr>
 <td>default_window_height</td>
 <td><code class="docutils literal notranslate">v7.0.6 -> latest </code></td>
 </tr>
 </table>
 </div>
 </li>
        <li> <span class="li-head">default_window_width</span> - Screen width (range from 0 - 65535). <span class="li-normal">type: int</span>
 <a id='label92' href="javascript:ContentClick('label93', 'label92');" onmouseover="ContentPreview('label93');" onmouseout="ContentUnpreview('label93');" title="click to collapse or expand..."> more... </a>
 <div id="label93" style="display:none">
 <table border="1">
 <tr>
 <td></td>
 <td colspan="1">Supported Version Ranges</td>
 </tr>
 <tr>
 <td>default_window_width</td>
 <td><code class="docutils literal notranslate">v7.0.6 -> latest </code></td>
 </tr>
 </table>
 </div>
 </li>
        <li> <span class="li-head">dhcp_ip_overlap</span> - Configure overlapping DHCP IP allocation assignment. <span class="li-normal">type: str</span> <span class="li-normal">choices: use-new, use-old</span>
 <a id='label94' href="javascript:ContentClick('label95', 'label94');" onmouseover="ContentPreview('label95');" onmouseout="ContentUnpreview('label95');" title="click to collapse or expand..."> more... </a>
 <div id="label95" style="display:none">
 <table border="1">
 <tr>
 <td></td>
 <td colspan="2">Supported Version Ranges</td>
 </tr>
 <tr>
 <td>dhcp_ip_overlap</td>
 <td><code class="docutils literal notranslate">v7.0.6 -> v7.0.12 </code></td>
 <td><code class="docutils literal notranslate">v7.2.1 -> latest </code></td>
 </tr>
 <tr>
 <td>[use-new]</td>
 <td><code class="docutils literal notranslate">v6.0.0 -> latest</code></td> <tr>
 <td>[use-old]</td>
 <td><code class="docutils literal notranslate">v6.0.0 -> latest</code></td> </table>
 </div>
 </li>
        <li> <span class="li-head">dhcp_ra_giaddr</span> - Relay agent gateway IP address to use in the giaddr field of DHCP requests. <span class="li-normal">type: str</span>
 <a id='label96' href="javascript:ContentClick('label97', 'label96');" onmouseover="ContentPreview('label97');" onmouseout="ContentUnpreview('label97');" title="click to collapse or expand..."> more... </a>
 <div id="label97" style="display:none">
 <table border="1">
 <tr>
 <td></td>
 <td colspan="1">Supported Version Ranges</td>
 </tr>
 <tr>
 <td>dhcp_ra_giaddr</td>
 <td><code class="docutils literal notranslate">v7.2.4 -> latest </code></td>
 </tr>
 </table>
 </div>
 </li>
        <li> <span class="li-head">dhcp6_ra_linkaddr</span> - Relay agent IPv6 link address to use in DHCP6 requests. <span class="li-normal">type: str</span>
 <a id='label98' href="javascript:ContentClick('label99', 'label98');" onmouseover="ContentPreview('label99');" onmouseout="ContentUnpreview('label99');" title="click to collapse or expand..."> more... </a>
 <div id="label99" style="display:none">
 <table border="1">
 <tr>
 <td></td>
 <td colspan="1">Supported Version Ranges</td>
 </tr>
 <tr>
 <td>dhcp6_ra_linkaddr</td>
 <td><code class="docutils literal notranslate">v7.2.4 -> latest </code></td>
 </tr>
 </table>
 </div>
 </li>
        <li> <span class="li-head">display_bookmark</span> - Enable to display the web portal bookmark widget. <span class="li-normal">type: str</span> <span class="li-normal">choices: enable, disable</span>
 <a id='label100' href="javascript:ContentClick('label101', 'label100');" onmouseover="ContentPreview('label101');" onmouseout="ContentUnpreview('label101');" title="click to collapse or expand..."> more... </a>
 <div id="label101" style="display:none">
 <table border="1">
 <tr>
 <td></td>
 <td colspan="1">Supported Version Ranges</td>
 </tr>
 <tr>
 <td>display_bookmark</td>
 <td><code class="docutils literal notranslate">v6.0.0 -> latest </code></td>
 </tr>
 <tr>
 <td>[enable]</td>
 <td><code class="docutils literal notranslate">v6.0.0 -> latest</code></td> <tr>
 <td>[disable]</td>
 <td><code class="docutils literal notranslate">v6.0.0 -> latest</code></td> </table>
 </div>
 </li>
        <li> <span class="li-head">display_connection_tools</span> - Enable to display the web portal connection tools widget. <span class="li-normal">type: str</span> <span class="li-normal">choices: enable, disable</span>
 <a id='label102' href="javascript:ContentClick('label103', 'label102');" onmouseover="ContentPreview('label103');" onmouseout="ContentUnpreview('label103');" title="click to collapse or expand..."> more... </a>
 <div id="label103" style="display:none">
 <table border="1">
 <tr>
 <td></td>
 <td colspan="1">Supported Version Ranges</td>
 </tr>
 <tr>
 <td>display_connection_tools</td>
 <td><code class="docutils literal notranslate">v6.0.0 -> latest </code></td>
 </tr>
 <tr>
 <td>[enable]</td>
 <td><code class="docutils literal notranslate">v6.0.0 -> latest</code></td> <tr>
 <td>[disable]</td>
 <td><code class="docutils literal notranslate">v6.0.0 -> latest</code></td> </table>
 </div>
 </li>
        <li> <span class="li-head">display_history</span> - Enable to display the web portal user login history widget. <span class="li-normal">type: str</span> <span class="li-normal">choices: enable, disable</span>
 <a id='label104' href="javascript:ContentClick('label105', 'label104');" onmouseover="ContentPreview('label105');" onmouseout="ContentUnpreview('label105');" title="click to collapse or expand..."> more... </a>
 <div id="label105" style="display:none">
 <table border="1">
 <tr>
 <td></td>
 <td colspan="1">Supported Version Ranges</td>
 </tr>
 <tr>
 <td>display_history</td>
 <td><code class="docutils literal notranslate">v6.0.0 -> latest </code></td>
 </tr>
 <tr>
 <td>[enable]</td>
 <td><code class="docutils literal notranslate">v6.0.0 -> latest</code></td> <tr>
 <td>[disable]</td>
 <td><code class="docutils literal notranslate">v6.0.0 -> latest</code></td> </table>
 </div>
 </li>
        <li> <span class="li-head">display_status</span> - Enable to display the web portal status widget. <span class="li-normal">type: str</span> <span class="li-normal">choices: enable, disable</span>
 <a id='label106' href="javascript:ContentClick('label107', 'label106');" onmouseover="ContentPreview('label107');" onmouseout="ContentUnpreview('label107');" title="click to collapse or expand..."> more... </a>
 <div id="label107" style="display:none">
 <table border="1">
 <tr>
 <td></td>
 <td colspan="1">Supported Version Ranges</td>
 </tr>
 <tr>
 <td>display_status</td>
 <td><code class="docutils literal notranslate">v6.0.0 -> latest </code></td>
 </tr>
 <tr>
 <td>[enable]</td>
 <td><code class="docutils literal notranslate">v6.0.0 -> latest</code></td> <tr>
 <td>[disable]</td>
 <td><code class="docutils literal notranslate">v6.0.0 -> latest</code></td> </table>
 </div>
 </li>
        <li> <span class="li-head">dns_server1</span> - IPv4 DNS server 1. <span class="li-normal">type: str</span>
 <a id='label108' href="javascript:ContentClick('label109', 'label108');" onmouseover="ContentPreview('label109');" onmouseout="ContentUnpreview('label109');" title="click to collapse or expand..."> more... </a>
 <div id="label109" style="display:none">
 <table border="1">
 <tr>
 <td></td>
 <td colspan="1">Supported Version Ranges</td>
 </tr>
 <tr>
 <td>dns_server1</td>
 <td><code class="docutils literal notranslate">v6.0.0 -> latest </code></td>
 </tr>
 </table>
 </div>
 </li>
        <li> <span class="li-head">dns_server2</span> - IPv4 DNS server 2. <span class="li-normal">type: str</span>
 <a id='label110' href="javascript:ContentClick('label111', 'label110');" onmouseover="ContentPreview('label111');" onmouseout="ContentUnpreview('label111');" title="click to collapse or expand..."> more... </a>
 <div id="label111" style="display:none">
 <table border="1">
 <tr>
 <td></td>
 <td colspan="1">Supported Version Ranges</td>
 </tr>
 <tr>
 <td>dns_server2</td>
 <td><code class="docutils literal notranslate">v6.0.0 -> latest </code></td>
 </tr>
 </table>
 </div>
 </li>
        <li> <span class="li-head">dns_suffix</span> - DNS suffix. <span class="li-normal">type: str</span>
 <a id='label112' href="javascript:ContentClick('label113', 'label112');" onmouseover="ContentPreview('label113');" onmouseout="ContentUnpreview('label113');" title="click to collapse or expand..."> more... </a>
 <div id="label113" style="display:none">
 <table border="1">
 <tr>
 <td></td>
 <td colspan="1">Supported Version Ranges</td>
 </tr>
 <tr>
 <td>dns_suffix</td>
 <td><code class="docutils literal notranslate">v6.0.0 -> latest </code></td>
 </tr>
 </table>
 </div>
 </li>
        <li> <span class="li-head">exclusive_routing</span> - Enable/disable all traffic go through tunnel only. <span class="li-normal">type: str</span> <span class="li-normal">choices: enable, disable</span>
 <a id='label114' href="javascript:ContentClick('label115', 'label114');" onmouseover="ContentPreview('label115');" onmouseout="ContentUnpreview('label115');" title="click to collapse or expand..."> more... </a>
 <div id="label115" style="display:none">
 <table border="1">
 <tr>
 <td></td>
 <td colspan="1">Supported Version Ranges</td>
 </tr>
 <tr>
 <td>exclusive_routing</td>
 <td><code class="docutils literal notranslate">v6.0.0 -> latest </code></td>
 </tr>
 <tr>
 <td>[enable]</td>
 <td><code class="docutils literal notranslate">v6.0.0 -> latest</code></td> <tr>
 <td>[disable]</td>
 <td><code class="docutils literal notranslate">v6.0.0 -> latest</code></td> </table>
 </div>
 </li>
        <li> <span class="li-head">focus_bookmark</span> - Enable to prioritize the placement of the bookmark section over the quick-connection section in the SSL-VPN application. <span class="li-normal">type: str</span> <span class="li-normal">choices: enable, disable</span>
 <a id='label116' href="javascript:ContentClick('label117', 'label116');" onmouseover="ContentPreview('label117');" onmouseout="ContentUnpreview('label117');" title="click to collapse or expand..."> more... </a>
 <div id="label117" style="display:none">
 <table border="1">
 <tr>
 <td></td>
 <td colspan="1">Supported Version Ranges</td>
 </tr>
 <tr>
 <td>focus_bookmark</td>
 <td><code class="docutils literal notranslate">v7.4.1 -> latest </code></td>
 </tr>
 <tr>
 <td>[enable]</td>
 <td><code class="docutils literal notranslate">v6.0.0 -> latest</code></td> <tr>
 <td>[disable]</td>
 <td><code class="docutils literal notranslate">v6.0.0 -> latest</code></td> </table>
 </div>
 </li>
        <li> <span class="li-head">forticlient_download</span> - Enable/disable download option for FortiClient. <span class="li-normal">type: str</span> <span class="li-normal">choices: enable, disable</span>
 <a id='label118' href="javascript:ContentClick('label119', 'label118');" onmouseover="ContentPreview('label119');" onmouseout="ContentUnpreview('label119');" title="click to collapse or expand..."> more... </a>
 <div id="label119" style="display:none">
 <table border="1">
 <tr>
 <td></td>
 <td colspan="1">Supported Version Ranges</td>
 </tr>
 <tr>
 <td>forticlient_download</td>
 <td><code class="docutils literal notranslate">v6.0.0 -> latest </code></td>
 </tr>
 <tr>
 <td>[enable]</td>
 <td><code class="docutils literal notranslate">v6.0.0 -> latest</code></td> <tr>
 <td>[disable]</td>
 <td><code class="docutils literal notranslate">v6.0.0 -> latest</code></td> </table>
 </div>
 </li>
        <li> <span class="li-head">forticlient_download_method</span> - FortiClient download method. <span class="li-normal">type: str</span> <span class="li-normal">choices: direct, ssl-vpn</span>
 <a id='label120' href="javascript:ContentClick('label121', 'label120');" onmouseover="ContentPreview('label121');" onmouseout="ContentUnpreview('label121');" title="click to collapse or expand..."> more... </a>
 <div id="label121" style="display:none">
 <table border="1">
 <tr>
 <td></td>
 <td colspan="1">Supported Version Ranges</td>
 </tr>
 <tr>
 <td>forticlient_download_method</td>
 <td><code class="docutils literal notranslate">v6.0.0 -> latest </code></td>
 </tr>
 <tr>
 <td>[direct]</td>
 <td><code class="docutils literal notranslate">v6.0.0 -> latest</code></td> <tr>
 <td>[ssl-vpn]</td>
 <td><code class="docutils literal notranslate">v6.0.0 -> latest</code></td> </table>
 </div>
 </li>
        <li> <span class="li-head">heading</span> - Web portal heading message. <span class="li-normal">type: str</span>
 <a id='label122' href="javascript:ContentClick('label123', 'label122');" onmouseover="ContentPreview('label123');" onmouseout="ContentUnpreview('label123');" title="click to collapse or expand..."> more... </a>
 <div id="label123" style="display:none">
 <table border="1">
 <tr>
 <td></td>
 <td colspan="1">Supported Version Ranges</td>
 </tr>
 <tr>
 <td>heading</td>
 <td><code class="docutils literal notranslate">v6.0.0 -> latest </code></td>
 </tr>
 </table>
 </div>
 </li>
        <li> <span class="li-head">hide_sso_credential</span> - Enable to prevent SSO credential being sent to client. <span class="li-normal">type: str</span> <span class="li-normal">choices: enable, disable</span>
 <a id='label124' href="javascript:ContentClick('label125', 'label124');" onmouseover="ContentPreview('label125');" onmouseout="ContentUnpreview('label125');" title="click to collapse or expand..."> more... </a>
 <div id="label125" style="display:none">
 <table border="1">
 <tr>
 <td></td>
 <td colspan="1">Supported Version Ranges</td>
 </tr>
 <tr>
 <td>hide_sso_credential</td>
 <td><code class="docutils literal notranslate">v6.0.0 -> latest </code></td>
 </tr>
 <tr>
 <td>[enable]</td>
 <td><code class="docutils literal notranslate">v6.0.0 -> latest</code></td> <tr>
 <td>[disable]</td>
 <td><code class="docutils literal notranslate">v6.0.0 -> latest</code></td> </table>
 </div>
 </li>
        <li> <span class="li-head">host_check</span> - Type of host checking performed on endpoints. <span class="li-normal">type: str</span> <span class="li-normal">choices: none, av, fw, av-fw, custom</span>
 <a id='label126' href="javascript:ContentClick('label127', 'label126');" onmouseover="ContentPreview('label127');" onmouseout="ContentUnpreview('label127');" title="click to collapse or expand..."> more... </a>
 <div id="label127" style="display:none">
 <table border="1">
 <tr>
 <td></td>
 <td colspan="1">Supported Version Ranges</td>
 </tr>
 <tr>
 <td>host_check</td>
 <td><code class="docutils literal notranslate">v6.0.0 -> latest </code></td>
 </tr>
 <tr>
 <td>[none]</td>
 <td><code class="docutils literal notranslate">v6.0.0 -> latest</code></td> <tr>
 <td>[av]</td>
 <td><code class="docutils literal notranslate">v6.0.0 -> latest</code></td> <tr>
 <td>[fw]</td>
 <td><code class="docutils literal notranslate">v6.0.0 -> latest</code></td> <tr>
 <td>[av-fw]</td>
 <td><code class="docutils literal notranslate">v6.0.0 -> latest</code></td> <tr>
 <td>[custom]</td>
 <td><code class="docutils literal notranslate">v6.0.0 -> latest</code></td> </table>
 </div>
 </li>
        <li> <span class="li-head">host_check_interval</span> - Periodic host check interval. Value of 0 means disabled and host checking only happens when the endpoint connects. <span class="li-normal">type: int</span>
 <a id='label128' href="javascript:ContentClick('label129', 'label128');" onmouseover="ContentPreview('label129');" onmouseout="ContentUnpreview('label129');" title="click to collapse or expand..."> more... </a>
 <div id="label129" style="display:none">
 <table border="1">
 <tr>
 <td></td>
 <td colspan="1">Supported Version Ranges</td>
 </tr>
 <tr>
 <td>host_check_interval</td>
 <td><code class="docutils literal notranslate">v6.0.0 -> latest </code></td>
 </tr>
 </table>
 </div>
 </li>
        <li> <span class="li-head">host_check_policy</span> - One or more policies to require the endpoint to have specific security software. <span class="li-normal">type: list</span> <span style="font-family:'Courier New'" class="li-required">member_path: host_check_policy:name</span>
 <a id='label130' href="javascript:ContentClick('label131', 'label130');" onmouseover="ContentPreview('label131');" onmouseout="ContentUnpreview('label131');" title="click to collapse or expand..."> more... </a>
 <div id="label131" style="display:none">
 <table border="1">
 <tr>
 <td></td><td colspan="1">Supported Version Ranges</td>
 </tr>
 <tr>
 <td>host_check_policy</td>
 <td><code class="docutils literal notranslate">v6.0.0 -> latest </code></td>
 </tr>
 </table>
 </div>
 </li>
            <ul class="ul-self">
            <li> <span class="li-head">name</span> - Host check software list name. Source vpn.ssl.web.host-check-software.name. <span class="li-normal">type: str</span> <span class="li-required">required: true</span>
 <a id='label132' href="javascript:ContentClick('label133', 'label132');" onmouseover="ContentPreview('label133');" onmouseout="ContentUnpreview('label133');" title="click to collapse or expand..."> more... </a>
 <div id="label133" style="display:none">
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
            </ul>
        <li> <span class="li-head">ip_mode</span> - Method by which users of this SSL-VPN tunnel obtain IP addresses. <span class="li-normal">type: str</span> <span class="li-normal">choices: range, user-group, dhcp, no-ip</span>
 <a id='label134' href="javascript:ContentClick('label135', 'label134');" onmouseover="ContentPreview('label135');" onmouseout="ContentUnpreview('label135');" title="click to collapse or expand..."> more... </a>
 <div id="label135" style="display:none">
 <table border="1">
 <tr>
 <td></td>
 <td colspan="1">Supported Version Ranges</td>
 </tr>
 <tr>
 <td>ip_mode</td>
 <td><code class="docutils literal notranslate">v6.0.0 -> latest </code></td>
 </tr>
 <tr>
 <td>[range]</td>
 <td><code class="docutils literal notranslate">v6.0.0 -> latest</code></td> <tr>
 <td>[user-group]</td>
 <td><code class="docutils literal notranslate">v6.0.0 -> latest</code></td> <tr>
 <td>[dhcp]</td>
 <td><code class="docutils literal notranslate">v7.0.6 -> v7.0.12</code></td>
 <td><code class="docutils literal notranslate">v7.2.1 -> latest</code></td>
 </tr>
 <tr>
 <td>[no-ip]</td>
 <td><code class="docutils literal notranslate">v7.2.4 -> latest</code></td>
 </tr>
 </table>
 </div>
 </li>
        <li> <span class="li-head">ip_pools</span> - IPv4 firewall source address objects reserved for SSL-VPN tunnel mode clients. <span class="li-normal">type: list</span> <span style="font-family:'Courier New'" class="li-required">member_path: ip_pools:name</span>
 <a id='label136' href="javascript:ContentClick('label137', 'label136');" onmouseover="ContentPreview('label137');" onmouseout="ContentUnpreview('label137');" title="click to collapse or expand..."> more... </a>
 <div id="label137" style="display:none">
 <table border="1">
 <tr>
 <td></td><td colspan="1">Supported Version Ranges</td>
 </tr>
 <tr>
 <td>ip_pools</td>
 <td><code class="docutils literal notranslate">v6.0.0 -> latest </code></td>
 </tr>
 </table>
 </div>
 </li>
            <ul class="ul-self">
            <li> <span class="li-head">name</span> - Address name. Source firewall.address.name firewall.addrgrp.name. <span class="li-normal">type: str</span> <span class="li-required">required: true</span>
 <a id='label138' href="javascript:ContentClick('label139', 'label138');" onmouseover="ContentPreview('label139');" onmouseout="ContentUnpreview('label139');" title="click to collapse or expand..."> more... </a>
 <div id="label139" style="display:none">
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
            </ul>
        <li> <span class="li-head">ipv6_dns_server1</span> - IPv6 DNS server 1. <span class="li-normal">type: str</span>
 <a id='label140' href="javascript:ContentClick('label141', 'label140');" onmouseover="ContentPreview('label141');" onmouseout="ContentUnpreview('label141');" title="click to collapse or expand..."> more... </a>
 <div id="label141" style="display:none">
 <table border="1">
 <tr>
 <td></td>
 <td colspan="1">Supported Version Ranges</td>
 </tr>
 <tr>
 <td>ipv6_dns_server1</td>
 <td><code class="docutils literal notranslate">v6.0.0 -> latest </code></td>
 </tr>
 </table>
 </div>
 </li>
        <li> <span class="li-head">ipv6_dns_server2</span> - IPv6 DNS server 2. <span class="li-normal">type: str</span>
 <a id='label142' href="javascript:ContentClick('label143', 'label142');" onmouseover="ContentPreview('label143');" onmouseout="ContentUnpreview('label143');" title="click to collapse or expand..."> more... </a>
 <div id="label143" style="display:none">
 <table border="1">
 <tr>
 <td></td>
 <td colspan="1">Supported Version Ranges</td>
 </tr>
 <tr>
 <td>ipv6_dns_server2</td>
 <td><code class="docutils literal notranslate">v6.0.0 -> latest </code></td>
 </tr>
 </table>
 </div>
 </li>
        <li> <span class="li-head">ipv6_exclusive_routing</span> - Enable/disable all IPv6 traffic go through tunnel only. <span class="li-normal">type: str</span> <span class="li-normal">choices: enable, disable</span>
 <a id='label144' href="javascript:ContentClick('label145', 'label144');" onmouseover="ContentPreview('label145');" onmouseout="ContentUnpreview('label145');" title="click to collapse or expand..."> more... </a>
 <div id="label145" style="display:none">
 <table border="1">
 <tr>
 <td></td>
 <td colspan="1">Supported Version Ranges</td>
 </tr>
 <tr>
 <td>ipv6_exclusive_routing</td>
 <td><code class="docutils literal notranslate">v6.0.0 -> latest </code></td>
 </tr>
 <tr>
 <td>[enable]</td>
 <td><code class="docutils literal notranslate">v6.0.0 -> latest</code></td> <tr>
 <td>[disable]</td>
 <td><code class="docutils literal notranslate">v6.0.0 -> latest</code></td> </table>
 </div>
 </li>
        <li> <span class="li-head">ipv6_pools</span> - IPv6 firewall source address objects reserved for SSL-VPN tunnel mode clients. <span class="li-normal">type: list</span> <span style="font-family:'Courier New'" class="li-required">member_path: ipv6_pools:name</span>
 <a id='label146' href="javascript:ContentClick('label147', 'label146');" onmouseover="ContentPreview('label147');" onmouseout="ContentUnpreview('label147');" title="click to collapse or expand..."> more... </a>
 <div id="label147" style="display:none">
 <table border="1">
 <tr>
 <td></td><td colspan="1">Supported Version Ranges</td>
 </tr>
 <tr>
 <td>ipv6_pools</td>
 <td><code class="docutils literal notranslate">v6.0.0 -> latest </code></td>
 </tr>
 </table>
 </div>
 </li>
            <ul class="ul-self">
            <li> <span class="li-head">name</span> - Address name. Source firewall.address6.name firewall.addrgrp6.name. <span class="li-normal">type: str</span> <span class="li-required">required: true</span>
 <a id='label148' href="javascript:ContentClick('label149', 'label148');" onmouseover="ContentPreview('label149');" onmouseout="ContentUnpreview('label149');" title="click to collapse or expand..."> more... </a>
 <div id="label149" style="display:none">
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
            </ul>
        <li> <span class="li-head">ipv6_service_restriction</span> - Enable/disable IPv6 tunnel service restriction. <span class="li-normal">type: str</span> <span class="li-normal">choices: enable, disable</span>
 <a id='label150' href="javascript:ContentClick('label151', 'label150');" onmouseover="ContentPreview('label151');" onmouseout="ContentUnpreview('label151');" title="click to collapse or expand..."> more... </a>
 <div id="label151" style="display:none">
 <table border="1">
 <tr>
 <td></td>
 <td colspan="1">Supported Version Ranges</td>
 </tr>
 <tr>
 <td>ipv6_service_restriction</td>
 <td><code class="docutils literal notranslate">v6.0.0 -> latest </code></td>
 </tr>
 <tr>
 <td>[enable]</td>
 <td><code class="docutils literal notranslate">v6.0.0 -> latest</code></td> <tr>
 <td>[disable]</td>
 <td><code class="docutils literal notranslate">v6.0.0 -> latest</code></td> </table>
 </div>
 </li>
        <li> <span class="li-head">ipv6_split_tunneling</span> - Enable/disable IPv6 split tunneling. <span class="li-normal">type: str</span> <span class="li-normal">choices: enable, disable</span>
 <a id='label152' href="javascript:ContentClick('label153', 'label152');" onmouseover="ContentPreview('label153');" onmouseout="ContentUnpreview('label153');" title="click to collapse or expand..."> more... </a>
 <div id="label153" style="display:none">
 <table border="1">
 <tr>
 <td></td>
 <td colspan="1">Supported Version Ranges</td>
 </tr>
 <tr>
 <td>ipv6_split_tunneling</td>
 <td><code class="docutils literal notranslate">v6.0.0 -> latest </code></td>
 </tr>
 <tr>
 <td>[enable]</td>
 <td><code class="docutils literal notranslate">v6.0.0 -> latest</code></td> <tr>
 <td>[disable]</td>
 <td><code class="docutils literal notranslate">v6.0.0 -> latest</code></td> </table>
 </div>
 </li>
        <li> <span class="li-head">ipv6_split_tunneling_routing_address</span> - IPv6 SSL-VPN tunnel mode firewall address objects that override firewall policy destination addresses to control split-tunneling access. <span class="li-normal">type: list</span> <span style="font-family:'Courier New'" class="li-required">member_path: ipv6_split_tunneling_routing_address:name</span>
 <a id='label154' href="javascript:ContentClick('label155', 'label154');" onmouseover="ContentPreview('label155');" onmouseout="ContentUnpreview('label155');" title="click to collapse or expand..."> more... </a>
 <div id="label155" style="display:none">
 <table border="1">
 <tr>
 <td></td><td colspan="1">Supported Version Ranges</td>
 </tr>
 <tr>
 <td>ipv6_split_tunneling_routing_address</td>
 <td><code class="docutils literal notranslate">v6.0.0 -> latest </code></td>
 </tr>
 </table>
 </div>
 </li>
            <ul class="ul-self">
            <li> <span class="li-head">name</span> - Address name. Source firewall.address6.name firewall.addrgrp6.name. <span class="li-normal">type: str</span> <span class="li-required">required: true</span>
 <a id='label156' href="javascript:ContentClick('label157', 'label156');" onmouseover="ContentPreview('label157');" onmouseout="ContentUnpreview('label157');" title="click to collapse or expand..."> more... </a>
 <div id="label157" style="display:none">
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
            </ul>
        <li> <span class="li-head">ipv6_split_tunneling_routing_negate</span> - Enable to negate IPv6 split tunneling routing address. <span class="li-normal">type: str</span> <span class="li-normal">choices: enable, disable</span>
 <a id='label158' href="javascript:ContentClick('label159', 'label158');" onmouseover="ContentPreview('label159');" onmouseout="ContentUnpreview('label159');" title="click to collapse or expand..."> more... </a>
 <div id="label159" style="display:none">
 <table border="1">
 <tr>
 <td></td>
 <td colspan="1">Supported Version Ranges</td>
 </tr>
 <tr>
 <td>ipv6_split_tunneling_routing_negate</td>
 <td><code class="docutils literal notranslate">v6.4.0 -> latest </code></td>
 </tr>
 <tr>
 <td>[enable]</td>
 <td><code class="docutils literal notranslate">v6.0.0 -> latest</code></td> <tr>
 <td>[disable]</td>
 <td><code class="docutils literal notranslate">v6.0.0 -> latest</code></td> </table>
 </div>
 </li>
        <li> <span class="li-head">ipv6_tunnel_mode</span> - Enable/disable IPv6 SSL-VPN tunnel mode. <span class="li-normal">type: str</span> <span class="li-normal">choices: enable, disable</span>
 <a id='label160' href="javascript:ContentClick('label161', 'label160');" onmouseover="ContentPreview('label161');" onmouseout="ContentUnpreview('label161');" title="click to collapse or expand..."> more... </a>
 <div id="label161" style="display:none">
 <table border="1">
 <tr>
 <td></td>
 <td colspan="1">Supported Version Ranges</td>
 </tr>
 <tr>
 <td>ipv6_tunnel_mode</td>
 <td><code class="docutils literal notranslate">v6.0.0 -> latest </code></td>
 </tr>
 <tr>
 <td>[enable]</td>
 <td><code class="docutils literal notranslate">v6.0.0 -> latest</code></td> <tr>
 <td>[disable]</td>
 <td><code class="docutils literal notranslate">v6.0.0 -> latest</code></td> </table>
 </div>
 </li>
        <li> <span class="li-head">ipv6_wins_server1</span> - IPv6 WINS server 1. <span class="li-normal">type: str</span>
 <a id='label162' href="javascript:ContentClick('label163', 'label162');" onmouseover="ContentPreview('label163');" onmouseout="ContentUnpreview('label163');" title="click to collapse or expand..."> more... </a>
 <div id="label163" style="display:none">
 <table border="1">
 <tr>
 <td></td>
 <td colspan="1">Supported Version Ranges</td>
 </tr>
 <tr>
 <td>ipv6_wins_server1</td>
 <td><code class="docutils literal notranslate">v6.0.0 -> latest </code></td>
 </tr>
 </table>
 </div>
 </li>
        <li> <span class="li-head">ipv6_wins_server2</span> - IPv6 WINS server 2. <span class="li-normal">type: str</span>
 <a id='label164' href="javascript:ContentClick('label165', 'label164');" onmouseover="ContentPreview('label165');" onmouseout="ContentUnpreview('label165');" title="click to collapse or expand..."> more... </a>
 <div id="label165" style="display:none">
 <table border="1">
 <tr>
 <td></td>
 <td colspan="1">Supported Version Ranges</td>
 </tr>
 <tr>
 <td>ipv6_wins_server2</td>
 <td><code class="docutils literal notranslate">v6.0.0 -> latest </code></td>
 </tr>
 </table>
 </div>
 </li>
        <li> <span class="li-head">keep_alive</span> - Enable/disable automatic reconnect for FortiClient connections. <span class="li-normal">type: str</span> <span class="li-normal">choices: enable, disable</span>
 <a id='label166' href="javascript:ContentClick('label167', 'label166');" onmouseover="ContentPreview('label167');" onmouseout="ContentUnpreview('label167');" title="click to collapse or expand..."> more... </a>
 <div id="label167" style="display:none">
 <table border="1">
 <tr>
 <td></td>
 <td colspan="1">Supported Version Ranges</td>
 </tr>
 <tr>
 <td>keep_alive</td>
 <td><code class="docutils literal notranslate">v6.0.0 -> latest </code></td>
 </tr>
 <tr>
 <td>[enable]</td>
 <td><code class="docutils literal notranslate">v6.0.0 -> latest</code></td> <tr>
 <td>[disable]</td>
 <td><code class="docutils literal notranslate">v6.0.0 -> latest</code></td> </table>
 </div>
 </li>
        <li> <span class="li-head">landing_page</span> - Landing page options. <span class="li-normal">type: dict</span>
 <a id='label168' href="javascript:ContentClick('label169', 'label168');" onmouseover="ContentPreview('label169');" onmouseout="ContentUnpreview('label169');" title="click to collapse or expand..."> more... </a>
 <div id="label169" style="display:none">
 <table border="1">
 <tr>
 <td></td><td colspan="1">Supported Version Ranges</td>
 </tr>
 <tr>
 <td>landing_page</td>
 <td><code class="docutils literal notranslate">v7.4.0 -> latest </code></td>
 </tr>
 </table>
 </div>
 </li>
            <ul class="ul-self">
            <li> <span class="li-head">form_data</span> - Form data. <span class="li-normal">type: list</span> <span style="font-family:'Courier New'" class="li-required">member_path: landing_page/form_data:name</span>
 <a id='label170' href="javascript:ContentClick('label171', 'label170');" onmouseover="ContentPreview('label171');" onmouseout="ContentUnpreview('label171');" title="click to collapse or expand..."> more... </a>
 <div id="label171" style="display:none">
 <table border="1">
 <tr>
 <td></td><td colspan="1">Supported Version Ranges</td>
 </tr>
 <tr>
 <td>form_data</td>
 <td><code class="docutils literal notranslate">v7.4.0 -> latest </code></td>
 </tr>
 </table>
 </div>
 </li>
                <ul class="ul-self">
                <li> <span class="li-head">name</span> - Name. <span class="li-normal">type: str</span> <span class="li-required">required: true</span>
 <a id='label172' href="javascript:ContentClick('label173', 'label172');" onmouseover="ContentPreview('label173');" onmouseout="ContentUnpreview('label173');" title="click to collapse or expand..."> more... </a>
 <div id="label173" style="display:none">
 <table border="1">
 <tr>
 <td></td>
 <td colspan="1">Supported Version Ranges</td>
 </tr>
 <tr>
 <td>name</td>
 <td><code class="docutils literal notranslate">v7.4.0 -> latest </code></td>
 </tr>
 </table>
 </div>
 </li>
                <li> <span class="li-head">value</span> - Value. <span class="li-normal">type: str</span>
 <a id='label174' href="javascript:ContentClick('label175', 'label174');" onmouseover="ContentPreview('label175');" onmouseout="ContentUnpreview('label175');" title="click to collapse or expand..."> more... </a>
 <div id="label175" style="display:none">
 <table border="1">
 <tr>
 <td></td>
 <td colspan="1">Supported Version Ranges</td>
 </tr>
 <tr>
 <td>value</td>
 <td><code class="docutils literal notranslate">v7.4.0 -> latest </code></td>
 </tr>
 </table>
 </div>
 </li>
                </ul>
            <li> <span class="li-head">logout_url</span> - Landing page log out URL. <span class="li-normal">type: str</span>
 <a id='label176' href="javascript:ContentClick('label177', 'label176');" onmouseover="ContentPreview('label177');" onmouseout="ContentUnpreview('label177');" title="click to collapse or expand..."> more... </a>
 <div id="label177" style="display:none">
 <table border="1">
 <tr>
 <td></td>
 <td colspan="1">Supported Version Ranges</td>
 </tr>
 <tr>
 <td>logout_url</td>
 <td><code class="docutils literal notranslate">v7.4.0 -> v7.4.0 </code></td>
 </tr>
 </table>
 </div>
 </li>
            <li> <span class="li-head">sso</span> - Single sign-on. <span class="li-normal">type: str</span> <span class="li-normal">choices: disable, static, auto</span>
 <a id='label178' href="javascript:ContentClick('label179', 'label178');" onmouseover="ContentPreview('label179');" onmouseout="ContentUnpreview('label179');" title="click to collapse or expand..."> more... </a>
 <div id="label179" style="display:none">
 <table border="1">
 <tr>
 <td></td>
 <td colspan="1">Supported Version Ranges</td>
 </tr>
 <tr>
 <td>sso</td>
 <td><code class="docutils literal notranslate">v7.4.0 -> latest </code></td>
 </tr>
 <tr>
 <td>[disable]</td>
 <td><code class="docutils literal notranslate">v6.0.0 -> latest</code></td> <tr>
 <td>[static]</td>
 <td><code class="docutils literal notranslate">v6.0.0 -> latest</code></td> <tr>
 <td>[auto]</td>
 <td><code class="docutils literal notranslate">v6.0.0 -> latest</code></td> </table>
 </div>
 </li>
            <li> <span class="li-head">sso_credential</span> - Single sign-on credentials. <span class="li-normal">type: str</span> <span class="li-normal">choices: sslvpn-login, alternative</span>
 <a id='label180' href="javascript:ContentClick('label181', 'label180');" onmouseover="ContentPreview('label181');" onmouseout="ContentUnpreview('label181');" title="click to collapse or expand..."> more... </a>
 <div id="label181" style="display:none">
 <table border="1">
 <tr>
 <td></td>
 <td colspan="1">Supported Version Ranges</td>
 </tr>
 <tr>
 <td>sso_credential</td>
 <td><code class="docutils literal notranslate">v7.4.0 -> latest </code></td>
 </tr>
 <tr>
 <td>[sslvpn-login]</td>
 <td><code class="docutils literal notranslate">v6.0.0 -> latest</code></td> <tr>
 <td>[alternative]</td>
 <td><code class="docutils literal notranslate">v6.0.0 -> latest</code></td> </table>
 </div>
 </li>
            <li> <span class="li-head">sso_password</span> - SSO password. <span class="li-normal">type: str</span>
 <a id='label182' href="javascript:ContentClick('label183', 'label182');" onmouseover="ContentPreview('label183');" onmouseout="ContentUnpreview('label183');" title="click to collapse or expand..."> more... </a>
 <div id="label183" style="display:none">
 <table border="1">
 <tr>
 <td></td>
 <td colspan="1">Supported Version Ranges</td>
 </tr>
 <tr>
 <td>sso_password</td>
 <td><code class="docutils literal notranslate">v7.4.0 -> latest </code></td>
 </tr>
 </table>
 </div>
 </li>
            <li> <span class="li-head">sso_username</span> - SSO user name. <span class="li-normal">type: str</span>
 <a id='label184' href="javascript:ContentClick('label185', 'label184');" onmouseover="ContentPreview('label185');" onmouseout="ContentUnpreview('label185');" title="click to collapse or expand..."> more... </a>
 <div id="label185" style="display:none">
 <table border="1">
 <tr>
 <td></td>
 <td colspan="1">Supported Version Ranges</td>
 </tr>
 <tr>
 <td>sso_username</td>
 <td><code class="docutils literal notranslate">v7.4.0 -> latest </code></td>
 </tr>
 </table>
 </div>
 </li>
            <li> <span class="li-head">url</span> - Landing page URL. <span class="li-normal">type: str</span>
 <a id='label186' href="javascript:ContentClick('label187', 'label186');" onmouseover="ContentPreview('label187');" onmouseout="ContentUnpreview('label187');" title="click to collapse or expand..."> more... </a>
 <div id="label187" style="display:none">
 <table border="1">
 <tr>
 <td></td>
 <td colspan="1">Supported Version Ranges</td>
 </tr>
 <tr>
 <td>url</td>
 <td><code class="docutils literal notranslate">v7.4.0 -> latest </code></td>
 </tr>
 </table>
 </div>
 </li>
            </ul>
        <li> <span class="li-head">landing_page_mode</span> - Enable/disable SSL-VPN landing page mode. <span class="li-normal">type: str</span> <span class="li-normal">choices: enable, disable</span>
 <a id='label188' href="javascript:ContentClick('label189', 'label188');" onmouseover="ContentPreview('label189');" onmouseout="ContentUnpreview('label189');" title="click to collapse or expand..."> more... </a>
 <div id="label189" style="display:none">
 <table border="1">
 <tr>
 <td></td>
 <td colspan="1">Supported Version Ranges</td>
 </tr>
 <tr>
 <td>landing_page_mode</td>
 <td><code class="docutils literal notranslate">v7.4.0 -> latest </code></td>
 </tr>
 <tr>
 <td>[enable]</td>
 <td><code class="docutils literal notranslate">v6.0.0 -> latest</code></td> <tr>
 <td>[disable]</td>
 <td><code class="docutils literal notranslate">v6.0.0 -> latest</code></td> </table>
 </div>
 </li>
        <li> <span class="li-head">limit_user_logins</span> - Enable to limit each user to one SSL-VPN session at a time. <span class="li-normal">type: str</span> <span class="li-normal">choices: enable, disable</span>
 <a id='label190' href="javascript:ContentClick('label191', 'label190');" onmouseover="ContentPreview('label191');" onmouseout="ContentUnpreview('label191');" title="click to collapse or expand..."> more... </a>
 <div id="label191" style="display:none">
 <table border="1">
 <tr>
 <td></td>
 <td colspan="1">Supported Version Ranges</td>
 </tr>
 <tr>
 <td>limit_user_logins</td>
 <td><code class="docutils literal notranslate">v6.0.0 -> latest </code></td>
 </tr>
 <tr>
 <td>[enable]</td>
 <td><code class="docutils literal notranslate">v6.0.0 -> latest</code></td> <tr>
 <td>[disable]</td>
 <td><code class="docutils literal notranslate">v6.0.0 -> latest</code></td> </table>
 </div>
 </li>
        <li> <span class="li-head">mac_addr_action</span> - Client MAC address action. <span class="li-normal">type: str</span> <span class="li-normal">choices: allow, deny</span>
 <a id='label192' href="javascript:ContentClick('label193', 'label192');" onmouseover="ContentPreview('label193');" onmouseout="ContentUnpreview('label193');" title="click to collapse or expand..."> more... </a>
 <div id="label193" style="display:none">
 <table border="1">
 <tr>
 <td></td>
 <td colspan="1">Supported Version Ranges</td>
 </tr>
 <tr>
 <td>mac_addr_action</td>
 <td><code class="docutils literal notranslate">v6.0.0 -> latest </code></td>
 </tr>
 <tr>
 <td>[allow]</td>
 <td><code class="docutils literal notranslate">v6.0.0 -> latest</code></td> <tr>
 <td>[deny]</td>
 <td><code class="docutils literal notranslate">v6.0.0 -> latest</code></td> </table>
 </div>
 </li>
        <li> <span class="li-head">mac_addr_check</span> - Enable/disable MAC address host checking. <span class="li-normal">type: str</span> <span class="li-normal">choices: enable, disable</span>
 <a id='label194' href="javascript:ContentClick('label195', 'label194');" onmouseover="ContentPreview('label195');" onmouseout="ContentUnpreview('label195');" title="click to collapse or expand..."> more... </a>
 <div id="label195" style="display:none">
 <table border="1">
 <tr>
 <td></td>
 <td colspan="1">Supported Version Ranges</td>
 </tr>
 <tr>
 <td>mac_addr_check</td>
 <td><code class="docutils literal notranslate">v6.0.0 -> latest </code></td>
 </tr>
 <tr>
 <td>[enable]</td>
 <td><code class="docutils literal notranslate">v6.0.0 -> latest</code></td> <tr>
 <td>[disable]</td>
 <td><code class="docutils literal notranslate">v6.0.0 -> latest</code></td> </table>
 </div>
 </li>
        <li> <span class="li-head">mac_addr_check_rule</span> - Client MAC address check rule. <span class="li-normal">type: list</span> <span style="font-family:'Courier New'" class="li-required">member_path: mac_addr_check_rule:name</span>
 <a id='label196' href="javascript:ContentClick('label197', 'label196');" onmouseover="ContentPreview('label197');" onmouseout="ContentUnpreview('label197');" title="click to collapse or expand..."> more... </a>
 <div id="label197" style="display:none">
 <table border="1">
 <tr>
 <td></td><td colspan="1">Supported Version Ranges</td>
 </tr>
 <tr>
 <td>mac_addr_check_rule</td>
 <td><code class="docutils literal notranslate">v6.0.0 -> latest </code></td>
 </tr>
 </table>
 </div>
 </li>
            <ul class="ul-self">
            <li> <span class="li-head">mac_addr_list</span> - Client MAC address list. <span class="li-normal">type: list</span> <span style="font-family:'Courier New'" class="li-required">member_path: mac_addr_check_rule:name/mac_addr_list:addr</span>
 <a id='label198' href="javascript:ContentClick('label199', 'label198');" onmouseover="ContentPreview('label199');" onmouseout="ContentUnpreview('label199');" title="click to collapse or expand..."> more... </a>
 <div id="label199" style="display:none">
 <table border="1">
 <tr>
 <td></td><td colspan="1">Supported Version Ranges</td>
 </tr>
 <tr>
 <td>mac_addr_list</td>
 <td><code class="docutils literal notranslate">v6.0.0 -> latest </code></td>
 </tr>
 </table>
 </div>
 </li>
                <ul class="ul-self">
                <li> <span class="li-head">addr</span> - Client MAC address. <span class="li-normal">type: str</span> <span class="li-required">required: true</span>
 <a id='label200' href="javascript:ContentClick('label201', 'label200');" onmouseover="ContentPreview('label201');" onmouseout="ContentUnpreview('label201');" title="click to collapse or expand..."> more... </a>
 <div id="label201" style="display:none">
 <table border="1">
 <tr>
 <td></td>
 <td colspan="1">Supported Version Ranges</td>
 </tr>
 <tr>
 <td>addr</td>
 <td><code class="docutils literal notranslate">v6.0.0 -> latest </code></td>
 </tr>
 </table>
 </div>
 </li>
                </ul>
            <li> <span class="li-head">mac_addr_mask</span> - Client MAC address mask. <span class="li-normal">type: int</span>
 <a id='label202' href="javascript:ContentClick('label203', 'label202');" onmouseover="ContentPreview('label203');" onmouseout="ContentUnpreview('label203');" title="click to collapse or expand..."> more... </a>
 <div id="label203" style="display:none">
 <table border="1">
 <tr>
 <td></td>
 <td colspan="1">Supported Version Ranges</td>
 </tr>
 <tr>
 <td>mac_addr_mask</td>
 <td><code class="docutils literal notranslate">v6.0.0 -> latest </code></td>
 </tr>
 </table>
 </div>
 </li>
            <li> <span class="li-head">name</span> - Client MAC address check rule name. <span class="li-normal">type: str</span> <span class="li-required">required: true</span>
 <a id='label204' href="javascript:ContentClick('label205', 'label204');" onmouseover="ContentPreview('label205');" onmouseout="ContentUnpreview('label205');" title="click to collapse or expand..."> more... </a>
 <div id="label205" style="display:none">
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
            </ul>
        <li> <span class="li-head">macos_forticlient_download_url</span> - Download URL for Mac FortiClient. <span class="li-normal">type: str</span>
 <a id='label206' href="javascript:ContentClick('label207', 'label206');" onmouseover="ContentPreview('label207');" onmouseout="ContentUnpreview('label207');" title="click to collapse or expand..."> more... </a>
 <div id="label207" style="display:none">
 <table border="1">
 <tr>
 <td></td>
 <td colspan="1">Supported Version Ranges</td>
 </tr>
 <tr>
 <td>macos_forticlient_download_url</td>
 <td><code class="docutils literal notranslate">v6.0.0 -> latest </code></td>
 </tr>
 </table>
 </div>
 </li>
        <li> <span class="li-head">name</span> - Portal name. <span class="li-normal">type: str</span> <span class="li-required">required: true</span>
 <a id='label208' href="javascript:ContentClick('label209', 'label208');" onmouseover="ContentPreview('label209');" onmouseout="ContentUnpreview('label209');" title="click to collapse or expand..."> more... </a>
 <div id="label209" style="display:none">
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
        <li> <span class="li-head">os_check</span> - Enable to let the FortiGate decide action based on client OS. <span class="li-normal">type: str</span> <span class="li-normal">choices: enable, disable</span>
 <a id='label210' href="javascript:ContentClick('label211', 'label210');" onmouseover="ContentPreview('label211');" onmouseout="ContentUnpreview('label211');" title="click to collapse or expand..."> more... </a>
 <div id="label211" style="display:none">
 <table border="1">
 <tr>
 <td></td>
 <td colspan="1">Supported Version Ranges</td>
 </tr>
 <tr>
 <td>os_check</td>
 <td><code class="docutils literal notranslate">v6.0.0 -> latest </code></td>
 </tr>
 <tr>
 <td>[enable]</td>
 <td><code class="docutils literal notranslate">v6.0.0 -> latest</code></td> <tr>
 <td>[disable]</td>
 <td><code class="docutils literal notranslate">v6.0.0 -> latest</code></td> </table>
 </div>
 </li>
        <li> <span class="li-head">os_check_list</span> - SSL-VPN OS checks. <span class="li-normal">type: list</span> <span style="font-family:'Courier New'" class="li-required">member_path: os_check_list:name</span>
 <a id='label212' href="javascript:ContentClick('label213', 'label212');" onmouseover="ContentPreview('label213');" onmouseout="ContentUnpreview('label213');" title="click to collapse or expand..."> more... </a>
 <div id="label213" style="display:none">
 <table border="1">
 <tr>
 <td></td><td colspan="2">Supported Version Ranges</td>
 </tr>
 <tr>
 <td>os_check_list</td>
 <td><code class="docutils literal notranslate">v6.0.0 -> v7.0.5 </code></td>
 <td><code class="docutils literal notranslate">v7.2.0 -> v7.2.0 </code></td>
 </tr>
 </table>
 </div>
 </li>
            <ul class="ul-self">
            <li> <span class="li-head">action</span> - OS check options. <span class="li-normal">type: str</span> <span class="li-normal">choices: deny, allow, check-up-to-date</span>
 <a id='label214' href="javascript:ContentClick('label215', 'label214');" onmouseover="ContentPreview('label215');" onmouseout="ContentUnpreview('label215');" title="click to collapse or expand..."> more... </a>
 <div id="label215" style="display:none">
 <table border="1">
 <tr>
 <td></td>
 <td colspan="2">Supported Version Ranges</td>
 </tr>
 <tr>
 <td>action</td>
 <td><code class="docutils literal notranslate">v6.0.0 -> v7.0.5 </code></td>
 <td><code class="docutils literal notranslate">v7.2.0 -> v7.2.0 </code></td>
 </tr>
 <tr>
 <td>[deny]</td>
 <td><code class="docutils literal notranslate">v6.0.0 -> latest</code></td> <tr>
 <td>[allow]</td>
 <td><code class="docutils literal notranslate">v6.0.0 -> latest</code></td> <tr>
 <td>[check-up-to-date]</td>
 <td><code class="docutils literal notranslate">v6.0.0 -> latest</code></td> </table>
 </div>
 </li>
            <li> <span class="li-head">latest_patch_level</span> - Latest OS patch level. <span class="li-normal">type: str</span>
 <a id='label216' href="javascript:ContentClick('label217', 'label216');" onmouseover="ContentPreview('label217');" onmouseout="ContentUnpreview('label217');" title="click to collapse or expand..."> more... </a>
 <div id="label217" style="display:none">
 <table border="1">
 <tr>
 <td></td>
 <td colspan="2">Supported Version Ranges</td>
 </tr>
 <tr>
 <td>latest_patch_level</td>
 <td><code class="docutils literal notranslate">v6.0.0 -> v7.0.5 </code></td>
 <td><code class="docutils literal notranslate">v7.2.0 -> v7.2.0 </code></td>
 </tr>
 </table>
 </div>
 </li>
            <li> <span class="li-head">name</span> - Name. <span class="li-normal">type: str</span> <span class="li-required">required: true</span>
 <a id='label218' href="javascript:ContentClick('label219', 'label218');" onmouseover="ContentPreview('label219');" onmouseout="ContentUnpreview('label219');" title="click to collapse or expand..."> more... </a>
 <div id="label219" style="display:none">
 <table border="1">
 <tr>
 <td></td>
 <td colspan="2">Supported Version Ranges</td>
 </tr>
 <tr>
 <td>name</td>
 <td><code class="docutils literal notranslate">v6.0.0 -> v7.0.5 </code></td>
 <td><code class="docutils literal notranslate">v7.2.0 -> v7.2.0 </code></td>
 </tr>
 </table>
 </div>
 </li>
            <li> <span class="li-head">tolerance</span> - OS patch level tolerance. <span class="li-normal">type: int</span>
 <a id='label220' href="javascript:ContentClick('label221', 'label220');" onmouseover="ContentPreview('label221');" onmouseout="ContentUnpreview('label221');" title="click to collapse or expand..."> more... </a>
 <div id="label221" style="display:none">
 <table border="1">
 <tr>
 <td></td>
 <td colspan="2">Supported Version Ranges</td>
 </tr>
 <tr>
 <td>tolerance</td>
 <td><code class="docutils literal notranslate">v6.0.0 -> v7.0.5 </code></td>
 <td><code class="docutils literal notranslate">v7.2.0 -> v7.2.0 </code></td>
 </tr>
 </table>
 </div>
 </li>
            </ul>
        <li> <span class="li-head">prefer_ipv6_dns</span> - Prefer to query IPv6 DNS server first if enabled. <span class="li-normal">type: str</span> <span class="li-normal">choices: enable, disable</span>
 <a id='label222' href="javascript:ContentClick('label223', 'label222');" onmouseover="ContentPreview('label223');" onmouseout="ContentUnpreview('label223');" title="click to collapse or expand..."> more... </a>
 <div id="label223" style="display:none">
 <table border="1">
 <tr>
 <td></td>
 <td colspan="1">Supported Version Ranges</td>
 </tr>
 <tr>
 <td>prefer_ipv6_dns</td>
 <td><code class="docutils literal notranslate">v7.0.0 -> latest </code></td>
 </tr>
 <tr>
 <td>[enable]</td>
 <td><code class="docutils literal notranslate">v6.0.0 -> latest</code></td> <tr>
 <td>[disable]</td>
 <td><code class="docutils literal notranslate">v6.0.0 -> latest</code></td> </table>
 </div>
 </li>
        <li> <span class="li-head">redir_url</span> - Client login redirect URL. <span class="li-normal">type: str</span>
 <a id='label224' href="javascript:ContentClick('label225', 'label224');" onmouseover="ContentPreview('label225');" onmouseout="ContentUnpreview('label225');" title="click to collapse or expand..."> more... </a>
 <div id="label225" style="display:none">
 <table border="1">
 <tr>
 <td></td>
 <td colspan="1">Supported Version Ranges</td>
 </tr>
 <tr>
 <td>redir_url</td>
 <td><code class="docutils literal notranslate">v6.0.0 -> latest </code></td>
 </tr>
 </table>
 </div>
 </li>
        <li> <span class="li-head">rewrite_ip_uri_ui</span> - Rewrite contents for URI contains IP and /ui/ . <span class="li-normal">type: str</span> <span class="li-normal">choices: enable, disable</span>
 <a id='label226' href="javascript:ContentClick('label227', 'label226');" onmouseover="ContentPreview('label227');" onmouseout="ContentUnpreview('label227');" title="click to collapse or expand..."> more... </a>
 <div id="label227" style="display:none">
 <table border="1">
 <tr>
 <td></td>
 <td colspan="1">Supported Version Ranges</td>
 </tr>
 <tr>
 <td>rewrite_ip_uri_ui</td>
 <td><code class="docutils literal notranslate">v7.0.0 -> latest </code></td>
 </tr>
 <tr>
 <td>[enable]</td>
 <td><code class="docutils literal notranslate">v6.0.0 -> latest</code></td> <tr>
 <td>[disable]</td>
 <td><code class="docutils literal notranslate">v6.0.0 -> latest</code></td> </table>
 </div>
 </li>
        <li> <span class="li-head">save_password</span> - Enable/disable FortiClient saving the user"s password. <span class="li-normal">type: str</span> <span class="li-normal">choices: enable, disable</span>
 <a id='label228' href="javascript:ContentClick('label229', 'label228');" onmouseover="ContentPreview('label229');" onmouseout="ContentUnpreview('label229');" title="click to collapse or expand..."> more... </a>
 <div id="label229" style="display:none">
 <table border="1">
 <tr>
 <td></td>
 <td colspan="1">Supported Version Ranges</td>
 </tr>
 <tr>
 <td>save_password</td>
 <td><code class="docutils literal notranslate">v6.0.0 -> latest </code></td>
 </tr>
 <tr>
 <td>[enable]</td>
 <td><code class="docutils literal notranslate">v6.0.0 -> latest</code></td> <tr>
 <td>[disable]</td>
 <td><code class="docutils literal notranslate">v6.0.0 -> latest</code></td> </table>
 </div>
 </li>
        <li> <span class="li-head">service_restriction</span> - Enable/disable tunnel service restriction. <span class="li-normal">type: str</span> <span class="li-normal">choices: enable, disable</span>
 <a id='label230' href="javascript:ContentClick('label231', 'label230');" onmouseover="ContentPreview('label231');" onmouseout="ContentUnpreview('label231');" title="click to collapse or expand..."> more... </a>
 <div id="label231" style="display:none">
 <table border="1">
 <tr>
 <td></td>
 <td colspan="1">Supported Version Ranges</td>
 </tr>
 <tr>
 <td>service_restriction</td>
 <td><code class="docutils literal notranslate">v6.0.0 -> latest </code></td>
 </tr>
 <tr>
 <td>[enable]</td>
 <td><code class="docutils literal notranslate">v6.0.0 -> latest</code></td> <tr>
 <td>[disable]</td>
 <td><code class="docutils literal notranslate">v6.0.0 -> latest</code></td> </table>
 </div>
 </li>
        <li> <span class="li-head">skip_check_for_browser</span> - Enable to skip host check for browser support. <span class="li-normal">type: str</span> <span class="li-normal">choices: enable, disable</span>
 <a id='label232' href="javascript:ContentClick('label233', 'label232');" onmouseover="ContentPreview('label233');" onmouseout="ContentUnpreview('label233');" title="click to collapse or expand..."> more... </a>
 <div id="label233" style="display:none">
 <table border="1">
 <tr>
 <td></td>
 <td colspan="1">Supported Version Ranges</td>
 </tr>
 <tr>
 <td>skip_check_for_browser</td>
 <td><code class="docutils literal notranslate">v6.2.0 -> latest </code></td>
 </tr>
 <tr>
 <td>[enable]</td>
 <td><code class="docutils literal notranslate">v6.0.0 -> latest</code></td> <tr>
 <td>[disable]</td>
 <td><code class="docutils literal notranslate">v6.0.0 -> latest</code></td> </table>
 </div>
 </li>
        <li> <span class="li-head">skip_check_for_unsupported_browser</span> - Enable to skip host check if browser does not support it. <span class="li-normal">type: str</span> <span class="li-normal">choices: enable, disable</span>
 <a id='label234' href="javascript:ContentClick('label235', 'label234');" onmouseover="ContentPreview('label235');" onmouseout="ContentUnpreview('label235');" title="click to collapse or expand..."> more... </a>
 <div id="label235" style="display:none">
 <table border="1">
 <tr>
 <td></td>
 <td colspan="1">Supported Version Ranges</td>
 </tr>
 <tr>
 <td>skip_check_for_unsupported_browser</td>
 <td><code class="docutils literal notranslate">v6.0.0 -> v6.0.11 </code></td>
 </tr>
 <tr>
 <td>[enable]</td>
 <td><code class="docutils literal notranslate">v6.0.0 -> latest</code></td> <tr>
 <td>[disable]</td>
 <td><code class="docutils literal notranslate">v6.0.0 -> latest</code></td> </table>
 </div>
 </li>
        <li> <span class="li-head">skip_check_for_unsupported_os</span> - Enable to skip host check if client OS does not support it. <span class="li-normal">type: str</span> <span class="li-normal">choices: enable, disable</span>
 <a id='label236' href="javascript:ContentClick('label237', 'label236');" onmouseover="ContentPreview('label237');" onmouseout="ContentUnpreview('label237');" title="click to collapse or expand..."> more... </a>
 <div id="label237" style="display:none">
 <table border="1">
 <tr>
 <td></td>
 <td colspan="1">Supported Version Ranges</td>
 </tr>
 <tr>
 <td>skip_check_for_unsupported_os</td>
 <td><code class="docutils literal notranslate">v6.0.0 -> latest </code></td>
 </tr>
 <tr>
 <td>[enable]</td>
 <td><code class="docutils literal notranslate">v6.0.0 -> latest</code></td> <tr>
 <td>[disable]</td>
 <td><code class="docutils literal notranslate">v6.0.0 -> latest</code></td> </table>
 </div>
 </li>
        <li> <span class="li-head">smb_max_version</span> - SMB maximum client protocol version. <span class="li-normal">type: str</span> <span class="li-normal">choices: smbv1, smbv2, smbv3</span>
 <a id='label238' href="javascript:ContentClick('label239', 'label238');" onmouseover="ContentPreview('label239');" onmouseout="ContentUnpreview('label239');" title="click to collapse or expand..."> more... </a>
 <div id="label239" style="display:none">
 <table border="1">
 <tr>
 <td></td>
 <td colspan="1">Supported Version Ranges</td>
 </tr>
 <tr>
 <td>smb_max_version</td>
 <td><code class="docutils literal notranslate">v6.2.0 -> latest </code></td>
 </tr>
 <tr>
 <td>[smbv1]</td>
 <td><code class="docutils literal notranslate">v6.0.0 -> latest</code></td> <tr>
 <td>[smbv2]</td>
 <td><code class="docutils literal notranslate">v6.0.0 -> latest</code></td> <tr>
 <td>[smbv3]</td>
 <td><code class="docutils literal notranslate">v6.0.0 -> latest</code></td> </table>
 </div>
 </li>
        <li> <span class="li-head">smb_min_version</span> - SMB minimum client protocol version. <span class="li-normal">type: str</span> <span class="li-normal">choices: smbv1, smbv2, smbv3</span>
 <a id='label240' href="javascript:ContentClick('label241', 'label240');" onmouseover="ContentPreview('label241');" onmouseout="ContentUnpreview('label241');" title="click to collapse or expand..."> more... </a>
 <div id="label241" style="display:none">
 <table border="1">
 <tr>
 <td></td>
 <td colspan="1">Supported Version Ranges</td>
 </tr>
 <tr>
 <td>smb_min_version</td>
 <td><code class="docutils literal notranslate">v6.2.0 -> latest </code></td>
 </tr>
 <tr>
 <td>[smbv1]</td>
 <td><code class="docutils literal notranslate">v6.0.0 -> latest</code></td> <tr>
 <td>[smbv2]</td>
 <td><code class="docutils literal notranslate">v6.0.0 -> latest</code></td> <tr>
 <td>[smbv3]</td>
 <td><code class="docutils literal notranslate">v6.0.0 -> latest</code></td> </table>
 </div>
 </li>
        <li> <span class="li-head">smb_ntlmv1_auth</span> - Enable support of NTLMv1 for Samba authentication. <span class="li-normal">type: str</span> <span class="li-normal">choices: enable, disable</span>
 <a id='label242' href="javascript:ContentClick('label243', 'label242');" onmouseover="ContentPreview('label243');" onmouseout="ContentUnpreview('label243');" title="click to collapse or expand..."> more... </a>
 <div id="label243" style="display:none">
 <table border="1">
 <tr>
 <td></td>
 <td colspan="1">Supported Version Ranges</td>
 </tr>
 <tr>
 <td>smb_ntlmv1_auth</td>
 <td><code class="docutils literal notranslate">v6.0.0 -> latest </code></td>
 </tr>
 <tr>
 <td>[enable]</td>
 <td><code class="docutils literal notranslate">v6.0.0 -> latest</code></td> <tr>
 <td>[disable]</td>
 <td><code class="docutils literal notranslate">v6.0.0 -> latest</code></td> </table>
 </div>
 </li>
        <li> <span class="li-head">smbv1</span> - SMB version 1. <span class="li-normal">type: str</span> <span class="li-normal">choices: enable, disable</span>
 <a id='label244' href="javascript:ContentClick('label245', 'label244');" onmouseover="ContentPreview('label245');" onmouseout="ContentUnpreview('label245');" title="click to collapse or expand..."> more... </a>
 <div id="label245" style="display:none">
 <table border="1">
 <tr>
 <td></td>
 <td colspan="1">Supported Version Ranges</td>
 </tr>
 <tr>
 <td>smbv1</td>
 <td><code class="docutils literal notranslate">v6.0.0 -> latest </code></td>
 </tr>
 <tr>
 <td>[enable]</td>
 <td><code class="docutils literal notranslate">v6.0.0 -> latest</code></td> <tr>
 <td>[disable]</td>
 <td><code class="docutils literal notranslate">v6.0.0 -> latest</code></td> </table>
 </div>
 </li>
        <li> <span class="li-head">split_dns</span> - Split DNS for SSL-VPN. <span class="li-normal">type: list</span> <span style="font-family:'Courier New'" class="li-required">member_path: split_dns:id</span>
 <a id='label246' href="javascript:ContentClick('label247', 'label246');" onmouseover="ContentPreview('label247');" onmouseout="ContentUnpreview('label247');" title="click to collapse or expand..."> more... </a>
 <div id="label247" style="display:none">
 <table border="1">
 <tr>
 <td></td><td colspan="1">Supported Version Ranges</td>
 </tr>
 <tr>
 <td>split_dns</td>
 <td><code class="docutils literal notranslate">v6.0.0 -> latest </code></td>
 </tr>
 </table>
 </div>
 </li>
            <ul class="ul-self">
            <li> <span class="li-head">dns_server1</span> - DNS server 1. <span class="li-normal">type: str</span>
 <a id='label248' href="javascript:ContentClick('label249', 'label248');" onmouseover="ContentPreview('label249');" onmouseout="ContentUnpreview('label249');" title="click to collapse or expand..."> more... </a>
 <div id="label249" style="display:none">
 <table border="1">
 <tr>
 <td></td>
 <td colspan="1">Supported Version Ranges</td>
 </tr>
 <tr>
 <td>dns_server1</td>
 <td><code class="docutils literal notranslate">v6.0.0 -> latest </code></td>
 </tr>
 </table>
 </div>
 </li>
            <li> <span class="li-head">dns_server2</span> - DNS server 2. <span class="li-normal">type: str</span>
 <a id='label250' href="javascript:ContentClick('label251', 'label250');" onmouseover="ContentPreview('label251');" onmouseout="ContentUnpreview('label251');" title="click to collapse or expand..."> more... </a>
 <div id="label251" style="display:none">
 <table border="1">
 <tr>
 <td></td>
 <td colspan="1">Supported Version Ranges</td>
 </tr>
 <tr>
 <td>dns_server2</td>
 <td><code class="docutils literal notranslate">v6.0.0 -> latest </code></td>
 </tr>
 </table>
 </div>
 </li>
            <li> <span class="li-head">domains</span> - Split DNS domains used for SSL-VPN clients separated by comma. <span class="li-normal">type: str</span>
 <a id='label252' href="javascript:ContentClick('label253', 'label252');" onmouseover="ContentPreview('label253');" onmouseout="ContentUnpreview('label253');" title="click to collapse or expand..."> more... </a>
 <div id="label253" style="display:none">
 <table border="1">
 <tr>
 <td></td>
 <td colspan="1">Supported Version Ranges</td>
 </tr>
 <tr>
 <td>domains</td>
 <td><code class="docutils literal notranslate">v6.0.0 -> latest </code></td>
 </tr>
 </table>
 </div>
 </li>
            <li> <span class="li-head">id</span> - ID. see <a href='#notes'>Notes</a>. <span class="li-normal">type: int</span> <span class="li-required">required: true</span>
 <a id='label254' href="javascript:ContentClick('label255', 'label254');" onmouseover="ContentPreview('label255');" onmouseout="ContentUnpreview('label255');" title="click to collapse or expand..."> more... </a>
 <div id="label255" style="display:none">
 <table border="1">
 <tr>
 <td></td>
 <td colspan="1">Supported Version Ranges</td>
 </tr>
 <tr>
 <td>id</td>
 <td><code class="docutils literal notranslate">v6.0.0 -> latest </code></td>
 </tr>
 </table>
 </div>
 </li>
            <li> <span class="li-head">ipv6_dns_server1</span> - IPv6 DNS server 1. <span class="li-normal">type: str</span>
 <a id='label256' href="javascript:ContentClick('label257', 'label256');" onmouseover="ContentPreview('label257');" onmouseout="ContentUnpreview('label257');" title="click to collapse or expand..."> more... </a>
 <div id="label257" style="display:none">
 <table border="1">
 <tr>
 <td></td>
 <td colspan="1">Supported Version Ranges</td>
 </tr>
 <tr>
 <td>ipv6_dns_server1</td>
 <td><code class="docutils literal notranslate">v6.0.0 -> latest </code></td>
 </tr>
 </table>
 </div>
 </li>
            <li> <span class="li-head">ipv6_dns_server2</span> - IPv6 DNS server 2. <span class="li-normal">type: str</span>
 <a id='label258' href="javascript:ContentClick('label259', 'label258');" onmouseover="ContentPreview('label259');" onmouseout="ContentUnpreview('label259');" title="click to collapse or expand..."> more... </a>
 <div id="label259" style="display:none">
 <table border="1">
 <tr>
 <td></td>
 <td colspan="1">Supported Version Ranges</td>
 </tr>
 <tr>
 <td>ipv6_dns_server2</td>
 <td><code class="docutils literal notranslate">v6.0.0 -> latest </code></td>
 </tr>
 </table>
 </div>
 </li>
            </ul>
        <li> <span class="li-head">split_tunneling</span> - Enable/disable IPv4 split tunneling. <span class="li-normal">type: str</span> <span class="li-normal">choices: enable, disable</span>
 <a id='label260' href="javascript:ContentClick('label261', 'label260');" onmouseover="ContentPreview('label261');" onmouseout="ContentUnpreview('label261');" title="click to collapse or expand..."> more... </a>
 <div id="label261" style="display:none">
 <table border="1">
 <tr>
 <td></td>
 <td colspan="1">Supported Version Ranges</td>
 </tr>
 <tr>
 <td>split_tunneling</td>
 <td><code class="docutils literal notranslate">v6.0.0 -> latest </code></td>
 </tr>
 <tr>
 <td>[enable]</td>
 <td><code class="docutils literal notranslate">v6.0.0 -> latest</code></td> <tr>
 <td>[disable]</td>
 <td><code class="docutils literal notranslate">v6.0.0 -> latest</code></td> </table>
 </div>
 </li>
        <li> <span class="li-head">split_tunneling_routing_address</span> - IPv4 SSL-VPN tunnel mode firewall address objects that override firewall policy destination addresses to control split-tunneling access. <span class="li-normal">type: list</span> <span style="font-family:'Courier New'" class="li-required">member_path: split_tunneling_routing_address:name</span>
 <a id='label262' href="javascript:ContentClick('label263', 'label262');" onmouseover="ContentPreview('label263');" onmouseout="ContentUnpreview('label263');" title="click to collapse or expand..."> more... </a>
 <div id="label263" style="display:none">
 <table border="1">
 <tr>
 <td></td><td colspan="1">Supported Version Ranges</td>
 </tr>
 <tr>
 <td>split_tunneling_routing_address</td>
 <td><code class="docutils literal notranslate">v6.0.0 -> latest </code></td>
 </tr>
 </table>
 </div>
 </li>
            <ul class="ul-self">
            <li> <span class="li-head">name</span> - Address name. Source firewall.address.name firewall.addrgrp.name. <span class="li-normal">type: str</span> <span class="li-required">required: true</span>
 <a id='label264' href="javascript:ContentClick('label265', 'label264');" onmouseover="ContentPreview('label265');" onmouseout="ContentUnpreview('label265');" title="click to collapse or expand..."> more... </a>
 <div id="label265" style="display:none">
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
            </ul>
        <li> <span class="li-head">split_tunneling_routing_negate</span> - Enable to negate split tunneling routing address. <span class="li-normal">type: str</span> <span class="li-normal">choices: enable, disable</span>
 <a id='label266' href="javascript:ContentClick('label267', 'label266');" onmouseover="ContentPreview('label267');" onmouseout="ContentUnpreview('label267');" title="click to collapse or expand..."> more... </a>
 <div id="label267" style="display:none">
 <table border="1">
 <tr>
 <td></td>
 <td colspan="1">Supported Version Ranges</td>
 </tr>
 <tr>
 <td>split_tunneling_routing_negate</td>
 <td><code class="docutils literal notranslate">v6.4.0 -> latest </code></td>
 </tr>
 <tr>
 <td>[enable]</td>
 <td><code class="docutils literal notranslate">v6.0.0 -> latest</code></td> <tr>
 <td>[disable]</td>
 <td><code class="docutils literal notranslate">v6.0.0 -> latest</code></td> </table>
 </div>
 </li>
        <li> <span class="li-head">theme</span> - Web portal color scheme. <span class="li-normal">type: str</span> <span class="li-normal">choices: jade, neutrino, mariner, graphite, melongene, jet-stream, security-fabric, dark-matter, onyx, eclipse, blue, green, red</span>
 <a id='label268' href="javascript:ContentClick('label269', 'label268');" onmouseover="ContentPreview('label269');" onmouseout="ContentUnpreview('label269');" title="click to collapse or expand..."> more... </a>
 <div id="label269" style="display:none">
 <table border="1">
 <tr>
 <td></td>
 <td colspan="1">Supported Version Ranges</td>
 </tr>
 <tr>
 <td>theme</td>
 <td><code class="docutils literal notranslate">v6.0.0 -> latest </code></td>
 </tr>
 <tr>
 <td>[jade]</td>
 <td><code class="docutils literal notranslate">v7.0.0 -> latest</code></td>
 </tr>
 <tr>
 <td>[neutrino]</td>
 <td><code class="docutils literal notranslate">v6.2.0 -> latest</code></td>
 </tr>
 <tr>
 <td>[mariner]</td>
 <td><code class="docutils literal notranslate">v6.0.0 -> latest</code></td> <tr>
 <td>[graphite]</td>
 <td><code class="docutils literal notranslate">v7.0.0 -> latest</code></td>
 </tr>
 <tr>
 <td>[melongene]</td>
 <td><code class="docutils literal notranslate">v6.0.0 -> latest</code></td> <tr>
 <td>[jet-stream]</td>
 <td><code class="docutils literal notranslate">v7.4.0 -> latest</code></td>
 </tr>
 <tr>
 <td>[security-fabric]</td>
 <td><code class="docutils literal notranslate">v7.4.0 -> latest</code></td>
 </tr>
 <tr>
 <td>[dark-matter]</td>
 <td><code class="docutils literal notranslate">v7.0.0 -> latest</code></td>
 </tr>
 <tr>
 <td>[onyx]</td>
 <td><code class="docutils literal notranslate">v7.0.0 -> latest</code></td>
 </tr>
 <tr>
 <td>[eclipse]</td>
 <td><code class="docutils literal notranslate">v7.0.0 -> latest</code></td>
 </tr>
 <tr>
 <td>[blue]</td>
 <td><code class="docutils literal notranslate">v6.0.0 -> v6.4.4</code></td>
 </tr>
 <tr>
 <td>[green]</td>
 <td><code class="docutils literal notranslate">v6.0.0 -> v6.4.4</code></td>
 </tr>
 <tr>
 <td>[red]</td>
 <td><code class="docutils literal notranslate">v6.0.0 -> v6.0.11</code></td>
 </tr>
 </table>
 </div>
 </li>
        <li> <span class="li-head">transform_backward_slashes</span> - Transform backward slashes to forward slashes in URLs. <span class="li-normal">type: str</span> <span class="li-normal">choices: enable, disable</span>
 <a id='label270' href="javascript:ContentClick('label271', 'label270');" onmouseover="ContentPreview('label271');" onmouseout="ContentUnpreview('label271');" title="click to collapse or expand..."> more... </a>
 <div id="label271" style="display:none">
 <table border="1">
 <tr>
 <td></td>
 <td colspan="1">Supported Version Ranges</td>
 </tr>
 <tr>
 <td>transform_backward_slashes</td>
 <td><code class="docutils literal notranslate">v6.2.0 -> v6.2.7 </code></td>
 </tr>
 <tr>
 <td>[enable]</td>
 <td><code class="docutils literal notranslate">v6.0.0 -> latest</code></td> <tr>
 <td>[disable]</td>
 <td><code class="docutils literal notranslate">v6.0.0 -> latest</code></td> </table>
 </div>
 </li>
        <li> <span class="li-head">tunnel_mode</span> - Enable/disable IPv4 SSL-VPN tunnel mode. <span class="li-normal">type: str</span> <span class="li-normal">choices: enable, disable</span>
 <a id='label272' href="javascript:ContentClick('label273', 'label272');" onmouseover="ContentPreview('label273');" onmouseout="ContentUnpreview('label273');" title="click to collapse or expand..."> more... </a>
 <div id="label273" style="display:none">
 <table border="1">
 <tr>
 <td></td>
 <td colspan="1">Supported Version Ranges</td>
 </tr>
 <tr>
 <td>tunnel_mode</td>
 <td><code class="docutils literal notranslate">v6.0.0 -> latest </code></td>
 </tr>
 <tr>
 <td>[enable]</td>
 <td><code class="docutils literal notranslate">v6.0.0 -> latest</code></td> <tr>
 <td>[disable]</td>
 <td><code class="docutils literal notranslate">v6.0.0 -> latest</code></td> </table>
 </div>
 </li>
        <li> <span class="li-head">use_sdwan</span> - Use SD-WAN rules to get output interface. <span class="li-normal">type: str</span> <span class="li-normal">choices: enable, disable</span>
 <a id='label274' href="javascript:ContentClick('label275', 'label274');" onmouseover="ContentPreview('label275');" onmouseout="ContentUnpreview('label275');" title="click to collapse or expand..."> more... </a>
 <div id="label275" style="display:none">
 <table border="1">
 <tr>
 <td></td>
 <td colspan="2">Supported Version Ranges</td>
 </tr>
 <tr>
 <td>use_sdwan</td>
 <td><code class="docutils literal notranslate">v6.2.7 -> v6.2.7 </code></td>
 <td><code class="docutils literal notranslate">v6.4.4 -> latest </code></td>
 </tr>
 <tr>
 <td>[enable]</td>
 <td><code class="docutils literal notranslate">v6.0.0 -> latest</code></td> <tr>
 <td>[disable]</td>
 <td><code class="docutils literal notranslate">v6.0.0 -> latest</code></td> </table>
 </div>
 </li>
        <li> <span class="li-head">user_bookmark</span> - Enable to allow web portal users to create their own bookmarks. <span class="li-normal">type: str</span> <span class="li-normal">choices: enable, disable</span>
 <a id='label276' href="javascript:ContentClick('label277', 'label276');" onmouseover="ContentPreview('label277');" onmouseout="ContentUnpreview('label277');" title="click to collapse or expand..."> more... </a>
 <div id="label277" style="display:none">
 <table border="1">
 <tr>
 <td></td>
 <td colspan="1">Supported Version Ranges</td>
 </tr>
 <tr>
 <td>user_bookmark</td>
 <td><code class="docutils literal notranslate">v6.0.0 -> latest </code></td>
 </tr>
 <tr>
 <td>[enable]</td>
 <td><code class="docutils literal notranslate">v6.0.0 -> latest</code></td> <tr>
 <td>[disable]</td>
 <td><code class="docutils literal notranslate">v6.0.0 -> latest</code></td> </table>
 </div>
 </li>
        <li> <span class="li-head">user_group_bookmark</span> - Enable to allow web portal users to create bookmarks for all users in the same user group. <span class="li-normal">type: str</span> <span class="li-normal">choices: enable, disable</span>
 <a id='label278' href="javascript:ContentClick('label279', 'label278');" onmouseover="ContentPreview('label279');" onmouseout="ContentUnpreview('label279');" title="click to collapse or expand..."> more... </a>
 <div id="label279" style="display:none">
 <table border="1">
 <tr>
 <td></td>
 <td colspan="1">Supported Version Ranges</td>
 </tr>
 <tr>
 <td>user_group_bookmark</td>
 <td><code class="docutils literal notranslate">v6.0.0 -> latest </code></td>
 </tr>
 <tr>
 <td>[enable]</td>
 <td><code class="docutils literal notranslate">v6.0.0 -> latest</code></td> <tr>
 <td>[disable]</td>
 <td><code class="docutils literal notranslate">v6.0.0 -> latest</code></td> </table>
 </div>
 </li>
        <li> <span class="li-head">web_mode</span> - Enable/disable SSL-VPN web mode. <span class="li-normal">type: str</span> <span class="li-normal">choices: enable, disable</span>
 <a id='label280' href="javascript:ContentClick('label281', 'label280');" onmouseover="ContentPreview('label281');" onmouseout="ContentUnpreview('label281');" title="click to collapse or expand..."> more... </a>
 <div id="label281" style="display:none">
 <table border="1">
 <tr>
 <td></td>
 <td colspan="1">Supported Version Ranges</td>
 </tr>
 <tr>
 <td>web_mode</td>
 <td><code class="docutils literal notranslate">v6.0.0 -> latest </code></td>
 </tr>
 <tr>
 <td>[enable]</td>
 <td><code class="docutils literal notranslate">v6.0.0 -> latest</code></td> <tr>
 <td>[disable]</td>
 <td><code class="docutils literal notranslate">v6.0.0 -> latest</code></td> </table>
 </div>
 </li>
        <li> <span class="li-head">windows_forticlient_download_url</span> - Download URL for Windows FortiClient. <span class="li-normal">type: str</span>
 <a id='label282' href="javascript:ContentClick('label283', 'label282');" onmouseover="ContentPreview('label283');" onmouseout="ContentUnpreview('label283');" title="click to collapse or expand..."> more... </a>
 <div id="label283" style="display:none">
 <table border="1">
 <tr>
 <td></td>
 <td colspan="1">Supported Version Ranges</td>
 </tr>
 <tr>
 <td>windows_forticlient_download_url</td>
 <td><code class="docutils literal notranslate">v6.0.0 -> latest </code></td>
 </tr>
 </table>
 </div>
 </li>
        <li> <span class="li-head">wins_server1</span> - IPv4 WINS server 1. <span class="li-normal">type: str</span>
 <a id='label284' href="javascript:ContentClick('label285', 'label284');" onmouseover="ContentPreview('label285');" onmouseout="ContentUnpreview('label285');" title="click to collapse or expand..."> more... </a>
 <div id="label285" style="display:none">
 <table border="1">
 <tr>
 <td></td>
 <td colspan="1">Supported Version Ranges</td>
 </tr>
 <tr>
 <td>wins_server1</td>
 <td><code class="docutils literal notranslate">v6.0.0 -> latest </code></td>
 </tr>
 </table>
 </div>
 </li>
        <li> <span class="li-head">wins_server2</span> - IPv4 WINS server 1. <span class="li-normal">type: str</span>
 <a id='label286' href="javascript:ContentClick('label287', 'label286');" onmouseover="ContentPreview('label287');" onmouseout="ContentUnpreview('label287');" title="click to collapse or expand..."> more... </a>
 <div id="label287" style="display:none">
 <table border="1">
 <tr>
 <td></td>
 <td colspan="1">Supported Version Ranges</td>
 </tr>
 <tr>
 <td>wins_server2</td>
 <td><code class="docutils literal notranslate">v6.0.0 -> latest </code></td>
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
    
    - name: Portal.
      fortinet.fortios.fortios_vpn_ssl_web_portal:
          vdom: "{{ vdom }}"
          state: "present"
          access_token: "<your_own_value>"
          vpn_ssl_web_portal:
              allow_user_access: "web"
              auto_connect: "enable"
              bookmark_group:
                  -
                      bookmarks:
                          -
                              additional_params: "<your_own_value>"
                              apptype: "ftp"
                              color_depth: "32"
                              description: "<your_own_value>"
                              domain: "<your_own_value>"
                              folder: "<your_own_value>"
                              form_data:
                                  -
                                      name: "default_name_14"
                                      value: "<your_own_value>"
                              height: "768"
                              host: "myhostname"
                              keyboard_layout: "ar-101"
                              listening_port: "0"
                              load_balancing_info: "<your_own_value>"
                              logon_password: "<your_own_value>"
                              logon_user: "<your_own_value>"
                              name: "default_name_23"
                              port: "0"
                              preconnection_blob: "<your_own_value>"
                              preconnection_id: "2147483648"
                              remote_port: "0"
                              restricted_admin: "enable"
                              security: "any"
                              send_preconnection_id: "enable"
                              server_layout: "de-de-qwertz"
                              show_status_window: "enable"
                              sso: "disable"
                              sso_credential: "sslvpn-login"
                              sso_credential_sent_once: "enable"
                              sso_password: "<your_own_value>"
                              sso_username: "<your_own_value>"
                              url: "myurl.com"
                              vnc_keyboard_layout: "default"
                              width: "1024"
                      name: "default_name_41"
              client_src_range: "enable"
              clipboard: "enable"
              custom_lang: "<your_own_value> (source system.custom-language.name)"
              customize_forticlient_download_url: "enable"
              default_protocol: "web"
              default_window_height: "768"
              default_window_width: "1024"
              dhcp_ip_overlap: "use-new"
              dhcp_ra_giaddr: "<your_own_value>"
              dhcp6_ra_linkaddr: "<your_own_value>"
              display_bookmark: "enable"
              display_connection_tools: "enable"
              display_history: "enable"
              display_status: "enable"
              dns_server1: "<your_own_value>"
              dns_server2: "<your_own_value>"
              dns_suffix: "<your_own_value>"
              exclusive_routing: "enable"
              focus_bookmark: "enable"
              forticlient_download: "enable"
              forticlient_download_method: "direct"
              heading: "<your_own_value>"
              hide_sso_credential: "enable"
              host_check: "none"
              host_check_interval: "0"
              host_check_policy:
                  -
                      name: "default_name_68 (source vpn.ssl.web.host-check-software.name)"
              ip_mode: "range"
              ip_pools:
                  -
                      name: "default_name_71 (source firewall.address.name firewall.addrgrp.name)"
              ipv6_dns_server1: "<your_own_value>"
              ipv6_dns_server2: "<your_own_value>"
              ipv6_exclusive_routing: "enable"
              ipv6_pools:
                  -
                      name: "default_name_76 (source firewall.address6.name firewall.addrgrp6.name)"
              ipv6_service_restriction: "enable"
              ipv6_split_tunneling: "enable"
              ipv6_split_tunneling_routing_address:
                  -
                      name: "default_name_80 (source firewall.address6.name firewall.addrgrp6.name)"
              ipv6_split_tunneling_routing_negate: "enable"
              ipv6_tunnel_mode: "enable"
              ipv6_wins_server1: "<your_own_value>"
              ipv6_wins_server2: "<your_own_value>"
              keep_alive: "enable"
              landing_page:
                  form_data:
                      -
                          name: "default_name_88"
                          value: "<your_own_value>"
                  logout_url: "<your_own_value>"
                  sso: "disable"
                  sso_credential: "sslvpn-login"
                  sso_password: "<your_own_value>"
                  sso_username: "<your_own_value>"
                  url: "myurl.com"
              landing_page_mode: "enable"
              limit_user_logins: "enable"
              mac_addr_action: "allow"
              mac_addr_check: "enable"
              mac_addr_check_rule:
                  -
                      mac_addr_list:
                          -
                              addr: "<your_own_value>"
                      mac_addr_mask: "48"
                      name: "default_name_104"
              macos_forticlient_download_url: "<your_own_value>"
              name: "default_name_106"
              os_check: "enable"
              os_check_list:
                  -
                      action: "deny"
                      latest_patch_level: "<your_own_value>"
                      name: "default_name_111"
                      tolerance: "0"
              prefer_ipv6_dns: "enable"
              redir_url: "<your_own_value>"
              rewrite_ip_uri_ui: "enable"
              save_password: "enable"
              service_restriction: "enable"
              skip_check_for_browser: "enable"
              skip_check_for_unsupported_browser: "enable"
              skip_check_for_unsupported_os: "enable"
              smb_max_version: "smbv1"
              smb_min_version: "smbv1"
              smb_ntlmv1_auth: "enable"
              smbv1: "enable"
              split_dns:
                  -
                      dns_server1: "<your_own_value>"
                      dns_server2: "<your_own_value>"
                      domains: "<your_own_value>"
                      id: "129"
                      ipv6_dns_server1: "<your_own_value>"
                      ipv6_dns_server2: "<your_own_value>"
              split_tunneling: "enable"
              split_tunneling_routing_address:
                  -
                      name: "default_name_134 (source firewall.address.name firewall.addrgrp.name)"
              split_tunneling_routing_negate: "enable"
              theme: "jade"
              transform_backward_slashes: "enable"
              tunnel_mode: "enable"
              use_sdwan: "enable"
              user_bookmark: "enable"
              user_group_bookmark: "enable"
              web_mode: "enable"
              windows_forticlient_download_url: "<your_own_value>"
              wins_server1: "<your_own_value>"
              wins_server2: "<your_own_value>"


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
