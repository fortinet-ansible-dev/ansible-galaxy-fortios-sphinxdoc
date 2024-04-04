:source: fortios_wireless_controller_timers.py

:orphan:

.. fortios_wireless_controller_timers:

fortios_wireless_controller_timers -- Configure CAPWAP timers in Fortinet's FortiOS and FortiGate.
++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++

.. versionadded:: 2.0.0

.. contents::
   :local:
   :depth: 1


Synopsis
--------
- This module is able to configure a FortiGate or FortiOS (FOS) device by allowing the user to set and modify wireless_controller feature and timers category. Examples include all parameters and values need to be adjusted to datasources before usage. Tested with FOS v6.0.0



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
    <li> <span class="li-head">wireless_controller_timers</span> - Configure CAPWAP timers. <span class="li-normal">type: dict</span>
 <a id='label0' href="javascript:ContentClick('label1', 'label0');" onmouseover="ContentPreview('label1');" onmouseout="ContentUnpreview('label1');" title="click to collapse or expand..."> more... </a>
 <div id="label1" style="display:none">
 <table border="1">
 <tr>
 <td></td><td colspan="1">Supported Version Ranges</td>
 </tr>
 <tr>
 <td>wireless_controller_timers</td>
 <td><code class="docutils literal notranslate">v6.0.0 -> 7.4.3 </code></td>
 </tr>
 </table>
 </div>
 </li>
        <ul class="ul-self">
        <li> <span class="li-head">ap_reboot_wait_interval1</span> - Time in minutes to wait before AP reboots when there is no controller detected (5 - 65535). <span class="li-normal">type: int</span>
 <a id='label2' href="javascript:ContentClick('label3', 'label2');" onmouseover="ContentPreview('label3');" onmouseout="ContentUnpreview('label3');" title="click to collapse or expand..."> more... </a>
 <div id="label3" style="display:none">
 <table border="1">
 <tr>
 <td></td>
 <td colspan="1">Supported Version Ranges</td>
 </tr>
 <tr>
 <td>ap_reboot_wait_interval1</td>
 <td><code class="docutils literal notranslate">v7.4.2 -> 7.4.3 </code></td>
 </tr>
 </table>
 </div>
 </li>
        <li> <span class="li-head">ap_reboot_wait_interval2</span> - Time in minutes to wait before AP reboots when there is no controller detected and standalone SSIDs are pushed to the AP in the previous session (5 - 65535). <span class="li-normal">type: int</span>
 <a id='label4' href="javascript:ContentClick('label5', 'label4');" onmouseover="ContentPreview('label5');" onmouseout="ContentUnpreview('label5');" title="click to collapse or expand..."> more... </a>
 <div id="label5" style="display:none">
 <table border="1">
 <tr>
 <td></td>
 <td colspan="1">Supported Version Ranges</td>
 </tr>
 <tr>
 <td>ap_reboot_wait_interval2</td>
 <td><code class="docutils literal notranslate">v7.4.2 -> 7.4.3 </code></td>
 </tr>
 </table>
 </div>
 </li>
        <li> <span class="li-head">ap_reboot_wait_time</span> - Time to reboot the AP when there is no controller detected and standalone SSIDs are pushed to the AP in the previous session, format hh :mm. <span class="li-normal">type: str</span>
 <a id='label6' href="javascript:ContentClick('label7', 'label6');" onmouseover="ContentPreview('label7');" onmouseout="ContentUnpreview('label7');" title="click to collapse or expand..."> more... </a>
 <div id="label7" style="display:none">
 <table border="1">
 <tr>
 <td></td>
 <td colspan="1">Supported Version Ranges</td>
 </tr>
 <tr>
 <td>ap_reboot_wait_time</td>
 <td><code class="docutils literal notranslate">v7.4.2 -> 7.4.3 </code></td>
 </tr>
 </table>
 </div>
 </li>
        <li> <span class="li-head">auth_timeout</span> - Time after which a client is considered failed in RADIUS authentication and times out (5 - 30 sec). <span class="li-normal">type: int</span>
 <a id='label8' href="javascript:ContentClick('label9', 'label8');" onmouseover="ContentPreview('label9');" onmouseout="ContentUnpreview('label9');" title="click to collapse or expand..."> more... </a>
 <div id="label9" style="display:none">
 <table border="1">
 <tr>
 <td></td>
 <td colspan="1">Supported Version Ranges</td>
 </tr>
 <tr>
 <td>auth_timeout</td>
 <td><code class="docutils literal notranslate">v7.0.6 -> 7.4.3 </code></td>
 </tr>
 </table>
 </div>
 </li>
        <li> <span class="li-head">ble_scan_report_intv</span> - Time between running Bluetooth Low Energy (BLE) reports (10 - 3600 sec). <span class="li-normal">type: int</span>
 <a id='label10' href="javascript:ContentClick('label11', 'label10');" onmouseover="ContentPreview('label11');" onmouseout="ContentUnpreview('label11');" title="click to collapse or expand..."> more... </a>
 <div id="label11" style="display:none">
 <table border="1">
 <tr>
 <td></td>
 <td colspan="1">Supported Version Ranges</td>
 </tr>
 <tr>
 <td>ble_scan_report_intv</td>
 <td><code class="docutils literal notranslate">v6.0.0 -> 7.4.3 </code></td>
 </tr>
 </table>
 </div>
 </li>
        <li> <span class="li-head">client_idle_rehome_timeout</span> - Time after which a client is considered idle and disconnected from the home controller (2 - 3600 sec). <span class="li-normal">type: int</span>
 <a id='label12' href="javascript:ContentClick('label13', 'label12');" onmouseover="ContentPreview('label13');" onmouseout="ContentUnpreview('label13');" title="click to collapse or expand..."> more... </a>
 <div id="label13" style="display:none">
 <table border="1">
 <tr>
 <td></td>
 <td colspan="1">Supported Version Ranges</td>
 </tr>
 <tr>
 <td>client_idle_rehome_timeout</td>
 <td><code class="docutils literal notranslate">v7.2.0 -> 7.4.3 </code></td>
 </tr>
 </table>
 </div>
 </li>
        <li> <span class="li-head">client_idle_timeout</span> - Time after which a client is considered idle and times out (20 - 3600 sec). <span class="li-normal">type: int</span>
 <a id='label14' href="javascript:ContentClick('label15', 'label14');" onmouseover="ContentPreview('label15');" onmouseout="ContentUnpreview('label15');" title="click to collapse or expand..."> more... </a>
 <div id="label15" style="display:none">
 <table border="1">
 <tr>
 <td></td>
 <td colspan="1">Supported Version Ranges</td>
 </tr>
 <tr>
 <td>client_idle_timeout</td>
 <td><code class="docutils literal notranslate">v6.0.0 -> 7.4.3 </code></td>
 </tr>
 </table>
 </div>
 </li>
        <li> <span class="li-head">darrp_day</span> - Weekday on which to run DARRP optimization. <span class="li-normal">type: str</span> <span class="li-normal">choices: sunday, monday, tuesday, wednesday, thursday, friday, saturday</span>
 <a id='label16' href="javascript:ContentClick('label17', 'label16');" onmouseover="ContentPreview('label17');" onmouseout="ContentUnpreview('label17');" title="click to collapse or expand..."> more... </a>
 <div id="label17" style="display:none">
 <table border="1">
 <tr>
 <td></td>
 <td colspan="1">Supported Version Ranges</td>
 </tr>
 <tr>
 <td>darrp_day</td>
 <td><code class="docutils literal notranslate">v6.0.0 -> v6.0.11 </code></td>
 </tr>
 <tr>
 <td>[sunday]</td>
 <td><code class="docutils literal notranslate">v6.0.0 -> v6.0.11</code></td>
 <tr>
 <td>[monday]</td>
 <td><code class="docutils literal notranslate">v6.0.0 -> v6.0.11</code></td>
 <tr>
 <td>[tuesday]</td>
 <td><code class="docutils literal notranslate">v6.0.0 -> v6.0.11</code></td>
 <tr>
 <td>[wednesday]</td>
 <td><code class="docutils literal notranslate">v6.0.0 -> v6.0.11</code></td>
 <tr>
 <td>[thursday]</td>
 <td><code class="docutils literal notranslate">v6.0.0 -> v6.0.11</code></td>
 <tr>
 <td>[friday]</td>
 <td><code class="docutils literal notranslate">v6.0.0 -> v6.0.11</code></td>
 <tr>
 <td>[saturday]</td>
 <td><code class="docutils literal notranslate">v6.0.0 -> v6.0.11</code></td>
 </table>
 </div>
 </li>
        <li> <span class="li-head">darrp_optimize</span> - Time for running Dynamic Automatic Radio Resource Provisioning (DARRP) optimizations (0 - 86400 sec). <span class="li-normal">type: int</span>
 <a id='label18' href="javascript:ContentClick('label19', 'label18');" onmouseover="ContentPreview('label19');" onmouseout="ContentUnpreview('label19');" title="click to collapse or expand..."> more... </a>
 <div id="label19" style="display:none">
 <table border="1">
 <tr>
 <td></td>
 <td colspan="1">Supported Version Ranges</td>
 </tr>
 <tr>
 <td>darrp_optimize</td>
 <td><code class="docutils literal notranslate">v6.0.0 -> v6.0.11 </code></td>
 </tr>
 </table>
 </div>
 </li>
        <li> <span class="li-head">darrp_time</span> - Time at which DARRP optimizations run (you can add up to 8 times). <span class="li-normal">type: list</span> <span style="font-family:'Courier New'" class="li-required">member_path: darrp_time:time</span>
 <a id='label20' href="javascript:ContentClick('label21', 'label20');" onmouseover="ContentPreview('label21');" onmouseout="ContentUnpreview('label21');" title="click to collapse or expand..."> more... </a>
 <div id="label21" style="display:none">
 <table border="1">
 <tr>
 <td></td><td colspan="1">Supported Version Ranges</td>
 </tr>
 <tr>
 <td>darrp_time</td>
 <td><code class="docutils literal notranslate">v6.0.0 -> v6.0.11 </code></td>
 </tr>
 </table>
 </div>
 </li>
            <ul class="ul-self">
            <li> <span class="li-head">time</span> - Time. <span class="li-normal">type: str</span> <span class="li-required">required: true</span>
 <a id='label22' href="javascript:ContentClick('label23', 'label22');" onmouseover="ContentPreview('label23');" onmouseout="ContentUnpreview('label23');" title="click to collapse or expand..."> more... </a>
 <div id="label23" style="display:none">
 <table border="1">
 <tr>
 <td></td>
 <td colspan="1">Supported Version Ranges</td>
 </tr>
 <tr>
 <td>time</td>
 <td><code class="docutils literal notranslate">v6.0.0 -> v6.0.11 </code></td>
 </tr>
 </table>
 </div>
 </li>
            </ul>
        <li> <span class="li-head">discovery_interval</span> - Time between discovery requests (2 - 180 sec). <span class="li-normal">type: int</span>
 <a id='label24' href="javascript:ContentClick('label25', 'label24');" onmouseover="ContentPreview('label25');" onmouseout="ContentUnpreview('label25');" title="click to collapse or expand..."> more... </a>
 <div id="label25" style="display:none">
 <table border="1">
 <tr>
 <td></td>
 <td colspan="1">Supported Version Ranges</td>
 </tr>
 <tr>
 <td>discovery_interval</td>
 <td><code class="docutils literal notranslate">v6.0.0 -> 7.4.3 </code></td>
 </tr>
 </table>
 </div>
 </li>
        <li> <span class="li-head">drma_interval</span> - Dynamic radio mode assignment (DRMA) schedule interval in minutes (10 - 1440). <span class="li-normal">type: int</span>
 <a id='label26' href="javascript:ContentClick('label27', 'label26');" onmouseover="ContentPreview('label27');" onmouseout="ContentUnpreview('label27');" title="click to collapse or expand..."> more... </a>
 <div id="label27" style="display:none">
 <table border="1">
 <tr>
 <td></td>
 <td colspan="1">Supported Version Ranges</td>
 </tr>
 <tr>
 <td>drma_interval</td>
 <td><code class="docutils literal notranslate">v6.4.4 -> 7.4.3 </code></td>
 </tr>
 </table>
 </div>
 </li>
        <li> <span class="li-head">echo_interval</span> - Time between echo requests sent by the managed WTP, AP, or FortiAP (1 - 255 sec). <span class="li-normal">type: int</span>
 <a id='label28' href="javascript:ContentClick('label29', 'label28');" onmouseover="ContentPreview('label29');" onmouseout="ContentUnpreview('label29');" title="click to collapse or expand..."> more... </a>
 <div id="label29" style="display:none">
 <table border="1">
 <tr>
 <td></td>
 <td colspan="1">Supported Version Ranges</td>
 </tr>
 <tr>
 <td>echo_interval</td>
 <td><code class="docutils literal notranslate">v6.0.0 -> 7.4.3 </code></td>
 </tr>
 </table>
 </div>
 </li>
        <li> <span class="li-head">fake_ap_log</span> - Time between recording logs about fake APs if periodic fake AP logging is configured (0 - 1440 min). <span class="li-normal">type: int</span>
 <a id='label30' href="javascript:ContentClick('label31', 'label30');" onmouseover="ContentPreview('label31');" onmouseout="ContentUnpreview('label31');" title="click to collapse or expand..."> more... </a>
 <div id="label31" style="display:none">
 <table border="1">
 <tr>
 <td></td>
 <td colspan="1">Supported Version Ranges</td>
 </tr>
 <tr>
 <td>fake_ap_log</td>
 <td><code class="docutils literal notranslate">v6.0.0 -> 7.4.3 </code></td>
 </tr>
 </table>
 </div>
 </li>
        <li> <span class="li-head">ipsec_intf_cleanup</span> - Time period to keep IPsec VPN interfaces up after WTP sessions are disconnected (30 - 3600 sec). <span class="li-normal">type: int</span>
 <a id='label32' href="javascript:ContentClick('label33', 'label32');" onmouseover="ContentPreview('label33');" onmouseout="ContentUnpreview('label33');" title="click to collapse or expand..."> more... </a>
 <div id="label33" style="display:none">
 <table border="1">
 <tr>
 <td></td>
 <td colspan="1">Supported Version Ranges</td>
 </tr>
 <tr>
 <td>ipsec_intf_cleanup</td>
 <td><code class="docutils literal notranslate">v6.0.0 -> 7.4.3 </code></td>
 </tr>
 </table>
 </div>
 </li>
        <li> <span class="li-head">nat_session_keep_alive</span> - Maximal time in seconds between control requests sent by the managed WTP, AP, or FortiAP (0 - 255 sec). <span class="li-normal">type: int</span>
 <a id='label34' href="javascript:ContentClick('label35', 'label34');" onmouseover="ContentPreview('label35');" onmouseout="ContentUnpreview('label35');" title="click to collapse or expand..."> more... </a>
 <div id="label35" style="display:none">
 <table border="1">
 <tr>
 <td></td>
 <td colspan="1">Supported Version Ranges</td>
 </tr>
 <tr>
 <td>nat_session_keep_alive</td>
 <td><code class="docutils literal notranslate">v7.4.2 -> 7.4.3 </code></td>
 </tr>
 </table>
 </div>
 </li>
        <li> <span class="li-head">radio_stats_interval</span> - Time between running radio reports (1 - 255 sec). <span class="li-normal">type: int</span>
 <a id='label36' href="javascript:ContentClick('label37', 'label36');" onmouseover="ContentPreview('label37');" onmouseout="ContentUnpreview('label37');" title="click to collapse or expand..."> more... </a>
 <div id="label37" style="display:none">
 <table border="1">
 <tr>
 <td></td>
 <td colspan="1">Supported Version Ranges</td>
 </tr>
 <tr>
 <td>radio_stats_interval</td>
 <td><code class="docutils literal notranslate">v6.0.0 -> 7.4.3 </code></td>
 </tr>
 </table>
 </div>
 </li>
        <li> <span class="li-head">rogue_ap_cleanup</span> - Time period in minutes to keep rogue AP after it is gone . <span class="li-normal">type: int</span>
 <a id='label38' href="javascript:ContentClick('label39', 'label38');" onmouseover="ContentPreview('label39');" onmouseout="ContentUnpreview('label39');" title="click to collapse or expand..."> more... </a>
 <div id="label39" style="display:none">
 <table border="1">
 <tr>
 <td></td>
 <td colspan="1">Supported Version Ranges</td>
 </tr>
 <tr>
 <td>rogue_ap_cleanup</td>
 <td><code class="docutils literal notranslate">v7.0.6 -> 7.4.3 </code></td>
 </tr>
 </table>
 </div>
 </li>
        <li> <span class="li-head">rogue_ap_log</span> - Time between logging rogue AP messages if periodic rogue AP logging is configured (0 - 1440 min). <span class="li-normal">type: int</span>
 <a id='label40' href="javascript:ContentClick('label41', 'label40');" onmouseover="ContentPreview('label41');" onmouseout="ContentUnpreview('label41');" title="click to collapse or expand..."> more... </a>
 <div id="label41" style="display:none">
 <table border="1">
 <tr>
 <td></td>
 <td colspan="1">Supported Version Ranges</td>
 </tr>
 <tr>
 <td>rogue_ap_log</td>
 <td><code class="docutils literal notranslate">v6.0.0 -> 7.4.3 </code></td>
 </tr>
 </table>
 </div>
 </li>
        <li> <span class="li-head">sta_capability_interval</span> - Time between running station capability reports (1 - 255 sec). <span class="li-normal">type: int</span>
 <a id='label42' href="javascript:ContentClick('label43', 'label42');" onmouseover="ContentPreview('label43');" onmouseout="ContentUnpreview('label43');" title="click to collapse or expand..."> more... </a>
 <div id="label43" style="display:none">
 <table border="1">
 <tr>
 <td></td>
 <td colspan="1">Supported Version Ranges</td>
 </tr>
 <tr>
 <td>sta_capability_interval</td>
 <td><code class="docutils literal notranslate">v6.0.0 -> 7.4.3 </code></td>
 </tr>
 </table>
 </div>
 </li>
        <li> <span class="li-head">sta_locate_timer</span> - Time between running client presence flushes to remove clients that are listed but no longer present (0 - 86400 sec). <span class="li-normal">type: int</span>
 <a id='label44' href="javascript:ContentClick('label45', 'label44');" onmouseover="ContentPreview('label45');" onmouseout="ContentUnpreview('label45');" title="click to collapse or expand..."> more... </a>
 <div id="label45" style="display:none">
 <table border="1">
 <tr>
 <td></td>
 <td colspan="1">Supported Version Ranges</td>
 </tr>
 <tr>
 <td>sta_locate_timer</td>
 <td><code class="docutils literal notranslate">v6.0.0 -> 7.4.3 </code></td>
 </tr>
 </table>
 </div>
 </li>
        <li> <span class="li-head">sta_stats_interval</span> - Time between running client (station) reports (1 - 255 sec). <span class="li-normal">type: int</span>
 <a id='label46' href="javascript:ContentClick('label47', 'label46');" onmouseover="ContentPreview('label47');" onmouseout="ContentUnpreview('label47');" title="click to collapse or expand..."> more... </a>
 <div id="label47" style="display:none">
 <table border="1">
 <tr>
 <td></td>
 <td colspan="1">Supported Version Ranges</td>
 </tr>
 <tr>
 <td>sta_stats_interval</td>
 <td><code class="docutils literal notranslate">v6.0.0 -> 7.4.3 </code></td>
 </tr>
 </table>
 </div>
 </li>
        <li> <span class="li-head">vap_stats_interval</span> - Time between running Virtual Access Point (VAP) reports (1 - 255 sec). <span class="li-normal">type: int</span>
 <a id='label48' href="javascript:ContentClick('label49', 'label48');" onmouseover="ContentPreview('label49');" onmouseout="ContentUnpreview('label49');" title="click to collapse or expand..."> more... </a>
 <div id="label49" style="display:none">
 <table border="1">
 <tr>
 <td></td>
 <td colspan="1">Supported Version Ranges</td>
 </tr>
 <tr>
 <td>vap_stats_interval</td>
 <td><code class="docutils literal notranslate">v6.0.0 -> 7.4.3 </code></td>
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
    
    - name: Configure CAPWAP timers.
      fortinet.fortios.fortios_wireless_controller_timers:
          vdom: "{{ vdom }}"
          wireless_controller_timers:
              ap_reboot_wait_interval1: "0"
              ap_reboot_wait_interval2: "0"
              ap_reboot_wait_time: "<your_own_value>"
              auth_timeout: "5"
              ble_scan_report_intv: "30"
              client_idle_rehome_timeout: "20"
              client_idle_timeout: "300"
              darrp_day: "sunday"
              darrp_optimize: "43200"
              darrp_time:
                  -
                      time: "<your_own_value>"
              discovery_interval: "5"
              drma_interval: "60"
              echo_interval: "30"
              fake_ap_log: "1"
              ipsec_intf_cleanup: "120"
              nat_session_keep_alive: "0"
              radio_stats_interval: "15"
              rogue_ap_cleanup: "0"
              rogue_ap_log: "0"
              sta_capability_interval: "30"
              sta_locate_timer: "1800"
              sta_stats_interval: "10"
              vap_stats_interval: "15"


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
