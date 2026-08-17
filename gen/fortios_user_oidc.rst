:source: fortios_user_oidc.py

:orphan:

.. fortios_user_oidc:

fortios_user_oidc -- OpenID Connect server entry configuration in Fortinet's FortiOS and FortiGate.
+++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++

.. versionadded:: 2.0.0

.. contents::
   :local:
   :depth: 1


Synopsis
--------
- This module is able to configure a FortiGate or FortiOS (FOS) device by allowing the user to set and modify user feature and oidc category. Examples include all parameters and values need to be adjusted to datasources before usage. Tested with FOS v6.0.0



Requirements
------------
The below requirements are needed on the host that executes this module.

- ansible>=2.16


Tips
----
Using member operation to add an element to an existing object.

FortiOS Version Compatibility
-----------------------------
Supported Version Ranges: v8.0.0


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
    <li> <span class="li-head">user_oidc</span> - OpenID Connect server entry configuration. <span class="li-normal">type: dict</span>
 <a id='label0' href="javascript:ContentClick('label1', 'label0');" onmouseover="ContentPreview('label1');" onmouseout="ContentUnpreview('label1');" title="click to collapse or expand..."> more... </a>
 <div id="label1" style="display:none">
 <table border="1">
 <tr>
 <td></td><td colspan="1">Supported Version Ranges</td>
 </tr>
 <tr>
 <td>user_oidc</td>
 <td><code class="docutils literal notranslate">v8.0.0 -> 8.0.0 </code></td>
 </tr>
 </table>
 </div>
 </li>
        <ul class="ul-self">
        <li> <span class="li-head">authorization_url</span> - OpenID Connect server authorization URL. <span class="li-normal">type: str</span>
 <a id='label2' href="javascript:ContentClick('label3', 'label2');" onmouseover="ContentPreview('label3');" onmouseout="ContentUnpreview('label3');" title="click to collapse or expand..."> more... </a>
 <div id="label3" style="display:none">
 <table border="1">
 <tr>
 <td></td>
 <td colspan="1">Supported Version Ranges</td>
 </tr>
 <tr>
 <td>authorization_url</td>
 <td><code class="docutils literal notranslate">v8.0.0 -> 8.0.0 </code></td>
 </tr>
 </table>
 </div>
 </li>
        <li> <span class="li-head">client_id</span> - OpenID Connect server client ID. <span class="li-normal">type: str</span>
 <a id='label4' href="javascript:ContentClick('label5', 'label4');" onmouseover="ContentPreview('label5');" onmouseout="ContentUnpreview('label5');" title="click to collapse or expand..."> more... </a>
 <div id="label5" style="display:none">
 <table border="1">
 <tr>
 <td></td>
 <td colspan="1">Supported Version Ranges</td>
 </tr>
 <tr>
 <td>client_id</td>
 <td><code class="docutils literal notranslate">v8.0.0 -> 8.0.0 </code></td>
 </tr>
 </table>
 </div>
 </li>
        <li> <span class="li-head">client_secret</span> - OpenID Connect server client secret. <span class="li-normal">type: str</span>
 <a id='label6' href="javascript:ContentClick('label7', 'label6');" onmouseover="ContentPreview('label7');" onmouseout="ContentUnpreview('label7');" title="click to collapse or expand..."> more... </a>
 <div id="label7" style="display:none">
 <table border="1">
 <tr>
 <td></td>
 <td colspan="1">Supported Version Ranges</td>
 </tr>
 <tr>
 <td>client_secret</td>
 <td><code class="docutils literal notranslate">v8.0.0 -> 8.0.0 </code></td>
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
 <td><code class="docutils literal notranslate">v8.0.0 -> 8.0.0 </code></td>
 </tr>
 </table>
 </div>
 </li>
        <li> <span class="li-head">discovery_url</span> - OpenID Connect server discovery URL. <span class="li-normal">type: str</span>
 <a id='label10' href="javascript:ContentClick('label11', 'label10');" onmouseover="ContentPreview('label11');" onmouseout="ContentUnpreview('label11');" title="click to collapse or expand..."> more... </a>
 <div id="label11" style="display:none">
 <table border="1">
 <tr>
 <td></td>
 <td colspan="1">Supported Version Ranges</td>
 </tr>
 <tr>
 <td>discovery_url</td>
 <td><code class="docutils literal notranslate">v8.0.0 -> 8.0.0 </code></td>
 </tr>
 </table>
 </div>
 </li>
        <li> <span class="li-head">domain_hint</span> - Domain Hint. <span class="li-normal">type: str</span>
 <a id='label12' href="javascript:ContentClick('label13', 'label12');" onmouseover="ContentPreview('label13');" onmouseout="ContentUnpreview('label13');" title="click to collapse or expand..."> more... </a>
 <div id="label13" style="display:none">
 <table border="1">
 <tr>
 <td></td>
 <td colspan="1">Supported Version Ranges</td>
 </tr>
 <tr>
 <td>domain_hint</td>
 <td><code class="docutils literal notranslate">v8.0.0 -> 8.0.0 </code></td>
 </tr>
 </table>
 </div>
 </li>
        <li> <span class="li-head">issuer</span> - OpenID Connect server issuer. <span class="li-normal">type: str</span>
 <a id='label14' href="javascript:ContentClick('label15', 'label14');" onmouseover="ContentPreview('label15');" onmouseout="ContentUnpreview('label15');" title="click to collapse or expand..."> more... </a>
 <div id="label15" style="display:none">
 <table border="1">
 <tr>
 <td></td>
 <td colspan="1">Supported Version Ranges</td>
 </tr>
 <tr>
 <td>issuer</td>
 <td><code class="docutils literal notranslate">v8.0.0 -> 8.0.0 </code></td>
 </tr>
 </table>
 </div>
 </li>
        <li> <span class="li-head">jwks_uri</span> - URL of the OP"s JWK Set document. <span class="li-normal">type: str</span>
 <a id='label16' href="javascript:ContentClick('label17', 'label16');" onmouseover="ContentPreview('label17');" onmouseout="ContentUnpreview('label17');" title="click to collapse or expand..."> more... </a>
 <div id="label17" style="display:none">
 <table border="1">
 <tr>
 <td></td>
 <td colspan="1">Supported Version Ranges</td>
 </tr>
 <tr>
 <td>jwks_uri</td>
 <td><code class="docutils literal notranslate">v8.0.0 -> 8.0.0 </code></td>
 </tr>
 </table>
 </div>
 </li>
        <li> <span class="li-head">ldap_server</span> - LDAP server name(s). <span class="li-normal">type: list</span> <span style="font-family:'Courier New'" class="li-required">member_path: ldap_server:name</span>
 <a id='label18' href="javascript:ContentClick('label19', 'label18');" onmouseover="ContentPreview('label19');" onmouseout="ContentUnpreview('label19');" title="click to collapse or expand..."> more... </a>
 <div id="label19" style="display:none">
 <table border="1">
 <tr>
 <td></td><td colspan="1">Supported Version Ranges</td>
 </tr>
 <tr>
 <td>ldap_server</td>
 <td><code class="docutils literal notranslate">v8.0.0 -> 8.0.0 </code></td>
 </tr>
 </table>
 </div>
 </li>
            <ul class="ul-self">
            <li> <span class="li-head">name</span> - LDAP server name. Source user.ldap.name. <span class="li-normal">type: str</span> <span class="li-required">required: true</span>
 <a id='label20' href="javascript:ContentClick('label21', 'label20');" onmouseover="ContentPreview('label21');" onmouseout="ContentUnpreview('label21');" title="click to collapse or expand..."> more... </a>
 <div id="label21" style="display:none">
 <table border="1">
 <tr>
 <td></td>
 <td colspan="1">Supported Version Ranges</td>
 </tr>
 <tr>
 <td>name</td>
 <td><code class="docutils literal notranslate">v8.0.0 -> 8.0.0 </code></td>
 </tr>
 </table>
 </div>
 </li>
            </ul>
        <li> <span class="li-head">name</span> - OpenID Connect server entry name. <span class="li-normal">type: str</span> <span class="li-required">required: true</span>
 <a id='label22' href="javascript:ContentClick('label23', 'label22');" onmouseover="ContentPreview('label23');" onmouseout="ContentUnpreview('label23');" title="click to collapse or expand..."> more... </a>
 <div id="label23" style="display:none">
 <table border="1">
 <tr>
 <td></td>
 <td colspan="1">Supported Version Ranges</td>
 </tr>
 <tr>
 <td>name</td>
 <td><code class="docutils literal notranslate">v8.0.0 -> 8.0.0 </code></td>
 </tr>
 </table>
 </div>
 </li>
        <li> <span class="li-head">token_url</span> - OpenID Connect server token URL. <span class="li-normal">type: str</span>
 <a id='label24' href="javascript:ContentClick('label25', 'label24');" onmouseover="ContentPreview('label25');" onmouseout="ContentUnpreview('label25');" title="click to collapse or expand..."> more... </a>
 <div id="label25" style="display:none">
 <table border="1">
 <tr>
 <td></td>
 <td colspan="1">Supported Version Ranges</td>
 </tr>
 <tr>
 <td>token_url</td>
 <td><code class="docutils literal notranslate">v8.0.0 -> 8.0.0 </code></td>
 </tr>
 </table>
 </div>
 </li>
        <li> <span class="li-head">type</span> - Type of OpenID Connect config. <span class="li-normal">type: str</span> <span class="li-normal">choices: discovery, manual</span>
 <a id='label26' href="javascript:ContentClick('label27', 'label26');" onmouseover="ContentPreview('label27');" onmouseout="ContentUnpreview('label27');" title="click to collapse or expand..."> more... </a>
 <div id="label27" style="display:none">
 <table border="1">
 <tr>
 <td></td>
 <td colspan="1">Supported Version Ranges</td>
 </tr>
 <tr>
 <td>type</td>
 <td><code class="docutils literal notranslate">v8.0.0 -> 8.0.0 </code></td>
 </tr>
 <tr>
 <td>[discovery]</td>
 <td><code class="docutils literal notranslate">v8.0.0 -> 8.0.0</code></td>
 <tr>
 <td>[manual]</td>
 <td><code class="docutils literal notranslate">v8.0.0 -> 8.0.0</code></td>
 </table>
 </div>
 </li>
        <li> <span class="li-head">user_attr_name</span> - Which field in ID token is username. <span class="li-normal">type: str</span> <span class="li-normal">choices: email, sub, preferred_username</span>
 <a id='label28' href="javascript:ContentClick('label29', 'label28');" onmouseover="ContentPreview('label29');" onmouseout="ContentUnpreview('label29');" title="click to collapse or expand..."> more... </a>
 <div id="label29" style="display:none">
 <table border="1">
 <tr>
 <td></td>
 <td colspan="1">Supported Version Ranges</td>
 </tr>
 <tr>
 <td>user_attr_name</td>
 <td><code class="docutils literal notranslate">v8.0.0 -> 8.0.0 </code></td>
 </tr>
 <tr>
 <td>[email]</td>
 <td><code class="docutils literal notranslate">v8.0.0 -> 8.0.0</code></td>
 <tr>
 <td>[sub]</td>
 <td><code class="docutils literal notranslate">v8.0.0 -> 8.0.0</code></td>
 <tr>
 <td>[preferred_username]</td>
 <td><code class="docutils literal notranslate">v8.0.0 -> 8.0.0</code></td>
 </table>
 </div>
 </li>
        <li> <span class="li-head">user_regex</span> - username must match this regex (case insensitive). <span class="li-normal">type: str</span>
 <a id='label30' href="javascript:ContentClick('label31', 'label30');" onmouseover="ContentPreview('label31');" onmouseout="ContentUnpreview('label31');" title="click to collapse or expand..."> more... </a>
 <div id="label31" style="display:none">
 <table border="1">
 <tr>
 <td></td>
 <td colspan="1">Supported Version Ranges</td>
 </tr>
 <tr>
 <td>user_regex</td>
 <td><code class="docutils literal notranslate">v8.0.0 -> 8.0.0 </code></td>
 </tr>
 </table>
 </div>
 </li>
        <li> <span class="li-head">verify_issuer</span> - Verify issuer in ID token . <span class="li-normal">type: str</span> <span class="li-normal">choices: enable, disable</span>
 <a id='label32' href="javascript:ContentClick('label33', 'label32');" onmouseover="ContentPreview('label33');" onmouseout="ContentUnpreview('label33');" title="click to collapse or expand..."> more... </a>
 <div id="label33" style="display:none">
 <table border="1">
 <tr>
 <td></td>
 <td colspan="1">Supported Version Ranges</td>
 </tr>
 <tr>
 <td>verify_issuer</td>
 <td><code class="docutils literal notranslate">v8.0.0 -> 8.0.0 </code></td>
 </tr>
 <tr>
 <td>[enable]</td>
 <td><code class="docutils literal notranslate">v8.0.0 -> 8.0.0</code></td>
 <tr>
 <td>[disable]</td>
 <td><code class="docutils literal notranslate">v8.0.0 -> 8.0.0</code></td>
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
    
    - name: OpenID Connect server entry configuration.
      fortinet.fortios.fortios_user_oidc:
          vdom: "{{ vdom }}"
          state: "present"
          access_token: "<your_own_value>"
          user_oidc:
              authorization_url: "<your_own_value>"
              client_id: "<your_own_value>"
              client_secret: "<your_own_value>"
              clock_tolerance: "15"
              discovery_url: "<your_own_value>"
              domain_hint: "<your_own_value>"
              issuer: "<your_own_value>"
              jwks_uri: "<your_own_value>"
              ldap_server:
                  -
                      name: "default_name_12 (source user.ldap.name)"
              name: "default_name_13"
              token_url: "<your_own_value>"
              type: "discovery"
              user_attr_name: "email"
              user_regex: "<your_own_value>"
              verify_issuer: "enable"


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
