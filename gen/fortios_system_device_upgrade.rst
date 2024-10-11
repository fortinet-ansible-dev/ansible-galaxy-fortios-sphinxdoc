:source: fortios_system_device_upgrade.py

:orphan:

.. fortios_system_device_upgrade:

fortios_system_device_upgrade -- Independent upgrades for managed devices in Fortinet's FortiOS and FortiGate.
++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++

.. versionadded:: 2.0.0

.. contents::
   :local:
   :depth: 1


Synopsis
--------
- This module is able to configure a FortiGate or FortiOS (FOS) device by allowing the user to set and modify system feature and device_upgrade category. Examples include all parameters and values need to be adjusted to datasources before usage. Tested with FOS v6.0.0



Requirements
------------
The below requirements are needed on the host that executes this module.

- ansible>=2.15


Tips
----
Using member operation to add an element to an existing object.

FortiOS Version Compatibility
-----------------------------
Supported Version Ranges: v7.2.4 -> v7.6.0


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
    <li> <span class="li-head">system_device_upgrade</span> - Independent upgrades for managed devices. <span class="li-normal">type: dict</span>
 <a id='label0' href="javascript:ContentClick('label1', 'label0');" onmouseover="ContentPreview('label1');" onmouseout="ContentUnpreview('label1');" title="click to collapse or expand..."> more... </a>
 <div id="label1" style="display:none">
 <table border="1">
 <tr>
 <td></td><td colspan="1">Supported Version Ranges</td>
 </tr>
 <tr>
 <td>system_device_upgrade</td>
 <td><code class="docutils literal notranslate">v7.2.4 -> 7.6.0 </code></td>
 </tr>
 </table>
 </div>
 </li>
        <ul class="ul-self">
        <li> <span class="li-head">device_type</span> - Fortinet device type. <span class="li-normal">type: str</span> <span class="li-normal">choices: fortigate, fortiswitch, fortiap, fortiextender</span>
 <a id='label2' href="javascript:ContentClick('label3', 'label2');" onmouseover="ContentPreview('label3');" onmouseout="ContentUnpreview('label3');" title="click to collapse or expand..."> more... </a>
 <div id="label3" style="display:none">
 <table border="1">
 <tr>
 <td></td>
 <td colspan="1">Supported Version Ranges</td>
 </tr>
 <tr>
 <td>device_type</td>
 <td><code class="docutils literal notranslate">v7.2.4 -> 7.6.0 </code></td>
 </tr>
 <tr>
 <td>[fortigate]</td>
 <td><code class="docutils literal notranslate">v7.4.2 -> 7.6.0</code></td>
 </tr>
 <tr>
 <td>[fortiswitch]</td>
 <td><code class="docutils literal notranslate">v7.2.4 -> 7.6.0</code></td>
 <tr>
 <td>[fortiap]</td>
 <td><code class="docutils literal notranslate">v7.2.4 -> 7.6.0</code></td>
 <tr>
 <td>[fortiextender]</td>
 <td><code class="docutils literal notranslate">v7.2.4 -> 7.6.0</code></td>
 </table>
 </div>
 </li>
        <li> <span class="li-head">failure_reason</span> - Upgrade failure reason. <span class="li-normal">type: str</span> <span class="li-normal">choices: none, internal, timeout, device-type-unsupported, download-failed, device-missing, version-unavailable, staging-failed, reboot-failed, device-not-reconnected, node-not-ready, no-final-confirmation, no-confirmation-query, config-error-log-nonempty, csf-tree-not-supported, node-failed</span>
 <a id='label4' href="javascript:ContentClick('label5', 'label4');" onmouseover="ContentPreview('label5');" onmouseout="ContentUnpreview('label5');" title="click to collapse or expand..."> more... </a>
 <div id="label5" style="display:none">
 <table border="1">
 <tr>
 <td></td>
 <td colspan="1">Supported Version Ranges</td>
 </tr>
 <tr>
 <td>failure_reason</td>
 <td><code class="docutils literal notranslate">v7.2.4 -> 7.6.0 </code></td>
 </tr>
 <tr>
 <td>[none]</td>
 <td><code class="docutils literal notranslate">v7.2.4 -> 7.6.0</code></td>
 <tr>
 <td>[internal]</td>
 <td><code class="docutils literal notranslate">v7.2.4 -> 7.6.0</code></td>
 <tr>
 <td>[timeout]</td>
 <td><code class="docutils literal notranslate">v7.2.4 -> 7.6.0</code></td>
 <tr>
 <td>[device-type-unsupported]</td>
 <td><code class="docutils literal notranslate">v7.2.4 -> 7.6.0</code></td>
 <tr>
 <td>[download-failed]</td>
 <td><code class="docutils literal notranslate">v7.2.4 -> 7.6.0</code></td>
 <tr>
 <td>[device-missing]</td>
 <td><code class="docutils literal notranslate">v7.2.4 -> 7.6.0</code></td>
 <tr>
 <td>[version-unavailable]</td>
 <td><code class="docutils literal notranslate">v7.2.4 -> 7.6.0</code></td>
 <tr>
 <td>[staging-failed]</td>
 <td><code class="docutils literal notranslate">v7.2.4 -> 7.6.0</code></td>
 <tr>
 <td>[reboot-failed]</td>
 <td><code class="docutils literal notranslate">v7.2.4 -> 7.6.0</code></td>
 <tr>
 <td>[device-not-reconnected]</td>
 <td><code class="docutils literal notranslate">v7.2.4 -> 7.6.0</code></td>
 <tr>
 <td>[node-not-ready]</td>
 <td><code class="docutils literal notranslate">v7.2.4 -> 7.6.0</code></td>
 <tr>
 <td>[no-final-confirmation]</td>
 <td><code class="docutils literal notranslate">v7.2.4 -> 7.6.0</code></td>
 <tr>
 <td>[no-confirmation-query]</td>
 <td><code class="docutils literal notranslate">v7.2.4 -> 7.6.0</code></td>
 <tr>
 <td>[config-error-log-nonempty]</td>
 <td><code class="docutils literal notranslate">v7.2.4 -> 7.6.0</code></td>
 <tr>
 <td>[csf-tree-not-supported]</td>
 <td><code class="docutils literal notranslate">v7.4.1 -> 7.6.0</code></td>
 </tr>
 <tr>
 <td>[node-failed]</td>
 <td><code class="docutils literal notranslate">v7.2.4 -> 7.6.0</code></td>
 </table>
 </div>
 </li>
        <li> <span class="li-head">ha_reboot_controller</span> - Serial number of the FortiGate unit that will control the reboot process for the federated upgrade of the HA cluster. <span class="li-normal">type: str</span>
 <a id='label6' href="javascript:ContentClick('label7', 'label6');" onmouseover="ContentPreview('label7');" onmouseout="ContentUnpreview('label7');" title="click to collapse or expand..."> more... </a>
 <div id="label7" style="display:none">
 <table border="1">
 <tr>
 <td></td>
 <td colspan="1">Supported Version Ranges</td>
 </tr>
 <tr>
 <td>ha_reboot_controller</td>
 <td><code class="docutils literal notranslate">v7.4.2 -> 7.6.0 </code></td>
 </tr>
 </table>
 </div>
 </li>
        <li> <span class="li-head">known_ha_members</span> - Known members of the HA cluster. If a member is missing at upgrade time, the upgrade will be cancelled. <span class="li-normal">type: list</span> <span style="font-family:'Courier New'" class="li-required">member_path: known_ha_members:serial</span>
 <a id='label8' href="javascript:ContentClick('label9', 'label8');" onmouseover="ContentPreview('label9');" onmouseout="ContentUnpreview('label9');" title="click to collapse or expand..."> more... </a>
 <div id="label9" style="display:none">
 <table border="1">
 <tr>
 <td></td><td colspan="1">Supported Version Ranges</td>
 </tr>
 <tr>
 <td>known_ha_members</td>
 <td><code class="docutils literal notranslate">v7.4.2 -> 7.6.0 </code></td>
 </tr>
 </table>
 </div>
 </li>
            <ul class="ul-self">
            <li> <span class="li-head">serial</span> - Serial number of HA member <span class="li-normal">type: str</span> <span class="li-required">required: true</span>
 <a id='label10' href="javascript:ContentClick('label11', 'label10');" onmouseover="ContentPreview('label11');" onmouseout="ContentUnpreview('label11');" title="click to collapse or expand..."> more... </a>
 <div id="label11" style="display:none">
 <table border="1">
 <tr>
 <td></td>
 <td colspan="1">Supported Version Ranges</td>
 </tr>
 <tr>
 <td>serial</td>
 <td><code class="docutils literal notranslate">v7.4.2 -> 7.6.0 </code></td>
 </tr>
 </table>
 </div>
 </li>
            </ul>
        <li> <span class="li-head">maximum_minutes</span> - Maximum number of minutes to allow for immediate upgrade preparation. <span class="li-normal">type: int</span>
 <a id='label12' href="javascript:ContentClick('label13', 'label12');" onmouseover="ContentPreview('label13');" onmouseout="ContentUnpreview('label13');" title="click to collapse or expand..."> more... </a>
 <div id="label13" style="display:none">
 <table border="1">
 <tr>
 <td></td>
 <td colspan="1">Supported Version Ranges</td>
 </tr>
 <tr>
 <td>maximum_minutes</td>
 <td><code class="docutils literal notranslate">v7.4.0 -> 7.6.0 </code></td>
 </tr>
 </table>
 </div>
 </li>
        <li> <span class="li-head">next_path_index</span> - The index of the next image to upgrade to. <span class="li-normal">type: int</span>
 <a id='label14' href="javascript:ContentClick('label15', 'label14');" onmouseover="ContentPreview('label15');" onmouseout="ContentUnpreview('label15');" title="click to collapse or expand..."> more... </a>
 <div id="label15" style="display:none">
 <table border="1">
 <tr>
 <td></td>
 <td colspan="1">Supported Version Ranges</td>
 </tr>
 <tr>
 <td>next_path_index</td>
 <td><code class="docutils literal notranslate">v7.6.0 -> 7.6.0 </code></td>
 </tr>
 </table>
 </div>
 </li>
        <li> <span class="li-head">serial</span> - Serial number of the node to include. <span class="li-normal">type: str</span> <span class="li-required">required: true</span>
 <a id='label16' href="javascript:ContentClick('label17', 'label16');" onmouseover="ContentPreview('label17');" onmouseout="ContentUnpreview('label17');" title="click to collapse or expand..."> more... </a>
 <div id="label17" style="display:none">
 <table border="1">
 <tr>
 <td></td>
 <td colspan="1">Supported Version Ranges</td>
 </tr>
 <tr>
 <td>serial</td>
 <td><code class="docutils literal notranslate">v7.2.4 -> 7.6.0 </code></td>
 </tr>
 </table>
 </div>
 </li>
        <li> <span class="li-head">setup_time</span> - Upgrade preparation start time in UTC (hh:mm yyyy/mm/dd UTC). <span class="li-normal">type: str</span>
 <a id='label18' href="javascript:ContentClick('label19', 'label18');" onmouseover="ContentPreview('label19');" onmouseout="ContentUnpreview('label19');" title="click to collapse or expand..."> more... </a>
 <div id="label19" style="display:none">
 <table border="1">
 <tr>
 <td></td>
 <td colspan="1">Supported Version Ranges</td>
 </tr>
 <tr>
 <td>setup_time</td>
 <td><code class="docutils literal notranslate">v7.2.4 -> 7.6.0 </code></td>
 </tr>
 </table>
 </div>
 </li>
        <li> <span class="li-head">status</span> - Current status of the upgrade. <span class="li-normal">type: str</span> <span class="li-normal">choices: disabled, initialized, downloading, device-disconnected, ready, coordinating, staging, final-check, upgrade-devices, cancelled, confirmed, done, dry-run-done, failed</span>
 <a id='label20' href="javascript:ContentClick('label21', 'label20');" onmouseover="ContentPreview('label21');" onmouseout="ContentUnpreview('label21');" title="click to collapse or expand..."> more... </a>
 <div id="label21" style="display:none">
 <table border="1">
 <tr>
 <td></td>
 <td colspan="1">Supported Version Ranges</td>
 </tr>
 <tr>
 <td>status</td>
 <td><code class="docutils literal notranslate">v7.2.4 -> 7.6.0 </code></td>
 </tr>
 <tr>
 <td>[disabled]</td>
 <td><code class="docutils literal notranslate">v7.2.4 -> 7.6.0</code></td>
 <tr>
 <td>[initialized]</td>
 <td><code class="docutils literal notranslate">v7.2.4 -> 7.6.0</code></td>
 <tr>
 <td>[downloading]</td>
 <td><code class="docutils literal notranslate">v7.2.4 -> 7.6.0</code></td>
 <tr>
 <td>[device-disconnected]</td>
 <td><code class="docutils literal notranslate">v7.2.4 -> 7.6.0</code></td>
 <tr>
 <td>[ready]</td>
 <td><code class="docutils literal notranslate">v7.2.4 -> 7.6.0</code></td>
 <tr>
 <td>[coordinating]</td>
 <td><code class="docutils literal notranslate">v7.2.4 -> 7.6.0</code></td>
 <tr>
 <td>[staging]</td>
 <td><code class="docutils literal notranslate">v7.2.4 -> 7.6.0</code></td>
 <tr>
 <td>[final-check]</td>
 <td><code class="docutils literal notranslate">v7.2.4 -> 7.6.0</code></td>
 <tr>
 <td>[upgrade-devices]</td>
 <td><code class="docutils literal notranslate">v7.2.4 -> 7.6.0</code></td>
 <tr>
 <td>[cancelled]</td>
 <td><code class="docutils literal notranslate">v7.2.4 -> 7.6.0</code></td>
 <tr>
 <td>[confirmed]</td>
 <td><code class="docutils literal notranslate">v7.2.4 -> 7.6.0</code></td>
 <tr>
 <td>[done]</td>
 <td><code class="docutils literal notranslate">v7.2.4 -> 7.6.0</code></td>
 <tr>
 <td>[dry-run-done]</td>
 <td><code class="docutils literal notranslate">v7.6.0 -> 7.6.0</code></td>
 </tr>
 <tr>
 <td>[failed]</td>
 <td><code class="docutils literal notranslate">v7.2.4 -> 7.6.0</code></td>
 </table>
 </div>
 </li>
        <li> <span class="li-head">time</span> - Scheduled upgrade execution time in UTC (hh:mm yyyy/mm/dd UTC). <span class="li-normal">type: str</span>
 <a id='label22' href="javascript:ContentClick('label23', 'label22');" onmouseover="ContentPreview('label23');" onmouseout="ContentUnpreview('label23');" title="click to collapse or expand..."> more... </a>
 <div id="label23" style="display:none">
 <table border="1">
 <tr>
 <td></td>
 <td colspan="1">Supported Version Ranges</td>
 </tr>
 <tr>
 <td>time</td>
 <td><code class="docutils literal notranslate">v7.2.4 -> 7.6.0 </code></td>
 </tr>
 </table>
 </div>
 </li>
        <li> <span class="li-head">timing</span> - Run immediately or at a scheduled time. <span class="li-normal">type: str</span> <span class="li-normal">choices: immediate, scheduled</span>
 <a id='label24' href="javascript:ContentClick('label25', 'label24');" onmouseover="ContentPreview('label25');" onmouseout="ContentUnpreview('label25');" title="click to collapse or expand..."> more... </a>
 <div id="label25" style="display:none">
 <table border="1">
 <tr>
 <td></td>
 <td colspan="1">Supported Version Ranges</td>
 </tr>
 <tr>
 <td>timing</td>
 <td><code class="docutils literal notranslate">v7.2.4 -> 7.6.0 </code></td>
 </tr>
 <tr>
 <td>[immediate]</td>
 <td><code class="docutils literal notranslate">v7.2.4 -> 7.6.0</code></td>
 <tr>
 <td>[scheduled]</td>
 <td><code class="docutils literal notranslate">v7.2.4 -> 7.6.0</code></td>
 </table>
 </div>
 </li>
        <li> <span class="li-head">upgrade_path</span> - Fortinet OS image versions to upgrade through in major-minor-patch format, such as 7-0-4. <span class="li-normal">type: str</span>
 <a id='label26' href="javascript:ContentClick('label27', 'label26');" onmouseover="ContentPreview('label27');" onmouseout="ContentUnpreview('label27');" title="click to collapse or expand..."> more... </a>
 <div id="label27" style="display:none">
 <table border="1">
 <tr>
 <td></td>
 <td colspan="1">Supported Version Ranges</td>
 </tr>
 <tr>
 <td>upgrade_path</td>
 <td><code class="docutils literal notranslate">v7.2.4 -> 7.6.0 </code></td>
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
    
    - name: Independent upgrades for managed devices.
      fortinet.fortios.fortios_system_device_upgrade:
          vdom: "{{ vdom }}"
          state: "present"
          access_token: "<your_own_value>"
          system_device_upgrade:
              device_type: "fortigate"
              failure_reason: "none"
              ha_reboot_controller: "<your_own_value>"
              known_ha_members:
                  -
                      serial: "<your_own_value>"
              maximum_minutes: "15"
              next_path_index: "0"
              serial: "<your_own_value>"
              setup_time: "<your_own_value>"
              status: "disabled"
              time: "<your_own_value>"
              timing: "immediate"
              upgrade_path: "<your_own_value>"


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
