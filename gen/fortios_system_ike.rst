:source: fortios_system_ike.py

:orphan:

.. fortios_system_ike:

fortios_system_ike -- Configure IKE global attributes in Fortinet's FortiOS and FortiGate.
++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++

.. versionadded:: 2.10

.. contents::
   :local:
   :depth: 1


Synopsis
--------
- This module is able to configure a FortiGate or FortiOS (FOS) device by allowing the user to set and modify system feature and ike category. Examples include all parameters and values need to be adjusted to datasources before usage. Tested with FOS v6.0.0



Requirements
------------
The below requirements are needed on the host that executes this module.

- ansible>=2.9.0


FortiOS Version Compatibility
-----------------------------


.. raw:: html

 <br>
 <table>
 <tr>
 <td></td>
 <td><code class="docutils literal notranslate">v7.0.0 </code></td>
 </tr>
 <tr>
 <td>fortios_system_ike</td>
 <td>yes</td>
 </tr>
 </table>
 <p>



Parameters
----------


.. raw:: html

    <ul>
    <li> <span class="li-head">access_token</span> - Token-based authentication. Generated from GUI of Fortigate. <span class="li-normal">type: str</span> <span class="li-required">required: False</span> </li>
    <li> <span class="li-head">enable_log</span> - Enable/Disable logging for task. <span class="li-normal">type: bool</span> <span class="li-required">required: False</span> <span class="li-normal">default: False</span> </li>
    <li> <span class="li-head">vdom</span> - Virtual domain, among those defined previously. A vdom is a virtual instance of the FortiGate that can be configured and used as a different unit. <span class="li-normal">type: str</span> <span class="li-normal">default: root</span> </li>
    <li> <span class="li-head">system_ike</span> - Configure IKE global attributes. <span class="li-normal">type: dict</span>
 <a id='label0' href="javascript:ContentClick('label1', 'label0');" onmouseover="ContentPreview('label1');" onmouseout="ContentUnpreview('label1');" title="click to collapse or expand..."> more... </a>
 <div id="label1" style="display:none">
 <table border="1">
 <tr>
 <td></td>
 <td><code class="docutils literal notranslate">v7.0.0 </code></td>
 </tr>
 <tr>
 <td>system_ike</td>
 <td>yes</td>
 </tr>
 </table>
 </div>
 </li>
        <ul class="ul-self">
        <li> <span class="li-head">dh_group_1</span> - Diffie-Hellman group 1 (MODP-768). <span class="li-normal">type: dict</span>
 <a id='label2' href="javascript:ContentClick('label3', 'label2');" onmouseover="ContentPreview('label3');" onmouseout="ContentUnpreview('label3');" title="click to collapse or expand..."> more... </a>
 <div id="label3" style="display:none">
 <table border="1">
 <tr>
 <td></td>
 <td><code class="docutils literal notranslate">v7.0.0 </code></td>
 </tr>
 <tr>
 <td>dh_group_1</td>
 <td>yes</td>
 </tr>
 </table>
 </div>
 </li>
            <ul class="ul-self">
            <li> <span class="li-head">keypair_cache</span> - Configure custom key pair cache size for this Diffie-Hellman group. <span class="li-normal">type: str</span> <span class="li-normal">choices: global, custom</span>
 <a id='label4' href="javascript:ContentClick('label5', 'label4');" onmouseover="ContentPreview('label5');" onmouseout="ContentUnpreview('label5');" title="click to collapse or expand..."> more... </a>
 <div id="label5" style="display:none">
 <table border="1">
 <tr>
 <td></td>
 <td><code class="docutils literal notranslate">v7.0.0 </code></td>
 </tr>
 <tr>
 <td>keypair_cache</td>
 <td>yes</td>
 </tr>
 <tr>
 <td>[global]</td>
 <td>yes</td>
 </tr>
 <tr>
 <td>[custom]</td>
 <td>yes</td>
 </tr>
 </table>
 </div>
 </li>
            <li> <span class="li-head">keypair_count</span> - Number of key pairs to pre-generate for this Diffie-Hellman group (per-worker). <span class="li-normal">type: int</span>
 <a id='label6' href="javascript:ContentClick('label7', 'label6');" onmouseover="ContentPreview('label7');" onmouseout="ContentUnpreview('label7');" title="click to collapse or expand..."> more... </a>
 <div id="label7" style="display:none">
 <table border="1">
 <tr>
 <td></td>
 <td><code class="docutils literal notranslate">v7.0.0 </code></td>
 </tr>
 <tr>
 <td>keypair_count</td>
 <td>yes</td>
 </tr>
 </table>
 </div>
 </li>
            <li> <span class="li-head">mode</span> - Use software (CPU) or hardware (CPX) to perform calculations for this Diffie-Hellman group. <span class="li-normal">type: str</span> <span class="li-normal">choices: software, hardware, global</span>
 <a id='label8' href="javascript:ContentClick('label9', 'label8');" onmouseover="ContentPreview('label9');" onmouseout="ContentUnpreview('label9');" title="click to collapse or expand..."> more... </a>
 <div id="label9" style="display:none">
 <table border="1">
 <tr>
 <td></td>
 <td><code class="docutils literal notranslate">v7.0.0 </code></td>
 </tr>
 <tr>
 <td>mode</td>
 <td>yes</td>
 </tr>
 <tr>
 <td>[software]</td>
 <td>yes</td>
 </tr>
 <tr>
 <td>[hardware]</td>
 <td>yes</td>
 </tr>
 <tr>
 <td>[global]</td>
 <td>yes</td>
 </tr>
 </table>
 </div>
 </li>
            </ul>
        <li> <span class="li-head">dh_group_14</span> - Diffie-Hellman group 14 (MODP-2048). <span class="li-normal">type: dict</span>
 <a id='label10' href="javascript:ContentClick('label11', 'label10');" onmouseover="ContentPreview('label11');" onmouseout="ContentUnpreview('label11');" title="click to collapse or expand..."> more... </a>
 <div id="label11" style="display:none">
 <table border="1">
 <tr>
 <td></td>
 <td><code class="docutils literal notranslate">v7.0.0 </code></td>
 </tr>
 <tr>
 <td>dh_group_14</td>
 <td>yes</td>
 </tr>
 </table>
 </div>
 </li>
            <ul class="ul-self">
            <li> <span class="li-head">keypair_cache</span> - Configure custom key pair cache size for this Diffie-Hellman group. <span class="li-normal">type: str</span> <span class="li-normal">choices: global, custom</span>
 <a id='label12' href="javascript:ContentClick('label13', 'label12');" onmouseover="ContentPreview('label13');" onmouseout="ContentUnpreview('label13');" title="click to collapse or expand..."> more... </a>
 <div id="label13" style="display:none">
 <table border="1">
 <tr>
 <td></td>
 <td><code class="docutils literal notranslate">v7.0.0 </code></td>
 </tr>
 <tr>
 <td>keypair_cache</td>
 <td>yes</td>
 </tr>
 <tr>
 <td>[global]</td>
 <td>yes</td>
 </tr>
 <tr>
 <td>[custom]</td>
 <td>yes</td>
 </tr>
 </table>
 </div>
 </li>
            <li> <span class="li-head">keypair_count</span> - Number of key pairs to pre-generate for this Diffie-Hellman group (per-worker). <span class="li-normal">type: int</span>
 <a id='label14' href="javascript:ContentClick('label15', 'label14');" onmouseover="ContentPreview('label15');" onmouseout="ContentUnpreview('label15');" title="click to collapse or expand..."> more... </a>
 <div id="label15" style="display:none">
 <table border="1">
 <tr>
 <td></td>
 <td><code class="docutils literal notranslate">v7.0.0 </code></td>
 </tr>
 <tr>
 <td>keypair_count</td>
 <td>yes</td>
 </tr>
 </table>
 </div>
 </li>
            <li> <span class="li-head">mode</span> - Use software (CPU) or hardware (CPX) to perform calculations for this Diffie-Hellman group. <span class="li-normal">type: str</span> <span class="li-normal">choices: software, hardware, global</span>
 <a id='label16' href="javascript:ContentClick('label17', 'label16');" onmouseover="ContentPreview('label17');" onmouseout="ContentUnpreview('label17');" title="click to collapse or expand..."> more... </a>
 <div id="label17" style="display:none">
 <table border="1">
 <tr>
 <td></td>
 <td><code class="docutils literal notranslate">v7.0.0 </code></td>
 </tr>
 <tr>
 <td>mode</td>
 <td>yes</td>
 </tr>
 <tr>
 <td>[software]</td>
 <td>yes</td>
 </tr>
 <tr>
 <td>[hardware]</td>
 <td>yes</td>
 </tr>
 <tr>
 <td>[global]</td>
 <td>yes</td>
 </tr>
 </table>
 </div>
 </li>
            </ul>
        <li> <span class="li-head">dh_group_15</span> - Diffie-Hellman group 15 (MODP-3072). <span class="li-normal">type: dict</span>
 <a id='label18' href="javascript:ContentClick('label19', 'label18');" onmouseover="ContentPreview('label19');" onmouseout="ContentUnpreview('label19');" title="click to collapse or expand..."> more... </a>
 <div id="label19" style="display:none">
 <table border="1">
 <tr>
 <td></td>
 <td><code class="docutils literal notranslate">v7.0.0 </code></td>
 </tr>
 <tr>
 <td>dh_group_15</td>
 <td>yes</td>
 </tr>
 </table>
 </div>
 </li>
            <ul class="ul-self">
            <li> <span class="li-head">keypair_cache</span> - Configure custom key pair cache size for this Diffie-Hellman group. <span class="li-normal">type: str</span> <span class="li-normal">choices: global, custom</span>
 <a id='label20' href="javascript:ContentClick('label21', 'label20');" onmouseover="ContentPreview('label21');" onmouseout="ContentUnpreview('label21');" title="click to collapse or expand..."> more... </a>
 <div id="label21" style="display:none">
 <table border="1">
 <tr>
 <td></td>
 <td><code class="docutils literal notranslate">v7.0.0 </code></td>
 </tr>
 <tr>
 <td>keypair_cache</td>
 <td>yes</td>
 </tr>
 <tr>
 <td>[global]</td>
 <td>yes</td>
 </tr>
 <tr>
 <td>[custom]</td>
 <td>yes</td>
 </tr>
 </table>
 </div>
 </li>
            <li> <span class="li-head">keypair_count</span> - Number of key pairs to pre-generate for this Diffie-Hellman group (per-worker). <span class="li-normal">type: int</span>
 <a id='label22' href="javascript:ContentClick('label23', 'label22');" onmouseover="ContentPreview('label23');" onmouseout="ContentUnpreview('label23');" title="click to collapse or expand..."> more... </a>
 <div id="label23" style="display:none">
 <table border="1">
 <tr>
 <td></td>
 <td><code class="docutils literal notranslate">v7.0.0 </code></td>
 </tr>
 <tr>
 <td>keypair_count</td>
 <td>yes</td>
 </tr>
 </table>
 </div>
 </li>
            <li> <span class="li-head">mode</span> - Use software (CPU) or hardware (CPX) to perform calculations for this Diffie-Hellman group. <span class="li-normal">type: str</span> <span class="li-normal">choices: software, hardware, global</span>
 <a id='label24' href="javascript:ContentClick('label25', 'label24');" onmouseover="ContentPreview('label25');" onmouseout="ContentUnpreview('label25');" title="click to collapse or expand..."> more... </a>
 <div id="label25" style="display:none">
 <table border="1">
 <tr>
 <td></td>
 <td><code class="docutils literal notranslate">v7.0.0 </code></td>
 </tr>
 <tr>
 <td>mode</td>
 <td>yes</td>
 </tr>
 <tr>
 <td>[software]</td>
 <td>yes</td>
 </tr>
 <tr>
 <td>[hardware]</td>
 <td>yes</td>
 </tr>
 <tr>
 <td>[global]</td>
 <td>yes</td>
 </tr>
 </table>
 </div>
 </li>
            </ul>
        <li> <span class="li-head">dh_group_16</span> - Diffie-Hellman group 16 (MODP-4096). <span class="li-normal">type: dict</span>
 <a id='label26' href="javascript:ContentClick('label27', 'label26');" onmouseover="ContentPreview('label27');" onmouseout="ContentUnpreview('label27');" title="click to collapse or expand..."> more... </a>
 <div id="label27" style="display:none">
 <table border="1">
 <tr>
 <td></td>
 <td><code class="docutils literal notranslate">v7.0.0 </code></td>
 </tr>
 <tr>
 <td>dh_group_16</td>
 <td>yes</td>
 </tr>
 </table>
 </div>
 </li>
            <ul class="ul-self">
            <li> <span class="li-head">keypair_cache</span> - Configure custom key pair cache size for this Diffie-Hellman group. <span class="li-normal">type: str</span> <span class="li-normal">choices: global, custom</span>
 <a id='label28' href="javascript:ContentClick('label29', 'label28');" onmouseover="ContentPreview('label29');" onmouseout="ContentUnpreview('label29');" title="click to collapse or expand..."> more... </a>
 <div id="label29" style="display:none">
 <table border="1">
 <tr>
 <td></td>
 <td><code class="docutils literal notranslate">v7.0.0 </code></td>
 </tr>
 <tr>
 <td>keypair_cache</td>
 <td>yes</td>
 </tr>
 <tr>
 <td>[global]</td>
 <td>yes</td>
 </tr>
 <tr>
 <td>[custom]</td>
 <td>yes</td>
 </tr>
 </table>
 </div>
 </li>
            <li> <span class="li-head">keypair_count</span> - Number of key pairs to pre-generate for this Diffie-Hellman group (per-worker). <span class="li-normal">type: int</span>
 <a id='label30' href="javascript:ContentClick('label31', 'label30');" onmouseover="ContentPreview('label31');" onmouseout="ContentUnpreview('label31');" title="click to collapse or expand..."> more... </a>
 <div id="label31" style="display:none">
 <table border="1">
 <tr>
 <td></td>
 <td><code class="docutils literal notranslate">v7.0.0 </code></td>
 </tr>
 <tr>
 <td>keypair_count</td>
 <td>yes</td>
 </tr>
 </table>
 </div>
 </li>
            <li> <span class="li-head">mode</span> - Use software (CPU) or hardware (CPX) to perform calculations for this Diffie-Hellman group. <span class="li-normal">type: str</span> <span class="li-normal">choices: software, hardware, global</span>
 <a id='label32' href="javascript:ContentClick('label33', 'label32');" onmouseover="ContentPreview('label33');" onmouseout="ContentUnpreview('label33');" title="click to collapse or expand..."> more... </a>
 <div id="label33" style="display:none">
 <table border="1">
 <tr>
 <td></td>
 <td><code class="docutils literal notranslate">v7.0.0 </code></td>
 </tr>
 <tr>
 <td>mode</td>
 <td>yes</td>
 </tr>
 <tr>
 <td>[software]</td>
 <td>yes</td>
 </tr>
 <tr>
 <td>[hardware]</td>
 <td>yes</td>
 </tr>
 <tr>
 <td>[global]</td>
 <td>yes</td>
 </tr>
 </table>
 </div>
 </li>
            </ul>
        <li> <span class="li-head">dh_group_17</span> - Diffie-Hellman group 17 (MODP-6144). <span class="li-normal">type: dict</span>
 <a id='label34' href="javascript:ContentClick('label35', 'label34');" onmouseover="ContentPreview('label35');" onmouseout="ContentUnpreview('label35');" title="click to collapse or expand..."> more... </a>
 <div id="label35" style="display:none">
 <table border="1">
 <tr>
 <td></td>
 <td><code class="docutils literal notranslate">v7.0.0 </code></td>
 </tr>
 <tr>
 <td>dh_group_17</td>
 <td>yes</td>
 </tr>
 </table>
 </div>
 </li>
            <ul class="ul-self">
            <li> <span class="li-head">keypair_cache</span> - Configure custom key pair cache size for this Diffie-Hellman group. <span class="li-normal">type: str</span> <span class="li-normal">choices: global, custom</span>
 <a id='label36' href="javascript:ContentClick('label37', 'label36');" onmouseover="ContentPreview('label37');" onmouseout="ContentUnpreview('label37');" title="click to collapse or expand..."> more... </a>
 <div id="label37" style="display:none">
 <table border="1">
 <tr>
 <td></td>
 <td><code class="docutils literal notranslate">v7.0.0 </code></td>
 </tr>
 <tr>
 <td>keypair_cache</td>
 <td>yes</td>
 </tr>
 <tr>
 <td>[global]</td>
 <td>yes</td>
 </tr>
 <tr>
 <td>[custom]</td>
 <td>yes</td>
 </tr>
 </table>
 </div>
 </li>
            <li> <span class="li-head">keypair_count</span> - Number of key pairs to pre-generate for this Diffie-Hellman group (per-worker). <span class="li-normal">type: int</span>
 <a id='label38' href="javascript:ContentClick('label39', 'label38');" onmouseover="ContentPreview('label39');" onmouseout="ContentUnpreview('label39');" title="click to collapse or expand..."> more... </a>
 <div id="label39" style="display:none">
 <table border="1">
 <tr>
 <td></td>
 <td><code class="docutils literal notranslate">v7.0.0 </code></td>
 </tr>
 <tr>
 <td>keypair_count</td>
 <td>yes</td>
 </tr>
 </table>
 </div>
 </li>
            <li> <span class="li-head">mode</span> - Use software (CPU) or hardware (CPX) to perform calculations for this Diffie-Hellman group. <span class="li-normal">type: str</span> <span class="li-normal">choices: software, hardware, global</span>
 <a id='label40' href="javascript:ContentClick('label41', 'label40');" onmouseover="ContentPreview('label41');" onmouseout="ContentUnpreview('label41');" title="click to collapse or expand..."> more... </a>
 <div id="label41" style="display:none">
 <table border="1">
 <tr>
 <td></td>
 <td><code class="docutils literal notranslate">v7.0.0 </code></td>
 </tr>
 <tr>
 <td>mode</td>
 <td>yes</td>
 </tr>
 <tr>
 <td>[software]</td>
 <td>yes</td>
 </tr>
 <tr>
 <td>[hardware]</td>
 <td>yes</td>
 </tr>
 <tr>
 <td>[global]</td>
 <td>yes</td>
 </tr>
 </table>
 </div>
 </li>
            </ul>
        <li> <span class="li-head">dh_group_18</span> - Diffie-Hellman group 18 (MODP-8192). <span class="li-normal">type: dict</span>
 <a id='label42' href="javascript:ContentClick('label43', 'label42');" onmouseover="ContentPreview('label43');" onmouseout="ContentUnpreview('label43');" title="click to collapse or expand..."> more... </a>
 <div id="label43" style="display:none">
 <table border="1">
 <tr>
 <td></td>
 <td><code class="docutils literal notranslate">v7.0.0 </code></td>
 </tr>
 <tr>
 <td>dh_group_18</td>
 <td>yes</td>
 </tr>
 </table>
 </div>
 </li>
            <ul class="ul-self">
            <li> <span class="li-head">keypair_cache</span> - Configure custom key pair cache size for this Diffie-Hellman group. <span class="li-normal">type: str</span> <span class="li-normal">choices: global, custom</span>
 <a id='label44' href="javascript:ContentClick('label45', 'label44');" onmouseover="ContentPreview('label45');" onmouseout="ContentUnpreview('label45');" title="click to collapse or expand..."> more... </a>
 <div id="label45" style="display:none">
 <table border="1">
 <tr>
 <td></td>
 <td><code class="docutils literal notranslate">v7.0.0 </code></td>
 </tr>
 <tr>
 <td>keypair_cache</td>
 <td>yes</td>
 </tr>
 <tr>
 <td>[global]</td>
 <td>yes</td>
 </tr>
 <tr>
 <td>[custom]</td>
 <td>yes</td>
 </tr>
 </table>
 </div>
 </li>
            <li> <span class="li-head">keypair_count</span> - Number of key pairs to pre-generate for this Diffie-Hellman group (per-worker). <span class="li-normal">type: int</span>
 <a id='label46' href="javascript:ContentClick('label47', 'label46');" onmouseover="ContentPreview('label47');" onmouseout="ContentUnpreview('label47');" title="click to collapse or expand..."> more... </a>
 <div id="label47" style="display:none">
 <table border="1">
 <tr>
 <td></td>
 <td><code class="docutils literal notranslate">v7.0.0 </code></td>
 </tr>
 <tr>
 <td>keypair_count</td>
 <td>yes</td>
 </tr>
 </table>
 </div>
 </li>
            <li> <span class="li-head">mode</span> - Use software (CPU) or hardware (CPX) to perform calculations for this Diffie-Hellman group. <span class="li-normal">type: str</span> <span class="li-normal">choices: software, hardware, global</span>
 <a id='label48' href="javascript:ContentClick('label49', 'label48');" onmouseover="ContentPreview('label49');" onmouseout="ContentUnpreview('label49');" title="click to collapse or expand..."> more... </a>
 <div id="label49" style="display:none">
 <table border="1">
 <tr>
 <td></td>
 <td><code class="docutils literal notranslate">v7.0.0 </code></td>
 </tr>
 <tr>
 <td>mode</td>
 <td>yes</td>
 </tr>
 <tr>
 <td>[software]</td>
 <td>yes</td>
 </tr>
 <tr>
 <td>[hardware]</td>
 <td>yes</td>
 </tr>
 <tr>
 <td>[global]</td>
 <td>yes</td>
 </tr>
 </table>
 </div>
 </li>
            </ul>
        <li> <span class="li-head">dh_group_19</span> - Diffie-Hellman group 19 (EC-P256). <span class="li-normal">type: dict</span>
 <a id='label50' href="javascript:ContentClick('label51', 'label50');" onmouseover="ContentPreview('label51');" onmouseout="ContentUnpreview('label51');" title="click to collapse or expand..."> more... </a>
 <div id="label51" style="display:none">
 <table border="1">
 <tr>
 <td></td>
 <td><code class="docutils literal notranslate">v7.0.0 </code></td>
 </tr>
 <tr>
 <td>dh_group_19</td>
 <td>yes</td>
 </tr>
 </table>
 </div>
 </li>
            <ul class="ul-self">
            <li> <span class="li-head">keypair_cache</span> - Configure custom key pair cache size for this Diffie-Hellman group. <span class="li-normal">type: str</span> <span class="li-normal">choices: global, custom</span>
 <a id='label52' href="javascript:ContentClick('label53', 'label52');" onmouseover="ContentPreview('label53');" onmouseout="ContentUnpreview('label53');" title="click to collapse or expand..."> more... </a>
 <div id="label53" style="display:none">
 <table border="1">
 <tr>
 <td></td>
 <td><code class="docutils literal notranslate">v7.0.0 </code></td>
 </tr>
 <tr>
 <td>keypair_cache</td>
 <td>yes</td>
 </tr>
 <tr>
 <td>[global]</td>
 <td>yes</td>
 </tr>
 <tr>
 <td>[custom]</td>
 <td>yes</td>
 </tr>
 </table>
 </div>
 </li>
            <li> <span class="li-head">keypair_count</span> - Number of key pairs to pre-generate for this Diffie-Hellman group (per-worker). <span class="li-normal">type: int</span>
 <a id='label54' href="javascript:ContentClick('label55', 'label54');" onmouseover="ContentPreview('label55');" onmouseout="ContentUnpreview('label55');" title="click to collapse or expand..."> more... </a>
 <div id="label55" style="display:none">
 <table border="1">
 <tr>
 <td></td>
 <td><code class="docutils literal notranslate">v7.0.0 </code></td>
 </tr>
 <tr>
 <td>keypair_count</td>
 <td>yes</td>
 </tr>
 </table>
 </div>
 </li>
            <li> <span class="li-head">mode</span> - Use software (CPU) or hardware (CPX) to perform calculations for this Diffie-Hellman group. <span class="li-normal">type: str</span> <span class="li-normal">choices: software, hardware, global</span>
 <a id='label56' href="javascript:ContentClick('label57', 'label56');" onmouseover="ContentPreview('label57');" onmouseout="ContentUnpreview('label57');" title="click to collapse or expand..."> more... </a>
 <div id="label57" style="display:none">
 <table border="1">
 <tr>
 <td></td>
 <td><code class="docutils literal notranslate">v7.0.0 </code></td>
 </tr>
 <tr>
 <td>mode</td>
 <td>yes</td>
 </tr>
 <tr>
 <td>[software]</td>
 <td>yes</td>
 </tr>
 <tr>
 <td>[hardware]</td>
 <td>yes</td>
 </tr>
 <tr>
 <td>[global]</td>
 <td>yes</td>
 </tr>
 </table>
 </div>
 </li>
            </ul>
        <li> <span class="li-head">dh_group_2</span> - Diffie-Hellman group 2 (MODP-1024). <span class="li-normal">type: dict</span>
 <a id='label58' href="javascript:ContentClick('label59', 'label58');" onmouseover="ContentPreview('label59');" onmouseout="ContentUnpreview('label59');" title="click to collapse or expand..."> more... </a>
 <div id="label59" style="display:none">
 <table border="1">
 <tr>
 <td></td>
 <td><code class="docutils literal notranslate">v7.0.0 </code></td>
 </tr>
 <tr>
 <td>dh_group_2</td>
 <td>yes</td>
 </tr>
 </table>
 </div>
 </li>
            <ul class="ul-self">
            <li> <span class="li-head">keypair_cache</span> - Configure custom key pair cache size for this Diffie-Hellman group. <span class="li-normal">type: str</span> <span class="li-normal">choices: global, custom</span>
 <a id='label60' href="javascript:ContentClick('label61', 'label60');" onmouseover="ContentPreview('label61');" onmouseout="ContentUnpreview('label61');" title="click to collapse or expand..."> more... </a>
 <div id="label61" style="display:none">
 <table border="1">
 <tr>
 <td></td>
 <td><code class="docutils literal notranslate">v7.0.0 </code></td>
 </tr>
 <tr>
 <td>keypair_cache</td>
 <td>yes</td>
 </tr>
 <tr>
 <td>[global]</td>
 <td>yes</td>
 </tr>
 <tr>
 <td>[custom]</td>
 <td>yes</td>
 </tr>
 </table>
 </div>
 </li>
            <li> <span class="li-head">keypair_count</span> - Number of key pairs to pre-generate for this Diffie-Hellman group (per-worker). <span class="li-normal">type: int</span>
 <a id='label62' href="javascript:ContentClick('label63', 'label62');" onmouseover="ContentPreview('label63');" onmouseout="ContentUnpreview('label63');" title="click to collapse or expand..."> more... </a>
 <div id="label63" style="display:none">
 <table border="1">
 <tr>
 <td></td>
 <td><code class="docutils literal notranslate">v7.0.0 </code></td>
 </tr>
 <tr>
 <td>keypair_count</td>
 <td>yes</td>
 </tr>
 </table>
 </div>
 </li>
            <li> <span class="li-head">mode</span> - Use software (CPU) or hardware (CPX) to perform calculations for this Diffie-Hellman group. <span class="li-normal">type: str</span> <span class="li-normal">choices: software, hardware, global</span>
 <a id='label64' href="javascript:ContentClick('label65', 'label64');" onmouseover="ContentPreview('label65');" onmouseout="ContentUnpreview('label65');" title="click to collapse or expand..."> more... </a>
 <div id="label65" style="display:none">
 <table border="1">
 <tr>
 <td></td>
 <td><code class="docutils literal notranslate">v7.0.0 </code></td>
 </tr>
 <tr>
 <td>mode</td>
 <td>yes</td>
 </tr>
 <tr>
 <td>[software]</td>
 <td>yes</td>
 </tr>
 <tr>
 <td>[hardware]</td>
 <td>yes</td>
 </tr>
 <tr>
 <td>[global]</td>
 <td>yes</td>
 </tr>
 </table>
 </div>
 </li>
            </ul>
        <li> <span class="li-head">dh_group_20</span> - Diffie-Hellman group 20 (EC-P384). <span class="li-normal">type: dict</span>
 <a id='label66' href="javascript:ContentClick('label67', 'label66');" onmouseover="ContentPreview('label67');" onmouseout="ContentUnpreview('label67');" title="click to collapse or expand..."> more... </a>
 <div id="label67" style="display:none">
 <table border="1">
 <tr>
 <td></td>
 <td><code class="docutils literal notranslate">v7.0.0 </code></td>
 </tr>
 <tr>
 <td>dh_group_20</td>
 <td>yes</td>
 </tr>
 </table>
 </div>
 </li>
            <ul class="ul-self">
            <li> <span class="li-head">keypair_cache</span> - Configure custom key pair cache size for this Diffie-Hellman group. <span class="li-normal">type: str</span> <span class="li-normal">choices: global, custom</span>
 <a id='label68' href="javascript:ContentClick('label69', 'label68');" onmouseover="ContentPreview('label69');" onmouseout="ContentUnpreview('label69');" title="click to collapse or expand..."> more... </a>
 <div id="label69" style="display:none">
 <table border="1">
 <tr>
 <td></td>
 <td><code class="docutils literal notranslate">v7.0.0 </code></td>
 </tr>
 <tr>
 <td>keypair_cache</td>
 <td>yes</td>
 </tr>
 <tr>
 <td>[global]</td>
 <td>yes</td>
 </tr>
 <tr>
 <td>[custom]</td>
 <td>yes</td>
 </tr>
 </table>
 </div>
 </li>
            <li> <span class="li-head">keypair_count</span> - Number of key pairs to pre-generate for this Diffie-Hellman group (per-worker). <span class="li-normal">type: int</span>
 <a id='label70' href="javascript:ContentClick('label71', 'label70');" onmouseover="ContentPreview('label71');" onmouseout="ContentUnpreview('label71');" title="click to collapse or expand..."> more... </a>
 <div id="label71" style="display:none">
 <table border="1">
 <tr>
 <td></td>
 <td><code class="docutils literal notranslate">v7.0.0 </code></td>
 </tr>
 <tr>
 <td>keypair_count</td>
 <td>yes</td>
 </tr>
 </table>
 </div>
 </li>
            <li> <span class="li-head">mode</span> - Use software (CPU) or hardware (CPX) to perform calculations for this Diffie-Hellman group. <span class="li-normal">type: str</span> <span class="li-normal">choices: software, hardware, global</span>
 <a id='label72' href="javascript:ContentClick('label73', 'label72');" onmouseover="ContentPreview('label73');" onmouseout="ContentUnpreview('label73');" title="click to collapse or expand..."> more... </a>
 <div id="label73" style="display:none">
 <table border="1">
 <tr>
 <td></td>
 <td><code class="docutils literal notranslate">v7.0.0 </code></td>
 </tr>
 <tr>
 <td>mode</td>
 <td>yes</td>
 </tr>
 <tr>
 <td>[software]</td>
 <td>yes</td>
 </tr>
 <tr>
 <td>[hardware]</td>
 <td>yes</td>
 </tr>
 <tr>
 <td>[global]</td>
 <td>yes</td>
 </tr>
 </table>
 </div>
 </li>
            </ul>
        <li> <span class="li-head">dh_group_21</span> - Diffie-Hellman group 21 (EC-P521). <span class="li-normal">type: dict</span>
 <a id='label74' href="javascript:ContentClick('label75', 'label74');" onmouseover="ContentPreview('label75');" onmouseout="ContentUnpreview('label75');" title="click to collapse or expand..."> more... </a>
 <div id="label75" style="display:none">
 <table border="1">
 <tr>
 <td></td>
 <td><code class="docutils literal notranslate">v7.0.0 </code></td>
 </tr>
 <tr>
 <td>dh_group_21</td>
 <td>yes</td>
 </tr>
 </table>
 </div>
 </li>
            <ul class="ul-self">
            <li> <span class="li-head">keypair_cache</span> - Configure custom key pair cache size for this Diffie-Hellman group. <span class="li-normal">type: str</span> <span class="li-normal">choices: global, custom</span>
 <a id='label76' href="javascript:ContentClick('label77', 'label76');" onmouseover="ContentPreview('label77');" onmouseout="ContentUnpreview('label77');" title="click to collapse or expand..."> more... </a>
 <div id="label77" style="display:none">
 <table border="1">
 <tr>
 <td></td>
 <td><code class="docutils literal notranslate">v7.0.0 </code></td>
 </tr>
 <tr>
 <td>keypair_cache</td>
 <td>yes</td>
 </tr>
 <tr>
 <td>[global]</td>
 <td>yes</td>
 </tr>
 <tr>
 <td>[custom]</td>
 <td>yes</td>
 </tr>
 </table>
 </div>
 </li>
            <li> <span class="li-head">keypair_count</span> - Number of key pairs to pre-generate for this Diffie-Hellman group (per-worker). <span class="li-normal">type: int</span>
 <a id='label78' href="javascript:ContentClick('label79', 'label78');" onmouseover="ContentPreview('label79');" onmouseout="ContentUnpreview('label79');" title="click to collapse or expand..."> more... </a>
 <div id="label79" style="display:none">
 <table border="1">
 <tr>
 <td></td>
 <td><code class="docutils literal notranslate">v7.0.0 </code></td>
 </tr>
 <tr>
 <td>keypair_count</td>
 <td>yes</td>
 </tr>
 </table>
 </div>
 </li>
            <li> <span class="li-head">mode</span> - Use software (CPU) or hardware (CPX) to perform calculations for this Diffie-Hellman group. <span class="li-normal">type: str</span> <span class="li-normal">choices: software, hardware, global</span>
 <a id='label80' href="javascript:ContentClick('label81', 'label80');" onmouseover="ContentPreview('label81');" onmouseout="ContentUnpreview('label81');" title="click to collapse or expand..."> more... </a>
 <div id="label81" style="display:none">
 <table border="1">
 <tr>
 <td></td>
 <td><code class="docutils literal notranslate">v7.0.0 </code></td>
 </tr>
 <tr>
 <td>mode</td>
 <td>yes</td>
 </tr>
 <tr>
 <td>[software]</td>
 <td>yes</td>
 </tr>
 <tr>
 <td>[hardware]</td>
 <td>yes</td>
 </tr>
 <tr>
 <td>[global]</td>
 <td>yes</td>
 </tr>
 </table>
 </div>
 </li>
            </ul>
        <li> <span class="li-head">dh_group_27</span> - Diffie-Hellman group 27 (EC-P224BP). <span class="li-normal">type: dict</span>
 <a id='label82' href="javascript:ContentClick('label83', 'label82');" onmouseover="ContentPreview('label83');" onmouseout="ContentUnpreview('label83');" title="click to collapse or expand..."> more... </a>
 <div id="label83" style="display:none">
 <table border="1">
 <tr>
 <td></td>
 <td><code class="docutils literal notranslate">v7.0.0 </code></td>
 </tr>
 <tr>
 <td>dh_group_27</td>
 <td>yes</td>
 </tr>
 </table>
 </div>
 </li>
            <ul class="ul-self">
            <li> <span class="li-head">keypair_cache</span> - Configure custom key pair cache size for this Diffie-Hellman group. <span class="li-normal">type: str</span> <span class="li-normal">choices: global, custom</span>
 <a id='label84' href="javascript:ContentClick('label85', 'label84');" onmouseover="ContentPreview('label85');" onmouseout="ContentUnpreview('label85');" title="click to collapse or expand..."> more... </a>
 <div id="label85" style="display:none">
 <table border="1">
 <tr>
 <td></td>
 <td><code class="docutils literal notranslate">v7.0.0 </code></td>
 </tr>
 <tr>
 <td>keypair_cache</td>
 <td>yes</td>
 </tr>
 <tr>
 <td>[global]</td>
 <td>yes</td>
 </tr>
 <tr>
 <td>[custom]</td>
 <td>yes</td>
 </tr>
 </table>
 </div>
 </li>
            <li> <span class="li-head">keypair_count</span> - Number of key pairs to pre-generate for this Diffie-Hellman group (per-worker). <span class="li-normal">type: int</span>
 <a id='label86' href="javascript:ContentClick('label87', 'label86');" onmouseover="ContentPreview('label87');" onmouseout="ContentUnpreview('label87');" title="click to collapse or expand..."> more... </a>
 <div id="label87" style="display:none">
 <table border="1">
 <tr>
 <td></td>
 <td><code class="docutils literal notranslate">v7.0.0 </code></td>
 </tr>
 <tr>
 <td>keypair_count</td>
 <td>yes</td>
 </tr>
 </table>
 </div>
 </li>
            <li> <span class="li-head">mode</span> - Use software (CPU) or hardware (CPX) to perform calculations for this Diffie-Hellman group. <span class="li-normal">type: str</span> <span class="li-normal">choices: software, hardware, global</span>
 <a id='label88' href="javascript:ContentClick('label89', 'label88');" onmouseover="ContentPreview('label89');" onmouseout="ContentUnpreview('label89');" title="click to collapse or expand..."> more... </a>
 <div id="label89" style="display:none">
 <table border="1">
 <tr>
 <td></td>
 <td><code class="docutils literal notranslate">v7.0.0 </code></td>
 </tr>
 <tr>
 <td>mode</td>
 <td>yes</td>
 </tr>
 <tr>
 <td>[software]</td>
 <td>yes</td>
 </tr>
 <tr>
 <td>[hardware]</td>
 <td>yes</td>
 </tr>
 <tr>
 <td>[global]</td>
 <td>yes</td>
 </tr>
 </table>
 </div>
 </li>
            </ul>
        <li> <span class="li-head">dh_group_28</span> - Diffie-Hellman group 28 (EC-P256BP). <span class="li-normal">type: dict</span>
 <a id='label90' href="javascript:ContentClick('label91', 'label90');" onmouseover="ContentPreview('label91');" onmouseout="ContentUnpreview('label91');" title="click to collapse or expand..."> more... </a>
 <div id="label91" style="display:none">
 <table border="1">
 <tr>
 <td></td>
 <td><code class="docutils literal notranslate">v7.0.0 </code></td>
 </tr>
 <tr>
 <td>dh_group_28</td>
 <td>yes</td>
 </tr>
 </table>
 </div>
 </li>
            <ul class="ul-self">
            <li> <span class="li-head">keypair_cache</span> - Configure custom key pair cache size for this Diffie-Hellman group. <span class="li-normal">type: str</span> <span class="li-normal">choices: global, custom</span>
 <a id='label92' href="javascript:ContentClick('label93', 'label92');" onmouseover="ContentPreview('label93');" onmouseout="ContentUnpreview('label93');" title="click to collapse or expand..."> more... </a>
 <div id="label93" style="display:none">
 <table border="1">
 <tr>
 <td></td>
 <td><code class="docutils literal notranslate">v7.0.0 </code></td>
 </tr>
 <tr>
 <td>keypair_cache</td>
 <td>yes</td>
 </tr>
 <tr>
 <td>[global]</td>
 <td>yes</td>
 </tr>
 <tr>
 <td>[custom]</td>
 <td>yes</td>
 </tr>
 </table>
 </div>
 </li>
            <li> <span class="li-head">keypair_count</span> - Number of key pairs to pre-generate for this Diffie-Hellman group (per-worker). <span class="li-normal">type: int</span>
 <a id='label94' href="javascript:ContentClick('label95', 'label94');" onmouseover="ContentPreview('label95');" onmouseout="ContentUnpreview('label95');" title="click to collapse or expand..."> more... </a>
 <div id="label95" style="display:none">
 <table border="1">
 <tr>
 <td></td>
 <td><code class="docutils literal notranslate">v7.0.0 </code></td>
 </tr>
 <tr>
 <td>keypair_count</td>
 <td>yes</td>
 </tr>
 </table>
 </div>
 </li>
            <li> <span class="li-head">mode</span> - Use software (CPU) or hardware (CPX) to perform calculations for this Diffie-Hellman group. <span class="li-normal">type: str</span> <span class="li-normal">choices: software, hardware, global</span>
 <a id='label96' href="javascript:ContentClick('label97', 'label96');" onmouseover="ContentPreview('label97');" onmouseout="ContentUnpreview('label97');" title="click to collapse or expand..."> more... </a>
 <div id="label97" style="display:none">
 <table border="1">
 <tr>
 <td></td>
 <td><code class="docutils literal notranslate">v7.0.0 </code></td>
 </tr>
 <tr>
 <td>mode</td>
 <td>yes</td>
 </tr>
 <tr>
 <td>[software]</td>
 <td>yes</td>
 </tr>
 <tr>
 <td>[hardware]</td>
 <td>yes</td>
 </tr>
 <tr>
 <td>[global]</td>
 <td>yes</td>
 </tr>
 </table>
 </div>
 </li>
            </ul>
        <li> <span class="li-head">dh_group_29</span> - Diffie-Hellman group 29 (EC-P384BP). <span class="li-normal">type: dict</span>
 <a id='label98' href="javascript:ContentClick('label99', 'label98');" onmouseover="ContentPreview('label99');" onmouseout="ContentUnpreview('label99');" title="click to collapse or expand..."> more... </a>
 <div id="label99" style="display:none">
 <table border="1">
 <tr>
 <td></td>
 <td><code class="docutils literal notranslate">v7.0.0 </code></td>
 </tr>
 <tr>
 <td>dh_group_29</td>
 <td>yes</td>
 </tr>
 </table>
 </div>
 </li>
            <ul class="ul-self">
            <li> <span class="li-head">keypair_cache</span> - Configure custom key pair cache size for this Diffie-Hellman group. <span class="li-normal">type: str</span> <span class="li-normal">choices: global, custom</span>
 <a id='label100' href="javascript:ContentClick('label101', 'label100');" onmouseover="ContentPreview('label101');" onmouseout="ContentUnpreview('label101');" title="click to collapse or expand..."> more... </a>
 <div id="label101" style="display:none">
 <table border="1">
 <tr>
 <td></td>
 <td><code class="docutils literal notranslate">v7.0.0 </code></td>
 </tr>
 <tr>
 <td>keypair_cache</td>
 <td>yes</td>
 </tr>
 <tr>
 <td>[global]</td>
 <td>yes</td>
 </tr>
 <tr>
 <td>[custom]</td>
 <td>yes</td>
 </tr>
 </table>
 </div>
 </li>
            <li> <span class="li-head">keypair_count</span> - Number of key pairs to pre-generate for this Diffie-Hellman group (per-worker). <span class="li-normal">type: int</span>
 <a id='label102' href="javascript:ContentClick('label103', 'label102');" onmouseover="ContentPreview('label103');" onmouseout="ContentUnpreview('label103');" title="click to collapse or expand..."> more... </a>
 <div id="label103" style="display:none">
 <table border="1">
 <tr>
 <td></td>
 <td><code class="docutils literal notranslate">v7.0.0 </code></td>
 </tr>
 <tr>
 <td>keypair_count</td>
 <td>yes</td>
 </tr>
 </table>
 </div>
 </li>
            <li> <span class="li-head">mode</span> - Use software (CPU) or hardware (CPX) to perform calculations for this Diffie-Hellman group. <span class="li-normal">type: str</span> <span class="li-normal">choices: software, hardware, global</span>
 <a id='label104' href="javascript:ContentClick('label105', 'label104');" onmouseover="ContentPreview('label105');" onmouseout="ContentUnpreview('label105');" title="click to collapse or expand..."> more... </a>
 <div id="label105" style="display:none">
 <table border="1">
 <tr>
 <td></td>
 <td><code class="docutils literal notranslate">v7.0.0 </code></td>
 </tr>
 <tr>
 <td>mode</td>
 <td>yes</td>
 </tr>
 <tr>
 <td>[software]</td>
 <td>yes</td>
 </tr>
 <tr>
 <td>[hardware]</td>
 <td>yes</td>
 </tr>
 <tr>
 <td>[global]</td>
 <td>yes</td>
 </tr>
 </table>
 </div>
 </li>
            </ul>
        <li> <span class="li-head">dh_group_30</span> - Diffie-Hellman group 30 (EC-P512BP). <span class="li-normal">type: dict</span>
 <a id='label106' href="javascript:ContentClick('label107', 'label106');" onmouseover="ContentPreview('label107');" onmouseout="ContentUnpreview('label107');" title="click to collapse or expand..."> more... </a>
 <div id="label107" style="display:none">
 <table border="1">
 <tr>
 <td></td>
 <td><code class="docutils literal notranslate">v7.0.0 </code></td>
 </tr>
 <tr>
 <td>dh_group_30</td>
 <td>yes</td>
 </tr>
 </table>
 </div>
 </li>
            <ul class="ul-self">
            <li> <span class="li-head">keypair_cache</span> - Configure custom key pair cache size for this Diffie-Hellman group. <span class="li-normal">type: str</span> <span class="li-normal">choices: global, custom</span>
 <a id='label108' href="javascript:ContentClick('label109', 'label108');" onmouseover="ContentPreview('label109');" onmouseout="ContentUnpreview('label109');" title="click to collapse or expand..."> more... </a>
 <div id="label109" style="display:none">
 <table border="1">
 <tr>
 <td></td>
 <td><code class="docutils literal notranslate">v7.0.0 </code></td>
 </tr>
 <tr>
 <td>keypair_cache</td>
 <td>yes</td>
 </tr>
 <tr>
 <td>[global]</td>
 <td>yes</td>
 </tr>
 <tr>
 <td>[custom]</td>
 <td>yes</td>
 </tr>
 </table>
 </div>
 </li>
            <li> <span class="li-head">keypair_count</span> - Number of key pairs to pre-generate for this Diffie-Hellman group (per-worker). <span class="li-normal">type: int</span>
 <a id='label110' href="javascript:ContentClick('label111', 'label110');" onmouseover="ContentPreview('label111');" onmouseout="ContentUnpreview('label111');" title="click to collapse or expand..."> more... </a>
 <div id="label111" style="display:none">
 <table border="1">
 <tr>
 <td></td>
 <td><code class="docutils literal notranslate">v7.0.0 </code></td>
 </tr>
 <tr>
 <td>keypair_count</td>
 <td>yes</td>
 </tr>
 </table>
 </div>
 </li>
            <li> <span class="li-head">mode</span> - Use software (CPU) or hardware (CPX) to perform calculations for this Diffie-Hellman group. <span class="li-normal">type: str</span> <span class="li-normal">choices: software, hardware, global</span>
 <a id='label112' href="javascript:ContentClick('label113', 'label112');" onmouseover="ContentPreview('label113');" onmouseout="ContentUnpreview('label113');" title="click to collapse or expand..."> more... </a>
 <div id="label113" style="display:none">
 <table border="1">
 <tr>
 <td></td>
 <td><code class="docutils literal notranslate">v7.0.0 </code></td>
 </tr>
 <tr>
 <td>mode</td>
 <td>yes</td>
 </tr>
 <tr>
 <td>[software]</td>
 <td>yes</td>
 </tr>
 <tr>
 <td>[hardware]</td>
 <td>yes</td>
 </tr>
 <tr>
 <td>[global]</td>
 <td>yes</td>
 </tr>
 </table>
 </div>
 </li>
            </ul>
        <li> <span class="li-head">dh_group_31</span> - Diffie-Hellman group 31 (EC-X25519). <span class="li-normal">type: dict</span>
 <a id='label114' href="javascript:ContentClick('label115', 'label114');" onmouseover="ContentPreview('label115');" onmouseout="ContentUnpreview('label115');" title="click to collapse or expand..."> more... </a>
 <div id="label115" style="display:none">
 <table border="1">
 <tr>
 <td></td>
 <td><code class="docutils literal notranslate">v7.0.0 </code></td>
 </tr>
 <tr>
 <td>dh_group_31</td>
 <td>yes</td>
 </tr>
 </table>
 </div>
 </li>
            <ul class="ul-self">
            <li> <span class="li-head">keypair_cache</span> - Configure custom key pair cache size for this Diffie-Hellman group. <span class="li-normal">type: str</span> <span class="li-normal">choices: global, custom</span>
 <a id='label116' href="javascript:ContentClick('label117', 'label116');" onmouseover="ContentPreview('label117');" onmouseout="ContentUnpreview('label117');" title="click to collapse or expand..."> more... </a>
 <div id="label117" style="display:none">
 <table border="1">
 <tr>
 <td></td>
 <td><code class="docutils literal notranslate">v7.0.0 </code></td>
 </tr>
 <tr>
 <td>keypair_cache</td>
 <td>yes</td>
 </tr>
 <tr>
 <td>[global]</td>
 <td>yes</td>
 </tr>
 <tr>
 <td>[custom]</td>
 <td>yes</td>
 </tr>
 </table>
 </div>
 </li>
            <li> <span class="li-head">keypair_count</span> - Number of key pairs to pre-generate for this Diffie-Hellman group (per-worker). <span class="li-normal">type: int</span>
 <a id='label118' href="javascript:ContentClick('label119', 'label118');" onmouseover="ContentPreview('label119');" onmouseout="ContentUnpreview('label119');" title="click to collapse or expand..."> more... </a>
 <div id="label119" style="display:none">
 <table border="1">
 <tr>
 <td></td>
 <td><code class="docutils literal notranslate">v7.0.0 </code></td>
 </tr>
 <tr>
 <td>keypair_count</td>
 <td>yes</td>
 </tr>
 </table>
 </div>
 </li>
            <li> <span class="li-head">mode</span> - Use software (CPU) or hardware (CPX) to perform calculations for this Diffie-Hellman group. <span class="li-normal">type: str</span> <span class="li-normal">choices: software, hardware, global</span>
 <a id='label120' href="javascript:ContentClick('label121', 'label120');" onmouseover="ContentPreview('label121');" onmouseout="ContentUnpreview('label121');" title="click to collapse or expand..."> more... </a>
 <div id="label121" style="display:none">
 <table border="1">
 <tr>
 <td></td>
 <td><code class="docutils literal notranslate">v7.0.0 </code></td>
 </tr>
 <tr>
 <td>mode</td>
 <td>yes</td>
 </tr>
 <tr>
 <td>[software]</td>
 <td>yes</td>
 </tr>
 <tr>
 <td>[hardware]</td>
 <td>yes</td>
 </tr>
 <tr>
 <td>[global]</td>
 <td>yes</td>
 </tr>
 </table>
 </div>
 </li>
            </ul>
        <li> <span class="li-head">dh_group_32</span> - Diffie-Hellman group 32 (EC-X448). <span class="li-normal">type: dict</span>
 <a id='label122' href="javascript:ContentClick('label123', 'label122');" onmouseover="ContentPreview('label123');" onmouseout="ContentUnpreview('label123');" title="click to collapse or expand..."> more... </a>
 <div id="label123" style="display:none">
 <table border="1">
 <tr>
 <td></td>
 <td><code class="docutils literal notranslate">v7.0.0 </code></td>
 </tr>
 <tr>
 <td>dh_group_32</td>
 <td>yes</td>
 </tr>
 </table>
 </div>
 </li>
            <ul class="ul-self">
            <li> <span class="li-head">keypair_cache</span> - Configure custom key pair cache size for this Diffie-Hellman group. <span class="li-normal">type: str</span> <span class="li-normal">choices: global, custom</span>
 <a id='label124' href="javascript:ContentClick('label125', 'label124');" onmouseover="ContentPreview('label125');" onmouseout="ContentUnpreview('label125');" title="click to collapse or expand..."> more... </a>
 <div id="label125" style="display:none">
 <table border="1">
 <tr>
 <td></td>
 <td><code class="docutils literal notranslate">v7.0.0 </code></td>
 </tr>
 <tr>
 <td>keypair_cache</td>
 <td>yes</td>
 </tr>
 <tr>
 <td>[global]</td>
 <td>yes</td>
 </tr>
 <tr>
 <td>[custom]</td>
 <td>yes</td>
 </tr>
 </table>
 </div>
 </li>
            <li> <span class="li-head">keypair_count</span> - Number of key pairs to pre-generate for this Diffie-Hellman group (per-worker). <span class="li-normal">type: int</span>
 <a id='label126' href="javascript:ContentClick('label127', 'label126');" onmouseover="ContentPreview('label127');" onmouseout="ContentUnpreview('label127');" title="click to collapse or expand..."> more... </a>
 <div id="label127" style="display:none">
 <table border="1">
 <tr>
 <td></td>
 <td><code class="docutils literal notranslate">v7.0.0 </code></td>
 </tr>
 <tr>
 <td>keypair_count</td>
 <td>yes</td>
 </tr>
 </table>
 </div>
 </li>
            <li> <span class="li-head">mode</span> - Use software (CPU) or hardware (CPX) to perform calculations for this Diffie-Hellman group. <span class="li-normal">type: str</span> <span class="li-normal">choices: software, hardware, global</span>
 <a id='label128' href="javascript:ContentClick('label129', 'label128');" onmouseover="ContentPreview('label129');" onmouseout="ContentUnpreview('label129');" title="click to collapse or expand..."> more... </a>
 <div id="label129" style="display:none">
 <table border="1">
 <tr>
 <td></td>
 <td><code class="docutils literal notranslate">v7.0.0 </code></td>
 </tr>
 <tr>
 <td>mode</td>
 <td>yes</td>
 </tr>
 <tr>
 <td>[software]</td>
 <td>yes</td>
 </tr>
 <tr>
 <td>[hardware]</td>
 <td>yes</td>
 </tr>
 <tr>
 <td>[global]</td>
 <td>yes</td>
 </tr>
 </table>
 </div>
 </li>
            </ul>
        <li> <span class="li-head">dh_group_5</span> - Diffie-Hellman group 5 (MODP-1536). <span class="li-normal">type: dict</span>
 <a id='label130' href="javascript:ContentClick('label131', 'label130');" onmouseover="ContentPreview('label131');" onmouseout="ContentUnpreview('label131');" title="click to collapse or expand..."> more... </a>
 <div id="label131" style="display:none">
 <table border="1">
 <tr>
 <td></td>
 <td><code class="docutils literal notranslate">v7.0.0 </code></td>
 </tr>
 <tr>
 <td>dh_group_5</td>
 <td>yes</td>
 </tr>
 </table>
 </div>
 </li>
            <ul class="ul-self">
            <li> <span class="li-head">keypair_cache</span> - Configure custom key pair cache size for this Diffie-Hellman group. <span class="li-normal">type: str</span> <span class="li-normal">choices: global, custom</span>
 <a id='label132' href="javascript:ContentClick('label133', 'label132');" onmouseover="ContentPreview('label133');" onmouseout="ContentUnpreview('label133');" title="click to collapse or expand..."> more... </a>
 <div id="label133" style="display:none">
 <table border="1">
 <tr>
 <td></td>
 <td><code class="docutils literal notranslate">v7.0.0 </code></td>
 </tr>
 <tr>
 <td>keypair_cache</td>
 <td>yes</td>
 </tr>
 <tr>
 <td>[global]</td>
 <td>yes</td>
 </tr>
 <tr>
 <td>[custom]</td>
 <td>yes</td>
 </tr>
 </table>
 </div>
 </li>
            <li> <span class="li-head">keypair_count</span> - Number of key pairs to pre-generate for this Diffie-Hellman group (per-worker). <span class="li-normal">type: int</span>
 <a id='label134' href="javascript:ContentClick('label135', 'label134');" onmouseover="ContentPreview('label135');" onmouseout="ContentUnpreview('label135');" title="click to collapse or expand..."> more... </a>
 <div id="label135" style="display:none">
 <table border="1">
 <tr>
 <td></td>
 <td><code class="docutils literal notranslate">v7.0.0 </code></td>
 </tr>
 <tr>
 <td>keypair_count</td>
 <td>yes</td>
 </tr>
 </table>
 </div>
 </li>
            <li> <span class="li-head">mode</span> - Use software (CPU) or hardware (CPX) to perform calculations for this Diffie-Hellman group. <span class="li-normal">type: str</span> <span class="li-normal">choices: software, hardware, global</span>
 <a id='label136' href="javascript:ContentClick('label137', 'label136');" onmouseover="ContentPreview('label137');" onmouseout="ContentUnpreview('label137');" title="click to collapse or expand..."> more... </a>
 <div id="label137" style="display:none">
 <table border="1">
 <tr>
 <td></td>
 <td><code class="docutils literal notranslate">v7.0.0 </code></td>
 </tr>
 <tr>
 <td>mode</td>
 <td>yes</td>
 </tr>
 <tr>
 <td>[software]</td>
 <td>yes</td>
 </tr>
 <tr>
 <td>[hardware]</td>
 <td>yes</td>
 </tr>
 <tr>
 <td>[global]</td>
 <td>yes</td>
 </tr>
 </table>
 </div>
 </li>
            </ul>
        <li> <span class="li-head">dh_keypair_cache</span> - Enable/disable Diffie-Hellman key pair cache. <span class="li-normal">type: str</span> <span class="li-normal">choices: enable, disable</span>
 <a id='label138' href="javascript:ContentClick('label139', 'label138');" onmouseover="ContentPreview('label139');" onmouseout="ContentUnpreview('label139');" title="click to collapse or expand..."> more... </a>
 <div id="label139" style="display:none">
 <table border="1">
 <tr>
 <td></td>
 <td><code class="docutils literal notranslate">v7.0.0 </code></td>
 </tr>
 <tr>
 <td>dh_keypair_cache</td>
 <td>yes</td>
 </tr>
 <tr>
 <td>[enable]</td>
 <td>yes</td>
 </tr>
 <tr>
 <td>[disable]</td>
 <td>yes</td>
 </tr>
 </table>
 </div>
 </li>
        <li> <span class="li-head">dh_keypair_count</span> - Number of key pairs to pre-generate for each Diffie-Hellman group (per-worker). <span class="li-normal">type: int</span>
 <a id='label140' href="javascript:ContentClick('label141', 'label140');" onmouseover="ContentPreview('label141');" onmouseout="ContentUnpreview('label141');" title="click to collapse or expand..."> more... </a>
 <div id="label141" style="display:none">
 <table border="1">
 <tr>
 <td></td>
 <td><code class="docutils literal notranslate">v7.0.0 </code></td>
 </tr>
 <tr>
 <td>dh_keypair_count</td>
 <td>yes</td>
 </tr>
 </table>
 </div>
 </li>
        <li> <span class="li-head">dh_keypair_throttle</span> - Enable/disable Diffie-Hellman key pair cache CPU throttling. <span class="li-normal">type: str</span> <span class="li-normal">choices: enable, disable</span>
 <a id='label142' href="javascript:ContentClick('label143', 'label142');" onmouseover="ContentPreview('label143');" onmouseout="ContentUnpreview('label143');" title="click to collapse or expand..."> more... </a>
 <div id="label143" style="display:none">
 <table border="1">
 <tr>
 <td></td>
 <td><code class="docutils literal notranslate">v7.0.0 </code></td>
 </tr>
 <tr>
 <td>dh_keypair_throttle</td>
 <td>yes</td>
 </tr>
 <tr>
 <td>[enable]</td>
 <td>yes</td>
 </tr>
 <tr>
 <td>[disable]</td>
 <td>yes</td>
 </tr>
 </table>
 </div>
 </li>
        <li> <span class="li-head">dh_mode</span> - Use software (CPU) or hardware (CPX) to perform Diffie-Hellman calculations. <span class="li-normal">type: str</span> <span class="li-normal">choices: software, hardware</span>
 <a id='label144' href="javascript:ContentClick('label145', 'label144');" onmouseover="ContentPreview('label145');" onmouseout="ContentUnpreview('label145');" title="click to collapse or expand..."> more... </a>
 <div id="label145" style="display:none">
 <table border="1">
 <tr>
 <td></td>
 <td><code class="docutils literal notranslate">v7.0.0 </code></td>
 </tr>
 <tr>
 <td>dh_mode</td>
 <td>yes</td>
 </tr>
 <tr>
 <td>[software]</td>
 <td>yes</td>
 </tr>
 <tr>
 <td>[hardware]</td>
 <td>yes</td>
 </tr>
 </table>
 </div>
 </li>
        <li> <span class="li-head">dh_multiprocess</span> - Enable/disable multiprocess Diffie-Hellman daemon for IKE. <span class="li-normal">type: str</span> <span class="li-normal">choices: enable, disable</span>
 <a id='label146' href="javascript:ContentClick('label147', 'label146');" onmouseover="ContentPreview('label147');" onmouseout="ContentUnpreview('label147');" title="click to collapse or expand..."> more... </a>
 <div id="label147" style="display:none">
 <table border="1">
 <tr>
 <td></td>
 <td><code class="docutils literal notranslate">v7.0.0 </code></td>
 </tr>
 <tr>
 <td>dh_multiprocess</td>
 <td>yes</td>
 </tr>
 <tr>
 <td>[enable]</td>
 <td>yes</td>
 </tr>
 <tr>
 <td>[disable]</td>
 <td>yes</td>
 </tr>
 </table>
 </div>
 </li>
        <li> <span class="li-head">dh_worker_count</span> - Number of Diffie-Hellman workers to start. <span class="li-normal">type: int</span>
 <a id='label148' href="javascript:ContentClick('label149', 'label148');" onmouseover="ContentPreview('label149');" onmouseout="ContentUnpreview('label149');" title="click to collapse or expand..."> more... </a>
 <div id="label149" style="display:none">
 <table border="1">
 <tr>
 <td></td>
 <td><code class="docutils literal notranslate">v7.0.0 </code></td>
 </tr>
 <tr>
 <td>dh_worker_count</td>
 <td>yes</td>
 </tr>
 </table>
 </div>
 </li>
        <li> <span class="li-head">embryonic_limit</span> - Maximum number of IPsec tunnels to negotiate simultaneously. <span class="li-normal">type: int</span>
 <a id='label150' href="javascript:ContentClick('label151', 'label150');" onmouseover="ContentPreview('label151');" onmouseout="ContentUnpreview('label151');" title="click to collapse or expand..."> more... </a>
 <div id="label151" style="display:none">
 <table border="1">
 <tr>
 <td></td>
 <td><code class="docutils literal notranslate">v7.0.0 </code></td>
 </tr>
 <tr>
 <td>embryonic_limit</td>
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
      - name: Configure IKE global attributes.
        fortios_system_ike:
          vdom:  "{{ vdom }}"
          system_ike:
            dh_group_1:
                keypair_cache: "global"
                keypair_count: "5"
                mode: "software"
            dh_group_14:
                keypair_cache: "global"
                keypair_count: "9"
                mode: "software"
            dh_group_15:
                keypair_cache: "global"
                keypair_count: "13"
                mode: "software"
            dh_group_16:
                keypair_cache: "global"
                keypair_count: "17"
                mode: "software"
            dh_group_17:
                keypair_cache: "global"
                keypair_count: "21"
                mode: "software"
            dh_group_18:
                keypair_cache: "global"
                keypair_count: "25"
                mode: "software"
            dh_group_19:
                keypair_cache: "global"
                keypair_count: "29"
                mode: "software"
            dh_group_2:
                keypair_cache: "global"
                keypair_count: "33"
                mode: "software"
            dh_group_20:
                keypair_cache: "global"
                keypair_count: "37"
                mode: "software"
            dh_group_21:
                keypair_cache: "global"
                keypair_count: "41"
                mode: "software"
            dh_group_27:
                keypair_cache: "global"
                keypair_count: "45"
                mode: "software"
            dh_group_28:
                keypair_cache: "global"
                keypair_count: "49"
                mode: "software"
            dh_group_29:
                keypair_cache: "global"
                keypair_count: "53"
                mode: "software"
            dh_group_30:
                keypair_cache: "global"
                keypair_count: "57"
                mode: "software"
            dh_group_31:
                keypair_cache: "global"
                keypair_count: "61"
                mode: "software"
            dh_group_32:
                keypair_cache: "global"
                keypair_count: "65"
                mode: "software"
            dh_group_5:
                keypair_cache: "global"
                keypair_count: "69"
                mode: "software"
            dh_keypair_cache: "enable"
            dh_keypair_count: "72"
            dh_keypair_throttle: "enable"
            dh_mode: "software"
            dh_multiprocess: "enable"
            dh_worker_count: "76"
            embryonic_limit: "77"
    


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
