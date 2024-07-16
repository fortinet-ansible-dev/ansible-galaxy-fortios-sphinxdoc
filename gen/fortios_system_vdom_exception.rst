:source: fortios_system_vdom_exception.py

:orphan:

.. fortios_system_vdom_exception:

fortios_system_vdom_exception -- Global configuration objects that can be configured independently across different ha peers for all VDOMs or for the defined VDOM scope in Fortinet's FortiOS and FortiGate.
+++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++

.. versionadded:: 2.0.0

.. contents::
   :local:
   :depth: 1


Synopsis
--------
- This module is able to configure a FortiGate or FortiOS (FOS) device by allowing the user to set and modify system feature and vdom_exception category. Examples include all parameters and values need to be adjusted to datasources before usage. Tested with FOS v6.0.0



Requirements
------------
The below requirements are needed on the host that executes this module.

- ansible>=2.15


Tips
----
Using member operation to add an element to an existing object.

FortiOS Version Compatibility
-----------------------------
Supported Version Ranges: v6.0.0 -> v7.4.4


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
    <li> <span class="li-head">system_vdom_exception</span> - Global configuration objects that can be configured independently across different ha peers for all VDOMs or for the defined VDOM scope. <span class="li-normal">type: dict</span>
 <a id='label0' href="javascript:ContentClick('label1', 'label0');" onmouseover="ContentPreview('label1');" onmouseout="ContentUnpreview('label1');" title="click to collapse or expand..."> more... </a>
 <div id="label1" style="display:none">
 <table border="1">
 <tr>
 <td></td><td colspan="1">Supported Version Ranges</td>
 </tr>
 <tr>
 <td>system_vdom_exception</td>
 <td><code class="docutils literal notranslate">v6.0.0 -> 7.4.4 </code></td>
 </tr>
 </table>
 </div>
 </li>
        <ul class="ul-self">
        <li> <span class="li-head">id</span> - Index (1 - 4096). see <a href='#notes'>Notes</a>. <span class="li-normal">type: int</span> <span class="li-required">required: true</span>
 <a id='label2' href="javascript:ContentClick('label3', 'label2');" onmouseover="ContentPreview('label3');" onmouseout="ContentUnpreview('label3');" title="click to collapse or expand..."> more... </a>
 <div id="label3" style="display:none">
 <table border="1">
 <tr>
 <td></td>
 <td colspan="1">Supported Version Ranges</td>
 </tr>
 <tr>
 <td>id</td>
 <td><code class="docutils literal notranslate">v6.0.0 -> 7.4.4 </code></td>
 </tr>
 </table>
 </div>
 </li>
        <li> <span class="li-head">object</span> - Name of the configuration object that can be configured independently for all VDOMs. <span class="li-normal">type: str</span> <span class="li-normal">choices: log.fortianalyzer.setting, log.fortianalyzer.override-setting, log.fortianalyzer2.setting, log.fortianalyzer2.override-setting, log.fortianalyzer3.setting, log.fortianalyzer3.override-setting, log.fortianalyzer-cloud.setting, log.fortianalyzer-cloud.override-setting, log.syslogd.setting, log.syslogd.override-setting, log.syslogd2.setting, log.syslogd2.override-setting, log.syslogd3.setting, log.syslogd3.override-setting, log.syslogd4.setting, log.syslogd4.override-setting, system.gre-tunnel, system.central-management, system.csf, user.radius, system.interface, vpn.ipsec.phase1-interface, vpn.ipsec.phase2-interface, router.bgp, router.route-map, router.prefix-list, firewall.ippool, firewall.ippool6, router.static, router.static6, firewall.vip, firewall.vip6, system.sdwan, system.saml, router.policy, router.policy6, log.syslogd.setting, log.syslogd.override-setting, firewall.address, firewall.vip46, firewall.vip64</span>
 <a id='label4' href="javascript:ContentClick('label5', 'label4');" onmouseover="ContentPreview('label5');" onmouseout="ContentUnpreview('label5');" title="click to collapse or expand..."> more... </a>
 <div id="label5" style="display:none">
 <table border="1">
 <tr>
 <td></td>
 <td colspan="1">Supported Version Ranges</td>
 </tr>
 <tr>
 <td>object</td>
 <td><code class="docutils literal notranslate">v6.0.0 -> 7.4.4 </code></td>
 </tr>
 <tr>
 <td>[log.fortianalyzer.setting]</td>
 <td><code class="docutils literal notranslate">v6.0.0 -> 7.4.4</code></td>
 <tr>
 <td>[log.fortianalyzer.override-setting]</td>
 <td><code class="docutils literal notranslate">v6.0.0 -> 7.4.4</code></td>
 <tr>
 <td>[log.fortianalyzer2.setting]</td>
 <td><code class="docutils literal notranslate">v6.0.0 -> v6.0.0</code></td>
 <td><code class="docutils literal notranslate">v6.0.11 -> 7.4.4</code></td>
 </tr>
 <tr>
 <td>[log.fortianalyzer2.override-setting]</td>
 <td><code class="docutils literal notranslate">v6.0.0 -> v6.0.0</code></td>
 <td><code class="docutils literal notranslate">v6.0.11 -> 7.4.4</code></td>
 </tr>
 <tr>
 <td>[log.fortianalyzer3.setting]</td>
 <td><code class="docutils literal notranslate">v6.0.0 -> v6.0.0</code></td>
 <td><code class="docutils literal notranslate">v6.0.11 -> 7.4.4</code></td>
 </tr>
 <tr>
 <td>[log.fortianalyzer3.override-setting]</td>
 <td><code class="docutils literal notranslate">v6.0.0 -> v6.0.0</code></td>
 <td><code class="docutils literal notranslate">v6.0.11 -> 7.4.4</code></td>
 </tr>
 <tr>
 <td>[log.fortianalyzer-cloud.setting]</td>
 <td><code class="docutils literal notranslate">v6.2.0 -> 7.4.4</code></td>
 </tr>
 <tr>
 <td>[log.fortianalyzer-cloud.override-setting]</td>
 <td><code class="docutils literal notranslate">v6.2.0 -> 7.4.4</code></td>
 </tr>
 <tr>
 <td>[log.syslogd.setting]</td>
 <td><code class="docutils literal notranslate">v6.4.0 -> 7.4.4</code></td>
 </tr>
 <tr>
 <td>[log.syslogd.override-setting]</td>
 <td><code class="docutils literal notranslate">v6.4.0 -> 7.4.4</code></td>
 </tr>
 <tr>
 <td>[log.syslogd2.setting]</td>
 <td><code class="docutils literal notranslate">v6.4.0 -> 7.4.4</code></td>
 </tr>
 <tr>
 <td>[log.syslogd2.override-setting]</td>
 <td><code class="docutils literal notranslate">v6.4.0 -> 7.4.4</code></td>
 </tr>
 <tr>
 <td>[log.syslogd3.setting]</td>
 <td><code class="docutils literal notranslate">v6.4.0 -> 7.4.4</code></td>
 </tr>
 <tr>
 <td>[log.syslogd3.override-setting]</td>
 <td><code class="docutils literal notranslate">v6.4.0 -> 7.4.4</code></td>
 </tr>
 <tr>
 <td>[log.syslogd4.setting]</td>
 <td><code class="docutils literal notranslate">v6.4.0 -> 7.4.4</code></td>
 </tr>
 <tr>
 <td>[log.syslogd4.override-setting]</td>
 <td><code class="docutils literal notranslate">v6.4.0 -> 7.4.4</code></td>
 </tr>
 <tr>
 <td>[system.gre-tunnel]</td>
 <td><code class="docutils literal notranslate">v7.0.1 -> 7.4.4</code></td>
 </tr>
 <tr>
 <td>[system.central-management]</td>
 <td><code class="docutils literal notranslate">v6.0.0 -> v6.0.0</code></td>
 <td><code class="docutils literal notranslate">v6.0.11 -> 7.4.4</code></td>
 </tr>
 <tr>
 <td>[system.csf]</td>
 <td><code class="docutils literal notranslate">v6.0.0 -> v6.0.0</code></td>
 <td><code class="docutils literal notranslate">v6.0.11 -> 7.4.4</code></td>
 </tr>
 <tr>
 <td>[user.radius]</td>
 <td><code class="docutils literal notranslate">v6.0.0 -> v6.0.0</code></td>
 <td><code class="docutils literal notranslate">v6.0.11 -> 7.4.4</code></td>
 </tr>
 <tr>
 <td>[system.interface]</td>
 </tr>
 <tr>
 <td>[vpn.ipsec.phase1-interface]</td>
 </tr>
 <tr>
 <td>[vpn.ipsec.phase2-interface]</td>
 </tr>
 <tr>
 <td>[router.bgp]</td>
 </tr>
 <tr>
 <td>[router.route-map]</td>
 </tr>
 <tr>
 <td>[router.prefix-list]</td>
 </tr>
 <tr>
 <td>[firewall.ippool]</td>
 </tr>
 <tr>
 <td>[firewall.ippool6]</td>
 </tr>
 <tr>
 <td>[router.static]</td>
 </tr>
 <tr>
 <td>[router.static6]</td>
 </tr>
 <tr>
 <td>[firewall.vip]</td>
 </tr>
 <tr>
 <td>[firewall.vip6]</td>
 </tr>
 <tr>
 <td>[system.sdwan]</td>
 </tr>
 <tr>
 <td>[system.saml]</td>
 </tr>
 <tr>
 <td>[router.policy]</td>
 </tr>
 <tr>
 <td>[router.policy6]</td>
 </tr>
 <tr>
 <td>[log.syslogd.setting]</td>
 <td><code class="docutils literal notranslate">v7.4.4 -> 7.4.4</code></td>
 </tr>
 <tr>
 <td>[log.syslogd.override-setting]</td>
 <td><code class="docutils literal notranslate">v7.4.4 -> 7.4.4</code></td>
 </tr>
 <tr>
 <td>[firewall.address]</td>
 <td><code class="docutils literal notranslate">v7.4.2 -> 7.4.4</code></td>
 </tr>
 <tr>
 <td>[firewall.vip46]</td>
 </tr>
 <tr>
 <td>[firewall.vip64]</td>
 </tr>
 </table>
 </div>
 </li>
        <li> <span class="li-head">oid</span> - Object ID. <span class="li-normal">type: int</span>
 <a id='label6' href="javascript:ContentClick('label7', 'label6');" onmouseover="ContentPreview('label7');" onmouseout="ContentUnpreview('label7');" title="click to collapse or expand..."> more... </a>
 <div id="label7" style="display:none">
 <table border="1">
 <tr>
 <td></td>
 <td colspan="2">Supported Version Ranges</td>
 </tr>
 <tr>
 <td>oid</td>
 <td><code class="docutils literal notranslate">v6.0.0 -> v6.0.11 </code></td>
 <td><code class="docutils literal notranslate">v6.2.3 -> v6.2.3 </code></td>
 </tr>
 </table>
 </div>
 </li>
        <li> <span class="li-head">scope</span> - Determine whether the configuration object can be configured separately for all VDOMs or if some VDOMs share the same configuration. <span class="li-normal">type: str</span> <span class="li-normal">choices: all, inclusive, exclusive</span>
 <a id='label8' href="javascript:ContentClick('label9', 'label8');" onmouseover="ContentPreview('label9');" onmouseout="ContentUnpreview('label9');" title="click to collapse or expand..."> more... </a>
 <div id="label9" style="display:none">
 <table border="1">
 <tr>
 <td></td>
 <td colspan="1">Supported Version Ranges</td>
 </tr>
 <tr>
 <td>scope</td>
 <td><code class="docutils literal notranslate">v6.0.0 -> 7.4.4 </code></td>
 </tr>
 <tr>
 <td>[all]</td>
 <td><code class="docutils literal notranslate">v6.0.0 -> 7.4.4</code></td>
 <tr>
 <td>[inclusive]</td>
 <td><code class="docutils literal notranslate">v6.0.0 -> 7.4.4</code></td>
 <tr>
 <td>[exclusive]</td>
 <td><code class="docutils literal notranslate">v6.0.0 -> 7.4.4</code></td>
 </table>
 </div>
 </li>
        <li> <span class="li-head">vdom</span> - Names of the VDOMs. <span class="li-normal">type: list</span> <span style="font-family:'Courier New'" class="li-required">member_path: vdom:name</span>
 <a id='label10' href="javascript:ContentClick('label11', 'label10');" onmouseover="ContentPreview('label11');" onmouseout="ContentUnpreview('label11');" title="click to collapse or expand..."> more... </a>
 <div id="label11" style="display:none">
 <table border="1">
 <tr>
 <td></td><td colspan="1">Supported Version Ranges</td>
 </tr>
 <tr>
 <td>vdom</td>
 <td><code class="docutils literal notranslate">v6.0.0 -> 7.4.4 </code></td>
 </tr>
 </table>
 </div>
 </li>
            <ul class="ul-self">
            <li> <span class="li-head">name</span> - VDOM name. Source system.vdom.name. <span class="li-normal">type: str</span> <span class="li-required">required: true</span>
 <a id='label12' href="javascript:ContentClick('label13', 'label12');" onmouseover="ContentPreview('label13');" onmouseout="ContentUnpreview('label13');" title="click to collapse or expand..."> more... </a>
 <div id="label13" style="display:none">
 <table border="1">
 <tr>
 <td></td>
 <td colspan="1">Supported Version Ranges</td>
 </tr>
 <tr>
 <td>name</td>
 <td><code class="docutils literal notranslate">v6.0.0 -> 7.4.4 </code></td>
 </tr>
 </table>
 </div>
 </li>
            </ul>
        </ul>
    </ul>


Notes
-----

.. note::

   - We highly recommend using your own value as the id instead of 0, while '0' is a special placeholder that allows the backend to assign the latest available number for the object, it does have limitations. Please find more details in Q&A.

   - Legacy fortiosapi has been deprecated, httpapi is the preferred way to run playbooks

   - The module supports check_mode.



Examples
--------

.. code-block:: yaml+jinja
    
    - name: Global configuration objects that can be configured independently across different ha peers for all VDOMs or for the defined VDOM scope.
      fortinet.fortios.fortios_system_vdom_exception:
          vdom: "{{ vdom }}"
          state: "present"
          access_token: "<your_own_value>"
          system_vdom_exception:
              id: "3"
              object: "log.fortianalyzer.setting"
              oid: "32767"
              scope: "all"
              vdom:
                  -
                      name: "default_name_8 (source system.vdom.name)"


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
