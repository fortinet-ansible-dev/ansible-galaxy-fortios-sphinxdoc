:source: fortios_system_replacemsg_mm7.py

:orphan:

.. fortios_system_replacemsg_mm7:

fortios_system_replacemsg_mm7 -- Replacement messages in Fortinet's FortiOS and FortiGate.
++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++

.. versionadded:: 2.0.0

.. contents::
   :local:
   :depth: 1


Synopsis
--------
- This module is able to configure a FortiGate or FortiOS (FOS) device by allowing the user to set and modify system_replacemsg feature and mm7 category. Examples include all parameters and values need to be adjusted to datasources before usage. Tested with FOS v6.0.0



Requirements
------------
The below requirements are needed on the host that executes this module.

- ansible>=2.15


Tips
----
Using member operation to add an element to an existing object.

FortiOS Version Compatibility
-----------------------------
Supported Version Ranges: v6.0.0 -> v6.2.7


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
    <li> <span class="li-head">system_replacemsg_mm7</span> - Replacement messages. <span class="li-normal">type: dict</span>
 <a id='label0' href="javascript:ContentClick('label1', 'label0');" onmouseover="ContentPreview('label1');" onmouseout="ContentUnpreview('label1');" title="click to collapse or expand..."> more... </a>
 <div id="label1" style="display:none">
 <table border="1">
 <tr>
 <td></td><td colspan="1">Supported Version Ranges</td>
 </tr>
 <tr>
 <td>system_replacemsg_mm7</td>
 <td><code class="docutils literal notranslate">v6.0.0 -> v6.2.7 </code></td>
 </tr>
 </table>
 </div>
 </li>
        <ul class="ul-self">
        <li> <span class="li-head">add_smil</span> - add message encapsulation <span class="li-normal">type: str</span> <span class="li-normal">choices: enable, disable</span>
 <a id='label2' href="javascript:ContentClick('label3', 'label2');" onmouseover="ContentPreview('label3');" onmouseout="ContentUnpreview('label3');" title="click to collapse or expand..."> more... </a>
 <div id="label3" style="display:none">
 <table border="1">
 <tr>
 <td></td>
 <td colspan="1">Supported Version Ranges</td>
 </tr>
 <tr>
 <td>add_smil</td>
 <td><code class="docutils literal notranslate">v6.0.0 -> v6.2.7 </code></td>
 </tr>
 <tr>
 <td>[enable]</td>
 <td><code class="docutils literal notranslate">v6.0.0 -> v6.2.7</code></td>
 <tr>
 <td>[disable]</td>
 <td><code class="docutils literal notranslate">v6.0.0 -> v6.2.7</code></td>
 </table>
 </div>
 </li>
        <li> <span class="li-head">addr_type</span> - from address type <span class="li-normal">type: str</span> <span class="li-normal">choices: rfc2822-addr, number, short-code</span>
 <a id='label4' href="javascript:ContentClick('label5', 'label4');" onmouseover="ContentPreview('label5');" onmouseout="ContentUnpreview('label5');" title="click to collapse or expand..."> more... </a>
 <div id="label5" style="display:none">
 <table border="1">
 <tr>
 <td></td>
 <td colspan="1">Supported Version Ranges</td>
 </tr>
 <tr>
 <td>addr_type</td>
 <td><code class="docutils literal notranslate">v6.0.0 -> v6.2.7 </code></td>
 </tr>
 <tr>
 <td>[rfc2822-addr]</td>
 <td><code class="docutils literal notranslate">v6.0.0 -> v6.2.7</code></td>
 <tr>
 <td>[number]</td>
 <td><code class="docutils literal notranslate">v6.0.0 -> v6.2.7</code></td>
 <tr>
 <td>[short-code]</td>
 <td><code class="docutils literal notranslate">v6.0.0 -> v6.2.7</code></td>
 </table>
 </div>
 </li>
        <li> <span class="li-head">allow_content_adaptation</span> - allow content adaptations <span class="li-normal">type: str</span> <span class="li-normal">choices: enable, disable</span>
 <a id='label6' href="javascript:ContentClick('label7', 'label6');" onmouseover="ContentPreview('label7');" onmouseout="ContentUnpreview('label7');" title="click to collapse or expand..."> more... </a>
 <div id="label7" style="display:none">
 <table border="1">
 <tr>
 <td></td>
 <td colspan="1">Supported Version Ranges</td>
 </tr>
 <tr>
 <td>allow_content_adaptation</td>
 <td><code class="docutils literal notranslate">v6.0.0 -> v6.2.7 </code></td>
 </tr>
 <tr>
 <td>[enable]</td>
 <td><code class="docutils literal notranslate">v6.0.0 -> v6.2.7</code></td>
 <tr>
 <td>[disable]</td>
 <td><code class="docutils literal notranslate">v6.0.0 -> v6.2.7</code></td>
 </table>
 </div>
 </li>
        <li> <span class="li-head">charset</span> - character encoding used for replacement message <span class="li-normal">type: str</span> <span class="li-normal">choices: utf-8, us-ascii</span>
 <a id='label8' href="javascript:ContentClick('label9', 'label8');" onmouseover="ContentPreview('label9');" onmouseout="ContentUnpreview('label9');" title="click to collapse or expand..."> more... </a>
 <div id="label9" style="display:none">
 <table border="1">
 <tr>
 <td></td>
 <td colspan="1">Supported Version Ranges</td>
 </tr>
 <tr>
 <td>charset</td>
 <td><code class="docutils literal notranslate">v6.0.0 -> v6.2.7 </code></td>
 </tr>
 <tr>
 <td>[utf-8]</td>
 <td><code class="docutils literal notranslate">v6.0.0 -> v6.2.7</code></td>
 <tr>
 <td>[us-ascii]</td>
 <td><code class="docutils literal notranslate">v6.0.0 -> v6.2.7</code></td>
 </table>
 </div>
 </li>
        <li> <span class="li-head">class</span> - message class <span class="li-normal">type: str</span> <span class="li-normal">choices: not-included, personal, informational, advertisement, auto</span>
 <a id='label10' href="javascript:ContentClick('label11', 'label10');" onmouseover="ContentPreview('label11');" onmouseout="ContentUnpreview('label11');" title="click to collapse or expand..."> more... </a>
 <div id="label11" style="display:none">
 <table border="1">
 <tr>
 <td></td>
 <td colspan="1">Supported Version Ranges</td>
 </tr>
 <tr>
 <td>class</td>
 <td><code class="docutils literal notranslate">v6.0.0 -> v6.2.7 </code></td>
 </tr>
 <tr>
 <td>[not-included]</td>
 <td><code class="docutils literal notranslate">v6.0.0 -> v6.2.7</code></td>
 <tr>
 <td>[personal]</td>
 <td><code class="docutils literal notranslate">v6.0.0 -> v6.2.7</code></td>
 <tr>
 <td>[informational]</td>
 <td><code class="docutils literal notranslate">v6.0.0 -> v6.2.7</code></td>
 <tr>
 <td>[advertisement]</td>
 <td><code class="docutils literal notranslate">v6.0.0 -> v6.2.7</code></td>
 <tr>
 <td>[auto]</td>
 <td><code class="docutils literal notranslate">v6.0.0 -> v6.2.7</code></td>
 </table>
 </div>
 </li>
        <li> <span class="li-head">format</span> - Format flag. <span class="li-normal">type: str</span> <span class="li-normal">choices: none, text, html, wml</span>
 <a id='label12' href="javascript:ContentClick('label13', 'label12');" onmouseover="ContentPreview('label13');" onmouseout="ContentUnpreview('label13');" title="click to collapse or expand..."> more... </a>
 <div id="label13" style="display:none">
 <table border="1">
 <tr>
 <td></td>
 <td colspan="1">Supported Version Ranges</td>
 </tr>
 <tr>
 <td>format</td>
 <td><code class="docutils literal notranslate">v6.0.0 -> v6.2.7 </code></td>
 </tr>
 <tr>
 <td>[none]</td>
 <td><code class="docutils literal notranslate">v6.0.0 -> v6.2.7</code></td>
 <tr>
 <td>[text]</td>
 <td><code class="docutils literal notranslate">v6.0.0 -> v6.2.7</code></td>
 <tr>
 <td>[html]</td>
 <td><code class="docutils literal notranslate">v6.0.0 -> v6.2.7</code></td>
 <tr>
 <td>[wml]</td>
 <td><code class="docutils literal notranslate">v6.0.0 -> v6.2.7</code></td>
 </table>
 </div>
 </li>
        <li> <span class="li-head">fos_message</span> - message text <span class="li-normal">type: str</span>
 <a id='label14' href="javascript:ContentClick('label15', 'label14');" onmouseover="ContentPreview('label15');" onmouseout="ContentUnpreview('label15');" title="click to collapse or expand..."> more... </a>
 <div id="label15" style="display:none">
 <table border="1">
 <tr>
 <td></td>
 <td colspan="1">Supported Version Ranges</td>
 </tr>
 <tr>
 <td>fos_message</td>
 <td><code class="docutils literal notranslate">v6.0.0 -> v6.2.7 </code></td>
 </tr>
 </table>
 </div>
 </li>
        <li> <span class="li-head">from</span> - from address <span class="li-normal">type: str</span>
 <a id='label16' href="javascript:ContentClick('label17', 'label16');" onmouseover="ContentPreview('label17');" onmouseout="ContentUnpreview('label17');" title="click to collapse or expand..."> more... </a>
 <div id="label17" style="display:none">
 <table border="1">
 <tr>
 <td></td>
 <td colspan="1">Supported Version Ranges</td>
 </tr>
 <tr>
 <td>from</td>
 <td><code class="docutils literal notranslate">v6.0.0 -> v6.2.7 </code></td>
 </tr>
 </table>
 </div>
 </li>
        <li> <span class="li-head">from_sender</span> - notification message sent from recipient <span class="li-normal">type: str</span> <span class="li-normal">choices: enable, disable</span>
 <a id='label18' href="javascript:ContentClick('label19', 'label18');" onmouseover="ContentPreview('label19');" onmouseout="ContentUnpreview('label19');" title="click to collapse or expand..."> more... </a>
 <div id="label19" style="display:none">
 <table border="1">
 <tr>
 <td></td>
 <td colspan="1">Supported Version Ranges</td>
 </tr>
 <tr>
 <td>from_sender</td>
 <td><code class="docutils literal notranslate">v6.0.0 -> v6.2.7 </code></td>
 </tr>
 <tr>
 <td>[enable]</td>
 <td><code class="docutils literal notranslate">v6.0.0 -> v6.2.7</code></td>
 <tr>
 <td>[disable]</td>
 <td><code class="docutils literal notranslate">v6.0.0 -> v6.2.7</code></td>
 </table>
 </div>
 </li>
        <li> <span class="li-head">header</span> - Header flag. <span class="li-normal">type: str</span> <span class="li-normal">choices: none, http, 8bit</span>
 <a id='label20' href="javascript:ContentClick('label21', 'label20');" onmouseover="ContentPreview('label21');" onmouseout="ContentUnpreview('label21');" title="click to collapse or expand..."> more... </a>
 <div id="label21" style="display:none">
 <table border="1">
 <tr>
 <td></td>
 <td colspan="1">Supported Version Ranges</td>
 </tr>
 <tr>
 <td>header</td>
 <td><code class="docutils literal notranslate">v6.0.0 -> v6.2.7 </code></td>
 </tr>
 <tr>
 <td>[none]</td>
 <td><code class="docutils literal notranslate">v6.0.0 -> v6.2.7</code></td>
 <tr>
 <td>[http]</td>
 <td><code class="docutils literal notranslate">v6.0.0 -> v6.2.7</code></td>
 <tr>
 <td>[8bit]</td>
 <td><code class="docutils literal notranslate">v6.0.0 -> v6.2.7</code></td>
 </table>
 </div>
 </li>
        <li> <span class="li-head">image</span> - Message string. Source system.replacemsg-image.name. <span class="li-normal">type: str</span>
 <a id='label22' href="javascript:ContentClick('label23', 'label22');" onmouseover="ContentPreview('label23');" onmouseout="ContentUnpreview('label23');" title="click to collapse or expand..."> more... </a>
 <div id="label23" style="display:none">
 <table border="1">
 <tr>
 <td></td>
 <td colspan="1">Supported Version Ranges</td>
 </tr>
 <tr>
 <td>image</td>
 <td><code class="docutils literal notranslate">v6.0.0 -> v6.2.7 </code></td>
 </tr>
 </table>
 </div>
 </li>
        <li> <span class="li-head">msg_type</span> - Message type. <span class="li-normal">type: str</span> <span class="li-required">required: true</span>
 <a id='label24' href="javascript:ContentClick('label25', 'label24');" onmouseover="ContentPreview('label25');" onmouseout="ContentUnpreview('label25');" title="click to collapse or expand..."> more... </a>
 <div id="label25" style="display:none">
 <table border="1">
 <tr>
 <td></td>
 <td colspan="1">Supported Version Ranges</td>
 </tr>
 <tr>
 <td>msg_type</td>
 <td><code class="docutils literal notranslate">v6.0.0 -> v6.2.7 </code></td>
 </tr>
 </table>
 </div>
 </li>
        <li> <span class="li-head">priority</span> - message priority <span class="li-normal">type: str</span> <span class="li-normal">choices: not-included, low, normal, high</span>
 <a id='label26' href="javascript:ContentClick('label27', 'label26');" onmouseover="ContentPreview('label27');" onmouseout="ContentUnpreview('label27');" title="click to collapse or expand..."> more... </a>
 <div id="label27" style="display:none">
 <table border="1">
 <tr>
 <td></td>
 <td colspan="1">Supported Version Ranges</td>
 </tr>
 <tr>
 <td>priority</td>
 <td><code class="docutils literal notranslate">v6.0.0 -> v6.2.7 </code></td>
 </tr>
 <tr>
 <td>[not-included]</td>
 <td><code class="docutils literal notranslate">v6.0.0 -> v6.2.7</code></td>
 <tr>
 <td>[low]</td>
 <td><code class="docutils literal notranslate">v6.0.0 -> v6.2.7</code></td>
 <tr>
 <td>[normal]</td>
 <td><code class="docutils literal notranslate">v6.0.0 -> v6.2.7</code></td>
 <tr>
 <td>[high]</td>
 <td><code class="docutils literal notranslate">v6.0.0 -> v6.2.7</code></td>
 </table>
 </div>
 </li>
        <li> <span class="li-head">rsp_status</span> - response status <span class="li-normal">type: str</span> <span class="li-normal">choices: success, partial-success, client-err, oper-restrict, addr-err, addr-not-found, content-refused, msg-id-not-found, link-id-not-found, msg-fmt-corrupt, app-id-not-found, repl-app-id-not-found, srv-err, not-possible, msg-rejected, multiple-addr-not-supp, app-addr-not-supp, gen-service-err, improper-ident, unsupp-ver, unsupp-oper, validation-err, service-err, service-unavail, service-denied, app-denied</span>
 <a id='label28' href="javascript:ContentClick('label29', 'label28');" onmouseover="ContentPreview('label29');" onmouseout="ContentUnpreview('label29');" title="click to collapse or expand..."> more... </a>
 <div id="label29" style="display:none">
 <table border="1">
 <tr>
 <td></td>
 <td colspan="1">Supported Version Ranges</td>
 </tr>
 <tr>
 <td>rsp_status</td>
 <td><code class="docutils literal notranslate">v6.0.0 -> v6.2.7 </code></td>
 </tr>
 <tr>
 <td>[success]</td>
 <td><code class="docutils literal notranslate">v6.0.0 -> v6.2.7</code></td>
 <tr>
 <td>[partial-success]</td>
 <td><code class="docutils literal notranslate">v6.0.0 -> v6.2.7</code></td>
 <tr>
 <td>[client-err]</td>
 <td><code class="docutils literal notranslate">v6.0.0 -> v6.2.7</code></td>
 <tr>
 <td>[oper-restrict]</td>
 <td><code class="docutils literal notranslate">v6.0.0 -> v6.2.7</code></td>
 <tr>
 <td>[addr-err]</td>
 <td><code class="docutils literal notranslate">v6.0.0 -> v6.2.7</code></td>
 <tr>
 <td>[addr-not-found]</td>
 <td><code class="docutils literal notranslate">v6.0.0 -> v6.2.7</code></td>
 <tr>
 <td>[content-refused]</td>
 <td><code class="docutils literal notranslate">v6.0.0 -> v6.2.7</code></td>
 <tr>
 <td>[msg-id-not-found]</td>
 <td><code class="docutils literal notranslate">v6.0.0 -> v6.2.7</code></td>
 <tr>
 <td>[link-id-not-found]</td>
 <td><code class="docutils literal notranslate">v6.0.0 -> v6.2.7</code></td>
 <tr>
 <td>[msg-fmt-corrupt]</td>
 <td><code class="docutils literal notranslate">v6.0.0 -> v6.2.7</code></td>
 <tr>
 <td>[app-id-not-found]</td>
 <td><code class="docutils literal notranslate">v6.0.0 -> v6.2.7</code></td>
 <tr>
 <td>[repl-app-id-not-found]</td>
 <td><code class="docutils literal notranslate">v6.0.0 -> v6.2.7</code></td>
 <tr>
 <td>[srv-err]</td>
 <td><code class="docutils literal notranslate">v6.0.0 -> v6.2.7</code></td>
 <tr>
 <td>[not-possible]</td>
 <td><code class="docutils literal notranslate">v6.0.0 -> v6.2.7</code></td>
 <tr>
 <td>[msg-rejected]</td>
 <td><code class="docutils literal notranslate">v6.0.0 -> v6.2.7</code></td>
 <tr>
 <td>[multiple-addr-not-supp]</td>
 <td><code class="docutils literal notranslate">v6.0.0 -> v6.2.7</code></td>
 <tr>
 <td>[app-addr-not-supp]</td>
 <td><code class="docutils literal notranslate">v6.0.0 -> v6.2.7</code></td>
 <tr>
 <td>[gen-service-err]</td>
 <td><code class="docutils literal notranslate">v6.0.0 -> v6.2.7</code></td>
 <tr>
 <td>[improper-ident]</td>
 <td><code class="docutils literal notranslate">v6.0.0 -> v6.2.7</code></td>
 <tr>
 <td>[unsupp-ver]</td>
 <td><code class="docutils literal notranslate">v6.0.0 -> v6.2.7</code></td>
 <tr>
 <td>[unsupp-oper]</td>
 <td><code class="docutils literal notranslate">v6.0.0 -> v6.2.7</code></td>
 <tr>
 <td>[validation-err]</td>
 <td><code class="docutils literal notranslate">v6.0.0 -> v6.2.7</code></td>
 <tr>
 <td>[service-err]</td>
 <td><code class="docutils literal notranslate">v6.0.0 -> v6.2.7</code></td>
 <tr>
 <td>[service-unavail]</td>
 <td><code class="docutils literal notranslate">v6.0.0 -> v6.2.7</code></td>
 <tr>
 <td>[service-denied]</td>
 <td><code class="docutils literal notranslate">v6.0.0 -> v6.2.7</code></td>
 <tr>
 <td>[app-denied]</td>
 <td><code class="docutils literal notranslate">v6.0.0 -> v6.2.7</code></td>
 </table>
 </div>
 </li>
        <li> <span class="li-head">smil_part</span> - message encapsulation text <span class="li-normal">type: str</span>
 <a id='label30' href="javascript:ContentClick('label31', 'label30');" onmouseover="ContentPreview('label31');" onmouseout="ContentUnpreview('label31');" title="click to collapse or expand..."> more... </a>
 <div id="label31" style="display:none">
 <table border="1">
 <tr>
 <td></td>
 <td colspan="1">Supported Version Ranges</td>
 </tr>
 <tr>
 <td>smil_part</td>
 <td><code class="docutils literal notranslate">v6.0.0 -> v6.2.7 </code></td>
 </tr>
 </table>
 </div>
 </li>
        <li> <span class="li-head">subject</span> - subject text string <span class="li-normal">type: str</span>
 <a id='label32' href="javascript:ContentClick('label33', 'label32');" onmouseover="ContentPreview('label33');" onmouseout="ContentUnpreview('label33');" title="click to collapse or expand..."> more... </a>
 <div id="label33" style="display:none">
 <table border="1">
 <tr>
 <td></td>
 <td colspan="1">Supported Version Ranges</td>
 </tr>
 <tr>
 <td>subject</td>
 <td><code class="docutils literal notranslate">v6.0.0 -> v6.2.7 </code></td>
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
    
    - name: Replacement messages.
      fortinet.fortios.fortios_system_replacemsg_mm7:
          vdom: "{{ vdom }}"
          state: "present"
          access_token: "<your_own_value>"
          system_replacemsg_mm7:
              add_smil: "enable"
              addr_type: "rfc2822-addr"
              allow_content_adaptation: "enable"
              charset: "utf-8"
              class: "not-included"
              format: "none"
              fos_message: "<your_own_value>"
              from: "<your_own_value>"
              from_sender: "enable"
              header: "none"
              image: "<your_own_value> (source system.replacemsg-image.name)"
              msg_type: "<your_own_value>"
              priority: "not-included"
              rsp_status: "success"
              smil_part: "<your_own_value>"
              subject: "<your_own_value>"


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
