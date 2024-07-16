:source: fortios_user_device.py

:orphan:

.. fortios_user_device:

fortios_user_device -- Configure devices in Fortinet's FortiOS and FortiGate.
+++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++

.. versionadded:: 2.0.0

.. contents::
   :local:
   :depth: 1


Synopsis
--------
- This module is able to configure a FortiGate or FortiOS (FOS) device by allowing the user to set and modify user feature and device category. Examples include all parameters and values need to be adjusted to datasources before usage. Tested with FOS v6.0.0



Requirements
------------
The below requirements are needed on the host that executes this module.

- ansible>=2.15


Tips
----
Using member operation to add an element to an existing object.

FortiOS Version Compatibility
-----------------------------
Supported Version Ranges: v6.0.0 -> v6.0.11, v6.2.3


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
    <li> <span class="li-head">user_device</span> - Configure devices. <span class="li-normal">type: dict</span>
 <a id='label0' href="javascript:ContentClick('label1', 'label0');" onmouseover="ContentPreview('label1');" onmouseout="ContentUnpreview('label1');" title="click to collapse or expand..."> more... </a>
 <div id="label1" style="display:none">
 <table border="1">
 <tr>
 <td></td><td colspan="2">Supported Version Ranges</td>
 </tr>
 <tr>
 <td>user_device</td>
 <td><code class="docutils literal notranslate">v6.0.0 -> v6.0.11 </code></td>
 <td><code class="docutils literal notranslate">v6.2.3 -> v6.2.3 </code></td>
 </tr>
 </table>
 </div>
 </li>
        <ul class="ul-self">
        <li> <span class="li-head">alias</span> - Device alias. <span class="li-normal">type: str</span> <span class="li-required">required: true</span>
 <a id='label2' href="javascript:ContentClick('label3', 'label2');" onmouseover="ContentPreview('label3');" onmouseout="ContentUnpreview('label3');" title="click to collapse or expand..."> more... </a>
 <div id="label3" style="display:none">
 <table border="1">
 <tr>
 <td></td>
 <td colspan="2">Supported Version Ranges</td>
 </tr>
 <tr>
 <td>alias</td>
 <td><code class="docutils literal notranslate">v6.0.0 -> v6.0.11 </code></td>
 <td><code class="docutils literal notranslate">v6.2.3 -> v6.2.3 </code></td>
 </tr>
 </table>
 </div>
 </li>
        <li> <span class="li-head">avatar</span> - Image file for avatar (maximum 4K base64 encoded). <span class="li-normal">type: str</span>
 <a id='label4' href="javascript:ContentClick('label5', 'label4');" onmouseover="ContentPreview('label5');" onmouseout="ContentUnpreview('label5');" title="click to collapse or expand..."> more... </a>
 <div id="label5" style="display:none">
 <table border="1">
 <tr>
 <td></td>
 <td colspan="2">Supported Version Ranges</td>
 </tr>
 <tr>
 <td>avatar</td>
 <td><code class="docutils literal notranslate">v6.0.0 -> v6.0.11 </code></td>
 <td><code class="docutils literal notranslate">v6.2.3 -> v6.2.3 </code></td>
 </tr>
 </table>
 </div>
 </li>
        <li> <span class="li-head">category</span> - Family. <span class="li-normal">type: str</span> <span class="li-normal">choices: none, amazon-device, android-device, blackberry-device, fortinet-device, ios-device, windows-device</span>
 <a id='label6' href="javascript:ContentClick('label7', 'label6');" onmouseover="ContentPreview('label7');" onmouseout="ContentUnpreview('label7');" title="click to collapse or expand..."> more... </a>
 <div id="label7" style="display:none">
 <table border="1">
 <tr>
 <td></td>
 <td colspan="2">Supported Version Ranges</td>
 </tr>
 <tr>
 <td>category</td>
 <td><code class="docutils literal notranslate">v6.0.0 -> v6.0.11 </code></td>
 <td><code class="docutils literal notranslate">v6.2.3 -> v6.2.3 </code></td>
 </tr>
 <tr>
 <td>[none]</td>
 <td><code class="docutils literal notranslate">v6.0.0 -> v6.0.11</code></td>
 </tr>
 <tr>
 <td>[amazon-device]</td>
 <td><code class="docutils literal notranslate">v6.0.0 -> v6.0.11</code></td>
 </tr>
 <tr>
 <td>[android-device]</td>
 <td><code class="docutils literal notranslate">v6.0.0 -> v6.0.11</code></td>
 </tr>
 <tr>
 <td>[blackberry-device]</td>
 <td><code class="docutils literal notranslate">v6.0.0 -> v6.0.11</code></td>
 </tr>
 <tr>
 <td>[fortinet-device]</td>
 <td><code class="docutils literal notranslate">v6.0.0 -> v6.0.11</code></td>
 </tr>
 <tr>
 <td>[ios-device]</td>
 <td><code class="docutils literal notranslate">v6.0.0 -> v6.0.11</code></td>
 </tr>
 <tr>
 <td>[windows-device]</td>
 <td><code class="docutils literal notranslate">v6.0.0 -> v6.0.11</code></td>
 </tr>
 </table>
 </div>
 </li>
        <li> <span class="li-head">comment</span> - Comment. <span class="li-normal">type: str</span>
 <a id='label8' href="javascript:ContentClick('label9', 'label8');" onmouseover="ContentPreview('label9');" onmouseout="ContentUnpreview('label9');" title="click to collapse or expand..."> more... </a>
 <div id="label9" style="display:none">
 <table border="1">
 <tr>
 <td></td>
 <td colspan="2">Supported Version Ranges</td>
 </tr>
 <tr>
 <td>comment</td>
 <td><code class="docutils literal notranslate">v6.0.0 -> v6.0.11 </code></td>
 <td><code class="docutils literal notranslate">v6.2.3 -> v6.2.3 </code></td>
 </tr>
 </table>
 </div>
 </li>
        <li> <span class="li-head">mac</span> - Device MAC address. <span class="li-normal">type: str</span>
 <a id='label10' href="javascript:ContentClick('label11', 'label10');" onmouseover="ContentPreview('label11');" onmouseout="ContentUnpreview('label11');" title="click to collapse or expand..."> more... </a>
 <div id="label11" style="display:none">
 <table border="1">
 <tr>
 <td></td>
 <td colspan="2">Supported Version Ranges</td>
 </tr>
 <tr>
 <td>mac</td>
 <td><code class="docutils literal notranslate">v6.0.0 -> v6.0.11 </code></td>
 <td><code class="docutils literal notranslate">v6.2.3 -> v6.2.3 </code></td>
 </tr>
 </table>
 </div>
 </li>
        <li> <span class="li-head">master_device</span> - Master device (optional). Source user.device.alias. <span class="li-normal">type: str</span>
 <a id='label12' href="javascript:ContentClick('label13', 'label12');" onmouseover="ContentPreview('label13');" onmouseout="ContentUnpreview('label13');" title="click to collapse or expand..."> more... </a>
 <div id="label13" style="display:none">
 <table border="1">
 <tr>
 <td></td>
 <td colspan="2">Supported Version Ranges</td>
 </tr>
 <tr>
 <td>master_device</td>
 <td><code class="docutils literal notranslate">v6.0.0 -> v6.0.11 </code></td>
 <td><code class="docutils literal notranslate">v6.2.3 -> v6.2.3 </code></td>
 </tr>
 </table>
 </div>
 </li>
        <li> <span class="li-head">tagging</span> - Config object tagging. <span class="li-normal">type: list</span> <span style="font-family:'Courier New'" class="li-required">member_path: tagging:name</span>
 <a id='label14' href="javascript:ContentClick('label15', 'label14');" onmouseover="ContentPreview('label15');" onmouseout="ContentUnpreview('label15');" title="click to collapse or expand..."> more... </a>
 <div id="label15" style="display:none">
 <table border="1">
 <tr>
 <td></td><td colspan="2">Supported Version Ranges</td>
 </tr>
 <tr>
 <td>tagging</td>
 <td><code class="docutils literal notranslate">v6.0.0 -> v6.0.11 </code></td>
 <td><code class="docutils literal notranslate">v6.2.3 -> v6.2.3 </code></td>
 </tr>
 </table>
 </div>
 </li>
            <ul class="ul-self">
            <li> <span class="li-head">category</span> - Tag category. Source system.object-tagging.category. <span class="li-normal">type: str</span>
 <a id='label16' href="javascript:ContentClick('label17', 'label16');" onmouseover="ContentPreview('label17');" onmouseout="ContentUnpreview('label17');" title="click to collapse or expand..."> more... </a>
 <div id="label17" style="display:none">
 <table border="1">
 <tr>
 <td></td>
 <td colspan="2">Supported Version Ranges</td>
 </tr>
 <tr>
 <td>category</td>
 <td><code class="docutils literal notranslate">v6.0.0 -> v6.0.11 </code></td>
 <td><code class="docutils literal notranslate">v6.2.3 -> v6.2.3 </code></td>
 </tr>
 </table>
 </div>
 </li>
            <li> <span class="li-head">name</span> - Tagging entry name. <span class="li-normal">type: str</span> <span class="li-required">required: true</span>
 <a id='label18' href="javascript:ContentClick('label19', 'label18');" onmouseover="ContentPreview('label19');" onmouseout="ContentUnpreview('label19');" title="click to collapse or expand..."> more... </a>
 <div id="label19" style="display:none">
 <table border="1">
 <tr>
 <td></td>
 <td colspan="2">Supported Version Ranges</td>
 </tr>
 <tr>
 <td>name</td>
 <td><code class="docutils literal notranslate">v6.0.0 -> v6.0.11 </code></td>
 <td><code class="docutils literal notranslate">v6.2.3 -> v6.2.3 </code></td>
 </tr>
 </table>
 </div>
 </li>
            <li> <span class="li-head">tags</span> - Tags. <span class="li-normal">type: list</span> <span style="font-family:'Courier New'" class="li-required">member_path: tagging:name/tags:name</span>
 <a id='label20' href="javascript:ContentClick('label21', 'label20');" onmouseover="ContentPreview('label21');" onmouseout="ContentUnpreview('label21');" title="click to collapse or expand..."> more... </a>
 <div id="label21" style="display:none">
 <table border="1">
 <tr>
 <td></td><td colspan="2">Supported Version Ranges</td>
 </tr>
 <tr>
 <td>tags</td>
 <td><code class="docutils literal notranslate">v6.0.0 -> v6.0.11 </code></td>
 <td><code class="docutils literal notranslate">v6.2.3 -> v6.2.3 </code></td>
 </tr>
 </table>
 </div>
 </li>
                <ul class="ul-self">
                <li> <span class="li-head">name</span> - Tag name. Source system.object-tagging.tags.name. <span class="li-normal">type: str</span> <span class="li-required">required: true</span>
 <a id='label22' href="javascript:ContentClick('label23', 'label22');" onmouseover="ContentPreview('label23');" onmouseout="ContentUnpreview('label23');" title="click to collapse or expand..."> more... </a>
 <div id="label23" style="display:none">
 <table border="1">
 <tr>
 <td></td>
 <td colspan="2">Supported Version Ranges</td>
 </tr>
 <tr>
 <td>name</td>
 <td><code class="docutils literal notranslate">v6.0.0 -> v6.0.11 </code></td>
 <td><code class="docutils literal notranslate">v6.2.3 -> v6.2.3 </code></td>
 </tr>
 </table>
 </div>
 </li>
                </ul>
            </ul>
        <li> <span class="li-head">type</span> - Type. <span class="li-normal">type: str</span> <span class="li-normal">choices: unknown, android-phone, android-tablet, blackberry-phone, blackberry-playbook, forticam, fortifone, fortinet-device, gaming-console, ip-phone, ipad, iphone, linux-pc, mac, media-streaming, printer, router-nat-device, windows-pc, windows-phone, windows-tablet, other-network-device</span>
 <a id='label24' href="javascript:ContentClick('label25', 'label24');" onmouseover="ContentPreview('label25');" onmouseout="ContentUnpreview('label25');" title="click to collapse or expand..."> more... </a>
 <div id="label25" style="display:none">
 <table border="1">
 <tr>
 <td></td>
 <td colspan="2">Supported Version Ranges</td>
 </tr>
 <tr>
 <td>type</td>
 <td><code class="docutils literal notranslate">v6.0.0 -> v6.0.11 </code></td>
 <td><code class="docutils literal notranslate">v6.2.3 -> v6.2.3 </code></td>
 </tr>
 <tr>
 <td>[unknown]</td>
 <td><code class="docutils literal notranslate">v6.0.0 -> v6.0.11</code></td>
 </tr>
 <tr>
 <td>[android-phone]</td>
 <td><code class="docutils literal notranslate">v6.0.0 -> v6.0.11</code></td>
 </tr>
 <tr>
 <td>[android-tablet]</td>
 <td><code class="docutils literal notranslate">v6.0.0 -> v6.0.11</code></td>
 </tr>
 <tr>
 <td>[blackberry-phone]</td>
 <td><code class="docutils literal notranslate">v6.0.0 -> v6.0.11</code></td>
 </tr>
 <tr>
 <td>[blackberry-playbook]</td>
 <td><code class="docutils literal notranslate">v6.0.0 -> v6.0.11</code></td>
 </tr>
 <tr>
 <td>[forticam]</td>
 <td><code class="docutils literal notranslate">v6.0.0 -> v6.0.11</code></td>
 </tr>
 <tr>
 <td>[fortifone]</td>
 <td><code class="docutils literal notranslate">v6.0.0 -> v6.0.11</code></td>
 </tr>
 <tr>
 <td>[fortinet-device]</td>
 <td><code class="docutils literal notranslate">v6.0.0 -> v6.0.11</code></td>
 </tr>
 <tr>
 <td>[gaming-console]</td>
 <td><code class="docutils literal notranslate">v6.0.0 -> v6.0.11</code></td>
 </tr>
 <tr>
 <td>[ip-phone]</td>
 <td><code class="docutils literal notranslate">v6.0.0 -> v6.0.11</code></td>
 </tr>
 <tr>
 <td>[ipad]</td>
 <td><code class="docutils literal notranslate">v6.0.0 -> v6.0.11</code></td>
 </tr>
 <tr>
 <td>[iphone]</td>
 <td><code class="docutils literal notranslate">v6.0.0 -> v6.0.11</code></td>
 </tr>
 <tr>
 <td>[linux-pc]</td>
 <td><code class="docutils literal notranslate">v6.0.0 -> v6.0.11</code></td>
 </tr>
 <tr>
 <td>[mac]</td>
 <td><code class="docutils literal notranslate">v6.0.0 -> v6.0.11</code></td>
 </tr>
 <tr>
 <td>[media-streaming]</td>
 <td><code class="docutils literal notranslate">v6.0.0 -> v6.0.11</code></td>
 </tr>
 <tr>
 <td>[printer]</td>
 <td><code class="docutils literal notranslate">v6.0.0 -> v6.0.11</code></td>
 </tr>
 <tr>
 <td>[router-nat-device]</td>
 <td><code class="docutils literal notranslate">v6.0.0 -> v6.0.11</code></td>
 </tr>
 <tr>
 <td>[windows-pc]</td>
 <td><code class="docutils literal notranslate">v6.0.0 -> v6.0.11</code></td>
 </tr>
 <tr>
 <td>[windows-phone]</td>
 <td><code class="docutils literal notranslate">v6.0.0 -> v6.0.11</code></td>
 </tr>
 <tr>
 <td>[windows-tablet]</td>
 <td><code class="docutils literal notranslate">v6.0.0 -> v6.0.11</code></td>
 </tr>
 <tr>
 <td>[other-network-device]</td>
 <td><code class="docutils literal notranslate">v6.0.0 -> v6.0.11</code></td>
 </tr>
 </table>
 </div>
 </li>
        <li> <span class="li-head">user</span> - User name. <span class="li-normal">type: str</span>
 <a id='label26' href="javascript:ContentClick('label27', 'label26');" onmouseover="ContentPreview('label27');" onmouseout="ContentUnpreview('label27');" title="click to collapse or expand..."> more... </a>
 <div id="label27" style="display:none">
 <table border="1">
 <tr>
 <td></td>
 <td colspan="2">Supported Version Ranges</td>
 </tr>
 <tr>
 <td>user</td>
 <td><code class="docutils literal notranslate">v6.0.0 -> v6.0.11 </code></td>
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

   - The module supports check_mode.



Examples
--------

.. code-block:: yaml+jinja
    
    - name: Configure devices.
      fortinet.fortios.fortios_user_device:
          vdom: "{{ vdom }}"
          state: "present"
          access_token: "<your_own_value>"
          user_device:
              alias: "<your_own_value>"
              avatar: "<your_own_value>"
              category: "none"
              comment: "Comment."
              mac: "<your_own_value>"
              master_device: "<your_own_value> (source user.device.alias)"
              tagging:
                  -
                      category: "<your_own_value> (source system.object-tagging.category)"
                      name: "default_name_11"
                      tags:
                          -
                              name: "default_name_13 (source system.object-tagging.tags.name)"
              type: "unknown"
              user: "<your_own_value>"


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
