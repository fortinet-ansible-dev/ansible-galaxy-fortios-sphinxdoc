:source: fortios_firewall_profile_group.py

:orphan:

.. fortios_firewall_profile_group:

fortios_firewall_profile_group -- Configure profile groups in Fortinet's FortiOS and FortiGate.
+++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++

.. versionadded:: 2.0.0

.. contents::
   :local:
   :depth: 1


Synopsis
--------
- This module is able to configure a FortiGate or FortiOS (FOS) device by allowing the user to set and modify firewall feature and profile_group category. Examples include all parameters and values need to be adjusted to datasources before usage. Tested with FOS v6.0.0



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
    <li> <span class="li-head">firewall_profile_group</span> - Configure profile groups. <span class="li-normal">type: dict</span>
 <a id='label0' href="javascript:ContentClick('label1', 'label0');" onmouseover="ContentPreview('label1');" onmouseout="ContentUnpreview('label1');" title="click to collapse or expand..."> more... </a>
 <div id="label1" style="display:none">
 <table border="1">
 <tr>
 <td></td><td colspan="1">Supported Version Ranges</td>
 </tr>
 <tr>
 <td>firewall_profile_group</td>
 <td><code class="docutils literal notranslate">v6.0.0 -> 7.4.4 </code></td>
 </tr>
 </table>
 </div>
 </li>
        <ul class="ul-self">
        <li> <span class="li-head">application_list</span> - Name of an existing Application list. Source application.list.name. <span class="li-normal">type: str</span>
 <a id='label2' href="javascript:ContentClick('label3', 'label2');" onmouseover="ContentPreview('label3');" onmouseout="ContentUnpreview('label3');" title="click to collapse or expand..."> more... </a>
 <div id="label3" style="display:none">
 <table border="1">
 <tr>
 <td></td>
 <td colspan="1">Supported Version Ranges</td>
 </tr>
 <tr>
 <td>application_list</td>
 <td><code class="docutils literal notranslate">v6.0.0 -> 7.4.4 </code></td>
 </tr>
 </table>
 </div>
 </li>
        <li> <span class="li-head">av_profile</span> - Name of an existing Antivirus profile. Source antivirus.profile.name. <span class="li-normal">type: str</span>
 <a id='label4' href="javascript:ContentClick('label5', 'label4');" onmouseover="ContentPreview('label5');" onmouseout="ContentUnpreview('label5');" title="click to collapse or expand..."> more... </a>
 <div id="label5" style="display:none">
 <table border="1">
 <tr>
 <td></td>
 <td colspan="1">Supported Version Ranges</td>
 </tr>
 <tr>
 <td>av_profile</td>
 <td><code class="docutils literal notranslate">v6.0.0 -> 7.4.4 </code></td>
 </tr>
 </table>
 </div>
 </li>
        <li> <span class="li-head">casb_profile</span> - Name of an existing CASB profile. Source casb.profile.name. <span class="li-normal">type: str</span>
 <a id='label6' href="javascript:ContentClick('label7', 'label6');" onmouseover="ContentPreview('label7');" onmouseout="ContentUnpreview('label7');" title="click to collapse or expand..."> more... </a>
 <div id="label7" style="display:none">
 <table border="1">
 <tr>
 <td></td>
 <td colspan="1">Supported Version Ranges</td>
 </tr>
 <tr>
 <td>casb_profile</td>
 <td><code class="docutils literal notranslate">v7.4.1 -> 7.4.4 </code></td>
 </tr>
 </table>
 </div>
 </li>
        <li> <span class="li-head">cifs_profile</span> - Name of an existing CIFS profile. Source cifs.profile.name. <span class="li-normal">type: str</span>
 <a id='label8' href="javascript:ContentClick('label9', 'label8');" onmouseover="ContentPreview('label9');" onmouseout="ContentUnpreview('label9');" title="click to collapse or expand..."> more... </a>
 <div id="label9" style="display:none">
 <table border="1">
 <tr>
 <td></td>
 <td colspan="1">Supported Version Ranges</td>
 </tr>
 <tr>
 <td>cifs_profile</td>
 <td><code class="docutils literal notranslate">v6.2.0 -> 7.4.4 </code></td>
 </tr>
 </table>
 </div>
 </li>
        <li> <span class="li-head">diameter_filter_profile</span> - Name of an existing Diameter filter profile. Source diameter-filter.profile.name. <span class="li-normal">type: str</span>
 <a id='label10' href="javascript:ContentClick('label11', 'label10');" onmouseover="ContentPreview('label11');" onmouseout="ContentUnpreview('label11');" title="click to collapse or expand..."> more... </a>
 <div id="label11" style="display:none">
 <table border="1">
 <tr>
 <td></td>
 <td colspan="1">Supported Version Ranges</td>
 </tr>
 <tr>
 <td>diameter_filter_profile</td>
 <td><code class="docutils literal notranslate">v7.4.2 -> 7.4.4 </code></td>
 </tr>
 </table>
 </div>
 </li>
        <li> <span class="li-head">dlp_profile</span> - Name of an existing DLP profile. Source dlp.profile.name. <span class="li-normal">type: str</span>
 <a id='label12' href="javascript:ContentClick('label13', 'label12');" onmouseover="ContentPreview('label13');" onmouseout="ContentUnpreview('label13');" title="click to collapse or expand..."> more... </a>
 <div id="label13" style="display:none">
 <table border="1">
 <tr>
 <td></td>
 <td colspan="1">Supported Version Ranges</td>
 </tr>
 <tr>
 <td>dlp_profile</td>
 <td><code class="docutils literal notranslate">v7.2.0 -> 7.4.4 </code></td>
 </tr>
 </table>
 </div>
 </li>
        <li> <span class="li-head">dlp_sensor</span> - Name of an existing DLP sensor. Source dlp.sensor.name. <span class="li-normal">type: str</span>
 <a id='label14' href="javascript:ContentClick('label15', 'label14');" onmouseover="ContentPreview('label15');" onmouseout="ContentUnpreview('label15');" title="click to collapse or expand..."> more... </a>
 <div id="label15" style="display:none">
 <table border="1">
 <tr>
 <td></td>
 <td colspan="1">Supported Version Ranges</td>
 </tr>
 <tr>
 <td>dlp_sensor</td>
 <td><code class="docutils literal notranslate">v6.0.0 -> v7.0.12 </code></td>
 </tr>
 </table>
 </div>
 </li>
        <li> <span class="li-head">dnsfilter_profile</span> - Name of an existing DNS filter profile. Source dnsfilter.profile.name. <span class="li-normal">type: str</span>
 <a id='label16' href="javascript:ContentClick('label17', 'label16');" onmouseover="ContentPreview('label17');" onmouseout="ContentUnpreview('label17');" title="click to collapse or expand..."> more... </a>
 <div id="label17" style="display:none">
 <table border="1">
 <tr>
 <td></td>
 <td colspan="1">Supported Version Ranges</td>
 </tr>
 <tr>
 <td>dnsfilter_profile</td>
 <td><code class="docutils literal notranslate">v6.0.0 -> 7.4.4 </code></td>
 </tr>
 </table>
 </div>
 </li>
        <li> <span class="li-head">emailfilter_profile</span> - Name of an existing email filter profile. Source emailfilter.profile.name. <span class="li-normal">type: str</span>
 <a id='label18' href="javascript:ContentClick('label19', 'label18');" onmouseover="ContentPreview('label19');" onmouseout="ContentUnpreview('label19');" title="click to collapse or expand..."> more... </a>
 <div id="label19" style="display:none">
 <table border="1">
 <tr>
 <td></td>
 <td colspan="1">Supported Version Ranges</td>
 </tr>
 <tr>
 <td>emailfilter_profile</td>
 <td><code class="docutils literal notranslate">v6.2.0 -> 7.4.4 </code></td>
 </tr>
 </table>
 </div>
 </li>
        <li> <span class="li-head">file_filter_profile</span> - Name of an existing file-filter profile. Source file-filter.profile.name. <span class="li-normal">type: str</span>
 <a id='label20' href="javascript:ContentClick('label21', 'label20');" onmouseover="ContentPreview('label21');" onmouseout="ContentUnpreview('label21');" title="click to collapse or expand..."> more... </a>
 <div id="label21" style="display:none">
 <table border="1">
 <tr>
 <td></td>
 <td colspan="1">Supported Version Ranges</td>
 </tr>
 <tr>
 <td>file_filter_profile</td>
 <td><code class="docutils literal notranslate">v6.4.0 -> 7.4.4 </code></td>
 </tr>
 </table>
 </div>
 </li>
        <li> <span class="li-head">icap_profile</span> - Name of an existing ICAP profile. Source icap.profile.name. <span class="li-normal">type: str</span>
 <a id='label22' href="javascript:ContentClick('label23', 'label22');" onmouseover="ContentPreview('label23');" onmouseout="ContentUnpreview('label23');" title="click to collapse or expand..."> more... </a>
 <div id="label23" style="display:none">
 <table border="1">
 <tr>
 <td></td>
 <td colspan="1">Supported Version Ranges</td>
 </tr>
 <tr>
 <td>icap_profile</td>
 <td><code class="docutils literal notranslate">v6.0.0 -> 7.4.4 </code></td>
 </tr>
 </table>
 </div>
 </li>
        <li> <span class="li-head">ips_sensor</span> - Name of an existing IPS sensor. Source ips.sensor.name. <span class="li-normal">type: str</span>
 <a id='label24' href="javascript:ContentClick('label25', 'label24');" onmouseover="ContentPreview('label25');" onmouseout="ContentUnpreview('label25');" title="click to collapse or expand..."> more... </a>
 <div id="label25" style="display:none">
 <table border="1">
 <tr>
 <td></td>
 <td colspan="1">Supported Version Ranges</td>
 </tr>
 <tr>
 <td>ips_sensor</td>
 <td><code class="docutils literal notranslate">v6.0.0 -> 7.4.4 </code></td>
 </tr>
 </table>
 </div>
 </li>
        <li> <span class="li-head">ips_voip_filter</span> - Name of an existing VoIP (ips) profile. Source voip.profile.name. <span class="li-normal">type: str</span>
 <a id='label26' href="javascript:ContentClick('label27', 'label26');" onmouseover="ContentPreview('label27');" onmouseout="ContentUnpreview('label27');" title="click to collapse or expand..."> more... </a>
 <div id="label27" style="display:none">
 <table border="1">
 <tr>
 <td></td>
 <td colspan="1">Supported Version Ranges</td>
 </tr>
 <tr>
 <td>ips_voip_filter</td>
 <td><code class="docutils literal notranslate">v7.4.0 -> 7.4.4 </code></td>
 </tr>
 </table>
 </div>
 </li>
        <li> <span class="li-head">mms_profile</span> - Name of an existing MMS profile. Source firewall.mms-profile.name. <span class="li-normal">type: str</span>
 <a id='label28' href="javascript:ContentClick('label29', 'label28');" onmouseover="ContentPreview('label29');" onmouseout="ContentUnpreview('label29');" title="click to collapse or expand..."> more... </a>
 <div id="label29" style="display:none">
 <table border="1">
 <tr>
 <td></td>
 <td colspan="1">Supported Version Ranges</td>
 </tr>
 <tr>
 <td>mms_profile</td>
 <td><code class="docutils literal notranslate">v6.0.0 -> v6.2.7 </code></td>
 </tr>
 </table>
 </div>
 </li>
        <li> <span class="li-head">name</span> - Profile group name. <span class="li-normal">type: str</span> <span class="li-required">required: true</span>
 <a id='label30' href="javascript:ContentClick('label31', 'label30');" onmouseover="ContentPreview('label31');" onmouseout="ContentUnpreview('label31');" title="click to collapse or expand..."> more... </a>
 <div id="label31" style="display:none">
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
        <li> <span class="li-head">profile_protocol_options</span> - Name of an existing Protocol options profile. Source firewall.profile-protocol-options.name. <span class="li-normal">type: str</span>
 <a id='label32' href="javascript:ContentClick('label33', 'label32');" onmouseover="ContentPreview('label33');" onmouseout="ContentUnpreview('label33');" title="click to collapse or expand..."> more... </a>
 <div id="label33" style="display:none">
 <table border="1">
 <tr>
 <td></td>
 <td colspan="1">Supported Version Ranges</td>
 </tr>
 <tr>
 <td>profile_protocol_options</td>
 <td><code class="docutils literal notranslate">v6.0.0 -> 7.4.4 </code></td>
 </tr>
 </table>
 </div>
 </li>
        <li> <span class="li-head">sctp_filter_profile</span> - Name of an existing SCTP filter profile. Source sctp-filter.profile.name. <span class="li-normal">type: str</span>
 <a id='label34' href="javascript:ContentClick('label35', 'label34');" onmouseover="ContentPreview('label35');" onmouseout="ContentUnpreview('label35');" title="click to collapse or expand..."> more... </a>
 <div id="label35" style="display:none">
 <table border="1">
 <tr>
 <td></td>
 <td colspan="1">Supported Version Ranges</td>
 </tr>
 <tr>
 <td>sctp_filter_profile</td>
 <td><code class="docutils literal notranslate">v7.0.1 -> 7.4.4 </code></td>
 </tr>
 </table>
 </div>
 </li>
        <li> <span class="li-head">spamfilter_profile</span> - Name of an existing Spam filter profile. Source spamfilter.profile.name. <span class="li-normal">type: str</span>
 <a id='label36' href="javascript:ContentClick('label37', 'label36');" onmouseover="ContentPreview('label37');" onmouseout="ContentUnpreview('label37');" title="click to collapse or expand..."> more... </a>
 <div id="label37" style="display:none">
 <table border="1">
 <tr>
 <td></td>
 <td colspan="1">Supported Version Ranges</td>
 </tr>
 <tr>
 <td>spamfilter_profile</td>
 <td><code class="docutils literal notranslate">v6.0.0 -> v6.0.11 </code></td>
 </tr>
 </table>
 </div>
 </li>
        <li> <span class="li-head">ssh_filter_profile</span> - Name of an existing SSH filter profile. Source ssh-filter.profile.name. <span class="li-normal">type: str</span>
 <a id='label38' href="javascript:ContentClick('label39', 'label38');" onmouseover="ContentPreview('label39');" onmouseout="ContentUnpreview('label39');" title="click to collapse or expand..."> more... </a>
 <div id="label39" style="display:none">
 <table border="1">
 <tr>
 <td></td>
 <td colspan="1">Supported Version Ranges</td>
 </tr>
 <tr>
 <td>ssh_filter_profile</td>
 <td><code class="docutils literal notranslate">v6.0.0 -> 7.4.4 </code></td>
 </tr>
 </table>
 </div>
 </li>
        <li> <span class="li-head">ssl_ssh_profile</span> - Name of an existing SSL SSH profile. Source firewall.ssl-ssh-profile.name. <span class="li-normal">type: str</span>
 <a id='label40' href="javascript:ContentClick('label41', 'label40');" onmouseover="ContentPreview('label41');" onmouseout="ContentUnpreview('label41');" title="click to collapse or expand..."> more... </a>
 <div id="label41" style="display:none">
 <table border="1">
 <tr>
 <td></td>
 <td colspan="1">Supported Version Ranges</td>
 </tr>
 <tr>
 <td>ssl_ssh_profile</td>
 <td><code class="docutils literal notranslate">v6.0.0 -> 7.4.4 </code></td>
 </tr>
 </table>
 </div>
 </li>
        <li> <span class="li-head">videofilter_profile</span> - Name of an existing VideoFilter profile. Source videofilter.profile.name. <span class="li-normal">type: str</span>
 <a id='label42' href="javascript:ContentClick('label43', 'label42');" onmouseover="ContentPreview('label43');" onmouseout="ContentUnpreview('label43');" title="click to collapse or expand..."> more... </a>
 <div id="label43" style="display:none">
 <table border="1">
 <tr>
 <td></td>
 <td colspan="1">Supported Version Ranges</td>
 </tr>
 <tr>
 <td>videofilter_profile</td>
 <td><code class="docutils literal notranslate">v7.0.0 -> 7.4.4 </code></td>
 </tr>
 </table>
 </div>
 </li>
        <li> <span class="li-head">virtual_patch_profile</span> - Name of an existing virtual-patch profile. Source virtual-patch.profile.name. <span class="li-normal">type: str</span>
 <a id='label44' href="javascript:ContentClick('label45', 'label44');" onmouseover="ContentPreview('label45');" onmouseout="ContentUnpreview('label45');" title="click to collapse or expand..."> more... </a>
 <div id="label45" style="display:none">
 <table border="1">
 <tr>
 <td></td>
 <td colspan="1">Supported Version Ranges</td>
 </tr>
 <tr>
 <td>virtual_patch_profile</td>
 <td><code class="docutils literal notranslate">v7.4.1 -> 7.4.4 </code></td>
 </tr>
 </table>
 </div>
 </li>
        <li> <span class="li-head">voip_profile</span> - Name of an existing VoIP (voipd) profile. Source voip.profile.name. <span class="li-normal">type: str</span>
 <a id='label46' href="javascript:ContentClick('label47', 'label46');" onmouseover="ContentPreview('label47');" onmouseout="ContentUnpreview('label47');" title="click to collapse or expand..."> more... </a>
 <div id="label47" style="display:none">
 <table border="1">
 <tr>
 <td></td>
 <td colspan="1">Supported Version Ranges</td>
 </tr>
 <tr>
 <td>voip_profile</td>
 <td><code class="docutils literal notranslate">v6.0.0 -> 7.4.4 </code></td>
 </tr>
 </table>
 </div>
 </li>
        <li> <span class="li-head">waf_profile</span> - Name of an existing Web application firewall profile. Source waf.profile.name. <span class="li-normal">type: str</span>
 <a id='label48' href="javascript:ContentClick('label49', 'label48');" onmouseover="ContentPreview('label49');" onmouseout="ContentUnpreview('label49');" title="click to collapse or expand..."> more... </a>
 <div id="label49" style="display:none">
 <table border="1">
 <tr>
 <td></td>
 <td colspan="1">Supported Version Ranges</td>
 </tr>
 <tr>
 <td>waf_profile</td>
 <td><code class="docutils literal notranslate">v6.0.0 -> 7.4.4 </code></td>
 </tr>
 </table>
 </div>
 </li>
        <li> <span class="li-head">webfilter_profile</span> - Name of an existing Web filter profile. Source webfilter.profile.name. <span class="li-normal">type: str</span>
 <a id='label50' href="javascript:ContentClick('label51', 'label50');" onmouseover="ContentPreview('label51');" onmouseout="ContentUnpreview('label51');" title="click to collapse or expand..."> more... </a>
 <div id="label51" style="display:none">
 <table border="1">
 <tr>
 <td></td>
 <td colspan="1">Supported Version Ranges</td>
 </tr>
 <tr>
 <td>webfilter_profile</td>
 <td><code class="docutils literal notranslate">v6.0.0 -> 7.4.4 </code></td>
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
    
    - name: Configure profile groups.
      fortinet.fortios.fortios_firewall_profile_group:
          vdom: "{{ vdom }}"
          state: "present"
          access_token: "<your_own_value>"
          firewall_profile_group:
              application_list: "<your_own_value> (source application.list.name)"
              av_profile: "<your_own_value> (source antivirus.profile.name)"
              casb_profile: "<your_own_value> (source casb.profile.name)"
              cifs_profile: "<your_own_value> (source cifs.profile.name)"
              diameter_filter_profile: "<your_own_value> (source diameter-filter.profile.name)"
              dlp_profile: "<your_own_value> (source dlp.profile.name)"
              dlp_sensor: "<your_own_value> (source dlp.sensor.name)"
              dnsfilter_profile: "<your_own_value> (source dnsfilter.profile.name)"
              emailfilter_profile: "<your_own_value> (source emailfilter.profile.name)"
              file_filter_profile: "<your_own_value> (source file-filter.profile.name)"
              icap_profile: "<your_own_value> (source icap.profile.name)"
              ips_sensor: "<your_own_value> (source ips.sensor.name)"
              ips_voip_filter: "<your_own_value> (source voip.profile.name)"
              mms_profile: "<your_own_value> (source firewall.mms-profile.name)"
              name: "default_name_17"
              profile_protocol_options: "<your_own_value> (source firewall.profile-protocol-options.name)"
              sctp_filter_profile: "<your_own_value> (source sctp-filter.profile.name)"
              spamfilter_profile: "<your_own_value> (source spamfilter.profile.name)"
              ssh_filter_profile: "<your_own_value> (source ssh-filter.profile.name)"
              ssl_ssh_profile: "<your_own_value> (source firewall.ssl-ssh-profile.name)"
              videofilter_profile: "<your_own_value> (source videofilter.profile.name)"
              virtual_patch_profile: "<your_own_value> (source virtual-patch.profile.name)"
              voip_profile: "<your_own_value> (source voip.profile.name)"
              waf_profile: "<your_own_value> (source waf.profile.name)"
              webfilter_profile: "<your_own_value> (source webfilter.profile.name)"


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
