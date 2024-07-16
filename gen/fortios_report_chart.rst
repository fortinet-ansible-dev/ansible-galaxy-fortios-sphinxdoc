:source: fortios_report_chart.py

:orphan:

.. fortios_report_chart:

fortios_report_chart -- Report chart widget configuration in Fortinet's FortiOS and FortiGate.
++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++

.. versionadded:: 2.0.0

.. contents::
   :local:
   :depth: 1


Synopsis
--------
- This module is able to configure a FortiGate or FortiOS (FOS) device by allowing the user to set and modify report feature and chart category. Examples include all parameters and values need to be adjusted to datasources before usage. Tested with FOS v6.0.0



Requirements
------------
The below requirements are needed on the host that executes this module.

- ansible>=2.15


Tips
----
Using member operation to add an element to an existing object.

FortiOS Version Compatibility
-----------------------------
Supported Version Ranges: v6.0.0 -> v6.4.4


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
    <li> <span class="li-head">report_chart</span> - Report chart widget configuration. <span class="li-normal">type: dict</span>
 <a id='label0' href="javascript:ContentClick('label1', 'label0');" onmouseover="ContentPreview('label1');" onmouseout="ContentUnpreview('label1');" title="click to collapse or expand..."> more... </a>
 <div id="label1" style="display:none">
 <table border="1">
 <tr>
 <td></td><td colspan="1">Supported Version Ranges</td>
 </tr>
 <tr>
 <td>report_chart</td>
 <td><code class="docutils literal notranslate">v6.0.0 -> v6.4.4 </code></td>
 </tr>
 </table>
 </div>
 </li>
        <ul class="ul-self">
        <li> <span class="li-head">background</span> - Chart background. <span class="li-normal">type: str</span>
 <a id='label2' href="javascript:ContentClick('label3', 'label2');" onmouseover="ContentPreview('label3');" onmouseout="ContentUnpreview('label3');" title="click to collapse or expand..."> more... </a>
 <div id="label3" style="display:none">
 <table border="1">
 <tr>
 <td></td>
 <td colspan="1">Supported Version Ranges</td>
 </tr>
 <tr>
 <td>background</td>
 <td><code class="docutils literal notranslate">v6.0.0 -> v6.4.4 </code></td>
 </tr>
 </table>
 </div>
 </li>
        <li> <span class="li-head">category</span> - Category. <span class="li-normal">type: str</span> <span class="li-normal">choices: misc, traffic, event, virus, webfilter, attack, spam, dlp, app-ctrl, vulnerability</span>
 <a id='label4' href="javascript:ContentClick('label5', 'label4');" onmouseover="ContentPreview('label5');" onmouseout="ContentUnpreview('label5');" title="click to collapse or expand..."> more... </a>
 <div id="label5" style="display:none">
 <table border="1">
 <tr>
 <td></td>
 <td colspan="1">Supported Version Ranges</td>
 </tr>
 <tr>
 <td>category</td>
 <td><code class="docutils literal notranslate">v6.0.0 -> v6.4.4 </code></td>
 </tr>
 <tr>
 <td>[misc]</td>
 <td><code class="docutils literal notranslate">v6.0.0 -> v6.4.4</code></td>
 <tr>
 <td>[traffic]</td>
 <td><code class="docutils literal notranslate">v6.0.0 -> v6.4.4</code></td>
 <tr>
 <td>[event]</td>
 <td><code class="docutils literal notranslate">v6.0.0 -> v6.4.4</code></td>
 <tr>
 <td>[virus]</td>
 <td><code class="docutils literal notranslate">v6.0.0 -> v6.4.4</code></td>
 <tr>
 <td>[webfilter]</td>
 <td><code class="docutils literal notranslate">v6.0.0 -> v6.4.4</code></td>
 <tr>
 <td>[attack]</td>
 <td><code class="docutils literal notranslate">v6.0.0 -> v6.4.4</code></td>
 <tr>
 <td>[spam]</td>
 <td><code class="docutils literal notranslate">v6.0.0 -> v6.4.4</code></td>
 <tr>
 <td>[dlp]</td>
 <td><code class="docutils literal notranslate">v6.0.0 -> v6.4.4</code></td>
 <tr>
 <td>[app-ctrl]</td>
 <td><code class="docutils literal notranslate">v6.0.0 -> v6.4.4</code></td>
 <tr>
 <td>[vulnerability]</td>
 <td><code class="docutils literal notranslate">v6.0.0 -> v6.4.4</code></td>
 </table>
 </div>
 </li>
        <li> <span class="li-head">category_series</span> - Category series of pie chart. <span class="li-normal">type: dict</span>
 <a id='label6' href="javascript:ContentClick('label7', 'label6');" onmouseover="ContentPreview('label7');" onmouseout="ContentUnpreview('label7');" title="click to collapse or expand..."> more... </a>
 <div id="label7" style="display:none">
 <table border="1">
 <tr>
 <td></td><td colspan="1">Supported Version Ranges</td>
 </tr>
 <tr>
 <td>category_series</td>
 <td><code class="docutils literal notranslate">v6.0.0 -> v6.4.4 </code></td>
 </tr>
 </table>
 </div>
 </li>
            <ul class="ul-self">
            <li> <span class="li-head">databind</span> - Category series value expression. <span class="li-normal">type: str</span>
 <a id='label8' href="javascript:ContentClick('label9', 'label8');" onmouseover="ContentPreview('label9');" onmouseout="ContentUnpreview('label9');" title="click to collapse or expand..."> more... </a>
 <div id="label9" style="display:none">
 <table border="1">
 <tr>
 <td></td>
 <td colspan="1">Supported Version Ranges</td>
 </tr>
 <tr>
 <td>databind</td>
 <td><code class="docutils literal notranslate">v6.0.0 -> v6.4.4 </code></td>
 </tr>
 </table>
 </div>
 </li>
            <li> <span class="li-head">font_size</span> - Font size of category-series title. <span class="li-normal">type: int</span>
 <a id='label10' href="javascript:ContentClick('label11', 'label10');" onmouseover="ContentPreview('label11');" onmouseout="ContentUnpreview('label11');" title="click to collapse or expand..."> more... </a>
 <div id="label11" style="display:none">
 <table border="1">
 <tr>
 <td></td>
 <td colspan="1">Supported Version Ranges</td>
 </tr>
 <tr>
 <td>font_size</td>
 <td><code class="docutils literal notranslate">v6.0.0 -> v6.4.4 </code></td>
 </tr>
 </table>
 </div>
 </li>
            </ul>
        <li> <span class="li-head">color_palette</span> - Color palette (system will pick color automatically by default). <span class="li-normal">type: str</span>
 <a id='label12' href="javascript:ContentClick('label13', 'label12');" onmouseover="ContentPreview('label13');" onmouseout="ContentUnpreview('label13');" title="click to collapse or expand..."> more... </a>
 <div id="label13" style="display:none">
 <table border="1">
 <tr>
 <td></td>
 <td colspan="1">Supported Version Ranges</td>
 </tr>
 <tr>
 <td>color_palette</td>
 <td><code class="docutils literal notranslate">v6.0.0 -> v6.4.4 </code></td>
 </tr>
 </table>
 </div>
 </li>
        <li> <span class="li-head">column</span> - Table column definition. <span class="li-normal">type: list</span> <span style="font-family:'Courier New'" class="li-required">member_path: column:id</span>
 <a id='label14' href="javascript:ContentClick('label15', 'label14');" onmouseover="ContentPreview('label15');" onmouseout="ContentUnpreview('label15');" title="click to collapse or expand..."> more... </a>
 <div id="label15" style="display:none">
 <table border="1">
 <tr>
 <td></td><td colspan="1">Supported Version Ranges</td>
 </tr>
 <tr>
 <td>column</td>
 <td><code class="docutils literal notranslate">v6.0.0 -> v6.4.4 </code></td>
 </tr>
 </table>
 </div>
 </li>
            <ul class="ul-self">
            <li> <span class="li-head">detail_unit</span> - Detail unit of column. <span class="li-normal">type: str</span>
 <a id='label16' href="javascript:ContentClick('label17', 'label16');" onmouseover="ContentPreview('label17');" onmouseout="ContentUnpreview('label17');" title="click to collapse or expand..."> more... </a>
 <div id="label17" style="display:none">
 <table border="1">
 <tr>
 <td></td>
 <td colspan="1">Supported Version Ranges</td>
 </tr>
 <tr>
 <td>detail_unit</td>
 <td><code class="docutils literal notranslate">v6.0.0 -> v6.4.4 </code></td>
 </tr>
 </table>
 </div>
 </li>
            <li> <span class="li-head">detail_value</span> - Detail value of column. <span class="li-normal">type: str</span>
 <a id='label18' href="javascript:ContentClick('label19', 'label18');" onmouseover="ContentPreview('label19');" onmouseout="ContentUnpreview('label19');" title="click to collapse or expand..."> more... </a>
 <div id="label19" style="display:none">
 <table border="1">
 <tr>
 <td></td>
 <td colspan="1">Supported Version Ranges</td>
 </tr>
 <tr>
 <td>detail_value</td>
 <td><code class="docutils literal notranslate">v6.0.0 -> v6.4.4 </code></td>
 </tr>
 </table>
 </div>
 </li>
            <li> <span class="li-head">footer_unit</span> - Footer unit of column. <span class="li-normal">type: str</span>
 <a id='label20' href="javascript:ContentClick('label21', 'label20');" onmouseover="ContentPreview('label21');" onmouseout="ContentUnpreview('label21');" title="click to collapse or expand..."> more... </a>
 <div id="label21" style="display:none">
 <table border="1">
 <tr>
 <td></td>
 <td colspan="1">Supported Version Ranges</td>
 </tr>
 <tr>
 <td>footer_unit</td>
 <td><code class="docutils literal notranslate">v6.0.0 -> v6.4.4 </code></td>
 </tr>
 </table>
 </div>
 </li>
            <li> <span class="li-head">footer_value</span> - Footer value of column. <span class="li-normal">type: str</span>
 <a id='label22' href="javascript:ContentClick('label23', 'label22');" onmouseover="ContentPreview('label23');" onmouseout="ContentUnpreview('label23');" title="click to collapse or expand..."> more... </a>
 <div id="label23" style="display:none">
 <table border="1">
 <tr>
 <td></td>
 <td colspan="1">Supported Version Ranges</td>
 </tr>
 <tr>
 <td>footer_value</td>
 <td><code class="docutils literal notranslate">v6.0.0 -> v6.4.4 </code></td>
 </tr>
 </table>
 </div>
 </li>
            <li> <span class="li-head">header_value</span> - Display name of table header. <span class="li-normal">type: str</span>
 <a id='label24' href="javascript:ContentClick('label25', 'label24');" onmouseover="ContentPreview('label25');" onmouseout="ContentUnpreview('label25');" title="click to collapse or expand..."> more... </a>
 <div id="label25" style="display:none">
 <table border="1">
 <tr>
 <td></td>
 <td colspan="1">Supported Version Ranges</td>
 </tr>
 <tr>
 <td>header_value</td>
 <td><code class="docutils literal notranslate">v6.0.0 -> v6.4.4 </code></td>
 </tr>
 </table>
 </div>
 </li>
            <li> <span class="li-head">id</span> - ID. see <a href='#notes'>Notes</a>. <span class="li-normal">type: int</span> <span class="li-required">required: true</span>
 <a id='label26' href="javascript:ContentClick('label27', 'label26');" onmouseover="ContentPreview('label27');" onmouseout="ContentUnpreview('label27');" title="click to collapse or expand..."> more... </a>
 <div id="label27" style="display:none">
 <table border="1">
 <tr>
 <td></td>
 <td colspan="1">Supported Version Ranges</td>
 </tr>
 <tr>
 <td>id</td>
 <td><code class="docutils literal notranslate">v6.0.0 -> v6.4.4 </code></td>
 </tr>
 </table>
 </div>
 </li>
            <li> <span class="li-head">mapping</span> - Show detail in certain display value for certain condition. <span class="li-normal">type: list</span> <span style="font-family:'Courier New'" class="li-required">member_path: column:id/mapping:id</span>
 <a id='label28' href="javascript:ContentClick('label29', 'label28');" onmouseover="ContentPreview('label29');" onmouseout="ContentUnpreview('label29');" title="click to collapse or expand..."> more... </a>
 <div id="label29" style="display:none">
 <table border="1">
 <tr>
 <td></td><td colspan="1">Supported Version Ranges</td>
 </tr>
 <tr>
 <td>mapping</td>
 <td><code class="docutils literal notranslate">v6.0.0 -> v6.4.4 </code></td>
 </tr>
 </table>
 </div>
 </li>
                <ul class="ul-self">
                <li> <span class="li-head">displayname</span> - Display name. <span class="li-normal">type: str</span>
 <a id='label30' href="javascript:ContentClick('label31', 'label30');" onmouseover="ContentPreview('label31');" onmouseout="ContentUnpreview('label31');" title="click to collapse or expand..."> more... </a>
 <div id="label31" style="display:none">
 <table border="1">
 <tr>
 <td></td>
 <td colspan="1">Supported Version Ranges</td>
 </tr>
 <tr>
 <td>displayname</td>
 <td><code class="docutils literal notranslate">v6.0.0 -> v6.4.4 </code></td>
 </tr>
 </table>
 </div>
 </li>
                <li> <span class="li-head">id</span> - id see <a href='#notes'>Notes</a>. <span class="li-normal">type: int</span> <span class="li-required">required: true</span>
 <a id='label32' href="javascript:ContentClick('label33', 'label32');" onmouseover="ContentPreview('label33');" onmouseout="ContentUnpreview('label33');" title="click to collapse or expand..."> more... </a>
 <div id="label33" style="display:none">
 <table border="1">
 <tr>
 <td></td>
 <td colspan="1">Supported Version Ranges</td>
 </tr>
 <tr>
 <td>id</td>
 <td><code class="docutils literal notranslate">v6.0.0 -> v6.4.4 </code></td>
 </tr>
 </table>
 </div>
 </li>
                <li> <span class="li-head">op</span> - Comparision operater. <span class="li-normal">type: str</span> <span class="li-normal">choices: none, greater, greater-equal, less, less-equal, equal, between</span>
 <a id='label34' href="javascript:ContentClick('label35', 'label34');" onmouseover="ContentPreview('label35');" onmouseout="ContentUnpreview('label35');" title="click to collapse or expand..."> more... </a>
 <div id="label35" style="display:none">
 <table border="1">
 <tr>
 <td></td>
 <td colspan="1">Supported Version Ranges</td>
 </tr>
 <tr>
 <td>op</td>
 <td><code class="docutils literal notranslate">v6.0.0 -> v6.4.4 </code></td>
 </tr>
 <tr>
 <td>[none]</td>
 <td><code class="docutils literal notranslate">v6.0.0 -> v6.4.4</code></td>
 <tr>
 <td>[greater]</td>
 <td><code class="docutils literal notranslate">v6.0.0 -> v6.4.4</code></td>
 <tr>
 <td>[greater-equal]</td>
 <td><code class="docutils literal notranslate">v6.0.0 -> v6.4.4</code></td>
 <tr>
 <td>[less]</td>
 <td><code class="docutils literal notranslate">v6.0.0 -> v6.4.4</code></td>
 <tr>
 <td>[less-equal]</td>
 <td><code class="docutils literal notranslate">v6.0.0 -> v6.4.4</code></td>
 <tr>
 <td>[equal]</td>
 <td><code class="docutils literal notranslate">v6.0.0 -> v6.4.4</code></td>
 <tr>
 <td>[between]</td>
 <td><code class="docutils literal notranslate">v6.0.0 -> v6.4.4</code></td>
 </table>
 </div>
 </li>
                <li> <span class="li-head">value_type</span> - Value type. <span class="li-normal">type: str</span> <span class="li-normal">choices: integer, string</span>
 <a id='label36' href="javascript:ContentClick('label37', 'label36');" onmouseover="ContentPreview('label37');" onmouseout="ContentUnpreview('label37');" title="click to collapse or expand..."> more... </a>
 <div id="label37" style="display:none">
 <table border="1">
 <tr>
 <td></td>
 <td colspan="1">Supported Version Ranges</td>
 </tr>
 <tr>
 <td>value_type</td>
 <td><code class="docutils literal notranslate">v6.0.0 -> v6.4.4 </code></td>
 </tr>
 <tr>
 <td>[integer]</td>
 <td><code class="docutils literal notranslate">v6.0.0 -> v6.4.4</code></td>
 <tr>
 <td>[string]</td>
 <td><code class="docutils literal notranslate">v6.0.0 -> v6.4.4</code></td>
 </table>
 </div>
 </li>
                <li> <span class="li-head">value1</span> - Value 1. <span class="li-normal">type: str</span>
 <a id='label38' href="javascript:ContentClick('label39', 'label38');" onmouseover="ContentPreview('label39');" onmouseout="ContentUnpreview('label39');" title="click to collapse or expand..."> more... </a>
 <div id="label39" style="display:none">
 <table border="1">
 <tr>
 <td></td>
 <td colspan="1">Supported Version Ranges</td>
 </tr>
 <tr>
 <td>value1</td>
 <td><code class="docutils literal notranslate">v6.0.0 -> v6.4.4 </code></td>
 </tr>
 </table>
 </div>
 </li>
                <li> <span class="li-head">value2</span> - Value 2. <span class="li-normal">type: str</span>
 <a id='label40' href="javascript:ContentClick('label41', 'label40');" onmouseover="ContentPreview('label41');" onmouseout="ContentUnpreview('label41');" title="click to collapse or expand..."> more... </a>
 <div id="label41" style="display:none">
 <table border="1">
 <tr>
 <td></td>
 <td colspan="1">Supported Version Ranges</td>
 </tr>
 <tr>
 <td>value2</td>
 <td><code class="docutils literal notranslate">v6.0.0 -> v6.4.4 </code></td>
 </tr>
 </table>
 </div>
 </li>
                </ul>
            </ul>
        <li> <span class="li-head">comments</span> - Comment. <span class="li-normal">type: str</span>
 <a id='label42' href="javascript:ContentClick('label43', 'label42');" onmouseover="ContentPreview('label43');" onmouseout="ContentUnpreview('label43');" title="click to collapse or expand..."> more... </a>
 <div id="label43" style="display:none">
 <table border="1">
 <tr>
 <td></td>
 <td colspan="1">Supported Version Ranges</td>
 </tr>
 <tr>
 <td>comments</td>
 <td><code class="docutils literal notranslate">v6.0.0 -> v6.4.4 </code></td>
 </tr>
 </table>
 </div>
 </li>
        <li> <span class="li-head">dataset</span> - Bind dataset to chart. <span class="li-normal">type: str</span>
 <a id='label44' href="javascript:ContentClick('label45', 'label44');" onmouseover="ContentPreview('label45');" onmouseout="ContentUnpreview('label45');" title="click to collapse or expand..."> more... </a>
 <div id="label45" style="display:none">
 <table border="1">
 <tr>
 <td></td>
 <td colspan="1">Supported Version Ranges</td>
 </tr>
 <tr>
 <td>dataset</td>
 <td><code class="docutils literal notranslate">v6.0.0 -> v6.4.4 </code></td>
 </tr>
 </table>
 </div>
 </li>
        <li> <span class="li-head">dimension</span> - Dimension. <span class="li-normal">type: str</span> <span class="li-normal">choices: 2D, 3D</span>
 <a id='label46' href="javascript:ContentClick('label47', 'label46');" onmouseover="ContentPreview('label47');" onmouseout="ContentUnpreview('label47');" title="click to collapse or expand..."> more... </a>
 <div id="label47" style="display:none">
 <table border="1">
 <tr>
 <td></td>
 <td colspan="1">Supported Version Ranges</td>
 </tr>
 <tr>
 <td>dimension</td>
 <td><code class="docutils literal notranslate">v6.0.0 -> v6.4.4 </code></td>
 </tr>
 <tr>
 <td>[2D]</td>
 <td><code class="docutils literal notranslate">v6.0.0 -> v6.4.4</code></td>
 <tr>
 <td>[3D]</td>
 <td><code class="docutils literal notranslate">v6.0.0 -> v6.4.4</code></td>
 </table>
 </div>
 </li>
        <li> <span class="li-head">drill_down_charts</span> - Drill down charts. <span class="li-normal">type: list</span> <span style="font-family:'Courier New'" class="li-required">member_path: drill_down_charts:id</span>
 <a id='label48' href="javascript:ContentClick('label49', 'label48');" onmouseover="ContentPreview('label49');" onmouseout="ContentUnpreview('label49');" title="click to collapse or expand..."> more... </a>
 <div id="label49" style="display:none">
 <table border="1">
 <tr>
 <td></td><td colspan="1">Supported Version Ranges</td>
 </tr>
 <tr>
 <td>drill_down_charts</td>
 <td><code class="docutils literal notranslate">v6.0.0 -> v6.4.4 </code></td>
 </tr>
 </table>
 </div>
 </li>
            <ul class="ul-self">
            <li> <span class="li-head">chart_name</span> - Drill down chart name. <span class="li-normal">type: str</span>
 <a id='label50' href="javascript:ContentClick('label51', 'label50');" onmouseover="ContentPreview('label51');" onmouseout="ContentUnpreview('label51');" title="click to collapse or expand..."> more... </a>
 <div id="label51" style="display:none">
 <table border="1">
 <tr>
 <td></td>
 <td colspan="1">Supported Version Ranges</td>
 </tr>
 <tr>
 <td>chart_name</td>
 <td><code class="docutils literal notranslate">v6.0.0 -> v6.4.4 </code></td>
 </tr>
 </table>
 </div>
 </li>
            <li> <span class="li-head">id</span> - Drill down chart ID. see <a href='#notes'>Notes</a>. <span class="li-normal">type: int</span> <span class="li-required">required: true</span>
 <a id='label52' href="javascript:ContentClick('label53', 'label52');" onmouseover="ContentPreview('label53');" onmouseout="ContentUnpreview('label53');" title="click to collapse or expand..."> more... </a>
 <div id="label53" style="display:none">
 <table border="1">
 <tr>
 <td></td>
 <td colspan="1">Supported Version Ranges</td>
 </tr>
 <tr>
 <td>id</td>
 <td><code class="docutils literal notranslate">v6.0.0 -> v6.4.4 </code></td>
 </tr>
 </table>
 </div>
 </li>
            <li> <span class="li-head">status</span> - Enable/disable this drill down chart. <span class="li-normal">type: str</span> <span class="li-normal">choices: enable, disable</span>
 <a id='label54' href="javascript:ContentClick('label55', 'label54');" onmouseover="ContentPreview('label55');" onmouseout="ContentUnpreview('label55');" title="click to collapse or expand..."> more... </a>
 <div id="label55" style="display:none">
 <table border="1">
 <tr>
 <td></td>
 <td colspan="1">Supported Version Ranges</td>
 </tr>
 <tr>
 <td>status</td>
 <td><code class="docutils literal notranslate">v6.0.0 -> v6.4.4 </code></td>
 </tr>
 <tr>
 <td>[enable]</td>
 <td><code class="docutils literal notranslate">v6.0.0 -> v6.4.4</code></td>
 <tr>
 <td>[disable]</td>
 <td><code class="docutils literal notranslate">v6.0.0 -> v6.4.4</code></td>
 </table>
 </div>
 </li>
            </ul>
        <li> <span class="li-head">favorite</span> - Favorite. <span class="li-normal">type: str</span> <span class="li-normal">choices: no, yes</span>
 <a id='label56' href="javascript:ContentClick('label57', 'label56');" onmouseover="ContentPreview('label57');" onmouseout="ContentUnpreview('label57');" title="click to collapse or expand..."> more... </a>
 <div id="label57" style="display:none">
 <table border="1">
 <tr>
 <td></td>
 <td colspan="1">Supported Version Ranges</td>
 </tr>
 <tr>
 <td>favorite</td>
 <td><code class="docutils literal notranslate">v6.0.0 -> v6.4.4 </code></td>
 </tr>
 <tr>
 <td>[no]</td>
 <td><code class="docutils literal notranslate">v6.0.0 -> v6.4.4</code></td>
 <tr>
 <td>[yes]</td>
 <td><code class="docutils literal notranslate">v6.0.0 -> v6.4.4</code></td>
 </table>
 </div>
 </li>
        <li> <span class="li-head">graph_type</span> - Graph type. <span class="li-normal">type: str</span> <span class="li-normal">choices: none, bar, pie, line, flow</span>
 <a id='label58' href="javascript:ContentClick('label59', 'label58');" onmouseover="ContentPreview('label59');" onmouseout="ContentUnpreview('label59');" title="click to collapse or expand..."> more... </a>
 <div id="label59" style="display:none">
 <table border="1">
 <tr>
 <td></td>
 <td colspan="1">Supported Version Ranges</td>
 </tr>
 <tr>
 <td>graph_type</td>
 <td><code class="docutils literal notranslate">v6.0.0 -> v6.4.4 </code></td>
 </tr>
 <tr>
 <td>[none]</td>
 <td><code class="docutils literal notranslate">v6.0.0 -> v6.4.4</code></td>
 <tr>
 <td>[bar]</td>
 <td><code class="docutils literal notranslate">v6.0.0 -> v6.4.4</code></td>
 <tr>
 <td>[pie]</td>
 <td><code class="docutils literal notranslate">v6.0.0 -> v6.4.4</code></td>
 <tr>
 <td>[line]</td>
 <td><code class="docutils literal notranslate">v6.0.0 -> v6.4.4</code></td>
 <tr>
 <td>[flow]</td>
 <td><code class="docutils literal notranslate">v6.0.0 -> v6.4.4</code></td>
 </table>
 </div>
 </li>
        <li> <span class="li-head">legend</span> - Enable/Disable Legend area. <span class="li-normal">type: str</span> <span class="li-normal">choices: enable, disable</span>
 <a id='label60' href="javascript:ContentClick('label61', 'label60');" onmouseover="ContentPreview('label61');" onmouseout="ContentUnpreview('label61');" title="click to collapse or expand..."> more... </a>
 <div id="label61" style="display:none">
 <table border="1">
 <tr>
 <td></td>
 <td colspan="1">Supported Version Ranges</td>
 </tr>
 <tr>
 <td>legend</td>
 <td><code class="docutils literal notranslate">v6.0.0 -> v6.4.4 </code></td>
 </tr>
 <tr>
 <td>[enable]</td>
 <td><code class="docutils literal notranslate">v6.0.0 -> v6.4.4</code></td>
 <tr>
 <td>[disable]</td>
 <td><code class="docutils literal notranslate">v6.0.0 -> v6.4.4</code></td>
 </table>
 </div>
 </li>
        <li> <span class="li-head">legend_font_size</span> - Font size of legend area. <span class="li-normal">type: int</span>
 <a id='label62' href="javascript:ContentClick('label63', 'label62');" onmouseover="ContentPreview('label63');" onmouseout="ContentUnpreview('label63');" title="click to collapse or expand..."> more... </a>
 <div id="label63" style="display:none">
 <table border="1">
 <tr>
 <td></td>
 <td colspan="1">Supported Version Ranges</td>
 </tr>
 <tr>
 <td>legend_font_size</td>
 <td><code class="docutils literal notranslate">v6.0.0 -> v6.4.4 </code></td>
 </tr>
 </table>
 </div>
 </li>
        <li> <span class="li-head">name</span> - Chart Widget Name <span class="li-normal">type: str</span> <span class="li-required">required: true</span>
 <a id='label64' href="javascript:ContentClick('label65', 'label64');" onmouseover="ContentPreview('label65');" onmouseout="ContentUnpreview('label65');" title="click to collapse or expand..."> more... </a>
 <div id="label65" style="display:none">
 <table border="1">
 <tr>
 <td></td>
 <td colspan="1">Supported Version Ranges</td>
 </tr>
 <tr>
 <td>name</td>
 <td><code class="docutils literal notranslate">v6.0.0 -> v6.4.4 </code></td>
 </tr>
 </table>
 </div>
 </li>
        <li> <span class="li-head">period</span> - Time period. <span class="li-normal">type: str</span> <span class="li-normal">choices: last24h, last7d</span>
 <a id='label66' href="javascript:ContentClick('label67', 'label66');" onmouseover="ContentPreview('label67');" onmouseout="ContentUnpreview('label67');" title="click to collapse or expand..."> more... </a>
 <div id="label67" style="display:none">
 <table border="1">
 <tr>
 <td></td>
 <td colspan="1">Supported Version Ranges</td>
 </tr>
 <tr>
 <td>period</td>
 <td><code class="docutils literal notranslate">v6.0.0 -> v6.4.4 </code></td>
 </tr>
 <tr>
 <td>[last24h]</td>
 <td><code class="docutils literal notranslate">v6.0.0 -> v6.4.4</code></td>
 <tr>
 <td>[last7d]</td>
 <td><code class="docutils literal notranslate">v6.0.0 -> v6.4.4</code></td>
 </table>
 </div>
 </li>
        <li> <span class="li-head">policy</span> - Used by monitor policy. <span class="li-normal">type: int</span>
 <a id='label68' href="javascript:ContentClick('label69', 'label68');" onmouseover="ContentPreview('label69');" onmouseout="ContentUnpreview('label69');" title="click to collapse or expand..."> more... </a>
 <div id="label69" style="display:none">
 <table border="1">
 <tr>
 <td></td>
 <td colspan="1">Supported Version Ranges</td>
 </tr>
 <tr>
 <td>policy</td>
 <td><code class="docutils literal notranslate">v6.0.0 -> v6.4.4 </code></td>
 </tr>
 </table>
 </div>
 </li>
        <li> <span class="li-head">style</span> - Style. <span class="li-normal">type: str</span> <span class="li-normal">choices: auto, manual</span>
 <a id='label70' href="javascript:ContentClick('label71', 'label70');" onmouseover="ContentPreview('label71');" onmouseout="ContentUnpreview('label71');" title="click to collapse or expand..."> more... </a>
 <div id="label71" style="display:none">
 <table border="1">
 <tr>
 <td></td>
 <td colspan="1">Supported Version Ranges</td>
 </tr>
 <tr>
 <td>style</td>
 <td><code class="docutils literal notranslate">v6.0.0 -> v6.4.4 </code></td>
 </tr>
 <tr>
 <td>[auto]</td>
 <td><code class="docutils literal notranslate">v6.0.0 -> v6.4.4</code></td>
 <tr>
 <td>[manual]</td>
 <td><code class="docutils literal notranslate">v6.0.0 -> v6.4.4</code></td>
 </table>
 </div>
 </li>
        <li> <span class="li-head">title</span> - Chart title. <span class="li-normal">type: str</span>
 <a id='label72' href="javascript:ContentClick('label73', 'label72');" onmouseover="ContentPreview('label73');" onmouseout="ContentUnpreview('label73');" title="click to collapse or expand..."> more... </a>
 <div id="label73" style="display:none">
 <table border="1">
 <tr>
 <td></td>
 <td colspan="1">Supported Version Ranges</td>
 </tr>
 <tr>
 <td>title</td>
 <td><code class="docutils literal notranslate">v6.0.0 -> v6.4.4 </code></td>
 </tr>
 </table>
 </div>
 </li>
        <li> <span class="li-head">title_font_size</span> - Font size of chart title. <span class="li-normal">type: int</span>
 <a id='label74' href="javascript:ContentClick('label75', 'label74');" onmouseover="ContentPreview('label75');" onmouseout="ContentUnpreview('label75');" title="click to collapse or expand..."> more... </a>
 <div id="label75" style="display:none">
 <table border="1">
 <tr>
 <td></td>
 <td colspan="1">Supported Version Ranges</td>
 </tr>
 <tr>
 <td>title_font_size</td>
 <td><code class="docutils literal notranslate">v6.0.0 -> v6.4.4 </code></td>
 </tr>
 </table>
 </div>
 </li>
        <li> <span class="li-head">type</span> - Chart type. <span class="li-normal">type: str</span> <span class="li-normal">choices: graph, table</span>
 <a id='label76' href="javascript:ContentClick('label77', 'label76');" onmouseover="ContentPreview('label77');" onmouseout="ContentUnpreview('label77');" title="click to collapse or expand..."> more... </a>
 <div id="label77" style="display:none">
 <table border="1">
 <tr>
 <td></td>
 <td colspan="1">Supported Version Ranges</td>
 </tr>
 <tr>
 <td>type</td>
 <td><code class="docutils literal notranslate">v6.0.0 -> v6.4.4 </code></td>
 </tr>
 <tr>
 <td>[graph]</td>
 <td><code class="docutils literal notranslate">v6.0.0 -> v6.4.4</code></td>
 <tr>
 <td>[table]</td>
 <td><code class="docutils literal notranslate">v6.0.0 -> v6.4.4</code></td>
 </table>
 </div>
 </li>
        <li> <span class="li-head">value_series</span> - Value series of pie chart. <span class="li-normal">type: dict</span>
 <a id='label78' href="javascript:ContentClick('label79', 'label78');" onmouseover="ContentPreview('label79');" onmouseout="ContentUnpreview('label79');" title="click to collapse or expand..."> more... </a>
 <div id="label79" style="display:none">
 <table border="1">
 <tr>
 <td></td><td colspan="1">Supported Version Ranges</td>
 </tr>
 <tr>
 <td>value_series</td>
 <td><code class="docutils literal notranslate">v6.0.0 -> v6.4.4 </code></td>
 </tr>
 </table>
 </div>
 </li>
            <ul class="ul-self">
            <li> <span class="li-head">databind</span> - Value series value expression. <span class="li-normal">type: str</span>
 <a id='label80' href="javascript:ContentClick('label81', 'label80');" onmouseover="ContentPreview('label81');" onmouseout="ContentUnpreview('label81');" title="click to collapse or expand..."> more... </a>
 <div id="label81" style="display:none">
 <table border="1">
 <tr>
 <td></td>
 <td colspan="1">Supported Version Ranges</td>
 </tr>
 <tr>
 <td>databind</td>
 <td><code class="docutils literal notranslate">v6.0.0 -> v6.4.4 </code></td>
 </tr>
 </table>
 </div>
 </li>
            </ul>
        <li> <span class="li-head">x_series</span> - X-series of chart. <span class="li-normal">type: dict</span>
 <a id='label82' href="javascript:ContentClick('label83', 'label82');" onmouseover="ContentPreview('label83');" onmouseout="ContentUnpreview('label83');" title="click to collapse or expand..."> more... </a>
 <div id="label83" style="display:none">
 <table border="1">
 <tr>
 <td></td><td colspan="1">Supported Version Ranges</td>
 </tr>
 <tr>
 <td>x_series</td>
 <td><code class="docutils literal notranslate">v6.0.0 -> v6.4.4 </code></td>
 </tr>
 </table>
 </div>
 </li>
            <ul class="ul-self">
            <li> <span class="li-head">caption</span> - X-series caption. <span class="li-normal">type: str</span>
 <a id='label84' href="javascript:ContentClick('label85', 'label84');" onmouseover="ContentPreview('label85');" onmouseout="ContentUnpreview('label85');" title="click to collapse or expand..."> more... </a>
 <div id="label85" style="display:none">
 <table border="1">
 <tr>
 <td></td>
 <td colspan="1">Supported Version Ranges</td>
 </tr>
 <tr>
 <td>caption</td>
 <td><code class="docutils literal notranslate">v6.0.0 -> v6.4.4 </code></td>
 </tr>
 </table>
 </div>
 </li>
            <li> <span class="li-head">caption_font_size</span> - X-series caption font size. <span class="li-normal">type: int</span>
 <a id='label86' href="javascript:ContentClick('label87', 'label86');" onmouseover="ContentPreview('label87');" onmouseout="ContentUnpreview('label87');" title="click to collapse or expand..."> more... </a>
 <div id="label87" style="display:none">
 <table border="1">
 <tr>
 <td></td>
 <td colspan="1">Supported Version Ranges</td>
 </tr>
 <tr>
 <td>caption_font_size</td>
 <td><code class="docutils literal notranslate">v6.0.0 -> v6.4.4 </code></td>
 </tr>
 </table>
 </div>
 </li>
            <li> <span class="li-head">databind</span> - X-series value expression. <span class="li-normal">type: str</span>
 <a id='label88' href="javascript:ContentClick('label89', 'label88');" onmouseover="ContentPreview('label89');" onmouseout="ContentUnpreview('label89');" title="click to collapse or expand..."> more... </a>
 <div id="label89" style="display:none">
 <table border="1">
 <tr>
 <td></td>
 <td colspan="1">Supported Version Ranges</td>
 </tr>
 <tr>
 <td>databind</td>
 <td><code class="docutils literal notranslate">v6.0.0 -> v6.4.4 </code></td>
 </tr>
 </table>
 </div>
 </li>
            <li> <span class="li-head">font_size</span> - X-series label font size. <span class="li-normal">type: int</span>
 <a id='label90' href="javascript:ContentClick('label91', 'label90');" onmouseover="ContentPreview('label91');" onmouseout="ContentUnpreview('label91');" title="click to collapse or expand..."> more... </a>
 <div id="label91" style="display:none">
 <table border="1">
 <tr>
 <td></td>
 <td colspan="1">Supported Version Ranges</td>
 </tr>
 <tr>
 <td>font_size</td>
 <td><code class="docutils literal notranslate">v6.0.0 -> v6.4.4 </code></td>
 </tr>
 </table>
 </div>
 </li>
            <li> <span class="li-head">is_category</span> - X-series represent category or not. <span class="li-normal">type: str</span> <span class="li-normal">choices: yes, no</span>
 <a id='label92' href="javascript:ContentClick('label93', 'label92');" onmouseover="ContentPreview('label93');" onmouseout="ContentUnpreview('label93');" title="click to collapse or expand..."> more... </a>
 <div id="label93" style="display:none">
 <table border="1">
 <tr>
 <td></td>
 <td colspan="1">Supported Version Ranges</td>
 </tr>
 <tr>
 <td>is_category</td>
 <td><code class="docutils literal notranslate">v6.0.0 -> v6.4.4 </code></td>
 </tr>
 <tr>
 <td>[yes]</td>
 <td><code class="docutils literal notranslate">v6.0.0 -> v6.4.4</code></td>
 <tr>
 <td>[no]</td>
 <td><code class="docutils literal notranslate">v6.0.0 -> v6.4.4</code></td>
 </table>
 </div>
 </li>
            <li> <span class="li-head">label_angle</span> - X-series label angle. <span class="li-normal">type: str</span> <span class="li-normal">choices: 45-degree, vertical, horizontal</span>
 <a id='label94' href="javascript:ContentClick('label95', 'label94');" onmouseover="ContentPreview('label95');" onmouseout="ContentUnpreview('label95');" title="click to collapse or expand..."> more... </a>
 <div id="label95" style="display:none">
 <table border="1">
 <tr>
 <td></td>
 <td colspan="1">Supported Version Ranges</td>
 </tr>
 <tr>
 <td>label_angle</td>
 <td><code class="docutils literal notranslate">v6.0.0 -> v6.4.4 </code></td>
 </tr>
 <tr>
 <td>[45-degree]</td>
 <td><code class="docutils literal notranslate">v6.0.0 -> v6.4.4</code></td>
 <tr>
 <td>[vertical]</td>
 <td><code class="docutils literal notranslate">v6.0.0 -> v6.4.4</code></td>
 <tr>
 <td>[horizontal]</td>
 <td><code class="docutils literal notranslate">v6.0.0 -> v6.4.4</code></td>
 </table>
 </div>
 </li>
            <li> <span class="li-head">scale_direction</span> - Scale increase or decrease. <span class="li-normal">type: str</span> <span class="li-normal">choices: decrease, increase</span>
 <a id='label96' href="javascript:ContentClick('label97', 'label96');" onmouseover="ContentPreview('label97');" onmouseout="ContentUnpreview('label97');" title="click to collapse or expand..."> more... </a>
 <div id="label97" style="display:none">
 <table border="1">
 <tr>
 <td></td>
 <td colspan="1">Supported Version Ranges</td>
 </tr>
 <tr>
 <td>scale_direction</td>
 <td><code class="docutils literal notranslate">v6.0.0 -> v6.4.4 </code></td>
 </tr>
 <tr>
 <td>[decrease]</td>
 <td><code class="docutils literal notranslate">v6.0.0 -> v6.4.4</code></td>
 <tr>
 <td>[increase]</td>
 <td><code class="docutils literal notranslate">v6.0.0 -> v6.4.4</code></td>
 </table>
 </div>
 </li>
            <li> <span class="li-head">scale_format</span> - Date/time format. <span class="li-normal">type: str</span> <span class="li-normal">choices: YYYY-MM-DD-HH-MM, YYYY-MM-DD HH, YYYY-MM-DD, YYYY-MM, YYYY, HH-MM, MM-DD</span>
 <a id='label98' href="javascript:ContentClick('label99', 'label98');" onmouseover="ContentPreview('label99');" onmouseout="ContentUnpreview('label99');" title="click to collapse or expand..."> more... </a>
 <div id="label99" style="display:none">
 <table border="1">
 <tr>
 <td></td>
 <td colspan="1">Supported Version Ranges</td>
 </tr>
 <tr>
 <td>scale_format</td>
 <td><code class="docutils literal notranslate">v6.0.0 -> v6.4.4 </code></td>
 </tr>
 <tr>
 <td>[YYYY-MM-DD-HH-MM]</td>
 <td><code class="docutils literal notranslate">v6.0.0 -> v6.4.4</code></td>
 <tr>
 <td>[YYYY-MM-DD HH]</td>
 <td><code class="docutils literal notranslate">v6.0.0 -> v6.4.4</code></td>
 <tr>
 <td>[YYYY-MM-DD]</td>
 <td><code class="docutils literal notranslate">v6.0.0 -> v6.4.4</code></td>
 <tr>
 <td>[YYYY-MM]</td>
 <td><code class="docutils literal notranslate">v6.0.0 -> v6.4.4</code></td>
 <tr>
 <td>[YYYY]</td>
 <td><code class="docutils literal notranslate">v6.0.0 -> v6.4.4</code></td>
 <tr>
 <td>[HH-MM]</td>
 <td><code class="docutils literal notranslate">v6.0.0 -> v6.4.4</code></td>
 <tr>
 <td>[MM-DD]</td>
 <td><code class="docutils literal notranslate">v6.0.0 -> v6.4.4</code></td>
 </table>
 </div>
 </li>
            <li> <span class="li-head">scale_step</span> - Scale step. <span class="li-normal">type: int</span>
 <a id='label100' href="javascript:ContentClick('label101', 'label100');" onmouseover="ContentPreview('label101');" onmouseout="ContentUnpreview('label101');" title="click to collapse or expand..."> more... </a>
 <div id="label101" style="display:none">
 <table border="1">
 <tr>
 <td></td>
 <td colspan="1">Supported Version Ranges</td>
 </tr>
 <tr>
 <td>scale_step</td>
 <td><code class="docutils literal notranslate">v6.0.0 -> v6.4.4 </code></td>
 </tr>
 </table>
 </div>
 </li>
            <li> <span class="li-head">scale_unit</span> - Scale unit. <span class="li-normal">type: str</span> <span class="li-normal">choices: minute, hour, day, month, year</span>
 <a id='label102' href="javascript:ContentClick('label103', 'label102');" onmouseover="ContentPreview('label103');" onmouseout="ContentUnpreview('label103');" title="click to collapse or expand..."> more... </a>
 <div id="label103" style="display:none">
 <table border="1">
 <tr>
 <td></td>
 <td colspan="1">Supported Version Ranges</td>
 </tr>
 <tr>
 <td>scale_unit</td>
 <td><code class="docutils literal notranslate">v6.0.0 -> v6.4.4 </code></td>
 </tr>
 <tr>
 <td>[minute]</td>
 <td><code class="docutils literal notranslate">v6.0.0 -> v6.4.4</code></td>
 <tr>
 <td>[hour]</td>
 <td><code class="docutils literal notranslate">v6.0.0 -> v6.4.4</code></td>
 <tr>
 <td>[day]</td>
 <td><code class="docutils literal notranslate">v6.0.0 -> v6.4.4</code></td>
 <tr>
 <td>[month]</td>
 <td><code class="docutils literal notranslate">v6.0.0 -> v6.4.4</code></td>
 <tr>
 <td>[year]</td>
 <td><code class="docutils literal notranslate">v6.0.0 -> v6.4.4</code></td>
 </table>
 </div>
 </li>
            <li> <span class="li-head">unit</span> - X-series unit. <span class="li-normal">type: str</span>
 <a id='label104' href="javascript:ContentClick('label105', 'label104');" onmouseover="ContentPreview('label105');" onmouseout="ContentUnpreview('label105');" title="click to collapse or expand..."> more... </a>
 <div id="label105" style="display:none">
 <table border="1">
 <tr>
 <td></td>
 <td colspan="1">Supported Version Ranges</td>
 </tr>
 <tr>
 <td>unit</td>
 <td><code class="docutils literal notranslate">v6.0.0 -> v6.4.4 </code></td>
 </tr>
 </table>
 </div>
 </li>
            </ul>
        <li> <span class="li-head">y_series</span> - Y-series of chart. <span class="li-normal">type: dict</span>
 <a id='label106' href="javascript:ContentClick('label107', 'label106');" onmouseover="ContentPreview('label107');" onmouseout="ContentUnpreview('label107');" title="click to collapse or expand..."> more... </a>
 <div id="label107" style="display:none">
 <table border="1">
 <tr>
 <td></td><td colspan="1">Supported Version Ranges</td>
 </tr>
 <tr>
 <td>y_series</td>
 <td><code class="docutils literal notranslate">v6.0.0 -> v6.4.4 </code></td>
 </tr>
 </table>
 </div>
 </li>
            <ul class="ul-self">
            <li> <span class="li-head">caption</span> - Y-series caption. <span class="li-normal">type: str</span>
 <a id='label108' href="javascript:ContentClick('label109', 'label108');" onmouseover="ContentPreview('label109');" onmouseout="ContentUnpreview('label109');" title="click to collapse or expand..."> more... </a>
 <div id="label109" style="display:none">
 <table border="1">
 <tr>
 <td></td>
 <td colspan="1">Supported Version Ranges</td>
 </tr>
 <tr>
 <td>caption</td>
 <td><code class="docutils literal notranslate">v6.0.0 -> v6.4.4 </code></td>
 </tr>
 </table>
 </div>
 </li>
            <li> <span class="li-head">caption_font_size</span> - Y-series caption font size. <span class="li-normal">type: int</span>
 <a id='label110' href="javascript:ContentClick('label111', 'label110');" onmouseover="ContentPreview('label111');" onmouseout="ContentUnpreview('label111');" title="click to collapse or expand..."> more... </a>
 <div id="label111" style="display:none">
 <table border="1">
 <tr>
 <td></td>
 <td colspan="1">Supported Version Ranges</td>
 </tr>
 <tr>
 <td>caption_font_size</td>
 <td><code class="docutils literal notranslate">v6.0.0 -> v6.4.4 </code></td>
 </tr>
 </table>
 </div>
 </li>
            <li> <span class="li-head">databind</span> - Y-series value expression. <span class="li-normal">type: str</span>
 <a id='label112' href="javascript:ContentClick('label113', 'label112');" onmouseover="ContentPreview('label113');" onmouseout="ContentUnpreview('label113');" title="click to collapse or expand..."> more... </a>
 <div id="label113" style="display:none">
 <table border="1">
 <tr>
 <td></td>
 <td colspan="1">Supported Version Ranges</td>
 </tr>
 <tr>
 <td>databind</td>
 <td><code class="docutils literal notranslate">v6.0.0 -> v6.4.4 </code></td>
 </tr>
 </table>
 </div>
 </li>
            <li> <span class="li-head">extra_databind</span> - Extra Y-series value. <span class="li-normal">type: str</span>
 <a id='label114' href="javascript:ContentClick('label115', 'label114');" onmouseover="ContentPreview('label115');" onmouseout="ContentUnpreview('label115');" title="click to collapse or expand..."> more... </a>
 <div id="label115" style="display:none">
 <table border="1">
 <tr>
 <td></td>
 <td colspan="1">Supported Version Ranges</td>
 </tr>
 <tr>
 <td>extra_databind</td>
 <td><code class="docutils literal notranslate">v6.0.0 -> v6.4.4 </code></td>
 </tr>
 </table>
 </div>
 </li>
            <li> <span class="li-head">extra_y</span> - Allow another Y-series value <span class="li-normal">type: str</span> <span class="li-normal">choices: enable, disable</span>
 <a id='label116' href="javascript:ContentClick('label117', 'label116');" onmouseover="ContentPreview('label117');" onmouseout="ContentUnpreview('label117');" title="click to collapse or expand..."> more... </a>
 <div id="label117" style="display:none">
 <table border="1">
 <tr>
 <td></td>
 <td colspan="1">Supported Version Ranges</td>
 </tr>
 <tr>
 <td>extra_y</td>
 <td><code class="docutils literal notranslate">v6.0.0 -> v6.4.4 </code></td>
 </tr>
 <tr>
 <td>[enable]</td>
 <td><code class="docutils literal notranslate">v6.0.0 -> v6.4.4</code></td>
 <tr>
 <td>[disable]</td>
 <td><code class="docutils literal notranslate">v6.0.0 -> v6.4.4</code></td>
 </table>
 </div>
 </li>
            <li> <span class="li-head">extra_y_legend</span> - Extra Y-series legend type/name. <span class="li-normal">type: str</span>
 <a id='label118' href="javascript:ContentClick('label119', 'label118');" onmouseover="ContentPreview('label119');" onmouseout="ContentUnpreview('label119');" title="click to collapse or expand..."> more... </a>
 <div id="label119" style="display:none">
 <table border="1">
 <tr>
 <td></td>
 <td colspan="1">Supported Version Ranges</td>
 </tr>
 <tr>
 <td>extra_y_legend</td>
 <td><code class="docutils literal notranslate">v6.0.0 -> v6.4.4 </code></td>
 </tr>
 </table>
 </div>
 </li>
            <li> <span class="li-head">font_size</span> - Y-series label font size. <span class="li-normal">type: int</span>
 <a id='label120' href="javascript:ContentClick('label121', 'label120');" onmouseover="ContentPreview('label121');" onmouseout="ContentUnpreview('label121');" title="click to collapse or expand..."> more... </a>
 <div id="label121" style="display:none">
 <table border="1">
 <tr>
 <td></td>
 <td colspan="1">Supported Version Ranges</td>
 </tr>
 <tr>
 <td>font_size</td>
 <td><code class="docutils literal notranslate">v6.0.0 -> v6.4.4 </code></td>
 </tr>
 </table>
 </div>
 </li>
            <li> <span class="li-head">group</span> - Y-series group option. <span class="li-normal">type: str</span>
 <a id='label122' href="javascript:ContentClick('label123', 'label122');" onmouseover="ContentPreview('label123');" onmouseout="ContentUnpreview('label123');" title="click to collapse or expand..."> more... </a>
 <div id="label123" style="display:none">
 <table border="1">
 <tr>
 <td></td>
 <td colspan="1">Supported Version Ranges</td>
 </tr>
 <tr>
 <td>group</td>
 <td><code class="docutils literal notranslate">v6.0.0 -> v6.4.4 </code></td>
 </tr>
 </table>
 </div>
 </li>
            <li> <span class="li-head">label_angle</span> - Y-series label angle. <span class="li-normal">type: str</span> <span class="li-normal">choices: 45-degree, vertical, horizontal</span>
 <a id='label124' href="javascript:ContentClick('label125', 'label124');" onmouseover="ContentPreview('label125');" onmouseout="ContentUnpreview('label125');" title="click to collapse or expand..."> more... </a>
 <div id="label125" style="display:none">
 <table border="1">
 <tr>
 <td></td>
 <td colspan="1">Supported Version Ranges</td>
 </tr>
 <tr>
 <td>label_angle</td>
 <td><code class="docutils literal notranslate">v6.0.0 -> v6.4.4 </code></td>
 </tr>
 <tr>
 <td>[45-degree]</td>
 <td><code class="docutils literal notranslate">v6.0.0 -> v6.4.4</code></td>
 <tr>
 <td>[vertical]</td>
 <td><code class="docutils literal notranslate">v6.0.0 -> v6.4.4</code></td>
 <tr>
 <td>[horizontal]</td>
 <td><code class="docutils literal notranslate">v6.0.0 -> v6.4.4</code></td>
 </table>
 </div>
 </li>
            <li> <span class="li-head">unit</span> - Y-series unit. <span class="li-normal">type: str</span>
 <a id='label126' href="javascript:ContentClick('label127', 'label126');" onmouseover="ContentPreview('label127');" onmouseout="ContentUnpreview('label127');" title="click to collapse or expand..."> more... </a>
 <div id="label127" style="display:none">
 <table border="1">
 <tr>
 <td></td>
 <td colspan="1">Supported Version Ranges</td>
 </tr>
 <tr>
 <td>unit</td>
 <td><code class="docutils literal notranslate">v6.0.0 -> v6.4.4 </code></td>
 </tr>
 </table>
 </div>
 </li>
            <li> <span class="li-head">y_legend</span> - First Y-series legend type/name. <span class="li-normal">type: str</span>
 <a id='label128' href="javascript:ContentClick('label129', 'label128');" onmouseover="ContentPreview('label129');" onmouseout="ContentUnpreview('label129');" title="click to collapse or expand..."> more... </a>
 <div id="label129" style="display:none">
 <table border="1">
 <tr>
 <td></td>
 <td colspan="1">Supported Version Ranges</td>
 </tr>
 <tr>
 <td>y_legend</td>
 <td><code class="docutils literal notranslate">v6.0.0 -> v6.4.4 </code></td>
 </tr>
 </table>
 </div>
 </li>
            </ul>
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
    
    - name: Report chart widget configuration.
      fortinet.fortios.fortios_report_chart:
          vdom: "{{ vdom }}"
          state: "present"
          access_token: "<your_own_value>"
          report_chart:
              background: "<your_own_value>"
              category: "misc"
              category_series:
                  databind: "<your_own_value>"
                  font_size: "10"
              color_palette: "<your_own_value>"
              column:
                  -
                      detail_unit: "<your_own_value>"
                      detail_value: "<your_own_value>"
                      footer_unit: "<your_own_value>"
                      footer_value: "<your_own_value>"
                      header_value: "<your_own_value>"
                      id: "15"
                      mapping:
                          -
                              displayname: "<your_own_value>"
                              id: "18"
                              op: "none"
                              value_type: "integer"
                              value1: "<your_own_value>"
                              value2: "<your_own_value>"
              comments: "<your_own_value>"
              dataset: "<your_own_value>"
              dimension: "2D"
              drill_down_charts:
                  -
                      chart_name: "<your_own_value>"
                      id: "28"
                      status: "enable"
              favorite: "no"
              graph_type: "none"
              legend: "enable"
              legend_font_size: "2147483647"
              name: "default_name_34"
              period: "last24h"
              policy: "2147483647"
              style: "auto"
              title: "<your_own_value>"
              title_font_size: "2147483647"
              type: "graph"
              value_series:
                  databind: "<your_own_value>"
              x_series:
                  caption: "<your_own_value>"
                  caption_font_size: "10"
                  databind: "<your_own_value>"
                  font_size: "10"
                  is_category: "yes"
                  label_angle: "45-degree"
                  scale_direction: "decrease"
                  scale_format: "YYYY-MM-DD-HH-MM"
                  scale_step: "32767"
                  scale_unit: "minute"
                  unit: "<your_own_value>"
              y_series:
                  caption: "<your_own_value>"
                  caption_font_size: "10"
                  databind: "<your_own_value>"
                  extra_databind: "<your_own_value>"
                  extra_y: "enable"
                  extra_y_legend: "<your_own_value>"
                  font_size: "10"
                  group: "<your_own_value>"
                  label_angle: "45-degree"
                  unit: "<your_own_value>"
                  y_legend: "<your_own_value>"


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
