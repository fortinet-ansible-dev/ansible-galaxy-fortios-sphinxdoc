:source: fortios_videofilter_profile.py

:orphan:

.. fortios_videofilter_profile:

fortios_videofilter_profile -- Configure VideoFilter profile in Fortinet's FortiOS and FortiGate.
+++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++

.. versionadded:: 2.0.0

.. contents::
   :local:
   :depth: 1


Synopsis
--------
- This module is able to configure a FortiGate or FortiOS (FOS) device by allowing the user to set and modify videofilter feature and profile category. Examples include all parameters and values need to be adjusted to datasources before usage. Tested with FOS v6.0.0



Requirements
------------
The below requirements are needed on the host that executes this module.

- ansible>=2.15


Tips
----
Using member operation to add an element to an existing object.

FortiOS Version Compatibility
-----------------------------
Supported Version Ranges: v7.0.0 -> v7.6.0


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
    <li> <span class="li-head">videofilter_profile</span> - Configure VideoFilter profile. <span class="li-normal">type: dict</span>
 <a id='label0' href="javascript:ContentClick('label1', 'label0');" onmouseover="ContentPreview('label1');" onmouseout="ContentUnpreview('label1');" title="click to collapse or expand..."> more... </a>
 <div id="label1" style="display:none">
 <table border="1">
 <tr>
 <td></td><td colspan="1">Supported Version Ranges</td>
 </tr>
 <tr>
 <td>videofilter_profile</td>
 <td><code class="docutils literal notranslate">v7.0.0 -> 7.6.0 </code></td>
 </tr>
 </table>
 </div>
 </li>
        <ul class="ul-self">
        <li> <span class="li-head">comment</span> - Comment. <span class="li-normal">type: str</span>
 <a id='label2' href="javascript:ContentClick('label3', 'label2');" onmouseover="ContentPreview('label3');" onmouseout="ContentUnpreview('label3');" title="click to collapse or expand..."> more... </a>
 <div id="label3" style="display:none">
 <table border="1">
 <tr>
 <td></td>
 <td colspan="1">Supported Version Ranges</td>
 </tr>
 <tr>
 <td>comment</td>
 <td><code class="docutils literal notranslate">v7.0.0 -> 7.6.0 </code></td>
 </tr>
 </table>
 </div>
 </li>
        <li> <span class="li-head">dailymotion</span> - Enable/disable Dailymotion video source. <span class="li-normal">type: str</span> <span class="li-normal">choices: enable, disable</span>
 <a id='label4' href="javascript:ContentClick('label5', 'label4');" onmouseover="ContentPreview('label5');" onmouseout="ContentUnpreview('label5');" title="click to collapse or expand..."> more... </a>
 <div id="label5" style="display:none">
 <table border="1">
 <tr>
 <td></td>
 <td colspan="1">Supported Version Ranges</td>
 </tr>
 <tr>
 <td>dailymotion</td>
 <td><code class="docutils literal notranslate">v7.0.0 -> 7.6.0 </code></td>
 </tr>
 <tr>
 <td>[enable]</td>
 <td><code class="docutils literal notranslate">v7.0.0 -> 7.6.0</code></td>
 <tr>
 <td>[disable]</td>
 <td><code class="docutils literal notranslate">v7.0.0 -> 7.6.0</code></td>
 </table>
 </div>
 </li>
        <li> <span class="li-head">default_action</span> - Video filter default action. <span class="li-normal">type: str</span> <span class="li-normal">choices: allow, monitor, block</span>
 <a id='label6' href="javascript:ContentClick('label7', 'label6');" onmouseover="ContentPreview('label7');" onmouseout="ContentUnpreview('label7');" title="click to collapse or expand..."> more... </a>
 <div id="label7" style="display:none">
 <table border="1">
 <tr>
 <td></td>
 <td colspan="1">Supported Version Ranges</td>
 </tr>
 <tr>
 <td>default_action</td>
 <td><code class="docutils literal notranslate">v7.4.0 -> v7.4.1 </code></td>
 </tr>
 <tr>
 <td>[allow]</td>
 <td><code class="docutils literal notranslate">v7.4.0 -> v7.4.1</code></td>
 <tr>
 <td>[monitor]</td>
 <td><code class="docutils literal notranslate">v7.4.0 -> v7.4.1</code></td>
 <tr>
 <td>[block]</td>
 <td><code class="docutils literal notranslate">v7.4.0 -> v7.4.1</code></td>
 </table>
 </div>
 </li>
        <li> <span class="li-head">filters</span> - YouTube filter entries. <span class="li-normal">type: list</span> <span style="font-family:'Courier New'" class="li-required">member_path: filters:id</span>
 <a id='label8' href="javascript:ContentClick('label9', 'label8');" onmouseover="ContentPreview('label9');" onmouseout="ContentUnpreview('label9');" title="click to collapse or expand..."> more... </a>
 <div id="label9" style="display:none">
 <table border="1">
 <tr>
 <td></td><td colspan="1">Supported Version Ranges</td>
 </tr>
 <tr>
 <td>filters</td>
 <td><code class="docutils literal notranslate">v7.4.2 -> 7.6.0 </code></td>
 </tr>
 </table>
 </div>
 </li>
            <ul class="ul-self">
            <li> <span class="li-head">action</span> - Video filter action. <span class="li-normal">type: str</span> <span class="li-normal">choices: allow, monitor, block</span>
 <a id='label10' href="javascript:ContentClick('label11', 'label10');" onmouseover="ContentPreview('label11');" onmouseout="ContentUnpreview('label11');" title="click to collapse or expand..."> more... </a>
 <div id="label11" style="display:none">
 <table border="1">
 <tr>
 <td></td>
 <td colspan="1">Supported Version Ranges</td>
 </tr>
 <tr>
 <td>action</td>
 <td><code class="docutils literal notranslate">v7.4.2 -> 7.6.0 </code></td>
 </tr>
 <tr>
 <td>[allow]</td>
 <td><code class="docutils literal notranslate">v7.4.2 -> 7.6.0</code></td>
 <tr>
 <td>[monitor]</td>
 <td><code class="docutils literal notranslate">v7.4.2 -> 7.6.0</code></td>
 <tr>
 <td>[block]</td>
 <td><code class="docutils literal notranslate">v7.4.2 -> 7.6.0</code></td>
 </table>
 </div>
 </li>
            <li> <span class="li-head">category</span> - FortiGuard category ID. <span class="li-normal">type: str</span>
 <a id='label12' href="javascript:ContentClick('label13', 'label12');" onmouseover="ContentPreview('label13');" onmouseout="ContentUnpreview('label13');" title="click to collapse or expand..."> more... </a>
 <div id="label13" style="display:none">
 <table border="1">
 <tr>
 <td></td>
 <td colspan="1">Supported Version Ranges</td>
 </tr>
 <tr>
 <td>category</td>
 <td><code class="docutils literal notranslate">v7.4.2 -> 7.6.0 </code></td>
 </tr>
 </table>
 </div>
 </li>
            <li> <span class="li-head">channel</span> - Channel ID. <span class="li-normal">type: str</span>
 <a id='label14' href="javascript:ContentClick('label15', 'label14');" onmouseover="ContentPreview('label15');" onmouseout="ContentUnpreview('label15');" title="click to collapse or expand..."> more... </a>
 <div id="label15" style="display:none">
 <table border="1">
 <tr>
 <td></td>
 <td colspan="1">Supported Version Ranges</td>
 </tr>
 <tr>
 <td>channel</td>
 <td><code class="docutils literal notranslate">v7.4.2 -> 7.6.0 </code></td>
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
 <td><code class="docutils literal notranslate">v7.4.2 -> 7.6.0 </code></td>
 </tr>
 </table>
 </div>
 </li>
            <li> <span class="li-head">id</span> - ID. see <a href='#notes'>Notes</a>. <span class="li-normal">type: int</span> <span class="li-required">required: true</span>
 <a id='label18' href="javascript:ContentClick('label19', 'label18');" onmouseover="ContentPreview('label19');" onmouseout="ContentUnpreview('label19');" title="click to collapse or expand..."> more... </a>
 <div id="label19" style="display:none">
 <table border="1">
 <tr>
 <td></td>
 <td colspan="1">Supported Version Ranges</td>
 </tr>
 <tr>
 <td>id</td>
 <td><code class="docutils literal notranslate">v7.4.2 -> 7.6.0 </code></td>
 </tr>
 </table>
 </div>
 </li>
            <li> <span class="li-head">keyword</span> - Video filter keyword ID. Source videofilter.keyword.id. <span class="li-normal">type: int</span>
 <a id='label20' href="javascript:ContentClick('label21', 'label20');" onmouseover="ContentPreview('label21');" onmouseout="ContentUnpreview('label21');" title="click to collapse or expand..."> more... </a>
 <div id="label21" style="display:none">
 <table border="1">
 <tr>
 <td></td>
 <td colspan="1">Supported Version Ranges</td>
 </tr>
 <tr>
 <td>keyword</td>
 <td><code class="docutils literal notranslate">v7.4.2 -> 7.6.0 </code></td>
 </tr>
 </table>
 </div>
 </li>
            <li> <span class="li-head">log</span> - Enable/disable logging. <span class="li-normal">type: str</span> <span class="li-normal">choices: enable, disable</span>
 <a id='label22' href="javascript:ContentClick('label23', 'label22');" onmouseover="ContentPreview('label23');" onmouseout="ContentUnpreview('label23');" title="click to collapse or expand..."> more... </a>
 <div id="label23" style="display:none">
 <table border="1">
 <tr>
 <td></td>
 <td colspan="1">Supported Version Ranges</td>
 </tr>
 <tr>
 <td>log</td>
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
            <li> <span class="li-head">type</span> - Filter type. <span class="li-normal">type: str</span> <span class="li-normal">choices: category, channel, title, description</span>
 <a id='label24' href="javascript:ContentClick('label25', 'label24');" onmouseover="ContentPreview('label25');" onmouseout="ContentUnpreview('label25');" title="click to collapse or expand..."> more... </a>
 <div id="label25" style="display:none">
 <table border="1">
 <tr>
 <td></td>
 <td colspan="1">Supported Version Ranges</td>
 </tr>
 <tr>
 <td>type</td>
 <td><code class="docutils literal notranslate">v7.4.2 -> 7.6.0 </code></td>
 </tr>
 <tr>
 <td>[category]</td>
 <td><code class="docutils literal notranslate">v7.4.2 -> 7.6.0</code></td>
 <tr>
 <td>[channel]</td>
 <td><code class="docutils literal notranslate">v7.4.2 -> 7.6.0</code></td>
 <tr>
 <td>[title]</td>
 <td><code class="docutils literal notranslate">v7.4.2 -> 7.6.0</code></td>
 <tr>
 <td>[description]</td>
 <td><code class="docutils literal notranslate">v7.4.2 -> 7.6.0</code></td>
 </table>
 </div>
 </li>
            </ul>
        <li> <span class="li-head">fortiguard_category</span> - Configure FortiGuard categories. <span class="li-normal">type: dict</span>
 <a id='label26' href="javascript:ContentClick('label27', 'label26');" onmouseover="ContentPreview('label27');" onmouseout="ContentUnpreview('label27');" title="click to collapse or expand..."> more... </a>
 <div id="label27" style="display:none">
 <table border="1">
 <tr>
 <td></td><td colspan="1">Supported Version Ranges</td>
 </tr>
 <tr>
 <td>fortiguard_category</td>
 <td><code class="docutils literal notranslate">v7.0.0 -> v7.4.1 </code></td>
 </tr>
 </table>
 </div>
 </li>
            <ul class="ul-self">
            <li> <span class="li-head">filters</span> - Configure VideoFilter FortiGuard category. <span class="li-normal">type: list</span> <span style="font-family:'Courier New'" class="li-required">member_path: fortiguard_category/filters:id</span>
 <a id='label28' href="javascript:ContentClick('label29', 'label28');" onmouseover="ContentPreview('label29');" onmouseout="ContentUnpreview('label29');" title="click to collapse or expand..."> more... </a>
 <div id="label29" style="display:none">
 <table border="1">
 <tr>
 <td></td><td colspan="1">Supported Version Ranges</td>
 </tr>
 <tr>
 <td>filters</td>
 <td><code class="docutils literal notranslate">v7.0.0 -> v7.4.1 </code></td>
 </tr>
 </table>
 </div>
 </li>
                <ul class="ul-self">
                <li> <span class="li-head">action</span> - VideoFilter action. <span class="li-normal">type: str</span> <span class="li-normal">choices: allow, monitor, block, bypass</span>
 <a id='label30' href="javascript:ContentClick('label31', 'label30');" onmouseover="ContentPreview('label31');" onmouseout="ContentUnpreview('label31');" title="click to collapse or expand..."> more... </a>
 <div id="label31" style="display:none">
 <table border="1">
 <tr>
 <td></td>
 <td colspan="1">Supported Version Ranges</td>
 </tr>
 <tr>
 <td>action</td>
 <td><code class="docutils literal notranslate">v7.0.0 -> v7.4.1 </code></td>
 </tr>
 <tr>
 <td>[allow]</td>
 <td><code class="docutils literal notranslate">v7.0.1 -> v7.4.1</code></td>
 </tr>
 <tr>
 <td>[monitor]</td>
 <td><code class="docutils literal notranslate">v7.0.0 -> v7.4.1</code></td>
 <tr>
 <td>[block]</td>
 <td><code class="docutils literal notranslate">v7.0.0 -> v7.4.1</code></td>
 <tr>
 <td>[bypass]</td>
 <td><code class="docutils literal notranslate">v7.0.0 -> v7.0.0</code></td>
 </tr>
 </table>
 </div>
 </li>
                <li> <span class="li-head">category_id</span> - Category ID. <span class="li-normal">type: int</span>
 <a id='label32' href="javascript:ContentClick('label33', 'label32');" onmouseover="ContentPreview('label33');" onmouseout="ContentUnpreview('label33');" title="click to collapse or expand..."> more... </a>
 <div id="label33" style="display:none">
 <table border="1">
 <tr>
 <td></td>
 <td colspan="1">Supported Version Ranges</td>
 </tr>
 <tr>
 <td>category_id</td>
 <td><code class="docutils literal notranslate">v7.0.0 -> v7.4.1 </code></td>
 </tr>
 </table>
 </div>
 </li>
                <li> <span class="li-head">id</span> - ID. see <a href='#notes'>Notes</a>. <span class="li-normal">type: int</span> <span class="li-required">required: true</span>
 <a id='label34' href="javascript:ContentClick('label35', 'label34');" onmouseover="ContentPreview('label35');" onmouseout="ContentUnpreview('label35');" title="click to collapse or expand..."> more... </a>
 <div id="label35" style="display:none">
 <table border="1">
 <tr>
 <td></td>
 <td colspan="1">Supported Version Ranges</td>
 </tr>
 <tr>
 <td>id</td>
 <td><code class="docutils literal notranslate">v7.0.0 -> v7.4.1 </code></td>
 </tr>
 </table>
 </div>
 </li>
                <li> <span class="li-head">log</span> - Enable/disable logging. <span class="li-normal">type: str</span> <span class="li-normal">choices: enable, disable</span>
 <a id='label36' href="javascript:ContentClick('label37', 'label36');" onmouseover="ContentPreview('label37');" onmouseout="ContentUnpreview('label37');" title="click to collapse or expand..."> more... </a>
 <div id="label37" style="display:none">
 <table border="1">
 <tr>
 <td></td>
 <td colspan="1">Supported Version Ranges</td>
 </tr>
 <tr>
 <td>log</td>
 <td><code class="docutils literal notranslate">v7.0.0 -> v7.4.1 </code></td>
 </tr>
 <tr>
 <td>[enable]</td>
 <td><code class="docutils literal notranslate">v7.0.0 -> v7.4.1</code></td>
 <tr>
 <td>[disable]</td>
 <td><code class="docutils literal notranslate">v7.0.0 -> v7.4.1</code></td>
 </table>
 </div>
 </li>
                </ul>
            </ul>
        <li> <span class="li-head">log</span> - Enable/disable logging. <span class="li-normal">type: str</span> <span class="li-normal">choices: enable, disable</span>
 <a id='label38' href="javascript:ContentClick('label39', 'label38');" onmouseover="ContentPreview('label39');" onmouseout="ContentUnpreview('label39');" title="click to collapse or expand..."> more... </a>
 <div id="label39" style="display:none">
 <table border="1">
 <tr>
 <td></td>
 <td colspan="1">Supported Version Ranges</td>
 </tr>
 <tr>
 <td>log</td>
 <td><code class="docutils literal notranslate">v7.4.0 -> v7.4.1 </code></td>
 </tr>
 <tr>
 <td>[enable]</td>
 <td><code class="docutils literal notranslate">v7.4.0 -> v7.4.1</code></td>
 <tr>
 <td>[disable]</td>
 <td><code class="docutils literal notranslate">v7.4.0 -> v7.4.1</code></td>
 </table>
 </div>
 </li>
        <li> <span class="li-head">name</span> - Name. <span class="li-normal">type: str</span> <span class="li-required">required: true</span>
 <a id='label40' href="javascript:ContentClick('label41', 'label40');" onmouseover="ContentPreview('label41');" onmouseout="ContentUnpreview('label41');" title="click to collapse or expand..."> more... </a>
 <div id="label41" style="display:none">
 <table border="1">
 <tr>
 <td></td>
 <td colspan="1">Supported Version Ranges</td>
 </tr>
 <tr>
 <td>name</td>
 <td><code class="docutils literal notranslate">v7.0.0 -> 7.6.0 </code></td>
 </tr>
 </table>
 </div>
 </li>
        <li> <span class="li-head">replacemsg_group</span> - Replacement message group. Source system.replacemsg-group.name. <span class="li-normal">type: str</span>
 <a id='label42' href="javascript:ContentClick('label43', 'label42');" onmouseover="ContentPreview('label43');" onmouseout="ContentUnpreview('label43');" title="click to collapse or expand..."> more... </a>
 <div id="label43" style="display:none">
 <table border="1">
 <tr>
 <td></td>
 <td colspan="1">Supported Version Ranges</td>
 </tr>
 <tr>
 <td>replacemsg_group</td>
 <td><code class="docutils literal notranslate">v7.0.1 -> 7.6.0 </code></td>
 </tr>
 </table>
 </div>
 </li>
        <li> <span class="li-head">vimeo</span> - Enable/disable Vimeo video source. <span class="li-normal">type: str</span> <span class="li-normal">choices: enable, disable</span>
 <a id='label44' href="javascript:ContentClick('label45', 'label44');" onmouseover="ContentPreview('label45');" onmouseout="ContentUnpreview('label45');" title="click to collapse or expand..."> more... </a>
 <div id="label45" style="display:none">
 <table border="1">
 <tr>
 <td></td>
 <td colspan="1">Supported Version Ranges</td>
 </tr>
 <tr>
 <td>vimeo</td>
 <td><code class="docutils literal notranslate">v7.0.0 -> 7.6.0 </code></td>
 </tr>
 <tr>
 <td>[enable]</td>
 <td><code class="docutils literal notranslate">v7.0.0 -> 7.6.0</code></td>
 <tr>
 <td>[disable]</td>
 <td><code class="docutils literal notranslate">v7.0.0 -> 7.6.0</code></td>
 </table>
 </div>
 </li>
        <li> <span class="li-head">vimeo_restrict</span> - Set Vimeo-restrict ("7" = don"t show mature content, "134" = don"t show unrated and mature content). A value of cookie "content_rating". <span class="li-normal">type: str</span>
 <a id='label46' href="javascript:ContentClick('label47', 'label46');" onmouseover="ContentPreview('label47');" onmouseout="ContentUnpreview('label47');" title="click to collapse or expand..."> more... </a>
 <div id="label47" style="display:none">
 <table border="1">
 <tr>
 <td></td>
 <td colspan="1">Supported Version Ranges</td>
 </tr>
 <tr>
 <td>vimeo_restrict</td>
 <td><code class="docutils literal notranslate">v7.0.0 -> v7.0.0 </code></td>
 </tr>
 </table>
 </div>
 </li>
        <li> <span class="li-head">youtube</span> - Enable/disable YouTube video source. <span class="li-normal">type: str</span> <span class="li-normal">choices: enable, disable</span>
 <a id='label48' href="javascript:ContentClick('label49', 'label48');" onmouseover="ContentPreview('label49');" onmouseout="ContentUnpreview('label49');" title="click to collapse or expand..."> more... </a>
 <div id="label49" style="display:none">
 <table border="1">
 <tr>
 <td></td>
 <td colspan="1">Supported Version Ranges</td>
 </tr>
 <tr>
 <td>youtube</td>
 <td><code class="docutils literal notranslate">v7.0.0 -> 7.6.0 </code></td>
 </tr>
 <tr>
 <td>[enable]</td>
 <td><code class="docutils literal notranslate">v7.0.0 -> 7.6.0</code></td>
 <tr>
 <td>[disable]</td>
 <td><code class="docutils literal notranslate">v7.0.0 -> 7.6.0</code></td>
 </table>
 </div>
 </li>
        <li> <span class="li-head">youtube_channel_filter</span> - Set YouTube channel filter. Source videofilter.youtube-channel-filter.id. <span class="li-normal">type: int</span>
 <a id='label50' href="javascript:ContentClick('label51', 'label50');" onmouseover="ContentPreview('label51');" onmouseout="ContentUnpreview('label51');" title="click to collapse or expand..."> more... </a>
 <div id="label51" style="display:none">
 <table border="1">
 <tr>
 <td></td>
 <td colspan="1">Supported Version Ranges</td>
 </tr>
 <tr>
 <td>youtube_channel_filter</td>
 <td><code class="docutils literal notranslate">v7.0.0 -> v7.4.1 </code></td>
 </tr>
 </table>
 </div>
 </li>
        <li> <span class="li-head">youtube_restrict</span> - Set YouTube-restrict mode. <span class="li-normal">type: str</span> <span class="li-normal">choices: none, strict, moderate</span>
 <a id='label52' href="javascript:ContentClick('label53', 'label52');" onmouseover="ContentPreview('label53');" onmouseout="ContentUnpreview('label53');" title="click to collapse or expand..."> more... </a>
 <div id="label53" style="display:none">
 <table border="1">
 <tr>
 <td></td>
 <td colspan="1">Supported Version Ranges</td>
 </tr>
 <tr>
 <td>youtube_restrict</td>
 <td><code class="docutils literal notranslate">v7.0.0 -> v7.0.0 </code></td>
 </tr>
 <tr>
 <td>[none]</td>
 <td><code class="docutils literal notranslate">v7.0.0 -> v7.0.0</code></td>
 <tr>
 <td>[strict]</td>
 <td><code class="docutils literal notranslate">v7.0.0 -> v7.0.0</code></td>
 <tr>
 <td>[moderate]</td>
 <td><code class="docutils literal notranslate">v7.0.0 -> v7.0.0</code></td>
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
    
    - name: Configure VideoFilter profile.
      fortinet.fortios.fortios_videofilter_profile:
          vdom: "{{ vdom }}"
          state: "present"
          access_token: "<your_own_value>"
          videofilter_profile:
              comment: "Comment."
              dailymotion: "enable"
              default_action: "allow"
              filters:
                  -
                      action: "allow"
                      category: "<your_own_value>"
                      channel: "<your_own_value>"
                      comment: "Comment."
                      id: "11"
                      keyword: "0"
                      log: "enable"
                      type: "category"
              fortiguard_category:
                  filters:
                      -
                          action: "allow"
                          category_id: "0"
                          id: "19"
                          log: "enable"
              log: "enable"
              name: "default_name_22"
              replacemsg_group: "<your_own_value> (source system.replacemsg-group.name)"
              vimeo: "enable"
              vimeo_restrict: "<your_own_value>"
              youtube: "enable"
              youtube_channel_filter: "0"
              youtube_restrict: "none"


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
