:source: fortios_vpn_certificate_setting.py

:orphan:

.. fortios_vpn_certificate_setting:

fortios_vpn_certificate_setting -- VPN certificate setting in Fortinet's FortiOS and FortiGate.
+++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++

.. versionadded:: 2.0.0

.. contents::
   :local:
   :depth: 1


Synopsis
--------
- This module is able to configure a FortiGate or FortiOS (FOS) device by allowing the user to set and modify vpn_certificate feature and setting category. Examples include all parameters and values need to be adjusted to datasources before usage. Tested with FOS v6.0.0



Requirements
------------
The below requirements are needed on the host that executes this module.

- ansible>=2.15


Tips
----
Using member operation to add an element to an existing object.

FortiOS Version Compatibility
-----------------------------
Supported Version Ranges: v6.0.0 -> 7.4.3



Parameters
----------


.. raw:: html

    <ul>
    <li> <span class="li-head">access_token</span> - Token-based authentication. Generated from GUI of Fortigate. <span class="li-normal">type: str</span> <span class="li-required">required: false</span> </li>
    <li> <span class="li-head">enable_log</span> - Enable/Disable logging for task. <span class="li-normal">type: bool</span> <span class="li-required">required: false</span> <span class="li-normal">default: False</span> </li>
    <li> <span class="li-head">vdom</span> - Virtual domain, among those defined previously. A vdom is a virtual instance of the FortiGate that can be configured and used as a different unit. <span class="li-normal">type: str</span> <span class="li-normal">default: root</span> </li>
    <li> <span class="li-head">member_path</span> - Member attribute path to operate on. <span class="li-normal">type: str</span> </li>
    <li> <span class="li-head">member_state</span> - Add or delete a member under specified attribute path. <span class="li-normal">type: str</span> <span class="li-normal">choices: present, absent</span> </li>
    <li> <span class="li-head">vpn_certificate_setting</span> - VPN certificate setting. <span class="li-normal">type: dict</span>
 <a id='label0' href="javascript:ContentClick('label1', 'label0');" onmouseover="ContentPreview('label1');" onmouseout="ContentUnpreview('label1');" title="click to collapse or expand..."> more... </a>
 <div id="label1" style="display:none">
 <table border="1">
 <tr>
 <td></td><td colspan="1">Supported Version Ranges</td>
 </tr>
 <tr>
 <td>vpn_certificate_setting</td>
 <td><code class="docutils literal notranslate">v6.0.0 -> 7.4.3 </code></td>
 </tr>
 </table>
 </div>
 </li>
        <ul class="ul-self">
        <li> <span class="li-head">cert_expire_warning</span> - Number of days before a certificate expires to send a warning. Set to 0 to disable sending of the warning (0 - 100). <span class="li-normal">type: int</span>
 <a id='label2' href="javascript:ContentClick('label3', 'label2');" onmouseover="ContentPreview('label3');" onmouseout="ContentUnpreview('label3');" title="click to collapse or expand..."> more... </a>
 <div id="label3" style="display:none">
 <table border="1">
 <tr>
 <td></td>
 <td colspan="1">Supported Version Ranges</td>
 </tr>
 <tr>
 <td>cert_expire_warning</td>
 <td><code class="docutils literal notranslate">v7.2.1 -> 7.4.3 </code></td>
 </tr>
 </table>
 </div>
 </li>
        <li> <span class="li-head">certname_dsa1024</span> - 1024 bit DSA key certificate for re-signing server certificates for SSL inspection. Source vpn.certificate.local.name. <span class="li-normal">type: str</span>
 <a id='label4' href="javascript:ContentClick('label5', 'label4');" onmouseover="ContentPreview('label5');" onmouseout="ContentUnpreview('label5');" title="click to collapse or expand..."> more... </a>
 <div id="label5" style="display:none">
 <table border="1">
 <tr>
 <td></td>
 <td colspan="1">Supported Version Ranges</td>
 </tr>
 <tr>
 <td>certname_dsa1024</td>
 <td><code class="docutils literal notranslate">v6.0.0 -> 7.4.3 </code></td>
 </tr>
 </table>
 </div>
 </li>
        <li> <span class="li-head">certname_dsa2048</span> - 2048 bit DSA key certificate for re-signing server certificates for SSL inspection. Source vpn.certificate.local.name. <span class="li-normal">type: str</span>
 <a id='label6' href="javascript:ContentClick('label7', 'label6');" onmouseover="ContentPreview('label7');" onmouseout="ContentUnpreview('label7');" title="click to collapse or expand..."> more... </a>
 <div id="label7" style="display:none">
 <table border="1">
 <tr>
 <td></td>
 <td colspan="1">Supported Version Ranges</td>
 </tr>
 <tr>
 <td>certname_dsa2048</td>
 <td><code class="docutils literal notranslate">v6.0.0 -> 7.4.3 </code></td>
 </tr>
 </table>
 </div>
 </li>
        <li> <span class="li-head">certname_ecdsa256</span> - 256 bit ECDSA key certificate for re-signing server certificates for SSL inspection. Source vpn.certificate.local.name. <span class="li-normal">type: str</span>
 <a id='label8' href="javascript:ContentClick('label9', 'label8');" onmouseover="ContentPreview('label9');" onmouseout="ContentUnpreview('label9');" title="click to collapse or expand..."> more... </a>
 <div id="label9" style="display:none">
 <table border="1">
 <tr>
 <td></td>
 <td colspan="1">Supported Version Ranges</td>
 </tr>
 <tr>
 <td>certname_ecdsa256</td>
 <td><code class="docutils literal notranslate">v6.0.0 -> 7.4.3 </code></td>
 </tr>
 </table>
 </div>
 </li>
        <li> <span class="li-head">certname_ecdsa384</span> - 384 bit ECDSA key certificate for re-signing server certificates for SSL inspection. Source vpn.certificate.local.name. <span class="li-normal">type: str</span>
 <a id='label10' href="javascript:ContentClick('label11', 'label10');" onmouseover="ContentPreview('label11');" onmouseout="ContentUnpreview('label11');" title="click to collapse or expand..."> more... </a>
 <div id="label11" style="display:none">
 <table border="1">
 <tr>
 <td></td>
 <td colspan="1">Supported Version Ranges</td>
 </tr>
 <tr>
 <td>certname_ecdsa384</td>
 <td><code class="docutils literal notranslate">v6.0.0 -> 7.4.3 </code></td>
 </tr>
 </table>
 </div>
 </li>
        <li> <span class="li-head">certname_ecdsa521</span> - 521 bit ECDSA key certificate for re-signing server certificates for SSL inspection. Source vpn.certificate.local.name. <span class="li-normal">type: str</span>
 <a id='label12' href="javascript:ContentClick('label13', 'label12');" onmouseover="ContentPreview('label13');" onmouseout="ContentUnpreview('label13');" title="click to collapse or expand..."> more... </a>
 <div id="label13" style="display:none">
 <table border="1">
 <tr>
 <td></td>
 <td colspan="1">Supported Version Ranges</td>
 </tr>
 <tr>
 <td>certname_ecdsa521</td>
 <td><code class="docutils literal notranslate">v6.2.0 -> 7.4.3 </code></td>
 </tr>
 </table>
 </div>
 </li>
        <li> <span class="li-head">certname_ed25519</span> - 253 bit EdDSA key certificate for re-signing server certificates for SSL inspection. Source vpn.certificate.local.name. <span class="li-normal">type: str</span>
 <a id='label14' href="javascript:ContentClick('label15', 'label14');" onmouseover="ContentPreview('label15');" onmouseout="ContentUnpreview('label15');" title="click to collapse or expand..."> more... </a>
 <div id="label15" style="display:none">
 <table border="1">
 <tr>
 <td></td>
 <td colspan="1">Supported Version Ranges</td>
 </tr>
 <tr>
 <td>certname_ed25519</td>
 <td><code class="docutils literal notranslate">v6.2.0 -> 7.4.3 </code></td>
 </tr>
 </table>
 </div>
 </li>
        <li> <span class="li-head">certname_ed448</span> - 456 bit EdDSA key certificate for re-signing server certificates for SSL inspection. Source vpn.certificate.local.name. <span class="li-normal">type: str</span>
 <a id='label16' href="javascript:ContentClick('label17', 'label16');" onmouseover="ContentPreview('label17');" onmouseout="ContentUnpreview('label17');" title="click to collapse or expand..."> more... </a>
 <div id="label17" style="display:none">
 <table border="1">
 <tr>
 <td></td>
 <td colspan="1">Supported Version Ranges</td>
 </tr>
 <tr>
 <td>certname_ed448</td>
 <td><code class="docutils literal notranslate">v6.2.0 -> 7.4.3 </code></td>
 </tr>
 </table>
 </div>
 </li>
        <li> <span class="li-head">certname_rsa1024</span> - 1024 bit RSA key certificate for re-signing server certificates for SSL inspection. Source vpn.certificate.local.name. <span class="li-normal">type: str</span>
 <a id='label18' href="javascript:ContentClick('label19', 'label18');" onmouseover="ContentPreview('label19');" onmouseout="ContentUnpreview('label19');" title="click to collapse or expand..."> more... </a>
 <div id="label19" style="display:none">
 <table border="1">
 <tr>
 <td></td>
 <td colspan="1">Supported Version Ranges</td>
 </tr>
 <tr>
 <td>certname_rsa1024</td>
 <td><code class="docutils literal notranslate">v6.0.0 -> 7.4.3 </code></td>
 </tr>
 </table>
 </div>
 </li>
        <li> <span class="li-head">certname_rsa2048</span> - 2048 bit RSA key certificate for re-signing server certificates for SSL inspection. Source vpn.certificate.local.name. <span class="li-normal">type: str</span>
 <a id='label20' href="javascript:ContentClick('label21', 'label20');" onmouseover="ContentPreview('label21');" onmouseout="ContentUnpreview('label21');" title="click to collapse or expand..."> more... </a>
 <div id="label21" style="display:none">
 <table border="1">
 <tr>
 <td></td>
 <td colspan="1">Supported Version Ranges</td>
 </tr>
 <tr>
 <td>certname_rsa2048</td>
 <td><code class="docutils literal notranslate">v6.0.0 -> 7.4.3 </code></td>
 </tr>
 </table>
 </div>
 </li>
        <li> <span class="li-head">certname_rsa4096</span> - 4096 bit RSA key certificate for re-signing server certificates for SSL inspection. Source vpn.certificate.local.name. <span class="li-normal">type: str</span>
 <a id='label22' href="javascript:ContentClick('label23', 'label22');" onmouseover="ContentPreview('label23');" onmouseout="ContentUnpreview('label23');" title="click to collapse or expand..."> more... </a>
 <div id="label23" style="display:none">
 <table border="1">
 <tr>
 <td></td>
 <td colspan="1">Supported Version Ranges</td>
 </tr>
 <tr>
 <td>certname_rsa4096</td>
 <td><code class="docutils literal notranslate">v6.2.0 -> 7.4.3 </code></td>
 </tr>
 </table>
 </div>
 </li>
        <li> <span class="li-head">check_ca_cert</span> - Enable/disable verification of the user certificate and pass authentication if any CA in the chain is trusted . <span class="li-normal">type: str</span> <span class="li-normal">choices: enable, disable</span>
 <a id='label24' href="javascript:ContentClick('label25', 'label24');" onmouseover="ContentPreview('label25');" onmouseout="ContentUnpreview('label25');" title="click to collapse or expand..."> more... </a>
 <div id="label25" style="display:none">
 <table border="1">
 <tr>
 <td></td>
 <td colspan="1">Supported Version Ranges</td>
 </tr>
 <tr>
 <td>check_ca_cert</td>
 <td><code class="docutils literal notranslate">v6.0.0 -> 7.4.3 </code></td>
 </tr>
 <tr>
 <td>[enable]</td>
 <td><code class="docutils literal notranslate">v6.0.0 -> 7.4.3</code></td>
 <tr>
 <td>[disable]</td>
 <td><code class="docutils literal notranslate">v6.0.0 -> 7.4.3</code></td>
 </table>
 </div>
 </li>
        <li> <span class="li-head">check_ca_chain</span> - Enable/disable verification of the entire certificate chain and pass authentication only if the chain is complete and all of the CAs in the chain are trusted . <span class="li-normal">type: str</span> <span class="li-normal">choices: enable, disable</span>
 <a id='label26' href="javascript:ContentClick('label27', 'label26');" onmouseover="ContentPreview('label27');" onmouseout="ContentUnpreview('label27');" title="click to collapse or expand..."> more... </a>
 <div id="label27" style="display:none">
 <table border="1">
 <tr>
 <td></td>
 <td colspan="1">Supported Version Ranges</td>
 </tr>
 <tr>
 <td>check_ca_chain</td>
 <td><code class="docutils literal notranslate">v6.0.0 -> 7.4.3 </code></td>
 </tr>
 <tr>
 <td>[enable]</td>
 <td><code class="docutils literal notranslate">v6.0.0 -> 7.4.3</code></td>
 <tr>
 <td>[disable]</td>
 <td><code class="docutils literal notranslate">v6.0.0 -> 7.4.3</code></td>
 </table>
 </div>
 </li>
        <li> <span class="li-head">cmp_key_usage_checking</span> - Enable/disable server certificate key usage checking in CMP mode . <span class="li-normal">type: str</span> <span class="li-normal">choices: enable, disable</span>
 <a id='label28' href="javascript:ContentClick('label29', 'label28');" onmouseover="ContentPreview('label29');" onmouseout="ContentUnpreview('label29');" title="click to collapse or expand..."> more... </a>
 <div id="label29" style="display:none">
 <table border="1">
 <tr>
 <td></td>
 <td colspan="3">Supported Version Ranges</td>
 </tr>
 <tr>
 <td>cmp_key_usage_checking</td>
 <td><code class="docutils literal notranslate">v6.0.0 -> v6.0.0 </code></td>
 <td><code class="docutils literal notranslate">v6.0.11 -> v6.2.0 </code></td>
 <td><code class="docutils literal notranslate">v6.2.5 -> 7.4.3 </code></td>
 </tr>
 <tr>
 <td>[enable]</td>
 <td><code class="docutils literal notranslate">v6.0.0 -> v6.0.0</code></td>
 <tr>
 <td>[disable]</td>
 <td><code class="docutils literal notranslate">v6.0.0 -> v6.0.0</code></td>
 </table>
 </div>
 </li>
        <li> <span class="li-head">cmp_save_extra_certs</span> - Enable/disable saving extra certificates in CMP mode . <span class="li-normal">type: str</span> <span class="li-normal">choices: enable, disable</span>
 <a id='label30' href="javascript:ContentClick('label31', 'label30');" onmouseover="ContentPreview('label31');" onmouseout="ContentUnpreview('label31');" title="click to collapse or expand..."> more... </a>
 <div id="label31" style="display:none">
 <table border="1">
 <tr>
 <td></td>
 <td colspan="1">Supported Version Ranges</td>
 </tr>
 <tr>
 <td>cmp_save_extra_certs</td>
 <td><code class="docutils literal notranslate">v6.0.0 -> 7.4.3 </code></td>
 </tr>
 <tr>
 <td>[enable]</td>
 <td><code class="docutils literal notranslate">v6.0.0 -> 7.4.3</code></td>
 <tr>
 <td>[disable]</td>
 <td><code class="docutils literal notranslate">v6.0.0 -> 7.4.3</code></td>
 </table>
 </div>
 </li>
        <li> <span class="li-head">cn_allow_multi</span> - When searching for a matching certificate, allow multiple CN fields in certificate subject name . <span class="li-normal">type: str</span> <span class="li-normal">choices: disable, enable</span>
 <a id='label32' href="javascript:ContentClick('label33', 'label32');" onmouseover="ContentPreview('label33');" onmouseout="ContentUnpreview('label33');" title="click to collapse or expand..."> more... </a>
 <div id="label33" style="display:none">
 <table border="1">
 <tr>
 <td></td>
 <td colspan="1">Supported Version Ranges</td>
 </tr>
 <tr>
 <td>cn_allow_multi</td>
 <td><code class="docutils literal notranslate">v7.0.1 -> 7.4.3 </code></td>
 </tr>
 <tr>
 <td>[disable]</td>
 <td><code class="docutils literal notranslate">v7.0.1 -> 7.4.3</code></td>
 <tr>
 <td>[enable]</td>
 <td><code class="docutils literal notranslate">v7.0.1 -> 7.4.3</code></td>
 </table>
 </div>
 </li>
        <li> <span class="li-head">cn_match</span> - When searching for a matching certificate, control how to do CN value matching with certificate subject name . <span class="li-normal">type: str</span> <span class="li-normal">choices: substring, value</span>
 <a id='label34' href="javascript:ContentClick('label35', 'label34');" onmouseover="ContentPreview('label35');" onmouseout="ContentUnpreview('label35');" title="click to collapse or expand..."> more... </a>
 <div id="label35" style="display:none">
 <table border="1">
 <tr>
 <td></td>
 <td colspan="1">Supported Version Ranges</td>
 </tr>
 <tr>
 <td>cn_match</td>
 <td><code class="docutils literal notranslate">v6.0.0 -> 7.4.3 </code></td>
 </tr>
 <tr>
 <td>[substring]</td>
 <td><code class="docutils literal notranslate">v6.0.0 -> 7.4.3</code></td>
 <tr>
 <td>[value]</td>
 <td><code class="docutils literal notranslate">v6.0.0 -> 7.4.3</code></td>
 </table>
 </div>
 </li>
        <li> <span class="li-head">crl_verification</span> - CRL verification options. <span class="li-normal">type: dict</span>
 <a id='label36' href="javascript:ContentClick('label37', 'label36');" onmouseover="ContentPreview('label37');" onmouseout="ContentUnpreview('label37');" title="click to collapse or expand..."> more... </a>
 <div id="label37" style="display:none">
 <table border="1">
 <tr>
 <td></td><td colspan="1">Supported Version Ranges</td>
 </tr>
 <tr>
 <td>crl_verification</td>
 <td><code class="docutils literal notranslate">v7.0.1 -> 7.4.3 </code></td>
 </tr>
 </table>
 </div>
 </li>
            <ul class="ul-self">
            <li> <span class="li-head">chain_crl_absence</span> - CRL verification option when CRL of any certificate in chain is absent . <span class="li-normal">type: str</span> <span class="li-normal">choices: ignore, revoke</span>
 <a id='label38' href="javascript:ContentClick('label39', 'label38');" onmouseover="ContentPreview('label39');" onmouseout="ContentUnpreview('label39');" title="click to collapse or expand..."> more... </a>
 <div id="label39" style="display:none">
 <table border="1">
 <tr>
 <td></td>
 <td colspan="1">Supported Version Ranges</td>
 </tr>
 <tr>
 <td>chain_crl_absence</td>
 <td><code class="docutils literal notranslate">v7.0.1 -> 7.4.3 </code></td>
 </tr>
 <tr>
 <td>[ignore]</td>
 <td><code class="docutils literal notranslate">v7.0.1 -> 7.4.3</code></td>
 <tr>
 <td>[revoke]</td>
 <td><code class="docutils literal notranslate">v7.0.1 -> 7.4.3</code></td>
 </table>
 </div>
 </li>
            <li> <span class="li-head">expiry</span> - CRL verification option when CRL is expired . <span class="li-normal">type: str</span> <span class="li-normal">choices: ignore, revoke</span>
 <a id='label40' href="javascript:ContentClick('label41', 'label40');" onmouseover="ContentPreview('label41');" onmouseout="ContentUnpreview('label41');" title="click to collapse or expand..."> more... </a>
 <div id="label41" style="display:none">
 <table border="1">
 <tr>
 <td></td>
 <td colspan="1">Supported Version Ranges</td>
 </tr>
 <tr>
 <td>expiry</td>
 <td><code class="docutils literal notranslate">v7.0.1 -> 7.4.3 </code></td>
 </tr>
 <tr>
 <td>[ignore]</td>
 <td><code class="docutils literal notranslate">v7.0.1 -> 7.4.3</code></td>
 <tr>
 <td>[revoke]</td>
 <td><code class="docutils literal notranslate">v7.0.1 -> 7.4.3</code></td>
 </table>
 </div>
 </li>
            <li> <span class="li-head">leaf_crl_absence</span> - CRL verification option when leaf CRL is absent . <span class="li-normal">type: str</span> <span class="li-normal">choices: ignore, revoke</span>
 <a id='label42' href="javascript:ContentClick('label43', 'label42');" onmouseover="ContentPreview('label43');" onmouseout="ContentUnpreview('label43');" title="click to collapse or expand..."> more... </a>
 <div id="label43" style="display:none">
 <table border="1">
 <tr>
 <td></td>
 <td colspan="1">Supported Version Ranges</td>
 </tr>
 <tr>
 <td>leaf_crl_absence</td>
 <td><code class="docutils literal notranslate">v7.0.1 -> 7.4.3 </code></td>
 </tr>
 <tr>
 <td>[ignore]</td>
 <td><code class="docutils literal notranslate">v7.0.1 -> 7.4.3</code></td>
 <tr>
 <td>[revoke]</td>
 <td><code class="docutils literal notranslate">v7.0.1 -> 7.4.3</code></td>
 </table>
 </div>
 </li>
            </ul>
        <li> <span class="li-head">interface</span> - Specify outgoing interface to reach server. Source system.interface.name. <span class="li-normal">type: str</span>
 <a id='label44' href="javascript:ContentClick('label45', 'label44');" onmouseover="ContentPreview('label45');" onmouseout="ContentUnpreview('label45');" title="click to collapse or expand..."> more... </a>
 <div id="label45" style="display:none">
 <table border="1">
 <tr>
 <td></td>
 <td colspan="3">Supported Version Ranges</td>
 </tr>
 <tr>
 <td>interface</td>
 <td><code class="docutils literal notranslate">v6.2.0 -> v6.2.0 </code></td>
 <td><code class="docutils literal notranslate">v6.2.5 -> v6.4.0 </code></td>
 <td><code class="docutils literal notranslate">v6.4.4 -> 7.4.3 </code></td>
 </tr>
 </table>
 </div>
 </li>
        <li> <span class="li-head">interface_select_method</span> - Specify how to select outgoing interface to reach server. <span class="li-normal">type: str</span> <span class="li-normal">choices: auto, sdwan, specify</span>
 <a id='label46' href="javascript:ContentClick('label47', 'label46');" onmouseover="ContentPreview('label47');" onmouseout="ContentUnpreview('label47');" title="click to collapse or expand..."> more... </a>
 <div id="label47" style="display:none">
 <table border="1">
 <tr>
 <td></td>
 <td colspan="3">Supported Version Ranges</td>
 </tr>
 <tr>
 <td>interface_select_method</td>
 <td><code class="docutils literal notranslate">v6.2.0 -> v6.2.0 </code></td>
 <td><code class="docutils literal notranslate">v6.2.5 -> v6.4.0 </code></td>
 <td><code class="docutils literal notranslate">v6.4.4 -> 7.4.3 </code></td>
 </tr>
 <tr>
 <td>[auto]</td>
 <td><code class="docutils literal notranslate">v6.2.0 -> v6.2.0</code></td>
 <tr>
 <td>[sdwan]</td>
 <td><code class="docutils literal notranslate">v6.2.0 -> v6.2.0</code></td>
 <tr>
 <td>[specify]</td>
 <td><code class="docutils literal notranslate">v6.2.0 -> v6.2.0</code></td>
 </table>
 </div>
 </li>
        <li> <span class="li-head">ocsp_default_server</span> - Default OCSP server. Source vpn.certificate.ocsp-server.name. <span class="li-normal">type: str</span>
 <a id='label48' href="javascript:ContentClick('label49', 'label48');" onmouseover="ContentPreview('label49');" onmouseout="ContentUnpreview('label49');" title="click to collapse or expand..."> more... </a>
 <div id="label49" style="display:none">
 <table border="1">
 <tr>
 <td></td>
 <td colspan="1">Supported Version Ranges</td>
 </tr>
 <tr>
 <td>ocsp_default_server</td>
 <td><code class="docutils literal notranslate">v6.0.0 -> 7.4.3 </code></td>
 </tr>
 </table>
 </div>
 </li>
        <li> <span class="li-head">ocsp_option</span> - Specify whether the OCSP URL is from certificate or configured OCSP server. <span class="li-normal">type: str</span> <span class="li-normal">choices: certificate, server</span>
 <a id='label50' href="javascript:ContentClick('label51', 'label50');" onmouseover="ContentPreview('label51');" onmouseout="ContentUnpreview('label51');" title="click to collapse or expand..."> more... </a>
 <div id="label51" style="display:none">
 <table border="1">
 <tr>
 <td></td>
 <td colspan="1">Supported Version Ranges</td>
 </tr>
 <tr>
 <td>ocsp_option</td>
 <td><code class="docutils literal notranslate">v6.2.0 -> 7.4.3 </code></td>
 </tr>
 <tr>
 <td>[certificate]</td>
 <td><code class="docutils literal notranslate">v6.2.0 -> 7.4.3</code></td>
 <tr>
 <td>[server]</td>
 <td><code class="docutils literal notranslate">v6.2.0 -> 7.4.3</code></td>
 </table>
 </div>
 </li>
        <li> <span class="li-head">ocsp_status</span> - Enable/disable receiving certificates using the OCSP. <span class="li-normal">type: str</span> <span class="li-normal">choices: enable, mandatory, disable</span>
 <a id='label52' href="javascript:ContentClick('label53', 'label52');" onmouseover="ContentPreview('label53');" onmouseout="ContentUnpreview('label53');" title="click to collapse or expand..."> more... </a>
 <div id="label53" style="display:none">
 <table border="1">
 <tr>
 <td></td>
 <td colspan="1">Supported Version Ranges</td>
 </tr>
 <tr>
 <td>ocsp_status</td>
 <td><code class="docutils literal notranslate">v6.0.0 -> 7.4.3 </code></td>
 </tr>
 <tr>
 <td>[enable]</td>
 <td><code class="docutils literal notranslate">v6.0.0 -> 7.4.3</code></td>
 <tr>
 <td>[mandatory]</td>
 <td><code class="docutils literal notranslate">v7.4.2 -> 7.4.3</code></td>
 </tr>
 <tr>
 <td>[disable]</td>
 <td><code class="docutils literal notranslate">v6.0.0 -> 7.4.3</code></td>
 </table>
 </div>
 </li>
        <li> <span class="li-head">proxy</span> - Proxy server FQDN or IP for OCSP/CA queries during certificate verification. <span class="li-normal">type: str</span>
 <a id='label54' href="javascript:ContentClick('label55', 'label54');" onmouseover="ContentPreview('label55');" onmouseout="ContentUnpreview('label55');" title="click to collapse or expand..."> more... </a>
 <div id="label55" style="display:none">
 <table border="1">
 <tr>
 <td></td>
 <td colspan="1">Supported Version Ranges</td>
 </tr>
 <tr>
 <td>proxy</td>
 <td><code class="docutils literal notranslate">v7.2.4 -> 7.4.3 </code></td>
 </tr>
 </table>
 </div>
 </li>
        <li> <span class="li-head">proxy_password</span> - Proxy server password. <span class="li-normal">type: str</span>
 <a id='label56' href="javascript:ContentClick('label57', 'label56');" onmouseover="ContentPreview('label57');" onmouseout="ContentUnpreview('label57');" title="click to collapse or expand..."> more... </a>
 <div id="label57" style="display:none">
 <table border="1">
 <tr>
 <td></td>
 <td colspan="1">Supported Version Ranges</td>
 </tr>
 <tr>
 <td>proxy_password</td>
 <td><code class="docutils literal notranslate">v7.2.4 -> 7.4.3 </code></td>
 </tr>
 </table>
 </div>
 </li>
        <li> <span class="li-head">proxy_port</span> - Proxy server port (1 - 65535). <span class="li-normal">type: int</span>
 <a id='label58' href="javascript:ContentClick('label59', 'label58');" onmouseover="ContentPreview('label59');" onmouseout="ContentUnpreview('label59');" title="click to collapse or expand..."> more... </a>
 <div id="label59" style="display:none">
 <table border="1">
 <tr>
 <td></td>
 <td colspan="1">Supported Version Ranges</td>
 </tr>
 <tr>
 <td>proxy_port</td>
 <td><code class="docutils literal notranslate">v7.2.4 -> 7.4.3 </code></td>
 </tr>
 </table>
 </div>
 </li>
        <li> <span class="li-head">proxy_username</span> - Proxy server user name. <span class="li-normal">type: str</span>
 <a id='label60' href="javascript:ContentClick('label61', 'label60');" onmouseover="ContentPreview('label61');" onmouseout="ContentUnpreview('label61');" title="click to collapse or expand..."> more... </a>
 <div id="label61" style="display:none">
 <table border="1">
 <tr>
 <td></td>
 <td colspan="1">Supported Version Ranges</td>
 </tr>
 <tr>
 <td>proxy_username</td>
 <td><code class="docutils literal notranslate">v7.2.4 -> 7.4.3 </code></td>
 </tr>
 </table>
 </div>
 </li>
        <li> <span class="li-head">source_ip</span> - Source IP address for dynamic AIA and OCSP queries. <span class="li-normal">type: str</span>
 <a id='label62' href="javascript:ContentClick('label63', 'label62');" onmouseover="ContentPreview('label63');" onmouseout="ContentUnpreview('label63');" title="click to collapse or expand..."> more... </a>
 <div id="label63" style="display:none">
 <table border="1">
 <tr>
 <td></td>
 <td colspan="1">Supported Version Ranges</td>
 </tr>
 <tr>
 <td>source_ip</td>
 <td><code class="docutils literal notranslate">v7.4.0 -> 7.4.3 </code></td>
 </tr>
 </table>
 </div>
 </li>
        <li> <span class="li-head">ssl_min_proto_version</span> - Minimum supported protocol version for SSL/TLS connections . <span class="li-normal">type: str</span> <span class="li-normal">choices: default, SSLv3, TLSv1, TLSv1-1, TLSv1-2, TLSv1-3</span>
 <a id='label64' href="javascript:ContentClick('label65', 'label64');" onmouseover="ContentPreview('label65');" onmouseout="ContentUnpreview('label65');" title="click to collapse or expand..."> more... </a>
 <div id="label65" style="display:none">
 <table border="1">
 <tr>
 <td></td>
 <td colspan="1">Supported Version Ranges</td>
 </tr>
 <tr>
 <td>ssl_min_proto_version</td>
 <td><code class="docutils literal notranslate">v6.0.0 -> 7.4.3 </code></td>
 </tr>
 <tr>
 <td>[default]</td>
 <td><code class="docutils literal notranslate">v6.0.0 -> 7.4.3</code></td>
 <tr>
 <td>[SSLv3]</td>
 <td><code class="docutils literal notranslate">v6.0.0 -> 7.4.3</code></td>
 <tr>
 <td>[TLSv1]</td>
 <td><code class="docutils literal notranslate">v6.0.0 -> 7.4.3</code></td>
 <tr>
 <td>[TLSv1-1]</td>
 <td><code class="docutils literal notranslate">v6.0.0 -> 7.4.3</code></td>
 <tr>
 <td>[TLSv1-2]</td>
 <td><code class="docutils literal notranslate">v6.0.0 -> 7.4.3</code></td>
 <tr>
 <td>[TLSv1-3]</td>
 <td><code class="docutils literal notranslate">v7.4.1 -> 7.4.3</code></td>
 </tr>
 </table>
 </div>
 </li>
        <li> <span class="li-head">ssl_ocsp_option</span> - Specify whether the OCSP URL is from the certificate or the default OCSP server. <span class="li-normal">type: str</span> <span class="li-normal">choices: certificate, server</span>
 <a id='label66' href="javascript:ContentClick('label67', 'label66');" onmouseover="ContentPreview('label67');" onmouseout="ContentUnpreview('label67');" title="click to collapse or expand..."> more... </a>
 <div id="label67" style="display:none">
 <table border="1">
 <tr>
 <td></td>
 <td colspan="1">Supported Version Ranges</td>
 </tr>
 <tr>
 <td>ssl_ocsp_option</td>
 <td><code class="docutils literal notranslate">v6.0.0 -> v6.0.11 </code></td>
 </tr>
 <tr>
 <td>[certificate]</td>
 <td><code class="docutils literal notranslate">v6.0.0 -> v6.0.11</code></td>
 <tr>
 <td>[server]</td>
 <td><code class="docutils literal notranslate">v6.0.0 -> v6.0.11</code></td>
 </table>
 </div>
 </li>
        <li> <span class="li-head">ssl_ocsp_source_ip</span> - Source IP address to use to communicate with the OCSP server. <span class="li-normal">type: str</span>
 <a id='label68' href="javascript:ContentClick('label69', 'label68');" onmouseover="ContentPreview('label69');" onmouseout="ContentUnpreview('label69');" title="click to collapse or expand..."> more... </a>
 <div id="label69" style="display:none">
 <table border="1">
 <tr>
 <td></td>
 <td colspan="2">Supported Version Ranges</td>
 </tr>
 <tr>
 <td>ssl_ocsp_source_ip</td>
 <td><code class="docutils literal notranslate">v6.2.0 -> v6.2.0 </code></td>
 <td><code class="docutils literal notranslate">v6.2.5 -> v7.2.4 </code></td>
 </tr>
 </table>
 </div>
 </li>
        <li> <span class="li-head">ssl_ocsp_status</span> - Enable/disable SSL OCSP. <span class="li-normal">type: str</span> <span class="li-normal">choices: enable, disable</span>
 <a id='label70' href="javascript:ContentClick('label71', 'label70');" onmouseover="ContentPreview('label71');" onmouseout="ContentUnpreview('label71');" title="click to collapse or expand..."> more... </a>
 <div id="label71" style="display:none">
 <table border="1">
 <tr>
 <td></td>
 <td colspan="1">Supported Version Ranges</td>
 </tr>
 <tr>
 <td>ssl_ocsp_status</td>
 <td><code class="docutils literal notranslate">v6.0.0 -> v6.0.11 </code></td>
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
        <li> <span class="li-head">strict_crl_check</span> - Enable/disable strict mode CRL checking. <span class="li-normal">type: str</span> <span class="li-normal">choices: enable, disable</span>
 <a id='label72' href="javascript:ContentClick('label73', 'label72');" onmouseover="ContentPreview('label73');" onmouseout="ContentUnpreview('label73');" title="click to collapse or expand..."> more... </a>
 <div id="label73" style="display:none">
 <table border="1">
 <tr>
 <td></td>
 <td colspan="1">Supported Version Ranges</td>
 </tr>
 <tr>
 <td>strict_crl_check</td>
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
        <li> <span class="li-head">strict_ocsp_check</span> - Enable/disable strict mode OCSP checking. <span class="li-normal">type: str</span> <span class="li-normal">choices: enable, disable</span>
 <a id='label74' href="javascript:ContentClick('label75', 'label74');" onmouseover="ContentPreview('label75');" onmouseout="ContentUnpreview('label75');" title="click to collapse or expand..."> more... </a>
 <div id="label75" style="display:none">
 <table border="1">
 <tr>
 <td></td>
 <td colspan="1">Supported Version Ranges</td>
 </tr>
 <tr>
 <td>strict_ocsp_check</td>
 <td><code class="docutils literal notranslate">v6.0.0 -> 7.4.3 </code></td>
 </tr>
 <tr>
 <td>[enable]</td>
 <td><code class="docutils literal notranslate">v6.0.0 -> 7.4.3</code></td>
 <tr>
 <td>[disable]</td>
 <td><code class="docutils literal notranslate">v6.0.0 -> 7.4.3</code></td>
 </table>
 </div>
 </li>
        <li> <span class="li-head">subject_match</span> - When searching for a matching certificate, control how to do RDN value matching with certificate subject name . <span class="li-normal">type: str</span> <span class="li-normal">choices: substring, value</span>
 <a id='label76' href="javascript:ContentClick('label77', 'label76');" onmouseover="ContentPreview('label77');" onmouseout="ContentUnpreview('label77');" title="click to collapse or expand..."> more... </a>
 <div id="label77" style="display:none">
 <table border="1">
 <tr>
 <td></td>
 <td colspan="1">Supported Version Ranges</td>
 </tr>
 <tr>
 <td>subject_match</td>
 <td><code class="docutils literal notranslate">v6.0.0 -> 7.4.3 </code></td>
 </tr>
 <tr>
 <td>[substring]</td>
 <td><code class="docutils literal notranslate">v6.0.0 -> 7.4.3</code></td>
 <tr>
 <td>[value]</td>
 <td><code class="docutils literal notranslate">v6.0.0 -> 7.4.3</code></td>
 </table>
 </div>
 </li>
        <li> <span class="li-head">subject_set</span> - When searching for a matching certificate, control how to do RDN set matching with certificate subject name . <span class="li-normal">type: str</span> <span class="li-normal">choices: subset, superset</span>
 <a id='label78' href="javascript:ContentClick('label79', 'label78');" onmouseover="ContentPreview('label79');" onmouseout="ContentUnpreview('label79');" title="click to collapse or expand..."> more... </a>
 <div id="label79" style="display:none">
 <table border="1">
 <tr>
 <td></td>
 <td colspan="1">Supported Version Ranges</td>
 </tr>
 <tr>
 <td>subject_set</td>
 <td><code class="docutils literal notranslate">v7.0.1 -> 7.4.3 </code></td>
 </tr>
 <tr>
 <td>[subset]</td>
 <td><code class="docutils literal notranslate">v7.0.1 -> 7.4.3</code></td>
 <tr>
 <td>[superset]</td>
 <td><code class="docutils literal notranslate">v7.0.1 -> 7.4.3</code></td>
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
    
    - name: VPN certificate setting.
      fortinet.fortios.fortios_vpn_certificate_setting:
          vdom: "{{ vdom }}"
          vpn_certificate_setting:
              cert_expire_warning: "14"
              certname_dsa1024: "<your_own_value> (source vpn.certificate.local.name)"
              certname_dsa2048: "<your_own_value> (source vpn.certificate.local.name)"
              certname_ecdsa256: "<your_own_value> (source vpn.certificate.local.name)"
              certname_ecdsa384: "<your_own_value> (source vpn.certificate.local.name)"
              certname_ecdsa521: "<your_own_value> (source vpn.certificate.local.name)"
              certname_ed25519: "<your_own_value> (source vpn.certificate.local.name)"
              certname_ed448: "<your_own_value> (source vpn.certificate.local.name)"
              certname_rsa1024: "<your_own_value> (source vpn.certificate.local.name)"
              certname_rsa2048: "<your_own_value> (source vpn.certificate.local.name)"
              certname_rsa4096: "<your_own_value> (source vpn.certificate.local.name)"
              check_ca_cert: "enable"
              check_ca_chain: "enable"
              cmp_key_usage_checking: "enable"
              cmp_save_extra_certs: "enable"
              cn_allow_multi: "disable"
              cn_match: "substring"
              crl_verification:
                  chain_crl_absence: "ignore"
                  expiry: "ignore"
                  leaf_crl_absence: "ignore"
              interface: "<your_own_value> (source system.interface.name)"
              interface_select_method: "auto"
              ocsp_default_server: "<your_own_value> (source vpn.certificate.ocsp-server.name)"
              ocsp_option: "certificate"
              ocsp_status: "enable"
              proxy: "<your_own_value>"
              proxy_password: "<your_own_value>"
              proxy_port: "8080"
              proxy_username: "<your_own_value>"
              source_ip: "84.230.14.43"
              ssl_min_proto_version: "default"
              ssl_ocsp_option: "certificate"
              ssl_ocsp_source_ip: "<your_own_value>"
              ssl_ocsp_status: "enable"
              strict_crl_check: "enable"
              strict_ocsp_check: "enable"
              subject_match: "substring"
              subject_set: "subset"


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
