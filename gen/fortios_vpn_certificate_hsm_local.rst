:source: fortios_vpn_certificate_hsm_local.py

:orphan:

.. fortios_vpn_certificate_hsm_local:

fortios_vpn_certificate_hsm_local -- Local certificates whose keys are stored on HSM in Fortinet's FortiOS and FortiGate.
+++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++

.. versionadded:: 2.0.0

.. contents::
   :local:
   :depth: 1


Synopsis
--------
- This module is able to configure a FortiGate or FortiOS (FOS) device by allowing the user to set and modify vpn_certificate feature and hsm_local category. Examples include all parameters and values need to be adjusted to datasources before usage. Tested with FOS v6.0.0



Requirements
------------
The below requirements are needed on the host that executes this module.

- ansible>=2.15


Tips
----
Using member operation to add an element to an existing object.

FortiOS Version Compatibility
-----------------------------
Supported Version Ranges: v7.6.3 -> v7.6.4


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
    <li> <span class="li-head">vpn_certificate_hsm_local</span> - Local certificates whose keys are stored on HSM. <span class="li-normal">type: dict</span>
 <a id='label0' href="javascript:ContentClick('label1', 'label0');" onmouseover="ContentPreview('label1');" onmouseout="ContentUnpreview('label1');" title="click to collapse or expand..."> more... </a>
 <div id="label1" style="display:none">
 <table border="1">
 <tr>
 <td></td><td colspan="1">Supported Version Ranges</td>
 </tr>
 <tr>
 <td>vpn_certificate_hsm_local</td>
 <td><code class="docutils literal notranslate">v7.6.3 -> 7.6.4 </code></td>
 </tr>
 </table>
 </div>
 </li>
        <ul class="ul-self">
        <li> <span class="li-head">api_version</span> - API version for communicating with HSM. <span class="li-normal">type: str</span> <span class="li-normal">choices: unknown, gch-default</span>
 <a id='label2' href="javascript:ContentClick('label3', 'label2');" onmouseover="ContentPreview('label3');" onmouseout="ContentUnpreview('label3');" title="click to collapse or expand..."> more... </a>
 <div id="label3" style="display:none">
 <table border="1">
 <tr>
 <td></td>
 <td colspan="1">Supported Version Ranges</td>
 </tr>
 <tr>
 <td>api_version</td>
 <td><code class="docutils literal notranslate">v7.6.3 -> 7.6.4 </code></td>
 </tr>
 <tr>
 <td>[unknown]</td>
 <td><code class="docutils literal notranslate">v7.6.3 -> 7.6.4</code></td>
 <tr>
 <td>[gch-default]</td>
 <td><code class="docutils literal notranslate">v7.6.3 -> 7.6.4</code></td>
 </table>
 </div>
 </li>
        <li> <span class="li-head">certificate</span> - PEM format certificate. <span class="li-normal">type: str</span>
 <a id='label4' href="javascript:ContentClick('label5', 'label4');" onmouseover="ContentPreview('label5');" onmouseout="ContentUnpreview('label5');" title="click to collapse or expand..."> more... </a>
 <div id="label5" style="display:none">
 <table border="1">
 <tr>
 <td></td>
 <td colspan="1">Supported Version Ranges</td>
 </tr>
 <tr>
 <td>certificate</td>
 <td><code class="docutils literal notranslate">v7.6.3 -> 7.6.4 </code></td>
 </tr>
 </table>
 </div>
 </li>
        <li> <span class="li-head">comments</span> - Comment. <span class="li-normal">type: str</span>
 <a id='label6' href="javascript:ContentClick('label7', 'label6');" onmouseover="ContentPreview('label7');" onmouseout="ContentUnpreview('label7');" title="click to collapse or expand..."> more... </a>
 <div id="label7" style="display:none">
 <table border="1">
 <tr>
 <td></td>
 <td colspan="1">Supported Version Ranges</td>
 </tr>
 <tr>
 <td>comments</td>
 <td><code class="docutils literal notranslate">v7.6.3 -> 7.6.4 </code></td>
 </tr>
 </table>
 </div>
 </li>
        <li> <span class="li-head">gch_cloud_service_name</span> - Cloud service config name to generate access token. Source system.cloud-service.name. <span class="li-normal">type: str</span>
 <a id='label8' href="javascript:ContentClick('label9', 'label8');" onmouseover="ContentPreview('label9');" onmouseout="ContentUnpreview('label9');" title="click to collapse or expand..."> more... </a>
 <div id="label9" style="display:none">
 <table border="1">
 <tr>
 <td></td>
 <td colspan="1">Supported Version Ranges</td>
 </tr>
 <tr>
 <td>gch_cloud_service_name</td>
 <td><code class="docutils literal notranslate">v7.6.3 -> 7.6.4 </code></td>
 </tr>
 </table>
 </div>
 </li>
        <li> <span class="li-head">gch_cryptokey</span> - Google Cloud HSM cryptokey. <span class="li-normal">type: str</span>
 <a id='label10' href="javascript:ContentClick('label11', 'label10');" onmouseover="ContentPreview('label11');" onmouseout="ContentUnpreview('label11');" title="click to collapse or expand..."> more... </a>
 <div id="label11" style="display:none">
 <table border="1">
 <tr>
 <td></td>
 <td colspan="1">Supported Version Ranges</td>
 </tr>
 <tr>
 <td>gch_cryptokey</td>
 <td><code class="docutils literal notranslate">v7.6.3 -> 7.6.4 </code></td>
 </tr>
 </table>
 </div>
 </li>
        <li> <span class="li-head">gch_cryptokey_algorithm</span> - Google Cloud HSM cryptokey algorithm. <span class="li-normal">type: str</span> <span class="li-normal">choices: rsa-sign-pkcs1-2048-sha256, rsa-sign-pkcs1-3072-sha256, rsa-sign-pkcs1-4096-sha256, rsa-sign-pkcs1-4096-sha512, rsa-sign-pss-2048-sha256, rsa-sign-pss-3072-sha256, rsa-sign-pss-4096-sha256, rsa-sign-pss-4096-sha512, ec-sign-p256-sha256, ec-sign-p384-sha384, ec-sign-secp256k1-sha256</span>
 <a id='label12' href="javascript:ContentClick('label13', 'label12');" onmouseover="ContentPreview('label13');" onmouseout="ContentUnpreview('label13');" title="click to collapse or expand..."> more... </a>
 <div id="label13" style="display:none">
 <table border="1">
 <tr>
 <td></td>
 <td colspan="1">Supported Version Ranges</td>
 </tr>
 <tr>
 <td>gch_cryptokey_algorithm</td>
 <td><code class="docutils literal notranslate">v7.6.3 -> 7.6.4 </code></td>
 </tr>
 <tr>
 <td>[rsa-sign-pkcs1-2048-sha256]</td>
 <td><code class="docutils literal notranslate">v7.6.3 -> 7.6.4</code></td>
 <tr>
 <td>[rsa-sign-pkcs1-3072-sha256]</td>
 <td><code class="docutils literal notranslate">v7.6.3 -> 7.6.4</code></td>
 <tr>
 <td>[rsa-sign-pkcs1-4096-sha256]</td>
 <td><code class="docutils literal notranslate">v7.6.3 -> 7.6.4</code></td>
 <tr>
 <td>[rsa-sign-pkcs1-4096-sha512]</td>
 <td><code class="docutils literal notranslate">v7.6.3 -> 7.6.4</code></td>
 <tr>
 <td>[rsa-sign-pss-2048-sha256]</td>
 <td><code class="docutils literal notranslate">v7.6.3 -> 7.6.4</code></td>
 <tr>
 <td>[rsa-sign-pss-3072-sha256]</td>
 <td><code class="docutils literal notranslate">v7.6.3 -> 7.6.4</code></td>
 <tr>
 <td>[rsa-sign-pss-4096-sha256]</td>
 <td><code class="docutils literal notranslate">v7.6.3 -> 7.6.4</code></td>
 <tr>
 <td>[rsa-sign-pss-4096-sha512]</td>
 <td><code class="docutils literal notranslate">v7.6.3 -> 7.6.4</code></td>
 <tr>
 <td>[ec-sign-p256-sha256]</td>
 <td><code class="docutils literal notranslate">v7.6.3 -> 7.6.4</code></td>
 <tr>
 <td>[ec-sign-p384-sha384]</td>
 <td><code class="docutils literal notranslate">v7.6.3 -> 7.6.4</code></td>
 <tr>
 <td>[ec-sign-secp256k1-sha256]</td>
 <td><code class="docutils literal notranslate">v7.6.3 -> 7.6.4</code></td>
 </table>
 </div>
 </li>
        <li> <span class="li-head">gch_cryptokey_version</span> - Google Cloud HSM cryptokey version. <span class="li-normal">type: str</span>
 <a id='label14' href="javascript:ContentClick('label15', 'label14');" onmouseover="ContentPreview('label15');" onmouseout="ContentUnpreview('label15');" title="click to collapse or expand..."> more... </a>
 <div id="label15" style="display:none">
 <table border="1">
 <tr>
 <td></td>
 <td colspan="1">Supported Version Ranges</td>
 </tr>
 <tr>
 <td>gch_cryptokey_version</td>
 <td><code class="docutils literal notranslate">v7.6.3 -> 7.6.4 </code></td>
 </tr>
 </table>
 </div>
 </li>
        <li> <span class="li-head">gch_keyring</span> - Google Cloud HSM keyring. <span class="li-normal">type: str</span>
 <a id='label16' href="javascript:ContentClick('label17', 'label16');" onmouseover="ContentPreview('label17');" onmouseout="ContentUnpreview('label17');" title="click to collapse or expand..."> more... </a>
 <div id="label17" style="display:none">
 <table border="1">
 <tr>
 <td></td>
 <td colspan="1">Supported Version Ranges</td>
 </tr>
 <tr>
 <td>gch_keyring</td>
 <td><code class="docutils literal notranslate">v7.6.3 -> 7.6.4 </code></td>
 </tr>
 </table>
 </div>
 </li>
        <li> <span class="li-head">gch_location</span> - Google Cloud HSM location. <span class="li-normal">type: str</span>
 <a id='label18' href="javascript:ContentClick('label19', 'label18');" onmouseover="ContentPreview('label19');" onmouseout="ContentUnpreview('label19');" title="click to collapse or expand..."> more... </a>
 <div id="label19" style="display:none">
 <table border="1">
 <tr>
 <td></td>
 <td colspan="1">Supported Version Ranges</td>
 </tr>
 <tr>
 <td>gch_location</td>
 <td><code class="docutils literal notranslate">v7.6.3 -> 7.6.4 </code></td>
 </tr>
 </table>
 </div>
 </li>
        <li> <span class="li-head">gch_project</span> - Google Cloud HSM project ID. <span class="li-normal">type: str</span>
 <a id='label20' href="javascript:ContentClick('label21', 'label20');" onmouseover="ContentPreview('label21');" onmouseout="ContentUnpreview('label21');" title="click to collapse or expand..."> more... </a>
 <div id="label21" style="display:none">
 <table border="1">
 <tr>
 <td></td>
 <td colspan="1">Supported Version Ranges</td>
 </tr>
 <tr>
 <td>gch_project</td>
 <td><code class="docutils literal notranslate">v7.6.3 -> 7.6.4 </code></td>
 </tr>
 </table>
 </div>
 </li>
        <li> <span class="li-head">name</span> - Name. <span class="li-normal">type: str</span> <span class="li-required">required: true</span>
 <a id='label22' href="javascript:ContentClick('label23', 'label22');" onmouseover="ContentPreview('label23');" onmouseout="ContentUnpreview('label23');" title="click to collapse or expand..."> more... </a>
 <div id="label23" style="display:none">
 <table border="1">
 <tr>
 <td></td>
 <td colspan="1">Supported Version Ranges</td>
 </tr>
 <tr>
 <td>name</td>
 <td><code class="docutils literal notranslate">v7.6.3 -> 7.6.4 </code></td>
 </tr>
 </table>
 </div>
 </li>
        <li> <span class="li-head">range</span> - Either a global or VDOM IP address range for the certificate. <span class="li-normal">type: str</span> <span class="li-normal">choices: global, vdom</span>
 <a id='label24' href="javascript:ContentClick('label25', 'label24');" onmouseover="ContentPreview('label25');" onmouseout="ContentUnpreview('label25');" title="click to collapse or expand..."> more... </a>
 <div id="label25" style="display:none">
 <table border="1">
 <tr>
 <td></td>
 <td colspan="1">Supported Version Ranges</td>
 </tr>
 <tr>
 <td>range</td>
 <td><code class="docutils literal notranslate">v7.6.3 -> 7.6.4 </code></td>
 </tr>
 <tr>
 <td>[global]</td>
 <td><code class="docutils literal notranslate">v7.6.3 -> 7.6.4</code></td>
 <tr>
 <td>[vdom]</td>
 <td><code class="docutils literal notranslate">v7.6.3 -> 7.6.4</code></td>
 </table>
 </div>
 </li>
        <li> <span class="li-head">source</span> - Certificate source type. <span class="li-normal">type: str</span> <span class="li-normal">choices: factory, user, bundle</span>
 <a id='label26' href="javascript:ContentClick('label27', 'label26');" onmouseover="ContentPreview('label27');" onmouseout="ContentUnpreview('label27');" title="click to collapse or expand..."> more... </a>
 <div id="label27" style="display:none">
 <table border="1">
 <tr>
 <td></td>
 <td colspan="1">Supported Version Ranges</td>
 </tr>
 <tr>
 <td>source</td>
 <td><code class="docutils literal notranslate">v7.6.3 -> 7.6.4 </code></td>
 </tr>
 <tr>
 <td>[factory]</td>
 <td><code class="docutils literal notranslate">v7.6.3 -> 7.6.4</code></td>
 <tr>
 <td>[user]</td>
 <td><code class="docutils literal notranslate">v7.6.3 -> 7.6.4</code></td>
 <tr>
 <td>[bundle]</td>
 <td><code class="docutils literal notranslate">v7.6.3 -> 7.6.4</code></td>
 </table>
 </div>
 </li>
        <li> <span class="li-head">vendor</span> - HSM vendor. <span class="li-normal">type: str</span> <span class="li-normal">choices: unknown, gch</span>
 <a id='label28' href="javascript:ContentClick('label29', 'label28');" onmouseover="ContentPreview('label29');" onmouseout="ContentUnpreview('label29');" title="click to collapse or expand..."> more... </a>
 <div id="label29" style="display:none">
 <table border="1">
 <tr>
 <td></td>
 <td colspan="1">Supported Version Ranges</td>
 </tr>
 <tr>
 <td>vendor</td>
 <td><code class="docutils literal notranslate">v7.6.3 -> 7.6.4 </code></td>
 </tr>
 <tr>
 <td>[unknown]</td>
 <td><code class="docutils literal notranslate">v7.6.3 -> 7.6.4</code></td>
 <tr>
 <td>[gch]</td>
 <td><code class="docutils literal notranslate">v7.6.3 -> 7.6.4</code></td>
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
    
    - name: Local certificates whose keys are stored on HSM.
      fortinet.fortios.fortios_vpn_certificate_hsm_local:
          vdom: "{{ vdom }}"
          state: "present"
          access_token: "<your_own_value>"
          vpn_certificate_hsm_local:
              api_version: "unknown"
              certificate: "<your_own_value>"
              comments: "<your_own_value>"
              gch_cloud_service_name: "<your_own_value> (source system.cloud-service.name)"
              gch_cryptokey: "<your_own_value>"
              gch_cryptokey_algorithm: "rsa-sign-pkcs1-2048-sha256"
              gch_cryptokey_version: "<your_own_value>"
              gch_keyring: "<your_own_value>"
              gch_location: "<your_own_value>"
              gch_project: "<your_own_value>"
              name: "default_name_13"
              range: "global"
              source: "factory"
              vendor: "unknown"


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
