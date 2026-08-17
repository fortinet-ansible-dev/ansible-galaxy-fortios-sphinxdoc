:source: fortios_llm_proxy.py

:orphan:

.. fortios_llm_proxy:

fortios_llm_proxy -- Configure LLM Proxy in Fortinet's FortiOS and FortiGate.
+++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++

.. versionadded:: 2.0.0

.. contents::
   :local:
   :depth: 1


Synopsis
--------
- This module is able to configure a FortiGate or FortiOS (FOS) device by allowing the user to set and modify llm feature and proxy category. Examples include all parameters and values need to be adjusted to datasources before usage. Tested with FOS v6.0.0



Requirements
------------
The below requirements are needed on the host that executes this module.

- ansible>=2.16


Tips
----
Using member operation to add an element to an existing object.

FortiOS Version Compatibility
-----------------------------
Supported Version Ranges: v8.0.0


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
    <li> <span class="li-head">llm_proxy</span> - Configure LLM Proxy. <span class="li-normal">type: dict</span>
 <a id='label0' href="javascript:ContentClick('label1', 'label0');" onmouseover="ContentPreview('label1');" onmouseout="ContentUnpreview('label1');" title="click to collapse or expand..."> more... </a>
 <div id="label1" style="display:none">
 <table border="1">
 <tr>
 <td></td><td colspan="1">Supported Version Ranges</td>
 </tr>
 <tr>
 <td>llm_proxy</td>
 <td><code class="docutils literal notranslate">v8.0.0 -> 8.0.0 </code></td>
 </tr>
 </table>
 </div>
 </li>
        <ul class="ul-self">
        <li> <span class="li-head">hostname</span> - hostname. Source firewall.address.name. <span class="li-normal">type: str</span>
 <a id='label2' href="javascript:ContentClick('label3', 'label2');" onmouseover="ContentPreview('label3');" onmouseout="ContentUnpreview('label3');" title="click to collapse or expand..."> more... </a>
 <div id="label3" style="display:none">
 <table border="1">
 <tr>
 <td></td>
 <td colspan="1">Supported Version Ranges</td>
 </tr>
 <tr>
 <td>hostname</td>
 <td><code class="docutils literal notranslate">v8.0.0 -> 8.0.0 </code></td>
 </tr>
 </table>
 </div>
 </li>
        <li> <span class="li-head">incoming_http_port</span> - LLM Proxy HTTP incoming port. <span class="li-normal">type: int</span>
 <a id='label4' href="javascript:ContentClick('label5', 'label4');" onmouseover="ContentPreview('label5');" onmouseout="ContentUnpreview('label5');" title="click to collapse or expand..."> more... </a>
 <div id="label5" style="display:none">
 <table border="1">
 <tr>
 <td></td>
 <td colspan="1">Supported Version Ranges</td>
 </tr>
 <tr>
 <td>incoming_http_port</td>
 <td><code class="docutils literal notranslate">v8.0.0 -> 8.0.0 </code></td>
 </tr>
 </table>
 </div>
 </li>
        <li> <span class="li-head">incoming_https_port</span> - LLM Proxy HTTPS incoming port. <span class="li-normal">type: int</span>
 <a id='label6' href="javascript:ContentClick('label7', 'label6');" onmouseover="ContentPreview('label7');" onmouseout="ContentUnpreview('label7');" title="click to collapse or expand..."> more... </a>
 <div id="label7" style="display:none">
 <table border="1">
 <tr>
 <td></td>
 <td colspan="1">Supported Version Ranges</td>
 </tr>
 <tr>
 <td>incoming_https_port</td>
 <td><code class="docutils literal notranslate">v8.0.0 -> 8.0.0 </code></td>
 </tr>
 </table>
 </div>
 </li>
        <li> <span class="li-head">incoming_ip</span> - LLM Proxy incoming IP. <span class="li-normal">type: str</span>
 <a id='label8' href="javascript:ContentClick('label9', 'label8');" onmouseover="ContentPreview('label9');" onmouseout="ContentUnpreview('label9');" title="click to collapse or expand..."> more... </a>
 <div id="label9" style="display:none">
 <table border="1">
 <tr>
 <td></td>
 <td colspan="1">Supported Version Ranges</td>
 </tr>
 <tr>
 <td>incoming_ip</td>
 <td><code class="docutils literal notranslate">v8.0.0 -> 8.0.0 </code></td>
 </tr>
 </table>
 </div>
 </li>
        <li> <span class="li-head">incoming_ip6</span> - LLM Proxy incoming IPv6. <span class="li-normal">type: str</span>
 <a id='label10' href="javascript:ContentClick('label11', 'label10');" onmouseover="ContentPreview('label11');" onmouseout="ContentUnpreview('label11');" title="click to collapse or expand..."> more... </a>
 <div id="label11" style="display:none">
 <table border="1">
 <tr>
 <td></td>
 <td colspan="1">Supported Version Ranges</td>
 </tr>
 <tr>
 <td>incoming_ip6</td>
 <td><code class="docutils literal notranslate">v8.0.0 -> 8.0.0 </code></td>
 </tr>
 </table>
 </div>
 </li>
        <li> <span class="li-head">interface</span> - Name of the interfaces to use LLM Proxy. <span class="li-normal">type: list</span> <span style="font-family:'Courier New'" class="li-required">member_path: interface:name</span>
 <a id='label12' href="javascript:ContentClick('label13', 'label12');" onmouseover="ContentPreview('label13');" onmouseout="ContentUnpreview('label13');" title="click to collapse or expand..."> more... </a>
 <div id="label13" style="display:none">
 <table border="1">
 <tr>
 <td></td><td colspan="1">Supported Version Ranges</td>
 </tr>
 <tr>
 <td>interface</td>
 <td><code class="docutils literal notranslate">v8.0.0 -> 8.0.0 </code></td>
 </tr>
 </table>
 </div>
 </li>
            <ul class="ul-self">
            <li> <span class="li-head">name</span> - Interface list. Source system.interface.name. <span class="li-normal">type: str</span> <span class="li-required">required: true</span>
 <a id='label14' href="javascript:ContentClick('label15', 'label14');" onmouseover="ContentPreview('label15');" onmouseout="ContentUnpreview('label15');" title="click to collapse or expand..."> more... </a>
 <div id="label15" style="display:none">
 <table border="1">
 <tr>
 <td></td>
 <td colspan="1">Supported Version Ranges</td>
 </tr>
 <tr>
 <td>name</td>
 <td><code class="docutils literal notranslate">v8.0.0 -> 8.0.0 </code></td>
 </tr>
 </table>
 </div>
 </li>
            </ul>
        <li> <span class="li-head">ipv6_status</span> - Enable/disable the LLM proxy on IPv6. <span class="li-normal">type: str</span> <span class="li-normal">choices: enable, disable</span>
 <a id='label16' href="javascript:ContentClick('label17', 'label16');" onmouseover="ContentPreview('label17');" onmouseout="ContentUnpreview('label17');" title="click to collapse or expand..."> more... </a>
 <div id="label17" style="display:none">
 <table border="1">
 <tr>
 <td></td>
 <td colspan="1">Supported Version Ranges</td>
 </tr>
 <tr>
 <td>ipv6_status</td>
 <td><code class="docutils literal notranslate">v8.0.0 -> 8.0.0 </code></td>
 </tr>
 <tr>
 <td>[enable]</td>
 <td><code class="docutils literal notranslate">v8.0.0 -> 8.0.0</code></td>
 <tr>
 <td>[disable]</td>
 <td><code class="docutils literal notranslate">v8.0.0 -> 8.0.0</code></td>
 </table>
 </div>
 </li>
        <li> <span class="li-head">name</span> - LLM Proxy name. <span class="li-normal">type: str</span> <span class="li-required">required: true</span>
 <a id='label18' href="javascript:ContentClick('label19', 'label18');" onmouseover="ContentPreview('label19');" onmouseout="ContentUnpreview('label19');" title="click to collapse or expand..."> more... </a>
 <div id="label19" style="display:none">
 <table border="1">
 <tr>
 <td></td>
 <td colspan="1">Supported Version Ranges</td>
 </tr>
 <tr>
 <td>name</td>
 <td><code class="docutils literal notranslate">v8.0.0 -> 8.0.0 </code></td>
 </tr>
 </table>
 </div>
 </li>
        <li> <span class="li-head">protocol</span> - Supported protocols. <span class="li-normal">type: list</span> <span class="li-normal">choices: http, https</span>
 <a id='label20' href="javascript:ContentClick('label21', 'label20');" onmouseover="ContentPreview('label21');" onmouseout="ContentUnpreview('label21');" title="click to collapse or expand..."> more... </a>
 <div id="label21" style="display:none">
 <table border="1">
 <tr>
 <td></td>
 <td colspan="1">Supported Version Ranges</td>
 </tr>
 <tr>
 <td>protocol</td>
 <td><code class="docutils literal notranslate">v8.0.0 -> 8.0.0 </code></td>
 </tr>
 <tr>
 <td>[http]</td>
 <td><code class="docutils literal notranslate">v8.0.0 -> 8.0.0</code></td>
 <tr>
 <td>[https]</td>
 <td><code class="docutils literal notranslate">v8.0.0 -> 8.0.0</code></td>
 </table>
 </div>
 </li>
        <li> <span class="li-head">srv_pool_max_concurrent_request</span> - Maximum number of concurrent requests that a server can handle . <span class="li-normal">type: int</span>
 <a id='label22' href="javascript:ContentClick('label23', 'label22');" onmouseover="ContentPreview('label23');" onmouseout="ContentUnpreview('label23');" title="click to collapse or expand..."> more... </a>
 <div id="label23" style="display:none">
 <table border="1">
 <tr>
 <td></td>
 <td colspan="1">Supported Version Ranges</td>
 </tr>
 <tr>
 <td>srv_pool_max_concurrent_request</td>
 <td><code class="docutils literal notranslate">v8.0.0 -> 8.0.0 </code></td>
 </tr>
 </table>
 </div>
 </li>
        <li> <span class="li-head">srv_pool_max_request</span> - Maximum number of requests that a server can handle before disconnecting sessions . <span class="li-normal">type: int</span>
 <a id='label24' href="javascript:ContentClick('label25', 'label24');" onmouseover="ContentPreview('label25');" onmouseout="ContentUnpreview('label25');" title="click to collapse or expand..."> more... </a>
 <div id="label25" style="display:none">
 <table border="1">
 <tr>
 <td></td>
 <td colspan="1">Supported Version Ranges</td>
 </tr>
 <tr>
 <td>srv_pool_max_request</td>
 <td><code class="docutils literal notranslate">v8.0.0 -> 8.0.0 </code></td>
 </tr>
 </table>
 </div>
 </li>
        <li> <span class="li-head">srv_pool_ttl</span> - Time-to-live for idle connections to servers. <span class="li-normal">type: int</span>
 <a id='label26' href="javascript:ContentClick('label27', 'label26');" onmouseover="ContentPreview('label27');" onmouseout="ContentUnpreview('label27');" title="click to collapse or expand..."> more... </a>
 <div id="label27" style="display:none">
 <table border="1">
 <tr>
 <td></td>
 <td colspan="1">Supported Version Ranges</td>
 </tr>
 <tr>
 <td>srv_pool_ttl</td>
 <td><code class="docutils literal notranslate">v8.0.0 -> 8.0.0 </code></td>
 </tr>
 </table>
 </div>
 </li>
        <li> <span class="li-head">ssl_certificate</span> - Name of the certificates to use for SSL handshake. <span class="li-normal">type: list</span> <span style="font-family:'Courier New'" class="li-required">member_path: ssl_certificate:name</span>
 <a id='label28' href="javascript:ContentClick('label29', 'label28');" onmouseover="ContentPreview('label29');" onmouseout="ContentUnpreview('label29');" title="click to collapse or expand..."> more... </a>
 <div id="label29" style="display:none">
 <table border="1">
 <tr>
 <td></td><td colspan="1">Supported Version Ranges</td>
 </tr>
 <tr>
 <td>ssl_certificate</td>
 <td><code class="docutils literal notranslate">v8.0.0 -> 8.0.0 </code></td>
 </tr>
 </table>
 </div>
 </li>
            <ul class="ul-self">
            <li> <span class="li-head">name</span> - Certificate list. Source vpn.certificate.local.name. <span class="li-normal">type: str</span> <span class="li-required">required: true</span>
 <a id='label30' href="javascript:ContentClick('label31', 'label30');" onmouseover="ContentPreview('label31');" onmouseout="ContentUnpreview('label31');" title="click to collapse or expand..."> more... </a>
 <div id="label31" style="display:none">
 <table border="1">
 <tr>
 <td></td>
 <td colspan="1">Supported Version Ranges</td>
 </tr>
 <tr>
 <td>name</td>
 <td><code class="docutils literal notranslate">v8.0.0 -> 8.0.0 </code></td>
 </tr>
 </table>
 </div>
 </li>
            </ul>
        <li> <span class="li-head">ssl_max_version</span> - Highest SSL/TLS version acceptable from a client. <span class="li-normal">type: str</span> <span class="li-normal">choices: ssl-3.0, tls-1.0, tls-1.1, tls-1.2, tls-1.3</span>
 <a id='label32' href="javascript:ContentClick('label33', 'label32');" onmouseover="ContentPreview('label33');" onmouseout="ContentUnpreview('label33');" title="click to collapse or expand..."> more... </a>
 <div id="label33" style="display:none">
 <table border="1">
 <tr>
 <td></td>
 <td colspan="1">Supported Version Ranges</td>
 </tr>
 <tr>
 <td>ssl_max_version</td>
 <td><code class="docutils literal notranslate">v8.0.0 -> 8.0.0 </code></td>
 </tr>
 <tr>
 <td>[ssl-3.0]</td>
 <td><code class="docutils literal notranslate">v8.0.0 -> 8.0.0</code></td>
 <tr>
 <td>[tls-1.0]</td>
 <td><code class="docutils literal notranslate">v8.0.0 -> 8.0.0</code></td>
 <tr>
 <td>[tls-1.1]</td>
 <td><code class="docutils literal notranslate">v8.0.0 -> 8.0.0</code></td>
 <tr>
 <td>[tls-1.2]</td>
 <td><code class="docutils literal notranslate">v8.0.0 -> 8.0.0</code></td>
 <tr>
 <td>[tls-1.3]</td>
 <td><code class="docutils literal notranslate">v8.0.0 -> 8.0.0</code></td>
 </table>
 </div>
 </li>
        <li> <span class="li-head">ssl_min_version</span> - Lowest SSL/TLS version acceptable from a client. <span class="li-normal">type: str</span> <span class="li-normal">choices: ssl-3.0, tls-1.0, tls-1.1, tls-1.2, tls-1.3</span>
 <a id='label34' href="javascript:ContentClick('label35', 'label34');" onmouseover="ContentPreview('label35');" onmouseout="ContentUnpreview('label35');" title="click to collapse or expand..."> more... </a>
 <div id="label35" style="display:none">
 <table border="1">
 <tr>
 <td></td>
 <td colspan="1">Supported Version Ranges</td>
 </tr>
 <tr>
 <td>ssl_min_version</td>
 <td><code class="docutils literal notranslate">v8.0.0 -> 8.0.0 </code></td>
 </tr>
 <tr>
 <td>[ssl-3.0]</td>
 <td><code class="docutils literal notranslate">v8.0.0 -> 8.0.0</code></td>
 <tr>
 <td>[tls-1.0]</td>
 <td><code class="docutils literal notranslate">v8.0.0 -> 8.0.0</code></td>
 <tr>
 <td>[tls-1.1]</td>
 <td><code class="docutils literal notranslate">v8.0.0 -> 8.0.0</code></td>
 <tr>
 <td>[tls-1.2]</td>
 <td><code class="docutils literal notranslate">v8.0.0 -> 8.0.0</code></td>
 <tr>
 <td>[tls-1.3]</td>
 <td><code class="docutils literal notranslate">v8.0.0 -> 8.0.0</code></td>
 </table>
 </div>
 </li>
        <li> <span class="li-head">status</span> - Enable/disable the LLM proxy. <span class="li-normal">type: str</span> <span class="li-normal">choices: enable, disable</span>
 <a id='label36' href="javascript:ContentClick('label37', 'label36');" onmouseover="ContentPreview('label37');" onmouseout="ContentUnpreview('label37');" title="click to collapse or expand..."> more... </a>
 <div id="label37" style="display:none">
 <table border="1">
 <tr>
 <td></td>
 <td colspan="1">Supported Version Ranges</td>
 </tr>
 <tr>
 <td>status</td>
 <td><code class="docutils literal notranslate">v8.0.0 -> 8.0.0 </code></td>
 </tr>
 <tr>
 <td>[enable]</td>
 <td><code class="docutils literal notranslate">v8.0.0 -> 8.0.0</code></td>
 <tr>
 <td>[disable]</td>
 <td><code class="docutils literal notranslate">v8.0.0 -> 8.0.0</code></td>
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
    
    - name: Configure LLM Proxy.
      fortinet.fortios.fortios_llm_proxy:
          vdom: "{{ vdom }}"
          state: "present"
          access_token: "<your_own_value>"
          llm_proxy:
              hostname: "myhostname (source firewall.address.name)"
              incoming_http_port: "8098"
              incoming_https_port: "8099"
              incoming_ip: "<your_own_value>"
              incoming_ip6: "<your_own_value>"
              interface:
                  -
                      name: "default_name_9 (source system.interface.name)"
              ipv6_status: "enable"
              name: "default_name_11"
              protocol: "http"
              srv_pool_max_concurrent_request: "0"
              srv_pool_max_request: "0"
              srv_pool_ttl: "30"
              ssl_certificate:
                  -
                      name: "default_name_17 (source vpn.certificate.local.name)"
              ssl_max_version: "ssl-3.0"
              ssl_min_version: "ssl-3.0"
              status: "enable"


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
