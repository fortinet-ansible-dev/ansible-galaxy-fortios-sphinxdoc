:source: fortios_user_saml.py

:orphan:

.. fortios_user_saml:

fortios_user_saml -- SAML server entry configuration in Fortinet's FortiOS and FortiGate.
+++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++

.. versionadded:: 2.0.0

.. contents::
   :local:
   :depth: 1


Synopsis
--------
- This module is able to configure a FortiGate or FortiOS (FOS) device by allowing the user to set and modify user feature and saml category. Examples include all parameters and values need to be adjusted to datasources before usage. Tested with FOS v6.0.0



Requirements
------------
The below requirements are needed on the host that executes this module.

- ansible>=2.15


Tips
----
Using member operation to add an element to an existing object.

FortiOS Version Compatibility
-----------------------------
Supported Version Ranges: v6.2.0 -> 7.4.3



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
    <li> <span class="li-head">user_saml</span> - SAML server entry configuration. <span class="li-normal">type: dict</span>
 <a id='label0' href="javascript:ContentClick('label1', 'label0');" onmouseover="ContentPreview('label1');" onmouseout="ContentUnpreview('label1');" title="click to collapse or expand..."> more... </a>
 <div id="label1" style="display:none">
 <table border="1">
 <tr>
 <td></td><td colspan="1">Supported Version Ranges</td>
 </tr>
 <tr>
 <td>user_saml</td>
 <td><code class="docutils literal notranslate">v6.2.0 -> 7.4.3 </code></td>
 </tr>
 </table>
 </div>
 </li>
        <ul class="ul-self">
        <li> <span class="li-head">adfs_claim</span> - Enable/disable ADFS Claim for user/group attribute in assertion statement . <span class="li-normal">type: str</span> <span class="li-normal">choices: enable, disable</span>
 <a id='label2' href="javascript:ContentClick('label3', 'label2');" onmouseover="ContentPreview('label3');" onmouseout="ContentUnpreview('label3');" title="click to collapse or expand..."> more... </a>
 <div id="label3" style="display:none">
 <table border="1">
 <tr>
 <td></td>
 <td colspan="1">Supported Version Ranges</td>
 </tr>
 <tr>
 <td>adfs_claim</td>
 <td><code class="docutils literal notranslate">v7.0.0 -> 7.4.3 </code></td>
 </tr>
 <tr>
 <td>[enable]</td>
 <td><code class="docutils literal notranslate">v7.0.0 -> 7.4.3</code></td>
 <tr>
 <td>[disable]</td>
 <td><code class="docutils literal notranslate">v7.0.0 -> 7.4.3</code></td>
 </table>
 </div>
 </li>
        <li> <span class="li-head">auth_url</span> - URL to verify authentication. <span class="li-normal">type: str</span>
 <a id='label4' href="javascript:ContentClick('label5', 'label4');" onmouseover="ContentPreview('label5');" onmouseout="ContentUnpreview('label5');" title="click to collapse or expand..."> more... </a>
 <div id="label5" style="display:none">
 <table border="1">
 <tr>
 <td></td>
 <td colspan="1">Supported Version Ranges</td>
 </tr>
 <tr>
 <td>auth_url</td>
 <td><code class="docutils literal notranslate">v7.2.1 -> v7.4.1 </code></td>
 </tr>
 </table>
 </div>
 </li>
        <li> <span class="li-head">cert</span> - Certificate to sign SAML messages. Source vpn.certificate.local.name. <span class="li-normal">type: str</span>
 <a id='label6' href="javascript:ContentClick('label7', 'label6');" onmouseover="ContentPreview('label7');" onmouseout="ContentUnpreview('label7');" title="click to collapse or expand..."> more... </a>
 <div id="label7" style="display:none">
 <table border="1">
 <tr>
 <td></td>
 <td colspan="1">Supported Version Ranges</td>
 </tr>
 <tr>
 <td>cert</td>
 <td><code class="docutils literal notranslate">v6.2.0 -> 7.4.3 </code></td>
 </tr>
 </table>
 </div>
 </li>
        <li> <span class="li-head">clock_tolerance</span> - Clock skew tolerance in seconds (0 - 300). <span class="li-normal">type: int</span>
 <a id='label8' href="javascript:ContentClick('label9', 'label8');" onmouseover="ContentPreview('label9');" onmouseout="ContentUnpreview('label9');" title="click to collapse or expand..."> more... </a>
 <div id="label9" style="display:none">
 <table border="1">
 <tr>
 <td></td>
 <td colspan="1">Supported Version Ranges</td>
 </tr>
 <tr>
 <td>clock_tolerance</td>
 <td><code class="docutils literal notranslate">v7.0.4 -> 7.4.3 </code></td>
 </tr>
 </table>
 </div>
 </li>
        <li> <span class="li-head">digest_method</span> - Digest method algorithm . <span class="li-normal">type: str</span> <span class="li-normal">choices: sha1, sha256</span>
 <a id='label10' href="javascript:ContentClick('label11', 'label10');" onmouseover="ContentPreview('label11');" onmouseout="ContentUnpreview('label11');" title="click to collapse or expand..."> more... </a>
 <div id="label11" style="display:none">
 <table border="1">
 <tr>
 <td></td>
 <td colspan="1">Supported Version Ranges</td>
 </tr>
 <tr>
 <td>digest_method</td>
 <td><code class="docutils literal notranslate">v7.0.0 -> 7.4.3 </code></td>
 </tr>
 <tr>
 <td>[sha1]</td>
 <td><code class="docutils literal notranslate">v7.0.0 -> 7.4.3</code></td>
 <tr>
 <td>[sha256]</td>
 <td><code class="docutils literal notranslate">v7.0.0 -> 7.4.3</code></td>
 </table>
 </div>
 </li>
        <li> <span class="li-head">entity_id</span> - SP entity ID. <span class="li-normal">type: str</span>
 <a id='label12' href="javascript:ContentClick('label13', 'label12');" onmouseover="ContentPreview('label13');" onmouseout="ContentUnpreview('label13');" title="click to collapse or expand..."> more... </a>
 <div id="label13" style="display:none">
 <table border="1">
 <tr>
 <td></td>
 <td colspan="1">Supported Version Ranges</td>
 </tr>
 <tr>
 <td>entity_id</td>
 <td><code class="docutils literal notranslate">v6.2.0 -> 7.4.3 </code></td>
 </tr>
 </table>
 </div>
 </li>
        <li> <span class="li-head">group_claim_type</span> - Group claim in assertion statement. <span class="li-normal">type: str</span> <span class="li-normal">choices: email, given-name, name, upn, common-name, email-adfs-1x, group, upn-adfs-1x, role, sur-name, ppid, name-identifier, authentication-method, deny-only-group-sid, deny-only-primary-sid, deny-only-primary-group-sid, group-sid, primary-group-sid, primary-sid, windows-account-name</span>
 <a id='label14' href="javascript:ContentClick('label15', 'label14');" onmouseover="ContentPreview('label15');" onmouseout="ContentUnpreview('label15');" title="click to collapse or expand..."> more... </a>
 <div id="label15" style="display:none">
 <table border="1">
 <tr>
 <td></td>
 <td colspan="1">Supported Version Ranges</td>
 </tr>
 <tr>
 <td>group_claim_type</td>
 <td><code class="docutils literal notranslate">v7.0.0 -> 7.4.3 </code></td>
 </tr>
 <tr>
 <td>[email]</td>
 <td><code class="docutils literal notranslate">v7.0.0 -> 7.4.3</code></td>
 <tr>
 <td>[given-name]</td>
 <td><code class="docutils literal notranslate">v7.0.0 -> 7.4.3</code></td>
 <tr>
 <td>[name]</td>
 <td><code class="docutils literal notranslate">v7.0.0 -> 7.4.3</code></td>
 <tr>
 <td>[upn]</td>
 <td><code class="docutils literal notranslate">v7.0.0 -> 7.4.3</code></td>
 <tr>
 <td>[common-name]</td>
 <td><code class="docutils literal notranslate">v7.0.0 -> 7.4.3</code></td>
 <tr>
 <td>[email-adfs-1x]</td>
 <td><code class="docutils literal notranslate">v7.0.0 -> 7.4.3</code></td>
 <tr>
 <td>[group]</td>
 <td><code class="docutils literal notranslate">v7.0.0 -> 7.4.3</code></td>
 <tr>
 <td>[upn-adfs-1x]</td>
 <td><code class="docutils literal notranslate">v7.0.0 -> 7.4.3</code></td>
 <tr>
 <td>[role]</td>
 <td><code class="docutils literal notranslate">v7.0.0 -> 7.4.3</code></td>
 <tr>
 <td>[sur-name]</td>
 <td><code class="docutils literal notranslate">v7.0.0 -> 7.4.3</code></td>
 <tr>
 <td>[ppid]</td>
 <td><code class="docutils literal notranslate">v7.0.0 -> 7.4.3</code></td>
 <tr>
 <td>[name-identifier]</td>
 <td><code class="docutils literal notranslate">v7.0.0 -> 7.4.3</code></td>
 <tr>
 <td>[authentication-method]</td>
 <td><code class="docutils literal notranslate">v7.0.0 -> 7.4.3</code></td>
 <tr>
 <td>[deny-only-group-sid]</td>
 <td><code class="docutils literal notranslate">v7.0.0 -> 7.4.3</code></td>
 <tr>
 <td>[deny-only-primary-sid]</td>
 <td><code class="docutils literal notranslate">v7.0.0 -> 7.4.3</code></td>
 <tr>
 <td>[deny-only-primary-group-sid]</td>
 <td><code class="docutils literal notranslate">v7.0.0 -> 7.4.3</code></td>
 <tr>
 <td>[group-sid]</td>
 <td><code class="docutils literal notranslate">v7.0.0 -> 7.4.3</code></td>
 <tr>
 <td>[primary-group-sid]</td>
 <td><code class="docutils literal notranslate">v7.0.0 -> 7.4.3</code></td>
 <tr>
 <td>[primary-sid]</td>
 <td><code class="docutils literal notranslate">v7.0.0 -> 7.4.3</code></td>
 <tr>
 <td>[windows-account-name]</td>
 <td><code class="docutils literal notranslate">v7.0.0 -> 7.4.3</code></td>
 </table>
 </div>
 </li>
        <li> <span class="li-head">group_name</span> - Group name in assertion statement. <span class="li-normal">type: str</span>
 <a id='label16' href="javascript:ContentClick('label17', 'label16');" onmouseover="ContentPreview('label17');" onmouseout="ContentUnpreview('label17');" title="click to collapse or expand..."> more... </a>
 <div id="label17" style="display:none">
 <table border="1">
 <tr>
 <td></td>
 <td colspan="1">Supported Version Ranges</td>
 </tr>
 <tr>
 <td>group_name</td>
 <td><code class="docutils literal notranslate">v6.2.0 -> 7.4.3 </code></td>
 </tr>
 </table>
 </div>
 </li>
        <li> <span class="li-head">idp_cert</span> - IDP Certificate name. Source vpn.certificate.remote.name. <span class="li-normal">type: str</span>
 <a id='label18' href="javascript:ContentClick('label19', 'label18');" onmouseover="ContentPreview('label19');" onmouseout="ContentUnpreview('label19');" title="click to collapse or expand..."> more... </a>
 <div id="label19" style="display:none">
 <table border="1">
 <tr>
 <td></td>
 <td colspan="1">Supported Version Ranges</td>
 </tr>
 <tr>
 <td>idp_cert</td>
 <td><code class="docutils literal notranslate">v6.2.0 -> 7.4.3 </code></td>
 </tr>
 </table>
 </div>
 </li>
        <li> <span class="li-head">idp_entity_id</span> - IDP entity ID. <span class="li-normal">type: str</span>
 <a id='label20' href="javascript:ContentClick('label21', 'label20');" onmouseover="ContentPreview('label21');" onmouseout="ContentUnpreview('label21');" title="click to collapse or expand..."> more... </a>
 <div id="label21" style="display:none">
 <table border="1">
 <tr>
 <td></td>
 <td colspan="1">Supported Version Ranges</td>
 </tr>
 <tr>
 <td>idp_entity_id</td>
 <td><code class="docutils literal notranslate">v6.2.0 -> 7.4.3 </code></td>
 </tr>
 </table>
 </div>
 </li>
        <li> <span class="li-head">idp_single_logout_url</span> - IDP single logout url. <span class="li-normal">type: str</span>
 <a id='label22' href="javascript:ContentClick('label23', 'label22');" onmouseover="ContentPreview('label23');" onmouseout="ContentUnpreview('label23');" title="click to collapse or expand..."> more... </a>
 <div id="label23" style="display:none">
 <table border="1">
 <tr>
 <td></td>
 <td colspan="1">Supported Version Ranges</td>
 </tr>
 <tr>
 <td>idp_single_logout_url</td>
 <td><code class="docutils literal notranslate">v6.2.0 -> 7.4.3 </code></td>
 </tr>
 </table>
 </div>
 </li>
        <li> <span class="li-head">idp_single_sign_on_url</span> - IDP single sign-on URL. <span class="li-normal">type: str</span>
 <a id='label24' href="javascript:ContentClick('label25', 'label24');" onmouseover="ContentPreview('label25');" onmouseout="ContentUnpreview('label25');" title="click to collapse or expand..."> more... </a>
 <div id="label25" style="display:none">
 <table border="1">
 <tr>
 <td></td>
 <td colspan="1">Supported Version Ranges</td>
 </tr>
 <tr>
 <td>idp_single_sign_on_url</td>
 <td><code class="docutils literal notranslate">v6.2.0 -> 7.4.3 </code></td>
 </tr>
 </table>
 </div>
 </li>
        <li> <span class="li-head">limit_relaystate</span> - Enable/disable limiting of relay-state parameter when it exceeds SAML 2.0 specification limits (80 bytes). <span class="li-normal">type: str</span> <span class="li-normal">choices: enable, disable</span>
 <a id='label26' href="javascript:ContentClick('label27', 'label26');" onmouseover="ContentPreview('label27');" onmouseout="ContentUnpreview('label27');" title="click to collapse or expand..."> more... </a>
 <div id="label27" style="display:none">
 <table border="1">
 <tr>
 <td></td>
 <td colspan="1">Supported Version Ranges</td>
 </tr>
 <tr>
 <td>limit_relaystate</td>
 <td><code class="docutils literal notranslate">v7.0.0 -> 7.4.3 </code></td>
 </tr>
 <tr>
 <td>[enable]</td>
 <td><code class="docutils literal notranslate">v7.0.0 -> 7.4.3</code></td>
 <tr>
 <td>[disable]</td>
 <td><code class="docutils literal notranslate">v7.0.0 -> 7.4.3</code></td>
 </table>
 </div>
 </li>
        <li> <span class="li-head">name</span> - SAML server entry name. <span class="li-normal">type: str</span> <span class="li-required">required: true</span>
 <a id='label28' href="javascript:ContentClick('label29', 'label28');" onmouseover="ContentPreview('label29');" onmouseout="ContentUnpreview('label29');" title="click to collapse or expand..."> more... </a>
 <div id="label29" style="display:none">
 <table border="1">
 <tr>
 <td></td>
 <td colspan="1">Supported Version Ranges</td>
 </tr>
 <tr>
 <td>name</td>
 <td><code class="docutils literal notranslate">v6.2.0 -> 7.4.3 </code></td>
 </tr>
 </table>
 </div>
 </li>
        <li> <span class="li-head">reauth</span> - Enable/disable signalling of IDP to force user re-authentication . <span class="li-normal">type: str</span> <span class="li-normal">choices: enable, disable</span>
 <a id='label30' href="javascript:ContentClick('label31', 'label30');" onmouseover="ContentPreview('label31');" onmouseout="ContentUnpreview('label31');" title="click to collapse or expand..."> more... </a>
 <div id="label31" style="display:none">
 <table border="1">
 <tr>
 <td></td>
 <td colspan="1">Supported Version Ranges</td>
 </tr>
 <tr>
 <td>reauth</td>
 <td><code class="docutils literal notranslate">v7.4.1 -> 7.4.3 </code></td>
 </tr>
 <tr>
 <td>[enable]</td>
 <td><code class="docutils literal notranslate">v7.4.1 -> 7.4.3</code></td>
 <tr>
 <td>[disable]</td>
 <td><code class="docutils literal notranslate">v7.4.1 -> 7.4.3</code></td>
 </table>
 </div>
 </li>
        <li> <span class="li-head">single_logout_url</span> - SP single logout URL. <span class="li-normal">type: str</span>
 <a id='label32' href="javascript:ContentClick('label33', 'label32');" onmouseover="ContentPreview('label33');" onmouseout="ContentUnpreview('label33');" title="click to collapse or expand..."> more... </a>
 <div id="label33" style="display:none">
 <table border="1">
 <tr>
 <td></td>
 <td colspan="1">Supported Version Ranges</td>
 </tr>
 <tr>
 <td>single_logout_url</td>
 <td><code class="docutils literal notranslate">v6.2.0 -> 7.4.3 </code></td>
 </tr>
 </table>
 </div>
 </li>
        <li> <span class="li-head">single_sign_on_url</span> - SP single sign-on URL. <span class="li-normal">type: str</span>
 <a id='label34' href="javascript:ContentClick('label35', 'label34');" onmouseover="ContentPreview('label35');" onmouseout="ContentUnpreview('label35');" title="click to collapse or expand..."> more... </a>
 <div id="label35" style="display:none">
 <table border="1">
 <tr>
 <td></td>
 <td colspan="1">Supported Version Ranges</td>
 </tr>
 <tr>
 <td>single_sign_on_url</td>
 <td><code class="docutils literal notranslate">v6.2.0 -> 7.4.3 </code></td>
 </tr>
 </table>
 </div>
 </li>
        <li> <span class="li-head">user_claim_type</span> - User name claim in assertion statement. <span class="li-normal">type: str</span> <span class="li-normal">choices: email, given-name, name, upn, common-name, email-adfs-1x, group, upn-adfs-1x, role, sur-name, ppid, name-identifier, authentication-method, deny-only-group-sid, deny-only-primary-sid, deny-only-primary-group-sid, group-sid, primary-group-sid, primary-sid, windows-account-name</span>
 <a id='label36' href="javascript:ContentClick('label37', 'label36');" onmouseover="ContentPreview('label37');" onmouseout="ContentUnpreview('label37');" title="click to collapse or expand..."> more... </a>
 <div id="label37" style="display:none">
 <table border="1">
 <tr>
 <td></td>
 <td colspan="1">Supported Version Ranges</td>
 </tr>
 <tr>
 <td>user_claim_type</td>
 <td><code class="docutils literal notranslate">v7.0.0 -> 7.4.3 </code></td>
 </tr>
 <tr>
 <td>[email]</td>
 <td><code class="docutils literal notranslate">v7.0.0 -> 7.4.3</code></td>
 <tr>
 <td>[given-name]</td>
 <td><code class="docutils literal notranslate">v7.0.0 -> 7.4.3</code></td>
 <tr>
 <td>[name]</td>
 <td><code class="docutils literal notranslate">v7.0.0 -> 7.4.3</code></td>
 <tr>
 <td>[upn]</td>
 <td><code class="docutils literal notranslate">v7.0.0 -> 7.4.3</code></td>
 <tr>
 <td>[common-name]</td>
 <td><code class="docutils literal notranslate">v7.0.0 -> 7.4.3</code></td>
 <tr>
 <td>[email-adfs-1x]</td>
 <td><code class="docutils literal notranslate">v7.0.0 -> 7.4.3</code></td>
 <tr>
 <td>[group]</td>
 <td><code class="docutils literal notranslate">v7.0.0 -> 7.4.3</code></td>
 <tr>
 <td>[upn-adfs-1x]</td>
 <td><code class="docutils literal notranslate">v7.0.0 -> 7.4.3</code></td>
 <tr>
 <td>[role]</td>
 <td><code class="docutils literal notranslate">v7.0.0 -> 7.4.3</code></td>
 <tr>
 <td>[sur-name]</td>
 <td><code class="docutils literal notranslate">v7.0.0 -> 7.4.3</code></td>
 <tr>
 <td>[ppid]</td>
 <td><code class="docutils literal notranslate">v7.0.0 -> 7.4.3</code></td>
 <tr>
 <td>[name-identifier]</td>
 <td><code class="docutils literal notranslate">v7.0.0 -> 7.4.3</code></td>
 <tr>
 <td>[authentication-method]</td>
 <td><code class="docutils literal notranslate">v7.0.0 -> 7.4.3</code></td>
 <tr>
 <td>[deny-only-group-sid]</td>
 <td><code class="docutils literal notranslate">v7.0.0 -> 7.4.3</code></td>
 <tr>
 <td>[deny-only-primary-sid]</td>
 <td><code class="docutils literal notranslate">v7.0.0 -> 7.4.3</code></td>
 <tr>
 <td>[deny-only-primary-group-sid]</td>
 <td><code class="docutils literal notranslate">v7.0.0 -> 7.4.3</code></td>
 <tr>
 <td>[group-sid]</td>
 <td><code class="docutils literal notranslate">v7.0.0 -> 7.4.3</code></td>
 <tr>
 <td>[primary-group-sid]</td>
 <td><code class="docutils literal notranslate">v7.0.0 -> 7.4.3</code></td>
 <tr>
 <td>[primary-sid]</td>
 <td><code class="docutils literal notranslate">v7.0.0 -> 7.4.3</code></td>
 <tr>
 <td>[windows-account-name]</td>
 <td><code class="docutils literal notranslate">v7.0.0 -> 7.4.3</code></td>
 </table>
 </div>
 </li>
        <li> <span class="li-head">user_name</span> - User name in assertion statement. <span class="li-normal">type: str</span>
 <a id='label38' href="javascript:ContentClick('label39', 'label38');" onmouseover="ContentPreview('label39');" onmouseout="ContentUnpreview('label39');" title="click to collapse or expand..."> more... </a>
 <div id="label39" style="display:none">
 <table border="1">
 <tr>
 <td></td>
 <td colspan="1">Supported Version Ranges</td>
 </tr>
 <tr>
 <td>user_name</td>
 <td><code class="docutils literal notranslate">v6.2.0 -> 7.4.3 </code></td>
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
    
    - name: SAML server entry configuration.
      fortinet.fortios.fortios_user_saml:
          vdom: "{{ vdom }}"
          state: "present"
          access_token: "<your_own_value>"
          user_saml:
              adfs_claim: "enable"
              auth_url: "<your_own_value>"
              cert: "<your_own_value> (source vpn.certificate.local.name)"
              clock_tolerance: "15"
              digest_method: "sha1"
              entity_id: "<your_own_value>"
              group_claim_type: "email"
              group_name: "<your_own_value>"
              idp_cert: "<your_own_value> (source vpn.certificate.remote.name)"
              idp_entity_id: "<your_own_value>"
              idp_single_logout_url: "<your_own_value>"
              idp_single_sign_on_url: "<your_own_value>"
              limit_relaystate: "enable"
              name: "default_name_16"
              reauth: "enable"
              single_logout_url: "<your_own_value>"
              single_sign_on_url: "<your_own_value>"
              user_claim_type: "email"
              user_name: "<your_own_value>"


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
