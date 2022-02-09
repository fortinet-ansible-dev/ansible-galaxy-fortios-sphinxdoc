:source: fortios_monitor_fact.py

:orphan:

.. :

fortios_monitor_fact -- Retrieve Facts of FortiOS Monitor Objects.
++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++

.. versionadded:: 2.10

.. contents::
   :local:
   :depth: 1


Synopsis
--------
- Collects monitor facts from network devices running the fortios operating system.  This facts module will only collect those facts which user specified in playbook.



Requirements
------------
The below requirements are needed on the host that executes this module.

- install galaxy collection fortinet.fortios >= ``2.0.0``.


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
    <li><span class="li-head">selector</span> - selector of the retrieved fortigate facts <span class="li-normal">type: str</span> <span class="li-required">choices:</span></li>
        <li style="list-style: none;"><section class="accordion">
        <input type="checkbox" name="collapse" id="handle2">
        <h2 class="handle">
            <label for="handle2"><u>Show full selector list...</u></label>
        </h2>
        <div class="content">
        <ul class="ul-self">
        azure_application-list
        <li><span class="li-head">azure_application-list</span> 
        
        </li>
        endpoint-control_avatar_download
        <li><span class="li-head">endpoint-control_avatar_download</span> - Download an endpoint avatar image. 
        <ul class="ul-self">
                <li><span class="li-required">default</span> - Default avatar name ['authuser'|'unauthuser'|'authuser_72'|'unauthuser_72']. Default avatar when endpoint / device avatar is not available. If default is not set, Not found 404 is returned. <span class="li-normal">type: string</span> <span class="li-normal">required: False</span> </li>
                <li><span class="li-required">fingerprint</span> - Avatar fingerprint. <span class="li-normal">type: string</span> <span class="li-normal">required: False</span> </li>
                <li><span class="li-required">uid</span> - Single FortiClient UID. <span class="li-normal">type: string</span> <span class="li-normal">required: False</span> </li>
                <li><span class="li-required">user</span> - User name of the endpoint. <span class="li-normal">type: string</span> <span class="li-normal">required: False</span> </li>
                
            </ul>
        
        </li>
        endpoint-control_ems_cert-status
        <li><span class="li-head">endpoint-control_ems_cert-status</span> - Retrieve authentication status of the EMS server certificate for a specific EMS. 
        <ul class="ul-self">
                <li><span class="li-required">with_cert</span> - Return detailed certificate information. Available when the certificate is authenticated by installed CA certificates.  <span class="li-normal">type: boolean</span> <span class="li-normal">required: False</span> </li>
                <li><span class="li-required">ems_name</span> - EMS server name (as defined in CLI table endpoint-control.fctems). <span class="li-normal">type: string</span> <span class="li-normal">required: True</span> </li>
                
            </ul>
        
        </li>
        endpoint-control_ems_status
        <li><span class="li-head">endpoint-control_ems_status</span> - Retrieve EMS connection status for a specific EMS. 
        <ul class="ul-self">
                <li><span class="li-required">ems_name</span> - EMS server name (as defined in CLI table endpoint-control.fctems). <span class="li-normal">type: string</span> <span class="li-normal">required: False</span> </li>
                <li><span class="li-required">ems_serial</span> - EMS serial <span class="li-normal">type: string</span> <span class="li-normal">required: False</span> </li>
                
            </ul>
        
        </li>
        endpoint-control_ems_status-summary
        <li><span class="li-head">endpoint-control_ems_status-summary</span> 
        
        </li>
        endpoint-control_installer
        <li><span class="li-head">endpoint-control_installer</span> - List available FortiClient installers. 
        <ul class="ul-self">
                <li><span class="li-required">min_version</span> - Filter: Minimum installer version. (String of the format n[.n[.n]]). <span class="li-normal">type: string</span> <span class="li-normal">required: False</span> </li>
                
            </ul>
        
        </li>
        endpoint-control_installer_download
        <li><span class="li-head">endpoint-control_installer_download</span> - Download a FortiClient installer via FortiGuard. 
        <ul class="ul-self">
                <li><span class="li-required">mkey</span> - Name of installer (image_id). <span class="li-normal">type: string</span> <span class="li-normal">required: True</span> </li>
                
            </ul>
        
        </li>
        endpoint-control_profile_xml
        <li><span class="li-head">endpoint-control_profile_xml</span> - List XML representation for each endpoint-control profile. 
        <ul class="ul-self">
                <li><span class="li-required">mkey</span> - Name of endpoint-control profile. <span class="li-normal">type: string</span> <span class="li-normal">required: False</span> </li>
                
            </ul>
        
        </li>
        endpoint-control_record-list
        <li><span class="li-head">endpoint-control_record-list</span> - List endpoint records. This should only be used when you need to retrieve endpoint information from FortiEMS. 
        <ul class="ul-self">
                <li><span class="li-required">intf_name</span> - Filter: Name of interface where the endpoint was detected. <span class="li-normal">type: string</span> <span class="li-normal">required: False</span> </li>
                
            </ul>
        
        </li>
        endpoint-control_registration_summary
        <li><span class="li-head">endpoint-control_registration_summary</span> 
        
        </li>
        endpoint-control_summary
        <li><span class="li-head">endpoint-control_summary</span> 
        
        </li>
        extender-controller_extender
        <li><span class="li-head">extender-controller_extender</span> - Retrieve statistics for specific configured FortiExtender units. 
        <ul class="ul-self">
                <li><span class="li-required">type</span> - Statistic type.'type' options are [system | modem | usage | last]. If 'type' is not specified, all types of statistics are retrieved. <span class="li-normal">type: string</span> <span class="li-normal">required: False</span> </li>
                <li><span class="li-required">id</span> - FortiExtender ID. <span class="li-normal">type: string</span> <span class="li-normal">required: True</span> </li>
                <li><span class="li-required">name</span> - List of FortiExtender IDs to query. <span class="li-normal">type: array</span> <span class="li-normal">required: False</span> </li>
                
            </ul>
        
        </li>
        firewall_acl
        <li><span class="li-head">firewall_acl</span> 
        
        </li>
        firewall_acl6
        <li><span class="li-head">firewall_acl6</span> 
        
        </li>
        firewall_address-dynamic
        <li><span class="li-head">firewall_address-dynamic</span> 
        
        </li>
        firewall_address-fqdns
        <li><span class="li-head">firewall_address-fqdns</span> 
        
        </li>
        firewall_address-fqdns6
        <li><span class="li-head">firewall_address-fqdns6</span> 
        
        </li>
        firewall_address6-dynamic
        <li><span class="li-head">firewall_address6-dynamic</span> 
        
        </li>
        firewall_central-snat-map
        <li><span class="li-head">firewall_central-snat-map</span> - List traffic statistics for firewall central SNAT policies. 
        <ul class="ul-self">
                <li><span class="li-required">ip_version</span> - Filter: Traffic IP Version. [ ipv4 | ipv6 ], if left empty, will retrieve data for both IPv4 and IPv6. <span class="li-normal">type: string</span> <span class="li-normal">required: False</span> </li>
                <li><span class="li-required">policyid</span> - Filter: Policy ID. <span class="li-normal">type: int</span> <span class="li-normal">required: False</span> </li>
                
            </ul>
        
        </li>
        firewall_consolidated-policy
        <li><span class="li-head">firewall_consolidated-policy</span> - List traffic statistics for consolidated policies. 
        <ul class="ul-self">
                <li><span class="li-required">policyid</span> - Filter: Policy ID. <span class="li-normal">type: int</span> <span class="li-normal">required: False</span> </li>
                
            </ul>
        
        </li>
        firewall_dnat
        <li><span class="li-head">firewall_dnat</span> - List hit count statistics for firewall virtual IP/server. 
        <ul class="ul-self">
                <li><span class="li-required">ip_version</span> - Filter: Traffic IP Version. [ ipv4 | ipv6 ], if left empty, will retrieve data for both IPv4 and IPv6. <span class="li-normal">type: string</span> <span class="li-normal">required: False</span> </li>
                <li><span class="li-required">uuid</span> - Filter: Virtual IP's UUID. <span class="li-normal">type: string</span> <span class="li-normal">required: False</span> </li>
                
            </ul>
        
        </li>
        firewall_gtp-runtime-statistics
        <li><span class="li-head">firewall_gtp-runtime-statistics</span> 
        
        </li>
        firewall_gtp-statistics
        <li><span class="li-head">firewall_gtp-statistics</span> 
        
        </li>
        firewall_health
        <li><span class="li-head">firewall_health</span> 
        
        </li>
        firewall_internet-service-details
        <li><span class="li-head">firewall_internet-service-details</span> - List all details for a given Internet Service ID. 
        <ul class="ul-self">
                <li><span class="li-required">count</span> - Maximum number of entries to return. Valid range is [20, 1000]; if a value is specified out of that range, it will be rounded up or down. Default value is 1000. <span class="li-normal">type: int</span> <span class="li-normal">required: False</span> </li>
                <li><span class="li-required">region_id</span> - Filter: Region ID. <span class="li-normal">type: int</span> <span class="li-normal">required: False</span> </li>
                <li><span class="li-required">summary_only</span> - Only return number of entries instead of entries. <span class="li-normal">type: boolean</span> <span class="li-normal">required: False</span> </li>
                <li><span class="li-required">city_id</span> - Filter: City ID. <span class="li-normal">type: int</span> <span class="li-normal">required: False</span> </li>
                <li><span class="li-required">country_id</span> - Filter: Country ID. <span class="li-normal">type: int</span> <span class="li-normal">required: False</span> </li>
                <li><span class="li-required">start</span> - Starting entry index. If a value is less than zero, it will be set to zero. <span class="li-normal">type: int</span> <span class="li-normal">required: False</span> </li>
                <li><span class="li-required">id</span> - ID of the Internet Service to get details for. <span class="li-normal">type: int</span> <span class="li-normal">required: True</span> </li>
                
            </ul>
        
        </li>
        firewall_internet-service-match
        <li><span class="li-head">firewall_internet-service-match</span> - List internet services that exist at a given IP or Subnet. 
        <ul class="ul-self">
                <li><span class="li-required">ip</span> - IP (in dot-decimal notation). <span class="li-normal">type: string</span> <span class="li-normal">required: True</span> </li>
                <li><span class="li-required">mask</span> - IP Mask (in dot-decimal notation). <span class="li-normal">type: string</span> <span class="li-normal">required: True</span> </li>
                
            </ul>
        
        </li>
        firewall_ippool
        <li><span class="li-head">firewall_ippool</span> 
        
        </li>
        firewall_ippool_mapping
        <li><span class="li-head">firewall_ippool_mapping</span> - Get the list of IPv4 mappings for the specified IP pool. 
        <ul class="ul-self">
                <li><span class="li-required">mkey</span> - The IP pool name. <span class="li-normal">type: string</span> <span class="li-normal">required: True</span> </li>
                
            </ul>
        
        </li>
        firewall_load-balance
        <li><span class="li-head">firewall_load-balance</span> - List all firewall load balance servers. 
        <ul class="ul-self">
                <li><span class="li-required">count</span> - Maximum number of entries to return. <span class="li-normal">type: int</span> <span class="li-normal">required: True</span> </li>
                <li><span class="li-required">start</span> - Starting entry index. <span class="li-normal">type: int</span> <span class="li-normal">required: False</span> </li>
                
            </ul>
        
        </li>
        firewall_local-in
        <li><span class="li-head">firewall_local-in</span> 
        
        </li>
        firewall_multicast-policy
        <li><span class="li-head">firewall_multicast-policy</span> - List traffic statistics for IPv4 firewall multicast policies. 
        <ul class="ul-self">
                <li><span class="li-required">policyid</span> - Filter: Policy ID. <span class="li-normal">type: int</span> <span class="li-normal">required: False</span> </li>
                
            </ul>
        
        </li>
        firewall_multicast-policy6
        <li><span class="li-head">firewall_multicast-policy6</span> - List traffic statistics for IPv6 firewall multicast policies. 
        <ul class="ul-self">
                <li><span class="li-required">policyid</span> - Filter: Policy ID. <span class="li-normal">type: int</span> <span class="li-normal">required: False</span> </li>
                
            </ul>
        
        </li>
        firewall_per-ip-shaper
        <li><span class="li-head">firewall_per-ip-shaper</span> 
        
        </li>
        firewall_policy
        <li><span class="li-head">firewall_policy</span> - List traffic statistics for firewall policies. 
        <ul class="ul-self">
                <li><span class="li-required">ip_version</span> - Filter: Traffic IP Version. [ ipv4 | ipv6 ], if left empty, will retrieve data for both ipv4 and ipv6. <span class="li-normal">type: string</span> <span class="li-normal">required: False</span> </li>
                <li><span class="li-required">policyid</span> - Filter: Policy ID. <span class="li-normal">type: int</span> <span class="li-normal">required: False</span> </li>
                
            </ul>
        
        </li>
        firewall_policy-lookup
        <li><span class="li-head">firewall_policy-lookup</span> - Performs a policy lookup by creating a dummy packet and asking the kernel which policy would be hit. 
        <ul class="ul-self">
                <li><span class="li-required">protocol</span> - Protocol. <span class="li-normal">type: string</span> <span class="li-normal">required: True</span> </li>
                <li><span class="li-required">dest</span> - Destination IP/FQDN. <span class="li-normal">type: string</span> <span class="li-normal">required: True</span> </li>
                <li><span class="li-required">icmpcode</span> - ICMP code. <span class="li-normal">type: int</span> <span class="li-normal">required: False</span> </li>
                <li><span class="li-required">icmptype</span> - ICMP type. <span class="li-normal">type: int</span> <span class="li-normal">required: False</span> </li>
                <li><span class="li-required">srcintf</span> - Source interface. <span class="li-normal">type: string</span> <span class="li-normal">required: True</span> </li>
                <li><span class="li-required">ipv6</span> - Perform an IPv6 lookup? <span class="li-normal">type: boolean</span> <span class="li-normal">required: False</span> </li>
                <li><span class="li-required">sourceport</span> - Source port. <span class="li-normal">type: int</span> <span class="li-normal">required: False</span> </li>
                <li><span class="li-required">sourceip</span> - Source IP. <span class="li-normal">type: string</span> <span class="li-normal">required: False</span> </li>
                <li><span class="li-required">destport</span> - Destination port. <span class="li-normal">type: int</span> <span class="li-normal">required: False</span> </li>
                
            </ul>
        
        </li>
        firewall_policy6
        <li><span class="li-head">firewall_policy6</span> - List traffic statistics for IPv6 policies. 
        <ul class="ul-self">
                <li><span class="li-required">policyid</span> - Filter: Policy ID. <span class="li-normal">type: int</span> <span class="li-normal">required: False</span> </li>
                
            </ul>
        
        </li>
        firewall_proxy-policy
        <li><span class="li-head">firewall_proxy-policy</span> - List traffic statistics for all explicit proxy policies. 
        <ul class="ul-self">
                <li><span class="li-required">policyid</span> - Filter: Policy ID. <span class="li-normal">type: int</span> <span class="li-normal">required: False</span> </li>
                
            </ul>
        
        </li>
        firewall_sdn-connector-filters
        <li><span class="li-head">firewall_sdn-connector-filters</span> - List all available filters for a specified SDN Fabric Connector. Used for Fabric Connector address objects. 
        <ul class="ul-self">
                <li><span class="li-required">connector</span> - Name of the SDN Fabric Connector to get the filters from. <span class="li-normal">type: string</span> <span class="li-normal">required: True</span> </li>
                
            </ul>
        
        </li>
        firewall_security-policy
        <li><span class="li-head">firewall_security-policy</span> - List IPS engine statistics for security policies. 
        <ul class="ul-self">
                <li><span class="li-required">policyid</span> - Filter: Policy ID. <span class="li-normal">type: int</span> <span class="li-normal">required: False</span> </li>
                
            </ul>
        
        </li>
        firewall_session
        <li><span class="li-head">firewall_session</span> - List all active firewall sessions (optionally filtered). 
        <ul class="ul-self">
                <li><span class="li-required">since</span> - Filter: Only return sessions generated since this Unix timestamp. <span class="li-normal">type: int</span> <span class="li-normal">required: False</span> </li>
                <li><span class="li-required">protocol</span> - Filter: Protocol name [all|igmp|tcp|udp|icmp|etc]. <span class="li-normal">type: string</span> <span class="li-normal">required: False</span> </li>
                <li><span class="li-required">web-domain</span> - Filter: Web domain. <span class="li-normal">type: string</span> <span class="li-normal">required: False</span> </li>
                <li><span class="li-required">srcintfrole</span> - Filter: Source interface roles. <span class="li-normal">type: array</span> <span class="li-normal">required: False</span> </li>
                <li><span class="li-required">owner</span> - Filter: Destination owner. <span class="li-normal">type: string</span> <span class="li-normal">required: False</span> </li>
                <li><span class="li-required">srcuuid</span> - Filter: Source UUID. <span class="li-normal">type: string</span> <span class="li-normal">required: False</span> </li>
                <li><span class="li-required">dstintfrole</span> - Filter: Destination interface roles. <span class="li-normal">type: array</span> <span class="li-normal">required: False</span> </li>
                <li><span class="li-required">security-policyid</span> - Filter: Security Policy ID. <span class="li-normal">type: int</span> <span class="li-normal">required: False</span> </li>
                <li><span class="li-required">natsourceaddress</span> - Filter: NAT source address. <span class="li-normal">type: string</span> <span class="li-normal">required: False</span> </li>
                <li><span class="li-required">source</span> - Filter: Source IP address. <span class="li-normal">type: string</span> <span class="li-normal">required: False</span> </li>
                <li><span class="li-required">destination</span> - Filter: Destination IP address. <span class="li-normal">type: string</span> <span class="li-normal">required: False</span> </li>
                <li><span class="li-required">application</span> - Filter: Application PROTO/PORT. (e.g. "TCP/443") <span class="li-normal">type: string</span> <span class="li-normal">required: False</span> </li>
                <li><span class="li-required">sourceport</span> - Filter: Source port. <span class="li-normal">type: int</span> <span class="li-normal">required: False</span> </li>
                <li><span class="li-required">natsourceport</span> - Filter: NAT source port. <span class="li-normal">type: int</span> <span class="li-normal">required: False</span> </li>
                <li><span class="li-required">start</span> - Starting entry index. <span class="li-normal">type: int</span> <span class="li-normal">required: False</span> </li>
                <li><span class="li-required">dstuuid</span> - Filter: Destination UUID. <span class="li-normal">type: string</span> <span class="li-normal">required: False</span> </li>
                <li><span class="li-required">username</span> - Filter: Authenticated username. <span class="li-normal">type: string</span> <span class="li-normal">required: False</span> </li>
                <li><span class="li-required">seconds</span> - Filter: Only return sessions generated in the last N seconds. <span class="li-normal">type: int</span> <span class="li-normal">required: False</span> </li>
                <li><span class="li-required">policyid</span> - Filter: Policy ID. <span class="li-normal">type: int</span> <span class="li-normal">required: False</span> </li>
                <li><span class="li-required">srcintf</span> - Filter: Source interface name. <span class="li-normal">type: string</span> <span class="li-normal">required: False</span> </li>
                <li><span class="li-required">destport</span> - Filter: Destination port. <span class="li-normal">type: int</span> <span class="li-normal">required: False</span> </li>
                <li><span class="li-required">count</span> - Maximum number of entries to return. Valid range is [20, 1000]; if a value is specified out of that range, it will be rounded up or down. <span class="li-normal">type: int</span> <span class="li-normal">required: True</span> </li>
                <li><span class="li-required">filter-csf</span> - Filter: Include sessions from downstream fortigates. <span class="li-normal">type: boolean</span> <span class="li-normal">required: False</span> </li>
                <li><span class="li-required">country</span> - Filter: Destination country name. <span class="li-normal">type: string</span> <span class="li-normal">required: False</span> </li>
                <li><span class="li-required">summary</span> - Enable/disable inclusion of session summary (setup rate, total sessions, etc). <span class="li-normal">type: boolean</span> <span class="li-normal">required: False</span> </li>
                <li><span class="li-required">shaper</span> - Filter: Forward traffic shaper name. <span class="li-normal">type: string</span> <span class="li-normal">required: False</span> </li>
                <li><span class="li-required">web-category</span> - Filter: Web category. <span class="li-normal">type: string</span> <span class="li-normal">required: False</span> </li>
                <li><span class="li-required">ip_version</span> - IP version [*ipv4 | ipv6 | ipboth]. <span class="li-normal">type: string</span> <span class="li-normal">required: False</span> </li>
                <li><span class="li-required">dstintf</span> - Filter: Destination interface name. <span class="li-normal">type: string</span> <span class="li-normal">required: False</span> </li>
                
            </ul>
        
        </li>
        firewall_shaper
        <li><span class="li-head">firewall_shaper</span> 
        
        </li>
        firewall_uuid-list
        <li><span class="li-head">firewall_uuid-list</span> 
        
        </li>
        firewall_uuid-type-lookup
        <li><span class="li-head">firewall_uuid-type-lookup</span> - Retrieve a mapping of UUIDs to their firewall object type for given UUIDs. 
        <ul class="ul-self">
                <li><span class="li-required">uuids</span> - List of UUIDs to be resolved. <span class="li-normal">type: array</span> <span class="li-normal">required: False</span> </li>
                
            </ul>
        
        </li>
        fortiguard_redirect-portal
        <li><span class="li-head">fortiguard_redirect-portal</span> 
        
        </li>
        fortiguard_service-communication-stats
        <li><span class="li-head">fortiguard_service-communication-stats</span> - Retrieve historical statistics for communication with FortiGuard services. 
        <ul class="ul-self">
                <li><span class="li-required">service_type</span> - To get stats for [forticare|fortiguard_download|fortiguard_query|forticloud_log|fortisandbox_cloud|fortiguard.com|ocvpn|sdns|fortitoken_registration|sms_service]. Defaults to all stats if not provided. <span class="li-normal">type: string</span> <span class="li-normal">required: False</span> </li>
                <li><span class="li-required">timeslot</span> - History timeslot of stats [1_hour|24_hour|1_week]. Defaults to all timeslots if not provided. <span class="li-normal">type: string</span> <span class="li-normal">required: False</span> </li>
                
            </ul>
        
        </li>
        fortiview_sandbox-file-details
        <li><span class="li-head">fortiview_sandbox-file-details</span> - Retrieve FortiSandbox analysis details for a specific file checksum. 
        <ul class="ul-self">
                <li><span class="li-required">checksum</span> - Checksum of a specific file that has been analyzed by the connected FortiSandbox. <span class="li-normal">type: string</span> <span class="li-normal">required: True</span> </li>
                
            </ul>
        
        </li>
        fortiview_sandbox-file-list
        <li><span class="li-head">fortiview_sandbox-file-list</span> 
        
        </li>
        fortiview_statistics
        <li><span class="li-head">fortiview_statistics</span> - Retrieve drill-down and summary data for FortiView (both realtime and historical). 
        <ul class="ul-self">
                <li><span class="li-required">count</span> - Maximum number of details to return. <span class="li-normal">type: int</span> <span class="li-normal">required: False</span> </li>
                <li><span class="li-required">end</span> - End timestamp. <span class="li-normal">type: int</span> <span class="li-normal">required: False</span> </li>
                <li><span class="li-required">realtime</span> - Set to true to retrieve realtime results (from kernel). <span class="li-normal">type: boolean</span> <span class="li-normal">required: False</span> </li>
                <li><span class="li-required">chart_only</span> - Only return graph values in results. <span class="li-normal">type: boolean</span> <span class="li-normal">required: False</span> </li>
                <li><span class="li-required">sort_by</span> - Sort by field. <span class="li-normal">type: string</span> <span class="li-normal">required: False</span> </li>
                <li><span class="li-required">filter</span> - A map of filter keys to arrays of values. <span class="li-normal">type: object</span> <span class="li-normal">required: False</span> </li>
                <li><span class="li-required">start</span> - Start timestamp. <span class="li-normal">type: int</span> <span class="li-normal">required: False</span> </li>
                <li><span class="li-required">sessionid</span> - FortiView request Session ID. <span class="li-normal">type: int</span> <span class="li-normal">required: False</span> </li>
                <li><span class="li-required">report_by</span> - Report by field. <span class="li-normal">type: string</span> <span class="li-normal">required: False</span> </li>
                <li><span class="li-required">device</span> - FortiView source device [disk|fortianalyzer|forticloud]. <span class="li-normal">type: string</span> <span class="li-normal">required: False</span> </li>
                <li><span class="li-required">ip_version</span> - IP version [*ipv4 | ipv6 | ipboth]. <span class="li-normal">type: string</span> <span class="li-normal">required: False</span> </li>
                
            </ul>
        
        </li>
        ips_anomaly
        <li><span class="li-head">ips_anomaly</span> 
        
        </li>
        ips_exceed-scan-range
        <li><span class="li-head">ips_exceed-scan-range</span> - Returns a list of applications that exceed the scan range from a list of application IDs. 
        <ul class="ul-self">
                <li><span class="li-required">ids</span> - List of application IDs. <span class="li-normal">type: array</span> <span class="li-normal">required: True</span> </li>
                
            </ul>
        
        </li>
        ips_hold-signatures
        <li><span class="li-head">ips_hold-signatures</span> - Return a list of IPS signatures that are on hold due to active hold time. 
        <ul class="ul-self">
                <li><span class="li-required">ips_sensor</span> - Optional filter: Provide the name of the IPS sensor to retrieve only the hold signatures being used by that sensor. <span class="li-normal">type: string</span> <span class="li-normal">required: False</span> </li>
                
            </ul>
        
        </li>
        ips_metadata
        <li><span class="li-head">ips_metadata</span> 
        
        </li>
        ips_rate-based
        <li><span class="li-head">ips_rate-based</span> 
        
        </li>
        license_fortianalyzer-status
        <li><span class="li-head">license_fortianalyzer-status</span> 
        
        </li>
        license_forticare-org-list
        <li><span class="li-head">license_forticare-org-list</span> 
        
        </li>
        license_forticare-resellers
        <li><span class="li-head">license_forticare-resellers</span> - Get current FortiCare resellers for the requested country. 
        <ul class="ul-self">
                <li><span class="li-required">country_code</span> - FortiGuard country code <span class="li-normal">type: int</span> <span class="li-normal">required: False</span> </li>
                
            </ul>
        
        </li>
        license_status
        <li><span class="li-head">license_status</span> 
        
        </li>
        log_av-archive_download
        <li><span class="li-head">log_av-archive_download</span> - Download file quarantined by AntiVirus. 
        <ul class="ul-self">
                <li><span class="li-required">mkey</span> - Checksum for quarantined file. <span class="li-normal">type: string</span> <span class="li-normal">required: True</span> </li>
                
            </ul>
        
        </li>
        log_current-disk-usage
        <li><span class="li-head">log_current-disk-usage</span> 
        
        </li>
        log_device_state
        <li><span class="li-head">log_device_state</span> 
        
        </li>
        log_event
        <li><span class="li-head">log_event</span> 
        
        </li>
        log_fortianalyzer
        <li><span class="li-head">log_fortianalyzer</span> - Return FortiAnalyzer/FortiManager log status. 
        <ul class="ul-self">
                <li><span class="li-required">srcip</span> - The IP to use to make the request to the FortiAnalyzer [<ip>|auto]. When set to "auto" it will use the FortiGate's routing table to determine the IP to make the request from. <span class="li-normal">type: string</span> <span class="li-normal">required: False</span> </li>
                <li><span class="li-required">scope</span> - Scope from which to test the connectivity of the FortiAnalyzer address [vdom|global]. <span class="li-normal">type: string</span> <span class="li-normal">required: False</span> </li>
                <li><span class="li-required">server</span> - FortiAnalyzer/FortiManager address. <span class="li-normal">type: string</span> <span class="li-normal">required: False</span> </li>
                
            </ul>
        
        </li>
        log_fortianalyzer-queue
        <li><span class="li-head">log_fortianalyzer-queue</span> - Retrieve information on FortiAnalyzer's queue state. Note:- FortiAnalyzer logs are queued only if upload-option is realtime. 
        <ul class="ul-self">
                <li><span class="li-required">scope</span> - Scope from which to retrieve FortiAnalyzer's queue state [vdom*|global]. <span class="li-normal">type: string</span> <span class="li-normal">required: False</span> </li>
                
            </ul>
        
        </li>
        log_forticloud
        <li><span class="li-head">log_forticloud</span> 
        
        </li>
        log_forticloud-report-list
        <li><span class="li-head">log_forticloud-report-list</span> 
        
        </li>
        log_forticloud-report_download
        <li><span class="li-head">log_forticloud-report_download</span> - Download PDF report from FortiCloud. 
        <ul class="ul-self">
                <li><span class="li-required">inline</span> - Set to 1 to download the report inline. <span class="li-normal">type: int</span> <span class="li-normal">required: False</span> </li>
                <li><span class="li-required">mkey</span> - FortiCloud Report ID. <span class="li-normal">type: int</span> <span class="li-normal">required: True</span> </li>
                
            </ul>
        
        </li>
        log_historic-daily-remote-logs
        <li><span class="li-head">log_historic-daily-remote-logs</span> - Returns the amount of logs in bytes sent daily to a remote logging service (FortiCloud or FortiAnalyzer). 
        <ul class="ul-self">
                <li><span class="li-required">server</span> - Service name [forticloud | fortianalyzer]. <span class="li-normal">type: string</span> <span class="li-normal">required: True</span> </li>
                
            </ul>
        
        </li>
        log_hourly-disk-usage
        <li><span class="li-head">log_hourly-disk-usage</span> 
        
        </li>
        log_ips-archive_download
        <li><span class="li-head">log_ips-archive_download</span> - Download IPS/application control packet capture files. Uses configured log display device. 
        <ul class="ul-self">
                <li><span class="li-required">pcap_no</span> - Packet capture roll number (required when log device is 'disk') <span class="li-normal">type: int</span> <span class="li-normal">required: False</span> </li>
                <li><span class="li-required">pcap_category</span> - Packet capture category (required when log device is 'disk') <span class="li-normal">type: int</span> <span class="li-normal">required: False</span> </li>
                <li><span class="li-required">mkey</span> - IPS archive ID. <span class="li-normal">type: int</span> <span class="li-normal">required: True</span> </li>
                
            </ul>
        
        </li>
        log_local-report-list
        <li><span class="li-head">log_local-report-list</span> 
        
        </li>
        log_local-report_download
        <li><span class="li-head">log_local-report_download</span> - Download local report 
        <ul class="ul-self">
                <li><span class="li-required">mkey</span> - Local Report Name. <span class="li-normal">type: string</span> <span class="li-normal">required: True</span> </li>
                
            </ul>
        
        </li>
        log_policy-archive_download
        <li><span class="li-head">log_policy-archive_download</span> - Download policy-based packet capture archive. 
        <ul class="ul-self">
                <li><span class="li-required">srcip</span> - Source IP. <span class="li-normal">type: string</span> <span class="li-normal">required: True</span> </li>
                <li><span class="li-required">dstip</span> - Destination IP. <span class="li-normal">type: string</span> <span class="li-normal">required: True</span> </li>
                <li><span class="li-required">mkey</span> - Session ID (from traffic log). <span class="li-normal">type: int</span> <span class="li-normal">required: True</span> </li>
                
            </ul>
        
        </li>
        log_stats
        <li><span class="li-head">log_stats</span> - Return number of logs sent by category per day for a specific log device. 
        <ul class="ul-self">
                <li><span class="li-required">dev</span> - Log device [*memory | disk | fortianalyzer | forticloud]. <span class="li-normal">type: string</span> <span class="li-normal">required: False</span> </li>
                
            </ul>
        
        </li>
        network_arp
        <li><span class="li-head">network_arp</span> 
        
        </li>
        network_ddns_lookup
        <li><span class="li-head">network_ddns_lookup</span> - Check DDNS FQDN availability. 
        <ul class="ul-self">
                <li><span class="li-required">domain</span> - Filter: domain to check. <span class="li-normal">type: string</span> <span class="li-normal">required: True</span> </li>
                
            </ul>
        
        </li>
        network_ddns_servers
        <li><span class="li-head">network_ddns_servers</span> 
        
        </li>
        network_dns_latency
        <li><span class="li-head">network_dns_latency</span> 
        
        </li>
        network_fortiguard_live-services-latency
        <li><span class="li-head">network_fortiguard_live-services-latency</span> 
        
        </li>
        network_lldp_neighbors
        <li><span class="li-head">network_lldp_neighbors</span> 
        
        </li>
        network_lldp_ports
        <li><span class="li-head">network_lldp_ports</span> - List all active LLDP ports. 
        <ul class="ul-self">
                <li><span class="li-required">mkey</span> - Filter: specific port name. <span class="li-normal">type: string</span> <span class="li-normal">required: False</span> </li>
                
            </ul>
        
        </li>
        network_reverse-ip-lookup
        <li><span class="li-head">network_reverse-ip-lookup</span> - Retrieve the resolved DNS domain name for a given IP address. 
        <ul class="ul-self">
                <li><span class="li-required">ip</span> - IP address (in dot-decimal notation). <span class="li-normal">type: string</span> <span class="li-normal">required: True</span> </li>
                
            </ul>
        
        </li>
        nsx_instance
        <li><span class="li-head">nsx_instance</span> - List NSX instances and their resource statistics. 
        <ul class="ul-self">
                <li><span class="li-required">mkey</span> - Filter: NSX SDN name. <span class="li-normal">type: string</span> <span class="li-normal">required: False</span> </li>
                
            </ul>
        
        </li>
        nsx_service_status
        <li><span class="li-head">nsx_service_status</span> - Retrieve NSX service status. 
        <ul class="ul-self">
                <li><span class="li-required">mkey</span> - Filter: NSX SDN name. <span class="li-normal">type: string</span> <span class="li-normal">required: False</span> </li>
                
            </ul>
        
        </li>
        registration_forticloud_device-status
        <li><span class="li-head">registration_forticloud_device-status</span> - Fetch device registration status from FortiCloud. Currently FortiSwitch and FortiAP are supported. 
        <ul class="ul-self">
                <li><span class="li-required">serials</span> - Serials of FortiSwitch and FortiAP to fetch registration status. <span class="li-normal">type: array</span> <span class="li-normal">required: True</span> </li>
                <li><span class="li-required">update_cache</span> - Clear cache and retrieve updated data. <span class="li-normal">type: boolean</span> <span class="li-normal">required: False</span> </li>
                
            </ul>
        
        </li>
        registration_forticloud_disclaimer
        <li><span class="li-head">registration_forticloud_disclaimer</span> 
        
        </li>
        registration_forticloud_domains
        <li><span class="li-head">registration_forticloud_domains</span> 
        
        </li>
        router_bgp_neighbors
        <li><span class="li-head">router_bgp_neighbors</span> 
        
        </li>
        router_bgp_neighbors6
        <li><span class="li-head">router_bgp_neighbors6</span> 
        
        </li>
        router_bgp_paths
        <li><span class="li-head">router_bgp_paths</span> - List all discovered BGP paths. 
        <ul class="ul-self">
                <li><span class="li-required">count</span> - Maximum number of entries to return (Default behavior will return all BGP Paths). <span class="li-normal">type: int</span> <span class="li-normal">required: False</span> </li>
                <li><span class="li-required">start</span> - Starting entry index. <span class="li-normal">type: int</span> <span class="li-normal">required: False</span> </li>
                
            </ul>
        
        </li>
        router_bgp_paths-statistics
        <li><span class="li-head">router_bgp_paths-statistics</span> - Retrieve BGP paths statistics, including number of IPv4 or IPv6 BGP paths. 
        <ul class="ul-self">
                <li><span class="li-required">ip_version</span> - IP version [*ipv4 | ipv6 | ipboth]. <span class="li-normal">type: string</span> <span class="li-normal">required: False</span> </li>
                
            </ul>
        
        </li>
        router_bgp_paths6
        <li><span class="li-head">router_bgp_paths6</span> - List all discovered IPv6 BGP paths. 
        <ul class="ul-self">
                <li><span class="li-required">count</span> - Maximum number of entries to return (Default behavior will return all BGP Paths). <span class="li-normal">type: int</span> <span class="li-normal">required: False</span> </li>
                <li><span class="li-required">start</span> - Starting entry index. <span class="li-normal">type: int</span> <span class="li-normal">required: False</span> </li>
                
            </ul>
        
        </li>
        router_ipv4
        <li><span class="li-head">router_ipv4</span> - List all active IPv4 routing table entries. 
        <ul class="ul-self">
                <li><span class="li-required">count</span> - Maximum number of entries to return (Default for all routes). <span class="li-normal">type: int</span> <span class="li-normal">required: False</span> </li>
                <li><span class="li-required">ip_mask</span> - Filter: IP/netmask. <span class="li-normal">type: string</span> <span class="li-normal">required: False</span> </li>
                <li><span class="li-required">start</span> - Starting entry index. <span class="li-normal">type: int</span> <span class="li-normal">required: False</span> </li>
                <li><span class="li-required">interface</span> - Filter: interface name. <span class="li-normal">type: string</span> <span class="li-normal">required: False</span> </li>
                <li><span class="li-required">type</span> - Filter: route type. <span class="li-normal">type: string</span> <span class="li-normal">required: False</span> </li>
                <li><span class="li-required">gateway</span> - Filter: gateway. <span class="li-normal">type: string</span> <span class="li-normal">required: False</span> </li>
                
            </ul>
        
        </li>
        router_ipv6
        <li><span class="li-head">router_ipv6</span> - List all active IPv6 routing table entries. 
        <ul class="ul-self">
                <li><span class="li-required">count</span> - Maximum number of entries to return (Default for all routes). <span class="li-normal">type: int</span> <span class="li-normal">required: False</span> </li>
                <li><span class="li-required">ip_mask</span> - Filter: IP/netmask. <span class="li-normal">type: string</span> <span class="li-normal">required: False</span> </li>
                <li><span class="li-required">start</span> - Starting entry index. <span class="li-normal">type: int</span> <span class="li-normal">required: False</span> </li>
                <li><span class="li-required">interface</span> - Filter: interface name. <span class="li-normal">type: string</span> <span class="li-normal">required: False</span> </li>
                <li><span class="li-required">type</span> - Filter: route type. <span class="li-normal">type: string</span> <span class="li-normal">required: False</span> </li>
                <li><span class="li-required">gateway</span> - Filter: gateway. <span class="li-normal">type: string</span> <span class="li-normal">required: False</span> </li>
                
            </ul>
        
        </li>
        router_lookup
        <li><span class="li-head">router_lookup</span> - Performs a route lookup by querying the routing table. 
        <ul class="ul-self">
                <li><span class="li-required">destination</span> - Destination IP/FQDN. <span class="li-normal">type: string</span> <span class="li-normal">required: True</span> </li>
                <li><span class="li-required">ipv6</span> - Perform an IPv6 lookup. <span class="li-normal">type: boolean</span> <span class="li-normal">required: False</span> </li>
                
            </ul>
        
        </li>
        router_lookup-policy
        <li><span class="li-head">router_lookup-policy</span> - Performs a route lookup by querying the policy routing table. 
        <ul class="ul-self">
                <li><span class="li-required">protocol_number</span> - IP Protocol Number. <span class="li-normal">type: int</span> <span class="li-normal">required: False</span> </li>
                <li><span class="li-required">destination</span> - Destination IP/FQDN. <span class="li-normal">type: string</span> <span class="li-normal">required: True</span> </li>
                <li><span class="li-required">source</span> - Source IP/FQDN. <span class="li-normal">type: string</span> <span class="li-normal">required: False</span> </li>
                <li><span class="li-required">ipv6</span> - Perform an IPv6 lookup. <span class="li-normal">type: boolean</span> <span class="li-normal">required: False</span> </li>
                <li><span class="li-required">destination_port</span> - Destination Port. <span class="li-normal">type: int</span> <span class="li-normal">required: False</span> </li>
                <li><span class="li-required">interface_name</span> - Incoming Interface. <span class="li-normal">type: string</span> <span class="li-normal">required: False</span> </li>
                
            </ul>
        
        </li>
        router_ospf_neighbors
        <li><span class="li-head">router_ospf_neighbors</span> 
        
        </li>
        router_policy
        <li><span class="li-head">router_policy</span> - Retrieve a list of active IPv4 policy routes. 
        <ul class="ul-self">
                <li><span class="li-required">count</span> - Maximum number of entries to return. <span class="li-normal">type: int</span> <span class="li-normal">required: False</span> </li>
                <li><span class="li-required">start</span> - Starting entry index. <span class="li-normal">type: int</span> <span class="li-normal">required: False</span> </li>
                <li><span class="li-required">count_only</span> - Returns the number of IPv4 policy routes only. <span class="li-normal">type: boolean</span> <span class="li-normal">required: False</span> </li>
                
            </ul>
        
        </li>
        router_policy6
        <li><span class="li-head">router_policy6</span> - Retrieve a list of active IPv6 policy routes. 
        <ul class="ul-self">
                <li><span class="li-required">count</span> - Maximum number of entries to return. <span class="li-normal">type: int</span> <span class="li-normal">required: False</span> </li>
                <li><span class="li-required">start</span> - Starting entry index. <span class="li-normal">type: int</span> <span class="li-normal">required: False</span> </li>
                <li><span class="li-required">count_only</span> - Returns the number of IPv6 policy routes only. <span class="li-normal">type: boolean</span> <span class="li-normal">required: False</span> </li>
                
            </ul>
        
        </li>
        router_statistics
        <li><span class="li-head">router_statistics</span> - Retrieve routing table statistics, including number of matched routes. 
        <ul class="ul-self">
                <li><span class="li-required">ip_version</span> - IP version (4|6). If not present, IPv4 and IPv6 will be returned. <span class="li-normal">type: int</span> <span class="li-normal">required: False</span> </li>
                <li><span class="li-required">ip_mask</span> - Filter: IP/netmask. <span class="li-normal">type: string</span> <span class="li-normal">required: False</span> </li>
                <li><span class="li-required">interface</span> - Filter: interface name. <span class="li-normal">type: string</span> <span class="li-normal">required: False</span> </li>
                <li><span class="li-required">type</span> - Filter: route type. <span class="li-normal">type: string</span> <span class="li-normal">required: False</span> </li>
                <li><span class="li-required">gateway</span> - Filter: gateway. <span class="li-normal">type: string</span> <span class="li-normal">required: False</span> </li>
                
            </ul>
        
        </li>
        switch-controller_detected-device
        <li><span class="li-head">switch-controller_detected-device</span> 
        
        </li>
        switch-controller_fsw-firmware
        <li><span class="li-head">switch-controller_fsw-firmware</span> - Retrieve a list of recommended firmware for managed FortiSwitches. 
        <ul class="ul-self">
                <li><span class="li-required">timeout</span> - FortiGuard connection timeout (defaults to 3 seconds). <span class="li-normal">type: string</span> <span class="li-normal">required: False</span> </li>
                <li><span class="li-required">mkey</span> - Filter: FortiSwitch ID. <span class="li-normal">type: string</span> <span class="li-normal">required: False</span> </li>
                
            </ul>
        
        </li>
        switch-controller_managed-switch
        <li><span class="li-head">switch-controller_managed-switch</span> - Retrieve statistics for configured FortiSwitches. Deprecated. It will be removed in 7.2.       It's replaced by /api/v2/monitor/switch-controller/managed-switch/status for faster performance. 
        <ul class="ul-self">
                <li><span class="li-required">port_stats</span> - Filter: Retrieve tx/rx statistics for ports of configured FortiSwitches. <span class="li-normal">type: boolean</span> <span class="li-normal">required: False</span> </li>
                <li><span class="li-required">stp_status</span> - Filter: Retrieve STP status for ports of configured FortiSwitches. <span class="li-normal">type: boolean</span> <span class="li-normal">required: False</span> </li>
                <li><span class="li-required">igmp_snooping_group</span> - Filter: Retrieve IGMP Snooping group for configured FortiSwitches. <span class="li-normal">type: boolean</span> <span class="li-normal">required: False</span> </li>
                <li><span class="li-required">qos_stats</span> - Filter: Retrieve QoS statistics for ports of configured FortiSwitches. <span class="li-normal">type: boolean</span> <span class="li-normal">required: False</span> </li>
                <li><span class="li-required">transceiver</span> - Filter: Retrieve transceiver information for ports of configured FortiSwitches. <span class="li-normal">type: boolean</span> <span class="li-normal">required: False</span> </li>
                <li><span class="li-required">poe</span> - Filter: Retrieve PoE statistics for ports of configured FortiSwitches. Port power usage is in Watt units. <span class="li-normal">type: boolean</span> <span class="li-normal">required: False</span> </li>
                <li><span class="li-required">mkey</span> - Filter: FortiSwitch ID. <span class="li-normal">type: string</span> <span class="li-normal">required: False</span> </li>
                
            </ul>
        
        </li>
        switch-controller_managed-switch_cable-status
        <li><span class="li-head">switch-controller_managed-switch_cable-status</span> - Diagnose cable information for a port. Virtual FortiSwitches and FortiLink ports are not supported. 
        <ul class="ul-self">
                <li><span class="li-required">port</span> - Name of managed FortiSwitch port. <span class="li-normal">type: string</span> <span class="li-normal">required: True</span> </li>
                <li><span class="li-required">mkey</span> - Name of managed FortiSwitch. <span class="li-normal">type: string</span> <span class="li-normal">required: True</span> </li>
                
            </ul>
        
        </li>
        switch-controller_managed-switch_dhcp-snooping
        <li><span class="li-head">switch-controller_managed-switch_dhcp-snooping</span> 
        
        </li>
        switch-controller_managed-switch_faceplate-xml
        <li><span class="li-head">switch-controller_managed-switch_faceplate-xml</span> - Retrieve XML for rendering FortiSwitch faceplate widget. 
        <ul class="ul-self">
                <li><span class="li-required">mkey</span> - Name of managed FortiSwitch. <span class="li-normal">type: string</span> <span class="li-normal">required: True</span> </li>
                
            </ul>
        
        </li>
        switch-controller_managed-switch_health
        <li><span class="li-head">switch-controller_managed-switch_health</span> - Retrieve health-check statistics for managed FortiSwitches. 
        <ul class="ul-self">
                <li><span class="li-required">mkey</span> - Filter: FortiSwitch ID. <span class="li-normal">type: string</span> <span class="li-normal">required: False</span> </li>
                
            </ul>
        
        </li>
        switch-controller_managed-switch_models
        <li><span class="li-head">switch-controller_managed-switch_models</span> 
        
        </li>
        switch-controller_managed-switch_port-stats
        <li><span class="li-head">switch-controller_managed-switch_port-stats</span> - Retrieve port statistics for configured FortiSwitches. 
        <ul class="ul-self">
                <li><span class="li-required">mkey</span> - Filter: FortiSwitch ID. <span class="li-normal">type: string</span> <span class="li-normal">required: False</span> </li>
                
            </ul>
        
        </li>
        switch-controller_managed-switch_status
        <li><span class="li-head">switch-controller_managed-switch_status</span> - Retrieve statistics for configured FortiSwitches. 
        <ul class="ul-self">
                <li><span class="li-required">mkey</span> - Filter: FortiSwitch ID. <span class="li-normal">type: string</span> <span class="li-normal">required: False</span> </li>
                
            </ul>
        
        </li>
        switch-controller_managed-switch_transceivers
        <li><span class="li-head">switch-controller_managed-switch_transceivers</span> 
        
        </li>
        switch-controller_matched-devices
        <li><span class="li-head">switch-controller_matched-devices</span> - Return a list of devices that match NAC and/or dynamic port policies. 
        <ul class="ul-self">
                <li><span class="li-required">include_dynamic</span> - If true, include devices that match dynamic port policies. Default value is false. <span class="li-normal">type: boolean</span> <span class="li-normal">required: False</span> </li>
                <li><span class="li-required">mkey</span> - FortiSwitch ID. Will return all devices if no ID is provided. <span class="li-normal">type: string</span> <span class="li-normal">required: False</span> </li>
                
            </ul>
        
        </li>
        switch-controller_mclag-icl_eligible-peer
        <li><span class="li-head">switch-controller_mclag-icl_eligible-peer</span> - Find a pair of FortiSwitches that are eligible to form a tier-1 MCLAG. 
        <ul class="ul-self">
                <li><span class="li-required">fortilink</span> - FortiLink interface name. <span class="li-normal">type: string</span> <span class="li-normal">required: True</span> </li>
                
            </ul>
        
        </li>
        switch-controller_validate-switch-prefix
        <li><span class="li-head">switch-controller_validate-switch-prefix</span> - Validate a FortiSwitch serial number prefix. Deprecated in 7.2 replaced by /api/v2/monitor/switch-controller/managed-switch/preprovision. 
        <ul class="ul-self">
                <li><span class="li-required">prefix</span> - Prefix of FortiSwitch serial number. <span class="li-normal">type: string</span> <span class="li-normal">required: False</span> </li>
                
            </ul>
        
        </li>
        system_3g-modem
        <li><span class="li-head">system_3g-modem</span> 
        
        </li>
        system_acquired-dns
        <li><span class="li-head">system_acquired-dns</span> 
        
        </li>
        system_automation-action_stats
        <li><span class="li-head">system_automation-action_stats</span> - Statistics for automation actions. 
        <ul class="ul-self">
                <li><span class="li-required">mkey</span> - Filter: Automation action name. <span class="li-normal">type: string</span> <span class="li-normal">required: False</span> </li>
                
            </ul>
        
        </li>
        system_automation-stitch_stats
        <li><span class="li-head">system_automation-stitch_stats</span> - Statistics for automation stitches. 
        <ul class="ul-self">
                <li><span class="li-required">mkey</span> - Filter: Automation stitch name. <span class="li-normal">type: string</span> <span class="li-normal">required: False</span> </li>
                
            </ul>
        
        </li>
        system_available-certificates
        <li><span class="li-head">system_available-certificates</span> - Get available certificates. 
        <ul class="ul-self">
                <li><span class="li-required">scope</span> - Scope of certificate [vdom*|global]. <span class="li-normal">type: string</span> <span class="li-normal">required: False</span> </li>
                <li><span class="li-required">with_remote</span> - Include remote certificates. <span class="li-normal">type: boolean</span> <span class="li-normal">required: False</span> </li>
                <li><span class="li-required">with_ca</span> - Include certificate authorities. <span class="li-normal">type: boolean</span> <span class="li-normal">required: False</span> </li>
                <li><span class="li-required">find_all_references</span> - Include reference counts across all VDOMs when scope is global. <span class="li-normal">type: boolean</span> <span class="li-normal">required: False</span> </li>
                <li><span class="li-required">with_crl</span> - Include certificate revocation lists. <span class="li-normal">type: boolean</span> <span class="li-normal">required: False</span> </li>
                
            </ul>
        
        </li>
        system_available-interfaces
        <li><span class="li-head">system_available-interfaces</span> - Retrieve a list of all interfaces along with some meta information regarding their availability. 
        <ul class="ul-self">
                <li><span class="li-required">scope</span> - Scope of interface list [vdom|global] <span class="li-normal">type: string</span> <span class="li-normal">required: False</span> </li>
                <li><span class="li-required">view_type</span> - Optionally include additional information for interfaces. This parameter can be repeated multiple times. 'ha': Includes extra meta information useful when dealing with interfaces related to HA configuration. Interfaces that are used by an HA cluster as management interfaces are also included in this view. 'zone': Includes extra meta information for determining zone membership eligibility. 'vwp': Includes extra meta information for determining virtual wire pair eligibility. 'sdwan': Includes extra meta information for determining SD-WAN eligibility. 'switch': Includes extra meta information for determining switch eligibility. 'hard-switch': Includes extra meta information for determining hard-switch eligibility. 'limited': Includes limited information on parent interfaces that are in another VDOM. 'stat': Includes TX/RX statistics data.  <span class="li-normal">type: string</span> <span class="li-normal">required: False</span> </li>
                
            </ul>
        
        </li>
        system_botnet
        <li><span class="li-head">system_botnet</span> - List all known IP-based botnet entries in FortiGuard botnet database. 
        <ul class="ul-self">
                <li><span class="li-required">count</span> - Maximum number of entries to return. <span class="li-normal">type: int</span> <span class="li-normal">required: False</span> </li>
                <li><span class="li-required">start</span> - Starting entry index. <span class="li-normal">type: int</span> <span class="li-normal">required: False</span> </li>
                <li><span class="li-required">include_hit_only</span> - Include entries with hits only. <span class="li-normal">type: boolean</span> <span class="li-normal">required: False</span> </li>
                
            </ul>
        
        </li>
        system_botnet-domains
        <li><span class="li-head">system_botnet-domains</span> - List all known domain-based botnet entries in FortiGuard botnet database. 
        <ul class="ul-self">
                <li><span class="li-required">count</span> - Maximum number of entries to return. <span class="li-normal">type: int</span> <span class="li-normal">required: False</span> </li>
                <li><span class="li-required">start</span> - Starting entry index. <span class="li-normal">type: int</span> <span class="li-normal">required: False</span> </li>
                
            </ul>
        
        </li>
        system_botnet-domains_hits
        <li><span class="li-head">system_botnet-domains_hits</span> 
        
        </li>
        system_botnet-domains_stat
        <li><span class="li-head">system_botnet-domains_stat</span> 
        
        </li>
        system_botnet_stat
        <li><span class="li-head">system_botnet_stat</span> 
        
        </li>
        system_certificate_download
        <li><span class="li-head">system_certificate_download</span> - Download certificate. 
        <ul class="ul-self">
                <li><span class="li-required">scope</span> - Scope of certificate [vdom*|global]. <span class="li-normal">type: string</span> <span class="li-normal">required: False</span> </li>
                <li><span class="li-required">type</span> - Type of certificate [local-cer|remote-cer|local-ca|remote-ca|local-csr|crl]. <span class="li-normal">type: string</span> <span class="li-normal">required: True</span> </li>
                <li><span class="li-required">mkey</span> - Name of certificate. <span class="li-normal">type: string</span> <span class="li-normal">required: True</span> </li>
                
            </ul>
        
        </li>
        system_check-port-availability
        <li><span class="li-head">system_check-port-availability</span> - Check whether a list of TCP port ranges is available for a certain service. 
        <ul class="ul-self">
                <li><span class="li-required">port_ranges</span> - List of TCP port range objects to check against. <span class="li-normal">type: array</span> <span class="li-normal">required: True</span> </li>
                <li><span class="li-required">service</span> - The service in which the ports could be available. 'service' options are [reserved | sysglobal | webproxy | ftpproxy | sslvpn | slaprobe | fsso | ftm_push]. If 'service' is not specified, the port ranges availability is checked against all services. <span class="li-normal">type: string</span> <span class="li-normal">required: False</span> </li>
                
            </ul>
        
        </li>
        system_com-log_download
        <li><span class="li-head">system_com-log_download</span> 
        
        </li>
        system_com-log_update
        <li><span class="li-head">system_com-log_update</span> 
        
        </li>
        system_config-error-log_download
        <li><span class="li-head">system_config-error-log_download</span> 
        
        </li>
        system_config-revision
        <li><span class="li-head">system_config-revision</span> 
        
        </li>
        system_config-revision_file
        <li><span class="li-head">system_config-revision_file</span> - Download a specific configuration revision. 
        <ul class="ul-self">
                <li><span class="li-required">config_id</span> - Configuration id. <span class="li-normal">type: int</span> <span class="li-normal">required: False</span> </li>
                
            </ul>
        
        </li>
        system_config-revision_info
        <li><span class="li-head">system_config-revision_info</span> - Retrieve meta information for a specific configuration revision. 
        <ul class="ul-self">
                <li><span class="li-required">config_id</span> - Configuration id. <span class="li-normal">type: int</span> <span class="li-normal">required: False</span> </li>
                
            </ul>
        
        </li>
        system_config-script
        <li><span class="li-head">system_config-script</span> 
        
        </li>
        system_config-sync_status
        <li><span class="li-head">system_config-sync_status</span> 
        
        </li>
        system_config_backup
        <li><span class="li-head">system_config_backup</span> - Backup system config 
        <ul class="ul-self">
                <li><span class="li-required">password</span> - Password to encrypt configuration data. <span class="li-normal">type: string</span> <span class="li-normal">required: False</span> </li>
                <li><span class="li-required">usb_filename</span> - When using 'usb' destination: the filename to save to on the connected USB device <span class="li-normal">type: string</span> <span class="li-normal">required: False</span> </li>
                <li><span class="li-required">destination</span> - Configuration file destination [file* | usb] <span class="li-normal">type: string</span> <span class="li-normal">required: False</span> </li>
                <li><span class="li-required">vdom</span> - If 'vdom' scope specified, the name of the VDOM to backup configuration. <span class="li-normal">type: string</span> <span class="li-normal">required: False</span> </li>
                <li><span class="li-required">scope</span> - Specify global or VDOM only backup [global | vdom]. <span class="li-normal">type: string</span> <span class="li-normal">required: True</span> </li>
                
            </ul>
        
        </li>
        system_config_restore-status
        <li><span class="li-head">system_config_restore-status</span> - Check the status of the restoring system configuration session. 
        <ul class="ul-self">
                <li><span class="li-required">session_id</span> - Session ID for restoring configuration. <span class="li-normal">type: string</span> <span class="li-normal">required: True</span> </li>
                
            </ul>
        
        </li>
        system_config_usb-filelist
        <li><span class="li-head">system_config_usb-filelist</span> 
        
        </li>
        system_csf
        <li><span class="li-head">system_csf</span> - Retrieve a full tree of downstream FortiGates registered to the Security Fabric. 
        <ul class="ul-self">
                <li><span class="li-required">scope</span> - Scope from which to retrieve the Security Fabric tree [vdom*|global]. <span class="li-normal">type: string</span> <span class="li-normal">required: False</span> </li>
                
            </ul>
        
        </li>
        system_csf_pending-authorizations
        <li><span class="li-head">system_csf_pending-authorizations</span> 
        
        </li>
        system_current-admins
        <li><span class="li-head">system_current-admins</span> 
        
        </li>
        system_debug_download
        <li><span class="li-head">system_debug_download</span> 
        
        </li>
        system_dhcp
        <li><span class="li-head">system_dhcp</span> - List all DHCP and DHCPv6 leases. 
        <ul class="ul-self">
                <li><span class="li-required">interface</span> - Filter: Retrieve DHCP leases for this interface only. <span class="li-normal">type: string</span> <span class="li-normal">required: False</span> </li>
                <li><span class="li-required">scope</span> - Scope from which to retrieve DHCP leases [vdom*|global]. Global scope is only accessible for global administrators. <span class="li-normal">type: string</span> <span class="li-normal">required: False</span> </li>
                <li><span class="li-required">ipv6</span> - Include IPv6 addresses in the response. <span class="li-normal">type: boolean</span> <span class="li-normal">required: False</span> </li>
                
            </ul>
        
        </li>
        system_external-resource_entry-list
        <li><span class="li-head">system_external-resource_entry-list</span> - Retrieve resource file status with a list of valid/invalid entries for the specific external resource. Empty lines and comment lines are not returned. 
        <ul class="ul-self">
                <li><span class="li-required">status_only</span> - Set to true to retrieve resource file status only. (Skip valid/invalid entries.) <span class="li-normal">type: boolean</span> <span class="li-normal">required: False</span> </li>
                <li><span class="li-required">mkey</span> - The external resource name to query. <span class="li-normal">type: string</span> <span class="li-normal">required: True</span> </li>
                <li><span class="li-required">include_notes</span> - Set to true to retrieve notes on the resource file. <span class="li-normal">type: boolean</span> <span class="li-normal">required: False</span> </li>
                
            </ul>
        
        </li>
        system_firmware
        <li><span class="li-head">system_firmware</span> 
        
        </li>
        system_firmware_upgrade-paths
        <li><span class="li-head">system_firmware_upgrade-paths</span> 
        
        </li>
        system_fortiguard-blacklist
        <li><span class="li-head">system_fortiguard-blacklist</span> - Retrieve blacklist information for a specified IP. 
        <ul class="ul-self">
                <li><span class="li-required">ip</span> - IPv4 address to check against. <span class="li-normal">type: string</span> <span class="li-normal">required: True</span> </li>
                <li><span class="li-required">timeout</span> - Timeout period in seconds (defaults to 5). <span class="li-normal">type: int</span> <span class="li-normal">required: False</span> </li>
                
            </ul>
        
        </li>
        system_fortiguard_server-info
        <li><span class="li-head">system_fortiguard_server-info</span> 
        
        </li>
        system_fortimanager_backup-details
        <li><span class="li-head">system_fortimanager_backup-details</span> - Get the properties of a FortiManager object. 
        <ul class="ul-self">
                <li><span class="li-required">datasource</span> - Object datasource. <span class="li-normal">type: string</span> <span class="li-normal">required: True</span> </li>
                <li><span class="li-required">mkey</span> - Object name. <span class="li-normal">type: string</span> <span class="li-normal">required: True</span> </li>
                
            </ul>
        
        </li>
        system_fortimanager_backup-summary
        <li><span class="li-head">system_fortimanager_backup-summary</span> 
        
        </li>
        system_fortimanager_status
        <li><span class="li-head">system_fortimanager_status</span> 
        
        </li>
        system_global-resources
        <li><span class="li-head">system_global-resources</span> 
        
        </li>
        system_global-search
        <li><span class="li-head">system_global-search</span> - Search for CMDB table objects based on search phrase. 
        <ul class="ul-self">
                <li><span class="li-required">scope</span> - Search scope [vdom|global]. <span class="li-normal">type: string</span> <span class="li-normal">required: False</span> </li>
                <li><span class="li-required">search</span> - Phrase used for searching. <span class="li-normal">type: string</span> <span class="li-normal">required: True</span> </li>
                <li><span class="li-required">skip_tables</span> - Array of CMDB tables to be skipped when doing global search. E.g. ['firewall.address', 'firewall.address6']. <span class="li-normal">type: array</span> <span class="li-normal">required: False</span> </li>
                <li><span class="li-required">search_tables</span> - Array of CMDB tables to search on. If not defined, global search function will do a search on all tables that the current user has read permission on. E.g ['firewall.address', 'firewall.address6']. <span class="li-normal">type: array</span> <span class="li-normal">required: False</span> </li>
                
            </ul>
        
        </li>
        system_ha-checksums
        <li><span class="li-head">system_ha-checksums</span> 
        
        </li>
        system_ha-history
        <li><span class="li-head">system_ha-history</span> 
        
        </li>
        system_ha-peer
        <li><span class="li-head">system_ha-peer</span> - Get configuration of peer(s) in HA cluster. Uptime is expressed in seconds. 
        <ul class="ul-self">
                <li><span class="li-required">serial_no</span> - Serial number of the HA member. If not specified, fetch information for all HA members <span class="li-normal">type: string</span> <span class="li-normal">required: False</span> </li>
                <li><span class="li-required">vcluster_id</span> - Virtual cluster number. If not specified, fetch information for all active vclusters <span class="li-normal">type: int</span> <span class="li-normal">required: False</span> </li>
                
            </ul>
        
        </li>
        system_ha-statistics
        <li><span class="li-head">system_ha-statistics</span> 
        
        </li>
        system_ha-table-checksums
        <li><span class="li-head">system_ha-table-checksums</span> - List of table checksums for members of HA cluster. 
        <ul class="ul-self">
                <li><span class="li-required">vdom_name</span> - VDOM name of the HA member. If not specified, fetch table checksums for global. <span class="li-normal">type: string</span> <span class="li-normal">required: False</span> </li>
                <li><span class="li-required">serial_no</span> - Serial number of the HA member. <span class="li-normal">type: string</span> <span class="li-normal">required: True</span> </li>
                
            </ul>
        
        </li>
        system_interface
        <li><span class="li-head">system_interface</span> - Retrieve statistics for all system interfaces. 
        <ul class="ul-self">
                <li><span class="li-required">scope</span> - Scope from which to retrieve the interface stats from [vdom|global]. <span class="li-normal">type: string</span> <span class="li-normal">required: False</span> </li>
                <li><span class="li-required">interface_name</span> - Filter: interface name. <span class="li-normal">type: string</span> <span class="li-normal">required: False</span> </li>
                <li><span class="li-required">include_vlan</span> - Enable to include VLANs in result list. <span class="li-normal">type: boolean</span> <span class="li-normal">required: False</span> </li>
                <li><span class="li-required">include_aggregate</span> - Enable to include Aggregate interfaces in result list. <span class="li-normal">type: boolean</span> <span class="li-normal">required: False</span> </li>
                
            </ul>
        
        </li>
        system_interface-connected-admins-info
        <li><span class="li-head">system_interface-connected-admins-info</span> - Return admins info that are connected to current interface. 
        <ul class="ul-self">
                <li><span class="li-required">interface</span> - Interface that admins is connected through. <span class="li-normal">type: string</span> <span class="li-normal">required: True</span> </li>
                
            </ul>
        
        </li>
        system_interface_dhcp-status
        <li><span class="li-head">system_interface_dhcp-status</span> - Retrieve the DHCP client status of an interface. 
        <ul class="ul-self">
                <li><span class="li-required">mkey</span> - Name of the interface. <span class="li-normal">type: string</span> <span class="li-normal">required: True</span> </li>
                <li><span class="li-required">ipv6</span> - Retrieve the DHCPv6 client status. <span class="li-normal">type: boolean</span> <span class="li-normal">required: False</span> </li>
                
            </ul>
        
        </li>
        system_interface_kernel-interfaces
        <li><span class="li-head">system_interface_kernel-interfaces</span> 
        
        </li>
        system_interface_poe
        <li><span class="li-head">system_interface_poe</span> - Retrieve PoE statistics for system interfaces. 
        <ul class="ul-self">
                <li><span class="li-required">scope</span> - Scope from which to retrieve the interface stats from [vdom|global] (default=vdom). <span class="li-normal">type: string</span> <span class="li-normal">required: False</span> </li>
                <li><span class="li-required">mkey</span> - Filter: Name of the interface to fetch PoE statistics for. <span class="li-normal">type: string</span> <span class="li-normal">required: False</span> </li>
                
            </ul>
        
        </li>
        system_interface_speed-test-status
        <li><span class="li-head">system_interface_speed-test-status</span> - Retrieve the current status of a speed-test with the results if finished. 
        <ul class="ul-self">
                <li><span class="li-required">id</span> - ID of the speed test. <span class="li-normal">type: int</span> <span class="li-normal">required: True</span> </li>
                
            </ul>
        
        </li>
        system_interface_transceivers
        <li><span class="li-head">system_interface_transceivers</span> - Get a list of transceivers being used by the FortiGate. 
        <ul class="ul-self">
                <li><span class="li-required">scope</span> - Scope from which to retrieve the transceiver information from [vdom|global]. <span class="li-normal">type: string</span> <span class="li-normal">required: False</span> </li>
                
            </ul>
        
        </li>
        system_ipconf
        <li><span class="li-head">system_ipconf</span> - Determine if there is an IP conflict for a specific IP using ARP. 
        <ul class="ul-self">
                <li><span class="li-required">devs</span> - List of interfaces to check for conflict. <span class="li-normal">type: array</span> <span class="li-normal">required: True</span> </li>
                <li><span class="li-required">ipaddr</span> - IPv4 address to check for conflict. <span class="li-normal">type: string</span> <span class="li-normal">required: True</span> </li>
                
            </ul>
        
        </li>
        system_link-monitor
        <li><span class="li-head">system_link-monitor</span> - Retrieve per-interface statistics for active link monitors. 
        <ul class="ul-self">
                <li><span class="li-required">mkey</span> - Name of link monitor. <span class="li-normal">type: string</span> <span class="li-normal">required: False</span> </li>
                
            </ul>
        
        </li>
        system_lte-modem_status
        <li><span class="li-head">system_lte-modem_status</span> 
        
        </li>
        system_modem
        <li><span class="li-head">system_modem</span> 
        
        </li>
        system_nat46-ippools
        <li><span class="li-head">system_nat46-ippools</span> 
        
        </li>
        system_ntp_status
        <li><span class="li-head">system_ntp_status</span> 
        
        </li>
        system_object-tagging_usage
        <li><span class="li-head">system_object-tagging_usage</span> 
        
        </li>
        system_object_usage
        <li><span class="li-head">system_object_usage</span> - Retrieve all objects that are currently using as well as objects that can use the given object. 
        <ul class="ul-self">
                <li><span class="li-required">scope</span> - Scope of resource [vdom|global]. <span class="li-normal">type: string</span> <span class="li-normal">required: False</span> </li>
                <li><span class="li-required">q_name</span> - The CMDB table's name <span class="li-normal">type: string</span> <span class="li-normal">required: False</span> </li>
                <li><span class="li-required">mkey</span> - The mkey for the object <span class="li-normal">type: string</span> <span class="li-normal">required: True</span> </li>
                <li><span class="li-required">qtypes</span> - List of CMDB table qTypes <span class="li-normal">type: array</span> <span class="li-normal">required: False</span> </li>
                <li><span class="li-required">q_path</span> - The CMDB table's path <span class="li-normal">type: string</span> <span class="li-normal">required: False</span> </li>
                
            </ul>
        
        </li>
        system_resolve-fqdn
        <li><span class="li-head">system_resolve-fqdn</span> - Resolves the provided FQDNs to FQDN -> IP mappings. 
        <ul class="ul-self">
                <li><span class="li-required">fqdn</span> - List of FQDNs to be resolved <span class="li-normal">type: array</span> <span class="li-normal">required: False</span> </li>
                <li><span class="li-required">ipv6</span> - Resolve for the AAAA record? <span class="li-normal">type: boolean</span> <span class="li-normal">required: False</span> </li>
                
            </ul>
        
        </li>
        system_resource_usage
        <li><span class="li-head">system_resource_usage</span> - Retreive current and historical usage data for a provided resource. 
        <ul class="ul-self">
                <li><span class="li-required">scope</span> - Scope of resource [vdom|global]. This parameter is only applicable if the FGT is in VDOM mode. <span class="li-normal">type: string</span> <span class="li-normal">required: False</span> </li>
                <li><span class="li-required">interval</span> - Time interval of resource usage [1-min|10-min|30-min|1-hour|12-hour|24-hour]. Defaults to all intervals if not provided. <span class="li-normal">type: string</span> <span class="li-normal">required: False</span> </li>
                <li><span class="li-required">resource</span> - Resource to get usage data for [cpu|mem|disk|session|session6|setuprate|setuprate6|disk_lograte|faz_lograte|forticloud_lograte|gtp_tunnel|gtp_tunnel_setup_rate]. Defaults to all resources if not provided. Additionally, [npu_session|npu_session6] data is available for devices that have an NPU and [nturbo_session|nturbo_session6] data is available for NP6 devices that support NTurbo. [gtp_tunnel|gtp_tunnel_setup_rate] data is available for carrier platforms only. <span class="li-normal">type: string</span> <span class="li-normal">required: False</span> </li>
                
            </ul>
        
        </li>
        system_running-processes
        <li><span class="li-head">system_running-processes</span> 
        
        </li>
        system_sandbox_cloud-regions
        <li><span class="li-head">system_sandbox_cloud-regions</span> 
        
        </li>
        system_sandbox_connection
        <li><span class="li-head">system_sandbox_connection</span> - Test the connection to FortiSandbox. 
        <ul class="ul-self">
                <li><span class="li-required">server</span> - IP/FQDN of the FortiSandbox to test. Uses the configured FortiSandbox IP/FQDN if no server is provided. <span class="li-normal">type: string</span> <span class="li-normal">required: False</span> </li>
                
            </ul>
        
        </li>
        system_sandbox_stats
        <li><span class="li-head">system_sandbox_stats</span> 
        
        </li>
        system_sandbox_status
        <li><span class="li-head">system_sandbox_status</span> 
        
        </li>
        system_sandbox_test-connect
        <li><span class="li-head">system_sandbox_test-connect</span> - Test the connectivity of a given FortiSandbox IP. 
        <ul class="ul-self">
                <li><span class="li-required">server</span> - IP/FQDN of the FortiSandbox to test. <span class="li-normal">type: string</span> <span class="li-normal">required: True</span> </li>
                
            </ul>
        
        </li>
        system_sdn-connector_nsx-security-tags
        <li><span class="li-head">system_sdn-connector_nsx-security-tags</span> - Retrieve a list of NSX security tags for connected NSX servers. 
        <ul class="ul-self">
                <li><span class="li-required">mkey</span> - Filter: NSX SDN connector name. <span class="li-normal">type: string</span> <span class="li-normal">required: False</span> </li>
                
            </ul>
        
        </li>
        system_sdn-connector_status
        <li><span class="li-head">system_sdn-connector_status</span> - Retrieve connection status for SDN connectors. 
        <ul class="ul-self">
                <li><span class="li-required">type</span> - Filter: SDN connector type. Ignored if mkey is specified. <span class="li-normal">type: string</span> <span class="li-normal">required: False</span> </li>
                <li><span class="li-required">mkey</span> - Filter: SDN connector name. <span class="li-normal">type: string</span> <span class="li-normal">required: False</span> </li>
                
            </ul>
        
        </li>
        system_security-rating
        <li><span class="li-head">system_security-rating</span> - Retrieve a Security Rating report result. Without ID specified, returns the most recent result. 
        <ul class="ul-self">
                <li><span class="li-required">scope</span> - Scope of the report [vdom*|global]. Global scope is only accessible for global administrators. <span class="li-normal">type: string</span> <span class="li-normal">required: False</span> </li>
                <li><span class="li-required">id</span> - Report ID. <span class="li-normal">type: int</span> <span class="li-normal">required: False</span> </li>
                <li><span class="li-required">report_type</span> - Report type to view, Security Report when unspecified. <span class="li-normal">type: string</span> <span class="li-normal">required: False</span> </li>
                
            </ul>
        
        </li>
        system_security-rating_history
        <li><span class="li-head">system_security-rating_history</span> - Retrieve Security Rating history. 
        <ul class="ul-self">
                <li><span class="li-required">report_type</span> - Security Rating report history to view, view Security Report when unspecified. <span class="li-normal">type: string</span> <span class="li-normal">required: False</span> </li>
                
            </ul>
        
        </li>
        system_security-rating_lang
        <li><span class="li-head">system_security-rating_lang</span> - Returns the requested Security Rating language mapping. 
        <ul class="ul-self">
                <li><span class="li-required">key</span> - Requested language mapping (en, fr, big5, euc-kr, GB2312, pg, sp, x-sjis). <span class="li-normal">type: string</span> <span class="li-normal">required: False</span> </li>
                
            </ul>
        
        </li>
        system_security-rating_status
        <li><span class="li-head">system_security-rating_status</span> - Check if a Security Rating report is currently running. 
        <ul class="ul-self">
                <li><span class="li-required">progress</span> - Query report progress. <span class="li-normal">type: boolean</span> <span class="li-normal">required: False</span> </li>
                <li><span class="li-required">id</span> - Report ID. <span class="li-normal">type: int</span> <span class="li-normal">required: False</span> </li>
                <li><span class="li-required">report_type</span> - Report type to view, Security Report when unspecified. <span class="li-normal">type: string</span> <span class="li-normal">required: False</span> </li>
                
            </ul>
        
        </li>
        system_security-rating_supported-reports
        <li><span class="li-head">system_security-rating_supported-reports</span> 
        
        </li>
        system_sensor-info
        <li><span class="li-head">system_sensor-info</span> 
        
        </li>
        system_sniffer
        <li><span class="li-head">system_sniffer</span> 
        
        </li>
        system_sniffer_download
        <li><span class="li-head">system_sniffer_download</span> - Download a stored packet capture. 
        <ul class="ul-self">
                <li><span class="li-required">mkey</span> - ID of packet capture entry. <span class="li-normal">type: int</span> <span class="li-normal">required: True</span> </li>
                
            </ul>
        
        </li>
        system_status
        <li><span class="li-head">system_status</span> 
        
        </li>
        system_storage
        <li><span class="li-head">system_storage</span> 
        
        </li>
        system_time
        <li><span class="li-head">system_time</span> 
        
        </li>
        system_timezone
        <li><span class="li-head">system_timezone</span> 
        
        </li>
        system_traffic-history_interface
        <li><span class="li-head">system_traffic-history_interface</span> - Retrieve history traffic stats for an interface. 
        <ul class="ul-self">
                <li><span class="li-required">interface</span> - Interface name. <span class="li-normal">type: string</span> <span class="li-normal">required: True</span> </li>
                <li><span class="li-required">time_period</span> - Time period to retrieve data for [hour | day | week]. <span class="li-normal">type: string</span> <span class="li-normal">required: True</span> </li>
                
            </ul>
        
        </li>
        system_traffic-history_top-applications
        <li><span class="li-head">system_traffic-history_top-applications</span> - Retrieve top FortiView applications traffic stats by bandwidth. 
        <ul class="ul-self">
                <li><span class="li-required">time_period</span> - Time period to retrieve data for [hour | day | week]. <span class="li-normal">type: string</span> <span class="li-normal">required: True</span> </li>
                
            </ul>
        
        </li>
        system_trusted-cert-authorities
        <li><span class="li-head">system_trusted-cert-authorities</span> - Get trusted certifiate authorities. 
        <ul class="ul-self">
                <li><span class="li-required">scope</span> - Scope of certificate [vdom*|global]. <span class="li-normal">type: string</span> <span class="li-normal">required: False</span> </li>
                
            </ul>
        
        </li>
        system_usb-log
        <li><span class="li-head">system_usb-log</span> 
        
        </li>
        system_vdom-link
        <li><span class="li-head">system_vdom-link</span> - Gets a list of all NPU VDOM Links and VDOM Links. 
        <ul class="ul-self">
                <li><span class="li-required">scope</span> - Scope from which to retrieve the VDOM link informaton from [vdom|global]. <span class="li-normal">type: string</span> <span class="li-normal">required: False</span> </li>
                
            </ul>
        
        </li>
        system_vdom-resource
        <li><span class="li-head">system_vdom-resource</span> 
        
        </li>
        system_vm-information
        <li><span class="li-head">system_vm-information</span> 
        
        </li>
        user_banned
        <li><span class="li-head">user_banned</span> 
        
        </li>
        user_collected-email
        <li><span class="li-head">user_collected-email</span> - List email addresses collected from captive portal. 
        <ul class="ul-self">
                <li><span class="li-required">ipv6</span> - Include collected email from IPv6 users. <span class="li-normal">type: boolean</span> <span class="li-normal">required: False</span> </li>
                
            </ul>
        
        </li>
        user_detected-device
        <li><span class="li-head">user_detected-device</span> - Retrieve a list of detected devices. 
        <ul class="ul-self">
                <li><span class="li-required">with_fortiap</span> - Retrieve FortiAP information. <span class="li-normal">type: boolean</span> <span class="li-normal">required: False</span> </li>
                <li><span class="li-required">with_user</span> - Retrieve authenticated user information. <span class="li-normal">type: boolean</span> <span class="li-normal">required: False</span> </li>
                <li><span class="li-required">with_endpoint</span> - Retrieve FortiClient endpoint information. <span class="li-normal">type: boolean</span> <span class="li-normal">required: False</span> </li>
                <li><span class="li-required">with_dhcp</span> - Retrieve DHCP lease information. <span class="li-normal">type: boolean</span> <span class="li-normal">required: False</span> </li>
                <li><span class="li-required">expand_child_macs</span> - Include child devices as separate entries in the list. <span class="li-normal">type: boolean</span> <span class="li-normal">required: False</span> </li>
                <li><span class="li-required">with_fortilink</span> - Retrieve FortiLink information. <span class="li-normal">type: boolean</span> <span class="li-normal">required: False</span> </li>
                
            </ul>
        
        </li>
        user_device
        <li><span class="li-head">user_device</span> - Retrieve a list of detected devices. 
        <ul class="ul-self">
                <li><span class="li-required">master_mac</span> - Filter: Master MAC of a device. Multiple entries could be returned. <span class="li-normal">type: string</span> <span class="li-normal">required: False</span> </li>
                <li><span class="li-required">master_only</span> - List of master device only. <span class="li-normal">type: boolean</span> <span class="li-normal">required: False</span> </li>
                
            </ul>
        
        </li>
        user_device-category
        <li><span class="li-head">user_device-category</span> 
        
        </li>
        user_device-type
        <li><span class="li-head">user_device-type</span> 
        
        </li>
        user_device_query
        <li><span class="li-head">user_device_query</span> - Retrieve user devices from user device store. List all the user devices if there is no filter set. 
        <ul class="ul-self">
                <li><span class="li-required">start</span> - Number of entries to skip from the beginning. <span class="li-normal">type: int</span> <span class="li-normal">required: False</span> </li>
                <li><span class="li-required">number</span> - Maximum number of entries to return. <span class="li-normal">type: int</span> <span class="li-normal">required: False</span> </li>
                <li><span class="li-required">filters</span> - A map of filters. Type: {"key":  "value"} <span class="li-normal">type: object</span> <span class="li-normal">required: False</span> </li>
                
            </ul>
        
        </li>
        user_firewall
        <li><span class="li-head">user_firewall</span> - List authenticated firewall users. 
        <ul class="ul-self">
                <li><span class="li-required">count</span> - Maximum number of entries to return. <span class="li-normal">type: int</span> <span class="li-normal">required: False</span> </li>
                <li><span class="li-required">start</span> - Starting entry index. <span class="li-normal">type: int</span> <span class="li-normal">required: False</span> </li>
                <li><span class="li-required">ipv4</span> - Include IPv4 user (default=true). <span class="li-normal">type: boolean</span> <span class="li-normal">required: False</span> </li>
                <li><span class="li-required">ipv6</span> - Include IPv6 users. <span class="li-normal">type: boolean</span> <span class="li-normal">required: False</span> </li>
                
            </ul>
        
        </li>
        user_fortitoken
        <li><span class="li-head">user_fortitoken</span> 
        
        </li>
        user_fortitoken-cloud_status
        <li><span class="li-head">user_fortitoken-cloud_status</span> 
        
        </li>
        user_fsso
        <li><span class="li-head">user_fsso</span> - Get a list of fsso and fsso polling status. 
        <ul class="ul-self">
                <li><span class="li-required">type</span> - Filter: Get the status for this type of FSSO entry [fsso|fsso-polling]. <span class="li-normal">type: string</span> <span class="li-normal">required: False</span> </li>
                <li><span class="li-required">mkey</span> - Filter: Get the status for a specific FSSO entry. `type` is required if this is set. <span class="li-normal">type: string</span> <span class="li-normal">required: False</span> </li>
                
            </ul>
        
        </li>
        user_info_query
        <li><span class="li-head">user_info_query</span> - Query user info. 
        <ul class="ul-self">
                <li><span class="li-required">start</span> - Number of entries to skip from the beginning. <span class="li-normal">type: int</span> <span class="li-normal">required: False</span> </li>
                <li><span class="li-required">number</span> - Maximum number of entries to return. <span class="li-normal">type: int</span> <span class="li-normal">required: False</span> </li>
                <li><span class="li-required">filters</span> - A list of filters. Type: {"type": string, "value": string} <span class="li-normal">type: array</span> <span class="li-normal">required: True</span> </li>
                
            </ul>
        
        </li>
        user_info_thumbnail
        <li><span class="li-head">user_info_thumbnail</span> - Get user info thumbnail. Returns the first match to the filter. 
        <ul class="ul-self">
                <li><span class="li-required">filters</span> - A list of filters. Type: {"type": string, "value": string} <span class="li-normal">type: array</span> <span class="li-normal">required: True</span> </li>
                
            </ul>
        
        </li>
        utm_antivirus_stats
        <li><span class="li-head">utm_antivirus_stats</span> 
        
        </li>
        utm_app-lookup
        <li><span class="li-head">utm_app-lookup</span> - Query remote FortiFlow database to resolve hosts to application control entries. 
        <ul class="ul-self">
                <li><span class="li-required">hosts</span> - List of hosts to resolve. <span class="li-normal">type: array</span> <span class="li-normal">required: False</span> </li>
                
            </ul>
        
        </li>
        utm_application-categories
        <li><span class="li-head">utm_application-categories</span> 
        
        </li>
        utm_blacklisted-certificates
        <li><span class="li-head">utm_blacklisted-certificates</span> - Retrieve a list of blacklisted SSL certificates. 
        <ul class="ul-self">
                <li><span class="li-required">count</span> - Maximum number of entries to return. Limit is set to 2000. <span class="li-normal">type: int</span> <span class="li-normal">required: True</span> </li>
                <li><span class="li-required">start</span> - Starting entry index. <span class="li-normal">type: int</span> <span class="li-normal">required: True</span> </li>
                
            </ul>
        
        </li>
        utm_blacklisted-certificates_statistics
        <li><span class="li-head">utm_blacklisted-certificates_statistics</span> 
        
        </li>
        videofilter_fortiguard-categories
        <li><span class="li-head">videofilter_fortiguard-categories</span> 
        
        </li>
        virtual-wan_health-check
        <li><span class="li-head">virtual-wan_health-check</span> 
        
        </li>
        virtual-wan_interface-log
        <li><span class="li-head">virtual-wan_interface-log</span> - Retrieve log of SD-WAN interface quality information. 
        <ul class="ul-self">
                <li><span class="li-required">interface</span> - Filter: Interface name. <span class="li-normal">type: string</span> <span class="li-normal">required: False</span> </li>
                <li><span class="li-required">seconds</span> - Filter: Only return SLA logs generated in the last N seconds. <span class="li-normal">type: int</span> <span class="li-normal">required: False</span> </li>
                <li><span class="li-required">since</span> - Filter: Only return SLA logs generated since this Unix timestamp. <span class="li-normal">type: int</span> <span class="li-normal">required: False</span> </li>
                
            </ul>
        
        </li>
        virtual-wan_members
        <li><span class="li-head">virtual-wan_members</span> 
        
        </li>
        virtual-wan_sla-log
        <li><span class="li-head">virtual-wan_sla-log</span> - Retrieve log of SLA probe results for for each SD-WAN SLA rule. 
        <ul class="ul-self">
                <li><span class="li-required">interface</span> - Filter: Interface name. <span class="li-normal">type: string</span> <span class="li-normal">required: False</span> </li>
                <li><span class="li-required">seconds</span> - Filter: Only return SLA logs generated in the last N seconds. <span class="li-normal">type: int</span> <span class="li-normal">required: False</span> </li>
                <li><span class="li-required">since</span> - Filter: Only return SLA logs generated since this Unix timestamp. <span class="li-normal">type: int</span> <span class="li-normal">required: False</span> </li>
                <li><span class="li-required">sla</span> - Filter: SLA name. <span class="li-normal">type: string</span> <span class="li-normal">required: False</span> </li>
                
            </ul>
        
        </li>
        vpn_ipsec
        <li><span class="li-head">vpn_ipsec</span> - Return an array of active IPsec VPNs. 
        <ul class="ul-self">
                <li><span class="li-required">tunnel</span> - Filter for a specific IPsec tunnel name. <span class="li-normal">type: string</span> <span class="li-normal">required: False</span> </li>
                <li><span class="li-required">start</span> - Starting entry index. <span class="li-normal">type: int</span> <span class="li-normal">required: False</span> </li>
                <li><span class="li-required">count</span> - Maximum number of entries to return. <span class="li-normal">type: int</span> <span class="li-normal">required: False</span> </li>
                
            </ul>
        
        </li>
        vpn_ocvpn_members
        <li><span class="li-head">vpn_ocvpn_members</span> 
        
        </li>
        vpn_ocvpn_meta
        <li><span class="li-head">vpn_ocvpn_meta</span> 
        
        </li>
        vpn_ocvpn_status
        <li><span class="li-head">vpn_ocvpn_status</span> 
        
        </li>
        vpn_one-click_members
        <li><span class="li-head">vpn_one-click_members</span> 
        
        </li>
        vpn_one-click_status
        <li><span class="li-head">vpn_one-click_status</span> 
        
        </li>
        vpn_ssl
        <li><span class="li-head">vpn_ssl</span> 
        
        </li>
        vpn_ssl_stats
        <li><span class="li-head">vpn_ssl_stats</span> 
        
        </li>
        wanopt_history
        <li><span class="li-head">wanopt_history</span> - Retrieve WAN opt. statistics history. 
        <ul class="ul-self">
                <li><span class="li-required">period</span> - Statistics period [10-min*|hour|day|week|30-day]. <span class="li-normal">type: string</span> <span class="li-normal">required: False</span> </li>
                
            </ul>
        
        </li>
        wanopt_peer_stats
        <li><span class="li-head">wanopt_peer_stats</span> 
        
        </li>
        wanopt_webcache
        <li><span class="li-head">wanopt_webcache</span> - Retrieve webcache statistics history. 
        <ul class="ul-self">
                <li><span class="li-required">period</span> - Statistics period [10-min*|hour|day|week|30-day]. <span class="li-normal">type: string</span> <span class="li-normal">required: False</span> </li>
                
            </ul>
        
        </li>
        web-ui_custom-language_download
        <li><span class="li-head">web-ui_custom-language_download</span> - Download a custom language file. 
        <ul class="ul-self">
                <li><span class="li-required">filename</span> - Name of custom language entry. <span class="li-normal">type: string</span> <span class="li-normal">required: True</span> </li>
                
            </ul>
        
        </li>
        webcache_stats
        <li><span class="li-head">webcache_stats</span> - Retrieve webcache statistics. 
        <ul class="ul-self">
                <li><span class="li-required">period</span> - Statistics period [10min|hour|day|month]. <span class="li-normal">type: string</span> <span class="li-normal">required: False</span> </li>
                
            </ul>
        
        </li>
        webfilter_category-quota
        <li><span class="li-head">webfilter_category-quota</span> - Retrieve quota usage statistics for webfilter categories. 
        <ul class="ul-self">
                <li><span class="li-required">profile</span> - Webfilter profile. <span class="li-normal">type: string</span> <span class="li-normal">required: False</span> </li>
                <li><span class="li-required">user</span> - User or IP (required if profile specified). <span class="li-normal">type: string</span> <span class="li-normal">required: False</span> </li>
                
            </ul>
        
        </li>
        webfilter_fortiguard-categories
        <li><span class="li-head">webfilter_fortiguard-categories</span> - Return FortiGuard web filter categories. 
        <ul class="ul-self">
                <li><span class="li-required">convert_unrated_id</span> - Convert Unrated category id to the one for CLI use. <span class="li-normal">type: boolean</span> <span class="li-normal">required: False</span> </li>
                <li><span class="li-required">include_unrated</span> - Include Unrated category in result list. <span class="li-normal">type: boolean</span> <span class="li-normal">required: False</span> </li>
                
            </ul>
        
        </li>
        webfilter_malicious-urls
        <li><span class="li-head">webfilter_malicious-urls</span> 
        
        </li>
        webfilter_malicious-urls_stat
        <li><span class="li-head">webfilter_malicious-urls_stat</span> 
        
        </li>
        webfilter_override
        <li><span class="li-head">webfilter_override</span> 
        
        </li>
        webfilter_trusted-urls
        <li><span class="li-head">webfilter_trusted-urls</span> 
        
        </li>
        webproxy_pacfile_download
        <li><span class="li-head">webproxy_pacfile_download</span> 
        
        </li>
        wifi_ap-names
        <li><span class="li-head">wifi_ap-names</span> 
        
        </li>
        wifi_ap_channels
        <li><span class="li-head">wifi_ap_channels</span> - Retrieve the set of channel lists for all possible band/configurations for the given FortiAP platform. 
        <ul class="ul-self">
                <li><span class="li-required">country</span> - Two-letter code for the country the AP is operating in. <span class="li-normal">type: string</span> <span class="li-normal">required: False</span> </li>
                <li><span class="li-required">indoor_outdoor</span> - FortiAP indoor/outdoor configuration value (0 for indoor, 1 for outdoor, 2 for default). <span class="li-normal">type: int</span> <span class="li-normal">required: False</span> </li>
                <li><span class="li-required">platform_type</span> - Short name for platform type (e.g. '220A') <span class="li-normal">type: string</span> <span class="li-normal">required: True</span> </li>
                
            </ul>
        
        </li>
        wifi_ap_status
        <li><span class="li-head">wifi_ap_status</span> 
        
        </li>
        wifi_client
        <li><span class="li-head">wifi_client</span> - Retrieve a list of connected WiFi clients. 
        <ul class="ul-self">
                <li><span class="li-required">count</span> - Maximum number of entries to return. <span class="li-normal">type: int</span> <span class="li-normal">required: False</span> </li>
                <li><span class="li-required">start</span> - Starting entry index. <span class="li-normal">type: int</span> <span class="li-normal">required: False</span> </li>
                <li><span class="li-required">type</span> - Request type [all*|fail-login]. <span class="li-normal">type: string</span> <span class="li-normal">required: False</span> </li>
                
            </ul>
        
        </li>
        wifi_euclid
        <li><span class="li-head">wifi_euclid</span> 
        
        </li>
        wifi_firmware
        <li><span class="li-head">wifi_firmware</span> - Retrieve a list of current and recommended firmware for FortiAPs in use. 
        <ul class="ul-self">
                <li><span class="li-required">timeout</span> - FortiGuard connection timeout (defaults to 2 seconds). <span class="li-normal">type: string</span> <span class="li-normal">required: False</span> </li>
                
            </ul>
        
        </li>
        wifi_interfering_ap
        <li><span class="li-head">wifi_interfering_ap</span> - Retrieve a list of interfering APs for one FortiAP radio. 
        <ul class="ul-self">
                <li><span class="li-required">wtp</span> - FortiAP ID to query. <span class="li-normal">type: string</span> <span class="li-normal">required: False</span> </li>
                <li><span class="li-required">start</span> - Starting entry index. <span class="li-normal">type: int</span> <span class="li-normal">required: False</span> </li>
                <li><span class="li-required">radio</span> - Radio ID. <span class="li-normal">type: int</span> <span class="li-normal">required: False</span> </li>
                <li><span class="li-required">count</span> - Maximum number of entries to return. <span class="li-normal">type: int</span> <span class="li-normal">required: False</span> </li>
                
            </ul>
        
        </li>
        wifi_managed_ap
        <li><span class="li-head">wifi_managed_ap</span> - Retrieve a list of managed FortiAPs. 
        <ul class="ul-self">
                <li><span class="li-required">incl_local</span> - Enable to include the local FortiWiFi device in the results. <span class="li-normal">type: boolean</span> <span class="li-normal">required: False</span> </li>
                <li><span class="li-required">wtp_id</span> - Filter: single managed FortiAP by ID. <span class="li-normal">type: string</span> <span class="li-normal">required: False</span> </li>
                
            </ul>
        
        </li>
        wifi_meta
        <li><span class="li-head">wifi_meta</span> 
        
        </li>
        wifi_network_list
        <li><span class="li-head">wifi_network_list</span> 
        
        </li>
        wifi_network_status
        <li><span class="li-head">wifi_network_status</span> 
        
        </li>
        wifi_region-image
        <li><span class="li-head">wifi_region-image</span> - Retrieves a floorplan/region image from a configured FortiAP region. 
        <ul class="ul-self">
                <li><span class="li-required">region_name</span> - Region name to retrieve image from. <span class="li-normal">type: string</span> <span class="li-normal">required: True</span> </li>
                
            </ul>
        
        </li>
        wifi_rogue_ap
        <li><span class="li-head">wifi_rogue_ap</span> - Retrieve a list of detected rogue APs. 
        <ul class="ul-self">
                <li><span class="li-required">count</span> - Maximum number of entries to return. <span class="li-normal">type: int</span> <span class="li-normal">required: False</span> </li>
                <li><span class="li-required">managed_ssid_only</span> - Filter: True to include only WiFi controller managed SSIDs. <span class="li-normal">type: boolean</span> <span class="li-normal">required: False</span> </li>
                <li><span class="li-required">start</span> - Starting entry index. <span class="li-normal">type: int</span> <span class="li-normal">required: False</span> </li>
                
            </ul>
        
        </li>
        wifi_spectrum
        <li><span class="li-head">wifi_spectrum</span> - Retrieve spectrum analysis information for a specific FortiAP. 
        <ul class="ul-self">
                <li><span class="li-required">wtp_id</span> - FortiAP ID to query. <span class="li-normal">type: string</span> <span class="li-normal">required: True</span> </li>
                
            </ul>
        
        </li>
        wifi_vlan-probe
        <li><span class="li-head">wifi_vlan-probe</span> - Retrieve the VLAN probe results. 
        <ul class="ul-self">
                <li><span class="li-required">wtp</span> - FortiAP ID. <span class="li-normal">type: string</span> <span class="li-normal">required: True</span> </li>
                <li><span class="li-required">ap_interface</span> - FortiAP interface to send the probe on. <span class="li-normal">type: int</span> <span class="li-normal">required: True</span> </li>
                
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

   - fortios_monitor_fact:
        vdom: ""
        enable_log: true
        formatters:
            - model_name
        filters:
            - model_name==FortiGat
        selector: 'system_status'

   - name: fact gathering
     fortios_monitor_fact:
        vdom: ""
        access_token: ""
        selector: 'firewall_acl'

   - name: fact gathering
     fortios_monitor_fact:
        vdom: ""
        access_token: ""
        selector: 'firewall_security-policy'
        params:
            policyid: '1'


Return Values
-------------
Common return values are documented: https://docs.ansible.com/ansible/latest/reference_appendices/common_return_values.html#common-return-values, the following are the fields unique to this module:

.. raw:: html

    <ul>

    <li> <span class="li-return">build</span> - Build number of the fortigate image <span class="li-normal">returned: always</span> <span class="li-normal">type: str</span> <span class="li-normal">sample: 1547</span></li>
    <li> <span class="li-return">http_method</span> - Last method used to provision the content into FortiGate <span class="li-normal">returned: always</span> <span class="li-normal">type: str</span> <span class="li-normal">sample: GET</span></li>
    <li> <span class="li-return">name</span> - Name of the table used to fulfill the request <span class="li-normal">returned: always</span> <span class="li-normal">type: str</span> <span class="li-normal">sample: firmware</span></li>
    <li> <span class="li-return">path</span> - Path of the table used to fulfill the request <span class="li-normal">returned: always</span> <span class="li-normal">type: str</span> <span class="li-normal">sample: system</span></li>
    <li> <span class="li-return">results</span> - Object list retrieved from device. <span class="li-normal">returned: always</span> <span class="li-normal">type: list</span></li>
    <li> <span class="li-return">revision</span> - Internal revision number <span class="li-normal">returned: always</span> <span class="li-normal">type: str</span> <span class="li-normal">sample: 17.0.2.10658</span></li>
    <li> <span class="li-return">serial</span> - Serial number of the unit <span class="li-normal">returned: always</span> <span class="li-normal">type: str</span> <span class="li-normal">sample: FGVMEVYYQT3AB5352</span></li>
    <li> <span class="li-return">status</span> - Indication of the operation's result <span class="li-normal">returned: always</span> <span class="li-normal">type: str</span> <span class="li-normal">sample: success</span></li>
    <li> <span class="li-return">vdom</span> - Virtual domain used <span class="li-normal">returned: always</span> <span class="li-normal">type: str</span> <span class="li-normal">sample: root</span></li>
    <li> <span class="li-return">version</span> - Version of the FortiGate <span class="li-normal">returned: always</span> <span class="li-normal">type: str</span> <span class="li-normal">sample: v5.6.3</span></li>
    <li> <span class="li-return">ansible_facts</span> - The list of fact subsets collected from the device <span class="li-normal">returned: always</span> <span class="li-normal">type: dict</span></li>
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