:source: fortios_log_fact.py

:orphan:

.. :

fortios_log_fact -- Retrieve Log Data of Fortios Log Objects.
++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++

.. versionadded:: 2.10

.. contents::
   :local:
   :depth: 1


Synopsis
--------
- Collects log data from network devices running the fortios operating system.  This module will only collect the log data specified in the playbook.



Requirements
------------
The below requirements are needed on the host that executes this module.

- install galaxy collection fortinet.fortios >= ``2.1.0``.


Parameters
----------


.. raw:: html

    <ul>
    <li> <span class="li-head">vdom</span> - Virtual domain, among those defined previously. A vdom is a virtual instance of the FortiGate that can be configured and used as a different unit. <span class="li-normal">type: str</span> <span class="li-required">required: False</span> <span class="li-normal">default: root</span></li>
    <li> <span class="li-head">enable_log</span> - Enable/Disable logging for task. <span class="li-normal">type: bool</span> <span class="li-required">required: False</span> <span class="li-normal">default: False</span> </li>
    <li> <span class="li-head">access_token</span> - Token-based authentication. Generated from GUI of Fortigate. <span class="li-normal">type: str</span> <span class="li-required">required: False</span> </li>
    <li> <span class="li-head">filters</span> - A list of expressions to filter the returned results. <span class="li-normal">type: list</span> <span class="li-required">required: False</span>
     <a id='label0' href="javascript:ContentClick('label1', 'label0');" onmouseover="ContentPreview('label1');" onmouseout="ContentUnpreview('label1');" title="click to collapse or expand..."> more... </a>
     <div id="label1" style="display:none">
     Filter item must be in the following format: <code class="docutils literal notranslate"><span class="pre">[key][operator][pattern]</span></code>, operators could be found in the table:
     <table border="1">
        <tr>
         <td><code class="docutils literal notranslate">Operator </code></td>
         <td><code class="docutils literal notranslate">Case sensitive </code></td>
         <td><code class="docutils literal notranslate">Description </code></td>
        </tr>
      <tr>
       <td>==</td>
       <td>Yes</td>
       <td>Pattern must be identical to the value.</td>
      </tr>
      <tr>
       <td>=*</td>
       <td>No</td>
       <td>Pattern must be identical to the value.</td>
      </tr>
      <tr>
       <td>!=</td>
       <td>Yes</td>
       <td>Pattern does not match the value.</td>
      </tr>
      <tr>
       <td>!*</td>
       <td>No</td>
       <td>Pattern does not match the value.</td>
      </tr>
      <tr>
       <td>=@</td>
       <td>No</td>
       <td>Pattern found within value.</td>
      </tr>
      <tr>
       <td>!@</td>
       <td>No</td>
       <td>Pattern not found within value.</td>
      </tr>
      <tr>
       <td><=</td>
       <td>n/a</td>
       <td>Value must be less than or equal to pattern.</td>
      </tr>
      <tr>
       <td><</td>
       <td>n/a</td>
       <td>Value must be less than pattern.</td>
      </tr>
      <tr>
       <td>>=</td>
       <td>n/a</td>
       <td>Value must be greater than or equal to pattern.</td>
      </tr>
      <tr>
       <td>></td>
       <td>n/a</td>
       <td>Value must be greater than pattern.</td>
      </tr>
      </table>
     </div>
    </li>
    <li> <span class="li-head">sorters</span> - A list of expressions to sort the returned results. <span class="li-normal">type: list</span> <span class="li-required">required: False</span>
        <a id='label2' href="javascript:ContentClick('label3', 'label2');" onmouseover="ContentPreview('label3');" onmouseout="ContentUnpreview('label3');" title="click to collapse or expand..."> more... </a>
       <div id="label3" style="display:none">
       Sorter item must be a <code class="docutils literal notranslate"><span class="pre">[key]</span></code> followed by a <code class="docutils literal notranslate"><span class="pre">,asc</span></code> or <code class="docutils literal notranslate"><span class="pre">,dsc</span></code> order derective.
       <br>
       examples: <code class="docutils literal notranslate"><span class="pre">name,asc</span></code> to sort the result by name in ascending order; <code class="docutils literal notranslate"><span class="pre">vlanid,asc</span></code> to sort the result by vlanid in descending order.
       </div>
    </li>
    <li> <span class="li-head">formatters</span> - A list of fields to display for returned results. <span class="li-normal">type: list</span> <span class="li-required">required: False</span> </li>
    <li><span class="li-head">selector</span> - selector of the retrieved log data <span class="li-normal">type: str</span> <span class="li-required">choices:</span></li>
        <li style="list-style: none;"><section class="accordion">
        <input type="checkbox" name="collapse" id="handle2">
        <h2 class="handle">
            <label for="handle2"><u>Show full selector list...</u></label>
        </h2>
        <div class="content">
        <ul class="ul-self">
        disk_anomaly_raw
        <li><span class="li-head">disk_anomaly_raw</span> - Log data for the given log type in raw format. 
        <ul class="ul-self">
                <li><span class="li-required">rows</span> - Number of rows to return. <span class="li-normal">type: int </span> </li>
                <li><span class="li-required">serial_no</span> - Retrieve log from the specified device. <span class="li-normal">type: string </span> </li>
                <li><span class="li-required">session_id</span> - Provide a session_id to continue getting data for that request. <span class="li-normal">type: int </span> </li>
                <li><span class="li-required">filter</span> - Filter expression(s). <span class="li-normal">type: string </span> </li>
                <li><span class="li-required">start</span> - Row number for the first row to return. <span class="li-normal">type: int </span> </li>
                <li><span class="li-required">is_ha_member</span> - Is the specified device an HA member. <span class="li-normal">type: boolean </span> </li>
                
            </ul>
        
        </li>
        disk_app-ctrl_archive
        <li><span class="li-head">disk_app-ctrl_archive</span> - Return a list of archived items for the desired type. :type can be app-ctrl or ips 
        <ul class="ul-self">
                <li><span class="li-required">roll</span> - Log roll number. (required if source is not fortianalyzer) <span class="li-normal">type: int </span> </li>
                <li><span class="li-required">mkey</span> - Archive identifier. <span class="li-normal">type: int </span> </li>
                
            </ul>
        
        </li>
        disk_app-ctrl_archive-download
        <li><span class="li-head">disk_app-ctrl_archive-download</span> - Download an archived file. 
        <ul class="ul-self">
                <li><span class="li-required">roll</span> - Log roll number (required if source is not fortianalyzer). <span class="li-normal">type: int </span> </li>
                <li><span class="li-required">mkey</span> - Archive identifier. <span class="li-normal">type: int </span> </li>
                <li><span class="li-required">filename</span> - File name to use when saving the file in the browser. <span class="li-normal">type: string </span> </li>
                
            </ul>
        
        </li>
        disk_app-ctrl_raw
        <li><span class="li-head">disk_app-ctrl_raw</span> - Log data for the given log type in raw format. 
        <ul class="ul-self">
                <li><span class="li-required">rows</span> - Number of rows to return. <span class="li-normal">type: int </span> </li>
                <li><span class="li-required">serial_no</span> - Retrieve log from the specified device. <span class="li-normal">type: string </span> </li>
                <li><span class="li-required">session_id</span> - Provide a session_id to continue getting data for that request. <span class="li-normal">type: int </span> </li>
                <li><span class="li-required">filter</span> - Filter expression(s). <span class="li-normal">type: string </span> </li>
                <li><span class="li-required">start</span> - Row number for the first row to return. <span class="li-normal">type: int </span> </li>
                <li><span class="li-required">is_ha_member</span> - Is the specified device an HA member. <span class="li-normal">type: boolean </span> </li>
                
            </ul>
        
        </li>
        disk_cifs_raw
        <li><span class="li-head">disk_cifs_raw</span> - Log data for the given log type in raw format. 
        <ul class="ul-self">
                <li><span class="li-required">rows</span> - Number of rows to return. <span class="li-normal">type: int </span> </li>
                <li><span class="li-required">serial_no</span> - Retrieve log from the specified device. <span class="li-normal">type: string </span> </li>
                <li><span class="li-required">session_id</span> - Provide a session_id to continue getting data for that request. <span class="li-normal">type: int </span> </li>
                <li><span class="li-required">filter</span> - Filter expression(s). <span class="li-normal">type: string </span> </li>
                <li><span class="li-required">start</span> - Row number for the first row to return. <span class="li-normal">type: int </span> </li>
                <li><span class="li-required">is_ha_member</span> - Is the specified device an HA member. <span class="li-normal">type: boolean </span> </li>
                
            </ul>
        
        </li>
        disk_dlp_raw
        <li><span class="li-head">disk_dlp_raw</span> - Log data for the given log type in raw format. 
        <ul class="ul-self">
                <li><span class="li-required">rows</span> - Number of rows to return. <span class="li-normal">type: int </span> </li>
                <li><span class="li-required">serial_no</span> - Retrieve log from the specified device. <span class="li-normal">type: string </span> </li>
                <li><span class="li-required">session_id</span> - Provide a session_id to continue getting data for that request. <span class="li-normal">type: int </span> </li>
                <li><span class="li-required">filter</span> - Filter expression(s). <span class="li-normal">type: string </span> </li>
                <li><span class="li-required">start</span> - Row number for the first row to return. <span class="li-normal">type: int </span> </li>
                <li><span class="li-required">is_ha_member</span> - Is the specified device an HA member. <span class="li-normal">type: boolean </span> </li>
                
            </ul>
        
        </li>
        disk_dns_raw
        <li><span class="li-head">disk_dns_raw</span> - Log data for the given log type in raw format. 
        <ul class="ul-self">
                <li><span class="li-required">rows</span> - Number of rows to return. <span class="li-normal">type: int </span> </li>
                <li><span class="li-required">serial_no</span> - Retrieve log from the specified device. <span class="li-normal">type: string </span> </li>
                <li><span class="li-required">session_id</span> - Provide a session_id to continue getting data for that request. <span class="li-normal">type: int </span> </li>
                <li><span class="li-required">filter</span> - Filter expression(s). <span class="li-normal">type: string </span> </li>
                <li><span class="li-required">start</span> - Row number for the first row to return. <span class="li-normal">type: int </span> </li>
                <li><span class="li-required">is_ha_member</span> - Is the specified device an HA member. <span class="li-normal">type: boolean </span> </li>
                
            </ul>
        
        </li>
        disk_emailfilter_raw
        <li><span class="li-head">disk_emailfilter_raw</span> - Log data for the given log type in raw format. 
        <ul class="ul-self">
                <li><span class="li-required">rows</span> - Number of rows to return. <span class="li-normal">type: int </span> </li>
                <li><span class="li-required">serial_no</span> - Retrieve log from the specified device. <span class="li-normal">type: string </span> </li>
                <li><span class="li-required">session_id</span> - Provide a session_id to continue getting data for that request. <span class="li-normal">type: int </span> </li>
                <li><span class="li-required">filter</span> - Filter expression(s). <span class="li-normal">type: string </span> </li>
                <li><span class="li-required">start</span> - Row number for the first row to return. <span class="li-normal">type: int </span> </li>
                <li><span class="li-required">is_ha_member</span> - Is the specified device an HA member. <span class="li-normal">type: boolean </span> </li>
                
            </ul>
        
        </li>
        disk_event_compliance-check
        <li><span class="li-head">disk_event_compliance-check</span> - Log data for the given log type (and subtype). Append '/raw' to retrieve in raw format. 
        <ul class="ul-self">
                <li><span class="li-required">rows</span> - Number of rows to return. <span class="li-normal">type: int </span> </li>
                <li><span class="li-required">extra</span> - Flag(s) for extra data to be included [reverse_lookup|country_id]. <span class="li-normal">type: string </span> </li>
                <li><span class="li-required">serial_no</span> - Retrieve log from the specified device. <span class="li-normal">type: string </span> </li>
                <li><span class="li-required">session_id</span> - Provide a session_id to continue getting data for that request. <span class="li-normal">type: int </span> </li>
                <li><span class="li-required">filter</span> - Filter expression(s). <span class="li-normal">type: string </span> </li>
                <li><span class="li-required">start</span> - Row number for the first row to return. <span class="li-normal">type: int </span> </li>
                <li><span class="li-required">is_ha_member</span> - Is the specified device an HA member. <span class="li-normal">type: boolean </span> </li>
                
            </ul>
        
        </li>
        disk_event_connector
        <li><span class="li-head">disk_event_connector</span> - Log data for the given log type (and subtype). Append '/raw' to retrieve in raw format. 
        <ul class="ul-self">
                <li><span class="li-required">rows</span> - Number of rows to return. <span class="li-normal">type: int </span> </li>
                <li><span class="li-required">extra</span> - Flag(s) for extra data to be included [reverse_lookup|country_id]. <span class="li-normal">type: string </span> </li>
                <li><span class="li-required">serial_no</span> - Retrieve log from the specified device. <span class="li-normal">type: string </span> </li>
                <li><span class="li-required">session_id</span> - Provide a session_id to continue getting data for that request. <span class="li-normal">type: int </span> </li>
                <li><span class="li-required">filter</span> - Filter expression(s). <span class="li-normal">type: string </span> </li>
                <li><span class="li-required">start</span> - Row number for the first row to return. <span class="li-normal">type: int </span> </li>
                <li><span class="li-required">is_ha_member</span> - Is the specified device an HA member. <span class="li-normal">type: boolean </span> </li>
                
            </ul>
        
        </li>
        disk_event_endpoint
        <li><span class="li-head">disk_event_endpoint</span> - Log data for the given log type (and subtype). Append '/raw' to retrieve in raw format. 
        <ul class="ul-self">
                <li><span class="li-required">rows</span> - Number of rows to return. <span class="li-normal">type: int </span> </li>
                <li><span class="li-required">extra</span> - Flag(s) for extra data to be included [reverse_lookup|country_id]. <span class="li-normal">type: string </span> </li>
                <li><span class="li-required">serial_no</span> - Retrieve log from the specified device. <span class="li-normal">type: string </span> </li>
                <li><span class="li-required">session_id</span> - Provide a session_id to continue getting data for that request. <span class="li-normal">type: int </span> </li>
                <li><span class="li-required">filter</span> - Filter expression(s). <span class="li-normal">type: string </span> </li>
                <li><span class="li-required">start</span> - Row number for the first row to return. <span class="li-normal">type: int </span> </li>
                <li><span class="li-required">is_ha_member</span> - Is the specified device an HA member. <span class="li-normal">type: boolean </span> </li>
                
            </ul>
        
        </li>
        disk_event_fortiextender
        <li><span class="li-head">disk_event_fortiextender</span> - Log data for the given log type (and subtype). Append '/raw' to retrieve in raw format. 
        <ul class="ul-self">
                <li><span class="li-required">rows</span> - Number of rows to return. <span class="li-normal">type: int </span> </li>
                <li><span class="li-required">extra</span> - Flag(s) for extra data to be included [reverse_lookup|country_id]. <span class="li-normal">type: string </span> </li>
                <li><span class="li-required">serial_no</span> - Retrieve log from the specified device. <span class="li-normal">type: string </span> </li>
                <li><span class="li-required">session_id</span> - Provide a session_id to continue getting data for that request. <span class="li-normal">type: int </span> </li>
                <li><span class="li-required">filter</span> - Filter expression(s). <span class="li-normal">type: string </span> </li>
                <li><span class="li-required">start</span> - Row number for the first row to return. <span class="li-normal">type: int </span> </li>
                <li><span class="li-required">is_ha_member</span> - Is the specified device an HA member. <span class="li-normal">type: boolean </span> </li>
                
            </ul>
        
        </li>
        disk_event_ha
        <li><span class="li-head">disk_event_ha</span> - Log data for the given log type (and subtype). Append '/raw' to retrieve in raw format. 
        <ul class="ul-self">
                <li><span class="li-required">rows</span> - Number of rows to return. <span class="li-normal">type: int </span> </li>
                <li><span class="li-required">extra</span> - Flag(s) for extra data to be included [reverse_lookup|country_id]. <span class="li-normal">type: string </span> </li>
                <li><span class="li-required">serial_no</span> - Retrieve log from the specified device. <span class="li-normal">type: string </span> </li>
                <li><span class="li-required">session_id</span> - Provide a session_id to continue getting data for that request. <span class="li-normal">type: int </span> </li>
                <li><span class="li-required">filter</span> - Filter expression(s). <span class="li-normal">type: string </span> </li>
                <li><span class="li-required">start</span> - Row number for the first row to return. <span class="li-normal">type: int </span> </li>
                <li><span class="li-required">is_ha_member</span> - Is the specified device an HA member. <span class="li-normal">type: boolean </span> </li>
                
            </ul>
        
        </li>
        disk_event_router
        <li><span class="li-head">disk_event_router</span> - Log data for the given log type (and subtype). Append '/raw' to retrieve in raw format. 
        <ul class="ul-self">
                <li><span class="li-required">rows</span> - Number of rows to return. <span class="li-normal">type: int </span> </li>
                <li><span class="li-required">extra</span> - Flag(s) for extra data to be included [reverse_lookup|country_id]. <span class="li-normal">type: string </span> </li>
                <li><span class="li-required">serial_no</span> - Retrieve log from the specified device. <span class="li-normal">type: string </span> </li>
                <li><span class="li-required">session_id</span> - Provide a session_id to continue getting data for that request. <span class="li-normal">type: int </span> </li>
                <li><span class="li-required">filter</span> - Filter expression(s). <span class="li-normal">type: string </span> </li>
                <li><span class="li-required">start</span> - Row number for the first row to return. <span class="li-normal">type: int </span> </li>
                <li><span class="li-required">is_ha_member</span> - Is the specified device an HA member. <span class="li-normal">type: boolean </span> </li>
                
            </ul>
        
        </li>
        disk_event_security-rating
        <li><span class="li-head">disk_event_security-rating</span> - Log data for the given log type (and subtype). Append '/raw' to retrieve in raw format. 
        <ul class="ul-self">
                <li><span class="li-required">rows</span> - Number of rows to return. <span class="li-normal">type: int </span> </li>
                <li><span class="li-required">extra</span> - Flag(s) for extra data to be included [reverse_lookup|country_id]. <span class="li-normal">type: string </span> </li>
                <li><span class="li-required">serial_no</span> - Retrieve log from the specified device. <span class="li-normal">type: string </span> </li>
                <li><span class="li-required">session_id</span> - Provide a session_id to continue getting data for that request. <span class="li-normal">type: int </span> </li>
                <li><span class="li-required">filter</span> - Filter expression(s). <span class="li-normal">type: string </span> </li>
                <li><span class="li-required">start</span> - Row number for the first row to return. <span class="li-normal">type: int </span> </li>
                <li><span class="li-required">is_ha_member</span> - Is the specified device an HA member. <span class="li-normal">type: boolean </span> </li>
                
            </ul>
        
        </li>
        disk_event_system
        <li><span class="li-head">disk_event_system</span> - Log data for the given log type (and subtype). Append '/raw' to retrieve in raw format. 
        <ul class="ul-self">
                <li><span class="li-required">rows</span> - Number of rows to return. <span class="li-normal">type: int </span> </li>
                <li><span class="li-required">extra</span> - Flag(s) for extra data to be included [reverse_lookup|country_id]. <span class="li-normal">type: string </span> </li>
                <li><span class="li-required">serial_no</span> - Retrieve log from the specified device. <span class="li-normal">type: string </span> </li>
                <li><span class="li-required">session_id</span> - Provide a session_id to continue getting data for that request. <span class="li-normal">type: int </span> </li>
                <li><span class="li-required">filter</span> - Filter expression(s). <span class="li-normal">type: string </span> </li>
                <li><span class="li-required">start</span> - Row number for the first row to return. <span class="li-normal">type: int </span> </li>
                <li><span class="li-required">is_ha_member</span> - Is the specified device an HA member. <span class="li-normal">type: boolean </span> </li>
                
            </ul>
        
        </li>
        disk_event_user
        <li><span class="li-head">disk_event_user</span> - Log data for the given log type (and subtype). Append '/raw' to retrieve in raw format. 
        <ul class="ul-self">
                <li><span class="li-required">rows</span> - Number of rows to return. <span class="li-normal">type: int </span> </li>
                <li><span class="li-required">extra</span> - Flag(s) for extra data to be included [reverse_lookup|country_id]. <span class="li-normal">type: string </span> </li>
                <li><span class="li-required">serial_no</span> - Retrieve log from the specified device. <span class="li-normal">type: string </span> </li>
                <li><span class="li-required">session_id</span> - Provide a session_id to continue getting data for that request. <span class="li-normal">type: int </span> </li>
                <li><span class="li-required">filter</span> - Filter expression(s). <span class="li-normal">type: string </span> </li>
                <li><span class="li-required">start</span> - Row number for the first row to return. <span class="li-normal">type: int </span> </li>
                <li><span class="li-required">is_ha_member</span> - Is the specified device an HA member. <span class="li-normal">type: boolean </span> </li>
                
            </ul>
        
        </li>
        disk_event_vpn
        <li><span class="li-head">disk_event_vpn</span> - Log data for the given log type (and subtype). Append '/raw' to retrieve in raw format. 
        <ul class="ul-self">
                <li><span class="li-required">rows</span> - Number of rows to return. <span class="li-normal">type: int </span> </li>
                <li><span class="li-required">extra</span> - Flag(s) for extra data to be included [reverse_lookup|country_id]. <span class="li-normal">type: string </span> </li>
                <li><span class="li-required">serial_no</span> - Retrieve log from the specified device. <span class="li-normal">type: string </span> </li>
                <li><span class="li-required">session_id</span> - Provide a session_id to continue getting data for that request. <span class="li-normal">type: int </span> </li>
                <li><span class="li-required">filter</span> - Filter expression(s). <span class="li-normal">type: string </span> </li>
                <li><span class="li-required">start</span> - Row number for the first row to return. <span class="li-normal">type: int </span> </li>
                <li><span class="li-required">is_ha_member</span> - Is the specified device an HA member. <span class="li-normal">type: boolean </span> </li>
                
            </ul>
        
        </li>
        disk_event_wad
        <li><span class="li-head">disk_event_wad</span> - Log data for the given log type (and subtype). Append '/raw' to retrieve in raw format. 
        <ul class="ul-self">
                <li><span class="li-required">rows</span> - Number of rows to return. <span class="li-normal">type: int </span> </li>
                <li><span class="li-required">extra</span> - Flag(s) for extra data to be included [reverse_lookup|country_id]. <span class="li-normal">type: string </span> </li>
                <li><span class="li-required">serial_no</span> - Retrieve log from the specified device. <span class="li-normal">type: string </span> </li>
                <li><span class="li-required">session_id</span> - Provide a session_id to continue getting data for that request. <span class="li-normal">type: int </span> </li>
                <li><span class="li-required">filter</span> - Filter expression(s). <span class="li-normal">type: string </span> </li>
                <li><span class="li-required">start</span> - Row number for the first row to return. <span class="li-normal">type: int </span> </li>
                <li><span class="li-required">is_ha_member</span> - Is the specified device an HA member. <span class="li-normal">type: boolean </span> </li>
                
            </ul>
        
        </li>
        disk_event_wireless
        <li><span class="li-head">disk_event_wireless</span> - Log data for the given log type (and subtype). Append '/raw' to retrieve in raw format. 
        <ul class="ul-self">
                <li><span class="li-required">rows</span> - Number of rows to return. <span class="li-normal">type: int </span> </li>
                <li><span class="li-required">extra</span> - Flag(s) for extra data to be included [reverse_lookup|country_id]. <span class="li-normal">type: string </span> </li>
                <li><span class="li-required">serial_no</span> - Retrieve log from the specified device. <span class="li-normal">type: string </span> </li>
                <li><span class="li-required">session_id</span> - Provide a session_id to continue getting data for that request. <span class="li-normal">type: int </span> </li>
                <li><span class="li-required">filter</span> - Filter expression(s). <span class="li-normal">type: string </span> </li>
                <li><span class="li-required">start</span> - Row number for the first row to return. <span class="li-normal">type: int </span> </li>
                <li><span class="li-required">is_ha_member</span> - Is the specified device an HA member. <span class="li-normal">type: boolean </span> </li>
                
            </ul>
        
        </li>
        disk_file-filter_raw
        <li><span class="li-head">disk_file-filter_raw</span> - Log data for the given log type in raw format. 
        <ul class="ul-self">
                <li><span class="li-required">rows</span> - Number of rows to return. <span class="li-normal">type: int </span> </li>
                <li><span class="li-required">serial_no</span> - Retrieve log from the specified device. <span class="li-normal">type: string </span> </li>
                <li><span class="li-required">session_id</span> - Provide a session_id to continue getting data for that request. <span class="li-normal">type: int </span> </li>
                <li><span class="li-required">filter</span> - Filter expression(s). <span class="li-normal">type: string </span> </li>
                <li><span class="li-required">start</span> - Row number for the first row to return. <span class="li-normal">type: int </span> </li>
                <li><span class="li-required">is_ha_member</span> - Is the specified device an HA member. <span class="li-normal">type: boolean </span> </li>
                
            </ul>
        
        </li>
        disk_gtp_raw
        <li><span class="li-head">disk_gtp_raw</span> - Log data for the given log type in raw format. 
        <ul class="ul-self">
                <li><span class="li-required">rows</span> - Number of rows to return. <span class="li-normal">type: int </span> </li>
                <li><span class="li-required">serial_no</span> - Retrieve log from the specified device. <span class="li-normal">type: string </span> </li>
                <li><span class="li-required">session_id</span> - Provide a session_id to continue getting data for that request. <span class="li-normal">type: int </span> </li>
                <li><span class="li-required">filter</span> - Filter expression(s). <span class="li-normal">type: string </span> </li>
                <li><span class="li-required">start</span> - Row number for the first row to return. <span class="li-normal">type: int </span> </li>
                <li><span class="li-required">is_ha_member</span> - Is the specified device an HA member. <span class="li-normal">type: boolean </span> </li>
                
            </ul>
        
        </li>
        disk_ips_archive
        <li><span class="li-head">disk_ips_archive</span> - Return a list of archived items for the desired type. :type can be app-ctrl or ips 
        <ul class="ul-self">
                <li><span class="li-required">roll</span> - Log roll number. (required if source is not fortianalyzer) <span class="li-normal">type: int </span> </li>
                <li><span class="li-required">mkey</span> - Archive identifier. <span class="li-normal">type: int </span> </li>
                
            </ul>
        
        </li>
        disk_ips_archive-download
        <li><span class="li-head">disk_ips_archive-download</span> - Download an archived file. 
        <ul class="ul-self">
                <li><span class="li-required">roll</span> - Log roll number (required if source is not fortianalyzer). <span class="li-normal">type: int </span> </li>
                <li><span class="li-required">mkey</span> - Archive identifier. <span class="li-normal">type: int </span> </li>
                <li><span class="li-required">filename</span> - File name to use when saving the file in the browser. <span class="li-normal">type: string </span> </li>
                
            </ul>
        
        </li>
        disk_ips_raw
        <li><span class="li-head">disk_ips_raw</span> - Log data for the given log type in raw format. 
        <ul class="ul-self">
                <li><span class="li-required">rows</span> - Number of rows to return. <span class="li-normal">type: int </span> </li>
                <li><span class="li-required">serial_no</span> - Retrieve log from the specified device. <span class="li-normal">type: string </span> </li>
                <li><span class="li-required">session_id</span> - Provide a session_id to continue getting data for that request. <span class="li-normal">type: int </span> </li>
                <li><span class="li-required">filter</span> - Filter expression(s). <span class="li-normal">type: string </span> </li>
                <li><span class="li-required">start</span> - Row number for the first row to return. <span class="li-normal">type: int </span> </li>
                <li><span class="li-required">is_ha_member</span> - Is the specified device an HA member. <span class="li-normal">type: boolean </span> </li>
                
            </ul>
        
        </li>
        disk_ssh_raw
        <li><span class="li-head">disk_ssh_raw</span> - Log data for the given log type in raw format. 
        <ul class="ul-self">
                <li><span class="li-required">rows</span> - Number of rows to return. <span class="li-normal">type: int </span> </li>
                <li><span class="li-required">serial_no</span> - Retrieve log from the specified device. <span class="li-normal">type: string </span> </li>
                <li><span class="li-required">session_id</span> - Provide a session_id to continue getting data for that request. <span class="li-normal">type: int </span> </li>
                <li><span class="li-required">filter</span> - Filter expression(s). <span class="li-normal">type: string </span> </li>
                <li><span class="li-required">start</span> - Row number for the first row to return. <span class="li-normal">type: int </span> </li>
                <li><span class="li-required">is_ha_member</span> - Is the specified device an HA member. <span class="li-normal">type: boolean </span> </li>
                
            </ul>
        
        </li>
        disk_ssl_raw
        <li><span class="li-head">disk_ssl_raw</span> - Log data for the given log type in raw format. 
        <ul class="ul-self">
                <li><span class="li-required">rows</span> - Number of rows to return. <span class="li-normal">type: int </span> </li>
                <li><span class="li-required">serial_no</span> - Retrieve log from the specified device. <span class="li-normal">type: string </span> </li>
                <li><span class="li-required">session_id</span> - Provide a session_id to continue getting data for that request. <span class="li-normal">type: int </span> </li>
                <li><span class="li-required">filter</span> - Filter expression(s). <span class="li-normal">type: string </span> </li>
                <li><span class="li-required">start</span> - Row number for the first row to return. <span class="li-normal">type: int </span> </li>
                <li><span class="li-required">is_ha_member</span> - Is the specified device an HA member. <span class="li-normal">type: boolean </span> </li>
                
            </ul>
        
        </li>
        disk_traffic_fortiview
        <li><span class="li-head">disk_traffic_fortiview</span> - Log data for the given log type (and subtype). Append '/raw' to retrieve in raw format. 
        <ul class="ul-self">
                <li><span class="li-required">rows</span> - Number of rows to return. <span class="li-normal">type: int </span> </li>
                <li><span class="li-required">extra</span> - Flag(s) for extra data to be included [reverse_lookup|country_id]. <span class="li-normal">type: string </span> </li>
                <li><span class="li-required">serial_no</span> - Retrieve log from the specified device. <span class="li-normal">type: string </span> </li>
                <li><span class="li-required">session_id</span> - Provide a session_id to continue getting data for that request. <span class="li-normal">type: int </span> </li>
                <li><span class="li-required">filter</span> - Filter expression(s). <span class="li-normal">type: string </span> </li>
                <li><span class="li-required">start</span> - Row number for the first row to return. <span class="li-normal">type: int </span> </li>
                <li><span class="li-required">is_ha_member</span> - Is the specified device an HA member. <span class="li-normal">type: boolean </span> </li>
                
            </ul>
        
        </li>
        disk_traffic_forward
        <li><span class="li-head">disk_traffic_forward</span> - Log data for the given log type (and subtype). Append '/raw' to retrieve in raw format. 
        <ul class="ul-self">
                <li><span class="li-required">rows</span> - Number of rows to return. <span class="li-normal">type: int </span> </li>
                <li><span class="li-required">extra</span> - Flag(s) for extra data to be included [reverse_lookup|country_id]. <span class="li-normal">type: string </span> </li>
                <li><span class="li-required">serial_no</span> - Retrieve log from the specified device. <span class="li-normal">type: string </span> </li>
                <li><span class="li-required">session_id</span> - Provide a session_id to continue getting data for that request. <span class="li-normal">type: int </span> </li>
                <li><span class="li-required">filter</span> - Filter expression(s). <span class="li-normal">type: string </span> </li>
                <li><span class="li-required">start</span> - Row number for the first row to return. <span class="li-normal">type: int </span> </li>
                <li><span class="li-required">is_ha_member</span> - Is the specified device an HA member. <span class="li-normal">type: boolean </span> </li>
                
            </ul>
        
        </li>
        disk_traffic_local
        <li><span class="li-head">disk_traffic_local</span> - Log data for the given log type (and subtype). Append '/raw' to retrieve in raw format. 
        <ul class="ul-self">
                <li><span class="li-required">rows</span> - Number of rows to return. <span class="li-normal">type: int </span> </li>
                <li><span class="li-required">extra</span> - Flag(s) for extra data to be included [reverse_lookup|country_id]. <span class="li-normal">type: string </span> </li>
                <li><span class="li-required">serial_no</span> - Retrieve log from the specified device. <span class="li-normal">type: string </span> </li>
                <li><span class="li-required">session_id</span> - Provide a session_id to continue getting data for that request. <span class="li-normal">type: int </span> </li>
                <li><span class="li-required">filter</span> - Filter expression(s). <span class="li-normal">type: string </span> </li>
                <li><span class="li-required">start</span> - Row number for the first row to return. <span class="li-normal">type: int </span> </li>
                <li><span class="li-required">is_ha_member</span> - Is the specified device an HA member. <span class="li-normal">type: boolean </span> </li>
                
            </ul>
        
        </li>
        disk_traffic_multicast
        <li><span class="li-head">disk_traffic_multicast</span> - Log data for the given log type (and subtype). Append '/raw' to retrieve in raw format. 
        <ul class="ul-self">
                <li><span class="li-required">rows</span> - Number of rows to return. <span class="li-normal">type: int </span> </li>
                <li><span class="li-required">extra</span> - Flag(s) for extra data to be included [reverse_lookup|country_id]. <span class="li-normal">type: string </span> </li>
                <li><span class="li-required">serial_no</span> - Retrieve log from the specified device. <span class="li-normal">type: string </span> </li>
                <li><span class="li-required">session_id</span> - Provide a session_id to continue getting data for that request. <span class="li-normal">type: int </span> </li>
                <li><span class="li-required">filter</span> - Filter expression(s). <span class="li-normal">type: string </span> </li>
                <li><span class="li-required">start</span> - Row number for the first row to return. <span class="li-normal">type: int </span> </li>
                <li><span class="li-required">is_ha_member</span> - Is the specified device an HA member. <span class="li-normal">type: boolean </span> </li>
                
            </ul>
        
        </li>
        disk_traffic_sniffer
        <li><span class="li-head">disk_traffic_sniffer</span> - Log data for the given log type (and subtype). Append '/raw' to retrieve in raw format. 
        <ul class="ul-self">
                <li><span class="li-required">rows</span> - Number of rows to return. <span class="li-normal">type: int </span> </li>
                <li><span class="li-required">extra</span> - Flag(s) for extra data to be included [reverse_lookup|country_id]. <span class="li-normal">type: string </span> </li>
                <li><span class="li-required">serial_no</span> - Retrieve log from the specified device. <span class="li-normal">type: string </span> </li>
                <li><span class="li-required">session_id</span> - Provide a session_id to continue getting data for that request. <span class="li-normal">type: int </span> </li>
                <li><span class="li-required">filter</span> - Filter expression(s). <span class="li-normal">type: string </span> </li>
                <li><span class="li-required">start</span> - Row number for the first row to return. <span class="li-normal">type: int </span> </li>
                <li><span class="li-required">is_ha_member</span> - Is the specified device an HA member. <span class="li-normal">type: boolean </span> </li>
                
            </ul>
        
        </li>
        disk_traffic_threat
        <li><span class="li-head">disk_traffic_threat</span> - Log data for the given log type (and subtype). Append '/raw' to retrieve in raw format. 
        <ul class="ul-self">
                <li><span class="li-required">rows</span> - Number of rows to return. <span class="li-normal">type: int </span> </li>
                <li><span class="li-required">extra</span> - Flag(s) for extra data to be included [reverse_lookup|country_id]. <span class="li-normal">type: string </span> </li>
                <li><span class="li-required">serial_no</span> - Retrieve log from the specified device. <span class="li-normal">type: string </span> </li>
                <li><span class="li-required">session_id</span> - Provide a session_id to continue getting data for that request. <span class="li-normal">type: int </span> </li>
                <li><span class="li-required">filter</span> - Filter expression(s). <span class="li-normal">type: string </span> </li>
                <li><span class="li-required">start</span> - Row number for the first row to return. <span class="li-normal">type: int </span> </li>
                <li><span class="li-required">is_ha_member</span> - Is the specified device an HA member. <span class="li-normal">type: boolean </span> </li>
                
            </ul>
        
        </li>
        disk_virus_archive
        <li><span class="li-head">disk_virus_archive</span> - Return a description of the quarantined virus file. 
        <ul class="ul-self">
                <li><span class="li-required">mkey</span> - checksum column from the virus log. <span class="li-normal">type: int </span> </li>
                <li><span class="li-required">filename</span> - Filename of the antivirus archive. (virus type only) <span class="li-normal">type: string </span> </li>
                
            </ul>
        
        </li>
        disk_virus_raw
        <li><span class="li-head">disk_virus_raw</span> - Log data for the given log type in raw format. 
        <ul class="ul-self">
                <li><span class="li-required">rows</span> - Number of rows to return. <span class="li-normal">type: int </span> </li>
                <li><span class="li-required">serial_no</span> - Retrieve log from the specified device. <span class="li-normal">type: string </span> </li>
                <li><span class="li-required">session_id</span> - Provide a session_id to continue getting data for that request. <span class="li-normal">type: int </span> </li>
                <li><span class="li-required">filter</span> - Filter expression(s). <span class="li-normal">type: string </span> </li>
                <li><span class="li-required">start</span> - Row number for the first row to return. <span class="li-normal">type: int </span> </li>
                <li><span class="li-required">is_ha_member</span> - Is the specified device an HA member. <span class="li-normal">type: boolean </span> </li>
                
            </ul>
        
        </li>
        disk_voip_raw
        <li><span class="li-head">disk_voip_raw</span> - Log data for the given log type in raw format. 
        <ul class="ul-self">
                <li><span class="li-required">rows</span> - Number of rows to return. <span class="li-normal">type: int </span> </li>
                <li><span class="li-required">serial_no</span> - Retrieve log from the specified device. <span class="li-normal">type: string </span> </li>
                <li><span class="li-required">session_id</span> - Provide a session_id to continue getting data for that request. <span class="li-normal">type: int </span> </li>
                <li><span class="li-required">filter</span> - Filter expression(s). <span class="li-normal">type: string </span> </li>
                <li><span class="li-required">start</span> - Row number for the first row to return. <span class="li-normal">type: int </span> </li>
                <li><span class="li-required">is_ha_member</span> - Is the specified device an HA member. <span class="li-normal">type: boolean </span> </li>
                
            </ul>
        
        </li>
        disk_waf_raw
        <li><span class="li-head">disk_waf_raw</span> - Log data for the given log type in raw format. 
        <ul class="ul-self">
                <li><span class="li-required">rows</span> - Number of rows to return. <span class="li-normal">type: int </span> </li>
                <li><span class="li-required">serial_no</span> - Retrieve log from the specified device. <span class="li-normal">type: string </span> </li>
                <li><span class="li-required">session_id</span> - Provide a session_id to continue getting data for that request. <span class="li-normal">type: int </span> </li>
                <li><span class="li-required">filter</span> - Filter expression(s). <span class="li-normal">type: string </span> </li>
                <li><span class="li-required">start</span> - Row number for the first row to return. <span class="li-normal">type: int </span> </li>
                <li><span class="li-required">is_ha_member</span> - Is the specified device an HA member. <span class="li-normal">type: boolean </span> </li>
                
            </ul>
        
        </li>
        disk_webfilter_raw
        <li><span class="li-head">disk_webfilter_raw</span> - Log data for the given log type in raw format. 
        <ul class="ul-self">
                <li><span class="li-required">rows</span> - Number of rows to return. <span class="li-normal">type: int </span> </li>
                <li><span class="li-required">serial_no</span> - Retrieve log from the specified device. <span class="li-normal">type: string </span> </li>
                <li><span class="li-required">session_id</span> - Provide a session_id to continue getting data for that request. <span class="li-normal">type: int </span> </li>
                <li><span class="li-required">filter</span> - Filter expression(s). <span class="li-normal">type: string </span> </li>
                <li><span class="li-required">start</span> - Row number for the first row to return. <span class="li-normal">type: int </span> </li>
                <li><span class="li-required">is_ha_member</span> - Is the specified device an HA member. <span class="li-normal">type: boolean </span> </li>
                
            </ul>
        
        </li>
        fortianalyzer_anomaly_raw
        <li><span class="li-head">fortianalyzer_anomaly_raw</span> - Log data for the given log type in raw format. 
        <ul class="ul-self">
                <li><span class="li-required">rows</span> - Number of rows to return. <span class="li-normal">type: int </span> </li>
                <li><span class="li-required">serial_no</span> - Retrieve log from the specified device. <span class="li-normal">type: string </span> </li>
                <li><span class="li-required">session_id</span> - Provide a session_id to continue getting data for that request. <span class="li-normal">type: int </span> </li>
                <li><span class="li-required">filter</span> - Filter expression(s). <span class="li-normal">type: string </span> </li>
                <li><span class="li-required">start</span> - Row number for the first row to return. <span class="li-normal">type: int </span> </li>
                <li><span class="li-required">is_ha_member</span> - Is the specified device an HA member. <span class="li-normal">type: boolean </span> </li>
                
            </ul>
        
        </li>
        fortianalyzer_app-ctrl_archive
        <li><span class="li-head">fortianalyzer_app-ctrl_archive</span> - Return a list of archived items for the desired type. :type can be app-ctrl or ips 
        <ul class="ul-self">
                <li><span class="li-required">roll</span> - Log roll number. (required if source is not fortianalyzer) <span class="li-normal">type: int </span> </li>
                <li><span class="li-required">mkey</span> - Archive identifier. <span class="li-normal">type: int </span> </li>
                
            </ul>
        
        </li>
        fortianalyzer_app-ctrl_archive-download
        <li><span class="li-head">fortianalyzer_app-ctrl_archive-download</span> - Download an archived file. 
        <ul class="ul-self">
                <li><span class="li-required">roll</span> - Log roll number (required if source is not fortianalyzer). <span class="li-normal">type: int </span> </li>
                <li><span class="li-required">mkey</span> - Archive identifier. <span class="li-normal">type: int </span> </li>
                <li><span class="li-required">filename</span> - File name to use when saving the file in the browser. <span class="li-normal">type: string </span> </li>
                
            </ul>
        
        </li>
        fortianalyzer_app-ctrl_raw
        <li><span class="li-head">fortianalyzer_app-ctrl_raw</span> - Log data for the given log type in raw format. 
        <ul class="ul-self">
                <li><span class="li-required">rows</span> - Number of rows to return. <span class="li-normal">type: int </span> </li>
                <li><span class="li-required">serial_no</span> - Retrieve log from the specified device. <span class="li-normal">type: string </span> </li>
                <li><span class="li-required">session_id</span> - Provide a session_id to continue getting data for that request. <span class="li-normal">type: int </span> </li>
                <li><span class="li-required">filter</span> - Filter expression(s). <span class="li-normal">type: string </span> </li>
                <li><span class="li-required">start</span> - Row number for the first row to return. <span class="li-normal">type: int </span> </li>
                <li><span class="li-required">is_ha_member</span> - Is the specified device an HA member. <span class="li-normal">type: boolean </span> </li>
                
            </ul>
        
        </li>
        fortianalyzer_cifs_raw
        <li><span class="li-head">fortianalyzer_cifs_raw</span> - Log data for the given log type in raw format. 
        <ul class="ul-self">
                <li><span class="li-required">rows</span> - Number of rows to return. <span class="li-normal">type: int </span> </li>
                <li><span class="li-required">serial_no</span> - Retrieve log from the specified device. <span class="li-normal">type: string </span> </li>
                <li><span class="li-required">session_id</span> - Provide a session_id to continue getting data for that request. <span class="li-normal">type: int </span> </li>
                <li><span class="li-required">filter</span> - Filter expression(s). <span class="li-normal">type: string </span> </li>
                <li><span class="li-required">start</span> - Row number for the first row to return. <span class="li-normal">type: int </span> </li>
                <li><span class="li-required">is_ha_member</span> - Is the specified device an HA member. <span class="li-normal">type: boolean </span> </li>
                
            </ul>
        
        </li>
        fortianalyzer_dlp_raw
        <li><span class="li-head">fortianalyzer_dlp_raw</span> - Log data for the given log type in raw format. 
        <ul class="ul-self">
                <li><span class="li-required">rows</span> - Number of rows to return. <span class="li-normal">type: int </span> </li>
                <li><span class="li-required">serial_no</span> - Retrieve log from the specified device. <span class="li-normal">type: string </span> </li>
                <li><span class="li-required">session_id</span> - Provide a session_id to continue getting data for that request. <span class="li-normal">type: int </span> </li>
                <li><span class="li-required">filter</span> - Filter expression(s). <span class="li-normal">type: string </span> </li>
                <li><span class="li-required">start</span> - Row number for the first row to return. <span class="li-normal">type: int </span> </li>
                <li><span class="li-required">is_ha_member</span> - Is the specified device an HA member. <span class="li-normal">type: boolean </span> </li>
                
            </ul>
        
        </li>
        fortianalyzer_dns_raw
        <li><span class="li-head">fortianalyzer_dns_raw</span> - Log data for the given log type in raw format. 
        <ul class="ul-self">
                <li><span class="li-required">rows</span> - Number of rows to return. <span class="li-normal">type: int </span> </li>
                <li><span class="li-required">serial_no</span> - Retrieve log from the specified device. <span class="li-normal">type: string </span> </li>
                <li><span class="li-required">session_id</span> - Provide a session_id to continue getting data for that request. <span class="li-normal">type: int </span> </li>
                <li><span class="li-required">filter</span> - Filter expression(s). <span class="li-normal">type: string </span> </li>
                <li><span class="li-required">start</span> - Row number for the first row to return. <span class="li-normal">type: int </span> </li>
                <li><span class="li-required">is_ha_member</span> - Is the specified device an HA member. <span class="li-normal">type: boolean </span> </li>
                
            </ul>
        
        </li>
        fortianalyzer_emailfilter_raw
        <li><span class="li-head">fortianalyzer_emailfilter_raw</span> - Log data for the given log type in raw format. 
        <ul class="ul-self">
                <li><span class="li-required">rows</span> - Number of rows to return. <span class="li-normal">type: int </span> </li>
                <li><span class="li-required">serial_no</span> - Retrieve log from the specified device. <span class="li-normal">type: string </span> </li>
                <li><span class="li-required">session_id</span> - Provide a session_id to continue getting data for that request. <span class="li-normal">type: int </span> </li>
                <li><span class="li-required">filter</span> - Filter expression(s). <span class="li-normal">type: string </span> </li>
                <li><span class="li-required">start</span> - Row number for the first row to return. <span class="li-normal">type: int </span> </li>
                <li><span class="li-required">is_ha_member</span> - Is the specified device an HA member. <span class="li-normal">type: boolean </span> </li>
                
            </ul>
        
        </li>
        fortianalyzer_event_compliance-check
        <li><span class="li-head">fortianalyzer_event_compliance-check</span> - Log data for the given log type (and subtype). Append '/raw' to retrieve in raw format. 
        <ul class="ul-self">
                <li><span class="li-required">rows</span> - Number of rows to return. <span class="li-normal">type: int </span> </li>
                <li><span class="li-required">extra</span> - Flag(s) for extra data to be included [reverse_lookup|country_id]. <span class="li-normal">type: string </span> </li>
                <li><span class="li-required">serial_no</span> - Retrieve log from the specified device. <span class="li-normal">type: string </span> </li>
                <li><span class="li-required">session_id</span> - Provide a session_id to continue getting data for that request. <span class="li-normal">type: int </span> </li>
                <li><span class="li-required">filter</span> - Filter expression(s). <span class="li-normal">type: string </span> </li>
                <li><span class="li-required">start</span> - Row number for the first row to return. <span class="li-normal">type: int </span> </li>
                <li><span class="li-required">is_ha_member</span> - Is the specified device an HA member. <span class="li-normal">type: boolean </span> </li>
                
            </ul>
        
        </li>
        fortianalyzer_event_connector
        <li><span class="li-head">fortianalyzer_event_connector</span> - Log data for the given log type (and subtype). Append '/raw' to retrieve in raw format. 
        <ul class="ul-self">
                <li><span class="li-required">rows</span> - Number of rows to return. <span class="li-normal">type: int </span> </li>
                <li><span class="li-required">extra</span> - Flag(s) for extra data to be included [reverse_lookup|country_id]. <span class="li-normal">type: string </span> </li>
                <li><span class="li-required">serial_no</span> - Retrieve log from the specified device. <span class="li-normal">type: string </span> </li>
                <li><span class="li-required">session_id</span> - Provide a session_id to continue getting data for that request. <span class="li-normal">type: int </span> </li>
                <li><span class="li-required">filter</span> - Filter expression(s). <span class="li-normal">type: string </span> </li>
                <li><span class="li-required">start</span> - Row number for the first row to return. <span class="li-normal">type: int </span> </li>
                <li><span class="li-required">is_ha_member</span> - Is the specified device an HA member. <span class="li-normal">type: boolean </span> </li>
                
            </ul>
        
        </li>
        fortianalyzer_event_endpoint
        <li><span class="li-head">fortianalyzer_event_endpoint</span> - Log data for the given log type (and subtype). Append '/raw' to retrieve in raw format. 
        <ul class="ul-self">
                <li><span class="li-required">rows</span> - Number of rows to return. <span class="li-normal">type: int </span> </li>
                <li><span class="li-required">extra</span> - Flag(s) for extra data to be included [reverse_lookup|country_id]. <span class="li-normal">type: string </span> </li>
                <li><span class="li-required">serial_no</span> - Retrieve log from the specified device. <span class="li-normal">type: string </span> </li>
                <li><span class="li-required">session_id</span> - Provide a session_id to continue getting data for that request. <span class="li-normal">type: int </span> </li>
                <li><span class="li-required">filter</span> - Filter expression(s). <span class="li-normal">type: string </span> </li>
                <li><span class="li-required">start</span> - Row number for the first row to return. <span class="li-normal">type: int </span> </li>
                <li><span class="li-required">is_ha_member</span> - Is the specified device an HA member. <span class="li-normal">type: boolean </span> </li>
                
            </ul>
        
        </li>
        fortianalyzer_event_fortiextender
        <li><span class="li-head">fortianalyzer_event_fortiextender</span> - Log data for the given log type (and subtype). Append '/raw' to retrieve in raw format. 
        <ul class="ul-self">
                <li><span class="li-required">rows</span> - Number of rows to return. <span class="li-normal">type: int </span> </li>
                <li><span class="li-required">extra</span> - Flag(s) for extra data to be included [reverse_lookup|country_id]. <span class="li-normal">type: string </span> </li>
                <li><span class="li-required">serial_no</span> - Retrieve log from the specified device. <span class="li-normal">type: string </span> </li>
                <li><span class="li-required">session_id</span> - Provide a session_id to continue getting data for that request. <span class="li-normal">type: int </span> </li>
                <li><span class="li-required">filter</span> - Filter expression(s). <span class="li-normal">type: string </span> </li>
                <li><span class="li-required">start</span> - Row number for the first row to return. <span class="li-normal">type: int </span> </li>
                <li><span class="li-required">is_ha_member</span> - Is the specified device an HA member. <span class="li-normal">type: boolean </span> </li>
                
            </ul>
        
        </li>
        fortianalyzer_event_ha
        <li><span class="li-head">fortianalyzer_event_ha</span> - Log data for the given log type (and subtype). Append '/raw' to retrieve in raw format. 
        <ul class="ul-self">
                <li><span class="li-required">rows</span> - Number of rows to return. <span class="li-normal">type: int </span> </li>
                <li><span class="li-required">extra</span> - Flag(s) for extra data to be included [reverse_lookup|country_id]. <span class="li-normal">type: string </span> </li>
                <li><span class="li-required">serial_no</span> - Retrieve log from the specified device. <span class="li-normal">type: string </span> </li>
                <li><span class="li-required">session_id</span> - Provide a session_id to continue getting data for that request. <span class="li-normal">type: int </span> </li>
                <li><span class="li-required">filter</span> - Filter expression(s). <span class="li-normal">type: string </span> </li>
                <li><span class="li-required">start</span> - Row number for the first row to return. <span class="li-normal">type: int </span> </li>
                <li><span class="li-required">is_ha_member</span> - Is the specified device an HA member. <span class="li-normal">type: boolean </span> </li>
                
            </ul>
        
        </li>
        fortianalyzer_event_router
        <li><span class="li-head">fortianalyzer_event_router</span> - Log data for the given log type (and subtype). Append '/raw' to retrieve in raw format. 
        <ul class="ul-self">
                <li><span class="li-required">rows</span> - Number of rows to return. <span class="li-normal">type: int </span> </li>
                <li><span class="li-required">extra</span> - Flag(s) for extra data to be included [reverse_lookup|country_id]. <span class="li-normal">type: string </span> </li>
                <li><span class="li-required">serial_no</span> - Retrieve log from the specified device. <span class="li-normal">type: string </span> </li>
                <li><span class="li-required">session_id</span> - Provide a session_id to continue getting data for that request. <span class="li-normal">type: int </span> </li>
                <li><span class="li-required">filter</span> - Filter expression(s). <span class="li-normal">type: string </span> </li>
                <li><span class="li-required">start</span> - Row number for the first row to return. <span class="li-normal">type: int </span> </li>
                <li><span class="li-required">is_ha_member</span> - Is the specified device an HA member. <span class="li-normal">type: boolean </span> </li>
                
            </ul>
        
        </li>
        fortianalyzer_event_security-rating
        <li><span class="li-head">fortianalyzer_event_security-rating</span> - Log data for the given log type (and subtype). Append '/raw' to retrieve in raw format. 
        <ul class="ul-self">
                <li><span class="li-required">rows</span> - Number of rows to return. <span class="li-normal">type: int </span> </li>
                <li><span class="li-required">extra</span> - Flag(s) for extra data to be included [reverse_lookup|country_id]. <span class="li-normal">type: string </span> </li>
                <li><span class="li-required">serial_no</span> - Retrieve log from the specified device. <span class="li-normal">type: string </span> </li>
                <li><span class="li-required">session_id</span> - Provide a session_id to continue getting data for that request. <span class="li-normal">type: int </span> </li>
                <li><span class="li-required">filter</span> - Filter expression(s). <span class="li-normal">type: string </span> </li>
                <li><span class="li-required">start</span> - Row number for the first row to return. <span class="li-normal">type: int </span> </li>
                <li><span class="li-required">is_ha_member</span> - Is the specified device an HA member. <span class="li-normal">type: boolean </span> </li>
                
            </ul>
        
        </li>
        fortianalyzer_event_system
        <li><span class="li-head">fortianalyzer_event_system</span> - Log data for the given log type (and subtype). Append '/raw' to retrieve in raw format. 
        <ul class="ul-self">
                <li><span class="li-required">rows</span> - Number of rows to return. <span class="li-normal">type: int </span> </li>
                <li><span class="li-required">extra</span> - Flag(s) for extra data to be included [reverse_lookup|country_id]. <span class="li-normal">type: string </span> </li>
                <li><span class="li-required">serial_no</span> - Retrieve log from the specified device. <span class="li-normal">type: string </span> </li>
                <li><span class="li-required">session_id</span> - Provide a session_id to continue getting data for that request. <span class="li-normal">type: int </span> </li>
                <li><span class="li-required">filter</span> - Filter expression(s). <span class="li-normal">type: string </span> </li>
                <li><span class="li-required">start</span> - Row number for the first row to return. <span class="li-normal">type: int </span> </li>
                <li><span class="li-required">is_ha_member</span> - Is the specified device an HA member. <span class="li-normal">type: boolean </span> </li>
                
            </ul>
        
        </li>
        fortianalyzer_event_user
        <li><span class="li-head">fortianalyzer_event_user</span> - Log data for the given log type (and subtype). Append '/raw' to retrieve in raw format. 
        <ul class="ul-self">
                <li><span class="li-required">rows</span> - Number of rows to return. <span class="li-normal">type: int </span> </li>
                <li><span class="li-required">extra</span> - Flag(s) for extra data to be included [reverse_lookup|country_id]. <span class="li-normal">type: string </span> </li>
                <li><span class="li-required">serial_no</span> - Retrieve log from the specified device. <span class="li-normal">type: string </span> </li>
                <li><span class="li-required">session_id</span> - Provide a session_id to continue getting data for that request. <span class="li-normal">type: int </span> </li>
                <li><span class="li-required">filter</span> - Filter expression(s). <span class="li-normal">type: string </span> </li>
                <li><span class="li-required">start</span> - Row number for the first row to return. <span class="li-normal">type: int </span> </li>
                <li><span class="li-required">is_ha_member</span> - Is the specified device an HA member. <span class="li-normal">type: boolean </span> </li>
                
            </ul>
        
        </li>
        fortianalyzer_event_vpn
        <li><span class="li-head">fortianalyzer_event_vpn</span> - Log data for the given log type (and subtype). Append '/raw' to retrieve in raw format. 
        <ul class="ul-self">
                <li><span class="li-required">rows</span> - Number of rows to return. <span class="li-normal">type: int </span> </li>
                <li><span class="li-required">extra</span> - Flag(s) for extra data to be included [reverse_lookup|country_id]. <span class="li-normal">type: string </span> </li>
                <li><span class="li-required">serial_no</span> - Retrieve log from the specified device. <span class="li-normal">type: string </span> </li>
                <li><span class="li-required">session_id</span> - Provide a session_id to continue getting data for that request. <span class="li-normal">type: int </span> </li>
                <li><span class="li-required">filter</span> - Filter expression(s). <span class="li-normal">type: string </span> </li>
                <li><span class="li-required">start</span> - Row number for the first row to return. <span class="li-normal">type: int </span> </li>
                <li><span class="li-required">is_ha_member</span> - Is the specified device an HA member. <span class="li-normal">type: boolean </span> </li>
                
            </ul>
        
        </li>
        fortianalyzer_event_wad
        <li><span class="li-head">fortianalyzer_event_wad</span> - Log data for the given log type (and subtype). Append '/raw' to retrieve in raw format. 
        <ul class="ul-self">
                <li><span class="li-required">rows</span> - Number of rows to return. <span class="li-normal">type: int </span> </li>
                <li><span class="li-required">extra</span> - Flag(s) for extra data to be included [reverse_lookup|country_id]. <span class="li-normal">type: string </span> </li>
                <li><span class="li-required">serial_no</span> - Retrieve log from the specified device. <span class="li-normal">type: string </span> </li>
                <li><span class="li-required">session_id</span> - Provide a session_id to continue getting data for that request. <span class="li-normal">type: int </span> </li>
                <li><span class="li-required">filter</span> - Filter expression(s). <span class="li-normal">type: string </span> </li>
                <li><span class="li-required">start</span> - Row number for the first row to return. <span class="li-normal">type: int </span> </li>
                <li><span class="li-required">is_ha_member</span> - Is the specified device an HA member. <span class="li-normal">type: boolean </span> </li>
                
            </ul>
        
        </li>
        fortianalyzer_event_wireless
        <li><span class="li-head">fortianalyzer_event_wireless</span> - Log data for the given log type (and subtype). Append '/raw' to retrieve in raw format. 
        <ul class="ul-self">
                <li><span class="li-required">rows</span> - Number of rows to return. <span class="li-normal">type: int </span> </li>
                <li><span class="li-required">extra</span> - Flag(s) for extra data to be included [reverse_lookup|country_id]. <span class="li-normal">type: string </span> </li>
                <li><span class="li-required">serial_no</span> - Retrieve log from the specified device. <span class="li-normal">type: string </span> </li>
                <li><span class="li-required">session_id</span> - Provide a session_id to continue getting data for that request. <span class="li-normal">type: int </span> </li>
                <li><span class="li-required">filter</span> - Filter expression(s). <span class="li-normal">type: string </span> </li>
                <li><span class="li-required">start</span> - Row number for the first row to return. <span class="li-normal">type: int </span> </li>
                <li><span class="li-required">is_ha_member</span> - Is the specified device an HA member. <span class="li-normal">type: boolean </span> </li>
                
            </ul>
        
        </li>
        fortianalyzer_file-filter_raw
        <li><span class="li-head">fortianalyzer_file-filter_raw</span> - Log data for the given log type in raw format. 
        <ul class="ul-self">
                <li><span class="li-required">rows</span> - Number of rows to return. <span class="li-normal">type: int </span> </li>
                <li><span class="li-required">serial_no</span> - Retrieve log from the specified device. <span class="li-normal">type: string </span> </li>
                <li><span class="li-required">session_id</span> - Provide a session_id to continue getting data for that request. <span class="li-normal">type: int </span> </li>
                <li><span class="li-required">filter</span> - Filter expression(s). <span class="li-normal">type: string </span> </li>
                <li><span class="li-required">start</span> - Row number for the first row to return. <span class="li-normal">type: int </span> </li>
                <li><span class="li-required">is_ha_member</span> - Is the specified device an HA member. <span class="li-normal">type: boolean </span> </li>
                
            </ul>
        
        </li>
        fortianalyzer_gtp_raw
        <li><span class="li-head">fortianalyzer_gtp_raw</span> - Log data for the given log type in raw format. 
        <ul class="ul-self">
                <li><span class="li-required">rows</span> - Number of rows to return. <span class="li-normal">type: int </span> </li>
                <li><span class="li-required">serial_no</span> - Retrieve log from the specified device. <span class="li-normal">type: string </span> </li>
                <li><span class="li-required">session_id</span> - Provide a session_id to continue getting data for that request. <span class="li-normal">type: int </span> </li>
                <li><span class="li-required">filter</span> - Filter expression(s). <span class="li-normal">type: string </span> </li>
                <li><span class="li-required">start</span> - Row number for the first row to return. <span class="li-normal">type: int </span> </li>
                <li><span class="li-required">is_ha_member</span> - Is the specified device an HA member. <span class="li-normal">type: boolean </span> </li>
                
            </ul>
        
        </li>
        fortianalyzer_ips_archive
        <li><span class="li-head">fortianalyzer_ips_archive</span> - Return a list of archived items for the desired type. :type can be app-ctrl or ips 
        <ul class="ul-self">
                <li><span class="li-required">roll</span> - Log roll number. (required if source is not fortianalyzer) <span class="li-normal">type: int </span> </li>
                <li><span class="li-required">mkey</span> - Archive identifier. <span class="li-normal">type: int </span> </li>
                
            </ul>
        
        </li>
        fortianalyzer_ips_archive-download
        <li><span class="li-head">fortianalyzer_ips_archive-download</span> - Download an archived file. 
        <ul class="ul-self">
                <li><span class="li-required">roll</span> - Log roll number (required if source is not fortianalyzer). <span class="li-normal">type: int </span> </li>
                <li><span class="li-required">mkey</span> - Archive identifier. <span class="li-normal">type: int </span> </li>
                <li><span class="li-required">filename</span> - File name to use when saving the file in the browser. <span class="li-normal">type: string </span> </li>
                
            </ul>
        
        </li>
        fortianalyzer_ips_raw
        <li><span class="li-head">fortianalyzer_ips_raw</span> - Log data for the given log type in raw format. 
        <ul class="ul-self">
                <li><span class="li-required">rows</span> - Number of rows to return. <span class="li-normal">type: int </span> </li>
                <li><span class="li-required">serial_no</span> - Retrieve log from the specified device. <span class="li-normal">type: string </span> </li>
                <li><span class="li-required">session_id</span> - Provide a session_id to continue getting data for that request. <span class="li-normal">type: int </span> </li>
                <li><span class="li-required">filter</span> - Filter expression(s). <span class="li-normal">type: string </span> </li>
                <li><span class="li-required">start</span> - Row number for the first row to return. <span class="li-normal">type: int </span> </li>
                <li><span class="li-required">is_ha_member</span> - Is the specified device an HA member. <span class="li-normal">type: boolean </span> </li>
                
            </ul>
        
        </li>
        fortianalyzer_ssh_raw
        <li><span class="li-head">fortianalyzer_ssh_raw</span> - Log data for the given log type in raw format. 
        <ul class="ul-self">
                <li><span class="li-required">rows</span> - Number of rows to return. <span class="li-normal">type: int </span> </li>
                <li><span class="li-required">serial_no</span> - Retrieve log from the specified device. <span class="li-normal">type: string </span> </li>
                <li><span class="li-required">session_id</span> - Provide a session_id to continue getting data for that request. <span class="li-normal">type: int </span> </li>
                <li><span class="li-required">filter</span> - Filter expression(s). <span class="li-normal">type: string </span> </li>
                <li><span class="li-required">start</span> - Row number for the first row to return. <span class="li-normal">type: int </span> </li>
                <li><span class="li-required">is_ha_member</span> - Is the specified device an HA member. <span class="li-normal">type: boolean </span> </li>
                
            </ul>
        
        </li>
        fortianalyzer_ssl_raw
        <li><span class="li-head">fortianalyzer_ssl_raw</span> - Log data for the given log type in raw format. 
        <ul class="ul-self">
                <li><span class="li-required">rows</span> - Number of rows to return. <span class="li-normal">type: int </span> </li>
                <li><span class="li-required">serial_no</span> - Retrieve log from the specified device. <span class="li-normal">type: string </span> </li>
                <li><span class="li-required">session_id</span> - Provide a session_id to continue getting data for that request. <span class="li-normal">type: int </span> </li>
                <li><span class="li-required">filter</span> - Filter expression(s). <span class="li-normal">type: string </span> </li>
                <li><span class="li-required">start</span> - Row number for the first row to return. <span class="li-normal">type: int </span> </li>
                <li><span class="li-required">is_ha_member</span> - Is the specified device an HA member. <span class="li-normal">type: boolean </span> </li>
                
            </ul>
        
        </li>
        fortianalyzer_traffic_fortiview
        <li><span class="li-head">fortianalyzer_traffic_fortiview</span> - Log data for the given log type (and subtype). Append '/raw' to retrieve in raw format. 
        <ul class="ul-self">
                <li><span class="li-required">rows</span> - Number of rows to return. <span class="li-normal">type: int </span> </li>
                <li><span class="li-required">extra</span> - Flag(s) for extra data to be included [reverse_lookup|country_id]. <span class="li-normal">type: string </span> </li>
                <li><span class="li-required">serial_no</span> - Retrieve log from the specified device. <span class="li-normal">type: string </span> </li>
                <li><span class="li-required">session_id</span> - Provide a session_id to continue getting data for that request. <span class="li-normal">type: int </span> </li>
                <li><span class="li-required">filter</span> - Filter expression(s). <span class="li-normal">type: string </span> </li>
                <li><span class="li-required">start</span> - Row number for the first row to return. <span class="li-normal">type: int </span> </li>
                <li><span class="li-required">is_ha_member</span> - Is the specified device an HA member. <span class="li-normal">type: boolean </span> </li>
                
            </ul>
        
        </li>
        fortianalyzer_traffic_forward
        <li><span class="li-head">fortianalyzer_traffic_forward</span> - Log data for the given log type (and subtype). Append '/raw' to retrieve in raw format. 
        <ul class="ul-self">
                <li><span class="li-required">rows</span> - Number of rows to return. <span class="li-normal">type: int </span> </li>
                <li><span class="li-required">extra</span> - Flag(s) for extra data to be included [reverse_lookup|country_id]. <span class="li-normal">type: string </span> </li>
                <li><span class="li-required">serial_no</span> - Retrieve log from the specified device. <span class="li-normal">type: string </span> </li>
                <li><span class="li-required">session_id</span> - Provide a session_id to continue getting data for that request. <span class="li-normal">type: int </span> </li>
                <li><span class="li-required">filter</span> - Filter expression(s). <span class="li-normal">type: string </span> </li>
                <li><span class="li-required">start</span> - Row number for the first row to return. <span class="li-normal">type: int </span> </li>
                <li><span class="li-required">is_ha_member</span> - Is the specified device an HA member. <span class="li-normal">type: boolean </span> </li>
                
            </ul>
        
        </li>
        fortianalyzer_traffic_local
        <li><span class="li-head">fortianalyzer_traffic_local</span> - Log data for the given log type (and subtype). Append '/raw' to retrieve in raw format. 
        <ul class="ul-self">
                <li><span class="li-required">rows</span> - Number of rows to return. <span class="li-normal">type: int </span> </li>
                <li><span class="li-required">extra</span> - Flag(s) for extra data to be included [reverse_lookup|country_id]. <span class="li-normal">type: string </span> </li>
                <li><span class="li-required">serial_no</span> - Retrieve log from the specified device. <span class="li-normal">type: string </span> </li>
                <li><span class="li-required">session_id</span> - Provide a session_id to continue getting data for that request. <span class="li-normal">type: int </span> </li>
                <li><span class="li-required">filter</span> - Filter expression(s). <span class="li-normal">type: string </span> </li>
                <li><span class="li-required">start</span> - Row number for the first row to return. <span class="li-normal">type: int </span> </li>
                <li><span class="li-required">is_ha_member</span> - Is the specified device an HA member. <span class="li-normal">type: boolean </span> </li>
                
            </ul>
        
        </li>
        fortianalyzer_traffic_multicast
        <li><span class="li-head">fortianalyzer_traffic_multicast</span> - Log data for the given log type (and subtype). Append '/raw' to retrieve in raw format. 
        <ul class="ul-self">
                <li><span class="li-required">rows</span> - Number of rows to return. <span class="li-normal">type: int </span> </li>
                <li><span class="li-required">extra</span> - Flag(s) for extra data to be included [reverse_lookup|country_id]. <span class="li-normal">type: string </span> </li>
                <li><span class="li-required">serial_no</span> - Retrieve log from the specified device. <span class="li-normal">type: string </span> </li>
                <li><span class="li-required">session_id</span> - Provide a session_id to continue getting data for that request. <span class="li-normal">type: int </span> </li>
                <li><span class="li-required">filter</span> - Filter expression(s). <span class="li-normal">type: string </span> </li>
                <li><span class="li-required">start</span> - Row number for the first row to return. <span class="li-normal">type: int </span> </li>
                <li><span class="li-required">is_ha_member</span> - Is the specified device an HA member. <span class="li-normal">type: boolean </span> </li>
                
            </ul>
        
        </li>
        fortianalyzer_traffic_sniffer
        <li><span class="li-head">fortianalyzer_traffic_sniffer</span> - Log data for the given log type (and subtype). Append '/raw' to retrieve in raw format. 
        <ul class="ul-self">
                <li><span class="li-required">rows</span> - Number of rows to return. <span class="li-normal">type: int </span> </li>
                <li><span class="li-required">extra</span> - Flag(s) for extra data to be included [reverse_lookup|country_id]. <span class="li-normal">type: string </span> </li>
                <li><span class="li-required">serial_no</span> - Retrieve log from the specified device. <span class="li-normal">type: string </span> </li>
                <li><span class="li-required">session_id</span> - Provide a session_id to continue getting data for that request. <span class="li-normal">type: int </span> </li>
                <li><span class="li-required">filter</span> - Filter expression(s). <span class="li-normal">type: string </span> </li>
                <li><span class="li-required">start</span> - Row number for the first row to return. <span class="li-normal">type: int </span> </li>
                <li><span class="li-required">is_ha_member</span> - Is the specified device an HA member. <span class="li-normal">type: boolean </span> </li>
                
            </ul>
        
        </li>
        fortianalyzer_traffic_threat
        <li><span class="li-head">fortianalyzer_traffic_threat</span> - Log data for the given log type (and subtype). Append '/raw' to retrieve in raw format. 
        <ul class="ul-self">
                <li><span class="li-required">rows</span> - Number of rows to return. <span class="li-normal">type: int </span> </li>
                <li><span class="li-required">extra</span> - Flag(s) for extra data to be included [reverse_lookup|country_id]. <span class="li-normal">type: string </span> </li>
                <li><span class="li-required">serial_no</span> - Retrieve log from the specified device. <span class="li-normal">type: string </span> </li>
                <li><span class="li-required">session_id</span> - Provide a session_id to continue getting data for that request. <span class="li-normal">type: int </span> </li>
                <li><span class="li-required">filter</span> - Filter expression(s). <span class="li-normal">type: string </span> </li>
                <li><span class="li-required">start</span> - Row number for the first row to return. <span class="li-normal">type: int </span> </li>
                <li><span class="li-required">is_ha_member</span> - Is the specified device an HA member. <span class="li-normal">type: boolean </span> </li>
                
            </ul>
        
        </li>
        fortianalyzer_virus_archive
        <li><span class="li-head">fortianalyzer_virus_archive</span> - Return a description of the quarantined virus file. 
        <ul class="ul-self">
                <li><span class="li-required">mkey</span> - checksum column from the virus log. <span class="li-normal">type: int </span> </li>
                <li><span class="li-required">filename</span> - Filename of the antivirus archive. (virus type only) <span class="li-normal">type: string </span> </li>
                
            </ul>
        
        </li>
        fortianalyzer_virus_raw
        <li><span class="li-head">fortianalyzer_virus_raw</span> - Log data for the given log type in raw format. 
        <ul class="ul-self">
                <li><span class="li-required">rows</span> - Number of rows to return. <span class="li-normal">type: int </span> </li>
                <li><span class="li-required">serial_no</span> - Retrieve log from the specified device. <span class="li-normal">type: string </span> </li>
                <li><span class="li-required">session_id</span> - Provide a session_id to continue getting data for that request. <span class="li-normal">type: int </span> </li>
                <li><span class="li-required">filter</span> - Filter expression(s). <span class="li-normal">type: string </span> </li>
                <li><span class="li-required">start</span> - Row number for the first row to return. <span class="li-normal">type: int </span> </li>
                <li><span class="li-required">is_ha_member</span> - Is the specified device an HA member. <span class="li-normal">type: boolean </span> </li>
                
            </ul>
        
        </li>
        fortianalyzer_voip_raw
        <li><span class="li-head">fortianalyzer_voip_raw</span> - Log data for the given log type in raw format. 
        <ul class="ul-self">
                <li><span class="li-required">rows</span> - Number of rows to return. <span class="li-normal">type: int </span> </li>
                <li><span class="li-required">serial_no</span> - Retrieve log from the specified device. <span class="li-normal">type: string </span> </li>
                <li><span class="li-required">session_id</span> - Provide a session_id to continue getting data for that request. <span class="li-normal">type: int </span> </li>
                <li><span class="li-required">filter</span> - Filter expression(s). <span class="li-normal">type: string </span> </li>
                <li><span class="li-required">start</span> - Row number for the first row to return. <span class="li-normal">type: int </span> </li>
                <li><span class="li-required">is_ha_member</span> - Is the specified device an HA member. <span class="li-normal">type: boolean </span> </li>
                
            </ul>
        
        </li>
        fortianalyzer_waf_raw
        <li><span class="li-head">fortianalyzer_waf_raw</span> - Log data for the given log type in raw format. 
        <ul class="ul-self">
                <li><span class="li-required">rows</span> - Number of rows to return. <span class="li-normal">type: int </span> </li>
                <li><span class="li-required">serial_no</span> - Retrieve log from the specified device. <span class="li-normal">type: string </span> </li>
                <li><span class="li-required">session_id</span> - Provide a session_id to continue getting data for that request. <span class="li-normal">type: int </span> </li>
                <li><span class="li-required">filter</span> - Filter expression(s). <span class="li-normal">type: string </span> </li>
                <li><span class="li-required">start</span> - Row number for the first row to return. <span class="li-normal">type: int </span> </li>
                <li><span class="li-required">is_ha_member</span> - Is the specified device an HA member. <span class="li-normal">type: boolean </span> </li>
                
            </ul>
        
        </li>
        fortianalyzer_webfilter_raw
        <li><span class="li-head">fortianalyzer_webfilter_raw</span> - Log data for the given log type in raw format. 
        <ul class="ul-self">
                <li><span class="li-required">rows</span> - Number of rows to return. <span class="li-normal">type: int </span> </li>
                <li><span class="li-required">serial_no</span> - Retrieve log from the specified device. <span class="li-normal">type: string </span> </li>
                <li><span class="li-required">session_id</span> - Provide a session_id to continue getting data for that request. <span class="li-normal">type: int </span> </li>
                <li><span class="li-required">filter</span> - Filter expression(s). <span class="li-normal">type: string </span> </li>
                <li><span class="li-required">start</span> - Row number for the first row to return. <span class="li-normal">type: int </span> </li>
                <li><span class="li-required">is_ha_member</span> - Is the specified device an HA member. <span class="li-normal">type: boolean </span> </li>
                
            </ul>
        
        </li>
        forticloud_anomaly_raw
        <li><span class="li-head">forticloud_anomaly_raw</span> - Log data for the given log type in raw format. 
        <ul class="ul-self">
                <li><span class="li-required">rows</span> - Number of rows to return. <span class="li-normal">type: int </span> </li>
                <li><span class="li-required">serial_no</span> - Retrieve log from the specified device. <span class="li-normal">type: string </span> </li>
                <li><span class="li-required">session_id</span> - Provide a session_id to continue getting data for that request. <span class="li-normal">type: int </span> </li>
                <li><span class="li-required">filter</span> - Filter expression(s). <span class="li-normal">type: string </span> </li>
                <li><span class="li-required">start</span> - Row number for the first row to return. <span class="li-normal">type: int </span> </li>
                <li><span class="li-required">is_ha_member</span> - Is the specified device an HA member. <span class="li-normal">type: boolean </span> </li>
                
            </ul>
        
        </li>
        forticloud_app-ctrl_archive
        <li><span class="li-head">forticloud_app-ctrl_archive</span> - Return a list of archived items for the desired type. :type can be app-ctrl or ips 
        <ul class="ul-self">
                <li><span class="li-required">roll</span> - Log roll number. (required if source is not fortianalyzer) <span class="li-normal">type: int </span> </li>
                <li><span class="li-required">mkey</span> - Archive identifier. <span class="li-normal">type: int </span> </li>
                
            </ul>
        
        </li>
        forticloud_app-ctrl_archive-download
        <li><span class="li-head">forticloud_app-ctrl_archive-download</span> - Download an archived file. 
        <ul class="ul-self">
                <li><span class="li-required">roll</span> - Log roll number (required if source is not fortianalyzer). <span class="li-normal">type: int </span> </li>
                <li><span class="li-required">mkey</span> - Archive identifier. <span class="li-normal">type: int </span> </li>
                <li><span class="li-required">filename</span> - File name to use when saving the file in the browser. <span class="li-normal">type: string </span> </li>
                
            </ul>
        
        </li>
        forticloud_app-ctrl_raw
        <li><span class="li-head">forticloud_app-ctrl_raw</span> - Log data for the given log type in raw format. 
        <ul class="ul-self">
                <li><span class="li-required">rows</span> - Number of rows to return. <span class="li-normal">type: int </span> </li>
                <li><span class="li-required">serial_no</span> - Retrieve log from the specified device. <span class="li-normal">type: string </span> </li>
                <li><span class="li-required">session_id</span> - Provide a session_id to continue getting data for that request. <span class="li-normal">type: int </span> </li>
                <li><span class="li-required">filter</span> - Filter expression(s). <span class="li-normal">type: string </span> </li>
                <li><span class="li-required">start</span> - Row number for the first row to return. <span class="li-normal">type: int </span> </li>
                <li><span class="li-required">is_ha_member</span> - Is the specified device an HA member. <span class="li-normal">type: boolean </span> </li>
                
            </ul>
        
        </li>
        forticloud_cifs_raw
        <li><span class="li-head">forticloud_cifs_raw</span> - Log data for the given log type in raw format. 
        <ul class="ul-self">
                <li><span class="li-required">rows</span> - Number of rows to return. <span class="li-normal">type: int </span> </li>
                <li><span class="li-required">serial_no</span> - Retrieve log from the specified device. <span class="li-normal">type: string </span> </li>
                <li><span class="li-required">session_id</span> - Provide a session_id to continue getting data for that request. <span class="li-normal">type: int </span> </li>
                <li><span class="li-required">filter</span> - Filter expression(s). <span class="li-normal">type: string </span> </li>
                <li><span class="li-required">start</span> - Row number for the first row to return. <span class="li-normal">type: int </span> </li>
                <li><span class="li-required">is_ha_member</span> - Is the specified device an HA member. <span class="li-normal">type: boolean </span> </li>
                
            </ul>
        
        </li>
        forticloud_dlp_raw
        <li><span class="li-head">forticloud_dlp_raw</span> - Log data for the given log type in raw format. 
        <ul class="ul-self">
                <li><span class="li-required">rows</span> - Number of rows to return. <span class="li-normal">type: int </span> </li>
                <li><span class="li-required">serial_no</span> - Retrieve log from the specified device. <span class="li-normal">type: string </span> </li>
                <li><span class="li-required">session_id</span> - Provide a session_id to continue getting data for that request. <span class="li-normal">type: int </span> </li>
                <li><span class="li-required">filter</span> - Filter expression(s). <span class="li-normal">type: string </span> </li>
                <li><span class="li-required">start</span> - Row number for the first row to return. <span class="li-normal">type: int </span> </li>
                <li><span class="li-required">is_ha_member</span> - Is the specified device an HA member. <span class="li-normal">type: boolean </span> </li>
                
            </ul>
        
        </li>
        forticloud_dns_raw
        <li><span class="li-head">forticloud_dns_raw</span> - Log data for the given log type in raw format. 
        <ul class="ul-self">
                <li><span class="li-required">rows</span> - Number of rows to return. <span class="li-normal">type: int </span> </li>
                <li><span class="li-required">serial_no</span> - Retrieve log from the specified device. <span class="li-normal">type: string </span> </li>
                <li><span class="li-required">session_id</span> - Provide a session_id to continue getting data for that request. <span class="li-normal">type: int </span> </li>
                <li><span class="li-required">filter</span> - Filter expression(s). <span class="li-normal">type: string </span> </li>
                <li><span class="li-required">start</span> - Row number for the first row to return. <span class="li-normal">type: int </span> </li>
                <li><span class="li-required">is_ha_member</span> - Is the specified device an HA member. <span class="li-normal">type: boolean </span> </li>
                
            </ul>
        
        </li>
        forticloud_emailfilter_raw
        <li><span class="li-head">forticloud_emailfilter_raw</span> - Log data for the given log type in raw format. 
        <ul class="ul-self">
                <li><span class="li-required">rows</span> - Number of rows to return. <span class="li-normal">type: int </span> </li>
                <li><span class="li-required">serial_no</span> - Retrieve log from the specified device. <span class="li-normal">type: string </span> </li>
                <li><span class="li-required">session_id</span> - Provide a session_id to continue getting data for that request. <span class="li-normal">type: int </span> </li>
                <li><span class="li-required">filter</span> - Filter expression(s). <span class="li-normal">type: string </span> </li>
                <li><span class="li-required">start</span> - Row number for the first row to return. <span class="li-normal">type: int </span> </li>
                <li><span class="li-required">is_ha_member</span> - Is the specified device an HA member. <span class="li-normal">type: boolean </span> </li>
                
            </ul>
        
        </li>
        forticloud_event_compliance-check
        <li><span class="li-head">forticloud_event_compliance-check</span> - Log data for the given log type (and subtype). Append '/raw' to retrieve in raw format. 
        <ul class="ul-self">
                <li><span class="li-required">rows</span> - Number of rows to return. <span class="li-normal">type: int </span> </li>
                <li><span class="li-required">extra</span> - Flag(s) for extra data to be included [reverse_lookup|country_id]. <span class="li-normal">type: string </span> </li>
                <li><span class="li-required">serial_no</span> - Retrieve log from the specified device. <span class="li-normal">type: string </span> </li>
                <li><span class="li-required">session_id</span> - Provide a session_id to continue getting data for that request. <span class="li-normal">type: int </span> </li>
                <li><span class="li-required">filter</span> - Filter expression(s). <span class="li-normal">type: string </span> </li>
                <li><span class="li-required">start</span> - Row number for the first row to return. <span class="li-normal">type: int </span> </li>
                <li><span class="li-required">is_ha_member</span> - Is the specified device an HA member. <span class="li-normal">type: boolean </span> </li>
                
            </ul>
        
        </li>
        forticloud_event_connector
        <li><span class="li-head">forticloud_event_connector</span> - Log data for the given log type (and subtype). Append '/raw' to retrieve in raw format. 
        <ul class="ul-self">
                <li><span class="li-required">rows</span> - Number of rows to return. <span class="li-normal">type: int </span> </li>
                <li><span class="li-required">extra</span> - Flag(s) for extra data to be included [reverse_lookup|country_id]. <span class="li-normal">type: string </span> </li>
                <li><span class="li-required">serial_no</span> - Retrieve log from the specified device. <span class="li-normal">type: string </span> </li>
                <li><span class="li-required">session_id</span> - Provide a session_id to continue getting data for that request. <span class="li-normal">type: int </span> </li>
                <li><span class="li-required">filter</span> - Filter expression(s). <span class="li-normal">type: string </span> </li>
                <li><span class="li-required">start</span> - Row number for the first row to return. <span class="li-normal">type: int </span> </li>
                <li><span class="li-required">is_ha_member</span> - Is the specified device an HA member. <span class="li-normal">type: boolean </span> </li>
                
            </ul>
        
        </li>
        forticloud_event_endpoint
        <li><span class="li-head">forticloud_event_endpoint</span> - Log data for the given log type (and subtype). Append '/raw' to retrieve in raw format. 
        <ul class="ul-self">
                <li><span class="li-required">rows</span> - Number of rows to return. <span class="li-normal">type: int </span> </li>
                <li><span class="li-required">extra</span> - Flag(s) for extra data to be included [reverse_lookup|country_id]. <span class="li-normal">type: string </span> </li>
                <li><span class="li-required">serial_no</span> - Retrieve log from the specified device. <span class="li-normal">type: string </span> </li>
                <li><span class="li-required">session_id</span> - Provide a session_id to continue getting data for that request. <span class="li-normal">type: int </span> </li>
                <li><span class="li-required">filter</span> - Filter expression(s). <span class="li-normal">type: string </span> </li>
                <li><span class="li-required">start</span> - Row number for the first row to return. <span class="li-normal">type: int </span> </li>
                <li><span class="li-required">is_ha_member</span> - Is the specified device an HA member. <span class="li-normal">type: boolean </span> </li>
                
            </ul>
        
        </li>
        forticloud_event_fortiextender
        <li><span class="li-head">forticloud_event_fortiextender</span> - Log data for the given log type (and subtype). Append '/raw' to retrieve in raw format. 
        <ul class="ul-self">
                <li><span class="li-required">rows</span> - Number of rows to return. <span class="li-normal">type: int </span> </li>
                <li><span class="li-required">extra</span> - Flag(s) for extra data to be included [reverse_lookup|country_id]. <span class="li-normal">type: string </span> </li>
                <li><span class="li-required">serial_no</span> - Retrieve log from the specified device. <span class="li-normal">type: string </span> </li>
                <li><span class="li-required">session_id</span> - Provide a session_id to continue getting data for that request. <span class="li-normal">type: int </span> </li>
                <li><span class="li-required">filter</span> - Filter expression(s). <span class="li-normal">type: string </span> </li>
                <li><span class="li-required">start</span> - Row number for the first row to return. <span class="li-normal">type: int </span> </li>
                <li><span class="li-required">is_ha_member</span> - Is the specified device an HA member. <span class="li-normal">type: boolean </span> </li>
                
            </ul>
        
        </li>
        forticloud_event_ha
        <li><span class="li-head">forticloud_event_ha</span> - Log data for the given log type (and subtype). Append '/raw' to retrieve in raw format. 
        <ul class="ul-self">
                <li><span class="li-required">rows</span> - Number of rows to return. <span class="li-normal">type: int </span> </li>
                <li><span class="li-required">extra</span> - Flag(s) for extra data to be included [reverse_lookup|country_id]. <span class="li-normal">type: string </span> </li>
                <li><span class="li-required">serial_no</span> - Retrieve log from the specified device. <span class="li-normal">type: string </span> </li>
                <li><span class="li-required">session_id</span> - Provide a session_id to continue getting data for that request. <span class="li-normal">type: int </span> </li>
                <li><span class="li-required">filter</span> - Filter expression(s). <span class="li-normal">type: string </span> </li>
                <li><span class="li-required">start</span> - Row number for the first row to return. <span class="li-normal">type: int </span> </li>
                <li><span class="li-required">is_ha_member</span> - Is the specified device an HA member. <span class="li-normal">type: boolean </span> </li>
                
            </ul>
        
        </li>
        forticloud_event_router
        <li><span class="li-head">forticloud_event_router</span> - Log data for the given log type (and subtype). Append '/raw' to retrieve in raw format. 
        <ul class="ul-self">
                <li><span class="li-required">rows</span> - Number of rows to return. <span class="li-normal">type: int </span> </li>
                <li><span class="li-required">extra</span> - Flag(s) for extra data to be included [reverse_lookup|country_id]. <span class="li-normal">type: string </span> </li>
                <li><span class="li-required">serial_no</span> - Retrieve log from the specified device. <span class="li-normal">type: string </span> </li>
                <li><span class="li-required">session_id</span> - Provide a session_id to continue getting data for that request. <span class="li-normal">type: int </span> </li>
                <li><span class="li-required">filter</span> - Filter expression(s). <span class="li-normal">type: string </span> </li>
                <li><span class="li-required">start</span> - Row number for the first row to return. <span class="li-normal">type: int </span> </li>
                <li><span class="li-required">is_ha_member</span> - Is the specified device an HA member. <span class="li-normal">type: boolean </span> </li>
                
            </ul>
        
        </li>
        forticloud_event_security-rating
        <li><span class="li-head">forticloud_event_security-rating</span> - Log data for the given log type (and subtype). Append '/raw' to retrieve in raw format. 
        <ul class="ul-self">
                <li><span class="li-required">rows</span> - Number of rows to return. <span class="li-normal">type: int </span> </li>
                <li><span class="li-required">extra</span> - Flag(s) for extra data to be included [reverse_lookup|country_id]. <span class="li-normal">type: string </span> </li>
                <li><span class="li-required">serial_no</span> - Retrieve log from the specified device. <span class="li-normal">type: string </span> </li>
                <li><span class="li-required">session_id</span> - Provide a session_id to continue getting data for that request. <span class="li-normal">type: int </span> </li>
                <li><span class="li-required">filter</span> - Filter expression(s). <span class="li-normal">type: string </span> </li>
                <li><span class="li-required">start</span> - Row number for the first row to return. <span class="li-normal">type: int </span> </li>
                <li><span class="li-required">is_ha_member</span> - Is the specified device an HA member. <span class="li-normal">type: boolean </span> </li>
                
            </ul>
        
        </li>
        forticloud_event_system
        <li><span class="li-head">forticloud_event_system</span> - Log data for the given log type (and subtype). Append '/raw' to retrieve in raw format. 
        <ul class="ul-self">
                <li><span class="li-required">rows</span> - Number of rows to return. <span class="li-normal">type: int </span> </li>
                <li><span class="li-required">extra</span> - Flag(s) for extra data to be included [reverse_lookup|country_id]. <span class="li-normal">type: string </span> </li>
                <li><span class="li-required">serial_no</span> - Retrieve log from the specified device. <span class="li-normal">type: string </span> </li>
                <li><span class="li-required">session_id</span> - Provide a session_id to continue getting data for that request. <span class="li-normal">type: int </span> </li>
                <li><span class="li-required">filter</span> - Filter expression(s). <span class="li-normal">type: string </span> </li>
                <li><span class="li-required">start</span> - Row number for the first row to return. <span class="li-normal">type: int </span> </li>
                <li><span class="li-required">is_ha_member</span> - Is the specified device an HA member. <span class="li-normal">type: boolean </span> </li>
                
            </ul>
        
        </li>
        forticloud_event_user
        <li><span class="li-head">forticloud_event_user</span> - Log data for the given log type (and subtype). Append '/raw' to retrieve in raw format. 
        <ul class="ul-self">
                <li><span class="li-required">rows</span> - Number of rows to return. <span class="li-normal">type: int </span> </li>
                <li><span class="li-required">extra</span> - Flag(s) for extra data to be included [reverse_lookup|country_id]. <span class="li-normal">type: string </span> </li>
                <li><span class="li-required">serial_no</span> - Retrieve log from the specified device. <span class="li-normal">type: string </span> </li>
                <li><span class="li-required">session_id</span> - Provide a session_id to continue getting data for that request. <span class="li-normal">type: int </span> </li>
                <li><span class="li-required">filter</span> - Filter expression(s). <span class="li-normal">type: string </span> </li>
                <li><span class="li-required">start</span> - Row number for the first row to return. <span class="li-normal">type: int </span> </li>
                <li><span class="li-required">is_ha_member</span> - Is the specified device an HA member. <span class="li-normal">type: boolean </span> </li>
                
            </ul>
        
        </li>
        forticloud_event_vpn
        <li><span class="li-head">forticloud_event_vpn</span> - Log data for the given log type (and subtype). Append '/raw' to retrieve in raw format. 
        <ul class="ul-self">
                <li><span class="li-required">rows</span> - Number of rows to return. <span class="li-normal">type: int </span> </li>
                <li><span class="li-required">extra</span> - Flag(s) for extra data to be included [reverse_lookup|country_id]. <span class="li-normal">type: string </span> </li>
                <li><span class="li-required">serial_no</span> - Retrieve log from the specified device. <span class="li-normal">type: string </span> </li>
                <li><span class="li-required">session_id</span> - Provide a session_id to continue getting data for that request. <span class="li-normal">type: int </span> </li>
                <li><span class="li-required">filter</span> - Filter expression(s). <span class="li-normal">type: string </span> </li>
                <li><span class="li-required">start</span> - Row number for the first row to return. <span class="li-normal">type: int </span> </li>
                <li><span class="li-required">is_ha_member</span> - Is the specified device an HA member. <span class="li-normal">type: boolean </span> </li>
                
            </ul>
        
        </li>
        forticloud_event_wad
        <li><span class="li-head">forticloud_event_wad</span> - Log data for the given log type (and subtype). Append '/raw' to retrieve in raw format. 
        <ul class="ul-self">
                <li><span class="li-required">rows</span> - Number of rows to return. <span class="li-normal">type: int </span> </li>
                <li><span class="li-required">extra</span> - Flag(s) for extra data to be included [reverse_lookup|country_id]. <span class="li-normal">type: string </span> </li>
                <li><span class="li-required">serial_no</span> - Retrieve log from the specified device. <span class="li-normal">type: string </span> </li>
                <li><span class="li-required">session_id</span> - Provide a session_id to continue getting data for that request. <span class="li-normal">type: int </span> </li>
                <li><span class="li-required">filter</span> - Filter expression(s). <span class="li-normal">type: string </span> </li>
                <li><span class="li-required">start</span> - Row number for the first row to return. <span class="li-normal">type: int </span> </li>
                <li><span class="li-required">is_ha_member</span> - Is the specified device an HA member. <span class="li-normal">type: boolean </span> </li>
                
            </ul>
        
        </li>
        forticloud_event_wireless
        <li><span class="li-head">forticloud_event_wireless</span> - Log data for the given log type (and subtype). Append '/raw' to retrieve in raw format. 
        <ul class="ul-self">
                <li><span class="li-required">rows</span> - Number of rows to return. <span class="li-normal">type: int </span> </li>
                <li><span class="li-required">extra</span> - Flag(s) for extra data to be included [reverse_lookup|country_id]. <span class="li-normal">type: string </span> </li>
                <li><span class="li-required">serial_no</span> - Retrieve log from the specified device. <span class="li-normal">type: string </span> </li>
                <li><span class="li-required">session_id</span> - Provide a session_id to continue getting data for that request. <span class="li-normal">type: int </span> </li>
                <li><span class="li-required">filter</span> - Filter expression(s). <span class="li-normal">type: string </span> </li>
                <li><span class="li-required">start</span> - Row number for the first row to return. <span class="li-normal">type: int </span> </li>
                <li><span class="li-required">is_ha_member</span> - Is the specified device an HA member. <span class="li-normal">type: boolean </span> </li>
                
            </ul>
        
        </li>
        forticloud_file-filter_raw
        <li><span class="li-head">forticloud_file-filter_raw</span> - Log data for the given log type in raw format. 
        <ul class="ul-self">
                <li><span class="li-required">rows</span> - Number of rows to return. <span class="li-normal">type: int </span> </li>
                <li><span class="li-required">serial_no</span> - Retrieve log from the specified device. <span class="li-normal">type: string </span> </li>
                <li><span class="li-required">session_id</span> - Provide a session_id to continue getting data for that request. <span class="li-normal">type: int </span> </li>
                <li><span class="li-required">filter</span> - Filter expression(s). <span class="li-normal">type: string </span> </li>
                <li><span class="li-required">start</span> - Row number for the first row to return. <span class="li-normal">type: int </span> </li>
                <li><span class="li-required">is_ha_member</span> - Is the specified device an HA member. <span class="li-normal">type: boolean </span> </li>
                
            </ul>
        
        </li>
        forticloud_gtp_raw
        <li><span class="li-head">forticloud_gtp_raw</span> - Log data for the given log type in raw format. 
        <ul class="ul-self">
                <li><span class="li-required">rows</span> - Number of rows to return. <span class="li-normal">type: int </span> </li>
                <li><span class="li-required">serial_no</span> - Retrieve log from the specified device. <span class="li-normal">type: string </span> </li>
                <li><span class="li-required">session_id</span> - Provide a session_id to continue getting data for that request. <span class="li-normal">type: int </span> </li>
                <li><span class="li-required">filter</span> - Filter expression(s). <span class="li-normal">type: string </span> </li>
                <li><span class="li-required">start</span> - Row number for the first row to return. <span class="li-normal">type: int </span> </li>
                <li><span class="li-required">is_ha_member</span> - Is the specified device an HA member. <span class="li-normal">type: boolean </span> </li>
                
            </ul>
        
        </li>
        forticloud_ips_archive
        <li><span class="li-head">forticloud_ips_archive</span> - Return a list of archived items for the desired type. :type can be app-ctrl or ips 
        <ul class="ul-self">
                <li><span class="li-required">roll</span> - Log roll number. (required if source is not fortianalyzer) <span class="li-normal">type: int </span> </li>
                <li><span class="li-required">mkey</span> - Archive identifier. <span class="li-normal">type: int </span> </li>
                
            </ul>
        
        </li>
        forticloud_ips_archive-download
        <li><span class="li-head">forticloud_ips_archive-download</span> - Download an archived file. 
        <ul class="ul-self">
                <li><span class="li-required">roll</span> - Log roll number (required if source is not fortianalyzer). <span class="li-normal">type: int </span> </li>
                <li><span class="li-required">mkey</span> - Archive identifier. <span class="li-normal">type: int </span> </li>
                <li><span class="li-required">filename</span> - File name to use when saving the file in the browser. <span class="li-normal">type: string </span> </li>
                
            </ul>
        
        </li>
        forticloud_ips_raw
        <li><span class="li-head">forticloud_ips_raw</span> - Log data for the given log type in raw format. 
        <ul class="ul-self">
                <li><span class="li-required">rows</span> - Number of rows to return. <span class="li-normal">type: int </span> </li>
                <li><span class="li-required">serial_no</span> - Retrieve log from the specified device. <span class="li-normal">type: string </span> </li>
                <li><span class="li-required">session_id</span> - Provide a session_id to continue getting data for that request. <span class="li-normal">type: int </span> </li>
                <li><span class="li-required">filter</span> - Filter expression(s). <span class="li-normal">type: string </span> </li>
                <li><span class="li-required">start</span> - Row number for the first row to return. <span class="li-normal">type: int </span> </li>
                <li><span class="li-required">is_ha_member</span> - Is the specified device an HA member. <span class="li-normal">type: boolean </span> </li>
                
            </ul>
        
        </li>
        forticloud_ssh_raw
        <li><span class="li-head">forticloud_ssh_raw</span> - Log data for the given log type in raw format. 
        <ul class="ul-self">
                <li><span class="li-required">rows</span> - Number of rows to return. <span class="li-normal">type: int </span> </li>
                <li><span class="li-required">serial_no</span> - Retrieve log from the specified device. <span class="li-normal">type: string </span> </li>
                <li><span class="li-required">session_id</span> - Provide a session_id to continue getting data for that request. <span class="li-normal">type: int </span> </li>
                <li><span class="li-required">filter</span> - Filter expression(s). <span class="li-normal">type: string </span> </li>
                <li><span class="li-required">start</span> - Row number for the first row to return. <span class="li-normal">type: int </span> </li>
                <li><span class="li-required">is_ha_member</span> - Is the specified device an HA member. <span class="li-normal">type: boolean </span> </li>
                
            </ul>
        
        </li>
        forticloud_ssl_raw
        <li><span class="li-head">forticloud_ssl_raw</span> - Log data for the given log type in raw format. 
        <ul class="ul-self">
                <li><span class="li-required">rows</span> - Number of rows to return. <span class="li-normal">type: int </span> </li>
                <li><span class="li-required">serial_no</span> - Retrieve log from the specified device. <span class="li-normal">type: string </span> </li>
                <li><span class="li-required">session_id</span> - Provide a session_id to continue getting data for that request. <span class="li-normal">type: int </span> </li>
                <li><span class="li-required">filter</span> - Filter expression(s). <span class="li-normal">type: string </span> </li>
                <li><span class="li-required">start</span> - Row number for the first row to return. <span class="li-normal">type: int </span> </li>
                <li><span class="li-required">is_ha_member</span> - Is the specified device an HA member. <span class="li-normal">type: boolean </span> </li>
                
            </ul>
        
        </li>
        forticloud_traffic_fortiview
        <li><span class="li-head">forticloud_traffic_fortiview</span> - Log data for the given log type (and subtype). Append '/raw' to retrieve in raw format. 
        <ul class="ul-self">
                <li><span class="li-required">rows</span> - Number of rows to return. <span class="li-normal">type: int </span> </li>
                <li><span class="li-required">extra</span> - Flag(s) for extra data to be included [reverse_lookup|country_id]. <span class="li-normal">type: string </span> </li>
                <li><span class="li-required">serial_no</span> - Retrieve log from the specified device. <span class="li-normal">type: string </span> </li>
                <li><span class="li-required">session_id</span> - Provide a session_id to continue getting data for that request. <span class="li-normal">type: int </span> </li>
                <li><span class="li-required">filter</span> - Filter expression(s). <span class="li-normal">type: string </span> </li>
                <li><span class="li-required">start</span> - Row number for the first row to return. <span class="li-normal">type: int </span> </li>
                <li><span class="li-required">is_ha_member</span> - Is the specified device an HA member. <span class="li-normal">type: boolean </span> </li>
                
            </ul>
        
        </li>
        forticloud_traffic_forward
        <li><span class="li-head">forticloud_traffic_forward</span> - Log data for the given log type (and subtype). Append '/raw' to retrieve in raw format. 
        <ul class="ul-self">
                <li><span class="li-required">rows</span> - Number of rows to return. <span class="li-normal">type: int </span> </li>
                <li><span class="li-required">extra</span> - Flag(s) for extra data to be included [reverse_lookup|country_id]. <span class="li-normal">type: string </span> </li>
                <li><span class="li-required">serial_no</span> - Retrieve log from the specified device. <span class="li-normal">type: string </span> </li>
                <li><span class="li-required">session_id</span> - Provide a session_id to continue getting data for that request. <span class="li-normal">type: int </span> </li>
                <li><span class="li-required">filter</span> - Filter expression(s). <span class="li-normal">type: string </span> </li>
                <li><span class="li-required">start</span> - Row number for the first row to return. <span class="li-normal">type: int </span> </li>
                <li><span class="li-required">is_ha_member</span> - Is the specified device an HA member. <span class="li-normal">type: boolean </span> </li>
                
            </ul>
        
        </li>
        forticloud_traffic_local
        <li><span class="li-head">forticloud_traffic_local</span> - Log data for the given log type (and subtype). Append '/raw' to retrieve in raw format. 
        <ul class="ul-self">
                <li><span class="li-required">rows</span> - Number of rows to return. <span class="li-normal">type: int </span> </li>
                <li><span class="li-required">extra</span> - Flag(s) for extra data to be included [reverse_lookup|country_id]. <span class="li-normal">type: string </span> </li>
                <li><span class="li-required">serial_no</span> - Retrieve log from the specified device. <span class="li-normal">type: string </span> </li>
                <li><span class="li-required">session_id</span> - Provide a session_id to continue getting data for that request. <span class="li-normal">type: int </span> </li>
                <li><span class="li-required">filter</span> - Filter expression(s). <span class="li-normal">type: string </span> </li>
                <li><span class="li-required">start</span> - Row number for the first row to return. <span class="li-normal">type: int </span> </li>
                <li><span class="li-required">is_ha_member</span> - Is the specified device an HA member. <span class="li-normal">type: boolean </span> </li>
                
            </ul>
        
        </li>
        forticloud_traffic_multicast
        <li><span class="li-head">forticloud_traffic_multicast</span> - Log data for the given log type (and subtype). Append '/raw' to retrieve in raw format. 
        <ul class="ul-self">
                <li><span class="li-required">rows</span> - Number of rows to return. <span class="li-normal">type: int </span> </li>
                <li><span class="li-required">extra</span> - Flag(s) for extra data to be included [reverse_lookup|country_id]. <span class="li-normal">type: string </span> </li>
                <li><span class="li-required">serial_no</span> - Retrieve log from the specified device. <span class="li-normal">type: string </span> </li>
                <li><span class="li-required">session_id</span> - Provide a session_id to continue getting data for that request. <span class="li-normal">type: int </span> </li>
                <li><span class="li-required">filter</span> - Filter expression(s). <span class="li-normal">type: string </span> </li>
                <li><span class="li-required">start</span> - Row number for the first row to return. <span class="li-normal">type: int </span> </li>
                <li><span class="li-required">is_ha_member</span> - Is the specified device an HA member. <span class="li-normal">type: boolean </span> </li>
                
            </ul>
        
        </li>
        forticloud_traffic_sniffer
        <li><span class="li-head">forticloud_traffic_sniffer</span> - Log data for the given log type (and subtype). Append '/raw' to retrieve in raw format. 
        <ul class="ul-self">
                <li><span class="li-required">rows</span> - Number of rows to return. <span class="li-normal">type: int </span> </li>
                <li><span class="li-required">extra</span> - Flag(s) for extra data to be included [reverse_lookup|country_id]. <span class="li-normal">type: string </span> </li>
                <li><span class="li-required">serial_no</span> - Retrieve log from the specified device. <span class="li-normal">type: string </span> </li>
                <li><span class="li-required">session_id</span> - Provide a session_id to continue getting data for that request. <span class="li-normal">type: int </span> </li>
                <li><span class="li-required">filter</span> - Filter expression(s). <span class="li-normal">type: string </span> </li>
                <li><span class="li-required">start</span> - Row number for the first row to return. <span class="li-normal">type: int </span> </li>
                <li><span class="li-required">is_ha_member</span> - Is the specified device an HA member. <span class="li-normal">type: boolean </span> </li>
                
            </ul>
        
        </li>
        forticloud_traffic_threat
        <li><span class="li-head">forticloud_traffic_threat</span> - Log data for the given log type (and subtype). Append '/raw' to retrieve in raw format. 
        <ul class="ul-self">
                <li><span class="li-required">rows</span> - Number of rows to return. <span class="li-normal">type: int </span> </li>
                <li><span class="li-required">extra</span> - Flag(s) for extra data to be included [reverse_lookup|country_id]. <span class="li-normal">type: string </span> </li>
                <li><span class="li-required">serial_no</span> - Retrieve log from the specified device. <span class="li-normal">type: string </span> </li>
                <li><span class="li-required">session_id</span> - Provide a session_id to continue getting data for that request. <span class="li-normal">type: int </span> </li>
                <li><span class="li-required">filter</span> - Filter expression(s). <span class="li-normal">type: string </span> </li>
                <li><span class="li-required">start</span> - Row number for the first row to return. <span class="li-normal">type: int </span> </li>
                <li><span class="li-required">is_ha_member</span> - Is the specified device an HA member. <span class="li-normal">type: boolean </span> </li>
                
            </ul>
        
        </li>
        forticloud_virus_archive
        <li><span class="li-head">forticloud_virus_archive</span> - Return a description of the quarantined virus file. 
        <ul class="ul-self">
                <li><span class="li-required">mkey</span> - checksum column from the virus log. <span class="li-normal">type: int </span> </li>
                <li><span class="li-required">filename</span> - Filename of the antivirus archive. (virus type only) <span class="li-normal">type: string </span> </li>
                
            </ul>
        
        </li>
        forticloud_virus_raw
        <li><span class="li-head">forticloud_virus_raw</span> - Log data for the given log type in raw format. 
        <ul class="ul-self">
                <li><span class="li-required">rows</span> - Number of rows to return. <span class="li-normal">type: int </span> </li>
                <li><span class="li-required">serial_no</span> - Retrieve log from the specified device. <span class="li-normal">type: string </span> </li>
                <li><span class="li-required">session_id</span> - Provide a session_id to continue getting data for that request. <span class="li-normal">type: int </span> </li>
                <li><span class="li-required">filter</span> - Filter expression(s). <span class="li-normal">type: string </span> </li>
                <li><span class="li-required">start</span> - Row number for the first row to return. <span class="li-normal">type: int </span> </li>
                <li><span class="li-required">is_ha_member</span> - Is the specified device an HA member. <span class="li-normal">type: boolean </span> </li>
                
            </ul>
        
        </li>
        forticloud_voip_raw
        <li><span class="li-head">forticloud_voip_raw</span> - Log data for the given log type in raw format. 
        <ul class="ul-self">
                <li><span class="li-required">rows</span> - Number of rows to return. <span class="li-normal">type: int </span> </li>
                <li><span class="li-required">serial_no</span> - Retrieve log from the specified device. <span class="li-normal">type: string </span> </li>
                <li><span class="li-required">session_id</span> - Provide a session_id to continue getting data for that request. <span class="li-normal">type: int </span> </li>
                <li><span class="li-required">filter</span> - Filter expression(s). <span class="li-normal">type: string </span> </li>
                <li><span class="li-required">start</span> - Row number for the first row to return. <span class="li-normal">type: int </span> </li>
                <li><span class="li-required">is_ha_member</span> - Is the specified device an HA member. <span class="li-normal">type: boolean </span> </li>
                
            </ul>
        
        </li>
        forticloud_waf_raw
        <li><span class="li-head">forticloud_waf_raw</span> - Log data for the given log type in raw format. 
        <ul class="ul-self">
                <li><span class="li-required">rows</span> - Number of rows to return. <span class="li-normal">type: int </span> </li>
                <li><span class="li-required">serial_no</span> - Retrieve log from the specified device. <span class="li-normal">type: string </span> </li>
                <li><span class="li-required">session_id</span> - Provide a session_id to continue getting data for that request. <span class="li-normal">type: int </span> </li>
                <li><span class="li-required">filter</span> - Filter expression(s). <span class="li-normal">type: string </span> </li>
                <li><span class="li-required">start</span> - Row number for the first row to return. <span class="li-normal">type: int </span> </li>
                <li><span class="li-required">is_ha_member</span> - Is the specified device an HA member. <span class="li-normal">type: boolean </span> </li>
                
            </ul>
        
        </li>
        forticloud_webfilter_raw
        <li><span class="li-head">forticloud_webfilter_raw</span> - Log data for the given log type in raw format. 
        <ul class="ul-self">
                <li><span class="li-required">rows</span> - Number of rows to return. <span class="li-normal">type: int </span> </li>
                <li><span class="li-required">serial_no</span> - Retrieve log from the specified device. <span class="li-normal">type: string </span> </li>
                <li><span class="li-required">session_id</span> - Provide a session_id to continue getting data for that request. <span class="li-normal">type: int </span> </li>
                <li><span class="li-required">filter</span> - Filter expression(s). <span class="li-normal">type: string </span> </li>
                <li><span class="li-required">start</span> - Row number for the first row to return. <span class="li-normal">type: int </span> </li>
                <li><span class="li-required">is_ha_member</span> - Is the specified device an HA member. <span class="li-normal">type: boolean </span> </li>
                
            </ul>
        
        </li>
        memory_anomaly_raw
        <li><span class="li-head">memory_anomaly_raw</span> - Log data for the given log type in raw format. 
        <ul class="ul-self">
                <li><span class="li-required">rows</span> - Number of rows to return. <span class="li-normal">type: int </span> </li>
                <li><span class="li-required">serial_no</span> - Retrieve log from the specified device. <span class="li-normal">type: string </span> </li>
                <li><span class="li-required">session_id</span> - Provide a session_id to continue getting data for that request. <span class="li-normal">type: int </span> </li>
                <li><span class="li-required">filter</span> - Filter expression(s). <span class="li-normal">type: string </span> </li>
                <li><span class="li-required">start</span> - Row number for the first row to return. <span class="li-normal">type: int </span> </li>
                <li><span class="li-required">is_ha_member</span> - Is the specified device an HA member. <span class="li-normal">type: boolean </span> </li>
                
            </ul>
        
        </li>
        memory_app-ctrl_archive
        <li><span class="li-head">memory_app-ctrl_archive</span> - Return a list of archived items for the desired type. :type can be app-ctrl or ips 
        <ul class="ul-self">
                <li><span class="li-required">roll</span> - Log roll number. (required if source is not fortianalyzer) <span class="li-normal">type: int </span> </li>
                <li><span class="li-required">mkey</span> - Archive identifier. <span class="li-normal">type: int </span> </li>
                
            </ul>
        
        </li>
        memory_app-ctrl_archive-download
        <li><span class="li-head">memory_app-ctrl_archive-download</span> - Download an archived file. 
        <ul class="ul-self">
                <li><span class="li-required">roll</span> - Log roll number (required if source is not fortianalyzer). <span class="li-normal">type: int </span> </li>
                <li><span class="li-required">mkey</span> - Archive identifier. <span class="li-normal">type: int </span> </li>
                <li><span class="li-required">filename</span> - File name to use when saving the file in the browser. <span class="li-normal">type: string </span> </li>
                
            </ul>
        
        </li>
        memory_app-ctrl_raw
        <li><span class="li-head">memory_app-ctrl_raw</span> - Log data for the given log type in raw format. 
        <ul class="ul-self">
                <li><span class="li-required">rows</span> - Number of rows to return. <span class="li-normal">type: int </span> </li>
                <li><span class="li-required">serial_no</span> - Retrieve log from the specified device. <span class="li-normal">type: string </span> </li>
                <li><span class="li-required">session_id</span> - Provide a session_id to continue getting data for that request. <span class="li-normal">type: int </span> </li>
                <li><span class="li-required">filter</span> - Filter expression(s). <span class="li-normal">type: string </span> </li>
                <li><span class="li-required">start</span> - Row number for the first row to return. <span class="li-normal">type: int </span> </li>
                <li><span class="li-required">is_ha_member</span> - Is the specified device an HA member. <span class="li-normal">type: boolean </span> </li>
                
            </ul>
        
        </li>
        memory_cifs_raw
        <li><span class="li-head">memory_cifs_raw</span> - Log data for the given log type in raw format. 
        <ul class="ul-self">
                <li><span class="li-required">rows</span> - Number of rows to return. <span class="li-normal">type: int </span> </li>
                <li><span class="li-required">serial_no</span> - Retrieve log from the specified device. <span class="li-normal">type: string </span> </li>
                <li><span class="li-required">session_id</span> - Provide a session_id to continue getting data for that request. <span class="li-normal">type: int </span> </li>
                <li><span class="li-required">filter</span> - Filter expression(s). <span class="li-normal">type: string </span> </li>
                <li><span class="li-required">start</span> - Row number for the first row to return. <span class="li-normal">type: int </span> </li>
                <li><span class="li-required">is_ha_member</span> - Is the specified device an HA member. <span class="li-normal">type: boolean </span> </li>
                
            </ul>
        
        </li>
        memory_dlp_raw
        <li><span class="li-head">memory_dlp_raw</span> - Log data for the given log type in raw format. 
        <ul class="ul-self">
                <li><span class="li-required">rows</span> - Number of rows to return. <span class="li-normal">type: int </span> </li>
                <li><span class="li-required">serial_no</span> - Retrieve log from the specified device. <span class="li-normal">type: string </span> </li>
                <li><span class="li-required">session_id</span> - Provide a session_id to continue getting data for that request. <span class="li-normal">type: int </span> </li>
                <li><span class="li-required">filter</span> - Filter expression(s). <span class="li-normal">type: string </span> </li>
                <li><span class="li-required">start</span> - Row number for the first row to return. <span class="li-normal">type: int </span> </li>
                <li><span class="li-required">is_ha_member</span> - Is the specified device an HA member. <span class="li-normal">type: boolean </span> </li>
                
            </ul>
        
        </li>
        memory_dns_raw
        <li><span class="li-head">memory_dns_raw</span> - Log data for the given log type in raw format. 
        <ul class="ul-self">
                <li><span class="li-required">rows</span> - Number of rows to return. <span class="li-normal">type: int </span> </li>
                <li><span class="li-required">serial_no</span> - Retrieve log from the specified device. <span class="li-normal">type: string </span> </li>
                <li><span class="li-required">session_id</span> - Provide a session_id to continue getting data for that request. <span class="li-normal">type: int </span> </li>
                <li><span class="li-required">filter</span> - Filter expression(s). <span class="li-normal">type: string </span> </li>
                <li><span class="li-required">start</span> - Row number for the first row to return. <span class="li-normal">type: int </span> </li>
                <li><span class="li-required">is_ha_member</span> - Is the specified device an HA member. <span class="li-normal">type: boolean </span> </li>
                
            </ul>
        
        </li>
        memory_emailfilter_raw
        <li><span class="li-head">memory_emailfilter_raw</span> - Log data for the given log type in raw format. 
        <ul class="ul-self">
                <li><span class="li-required">rows</span> - Number of rows to return. <span class="li-normal">type: int </span> </li>
                <li><span class="li-required">serial_no</span> - Retrieve log from the specified device. <span class="li-normal">type: string </span> </li>
                <li><span class="li-required">session_id</span> - Provide a session_id to continue getting data for that request. <span class="li-normal">type: int </span> </li>
                <li><span class="li-required">filter</span> - Filter expression(s). <span class="li-normal">type: string </span> </li>
                <li><span class="li-required">start</span> - Row number for the first row to return. <span class="li-normal">type: int </span> </li>
                <li><span class="li-required">is_ha_member</span> - Is the specified device an HA member. <span class="li-normal">type: boolean </span> </li>
                
            </ul>
        
        </li>
        memory_event_compliance-check
        <li><span class="li-head">memory_event_compliance-check</span> - Log data for the given log type (and subtype). Append '/raw' to retrieve in raw format. 
        <ul class="ul-self">
                <li><span class="li-required">rows</span> - Number of rows to return. <span class="li-normal">type: int </span> </li>
                <li><span class="li-required">extra</span> - Flag(s) for extra data to be included [reverse_lookup|country_id]. <span class="li-normal">type: string </span> </li>
                <li><span class="li-required">serial_no</span> - Retrieve log from the specified device. <span class="li-normal">type: string </span> </li>
                <li><span class="li-required">session_id</span> - Provide a session_id to continue getting data for that request. <span class="li-normal">type: int </span> </li>
                <li><span class="li-required">filter</span> - Filter expression(s). <span class="li-normal">type: string </span> </li>
                <li><span class="li-required">start</span> - Row number for the first row to return. <span class="li-normal">type: int </span> </li>
                <li><span class="li-required">is_ha_member</span> - Is the specified device an HA member. <span class="li-normal">type: boolean </span> </li>
                
            </ul>
        
        </li>
        memory_event_connector
        <li><span class="li-head">memory_event_connector</span> - Log data for the given log type (and subtype). Append '/raw' to retrieve in raw format. 
        <ul class="ul-self">
                <li><span class="li-required">rows</span> - Number of rows to return. <span class="li-normal">type: int </span> </li>
                <li><span class="li-required">extra</span> - Flag(s) for extra data to be included [reverse_lookup|country_id]. <span class="li-normal">type: string </span> </li>
                <li><span class="li-required">serial_no</span> - Retrieve log from the specified device. <span class="li-normal">type: string </span> </li>
                <li><span class="li-required">session_id</span> - Provide a session_id to continue getting data for that request. <span class="li-normal">type: int </span> </li>
                <li><span class="li-required">filter</span> - Filter expression(s). <span class="li-normal">type: string </span> </li>
                <li><span class="li-required">start</span> - Row number for the first row to return. <span class="li-normal">type: int </span> </li>
                <li><span class="li-required">is_ha_member</span> - Is the specified device an HA member. <span class="li-normal">type: boolean </span> </li>
                
            </ul>
        
        </li>
        memory_event_endpoint
        <li><span class="li-head">memory_event_endpoint</span> - Log data for the given log type (and subtype). Append '/raw' to retrieve in raw format. 
        <ul class="ul-self">
                <li><span class="li-required">rows</span> - Number of rows to return. <span class="li-normal">type: int </span> </li>
                <li><span class="li-required">extra</span> - Flag(s) for extra data to be included [reverse_lookup|country_id]. <span class="li-normal">type: string </span> </li>
                <li><span class="li-required">serial_no</span> - Retrieve log from the specified device. <span class="li-normal">type: string </span> </li>
                <li><span class="li-required">session_id</span> - Provide a session_id to continue getting data for that request. <span class="li-normal">type: int </span> </li>
                <li><span class="li-required">filter</span> - Filter expression(s). <span class="li-normal">type: string </span> </li>
                <li><span class="li-required">start</span> - Row number for the first row to return. <span class="li-normal">type: int </span> </li>
                <li><span class="li-required">is_ha_member</span> - Is the specified device an HA member. <span class="li-normal">type: boolean </span> </li>
                
            </ul>
        
        </li>
        memory_event_fortiextender
        <li><span class="li-head">memory_event_fortiextender</span> - Log data for the given log type (and subtype). Append '/raw' to retrieve in raw format. 
        <ul class="ul-self">
                <li><span class="li-required">rows</span> - Number of rows to return. <span class="li-normal">type: int </span> </li>
                <li><span class="li-required">extra</span> - Flag(s) for extra data to be included [reverse_lookup|country_id]. <span class="li-normal">type: string </span> </li>
                <li><span class="li-required">serial_no</span> - Retrieve log from the specified device. <span class="li-normal">type: string </span> </li>
                <li><span class="li-required">session_id</span> - Provide a session_id to continue getting data for that request. <span class="li-normal">type: int </span> </li>
                <li><span class="li-required">filter</span> - Filter expression(s). <span class="li-normal">type: string </span> </li>
                <li><span class="li-required">start</span> - Row number for the first row to return. <span class="li-normal">type: int </span> </li>
                <li><span class="li-required">is_ha_member</span> - Is the specified device an HA member. <span class="li-normal">type: boolean </span> </li>
                
            </ul>
        
        </li>
        memory_event_ha
        <li><span class="li-head">memory_event_ha</span> - Log data for the given log type (and subtype). Append '/raw' to retrieve in raw format. 
        <ul class="ul-self">
                <li><span class="li-required">rows</span> - Number of rows to return. <span class="li-normal">type: int </span> </li>
                <li><span class="li-required">extra</span> - Flag(s) for extra data to be included [reverse_lookup|country_id]. <span class="li-normal">type: string </span> </li>
                <li><span class="li-required">serial_no</span> - Retrieve log from the specified device. <span class="li-normal">type: string </span> </li>
                <li><span class="li-required">session_id</span> - Provide a session_id to continue getting data for that request. <span class="li-normal">type: int </span> </li>
                <li><span class="li-required">filter</span> - Filter expression(s). <span class="li-normal">type: string </span> </li>
                <li><span class="li-required">start</span> - Row number for the first row to return. <span class="li-normal">type: int </span> </li>
                <li><span class="li-required">is_ha_member</span> - Is the specified device an HA member. <span class="li-normal">type: boolean </span> </li>
                
            </ul>
        
        </li>
        memory_event_router
        <li><span class="li-head">memory_event_router</span> - Log data for the given log type (and subtype). Append '/raw' to retrieve in raw format. 
        <ul class="ul-self">
                <li><span class="li-required">rows</span> - Number of rows to return. <span class="li-normal">type: int </span> </li>
                <li><span class="li-required">extra</span> - Flag(s) for extra data to be included [reverse_lookup|country_id]. <span class="li-normal">type: string </span> </li>
                <li><span class="li-required">serial_no</span> - Retrieve log from the specified device. <span class="li-normal">type: string </span> </li>
                <li><span class="li-required">session_id</span> - Provide a session_id to continue getting data for that request. <span class="li-normal">type: int </span> </li>
                <li><span class="li-required">filter</span> - Filter expression(s). <span class="li-normal">type: string </span> </li>
                <li><span class="li-required">start</span> - Row number for the first row to return. <span class="li-normal">type: int </span> </li>
                <li><span class="li-required">is_ha_member</span> - Is the specified device an HA member. <span class="li-normal">type: boolean </span> </li>
                
            </ul>
        
        </li>
        memory_event_security-rating
        <li><span class="li-head">memory_event_security-rating</span> - Log data for the given log type (and subtype). Append '/raw' to retrieve in raw format. 
        <ul class="ul-self">
                <li><span class="li-required">rows</span> - Number of rows to return. <span class="li-normal">type: int </span> </li>
                <li><span class="li-required">extra</span> - Flag(s) for extra data to be included [reverse_lookup|country_id]. <span class="li-normal">type: string </span> </li>
                <li><span class="li-required">serial_no</span> - Retrieve log from the specified device. <span class="li-normal">type: string </span> </li>
                <li><span class="li-required">session_id</span> - Provide a session_id to continue getting data for that request. <span class="li-normal">type: int </span> </li>
                <li><span class="li-required">filter</span> - Filter expression(s). <span class="li-normal">type: string </span> </li>
                <li><span class="li-required">start</span> - Row number for the first row to return. <span class="li-normal">type: int </span> </li>
                <li><span class="li-required">is_ha_member</span> - Is the specified device an HA member. <span class="li-normal">type: boolean </span> </li>
                
            </ul>
        
        </li>
        memory_event_system
        <li><span class="li-head">memory_event_system</span> - Log data for the given log type (and subtype). Append '/raw' to retrieve in raw format. 
        <ul class="ul-self">
                <li><span class="li-required">rows</span> - Number of rows to return. <span class="li-normal">type: int </span> </li>
                <li><span class="li-required">extra</span> - Flag(s) for extra data to be included [reverse_lookup|country_id]. <span class="li-normal">type: string </span> </li>
                <li><span class="li-required">serial_no</span> - Retrieve log from the specified device. <span class="li-normal">type: string </span> </li>
                <li><span class="li-required">session_id</span> - Provide a session_id to continue getting data for that request. <span class="li-normal">type: int </span> </li>
                <li><span class="li-required">filter</span> - Filter expression(s). <span class="li-normal">type: string </span> </li>
                <li><span class="li-required">start</span> - Row number for the first row to return. <span class="li-normal">type: int </span> </li>
                <li><span class="li-required">is_ha_member</span> - Is the specified device an HA member. <span class="li-normal">type: boolean </span> </li>
                
            </ul>
        
        </li>
        memory_event_user
        <li><span class="li-head">memory_event_user</span> - Log data for the given log type (and subtype). Append '/raw' to retrieve in raw format. 
        <ul class="ul-self">
                <li><span class="li-required">rows</span> - Number of rows to return. <span class="li-normal">type: int </span> </li>
                <li><span class="li-required">extra</span> - Flag(s) for extra data to be included [reverse_lookup|country_id]. <span class="li-normal">type: string </span> </li>
                <li><span class="li-required">serial_no</span> - Retrieve log from the specified device. <span class="li-normal">type: string </span> </li>
                <li><span class="li-required">session_id</span> - Provide a session_id to continue getting data for that request. <span class="li-normal">type: int </span> </li>
                <li><span class="li-required">filter</span> - Filter expression(s). <span class="li-normal">type: string </span> </li>
                <li><span class="li-required">start</span> - Row number for the first row to return. <span class="li-normal">type: int </span> </li>
                <li><span class="li-required">is_ha_member</span> - Is the specified device an HA member. <span class="li-normal">type: boolean </span> </li>
                
            </ul>
        
        </li>
        memory_event_vpn
        <li><span class="li-head">memory_event_vpn</span> - Log data for the given log type (and subtype). Append '/raw' to retrieve in raw format. 
        <ul class="ul-self">
                <li><span class="li-required">rows</span> - Number of rows to return. <span class="li-normal">type: int </span> </li>
                <li><span class="li-required">extra</span> - Flag(s) for extra data to be included [reverse_lookup|country_id]. <span class="li-normal">type: string </span> </li>
                <li><span class="li-required">serial_no</span> - Retrieve log from the specified device. <span class="li-normal">type: string </span> </li>
                <li><span class="li-required">session_id</span> - Provide a session_id to continue getting data for that request. <span class="li-normal">type: int </span> </li>
                <li><span class="li-required">filter</span> - Filter expression(s). <span class="li-normal">type: string </span> </li>
                <li><span class="li-required">start</span> - Row number for the first row to return. <span class="li-normal">type: int </span> </li>
                <li><span class="li-required">is_ha_member</span> - Is the specified device an HA member. <span class="li-normal">type: boolean </span> </li>
                
            </ul>
        
        </li>
        memory_event_wad
        <li><span class="li-head">memory_event_wad</span> - Log data for the given log type (and subtype). Append '/raw' to retrieve in raw format. 
        <ul class="ul-self">
                <li><span class="li-required">rows</span> - Number of rows to return. <span class="li-normal">type: int </span> </li>
                <li><span class="li-required">extra</span> - Flag(s) for extra data to be included [reverse_lookup|country_id]. <span class="li-normal">type: string </span> </li>
                <li><span class="li-required">serial_no</span> - Retrieve log from the specified device. <span class="li-normal">type: string </span> </li>
                <li><span class="li-required">session_id</span> - Provide a session_id to continue getting data for that request. <span class="li-normal">type: int </span> </li>
                <li><span class="li-required">filter</span> - Filter expression(s). <span class="li-normal">type: string </span> </li>
                <li><span class="li-required">start</span> - Row number for the first row to return. <span class="li-normal">type: int </span> </li>
                <li><span class="li-required">is_ha_member</span> - Is the specified device an HA member. <span class="li-normal">type: boolean </span> </li>
                
            </ul>
        
        </li>
        memory_event_wireless
        <li><span class="li-head">memory_event_wireless</span> - Log data for the given log type (and subtype). Append '/raw' to retrieve in raw format. 
        <ul class="ul-self">
                <li><span class="li-required">rows</span> - Number of rows to return. <span class="li-normal">type: int </span> </li>
                <li><span class="li-required">extra</span> - Flag(s) for extra data to be included [reverse_lookup|country_id]. <span class="li-normal">type: string </span> </li>
                <li><span class="li-required">serial_no</span> - Retrieve log from the specified device. <span class="li-normal">type: string </span> </li>
                <li><span class="li-required">session_id</span> - Provide a session_id to continue getting data for that request. <span class="li-normal">type: int </span> </li>
                <li><span class="li-required">filter</span> - Filter expression(s). <span class="li-normal">type: string </span> </li>
                <li><span class="li-required">start</span> - Row number for the first row to return. <span class="li-normal">type: int </span> </li>
                <li><span class="li-required">is_ha_member</span> - Is the specified device an HA member. <span class="li-normal">type: boolean </span> </li>
                
            </ul>
        
        </li>
        memory_file-filter_raw
        <li><span class="li-head">memory_file-filter_raw</span> - Log data for the given log type in raw format. 
        <ul class="ul-self">
                <li><span class="li-required">rows</span> - Number of rows to return. <span class="li-normal">type: int </span> </li>
                <li><span class="li-required">serial_no</span> - Retrieve log from the specified device. <span class="li-normal">type: string </span> </li>
                <li><span class="li-required">session_id</span> - Provide a session_id to continue getting data for that request. <span class="li-normal">type: int </span> </li>
                <li><span class="li-required">filter</span> - Filter expression(s). <span class="li-normal">type: string </span> </li>
                <li><span class="li-required">start</span> - Row number for the first row to return. <span class="li-normal">type: int </span> </li>
                <li><span class="li-required">is_ha_member</span> - Is the specified device an HA member. <span class="li-normal">type: boolean </span> </li>
                
            </ul>
        
        </li>
        memory_gtp_raw
        <li><span class="li-head">memory_gtp_raw</span> - Log data for the given log type in raw format. 
        <ul class="ul-self">
                <li><span class="li-required">rows</span> - Number of rows to return. <span class="li-normal">type: int </span> </li>
                <li><span class="li-required">serial_no</span> - Retrieve log from the specified device. <span class="li-normal">type: string </span> </li>
                <li><span class="li-required">session_id</span> - Provide a session_id to continue getting data for that request. <span class="li-normal">type: int </span> </li>
                <li><span class="li-required">filter</span> - Filter expression(s). <span class="li-normal">type: string </span> </li>
                <li><span class="li-required">start</span> - Row number for the first row to return. <span class="li-normal">type: int </span> </li>
                <li><span class="li-required">is_ha_member</span> - Is the specified device an HA member. <span class="li-normal">type: boolean </span> </li>
                
            </ul>
        
        </li>
        memory_ips_archive
        <li><span class="li-head">memory_ips_archive</span> - Return a list of archived items for the desired type. :type can be app-ctrl or ips 
        <ul class="ul-self">
                <li><span class="li-required">roll</span> - Log roll number. (required if source is not fortianalyzer) <span class="li-normal">type: int </span> </li>
                <li><span class="li-required">mkey</span> - Archive identifier. <span class="li-normal">type: int </span> </li>
                
            </ul>
        
        </li>
        memory_ips_archive-download
        <li><span class="li-head">memory_ips_archive-download</span> - Download an archived file. 
        <ul class="ul-self">
                <li><span class="li-required">roll</span> - Log roll number (required if source is not fortianalyzer). <span class="li-normal">type: int </span> </li>
                <li><span class="li-required">mkey</span> - Archive identifier. <span class="li-normal">type: int </span> </li>
                <li><span class="li-required">filename</span> - File name to use when saving the file in the browser. <span class="li-normal">type: string </span> </li>
                
            </ul>
        
        </li>
        memory_ips_raw
        <li><span class="li-head">memory_ips_raw</span> - Log data for the given log type in raw format. 
        <ul class="ul-self">
                <li><span class="li-required">rows</span> - Number of rows to return. <span class="li-normal">type: int </span> </li>
                <li><span class="li-required">serial_no</span> - Retrieve log from the specified device. <span class="li-normal">type: string </span> </li>
                <li><span class="li-required">session_id</span> - Provide a session_id to continue getting data for that request. <span class="li-normal">type: int </span> </li>
                <li><span class="li-required">filter</span> - Filter expression(s). <span class="li-normal">type: string </span> </li>
                <li><span class="li-required">start</span> - Row number for the first row to return. <span class="li-normal">type: int </span> </li>
                <li><span class="li-required">is_ha_member</span> - Is the specified device an HA member. <span class="li-normal">type: boolean </span> </li>
                
            </ul>
        
        </li>
        memory_ssh_raw
        <li><span class="li-head">memory_ssh_raw</span> - Log data for the given log type in raw format. 
        <ul class="ul-self">
                <li><span class="li-required">rows</span> - Number of rows to return. <span class="li-normal">type: int </span> </li>
                <li><span class="li-required">serial_no</span> - Retrieve log from the specified device. <span class="li-normal">type: string </span> </li>
                <li><span class="li-required">session_id</span> - Provide a session_id to continue getting data for that request. <span class="li-normal">type: int </span> </li>
                <li><span class="li-required">filter</span> - Filter expression(s). <span class="li-normal">type: string </span> </li>
                <li><span class="li-required">start</span> - Row number for the first row to return. <span class="li-normal">type: int </span> </li>
                <li><span class="li-required">is_ha_member</span> - Is the specified device an HA member. <span class="li-normal">type: boolean </span> </li>
                
            </ul>
        
        </li>
        memory_ssl_raw
        <li><span class="li-head">memory_ssl_raw</span> - Log data for the given log type in raw format. 
        <ul class="ul-self">
                <li><span class="li-required">rows</span> - Number of rows to return. <span class="li-normal">type: int </span> </li>
                <li><span class="li-required">serial_no</span> - Retrieve log from the specified device. <span class="li-normal">type: string </span> </li>
                <li><span class="li-required">session_id</span> - Provide a session_id to continue getting data for that request. <span class="li-normal">type: int </span> </li>
                <li><span class="li-required">filter</span> - Filter expression(s). <span class="li-normal">type: string </span> </li>
                <li><span class="li-required">start</span> - Row number for the first row to return. <span class="li-normal">type: int </span> </li>
                <li><span class="li-required">is_ha_member</span> - Is the specified device an HA member. <span class="li-normal">type: boolean </span> </li>
                
            </ul>
        
        </li>
        memory_traffic_fortiview
        <li><span class="li-head">memory_traffic_fortiview</span> - Log data for the given log type (and subtype). Append '/raw' to retrieve in raw format. 
        <ul class="ul-self">
                <li><span class="li-required">rows</span> - Number of rows to return. <span class="li-normal">type: int </span> </li>
                <li><span class="li-required">extra</span> - Flag(s) for extra data to be included [reverse_lookup|country_id]. <span class="li-normal">type: string </span> </li>
                <li><span class="li-required">serial_no</span> - Retrieve log from the specified device. <span class="li-normal">type: string </span> </li>
                <li><span class="li-required">session_id</span> - Provide a session_id to continue getting data for that request. <span class="li-normal">type: int </span> </li>
                <li><span class="li-required">filter</span> - Filter expression(s). <span class="li-normal">type: string </span> </li>
                <li><span class="li-required">start</span> - Row number for the first row to return. <span class="li-normal">type: int </span> </li>
                <li><span class="li-required">is_ha_member</span> - Is the specified device an HA member. <span class="li-normal">type: boolean </span> </li>
                
            </ul>
        
        </li>
        memory_traffic_forward
        <li><span class="li-head">memory_traffic_forward</span> - Log data for the given log type (and subtype). Append '/raw' to retrieve in raw format. 
        <ul class="ul-self">
                <li><span class="li-required">rows</span> - Number of rows to return. <span class="li-normal">type: int </span> </li>
                <li><span class="li-required">extra</span> - Flag(s) for extra data to be included [reverse_lookup|country_id]. <span class="li-normal">type: string </span> </li>
                <li><span class="li-required">serial_no</span> - Retrieve log from the specified device. <span class="li-normal">type: string </span> </li>
                <li><span class="li-required">session_id</span> - Provide a session_id to continue getting data for that request. <span class="li-normal">type: int </span> </li>
                <li><span class="li-required">filter</span> - Filter expression(s). <span class="li-normal">type: string </span> </li>
                <li><span class="li-required">start</span> - Row number for the first row to return. <span class="li-normal">type: int </span> </li>
                <li><span class="li-required">is_ha_member</span> - Is the specified device an HA member. <span class="li-normal">type: boolean </span> </li>
                
            </ul>
        
        </li>
        memory_traffic_local
        <li><span class="li-head">memory_traffic_local</span> - Log data for the given log type (and subtype). Append '/raw' to retrieve in raw format. 
        <ul class="ul-self">
                <li><span class="li-required">rows</span> - Number of rows to return. <span class="li-normal">type: int </span> </li>
                <li><span class="li-required">extra</span> - Flag(s) for extra data to be included [reverse_lookup|country_id]. <span class="li-normal">type: string </span> </li>
                <li><span class="li-required">serial_no</span> - Retrieve log from the specified device. <span class="li-normal">type: string </span> </li>
                <li><span class="li-required">session_id</span> - Provide a session_id to continue getting data for that request. <span class="li-normal">type: int </span> </li>
                <li><span class="li-required">filter</span> - Filter expression(s). <span class="li-normal">type: string </span> </li>
                <li><span class="li-required">start</span> - Row number for the first row to return. <span class="li-normal">type: int </span> </li>
                <li><span class="li-required">is_ha_member</span> - Is the specified device an HA member. <span class="li-normal">type: boolean </span> </li>
                
            </ul>
        
        </li>
        memory_traffic_multicast
        <li><span class="li-head">memory_traffic_multicast</span> - Log data for the given log type (and subtype). Append '/raw' to retrieve in raw format. 
        <ul class="ul-self">
                <li><span class="li-required">rows</span> - Number of rows to return. <span class="li-normal">type: int </span> </li>
                <li><span class="li-required">extra</span> - Flag(s) for extra data to be included [reverse_lookup|country_id]. <span class="li-normal">type: string </span> </li>
                <li><span class="li-required">serial_no</span> - Retrieve log from the specified device. <span class="li-normal">type: string </span> </li>
                <li><span class="li-required">session_id</span> - Provide a session_id to continue getting data for that request. <span class="li-normal">type: int </span> </li>
                <li><span class="li-required">filter</span> - Filter expression(s). <span class="li-normal">type: string </span> </li>
                <li><span class="li-required">start</span> - Row number for the first row to return. <span class="li-normal">type: int </span> </li>
                <li><span class="li-required">is_ha_member</span> - Is the specified device an HA member. <span class="li-normal">type: boolean </span> </li>
                
            </ul>
        
        </li>
        memory_traffic_sniffer
        <li><span class="li-head">memory_traffic_sniffer</span> - Log data for the given log type (and subtype). Append '/raw' to retrieve in raw format. 
        <ul class="ul-self">
                <li><span class="li-required">rows</span> - Number of rows to return. <span class="li-normal">type: int </span> </li>
                <li><span class="li-required">extra</span> - Flag(s) for extra data to be included [reverse_lookup|country_id]. <span class="li-normal">type: string </span> </li>
                <li><span class="li-required">serial_no</span> - Retrieve log from the specified device. <span class="li-normal">type: string </span> </li>
                <li><span class="li-required">session_id</span> - Provide a session_id to continue getting data for that request. <span class="li-normal">type: int </span> </li>
                <li><span class="li-required">filter</span> - Filter expression(s). <span class="li-normal">type: string </span> </li>
                <li><span class="li-required">start</span> - Row number for the first row to return. <span class="li-normal">type: int </span> </li>
                <li><span class="li-required">is_ha_member</span> - Is the specified device an HA member. <span class="li-normal">type: boolean </span> </li>
                
            </ul>
        
        </li>
        memory_traffic_threat
        <li><span class="li-head">memory_traffic_threat</span> - Log data for the given log type (and subtype). Append '/raw' to retrieve in raw format. 
        <ul class="ul-self">
                <li><span class="li-required">rows</span> - Number of rows to return. <span class="li-normal">type: int </span> </li>
                <li><span class="li-required">extra</span> - Flag(s) for extra data to be included [reverse_lookup|country_id]. <span class="li-normal">type: string </span> </li>
                <li><span class="li-required">serial_no</span> - Retrieve log from the specified device. <span class="li-normal">type: string </span> </li>
                <li><span class="li-required">session_id</span> - Provide a session_id to continue getting data for that request. <span class="li-normal">type: int </span> </li>
                <li><span class="li-required">filter</span> - Filter expression(s). <span class="li-normal">type: string </span> </li>
                <li><span class="li-required">start</span> - Row number for the first row to return. <span class="li-normal">type: int </span> </li>
                <li><span class="li-required">is_ha_member</span> - Is the specified device an HA member. <span class="li-normal">type: boolean </span> </li>
                
            </ul>
        
        </li>
        memory_virus_archive
        <li><span class="li-head">memory_virus_archive</span> - Return a description of the quarantined virus file. 
        <ul class="ul-self">
                <li><span class="li-required">mkey</span> - checksum column from the virus log. <span class="li-normal">type: int </span> </li>
                <li><span class="li-required">filename</span> - Filename of the antivirus archive. (virus type only) <span class="li-normal">type: string </span> </li>
                
            </ul>
        
        </li>
        memory_virus_raw
        <li><span class="li-head">memory_virus_raw</span> - Log data for the given log type in raw format. 
        <ul class="ul-self">
                <li><span class="li-required">rows</span> - Number of rows to return. <span class="li-normal">type: int </span> </li>
                <li><span class="li-required">serial_no</span> - Retrieve log from the specified device. <span class="li-normal">type: string </span> </li>
                <li><span class="li-required">session_id</span> - Provide a session_id to continue getting data for that request. <span class="li-normal">type: int </span> </li>
                <li><span class="li-required">filter</span> - Filter expression(s). <span class="li-normal">type: string </span> </li>
                <li><span class="li-required">start</span> - Row number for the first row to return. <span class="li-normal">type: int </span> </li>
                <li><span class="li-required">is_ha_member</span> - Is the specified device an HA member. <span class="li-normal">type: boolean </span> </li>
                
            </ul>
        
        </li>
        memory_voip_raw
        <li><span class="li-head">memory_voip_raw</span> - Log data for the given log type in raw format. 
        <ul class="ul-self">
                <li><span class="li-required">rows</span> - Number of rows to return. <span class="li-normal">type: int </span> </li>
                <li><span class="li-required">serial_no</span> - Retrieve log from the specified device. <span class="li-normal">type: string </span> </li>
                <li><span class="li-required">session_id</span> - Provide a session_id to continue getting data for that request. <span class="li-normal">type: int </span> </li>
                <li><span class="li-required">filter</span> - Filter expression(s). <span class="li-normal">type: string </span> </li>
                <li><span class="li-required">start</span> - Row number for the first row to return. <span class="li-normal">type: int </span> </li>
                <li><span class="li-required">is_ha_member</span> - Is the specified device an HA member. <span class="li-normal">type: boolean </span> </li>
                
            </ul>
        
        </li>
        memory_waf_raw
        <li><span class="li-head">memory_waf_raw</span> - Log data for the given log type in raw format. 
        <ul class="ul-self">
                <li><span class="li-required">rows</span> - Number of rows to return. <span class="li-normal">type: int </span> </li>
                <li><span class="li-required">serial_no</span> - Retrieve log from the specified device. <span class="li-normal">type: string </span> </li>
                <li><span class="li-required">session_id</span> - Provide a session_id to continue getting data for that request. <span class="li-normal">type: int </span> </li>
                <li><span class="li-required">filter</span> - Filter expression(s). <span class="li-normal">type: string </span> </li>
                <li><span class="li-required">start</span> - Row number for the first row to return. <span class="li-normal">type: int </span> </li>
                <li><span class="li-required">is_ha_member</span> - Is the specified device an HA member. <span class="li-normal">type: boolean </span> </li>
                
            </ul>
        
        </li>
        memory_webfilter_raw
        <li><span class="li-head">memory_webfilter_raw</span> - Log data for the given log type in raw format. 
        <ul class="ul-self">
                <li><span class="li-required">rows</span> - Number of rows to return. <span class="li-normal">type: int </span> </li>
                <li><span class="li-required">serial_no</span> - Retrieve log from the specified device. <span class="li-normal">type: string </span> </li>
                <li><span class="li-required">session_id</span> - Provide a session_id to continue getting data for that request. <span class="li-normal">type: int </span> </li>
                <li><span class="li-required">filter</span> - Filter expression(s). <span class="li-normal">type: string </span> </li>
                <li><span class="li-required">start</span> - Row number for the first row to return. <span class="li-normal">type: int </span> </li>
                <li><span class="li-required">is_ha_member</span> - Is the specified device an HA member. <span class="li-normal">type: boolean </span> </li>
                
            </ul>
        
        </li>
        </ul>
        </div>
        </section>
    <li><span class="li-head">params</span> - the parameter for each selector, see definition in above list.<span class="li-normal">type: dict</span></li>


Notes
-----

.. note::

   - Different ``selector`` may have different parameters, users are expected to look up them for a specific selector.

   - For some selectors, the objects are global, no ``params`` are allowed to appear.

   - Not all parameters are required for a slector.

   - This module is exclusivly for FortiOS monitor API.

   - The result of API request is stored in ``results``.

   - There are three filtering parameters: ``filters``, ``sorters`` and ``formatters``, please see `filtering spec`_ for more information.

Examples
--------

.. code-block:: yaml+jinja

 - hosts: fortigate03
   connection: httpapi
   collections:
   - fortinet.fortios
   vars:
    vdom: "root"
    ansible_httpapi_use_ssl: yes
    ansible_httpapi_validate_certs: no
    ansible_httpapi_port: 443
   tasks:
   - name: Get system event log with logid==0100032038
     fortios_log_fact:
       filters:
         - logid==0100032038
       selector: "disk_event_system"
       params:
         rows: 100

   - name: Get a description of the quarantined virus file
     fortios_log_fact:
       selector: "forticloud_virus_archive"


Return Values
-------------
Common return values are documented: https://docs.ansible.com/ansible/latest/reference_appendices/common_return_values.html#common-return-values, the following are the fields unique to this module:

.. raw:: html

    <ul>

    <li> <span class="li-return">build</span> - Build number of the fortigate image <span class="li-normal">returned: always</span> <span class="li-normal">type: str</span> <span class="li-normal">sample: 1547</span></li>
    <li> <span class="li-return">rows</span> - Number of rows to return <span class="li-normal">returned: always</span> <span class="li-normal">type: int</span> <span class="li-normal">sample: 400</span></li>
    <li> <span class="li-return">serial</span> - Serial number of the unit <span class="li-normal">returned: always</span> <span class="li-normal">type: str</span> <span class="li-normal">sample: FGVMEVYYQT3AB5352</span></li>
    <li> <span class="li-return">session_id</span> - Session id for the request <span class="li-normal">returned: always</span> <span class="li-normal">type: int</span> <span class="li-normal">sample: 7</span></li>
    <li> <span class="li-return">start</span> - Row number for the first row to return <span class="li-normal">returned: always</span> <span class="li-normal">type: int</span> <span class="li-normal">sample: 0</span></li>
    <li> <span class="li-return">status</span> - Indication of the operation's result <span class="li-normal">returned: always</span> <span class="li-normal">type: str</span> <span class="li-normal">sample: success</span></li>
    <li> <span class="li-return">subcategory</span> - Type of log that can be retrieved <span class="li-normal">returned: always</span> <span class="li-normal">type: str</span> <span class="li-normal">sample: system</span></li>
    <li> <span class="li-return">total_lines</span> - Total lines returned from the result <span class="li-normal">returned: always</span> <span class="li-normal">type: int</span> <span class="li-normal">sample: 510</span></li>
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
- Frank Shen (@fshen01)


.. hint::
    If you notice any issues in this documentation, you can create a pull request to improve it.

.. _filtering spec: https://fndn.fortinet.net/index.php?/fortiapi/1-fortios/597/