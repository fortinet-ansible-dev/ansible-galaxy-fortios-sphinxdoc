:source: fortios_router_static6.py

:orphan:

.. fortios_router_static6:

fortios_router_static6 -- Configure IPv6 static routing tables in Fortinet's FortiOS and FortiGate.
+++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++

.. versionadded:: 2.0.0

.. contents::
   :local:
   :depth: 1


Synopsis
--------
- This module is able to configure a FortiGate or FortiOS (FOS) device by allowing the user to set and modify router feature and static6 category. Examples include all parameters and values need to be adjusted to datasources before usage. Tested with FOS v6.0.0



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
    <li> <span class="li-head">router_static6</span> - Configure IPv6 static routing tables. <span class="li-normal">type: dict</span>
 <a id='label0' href="javascript:ContentClick('label1', 'label0');" onmouseover="ContentPreview('label1');" onmouseout="ContentUnpreview('label1');" title="click to collapse or expand..."> more... </a>
 <div id="label1" style="display:none">
 <table border="1">
 <tr>
 <td></td><td colspan="1">Supported Version Ranges</td>
 </tr>
 <tr>
 <td>router_static6</td>
 <td><code class="docutils literal notranslate">v6.0.0 -> 7.6.2 </code></td>
 </tr>
 </table>
 </div>
 </li>
        <ul class="ul-self">
        <li> <span class="li-head">bfd</span> - Enable/disable Bidirectional Forwarding Detection (BFD). <span class="li-normal">type: str</span> <span class="li-normal">choices: enable, disable</span>
 <a id='label2' href="javascript:ContentClick('label3', 'label2');" onmouseover="ContentPreview('label3');" onmouseout="ContentUnpreview('label3');" title="click to collapse or expand..."> more... </a>
 <div id="label3" style="display:none">
 <table border="1">
 <tr>
 <td></td>
 <td colspan="1">Supported Version Ranges</td>
 </tr>
 <tr>
 <td>bfd</td>
 <td><code class="docutils literal notranslate">v6.0.0 -> 7.6.2 </code></td>
 </tr>
 <tr>
 <td>[enable]</td>
 <td><code class="docutils literal notranslate">v6.0.0 -> 7.6.2</code></td>
 <tr>
 <td>[disable]</td>
 <td><code class="docutils literal notranslate">v6.0.0 -> 7.6.2</code></td>
 </table>
 </div>
 </li>
        <li> <span class="li-head">blackhole</span> - Enable/disable black hole. <span class="li-normal">type: str</span> <span class="li-normal">choices: enable, disable</span>
 <a id='label4' href="javascript:ContentClick('label5', 'label4');" onmouseover="ContentPreview('label5');" onmouseout="ContentUnpreview('label5');" title="click to collapse or expand..."> more... </a>
 <div id="label5" style="display:none">
 <table border="1">
 <tr>
 <td></td>
 <td colspan="1">Supported Version Ranges</td>
 </tr>
 <tr>
 <td>blackhole</td>
 <td><code class="docutils literal notranslate">v6.0.0 -> 7.6.2 </code></td>
 </tr>
 <tr>
 <td>[enable]</td>
 <td><code class="docutils literal notranslate">v6.0.0 -> 7.6.2</code></td>
 <tr>
 <td>[disable]</td>
 <td><code class="docutils literal notranslate">v6.0.0 -> 7.6.2</code></td>
 </table>
 </div>
 </li>
        <li> <span class="li-head">comment</span> - Optional comments. <span class="li-normal">type: str</span>
 <a id='label6' href="javascript:ContentClick('label7', 'label6');" onmouseover="ContentPreview('label7');" onmouseout="ContentUnpreview('label7');" title="click to collapse or expand..."> more... </a>
 <div id="label7" style="display:none">
 <table border="1">
 <tr>
 <td></td>
 <td colspan="1">Supported Version Ranges</td>
 </tr>
 <tr>
 <td>comment</td>
 <td><code class="docutils literal notranslate">v6.0.0 -> 7.6.2 </code></td>
 </tr>
 </table>
 </div>
 </li>
        <li> <span class="li-head">device</span> - Gateway out interface or tunnel. Source system.interface.name. <span class="li-normal">type: str</span>
 <a id='label8' href="javascript:ContentClick('label9', 'label8');" onmouseover="ContentPreview('label9');" onmouseout="ContentUnpreview('label9');" title="click to collapse or expand..."> more... </a>
 <div id="label9" style="display:none">
 <table border="1">
 <tr>
 <td></td>
 <td colspan="1">Supported Version Ranges</td>
 </tr>
 <tr>
 <td>device</td>
 <td><code class="docutils literal notranslate">v6.0.0 -> 7.6.2 </code></td>
 </tr>
 </table>
 </div>
 </li>
        <li> <span class="li-head">devindex</span> - Device index (0 - 4294967295). <span class="li-normal">type: int</span>
 <a id='label10' href="javascript:ContentClick('label11', 'label10');" onmouseover="ContentPreview('label11');" onmouseout="ContentUnpreview('label11');" title="click to collapse or expand..."> more... </a>
 <div id="label11" style="display:none">
 <table border="1">
 <tr>
 <td></td>
 <td colspan="1">Supported Version Ranges</td>
 </tr>
 <tr>
 <td>devindex</td>
 <td><code class="docutils literal notranslate">v6.0.0 -> 7.6.2 </code></td>
 </tr>
 </table>
 </div>
 </li>
        <li> <span class="li-head">distance</span> - Administrative distance (1 - 255). <span class="li-normal">type: int</span>
 <a id='label12' href="javascript:ContentClick('label13', 'label12');" onmouseover="ContentPreview('label13');" onmouseout="ContentUnpreview('label13');" title="click to collapse or expand..."> more... </a>
 <div id="label13" style="display:none">
 <table border="1">
 <tr>
 <td></td>
 <td colspan="1">Supported Version Ranges</td>
 </tr>
 <tr>
 <td>distance</td>
 <td><code class="docutils literal notranslate">v6.0.0 -> 7.6.2 </code></td>
 </tr>
 </table>
 </div>
 </li>
        <li> <span class="li-head">dst</span> - Destination IPv6 prefix. <span class="li-normal">type: str</span>
 <a id='label14' href="javascript:ContentClick('label15', 'label14');" onmouseover="ContentPreview('label15');" onmouseout="ContentUnpreview('label15');" title="click to collapse or expand..."> more... </a>
 <div id="label15" style="display:none">
 <table border="1">
 <tr>
 <td></td>
 <td colspan="1">Supported Version Ranges</td>
 </tr>
 <tr>
 <td>dst</td>
 <td><code class="docutils literal notranslate">v6.0.0 -> 7.6.2 </code></td>
 </tr>
 </table>
 </div>
 </li>
        <li> <span class="li-head">dstaddr</span> - Name of firewall address or address group. Source firewall.address6.name firewall.addrgrp6.name. <span class="li-normal">type: str</span>
 <a id='label16' href="javascript:ContentClick('label17', 'label16');" onmouseover="ContentPreview('label17');" onmouseout="ContentUnpreview('label17');" title="click to collapse or expand..."> more... </a>
 <div id="label17" style="display:none">
 <table border="1">
 <tr>
 <td></td>
 <td colspan="1">Supported Version Ranges</td>
 </tr>
 <tr>
 <td>dstaddr</td>
 <td><code class="docutils literal notranslate">v7.2.1 -> 7.6.2 </code></td>
 </tr>
 </table>
 </div>
 </li>
        <li> <span class="li-head">dynamic_gateway</span> - Enable use of dynamic gateway retrieved from Router Advertisement (RA). <span class="li-normal">type: str</span> <span class="li-normal">choices: enable, disable</span>
 <a id='label18' href="javascript:ContentClick('label19', 'label18');" onmouseover="ContentPreview('label19');" onmouseout="ContentUnpreview('label19');" title="click to collapse or expand..."> more... </a>
 <div id="label19" style="display:none">
 <table border="1">
 <tr>
 <td></td>
 <td colspan="1">Supported Version Ranges</td>
 </tr>
 <tr>
 <td>dynamic_gateway</td>
 <td><code class="docutils literal notranslate">v7.0.0 -> 7.6.2 </code></td>
 </tr>
 <tr>
 <td>[enable]</td>
 <td><code class="docutils literal notranslate">v7.0.0 -> 7.6.2</code></td>
 <tr>
 <td>[disable]</td>
 <td><code class="docutils literal notranslate">v7.0.0 -> 7.6.2</code></td>
 </table>
 </div>
 </li>
        <li> <span class="li-head">gateway</span> - IPv6 address of the gateway. <span class="li-normal">type: str</span>
 <a id='label20' href="javascript:ContentClick('label21', 'label20');" onmouseover="ContentPreview('label21');" onmouseout="ContentUnpreview('label21');" title="click to collapse or expand..."> more... </a>
 <div id="label21" style="display:none">
 <table border="1">
 <tr>
 <td></td>
 <td colspan="1">Supported Version Ranges</td>
 </tr>
 <tr>
 <td>gateway</td>
 <td><code class="docutils literal notranslate">v6.0.0 -> 7.6.2 </code></td>
 </tr>
 </table>
 </div>
 </li>
        <li> <span class="li-head">link_monitor_exempt</span> - Enable/disable withdrawal of this static route when link monitor or health check is down. <span class="li-normal">type: str</span> <span class="li-normal">choices: enable, disable</span>
 <a id='label22' href="javascript:ContentClick('label23', 'label22');" onmouseover="ContentPreview('label23');" onmouseout="ContentUnpreview('label23');" title="click to collapse or expand..."> more... </a>
 <div id="label23" style="display:none">
 <table border="1">
 <tr>
 <td></td>
 <td colspan="1">Supported Version Ranges</td>
 </tr>
 <tr>
 <td>link_monitor_exempt</td>
 <td><code class="docutils literal notranslate">v6.2.0 -> 7.6.2 </code></td>
 </tr>
 <tr>
 <td>[enable]</td>
 <td><code class="docutils literal notranslate">v6.2.0 -> 7.6.2</code></td>
 <tr>
 <td>[disable]</td>
 <td><code class="docutils literal notranslate">v6.2.0 -> 7.6.2</code></td>
 </table>
 </div>
 </li>
        <li> <span class="li-head">priority</span> - Administrative priority (1 - 65535). <span class="li-normal">type: int</span>
 <a id='label24' href="javascript:ContentClick('label25', 'label24');" onmouseover="ContentPreview('label25');" onmouseout="ContentUnpreview('label25');" title="click to collapse or expand..."> more... </a>
 <div id="label25" style="display:none">
 <table border="1">
 <tr>
 <td></td>
 <td colspan="1">Supported Version Ranges</td>
 </tr>
 <tr>
 <td>priority</td>
 <td><code class="docutils literal notranslate">v6.0.0 -> 7.6.2 </code></td>
 </tr>
 </table>
 </div>
 </li>
        <li> <span class="li-head">sdwan</span> - Enable/disable egress through the SD-WAN. <span class="li-normal">type: str</span> <span class="li-normal">choices: enable, disable</span>
 <a id='label26' href="javascript:ContentClick('label27', 'label26');" onmouseover="ContentPreview('label27');" onmouseout="ContentUnpreview('label27');" title="click to collapse or expand..."> more... </a>
 <div id="label27" style="display:none">
 <table border="1">
 <tr>
 <td></td>
 <td colspan="1">Supported Version Ranges</td>
 </tr>
 <tr>
 <td>sdwan</td>
 <td><code class="docutils literal notranslate">v6.4.0 -> v7.0.0 </code></td>
 </tr>
 <tr>
 <td>[enable]</td>
 <td><code class="docutils literal notranslate">v6.4.0 -> v7.0.0</code></td>
 <tr>
 <td>[disable]</td>
 <td><code class="docutils literal notranslate">v6.4.0 -> v7.0.0</code></td>
 </table>
 </div>
 </li>
        <li> <span class="li-head">sdwan_zone</span> - Choose SD-WAN Zone. <span class="li-normal">type: list</span> <span style="font-family:'Courier New'" class="li-required">member_path: sdwan_zone:name</span>
 <a id='label28' href="javascript:ContentClick('label29', 'label28');" onmouseover="ContentPreview('label29');" onmouseout="ContentUnpreview('label29');" title="click to collapse or expand..."> more... </a>
 <div id="label29" style="display:none">
 <table border="1">
 <tr>
 <td></td><td colspan="1">Supported Version Ranges</td>
 </tr>
 <tr>
 <td>sdwan_zone</td>
 <td><code class="docutils literal notranslate">v7.0.1 -> 7.6.2 </code></td>
 </tr>
 </table>
 </div>
 </li>
            <ul class="ul-self">
            <li> <span class="li-head">name</span> - SD-WAN zone name. Source system.sdwan.zone.name. <span class="li-normal">type: str</span> <span class="li-required">required: true</span>
 <a id='label30' href="javascript:ContentClick('label31', 'label30');" onmouseover="ContentPreview('label31');" onmouseout="ContentUnpreview('label31');" title="click to collapse or expand..."> more... </a>
 <div id="label31" style="display:none">
 <table border="1">
 <tr>
 <td></td>
 <td colspan="1">Supported Version Ranges</td>
 </tr>
 <tr>
 <td>name</td>
 <td><code class="docutils literal notranslate">v7.0.1 -> 7.6.2 </code></td>
 </tr>
 </table>
 </div>
 </li>
            </ul>
        <li> <span class="li-head">seq_num</span> - Sequence number. see <a href='#notes'>Notes</a>. <span class="li-normal">type: int</span> <span class="li-required">required: true</span>
 <a id='label32' href="javascript:ContentClick('label33', 'label32');" onmouseover="ContentPreview('label33');" onmouseout="ContentUnpreview('label33');" title="click to collapse or expand..."> more... </a>
 <div id="label33" style="display:none">
 <table border="1">
 <tr>
 <td></td>
 <td colspan="1">Supported Version Ranges</td>
 </tr>
 <tr>
 <td>seq_num</td>
 <td><code class="docutils literal notranslate">v6.0.0 -> 7.6.2 </code></td>
 </tr>
 </table>
 </div>
 </li>
        <li> <span class="li-head">status</span> - Enable/disable this static route. <span class="li-normal">type: str</span> <span class="li-normal">choices: enable, disable</span>
 <a id='label34' href="javascript:ContentClick('label35', 'label34');" onmouseover="ContentPreview('label35');" onmouseout="ContentUnpreview('label35');" title="click to collapse or expand..."> more... </a>
 <div id="label35" style="display:none">
 <table border="1">
 <tr>
 <td></td>
 <td colspan="1">Supported Version Ranges</td>
 </tr>
 <tr>
 <td>status</td>
 <td><code class="docutils literal notranslate">v6.0.0 -> 7.6.2 </code></td>
 </tr>
 <tr>
 <td>[enable]</td>
 <td><code class="docutils literal notranslate">v6.0.0 -> 7.6.2</code></td>
 <tr>
 <td>[disable]</td>
 <td><code class="docutils literal notranslate">v6.0.0 -> 7.6.2</code></td>
 </table>
 </div>
 </li>
        <li> <span class="li-head">tag</span> - Route tag. <span class="li-normal">type: int</span>
 <a id='label36' href="javascript:ContentClick('label37', 'label36');" onmouseover="ContentPreview('label37');" onmouseout="ContentUnpreview('label37');" title="click to collapse or expand..."> more... </a>
 <div id="label37" style="display:none">
 <table border="1">
 <tr>
 <td></td>
 <td colspan="1">Supported Version Ranges</td>
 </tr>
 <tr>
 <td>tag</td>
 <td><code class="docutils literal notranslate">v7.6.1 -> 7.6.2 </code></td>
 </tr>
 </table>
 </div>
 </li>
        <li> <span class="li-head">virtual_wan_link</span> - Enable/disable egress through the virtual-wan-link. <span class="li-normal">type: str</span> <span class="li-normal">choices: enable, disable</span>
 <a id='label38' href="javascript:ContentClick('label39', 'label38');" onmouseover="ContentPreview('label39');" onmouseout="ContentUnpreview('label39');" title="click to collapse or expand..."> more... </a>
 <div id="label39" style="display:none">
 <table border="1">
 <tr>
 <td></td>
 <td colspan="1">Supported Version Ranges</td>
 </tr>
 <tr>
 <td>virtual_wan_link</td>
 <td><code class="docutils literal notranslate">v6.0.0 -> v6.2.7 </code></td>
 </tr>
 <tr>
 <td>[enable]</td>
 <td><code class="docutils literal notranslate">v6.0.0 -> v6.2.7</code></td>
 <tr>
 <td>[disable]</td>
 <td><code class="docutils literal notranslate">v6.0.0 -> v6.2.7</code></td>
 </table>
 </div>
 </li>
        <li> <span class="li-head">vrf</span> - Virtual Routing Forwarding ID. <span class="li-normal">type: int</span>
 <a id='label40' href="javascript:ContentClick('label41', 'label40');" onmouseover="ContentPreview('label41');" onmouseout="ContentUnpreview('label41');" title="click to collapse or expand..."> more... </a>
 <div id="label41" style="display:none">
 <table border="1">
 <tr>
 <td></td>
 <td colspan="1">Supported Version Ranges</td>
 </tr>
 <tr>
 <td>vrf</td>
 <td><code class="docutils literal notranslate">v7.0.1 -> 7.6.2 </code></td>
 </tr>
 </table>
 </div>
 </li>
        <li> <span class="li-head">weight</span> - Administrative weight (0 - 255). <span class="li-normal">type: int</span>
 <a id='label42' href="javascript:ContentClick('label43', 'label42');" onmouseover="ContentPreview('label43');" onmouseout="ContentUnpreview('label43');" title="click to collapse or expand..."> more... </a>
 <div id="label43" style="display:none">
 <table border="1">
 <tr>
 <td></td>
 <td colspan="1">Supported Version Ranges</td>
 </tr>
 <tr>
 <td>weight</td>
 <td><code class="docutils literal notranslate">v7.2.1 -> 7.6.2 </code></td>
 </tr>
 </table>
 </div>
 </li>
        </ul>
    </ul>


Notes
-----

.. note::

   - We highly recommend using your own value as the seq_num instead of 0, while '0' is a special placeholder that allows the backend to assign the latest available number for the object, it does have limitations. Please find more details in Q&A.

   - Legacy fortiosapi has been deprecated, httpapi is the preferred way to run playbooks

   - The module supports check_mode.



Examples
--------

.. code-block:: yaml+jinja
    
    - name: Configure IPv6 static routing tables.
      fortinet.fortios.fortios_router_static6:
          vdom: "{{ vdom }}"
          state: "present"
          access_token: "<your_own_value>"
          router_static6:
              bfd: "enable"
              blackhole: "enable"
              comment: "Optional comments."
              device: "<your_own_value> (source system.interface.name)"
              devindex: "0"
              distance: "10"
              dst: "<your_own_value>"
              dstaddr: "<your_own_value> (source firewall.address6.name firewall.addrgrp6.name)"
              dynamic_gateway: "enable"
              gateway: "<your_own_value>"
              link_monitor_exempt: "enable"
              priority: "1024"
              sdwan: "enable"
              sdwan_zone:
                  -
                      name: "default_name_17 (source system.sdwan.zone.name)"
              seq_num: "<you_own_value>"
              status: "enable"
              tag: "0"
              virtual_wan_link: "enable"
              vrf: "unspecified"
              weight: "0"


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
