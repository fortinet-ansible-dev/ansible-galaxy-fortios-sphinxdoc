:source: fortios_wireless_controller_setting.py

:orphan:

.. fortios_wireless_controller_setting:

fortios_wireless_controller_setting -- VDOM wireless controller configuration in Fortinet's FortiOS and FortiGate.
++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++

.. versionadded:: 2.0.0

.. contents::
   :local:
   :depth: 1


Synopsis
--------
- This module is able to configure a FortiGate or FortiOS (FOS) device by allowing the user to set and modify wireless_controller feature and setting category. Examples include all parameters and values need to be adjusted to datasources before usage. Tested with FOS v6.0.0



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
    <li> <span class="li-head">wireless_controller_setting</span> - VDOM wireless controller configuration. <span class="li-normal">type: dict</span>
 <a id='label0' href="javascript:ContentClick('label1', 'label0');" onmouseover="ContentPreview('label1');" onmouseout="ContentUnpreview('label1');" title="click to collapse or expand..."> more... </a>
 <div id="label1" style="display:none">
 <table border="1">
 <tr>
 <td></td><td colspan="1">Supported Version Ranges</td>
 </tr>
 <tr>
 <td>wireless_controller_setting</td>
 <td><code class="docutils literal notranslate">v6.0.0 -> 7.6.0 </code></td>
 </tr>
 </table>
 </div>
 </li>
        <ul class="ul-self">
        <li> <span class="li-head">account_id</span> - FortiCloud customer account ID. <span class="li-normal">type: str</span>
 <a id='label2' href="javascript:ContentClick('label3', 'label2');" onmouseover="ContentPreview('label3');" onmouseout="ContentUnpreview('label3');" title="click to collapse or expand..."> more... </a>
 <div id="label3" style="display:none">
 <table border="1">
 <tr>
 <td></td>
 <td colspan="1">Supported Version Ranges</td>
 </tr>
 <tr>
 <td>account_id</td>
 <td><code class="docutils literal notranslate">v6.0.0 -> 7.6.0 </code></td>
 </tr>
 </table>
 </div>
 </li>
        <li> <span class="li-head">country</span> - Country or region in which the FortiGate is located. The country determines the 802.11 bands and channels that are available. <span class="li-normal">type: str</span> <span class="li-normal">choices: --, AF, AL, DZ, AS, AO, AR, AM, AU, AT, AZ, BS, BH, BD, BB, BY, BE, BZ, BJ, BM, BT, BO, BA, BW, BR, BN, BG, BF, KH, CM, KY, CF, TD, CL, CN, CX, CO, CG, CD, CR, HR, CY, CZ, DK, DJ, DM, DO, EC, EG, SV, ET, EE, GF, PF, FO, FJ, FI, FR, GA, GE, GM, DE, GH, GI, GR, GL, GD, GP, GU, GT, GY, HT, HN, HK, HU, IS, IN, ID, IQ, IE, IM, IL, IT, CI, JM, JO, KZ, KE, KR, KW, LA, LV, LB, LS, LR, LY, LI, LT, LU, MO, MK, MG, MW, MY, MV, ML, MT, MH, MQ, MR, MU, YT, MX, FM, MD, MC, MN, MA, MZ, MM, NA, NP, NL, AN, AW, NZ, NI, NE, NG, NO, MP, OM, PK, PW, PA, PG, PY, PE, PH, PL, PT, PR, QA, RE, RO, RU, RW, BL, KN, LC, MF, PM, VC, SA, SN, RS, ME, SL, SG, SK, SI, SO, ZA, ES, LK, SR, SZ, SE, CH, TW, TZ, TH, TG, TT, TN, TR, TM, AE, TC, UG, UA, GB, US, PS, UY, UZ, VU, VE, VN, VI, WF, YE, ZM, ZW, JP, CA, IR, KP, SD, SY, ZB</span>
 <a id='label4' href="javascript:ContentClick('label5', 'label4');" onmouseover="ContentPreview('label5');" onmouseout="ContentUnpreview('label5');" title="click to collapse or expand..."> more... </a>
 <div id="label5" style="display:none">
 <table border="1">
 <tr>
 <td></td>
 <td colspan="1">Supported Version Ranges</td>
 </tr>
 <tr>
 <td>country</td>
 <td><code class="docutils literal notranslate">v6.0.0 -> 7.6.0 </code></td>
 </tr>
 <tr>
 <td>[--]</td>
 <td><code class="docutils literal notranslate">v7.0.1 -> 7.6.0</code></td>
 </tr>
 <tr>
 <td>[AF]</td>
 <td><code class="docutils literal notranslate">v7.0.0 -> 7.6.0</code></td>
 </tr>
 <tr>
 <td>[AL]</td>
 <td><code class="docutils literal notranslate">v6.0.0 -> 7.6.0</code></td>
 <tr>
 <td>[DZ]</td>
 <td><code class="docutils literal notranslate">v6.0.0 -> 7.6.0</code></td>
 <tr>
 <td>[AS]</td>
 <td><code class="docutils literal notranslate">v7.0.0 -> 7.6.0</code></td>
 </tr>
 <tr>
 <td>[AO]</td>
 <td><code class="docutils literal notranslate">v6.0.0 -> 7.6.0</code></td>
 <tr>
 <td>[AR]</td>
 <td><code class="docutils literal notranslate">v6.0.0 -> 7.6.0</code></td>
 <tr>
 <td>[AM]</td>
 <td><code class="docutils literal notranslate">v6.0.0 -> 7.6.0</code></td>
 <tr>
 <td>[AU]</td>
 <td><code class="docutils literal notranslate">v6.0.0 -> 7.6.0</code></td>
 <tr>
 <td>[AT]</td>
 <td><code class="docutils literal notranslate">v6.0.0 -> 7.6.0</code></td>
 <tr>
 <td>[AZ]</td>
 <td><code class="docutils literal notranslate">v6.0.0 -> 7.6.0</code></td>
 <tr>
 <td>[BS]</td>
 <td><code class="docutils literal notranslate">v6.4.0 -> 7.6.0</code></td>
 </tr>
 <tr>
 <td>[BH]</td>
 <td><code class="docutils literal notranslate">v6.0.0 -> 7.6.0</code></td>
 <tr>
 <td>[BD]</td>
 <td><code class="docutils literal notranslate">v6.0.0 -> 7.6.0</code></td>
 <tr>
 <td>[BB]</td>
 <td><code class="docutils literal notranslate">v6.0.0 -> 7.6.0</code></td>
 <tr>
 <td>[BY]</td>
 <td><code class="docutils literal notranslate">v6.0.0 -> 7.6.0</code></td>
 <tr>
 <td>[BE]</td>
 <td><code class="docutils literal notranslate">v6.0.0 -> 7.6.0</code></td>
 <tr>
 <td>[BZ]</td>
 <td><code class="docutils literal notranslate">v6.0.0 -> 7.6.0</code></td>
 <tr>
 <td>[BJ]</td>
 <td><code class="docutils literal notranslate">v7.0.0 -> 7.6.0</code></td>
 </tr>
 <tr>
 <td>[BM]</td>
 <td><code class="docutils literal notranslate">v7.0.0 -> 7.6.0</code></td>
 </tr>
 <tr>
 <td>[BT]</td>
 <td><code class="docutils literal notranslate">v7.0.0 -> 7.6.0</code></td>
 </tr>
 <tr>
 <td>[BO]</td>
 <td><code class="docutils literal notranslate">v6.0.0 -> 7.6.0</code></td>
 <tr>
 <td>[BA]</td>
 <td><code class="docutils literal notranslate">v6.0.0 -> 7.6.0</code></td>
 <tr>
 <td>[BW]</td>
 <td><code class="docutils literal notranslate">v7.0.0 -> 7.6.0</code></td>
 </tr>
 <tr>
 <td>[BR]</td>
 <td><code class="docutils literal notranslate">v6.0.0 -> 7.6.0</code></td>
 <tr>
 <td>[BN]</td>
 <td><code class="docutils literal notranslate">v6.0.0 -> 7.6.0</code></td>
 <tr>
 <td>[BG]</td>
 <td><code class="docutils literal notranslate">v6.0.0 -> 7.6.0</code></td>
 <tr>
 <td>[BF]</td>
 <td><code class="docutils literal notranslate">v6.4.0 -> v6.4.0</code></td>
 <td><code class="docutils literal notranslate">v6.4.4 -> 7.6.0</code></td>
 </tr>
 <tr>
 <td>[KH]</td>
 <td><code class="docutils literal notranslate">v6.0.0 -> 7.6.0</code></td>
 <tr>
 <td>[CM]</td>
 <td><code class="docutils literal notranslate">v7.0.0 -> 7.6.0</code></td>
 </tr>
 <tr>
 <td>[KY]</td>
 <td><code class="docutils literal notranslate">v6.4.0 -> v6.4.0</code></td>
 <td><code class="docutils literal notranslate">v6.4.4 -> 7.6.0</code></td>
 </tr>
 <tr>
 <td>[CF]</td>
 <td><code class="docutils literal notranslate">v6.2.0 -> 7.6.0</code></td>
 </tr>
 <tr>
 <td>[TD]</td>
 <td><code class="docutils literal notranslate">v7.0.0 -> 7.6.0</code></td>
 </tr>
 <tr>
 <td>[CL]</td>
 <td><code class="docutils literal notranslate">v6.0.0 -> 7.6.0</code></td>
 <tr>
 <td>[CN]</td>
 <td><code class="docutils literal notranslate">v6.0.0 -> 7.6.0</code></td>
 <tr>
 <td>[CX]</td>
 <td><code class="docutils literal notranslate">v6.4.0 -> v6.4.0</code></td>
 <td><code class="docutils literal notranslate">v6.4.4 -> 7.6.0</code></td>
 </tr>
 <tr>
 <td>[CO]</td>
 <td><code class="docutils literal notranslate">v6.0.0 -> 7.6.0</code></td>
 <tr>
 <td>[CG]</td>
 <td><code class="docutils literal notranslate">v7.0.0 -> 7.6.0</code></td>
 </tr>
 <tr>
 <td>[CD]</td>
 <td><code class="docutils literal notranslate">v7.0.0 -> 7.6.0</code></td>
 </tr>
 <tr>
 <td>[CR]</td>
 <td><code class="docutils literal notranslate">v6.0.0 -> 7.6.0</code></td>
 <tr>
 <td>[HR]</td>
 <td><code class="docutils literal notranslate">v6.0.0 -> 7.6.0</code></td>
 <tr>
 <td>[CY]</td>
 <td><code class="docutils literal notranslate">v6.0.0 -> 7.6.0</code></td>
 <tr>
 <td>[CZ]</td>
 <td><code class="docutils literal notranslate">v6.0.0 -> 7.6.0</code></td>
 <tr>
 <td>[DK]</td>
 <td><code class="docutils literal notranslate">v6.0.0 -> 7.6.0</code></td>
 <tr>
 <td>[DJ]</td>
 <td><code class="docutils literal notranslate">v7.4.1 -> 7.6.0</code></td>
 </tr>
 <tr>
 <td>[DM]</td>
 <td><code class="docutils literal notranslate">v7.0.0 -> 7.6.0</code></td>
 </tr>
 <tr>
 <td>[DO]</td>
 <td><code class="docutils literal notranslate">v6.0.0 -> 7.6.0</code></td>
 <tr>
 <td>[EC]</td>
 <td><code class="docutils literal notranslate">v6.0.0 -> 7.6.0</code></td>
 <tr>
 <td>[EG]</td>
 <td><code class="docutils literal notranslate">v6.0.0 -> 7.6.0</code></td>
 <tr>
 <td>[SV]</td>
 <td><code class="docutils literal notranslate">v6.0.0 -> 7.6.0</code></td>
 <tr>
 <td>[ET]</td>
 <td><code class="docutils literal notranslate">v7.0.0 -> 7.6.0</code></td>
 </tr>
 <tr>
 <td>[EE]</td>
 <td><code class="docutils literal notranslate">v6.0.0 -> 7.6.0</code></td>
 <tr>
 <td>[GF]</td>
 <td><code class="docutils literal notranslate">v7.0.0 -> 7.6.0</code></td>
 </tr>
 <tr>
 <td>[PF]</td>
 <td><code class="docutils literal notranslate">v7.0.0 -> 7.6.0</code></td>
 </tr>
 <tr>
 <td>[FO]</td>
 <td><code class="docutils literal notranslate">v7.0.0 -> 7.6.0</code></td>
 </tr>
 <tr>
 <td>[FJ]</td>
 <td><code class="docutils literal notranslate">v7.0.0 -> 7.6.0</code></td>
 </tr>
 <tr>
 <td>[FI]</td>
 <td><code class="docutils literal notranslate">v6.0.0 -> 7.6.0</code></td>
 <tr>
 <td>[FR]</td>
 <td><code class="docutils literal notranslate">v6.0.0 -> 7.6.0</code></td>
 <tr>
 <td>[GA]</td>
 <td><code class="docutils literal notranslate">v7.4.1 -> 7.6.0</code></td>
 </tr>
 <tr>
 <td>[GE]</td>
 <td><code class="docutils literal notranslate">v6.0.0 -> 7.6.0</code></td>
 <tr>
 <td>[GM]</td>
 <td><code class="docutils literal notranslate">v7.4.1 -> 7.6.0</code></td>
 </tr>
 <tr>
 <td>[DE]</td>
 <td><code class="docutils literal notranslate">v6.0.0 -> 7.6.0</code></td>
 <tr>
 <td>[GH]</td>
 <td><code class="docutils literal notranslate">v6.4.0 -> v6.4.0</code></td>
 <td><code class="docutils literal notranslate">v6.4.4 -> 7.6.0</code></td>
 </tr>
 <tr>
 <td>[GI]</td>
 <td><code class="docutils literal notranslate">v7.0.0 -> 7.6.0</code></td>
 </tr>
 <tr>
 <td>[GR]</td>
 <td><code class="docutils literal notranslate">v6.0.0 -> 7.6.0</code></td>
 <tr>
 <td>[GL]</td>
 <td><code class="docutils literal notranslate">v6.0.0 -> 7.6.0</code></td>
 <tr>
 <td>[GD]</td>
 <td><code class="docutils literal notranslate">v6.0.0 -> 7.6.0</code></td>
 <tr>
 <td>[GP]</td>
 <td><code class="docutils literal notranslate">v7.0.0 -> 7.6.0</code></td>
 </tr>
 <tr>
 <td>[GU]</td>
 <td><code class="docutils literal notranslate">v6.0.0 -> 7.6.0</code></td>
 <tr>
 <td>[GT]</td>
 <td><code class="docutils literal notranslate">v6.0.0 -> 7.6.0</code></td>
 <tr>
 <td>[GY]</td>
 <td><code class="docutils literal notranslate">v6.4.0 -> v6.4.0</code></td>
 <td><code class="docutils literal notranslate">v6.4.4 -> 7.6.0</code></td>
 </tr>
 <tr>
 <td>[HT]</td>
 <td><code class="docutils literal notranslate">v6.0.0 -> 7.6.0</code></td>
 <tr>
 <td>[HN]</td>
 <td><code class="docutils literal notranslate">v6.0.0 -> 7.6.0</code></td>
 <tr>
 <td>[HK]</td>
 <td><code class="docutils literal notranslate">v6.0.0 -> 7.6.0</code></td>
 <tr>
 <td>[HU]</td>
 <td><code class="docutils literal notranslate">v6.0.0 -> 7.6.0</code></td>
 <tr>
 <td>[IS]</td>
 <td><code class="docutils literal notranslate">v6.0.0 -> 7.6.0</code></td>
 <tr>
 <td>[IN]</td>
 <td><code class="docutils literal notranslate">v6.0.0 -> 7.6.0</code></td>
 <tr>
 <td>[ID]</td>
 <td><code class="docutils literal notranslate">v6.0.0 -> 7.6.0</code></td>
 <tr>
 <td>[IQ]</td>
 <td><code class="docutils literal notranslate">v7.0.0 -> 7.6.0</code></td>
 </tr>
 <tr>
 <td>[IE]</td>
 <td><code class="docutils literal notranslate">v6.0.0 -> 7.6.0</code></td>
 <tr>
 <td>[IM]</td>
 <td><code class="docutils literal notranslate">v7.0.0 -> 7.6.0</code></td>
 </tr>
 <tr>
 <td>[IL]</td>
 <td><code class="docutils literal notranslate">v6.0.0 -> 7.6.0</code></td>
 <tr>
 <td>[IT]</td>
 <td><code class="docutils literal notranslate">v6.0.0 -> 7.6.0</code></td>
 <tr>
 <td>[CI]</td>
 <td><code class="docutils literal notranslate">v6.4.0 -> v6.4.0</code></td>
 <td><code class="docutils literal notranslate">v6.4.4 -> 7.6.0</code></td>
 </tr>
 <tr>
 <td>[JM]</td>
 <td><code class="docutils literal notranslate">v6.0.0 -> 7.6.0</code></td>
 <tr>
 <td>[JO]</td>
 <td><code class="docutils literal notranslate">v6.0.0 -> 7.6.0</code></td>
 <tr>
 <td>[KZ]</td>
 <td><code class="docutils literal notranslate">v6.0.0 -> 7.6.0</code></td>
 <tr>
 <td>[KE]</td>
 <td><code class="docutils literal notranslate">v6.0.0 -> 7.6.0</code></td>
 <tr>
 <td>[KR]</td>
 <td><code class="docutils literal notranslate">v6.0.0 -> 7.6.0</code></td>
 <tr>
 <td>[KW]</td>
 <td><code class="docutils literal notranslate">v6.0.0 -> 7.6.0</code></td>
 <tr>
 <td>[LA]</td>
 <td><code class="docutils literal notranslate">v7.0.0 -> 7.6.0</code></td>
 </tr>
 <tr>
 <td>[LV]</td>
 <td><code class="docutils literal notranslate">v6.0.0 -> 7.6.0</code></td>
 <tr>
 <td>[LB]</td>
 <td><code class="docutils literal notranslate">v6.0.0 -> 7.6.0</code></td>
 <tr>
 <td>[LS]</td>
 <td><code class="docutils literal notranslate">v7.0.0 -> 7.6.0</code></td>
 </tr>
 <tr>
 <td>[LR]</td>
 <td><code class="docutils literal notranslate">v7.4.1 -> 7.6.0</code></td>
 </tr>
 <tr>
 <td>[LY]</td>
 <td><code class="docutils literal notranslate">v7.0.0 -> 7.6.0</code></td>
 </tr>
 <tr>
 <td>[LI]</td>
 <td><code class="docutils literal notranslate">v6.0.0 -> 7.6.0</code></td>
 <tr>
 <td>[LT]</td>
 <td><code class="docutils literal notranslate">v6.0.0 -> 7.6.0</code></td>
 <tr>
 <td>[LU]</td>
 <td><code class="docutils literal notranslate">v6.0.0 -> 7.6.0</code></td>
 <tr>
 <td>[MO]</td>
 <td><code class="docutils literal notranslate">v6.0.0 -> 7.6.0</code></td>
 <tr>
 <td>[MK]</td>
 <td><code class="docutils literal notranslate">v6.0.0 -> 7.6.0</code></td>
 <tr>
 <td>[MG]</td>
 <td><code class="docutils literal notranslate">v7.0.0 -> 7.6.0</code></td>
 </tr>
 <tr>
 <td>[MW]</td>
 <td><code class="docutils literal notranslate">v6.4.0 -> v6.4.0</code></td>
 <td><code class="docutils literal notranslate">v6.4.4 -> 7.6.0</code></td>
 </tr>
 <tr>
 <td>[MY]</td>
 <td><code class="docutils literal notranslate">v6.0.0 -> 7.6.0</code></td>
 <tr>
 <td>[MV]</td>
 <td><code class="docutils literal notranslate">v6.4.0 -> v6.4.0</code></td>
 <td><code class="docutils literal notranslate">v6.4.4 -> 7.6.0</code></td>
 </tr>
 <tr>
 <td>[ML]</td>
 <td><code class="docutils literal notranslate">v7.0.0 -> 7.6.0</code></td>
 </tr>
 <tr>
 <td>[MT]</td>
 <td><code class="docutils literal notranslate">v6.0.0 -> 7.6.0</code></td>
 <tr>
 <td>[MH]</td>
 <td><code class="docutils literal notranslate">v7.0.0 -> 7.6.0</code></td>
 </tr>
 <tr>
 <td>[MQ]</td>
 <td><code class="docutils literal notranslate">v7.0.0 -> 7.6.0</code></td>
 </tr>
 <tr>
 <td>[MR]</td>
 <td><code class="docutils literal notranslate">v7.0.0 -> 7.6.0</code></td>
 </tr>
 <tr>
 <td>[MU]</td>
 <td><code class="docutils literal notranslate">v7.0.0 -> 7.6.0</code></td>
 </tr>
 <tr>
 <td>[YT]</td>
 <td><code class="docutils literal notranslate">v7.0.0 -> 7.6.0</code></td>
 </tr>
 <tr>
 <td>[MX]</td>
 <td><code class="docutils literal notranslate">v6.0.0 -> 7.6.0</code></td>
 <tr>
 <td>[FM]</td>
 <td><code class="docutils literal notranslate">v6.4.0 -> v6.4.0</code></td>
 <td><code class="docutils literal notranslate">v6.4.4 -> 7.6.0</code></td>
 </tr>
 <tr>
 <td>[MD]</td>
 <td><code class="docutils literal notranslate">v7.0.0 -> 7.6.0</code></td>
 </tr>
 <tr>
 <td>[MC]</td>
 <td><code class="docutils literal notranslate">v6.0.0 -> 7.6.0</code></td>
 <tr>
 <td>[MN]</td>
 <td><code class="docutils literal notranslate">v7.0.8 -> v7.0.12</code></td>
 <td><code class="docutils literal notranslate">v7.2.4 -> 7.6.0</code></td>
 </tr>
 <tr>
 <td>[MA]</td>
 <td><code class="docutils literal notranslate">v6.0.0 -> 7.6.0</code></td>
 <tr>
 <td>[MZ]</td>
 <td><code class="docutils literal notranslate">v6.0.0 -> 7.6.0</code></td>
 <tr>
 <td>[MM]</td>
 <td><code class="docutils literal notranslate">v6.0.0 -> 7.6.0</code></td>
 <tr>
 <td>[NA]</td>
 <td><code class="docutils literal notranslate">v6.0.0 -> 7.6.0</code></td>
 <tr>
 <td>[NP]</td>
 <td><code class="docutils literal notranslate">v6.0.0 -> 7.6.0</code></td>
 <tr>
 <td>[NL]</td>
 <td><code class="docutils literal notranslate">v6.0.0 -> 7.6.0</code></td>
 <tr>
 <td>[AN]</td>
 <td><code class="docutils literal notranslate">v6.0.0 -> 7.6.0</code></td>
 <tr>
 <td>[AW]</td>
 <td><code class="docutils literal notranslate">v6.0.0 -> 7.6.0</code></td>
 <tr>
 <td>[NZ]</td>
 <td><code class="docutils literal notranslate">v6.0.0 -> 7.6.0</code></td>
 <tr>
 <td>[NI]</td>
 <td><code class="docutils literal notranslate">v7.0.0 -> 7.6.0</code></td>
 </tr>
 <tr>
 <td>[NE]</td>
 <td><code class="docutils literal notranslate">v7.0.0 -> 7.6.0</code></td>
 </tr>
 <tr>
 <td>[NG]</td>
 <td><code class="docutils literal notranslate">v7.4.1 -> 7.6.0</code></td>
 </tr>
 <tr>
 <td>[NO]</td>
 <td><code class="docutils literal notranslate">v6.0.0 -> 7.6.0</code></td>
 <tr>
 <td>[MP]</td>
 <td><code class="docutils literal notranslate">v7.0.0 -> 7.6.0</code></td>
 </tr>
 <tr>
 <td>[OM]</td>
 <td><code class="docutils literal notranslate">v6.0.0 -> 7.6.0</code></td>
 <tr>
 <td>[PK]</td>
 <td><code class="docutils literal notranslate">v6.0.0 -> 7.6.0</code></td>
 <tr>
 <td>[PW]</td>
 <td><code class="docutils literal notranslate">v7.0.0 -> 7.6.0</code></td>
 </tr>
 <tr>
 <td>[PA]</td>
 <td><code class="docutils literal notranslate">v6.0.0 -> 7.6.0</code></td>
 <tr>
 <td>[PG]</td>
 <td><code class="docutils literal notranslate">v6.0.0 -> 7.6.0</code></td>
 <tr>
 <td>[PY]</td>
 <td><code class="docutils literal notranslate">v6.0.0 -> 7.6.0</code></td>
 <tr>
 <td>[PE]</td>
 <td><code class="docutils literal notranslate">v6.0.0 -> 7.6.0</code></td>
 <tr>
 <td>[PH]</td>
 <td><code class="docutils literal notranslate">v6.0.0 -> 7.6.0</code></td>
 <tr>
 <td>[PL]</td>
 <td><code class="docutils literal notranslate">v6.0.0 -> 7.6.0</code></td>
 <tr>
 <td>[PT]</td>
 <td><code class="docutils literal notranslate">v6.0.0 -> 7.6.0</code></td>
 <tr>
 <td>[PR]</td>
 <td><code class="docutils literal notranslate">v6.0.0 -> 7.6.0</code></td>
 <tr>
 <td>[QA]</td>
 <td><code class="docutils literal notranslate">v6.0.0 -> 7.6.0</code></td>
 <tr>
 <td>[RE]</td>
 <td><code class="docutils literal notranslate">v7.0.0 -> 7.6.0</code></td>
 </tr>
 <tr>
 <td>[RO]</td>
 <td><code class="docutils literal notranslate">v6.0.0 -> 7.6.0</code></td>
 <tr>
 <td>[RU]</td>
 <td><code class="docutils literal notranslate">v6.0.0 -> 7.6.0</code></td>
 <tr>
 <td>[RW]</td>
 <td><code class="docutils literal notranslate">v6.0.0 -> 7.6.0</code></td>
 <tr>
 <td>[BL]</td>
 <td><code class="docutils literal notranslate">v7.0.0 -> 7.6.0</code></td>
 </tr>
 <tr>
 <td>[KN]</td>
 <td><code class="docutils literal notranslate">v6.4.0 -> v6.4.0</code></td>
 <td><code class="docutils literal notranslate">v6.4.4 -> 7.6.0</code></td>
 </tr>
 <tr>
 <td>[LC]</td>
 <td><code class="docutils literal notranslate">v6.4.0 -> v6.4.0</code></td>
 <td><code class="docutils literal notranslate">v6.4.4 -> 7.6.0</code></td>
 </tr>
 <tr>
 <td>[MF]</td>
 <td><code class="docutils literal notranslate">v7.0.0 -> 7.6.0</code></td>
 </tr>
 <tr>
 <td>[PM]</td>
 <td><code class="docutils literal notranslate">v7.0.0 -> 7.6.0</code></td>
 </tr>
 <tr>
 <td>[VC]</td>
 <td><code class="docutils literal notranslate">v6.4.0 -> v6.4.0</code></td>
 <td><code class="docutils literal notranslate">v6.4.4 -> 7.6.0</code></td>
 </tr>
 <tr>
 <td>[SA]</td>
 <td><code class="docutils literal notranslate">v6.0.0 -> 7.6.0</code></td>
 <tr>
 <td>[SN]</td>
 <td><code class="docutils literal notranslate">v6.4.0 -> v6.4.0</code></td>
 <td><code class="docutils literal notranslate">v6.4.4 -> 7.6.0</code></td>
 </tr>
 <tr>
 <td>[RS]</td>
 <td><code class="docutils literal notranslate">v6.0.0 -> 7.6.0</code></td>
 <tr>
 <td>[ME]</td>
 <td><code class="docutils literal notranslate">v6.0.0 -> 7.6.0</code></td>
 <tr>
 <td>[SL]</td>
 <td><code class="docutils literal notranslate">v7.0.0 -> 7.6.0</code></td>
 </tr>
 <tr>
 <td>[SG]</td>
 <td><code class="docutils literal notranslate">v6.0.0 -> 7.6.0</code></td>
 <tr>
 <td>[SK]</td>
 <td><code class="docutils literal notranslate">v6.0.0 -> 7.6.0</code></td>
 <tr>
 <td>[SI]</td>
 <td><code class="docutils literal notranslate">v6.0.0 -> 7.6.0</code></td>
 <tr>
 <td>[SO]</td>
 <td><code class="docutils literal notranslate">v7.4.1 -> 7.6.0</code></td>
 </tr>
 <tr>
 <td>[ZA]</td>
 <td><code class="docutils literal notranslate">v6.0.0 -> 7.6.0</code></td>
 <tr>
 <td>[ES]</td>
 <td><code class="docutils literal notranslate">v6.0.0 -> 7.6.0</code></td>
 <tr>
 <td>[LK]</td>
 <td><code class="docutils literal notranslate">v6.0.0 -> 7.6.0</code></td>
 <tr>
 <td>[SR]</td>
 <td><code class="docutils literal notranslate">v7.0.0 -> 7.6.0</code></td>
 </tr>
 <tr>
 <td>[SZ]</td>
 <td><code class="docutils literal notranslate">v7.4.1 -> 7.6.0</code></td>
 </tr>
 <tr>
 <td>[SE]</td>
 <td><code class="docutils literal notranslate">v6.0.0 -> 7.6.0</code></td>
 <tr>
 <td>[CH]</td>
 <td><code class="docutils literal notranslate">v6.0.0 -> 7.6.0</code></td>
 <tr>
 <td>[TW]</td>
 <td><code class="docutils literal notranslate">v6.0.0 -> 7.6.0</code></td>
 <tr>
 <td>[TZ]</td>
 <td><code class="docutils literal notranslate">v6.0.0 -> 7.6.0</code></td>
 <tr>
 <td>[TH]</td>
 <td><code class="docutils literal notranslate">v6.0.0 -> 7.6.0</code></td>
 <tr>
 <td>[TG]</td>
 <td><code class="docutils literal notranslate">v7.0.0 -> 7.6.0</code></td>
 </tr>
 <tr>
 <td>[TT]</td>
 <td><code class="docutils literal notranslate">v6.0.0 -> 7.6.0</code></td>
 <tr>
 <td>[TN]</td>
 <td><code class="docutils literal notranslate">v6.0.0 -> 7.6.0</code></td>
 <tr>
 <td>[TR]</td>
 <td><code class="docutils literal notranslate">v6.0.0 -> 7.6.0</code></td>
 <tr>
 <td>[TM]</td>
 <td><code class="docutils literal notranslate">v6.4.0 -> v6.4.0</code></td>
 <td><code class="docutils literal notranslate">v6.4.4 -> 7.6.0</code></td>
 </tr>
 <tr>
 <td>[AE]</td>
 <td><code class="docutils literal notranslate">v6.0.0 -> 7.6.0</code></td>
 <tr>
 <td>[TC]</td>
 <td><code class="docutils literal notranslate">v6.4.0 -> v6.4.0</code></td>
 <td><code class="docutils literal notranslate">v6.4.4 -> 7.6.0</code></td>
 </tr>
 <tr>
 <td>[UG]</td>
 <td><code class="docutils literal notranslate">v6.4.0 -> v6.4.0</code></td>
 <td><code class="docutils literal notranslate">v6.4.4 -> 7.6.0</code></td>
 </tr>
 <tr>
 <td>[UA]</td>
 <td><code class="docutils literal notranslate">v6.0.0 -> 7.6.0</code></td>
 <tr>
 <td>[GB]</td>
 <td><code class="docutils literal notranslate">v6.0.0 -> 7.6.0</code></td>
 <tr>
 <td>[US]</td>
 <td><code class="docutils literal notranslate">v6.0.0 -> 7.6.0</code></td>
 <tr>
 <td>[PS]</td>
 <td><code class="docutils literal notranslate">v6.0.0 -> 7.6.0</code></td>
 <tr>
 <td>[UY]</td>
 <td><code class="docutils literal notranslate">v6.0.0 -> 7.6.0</code></td>
 <tr>
 <td>[UZ]</td>
 <td><code class="docutils literal notranslate">v6.0.0 -> 7.6.0</code></td>
 <tr>
 <td>[VU]</td>
 <td><code class="docutils literal notranslate">v6.4.0 -> v6.4.0</code></td>
 <td><code class="docutils literal notranslate">v6.4.4 -> 7.6.0</code></td>
 </tr>
 <tr>
 <td>[VE]</td>
 <td><code class="docutils literal notranslate">v6.0.0 -> 7.6.0</code></td>
 <tr>
 <td>[VN]</td>
 <td><code class="docutils literal notranslate">v6.0.0 -> 7.6.0</code></td>
 <tr>
 <td>[VI]</td>
 <td><code class="docutils literal notranslate">v7.0.0 -> 7.6.0</code></td>
 </tr>
 <tr>
 <td>[WF]</td>
 <td><code class="docutils literal notranslate">v7.0.0 -> 7.6.0</code></td>
 </tr>
 <tr>
 <td>[YE]</td>
 <td><code class="docutils literal notranslate">v6.0.0 -> 7.6.0</code></td>
 <tr>
 <td>[ZM]</td>
 <td><code class="docutils literal notranslate">v7.0.0 -> 7.6.0</code></td>
 </tr>
 <tr>
 <td>[ZW]</td>
 <td><code class="docutils literal notranslate">v6.0.0 -> 7.6.0</code></td>
 <tr>
 <td>[JP]</td>
 <td><code class="docutils literal notranslate">v6.0.0 -> 7.6.0</code></td>
 <tr>
 <td>[CA]</td>
 <td><code class="docutils literal notranslate">v6.0.0 -> 7.6.0</code></td>
 <tr>
 <td>[IR]</td>
 <td><code class="docutils literal notranslate">v6.0.0 -> v6.4.4</code></td>
 </tr>
 <tr>
 <td>[KP]</td>
 <td><code class="docutils literal notranslate">v6.0.0 -> v6.4.4</code></td>
 </tr>
 <tr>
 <td>[SD]</td>
 <td><code class="docutils literal notranslate">v6.0.0 -> v6.4.4</code></td>
 </tr>
 <tr>
 <td>[SY]</td>
 <td><code class="docutils literal notranslate">v6.0.0 -> v6.4.4</code></td>
 </tr>
 <tr>
 <td>[ZB]</td>
 <td><code class="docutils literal notranslate">v6.0.0 -> v6.4.4</code></td>
 </tr>
 </table>
 </div>
 </li>
        <li> <span class="li-head">darrp_optimize</span> - Time for running Distributed Automatic Radio Resource Provisioning (DARRP) optimizations (0 - 86400 sec). <span class="li-normal">type: int</span>
 <a id='label6' href="javascript:ContentClick('label7', 'label6');" onmouseover="ContentPreview('label7');" onmouseout="ContentUnpreview('label7');" title="click to collapse or expand..."> more... </a>
 <div id="label7" style="display:none">
 <table border="1">
 <tr>
 <td></td>
 <td colspan="1">Supported Version Ranges</td>
 </tr>
 <tr>
 <td>darrp_optimize</td>
 <td><code class="docutils literal notranslate">v6.2.0 -> 7.6.0 </code></td>
 </tr>
 </table>
 </div>
 </li>
        <li> <span class="li-head">darrp_optimize_schedules</span> - Firewall schedules for DARRP running time. DARRP will run periodically based on darrp-optimize within the schedules. Separate multiple schedule names with a space. <span class="li-normal">type: list</span> <span style="font-family:'Courier New'" class="li-required">member_path: darrp_optimize_schedules:name</span>
 <a id='label8' href="javascript:ContentClick('label9', 'label8');" onmouseover="ContentPreview('label9');" onmouseout="ContentUnpreview('label9');" title="click to collapse or expand..."> more... </a>
 <div id="label9" style="display:none">
 <table border="1">
 <tr>
 <td></td><td colspan="1">Supported Version Ranges</td>
 </tr>
 <tr>
 <td>darrp_optimize_schedules</td>
 <td><code class="docutils literal notranslate">v6.2.0 -> 7.6.0 </code></td>
 </tr>
 </table>
 </div>
 </li>
            <ul class="ul-self">
            <li> <span class="li-head">name</span> - Schedule name. Source firewall.schedule.group.name firewall.schedule.recurring.name firewall.schedule.onetime.name. <span class="li-normal">type: str</span> <span class="li-required">required: true</span>
 <a id='label10' href="javascript:ContentClick('label11', 'label10');" onmouseover="ContentPreview('label11');" onmouseout="ContentUnpreview('label11');" title="click to collapse or expand..."> more... </a>
 <div id="label11" style="display:none">
 <table border="1">
 <tr>
 <td></td>
 <td colspan="1">Supported Version Ranges</td>
 </tr>
 <tr>
 <td>name</td>
 <td><code class="docutils literal notranslate">v6.2.0 -> 7.6.0 </code></td>
 </tr>
 </table>
 </div>
 </li>
            </ul>
        <li> <span class="li-head">device_holdoff</span> - Lower limit of creation time of device for identification in minutes (0 - 60). <span class="li-normal">type: int</span>
 <a id='label12' href="javascript:ContentClick('label13', 'label12');" onmouseover="ContentPreview('label13');" onmouseout="ContentUnpreview('label13');" title="click to collapse or expand..."> more... </a>
 <div id="label13" style="display:none">
 <table border="1">
 <tr>
 <td></td>
 <td colspan="2">Supported Version Ranges</td>
 </tr>
 <tr>
 <td>device_holdoff</td>
 <td><code class="docutils literal notranslate">v6.4.0 -> v6.4.0 </code></td>
 <td><code class="docutils literal notranslate">v6.4.4 -> 7.6.0 </code></td>
 </tr>
 </table>
 </div>
 </li>
        <li> <span class="li-head">device_idle</span> - Upper limit of idle time of device for identification in minutes (0 - 14400). <span class="li-normal">type: int</span>
 <a id='label14' href="javascript:ContentClick('label15', 'label14');" onmouseover="ContentPreview('label15');" onmouseout="ContentUnpreview('label15');" title="click to collapse or expand..."> more... </a>
 <div id="label15" style="display:none">
 <table border="1">
 <tr>
 <td></td>
 <td colspan="2">Supported Version Ranges</td>
 </tr>
 <tr>
 <td>device_idle</td>
 <td><code class="docutils literal notranslate">v6.4.0 -> v6.4.0 </code></td>
 <td><code class="docutils literal notranslate">v6.4.4 -> 7.6.0 </code></td>
 </tr>
 </table>
 </div>
 </li>
        <li> <span class="li-head">device_weight</span> - Upper limit of confidence of device for identification (0 - 255). <span class="li-normal">type: int</span>
 <a id='label16' href="javascript:ContentClick('label17', 'label16');" onmouseover="ContentPreview('label17');" onmouseout="ContentUnpreview('label17');" title="click to collapse or expand..."> more... </a>
 <div id="label17" style="display:none">
 <table border="1">
 <tr>
 <td></td>
 <td colspan="2">Supported Version Ranges</td>
 </tr>
 <tr>
 <td>device_weight</td>
 <td><code class="docutils literal notranslate">v6.4.0 -> v6.4.0 </code></td>
 <td><code class="docutils literal notranslate">v6.4.4 -> 7.6.0 </code></td>
 </tr>
 </table>
 </div>
 </li>
        <li> <span class="li-head">duplicate_ssid</span> - Enable/disable allowing Virtual Access Points (VAPs) to use the same SSID name in the same VDOM. <span class="li-normal">type: str</span> <span class="li-normal">choices: enable, disable</span>
 <a id='label18' href="javascript:ContentClick('label19', 'label18');" onmouseover="ContentPreview('label19');" onmouseout="ContentUnpreview('label19');" title="click to collapse or expand..."> more... </a>
 <div id="label19" style="display:none">
 <table border="1">
 <tr>
 <td></td>
 <td colspan="1">Supported Version Ranges</td>
 </tr>
 <tr>
 <td>duplicate_ssid</td>
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
        <li> <span class="li-head">fake_ssid_action</span> - Actions taken for detected fake SSID. <span class="li-normal">type: list</span> <span class="li-normal">choices: log, suppress</span>
 <a id='label20' href="javascript:ContentClick('label21', 'label20');" onmouseover="ContentPreview('label21');" onmouseout="ContentUnpreview('label21');" title="click to collapse or expand..."> more... </a>
 <div id="label21" style="display:none">
 <table border="1">
 <tr>
 <td></td>
 <td colspan="1">Supported Version Ranges</td>
 </tr>
 <tr>
 <td>fake_ssid_action</td>
 <td><code class="docutils literal notranslate">v6.2.0 -> 7.6.0 </code></td>
 </tr>
 <tr>
 <td>[log]</td>
 <td><code class="docutils literal notranslate">v6.2.0 -> 7.6.0</code></td>
 <tr>
 <td>[suppress]</td>
 <td><code class="docutils literal notranslate">v6.2.0 -> 7.6.0</code></td>
 </table>
 </div>
 </li>
        <li> <span class="li-head">fapc_compatibility</span> - Enable/disable FAP-C series compatibility. <span class="li-normal">type: str</span> <span class="li-normal">choices: enable, disable</span>
 <a id='label22' href="javascript:ContentClick('label23', 'label22');" onmouseover="ContentPreview('label23');" onmouseout="ContentUnpreview('label23');" title="click to collapse or expand..."> more... </a>
 <div id="label23" style="display:none">
 <table border="1">
 <tr>
 <td></td>
 <td colspan="1">Supported Version Ranges</td>
 </tr>
 <tr>
 <td>fapc_compatibility</td>
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
        <li> <span class="li-head">firmware_provision_on_authorization</span> - Enable/disable automatic provisioning of latest firmware on authorization. <span class="li-normal">type: str</span> <span class="li-normal">choices: enable, disable</span>
 <a id='label24' href="javascript:ContentClick('label25', 'label24');" onmouseover="ContentPreview('label25');" onmouseout="ContentUnpreview('label25');" title="click to collapse or expand..."> more... </a>
 <div id="label25" style="display:none">
 <table border="1">
 <tr>
 <td></td>
 <td colspan="1">Supported Version Ranges</td>
 </tr>
 <tr>
 <td>firmware_provision_on_authorization</td>
 <td><code class="docutils literal notranslate">v7.0.2 -> 7.6.0 </code></td>
 </tr>
 <tr>
 <td>[enable]</td>
 <td><code class="docutils literal notranslate">v7.0.2 -> 7.6.0</code></td>
 <tr>
 <td>[disable]</td>
 <td><code class="docutils literal notranslate">v7.0.2 -> 7.6.0</code></td>
 </table>
 </div>
 </li>
        <li> <span class="li-head">offending_ssid</span> - Configure offending SSID. <span class="li-normal">type: list</span> <span style="font-family:'Courier New'" class="li-required">member_path: offending_ssid:id</span>
 <a id='label26' href="javascript:ContentClick('label27', 'label26');" onmouseover="ContentPreview('label27');" onmouseout="ContentUnpreview('label27');" title="click to collapse or expand..."> more... </a>
 <div id="label27" style="display:none">
 <table border="1">
 <tr>
 <td></td><td colspan="1">Supported Version Ranges</td>
 </tr>
 <tr>
 <td>offending_ssid</td>
 <td><code class="docutils literal notranslate">v6.2.0 -> 7.6.0 </code></td>
 </tr>
 </table>
 </div>
 </li>
            <ul class="ul-self">
            <li> <span class="li-head">action</span> - Actions taken for detected offending SSID. <span class="li-normal">type: list</span> <span class="li-normal">choices: log, suppress</span>
 <a id='label28' href="javascript:ContentClick('label29', 'label28');" onmouseover="ContentPreview('label29');" onmouseout="ContentUnpreview('label29');" title="click to collapse or expand..."> more... </a>
 <div id="label29" style="display:none">
 <table border="1">
 <tr>
 <td></td>
 <td colspan="1">Supported Version Ranges</td>
 </tr>
 <tr>
 <td>action</td>
 <td><code class="docutils literal notranslate">v6.2.0 -> 7.6.0 </code></td>
 </tr>
 <tr>
 <td>[log]</td>
 <td><code class="docutils literal notranslate">v6.2.0 -> 7.6.0</code></td>
 <tr>
 <td>[suppress]</td>
 <td><code class="docutils literal notranslate">v6.2.0 -> 7.6.0</code></td>
 </table>
 </div>
 </li>
            <li> <span class="li-head">id</span> - ID. see <a href='#notes'>Notes</a>. <span class="li-normal">type: int</span> <span class="li-required">required: true</span>
 <a id='label30' href="javascript:ContentClick('label31', 'label30');" onmouseover="ContentPreview('label31');" onmouseout="ContentUnpreview('label31');" title="click to collapse or expand..."> more... </a>
 <div id="label31" style="display:none">
 <table border="1">
 <tr>
 <td></td>
 <td colspan="1">Supported Version Ranges</td>
 </tr>
 <tr>
 <td>id</td>
 <td><code class="docutils literal notranslate">v6.2.0 -> 7.6.0 </code></td>
 </tr>
 </table>
 </div>
 </li>
            <li> <span class="li-head">ssid_pattern</span> - Define offending SSID pattern (case insensitive). For example, word, word*, *word, wo*rd. <span class="li-normal">type: str</span>
 <a id='label32' href="javascript:ContentClick('label33', 'label32');" onmouseover="ContentPreview('label33');" onmouseout="ContentUnpreview('label33');" title="click to collapse or expand..."> more... </a>
 <div id="label33" style="display:none">
 <table border="1">
 <tr>
 <td></td>
 <td colspan="1">Supported Version Ranges</td>
 </tr>
 <tr>
 <td>ssid_pattern</td>
 <td><code class="docutils literal notranslate">v6.2.0 -> 7.6.0 </code></td>
 </tr>
 </table>
 </div>
 </li>
            </ul>
        <li> <span class="li-head">phishing_ssid_detect</span> - Enable/disable phishing SSID detection. <span class="li-normal">type: str</span> <span class="li-normal">choices: enable, disable</span>
 <a id='label34' href="javascript:ContentClick('label35', 'label34');" onmouseover="ContentPreview('label35');" onmouseout="ContentUnpreview('label35');" title="click to collapse or expand..."> more... </a>
 <div id="label35" style="display:none">
 <table border="1">
 <tr>
 <td></td>
 <td colspan="1">Supported Version Ranges</td>
 </tr>
 <tr>
 <td>phishing_ssid_detect</td>
 <td><code class="docutils literal notranslate">v6.2.0 -> 7.6.0 </code></td>
 </tr>
 <tr>
 <td>[enable]</td>
 <td><code class="docutils literal notranslate">v6.2.0 -> 7.6.0</code></td>
 <tr>
 <td>[disable]</td>
 <td><code class="docutils literal notranslate">v6.2.0 -> 7.6.0</code></td>
 </table>
 </div>
 </li>
        <li> <span class="li-head">rolling_wtp_upgrade</span> - Enable/disable rolling WTP upgrade . <span class="li-normal">type: str</span> <span class="li-normal">choices: enable, disable</span>
 <a id='label36' href="javascript:ContentClick('label37', 'label36');" onmouseover="ContentPreview('label37');" onmouseout="ContentUnpreview('label37');" title="click to collapse or expand..."> more... </a>
 <div id="label37" style="display:none">
 <table border="1">
 <tr>
 <td></td>
 <td colspan="1">Supported Version Ranges</td>
 </tr>
 <tr>
 <td>rolling_wtp_upgrade</td>
 <td><code class="docutils literal notranslate">v7.4.2 -> 7.6.0 </code></td>
 </tr>
 <tr>
 <td>[enable]</td>
 <td><code class="docutils literal notranslate">v7.4.2 -> 7.6.0</code></td>
 <tr>
 <td>[disable]</td>
 <td><code class="docutils literal notranslate">v7.4.2 -> 7.6.0</code></td>
 </table>
 </div>
 </li>
        <li> <span class="li-head">wfa_compatibility</span> - Enable/disable WFA compatibility. <span class="li-normal">type: str</span> <span class="li-normal">choices: enable, disable</span>
 <a id='label38' href="javascript:ContentClick('label39', 'label38');" onmouseover="ContentPreview('label39');" onmouseout="ContentUnpreview('label39');" title="click to collapse or expand..."> more... </a>
 <div id="label39" style="display:none">
 <table border="1">
 <tr>
 <td></td>
 <td colspan="1">Supported Version Ranges</td>
 </tr>
 <tr>
 <td>wfa_compatibility</td>
 <td><code class="docutils literal notranslate">v6.2.0 -> 7.6.0 </code></td>
 </tr>
 <tr>
 <td>[enable]</td>
 <td><code class="docutils literal notranslate">v6.2.0 -> 7.6.0</code></td>
 <tr>
 <td>[disable]</td>
 <td><code class="docutils literal notranslate">v6.2.0 -> 7.6.0</code></td>
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
    
    - name: VDOM wireless controller configuration.
      fortinet.fortios.fortios_wireless_controller_setting:
          vdom: "{{ vdom }}"
          wireless_controller_setting:
              account_id: "<your_own_value>"
              country: "--"
              darrp_optimize: "86400"
              darrp_optimize_schedules:
                  -
                      name: "default_name_7 (source firewall.schedule.group.name firewall.schedule.recurring.name firewall.schedule.onetime.name)"
              device_holdoff: "5"
              device_idle: "1440"
              device_weight: "1"
              duplicate_ssid: "enable"
              fake_ssid_action: "log"
              fapc_compatibility: "enable"
              firmware_provision_on_authorization: "enable"
              offending_ssid:
                  -
                      action: "log"
                      id: "17"
                      ssid_pattern: "<your_own_value>"
              phishing_ssid_detect: "enable"
              rolling_wtp_upgrade: "enable"
              wfa_compatibility: "enable"


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
