:source: fortios_switch_controller_qos_ip_dscp_map.py

:orphan:

.. fortios_switch_controller_qos_ip_dscp_map:

fortios_switch_controller_qos_ip_dscp_map -- Configure FortiSwitch QoS IP precedence/DSCP in Fortinet's FortiOS and FortiGate.
++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++

.. versionadded:: 2.0.0

.. contents::
   :local:
   :depth: 1


Synopsis
--------
- This module is able to configure a FortiGate or FortiOS (FOS) device by allowing the user to set and modify switch_controller_qos feature and ip_dscp_map category. Examples include all parameters and values need to be adjusted to datasources before usage. Tested with FOS v6.0.0



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
    <li> <span class="li-head">switch_controller_qos_ip_dscp_map</span> - Configure FortiSwitch QoS IP precedence/DSCP. <span class="li-normal">type: dict</span>
 <a id='label0' href="javascript:ContentClick('label1', 'label0');" onmouseover="ContentPreview('label1');" onmouseout="ContentUnpreview('label1');" title="click to collapse or expand..."> more... </a>
 <div id="label1" style="display:none">
 <table border="1">
 <tr>
 <td></td><td colspan="1">Supported Version Ranges</td>
 </tr>
 <tr>
 <td>switch_controller_qos_ip_dscp_map</td>
 <td><code class="docutils literal notranslate">v6.0.0 -> 7.6.2 </code></td>
 </tr>
 </table>
 </div>
 </li>
        <ul class="ul-self">
        <li> <span class="li-head">description</span> - Description of the ip-dscp map name. <span class="li-normal">type: str</span>
 <a id='label2' href="javascript:ContentClick('label3', 'label2');" onmouseover="ContentPreview('label3');" onmouseout="ContentUnpreview('label3');" title="click to collapse or expand..."> more... </a>
 <div id="label3" style="display:none">
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
        <li> <span class="li-head">map</span> - Maps between IP-DSCP value to COS queue. <span class="li-normal">type: list</span> <span style="font-family:'Courier New'" class="li-required">member_path: map:name</span>
 <a id='label4' href="javascript:ContentClick('label5', 'label4');" onmouseover="ContentPreview('label5');" onmouseout="ContentUnpreview('label5');" title="click to collapse or expand..."> more... </a>
 <div id="label5" style="display:none">
 <table border="1">
 <tr>
 <td></td><td colspan="1">Supported Version Ranges</td>
 </tr>
 <tr>
 <td>map</td>
 <td><code class="docutils literal notranslate">v6.0.0 -> 7.6.2 </code></td>
 </tr>
 </table>
 </div>
 </li>
            <ul class="ul-self">
            <li> <span class="li-head">cos_queue</span> - COS queue number. <span class="li-normal">type: int</span>
 <a id='label6' href="javascript:ContentClick('label7', 'label6');" onmouseover="ContentPreview('label7');" onmouseout="ContentUnpreview('label7');" title="click to collapse or expand..."> more... </a>
 <div id="label7" style="display:none">
 <table border="1">
 <tr>
 <td></td>
 <td colspan="1">Supported Version Ranges</td>
 </tr>
 <tr>
 <td>cos_queue</td>
 <td><code class="docutils literal notranslate">v6.0.0 -> 7.6.2 </code></td>
 </tr>
 </table>
 </div>
 </li>
            <li> <span class="li-head">diffserv</span> - Differentiated service. <span class="li-normal">type: list</span> <span class="li-normal">choices: CS0, CS1, AF11, AF12, AF13, CS2, AF21, AF22, AF23, CS3, AF31, AF32, AF33, CS4, AF41, AF42, AF43, CS5, EF, CS6, CS7</span>
 <a id='label8' href="javascript:ContentClick('label9', 'label8');" onmouseover="ContentPreview('label9');" onmouseout="ContentUnpreview('label9');" title="click to collapse or expand..."> more... </a>
 <div id="label9" style="display:none">
 <table border="1">
 <tr>
 <td></td>
 <td colspan="1">Supported Version Ranges</td>
 </tr>
 <tr>
 <td>diffserv</td>
 <td><code class="docutils literal notranslate">v6.0.0 -> 7.6.2 </code></td>
 </tr>
 <tr>
 <td>[CS0]</td>
 <td><code class="docutils literal notranslate">v6.0.0 -> 7.6.2</code></td>
 <tr>
 <td>[CS1]</td>
 <td><code class="docutils literal notranslate">v6.0.0 -> 7.6.2</code></td>
 <tr>
 <td>[AF11]</td>
 <td><code class="docutils literal notranslate">v6.0.0 -> 7.6.2</code></td>
 <tr>
 <td>[AF12]</td>
 <td><code class="docutils literal notranslate">v6.0.0 -> 7.6.2</code></td>
 <tr>
 <td>[AF13]</td>
 <td><code class="docutils literal notranslate">v6.0.0 -> 7.6.2</code></td>
 <tr>
 <td>[CS2]</td>
 <td><code class="docutils literal notranslate">v6.0.0 -> 7.6.2</code></td>
 <tr>
 <td>[AF21]</td>
 <td><code class="docutils literal notranslate">v6.0.0 -> 7.6.2</code></td>
 <tr>
 <td>[AF22]</td>
 <td><code class="docutils literal notranslate">v6.0.0 -> 7.6.2</code></td>
 <tr>
 <td>[AF23]</td>
 <td><code class="docutils literal notranslate">v6.0.0 -> 7.6.2</code></td>
 <tr>
 <td>[CS3]</td>
 <td><code class="docutils literal notranslate">v6.0.0 -> 7.6.2</code></td>
 <tr>
 <td>[AF31]</td>
 <td><code class="docutils literal notranslate">v6.0.0 -> 7.6.2</code></td>
 <tr>
 <td>[AF32]</td>
 <td><code class="docutils literal notranslate">v6.0.0 -> 7.6.2</code></td>
 <tr>
 <td>[AF33]</td>
 <td><code class="docutils literal notranslate">v6.0.0 -> 7.6.2</code></td>
 <tr>
 <td>[CS4]</td>
 <td><code class="docutils literal notranslate">v6.0.0 -> 7.6.2</code></td>
 <tr>
 <td>[AF41]</td>
 <td><code class="docutils literal notranslate">v6.0.0 -> 7.6.2</code></td>
 <tr>
 <td>[AF42]</td>
 <td><code class="docutils literal notranslate">v6.0.0 -> 7.6.2</code></td>
 <tr>
 <td>[AF43]</td>
 <td><code class="docutils literal notranslate">v6.0.0 -> 7.6.2</code></td>
 <tr>
 <td>[CS5]</td>
 <td><code class="docutils literal notranslate">v6.0.0 -> 7.6.2</code></td>
 <tr>
 <td>[EF]</td>
 <td><code class="docutils literal notranslate">v6.0.0 -> 7.6.2</code></td>
 <tr>
 <td>[CS6]</td>
 <td><code class="docutils literal notranslate">v6.0.0 -> 7.6.2</code></td>
 <tr>
 <td>[CS7]</td>
 <td><code class="docutils literal notranslate">v6.0.0 -> 7.6.2</code></td>
 </table>
 </div>
 </li>
            <li> <span class="li-head">ip_precedence</span> - IP Precedence. <span class="li-normal">type: list</span> <span class="li-normal">choices: network-control, internetwork-control, critic-ecp, flashoverride, flash, immediate, priority, routine</span>
 <a id='label10' href="javascript:ContentClick('label11', 'label10');" onmouseover="ContentPreview('label11');" onmouseout="ContentUnpreview('label11');" title="click to collapse or expand..."> more... </a>
 <div id="label11" style="display:none">
 <table border="1">
 <tr>
 <td></td>
 <td colspan="1">Supported Version Ranges</td>
 </tr>
 <tr>
 <td>ip_precedence</td>
 <td><code class="docutils literal notranslate">v6.0.0 -> 7.6.2 </code></td>
 </tr>
 <tr>
 <td>[network-control]</td>
 <td><code class="docutils literal notranslate">v6.0.0 -> 7.6.2</code></td>
 <tr>
 <td>[internetwork-control]</td>
 <td><code class="docutils literal notranslate">v6.0.0 -> 7.6.2</code></td>
 <tr>
 <td>[critic-ecp]</td>
 <td><code class="docutils literal notranslate">v6.0.0 -> 7.6.2</code></td>
 <tr>
 <td>[flashoverride]</td>
 <td><code class="docutils literal notranslate">v6.0.0 -> 7.6.2</code></td>
 <tr>
 <td>[flash]</td>
 <td><code class="docutils literal notranslate">v6.0.0 -> 7.6.2</code></td>
 <tr>
 <td>[immediate]</td>
 <td><code class="docutils literal notranslate">v6.0.0 -> 7.6.2</code></td>
 <tr>
 <td>[priority]</td>
 <td><code class="docutils literal notranslate">v6.0.0 -> 7.6.2</code></td>
 <tr>
 <td>[routine]</td>
 <td><code class="docutils literal notranslate">v6.0.0 -> 7.6.2</code></td>
 </table>
 </div>
 </li>
            <li> <span class="li-head">name</span> - Dscp mapping entry name. <span class="li-normal">type: str</span> <span class="li-required">required: true</span>
 <a id='label12' href="javascript:ContentClick('label13', 'label12');" onmouseover="ContentPreview('label13');" onmouseout="ContentUnpreview('label13');" title="click to collapse or expand..."> more... </a>
 <div id="label13" style="display:none">
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
            <li> <span class="li-head">value</span> - Raw values of DSCP (0 - 63). <span class="li-normal">type: str</span>
 <a id='label14' href="javascript:ContentClick('label15', 'label14');" onmouseover="ContentPreview('label15');" onmouseout="ContentUnpreview('label15');" title="click to collapse or expand..."> more... </a>
 <div id="label15" style="display:none">
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
        <li> <span class="li-head">name</span> - Dscp map name. <span class="li-normal">type: str</span> <span class="li-required">required: true</span>
 <a id='label16' href="javascript:ContentClick('label17', 'label16');" onmouseover="ContentPreview('label17');" onmouseout="ContentUnpreview('label17');" title="click to collapse or expand..."> more... </a>
 <div id="label17" style="display:none">
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
    
    - name: Configure FortiSwitch QoS IP precedence/DSCP.
      fortinet.fortios.fortios_switch_controller_qos_ip_dscp_map:
          vdom: "{{ vdom }}"
          state: "present"
          access_token: "<your_own_value>"
          switch_controller_qos_ip_dscp_map:
              description: "<your_own_value>"
              map:
                  -
                      cos_queue: "0"
                      diffserv: "CS0"
                      ip_precedence: "network-control"
                      name: "default_name_8"
                      value: "<your_own_value>"
              name: "default_name_10"


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
