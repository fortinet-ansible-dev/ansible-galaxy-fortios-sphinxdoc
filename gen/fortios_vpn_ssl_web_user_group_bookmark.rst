:source: fortios_vpn_ssl_web_user_group_bookmark.py

:orphan:

.. fortios_vpn_ssl_web_user_group_bookmark:

fortios_vpn_ssl_web_user_group_bookmark -- Configure SSL-VPN user group bookmark in Fortinet's FortiOS and FortiGate.
+++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++

.. versionadded:: 2.0.0

.. contents::
   :local:
   :depth: 1


Synopsis
--------
- This module is able to configure a FortiGate or FortiOS (FOS) device by allowing the user to set and modify vpn_ssl_web feature and user_group_bookmark category. Examples include all parameters and values need to be adjusted to datasources before usage. Tested with FOS v6.0.0



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
    <li> <span class="li-head">vpn_ssl_web_user_group_bookmark</span> - Configure SSL-VPN user group bookmark. <span class="li-normal">type: dict</span>
 <a id='label0' href="javascript:ContentClick('label1', 'label0');" onmouseover="ContentPreview('label1');" onmouseout="ContentUnpreview('label1');" title="click to collapse or expand..."> more... </a>
 <div id="label1" style="display:none">
 <table border="1">
 <tr>
 <td></td><td colspan="1">Supported Version Ranges</td>
 </tr>
 <tr>
 <td>vpn_ssl_web_user_group_bookmark</td>
 <td><code class="docutils literal notranslate">v6.0.0 -> 7.6.2 </code></td>
 </tr>
 </table>
 </div>
 </li>
        <ul class="ul-self">
        <li> <span class="li-head">bookmarks</span> - Bookmark table. <span class="li-normal">type: list</span> <span style="font-family:'Courier New'" class="li-required">member_path: bookmarks:name</span>
 <a id='label2' href="javascript:ContentClick('label3', 'label2');" onmouseover="ContentPreview('label3');" onmouseout="ContentUnpreview('label3');" title="click to collapse or expand..."> more... </a>
 <div id="label3" style="display:none">
 <table border="1">
 <tr>
 <td></td><td colspan="1">Supported Version Ranges</td>
 </tr>
 <tr>
 <td>bookmarks</td>
 <td><code class="docutils literal notranslate">v6.0.0 -> 7.6.2 </code></td>
 </tr>
 </table>
 </div>
 </li>
            <ul class="ul-self">
            <li> <span class="li-head">additional_params</span> - Additional parameters. <span class="li-normal">type: str</span>
 <a id='label4' href="javascript:ContentClick('label5', 'label4');" onmouseover="ContentPreview('label5');" onmouseout="ContentUnpreview('label5');" title="click to collapse or expand..."> more... </a>
 <div id="label5" style="display:none">
 <table border="1">
 <tr>
 <td></td>
 <td colspan="1">Supported Version Ranges</td>
 </tr>
 <tr>
 <td>additional_params</td>
 <td><code class="docutils literal notranslate">v6.0.0 -> 7.6.2 </code></td>
 </tr>
 </table>
 </div>
 </li>
            <li> <span class="li-head">apptype</span> - Application type. <span class="li-normal">type: str</span> <span class="li-normal">choices: ftp, rdp, sftp, smb, ssh, telnet, vnc, web, citrix, portforward</span>
 <a id='label6' href="javascript:ContentClick('label7', 'label6');" onmouseover="ContentPreview('label7');" onmouseout="ContentUnpreview('label7');" title="click to collapse or expand..."> more... </a>
 <div id="label7" style="display:none">
 <table border="1">
 <tr>
 <td></td>
 <td colspan="1">Supported Version Ranges</td>
 </tr>
 <tr>
 <td>apptype</td>
 <td><code class="docutils literal notranslate">v6.0.0 -> 7.6.2 </code></td>
 </tr>
 <tr>
 <td>[ftp]</td>
 <td><code class="docutils literal notranslate">v6.0.0 -> 7.6.2</code></td>
 <tr>
 <td>[rdp]</td>
 <td><code class="docutils literal notranslate">v6.0.0 -> 7.6.2</code></td>
 <tr>
 <td>[sftp]</td>
 <td><code class="docutils literal notranslate">v6.2.0 -> 7.6.2</code></td>
 </tr>
 <tr>
 <td>[smb]</td>
 <td><code class="docutils literal notranslate">v6.0.0 -> 7.6.2</code></td>
 <tr>
 <td>[ssh]</td>
 <td><code class="docutils literal notranslate">v6.0.0 -> 7.6.2</code></td>
 <tr>
 <td>[telnet]</td>
 <td><code class="docutils literal notranslate">v6.0.0 -> 7.6.2</code></td>
 <tr>
 <td>[vnc]</td>
 <td><code class="docutils literal notranslate">v6.0.0 -> 7.6.2</code></td>
 <tr>
 <td>[web]</td>
 <td><code class="docutils literal notranslate">v6.0.0 -> 7.6.2</code></td>
 <tr>
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
 <a id='label8' href="javascript:ContentClick('label9', 'label8');" onmouseover="ContentPreview('label9');" onmouseout="ContentUnpreview('label9');" title="click to collapse or expand..."> more... </a>
 <div id="label9" style="display:none">
 <table border="1">
 <tr>
 <td></td>
 <td colspan="1">Supported Version Ranges</td>
 </tr>
 <tr>
 <td>color_depth</td>
 <td><code class="docutils literal notranslate">v7.0.1 -> 7.6.2 </code></td>
 </tr>
 <tr>
 <td>[32]</td>
 <td><code class="docutils literal notranslate">v7.0.1 -> 7.6.2</code></td>
 <tr>
 <td>[16]</td>
 <td><code class="docutils literal notranslate">v7.0.1 -> 7.6.2</code></td>
 <tr>
 <td>[8]</td>
 <td><code class="docutils literal notranslate">v7.0.1 -> 7.6.2</code></td>
 </table>
 </div>
 </li>
            <li> <span class="li-head">description</span> - Description. <span class="li-normal">type: str</span>
 <a id='label10' href="javascript:ContentClick('label11', 'label10');" onmouseover="ContentPreview('label11');" onmouseout="ContentUnpreview('label11');" title="click to collapse or expand..."> more... </a>
 <div id="label11" style="display:none">
 <table border="1">
 <tr>
 <td></td>
 <td colspan="1">Supported Version Ranges</td>
 </tr>
 <tr>
 <td>description</td>
 <td><code class="docutils literal notranslate">v6.0.0 -> 7.6.2 </code></td>
 </tr>
 </table>
 </div>
 </li>
            <li> <span class="li-head">domain</span> - Login domain. <span class="li-normal">type: str</span>
 <a id='label12' href="javascript:ContentClick('label13', 'label12');" onmouseover="ContentPreview('label13');" onmouseout="ContentUnpreview('label13');" title="click to collapse or expand..."> more... </a>
 <div id="label13" style="display:none">
 <table border="1">
 <tr>
 <td></td>
 <td colspan="2">Supported Version Ranges</td>
 </tr>
 <tr>
 <td>domain</td>
 <td><code class="docutils literal notranslate">v6.4.0 -> v6.4.0 </code></td>
 <td><code class="docutils literal notranslate">v6.4.4 -> 7.6.2 </code></td>
 </tr>
 </table>
 </div>
 </li>
            <li> <span class="li-head">folder</span> - Network shared file folder parameter. <span class="li-normal">type: str</span>
 <a id='label14' href="javascript:ContentClick('label15', 'label14');" onmouseover="ContentPreview('label15');" onmouseout="ContentUnpreview('label15');" title="click to collapse or expand..."> more... </a>
 <div id="label15" style="display:none">
 <table border="1">
 <tr>
 <td></td>
 <td colspan="1">Supported Version Ranges</td>
 </tr>
 <tr>
 <td>folder</td>
 <td><code class="docutils literal notranslate">v6.0.0 -> 7.6.2 </code></td>
 </tr>
 </table>
 </div>
 </li>
            <li> <span class="li-head">form_data</span> - Form data. <span class="li-normal">type: list</span> <span style="font-family:'Courier New'" class="li-required">member_path: bookmarks:name/form_data:name</span>
 <a id='label16' href="javascript:ContentClick('label17', 'label16');" onmouseover="ContentPreview('label17');" onmouseout="ContentUnpreview('label17');" title="click to collapse or expand..."> more... </a>
 <div id="label17" style="display:none">
 <table border="1">
 <tr>
 <td></td><td colspan="1">Supported Version Ranges</td>
 </tr>
 <tr>
 <td>form_data</td>
 <td><code class="docutils literal notranslate">v6.0.0 -> 7.6.2 </code></td>
 </tr>
 </table>
 </div>
 </li>
                <ul class="ul-self">
                <li> <span class="li-head">name</span> - Name. <span class="li-normal">type: str</span> <span class="li-required">required: true</span>
 <a id='label18' href="javascript:ContentClick('label19', 'label18');" onmouseover="ContentPreview('label19');" onmouseout="ContentUnpreview('label19');" title="click to collapse or expand..."> more... </a>
 <div id="label19" style="display:none">
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
                <li> <span class="li-head">value</span> - Value. <span class="li-normal">type: str</span>
 <a id='label20' href="javascript:ContentClick('label21', 'label20');" onmouseover="ContentPreview('label21');" onmouseout="ContentUnpreview('label21');" title="click to collapse or expand..."> more... </a>
 <div id="label21" style="display:none">
 <table border="1">
 <tr>
 <td></td>
 <td colspan="1">Supported Version Ranges</td>
 </tr>
 <tr>
 <td>value</td>
 <td><code class="docutils literal notranslate">v6.0.0 -> 7.6.2 </code></td>
 </tr>
 </table>
 </div>
 </li>
                </ul>
            <li> <span class="li-head">height</span> - Screen height (range from 0 - 65535). <span class="li-normal">type: int</span>
 <a id='label22' href="javascript:ContentClick('label23', 'label22');" onmouseover="ContentPreview('label23');" onmouseout="ContentUnpreview('label23');" title="click to collapse or expand..."> more... </a>
 <div id="label23" style="display:none">
 <table border="1">
 <tr>
 <td></td>
 <td colspan="1">Supported Version Ranges</td>
 </tr>
 <tr>
 <td>height</td>
 <td><code class="docutils literal notranslate">v7.0.4 -> 7.6.2 </code></td>
 </tr>
 </table>
 </div>
 </li>
            <li> <span class="li-head">host</span> - Host name/IP parameter. <span class="li-normal">type: str</span>
 <a id='label24' href="javascript:ContentClick('label25', 'label24');" onmouseover="ContentPreview('label25');" onmouseout="ContentUnpreview('label25');" title="click to collapse or expand..."> more... </a>
 <div id="label25" style="display:none">
 <table border="1">
 <tr>
 <td></td>
 <td colspan="1">Supported Version Ranges</td>
 </tr>
 <tr>
 <td>host</td>
 <td><code class="docutils literal notranslate">v6.0.0 -> 7.6.2 </code></td>
 </tr>
 </table>
 </div>
 </li>
            <li> <span class="li-head">keyboard_layout</span> - Keyboard layout. <span class="li-normal">type: str</span> <span class="li-normal">choices: ar-101, ar-102, ar-102-azerty, can-mul, cz, cz-qwerty, cz-pr, da, nl, de, de-ch, de-ibm, en-uk, en-uk-ext, en-us, en-us-dvorak, es, es-var, fi, fi-sami, fr, fr-apple, fr-ca, fr-ch, fr-be, hr, hu, hu-101, it, it-142, ja, ja-106, ko, la-am, lt, lt-ibm, lt-std, lav-std, lav-leg, mk, mk-std, no, no-sami, pol-214, pol-pr, pt, pt-br, pt-br-abnt2, ru, ru-mne, ru-t, sl, sv, sv-sami, tuk, tur-f, tur-q, zh-sym-sg-us, zh-sym-us, zh-tr-hk, zh-tr-mo, zh-tr-us</span>
 <a id='label26' href="javascript:ContentClick('label27', 'label26');" onmouseover="ContentPreview('label27');" onmouseout="ContentUnpreview('label27');" title="click to collapse or expand..."> more... </a>
 <div id="label27" style="display:none">
 <table border="1">
 <tr>
 <td></td>
 <td colspan="1">Supported Version Ranges</td>
 </tr>
 <tr>
 <td>keyboard_layout</td>
 <td><code class="docutils literal notranslate">v7.0.1 -> 7.6.2 </code></td>
 </tr>
 <tr>
 <td>[ar-101]</td>
 <td><code class="docutils literal notranslate">v7.0.1 -> 7.6.2</code></td>
 <tr>
 <td>[ar-102]</td>
 <td><code class="docutils literal notranslate">v7.0.1 -> 7.6.2</code></td>
 <tr>
 <td>[ar-102-azerty]</td>
 <td><code class="docutils literal notranslate">v7.0.1 -> 7.6.2</code></td>
 <tr>
 <td>[can-mul]</td>
 <td><code class="docutils literal notranslate">v7.0.1 -> 7.6.2</code></td>
 <tr>
 <td>[cz]</td>
 <td><code class="docutils literal notranslate">v7.0.1 -> 7.6.2</code></td>
 <tr>
 <td>[cz-qwerty]</td>
 <td><code class="docutils literal notranslate">v7.0.1 -> 7.6.2</code></td>
 <tr>
 <td>[cz-pr]</td>
 <td><code class="docutils literal notranslate">v7.0.1 -> 7.6.2</code></td>
 <tr>
 <td>[da]</td>
 <td><code class="docutils literal notranslate">v7.0.1 -> 7.6.2</code></td>
 <tr>
 <td>[nl]</td>
 <td><code class="docutils literal notranslate">v7.0.1 -> 7.6.2</code></td>
 <tr>
 <td>[de]</td>
 <td><code class="docutils literal notranslate">v7.0.1 -> 7.6.2</code></td>
 <tr>
 <td>[de-ch]</td>
 <td><code class="docutils literal notranslate">v7.0.1 -> 7.6.2</code></td>
 <tr>
 <td>[de-ibm]</td>
 <td><code class="docutils literal notranslate">v7.0.1 -> 7.6.2</code></td>
 <tr>
 <td>[en-uk]</td>
 <td><code class="docutils literal notranslate">v7.0.1 -> 7.6.2</code></td>
 <tr>
 <td>[en-uk-ext]</td>
 <td><code class="docutils literal notranslate">v7.0.1 -> 7.6.2</code></td>
 <tr>
 <td>[en-us]</td>
 <td><code class="docutils literal notranslate">v7.0.1 -> 7.6.2</code></td>
 <tr>
 <td>[en-us-dvorak]</td>
 <td><code class="docutils literal notranslate">v7.0.1 -> 7.6.2</code></td>
 <tr>
 <td>[es]</td>
 <td><code class="docutils literal notranslate">v7.0.1 -> 7.6.2</code></td>
 <tr>
 <td>[es-var]</td>
 <td><code class="docutils literal notranslate">v7.0.1 -> 7.6.2</code></td>
 <tr>
 <td>[fi]</td>
 <td><code class="docutils literal notranslate">v7.0.1 -> 7.6.2</code></td>
 <tr>
 <td>[fi-sami]</td>
 <td><code class="docutils literal notranslate">v7.0.1 -> 7.6.2</code></td>
 <tr>
 <td>[fr]</td>
 <td><code class="docutils literal notranslate">v7.0.1 -> 7.6.2</code></td>
 <tr>
 <td>[fr-apple]</td>
 <td><code class="docutils literal notranslate">v7.0.6 -> 7.6.2</code></td>
 </tr>
 <tr>
 <td>[fr-ca]</td>
 <td><code class="docutils literal notranslate">v7.0.1 -> 7.6.2</code></td>
 <tr>
 <td>[fr-ch]</td>
 <td><code class="docutils literal notranslate">v7.0.1 -> 7.6.2</code></td>
 <tr>
 <td>[fr-be]</td>
 <td><code class="docutils literal notranslate">v7.0.1 -> 7.6.2</code></td>
 <tr>
 <td>[hr]</td>
 <td><code class="docutils literal notranslate">v7.0.1 -> 7.6.2</code></td>
 <tr>
 <td>[hu]</td>
 <td><code class="docutils literal notranslate">v7.0.1 -> 7.6.2</code></td>
 <tr>
 <td>[hu-101]</td>
 <td><code class="docutils literal notranslate">v7.0.1 -> 7.6.2</code></td>
 <tr>
 <td>[it]</td>
 <td><code class="docutils literal notranslate">v7.0.1 -> 7.6.2</code></td>
 <tr>
 <td>[it-142]</td>
 <td><code class="docutils literal notranslate">v7.0.1 -> 7.6.2</code></td>
 <tr>
 <td>[ja]</td>
 <td><code class="docutils literal notranslate">v7.0.1 -> 7.6.2</code></td>
 <tr>
 <td>[ja-106]</td>
 <td><code class="docutils literal notranslate">v7.4.2 -> 7.6.2</code></td>
 </tr>
 <tr>
 <td>[ko]</td>
 <td><code class="docutils literal notranslate">v7.0.1 -> 7.6.2</code></td>
 <tr>
 <td>[la-am]</td>
 <td><code class="docutils literal notranslate">v7.4.1 -> 7.6.2</code></td>
 </tr>
 <tr>
 <td>[lt]</td>
 <td><code class="docutils literal notranslate">v7.0.1 -> 7.6.2</code></td>
 <tr>
 <td>[lt-ibm]</td>
 <td><code class="docutils literal notranslate">v7.0.1 -> 7.6.2</code></td>
 <tr>
 <td>[lt-std]</td>
 <td><code class="docutils literal notranslate">v7.0.1 -> 7.6.2</code></td>
 <tr>
 <td>[lav-std]</td>
 <td><code class="docutils literal notranslate">v7.0.1 -> 7.6.2</code></td>
 <tr>
 <td>[lav-leg]</td>
 <td><code class="docutils literal notranslate">v7.0.1 -> 7.6.2</code></td>
 <tr>
 <td>[mk]</td>
 <td><code class="docutils literal notranslate">v7.0.1 -> 7.6.2</code></td>
 <tr>
 <td>[mk-std]</td>
 <td><code class="docutils literal notranslate">v7.0.1 -> 7.6.2</code></td>
 <tr>
 <td>[no]</td>
 <td><code class="docutils literal notranslate">v7.0.1 -> 7.6.2</code></td>
 <tr>
 <td>[no-sami]</td>
 <td><code class="docutils literal notranslate">v7.0.1 -> 7.6.2</code></td>
 <tr>
 <td>[pol-214]</td>
 <td><code class="docutils literal notranslate">v7.0.1 -> 7.6.2</code></td>
 <tr>
 <td>[pol-pr]</td>
 <td><code class="docutils literal notranslate">v7.0.1 -> 7.6.2</code></td>
 <tr>
 <td>[pt]</td>
 <td><code class="docutils literal notranslate">v7.0.1 -> 7.6.2</code></td>
 <tr>
 <td>[pt-br]</td>
 <td><code class="docutils literal notranslate">v7.0.1 -> 7.6.2</code></td>
 <tr>
 <td>[pt-br-abnt2]</td>
 <td><code class="docutils literal notranslate">v7.0.1 -> 7.6.2</code></td>
 <tr>
 <td>[ru]</td>
 <td><code class="docutils literal notranslate">v7.0.1 -> 7.6.2</code></td>
 <tr>
 <td>[ru-mne]</td>
 <td><code class="docutils literal notranslate">v7.0.1 -> 7.6.2</code></td>
 <tr>
 <td>[ru-t]</td>
 <td><code class="docutils literal notranslate">v7.0.1 -> 7.6.2</code></td>
 <tr>
 <td>[sl]</td>
 <td><code class="docutils literal notranslate">v7.0.1 -> 7.6.2</code></td>
 <tr>
 <td>[sv]</td>
 <td><code class="docutils literal notranslate">v7.0.1 -> 7.6.2</code></td>
 <tr>
 <td>[sv-sami]</td>
 <td><code class="docutils literal notranslate">v7.0.1 -> 7.6.2</code></td>
 <tr>
 <td>[tuk]</td>
 <td><code class="docutils literal notranslate">v7.0.1 -> 7.6.2</code></td>
 <tr>
 <td>[tur-f]</td>
 <td><code class="docutils literal notranslate">v7.0.1 -> 7.6.2</code></td>
 <tr>
 <td>[tur-q]</td>
 <td><code class="docutils literal notranslate">v7.0.1 -> 7.6.2</code></td>
 <tr>
 <td>[zh-sym-sg-us]</td>
 <td><code class="docutils literal notranslate">v7.0.1 -> 7.6.2</code></td>
 <tr>
 <td>[zh-sym-us]</td>
 <td><code class="docutils literal notranslate">v7.0.1 -> 7.6.2</code></td>
 <tr>
 <td>[zh-tr-hk]</td>
 <td><code class="docutils literal notranslate">v7.0.1 -> 7.6.2</code></td>
 <tr>
 <td>[zh-tr-mo]</td>
 <td><code class="docutils literal notranslate">v7.0.1 -> 7.6.2</code></td>
 <tr>
 <td>[zh-tr-us]</td>
 <td><code class="docutils literal notranslate">v7.0.1 -> 7.6.2</code></td>
 </table>
 </div>
 </li>
            <li> <span class="li-head">listening_port</span> - Listening port (0 - 65535). <span class="li-normal">type: int</span>
 <a id='label28' href="javascript:ContentClick('label29', 'label28');" onmouseover="ContentPreview('label29');" onmouseout="ContentUnpreview('label29');" title="click to collapse or expand..."> more... </a>
 <div id="label29" style="display:none">
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
 <a id='label30' href="javascript:ContentClick('label31', 'label30');" onmouseover="ContentPreview('label31');" onmouseout="ContentUnpreview('label31');" title="click to collapse or expand..."> more... </a>
 <div id="label31" style="display:none">
 <table border="1">
 <tr>
 <td></td>
 <td colspan="1">Supported Version Ranges</td>
 </tr>
 <tr>
 <td>load_balancing_info</td>
 <td><code class="docutils literal notranslate">v6.0.0 -> 7.6.2 </code></td>
 </tr>
 </table>
 </div>
 </li>
            <li> <span class="li-head">logon_password</span> - Logon password. <span class="li-normal">type: str</span>
 <a id='label32' href="javascript:ContentClick('label33', 'label32');" onmouseover="ContentPreview('label33');" onmouseout="ContentUnpreview('label33');" title="click to collapse or expand..."> more... </a>
 <div id="label33" style="display:none">
 <table border="1">
 <tr>
 <td></td>
 <td colspan="1">Supported Version Ranges</td>
 </tr>
 <tr>
 <td>logon_password</td>
 <td><code class="docutils literal notranslate">v6.0.0 -> 7.6.2 </code></td>
 </tr>
 </table>
 </div>
 </li>
            <li> <span class="li-head">logon_user</span> - Logon user. <span class="li-normal">type: str</span>
 <a id='label34' href="javascript:ContentClick('label35', 'label34');" onmouseover="ContentPreview('label35');" onmouseout="ContentUnpreview('label35');" title="click to collapse or expand..."> more... </a>
 <div id="label35" style="display:none">
 <table border="1">
 <tr>
 <td></td>
 <td colspan="1">Supported Version Ranges</td>
 </tr>
 <tr>
 <td>logon_user</td>
 <td><code class="docutils literal notranslate">v6.0.0 -> 7.6.2 </code></td>
 </tr>
 </table>
 </div>
 </li>
            <li> <span class="li-head">name</span> - Bookmark name. <span class="li-normal">type: str</span> <span class="li-required">required: true</span>
 <a id='label36' href="javascript:ContentClick('label37', 'label36');" onmouseover="ContentPreview('label37');" onmouseout="ContentUnpreview('label37');" title="click to collapse or expand..."> more... </a>
 <div id="label37" style="display:none">
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
            <li> <span class="li-head">port</span> - Remote port. <span class="li-normal">type: int</span>
 <a id='label38' href="javascript:ContentClick('label39', 'label38');" onmouseover="ContentPreview('label39');" onmouseout="ContentUnpreview('label39');" title="click to collapse or expand..."> more... </a>
 <div id="label39" style="display:none">
 <table border="1">
 <tr>
 <td></td>
 <td colspan="1">Supported Version Ranges</td>
 </tr>
 <tr>
 <td>port</td>
 <td><code class="docutils literal notranslate">v6.0.0 -> 7.6.2 </code></td>
 </tr>
 </table>
 </div>
 </li>
            <li> <span class="li-head">preconnection_blob</span> - An arbitrary string which identifies the RDP source. <span class="li-normal">type: str</span>
 <a id='label40' href="javascript:ContentClick('label41', 'label40');" onmouseover="ContentPreview('label41');" onmouseout="ContentUnpreview('label41');" title="click to collapse or expand..."> more... </a>
 <div id="label41" style="display:none">
 <table border="1">
 <tr>
 <td></td>
 <td colspan="1">Supported Version Ranges</td>
 </tr>
 <tr>
 <td>preconnection_blob</td>
 <td><code class="docutils literal notranslate">v6.0.0 -> 7.6.2 </code></td>
 </tr>
 </table>
 </div>
 </li>
            <li> <span class="li-head">preconnection_id</span> - The numeric ID of the RDP source (0-4294967295). <span class="li-normal">type: int</span>
 <a id='label42' href="javascript:ContentClick('label43', 'label42');" onmouseover="ContentPreview('label43');" onmouseout="ContentUnpreview('label43');" title="click to collapse or expand..."> more... </a>
 <div id="label43" style="display:none">
 <table border="1">
 <tr>
 <td></td>
 <td colspan="1">Supported Version Ranges</td>
 </tr>
 <tr>
 <td>preconnection_id</td>
 <td><code class="docutils literal notranslate">v6.0.0 -> 7.6.2 </code></td>
 </tr>
 </table>
 </div>
 </li>
            <li> <span class="li-head">remote_port</span> - Remote port (0 - 65535). <span class="li-normal">type: int</span>
 <a id='label44' href="javascript:ContentClick('label45', 'label44');" onmouseover="ContentPreview('label45');" onmouseout="ContentUnpreview('label45');" title="click to collapse or expand..."> more... </a>
 <div id="label45" style="display:none">
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
 <a id='label46' href="javascript:ContentClick('label47', 'label46');" onmouseover="ContentPreview('label47');" onmouseout="ContentUnpreview('label47');" title="click to collapse or expand..."> more... </a>
 <div id="label47" style="display:none">
 <table border="1">
 <tr>
 <td></td>
 <td colspan="1">Supported Version Ranges</td>
 </tr>
 <tr>
 <td>restricted_admin</td>
 <td><code class="docutils literal notranslate">v7.0.1 -> 7.6.2 </code></td>
 </tr>
 <tr>
 <td>[enable]</td>
 <td><code class="docutils literal notranslate">v7.0.1 -> 7.6.2</code></td>
 <tr>
 <td>[disable]</td>
 <td><code class="docutils literal notranslate">v7.0.1 -> 7.6.2</code></td>
 </table>
 </div>
 </li>
            <li> <span class="li-head">security</span> - Security mode for RDP connection . <span class="li-normal">type: str</span> <span class="li-normal">choices: any, rdp, nla, tls</span>
 <a id='label48' href="javascript:ContentClick('label49', 'label48');" onmouseover="ContentPreview('label49');" onmouseout="ContentUnpreview('label49');" title="click to collapse or expand..."> more... </a>
 <div id="label49" style="display:none">
 <table border="1">
 <tr>
 <td></td>
 <td colspan="1">Supported Version Ranges</td>
 </tr>
 <tr>
 <td>security</td>
 <td><code class="docutils literal notranslate">v6.0.0 -> 7.6.2 </code></td>
 </tr>
 <tr>
 <td>[any]</td>
 <td><code class="docutils literal notranslate">v6.0.0 -> 7.6.2</code></td>
 <tr>
 <td>[rdp]</td>
 <td><code class="docutils literal notranslate">v6.0.0 -> 7.6.2</code></td>
 <tr>
 <td>[nla]</td>
 <td><code class="docutils literal notranslate">v6.0.0 -> 7.6.2</code></td>
 <tr>
 <td>[tls]</td>
 <td><code class="docutils literal notranslate">v6.0.0 -> 7.6.2</code></td>
 </table>
 </div>
 </li>
            <li> <span class="li-head">send_preconnection_id</span> - Enable/disable sending of preconnection ID. <span class="li-normal">type: str</span> <span class="li-normal">choices: enable, disable</span>
 <a id='label50' href="javascript:ContentClick('label51', 'label50');" onmouseover="ContentPreview('label51');" onmouseout="ContentUnpreview('label51');" title="click to collapse or expand..."> more... </a>
 <div id="label51" style="display:none">
 <table border="1">
 <tr>
 <td></td>
 <td colspan="1">Supported Version Ranges</td>
 </tr>
 <tr>
 <td>send_preconnection_id</td>
 <td><code class="docutils literal notranslate">v7.0.1 -> 7.6.2 </code></td>
 </tr>
 <tr>
 <td>[enable]</td>
 <td><code class="docutils literal notranslate">v7.0.1 -> 7.6.2</code></td>
 <tr>
 <td>[disable]</td>
 <td><code class="docutils literal notranslate">v7.0.1 -> 7.6.2</code></td>
 </table>
 </div>
 </li>
            <li> <span class="li-head">server_layout</span> - Server side keyboard layout. <span class="li-normal">type: str</span> <span class="li-normal">choices: de-de-qwertz, en-gb-qwerty, en-us-qwerty, es-es-qwerty, fr-ca-qwerty, fr-fr-azerty, fr-ch-qwertz, it-it-qwerty, ja-jp-qwerty, pt-br-qwerty, sv-se-qwerty, tr-tr-qwerty, failsafe</span>
 <a id='label52' href="javascript:ContentClick('label53', 'label52');" onmouseover="ContentPreview('label53');" onmouseout="ContentUnpreview('label53');" title="click to collapse or expand..."> more... </a>
 <div id="label53" style="display:none">
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
 <td><code class="docutils literal notranslate">v6.0.0 -> v7.0.0</code></td>
 <tr>
 <td>[en-gb-qwerty]</td>
 <td><code class="docutils literal notranslate">v6.0.0 -> v7.0.0</code></td>
 <tr>
 <td>[en-us-qwerty]</td>
 <td><code class="docutils literal notranslate">v6.0.0 -> v7.0.0</code></td>
 <tr>
 <td>[es-es-qwerty]</td>
 <td><code class="docutils literal notranslate">v6.0.0 -> v7.0.0</code></td>
 <tr>
 <td>[fr-ca-qwerty]</td>
 <td><code class="docutils literal notranslate">v6.2.0 -> v7.0.0</code></td>
 </tr>
 <tr>
 <td>[fr-fr-azerty]</td>
 <td><code class="docutils literal notranslate">v6.0.0 -> v7.0.0</code></td>
 <tr>
 <td>[fr-ch-qwertz]</td>
 <td><code class="docutils literal notranslate">v6.0.0 -> v7.0.0</code></td>
 <tr>
 <td>[it-it-qwerty]</td>
 <td><code class="docutils literal notranslate">v6.0.0 -> v7.0.0</code></td>
 <tr>
 <td>[ja-jp-qwerty]</td>
 <td><code class="docutils literal notranslate">v6.0.0 -> v7.0.0</code></td>
 <tr>
 <td>[pt-br-qwerty]</td>
 <td><code class="docutils literal notranslate">v6.0.0 -> v7.0.0</code></td>
 <tr>
 <td>[sv-se-qwerty]</td>
 <td><code class="docutils literal notranslate">v6.0.0 -> v7.0.0</code></td>
 <tr>
 <td>[tr-tr-qwerty]</td>
 <td><code class="docutils literal notranslate">v6.0.0 -> v7.0.0</code></td>
 <tr>
 <td>[failsafe]</td>
 <td><code class="docutils literal notranslate">v6.0.0 -> v7.0.0</code></td>
 </table>
 </div>
 </li>
            <li> <span class="li-head">show_status_window</span> - Enable/disable showing of status window. <span class="li-normal">type: str</span> <span class="li-normal">choices: enable, disable</span>
 <a id='label54' href="javascript:ContentClick('label55', 'label54');" onmouseover="ContentPreview('label55');" onmouseout="ContentUnpreview('label55');" title="click to collapse or expand..."> more... </a>
 <div id="label55" style="display:none">
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
 <td><code class="docutils literal notranslate">v6.0.0 -> v7.0.0</code></td>
 <tr>
 <td>[disable]</td>
 <td><code class="docutils literal notranslate">v6.0.0 -> v7.0.0</code></td>
 </table>
 </div>
 </li>
            <li> <span class="li-head">sso</span> - Single sign-on. <span class="li-normal">type: str</span> <span class="li-normal">choices: disable, static, auto</span>
 <a id='label56' href="javascript:ContentClick('label57', 'label56');" onmouseover="ContentPreview('label57');" onmouseout="ContentUnpreview('label57');" title="click to collapse or expand..."> more... </a>
 <div id="label57" style="display:none">
 <table border="1">
 <tr>
 <td></td>
 <td colspan="1">Supported Version Ranges</td>
 </tr>
 <tr>
 <td>sso</td>
 <td><code class="docutils literal notranslate">v6.0.0 -> 7.6.2 </code></td>
 </tr>
 <tr>
 <td>[disable]</td>
 <td><code class="docutils literal notranslate">v6.0.0 -> 7.6.2</code></td>
 <tr>
 <td>[static]</td>
 <td><code class="docutils literal notranslate">v6.0.0 -> 7.6.2</code></td>
 <tr>
 <td>[auto]</td>
 <td><code class="docutils literal notranslate">v6.0.0 -> 7.6.2</code></td>
 </table>
 </div>
 </li>
            <li> <span class="li-head">sso_credential</span> - Single sign-on credentials. <span class="li-normal">type: str</span> <span class="li-normal">choices: sslvpn-login, alternative</span>
 <a id='label58' href="javascript:ContentClick('label59', 'label58');" onmouseover="ContentPreview('label59');" onmouseout="ContentUnpreview('label59');" title="click to collapse or expand..."> more... </a>
 <div id="label59" style="display:none">
 <table border="1">
 <tr>
 <td></td>
 <td colspan="1">Supported Version Ranges</td>
 </tr>
 <tr>
 <td>sso_credential</td>
 <td><code class="docutils literal notranslate">v6.0.0 -> 7.6.2 </code></td>
 </tr>
 <tr>
 <td>[sslvpn-login]</td>
 <td><code class="docutils literal notranslate">v6.0.0 -> 7.6.2</code></td>
 <tr>
 <td>[alternative]</td>
 <td><code class="docutils literal notranslate">v6.0.0 -> 7.6.2</code></td>
 </table>
 </div>
 </li>
            <li> <span class="li-head">sso_credential_sent_once</span> - Single sign-on credentials are only sent once to remote server. <span class="li-normal">type: str</span> <span class="li-normal">choices: enable, disable</span>
 <a id='label60' href="javascript:ContentClick('label61', 'label60');" onmouseover="ContentPreview('label61');" onmouseout="ContentUnpreview('label61');" title="click to collapse or expand..."> more... </a>
 <div id="label61" style="display:none">
 <table border="1">
 <tr>
 <td></td>
 <td colspan="1">Supported Version Ranges</td>
 </tr>
 <tr>
 <td>sso_credential_sent_once</td>
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
            <li> <span class="li-head">sso_password</span> - SSO password. <span class="li-normal">type: str</span>
 <a id='label62' href="javascript:ContentClick('label63', 'label62');" onmouseover="ContentPreview('label63');" onmouseout="ContentUnpreview('label63');" title="click to collapse or expand..."> more... </a>
 <div id="label63" style="display:none">
 <table border="1">
 <tr>
 <td></td>
 <td colspan="1">Supported Version Ranges</td>
 </tr>
 <tr>
 <td>sso_password</td>
 <td><code class="docutils literal notranslate">v6.0.0 -> 7.6.2 </code></td>
 </tr>
 </table>
 </div>
 </li>
            <li> <span class="li-head">sso_username</span> - SSO user name. <span class="li-normal">type: str</span>
 <a id='label64' href="javascript:ContentClick('label65', 'label64');" onmouseover="ContentPreview('label65');" onmouseout="ContentUnpreview('label65');" title="click to collapse or expand..."> more... </a>
 <div id="label65" style="display:none">
 <table border="1">
 <tr>
 <td></td>
 <td colspan="1">Supported Version Ranges</td>
 </tr>
 <tr>
 <td>sso_username</td>
 <td><code class="docutils literal notranslate">v6.0.0 -> 7.6.2 </code></td>
 </tr>
 </table>
 </div>
 </li>
            <li> <span class="li-head">url</span> - URL parameter. <span class="li-normal">type: str</span>
 <a id='label66' href="javascript:ContentClick('label67', 'label66');" onmouseover="ContentPreview('label67');" onmouseout="ContentUnpreview('label67');" title="click to collapse or expand..."> more... </a>
 <div id="label67" style="display:none">
 <table border="1">
 <tr>
 <td></td>
 <td colspan="1">Supported Version Ranges</td>
 </tr>
 <tr>
 <td>url</td>
 <td><code class="docutils literal notranslate">v6.0.0 -> 7.6.2 </code></td>
 </tr>
 </table>
 </div>
 </li>
            <li> <span class="li-head">vnc_keyboard_layout</span> - Keyboard layout. <span class="li-normal">type: str</span> <span class="li-normal">choices: default, da, nl, en-uk, en-uk-ext, fi, fr, fr-be, fr-ca-mul, de, de-ch, it, it-142, pt, pt-br-abnt2, no, gd, es, sv, us-intl</span>
 <a id='label68' href="javascript:ContentClick('label69', 'label68');" onmouseover="ContentPreview('label69');" onmouseout="ContentUnpreview('label69');" title="click to collapse or expand..."> more... </a>
 <div id="label69" style="display:none">
 <table border="1">
 <tr>
 <td></td>
 <td colspan="1">Supported Version Ranges</td>
 </tr>
 <tr>
 <td>vnc_keyboard_layout</td>
 <td><code class="docutils literal notranslate">v7.2.4 -> 7.6.2 </code></td>
 </tr>
 <tr>
 <td>[default]</td>
 <td><code class="docutils literal notranslate">v7.2.4 -> 7.6.2</code></td>
 <tr>
 <td>[da]</td>
 <td><code class="docutils literal notranslate">v7.2.4 -> 7.6.2</code></td>
 <tr>
 <td>[nl]</td>
 <td><code class="docutils literal notranslate">v7.2.4 -> 7.6.2</code></td>
 <tr>
 <td>[en-uk]</td>
 <td><code class="docutils literal notranslate">v7.2.4 -> 7.6.2</code></td>
 <tr>
 <td>[en-uk-ext]</td>
 <td><code class="docutils literal notranslate">v7.2.4 -> 7.6.2</code></td>
 <tr>
 <td>[fi]</td>
 <td><code class="docutils literal notranslate">v7.2.4 -> 7.6.2</code></td>
 <tr>
 <td>[fr]</td>
 <td><code class="docutils literal notranslate">v7.2.4 -> 7.6.2</code></td>
 <tr>
 <td>[fr-be]</td>
 <td><code class="docutils literal notranslate">v7.2.4 -> 7.6.2</code></td>
 <tr>
 <td>[fr-ca-mul]</td>
 <td><code class="docutils literal notranslate">v7.2.4 -> 7.6.2</code></td>
 <tr>
 <td>[de]</td>
 <td><code class="docutils literal notranslate">v7.2.4 -> 7.6.2</code></td>
 <tr>
 <td>[de-ch]</td>
 <td><code class="docutils literal notranslate">v7.2.4 -> 7.6.2</code></td>
 <tr>
 <td>[it]</td>
 <td><code class="docutils literal notranslate">v7.2.4 -> 7.6.2</code></td>
 <tr>
 <td>[it-142]</td>
 <td><code class="docutils literal notranslate">v7.2.4 -> 7.6.2</code></td>
 <tr>
 <td>[pt]</td>
 <td><code class="docutils literal notranslate">v7.2.4 -> 7.6.2</code></td>
 <tr>
 <td>[pt-br-abnt2]</td>
 <td><code class="docutils literal notranslate">v7.2.4 -> 7.6.2</code></td>
 <tr>
 <td>[no]</td>
 <td><code class="docutils literal notranslate">v7.2.4 -> 7.6.2</code></td>
 <tr>
 <td>[gd]</td>
 <td><code class="docutils literal notranslate">v7.2.4 -> 7.6.2</code></td>
 <tr>
 <td>[es]</td>
 <td><code class="docutils literal notranslate">v7.2.4 -> 7.6.2</code></td>
 <tr>
 <td>[sv]</td>
 <td><code class="docutils literal notranslate">v7.2.4 -> 7.6.2</code></td>
 <tr>
 <td>[us-intl]</td>
 <td><code class="docutils literal notranslate">v7.2.4 -> 7.6.2</code></td>
 </table>
 </div>
 </li>
            <li> <span class="li-head">width</span> - Screen width (range from 0 - 65535). <span class="li-normal">type: int</span>
 <a id='label70' href="javascript:ContentClick('label71', 'label70');" onmouseover="ContentPreview('label71');" onmouseout="ContentUnpreview('label71');" title="click to collapse or expand..."> more... </a>
 <div id="label71" style="display:none">
 <table border="1">
 <tr>
 <td></td>
 <td colspan="1">Supported Version Ranges</td>
 </tr>
 <tr>
 <td>width</td>
 <td><code class="docutils literal notranslate">v7.0.4 -> 7.6.2 </code></td>
 </tr>
 </table>
 </div>
 </li>
            </ul>
        <li> <span class="li-head">name</span> - Group name. Source user.group.name. <span class="li-normal">type: str</span> <span class="li-required">required: true</span>
 <a id='label72' href="javascript:ContentClick('label73', 'label72');" onmouseover="ContentPreview('label73');" onmouseout="ContentUnpreview('label73');" title="click to collapse or expand..."> more... </a>
 <div id="label73" style="display:none">
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
    </ul>


Notes
-----

.. note::

   - Legacy fortiosapi has been deprecated, httpapi is the preferred way to run playbooks

   - The module supports check_mode.



Examples
--------

.. code-block:: yaml+jinja
    
    - name: Configure SSL-VPN user group bookmark.
      fortinet.fortios.fortios_vpn_ssl_web_user_group_bookmark:
          vdom: "{{ vdom }}"
          state: "present"
          access_token: "<your_own_value>"
          vpn_ssl_web_user_group_bookmark:
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
                              name: "default_name_11"
                              value: "<your_own_value>"
                      height: "768"
                      host: "myhostname"
                      keyboard_layout: "ar-101"
                      listening_port: "0"
                      load_balancing_info: "<your_own_value>"
                      logon_password: "<your_own_value>"
                      logon_user: "<your_own_value>"
                      name: "default_name_20"
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
              name: "default_name_38 (source user.group.name)"


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
