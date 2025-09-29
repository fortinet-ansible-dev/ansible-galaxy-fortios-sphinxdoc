:source: fortios_telemetry_controller_profile.py

:orphan:

.. fortios_telemetry_controller_profile:

fortios_telemetry_controller_profile -- Configure FortiTelemetry profiles in Fortinet's FortiOS and FortiGate.
++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++

.. versionadded:: 2.0.0

.. contents::
   :local:
   :depth: 1


Synopsis
--------
- This module is able to configure a FortiGate or FortiOS (FOS) device by allowing the user to set and modify telemetry_controller feature and profile category. Examples include all parameters and values need to be adjusted to datasources before usage. Tested with FOS v6.0.0



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
    <li> <span class="li-head">telemetry_controller_profile</span> - Configure FortiTelemetry profiles. <span class="li-normal">type: dict</span>
 <a id='label0' href="javascript:ContentClick('label1', 'label0');" onmouseover="ContentPreview('label1');" onmouseout="ContentUnpreview('label1');" title="click to collapse or expand..."> more... </a>
 <div id="label1" style="display:none">
 <table border="1">
 <tr>
 <td></td><td colspan="1">Supported Version Ranges</td>
 </tr>
 <tr>
 <td>telemetry_controller_profile</td>
 <td><code class="docutils literal notranslate">v7.6.3 -> 7.6.4 </code></td>
 </tr>
 </table>
 </div>
 </li>
        <ul class="ul-self">
        <li> <span class="li-head">application</span> - Configure applications. <span class="li-normal">type: list</span> <span style="font-family:'Courier New'" class="li-required">member_path: application:id</span>
 <a id='label2' href="javascript:ContentClick('label3', 'label2');" onmouseover="ContentPreview('label3');" onmouseout="ContentUnpreview('label3');" title="click to collapse or expand..."> more... </a>
 <div id="label3" style="display:none">
 <table border="1">
 <tr>
 <td></td><td colspan="1">Supported Version Ranges</td>
 </tr>
 <tr>
 <td>application</td>
 <td><code class="docutils literal notranslate">v7.6.3 -> 7.6.4 </code></td>
 </tr>
 </table>
 </div>
 </li>
            <ul class="ul-self">
            <li> <span class="li-head">app_name</span> - Application name. Source telemetry-controller.application.custom.app-name telemetry-controller.application.predefine.app-name. <span class="li-normal">type: str</span>
 <a id='label4' href="javascript:ContentClick('label5', 'label4');" onmouseover="ContentPreview('label5');" onmouseout="ContentUnpreview('label5');" title="click to collapse or expand..."> more... </a>
 <div id="label5" style="display:none">
 <table border="1">
 <tr>
 <td></td>
 <td colspan="1">Supported Version Ranges</td>
 </tr>
 <tr>
 <td>app_name</td>
 <td><code class="docutils literal notranslate">v7.6.3 -> 7.6.4 </code></td>
 </tr>
 </table>
 </div>
 </li>
            <li> <span class="li-head">id</span> - ID. see <a href='#notes'>Notes</a>. <span class="li-normal">type: int</span> <span class="li-required">required: true</span>
 <a id='label6' href="javascript:ContentClick('label7', 'label6');" onmouseover="ContentPreview('label7');" onmouseout="ContentUnpreview('label7');" title="click to collapse or expand..."> more... </a>
 <div id="label7" style="display:none">
 <table border="1">
 <tr>
 <td></td>
 <td colspan="1">Supported Version Ranges</td>
 </tr>
 <tr>
 <td>id</td>
 <td><code class="docutils literal notranslate">v7.6.3 -> 7.6.4 </code></td>
 </tr>
 </table>
 </div>
 </li>
            <li> <span class="li-head">interval</span> - Time in milliseconds to check the application (1000 - 86,400 * 1000). <span class="li-normal">type: int</span>
 <a id='label8' href="javascript:ContentClick('label9', 'label8');" onmouseover="ContentPreview('label9');" onmouseout="ContentUnpreview('label9');" title="click to collapse or expand..."> more... </a>
 <div id="label9" style="display:none">
 <table border="1">
 <tr>
 <td></td>
 <td colspan="1">Supported Version Ranges</td>
 </tr>
 <tr>
 <td>interval</td>
 <td><code class="docutils literal notranslate">v7.6.3 -> 7.6.4 </code></td>
 </tr>
 </table>
 </div>
 </li>
            <li> <span class="li-head">monitor</span> - Enable/disable monitoring of the application. <span class="li-normal">type: str</span> <span class="li-normal">choices: enable, disable</span>
 <a id='label10' href="javascript:ContentClick('label11', 'label10');" onmouseover="ContentPreview('label11');" onmouseout="ContentUnpreview('label11');" title="click to collapse or expand..."> more... </a>
 <div id="label11" style="display:none">
 <table border="1">
 <tr>
 <td></td>
 <td colspan="1">Supported Version Ranges</td>
 </tr>
 <tr>
 <td>monitor</td>
 <td><code class="docutils literal notranslate">v7.6.3 -> 7.6.4 </code></td>
 </tr>
 <tr>
 <td>[enable]</td>
 <td><code class="docutils literal notranslate">v7.6.3 -> 7.6.4</code></td>
 <tr>
 <td>[disable]</td>
 <td><code class="docutils literal notranslate">v7.6.3 -> 7.6.4</code></td>
 </table>
 </div>
 </li>
            <li> <span class="li-head">sla</span> - Service level agreement (SLA). <span class="li-normal">type: dict</span>
 <a id='label12' href="javascript:ContentClick('label13', 'label12');" onmouseover="ContentPreview('label13');" onmouseout="ContentUnpreview('label13');" title="click to collapse or expand..."> more... </a>
 <div id="label13" style="display:none">
 <table border="1">
 <tr>
 <td></td><td colspan="1">Supported Version Ranges</td>
 </tr>
 <tr>
 <td>sla</td>
 <td><code class="docutils literal notranslate">v7.6.3 -> 7.6.4 </code></td>
 </tr>
 </table>
 </div>
 </li>
                <ul class="ul-self">
                <li> <span class="li-head">app_throughput_threshold</span> - Threshold of application throughput in megabytes (0 - 10,000). <span class="li-normal">type: int</span>
 <a id='label14' href="javascript:ContentClick('label15', 'label14');" onmouseover="ContentPreview('label15');" onmouseout="ContentUnpreview('label15');" title="click to collapse or expand..."> more... </a>
 <div id="label15" style="display:none">
 <table border="1">
 <tr>
 <td></td>
 <td colspan="1">Supported Version Ranges</td>
 </tr>
 <tr>
 <td>app_throughput_threshold</td>
 <td><code class="docutils literal notranslate">v7.6.3 -> 7.6.4 </code></td>
 </tr>
 </table>
 </div>
 </li>
                <li> <span class="li-head">atdt_threshold</span> - Threshold of application total downloading time in milliseconds (0 - 10,000,000). <span class="li-normal">type: int</span>
 <a id='label16' href="javascript:ContentClick('label17', 'label16');" onmouseover="ContentPreview('label17');" onmouseout="ContentUnpreview('label17');" title="click to collapse or expand..."> more... </a>
 <div id="label17" style="display:none">
 <table border="1">
 <tr>
 <td></td>
 <td colspan="1">Supported Version Ranges</td>
 </tr>
 <tr>
 <td>atdt_threshold</td>
 <td><code class="docutils literal notranslate">v7.6.3 -> 7.6.4 </code></td>
 </tr>
 </table>
 </div>
 </li>
                <li> <span class="li-head">dns_time_threshold</span> - Threshold of 95th percentile of DNS resolution time in milliseconds (0 - 10,000,000). <span class="li-normal">type: int</span>
 <a id='label18' href="javascript:ContentClick('label19', 'label18');" onmouseover="ContentPreview('label19');" onmouseout="ContentUnpreview('label19');" title="click to collapse or expand..."> more... </a>
 <div id="label19" style="display:none">
 <table border="1">
 <tr>
 <td></td>
 <td colspan="1">Supported Version Ranges</td>
 </tr>
 <tr>
 <td>dns_time_threshold</td>
 <td><code class="docutils literal notranslate">v7.6.3 -> 7.6.4 </code></td>
 </tr>
 </table>
 </div>
 </li>
                <li> <span class="li-head">experience_score_threshold</span> - Threshold of experience score (0 - 10). <span class="li-normal">type: int</span>
 <a id='label20' href="javascript:ContentClick('label21', 'label20');" onmouseover="ContentPreview('label21');" onmouseout="ContentUnpreview('label21');" title="click to collapse or expand..."> more... </a>
 <div id="label21" style="display:none">
 <table border="1">
 <tr>
 <td></td>
 <td colspan="1">Supported Version Ranges</td>
 </tr>
 <tr>
 <td>experience_score_threshold</td>
 <td><code class="docutils literal notranslate">v7.6.3 -> 7.6.4 </code></td>
 </tr>
 </table>
 </div>
 </li>
                <li> <span class="li-head">failure_rate_threshold</span> - Threshold of failure rate (0 - 100). <span class="li-normal">type: int</span>
 <a id='label22' href="javascript:ContentClick('label23', 'label22');" onmouseover="ContentPreview('label23');" onmouseout="ContentUnpreview('label23');" title="click to collapse or expand..."> more... </a>
 <div id="label23" style="display:none">
 <table border="1">
 <tr>
 <td></td>
 <td colspan="1">Supported Version Ranges</td>
 </tr>
 <tr>
 <td>failure_rate_threshold</td>
 <td><code class="docutils literal notranslate">v7.6.3 -> 7.6.4 </code></td>
 </tr>
 </table>
 </div>
 </li>
                <li> <span class="li-head">jitter_threshold</span> - Threshold of jitter in milliseconds (0 - 10,000,000). <span class="li-normal">type: int</span>
 <a id='label24' href="javascript:ContentClick('label25', 'label24');" onmouseover="ContentPreview('label25');" onmouseout="ContentUnpreview('label25');" title="click to collapse or expand..."> more... </a>
 <div id="label25" style="display:none">
 <table border="1">
 <tr>
 <td></td>
 <td colspan="1">Supported Version Ranges</td>
 </tr>
 <tr>
 <td>jitter_threshold</td>
 <td><code class="docutils literal notranslate">v7.6.3 -> 7.6.4 </code></td>
 </tr>
 </table>
 </div>
 </li>
                <li> <span class="li-head">latency_threshold</span> - Threshold of latency in milliseconds (0 - 10,000,000). <span class="li-normal">type: int</span>
 <a id='label26' href="javascript:ContentClick('label27', 'label26');" onmouseover="ContentPreview('label27');" onmouseout="ContentUnpreview('label27');" title="click to collapse or expand..."> more... </a>
 <div id="label27" style="display:none">
 <table border="1">
 <tr>
 <td></td>
 <td colspan="1">Supported Version Ranges</td>
 </tr>
 <tr>
 <td>latency_threshold</td>
 <td><code class="docutils literal notranslate">v7.6.3 -> 7.6.4 </code></td>
 </tr>
 </table>
 </div>
 </li>
                <li> <span class="li-head">packet_loss_threshold</span> - Threshold of packet loss (0 - 100). <span class="li-normal">type: int</span>
 <a id='label28' href="javascript:ContentClick('label29', 'label28');" onmouseover="ContentPreview('label29');" onmouseout="ContentUnpreview('label29');" title="click to collapse or expand..."> more... </a>
 <div id="label29" style="display:none">
 <table border="1">
 <tr>
 <td></td>
 <td colspan="1">Supported Version Ranges</td>
 </tr>
 <tr>
 <td>packet_loss_threshold</td>
 <td><code class="docutils literal notranslate">v7.6.3 -> 7.6.4 </code></td>
 </tr>
 </table>
 </div>
 </li>
                <li> <span class="li-head">sla_factor</span> - Criteria on which metric to SLA threshold list. <span class="li-normal">type: list</span> <span class="li-normal">choices: experience-score, failure-rate, latency, jitter, packet-loss, ttfb, atdt, tcp-rtt, dns-time, tls-time, app-throughput</span>
 <a id='label30' href="javascript:ContentClick('label31', 'label30');" onmouseover="ContentPreview('label31');" onmouseout="ContentUnpreview('label31');" title="click to collapse or expand..."> more... </a>
 <div id="label31" style="display:none">
 <table border="1">
 <tr>
 <td></td>
 <td colspan="1">Supported Version Ranges</td>
 </tr>
 <tr>
 <td>sla_factor</td>
 <td><code class="docutils literal notranslate">v7.6.3 -> 7.6.4 </code></td>
 </tr>
 <tr>
 <td>[experience-score]</td>
 <td><code class="docutils literal notranslate">v7.6.3 -> 7.6.4</code></td>
 <tr>
 <td>[failure-rate]</td>
 <td><code class="docutils literal notranslate">v7.6.3 -> 7.6.4</code></td>
 <tr>
 <td>[latency]</td>
 <td><code class="docutils literal notranslate">v7.6.3 -> 7.6.4</code></td>
 <tr>
 <td>[jitter]</td>
 <td><code class="docutils literal notranslate">v7.6.3 -> 7.6.4</code></td>
 <tr>
 <td>[packet-loss]</td>
 <td><code class="docutils literal notranslate">v7.6.3 -> 7.6.4</code></td>
 <tr>
 <td>[ttfb]</td>
 <td><code class="docutils literal notranslate">v7.6.3 -> 7.6.4</code></td>
 <tr>
 <td>[atdt]</td>
 <td><code class="docutils literal notranslate">v7.6.3 -> 7.6.4</code></td>
 <tr>
 <td>[tcp-rtt]</td>
 <td><code class="docutils literal notranslate">v7.6.3 -> 7.6.4</code></td>
 <tr>
 <td>[dns-time]</td>
 <td><code class="docutils literal notranslate">v7.6.3 -> 7.6.4</code></td>
 <tr>
 <td>[tls-time]</td>
 <td><code class="docutils literal notranslate">v7.6.3 -> 7.6.4</code></td>
 <tr>
 <td>[app-throughput]</td>
 <td><code class="docutils literal notranslate">v7.6.3 -> 7.6.4</code></td>
 </table>
 </div>
 </li>
                <li> <span class="li-head">tcp_rtt_threshold</span> - Threshold of TCP round-trip time in milliseconds (0 - 10,000,000). <span class="li-normal">type: int</span>
 <a id='label32' href="javascript:ContentClick('label33', 'label32');" onmouseover="ContentPreview('label33');" onmouseout="ContentUnpreview('label33');" title="click to collapse or expand..."> more... </a>
 <div id="label33" style="display:none">
 <table border="1">
 <tr>
 <td></td>
 <td colspan="1">Supported Version Ranges</td>
 </tr>
 <tr>
 <td>tcp_rtt_threshold</td>
 <td><code class="docutils literal notranslate">v7.6.3 -> 7.6.4 </code></td>
 </tr>
 </table>
 </div>
 </li>
                <li> <span class="li-head">tls_time_threshold</span> - Threshold of 95th percentile of TLS handshake time in milliseconds (0 - 10,000,000). <span class="li-normal">type: int</span>
 <a id='label34' href="javascript:ContentClick('label35', 'label34');" onmouseover="ContentPreview('label35');" onmouseout="ContentUnpreview('label35');" title="click to collapse or expand..."> more... </a>
 <div id="label35" style="display:none">
 <table border="1">
 <tr>
 <td></td>
 <td colspan="1">Supported Version Ranges</td>
 </tr>
 <tr>
 <td>tls_time_threshold</td>
 <td><code class="docutils literal notranslate">v7.6.3 -> 7.6.4 </code></td>
 </tr>
 </table>
 </div>
 </li>
                <li> <span class="li-head">ttfb_threshold</span> - Threshold of time to first byte in milliseconds (0 - 10,000,000). <span class="li-normal">type: int</span>
 <a id='label36' href="javascript:ContentClick('label37', 'label36');" onmouseover="ContentPreview('label37');" onmouseout="ContentUnpreview('label37');" title="click to collapse or expand..."> more... </a>
 <div id="label37" style="display:none">
 <table border="1">
 <tr>
 <td></td>
 <td colspan="1">Supported Version Ranges</td>
 </tr>
 <tr>
 <td>ttfb_threshold</td>
 <td><code class="docutils literal notranslate">v7.6.3 -> 7.6.4 </code></td>
 </tr>
 </table>
 </div>
 </li>
                </ul>
            </ul>
        <li> <span class="li-head">comment</span> - Comment. <span class="li-normal">type: str</span>
 <a id='label38' href="javascript:ContentClick('label39', 'label38');" onmouseover="ContentPreview('label39');" onmouseout="ContentUnpreview('label39');" title="click to collapse or expand..."> more... </a>
 <div id="label39" style="display:none">
 <table border="1">
 <tr>
 <td></td>
 <td colspan="1">Supported Version Ranges</td>
 </tr>
 <tr>
 <td>comment</td>
 <td><code class="docutils literal notranslate">v7.6.3 -> 7.6.4 </code></td>
 </tr>
 </table>
 </div>
 </li>
        <li> <span class="li-head">name</span> - Name of the profile. <span class="li-normal">type: str</span> <span class="li-required">required: true</span>
 <a id='label40' href="javascript:ContentClick('label41', 'label40');" onmouseover="ContentPreview('label41');" onmouseout="ContentUnpreview('label41');" title="click to collapse or expand..."> more... </a>
 <div id="label41" style="display:none">
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
        </ul>
    </ul>


Notes
-----

.. note::

   - Legacy fortiosapi has been deprecated, httpapi is the preferred way to run playbooks



Examples
--------

.. code-block:: yaml+jinja
    
    - name: Configure FortiTelemetry profiles.
      fortinet.fortios.fortios_telemetry_controller_profile:
          vdom: "{{ vdom }}"
          state: "present"
          access_token: "<your_own_value>"
          telemetry_controller_profile:
              application:
                  -
                      app_name: "<your_own_value> (source telemetry-controller.application.custom.app-name telemetry-controller.application.predefine.app-name)"
                      id: "5"
                      interval: "300000"
                      monitor: "enable"
                      sla:
                          app_throughput_threshold: "2"
                          atdt_threshold: "3000"
                          dns_time_threshold: "100"
                          experience_score_threshold: "6"
                          failure_rate_threshold: "5"
                          jitter_threshold: "50"
                          latency_threshold: "100"
                          packet_loss_threshold: "5"
                          sla_factor: "experience-score"
                          tcp_rtt_threshold: "100"
                          tls_time_threshold: "200"
                          ttfb_threshold: "200"
              comment: "Comment."
              name: "default_name_22"


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
