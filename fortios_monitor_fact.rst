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
    <li><span class="li-head">selector</span> - selector of the retrieved fortimanager facts <span class="li-normal">type: str</span> <span class="li-required">choices:</span></li>
        <li style="list-style: none;"><section class="accordion">
        <input type="checkbox" name="collapse" id="handle2">
        <h2 class="handle">
            <label for="handle2"><u>Show full selector list...</u></label>
        </h2>
        <div class="content">
        <ul class="ul-self">
        <li><span class="li-head">endpoint-control_avatar_download</span> - Download an endpoint avatar image. 
        <ul class="ul-self">
                <li><span class="li-required">default</span> - Default avatar name ['authuser'|'unauthuser'|'authuser_72'|'unauthuser_72']. Default avatar when endpoint / device avatar is not available. If default is not set, Not found 404 is returned. <span class="li-normal">type: string </span> </li>
                <li><span class="li-required">uid</span> - Single FortiClient UID. <span class="li-normal">type: string </span> </li>
                <li><span class="li-required">user</span> - User name of the endpoint. <span class="li-normal">type: string </span> </li>
                
            </ul>
        
        </li>
        <li><span class="li-head">endpoint-control_ems_cert-status</span> - Retrieve authentication status of the EMS server certificate for a specific EMS. 
        <ul class="ul-self">
                <li><span class="li-required">with_cert</span> - Return detailed certificate information. Available when the certificate is authenticated by installed CA certificates.  <span class="li-normal">type: boolean </span> </li>
                <li><span class="li-required">ems_name</span> - EMS server name (as defined in CLI table endpoint-control.fctems). <span class="li-normal">type: string </span> </li>
                
            </ul>
        
        </li>
        <li><span class="li-head">endpoint-control_ems_status</span> - Retrieve EMS connection status for a specific EMS. 
        <ul class="ul-self">
                <li><span class="li-required">ems_name</span> - EMS server name (as defined in CLI table endpoint-control.fctems). <span class="li-normal">type: string </span> </li>
                
            </ul>
        
        </li>
        <li><span class="li-head">endpoint-control_installer</span> - List available FortiClient installers. 
        <ul class="ul-self">
                <li><span class="li-required">min_version</span> - Filter: Minimum installer version. (String of the format n[.n[.n]]). <span class="li-normal">type: string </span> </li>
                
            </ul>
        
        </li>
        <li><span class="li-head">endpoint-control_installer_download</span> - Download a FortiClient installer via FortiGuard. 
        <ul class="ul-self">
                <li><span class="li-required">mkey</span> - Name of installer (image_id). <span class="li-normal">type: string </span> </li>
                
            </ul>
        
        </li>
        <li><span class="li-head">endpoint-control_record-list</span> - List endpoint records. 
        <ul class="ul-self">
                <li><span class="li-required">intf_name</span> - Filter: Name of interface where the endpoint was detected. <span class="li-normal">type: string </span> </li>
                
            </ul>
        
        </li>
        <li><span class="li-head">endpoint-control_summary</span> 
        
        </li>
        <li><span class="li-head">extender-controller_extender</span> - Retrieve statistics for specific configured FortiExtender units. 
        <ul class="ul-self">
                <li><span class="li-required">type</span> - Statistic type.'type' options are [system | modem | usage | last]. If 'type' is not specified, all types of statistics are retrieved. <span class="li-normal">type: string </span> </li>
                <li><span class="li-required">id</span> - List of FortiExtender IDs to query. <span class="li-normal">type: array </span> </li>
                
            </ul>
        
        </li>
        <li><span class="li-head">firewall_acl</span> 
        
        </li>
        <li><span class="li-head">firewall_acl6</span> 
        
        </li>
        <li><span class="li-head">firewall_address-dynamic</span> 
        
        </li>
        <li><span class="li-head">firewall_address-fqdns</span> 
        
        </li>
        <li><span class="li-head">firewall_address-fqdns6</span> 
        
        </li>
        <li><span class="li-head">firewall_address6-dynamic</span> 
        
        </li>
        <li><span class="li-head">firewall_health</span> 
        
        </li>
        <li><span class="li-head">firewall_internet-service-details</span> - List all details for a given Internet Service ID. 
        <ul class="ul-self">
                <li><span class="li-required">count</span> - Maximum number of entries to return. Valid range is [20, 1000]; if a value is specified out of that range, it will be rounded up or down. Default value is 1000. <span class="li-normal">type: int </span> </li>
                <li><span class="li-required">region_id</span> - Filter: Region ID. <span class="li-normal">type: int </span> </li>
                <li><span class="li-required">summary_only</span> - Only return number of entries instead of entries. <span class="li-normal">type: boolean </span> </li>
                <li><span class="li-required">city_id</span> - Filter: City ID. <span class="li-normal">type: int </span> </li>
                <li><span class="li-required">country_id</span> - Filter: Country ID. <span class="li-normal">type: int </span> </li>
                <li><span class="li-required">start</span> - Starting entry index. If a value is less than zero, it will be set to zero. <span class="li-normal">type: int </span> </li>
                <li><span class="li-required">id</span> - ID of the Internet Service to get details for. <span class="li-normal">type: int </span> </li>
                
            </ul>
        
        </li>
        <li><span class="li-head">firewall_internet-service-match</span> - List internet services that exist at a given IP or Subnet. 
        <ul class="ul-self">
                <li><span class="li-required">ip</span> - IP (in dot-decimal notation). <span class="li-normal">type: string </span> </li>
                <li><span class="li-required">mask</span> - IP Mask (in dot-decimal notation). <span class="li-normal">type: string </span> </li>
                
            </ul>
        
        </li>
        <li><span class="li-head">firewall_ippool</span> 
        
        </li>
        <li><span class="li-head">firewall_load-balance</span> - List all firewall load balance servers. 
        <ul class="ul-self">
                <li><span class="li-required">count</span> - Maximum number of entries to return. <span class="li-normal">type: int </span> </li>
                <li><span class="li-required">start</span> - Starting entry index. <span class="li-normal">type: int </span> </li>
                
            </ul>
        
        </li>
        <li><span class="li-head">firewall_local-in</span> 
        
        </li>
        <li><span class="li-head">firewall_per-ip-shaper</span> 
        
        </li>
        <li><span class="li-head">firewall_policy</span> - List traffic statistics for firewall policies. 
        <ul class="ul-self">
                <li><span class="li-required">ip_version</span> - Filter: Traffic IP Version. [ ipv4 | ipv6 ], if left empty, will retrieve data for both ipv4 and ipv6. <span class="li-normal">type: string </span> </li>
                <li><span class="li-required">policyid</span> - Filter: Policy ID. <span class="li-normal">type: int </span> </li>
                
            </ul>
        
        </li>
        <li><span class="li-head">firewall_policy-lookup</span> - Performs a policy lookup by creating a dummy packet and asking the kernel which policy would be hit. 
        <ul class="ul-self">
                <li><span class="li-required">protocol</span> - Protocol. <span class="li-normal">type: string </span> </li>
                <li><span class="li-required">dest</span> - Destination IP/FQDN. <span class="li-normal">type: string </span> </li>
                <li><span class="li-required">icmpcode</span> - ICMP code. <span class="li-normal">type: int </span> </li>
                <li><span class="li-required">icmptype</span> - ICMP type. <span class="li-normal">type: int </span> </li>
                <li><span class="li-required">srcintf</span> - Source interface. <span class="li-normal">type: string </span> </li>
                <li><span class="li-required">ipv6</span> - Perform an IPv6 lookup? <span class="li-normal">type: boolean </span> </li>
                <li><span class="li-required">sourceport</span> - Source port. <span class="li-normal">type: int </span> </li>
                <li><span class="li-required">sourceip</span> - Source IP. <span class="li-normal">type: string </span> </li>
                <li><span class="li-required">destport</span> - Destination port. <span class="li-normal">type: int </span> </li>
                
            </ul>
        
        </li>
        <li><span class="li-head">firewall_proxy-policy</span> - List traffic statistics for all explicit proxy policies. 
        <ul class="ul-self">
                <li><span class="li-required">policyid</span> - Filter: Policy ID. <span class="li-normal">type: int </span> </li>
                
            </ul>
        
        </li>
        <li><span class="li-head">firewall_sdn-connector-filters</span> - List all available filters for a specified SDN Fabric Connector. Used for Fabric Connector address objects. 
        <ul class="ul-self">
                <li><span class="li-required">connector</span> - Name of the SDN Fabric Connector to get the filters from. <span class="li-normal">type: string </span> </li>
                
            </ul>
        
        </li>
        <li><span class="li-head">firewall_security-policy</span> - List IPS engine statistics for security policies. 
        <ul class="ul-self">
                <li><span class="li-required">policyid</span> - Filter: Policy ID. <span class="li-normal">type: int </span> </li>
                
            </ul>
        
        </li>
        <li><span class="li-head">firewall_session</span> - List all active firewall sessions (optionally filtered). 
        <ul class="ul-self">
                <li><span class="li-required">since</span> - Filter: Only return sessions generated since this Unix timestamp. <span class="li-normal">type: int </span> </li>
                <li><span class="li-required">protocol</span> - Filter: Protocol name [all|igmp|tcp|udp|icmp|etc]. <span class="li-normal">type: string </span> </li>
                <li><span class="li-required">nturbo</span> - Filter: 1 to include nTurbo sessions, 0 to exclude. <span class="li-normal">type: int </span> </li>
                <li><span class="li-required">srcintfrole</span> - Filter: Source interface roles. <span class="li-normal">type: array </span> </li>
                <li><span class="li-required">owner</span> - Filter: Destination owner. <span class="li-normal">type: string </span> </li>
                <li><span class="li-required">srcuuid</span> - Filter: Source UUID. <span class="li-normal">type: string </span> </li>
                <li><span class="li-required">dstintfrole</span> - Filter: Destination interface roles. <span class="li-normal">type: array </span> </li>
                <li><span class="li-required">natsourceaddress</span> - Filter: NAT source address. <span class="li-normal">type: string </span> </li>
                <li><span class="li-required">source</span> - Filter: Source IP address. <span class="li-normal">type: string </span> </li>
                <li><span class="li-required">destination</span> - Filter: Destination IP address. <span class="li-normal">type: string </span> </li>
                <li><span class="li-required">application</span> - Filter: Application PROTO/PORT. (e.g. "TCP/443") <span class="li-normal">type: string </span> </li>
                <li><span class="li-required">sourceport</span> - Filter: Source port. <span class="li-normal">type: int </span> </li>
                <li><span class="li-required">natsourceport</span> - Filter: NAT source port. <span class="li-normal">type: int </span> </li>
                <li><span class="li-required">start</span> - Starting entry index. <span class="li-normal">type: int </span> </li>
                <li><span class="li-required">dstuuid</span> - Filter: Destination UUID. <span class="li-normal">type: string </span> </li>
                <li><span class="li-required">username</span> - Filter: Authenticated username. <span class="li-normal">type: string </span> </li>
                <li><span class="li-required">seconds</span> - Filter: Only return sessions generated in the last N seconds. <span class="li-normal">type: int </span> </li>
                <li><span class="li-required">policyid</span> - Filter: Policy ID. <span class="li-normal">type: int </span> </li>
                <li><span class="li-required">srcintf</span> - Filter: Source interface name. <span class="li-normal">type: string </span> </li>
                <li><span class="li-required">fortiasic</span> - Filter: 1 to include NPU accelerated sessions, 0 to exclude. <span class="li-normal">type: int </span> </li>
                <li><span class="li-required">destport</span> - Filter: Destination port. <span class="li-normal">type: int </span> </li>
                <li><span class="li-required">count</span> - Maximum number of entries to return. Valid range is [20, 1000]; if a value is specified out of that range, it will be rounded up or down. <span class="li-normal">type: int </span> </li>
                <li><span class="li-required">filter-csf</span> - Filter: Include sessions from downstream fortigates. <span class="li-normal">type: boolean </span> </li>
                <li><span class="li-required">country</span> - Filter: Destination country name. <span class="li-normal">type: string </span> </li>
                <li><span class="li-required">summary</span> - Enable/disable inclusion of session summary (setup rate, total sessions, etc). <span class="li-normal">type: boolean </span> </li>
                <li><span class="li-required">shaper</span> - Filter: Forward traffic shaper name. <span class="li-normal">type: string </span> </li>
                <li><span class="li-required">ip_version</span> - IP version [*ipv4 | ipv6 | ipboth]. <span class="li-normal">type: string </span> </li>
                <li><span class="li-required">dstintf</span> - Filter: Destination interface name. <span class="li-normal">type: string </span> </li>
                
            </ul>
        
        </li>
        <li><span class="li-head">firewall_shaper</span> 
        
        </li>
        <li><span class="li-head">firewall_uuid-list</span> 
        
        </li>
        <li><span class="li-head">firewall_uuid-type-lookup</span> - Retrieve a mapping of UUIDs to their firewall object type for given UUIDs. 
        <ul class="ul-self">
                <li><span class="li-required">uuids</span> - List of UUIDs to be resolved. <span class="li-normal">type: array </span> </li>
                
            </ul>
        
        </li>
        <li><span class="li-head">fortiguard_redirect-portal</span> 
        
        </li>
        <li><span class="li-head">fortiguard_service-communication-stats</span> - Retrieve historical statistics for communication with FortiGuard services. 
        <ul class="ul-self">
                <li><span class="li-required">service_type</span> - To get stats for [forticare|fortiguard_download|fortiguard_query|forticloud_log|fortisandbox_cloud|fortiguard.com|ocvpn|sdns|fortitoken_registration|sms_service]. Defaults to all stats if not provided. <span class="li-normal">type: string </span> </li>
                <li><span class="li-required">timeslot</span> - History timeslot of stats [1_hour|24_hour|1_week]. Defaults to all timeslots if not provided. <span class="li-normal">type: string </span> </li>
                
            </ul>
        
        </li>
        <li><span class="li-head">fortiview_sandbox-file-details</span> - Retrieve FortiSandbox analysis details for a specific file checksum. 
        <ul class="ul-self">
                <li><span class="li-required">checksum</span> - Checksum of a specific file that has been analyzed by the connected FortiSandbox. <span class="li-normal">type: string </span> </li>
                
            </ul>
        
        </li>
        <li><span class="li-head">fortiview_sandbox-file-list</span> 
        
        </li>
        <li><span class="li-head">fortiview_statistics</span> - Retrieve drill-down and summary data for FortiView (both realtime and historical). 
        <ul class="ul-self">
                <li><span class="li-required">count</span> - Maximum number of details to return. <span class="li-normal">type: int </span> </li>
                <li><span class="li-required">end</span> - End timestamp. <span class="li-normal">type: int </span> </li>
                <li><span class="li-required">realtime</span> - Set to true to retrieve realtime results (from kernel). <span class="li-normal">type: boolean </span> </li>
                <li><span class="li-required">chart_only</span> - Only return graph values in results. <span class="li-normal">type: boolean </span> </li>
                <li><span class="li-required">sort_by</span> - Sort by field. <span class="li-normal">type: string </span> </li>
                <li><span class="li-required">filter</span> - A map of filter keys to arrays of values. <span class="li-normal">type: object </span> </li>
                <li><span class="li-required">start</span> - Start timestamp. <span class="li-normal">type: int </span> </li>
                <li><span class="li-required">sessionid</span> - FortiView request Session ID. <span class="li-normal">type: int </span> </li>
                <li><span class="li-required">report_by</span> - Report by field. <span class="li-normal">type: string </span> </li>
                <li><span class="li-required">device</span> - FortiView source device [disk|fortianalyzer|forticloud]. <span class="li-normal">type: string </span> </li>
                <li><span class="li-required">ip_version</span> - IP version [*ipv4 | ipv6 | ipboth]. <span class="li-normal">type: string </span> </li>
                
            </ul>
        
        </li>
        <li><span class="li-head">ips_anomaly</span> 
        
        </li>
        <li><span class="li-head">ips_metadata</span> 
        
        </li>
        <li><span class="li-head">ips_rate-based</span> 
        
        </li>
        <li><span class="li-head">license_fortianalyzer-status</span> 
        
        </li>
        <li><span class="li-head">license_forticare-org-list</span> 
        
        </li>
        <li><span class="li-head">license_forticare-resellers</span> - Get current FortiCare resellers for the requested country. 
        <ul class="ul-self">
                <li><span class="li-required">country_code</span> - FortiGuard country code <span class="li-normal">type: int </span> </li>
                
            </ul>
        
        </li>
        <li><span class="li-head">license_status</span> 
        
        </li>
        <li><span class="li-head">log_av-archive_download</span> - Download file quarantined by AntiVirus. 
        <ul class="ul-self">
                <li><span class="li-required">mkey</span> - Checksum for quarantined file. <span class="li-normal">type: string </span> </li>
                
            </ul>
        
        </li>
        <li><span class="li-head">log_current-disk-usage</span> 
        
        </li>
        <li><span class="li-head">log_device_state</span> 
        
        </li>
        <li><span class="li-head">log_event</span> 
        
        </li>
        <li><span class="li-head">log_fortianalyzer</span> - Return FortiAnalyzer/FortiManager log status. 
        <ul class="ul-self">
                <li><span class="li-required">srcip</span> - The IP to use to make the request to the FortiAnalyzer [<ip>|auto]. When set to "auto" it will use the FortiGate's routing table to determine the IP to make the request from. <span class="li-normal">type: string </span> </li>
                <li><span class="li-required">scope</span> - Scope from which to test the connectivity of the FortiAnalyzer address [vdom|global]. <span class="li-normal">type: string </span> </li>
                <li><span class="li-required">server</span> - FortiAnalyzer/FortiManager address. <span class="li-normal">type: string </span> </li>
                
            </ul>
        
        </li>
        <li><span class="li-head">log_fortianalyzer-queue</span> - Retrieve information on FortiAnalyzer's queue state. Note:- FortiAnalyzer logs are queued only if upload-option is realtime. 
        <ul class="ul-self">
                <li><span class="li-required">scope</span> - Scope from which to retrieve FortiAnalyzer's queue state [vdom*|global]. <span class="li-normal">type: string </span> </li>
                
            </ul>
        
        </li>
        <li><span class="li-head">log_forticloud</span> 
        
        </li>
        <li><span class="li-head">log_forticloud-report-list</span> 
        
        </li>
        <li><span class="li-head">log_forticloud-report_download</span> - Download PDF report from FortiCloud. 
        <ul class="ul-self">
                <li><span class="li-required">inline</span> - Set to 1 to download the report inline. <span class="li-normal">type: int </span> </li>
                <li><span class="li-required">mkey</span> - FortiCloud Report ID. <span class="li-normal">type: int </span> </li>
                
            </ul>
        
        </li>
        <li><span class="li-head">log_historic-daily-remote-logs</span> - Returns the amount of logs in bytes sent daily to a remote logging service (FortiCloud or FortiAnalyzer). 
        <ul class="ul-self">
                <li><span class="li-required">server</span> - Service name [forticloud | fortianalyzer]. <span class="li-normal">type: string </span> </li>
                
            </ul>
        
        </li>
        <li><span class="li-head">log_hourly-disk-usage</span> 
        
        </li>
        <li><span class="li-head">log_ips-archive_download</span> - Download IPS/application control packet capture files. Uses configured log display device. 
        <ul class="ul-self">
                <li><span class="li-required">pcap_no</span> - Packet capture roll number (required when log device is 'disk') <span class="li-normal">type: int </span> </li>
                <li><span class="li-required">pcap_category</span> - Packet capture category (required when log device is 'disk') <span class="li-normal">type: int </span> </li>
                <li><span class="li-required">mkey</span> - IPS archive ID. <span class="li-normal">type: int </span> </li>
                
            </ul>
        
        </li>
        <li><span class="li-head">log_local-report-list</span> 
        
        </li>
        <li><span class="li-head">log_local-report_download</span> - Download local report 
        <ul class="ul-self">
                <li><span class="li-required">mkey</span> - Local Report Name. <span class="li-normal">type: string </span> </li>
                
            </ul>
        
        </li>
        <li><span class="li-head">log_policy-archive_download</span> - Download policy-based packet capture archive. 
        <ul class="ul-self">
                <li><span class="li-required">srcip</span> - Source IP. <span class="li-normal">type: string </span> </li>
                <li><span class="li-required">dstip</span> - Destination IP. <span class="li-normal">type: string </span> </li>
                <li><span class="li-required">mkey</span> - Session ID (from traffic log). <span class="li-normal">type: int </span> </li>
                
            </ul>
        
        </li>
        <li><span class="li-head">log_stats</span> - Return number of logs sent by category per day for a specific log device. 
        <ul class="ul-self">
                <li><span class="li-required">dev</span> - Log device [*memory | disk | fortianalyzer | forticloud]. <span class="li-normal">type: string </span> </li>
                
            </ul>
        
        </li>
        <li><span class="li-head">network_ddns_lookup</span> - Check DDNS FQDN availability. 
        <ul class="ul-self">
                <li><span class="li-required">domain</span> - Filter: domain to check. <span class="li-normal">type: string </span> </li>
                
            </ul>
        
        </li>
        <li><span class="li-head">network_ddns_servers</span> 
        
        </li>
        <li><span class="li-head">network_dns_latency</span> 
        
        </li>
        <li><span class="li-head">network_fortiguard_live-services-latency</span> 
        
        </li>
        <li><span class="li-head">network_lldp_neighbors</span> 
        
        </li>
        <li><span class="li-head">network_lldp_ports</span> - List all active LLDP ports. 
        <ul class="ul-self">
                <li><span class="li-required">mkey</span> - Filter: specific port name. <span class="li-normal">type: string </span> </li>
                
            </ul>
        
        </li>
        <li><span class="li-head">network_reverse-ip-lookup</span> - Retrieve the resolved DNS domain name for a given IP address. 
        <ul class="ul-self">
                <li><span class="li-required">ip</span> - IP address (in dot-decimal notation). <span class="li-normal">type: string </span> </li>
                
            </ul>
        
        </li>
        <li><span class="li-head">nsx_instance</span> - List NSX instances and their resource statistics. 
        <ul class="ul-self">
                <li><span class="li-required">mkey</span> - Filter: NSX SDN name. <span class="li-normal">type: string </span> </li>
                
            </ul>
        
        </li>
        <li><span class="li-head">nsx_service_status</span> - Retrieve NSX service status. 
        <ul class="ul-self">
                <li><span class="li-required">mkey</span> - Filter: NSX SDN name. <span class="li-normal">type: string </span> </li>
                
            </ul>
        
        </li>
        <li><span class="li-head">registration_forticloud_device-status</span> - Fetch device registration status from FortiCloud. Currently FortiSwitch and FortiAP are supported. 
        <ul class="ul-self">
                <li><span class="li-required">serials</span> - Serials of FortiSwitch and FortiAP to fetch registration status. <span class="li-normal">type: array </span> </li>
                <li><span class="li-required">update_cache</span> - Clear cache and retrieve updated data. <span class="li-normal">type: array </span> </li>
                
            </ul>
        
        </li>
        <li><span class="li-head">registration_forticloud_disclaimer</span> 
        
        </li>
        <li><span class="li-head">registration_forticloud_domains</span> 
        
        </li>
        <li><span class="li-head">router_ipv4</span> - List all active IPv4 routing table entries. 
        <ul class="ul-self">
                <li><span class="li-required">count</span> - Maximum number of entries to return (Default for all routes). <span class="li-normal">type: int </span> </li>
                <li><span class="li-required">ip_mask</span> - Filter: IP/netmask. <span class="li-normal">type: string </span> </li>
                <li><span class="li-required">start</span> - Starting entry index. <span class="li-normal">type: int </span> </li>
                <li><span class="li-required">interface</span> - Filter: interface name. <span class="li-normal">type: string </span> </li>
                <li><span class="li-required">type</span> - Filter: route type. <span class="li-normal">type: string </span> </li>
                <li><span class="li-required">gateway</span> - Filter: gateway. <span class="li-normal">type: string </span> </li>
                
            </ul>
        
        </li>
        <li><span class="li-head">router_ipv6</span> - List all active IPv6 routing table entries. 
        <ul class="ul-self">
                <li><span class="li-required">count</span> - Maximum number of entries to return (Default for all routes). <span class="li-normal">type: int </span> </li>
                <li><span class="li-required">ip_mask</span> - Filter: IP/netmask. <span class="li-normal">type: string </span> </li>
                <li><span class="li-required">start</span> - Starting entry index. <span class="li-normal">type: int </span> </li>
                <li><span class="li-required">interface</span> - Filter: interface name. <span class="li-normal">type: string </span> </li>
                <li><span class="li-required">type</span> - Filter: route type. <span class="li-normal">type: string </span> </li>
                <li><span class="li-required">gateway</span> - Filter: gateway. <span class="li-normal">type: string </span> </li>
                
            </ul>
        
        </li>
        <li><span class="li-head">router_lookup</span> - Performs a route lookup by querying the routing table. 
        <ul class="ul-self">
                <li><span class="li-required">destination</span> - Destination IP/FQDN. <span class="li-normal">type: string </span> </li>
                <li><span class="li-required">ipv6</span> - Perform an IPv6 lookup. <span class="li-normal">type: boolean </span> </li>
                
            </ul>
        
        </li>
        <li><span class="li-head">router_lookup-policy</span> - Performs a route lookup by querying the policy routing table. 
        <ul class="ul-self">
                <li><span class="li-required">protocol_number</span> - IP Protocol Number. <span class="li-normal">type: int </span> </li>
                <li><span class="li-required">destination</span> - Destination IP/FQDN. <span class="li-normal">type: string </span> </li>
                <li><span class="li-required">source</span> - Source IP/FQDN. <span class="li-normal">type: string </span> </li>
                <li><span class="li-required">ipv6</span> - Perform an IPv6 lookup. <span class="li-normal">type: boolean </span> </li>
                <li><span class="li-required">destination_port</span> - Destination Port. <span class="li-normal">type: int </span> </li>
                <li><span class="li-required">interface_name</span> - Incoming Interface. <span class="li-normal">type: string </span> </li>
                
            </ul>
        
        </li>
        <li><span class="li-head">router_policy</span> - Retrieve a list of active IPv4 policy routes. 
        <ul class="ul-self">
                <li><span class="li-required">count</span> - Maximum number of entries to return. <span class="li-normal">type: int </span> </li>
                <li><span class="li-required">start</span> - Starting entry index. <span class="li-normal">type: int </span> </li>
                <li><span class="li-required">count_only</span> - Returns the number of IPv4 policy routes only. <span class="li-normal">type: boolean </span> </li>
                
            </ul>
        
        </li>
        <li><span class="li-head">router_policy6</span> - Retrieve a list of active IPv6 policy routes. 
        <ul class="ul-self">
                <li><span class="li-required">count</span> - Maximum number of entries to return. <span class="li-normal">type: int </span> </li>
                <li><span class="li-required">start</span> - Starting entry index. <span class="li-normal">type: int </span> </li>
                <li><span class="li-required">count_only</span> - Returns the number of IPv6 policy routes only. <span class="li-normal">type: boolean </span> </li>
                
            </ul>
        
        </li>
        <li><span class="li-head">router_statistics</span> - Retrieve routing table statistics, including number of matched routes. 
        <ul class="ul-self">
                <li><span class="li-required">ip_version</span> - IP version (4|6). If not present, IPv4 and IPv6 will be returned. <span class="li-normal">type: int </span> </li>
                <li><span class="li-required">ip_mask</span> - Filter: IP/netmask. <span class="li-normal">type: string </span> </li>
                <li><span class="li-required">interface</span> - Filter: interface name. <span class="li-normal">type: string </span> </li>
                <li><span class="li-required">type</span> - Filter: route type. <span class="li-normal">type: string </span> </li>
                <li><span class="li-required">gateway</span> - Filter: gateway. <span class="li-normal">type: string </span> </li>
                
            </ul>
        
        </li>
        <li><span class="li-head">switch-controller_detected-device</span> 
        
        </li>
        <li><span class="li-head">switch-controller_fsw-firmware</span> - Retrieve a list of recommended firmware for managed FortiSwitches. 
        <ul class="ul-self">
                <li><span class="li-required">timeout</span> - FortiGuard connection timeout (defaults to 3 seconds). <span class="li-normal">type: string </span> </li>
                <li><span class="li-required">mkey</span> - Filter: FortiSwitch ID. <span class="li-normal">type: string </span> </li>
                
            </ul>
        
        </li>
        <li><span class="li-head">switch-controller_managed-switch</span> - Retrieve statistics for configured FortiSwitches 
        <ul class="ul-self">
                <li><span class="li-required">fsw_id</span> - DEPRECATED since 5.6.1, will be removed in 6.4. Please use mkey instead. <span class="li-normal">type: string </span> </li>
                <li><span class="li-required">port_stats</span> - Filter: Retrieve tx/rx statistics for ports of configured FortiSwitches. <span class="li-normal">type: boolean </span> </li>
                <li><span class="li-required">stp_status</span> - Filter: Retrieve STP status for ports of configured FortiSwitches. <span class="li-normal">type: boolean </span> </li>
                <li><span class="li-required">igmp_snooping_group</span> - Filter: Retrieve IGMP Snooping group for configured FortiSwitches. <span class="li-normal">type: boolean </span> </li>
                <li><span class="li-required">qos_stats</span> - Filter: Retrieve QoS statistics for ports of configured FortiSwitches. <span class="li-normal">type: boolean </span> </li>
                <li><span class="li-required">transceiver</span> - Filter: Retrieve transceiver information for ports of configured FortiSwitches. <span class="li-normal">type: boolean </span> </li>
                <li><span class="li-required">poe</span> - Filter: Retrieve PoE statistics for ports of configured FortiSwitches. Port power usage is in Watt units. <span class="li-normal">type: boolean </span> </li>
                <li><span class="li-required">mkey</span> - Filter: FortiSwitch ID. <span class="li-normal">type: string </span> </li>
                
            </ul>
        
        </li>
        <li><span class="li-head">switch-controller_managed-switch_dhcp-snooping</span> 
        
        </li>
        <li><span class="li-head">switch-controller_managed-switch_faceplate-xml</span> - Retrieve XML for rendering FortiSwitch faceplate widget. 
        <ul class="ul-self">
                <li><span class="li-required">mkey</span> - Name of managed FortiSwitch. <span class="li-normal">type: string </span> </li>
                
            </ul>
        
        </li>
        <li><span class="li-head">switch-controller_managed-switch_transceivers</span> 
        
        </li>
        <li><span class="li-head">switch-controller_validate-switch-prefix</span> - Validate a FortiSwitch serial number prefix. 
        <ul class="ul-self">
                <li><span class="li-required">prefix</span> - Prefix of FortiSwitch serial number. <span class="li-normal">type: string </span> </li>
                
            </ul>
        
        </li>
        <li><span class="li-head">system_3g-modem</span> 
        
        </li>
        <li><span class="li-head">system_acquired-dns</span> 
        
        </li>
        <li><span class="li-head">system_automation-stitch_stats</span> - Stats for automation stitches. 
        <ul class="ul-self">
                <li><span class="li-required">mkey</span> - Filter: Automation stitch name. <span class="li-normal">type: string </span> </li>
                
            </ul>
        
        </li>
        <li><span class="li-head">system_available-certificates</span> - Get available certificates. 
        <ul class="ul-self">
                <li><span class="li-required">scope</span> - Scope of certificate [vdom*|global]. <span class="li-normal">type: string </span> </li>
                <li><span class="li-required">with_remote</span> - Include remote certificates. <span class="li-normal">type: boolean </span> </li>
                <li><span class="li-required">with_ca</span> - Include certificate authorities. <span class="li-normal">type: boolean </span> </li>
                <li><span class="li-required">with_crl</span> - Include certificate revocation lists. <span class="li-normal">type: boolean </span> </li>
                
            </ul>
        
        </li>
        <li><span class="li-head">system_available-interfaces</span> - Retrieve a list of all interfaces along with some meta information regarding their availability. 
        <ul class="ul-self">
                <li><span class="li-required">scope</span> - Scope of interface list [vdom|global] <span class="li-normal">type: string </span> </li>
                <li><span class="li-required">view_type</span> - Optionally include additional information for interfaces. This parameter can be repeated multiple times. 'poe': Includes PoE information for supported ports (DEPRECATED in 6.4). 'ha': Includes extra meta information useful when dealing with interfaces related to HA configuration. Interfaces that are used by an HA cluster as management interfaces are also included in this view. 'zone': Includes extra meta information for determining zone membership eligibility. 'vwp': Includes extra meta information for determining virtual wire pair eligibility. 'sdwan': Includes extra meta information for determining SD-WAN eligibility. 'switch': Includes extra meta information for determining switch eligibility. 'hard-switch': Includes extra meta information for determining hard-switch eligibility. 'limited': Includes limited information on parent interfaces that are in another VDOM.  <span class="li-normal">type: string </span> </li>
                
            </ul>
        
        </li>
        <li><span class="li-head">system_botnet</span> - List all known IP-based botnet entries in FortiGuard botnet database. 
        <ul class="ul-self">
                <li><span class="li-required">count</span> - Maximum number of entries to return. <span class="li-normal">type: int </span> </li>
                <li><span class="li-required">start</span> - Starting entry index. <span class="li-normal">type: int </span> </li>
                <li><span class="li-required">include_hit_only</span> - Include entries with hits only. <span class="li-normal">type: boolean </span> </li>
                
            </ul>
        
        </li>
        <li><span class="li-head">system_botnet-domains</span> - List all known domain-based botnet entries in FortiGuard botnet database. 
        <ul class="ul-self">
                <li><span class="li-required">count</span> - Maximum number of entries to return. <span class="li-normal">type: int </span> </li>
                <li><span class="li-required">start</span> - Starting entry index. <span class="li-normal">type: int </span> </li>
                
            </ul>
        
        </li>
        <li><span class="li-head">system_botnet-domains_hits</span> 
        
        </li>
        <li><span class="li-head">system_botnet-domains_stat</span> 
        
        </li>
        <li><span class="li-head">system_botnet_stat</span> 
        
        </li>
        <li><span class="li-head">system_certificate_download</span> - Download certificate. 
        <ul class="ul-self">
                <li><span class="li-required">scope</span> - Scope of certificate [vdom*|global]. <span class="li-normal">type: string </span> </li>
                <li><span class="li-required">type</span> - Type of certificate [local-cer|remote-cer|local-ca|remote-ca|local-csr|crl]. <span class="li-normal">type: string </span> </li>
                <li><span class="li-required">mkey</span> - Name of certificate. <span class="li-normal">type: string </span> </li>
                
            </ul>
        
        </li>
        <li><span class="li-head">system_check-port-availability</span> - Check whether a list of TCP port ranges is available for a certain service. 
        <ul class="ul-self">
                <li><span class="li-required">port_ranges</span> - List of TCP port range objects to check against. <span class="li-normal">type: array </span> </li>
                <li><span class="li-required">service</span> - The service in which the ports could be available. 'service' options are [reserved | sysglobal | webproxy | ftpproxy | sslvpn | slaprobe | fsso | ftm_push]. If 'service' is not specified, the port ranges availability is checked against all services. <span class="li-normal">type: string </span> </li>
                
            </ul>
        
        </li>
        <li><span class="li-head">system_com-log_download</span> 
        
        </li>
        <li><span class="li-head">system_com-log_update</span> 
        
        </li>
        <li><span class="li-head">system_config-revision</span> 
        
        </li>
        <li><span class="li-head">system_config-revision_file</span> - Download a specific configuration revision. 
        <ul class="ul-self">
                <li><span class="li-required">config_id</span> - Configuration id. <span class="li-normal">type: int </span> </li>
                
            </ul>
        
        </li>
        <li><span class="li-head">system_config-revision_info</span> - Retrieve meta information for a specific configuration revision. 
        <ul class="ul-self">
                <li><span class="li-required">config_id</span> - Configuration id. <span class="li-normal">type: int </span> </li>
                
            </ul>
        
        </li>
        <li><span class="li-head">system_config-script</span> 
        
        </li>
        <li><span class="li-head">system_config-sync_status</span> 
        
        </li>
        <li><span class="li-head">system_config_backup</span> - Backup system config 
        <ul class="ul-self">
                <li><span class="li-required">password</span> - Password to encrypt configuration data. <span class="li-normal">type: string </span> </li>
                <li><span class="li-required">usb_filename</span> - When using 'usb' destination: the filename to save to on the connected USB device <span class="li-normal">type: string </span> </li>
                <li><span class="li-required">destination</span> - Configuration file destination [file* | usb] <span class="li-normal">type: string </span> </li>
                <li><span class="li-required">vdom</span> - If 'vdom' scope specified, the name of the VDOM to backup configuration. <span class="li-normal">type: string </span> </li>
                <li><span class="li-required">scope</span> - Specify global or VDOM only backup [global | vdom]. <span class="li-normal">type: string </span> </li>
                
            </ul>
        
        </li>
        <li><span class="li-head">system_config_usb-filelist</span> 
        
        </li>
        <li><span class="li-head">system_csf</span> - Retrieve a full tree of downstream FortiGates registered to the Security Fabric. 
        <ul class="ul-self">
                <li><span class="li-required">scope</span> - Scope from which to retrieve the Security Fabric tree [vdom*|global]. <span class="li-normal">type: string </span> </li>
                
            </ul>
        
        </li>
        <li><span class="li-head">system_csf_pending-authorizations</span> 
        
        </li>
        <li><span class="li-head">system_current-admins</span> 
        
        </li>
        <li><span class="li-head">system_debug_download</span> 
        
        </li>
        <li><span class="li-head">system_dhcp</span> - List all DHCP and DHCPv6 leases. 
        <ul class="ul-self">
                <li><span class="li-required">interface</span> - Filter: Retrieve DHCP leases for this interface only. <span class="li-normal">type: string </span> </li>
                <li><span class="li-required">scope</span> - Scope from which to retrieve DHCP leases [vdom*|global]. Global scope is only accessible for global administrators. <span class="li-normal">type: string </span> </li>
                <li><span class="li-required">ipv6</span> - Include IPv6 addresses in the response. <span class="li-normal">type: boolean </span> </li>
                
            </ul>
        
        </li>
        <li><span class="li-head">system_firmware</span> 
        
        </li>
        <li><span class="li-head">system_firmware_upgrade-paths</span> 
        
        </li>
        <li><span class="li-head">system_fortiguard_server-info</span> 
        
        </li>
        <li><span class="li-head">system_fortimanager_backup-details</span> - Get the properties of a FortiManager object. 
        <ul class="ul-self">
                <li><span class="li-required">datasource</span> - Object datasource. <span class="li-normal">type: string </span> </li>
                <li><span class="li-required">mkey</span> - Object name. <span class="li-normal">type: string </span> </li>
                
            </ul>
        
        </li>
        <li><span class="li-head">system_fortimanager_backup-summary</span> 
        
        </li>
        <li><span class="li-head">system_fortimanager_status</span> 
        
        </li>
        <li><span class="li-head">system_global-resources</span> 
        
        </li>
        <li><span class="li-head">system_ha-checksums</span> 
        
        </li>
        <li><span class="li-head">system_ha-history</span> 
        
        </li>
        <li><span class="li-head">system_ha-peer</span> - Get configuration of peer(s) in HA cluster. Uptime is expressed in seconds. 
        <ul class="ul-self">
                <li><span class="li-required">serial_no</span> - Serial number of the HA member. If not specified, fetch information for all HA members <span class="li-normal">type: string </span> </li>
                <li><span class="li-required">vcluster_id</span> - Virtual cluster number. If not specified, fetch information for all active vclusters <span class="li-normal">type: int </span> </li>
                
            </ul>
        
        </li>
        <li><span class="li-head">system_ha-statistics</span> 
        
        </li>
        <li><span class="li-head">system_interface</span> - Retrieve statistics for all system interfaces. 
        <ul class="ul-self">
                <li><span class="li-required">scope</span> - Scope from which to retrieve the interface stats from [vdom|global]. <span class="li-normal">type: string </span> </li>
                <li><span class="li-required">interface_name</span> - Filter: interface name. <span class="li-normal">type: string </span> </li>
                <li><span class="li-required">include_vlan</span> - Enable to include VLANs in result list. <span class="li-normal">type: boolean </span> </li>
                <li><span class="li-required">include_aggregate</span> - Enable to include Aggregate interfaces in result list. <span class="li-normal">type: boolean </span> </li>
                
            </ul>
        
        </li>
        <li><span class="li-head">system_interface_dhcp-status</span> - Retrieve the DHCP client status of an interface. 
        <ul class="ul-self">
                <li><span class="li-required">mkey</span> - Name of the interface. <span class="li-normal">type: string </span> </li>
                
            </ul>
        
        </li>
        <li><span class="li-head">system_interface_poe</span> - Retrieve PoE statistics for system interfaces. 
        <ul class="ul-self">
                <li><span class="li-required">scope</span> - Scope from which to retrieve the interface stats from [vdom|global] (default=vdom). <span class="li-normal">type: string </span> </li>
                <li><span class="li-required">mkey</span> - Filter: Name of the interface to fetch PoE statistics for. <span class="li-normal">type: string </span> </li>
                
            </ul>
        
        </li>
        <li><span class="li-head">system_interface_speed-test-status</span> - Retrieve the current status of a speed-test with the results if finished. 
        <ul class="ul-self">
                <li><span class="li-required">id</span> - ID of the speed test. <span class="li-normal">type: int </span> </li>
                
            </ul>
        
        </li>
        <li><span class="li-head">system_interface_transceivers</span> - Get a list of transceivers being used by the FortiGate. 
        <ul class="ul-self">
                <li><span class="li-required">scope</span> - Scope from which to retrieve the transceiver information from [vdom|global]. <span class="li-normal">type: string </span> </li>
                
            </ul>
        
        </li>
        <li><span class="li-head">system_ipconf</span> - Determine if there is an IP conflict for a specific IP using ARP. 
        <ul class="ul-self">
                <li><span class="li-required">devs</span> - List of interfaces to check for conflict. <span class="li-normal">type: array </span> </li>
                <li><span class="li-required">ipaddr</span> - IPv4 address to check for conflict. <span class="li-normal">type: string </span> </li>
                
            </ul>
        
        </li>
        <li><span class="li-head">system_link-monitor</span> - Retrieve per-interface statistics for active link monitors. 
        <ul class="ul-self">
                <li><span class="li-required">mkey</span> - Name of link monitor. <span class="li-normal">type: string </span> </li>
                
            </ul>
        
        </li>
        <li><span class="li-head">system_modem</span> 
        
        </li>
        <li><span class="li-head">system_nat46-ippools</span> 
        
        </li>
        <li><span class="li-head">system_object_usage</span> - Retrieve all objects that are currently using as well as objects that can use the given object. 
        <ul class="ul-self">
                <li><span class="li-required">scope</span> - Scope of resource [vdom|global]. <span class="li-normal">type: string </span> </li>
                <li><span class="li-required">q_name</span> - The CMDB table's name <span class="li-normal">type: string </span> </li>
                <li><span class="li-required">mkey</span> - The mkey for the object <span class="li-normal">type: string </span> </li>
                <li><span class="li-required">qtypes</span> - List of CMDB table qTypes <span class="li-normal">type: array </span> </li>
                <li><span class="li-required">q_path</span> - The CMDB table's path <span class="li-normal">type: string </span> </li>
                
            </ul>
        
        </li>
        <li><span class="li-head">system_resolve-fqdn</span> - Resolves the provided FQDNs to FQDN -> IP mappings. 
        <ul class="ul-self">
                <li><span class="li-required">fqdn</span> - List of FQDNs to be resolved <span class="li-normal">type: array </span> </li>
                <li><span class="li-required">ipv6</span> - Resolve for the AAAA record? <span class="li-normal">type: boolean </span> </li>
                
            </ul>
        
        </li>
        <li><span class="li-head">system_resource_usage</span> - Retreive current and historical usage data for a provided resource. 
        <ul class="ul-self">
                <li><span class="li-required">scope</span> - Scope of resource [vdom|global]. This parameter is only applicable if the FGT is in VDOM mode. <span class="li-normal">type: string </span> </li>
                <li><span class="li-required">interval</span> - Time interval of resource usage [1-min|10-min|30-min|1-hour|12-hour|24-hour]. Defaults to all intervals if not provided. <span class="li-normal">type: string </span> </li>
                <li><span class="li-required">resource</span> - Resource to get usage data for [cpu|mem|disk|session|session6|setuprate|setuprate6|disk_lograte|faz_lograte|forticloud_lograte]. Defaults to all resources if not provided. Additionally, [npu_session|npu_session6] data is available for devices that have an NPU and [nturbo_session|nturbo_session6] data is available for NP6 devices that support NTurbo. <span class="li-normal">type: string </span> </li>
                
            </ul>
        
        </li>
        <li><span class="li-head">system_sandbox_cloud-regions</span> 
        
        </li>
        <li><span class="li-head">system_sandbox_stats</span> 
        
        </li>
        <li><span class="li-head">system_sandbox_status</span> 
        
        </li>
        <li><span class="li-head">system_sandbox_test-connect</span> - Test the connectivity of a given FortiSandbox IP. 
        <ul class="ul-self">
                <li><span class="li-required">server</span> - IP of the FortiSandbox to test. <span class="li-normal">type: string </span> </li>
                
            </ul>
        
        </li>
        <li><span class="li-head">system_sdn-connector_nsx-security-tags</span> - Retrieve a list of NSX security tags for connected NSX servers. 
        <ul class="ul-self">
                <li><span class="li-required">mkey</span> - Filter: NSX SDN connector name. <span class="li-normal">type: string </span> </li>
                
            </ul>
        
        </li>
        <li><span class="li-head">system_sdn-connector_status</span> - Retrieve connection status for SDN connectors. 
        <ul class="ul-self">
                <li><span class="li-required">type</span> - Filter: SDN connector type. Ignored if mkey is specified. <span class="li-normal">type: string </span> </li>
                <li><span class="li-required">mkey</span> - Filter: SDN connector name. <span class="li-normal">type: string </span> </li>
                
            </ul>
        
        </li>
        <li><span class="li-head">system_security-rating</span> - Retrieve a Security Rating report result. Without ID specified, returns the most recent result. 
        <ul class="ul-self">
                <li><span class="li-required">scope</span> - Scope of the report [vdom*|global]. Global scope is only accessible for global administrators. <span class="li-normal">type: string </span> </li>
                <li><span class="li-required">id</span> - Report ID. <span class="li-normal">type: int </span> </li>
                <li><span class="li-required">report_type</span> - Report type to view, Security Report when unspecified. <span class="li-normal">type: string </span> </li>
                
            </ul>
        
        </li>
        <li><span class="li-head">system_security-rating_history</span> - Retrieve Security Rating history. 
        <ul class="ul-self">
                <li><span class="li-required">report_type</span> - Security Rating report history to view, view Security Report when unspecified. <span class="li-normal">type: string </span> </li>
                
            </ul>
        
        </li>
        <li><span class="li-head">system_security-rating_lang</span> - Returns the requested Security Rating language mapping. 
        <ul class="ul-self">
                <li><span class="li-required">key</span> - Requested language mapping (en, fr, big5, euc-kr, GB2312, pg, sp, x-sjis). <span class="li-normal">type: string </span> </li>
                
            </ul>
        
        </li>
        <li><span class="li-head">system_security-rating_status</span> - Check if a Security Rating report is currently running. 
        <ul class="ul-self">
                <li><span class="li-required">progress</span> - Query report progress. <span class="li-normal">type: boolean </span> </li>
                <li><span class="li-required">id</span> - Report ID. <span class="li-normal">type: int </span> </li>
                <li><span class="li-required">report_type</span> - Report type to view, Security Report when unspecified. <span class="li-normal">type: string </span> </li>
                
            </ul>
        
        </li>
        <li><span class="li-head">system_security-rating_supported-reports</span> 
        
        </li>
        <li><span class="li-head">system_sensor-info</span> 
        
        </li>
        <li><span class="li-head">system_sniffer</span> 
        
        </li>
        <li><span class="li-head">system_sniffer_download</span> - Download a stored packet capture. 
        <ul class="ul-self">
                <li><span class="li-required">mkey</span> - ID of packet capture entry. <span class="li-normal">type: int </span> </li>
                
            </ul>
        
        </li>
        <li><span class="li-head">system_status</span> 
        
        </li>
        <li><span class="li-head">system_storage</span> 
        
        </li>
        <li><span class="li-head">system_time</span> 
        
        </li>
        <li><span class="li-head">system_timezone</span> 
        
        </li>
        <li><span class="li-head">system_trusted-cert-authorities</span> - Get trusted certifiate authorities. 
        <ul class="ul-self">
                <li><span class="li-required">scope</span> - Scope of certificate [vdom*|global]. <span class="li-normal">type: string </span> </li>
                
            </ul>
        
        </li>
        <li><span class="li-head">system_usb-log</span> 
        
        </li>
        <li><span class="li-head">system_vdom-link</span> - Gets a list of all NPU VDOM Links and VDOM Links. 
        <ul class="ul-self">
                <li><span class="li-required">scope</span> - Scope from which to retrieve the VDOM link informaton from [vdom|global]. <span class="li-normal">type: string </span> </li>
                
            </ul>
        
        </li>
        <li><span class="li-head">system_vdom-resource</span> 
        
        </li>
        <li><span class="li-head">system_vm-information</span> 
        
        </li>
        <li><span class="li-head">user_banned</span> 
        
        </li>
        <li><span class="li-head">user_collected-email</span> - List email addresses collected from captive portal 
        <ul class="ul-self">
                <li><span class="li-required">ipv6</span> - Include collected email from IPv6 users. <span class="li-normal">type: boolean </span> </li>
                
            </ul>
        
        </li>
        <li><span class="li-head">user_detected-device</span> - Retrieve a list of detected devices. 
        <ul class="ul-self">
                <li><span class="li-required">with_fortiap</span> - Retrieve FortiAP information. <span class="li-normal">type: boolean </span> </li>
                <li><span class="li-required">with_user</span> - Retrieve authenticated user information. <span class="li-normal">type: boolean </span> </li>
                <li><span class="li-required">with_endpoint</span> - Retrieve FortiClient endpoint information. <span class="li-normal">type: boolean </span> </li>
                <li><span class="li-required">with_dhcp</span> - Retrieve DHCP lease information. <span class="li-normal">type: boolean </span> </li>
                <li><span class="li-required">expand_child_macs</span> - Include child devices as separate entries in the list. <span class="li-normal">type: boolean </span> </li>
                <li><span class="li-required">with_fortilink</span> - Retrieve FortiLink information. <span class="li-normal">type: boolean </span> </li>
                
            </ul>
        
        </li>
        <li><span class="li-head">user_device</span> - Retrieve a list of detected devices. 
        <ul class="ul-self">
                <li><span class="li-required">master_mac</span> - Filter: Master MAC of a device. Multiple entries could be returned. <span class="li-normal">type: string </span> </li>
                <li><span class="li-required">master_only</span> - List of master device only. <span class="li-normal">type: boolean </span> </li>
                
            </ul>
        
        </li>
        <li><span class="li-head">user_firewall</span> - List authenticated firewall users. 
        <ul class="ul-self">
                <li><span class="li-required">count</span> - Maximum number of entries to return. <span class="li-normal">type: int </span> </li>
                <li><span class="li-required">start</span> - Starting entry index. <span class="li-normal">type: int </span> </li>
                <li><span class="li-required">ipv4</span> - Include IPv4 user (default=true). <span class="li-normal">type: boolean </span> </li>
                <li><span class="li-required">ipv6</span> - Include IPv6 users. <span class="li-normal">type: boolean </span> </li>
                
            </ul>
        
        </li>
        <li><span class="li-head">user_fortitoken</span> 
        
        </li>
        <li><span class="li-head">user_fsso</span> - Get a list of fsso and fsso polling status. 
        <ul class="ul-self">
                <li><span class="li-required">type</span> - Filter: Get the status for this type of FSSO entry [fsso|fsso-polling]. <span class="li-normal">type: string </span> </li>
                <li><span class="li-required">mkey</span> - Filter: Get the status for a specific FSSO entry. `type` is required if this is set. <span class="li-normal">type: string </span> </li>
                
            </ul>
        
        </li>
        <li><span class="li-head">user_info_query</span> - Query user info. 
        <ul class="ul-self">
                <li><span class="li-required">keys</span> - A list of keys to be returned. Omit to return all keys. Type: string <span class="li-normal">type: array </span> </li>
                <li><span class="li-required">start</span> - Number of entries to skip from the beginning. <span class="li-normal">type: int </span> </li>
                <li><span class="li-required">number</span> - Maximum number of entries to return. <span class="li-normal">type: int </span> </li>
                <li><span class="li-required">filters</span> - A list of filters. Type: {"type": string, "value": string} <span class="li-normal">type: array </span> </li>
                
            </ul>
        
        </li>
        <li><span class="li-head">user_info_thumbnail</span> - Get user info thumbnail. Returns the first match to the filter. 
        <ul class="ul-self">
                <li><span class="li-required">filters</span> - A list of filters. Type: {"type": string, "value": string} <span class="li-normal">type: array </span> </li>
                
            </ul>
        
        </li>
        <li><span class="li-head">utm_antivirus_stats</span> 
        
        </li>
        <li><span class="li-head">utm_app-lookup</span> - Query remote FortiFlow database to resolve hosts to application control entries. 
        <ul class="ul-self">
                <li><span class="li-required">hosts</span> - List of hosts to resolve. <span class="li-normal">type: array </span> </li>
                
            </ul>
        
        </li>
        <li><span class="li-head">utm_application-categories</span> 
        
        </li>
        <li><span class="li-head">utm_blacklisted-certificates</span> - Retrieve a list of blacklisted SSL certificates. 
        <ul class="ul-self">
                <li><span class="li-required">count</span> - Maximum number of entries to return. Limit is set to 2000. <span class="li-normal">type: int </span> </li>
                <li><span class="li-required">start</span> - Starting entry index. <span class="li-normal">type: int </span> </li>
                
            </ul>
        
        </li>
        <li><span class="li-head">utm_blacklisted-certificates_statistics</span> 
        
        </li>
        <li><span class="li-head">virtual-wan_health-check</span> 
        
        </li>
        <li><span class="li-head">virtual-wan_interface-log</span> - Retrieve log of SD-WAN interface quality information. 
        <ul class="ul-self">
                <li><span class="li-required">interface</span> - Filter: Interface name. <span class="li-normal">type: string </span> </li>
                <li><span class="li-required">seconds</span> - Filter: Only return SLA logs generated in the last N seconds. <span class="li-normal">type: int </span> </li>
                <li><span class="li-required">since</span> - Filter: Only return SLA logs generated since this Unix timestamp. <span class="li-normal">type: int </span> </li>
                
            </ul>
        
        </li>
        <li><span class="li-head">virtual-wan_members</span> 
        
        </li>
        <li><span class="li-head">virtual-wan_sla-log</span> - Retrieve log of SLA probe results for for each SD-WAN SLA rule. 
        <ul class="ul-self">
                <li><span class="li-required">interface</span> - Filter: Interface name. <span class="li-normal">type: string </span> </li>
                <li><span class="li-required">seconds</span> - Filter: Only return SLA logs generated in the last N seconds. <span class="li-normal">type: int </span> </li>
                <li><span class="li-required">since</span> - Filter: Only return SLA logs generated since this Unix timestamp. <span class="li-normal">type: int </span> </li>
                <li><span class="li-required">sla</span> - Filter: SLA name. <span class="li-normal">type: string </span> </li>
                
            </ul>
        
        </li>
        <li><span class="li-head">vpn_ipsec</span> - Return an array of active IPsec VPNs. 
        <ul class="ul-self">
                <li><span class="li-required">tunnel</span> - Filter for a specific IPsec tunnel name. <span class="li-normal">type: string </span> </li>
                <li><span class="li-required">start</span> - Starting entry index. <span class="li-normal">type: int </span> </li>
                <li><span class="li-required">count</span> - Maximum number of entries to return. <span class="li-normal">type: int </span> </li>
                
            </ul>
        
        </li>
        <li><span class="li-head">vpn_ocvpn_members</span> 
        
        </li>
        <li><span class="li-head">vpn_ocvpn_meta</span> 
        
        </li>
        <li><span class="li-head">vpn_ocvpn_status</span> 
        
        </li>
        <li><span class="li-head">vpn_ssl</span> 
        
        </li>
        <li><span class="li-head">vpn_ssl_stats</span> 
        
        </li>
        <li><span class="li-head">wanopt_history</span> - Retrieve WAN opt. statistics history. 
        <ul class="ul-self">
                <li><span class="li-required">period</span> - Statistics period [10-min*|hour|day|week|30-day]. <span class="li-normal">type: string </span> </li>
                
            </ul>
        
        </li>
        <li><span class="li-head">wanopt_peer_stats</span> 
        
        </li>
        <li><span class="li-head">wanopt_webcache</span> - Retrieve webcache statistics history. 
        <ul class="ul-self">
                <li><span class="li-required">period</span> - Statistics period [10-min*|hour|day|week|30-day]. <span class="li-normal">type: string </span> </li>
                
            </ul>
        
        </li>
        <li><span class="li-head">web-ui_custom-language_download</span> - Download a custom language file. 
        <ul class="ul-self">
                <li><span class="li-required">filename</span> - Name of custom language entry. <span class="li-normal">type: string </span> </li>
                
            </ul>
        
        </li>
        <li><span class="li-head">webcache_stats</span> - Retrieve webcache statistics. 
        <ul class="ul-self">
                <li><span class="li-required">period</span> - Statistics period [10min|hour|day|month]. <span class="li-normal">type: string </span> </li>
                
            </ul>
        
        </li>
        <li><span class="li-head">webfilter_category-quota</span> - Retrieve quota usage statistics for webfilter categories. 
        <ul class="ul-self">
                <li><span class="li-required">profile</span> - Webfilter profile. <span class="li-normal">type: string </span> </li>
                <li><span class="li-required">user</span> - User or IP (required if profile specified). <span class="li-normal">type: string </span> </li>
                
            </ul>
        
        </li>
        <li><span class="li-head">webfilter_fortiguard-categories</span> - Return FortiGuard web filter categories. 
        <ul class="ul-self">
                <li><span class="li-required">convert_unrated_id</span> - Convert Unrated category id to the one for CLI use. <span class="li-normal">type: boolean </span> </li>
                <li><span class="li-required">include_unrated</span> - Include Unrated category in result list. <span class="li-normal">type: boolean </span> </li>
                
            </ul>
        
        </li>
        <li><span class="li-head">webfilter_malicious-urls</span> 
        
        </li>
        <li><span class="li-head">webfilter_malicious-urls_stat</span> 
        
        </li>
        <li><span class="li-head">webfilter_override</span> 
        
        </li>
        <li><span class="li-head">webfilter_trusted-urls</span> 
        
        </li>
        <li><span class="li-head">webproxy_pacfile_download</span> 
        
        </li>
        <li><span class="li-head">wifi_ap_status</span> 
        
        </li>
        <li><span class="li-head">wifi_client</span> - Retrieve a list of connected WiFi clients. 
        <ul class="ul-self">
                <li><span class="li-required">count</span> - Maximum number of entries to return. <span class="li-normal">type: int </span> </li>
                <li><span class="li-required">start</span> - Starting entry index. <span class="li-normal">type: int </span> </li>
                <li><span class="li-required">type</span> - Request type [all*|fail-login]. <span class="li-normal">type: string </span> </li>
                
            </ul>
        
        </li>
        <li><span class="li-head">wifi_euclid</span> 
        
        </li>
        <li><span class="li-head">wifi_firmware</span> - Retrieve a list of current and recommended firmware for FortiAPs in use. 
        <ul class="ul-self">
                <li><span class="li-required">timeout</span> - FortiGuard connection timeout (defaults to 2 seconds). <span class="li-normal">type: string </span> </li>
                
            </ul>
        
        </li>
        <li><span class="li-head">wifi_interfering_ap</span> - Retrieve a list of interfering APs for one FortiAP radio. 
        <ul class="ul-self">
                <li><span class="li-required">wtp</span> - FortiAP ID to query. <span class="li-normal">type: string </span> </li>
                <li><span class="li-required">start</span> - Starting entry index. <span class="li-normal">type: int </span> </li>
                <li><span class="li-required">radio</span> - Radio ID. <span class="li-normal">type: int </span> </li>
                <li><span class="li-required">count</span> - Maximum number of entries to return. <span class="li-normal">type: int </span> </li>
                
            </ul>
        
        </li>
        <li><span class="li-head">wifi_managed_ap</span> - Retrieve a list of managed FortiAPs. 
        <ul class="ul-self">
                <li><span class="li-required">incl_local</span> - Enable to include the local FortiWiFi device in the results. <span class="li-normal">type: boolean </span> </li>
                <li><span class="li-required">wtp_id</span> - Filter: single managed FortiAP by ID. <span class="li-normal">type: string </span> </li>
                
            </ul>
        
        </li>
        <li><span class="li-head">wifi_network_list</span> 
        
        </li>
        <li><span class="li-head">wifi_network_status</span> 
        
        </li>
        <li><span class="li-head">wifi_region-image</span> - Retrieves a floorplan/region image from a configured FortiAP region. 
        <ul class="ul-self">
                <li><span class="li-required">region_name</span> - Region name to retrieve image from. <span class="li-normal">type: string </span> </li>
                
            </ul>
        
        </li>
        <li><span class="li-head">wifi_rogue_ap</span> - Retrieve a list of detected rogue APs. 
        <ul class="ul-self">
                <li><span class="li-required">count</span> - Maximum number of entries to return. <span class="li-normal">type: int </span> </li>
                <li><span class="li-required">start</span> - Starting entry index. <span class="li-normal">type: int </span> </li>
                
            </ul>
        
        </li>
        <li><span class="li-head">wifi_spectrum</span> - Retrieve spectrum analysis information for a specific FortiAP. 
        <ul class="ul-self">
                <li><span class="li-required">wtp_id</span> - FortiAP ID to query. <span class="li-normal">type: string </span> </li>
                
            </ul>
        
        </li>
        <li><span class="li-head">wifi_vlan-probe</span> - Retrieve the VLAN probe results. 
        <ul class="ul-self">
                <li><span class="li-required">wtp</span> - FortiAP ID. <span class="li-normal">type: string </span> </li>
                <li><span class="li-required">ap_interface</span> - FortiAP interface to send the probe on. <span class="li-normal">type: int </span> </li>
                
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