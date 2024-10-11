:source: fortios_webfilter_fortiguard.py

:orphan:

.. fortios_webfilter_fortiguard:

fortios_webfilter_fortiguard -- Configure FortiGuard Web Filter service in Fortinet's FortiOS and FortiGate.
++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++

.. versionadded:: 2.0.0

.. contents::
   :local:
   :depth: 1


Synopsis
--------
- This module is able to configure a FortiGate or FortiOS (FOS) device by allowing the user to set and modify webfilter feature and fortiguard category. Examples include all parameters and values need to be adjusted to datasources before usage. Tested with FOS v6.0.0



Requirements
------------
The below requirements are needed on the host that executes this module.

- ansible>=2.15


Tips
----
Using member operation to add an element to an existing object.

FortiOS Version Compatibility
-----------------------------
Supported Version Ranges: v6.0.0 -> v7.6.0


Parameters
----------


.. raw:: html

    <ul>
    <li> <span class="li-head">access_token</span> - Token-based authentication. Generated from GUI of Fortigate. <span class="li-normal">type: str</span> <span class="li-required">required: false</span> </li>
    <li> <span class="li-head">enable_log</span> - Enable/Disable logging for task. <span class="li-normal">type: bool</span> <span class="li-required">required: false</span> <span class="li-normal">default: False</span> </li>
    <li> <span class="li-head">vdom</span> - Virtual domain, among those defined previously. A vdom is a virtual instance of the FortiGate that can be configured and used as a different unit. <span class="li-normal">type: str</span> <span class="li-normal">default: root</span> </li>
    <li> <span class="li-head">member_path</span> - Member attribute path to operate on. <span class="li-normal">type: str</span> </li>
    <li> <span class="li-head">member_state</span> - Add or delete a member under specified attribute path. <span class="li-normal">type: str</span> <span class="li-normal">choices: present, absent</span> </li>
    <li> <span class="li-head">webfilter_fortiguard</span> - Configure FortiGuard Web Filter service. <span class="li-normal">type: dict</span>
 <a id='label0' href="javascript:ContentClick('label1', 'label0');" onmouseover="ContentPreview('label1');" onmouseout="ContentUnpreview('label1');" title="click to collapse or expand..."> more... </a>
 <div id="label1" style="display:none">
 <table border="1">
 <tr>
 <td></td><td colspan="1">Supported Version Ranges</td>
 </tr>
 <tr>
 <td>webfilter_fortiguard</td>
 <td><code class="docutils literal notranslate">v6.0.0 -> 7.6.0 </code></td>
 </tr>
 </table>
 </div>
 </li>
        <ul class="ul-self">
        <li> <span class="li-head">cache_mem_percent</span> - Maximum percentage of available memory allocated to caching (1 - 15). <span class="li-normal">type: int</span>
 <a id='label2' href="javascript:ContentClick('label3', 'label2');" onmouseover="ContentPreview('label3');" onmouseout="ContentUnpreview('label3');" title="click to collapse or expand..."> more... </a>
 <div id="label3" style="display:none">
 <table border="1">
 <tr>
 <td></td>
 <td colspan="1">Supported Version Ranges</td>
 </tr>
 <tr>
 <td>cache_mem_percent</td>
 <td><code class="docutils literal notranslate">v6.0.0 -> v7.2.4 </code></td>
 </tr>
 </table>
 </div>
 </li>
        <li> <span class="li-head">cache_mem_permille</span> - Maximum permille of available memory allocated to caching (1 - 150). <span class="li-normal">type: int</span>
 <a id='label4' href="javascript:ContentClick('label5', 'label4');" onmouseover="ContentPreview('label5');" onmouseout="ContentUnpreview('label5');" title="click to collapse or expand..."> more... </a>
 <div id="label5" style="display:none">
 <table border="1">
 <tr>
 <td></td>
 <td colspan="1">Supported Version Ranges</td>
 </tr>
 <tr>
 <td>cache_mem_permille</td>
 <td><code class="docutils literal notranslate">v7.4.0 -> 7.6.0 </code></td>
 </tr>
 </table>
 </div>
 </li>
        <li> <span class="li-head">cache_mode</span> - Cache entry expiration mode. <span class="li-normal">type: str</span> <span class="li-normal">choices: ttl, db-ver</span>
 <a id='label6' href="javascript:ContentClick('label7', 'label6');" onmouseover="ContentPreview('label7');" onmouseout="ContentUnpreview('label7');" title="click to collapse or expand..."> more... </a>
 <div id="label7" style="display:none">
 <table border="1">
 <tr>
 <td></td>
 <td colspan="1">Supported Version Ranges</td>
 </tr>
 <tr>
 <td>cache_mode</td>
 <td><code class="docutils literal notranslate">v6.0.0 -> 7.6.0 </code></td>
 </tr>
 <tr>
 <td>[ttl]</td>
 <td><code class="docutils literal notranslate">v6.0.0 -> 7.6.0</code></td>
 <tr>
 <td>[db-ver]</td>
 <td><code class="docutils literal notranslate">v6.0.0 -> 7.6.0</code></td>
 </table>
 </div>
 </li>
        <li> <span class="li-head">cache_prefix_match</span> - Enable/disable prefix matching in the cache. <span class="li-normal">type: str</span> <span class="li-normal">choices: enable, disable</span>
 <a id='label8' href="javascript:ContentClick('label9', 'label8');" onmouseover="ContentPreview('label9');" onmouseout="ContentUnpreview('label9');" title="click to collapse or expand..."> more... </a>
 <div id="label9" style="display:none">
 <table border="1">
 <tr>
 <td></td>
 <td colspan="1">Supported Version Ranges</td>
 </tr>
 <tr>
 <td>cache_prefix_match</td>
 <td><code class="docutils literal notranslate">v6.0.0 -> 7.6.0 </code></td>
 </tr>
 <tr>
 <td>[enable]</td>
 <td><code class="docutils literal notranslate">v6.0.0 -> 7.6.0</code></td>
 <tr>
 <td>[disable]</td>
 <td><code class="docutils literal notranslate">v6.0.0 -> 7.6.0</code></td>
 </table>
 </div>
 </li>
        <li> <span class="li-head">close_ports</span> - Close ports used for HTTP/HTTPS override authentication and disable user overrides. <span class="li-normal">type: str</span> <span class="li-normal">choices: enable, disable</span>
 <a id='label10' href="javascript:ContentClick('label11', 'label10');" onmouseover="ContentPreview('label11');" onmouseout="ContentUnpreview('label11');" title="click to collapse or expand..."> more... </a>
 <div id="label11" style="display:none">
 <table border="1">
 <tr>
 <td></td>
 <td colspan="1">Supported Version Ranges</td>
 </tr>
 <tr>
 <td>close_ports</td>
 <td><code class="docutils literal notranslate">v6.0.0 -> 7.6.0 </code></td>
 </tr>
 <tr>
 <td>[enable]</td>
 <td><code class="docutils literal notranslate">v6.0.0 -> 7.6.0</code></td>
 <tr>
 <td>[disable]</td>
 <td><code class="docutils literal notranslate">v6.0.0 -> 7.6.0</code></td>
 </table>
 </div>
 </li>
        <li> <span class="li-head">embed_image</span> - Enable/disable embedding images into replacement messages . <span class="li-normal">type: str</span> <span class="li-normal">choices: enable, disable</span>
 <a id='label12' href="javascript:ContentClick('label13', 'label12');" onmouseover="ContentPreview('label13');" onmouseout="ContentUnpreview('label13');" title="click to collapse or expand..."> more... </a>
 <div id="label13" style="display:none">
 <table border="1">
 <tr>
 <td></td>
 <td colspan="1">Supported Version Ranges</td>
 </tr>
 <tr>
 <td>embed_image</td>
 <td><code class="docutils literal notranslate">v7.2.4 -> 7.6.0 </code></td>
 </tr>
 <tr>
 <td>[enable]</td>
 <td><code class="docutils literal notranslate">v7.2.4 -> 7.6.0</code></td>
 <tr>
 <td>[disable]</td>
 <td><code class="docutils literal notranslate">v7.2.4 -> 7.6.0</code></td>
 </table>
 </div>
 </li>
        <li> <span class="li-head">ovrd_auth_https</span> - Enable/disable use of HTTPS for override authentication. <span class="li-normal">type: str</span> <span class="li-normal">choices: enable, disable</span>
 <a id='label14' href="javascript:ContentClick('label15', 'label14');" onmouseover="ContentPreview('label15');" onmouseout="ContentUnpreview('label15');" title="click to collapse or expand..."> more... </a>
 <div id="label15" style="display:none">
 <table border="1">
 <tr>
 <td></td>
 <td colspan="1">Supported Version Ranges</td>
 </tr>
 <tr>
 <td>ovrd_auth_https</td>
 <td><code class="docutils literal notranslate">v6.0.0 -> 7.6.0 </code></td>
 </tr>
 <tr>
 <td>[enable]</td>
 <td><code class="docutils literal notranslate">v6.0.0 -> 7.6.0</code></td>
 <tr>
 <td>[disable]</td>
 <td><code class="docutils literal notranslate">v6.0.0 -> 7.6.0</code></td>
 </table>
 </div>
 </li>
        <li> <span class="li-head">ovrd_auth_port</span> - Port to use for FortiGuard Web Filter override authentication. <span class="li-normal">type: int</span>
 <a id='label16' href="javascript:ContentClick('label17', 'label16');" onmouseover="ContentPreview('label17');" onmouseout="ContentUnpreview('label17');" title="click to collapse or expand..."> more... </a>
 <div id="label17" style="display:none">
 <table border="1">
 <tr>
 <td></td>
 <td colspan="2">Supported Version Ranges</td>
 </tr>
 <tr>
 <td>ovrd_auth_port</td>
 <td><code class="docutils literal notranslate">v6.0.0 -> v6.0.11 </code></td>
 <td><code class="docutils literal notranslate">v6.2.3 -> v6.2.3 </code></td>
 </tr>
 </table>
 </div>
 </li>
        <li> <span class="li-head">ovrd_auth_port_http</span> - Port to use for FortiGuard Web Filter HTTP override authentication. <span class="li-normal">type: int</span>
 <a id='label18' href="javascript:ContentClick('label19', 'label18');" onmouseover="ContentPreview('label19');" onmouseout="ContentUnpreview('label19');" title="click to collapse or expand..."> more... </a>
 <div id="label19" style="display:none">
 <table border="1">
 <tr>
 <td></td>
 <td colspan="1">Supported Version Ranges</td>
 </tr>
 <tr>
 <td>ovrd_auth_port_http</td>
 <td><code class="docutils literal notranslate">v6.0.0 -> 7.6.0 </code></td>
 </tr>
 </table>
 </div>
 </li>
        <li> <span class="li-head">ovrd_auth_port_https</span> - Port to use for FortiGuard Web Filter HTTPS override authentication in proxy mode. <span class="li-normal">type: int</span>
 <a id='label20' href="javascript:ContentClick('label21', 'label20');" onmouseover="ContentPreview('label21');" onmouseout="ContentUnpreview('label21');" title="click to collapse or expand..."> more... </a>
 <div id="label21" style="display:none">
 <table border="1">
 <tr>
 <td></td>
 <td colspan="1">Supported Version Ranges</td>
 </tr>
 <tr>
 <td>ovrd_auth_port_https</td>
 <td><code class="docutils literal notranslate">v6.0.0 -> 7.6.0 </code></td>
 </tr>
 </table>
 </div>
 </li>
        <li> <span class="li-head">ovrd_auth_port_https_flow</span> - Port to use for FortiGuard Web Filter HTTPS override authentication in flow mode. <span class="li-normal">type: int</span>
 <a id='label22' href="javascript:ContentClick('label23', 'label22');" onmouseover="ContentPreview('label23');" onmouseout="ContentUnpreview('label23');" title="click to collapse or expand..."> more... </a>
 <div id="label23" style="display:none">
 <table border="1">
 <tr>
 <td></td>
 <td colspan="1">Supported Version Ranges</td>
 </tr>
 <tr>
 <td>ovrd_auth_port_https_flow</td>
 <td><code class="docutils literal notranslate">v6.2.0 -> 7.6.0 </code></td>
 </tr>
 </table>
 </div>
 </li>
        <li> <span class="li-head">ovrd_auth_port_warning</span> - Port to use for FortiGuard Web Filter Warning override authentication. <span class="li-normal">type: int</span>
 <a id='label24' href="javascript:ContentClick('label25', 'label24');" onmouseover="ContentPreview('label25');" onmouseout="ContentUnpreview('label25');" title="click to collapse or expand..."> more... </a>
 <div id="label25" style="display:none">
 <table border="1">
 <tr>
 <td></td>
 <td colspan="1">Supported Version Ranges</td>
 </tr>
 <tr>
 <td>ovrd_auth_port_warning</td>
 <td><code class="docutils literal notranslate">v6.0.0 -> 7.6.0 </code></td>
 </tr>
 </table>
 </div>
 </li>
        <li> <span class="li-head">request_packet_size_limit</span> - Limit size of URL request packets sent to FortiGuard server (0 for default). <span class="li-normal">type: int</span>
 <a id='label26' href="javascript:ContentClick('label27', 'label26');" onmouseover="ContentPreview('label27');" onmouseout="ContentUnpreview('label27');" title="click to collapse or expand..."> more... </a>
 <div id="label27" style="display:none">
 <table border="1">
 <tr>
 <td></td>
 <td colspan="1">Supported Version Ranges</td>
 </tr>
 <tr>
 <td>request_packet_size_limit</td>
 <td><code class="docutils literal notranslate">v6.0.0 -> 7.6.0 </code></td>
 </tr>
 </table>
 </div>
 </li>
        <li> <span class="li-head">warn_auth_https</span> - Enable/disable use of HTTPS for warning and authentication. <span class="li-normal">type: str</span> <span class="li-normal">choices: enable, disable</span>
 <a id='label28' href="javascript:ContentClick('label29', 'label28');" onmouseover="ContentPreview('label29');" onmouseout="ContentUnpreview('label29');" title="click to collapse or expand..."> more... </a>
 <div id="label29" style="display:none">
 <table border="1">
 <tr>
 <td></td>
 <td colspan="1">Supported Version Ranges</td>
 </tr>
 <tr>
 <td>warn_auth_https</td>
 <td><code class="docutils literal notranslate">v6.0.0 -> 7.6.0 </code></td>
 </tr>
 <tr>
 <td>[enable]</td>
 <td><code class="docutils literal notranslate">v6.0.0 -> 7.6.0</code></td>
 <tr>
 <td>[disable]</td>
 <td><code class="docutils literal notranslate">v6.0.0 -> 7.6.0</code></td>
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
    
    - name: Configure FortiGuard Web Filter service.
      fortinet.fortios.fortios_webfilter_fortiguard:
          vdom: "{{ vdom }}"
          webfilter_fortiguard:
              cache_mem_percent: "2"
              cache_mem_permille: "1"
              cache_mode: "ttl"
              cache_prefix_match: "enable"
              close_ports: "enable"
              embed_image: "enable"
              ovrd_auth_https: "enable"
              ovrd_auth_port: "32767"
              ovrd_auth_port_http: "8008"
              ovrd_auth_port_https: "8010"
              ovrd_auth_port_https_flow: "8015"
              ovrd_auth_port_warning: "8020"
              request_packet_size_limit: "0"
              warn_auth_https: "enable"


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
