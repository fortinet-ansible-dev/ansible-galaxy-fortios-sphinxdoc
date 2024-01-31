:source: fortios_firewall_mms_profile.py

:orphan:

.. fortios_firewall_mms_profile:

fortios_firewall_mms_profile -- Configure MMS profiles in Fortinet's FortiOS and FortiGate.
+++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++

.. versionadded:: 2.0.0

.. contents::
   :local:
   :depth: 1


Synopsis
--------
- This module is able to configure a FortiGate or FortiOS (FOS) device by allowing the user to set and modify firewall feature and mms_profile category. Examples include all parameters and values need to be adjusted to datasources before usage. Tested with FOS v6.0.0



Requirements
------------
The below requirements are needed on the host that executes this module.

- ansible>=2.14


Tips
----
Using member operation to add an element to an existing object.

FortiOS Version Compatibility
-----------------------------


.. raw:: html

 <br>
 <table border="1">
 <tr>
 <td></td><td colspan="1">Supported Version Ranges</td>
 </tr>
 <tr>
 <td>fortios_firewall_mms_profile</td>
 <td><code class="docutils literal notranslate">v6.0.0 -> v6.2.7 </code></td>
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
    <li> <span class="li-head">firewall_mms_profile</span> - Configure MMS profiles. <span class="li-normal">type: dict</span>
 <a id='label0' href="javascript:ContentClick('label1', 'label0');" onmouseover="ContentPreview('label1');" onmouseout="ContentUnpreview('label1');" title="click to collapse or expand..."> more... </a>
 <div id="label1" style="display:none">
 <table border="1">
 <tr>
 <td></td><td colspan="1">Supported Version Ranges</td>
 </tr>
 <tr>
 <td>firewall_mms_profile</td>
 <td><code class="docutils literal notranslate">v6.0.0 -> v6.2.7 </code></td>
 </tr>
 </table>
 </div>
 </li>
        <ul class="ul-self">
        <li> <span class="li-head">avnotificationtable</span> - AntiVirus notification table ID. Source antivirus.notification.id. <span class="li-normal">type: int</span>
 <a id='label2' href="javascript:ContentClick('label3', 'label2');" onmouseover="ContentPreview('label3');" onmouseout="ContentUnpreview('label3');" title="click to collapse or expand..."> more... </a>
 <div id="label3" style="display:none">
 <table border="1">
 <tr>
 <td></td>
 <td colspan="1">Supported Version Ranges</td>
 </tr>
 <tr>
 <td>avnotificationtable</td>
 <td><code class="docutils literal notranslate">v6.0.0 -> v6.2.7 </code></td>
 </tr>
 </table>
 </div>
 </li>
        <li> <span class="li-head">bwordtable</span> - MMS banned word table ID. Source webfilter.content.id. <span class="li-normal">type: int</span>
 <a id='label4' href="javascript:ContentClick('label5', 'label4');" onmouseover="ContentPreview('label5');" onmouseout="ContentUnpreview('label5');" title="click to collapse or expand..."> more... </a>
 <div id="label5" style="display:none">
 <table border="1">
 <tr>
 <td></td>
 <td colspan="1">Supported Version Ranges</td>
 </tr>
 <tr>
 <td>bwordtable</td>
 <td><code class="docutils literal notranslate">v6.0.0 -> v6.2.7 </code></td>
 </tr>
 </table>
 </div>
 </li>
        <li> <span class="li-head">carrier_endpoint_prefix</span> - Enable/disable prefixing of end point values. <span class="li-normal">type: str</span> <span class="li-normal">choices: enable, disable</span>
 <a id='label6' href="javascript:ContentClick('label7', 'label6');" onmouseover="ContentPreview('label7');" onmouseout="ContentUnpreview('label7');" title="click to collapse or expand..."> more... </a>
 <div id="label7" style="display:none">
 <table border="1">
 <tr>
 <td></td>
 <td colspan="1">Supported Version Ranges</td>
 </tr>
 <tr>
 <td>carrier_endpoint_prefix</td>
 <td><code class="docutils literal notranslate">v6.0.0 -> v6.2.7 </code></td>
 </tr>
 <tr>
 <td>[enable]</td>
 <td><code class="docutils literal notranslate">v6.0.0 -> latest</code></td> <tr>
 <td>[disable]</td>
 <td><code class="docutils literal notranslate">v6.0.0 -> latest</code></td> </table>
 </div>
 </li>
        <li> <span class="li-head">carrier_endpoint_prefix_range_max</span> - Maximum length of end point value that can be prefixed (1 - 48). <span class="li-normal">type: int</span>
 <a id='label8' href="javascript:ContentClick('label9', 'label8');" onmouseover="ContentPreview('label9');" onmouseout="ContentUnpreview('label9');" title="click to collapse or expand..."> more... </a>
 <div id="label9" style="display:none">
 <table border="1">
 <tr>
 <td></td>
 <td colspan="1">Supported Version Ranges</td>
 </tr>
 <tr>
 <td>carrier_endpoint_prefix_range_max</td>
 <td><code class="docutils literal notranslate">v6.0.0 -> v6.2.7 </code></td>
 </tr>
 </table>
 </div>
 </li>
        <li> <span class="li-head">carrier_endpoint_prefix_range_min</span> - Minimum end point length to be prefixed (1 - 48). <span class="li-normal">type: int</span>
 <a id='label10' href="javascript:ContentClick('label11', 'label10');" onmouseover="ContentPreview('label11');" onmouseout="ContentUnpreview('label11');" title="click to collapse or expand..."> more... </a>
 <div id="label11" style="display:none">
 <table border="1">
 <tr>
 <td></td>
 <td colspan="1">Supported Version Ranges</td>
 </tr>
 <tr>
 <td>carrier_endpoint_prefix_range_min</td>
 <td><code class="docutils literal notranslate">v6.0.0 -> v6.2.7 </code></td>
 </tr>
 </table>
 </div>
 </li>
        <li> <span class="li-head">carrier_endpoint_prefix_string</span> - String with which to prefix End point values. <span class="li-normal">type: str</span>
 <a id='label12' href="javascript:ContentClick('label13', 'label12');" onmouseover="ContentPreview('label13');" onmouseout="ContentUnpreview('label13');" title="click to collapse or expand..."> more... </a>
 <div id="label13" style="display:none">
 <table border="1">
 <tr>
 <td></td>
 <td colspan="1">Supported Version Ranges</td>
 </tr>
 <tr>
 <td>carrier_endpoint_prefix_string</td>
 <td><code class="docutils literal notranslate">v6.0.0 -> v6.2.7 </code></td>
 </tr>
 </table>
 </div>
 </li>
        <li> <span class="li-head">carrierendpointbwltable</span> - Carrier end point filter table ID. Source firewall.carrier-endpoint-bwl.id. <span class="li-normal">type: int</span>
 <a id='label14' href="javascript:ContentClick('label15', 'label14');" onmouseover="ContentPreview('label15');" onmouseout="ContentUnpreview('label15');" title="click to collapse or expand..."> more... </a>
 <div id="label15" style="display:none">
 <table border="1">
 <tr>
 <td></td>
 <td colspan="1">Supported Version Ranges</td>
 </tr>
 <tr>
 <td>carrierendpointbwltable</td>
 <td><code class="docutils literal notranslate">v6.0.0 -> v6.2.7 </code></td>
 </tr>
 </table>
 </div>
 </li>
        <li> <span class="li-head">comment</span> - Comment. <span class="li-normal">type: str</span>
 <a id='label16' href="javascript:ContentClick('label17', 'label16');" onmouseover="ContentPreview('label17');" onmouseout="ContentUnpreview('label17');" title="click to collapse or expand..."> more... </a>
 <div id="label17" style="display:none">
 <table border="1">
 <tr>
 <td></td>
 <td colspan="1">Supported Version Ranges</td>
 </tr>
 <tr>
 <td>comment</td>
 <td><code class="docutils literal notranslate">v6.0.0 -> v6.2.7 </code></td>
 </tr>
 </table>
 </div>
 </li>
        <li> <span class="li-head">dupe</span> - Duplicate configuration. <span class="li-normal">type: list</span> <span style="font-family:'Courier New'" class="li-required">member_path: dupe:protocol</span>
 <a id='label18' href="javascript:ContentClick('label19', 'label18');" onmouseover="ContentPreview('label19');" onmouseout="ContentUnpreview('label19');" title="click to collapse or expand..."> more... </a>
 <div id="label19" style="display:none">
 <table border="1">
 <tr>
 <td></td><td colspan="1">Supported Version Ranges</td>
 </tr>
 <tr>
 <td>dupe</td>
 <td><code class="docutils literal notranslate">v6.0.0 -> v6.2.7 </code></td>
 </tr>
 </table>
 </div>
 </li>
            <ul class="ul-self">
            <li> <span class="li-head">action1</span> - Action to take when threshold reached. <span class="li-normal">type: list</span> <span class="li-normal">choices: block, archive, log, archive-first, alert-notif</span>
 <a id='label20' href="javascript:ContentClick('label21', 'label20');" onmouseover="ContentPreview('label21');" onmouseout="ContentUnpreview('label21');" title="click to collapse or expand..."> more... </a>
 <div id="label21" style="display:none">
 <table border="1">
 <tr>
 <td></td>
 <td colspan="1">Supported Version Ranges</td>
 </tr>
 <tr>
 <td>action1</td>
 <td><code class="docutils literal notranslate">v6.0.0 -> v6.2.7 </code></td>
 </tr>
 <tr>
 <td>[block]</td>
 <td><code class="docutils literal notranslate">v6.0.0 -> latest</code></td> <tr>
 <td>[archive]</td>
 <td><code class="docutils literal notranslate">v6.0.0 -> latest</code></td> <tr>
 <td>[log]</td>
 <td><code class="docutils literal notranslate">v6.0.0 -> latest</code></td> <tr>
 <td>[archive-first]</td>
 <td><code class="docutils literal notranslate">v6.0.0 -> latest</code></td> <tr>
 <td>[alert-notif]</td>
 <td><code class="docutils literal notranslate">v6.0.0 -> latest</code></td> </table>
 </div>
 </li>
            <li> <span class="li-head">action2</span> - Action to take when threshold reached. <span class="li-normal">type: list</span> <span class="li-normal">choices: block, archive, log, archive-first, alert-notif</span>
 <a id='label22' href="javascript:ContentClick('label23', 'label22');" onmouseover="ContentPreview('label23');" onmouseout="ContentUnpreview('label23');" title="click to collapse or expand..."> more... </a>
 <div id="label23" style="display:none">
 <table border="1">
 <tr>
 <td></td>
 <td colspan="1">Supported Version Ranges</td>
 </tr>
 <tr>
 <td>action2</td>
 <td><code class="docutils literal notranslate">v6.0.0 -> v6.2.7 </code></td>
 </tr>
 <tr>
 <td>[block]</td>
 <td><code class="docutils literal notranslate">v6.0.0 -> latest</code></td> <tr>
 <td>[archive]</td>
 <td><code class="docutils literal notranslate">v6.0.0 -> latest</code></td> <tr>
 <td>[log]</td>
 <td><code class="docutils literal notranslate">v6.0.0 -> latest</code></td> <tr>
 <td>[archive-first]</td>
 <td><code class="docutils literal notranslate">v6.0.0 -> latest</code></td> <tr>
 <td>[alert-notif]</td>
 <td><code class="docutils literal notranslate">v6.0.0 -> latest</code></td> </table>
 </div>
 </li>
            <li> <span class="li-head">action3</span> - Action to take when threshold reached. <span class="li-normal">type: list</span> <span class="li-normal">choices: block, archive, log, archive-first, alert-notif</span>
 <a id='label24' href="javascript:ContentClick('label25', 'label24');" onmouseover="ContentPreview('label25');" onmouseout="ContentUnpreview('label25');" title="click to collapse or expand..."> more... </a>
 <div id="label25" style="display:none">
 <table border="1">
 <tr>
 <td></td>
 <td colspan="1">Supported Version Ranges</td>
 </tr>
 <tr>
 <td>action3</td>
 <td><code class="docutils literal notranslate">v6.0.0 -> v6.2.7 </code></td>
 </tr>
 <tr>
 <td>[block]</td>
 <td><code class="docutils literal notranslate">v6.0.0 -> latest</code></td> <tr>
 <td>[archive]</td>
 <td><code class="docutils literal notranslate">v6.0.0 -> latest</code></td> <tr>
 <td>[log]</td>
 <td><code class="docutils literal notranslate">v6.0.0 -> latest</code></td> <tr>
 <td>[archive-first]</td>
 <td><code class="docutils literal notranslate">v6.0.0 -> latest</code></td> <tr>
 <td>[alert-notif]</td>
 <td><code class="docutils literal notranslate">v6.0.0 -> latest</code></td> </table>
 </div>
 </li>
            <li> <span class="li-head">block_time1</span> - Duration for which action takes effect (0 - 35791 min). <span class="li-normal">type: int</span>
 <a id='label26' href="javascript:ContentClick('label27', 'label26');" onmouseover="ContentPreview('label27');" onmouseout="ContentUnpreview('label27');" title="click to collapse or expand..."> more... </a>
 <div id="label27" style="display:none">
 <table border="1">
 <tr>
 <td></td>
 <td colspan="1">Supported Version Ranges</td>
 </tr>
 <tr>
 <td>block_time1</td>
 <td><code class="docutils literal notranslate">v6.0.0 -> v6.2.7 </code></td>
 </tr>
 </table>
 </div>
 </li>
            <li> <span class="li-head">block_time2</span> - Duration for which action takes effect (0 - 35791 min). <span class="li-normal">type: int</span>
 <a id='label28' href="javascript:ContentClick('label29', 'label28');" onmouseover="ContentPreview('label29');" onmouseout="ContentUnpreview('label29');" title="click to collapse or expand..."> more... </a>
 <div id="label29" style="display:none">
 <table border="1">
 <tr>
 <td></td>
 <td colspan="1">Supported Version Ranges</td>
 </tr>
 <tr>
 <td>block_time2</td>
 <td><code class="docutils literal notranslate">v6.0.0 -> v6.2.7 </code></td>
 </tr>
 </table>
 </div>
 </li>
            <li> <span class="li-head">block_time3</span> - Duration action takes effect (0 - 35791 min). <span class="li-normal">type: int</span>
 <a id='label30' href="javascript:ContentClick('label31', 'label30');" onmouseover="ContentPreview('label31');" onmouseout="ContentUnpreview('label31');" title="click to collapse or expand..."> more... </a>
 <div id="label31" style="display:none">
 <table border="1">
 <tr>
 <td></td>
 <td colspan="1">Supported Version Ranges</td>
 </tr>
 <tr>
 <td>block_time3</td>
 <td><code class="docutils literal notranslate">v6.0.0 -> v6.2.7 </code></td>
 </tr>
 </table>
 </div>
 </li>
            <li> <span class="li-head">limit1</span> - Maximum number of messages allowed. <span class="li-normal">type: int</span>
 <a id='label32' href="javascript:ContentClick('label33', 'label32');" onmouseover="ContentPreview('label33');" onmouseout="ContentUnpreview('label33');" title="click to collapse or expand..."> more... </a>
 <div id="label33" style="display:none">
 <table border="1">
 <tr>
 <td></td>
 <td colspan="1">Supported Version Ranges</td>
 </tr>
 <tr>
 <td>limit1</td>
 <td><code class="docutils literal notranslate">v6.0.0 -> v6.2.7 </code></td>
 </tr>
 </table>
 </div>
 </li>
            <li> <span class="li-head">limit2</span> - Maximum number of messages allowed. <span class="li-normal">type: int</span>
 <a id='label34' href="javascript:ContentClick('label35', 'label34');" onmouseover="ContentPreview('label35');" onmouseout="ContentUnpreview('label35');" title="click to collapse or expand..."> more... </a>
 <div id="label35" style="display:none">
 <table border="1">
 <tr>
 <td></td>
 <td colspan="1">Supported Version Ranges</td>
 </tr>
 <tr>
 <td>limit2</td>
 <td><code class="docutils literal notranslate">v6.0.0 -> v6.2.7 </code></td>
 </tr>
 </table>
 </div>
 </li>
            <li> <span class="li-head">limit3</span> - Maximum number of messages allowed. <span class="li-normal">type: int</span>
 <a id='label36' href="javascript:ContentClick('label37', 'label36');" onmouseover="ContentPreview('label37');" onmouseout="ContentUnpreview('label37');" title="click to collapse or expand..."> more... </a>
 <div id="label37" style="display:none">
 <table border="1">
 <tr>
 <td></td>
 <td colspan="1">Supported Version Ranges</td>
 </tr>
 <tr>
 <td>limit3</td>
 <td><code class="docutils literal notranslate">v6.0.0 -> v6.2.7 </code></td>
 </tr>
 </table>
 </div>
 </li>
            <li> <span class="li-head">protocol</span> - Protocol. <span class="li-normal">type: str</span> <span class="li-required">required: true</span>
 <a id='label38' href="javascript:ContentClick('label39', 'label38');" onmouseover="ContentPreview('label39');" onmouseout="ContentUnpreview('label39');" title="click to collapse or expand..."> more... </a>
 <div id="label39" style="display:none">
 <table border="1">
 <tr>
 <td></td>
 <td colspan="1">Supported Version Ranges</td>
 </tr>
 <tr>
 <td>protocol</td>
 <td><code class="docutils literal notranslate">v6.0.0 -> v6.2.7 </code></td>
 </tr>
 </table>
 </div>
 </li>
            <li> <span class="li-head">status1</span> - Enable/disable status1 detection. <span class="li-normal">type: str</span> <span class="li-normal">choices: enable, disable</span>
 <a id='label40' href="javascript:ContentClick('label41', 'label40');" onmouseover="ContentPreview('label41');" onmouseout="ContentUnpreview('label41');" title="click to collapse or expand..."> more... </a>
 <div id="label41" style="display:none">
 <table border="1">
 <tr>
 <td></td>
 <td colspan="1">Supported Version Ranges</td>
 </tr>
 <tr>
 <td>status1</td>
 <td><code class="docutils literal notranslate">v6.0.0 -> v6.2.7 </code></td>
 </tr>
 <tr>
 <td>[enable]</td>
 <td><code class="docutils literal notranslate">v6.0.0 -> latest</code></td> <tr>
 <td>[disable]</td>
 <td><code class="docutils literal notranslate">v6.0.0 -> latest</code></td> </table>
 </div>
 </li>
            <li> <span class="li-head">status2</span> - Enable/disable status2 detection. <span class="li-normal">type: str</span> <span class="li-normal">choices: enable, disable</span>
 <a id='label42' href="javascript:ContentClick('label43', 'label42');" onmouseover="ContentPreview('label43');" onmouseout="ContentUnpreview('label43');" title="click to collapse or expand..."> more... </a>
 <div id="label43" style="display:none">
 <table border="1">
 <tr>
 <td></td>
 <td colspan="1">Supported Version Ranges</td>
 </tr>
 <tr>
 <td>status2</td>
 <td><code class="docutils literal notranslate">v6.0.0 -> v6.2.7 </code></td>
 </tr>
 <tr>
 <td>[enable]</td>
 <td><code class="docutils literal notranslate">v6.0.0 -> latest</code></td> <tr>
 <td>[disable]</td>
 <td><code class="docutils literal notranslate">v6.0.0 -> latest</code></td> </table>
 </div>
 </li>
            <li> <span class="li-head">status3</span> - Enable/disable status3 detection. <span class="li-normal">type: str</span> <span class="li-normal">choices: enable, disable</span>
 <a id='label44' href="javascript:ContentClick('label45', 'label44');" onmouseover="ContentPreview('label45');" onmouseout="ContentUnpreview('label45');" title="click to collapse or expand..."> more... </a>
 <div id="label45" style="display:none">
 <table border="1">
 <tr>
 <td></td>
 <td colspan="1">Supported Version Ranges</td>
 </tr>
 <tr>
 <td>status3</td>
 <td><code class="docutils literal notranslate">v6.0.0 -> v6.2.7 </code></td>
 </tr>
 <tr>
 <td>[enable]</td>
 <td><code class="docutils literal notranslate">v6.0.0 -> latest</code></td> <tr>
 <td>[disable]</td>
 <td><code class="docutils literal notranslate">v6.0.0 -> latest</code></td> </table>
 </div>
 </li>
            <li> <span class="li-head">window1</span> - Window to count messages over (1 - 2880 min). <span class="li-normal">type: int</span>
 <a id='label46' href="javascript:ContentClick('label47', 'label46');" onmouseover="ContentPreview('label47');" onmouseout="ContentUnpreview('label47');" title="click to collapse or expand..."> more... </a>
 <div id="label47" style="display:none">
 <table border="1">
 <tr>
 <td></td>
 <td colspan="1">Supported Version Ranges</td>
 </tr>
 <tr>
 <td>window1</td>
 <td><code class="docutils literal notranslate">v6.0.0 -> v6.2.7 </code></td>
 </tr>
 </table>
 </div>
 </li>
            <li> <span class="li-head">window2</span> - Window to count messages over (1 - 2880 min). <span class="li-normal">type: int</span>
 <a id='label48' href="javascript:ContentClick('label49', 'label48');" onmouseover="ContentPreview('label49');" onmouseout="ContentUnpreview('label49');" title="click to collapse or expand..."> more... </a>
 <div id="label49" style="display:none">
 <table border="1">
 <tr>
 <td></td>
 <td colspan="1">Supported Version Ranges</td>
 </tr>
 <tr>
 <td>window2</td>
 <td><code class="docutils literal notranslate">v6.0.0 -> v6.2.7 </code></td>
 </tr>
 </table>
 </div>
 </li>
            <li> <span class="li-head">window3</span> - Window to count messages over (1 - 2880 min). <span class="li-normal">type: int</span>
 <a id='label50' href="javascript:ContentClick('label51', 'label50');" onmouseover="ContentPreview('label51');" onmouseout="ContentUnpreview('label51');" title="click to collapse or expand..."> more... </a>
 <div id="label51" style="display:none">
 <table border="1">
 <tr>
 <td></td>
 <td colspan="1">Supported Version Ranges</td>
 </tr>
 <tr>
 <td>window3</td>
 <td><code class="docutils literal notranslate">v6.0.0 -> v6.2.7 </code></td>
 </tr>
 </table>
 </div>
 </li>
            </ul>
        <li> <span class="li-head">extended_utm_log</span> - Enable/disable detailed UTM log messages. <span class="li-normal">type: str</span>
 <a id='label52' href="javascript:ContentClick('label53', 'label52');" onmouseover="ContentPreview('label53');" onmouseout="ContentUnpreview('label53');" title="click to collapse or expand..."> more... </a>
 <div id="label53" style="display:none">
 <table border="1">
 <tr>
 <td></td>
 <td colspan="1">Supported Version Ranges</td>
 </tr>
 <tr>
 <td>extended_utm_log</td>
 <td><code class="docutils literal notranslate">v6.0.0 -> v6.2.7 </code></td>
 </tr>
 </table>
 </div>
 </li>
        <li> <span class="li-head">flood</span> - Flood configuration. <span class="li-normal">type: list</span> <span style="font-family:'Courier New'" class="li-required">member_path: flood:protocol</span>
 <a id='label54' href="javascript:ContentClick('label55', 'label54');" onmouseover="ContentPreview('label55');" onmouseout="ContentUnpreview('label55');" title="click to collapse or expand..."> more... </a>
 <div id="label55" style="display:none">
 <table border="1">
 <tr>
 <td></td><td colspan="1">Supported Version Ranges</td>
 </tr>
 <tr>
 <td>flood</td>
 <td><code class="docutils literal notranslate">v6.0.0 -> v6.2.7 </code></td>
 </tr>
 </table>
 </div>
 </li>
            <ul class="ul-self">
            <li> <span class="li-head">action1</span> - Action to take when threshold reached. <span class="li-normal">type: list</span> <span class="li-normal">choices: block, archive, log, archive-first, alert-notif</span>
 <a id='label56' href="javascript:ContentClick('label57', 'label56');" onmouseover="ContentPreview('label57');" onmouseout="ContentUnpreview('label57');" title="click to collapse or expand..."> more... </a>
 <div id="label57" style="display:none">
 <table border="1">
 <tr>
 <td></td>
 <td colspan="1">Supported Version Ranges</td>
 </tr>
 <tr>
 <td>action1</td>
 <td><code class="docutils literal notranslate">v6.0.0 -> v6.2.7 </code></td>
 </tr>
 <tr>
 <td>[block]</td>
 <td><code class="docutils literal notranslate">v6.0.0 -> latest</code></td> <tr>
 <td>[archive]</td>
 <td><code class="docutils literal notranslate">v6.0.0 -> latest</code></td> <tr>
 <td>[log]</td>
 <td><code class="docutils literal notranslate">v6.0.0 -> latest</code></td> <tr>
 <td>[archive-first]</td>
 <td><code class="docutils literal notranslate">v6.0.0 -> latest</code></td> <tr>
 <td>[alert-notif]</td>
 <td><code class="docutils literal notranslate">v6.0.0 -> latest</code></td> </table>
 </div>
 </li>
            <li> <span class="li-head">action2</span> - Action to take when threshold reached. <span class="li-normal">type: list</span> <span class="li-normal">choices: block, archive, log, archive-first, alert-notif</span>
 <a id='label58' href="javascript:ContentClick('label59', 'label58');" onmouseover="ContentPreview('label59');" onmouseout="ContentUnpreview('label59');" title="click to collapse or expand..."> more... </a>
 <div id="label59" style="display:none">
 <table border="1">
 <tr>
 <td></td>
 <td colspan="1">Supported Version Ranges</td>
 </tr>
 <tr>
 <td>action2</td>
 <td><code class="docutils literal notranslate">v6.0.0 -> v6.2.7 </code></td>
 </tr>
 <tr>
 <td>[block]</td>
 <td><code class="docutils literal notranslate">v6.0.0 -> latest</code></td> <tr>
 <td>[archive]</td>
 <td><code class="docutils literal notranslate">v6.0.0 -> latest</code></td> <tr>
 <td>[log]</td>
 <td><code class="docutils literal notranslate">v6.0.0 -> latest</code></td> <tr>
 <td>[archive-first]</td>
 <td><code class="docutils literal notranslate">v6.0.0 -> latest</code></td> <tr>
 <td>[alert-notif]</td>
 <td><code class="docutils literal notranslate">v6.0.0 -> latest</code></td> </table>
 </div>
 </li>
            <li> <span class="li-head">action3</span> - Action to take when threshold reached. <span class="li-normal">type: list</span> <span class="li-normal">choices: block, archive, log, archive-first, alert-notif</span>
 <a id='label60' href="javascript:ContentClick('label61', 'label60');" onmouseover="ContentPreview('label61');" onmouseout="ContentUnpreview('label61');" title="click to collapse or expand..."> more... </a>
 <div id="label61" style="display:none">
 <table border="1">
 <tr>
 <td></td>
 <td colspan="1">Supported Version Ranges</td>
 </tr>
 <tr>
 <td>action3</td>
 <td><code class="docutils literal notranslate">v6.0.0 -> v6.2.7 </code></td>
 </tr>
 <tr>
 <td>[block]</td>
 <td><code class="docutils literal notranslate">v6.0.0 -> latest</code></td> <tr>
 <td>[archive]</td>
 <td><code class="docutils literal notranslate">v6.0.0 -> latest</code></td> <tr>
 <td>[log]</td>
 <td><code class="docutils literal notranslate">v6.0.0 -> latest</code></td> <tr>
 <td>[archive-first]</td>
 <td><code class="docutils literal notranslate">v6.0.0 -> latest</code></td> <tr>
 <td>[alert-notif]</td>
 <td><code class="docutils literal notranslate">v6.0.0 -> latest</code></td> </table>
 </div>
 </li>
            <li> <span class="li-head">block_time1</span> - Duration for which action takes effect (0 - 35791 min). <span class="li-normal">type: int</span>
 <a id='label62' href="javascript:ContentClick('label63', 'label62');" onmouseover="ContentPreview('label63');" onmouseout="ContentUnpreview('label63');" title="click to collapse or expand..."> more... </a>
 <div id="label63" style="display:none">
 <table border="1">
 <tr>
 <td></td>
 <td colspan="1">Supported Version Ranges</td>
 </tr>
 <tr>
 <td>block_time1</td>
 <td><code class="docutils literal notranslate">v6.0.0 -> v6.2.7 </code></td>
 </tr>
 </table>
 </div>
 </li>
            <li> <span class="li-head">block_time2</span> - Duration for which action takes effect (0 - 35791 min). <span class="li-normal">type: int</span>
 <a id='label64' href="javascript:ContentClick('label65', 'label64');" onmouseover="ContentPreview('label65');" onmouseout="ContentUnpreview('label65');" title="click to collapse or expand..."> more... </a>
 <div id="label65" style="display:none">
 <table border="1">
 <tr>
 <td></td>
 <td colspan="1">Supported Version Ranges</td>
 </tr>
 <tr>
 <td>block_time2</td>
 <td><code class="docutils literal notranslate">v6.0.0 -> v6.2.7 </code></td>
 </tr>
 </table>
 </div>
 </li>
            <li> <span class="li-head">block_time3</span> - Duration action takes effect (0 - 35791 min). <span class="li-normal">type: int</span>
 <a id='label66' href="javascript:ContentClick('label67', 'label66');" onmouseover="ContentPreview('label67');" onmouseout="ContentUnpreview('label67');" title="click to collapse or expand..."> more... </a>
 <div id="label67" style="display:none">
 <table border="1">
 <tr>
 <td></td>
 <td colspan="1">Supported Version Ranges</td>
 </tr>
 <tr>
 <td>block_time3</td>
 <td><code class="docutils literal notranslate">v6.0.0 -> v6.2.7 </code></td>
 </tr>
 </table>
 </div>
 </li>
            <li> <span class="li-head">limit1</span> - Maximum number of messages allowed. <span class="li-normal">type: int</span>
 <a id='label68' href="javascript:ContentClick('label69', 'label68');" onmouseover="ContentPreview('label69');" onmouseout="ContentUnpreview('label69');" title="click to collapse or expand..."> more... </a>
 <div id="label69" style="display:none">
 <table border="1">
 <tr>
 <td></td>
 <td colspan="1">Supported Version Ranges</td>
 </tr>
 <tr>
 <td>limit1</td>
 <td><code class="docutils literal notranslate">v6.0.0 -> v6.2.7 </code></td>
 </tr>
 </table>
 </div>
 </li>
            <li> <span class="li-head">limit2</span> - Maximum number of messages allowed. <span class="li-normal">type: int</span>
 <a id='label70' href="javascript:ContentClick('label71', 'label70');" onmouseover="ContentPreview('label71');" onmouseout="ContentUnpreview('label71');" title="click to collapse or expand..."> more... </a>
 <div id="label71" style="display:none">
 <table border="1">
 <tr>
 <td></td>
 <td colspan="1">Supported Version Ranges</td>
 </tr>
 <tr>
 <td>limit2</td>
 <td><code class="docutils literal notranslate">v6.0.0 -> v6.2.7 </code></td>
 </tr>
 </table>
 </div>
 </li>
            <li> <span class="li-head">limit3</span> - Maximum number of messages allowed. <span class="li-normal">type: int</span>
 <a id='label72' href="javascript:ContentClick('label73', 'label72');" onmouseover="ContentPreview('label73');" onmouseout="ContentUnpreview('label73');" title="click to collapse or expand..."> more... </a>
 <div id="label73" style="display:none">
 <table border="1">
 <tr>
 <td></td>
 <td colspan="1">Supported Version Ranges</td>
 </tr>
 <tr>
 <td>limit3</td>
 <td><code class="docutils literal notranslate">v6.0.0 -> v6.2.7 </code></td>
 </tr>
 </table>
 </div>
 </li>
            <li> <span class="li-head">protocol</span> - Protocol. <span class="li-normal">type: str</span> <span class="li-required">required: true</span>
 <a id='label74' href="javascript:ContentClick('label75', 'label74');" onmouseover="ContentPreview('label75');" onmouseout="ContentUnpreview('label75');" title="click to collapse or expand..."> more... </a>
 <div id="label75" style="display:none">
 <table border="1">
 <tr>
 <td></td>
 <td colspan="1">Supported Version Ranges</td>
 </tr>
 <tr>
 <td>protocol</td>
 <td><code class="docutils literal notranslate">v6.0.0 -> v6.2.7 </code></td>
 </tr>
 </table>
 </div>
 </li>
            <li> <span class="li-head">status1</span> - Enable/disable status1 detection. <span class="li-normal">type: str</span> <span class="li-normal">choices: enable, disable</span>
 <a id='label76' href="javascript:ContentClick('label77', 'label76');" onmouseover="ContentPreview('label77');" onmouseout="ContentUnpreview('label77');" title="click to collapse or expand..."> more... </a>
 <div id="label77" style="display:none">
 <table border="1">
 <tr>
 <td></td>
 <td colspan="1">Supported Version Ranges</td>
 </tr>
 <tr>
 <td>status1</td>
 <td><code class="docutils literal notranslate">v6.0.0 -> v6.2.7 </code></td>
 </tr>
 <tr>
 <td>[enable]</td>
 <td><code class="docutils literal notranslate">v6.0.0 -> latest</code></td> <tr>
 <td>[disable]</td>
 <td><code class="docutils literal notranslate">v6.0.0 -> latest</code></td> </table>
 </div>
 </li>
            <li> <span class="li-head">status2</span> - Enable/disable status2 detection. <span class="li-normal">type: str</span> <span class="li-normal">choices: enable, disable</span>
 <a id='label78' href="javascript:ContentClick('label79', 'label78');" onmouseover="ContentPreview('label79');" onmouseout="ContentUnpreview('label79');" title="click to collapse or expand..."> more... </a>
 <div id="label79" style="display:none">
 <table border="1">
 <tr>
 <td></td>
 <td colspan="1">Supported Version Ranges</td>
 </tr>
 <tr>
 <td>status2</td>
 <td><code class="docutils literal notranslate">v6.0.0 -> v6.2.7 </code></td>
 </tr>
 <tr>
 <td>[enable]</td>
 <td><code class="docutils literal notranslate">v6.0.0 -> latest</code></td> <tr>
 <td>[disable]</td>
 <td><code class="docutils literal notranslate">v6.0.0 -> latest</code></td> </table>
 </div>
 </li>
            <li> <span class="li-head">status3</span> - Enable/disable status3 detection. <span class="li-normal">type: str</span> <span class="li-normal">choices: enable, disable</span>
 <a id='label80' href="javascript:ContentClick('label81', 'label80');" onmouseover="ContentPreview('label81');" onmouseout="ContentUnpreview('label81');" title="click to collapse or expand..."> more... </a>
 <div id="label81" style="display:none">
 <table border="1">
 <tr>
 <td></td>
 <td colspan="1">Supported Version Ranges</td>
 </tr>
 <tr>
 <td>status3</td>
 <td><code class="docutils literal notranslate">v6.0.0 -> v6.2.7 </code></td>
 </tr>
 <tr>
 <td>[enable]</td>
 <td><code class="docutils literal notranslate">v6.0.0 -> latest</code></td> <tr>
 <td>[disable]</td>
 <td><code class="docutils literal notranslate">v6.0.0 -> latest</code></td> </table>
 </div>
 </li>
            <li> <span class="li-head">window1</span> - Window to count messages over (1 - 2880 min). <span class="li-normal">type: int</span>
 <a id='label82' href="javascript:ContentClick('label83', 'label82');" onmouseover="ContentPreview('label83');" onmouseout="ContentUnpreview('label83');" title="click to collapse or expand..."> more... </a>
 <div id="label83" style="display:none">
 <table border="1">
 <tr>
 <td></td>
 <td colspan="1">Supported Version Ranges</td>
 </tr>
 <tr>
 <td>window1</td>
 <td><code class="docutils literal notranslate">v6.0.0 -> v6.2.7 </code></td>
 </tr>
 </table>
 </div>
 </li>
            <li> <span class="li-head">window2</span> - Window to count messages over (1 - 2880 min). <span class="li-normal">type: int</span>
 <a id='label84' href="javascript:ContentClick('label85', 'label84');" onmouseover="ContentPreview('label85');" onmouseout="ContentUnpreview('label85');" title="click to collapse or expand..."> more... </a>
 <div id="label85" style="display:none">
 <table border="1">
 <tr>
 <td></td>
 <td colspan="1">Supported Version Ranges</td>
 </tr>
 <tr>
 <td>window2</td>
 <td><code class="docutils literal notranslate">v6.0.0 -> v6.2.7 </code></td>
 </tr>
 </table>
 </div>
 </li>
            <li> <span class="li-head">window3</span> - Window to count messages over (1 - 2880 min). <span class="li-normal">type: int</span>
 <a id='label86' href="javascript:ContentClick('label87', 'label86');" onmouseover="ContentPreview('label87');" onmouseout="ContentUnpreview('label87');" title="click to collapse or expand..."> more... </a>
 <div id="label87" style="display:none">
 <table border="1">
 <tr>
 <td></td>
 <td colspan="1">Supported Version Ranges</td>
 </tr>
 <tr>
 <td>window3</td>
 <td><code class="docutils literal notranslate">v6.0.0 -> v6.2.7 </code></td>
 </tr>
 </table>
 </div>
 </li>
            </ul>
        <li> <span class="li-head">mm1</span> - MM1 options. <span class="li-normal">type: list</span> <span class="li-normal">choices: avmonitor, oversize, quarantine, scan, bannedword, chunkedbypass, clientcomfort, servercomfort, carrier-endpoint-bwl, remove-blocked, mms-checksum</span>
 <a id='label88' href="javascript:ContentClick('label89', 'label88');" onmouseover="ContentPreview('label89');" onmouseout="ContentUnpreview('label89');" title="click to collapse or expand..."> more... </a>
 <div id="label89" style="display:none">
 <table border="1">
 <tr>
 <td></td>
 <td colspan="1">Supported Version Ranges</td>
 </tr>
 <tr>
 <td>mm1</td>
 <td><code class="docutils literal notranslate">v6.0.0 -> v6.2.7 </code></td>
 </tr>
 <tr>
 <td>[avmonitor]</td>
 <td><code class="docutils literal notranslate">v6.0.0 -> latest</code></td> <tr>
 <td>[oversize]</td>
 <td><code class="docutils literal notranslate">v6.0.0 -> latest</code></td> <tr>
 <td>[quarantine]</td>
 <td><code class="docutils literal notranslate">v6.0.0 -> latest</code></td> <tr>
 <td>[scan]</td>
 <td><code class="docutils literal notranslate">v6.0.0 -> latest</code></td> <tr>
 <td>[bannedword]</td>
 <td><code class="docutils literal notranslate">v6.0.0 -> latest</code></td> <tr>
 <td>[chunkedbypass]</td>
 <td><code class="docutils literal notranslate">v6.0.0 -> latest</code></td> <tr>
 <td>[clientcomfort]</td>
 <td><code class="docutils literal notranslate">v6.0.0 -> latest</code></td> <tr>
 <td>[servercomfort]</td>
 <td><code class="docutils literal notranslate">v6.0.0 -> latest</code></td> <tr>
 <td>[carrier-endpoint-bwl]</td>
 <td><code class="docutils literal notranslate">v6.0.0 -> latest</code></td> <tr>
 <td>[remove-blocked]</td>
 <td><code class="docutils literal notranslate">v6.0.0 -> latest</code></td> <tr>
 <td>[mms-checksum]</td>
 <td><code class="docutils literal notranslate">v6.0.0 -> latest</code></td> </table>
 </div>
 </li>
        <li> <span class="li-head">mm1_addr_hdr</span> - HTTP header field (for MM1) containing user address. <span class="li-normal">type: str</span>
 <a id='label90' href="javascript:ContentClick('label91', 'label90');" onmouseover="ContentPreview('label91');" onmouseout="ContentUnpreview('label91');" title="click to collapse or expand..."> more... </a>
 <div id="label91" style="display:none">
 <table border="1">
 <tr>
 <td></td>
 <td colspan="1">Supported Version Ranges</td>
 </tr>
 <tr>
 <td>mm1_addr_hdr</td>
 <td><code class="docutils literal notranslate">v6.0.0 -> v6.2.7 </code></td>
 </tr>
 </table>
 </div>
 </li>
        <li> <span class="li-head">mm1_addr_source</span> - Source for MM1 user address. <span class="li-normal">type: str</span> <span class="li-normal">choices: http-header, cookie</span>
 <a id='label92' href="javascript:ContentClick('label93', 'label92');" onmouseover="ContentPreview('label93');" onmouseout="ContentUnpreview('label93');" title="click to collapse or expand..."> more... </a>
 <div id="label93" style="display:none">
 <table border="1">
 <tr>
 <td></td>
 <td colspan="1">Supported Version Ranges</td>
 </tr>
 <tr>
 <td>mm1_addr_source</td>
 <td><code class="docutils literal notranslate">v6.0.0 -> v6.2.7 </code></td>
 </tr>
 <tr>
 <td>[http-header]</td>
 <td><code class="docutils literal notranslate">v6.0.0 -> latest</code></td> <tr>
 <td>[cookie]</td>
 <td><code class="docutils literal notranslate">v6.0.0 -> latest</code></td> </table>
 </div>
 </li>
        <li> <span class="li-head">mm1_convert_hex</span> - Enable/disable converting user address from HEX string for MM1. <span class="li-normal">type: str</span> <span class="li-normal">choices: enable, disable</span>
 <a id='label94' href="javascript:ContentClick('label95', 'label94');" onmouseover="ContentPreview('label95');" onmouseout="ContentUnpreview('label95');" title="click to collapse or expand..."> more... </a>
 <div id="label95" style="display:none">
 <table border="1">
 <tr>
 <td></td>
 <td colspan="1">Supported Version Ranges</td>
 </tr>
 <tr>
 <td>mm1_convert_hex</td>
 <td><code class="docutils literal notranslate">v6.0.0 -> v6.2.7 </code></td>
 </tr>
 <tr>
 <td>[enable]</td>
 <td><code class="docutils literal notranslate">v6.0.0 -> latest</code></td> <tr>
 <td>[disable]</td>
 <td><code class="docutils literal notranslate">v6.0.0 -> latest</code></td> </table>
 </div>
 </li>
        <li> <span class="li-head">mm1_outbreak_prevention</span> - Enable Virus Outbreak Prevention service. <span class="li-normal">type: str</span> <span class="li-normal">choices: disabled, files, full-archive</span>
 <a id='label96' href="javascript:ContentClick('label97', 'label96');" onmouseover="ContentPreview('label97');" onmouseout="ContentUnpreview('label97');" title="click to collapse or expand..."> more... </a>
 <div id="label97" style="display:none">
 <table border="1">
 <tr>
 <td></td>
 <td colspan="1">Supported Version Ranges</td>
 </tr>
 <tr>
 <td>mm1_outbreak_prevention</td>
 <td><code class="docutils literal notranslate">v6.0.0 -> v6.2.7 </code></td>
 </tr>
 <tr>
 <td>[disabled]</td>
 <td><code class="docutils literal notranslate">v6.0.0 -> latest</code></td> <tr>
 <td>[files]</td>
 <td><code class="docutils literal notranslate">v6.0.0 -> latest</code></td> <tr>
 <td>[full-archive]</td>
 <td><code class="docutils literal notranslate">v6.0.0 -> latest</code></td> </table>
 </div>
 </li>
        <li> <span class="li-head">mm1_retr_dupe</span> - Enable/disable duplicate scanning of MM1 retr. <span class="li-normal">type: str</span> <span class="li-normal">choices: enable, disable</span>
 <a id='label98' href="javascript:ContentClick('label99', 'label98');" onmouseover="ContentPreview('label99');" onmouseout="ContentUnpreview('label99');" title="click to collapse or expand..."> more... </a>
 <div id="label99" style="display:none">
 <table border="1">
 <tr>
 <td></td>
 <td colspan="1">Supported Version Ranges</td>
 </tr>
 <tr>
 <td>mm1_retr_dupe</td>
 <td><code class="docutils literal notranslate">v6.0.0 -> v6.2.7 </code></td>
 </tr>
 <tr>
 <td>[enable]</td>
 <td><code class="docutils literal notranslate">v6.0.0 -> latest</code></td> <tr>
 <td>[disable]</td>
 <td><code class="docutils literal notranslate">v6.0.0 -> latest</code></td> </table>
 </div>
 </li>
        <li> <span class="li-head">mm1_retrieve_scan</span> - Enable/disable scanning on MM1 retrieve configuration messages. <span class="li-normal">type: str</span> <span class="li-normal">choices: enable, disable</span>
 <a id='label100' href="javascript:ContentClick('label101', 'label100');" onmouseover="ContentPreview('label101');" onmouseout="ContentUnpreview('label101');" title="click to collapse or expand..."> more... </a>
 <div id="label101" style="display:none">
 <table border="1">
 <tr>
 <td></td>
 <td colspan="1">Supported Version Ranges</td>
 </tr>
 <tr>
 <td>mm1_retrieve_scan</td>
 <td><code class="docutils literal notranslate">v6.0.0 -> v6.2.7 </code></td>
 </tr>
 <tr>
 <td>[enable]</td>
 <td><code class="docutils literal notranslate">v6.0.0 -> latest</code></td> <tr>
 <td>[disable]</td>
 <td><code class="docutils literal notranslate">v6.0.0 -> latest</code></td> </table>
 </div>
 </li>
        <li> <span class="li-head">mm1comfortamount</span> - MM1 comfort amount (0 - 4294967295). <span class="li-normal">type: int</span>
 <a id='label102' href="javascript:ContentClick('label103', 'label102');" onmouseover="ContentPreview('label103');" onmouseout="ContentUnpreview('label103');" title="click to collapse or expand..."> more... </a>
 <div id="label103" style="display:none">
 <table border="1">
 <tr>
 <td></td>
 <td colspan="1">Supported Version Ranges</td>
 </tr>
 <tr>
 <td>mm1comfortamount</td>
 <td><code class="docutils literal notranslate">v6.0.0 -> v6.2.7 </code></td>
 </tr>
 </table>
 </div>
 </li>
        <li> <span class="li-head">mm1comfortinterval</span> - MM1 comfort interval (0 - 4294967295). <span class="li-normal">type: int</span>
 <a id='label104' href="javascript:ContentClick('label105', 'label104');" onmouseover="ContentPreview('label105');" onmouseout="ContentUnpreview('label105');" title="click to collapse or expand..."> more... </a>
 <div id="label105" style="display:none">
 <table border="1">
 <tr>
 <td></td>
 <td colspan="1">Supported Version Ranges</td>
 </tr>
 <tr>
 <td>mm1comfortinterval</td>
 <td><code class="docutils literal notranslate">v6.0.0 -> v6.2.7 </code></td>
 </tr>
 </table>
 </div>
 </li>
        <li> <span class="li-head">mm1oversizelimit</span> - Maximum file size to scan (1 - 819200 kB). <span class="li-normal">type: int</span>
 <a id='label106' href="javascript:ContentClick('label107', 'label106');" onmouseover="ContentPreview('label107');" onmouseout="ContentUnpreview('label107');" title="click to collapse or expand..."> more... </a>
 <div id="label107" style="display:none">
 <table border="1">
 <tr>
 <td></td>
 <td colspan="1">Supported Version Ranges</td>
 </tr>
 <tr>
 <td>mm1oversizelimit</td>
 <td><code class="docutils literal notranslate">v6.0.0 -> v6.2.7 </code></td>
 </tr>
 </table>
 </div>
 </li>
        <li> <span class="li-head">mm3</span> - MM3 options. <span class="li-normal">type: list</span> <span class="li-normal">choices: avmonitor, oversize, quarantine, scan, bannedword, fragmail, splice, carrier-endpoint-bwl, remove-blocked, mms-checksum</span>
 <a id='label108' href="javascript:ContentClick('label109', 'label108');" onmouseover="ContentPreview('label109');" onmouseout="ContentUnpreview('label109');" title="click to collapse or expand..."> more... </a>
 <div id="label109" style="display:none">
 <table border="1">
 <tr>
 <td></td>
 <td colspan="1">Supported Version Ranges</td>
 </tr>
 <tr>
 <td>mm3</td>
 <td><code class="docutils literal notranslate">v6.0.0 -> v6.2.7 </code></td>
 </tr>
 <tr>
 <td>[avmonitor]</td>
 <td><code class="docutils literal notranslate">v6.0.0 -> latest</code></td> <tr>
 <td>[oversize]</td>
 <td><code class="docutils literal notranslate">v6.0.0 -> latest</code></td> <tr>
 <td>[quarantine]</td>
 <td><code class="docutils literal notranslate">v6.0.0 -> latest</code></td> <tr>
 <td>[scan]</td>
 <td><code class="docutils literal notranslate">v6.0.0 -> latest</code></td> <tr>
 <td>[bannedword]</td>
 <td><code class="docutils literal notranslate">v6.0.0 -> latest</code></td> <tr>
 <td>[fragmail]</td>
 <td><code class="docutils literal notranslate">v6.0.0 -> latest</code></td> <tr>
 <td>[splice]</td>
 <td><code class="docutils literal notranslate">v6.0.0 -> latest</code></td> <tr>
 <td>[carrier-endpoint-bwl]</td>
 <td><code class="docutils literal notranslate">v6.0.0 -> latest</code></td> <tr>
 <td>[remove-blocked]</td>
 <td><code class="docutils literal notranslate">v6.0.0 -> latest</code></td> <tr>
 <td>[mms-checksum]</td>
 <td><code class="docutils literal notranslate">v6.0.0 -> latest</code></td> </table>
 </div>
 </li>
        <li> <span class="li-head">mm3_outbreak_prevention</span> - Enable Virus Outbreak Prevention service. <span class="li-normal">type: str</span> <span class="li-normal">choices: disabled, files, full-archive</span>
 <a id='label110' href="javascript:ContentClick('label111', 'label110');" onmouseover="ContentPreview('label111');" onmouseout="ContentUnpreview('label111');" title="click to collapse or expand..."> more... </a>
 <div id="label111" style="display:none">
 <table border="1">
 <tr>
 <td></td>
 <td colspan="1">Supported Version Ranges</td>
 </tr>
 <tr>
 <td>mm3_outbreak_prevention</td>
 <td><code class="docutils literal notranslate">v6.0.0 -> v6.2.7 </code></td>
 </tr>
 <tr>
 <td>[disabled]</td>
 <td><code class="docutils literal notranslate">v6.0.0 -> latest</code></td> <tr>
 <td>[files]</td>
 <td><code class="docutils literal notranslate">v6.0.0 -> latest</code></td> <tr>
 <td>[full-archive]</td>
 <td><code class="docutils literal notranslate">v6.0.0 -> latest</code></td> </table>
 </div>
 </li>
        <li> <span class="li-head">mm3oversizelimit</span> - Maximum file size to scan (1 - 819200 kB). <span class="li-normal">type: int</span>
 <a id='label112' href="javascript:ContentClick('label113', 'label112');" onmouseover="ContentPreview('label113');" onmouseout="ContentUnpreview('label113');" title="click to collapse or expand..."> more... </a>
 <div id="label113" style="display:none">
 <table border="1">
 <tr>
 <td></td>
 <td colspan="1">Supported Version Ranges</td>
 </tr>
 <tr>
 <td>mm3oversizelimit</td>
 <td><code class="docutils literal notranslate">v6.0.0 -> v6.2.7 </code></td>
 </tr>
 </table>
 </div>
 </li>
        <li> <span class="li-head">mm4</span> - MM4 options. <span class="li-normal">type: list</span> <span class="li-normal">choices: avmonitor, oversize, quarantine, scan, bannedword, fragmail, splice, carrier-endpoint-bwl, remove-blocked, mms-checksum</span>
 <a id='label114' href="javascript:ContentClick('label115', 'label114');" onmouseover="ContentPreview('label115');" onmouseout="ContentUnpreview('label115');" title="click to collapse or expand..."> more... </a>
 <div id="label115" style="display:none">
 <table border="1">
 <tr>
 <td></td>
 <td colspan="1">Supported Version Ranges</td>
 </tr>
 <tr>
 <td>mm4</td>
 <td><code class="docutils literal notranslate">v6.0.0 -> v6.2.7 </code></td>
 </tr>
 <tr>
 <td>[avmonitor]</td>
 <td><code class="docutils literal notranslate">v6.0.0 -> latest</code></td> <tr>
 <td>[oversize]</td>
 <td><code class="docutils literal notranslate">v6.0.0 -> latest</code></td> <tr>
 <td>[quarantine]</td>
 <td><code class="docutils literal notranslate">v6.0.0 -> latest</code></td> <tr>
 <td>[scan]</td>
 <td><code class="docutils literal notranslate">v6.0.0 -> latest</code></td> <tr>
 <td>[bannedword]</td>
 <td><code class="docutils literal notranslate">v6.0.0 -> latest</code></td> <tr>
 <td>[fragmail]</td>
 <td><code class="docutils literal notranslate">v6.0.0 -> latest</code></td> <tr>
 <td>[splice]</td>
 <td><code class="docutils literal notranslate">v6.0.0 -> latest</code></td> <tr>
 <td>[carrier-endpoint-bwl]</td>
 <td><code class="docutils literal notranslate">v6.0.0 -> latest</code></td> <tr>
 <td>[remove-blocked]</td>
 <td><code class="docutils literal notranslate">v6.0.0 -> latest</code></td> <tr>
 <td>[mms-checksum]</td>
 <td><code class="docutils literal notranslate">v6.0.0 -> latest</code></td> </table>
 </div>
 </li>
        <li> <span class="li-head">mm4_outbreak_prevention</span> - Enable Virus Outbreak Prevention service. <span class="li-normal">type: str</span> <span class="li-normal">choices: disabled, files, full-archive</span>
 <a id='label116' href="javascript:ContentClick('label117', 'label116');" onmouseover="ContentPreview('label117');" onmouseout="ContentUnpreview('label117');" title="click to collapse or expand..."> more... </a>
 <div id="label117" style="display:none">
 <table border="1">
 <tr>
 <td></td>
 <td colspan="1">Supported Version Ranges</td>
 </tr>
 <tr>
 <td>mm4_outbreak_prevention</td>
 <td><code class="docutils literal notranslate">v6.0.0 -> v6.2.7 </code></td>
 </tr>
 <tr>
 <td>[disabled]</td>
 <td><code class="docutils literal notranslate">v6.0.0 -> latest</code></td> <tr>
 <td>[files]</td>
 <td><code class="docutils literal notranslate">v6.0.0 -> latest</code></td> <tr>
 <td>[full-archive]</td>
 <td><code class="docutils literal notranslate">v6.0.0 -> latest</code></td> </table>
 </div>
 </li>
        <li> <span class="li-head">mm4oversizelimit</span> - Maximum file size to scan (1 - 819200 kB). <span class="li-normal">type: int</span>
 <a id='label118' href="javascript:ContentClick('label119', 'label118');" onmouseover="ContentPreview('label119');" onmouseout="ContentUnpreview('label119');" title="click to collapse or expand..."> more... </a>
 <div id="label119" style="display:none">
 <table border="1">
 <tr>
 <td></td>
 <td colspan="1">Supported Version Ranges</td>
 </tr>
 <tr>
 <td>mm4oversizelimit</td>
 <td><code class="docutils literal notranslate">v6.0.0 -> v6.2.7 </code></td>
 </tr>
 </table>
 </div>
 </li>
        <li> <span class="li-head">mm7</span> - MM7 options. <span class="li-normal">type: list</span> <span class="li-normal">choices: avmonitor, oversize, quarantine, scan, bannedword, chunkedbypass, clientcomfort, servercomfort, carrier-endpoint-bwl, remove-blocked, mms-checksum</span>
 <a id='label120' href="javascript:ContentClick('label121', 'label120');" onmouseover="ContentPreview('label121');" onmouseout="ContentUnpreview('label121');" title="click to collapse or expand..."> more... </a>
 <div id="label121" style="display:none">
 <table border="1">
 <tr>
 <td></td>
 <td colspan="1">Supported Version Ranges</td>
 </tr>
 <tr>
 <td>mm7</td>
 <td><code class="docutils literal notranslate">v6.0.0 -> v6.2.7 </code></td>
 </tr>
 <tr>
 <td>[avmonitor]</td>
 <td><code class="docutils literal notranslate">v6.0.0 -> latest</code></td> <tr>
 <td>[oversize]</td>
 <td><code class="docutils literal notranslate">v6.0.0 -> latest</code></td> <tr>
 <td>[quarantine]</td>
 <td><code class="docutils literal notranslate">v6.0.0 -> latest</code></td> <tr>
 <td>[scan]</td>
 <td><code class="docutils literal notranslate">v6.0.0 -> latest</code></td> <tr>
 <td>[bannedword]</td>
 <td><code class="docutils literal notranslate">v6.0.0 -> latest</code></td> <tr>
 <td>[chunkedbypass]</td>
 <td><code class="docutils literal notranslate">v6.0.0 -> latest</code></td> <tr>
 <td>[clientcomfort]</td>
 <td><code class="docutils literal notranslate">v6.0.0 -> latest</code></td> <tr>
 <td>[servercomfort]</td>
 <td><code class="docutils literal notranslate">v6.0.0 -> latest</code></td> <tr>
 <td>[carrier-endpoint-bwl]</td>
 <td><code class="docutils literal notranslate">v6.0.0 -> latest</code></td> <tr>
 <td>[remove-blocked]</td>
 <td><code class="docutils literal notranslate">v6.0.0 -> latest</code></td> <tr>
 <td>[mms-checksum]</td>
 <td><code class="docutils literal notranslate">v6.0.0 -> latest</code></td> </table>
 </div>
 </li>
        <li> <span class="li-head">mm7_addr_hdr</span> - HTTP header field (for MM7) containing user address. <span class="li-normal">type: str</span>
 <a id='label122' href="javascript:ContentClick('label123', 'label122');" onmouseover="ContentPreview('label123');" onmouseout="ContentUnpreview('label123');" title="click to collapse or expand..."> more... </a>
 <div id="label123" style="display:none">
 <table border="1">
 <tr>
 <td></td>
 <td colspan="1">Supported Version Ranges</td>
 </tr>
 <tr>
 <td>mm7_addr_hdr</td>
 <td><code class="docutils literal notranslate">v6.0.0 -> v6.2.7 </code></td>
 </tr>
 </table>
 </div>
 </li>
        <li> <span class="li-head">mm7_addr_source</span> - Source for MM7 user address. <span class="li-normal">type: str</span> <span class="li-normal">choices: http-header, cookie</span>
 <a id='label124' href="javascript:ContentClick('label125', 'label124');" onmouseover="ContentPreview('label125');" onmouseout="ContentUnpreview('label125');" title="click to collapse or expand..."> more... </a>
 <div id="label125" style="display:none">
 <table border="1">
 <tr>
 <td></td>
 <td colspan="1">Supported Version Ranges</td>
 </tr>
 <tr>
 <td>mm7_addr_source</td>
 <td><code class="docutils literal notranslate">v6.0.0 -> v6.2.7 </code></td>
 </tr>
 <tr>
 <td>[http-header]</td>
 <td><code class="docutils literal notranslate">v6.0.0 -> latest</code></td> <tr>
 <td>[cookie]</td>
 <td><code class="docutils literal notranslate">v6.0.0 -> latest</code></td> </table>
 </div>
 </li>
        <li> <span class="li-head">mm7_convert_hex</span> - Enable/disable conversion of user address from HEX string for MM7. <span class="li-normal">type: str</span> <span class="li-normal">choices: enable, disable</span>
 <a id='label126' href="javascript:ContentClick('label127', 'label126');" onmouseover="ContentPreview('label127');" onmouseout="ContentUnpreview('label127');" title="click to collapse or expand..."> more... </a>
 <div id="label127" style="display:none">
 <table border="1">
 <tr>
 <td></td>
 <td colspan="1">Supported Version Ranges</td>
 </tr>
 <tr>
 <td>mm7_convert_hex</td>
 <td><code class="docutils literal notranslate">v6.0.0 -> v6.2.7 </code></td>
 </tr>
 <tr>
 <td>[enable]</td>
 <td><code class="docutils literal notranslate">v6.0.0 -> latest</code></td> <tr>
 <td>[disable]</td>
 <td><code class="docutils literal notranslate">v6.0.0 -> latest</code></td> </table>
 </div>
 </li>
        <li> <span class="li-head">mm7_outbreak_prevention</span> - Enable Virus Outbreak Prevention service. <span class="li-normal">type: str</span> <span class="li-normal">choices: disabled, files, full-archive</span>
 <a id='label128' href="javascript:ContentClick('label129', 'label128');" onmouseover="ContentPreview('label129');" onmouseout="ContentUnpreview('label129');" title="click to collapse or expand..."> more... </a>
 <div id="label129" style="display:none">
 <table border="1">
 <tr>
 <td></td>
 <td colspan="1">Supported Version Ranges</td>
 </tr>
 <tr>
 <td>mm7_outbreak_prevention</td>
 <td><code class="docutils literal notranslate">v6.0.0 -> v6.2.7 </code></td>
 </tr>
 <tr>
 <td>[disabled]</td>
 <td><code class="docutils literal notranslate">v6.0.0 -> latest</code></td> <tr>
 <td>[files]</td>
 <td><code class="docutils literal notranslate">v6.0.0 -> latest</code></td> <tr>
 <td>[full-archive]</td>
 <td><code class="docutils literal notranslate">v6.0.0 -> latest</code></td> </table>
 </div>
 </li>
        <li> <span class="li-head">mm7comfortamount</span> - MM7 comfort amount (0 - 4294967295). <span class="li-normal">type: int</span>
 <a id='label130' href="javascript:ContentClick('label131', 'label130');" onmouseover="ContentPreview('label131');" onmouseout="ContentUnpreview('label131');" title="click to collapse or expand..."> more... </a>
 <div id="label131" style="display:none">
 <table border="1">
 <tr>
 <td></td>
 <td colspan="1">Supported Version Ranges</td>
 </tr>
 <tr>
 <td>mm7comfortamount</td>
 <td><code class="docutils literal notranslate">v6.0.0 -> v6.2.7 </code></td>
 </tr>
 </table>
 </div>
 </li>
        <li> <span class="li-head">mm7comfortinterval</span> - MM7 comfort interval (0 - 4294967295). <span class="li-normal">type: int</span>
 <a id='label132' href="javascript:ContentClick('label133', 'label132');" onmouseover="ContentPreview('label133');" onmouseout="ContentUnpreview('label133');" title="click to collapse or expand..."> more... </a>
 <div id="label133" style="display:none">
 <table border="1">
 <tr>
 <td></td>
 <td colspan="1">Supported Version Ranges</td>
 </tr>
 <tr>
 <td>mm7comfortinterval</td>
 <td><code class="docutils literal notranslate">v6.0.0 -> v6.2.7 </code></td>
 </tr>
 </table>
 </div>
 </li>
        <li> <span class="li-head">mm7oversizelimit</span> - Maximum file size to scan (1 - 819200 kB). <span class="li-normal">type: int</span>
 <a id='label134' href="javascript:ContentClick('label135', 'label134');" onmouseover="ContentPreview('label135');" onmouseout="ContentUnpreview('label135');" title="click to collapse or expand..."> more... </a>
 <div id="label135" style="display:none">
 <table border="1">
 <tr>
 <td></td>
 <td colspan="1">Supported Version Ranges</td>
 </tr>
 <tr>
 <td>mm7oversizelimit</td>
 <td><code class="docutils literal notranslate">v6.0.0 -> v6.2.7 </code></td>
 </tr>
 </table>
 </div>
 </li>
        <li> <span class="li-head">mms_antispam_mass_log</span> - Enable/disable logging for MMS antispam mass. <span class="li-normal">type: str</span> <span class="li-normal">choices: enable, disable</span>
 <a id='label136' href="javascript:ContentClick('label137', 'label136');" onmouseover="ContentPreview('label137');" onmouseout="ContentUnpreview('label137');" title="click to collapse or expand..."> more... </a>
 <div id="label137" style="display:none">
 <table border="1">
 <tr>
 <td></td>
 <td colspan="1">Supported Version Ranges</td>
 </tr>
 <tr>
 <td>mms_antispam_mass_log</td>
 <td><code class="docutils literal notranslate">v6.0.0 -> v6.2.7 </code></td>
 </tr>
 <tr>
 <td>[enable]</td>
 <td><code class="docutils literal notranslate">v6.0.0 -> latest</code></td> <tr>
 <td>[disable]</td>
 <td><code class="docutils literal notranslate">v6.0.0 -> latest</code></td> </table>
 </div>
 </li>
        <li> <span class="li-head">mms_av_block_log</span> - Enable/disable logging for MMS antivirus file blocking. <span class="li-normal">type: str</span> <span class="li-normal">choices: enable, disable</span>
 <a id='label138' href="javascript:ContentClick('label139', 'label138');" onmouseover="ContentPreview('label139');" onmouseout="ContentUnpreview('label139');" title="click to collapse or expand..."> more... </a>
 <div id="label139" style="display:none">
 <table border="1">
 <tr>
 <td></td>
 <td colspan="1">Supported Version Ranges</td>
 </tr>
 <tr>
 <td>mms_av_block_log</td>
 <td><code class="docutils literal notranslate">v6.0.0 -> v6.2.7 </code></td>
 </tr>
 <tr>
 <td>[enable]</td>
 <td><code class="docutils literal notranslate">v6.0.0 -> latest</code></td> <tr>
 <td>[disable]</td>
 <td><code class="docutils literal notranslate">v6.0.0 -> latest</code></td> </table>
 </div>
 </li>
        <li> <span class="li-head">mms_av_oversize_log</span> - Enable/disable logging for MMS antivirus oversize file blocking. <span class="li-normal">type: str</span> <span class="li-normal">choices: enable, disable</span>
 <a id='label140' href="javascript:ContentClick('label141', 'label140');" onmouseover="ContentPreview('label141');" onmouseout="ContentUnpreview('label141');" title="click to collapse or expand..."> more... </a>
 <div id="label141" style="display:none">
 <table border="1">
 <tr>
 <td></td>
 <td colspan="1">Supported Version Ranges</td>
 </tr>
 <tr>
 <td>mms_av_oversize_log</td>
 <td><code class="docutils literal notranslate">v6.0.0 -> v6.2.7 </code></td>
 </tr>
 <tr>
 <td>[enable]</td>
 <td><code class="docutils literal notranslate">v6.0.0 -> latest</code></td> <tr>
 <td>[disable]</td>
 <td><code class="docutils literal notranslate">v6.0.0 -> latest</code></td> </table>
 </div>
 </li>
        <li> <span class="li-head">mms_av_virus_log</span> - Enable/disable logging for MMS antivirus scanning. <span class="li-normal">type: str</span> <span class="li-normal">choices: enable, disable</span>
 <a id='label142' href="javascript:ContentClick('label143', 'label142');" onmouseover="ContentPreview('label143');" onmouseout="ContentUnpreview('label143');" title="click to collapse or expand..."> more... </a>
 <div id="label143" style="display:none">
 <table border="1">
 <tr>
 <td></td>
 <td colspan="1">Supported Version Ranges</td>
 </tr>
 <tr>
 <td>mms_av_virus_log</td>
 <td><code class="docutils literal notranslate">v6.0.0 -> v6.2.7 </code></td>
 </tr>
 <tr>
 <td>[enable]</td>
 <td><code class="docutils literal notranslate">v6.0.0 -> latest</code></td> <tr>
 <td>[disable]</td>
 <td><code class="docutils literal notranslate">v6.0.0 -> latest</code></td> </table>
 </div>
 </li>
        <li> <span class="li-head">mms_carrier_endpoint_filter_log</span> - Enable/disable logging for MMS end point filter blocking. <span class="li-normal">type: str</span> <span class="li-normal">choices: enable, disable</span>
 <a id='label144' href="javascript:ContentClick('label145', 'label144');" onmouseover="ContentPreview('label145');" onmouseout="ContentUnpreview('label145');" title="click to collapse or expand..."> more... </a>
 <div id="label145" style="display:none">
 <table border="1">
 <tr>
 <td></td>
 <td colspan="1">Supported Version Ranges</td>
 </tr>
 <tr>
 <td>mms_carrier_endpoint_filter_log</td>
 <td><code class="docutils literal notranslate">v6.0.0 -> v6.2.7 </code></td>
 </tr>
 <tr>
 <td>[enable]</td>
 <td><code class="docutils literal notranslate">v6.0.0 -> latest</code></td> <tr>
 <td>[disable]</td>
 <td><code class="docutils literal notranslate">v6.0.0 -> latest</code></td> </table>
 </div>
 </li>
        <li> <span class="li-head">mms_checksum_log</span> - Enable/disable MMS content checksum logging. <span class="li-normal">type: str</span> <span class="li-normal">choices: enable, disable</span>
 <a id='label146' href="javascript:ContentClick('label147', 'label146');" onmouseover="ContentPreview('label147');" onmouseout="ContentUnpreview('label147');" title="click to collapse or expand..."> more... </a>
 <div id="label147" style="display:none">
 <table border="1">
 <tr>
 <td></td>
 <td colspan="1">Supported Version Ranges</td>
 </tr>
 <tr>
 <td>mms_checksum_log</td>
 <td><code class="docutils literal notranslate">v6.0.0 -> v6.2.7 </code></td>
 </tr>
 <tr>
 <td>[enable]</td>
 <td><code class="docutils literal notranslate">v6.0.0 -> latest</code></td> <tr>
 <td>[disable]</td>
 <td><code class="docutils literal notranslate">v6.0.0 -> latest</code></td> </table>
 </div>
 </li>
        <li> <span class="li-head">mms_checksum_table</span> - MMS content checksum table ID. Source antivirus.mms-checksum.id. <span class="li-normal">type: int</span>
 <a id='label148' href="javascript:ContentClick('label149', 'label148');" onmouseover="ContentPreview('label149');" onmouseout="ContentUnpreview('label149');" title="click to collapse or expand..."> more... </a>
 <div id="label149" style="display:none">
 <table border="1">
 <tr>
 <td></td>
 <td colspan="1">Supported Version Ranges</td>
 </tr>
 <tr>
 <td>mms_checksum_table</td>
 <td><code class="docutils literal notranslate">v6.0.0 -> v6.2.7 </code></td>
 </tr>
 </table>
 </div>
 </li>
        <li> <span class="li-head">mms_notification_log</span> - Enable/disable logging for MMS notification messages. <span class="li-normal">type: str</span> <span class="li-normal">choices: enable, disable</span>
 <a id='label150' href="javascript:ContentClick('label151', 'label150');" onmouseover="ContentPreview('label151');" onmouseout="ContentUnpreview('label151');" title="click to collapse or expand..."> more... </a>
 <div id="label151" style="display:none">
 <table border="1">
 <tr>
 <td></td>
 <td colspan="1">Supported Version Ranges</td>
 </tr>
 <tr>
 <td>mms_notification_log</td>
 <td><code class="docutils literal notranslate">v6.0.0 -> v6.2.7 </code></td>
 </tr>
 <tr>
 <td>[enable]</td>
 <td><code class="docutils literal notranslate">v6.0.0 -> latest</code></td> <tr>
 <td>[disable]</td>
 <td><code class="docutils literal notranslate">v6.0.0 -> latest</code></td> </table>
 </div>
 </li>
        <li> <span class="li-head">mms_web_content_log</span> - Enable/disable logging for MMS web content blocking. <span class="li-normal">type: str</span> <span class="li-normal">choices: enable, disable</span>
 <a id='label152' href="javascript:ContentClick('label153', 'label152');" onmouseover="ContentPreview('label153');" onmouseout="ContentUnpreview('label153');" title="click to collapse or expand..."> more... </a>
 <div id="label153" style="display:none">
 <table border="1">
 <tr>
 <td></td>
 <td colspan="1">Supported Version Ranges</td>
 </tr>
 <tr>
 <td>mms_web_content_log</td>
 <td><code class="docutils literal notranslate">v6.0.0 -> v6.2.7 </code></td>
 </tr>
 <tr>
 <td>[enable]</td>
 <td><code class="docutils literal notranslate">v6.0.0 -> latest</code></td> <tr>
 <td>[disable]</td>
 <td><code class="docutils literal notranslate">v6.0.0 -> latest</code></td> </table>
 </div>
 </li>
        <li> <span class="li-head">mmsbwordthreshold</span> - MMS banned word threshold. <span class="li-normal">type: int</span>
 <a id='label154' href="javascript:ContentClick('label155', 'label154');" onmouseover="ContentPreview('label155');" onmouseout="ContentUnpreview('label155');" title="click to collapse or expand..."> more... </a>
 <div id="label155" style="display:none">
 <table border="1">
 <tr>
 <td></td>
 <td colspan="1">Supported Version Ranges</td>
 </tr>
 <tr>
 <td>mmsbwordthreshold</td>
 <td><code class="docutils literal notranslate">v6.0.0 -> v6.2.7 </code></td>
 </tr>
 </table>
 </div>
 </li>
        <li> <span class="li-head">name</span> - Profile name. <span class="li-normal">type: str</span> <span class="li-required">required: true</span>
 <a id='label156' href="javascript:ContentClick('label157', 'label156');" onmouseover="ContentPreview('label157');" onmouseout="ContentUnpreview('label157');" title="click to collapse or expand..."> more... </a>
 <div id="label157" style="display:none">
 <table border="1">
 <tr>
 <td></td>
 <td colspan="1">Supported Version Ranges</td>
 </tr>
 <tr>
 <td>name</td>
 <td><code class="docutils literal notranslate">v6.0.0 -> v6.2.7 </code></td>
 </tr>
 </table>
 </div>
 </li>
        <li> <span class="li-head">notif_msisdn</span> - Notification for MSISDNs. <span class="li-normal">type: list</span> <span style="font-family:'Courier New'" class="li-required">member_path: notif_msisdn:msisdn</span>
 <a id='label158' href="javascript:ContentClick('label159', 'label158');" onmouseover="ContentPreview('label159');" onmouseout="ContentUnpreview('label159');" title="click to collapse or expand..."> more... </a>
 <div id="label159" style="display:none">
 <table border="1">
 <tr>
 <td></td><td colspan="1">Supported Version Ranges</td>
 </tr>
 <tr>
 <td>notif_msisdn</td>
 <td><code class="docutils literal notranslate">v6.0.0 -> v6.2.7 </code></td>
 </tr>
 </table>
 </div>
 </li>
            <ul class="ul-self">
            <li> <span class="li-head">msisdn</span> - Recipient MSISDN. <span class="li-normal">type: str</span> <span class="li-required">required: true</span>
 <a id='label160' href="javascript:ContentClick('label161', 'label160');" onmouseover="ContentPreview('label161');" onmouseout="ContentUnpreview('label161');" title="click to collapse or expand..."> more... </a>
 <div id="label161" style="display:none">
 <table border="1">
 <tr>
 <td></td>
 <td colspan="1">Supported Version Ranges</td>
 </tr>
 <tr>
 <td>msisdn</td>
 <td><code class="docutils literal notranslate">v6.0.0 -> v6.2.7 </code></td>
 </tr>
 </table>
 </div>
 </li>
            <li> <span class="li-head">threshold</span> - Thresholds on which this MSISDN will receive an alert. <span class="li-normal">type: list</span> <span class="li-normal">choices: flood-thresh-1, flood-thresh-2, flood-thresh-3, dupe-thresh-1, dupe-thresh-2, dupe-thresh-3</span>
 <a id='label162' href="javascript:ContentClick('label163', 'label162');" onmouseover="ContentPreview('label163');" onmouseout="ContentUnpreview('label163');" title="click to collapse or expand..."> more... </a>
 <div id="label163" style="display:none">
 <table border="1">
 <tr>
 <td></td>
 <td colspan="1">Supported Version Ranges</td>
 </tr>
 <tr>
 <td>threshold</td>
 <td><code class="docutils literal notranslate">v6.0.0 -> v6.2.7 </code></td>
 </tr>
 <tr>
 <td>[flood-thresh-1]</td>
 <td><code class="docutils literal notranslate">v6.0.0 -> latest</code></td> <tr>
 <td>[flood-thresh-2]</td>
 <td><code class="docutils literal notranslate">v6.0.0 -> latest</code></td> <tr>
 <td>[flood-thresh-3]</td>
 <td><code class="docutils literal notranslate">v6.0.0 -> latest</code></td> <tr>
 <td>[dupe-thresh-1]</td>
 <td><code class="docutils literal notranslate">v6.0.0 -> latest</code></td> <tr>
 <td>[dupe-thresh-2]</td>
 <td><code class="docutils literal notranslate">v6.0.0 -> latest</code></td> <tr>
 <td>[dupe-thresh-3]</td>
 <td><code class="docutils literal notranslate">v6.0.0 -> latest</code></td> </table>
 </div>
 </li>
            </ul>
        <li> <span class="li-head">notification</span> - Notification configuration. <span class="li-normal">type: list</span> <span style="font-family:'Courier New'" class="li-required">member_path: notification:protocol</span>
 <a id='label164' href="javascript:ContentClick('label165', 'label164');" onmouseover="ContentPreview('label165');" onmouseout="ContentUnpreview('label165');" title="click to collapse or expand..."> more... </a>
 <div id="label165" style="display:none">
 <table border="1">
 <tr>
 <td></td><td colspan="1">Supported Version Ranges</td>
 </tr>
 <tr>
 <td>notification</td>
 <td><code class="docutils literal notranslate">v6.0.0 -> v6.2.7 </code></td>
 </tr>
 </table>
 </div>
 </li>
            <ul class="ul-self">
            <li> <span class="li-head">alert_int</span> - Alert notification send interval. <span class="li-normal">type: int</span>
 <a id='label166' href="javascript:ContentClick('label167', 'label166');" onmouseover="ContentPreview('label167');" onmouseout="ContentUnpreview('label167');" title="click to collapse or expand..."> more... </a>
 <div id="label167" style="display:none">
 <table border="1">
 <tr>
 <td></td>
 <td colspan="1">Supported Version Ranges</td>
 </tr>
 <tr>
 <td>alert_int</td>
 <td><code class="docutils literal notranslate">v6.0.0 -> v6.2.7 </code></td>
 </tr>
 </table>
 </div>
 </li>
            <li> <span class="li-head">alert_int_mode</span> - Alert notification interval mode. <span class="li-normal">type: str</span> <span class="li-normal">choices: hours, minutes</span>
 <a id='label168' href="javascript:ContentClick('label169', 'label168');" onmouseover="ContentPreview('label169');" onmouseout="ContentUnpreview('label169');" title="click to collapse or expand..."> more... </a>
 <div id="label169" style="display:none">
 <table border="1">
 <tr>
 <td></td>
 <td colspan="1">Supported Version Ranges</td>
 </tr>
 <tr>
 <td>alert_int_mode</td>
 <td><code class="docutils literal notranslate">v6.0.0 -> v6.2.7 </code></td>
 </tr>
 <tr>
 <td>[hours]</td>
 <td><code class="docutils literal notranslate">v6.0.0 -> latest</code></td> <tr>
 <td>[minutes]</td>
 <td><code class="docutils literal notranslate">v6.0.0 -> latest</code></td> </table>
 </div>
 </li>
            <li> <span class="li-head">alert_src_msisdn</span> - Specify from address for alert messages. <span class="li-normal">type: str</span>
 <a id='label170' href="javascript:ContentClick('label171', 'label170');" onmouseover="ContentPreview('label171');" onmouseout="ContentUnpreview('label171');" title="click to collapse or expand..."> more... </a>
 <div id="label171" style="display:none">
 <table border="1">
 <tr>
 <td></td>
 <td colspan="1">Supported Version Ranges</td>
 </tr>
 <tr>
 <td>alert_src_msisdn</td>
 <td><code class="docutils literal notranslate">v6.0.0 -> v6.2.7 </code></td>
 </tr>
 </table>
 </div>
 </li>
            <li> <span class="li-head">alert_status</span> - Alert notification status. <span class="li-normal">type: str</span> <span class="li-normal">choices: enable, disable</span>
 <a id='label172' href="javascript:ContentClick('label173', 'label172');" onmouseover="ContentPreview('label173');" onmouseout="ContentUnpreview('label173');" title="click to collapse or expand..."> more... </a>
 <div id="label173" style="display:none">
 <table border="1">
 <tr>
 <td></td>
 <td colspan="1">Supported Version Ranges</td>
 </tr>
 <tr>
 <td>alert_status</td>
 <td><code class="docutils literal notranslate">v6.0.0 -> v6.2.7 </code></td>
 </tr>
 <tr>
 <td>[enable]</td>
 <td><code class="docutils literal notranslate">v6.0.0 -> latest</code></td> <tr>
 <td>[disable]</td>
 <td><code class="docutils literal notranslate">v6.0.0 -> latest</code></td> </table>
 </div>
 </li>
            <li> <span class="li-head">bword_int</span> - Banned word notification send interval. <span class="li-normal">type: int</span>
 <a id='label174' href="javascript:ContentClick('label175', 'label174');" onmouseover="ContentPreview('label175');" onmouseout="ContentUnpreview('label175');" title="click to collapse or expand..."> more... </a>
 <div id="label175" style="display:none">
 <table border="1">
 <tr>
 <td></td>
 <td colspan="1">Supported Version Ranges</td>
 </tr>
 <tr>
 <td>bword_int</td>
 <td><code class="docutils literal notranslate">v6.0.0 -> v6.2.7 </code></td>
 </tr>
 </table>
 </div>
 </li>
            <li> <span class="li-head">bword_int_mode</span> - Banned word notification interval mode. <span class="li-normal">type: str</span> <span class="li-normal">choices: hours, minutes</span>
 <a id='label176' href="javascript:ContentClick('label177', 'label176');" onmouseover="ContentPreview('label177');" onmouseout="ContentUnpreview('label177');" title="click to collapse or expand..."> more... </a>
 <div id="label177" style="display:none">
 <table border="1">
 <tr>
 <td></td>
 <td colspan="1">Supported Version Ranges</td>
 </tr>
 <tr>
 <td>bword_int_mode</td>
 <td><code class="docutils literal notranslate">v6.0.0 -> v6.2.7 </code></td>
 </tr>
 <tr>
 <td>[hours]</td>
 <td><code class="docutils literal notranslate">v6.0.0 -> latest</code></td> <tr>
 <td>[minutes]</td>
 <td><code class="docutils literal notranslate">v6.0.0 -> latest</code></td> </table>
 </div>
 </li>
            <li> <span class="li-head">bword_status</span> - Banned word notification status. <span class="li-normal">type: str</span> <span class="li-normal">choices: enable, disable</span>
 <a id='label178' href="javascript:ContentClick('label179', 'label178');" onmouseover="ContentPreview('label179');" onmouseout="ContentUnpreview('label179');" title="click to collapse or expand..."> more... </a>
 <div id="label179" style="display:none">
 <table border="1">
 <tr>
 <td></td>
 <td colspan="1">Supported Version Ranges</td>
 </tr>
 <tr>
 <td>bword_status</td>
 <td><code class="docutils literal notranslate">v6.0.0 -> v6.2.7 </code></td>
 </tr>
 <tr>
 <td>[enable]</td>
 <td><code class="docutils literal notranslate">v6.0.0 -> latest</code></td> <tr>
 <td>[disable]</td>
 <td><code class="docutils literal notranslate">v6.0.0 -> latest</code></td> </table>
 </div>
 </li>
            <li> <span class="li-head">carrier_endpoint_bwl_int</span> - Carrier end point black/white list notification send interval. <span class="li-normal">type: int</span>
 <a id='label180' href="javascript:ContentClick('label181', 'label180');" onmouseover="ContentPreview('label181');" onmouseout="ContentUnpreview('label181');" title="click to collapse or expand..."> more... </a>
 <div id="label181" style="display:none">
 <table border="1">
 <tr>
 <td></td>
 <td colspan="1">Supported Version Ranges</td>
 </tr>
 <tr>
 <td>carrier_endpoint_bwl_int</td>
 <td><code class="docutils literal notranslate">v6.0.0 -> v6.2.7 </code></td>
 </tr>
 </table>
 </div>
 </li>
            <li> <span class="li-head">carrier_endpoint_bwl_int_mode</span> - Carrier end point black/white list notification interval mode. <span class="li-normal">type: str</span> <span class="li-normal">choices: hours, minutes</span>
 <a id='label182' href="javascript:ContentClick('label183', 'label182');" onmouseover="ContentPreview('label183');" onmouseout="ContentUnpreview('label183');" title="click to collapse or expand..."> more... </a>
 <div id="label183" style="display:none">
 <table border="1">
 <tr>
 <td></td>
 <td colspan="1">Supported Version Ranges</td>
 </tr>
 <tr>
 <td>carrier_endpoint_bwl_int_mode</td>
 <td><code class="docutils literal notranslate">v6.0.0 -> v6.2.7 </code></td>
 </tr>
 <tr>
 <td>[hours]</td>
 <td><code class="docutils literal notranslate">v6.0.0 -> latest</code></td> <tr>
 <td>[minutes]</td>
 <td><code class="docutils literal notranslate">v6.0.0 -> latest</code></td> </table>
 </div>
 </li>
            <li> <span class="li-head">carrier_endpoint_bwl_status</span> - Carrier end point black/white list notification status. <span class="li-normal">type: str</span> <span class="li-normal">choices: enable, disable</span>
 <a id='label184' href="javascript:ContentClick('label185', 'label184');" onmouseover="ContentPreview('label185');" onmouseout="ContentUnpreview('label185');" title="click to collapse or expand..."> more... </a>
 <div id="label185" style="display:none">
 <table border="1">
 <tr>
 <td></td>
 <td colspan="1">Supported Version Ranges</td>
 </tr>
 <tr>
 <td>carrier_endpoint_bwl_status</td>
 <td><code class="docutils literal notranslate">v6.0.0 -> v6.2.7 </code></td>
 </tr>
 <tr>
 <td>[enable]</td>
 <td><code class="docutils literal notranslate">v6.0.0 -> latest</code></td> <tr>
 <td>[disable]</td>
 <td><code class="docutils literal notranslate">v6.0.0 -> latest</code></td> </table>
 </div>
 </li>
            <li> <span class="li-head">days_allowed</span> - Weekdays on which notification messages may be sent. <span class="li-normal">type: list</span> <span class="li-normal">choices: sunday, monday, tuesday, wednesday, thursday, friday, saturday</span>
 <a id='label186' href="javascript:ContentClick('label187', 'label186');" onmouseover="ContentPreview('label187');" onmouseout="ContentUnpreview('label187');" title="click to collapse or expand..."> more... </a>
 <div id="label187" style="display:none">
 <table border="1">
 <tr>
 <td></td>
 <td colspan="1">Supported Version Ranges</td>
 </tr>
 <tr>
 <td>days_allowed</td>
 <td><code class="docutils literal notranslate">v6.0.0 -> v6.2.7 </code></td>
 </tr>
 <tr>
 <td>[sunday]</td>
 <td><code class="docutils literal notranslate">v6.0.0 -> latest</code></td> <tr>
 <td>[monday]</td>
 <td><code class="docutils literal notranslate">v6.0.0 -> latest</code></td> <tr>
 <td>[tuesday]</td>
 <td><code class="docutils literal notranslate">v6.0.0 -> latest</code></td> <tr>
 <td>[wednesday]</td>
 <td><code class="docutils literal notranslate">v6.0.0 -> latest</code></td> <tr>
 <td>[thursday]</td>
 <td><code class="docutils literal notranslate">v6.0.0 -> latest</code></td> <tr>
 <td>[friday]</td>
 <td><code class="docutils literal notranslate">v6.0.0 -> latest</code></td> <tr>
 <td>[saturday]</td>
 <td><code class="docutils literal notranslate">v6.0.0 -> latest</code></td> </table>
 </div>
 </li>
            <li> <span class="li-head">detect_server</span> - Enable/disable automatic server address determination. <span class="li-normal">type: str</span> <span class="li-normal">choices: enable, disable</span>
 <a id='label188' href="javascript:ContentClick('label189', 'label188');" onmouseover="ContentPreview('label189');" onmouseout="ContentUnpreview('label189');" title="click to collapse or expand..."> more... </a>
 <div id="label189" style="display:none">
 <table border="1">
 <tr>
 <td></td>
 <td colspan="1">Supported Version Ranges</td>
 </tr>
 <tr>
 <td>detect_server</td>
 <td><code class="docutils literal notranslate">v6.0.0 -> v6.2.7 </code></td>
 </tr>
 <tr>
 <td>[enable]</td>
 <td><code class="docutils literal notranslate">v6.0.0 -> latest</code></td> <tr>
 <td>[disable]</td>
 <td><code class="docutils literal notranslate">v6.0.0 -> latest</code></td> </table>
 </div>
 </li>
            <li> <span class="li-head">dupe_int</span> - Duplicate notification send interval. <span class="li-normal">type: int</span>
 <a id='label190' href="javascript:ContentClick('label191', 'label190');" onmouseover="ContentPreview('label191');" onmouseout="ContentUnpreview('label191');" title="click to collapse or expand..."> more... </a>
 <div id="label191" style="display:none">
 <table border="1">
 <tr>
 <td></td>
 <td colspan="1">Supported Version Ranges</td>
 </tr>
 <tr>
 <td>dupe_int</td>
 <td><code class="docutils literal notranslate">v6.0.0 -> v6.2.7 </code></td>
 </tr>
 </table>
 </div>
 </li>
            <li> <span class="li-head">dupe_int_mode</span> - Duplicate notification interval mode. <span class="li-normal">type: str</span> <span class="li-normal">choices: hours, minutes</span>
 <a id='label192' href="javascript:ContentClick('label193', 'label192');" onmouseover="ContentPreview('label193');" onmouseout="ContentUnpreview('label193');" title="click to collapse or expand..."> more... </a>
 <div id="label193" style="display:none">
 <table border="1">
 <tr>
 <td></td>
 <td colspan="1">Supported Version Ranges</td>
 </tr>
 <tr>
 <td>dupe_int_mode</td>
 <td><code class="docutils literal notranslate">v6.0.0 -> v6.2.7 </code></td>
 </tr>
 <tr>
 <td>[hours]</td>
 <td><code class="docutils literal notranslate">v6.0.0 -> latest</code></td> <tr>
 <td>[minutes]</td>
 <td><code class="docutils literal notranslate">v6.0.0 -> latest</code></td> </table>
 </div>
 </li>
            <li> <span class="li-head">dupe_status</span> - Duplicate notification status. <span class="li-normal">type: str</span> <span class="li-normal">choices: enable, disable</span>
 <a id='label194' href="javascript:ContentClick('label195', 'label194');" onmouseover="ContentPreview('label195');" onmouseout="ContentUnpreview('label195');" title="click to collapse or expand..."> more... </a>
 <div id="label195" style="display:none">
 <table border="1">
 <tr>
 <td></td>
 <td colspan="1">Supported Version Ranges</td>
 </tr>
 <tr>
 <td>dupe_status</td>
 <td><code class="docutils literal notranslate">v6.0.0 -> v6.2.7 </code></td>
 </tr>
 <tr>
 <td>[enable]</td>
 <td><code class="docutils literal notranslate">v6.0.0 -> latest</code></td> <tr>
 <td>[disable]</td>
 <td><code class="docutils literal notranslate">v6.0.0 -> latest</code></td> </table>
 </div>
 </li>
            <li> <span class="li-head">file_block_int</span> - File block notification send interval. <span class="li-normal">type: int</span>
 <a id='label196' href="javascript:ContentClick('label197', 'label196');" onmouseover="ContentPreview('label197');" onmouseout="ContentUnpreview('label197');" title="click to collapse or expand..."> more... </a>
 <div id="label197" style="display:none">
 <table border="1">
 <tr>
 <td></td>
 <td colspan="1">Supported Version Ranges</td>
 </tr>
 <tr>
 <td>file_block_int</td>
 <td><code class="docutils literal notranslate">v6.0.0 -> v6.2.7 </code></td>
 </tr>
 </table>
 </div>
 </li>
            <li> <span class="li-head">file_block_int_mode</span> - File block notification interval mode. <span class="li-normal">type: str</span> <span class="li-normal">choices: hours, minutes</span>
 <a id='label198' href="javascript:ContentClick('label199', 'label198');" onmouseover="ContentPreview('label199');" onmouseout="ContentUnpreview('label199');" title="click to collapse or expand..."> more... </a>
 <div id="label199" style="display:none">
 <table border="1">
 <tr>
 <td></td>
 <td colspan="1">Supported Version Ranges</td>
 </tr>
 <tr>
 <td>file_block_int_mode</td>
 <td><code class="docutils literal notranslate">v6.0.0 -> v6.2.7 </code></td>
 </tr>
 <tr>
 <td>[hours]</td>
 <td><code class="docutils literal notranslate">v6.0.0 -> latest</code></td> <tr>
 <td>[minutes]</td>
 <td><code class="docutils literal notranslate">v6.0.0 -> latest</code></td> </table>
 </div>
 </li>
            <li> <span class="li-head">file_block_status</span> - File block notification status. <span class="li-normal">type: str</span> <span class="li-normal">choices: enable, disable</span>
 <a id='label200' href="javascript:ContentClick('label201', 'label200');" onmouseover="ContentPreview('label201');" onmouseout="ContentUnpreview('label201');" title="click to collapse or expand..."> more... </a>
 <div id="label201" style="display:none">
 <table border="1">
 <tr>
 <td></td>
 <td colspan="1">Supported Version Ranges</td>
 </tr>
 <tr>
 <td>file_block_status</td>
 <td><code class="docutils literal notranslate">v6.0.0 -> v6.2.7 </code></td>
 </tr>
 <tr>
 <td>[enable]</td>
 <td><code class="docutils literal notranslate">v6.0.0 -> latest</code></td> <tr>
 <td>[disable]</td>
 <td><code class="docutils literal notranslate">v6.0.0 -> latest</code></td> </table>
 </div>
 </li>
            <li> <span class="li-head">flood_int</span> - Flood notification send interval. <span class="li-normal">type: int</span>
 <a id='label202' href="javascript:ContentClick('label203', 'label202');" onmouseover="ContentPreview('label203');" onmouseout="ContentUnpreview('label203');" title="click to collapse or expand..."> more... </a>
 <div id="label203" style="display:none">
 <table border="1">
 <tr>
 <td></td>
 <td colspan="1">Supported Version Ranges</td>
 </tr>
 <tr>
 <td>flood_int</td>
 <td><code class="docutils literal notranslate">v6.0.0 -> v6.2.7 </code></td>
 </tr>
 </table>
 </div>
 </li>
            <li> <span class="li-head">flood_int_mode</span> - Flood notification interval mode. <span class="li-normal">type: str</span> <span class="li-normal">choices: hours, minutes</span>
 <a id='label204' href="javascript:ContentClick('label205', 'label204');" onmouseover="ContentPreview('label205');" onmouseout="ContentUnpreview('label205');" title="click to collapse or expand..."> more... </a>
 <div id="label205" style="display:none">
 <table border="1">
 <tr>
 <td></td>
 <td colspan="1">Supported Version Ranges</td>
 </tr>
 <tr>
 <td>flood_int_mode</td>
 <td><code class="docutils literal notranslate">v6.0.0 -> v6.2.7 </code></td>
 </tr>
 <tr>
 <td>[hours]</td>
 <td><code class="docutils literal notranslate">v6.0.0 -> latest</code></td> <tr>
 <td>[minutes]</td>
 <td><code class="docutils literal notranslate">v6.0.0 -> latest</code></td> </table>
 </div>
 </li>
            <li> <span class="li-head">flood_status</span> - Flood notification status. <span class="li-normal">type: str</span> <span class="li-normal">choices: enable, disable</span>
 <a id='label206' href="javascript:ContentClick('label207', 'label206');" onmouseover="ContentPreview('label207');" onmouseout="ContentUnpreview('label207');" title="click to collapse or expand..."> more... </a>
 <div id="label207" style="display:none">
 <table border="1">
 <tr>
 <td></td>
 <td colspan="1">Supported Version Ranges</td>
 </tr>
 <tr>
 <td>flood_status</td>
 <td><code class="docutils literal notranslate">v6.0.0 -> v6.2.7 </code></td>
 </tr>
 <tr>
 <td>[enable]</td>
 <td><code class="docutils literal notranslate">v6.0.0 -> latest</code></td> <tr>
 <td>[disable]</td>
 <td><code class="docutils literal notranslate">v6.0.0 -> latest</code></td> </table>
 </div>
 </li>
            <li> <span class="li-head">from_in_header</span> - Enable/disable insertion of from address in HTTP header. <span class="li-normal">type: str</span> <span class="li-normal">choices: enable, disable</span>
 <a id='label208' href="javascript:ContentClick('label209', 'label208');" onmouseover="ContentPreview('label209');" onmouseout="ContentUnpreview('label209');" title="click to collapse or expand..."> more... </a>
 <div id="label209" style="display:none">
 <table border="1">
 <tr>
 <td></td>
 <td colspan="1">Supported Version Ranges</td>
 </tr>
 <tr>
 <td>from_in_header</td>
 <td><code class="docutils literal notranslate">v6.0.0 -> v6.2.7 </code></td>
 </tr>
 <tr>
 <td>[enable]</td>
 <td><code class="docutils literal notranslate">v6.0.0 -> latest</code></td> <tr>
 <td>[disable]</td>
 <td><code class="docutils literal notranslate">v6.0.0 -> latest</code></td> </table>
 </div>
 </li>
            <li> <span class="li-head">mms_checksum_int</span> - MMS checksum notification send interval. <span class="li-normal">type: int</span>
 <a id='label210' href="javascript:ContentClick('label211', 'label210');" onmouseover="ContentPreview('label211');" onmouseout="ContentUnpreview('label211');" title="click to collapse or expand..."> more... </a>
 <div id="label211" style="display:none">
 <table border="1">
 <tr>
 <td></td>
 <td colspan="1">Supported Version Ranges</td>
 </tr>
 <tr>
 <td>mms_checksum_int</td>
 <td><code class="docutils literal notranslate">v6.0.0 -> v6.2.7 </code></td>
 </tr>
 </table>
 </div>
 </li>
            <li> <span class="li-head">mms_checksum_int_mode</span> - MMS checksum notification interval mode. <span class="li-normal">type: str</span> <span class="li-normal">choices: hours, minutes</span>
 <a id='label212' href="javascript:ContentClick('label213', 'label212');" onmouseover="ContentPreview('label213');" onmouseout="ContentUnpreview('label213');" title="click to collapse or expand..."> more... </a>
 <div id="label213" style="display:none">
 <table border="1">
 <tr>
 <td></td>
 <td colspan="1">Supported Version Ranges</td>
 </tr>
 <tr>
 <td>mms_checksum_int_mode</td>
 <td><code class="docutils literal notranslate">v6.0.0 -> v6.2.7 </code></td>
 </tr>
 <tr>
 <td>[hours]</td>
 <td><code class="docutils literal notranslate">v6.0.0 -> latest</code></td> <tr>
 <td>[minutes]</td>
 <td><code class="docutils literal notranslate">v6.0.0 -> latest</code></td> </table>
 </div>
 </li>
            <li> <span class="li-head">mms_checksum_status</span> - MMS checksum notification status. <span class="li-normal">type: str</span> <span class="li-normal">choices: enable, disable</span>
 <a id='label214' href="javascript:ContentClick('label215', 'label214');" onmouseover="ContentPreview('label215');" onmouseout="ContentUnpreview('label215');" title="click to collapse or expand..."> more... </a>
 <div id="label215" style="display:none">
 <table border="1">
 <tr>
 <td></td>
 <td colspan="1">Supported Version Ranges</td>
 </tr>
 <tr>
 <td>mms_checksum_status</td>
 <td><code class="docutils literal notranslate">v6.0.0 -> v6.2.7 </code></td>
 </tr>
 <tr>
 <td>[enable]</td>
 <td><code class="docutils literal notranslate">v6.0.0 -> latest</code></td> <tr>
 <td>[disable]</td>
 <td><code class="docutils literal notranslate">v6.0.0 -> latest</code></td> </table>
 </div>
 </li>
            <li> <span class="li-head">mmsc_hostname</span> - Host name or IP address of the MMSC. <span class="li-normal">type: str</span>
 <a id='label216' href="javascript:ContentClick('label217', 'label216');" onmouseover="ContentPreview('label217');" onmouseout="ContentUnpreview('label217');" title="click to collapse or expand..."> more... </a>
 <div id="label217" style="display:none">
 <table border="1">
 <tr>
 <td></td>
 <td colspan="1">Supported Version Ranges</td>
 </tr>
 <tr>
 <td>mmsc_hostname</td>
 <td><code class="docutils literal notranslate">v6.0.0 -> v6.2.7 </code></td>
 </tr>
 </table>
 </div>
 </li>
            <li> <span class="li-head">mmsc_password</span> - Password required for authentication with the MMSC. <span class="li-normal">type: str</span>
 <a id='label218' href="javascript:ContentClick('label219', 'label218');" onmouseover="ContentPreview('label219');" onmouseout="ContentUnpreview('label219');" title="click to collapse or expand..."> more... </a>
 <div id="label219" style="display:none">
 <table border="1">
 <tr>
 <td></td>
 <td colspan="1">Supported Version Ranges</td>
 </tr>
 <tr>
 <td>mmsc_password</td>
 <td><code class="docutils literal notranslate">v6.0.0 -> v6.2.7 </code></td>
 </tr>
 </table>
 </div>
 </li>
            <li> <span class="li-head">mmsc_port</span> - Port used on the MMSC for sending MMS messages (1 - 65535). <span class="li-normal">type: int</span>
 <a id='label220' href="javascript:ContentClick('label221', 'label220');" onmouseover="ContentPreview('label221');" onmouseout="ContentUnpreview('label221');" title="click to collapse or expand..."> more... </a>
 <div id="label221" style="display:none">
 <table border="1">
 <tr>
 <td></td>
 <td colspan="1">Supported Version Ranges</td>
 </tr>
 <tr>
 <td>mmsc_port</td>
 <td><code class="docutils literal notranslate">v6.0.0 -> v6.2.7 </code></td>
 </tr>
 </table>
 </div>
 </li>
            <li> <span class="li-head">mmsc_url</span> - URL used on the MMSC for sending MMS messages. <span class="li-normal">type: str</span>
 <a id='label222' href="javascript:ContentClick('label223', 'label222');" onmouseover="ContentPreview('label223');" onmouseout="ContentUnpreview('label223');" title="click to collapse or expand..."> more... </a>
 <div id="label223" style="display:none">
 <table border="1">
 <tr>
 <td></td>
 <td colspan="1">Supported Version Ranges</td>
 </tr>
 <tr>
 <td>mmsc_url</td>
 <td><code class="docutils literal notranslate">v6.0.0 -> v6.2.7 </code></td>
 </tr>
 </table>
 </div>
 </li>
            <li> <span class="li-head">mmsc_username</span> - User name required for authentication with the MMSC. <span class="li-normal">type: str</span>
 <a id='label224' href="javascript:ContentClick('label225', 'label224');" onmouseover="ContentPreview('label225');" onmouseout="ContentUnpreview('label225');" title="click to collapse or expand..."> more... </a>
 <div id="label225" style="display:none">
 <table border="1">
 <tr>
 <td></td>
 <td colspan="1">Supported Version Ranges</td>
 </tr>
 <tr>
 <td>mmsc_username</td>
 <td><code class="docutils literal notranslate">v6.0.0 -> v6.2.7 </code></td>
 </tr>
 </table>
 </div>
 </li>
            <li> <span class="li-head">msg_protocol</span> - Protocol to use for sending notification messages. <span class="li-normal">type: str</span> <span class="li-normal">choices: mm1, mm3, mm4, mm7</span>
 <a id='label226' href="javascript:ContentClick('label227', 'label226');" onmouseover="ContentPreview('label227');" onmouseout="ContentUnpreview('label227');" title="click to collapse or expand..."> more... </a>
 <div id="label227" style="display:none">
 <table border="1">
 <tr>
 <td></td>
 <td colspan="1">Supported Version Ranges</td>
 </tr>
 <tr>
 <td>msg_protocol</td>
 <td><code class="docutils literal notranslate">v6.0.0 -> v6.2.7 </code></td>
 </tr>
 <tr>
 <td>[mm1]</td>
 <td><code class="docutils literal notranslate">v6.0.0 -> latest</code></td> <tr>
 <td>[mm3]</td>
 <td><code class="docutils literal notranslate">v6.0.0 -> latest</code></td> <tr>
 <td>[mm4]</td>
 <td><code class="docutils literal notranslate">v6.0.0 -> latest</code></td> <tr>
 <td>[mm7]</td>
 <td><code class="docutils literal notranslate">v6.0.0 -> latest</code></td> </table>
 </div>
 </li>
            <li> <span class="li-head">msg_type</span> - MM7 message type. <span class="li-normal">type: str</span> <span class="li-normal">choices: submit-req, deliver-req</span>
 <a id='label228' href="javascript:ContentClick('label229', 'label228');" onmouseover="ContentPreview('label229');" onmouseout="ContentUnpreview('label229');" title="click to collapse or expand..."> more... </a>
 <div id="label229" style="display:none">
 <table border="1">
 <tr>
 <td></td>
 <td colspan="1">Supported Version Ranges</td>
 </tr>
 <tr>
 <td>msg_type</td>
 <td><code class="docutils literal notranslate">v6.0.0 -> v6.2.7 </code></td>
 </tr>
 <tr>
 <td>[submit-req]</td>
 <td><code class="docutils literal notranslate">v6.0.0 -> latest</code></td> <tr>
 <td>[deliver-req]</td>
 <td><code class="docutils literal notranslate">v6.0.0 -> latest</code></td> </table>
 </div>
 </li>
            <li> <span class="li-head">protocol</span> - Protocol. <span class="li-normal">type: str</span> <span class="li-required">required: true</span>
 <a id='label230' href="javascript:ContentClick('label231', 'label230');" onmouseover="ContentPreview('label231');" onmouseout="ContentUnpreview('label231');" title="click to collapse or expand..."> more... </a>
 <div id="label231" style="display:none">
 <table border="1">
 <tr>
 <td></td>
 <td colspan="1">Supported Version Ranges</td>
 </tr>
 <tr>
 <td>protocol</td>
 <td><code class="docutils literal notranslate">v6.0.0 -> v6.2.7 </code></td>
 </tr>
 </table>
 </div>
 </li>
            <li> <span class="li-head">rate_limit</span> - Rate limit for sending notification messages (0 - 250). <span class="li-normal">type: int</span>
 <a id='label232' href="javascript:ContentClick('label233', 'label232');" onmouseover="ContentPreview('label233');" onmouseout="ContentUnpreview('label233');" title="click to collapse or expand..."> more... </a>
 <div id="label233" style="display:none">
 <table border="1">
 <tr>
 <td></td>
 <td colspan="1">Supported Version Ranges</td>
 </tr>
 <tr>
 <td>rate_limit</td>
 <td><code class="docutils literal notranslate">v6.0.0 -> v6.2.7 </code></td>
 </tr>
 </table>
 </div>
 </li>
            <li> <span class="li-head">tod_window_duration</span> - Time of day window duration. <span class="li-normal">type: str</span>
 <a id='label234' href="javascript:ContentClick('label235', 'label234');" onmouseover="ContentPreview('label235');" onmouseout="ContentUnpreview('label235');" title="click to collapse or expand..."> more... </a>
 <div id="label235" style="display:none">
 <table border="1">
 <tr>
 <td></td>
 <td colspan="1">Supported Version Ranges</td>
 </tr>
 <tr>
 <td>tod_window_duration</td>
 <td><code class="docutils literal notranslate">v6.0.0 -> v6.2.7 </code></td>
 </tr>
 </table>
 </div>
 </li>
            <li> <span class="li-head">tod_window_end</span> - Obsolete. <span class="li-normal">type: str</span>
 <a id='label236' href="javascript:ContentClick('label237', 'label236');" onmouseover="ContentPreview('label237');" onmouseout="ContentUnpreview('label237');" title="click to collapse or expand..."> more... </a>
 <div id="label237" style="display:none">
 <table border="1">
 <tr>
 <td></td>
 <td colspan="1">Supported Version Ranges</td>
 </tr>
 <tr>
 <td>tod_window_end</td>
 <td><code class="docutils literal notranslate">v6.0.0 -> v6.2.7 </code></td>
 </tr>
 </table>
 </div>
 </li>
            <li> <span class="li-head">tod_window_start</span> - Time of day window start. <span class="li-normal">type: str</span>
 <a id='label238' href="javascript:ContentClick('label239', 'label238');" onmouseover="ContentPreview('label239');" onmouseout="ContentUnpreview('label239');" title="click to collapse or expand..."> more... </a>
 <div id="label239" style="display:none">
 <table border="1">
 <tr>
 <td></td>
 <td colspan="1">Supported Version Ranges</td>
 </tr>
 <tr>
 <td>tod_window_start</td>
 <td><code class="docutils literal notranslate">v6.0.0 -> v6.2.7 </code></td>
 </tr>
 </table>
 </div>
 </li>
            <li> <span class="li-head">user_domain</span> - Domain name to which the user addresses belong. <span class="li-normal">type: str</span>
 <a id='label240' href="javascript:ContentClick('label241', 'label240');" onmouseover="ContentPreview('label241');" onmouseout="ContentUnpreview('label241');" title="click to collapse or expand..."> more... </a>
 <div id="label241" style="display:none">
 <table border="1">
 <tr>
 <td></td>
 <td colspan="1">Supported Version Ranges</td>
 </tr>
 <tr>
 <td>user_domain</td>
 <td><code class="docutils literal notranslate">v6.0.0 -> v6.2.7 </code></td>
 </tr>
 </table>
 </div>
 </li>
            <li> <span class="li-head">vas_id</span> - VAS identifier. <span class="li-normal">type: str</span>
 <a id='label242' href="javascript:ContentClick('label243', 'label242');" onmouseover="ContentPreview('label243');" onmouseout="ContentUnpreview('label243');" title="click to collapse or expand..."> more... </a>
 <div id="label243" style="display:none">
 <table border="1">
 <tr>
 <td></td>
 <td colspan="1">Supported Version Ranges</td>
 </tr>
 <tr>
 <td>vas_id</td>
 <td><code class="docutils literal notranslate">v6.0.0 -> v6.2.7 </code></td>
 </tr>
 </table>
 </div>
 </li>
            <li> <span class="li-head">vasp_id</span> - VASP identifier. <span class="li-normal">type: str</span>
 <a id='label244' href="javascript:ContentClick('label245', 'label244');" onmouseover="ContentPreview('label245');" onmouseout="ContentUnpreview('label245');" title="click to collapse or expand..."> more... </a>
 <div id="label245" style="display:none">
 <table border="1">
 <tr>
 <td></td>
 <td colspan="1">Supported Version Ranges</td>
 </tr>
 <tr>
 <td>vasp_id</td>
 <td><code class="docutils literal notranslate">v6.0.0 -> v6.2.7 </code></td>
 </tr>
 </table>
 </div>
 </li>
            <li> <span class="li-head">virus_int</span> - Virus notification send interval. <span class="li-normal">type: int</span>
 <a id='label246' href="javascript:ContentClick('label247', 'label246');" onmouseover="ContentPreview('label247');" onmouseout="ContentUnpreview('label247');" title="click to collapse or expand..."> more... </a>
 <div id="label247" style="display:none">
 <table border="1">
 <tr>
 <td></td>
 <td colspan="1">Supported Version Ranges</td>
 </tr>
 <tr>
 <td>virus_int</td>
 <td><code class="docutils literal notranslate">v6.0.0 -> v6.2.7 </code></td>
 </tr>
 </table>
 </div>
 </li>
            <li> <span class="li-head">virus_int_mode</span> - Virus notification interval mode. <span class="li-normal">type: str</span> <span class="li-normal">choices: hours, minutes</span>
 <a id='label248' href="javascript:ContentClick('label249', 'label248');" onmouseover="ContentPreview('label249');" onmouseout="ContentUnpreview('label249');" title="click to collapse or expand..."> more... </a>
 <div id="label249" style="display:none">
 <table border="1">
 <tr>
 <td></td>
 <td colspan="1">Supported Version Ranges</td>
 </tr>
 <tr>
 <td>virus_int_mode</td>
 <td><code class="docutils literal notranslate">v6.0.0 -> v6.2.7 </code></td>
 </tr>
 <tr>
 <td>[hours]</td>
 <td><code class="docutils literal notranslate">v6.0.0 -> latest</code></td> <tr>
 <td>[minutes]</td>
 <td><code class="docutils literal notranslate">v6.0.0 -> latest</code></td> </table>
 </div>
 </li>
            <li> <span class="li-head">virus_status</span> - Virus notification status. <span class="li-normal">type: str</span> <span class="li-normal">choices: enable, disable</span>
 <a id='label250' href="javascript:ContentClick('label251', 'label250');" onmouseover="ContentPreview('label251');" onmouseout="ContentUnpreview('label251');" title="click to collapse or expand..."> more... </a>
 <div id="label251" style="display:none">
 <table border="1">
 <tr>
 <td></td>
 <td colspan="1">Supported Version Ranges</td>
 </tr>
 <tr>
 <td>virus_status</td>
 <td><code class="docutils literal notranslate">v6.0.0 -> v6.2.7 </code></td>
 </tr>
 <tr>
 <td>[enable]</td>
 <td><code class="docutils literal notranslate">v6.0.0 -> latest</code></td> <tr>
 <td>[disable]</td>
 <td><code class="docutils literal notranslate">v6.0.0 -> latest</code></td> </table>
 </div>
 </li>
            </ul>
        <li> <span class="li-head">outbreak_prevention</span> - Configure Virus Outbreak Prevention settings. <span class="li-normal">type: dict</span>
 <a id='label252' href="javascript:ContentClick('label253', 'label252');" onmouseover="ContentPreview('label253');" onmouseout="ContentUnpreview('label253');" title="click to collapse or expand..."> more... </a>
 <div id="label253" style="display:none">
 <table border="1">
 <tr>
 <td></td><td colspan="1">Supported Version Ranges</td>
 </tr>
 <tr>
 <td>outbreak_prevention</td>
 <td><code class="docutils literal notranslate">v6.2.0 -> v6.2.7 </code></td>
 </tr>
 </table>
 </div>
 </li>
            <ul class="ul-self">
            <li> <span class="li-head">external_blocklist</span> - Enable/disable external malware blocklist. <span class="li-normal">type: str</span> <span class="li-normal">choices: disable, enable</span>
 <a id='label254' href="javascript:ContentClick('label255', 'label254');" onmouseover="ContentPreview('label255');" onmouseout="ContentUnpreview('label255');" title="click to collapse or expand..."> more... </a>
 <div id="label255" style="display:none">
 <table border="1">
 <tr>
 <td></td>
 <td colspan="1">Supported Version Ranges</td>
 </tr>
 <tr>
 <td>external_blocklist</td>
 <td><code class="docutils literal notranslate">v6.2.0 -> v6.2.7 </code></td>
 </tr>
 <tr>
 <td>[disable]</td>
 <td><code class="docutils literal notranslate">v6.0.0 -> latest</code></td> <tr>
 <td>[enable]</td>
 <td><code class="docutils literal notranslate">v6.0.0 -> latest</code></td> </table>
 </div>
 </li>
            <li> <span class="li-head">ftgd_service</span> - Enable/disable FortiGuard Virus outbreak prevention service. <span class="li-normal">type: str</span> <span class="li-normal">choices: disable, enable</span>
 <a id='label256' href="javascript:ContentClick('label257', 'label256');" onmouseover="ContentPreview('label257');" onmouseout="ContentUnpreview('label257');" title="click to collapse or expand..."> more... </a>
 <div id="label257" style="display:none">
 <table border="1">
 <tr>
 <td></td>
 <td colspan="1">Supported Version Ranges</td>
 </tr>
 <tr>
 <td>ftgd_service</td>
 <td><code class="docutils literal notranslate">v6.2.0 -> v6.2.7 </code></td>
 </tr>
 <tr>
 <td>[disable]</td>
 <td><code class="docutils literal notranslate">v6.0.0 -> latest</code></td> <tr>
 <td>[enable]</td>
 <td><code class="docutils literal notranslate">v6.0.0 -> latest</code></td> </table>
 </div>
 </li>
            </ul>
        <li> <span class="li-head">remove_blocked_const_length</span> - Enable/disable MMS replacement of blocked file constant length. <span class="li-normal">type: str</span> <span class="li-normal">choices: enable, disable</span>
 <a id='label258' href="javascript:ContentClick('label259', 'label258');" onmouseover="ContentPreview('label259');" onmouseout="ContentUnpreview('label259');" title="click to collapse or expand..."> more... </a>
 <div id="label259" style="display:none">
 <table border="1">
 <tr>
 <td></td>
 <td colspan="1">Supported Version Ranges</td>
 </tr>
 <tr>
 <td>remove_blocked_const_length</td>
 <td><code class="docutils literal notranslate">v6.0.0 -> v6.2.7 </code></td>
 </tr>
 <tr>
 <td>[enable]</td>
 <td><code class="docutils literal notranslate">v6.0.0 -> latest</code></td> <tr>
 <td>[disable]</td>
 <td><code class="docutils literal notranslate">v6.0.0 -> latest</code></td> </table>
 </div>
 </li>
        <li> <span class="li-head">replacemsg_group</span> - Replacement message group. Source system.replacemsg-group.name. <span class="li-normal">type: str</span>
 <a id='label260' href="javascript:ContentClick('label261', 'label260');" onmouseover="ContentPreview('label261');" onmouseout="ContentUnpreview('label261');" title="click to collapse or expand..."> more... </a>
 <div id="label261" style="display:none">
 <table border="1">
 <tr>
 <td></td>
 <td colspan="1">Supported Version Ranges</td>
 </tr>
 <tr>
 <td>replacemsg_group</td>
 <td><code class="docutils literal notranslate">v6.0.0 -> v6.2.7 </code></td>
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
    
    - name: Configure MMS profiles.
      fortinet.fortios.fortios_firewall_mms_profile:
          vdom: "{{ vdom }}"
          state: "present"
          access_token: "<your_own_value>"
          firewall_mms_profile:
              avnotificationtable: "2147483647"
              bwordtable: "2147483647"
              carrier_endpoint_prefix: "enable"
              carrier_endpoint_prefix_range_max: "24"
              carrier_endpoint_prefix_range_min: "24"
              carrier_endpoint_prefix_string: "<your_own_value>"
              carrierendpointbwltable: "2147483647"
              comment: "Comment."
              dupe:
                  -
                      action1: "block"
                      action2: "block"
                      action3: "block"
                      block_time1: "17895"
                      block_time2: "17895"
                      block_time3: "17895"
                      limit1: "1073741823"
                      limit2: "1073741823"
                      limit3: "1073741823"
                      protocol: "<your_own_value>"
                      status1: "enable"
                      status2: "enable"
                      status3: "enable"
                      window1: "1440"
                      window2: "1440"
                      window3: "1440"
              extended_utm_log: "<your_own_value>"
              flood:
                  -
                      action1: "block"
                      action2: "block"
                      action3: "block"
                      block_time1: "17895"
                      block_time2: "17895"
                      block_time3: "17895"
                      limit1: "1073741823"
                      limit2: "1073741823"
                      limit3: "1073741823"
                      protocol: "<your_own_value>"
                      status1: "enable"
                      status2: "enable"
                      status3: "enable"
                      window1: "1440"
                      window2: "1440"
                      window3: "1440"
              mm1: "avmonitor"
              mm1_addr_hdr: "<your_own_value>"
              mm1_addr_source: "http-header"
              mm1_convert_hex: "enable"
              mm1_outbreak_prevention: "disabled"
              mm1_retr_dupe: "enable"
              mm1_retrieve_scan: "enable"
              mm1comfortamount: "2147483647"
              mm1comfortinterval: "2147483647"
              mm1oversizelimit: "409600"
              mm3: "avmonitor"
              mm3_outbreak_prevention: "disabled"
              mm3oversizelimit: "409600"
              mm4: "avmonitor"
              mm4_outbreak_prevention: "disabled"
              mm4oversizelimit: "409600"
              mm7: "avmonitor"
              mm7_addr_hdr: "<your_own_value>"
              mm7_addr_source: "http-header"
              mm7_convert_hex: "enable"
              mm7_outbreak_prevention: "disabled"
              mm7comfortamount: "2147483647"
              mm7comfortinterval: "2147483647"
              mm7oversizelimit: "409600"
              mms_antispam_mass_log: "enable"
              mms_av_block_log: "enable"
              mms_av_oversize_log: "enable"
              mms_av_virus_log: "enable"
              mms_carrier_endpoint_filter_log: "enable"
              mms_checksum_log: "enable"
              mms_checksum_table: "2147483647"
              mms_notification_log: "enable"
              mms_web_content_log: "enable"
              mmsbwordthreshold: "1073741823"
              name: "default_name_80"
              notif_msisdn:
                  -
                      msisdn: "<your_own_value>"
                      threshold: "flood-thresh-1"
              notification:
                  -
                      alert_int: "720"
                      alert_int_mode: "hours"
                      alert_src_msisdn: "<your_own_value>"
                      alert_status: "enable"
                      bword_int: "720"
                      bword_int_mode: "hours"
                      bword_status: "enable"
                      carrier_endpoint_bwl_int: "720"
                      carrier_endpoint_bwl_int_mode: "hours"
                      carrier_endpoint_bwl_status: "enable"
                      days_allowed: "sunday"
                      detect_server: "enable"
                      dupe_int: "720"
                      dupe_int_mode: "hours"
                      dupe_status: "enable"
                      file_block_int: "720"
                      file_block_int_mode: "hours"
                      file_block_status: "enable"
                      flood_int: "720"
                      flood_int_mode: "hours"
                      flood_status: "enable"
                      from_in_header: "enable"
                      mms_checksum_int: "720"
                      mms_checksum_int_mode: "hours"
                      mms_checksum_status: "enable"
                      mmsc_hostname: "myhostname"
                      mmsc_password: "<your_own_value>"
                      mmsc_port: "32767"
                      mmsc_url: "<your_own_value>"
                      mmsc_username: "<your_own_value>"
                      msg_protocol: "mm1"
                      msg_type: "submit-req"
                      protocol: "<your_own_value>"
                      rate_limit: "125"
                      tod_window_duration: "<your_own_value>"
                      tod_window_end: "<your_own_value>"
                      tod_window_start: "<your_own_value>"
                      user_domain: "<your_own_value>"
                      vas_id: "<your_own_value>"
                      vasp_id: "<your_own_value>"
                      virus_int: "720"
                      virus_int_mode: "hours"
                      virus_status: "enable"
              outbreak_prevention:
                  external_blocklist: "disable"
                  ftgd_service: "disable"
              remove_blocked_const_length: "enable"
              replacemsg_group: "<your_own_value> (source system.replacemsg-group.name)"


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
