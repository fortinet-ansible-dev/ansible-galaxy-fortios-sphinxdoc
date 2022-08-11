:source: fortios_firewall_ip_translation.py

:orphan:

.. fortios_firewall_ip_translation:

fortios_firewall_ip_translation -- Configure firewall IP-translation in Fortinet's FortiOS and FortiGate.
+++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++

.. versionadded:: 2.0.0

.. contents::
   :local:
   :depth: 1


Synopsis
--------
- This module is able to configure a FortiGate or FortiOS (FOS) device by allowing the user to set and modify firewall feature and ip_translation category. Examples include all parameters and values need to be adjusted to datasources before usage. Tested with FOS v6.0.0



Requirements
------------
The below requirements are needed on the host that executes this module.

- ansible>=2.9


FortiOS Version Compatibility
-----------------------------


.. raw:: html

 <br>
 <table>
 <tr>
 <td></td>
 <td><code class="docutils literal notranslate">v6.0.0 </code></td>
 <td><code class="docutils literal notranslate">v6.0.5 </code></td>
 <td><code class="docutils literal notranslate">v6.0.11 </code></td>
 <td><code class="docutils literal notranslate">v6.2.0 </code></td>
 <td><code class="docutils literal notranslate">v6.2.3 </code></td>
 <td><code class="docutils literal notranslate">v6.2.5 </code></td>
 <td><code class="docutils literal notranslate">v6.2.7 </code></td>
 <td><code class="docutils literal notranslate">v6.4.0 </code></td>
 <td><code class="docutils literal notranslate">v6.4.1 </code></td>
 <td><code class="docutils literal notranslate">v6.4.4 </code></td>
 <td><code class="docutils literal notranslate">v7.0.0 </code></td>
 <td><code class="docutils literal notranslate">v7.0.1 </code></td>
 <td><code class="docutils literal notranslate">v7.0.2 </code></td>
 <td><code class="docutils literal notranslate">v7.0.3 </code></td>
 <td><code class="docutils literal notranslate">v7.0.4 </code></td>
 <td><code class="docutils literal notranslate">v7.0.5 </code></td>
 <td><code class="docutils literal notranslate">v7.2.0 </code></td>
 </tr>
 <tr>
 <td>fortios_firewall_ip_translation</td>
 <td>yes</td>
 <td>yes</td>
 <td>yes</td>
 <td>yes</td>
 <td>yes</td>
 <td>yes</td>
 <td>yes</td>
 <td>yes</td>
 <td>yes</td>
 <td>yes</td>
 <td>yes</td>
 <td>yes</td>
 <td>yes</td>
 <td>yes</td>
 <td>yes</td>
 <td>yes</td>
 <td>yes</td>
 </tr>
 </table>
 <p>



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
    <li> <span class="li-head">firewall_ip_translation</span> - Configure firewall IP-translation. <span class="li-normal">type: dict</span>
 <a id='label0' href="javascript:ContentClick('label1', 'label0');" onmouseover="ContentPreview('label1');" onmouseout="ContentUnpreview('label1');" title="click to collapse or expand..."> more... </a>
 <div id="label1" style="display:none">
 <table border="1">
 <tr>
 <td></td>
 <td><code class="docutils literal notranslate">v6.0.0 </code></td>
 <td><code class="docutils literal notranslate">v6.0.5 </code></td>
 <td><code class="docutils literal notranslate">v6.0.11 </code></td>
 <td><code class="docutils literal notranslate">v6.2.0 </code></td>
 <td><code class="docutils literal notranslate">v6.2.3 </code></td>
 <td><code class="docutils literal notranslate">v6.2.5 </code></td>
 <td><code class="docutils literal notranslate">v6.2.7 </code></td>
 <td><code class="docutils literal notranslate">v6.4.0 </code></td>
 <td><code class="docutils literal notranslate">v6.4.1 </code></td>
 <td><code class="docutils literal notranslate">v6.4.4 </code></td>
 <td><code class="docutils literal notranslate">v7.0.0 </code></td>
 <td><code class="docutils literal notranslate">v7.0.1 </code></td>
 <td><code class="docutils literal notranslate">v7.0.2 </code></td>
 <td><code class="docutils literal notranslate">v7.0.3 </code></td>
 <td><code class="docutils literal notranslate">v7.0.4 </code></td>
 <td><code class="docutils literal notranslate">v7.0.5 </code></td>
 <td><code class="docutils literal notranslate">v7.2.0 </code></td>
 </tr>
 <tr>
 <td>firewall_ip_translation</td>
 <td>yes</td>
 <td>yes</td>
 <td>yes</td>
 <td>yes</td>
 <td>yes</td>
 <td>yes</td>
 <td>yes</td>
 <td>yes</td>
 <td>yes</td>
 <td>yes</td>
 <td>yes</td>
 <td>yes</td>
 <td>yes</td>
 <td>yes</td>
 <td>yes</td>
 <td>yes</td>
 <td>yes</td>
 </tr>
 </table>
 </div>
 </li>
        <ul class="ul-self">
        <li> <span class="li-head">endip</span> - Final IPv4 address (inclusive) in the range of the addresses to be translated (format xxx.xxx.xxx.xxx). <span class="li-normal">type: str</span>
 <a id='label2' href="javascript:ContentClick('label3', 'label2');" onmouseover="ContentPreview('label3');" onmouseout="ContentUnpreview('label3');" title="click to collapse or expand..."> more... </a>
 <div id="label3" style="display:none">
 <table border="1">
 <tr>
 <td></td>
 <td><code class="docutils literal notranslate">v6.0.0 </code></td>
 <td><code class="docutils literal notranslate">v6.0.5 </code></td>
 <td><code class="docutils literal notranslate">v6.0.11 </code></td>
 <td><code class="docutils literal notranslate">v6.2.0 </code></td>
 <td><code class="docutils literal notranslate">v6.2.3 </code></td>
 <td><code class="docutils literal notranslate">v6.2.5 </code></td>
 <td><code class="docutils literal notranslate">v6.2.7 </code></td>
 <td><code class="docutils literal notranslate">v6.4.0 </code></td>
 <td><code class="docutils literal notranslate">v6.4.1 </code></td>
 <td><code class="docutils literal notranslate">v6.4.4 </code></td>
 <td><code class="docutils literal notranslate">v7.0.0 </code></td>
 <td><code class="docutils literal notranslate">v7.0.1 </code></td>
 <td><code class="docutils literal notranslate">v7.0.2 </code></td>
 <td><code class="docutils literal notranslate">v7.0.3 </code></td>
 <td><code class="docutils literal notranslate">v7.0.4 </code></td>
 <td><code class="docutils literal notranslate">v7.0.5 </code></td>
 <td><code class="docutils literal notranslate">v7.2.0 </code></td>
 </tr>
 <tr>
 <td>endip</td>
 <td>yes</td>
 <td>yes</td>
 <td>yes</td>
 <td>yes</td>
 <td>yes</td>
 <td>yes</td>
 <td>yes</td>
 <td>yes</td>
 <td>yes</td>
 <td>yes</td>
 <td>yes</td>
 <td>yes</td>
 <td>yes</td>
 <td>yes</td>
 <td>yes</td>
 <td>yes</td>
 <td>yes</td>
 </tr>
 </table>
 </div>
 </li>
        <li> <span class="li-head">map_startip</span> - Address to be used as the starting point for translation in the range (format xxx.xxx.xxx.xxx). <span class="li-normal">type: str</span>
 <a id='label4' href="javascript:ContentClick('label5', 'label4');" onmouseover="ContentPreview('label5');" onmouseout="ContentUnpreview('label5');" title="click to collapse or expand..."> more... </a>
 <div id="label5" style="display:none">
 <table border="1">
 <tr>
 <td></td>
 <td><code class="docutils literal notranslate">v6.0.0 </code></td>
 <td><code class="docutils literal notranslate">v6.0.5 </code></td>
 <td><code class="docutils literal notranslate">v6.0.11 </code></td>
 <td><code class="docutils literal notranslate">v6.2.0 </code></td>
 <td><code class="docutils literal notranslate">v6.2.3 </code></td>
 <td><code class="docutils literal notranslate">v6.2.5 </code></td>
 <td><code class="docutils literal notranslate">v6.2.7 </code></td>
 <td><code class="docutils literal notranslate">v6.4.0 </code></td>
 <td><code class="docutils literal notranslate">v6.4.1 </code></td>
 <td><code class="docutils literal notranslate">v6.4.4 </code></td>
 <td><code class="docutils literal notranslate">v7.0.0 </code></td>
 <td><code class="docutils literal notranslate">v7.0.1 </code></td>
 <td><code class="docutils literal notranslate">v7.0.2 </code></td>
 <td><code class="docutils literal notranslate">v7.0.3 </code></td>
 <td><code class="docutils literal notranslate">v7.0.4 </code></td>
 <td><code class="docutils literal notranslate">v7.0.5 </code></td>
 <td><code class="docutils literal notranslate">v7.2.0 </code></td>
 </tr>
 <tr>
 <td>map_startip</td>
 <td>yes</td>
 <td>yes</td>
 <td>yes</td>
 <td>yes</td>
 <td>yes</td>
 <td>yes</td>
 <td>yes</td>
 <td>yes</td>
 <td>yes</td>
 <td>yes</td>
 <td>yes</td>
 <td>yes</td>
 <td>yes</td>
 <td>yes</td>
 <td>yes</td>
 <td>yes</td>
 <td>yes</td>
 </tr>
 </table>
 </div>
 </li>
        <li> <span class="li-head">startip</span> - First IPv4 address (inclusive) in the range of the addresses to be translated (format xxx.xxx.xxx.xxx). <span class="li-normal">type: str</span>
 <a id='label6' href="javascript:ContentClick('label7', 'label6');" onmouseover="ContentPreview('label7');" onmouseout="ContentUnpreview('label7');" title="click to collapse or expand..."> more... </a>
 <div id="label7" style="display:none">
 <table border="1">
 <tr>
 <td></td>
 <td><code class="docutils literal notranslate">v6.0.0 </code></td>
 <td><code class="docutils literal notranslate">v6.0.5 </code></td>
 <td><code class="docutils literal notranslate">v6.0.11 </code></td>
 <td><code class="docutils literal notranslate">v6.2.0 </code></td>
 <td><code class="docutils literal notranslate">v6.2.3 </code></td>
 <td><code class="docutils literal notranslate">v6.2.5 </code></td>
 <td><code class="docutils literal notranslate">v6.2.7 </code></td>
 <td><code class="docutils literal notranslate">v6.4.0 </code></td>
 <td><code class="docutils literal notranslate">v6.4.1 </code></td>
 <td><code class="docutils literal notranslate">v6.4.4 </code></td>
 <td><code class="docutils literal notranslate">v7.0.0 </code></td>
 <td><code class="docutils literal notranslate">v7.0.1 </code></td>
 <td><code class="docutils literal notranslate">v7.0.2 </code></td>
 <td><code class="docutils literal notranslate">v7.0.3 </code></td>
 <td><code class="docutils literal notranslate">v7.0.4 </code></td>
 <td><code class="docutils literal notranslate">v7.0.5 </code></td>
 <td><code class="docutils literal notranslate">v7.2.0 </code></td>
 </tr>
 <tr>
 <td>startip</td>
 <td>yes</td>
 <td>yes</td>
 <td>yes</td>
 <td>yes</td>
 <td>yes</td>
 <td>yes</td>
 <td>yes</td>
 <td>yes</td>
 <td>yes</td>
 <td>yes</td>
 <td>yes</td>
 <td>yes</td>
 <td>yes</td>
 <td>yes</td>
 <td>yes</td>
 <td>yes</td>
 <td>yes</td>
 </tr>
 </table>
 </div>
 </li>
        <li> <span class="li-head">transid</span> - IP translation ID. <span class="li-normal">type: int</span> <span class="li-required">required: true</span>
 <a id='label8' href="javascript:ContentClick('label9', 'label8');" onmouseover="ContentPreview('label9');" onmouseout="ContentUnpreview('label9');" title="click to collapse or expand..."> more... </a>
 <div id="label9" style="display:none">
 <table border="1">
 <tr>
 <td></td>
 <td><code class="docutils literal notranslate">v6.0.0 </code></td>
 <td><code class="docutils literal notranslate">v6.0.5 </code></td>
 <td><code class="docutils literal notranslate">v6.0.11 </code></td>
 <td><code class="docutils literal notranslate">v6.2.0 </code></td>
 <td><code class="docutils literal notranslate">v6.2.3 </code></td>
 <td><code class="docutils literal notranslate">v6.2.5 </code></td>
 <td><code class="docutils literal notranslate">v6.2.7 </code></td>
 <td><code class="docutils literal notranslate">v6.4.0 </code></td>
 <td><code class="docutils literal notranslate">v6.4.1 </code></td>
 <td><code class="docutils literal notranslate">v6.4.4 </code></td>
 <td><code class="docutils literal notranslate">v7.0.0 </code></td>
 <td><code class="docutils literal notranslate">v7.0.1 </code></td>
 <td><code class="docutils literal notranslate">v7.0.2 </code></td>
 <td><code class="docutils literal notranslate">v7.0.3 </code></td>
 <td><code class="docutils literal notranslate">v7.0.4 </code></td>
 <td><code class="docutils literal notranslate">v7.0.5 </code></td>
 <td><code class="docutils literal notranslate">v7.2.0 </code></td>
 </tr>
 <tr>
 <td>transid</td>
 <td>yes</td>
 <td>yes</td>
 <td>yes</td>
 <td>yes</td>
 <td>yes</td>
 <td>yes</td>
 <td>yes</td>
 <td>yes</td>
 <td>yes</td>
 <td>yes</td>
 <td>yes</td>
 <td>yes</td>
 <td>yes</td>
 <td>yes</td>
 <td>yes</td>
 <td>yes</td>
 <td>yes</td>
 </tr>
 </table>
 </div>
 </li>
        <li> <span class="li-head">type</span> - IP translation type (option: SCTP). <span class="li-normal">type: str</span> <span class="li-normal">choices: SCTP</span>
 <a id='label10' href="javascript:ContentClick('label11', 'label10');" onmouseover="ContentPreview('label11');" onmouseout="ContentUnpreview('label11');" title="click to collapse or expand..."> more... </a>
 <div id="label11" style="display:none">
 <table border="1">
 <tr>
 <td></td>
 <td><code class="docutils literal notranslate">v6.0.0 </code></td>
 <td><code class="docutils literal notranslate">v6.0.5 </code></td>
 <td><code class="docutils literal notranslate">v6.0.11 </code></td>
 <td><code class="docutils literal notranslate">v6.2.0 </code></td>
 <td><code class="docutils literal notranslate">v6.2.3 </code></td>
 <td><code class="docutils literal notranslate">v6.2.5 </code></td>
 <td><code class="docutils literal notranslate">v6.2.7 </code></td>
 <td><code class="docutils literal notranslate">v6.4.0 </code></td>
 <td><code class="docutils literal notranslate">v6.4.1 </code></td>
 <td><code class="docutils literal notranslate">v6.4.4 </code></td>
 <td><code class="docutils literal notranslate">v7.0.0 </code></td>
 <td><code class="docutils literal notranslate">v7.0.1 </code></td>
 <td><code class="docutils literal notranslate">v7.0.2 </code></td>
 <td><code class="docutils literal notranslate">v7.0.3 </code></td>
 <td><code class="docutils literal notranslate">v7.0.4 </code></td>
 <td><code class="docutils literal notranslate">v7.0.5 </code></td>
 <td><code class="docutils literal notranslate">v7.2.0 </code></td>
 </tr>
 <tr>
 <td>type</td>
 <td>yes</td>
 <td>yes</td>
 <td>yes</td>
 <td>yes</td>
 <td>yes</td>
 <td>yes</td>
 <td>yes</td>
 <td>yes</td>
 <td>yes</td>
 <td>yes</td>
 <td>yes</td>
 <td>yes</td>
 <td>yes</td>
 <td>yes</td>
 <td>yes</td>
 <td>yes</td>
 <td>yes</td>
 </tr>
 <tr>
 <td>[SCTP]</td>
 <td>yes</td>
 <td>yes</td>
 <td>yes</td>
 <td>yes</td>
 <td>yes</td>
 <td>yes</td>
 <td>yes</td>
 <td>yes</td>
 <td>yes</td>
 <td>yes</td>
 <td>yes</td>
 <td>yes</td>
 <td>yes</td>
 <td>yes</td>
 <td>yes</td>
 <td>yes</td>
 <td>yes</td>
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
    
    - hosts: fortigates
      collections:
        - fortinet.fortios
      connection: httpapi
      vars:
       vdom: "root"
       ansible_httpapi_use_ssl: yes
       ansible_httpapi_validate_certs: no
       ansible_httpapi_port: 443
      tasks:
      - name: Configure firewall IP-translation.
        fortios_firewall_ip_translation:
          vdom:  "{{ vdom }}"
          state: "present"
          access_token: "<your_own_value>"
          firewall_ip_translation:
            endip: "<your_own_value>"
            map_startip: "<your_own_value>"
            startip: "<your_own_value>"
            transid: "6"
            type: "SCTP"
    


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
