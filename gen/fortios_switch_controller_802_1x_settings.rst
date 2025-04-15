:source: fortios_switch_controller_802_1x_settings.py

:orphan:

.. fortios_switch_controller_802_1x_settings:

fortios_switch_controller_802_1x_settings -- Configure global 802.1X settings in Fortinet's FortiOS and FortiGate.
++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++

.. versionadded:: 2.0.0

.. contents::
   :local:
   :depth: 1


Synopsis
--------
- This module is able to configure a FortiGate or FortiOS (FOS) device by allowing the user to set and modify switch_controller feature and 802_1x_settings category. Examples include all parameters and values need to be adjusted to datasources before usage. Tested with FOS v6.0.0



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
    <li> <span class="li-head">switch_controller_802_1x_settings</span> - Configure global 802.1X settings. <span class="li-normal">type: dict</span>
 <a id='label0' href="javascript:ContentClick('label1', 'label0');" onmouseover="ContentPreview('label1');" onmouseout="ContentUnpreview('label1');" title="click to collapse or expand..."> more... </a>
 <div id="label1" style="display:none">
 <table border="1">
 <tr>
 <td></td><td colspan="1">Supported Version Ranges</td>
 </tr>
 <tr>
 <td>switch_controller_802_1x_settings</td>
 <td><code class="docutils literal notranslate">v6.0.0 -> 7.6.2 </code></td>
 </tr>
 </table>
 </div>
 </li>
        <ul class="ul-self">
        <li> <span class="li-head">link_down_auth</span> - Interface-reauthentication state to set if a link is down. <span class="li-normal">type: str</span> <span class="li-normal">choices: set-unauth, no-action</span>
 <a id='label2' href="javascript:ContentClick('label3', 'label2');" onmouseover="ContentPreview('label3');" onmouseout="ContentUnpreview('label3');" title="click to collapse or expand..."> more... </a>
 <div id="label3" style="display:none">
 <table border="1">
 <tr>
 <td></td>
 <td colspan="1">Supported Version Ranges</td>
 </tr>
 <tr>
 <td>link_down_auth</td>
 <td><code class="docutils literal notranslate">v6.0.0 -> 7.6.2 </code></td>
 </tr>
 <tr>
 <td>[set-unauth]</td>
 <td><code class="docutils literal notranslate">v6.0.0 -> 7.6.2</code></td>
 <tr>
 <td>[no-action]</td>
 <td><code class="docutils literal notranslate">v6.0.0 -> 7.6.2</code></td>
 </table>
 </div>
 </li>
        <li> <span class="li-head">mab_reauth</span> - Enable/disable MAB re-authentication. <span class="li-normal">type: str</span> <span class="li-normal">choices: disable, enable</span>
 <a id='label4' href="javascript:ContentClick('label5', 'label4');" onmouseover="ContentPreview('label5');" onmouseout="ContentUnpreview('label5');" title="click to collapse or expand..."> more... </a>
 <div id="label5" style="display:none">
 <table border="1">
 <tr>
 <td></td>
 <td colspan="1">Supported Version Ranges</td>
 </tr>
 <tr>
 <td>mab_reauth</td>
 <td><code class="docutils literal notranslate">v7.2.0 -> 7.6.2 </code></td>
 </tr>
 <tr>
 <td>[disable]</td>
 <td><code class="docutils literal notranslate">v7.2.0 -> 7.6.2</code></td>
 <tr>
 <td>[enable]</td>
 <td><code class="docutils literal notranslate">v7.2.0 -> 7.6.2</code></td>
 </table>
 </div>
 </li>
        <li> <span class="li-head">mac_called_station_delimiter</span> - MAC called station delimiter . <span class="li-normal">type: str</span> <span class="li-normal">choices: colon, hyphen, none, single-hyphen</span>
 <a id='label6' href="javascript:ContentClick('label7', 'label6');" onmouseover="ContentPreview('label7');" onmouseout="ContentUnpreview('label7');" title="click to collapse or expand..."> more... </a>
 <div id="label7" style="display:none">
 <table border="1">
 <tr>
 <td></td>
 <td colspan="1">Supported Version Ranges</td>
 </tr>
 <tr>
 <td>mac_called_station_delimiter</td>
 <td><code class="docutils literal notranslate">v7.4.2 -> 7.6.2 </code></td>
 </tr>
 <tr>
 <td>[colon]</td>
 <td><code class="docutils literal notranslate">v7.4.2 -> 7.6.2</code></td>
 <tr>
 <td>[hyphen]</td>
 <td><code class="docutils literal notranslate">v7.4.2 -> 7.6.2</code></td>
 <tr>
 <td>[none]</td>
 <td><code class="docutils literal notranslate">v7.4.2 -> 7.6.2</code></td>
 <tr>
 <td>[single-hyphen]</td>
 <td><code class="docutils literal notranslate">v7.4.2 -> 7.6.2</code></td>
 </table>
 </div>
 </li>
        <li> <span class="li-head">mac_calling_station_delimiter</span> - MAC calling station delimiter . <span class="li-normal">type: str</span> <span class="li-normal">choices: colon, hyphen, none, single-hyphen</span>
 <a id='label8' href="javascript:ContentClick('label9', 'label8');" onmouseover="ContentPreview('label9');" onmouseout="ContentUnpreview('label9');" title="click to collapse or expand..."> more... </a>
 <div id="label9" style="display:none">
 <table border="1">
 <tr>
 <td></td>
 <td colspan="1">Supported Version Ranges</td>
 </tr>
 <tr>
 <td>mac_calling_station_delimiter</td>
 <td><code class="docutils literal notranslate">v7.4.2 -> 7.6.2 </code></td>
 </tr>
 <tr>
 <td>[colon]</td>
 <td><code class="docutils literal notranslate">v7.4.2 -> 7.6.2</code></td>
 <tr>
 <td>[hyphen]</td>
 <td><code class="docutils literal notranslate">v7.4.2 -> 7.6.2</code></td>
 <tr>
 <td>[none]</td>
 <td><code class="docutils literal notranslate">v7.4.2 -> 7.6.2</code></td>
 <tr>
 <td>[single-hyphen]</td>
 <td><code class="docutils literal notranslate">v7.4.2 -> 7.6.2</code></td>
 </table>
 </div>
 </li>
        <li> <span class="li-head">mac_case</span> - MAC case . <span class="li-normal">type: str</span> <span class="li-normal">choices: lowercase, uppercase</span>
 <a id='label10' href="javascript:ContentClick('label11', 'label10');" onmouseover="ContentPreview('label11');" onmouseout="ContentUnpreview('label11');" title="click to collapse or expand..."> more... </a>
 <div id="label11" style="display:none">
 <table border="1">
 <tr>
 <td></td>
 <td colspan="1">Supported Version Ranges</td>
 </tr>
 <tr>
 <td>mac_case</td>
 <td><code class="docutils literal notranslate">v7.4.2 -> 7.6.2 </code></td>
 </tr>
 <tr>
 <td>[lowercase]</td>
 <td><code class="docutils literal notranslate">v7.4.2 -> 7.6.2</code></td>
 <tr>
 <td>[uppercase]</td>
 <td><code class="docutils literal notranslate">v7.4.2 -> 7.6.2</code></td>
 </table>
 </div>
 </li>
        <li> <span class="li-head">mac_password_delimiter</span> - MAC authentication password delimiter . <span class="li-normal">type: str</span> <span class="li-normal">choices: colon, hyphen, none, single-hyphen</span>
 <a id='label12' href="javascript:ContentClick('label13', 'label12');" onmouseover="ContentPreview('label13');" onmouseout="ContentUnpreview('label13');" title="click to collapse or expand..."> more... </a>
 <div id="label13" style="display:none">
 <table border="1">
 <tr>
 <td></td>
 <td colspan="1">Supported Version Ranges</td>
 </tr>
 <tr>
 <td>mac_password_delimiter</td>
 <td><code class="docutils literal notranslate">v7.4.2 -> 7.6.2 </code></td>
 </tr>
 <tr>
 <td>[colon]</td>
 <td><code class="docutils literal notranslate">v7.4.2 -> 7.6.2</code></td>
 <tr>
 <td>[hyphen]</td>
 <td><code class="docutils literal notranslate">v7.4.2 -> 7.6.2</code></td>
 <tr>
 <td>[none]</td>
 <td><code class="docutils literal notranslate">v7.4.2 -> 7.6.2</code></td>
 <tr>
 <td>[single-hyphen]</td>
 <td><code class="docutils literal notranslate">v7.4.2 -> 7.6.2</code></td>
 </table>
 </div>
 </li>
        <li> <span class="li-head">mac_username_delimiter</span> - MAC authentication username delimiter . <span class="li-normal">type: str</span> <span class="li-normal">choices: colon, hyphen, none, single-hyphen</span>
 <a id='label14' href="javascript:ContentClick('label15', 'label14');" onmouseover="ContentPreview('label15');" onmouseout="ContentUnpreview('label15');" title="click to collapse or expand..."> more... </a>
 <div id="label15" style="display:none">
 <table border="1">
 <tr>
 <td></td>
 <td colspan="1">Supported Version Ranges</td>
 </tr>
 <tr>
 <td>mac_username_delimiter</td>
 <td><code class="docutils literal notranslate">v7.4.2 -> 7.6.2 </code></td>
 </tr>
 <tr>
 <td>[colon]</td>
 <td><code class="docutils literal notranslate">v7.4.2 -> 7.6.2</code></td>
 <tr>
 <td>[hyphen]</td>
 <td><code class="docutils literal notranslate">v7.4.2 -> 7.6.2</code></td>
 <tr>
 <td>[none]</td>
 <td><code class="docutils literal notranslate">v7.4.2 -> 7.6.2</code></td>
 <tr>
 <td>[single-hyphen]</td>
 <td><code class="docutils literal notranslate">v7.4.2 -> 7.6.2</code></td>
 </table>
 </div>
 </li>
        <li> <span class="li-head">max_reauth_attempt</span> - Maximum number of authentication attempts (0 - 15). <span class="li-normal">type: int</span>
 <a id='label16' href="javascript:ContentClick('label17', 'label16');" onmouseover="ContentPreview('label17');" onmouseout="ContentUnpreview('label17');" title="click to collapse or expand..."> more... </a>
 <div id="label17" style="display:none">
 <table border="1">
 <tr>
 <td></td>
 <td colspan="1">Supported Version Ranges</td>
 </tr>
 <tr>
 <td>max_reauth_attempt</td>
 <td><code class="docutils literal notranslate">v6.0.0 -> 7.6.2 </code></td>
 </tr>
 </table>
 </div>
 </li>
        <li> <span class="li-head">reauth_period</span> - Period of time to allow for reauthentication (1 - 1440 sec). <span class="li-normal">type: int</span>
 <a id='label18' href="javascript:ContentClick('label19', 'label18');" onmouseover="ContentPreview('label19');" onmouseout="ContentUnpreview('label19');" title="click to collapse or expand..."> more... </a>
 <div id="label19" style="display:none">
 <table border="1">
 <tr>
 <td></td>
 <td colspan="1">Supported Version Ranges</td>
 </tr>
 <tr>
 <td>reauth_period</td>
 <td><code class="docutils literal notranslate">v6.0.0 -> 7.6.2 </code></td>
 </tr>
 </table>
 </div>
 </li>
        <li> <span class="li-head">tx_period</span> - 802.1X Tx period (seconds). <span class="li-normal">type: int</span>
 <a id='label20' href="javascript:ContentClick('label21', 'label20');" onmouseover="ContentPreview('label21');" onmouseout="ContentUnpreview('label21');" title="click to collapse or expand..."> more... </a>
 <div id="label21" style="display:none">
 <table border="1">
 <tr>
 <td></td>
 <td colspan="1">Supported Version Ranges</td>
 </tr>
 <tr>
 <td>tx_period</td>
 <td><code class="docutils literal notranslate">v6.4.0 -> 7.6.2 </code></td>
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
    
    - name: Configure global 802.1X settings.
      fortinet.fortios.fortios_switch_controller_802_1x_settings:
          vdom: "{{ vdom }}"
          switch_controller_802_1x_settings:
              link_down_auth: "set-unauth"
              mab_reauth: "disable"
              mac_called_station_delimiter: "colon"
              mac_calling_station_delimiter: "colon"
              mac_case: "lowercase"
              mac_password_delimiter: "colon"
              mac_username_delimiter: "colon"
              max_reauth_attempt: "3"
              reauth_period: "60"
              tx_period: "30"


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
