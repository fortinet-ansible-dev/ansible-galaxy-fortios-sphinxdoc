:source: fortios_monitor.py

:orphan:

.. :

fortios_monitor -- Ansible Module for FortiOS Monitor API.
++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++

.. versionadded:: 2.10

.. contents::
   :local:
   :depth: 1


Synopsis
--------
- Request FortiOS appliances to perform specific actions or procedures. This module contain all the FortiOS monitor API.



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
    <li><span class="li-head">selector</span> - Action taken in FortiOS appliance. <span class="li-normal">type: str</span> <span class="li-required">choices:</span></li>
        <li style="list-style: none;"><section class="accordion">
        <input type="checkbox" name="collapse" id="handle2">
        <h2 class="handle">
            <label for="handle2"><u>Show full selector list...</u></label>
        </h2>
        <div class="content">
        <ul class="ul-self">
        <li><span class="li-head">abort.user.query</span> - Abort a running user device unified query. 
        <ul class="ul-self">
                <li><span class="li-required">query_id</span> - Provide a query ID to abort an unified type query. <span class="li-normal">type: int  required: True </span> </li>
                
            </ul>
        
        </li>
        <li><span class="li-head">activate.user.fortitoken</span> - Activate a set of FortiTokens by serial number. 
        <ul class="ul-self">
                <li><span class="li-required">tokens</span> - List of FortiToken serial numbers to activate. If omitted, all tokens will be used. <span class="li-normal">type: array  required: False </span> </li>
                
            </ul>
        
        </li>
        <li><span class="li-head">add-license.registration.forticare</span> - Add a FortiCare license. 
        <ul class="ul-self">
                <li><span class="li-required">registration_code</span> - FortiCare contract number. <span class="li-normal">type: string  required: True </span> </li>
                
            </ul>
        
        </li>
        <li><span class="li-head">add-license.registration.vdom</span> - Add a VDOM license. 
        <ul class="ul-self">
                <li><span class="li-required">license</span> - VDOM license key. <span class="li-normal">type: string  required: True </span> </li>
                
            </ul>
        
        </li>
        <li><span class="li-head">add.firewall.clearpass-address</span> - Add ClearPass address with SPT (System Posture Token) value. 
        <ul class="ul-self">
                <li><span class="li-required">endpoint_ip</span> - Endpoint IPv4 address. <span class="li-normal">type: array  required: True </span> </li>
                <li><span class="li-required">spt</span> - SPT value [healthy|checkup|transient|quarantine|infected|unknown*]. <span class="li-normal">type: string  required: False </span> </li>
                
            </ul>
        
        </li>
        <li><span class="li-head">add.nsx.service</span> - Add NSX service to connector. 
        <ul class="ul-self">
                <li><span class="li-required">mkey</span> - NSX connector name. <span class="li-normal">type: string  required: True </span> </li>
                
            </ul>
        
        </li>
        <li><span class="li-head">add_users.user.banned</span> - Immediately add one or more users to the banned list. 
        <ul class="ul-self">
                <li><span class="li-required">ip_addresses</span> - List of IP Addresses to ban. IPv4 and IPv6 addresses are allowed. <span class="li-normal">type: array  required: True </span> </li>
                <li><span class="li-required">expiry</span> - Time until expiry in seconds. 0 for indefinite ban. <span class="li-normal">type: int  required: False </span> </li>
                
            </ul>
        
        </li>
        <li><span class="li-head">auth.user.firewall</span> - Trigger authentication for a single firewall user. 
        <ul class="ul-self">
                <li><span class="li-required">username</span> - User name. <span class="li-normal">type: string  required: True </span> </li>
                <li><span class="li-required">ip</span> - User IP address. <span class="li-normal">type: string  required: True </span> </li>
                <li><span class="li-required">server</span> - Name of an existing LDAP server entry. If supplied, authenticate that user against any matched groups on that LDAP server. <span class="li-normal">type: string  required: False </span> </li>
                
            </ul>
        
        </li>
        <li><span class="li-head">backup-action.system.fortimanager</span> - Import or update from FortiManager objects. 
        <ul class="ul-self">
                <li><span class="li-required">operation</span> - Operation to perform on the given CMDB objects [import|update]. <span class="li-normal">type: string  required: True </span> </li>
                <li><span class="li-required">objects</span> - Array of CMDB tables and mkeys. <span class="li-normal">type: array  required: True </span> </li>
                
            </ul>
        
        </li>
        <li><span class="li-head">backup.system.config</span> - Backup system config 
        <ul class="ul-self">
                <li><span class="li-required">destination</span> - Configuration file destination [file* | usb]. <span class="li-normal">type: string  required: False </span> </li>
                <li><span class="li-required">usb_filename</span> - When using 'usb' destination: the filename to save to on the connected USB device. <span class="li-normal">type: string  required: False </span> </li>
                <li><span class="li-required">password</span> - Password to encrypt configuration data. <span class="li-normal">type: string  required: False </span> </li>
                <li><span class="li-required">scope</span> - Specify global or VDOM only backup [global | vdom]. <span class="li-normal">type: string  required: True </span> </li>
                <li><span class="li-required">vdom</span> - If 'vdom' scope specified, the name of the VDOM to backup configuration. <span class="li-normal">type: string  required: False </span> </li>
                <li><span class="li-required">password_mask</span> - True to replace all the secrects and passwords with a mask. <span class="li-normal">type: boolean  required: False </span> </li>
                <li><span class="li-required">file_format</span> - Configuration file format [fos* | yaml]. <span class="li-normal">type: string  required: False </span> </li>
                
            </ul>
        
        </li>
        <li><span class="li-head">block.endpoint-control.registration</span> - Block endpoint by FortiClient UID or MAC. 
        <ul class="ul-self">
                <li><span class="li-required">uid</span> - Single FortiClient UID to block. <span class="li-normal">type: string  required: False </span> </li>
                <li><span class="li-required">mac</span> - Single MAC to block. <span class="li-normal">type: string  required: False </span> </li>
                
            </ul>
        
        </li>
        <li><span class="li-head">bounce-port.switch-controller.managed-switch</span> - Reset the port to force all connected clients to re-request DHCP lease. All active client sessions will be terminated. 
        <ul class="ul-self">
                <li><span class="li-required">mkey</span> - FortiSwitch ID. <span class="li-normal">type: string  required: True </span> </li>
                <li><span class="li-required">port</span> - FortiSwitch Port ID. <span class="li-normal">type: string  required: True </span> </li>
                <li><span class="li-required">duration</span> - Duration in seconds from 1 to 5 for port to be down. Defaults to 1 second if not provided. <span class="li-normal">type: int  required: False </span> </li>
                <li><span class="li-required">stop</span> - Stop a bounce in progress. <span class="li-normal">type: boolean  required: False </span> </li>
                
            </ul>
        
        </li>
        <li><span class="li-head">cancel.fortiview.session</span> - Cancel a FortiView request session. 
        <ul class="ul-self">
                <li><span class="li-required">sessionid</span> - Session ID to cancel. <span class="li-normal">type: int  required: False </span> </li>
                <li><span class="li-required">device</span> - FortiView request session's device. [disk|faz] <span class="li-normal">type: string  required: False </span> </li>
                <li><span class="li-required">report_by</span> - Report by field. <span class="li-normal">type: string  required: False </span> </li>
                <li><span class="li-required">view_level</span> - FortiView View level. <span class="li-normal">type: string  required: False </span> </li>
                
            </ul>
        
        </li>
        <li><span class="li-head">change-password.user.local</span> - Change password for local user. 
        <ul class="ul-self">
                <li><span class="li-required">username</span> - User name. <span class="li-normal">type: string  required: True </span> </li>
                <li><span class="li-required">new_password</span> - Password. <span class="li-normal">type: string  required: True </span> </li>
                
            </ul>
        
        </li>
        <li><span class="li-head">change-vdom-mode.system.admin</span> - Switch between VDOM modes. 
        <ul class="ul-self">
                <li><span class="li-required">vdom-mode</span> - VDOM mode [no-vdom|split-vdom|multi-vdom] <span class="li-normal">type: string  required: True </span> </li>
                
            </ul>
        
        </li>
        <li><span class="li-head">check.endpoint-control.registration-password</span> - Check if provided registration password is valid for current VDOM. 
        <ul class="ul-self">
                <li><span class="li-required">password</span> - Registration password to test. <span class="li-normal">type: string  required: True </span> </li>
                
            </ul>
        
        </li>
        <li><span class="li-head">clear-counters.firewall.central-snat-map</span> - Reset traffic statistics for one or more firewall central SNAT policy by policy ID. 
        <ul class="ul-self">
                <li><span class="li-required">policy</span> - Single policy ID to reset. <span class="li-normal">type: int  required: False </span> </li>
                
            </ul>
        
        </li>
        <li><span class="li-head">clear-counters.firewall.dnat</span> - Reset hit count statistics for one or more firewall virtual IP/server by ID. 
        <ul class="ul-self">
                <li><span class="li-required">id</span> - Single IDs to reset. <span class="li-normal">type: int  required: False </span> </li>
                <li><span class="li-required">is_ipv6</span> - Clear only IPv6 VIP stats. <span class="li-normal">type: boolean  required: False </span> </li>
                
            </ul>
        
        </li>
        <li><span class="li-head">clear-counters.firewall.ztna-firewall-policy</span> - Reset traffic statistics for one or more ZTNA firewall policies by policy ID. 
        <ul class="ul-self">
                <li><span class="li-required">policy</span> - Single ZTNA firewall policy ID to reset. <span class="li-normal">type: int  required: False </span> </li>
                
            </ul>
        
        </li>
        <li><span class="li-head">clear-soft-in.router.bgp</span> - Inbound soft-reconfiguration for BGP peers. 
        
        </li>
        <li><span class="li-head">clear-soft-out.router.bgp</span> - Outbound soft-reconfiguration for BGP peers. 
        
        </li>
        <li><span class="li-head">clear-statistics.system.fortiguard</span> - Immediately clear all FortiGuard statistics. 
        
        </li>
        <li><span class="li-head">clear.system.crash-log</span> - Clear system crash log. 
        
        </li>
        <li><span class="li-head">clear.system.sniffer</span> - Clear the results of a specified packet capture. 
        <ul class="ul-self">
                <li><span class="li-required">mkey</span> - ID of packet capture entry. <span class="li-normal">type: int  required: True </span> </li>
                
            </ul>
        
        </li>
        <li><span class="li-head">clear.vpn.ike</span> - Clear IKE gateways. 
        <ul class="ul-self">
                <li><span class="li-required">mkey</span> - Name of the IKE gateway to clear. <span class="li-normal">type: string  required: True </span> </li>
                
            </ul>
        
        </li>
        <li><span class="li-head">clear_all.firewall.session</span> - Immediately clear all active IPv4 and IPv6 sessions and IPS sessions of current VDOM. 
        
        </li>
        <li><span class="li-head">clear_all.user.banned</span> - Immediately clear all banned users. 
        
        </li>
        <li><span class="li-head">clear_all.wifi.rogue_ap</span> - Clear all detected rogue APs. 
        
        </li>
        <li><span class="li-head">clear_counters.firewall.acl</span> - Reset counters for one or more IPv4 ACLs by policy ID. 
        <ul class="ul-self">
                <li><span class="li-required">policy</span> - Single policy ID to reset. <span class="li-normal">type: int  required: False </span> </li>
                
            </ul>
        
        </li>
        <li><span class="li-head">clear_counters.firewall.acl6</span> - Reset counters for one or more IPv6 ACLs by policy ID. 
        <ul class="ul-self">
                <li><span class="li-required">policy</span> - Single policy ID to reset. <span class="li-normal">type: int  required: False </span> </li>
                
            </ul>
        
        </li>
        <li><span class="li-head">clear_counters.firewall.consolidated-policy</span> - Reset traffic statistics for one or more consolidated policies by policy ID. 
        <ul class="ul-self">
                <li><span class="li-required">policy</span> - Single policy ID to reset. <span class="li-normal">type: int  required: False </span> </li>
                
            </ul>
        
        </li>
        <li><span class="li-head">clear_counters.firewall.multicast-policy</span> - Reset traffic statistics for one or more firewall IPv4 multicast policies by policy ID. 
        <ul class="ul-self">
                <li><span class="li-required">policy</span> - Single policy ID to reset. <span class="li-normal">type: int  required: False </span> </li>
                
            </ul>
        
        </li>
        <li><span class="li-head">clear_counters.firewall.multicast-policy6</span> - Reset traffic statistics for one or more firewall IPv6 multicast policies by policy ID. 
        <ul class="ul-self">
                <li><span class="li-required">policy</span> - Single policy ID to reset. <span class="li-normal">type: int  required: False </span> </li>
                
            </ul>
        
        </li>
        <li><span class="li-head">clear_counters.firewall.policy</span> - Reset traffic statistics for one or more firewall policies by policy ID. 
        <ul class="ul-self">
                <li><span class="li-required">policy</span> - Single policy ID to reset. <span class="li-normal">type: int  required: False </span> </li>
                
            </ul>
        
        </li>
        <li><span class="li-head">clear_counters.firewall.policy6</span> - Reset traffic statistics for one or more IPv6 policies by policy ID. 
        <ul class="ul-self">
                <li><span class="li-required">policy</span> - Single policy ID to reset. <span class="li-normal">type: int  required: False </span> </li>
                
            </ul>
        
        </li>
        <li><span class="li-head">clear_counters.firewall.proxy-policy</span> - Reset traffic statistics for one or more explicit proxy policies by policy ID. 
        <ul class="ul-self">
                <li><span class="li-required">policy</span> - Single policy ID to reset. <span class="li-normal">type: int  required: False </span> </li>
                
            </ul>
        
        </li>
        <li><span class="li-head">clear_counters.firewall.security-policy</span> - Reset traffic statistics for one or more security policies by policy ID. 
        <ul class="ul-self">
                <li><span class="li-required">policy</span> - Single policy ID to reset. <span class="li-normal">type: int  required: False </span> </li>
                
            </ul>
        
        </li>
        <li><span class="li-head">clear_tunnel.vpn.ssl</span> - Remove all active tunnel sessions in current virtual domain. 
        
        </li>
        <li><span class="li-head">clear_users.user.banned</span> - Immediately clear a list of specific banned users by IP. 
        <ul class="ul-self">
                <li><span class="li-required">ip_addresses</span> - List of banned user IPs to clear. IPv4 and IPv6 addresses are allowed. <span class="li-normal">type: array  required: True </span> </li>
                
            </ul>
        
        </li>
        <li><span class="li-head">close-all.firewall.session</span> - Immediately close all active IPv4 and IPv6 sessions, as well as IPS sessions of the current VDOM. 
        
        </li>
        <li><span class="li-head">close-multiple.firewall.session</span> - Close multiple IPv4 firewall sessions which match the provided criteria. 
        <ul class="ul-self">
                <li><span class="li-required">proto</span> - Protocol name [tcp|udp|icmp|...] or number. <span class="li-normal">type: string  required: False </span> </li>
                <li><span class="li-required">saddr</span> - Source address. <span class="li-normal">type: string  required: False </span> </li>
                <li><span class="li-required">daddr</span> - Destination address. <span class="li-normal">type: string  required: False </span> </li>
                <li><span class="li-required">sport</span> - Source port. <span class="li-normal">type: int  required: False </span> </li>
                <li><span class="li-required">dport</span> - Destination port. <span class="li-normal">type: int  required: False </span> </li>
                <li><span class="li-required">naddr</span> - NAT'd source IP address. <span class="li-normal">type: string  required: False </span> </li>
                <li><span class="li-required">nport</span> - NAT'd source port. <span class="li-normal">type: int  required: False </span> </li>
                <li><span class="li-required">policy</span> - Policy ID. <span class="li-normal">type: int  required: False </span> </li>
                
            </ul>
        
        </li>
        <li><span class="li-head">close-multiple.firewall.session6</span> - Close multiple IPv6 firewall sessions which match the provided criteria. 
        <ul class="ul-self">
                <li><span class="li-required">proto</span> - Protocol name [tcp|udp|icmp|...] or number. <span class="li-normal">type: string  required: False </span> </li>
                <li><span class="li-required">saddr</span> - Source address. <span class="li-normal">type: string  required: False </span> </li>
                <li><span class="li-required">daddr</span> - Destination address. <span class="li-normal">type: string  required: False </span> </li>
                <li><span class="li-required">sport</span> - Source port. <span class="li-normal">type: int  required: False </span> </li>
                <li><span class="li-required">dport</span> - Destination port. <span class="li-normal">type: int  required: False </span> </li>
                <li><span class="li-required">policy</span> - Policy ID. <span class="li-normal">type: int  required: False </span> </li>
                
            </ul>
        
        </li>
        <li><span class="li-head">close.firewall.session</span> - Close a single firewall session that matches all provided criteria. 
        <ul class="ul-self">
                <li><span class="li-required">pro</span> - Protocol name [tcp|udp|icmp|...]. <span class="li-normal">type: string  required: True </span> </li>
                <li><span class="li-required">saddr</span> - Source address. <span class="li-normal">type: string  required: True </span> </li>
                <li><span class="li-required">daddr</span> - Destination address. <span class="li-normal">type: string  required: True </span> </li>
                <li><span class="li-required">sport</span> - Source port. <span class="li-normal">type: int  required: True </span> </li>
                <li><span class="li-required">dport</span> - Destination port. <span class="li-normal">type: int  required: True </span> </li>
                
            </ul>
        
        </li>
        <li><span class="li-head">config.system.fortimanager</span> - Configure FortiManager IP. Register FortiManager if 'fortimanager_ip' is provided.       Unregister FortiManager if only 'unregister' parameter is specified and set to true. 
        <ul class="ul-self">
                <li><span class="li-required">fortimanager_ip</span> - FortiManager IP address. <span class="li-normal">type: string  required: False </span> </li>
                <li><span class="li-required">unregister</span> - Unregister the FortiManager (default=false). <span class="li-normal">type: boolean  required: False </span> </li>
                
            </ul>
        
        </li>
        <li><span class="li-head">connect.system.modem</span> - Trigger a connect for the configured modem. 
        
        </li>
        <li><span class="li-head">connect.wifi.network</span> - When FortiWiFi is in client mode, connect to the specified network, if configured in the 'wifi' interface. 
        <ul class="ul-self">
                <li><span class="li-required">ssid</span> - SSID of network to connect to. <span class="li-normal">type: string  required: True </span> </li>
                
            </ul>
        
        </li>
        <li><span class="li-head">create-default.wifi.ap-profile</span> - Create a default FortiAP profile for the specified platform. 
        <ul class="ul-self">
                <li><span class="li-required">platform</span> - FortiAP platform to create a default profile for. <span class="li-normal">type: string  required: True </span> </li>
                
            </ul>
        
        </li>
        <li><span class="li-head">create.forticonverter.ticket</span> - Create a new FortiConverter service ticket to initiate a migration. 
        
        </li>
        <li><span class="li-head">create.registration.forticare</span> - Create a new FortiCare account. 
        <ul class="ul-self">
                <li><span class="li-required">email</span> - Account email. <span class="li-normal">type: string  required: True </span> </li>
                <li><span class="li-required">password</span> - Account password. <span class="li-normal">type: string  required: True </span> </li>
                <li><span class="li-required">first_name</span> - First name. <span class="li-normal">type: string  required: True </span> </li>
                <li><span class="li-required">last_name</span> - Last name. <span class="li-normal">type: string  required: True </span> </li>
                <li><span class="li-required">title</span> - Title. <span class="li-normal">type: string  required: False </span> </li>
                <li><span class="li-required">company</span> - Company. <span class="li-normal">type: string  required: True </span> </li>
                <li><span class="li-required">address</span> - Address. <span class="li-normal">type: string  required: True </span> </li>
                <li><span class="li-required">city</span> - City. <span class="li-normal">type: string  required: True </span> </li>
                <li><span class="li-required">country_code</span> - Country code. <span class="li-normal">type: int  required: True </span> </li>
                <li><span class="li-required">state</span> - State/Province. <span class="li-normal">type: string  required: True </span> </li>
                <li><span class="li-required">state_code</span> - State/Province code. <span class="li-normal">type: string  required: False </span> </li>
                <li><span class="li-required">postal_code</span> - Postal code. <span class="li-normal">type: string  required: True </span> </li>
                <li><span class="li-required">phone</span> - Phone number. <span class="li-normal">type: string  required: True </span> </li>
                <li><span class="li-required">industry</span> - Industry. <span class="li-normal">type: string  required: True </span> </li>
                <li><span class="li-required">industry_id</span> - Industry ID. <span class="li-normal">type: int  required: True </span> </li>
                <li><span class="li-required">orgsize_id</span> - Organization size ID. <span class="li-normal">type: int  required: True </span> </li>
                <li><span class="li-required">reseller_name</span> - Reseller name. <span class="li-normal">type: string  required: True </span> </li>
                <li><span class="li-required">reseller_id</span> - Reseller ID. <span class="li-normal">type: int  required: True </span> </li>
                <li><span class="li-required">is_government</span> - Set to true if the end-user is affiliated with a government. <span class="li-normal">type: boolean  required: False </span> </li>
                
            </ul>
        
        </li>
        <li><span class="li-head">create.registration.forticloud</span> - Create a FortiCloud account. 
        <ul class="ul-self">
                <li><span class="li-required">email</span> - Account email. <span class="li-normal">type: string  required: True </span> </li>
                <li><span class="li-required">password</span> - Account password. <span class="li-normal">type: string  required: True </span> </li>
                <li><span class="li-required">send_logs</span> - Send logs to FortiCloud. <span class="li-normal">type: boolean  required: False </span> </li>
                
            </ul>
        
        </li>
        <li><span class="li-head">create.vpn-certificate.local</span> - Generate a new certificate signed by Fortinet_CA_SSL. 
        <ul class="ul-self">
                <li><span class="li-required">certname</span> - Certificate name. <span class="li-normal">type: string  required: True </span> </li>
                <li><span class="li-required">common_name</span> - Certificate common name. <span class="li-normal">type: string  required: True </span> </li>
                <li><span class="li-required">scope</span> - Scope of local certificate [vdom*|global]. Global scope is only accessible for global administrators. <span class="li-normal">type: string  required: True </span> </li>
                
            </ul>
        
        </li>
        <li><span class="li-head">create.web-ui.custom-language</span> - Upload custom language file to this Fortigate. 
        <ul class="ul-self">
                <li><span class="li-required">lang_name</span> - Name of custom language entry. <span class="li-normal">type: string  required: True </span> </li>
                <li><span class="li-required">lang_comments</span> - Comments of custom language entry. <span class="li-normal">type: string  required: False </span> </li>
                <li><span class="li-required">file_content</span> - Provided when uploading a file: base64 encoded file data. Must not contain whitespace or other invalid base64 characters. Must be included in HTTP body. <span class="li-normal">type: string  required: False </span> </li>
                
            </ul>
        
        </li>
        <li><span class="li-head">deauth.user.firewall</span> - Deauthenticate single, multiple, or all firewall users. 
        <ul class="ul-self">
                <li><span class="li-required">user_type</span> - User type [proxy|firewall]. Required for both proxy and firewall users. <span class="li-normal">type: string  required: False </span> </li>
                <li><span class="li-required">id</span> - User ID. Required for both proxy and firewall users. <span class="li-normal">type: int  required: False </span> </li>
                <li><span class="li-required">ip</span> - User IP address. Required for both proxy and firewall users. <span class="li-normal">type: string  required: False </span> </li>
                <li><span class="li-required">ip_version</span> - IP version [ip4|ip6]. Only required if user_type is firewall. <span class="li-normal">type: string  required: False </span> </li>
                <li><span class="li-required">method</span> - Authentication method [fsso|rsso|ntlm|firewall|wsso|fsso_citrix|sso_guest]. Only required if user_type is firewall. <span class="li-normal">type: string  required: False </span> </li>
                <li><span class="li-required">all</span> - Set to true to deauthenticate all users. Other parameters will be ignored. <span class="li-normal">type: boolean  required: False </span> </li>
                <li><span class="li-required">users</span> - Array of user objects to deauthenticate. Use this to deauthenticate multiple users at once. Each object should include the above properties. <span class="li-normal">type: array  required: False </span> </li>
                
            </ul>
        
        </li>
        <li><span class="li-head">delete.firewall.clearpass-address</span> - Delete ClearPass address with SPT (System Posture Token) value. 
        <ul class="ul-self">
                <li><span class="li-required">endpoint_ip</span> - Endpoint IPv4 address. <span class="li-normal">type: array  required: True </span> </li>
                <li><span class="li-required">spt</span> - SPT value [healthy|checkup|transient|quarantine|infected|unknown*]. <span class="li-normal">type: string  required: False </span> </li>
                
            </ul>
        
        </li>
        <li><span class="li-head">delete.log.local-report</span> - Delete a local report. 
        <ul class="ul-self">
                <li><span class="li-required">mkeys</span> - Local Report Name. <span class="li-normal">type: array  required: True </span> </li>
                
            </ul>
        
        </li>
        <li><span class="li-head">delete.system.config-revision</span> - Deletes one or more system configuration revisions. 
        <ul class="ul-self">
                <li><span class="li-required">config_ids</span> - List of configuration ids. <span class="li-normal">type: array  required: True </span> </li>
                
            </ul>
        
        </li>
        <li><span class="li-head">delete.system.config-script</span> - Delete the history of config scripts. 
        <ul class="ul-self">
                <li><span class="li-required">id_list</span> - List of config script history ids to delete. <span class="li-normal">type: array  required: True </span> </li>
                
            </ul>
        
        </li>
        <li><span class="li-head">delete.vpn.ssl</span> - Terminate the provided Agentless VPN session. 
        <ul class="ul-self">
                <li><span class="li-required">type</span> - The session type [websession|subsession]. <span class="li-normal">type: string  required: True </span> </li>
                <li><span class="li-required">index</span> - The session index. <span class="li-normal">type: int  required: True </span> </li>
                
            </ul>
        
        </li>
        <li><span class="li-head">delete.webfilter.override</span> - Delete a configured webfilter override. 
        <ul class="ul-self">
                <li><span class="li-required">mkey</span> - ID of webfilter override to delete. <span class="li-normal">type: string  required: False </span> </li>
                
            </ul>
        
        </li>
        <li><span class="li-head">deregister-device.registration.forticare</span> - Deregister the FortiGate from a FortiCare account. 
        <ul class="ul-self">
                <li><span class="li-required">email</span> - FortiCare email. <span class="li-normal">type: string  required: True </span> </li>
                <li><span class="li-required">password</span> - Account password. <span class="li-normal">type: string  required: True </span> </li>
                
            </ul>
        
        </li>
        <li><span class="li-head">deregister.endpoint-control.registration</span> - Deregister endpoint by FortiClient UID or MAC. 
        <ul class="ul-self">
                <li><span class="li-required">uid</span> - Single FortiClient UID to deregister. <span class="li-normal">type: string  required: False </span> </li>
                <li><span class="li-required">mac</span> - Single MAC to deregister. <span class="li-normal">type: string  required: False </span> </li>
                
            </ul>
        
        </li>
        <li><span class="li-head">dhcp-renew.system.interface</span> - Renew DHCP lease of an interface. 
        <ul class="ul-self">
                <li><span class="li-required">mkey</span> - Name of the interface. <span class="li-normal">type: string  required: True </span> </li>
                <li><span class="li-required">ipv6</span> - Renew the DHCPv6 lease. <span class="li-normal">type: boolean  required: False </span> </li>
                
            </ul>
        
        </li>
        <li><span class="li-head">diagnose.extender-controller.extender</span> - Execute diagnotic commands. 
        <ul class="ul-self">
                <li><span class="li-required">id</span> - FortiExtender ID. <span class="li-normal">type: string  required: True </span> </li>
                <li><span class="li-required">cmd</span> - Command to execute. <span class="li-normal">type: string  required: True </span> </li>
                
            </ul>
        
        </li>
        <li><span class="li-head">disassociate.wifi.client</span> - Disassociate a WiFi client from the FortiAP it's currently connected to. The client will need to reassociate with the same FortiAP or another to resume connectivity. 
        <ul class="ul-self">
                <li><span class="li-required">mac</span> - MAC address. <span class="li-normal">type: string  required: True </span> </li>
                
            </ul>
        
        </li>
        <li><span class="li-head">disconnect.system.ha-peer</span> - Update configuration of peer in HA cluster. 
        <ul class="ul-self">
                <li><span class="li-required">serial_no</span> - Serial number of the HA member. <span class="li-normal">type: string  required: True </span> </li>
                <li><span class="li-required">interface</span> - Name of the interface which should be assigned for management. <span class="li-normal">type: string  required: True </span> </li>
                <li><span class="li-required">ip</span> - IP to assign to the selected interface. <span class="li-normal">type: string  required: True </span> </li>
                <li><span class="li-required">mask</span> - Full network mask to assign to the selected interface. <span class="li-normal">type: string  required: True </span> </li>
                
            </ul>
        
        </li>
        <li><span class="li-head">disconnect.system.modem</span> - Trigger a disconnect for the configured modem. 
        
        </li>
        <li><span class="li-head">download-eval.system.vmlicense</span> - Download Evaluation VM License and reboot immediately if successful. 
        <ul class="ul-self">
                <li><span class="li-required">account_id</span> - FortiCare account email. <span class="li-normal">type: string  required: True </span> </li>
                <li><span class="li-required">account_password</span> - FortiCare account password. <span class="li-normal">type: string  required: True </span> </li>
                <li><span class="li-required">is_government</span> - Is the account in use by a government user? <span class="li-normal">type: boolean  required: False </span> </li>
                
            </ul>
        
        </li>
        <li><span class="li-head">download.switch-controller.fsw-firmware</span> - Download FortiSwitch firmware from FortiGuard to the FortiGate according to FortiSwitch image ID. 
        <ul class="ul-self">
                <li><span class="li-required">image_id</span> - FortiSwitch image ID. <span class="li-normal">type: string  required: True </span> </li>
                
            </ul>
        
        </li>
        <li><span class="li-head">download.system.vmlicense</span> - Download Flex-VM license and reboot immediately if successful. 
        <ul class="ul-self">
                <li><span class="li-required">token</span> - VM license token. <span class="li-normal">type: string  required: False </span> </li>
                <li><span class="li-required">proxy_url</span> - HTTP proxy URL in the form: http://user:pass@proxyip:proxyport. <span class="li-normal">type: string  required: False </span> </li>
                
            </ul>
        
        </li>
        <li><span class="li-head">download.wifi.firmware</span> - Download FortiAP firmware from FortiGuard to the FortiGate according to FortiAP image ID. 
        <ul class="ul-self">
                <li><span class="li-required">image_id</span> - FortiAP image ID. <span class="li-normal">type: string  required: True </span> </li>
                
            </ul>
        
        </li>
        <li><span class="li-head">dump.system.com-log</span> - Dump system com-log to file. 
        
        </li>
        <li><span class="li-head">dynamic.system.external-resource</span> - Push updates to the specified external resource. 
        <ul class="ul-self">
                <li><span class="li-required">commands</span> - The commands to execute to update dynamic external resources. <span class="li-normal">type: array  required: True </span> </li>
                
            </ul>
        
        </li>
        <li><span class="li-head">eject.system.usb-device</span> - Eject USB drives for safe removal. 
        
        </li>
        <li><span class="li-head">email.user.guest</span> - Sent guest login details via email. 
        <ul class="ul-self">
                <li><span class="li-required">group</span> - Guest group name. <span class="li-normal">type: string  required: True </span> </li>
                <li><span class="li-required">guest</span> - Guest user IDs. <span class="li-normal">type: array  required: True </span> </li>
                
            </ul>
        
        </li>
        <li><span class="li-head">enable-app-bandwidth-tracking.system.traffic-history</span> - Enable FortiView application bandwidth tracking. 
        
        </li>
        <li><span class="li-head">factory-reset.switch-controller.managed-switch</span> - Send 'Factory Reset' command to a given FortiSwitch. 
        <ul class="ul-self">
                <li><span class="li-required">mkey</span> - Name of managed FortiSwitch. <span class="li-normal">type: string  required: True </span> </li>
                
            </ul>
        
        </li>
        <li><span class="li-head">flush.firewall.gtp</span> - Flush GTP tunnels. 
        <ul class="ul-self">
                <li><span class="li-required">scope</span> - Scope from which to flush tunnels from [global|*vdom]. <span class="li-normal">type: string  required: False </span> </li>
                <li><span class="li-required">gtp_profile</span> - Filter: GTP profile. <span class="li-normal">type: string  required: False </span> </li>
                <li><span class="li-required">version</span> - Filter: GTP version. <span class="li-normal">type: int  required: False </span> </li>
                <li><span class="li-required">imsi</span> - Filter: International mobile subscriber identity. <span class="li-normal">type: string  required: False </span> </li>
                <li><span class="li-required">msisdn</span> - Filter: Mobile station international subscriber directory number <span class="li-normal">type: string  required: False </span> </li>
                <li><span class="li-required">ms_addr</span> - Filter: Mobile user IP address. <span class="li-normal">type: string  required: False </span> </li>
                <li><span class="li-required">ms_addr6</span> - Filter: Mobile user IPv6 address. <span class="li-normal">type: string  required: False </span> </li>
                <li><span class="li-required">cteid</span> - Filter: Control plane fully qualified tunnel endpoint identifier. <span class="li-normal">type: int  required: False </span> </li>
                <li><span class="li-required">cteid_addr</span> - Filter: Control plane TEID IP address. <span class="li-normal">type: string  required: False </span> </li>
                <li><span class="li-required">cteid_addr6</span> - Filter: Control plane TEID IPv6 address. <span class="li-normal">type: string  required: False </span> </li>
                <li><span class="li-required">fteid</span> - Filter: Data plane fully qualified tunnel endpoint identifier. <span class="li-normal">type: int  required: False </span> </li>
                <li><span class="li-required">fteid_addr</span> - Filter: Data plane TEID IP address. <span class="li-normal">type: string  required: False </span> </li>
                <li><span class="li-required">fteid_addr6</span> - Filter: Data plane TEID IPv6 address. <span class="li-normal">type: string  required: False </span> </li>
                <li><span class="li-required">apn</span> - Filter: Access point name. <span class="li-normal">type: string  required: False </span> </li>
                
            </ul>
        
        </li>
        <li><span class="li-head">format.system.logdisk</span> - Format log disk. 
        <ul class="ul-self">
                <li><span class="li-required">raid</span> - RAID level [Raid-0|Raid-1|Raid-5|Raid-10]. <span class="li-normal">type: string  required: True </span> </li>
                
            </ul>
        
        </li>
        <li><span class="li-head">forticonverter.set-source-sn</span> - Set the source FortiGate which will upload its config. 
        <ul class="ul-self">
                <li><span class="li-required">source_sn</span> - Source FortiGate serial. <span class="li-normal">type: string  required: True </span> </li>
                <li><span class="li-required">ticket_id</span> - Service ticket ID. <span class="li-normal">type: string  required: True </span> </li>
                
            </ul>
        
        </li>
        <li><span class="li-head">generate-key.system.api-user</span> - Generate a new api-key for the specified api-key-auth admin. The old api-key will be replaced. The response contains the only chance to read the new api-key plaintext in the api_key field. 
        <ul class="ul-self">
                <li><span class="li-required">api-user</span> - Generate a new token for this api-user. <span class="li-normal">type: string  required: True </span> </li>
                <li><span class="li-required">expiry</span> - Optional expiry of API key in minutes from now (valid range: 1 - 10080). <span class="li-normal">type: int  required: False </span> </li>
                
            </ul>
        
        </li>
        <li><span class="li-head">generate-keys.wifi.ssid</span> - Generate pre-shared keys for specific multi pre-shared key profile. 
        <ul class="ul-self">
                <li><span class="li-required">mpsk_profile</span> - Multi pre-shared key profile to add keys to. <span class="li-normal">type: string  required: True </span> </li>
                <li><span class="li-required">group</span> - Multi pre-shared key group to add keys to. <span class="li-normal">type: string  required: True </span> </li>
                <li><span class="li-required">prefix</span> - Prefix to be added at the start of the generated key's name. <span class="li-normal">type: string  required: True </span> </li>
                <li><span class="li-required">count</span> - Number of keys to be generated [1-512]. <span class="li-normal">type: int  required: True </span> </li>
                <li><span class="li-required">key_length</span> - Length of the keys to be generated [8-63]. <span class="li-normal">type: int  required: True </span> </li>
                
            </ul>
        
        </li>
        <li><span class="li-head">generate.vpn-certificate.csr</span> - Generate a certificate signing request (CSR) and a private key. The CSR can be retrieved / downloaded from CLI, GUI and REST API. 
        <ul class="ul-self">
                <li><span class="li-required">certname</span> - Certicate name. Used to retrieve / download the CSR. Not included in CSR and key content. <span class="li-normal">type: string  required: True </span> </li>
                <li><span class="li-required">subject</span> - Subject (Host IP/Domain Name/E-Mail). Common Name (CN) of the certificate subject. <span class="li-normal">type: string  required: True </span> </li>
                <li><span class="li-required">keytype</span> - Generate a RSA or an elliptic curve certificate request [rsa|ec]. The Elliptic Curve option is unavailable if the FortiGate is a Low Encryption Device (LENC) <span class="li-normal">type: string  required: True </span> </li>
                <li><span class="li-required">keysize</span> - Key size.[1024|1536|2048|4096]. 512 only if the FortiGate is a Low Encryption Device (LENC). Required when keytype is RSA. <span class="li-normal">type: int  required: False </span> </li>
                <li><span class="li-required">curvename</span> - Elliptic curve name. [secp256r1|secp384r1|secp521r1]. Unavailable if the FortiGate is a Low Encryption Device (LENC). Required when keytype is ec. <span class="li-normal">type: string  required: False </span> </li>
                <li><span class="li-required">orgunits</span> - List of organization units. Organization Units (OU) of the certificate subject. <span class="li-normal">type: array  required: False </span> </li>
                <li><span class="li-required">org</span> - Organization (O) of the certificate subject. <span class="li-normal">type: string  required: False </span> </li>
                <li><span class="li-required">city</span> - Locality (L) of the certificate subject. <span class="li-normal">type: string  required: False </span> </li>
                <li><span class="li-required">state</span> - State (ST) of the certificate subject. <span class="li-normal">type: string  required: False </span> </li>
                <li><span class="li-required">countrycode</span> - Country (C) of the certificate subject. <span class="li-normal">type: string  required: False </span> </li>
                <li><span class="li-required">email</span> - Email of the certificate subject. <span class="li-normal">type: string  required: False </span> </li>
                <li><span class="li-required">subject_alt_name</span> - Subject alternative name (SAN) of the certificate. <span class="li-normal">type: string  required: False </span> </li>
                <li><span class="li-required">password</span> - Password / pass phrase for the private key. If not provided, FortiGate generates a random one. <span class="li-normal">type: string  required: False </span> </li>
                <li><span class="li-required">scep_url</span> - SCEP server URL. If provided, use the url to enroll the csr through SCEP. <span class="li-normal">type: string  required: False </span> </li>
                <li><span class="li-required">scep_password</span> - SCEP challenge password. Some SCEP servers may require challege password. Provide it when SCEP server requires. <span class="li-normal">type: string  required: False </span> </li>
                <li><span class="li-required">scope</span> - Scope of CSR [vdom*|global]. Global scope is only accessible for global administrators <span class="li-normal">type: string  required: False </span> </li>
                
            </ul>
        
        </li>
        <li><span class="li-head">generic-address.system.external-resource</span> - Push JSON data to the specified external resource. 
        <ul class="ul-self">
                <li><span class="li-required">mkey</span> - The name of the external resource to update. <span class="li-normal">type: string  required: True </span> </li>
                <li><span class="li-required">data</span> - JSON data. <span class="li-normal">type: object  required: True </span> </li>
                
            </ul>
        
        </li>
        <li><span class="li-head">geoip.geoip-query</span> - Retrieve location details for IPs queried against FortiGuard's geoip service. 
        <ul class="ul-self">
                <li><span class="li-required">ip_addresses</span> - One or more IP address strings to query for location details. <span class="li-normal">type: array  required: True </span> </li>
                
            </ul>
        
        </li>
        <li><span class="li-head">import-mobile.user.fortitoken</span> - Import a list of tokens from FortiGuard to the FortiGate unit. 
        <ul class="ul-self">
                <li><span class="li-required">code</span> - Activation code on redemption certificate. <span class="li-normal">type: string  required: True </span> </li>
                
            </ul>
        
        </li>
        <li><span class="li-head">import-seed.user.fortitoken</span> - Import a FortiToken seed file. 
        <ul class="ul-self">
                <li><span class="li-required">file_content</span> - Provided when uploading a file: base64 encoded file data. Must not contain whitespace or other invalid base64 characters. Must be included in HTTP body. <span class="li-normal">type: string  required: False </span> </li>
                
            </ul>
        
        </li>
        <li><span class="li-head">import-trial.user.fortitoken</span> - Import trial mobile FortiTokens. 
        
        </li>
        <li><span class="li-head">import.vpn-certificate.ca</span> - Import CA certificate. 
        <ul class="ul-self">
                <li><span class="li-required">import_method</span> - Method of importing CA certificate.[file|scep] <span class="li-normal">type: string  required: True </span> </li>
                <li><span class="li-required">scep_url</span> - SCEP server URL. Required for import via SCEP <span class="li-normal">type: string  required: False </span> </li>
                <li><span class="li-required">scep_ca_id</span> - SCEP server CA identifier for import via SCEP. <span class="li-normal">type: string  required: False </span> </li>
                <li><span class="li-required">scope</span> - Scope of CA certificate [vdom*|global]. Global scope is only accessible for global administrators <span class="li-normal">type: string  required: False </span> </li>
                <li><span class="li-required">file_content</span> - Provided when uploading a file: base64 encoded file data. Must not contain whitespace or other invalid base64 characters. Must be included in HTTP body. <span class="li-normal">type: string  required: False </span> </li>
                
            </ul>
        
        </li>
        <li><span class="li-head">import.vpn-certificate.crl</span> - Import certificate revocation lists (CRL) from file content. 
        <ul class="ul-self">
                <li><span class="li-required">scope</span> - Scope of CRL [vdom*|global]. Global scope is only accessible for global administrators <span class="li-normal">type: string  required: False </span> </li>
                <li><span class="li-required">file_content</span> - Provided when uploading a file: base64 encoded file data. Must not contain whitespace or other invalid base64 characters. Must be included in HTTP body. <span class="li-normal">type: string  required: False </span> </li>
                
            </ul>
        
        </li>
        <li><span class="li-head">import.vpn-certificate.local</span> - Import local certificate. 
        <ul class="ul-self">
                <li><span class="li-required">type</span> - Type of certificate.[local|pkcs12|regular] <span class="li-normal">type: string  required: True </span> </li>
                <li><span class="li-required">certname</span> - Certificate name for pkcs12 and regular certificate types. <span class="li-normal">type: string  required: False </span> </li>
                <li><span class="li-required">password</span> - Optional password for pkcs12 and regular certificate types. <span class="li-normal">type: string  required: False </span> </li>
                <li><span class="li-required">key_file_content</span> - Key content encoded in BASE64 for regular certificate type. <span class="li-normal">type: string  required: False </span> </li>
                <li><span class="li-required">scope</span> - Scope of local certificate [vdom*|global]. Global scope is only accessible for global administrators <span class="li-normal">type: string  required: False </span> </li>
                <li><span class="li-required">acme_domain</span> - A valid domain that resolves to an IP whose TCP port 443 reaches this FortiGate. <span class="li-normal">type: string  required: False </span> </li>
                <li><span class="li-required">acme_email</span> - Contact email address that is required by some CAs such as LetsEncrypt. <span class="li-normal">type: string  required: False </span> </li>
                <li><span class="li-required">acme_ca_url</span> - URL for the ACME CA server. <span class="li-normal">type: string  required: False </span> </li>
                <li><span class="li-required">acme_rsa_key_size</span> - Length of the RSA private key for the generated cert. <span class="li-normal">type: int  required: False </span> </li>
                <li><span class="li-required">acme_renew_window</span> - Certificate renewal window in days. <span class="li-normal">type: int  required: False </span> </li>
                <li><span class="li-required">file_content</span> - Provided when uploading a file: base64 encoded file data. Must not contain whitespace or other invalid base64 characters. Must be included in HTTP body. <span class="li-normal">type: string  required: False </span> </li>
                
            </ul>
        
        </li>
        <li><span class="li-head">import.vpn-certificate.remote</span> - Import remote certificate. 
        <ul class="ul-self">
                <li><span class="li-required">scope</span> - Scope of CRL [vdom*|global]. Global scope is only accessible for global administrators <span class="li-normal">type: string  required: False </span> </li>
                <li><span class="li-required">file_content</span> - Provided when uploading a file: base64 encoded file data. Must not contain whitespace or other invalid base64 characters. Must be included in HTTP body. <span class="li-normal">type: string  required: False </span> </li>
                
            </ul>
        
        </li>
        <li><span class="li-head">import.web-ui.language</span> - Import localization language file to this FortiGate. 
        <ul class="ul-self">
                <li><span class="li-required">file_content</span> - Provided when uploading a file: base64 encoded file data. Must not contain whitespace or other invalid base64 characters. Must be included in HTTP body. <span class="li-normal">type: string  required: False </span> </li>
                
            </ul>
        
        </li>
        <li><span class="li-head">keep-alive.wifi.spectrum</span> - Extend duration of an existing spectrum analysis for a specific FortiAP. 
        <ul class="ul-self">
                <li><span class="li-required">wtp_id</span> - FortiAP ID. <span class="li-normal">type: string  required: True </span> </li>
                <li><span class="li-required">radio_id</span> - Radio ID. <span class="li-normal">type: int  required: True </span> </li>
                <li><span class="li-required">duration</span> - Duration in seconds. <span class="li-normal">type: int  required: True </span> </li>
                
            </ul>
        
        </li>
        <li><span class="li-head">kill.system.process</span> - Kill a running process. 
        <ul class="ul-self">
                <li><span class="li-required">pid</span> - The process ID. <span class="li-normal">type: int  required: True </span> </li>
                <li><span class="li-required">signal</span> - Signal to use when killing the process [9 (SIGKILL) | 11 (SIGSEGV) | 15 (SIGTERM)]. Defaults to 15. <span class="li-normal">type: int  required: False </span> </li>
                
            </ul>
        
        </li>
        <li><span class="li-head">led-blink.wifi.managed_ap</span> - Turn a managed FortiAP's LED blinking on or off. 
        <ul class="ul-self">
                <li><span class="li-required">serials</span> - FortiAP IDs to turn LED blink on/off. <span class="li-normal">type: array  required: True </span> </li>
                <li><span class="li-required">blink</span> - True to turn on blinking, false to turn off. <span class="li-normal">type: boolean  required: True </span> </li>
                <li><span class="li-required">duration</span> - Time to blink, in seconds. 0 or omit for indefinite. <span class="li-normal">type: int  required: False </span> </li>
                
            </ul>
        
        </li>
        <li><span class="li-head">login.registration.forticare</span> - Login to FortiCare. 
        <ul class="ul-self">
                <li><span class="li-required">serial</span> - Serial number of an HA cluster member to register to login to FortiCare. Current device will be selected if not set. <span class="li-normal">type: string  required: False </span> </li>
                <li><span class="li-required">email</span> - Account email. <span class="li-normal">type: string  required: True </span> </li>
                <li><span class="li-required">password</span> - Account password. <span class="li-normal">type: string  required: True </span> </li>
                <li><span class="li-required">reseller_name</span> - Reseller name. <span class="li-normal">type: string  required: True </span> </li>
                <li><span class="li-required">reseller_id</span> - Reseller ID. <span class="li-normal">type: int  required: True </span> </li>
                <li><span class="li-required">agreement_accepted</span> - Set to true if the end-user accepted the agreement. <span class="li-normal">type: boolean  required: False </span> </li>
                <li><span class="li-required">is_government</span> - Set to true if the end-user is affiliated with a government. <span class="li-normal">type: boolean  required: False </span> </li>
                
            </ul>
        
        </li>
        <li><span class="li-head">login.registration.forticloud</span> - Login to FortiCloud. 
        <ul class="ul-self">
                <li><span class="li-required">email</span> - Account email. <span class="li-normal">type: string  required: True </span> </li>
                <li><span class="li-required">password</span> - Account password. <span class="li-normal">type: string  required: True </span> </li>
                <li><span class="li-required">send_logs</span> - Send logs to FortiCloud. <span class="li-normal">type: boolean  required: False </span> </li>
                <li><span class="li-required">domain</span> - FortiCloud domain. <span class="li-normal">type: string  required: False </span> </li>
                
            </ul>
        
        </li>
        <li><span class="li-head">logout.registration.forticloud</span> - Logout from FortiCloud. 
        
        </li>
        <li><span class="li-head">manual-update.system.fortiguard</span> - Manually update entitlements. 
        <ul class="ul-self">
                <li><span class="li-required">file_content</span> - Provided when uploading a file: base64 encoded file data. Must not contain whitespace or other invalid base64 characters. Must be included in HTTP body. <span class="li-normal">type: string  required: False </span> </li>
                
            </ul>
        
        </li>
        <li><span class="li-head">migrate.registration.forticloud</span> - Migrate standalone FortiGate Cloud account to FortiCloud. 
        <ul class="ul-self">
                <li><span class="li-required">email</span> - Account email. <span class="li-normal">type: string  required: True </span> </li>
                <li><span class="li-required">password</span> - Account password. <span class="li-normal">type: string  required: True </span> </li>
                
            </ul>
        
        </li>
        <li><span class="li-head">poe-reset.switch-controller.managed-switch</span> - Reset PoE on a given FortiSwitch's port. 
        <ul class="ul-self">
                <li><span class="li-required">mkey</span> - Name of managed FortiSwitch. <span class="li-normal">type: string  required: True </span> </li>
                <li><span class="li-required">port</span> - Name of port to reset PoE on. <span class="li-normal">type: string  required: True </span> </li>
                
            </ul>
        
        </li>
        <li><span class="li-head">port-stats-reset.switch-controller.managed-switch</span> - Reset port statistics for a given FortiSwitch. 
        <ul class="ul-self">
                <li><span class="li-required">mkey</span> - FortiSwitch ID. <span class="li-normal">type: string  required: True </span> </li>
                <li><span class="li-required">ports</span> - Name of ports to reset statistics on. <span class="li-normal">type: array  required: False </span> </li>
                
            </ul>
        
        </li>
        <li><span class="li-head">provision-user.vpn.ssl</span> - Provision SSL-VPN users with target applications. The provisioning message (email or SMS) is sent with no confirmation of success. 
        <ul class="ul-self">
                <li><span class="li-required">host</span> - The hostname/IP address of the VPN server. <span class="li-normal">type: string  required: True </span> </li>
                <li><span class="li-required">port</span> - The port of the VPN server. <span class="li-normal">type: int  required: True </span> </li>
                <li><span class="li-required">vpn_name</span> - The name of the VPN configuration. <span class="li-normal">type: string  required: True </span> </li>
                <li><span class="li-required">method</span> - Method to send [email|sms]. If not set, email will be the default. <span class="li-normal">type: string  required: False </span> </li>
                <li><span class="li-required">email_list</span> - The email address that the VPN configuration message should be sent to. Required if "method" is "email". <span class="li-normal">type: string  required: False </span> </li>
                <li><span class="li-required">phone_user_list</span> - The user that the VPN configuration SMS should be sent to. At least one of "phone_user_list" or "phone_number_list" is required if "method" is "sms". <span class="li-normal">type: string  required: False </span> </li>
                <li><span class="li-required">phone_number_list</span> - The phone number that the VPN configuration SMS should be sent to. At least one of "phone_user_list" or "phone_number_list" is required if "method" is "sms". <span class="li-normal">type: string  required: False </span> </li>
                <li><span class="li-required">sms_method</span> - The method to be used for sending the SMS [fortiguard|custom]. Default is "fortiguard". <span class="li-normal">type: string  required: False </span> </li>
                <li><span class="li-required">sms_server</span> - The SMS server to be used for sending SMS messages, required if "custom" SMS method is chosen. <span class="li-normal">type: string  required: False </span> </li>
                
            </ul>
        
        </li>
        <li><span class="li-head">provision.user.fortitoken</span> - Provision a set of FortiTokens by serial number. 
        <ul class="ul-self">
                <li><span class="li-required">tokens</span> - List of FortiToken serial numbers to provision. If omitted, all tokens will be used. <span class="li-normal">type: array  required: False </span> </li>
                
            </ul>
        
        </li>
        <li><span class="li-head">pse-config.switch-controller.recommendation</span> - Execute switch recommendation for pse-config to prevent PSE-PSE scenarios. 
        <ul class="ul-self">
                <li><span class="li-required">fortilink</span> - FortiLink interface name. <span class="li-normal">type: string  required: True </span> </li>
                
            </ul>
        
        </li>
        <li><span class="li-head">purdue-level.user.device</span> - Update the Purdue level of device from device store. 
        <ul class="ul-self">
                <li><span class="li-required">mac</span> - Main MAC address of the device. <span class="li-normal">type: string  required: True </span> </li>
                <li><span class="li-required">ip</span> - IP address of the device. <span class="li-normal">type: string  required: False </span> </li>
                <li><span class="li-required">level</span> - Purdue level of the device [1|1.5|2|2.5|3|3.5|4|5|5.5]. <span class="li-normal">type: string  required: True </span> </li>
                
            </ul>
        
        </li>
        <li><span class="li-head">push.switch-controller.fsw-firmware</span> - Push FortiSwitch firmware to the given device. 
        <ul class="ul-self">
                <li><span class="li-required">switch_id</span> - The target device's switch ID. <span class="li-normal">type: string  required: True </span> </li>
                <li><span class="li-required">image_id</span> - FortiSwitch image ID. <span class="li-normal">type: string  required: True </span> </li>
                
            </ul>
        
        </li>
        <li><span class="li-head">push.wifi.firmware</span> - Push FortiAP firmware to the given device. 
        <ul class="ul-self">
                <li><span class="li-required">serial</span> - The target device's serial. <span class="li-normal">type: string  required: True </span> </li>
                <li><span class="li-required">image_id</span> - FortiAP image ID. <span class="li-normal">type: string  required: True </span> </li>
                
            </ul>
        
        </li>
        <li><span class="li-head">quarantine.endpoint-control.registration</span> - Quarantine endpoint by FortiClient UID or MAC. 
        <ul class="ul-self">
                <li><span class="li-required">uid</span> - Single FortiClient UID to quarantine. <span class="li-normal">type: string  required: False </span> </li>
                <li><span class="li-required">mac</span> - Single MAC to quarantine. <span class="li-normal">type: string  required: False </span> </li>
                
            </ul>
        
        </li>
        <li><span class="li-head">read-info.system.certificate</span> - Get certificate information from a certificate string. 
        <ul class="ul-self">
                <li><span class="li-required">value</span> - PEM formatted certificate. <span class="li-normal">type: string  required: True </span> </li>
                
            </ul>
        
        </li>
        <li><span class="li-head">reboot.system.os</span> - Immediately reboot this device. 
        <ul class="ul-self">
                <li><span class="li-required">event_log_message</span> - Message to be logged in event log. <span class="li-normal">type: string  required: False </span> </li>
                
            </ul>
        
        </li>
        <li><span class="li-head">refresh-server.user.fsso</span> - Refresh remote agent group list for all fsso agents. 
        
        </li>
        <li><span class="li-head">refresh.azure.application-list</span> - Update the Azure application list data or get the status of an update. 
        <ul class="ul-self">
                <li><span class="li-required">last_update_time</span> - Timestamp of a previous update request. If this is not provided then it will refresh the Azure application list data. <span class="li-normal">type: int  required: False </span> </li>
                
            </ul>
        
        </li>
        <li><span class="li-head">refresh.system.external-resource</span> - Fetch the external resource file and refresh status for the specified external resource. 
        <ul class="ul-self">
                <li><span class="li-required">mkey</span> - The name of the external resource to query. <span class="li-normal">type: string  required: True </span> </li>
                <li><span class="li-required">check_status_only</span> - Set to true to return only the refresh status. <span class="li-normal">type: boolean  required: False </span> </li>
                <li><span class="li-required">last_connection_time</span> - The timestamp of last connection to the resource; used for checking refresh status. <span class="li-normal">type: int  required: False </span> </li>
                
            </ul>
        
        </li>
        <li><span class="li-head">refresh.user.fortitoken</span> - Refresh a set of FortiTokens by serial number. 
        <ul class="ul-self">
                <li><span class="li-required">tokens</span> - List of FortiToken serial numbers to refresh. If omitted, all tokens will be used. <span class="li-normal">type: array  required: False </span> </li>
                
            </ul>
        
        </li>
        <li><span class="li-head">register-appliance.system.csf</span> - Register appliance to Security Fabric. 
        <ul class="ul-self">
                <li><span class="li-required">type</span> - Appliance type (Example: 'faz'). <span class="li-normal">type: string  required: True </span> </li>
                <li><span class="li-required">mgmt_ip</span> - Management IP or FQDN. <span class="li-normal">type: string  required: True </span> </li>
                <li><span class="li-required">mgmt_port</span> - Management port. <span class="li-normal">type: int  required: False </span> </li>
                <li><span class="li-required">mgmt_url_parameters</span> - Array of URL parameters. Each item is a key/value pair. If provided, the URL parameters will be included in the management IP URL. <span class="li-normal">type: array  required: False </span> </li>
                <li><span class="li-required">serial</span> - Serial number. <span class="li-normal">type: string  required: True </span> </li>
                <li><span class="li-required">hostname</span> - Host name. <span class="li-normal">type: string  required: False </span> </li>
                
            </ul>
        
        </li>
        <li><span class="li-head">register-device.registration.forticloud</span> - Register a device to FortiCloud through FortiGate. Currently FortiSwitches, FortiAPs and FortiExtenders are supported. 
        <ul class="ul-self">
                <li><span class="li-required">serial</span> - Device serial number <span class="li-normal">type: string  required: False </span> </li>
                <li><span class="li-required">email</span> - FortiCloud email. <span class="li-normal">type: string  required: True </span> </li>
                <li><span class="li-required">password</span> - Password. <span class="li-normal">type: string  required: True </span> </li>
                <li><span class="li-required">reseller</span> - Reseller. <span class="li-normal">type: string  required: True </span> </li>
                <li><span class="li-required">reseller_id</span> - Reseller ID. <span class="li-normal">type: int  required: True </span> </li>
                <li><span class="li-required">country</span> - Country. <span class="li-normal">type: string  required: True </span> </li>
                <li><span class="li-required">is_government</span> - Set to true if the end-user is affiliated with a government. <span class="li-normal">type: boolean  required: False </span> </li>
                <li><span class="li-required">agreement_accepted</span> - Set to true if the end-user accepted the agreement. <span class="li-normal">type: boolean  required: False </span> </li>
                
            </ul>
        
        </li>
        <li><span class="li-head">remove.user.device</span> - Remove single or multiple user devices specified by host MAC addresses. 
        <ul class="ul-self">
                <li><span class="li-required">macs</span> - An array of host MAC addresses to be removed. <span class="li-normal">type: array  required: False </span> </li>
                
            </ul>
        
        </li>
        <li><span class="li-head">report.sdwan.link-monitor-metrics</span> - Report the application-level performance metrics collected by other fabric devices. 
        <ul class="ul-self">
                <li><span class="li-required">agent_ip</span> - IPv4 or IPv6 address. <span class="li-normal">type: string  required: True </span> </li>
                <li><span class="li-required">application_name</span> - Destination application that the FMR agent is monitoring. <span class="li-normal">type: string  required: True </span> </li>
                <li><span class="li-required">application_id</span> - Destination application ID based on the FortiGuard Application Control DB. <span class="li-normal">type: int  required: True </span> </li>
                <li><span class="li-required">latency</span> - Latency to report (ms). <span class="li-normal">type: double  required: True </span> </li>
                <li><span class="li-required">jitter</span> - Jitter to report (ms). <span class="li-normal">type: double  required: True </span> </li>
                <li><span class="li-required">packet_loss</span> - Packet loss to report [0, 100]. <span class="li-normal">type: double  required: True </span> </li>
                <li><span class="li-required">ntt</span> - Network transmit time (ms). <span class="li-normal">type: double  required: False </span> </li>
                <li><span class="li-required">srt</span> - Server response time (ms). <span class="li-normal">type: double  required: False </span> </li>
                <li><span class="li-required">application_error</span> - Application errors in the current session. <span class="li-normal">type: double  required: False </span> </li>
                
            </ul>
        
        </li>
        <li><span class="li-head">reset.extender-controller.extender</span> - Reset a specific FortiExtender unit. 
        <ul class="ul-self">
                <li><span class="li-required">id</span> - FortiExtender ID to reset. <span class="li-normal">type: string  required: True </span> </li>
                
            </ul>
        
        </li>
        <li><span class="li-head">reset.firewall.central-snat-map</span> - Reset traffic statistics for all firewall central SNAT policies. 
        
        </li>
        <li><span class="li-head">reset.firewall.consolidated-policy</span> - Reset traffic statistics for all consolidated policies. 
        
        </li>
        <li><span class="li-head">reset.firewall.dnat</span> - Reset hit count statistics for all firewall virtual IPs/servers. 
        
        </li>
        <li><span class="li-head">reset.firewall.multicast-policy</span> - Reset traffic statistics for all IPv4 firewall multicast policies. 
        
        </li>
        <li><span class="li-head">reset.firewall.multicast-policy6</span> - Reset traffic statistics for all IPv6 firewall multicast policies. 
        
        </li>
        <li><span class="li-head">reset.firewall.per-ip-shaper</span> - Reset statistics for all configured firewall per-IP traffic shapers. 
        
        </li>
        <li><span class="li-head">reset.firewall.policy</span> - Reset traffic statistics for all firewall policies. 
        
        </li>
        <li><span class="li-head">reset.firewall.policy6</span> - Reset traffic statistics for all IPv6 policies. 
        
        </li>
        <li><span class="li-head">reset.firewall.shaper</span> - Reset statistics for all configured traffic shapers. 
        
        </li>
        <li><span class="li-head">reset.log.stats</span> - Reset logging statistics for all log devices. 
        
        </li>
        <li><span class="li-head">reset.system.modem</span> - Reset statistics for internal/external configured modem. 
        
        </li>
        <li><span class="li-head">reset.wanopt.history</span> - Reset WAN opt. statistics. 
        
        </li>
        <li><span class="li-head">reset.wanopt.peer_stats</span> - Reset WAN opt peer statistics. 
        
        </li>
        <li><span class="li-head">reset.wanopt.webcache</span> - Reset webcache statistics. 
        
        </li>
        <li><span class="li-head">reset.webcache.stats</span> - Reset all webcache statistics. 
        
        </li>
        <li><span class="li-head">reset.webfilter.category-quota</span> - Reset webfilter quota for user or IP. 
        <ul class="ul-self">
                <li><span class="li-required">profile</span> - Webfilter profile to reset. <span class="li-normal">type: string  required: False </span> </li>
                <li><span class="li-required">user</span> - User or IP to reset with. <span class="li-normal">type: string  required: False </span> </li>
                
            </ul>
        
        </li>
        <li><span class="li-head">reset.wifi.euclid</span> - Reset presence analytics statistics. 
        
        </li>
        <li><span class="li-head">restart.switch-controller.managed-switch</span> - Restart a given FortiSwitch. 
        <ul class="ul-self">
                <li><span class="li-required">mkey</span> - Name of managed FortiSwitch. <span class="li-normal">type: string  required: True </span> </li>
                
            </ul>
        
        </li>
        <li><span class="li-head">restart.system.sniffer</span> - Restart specified packet capture. 
        <ul class="ul-self">
                <li><span class="li-required">mkey</span> - ID of packet capture entry. <span class="li-normal">type: int  required: True </span> </li>
                
            </ul>
        
        </li>
        <li><span class="li-head">restart.wifi.managed_ap</span> - Restart a given FortiAP. 
        <ul class="ul-self">
                <li><span class="li-required">wtpname</span> - FortiAP name. <span class="li-normal">type: string  required: False </span> </li>
                
            </ul>
        
        </li>
        <li><span class="li-head">restore.system.config</span> - Restore system configuration from uploaded file or from USB. 
        <ul class="ul-self">
                <li><span class="li-required">source</span> - Configuration file data source [upload | usb | revision]. <span class="li-normal">type: string  required: True </span> </li>
                <li><span class="li-required">usb_filename</span> - When using 'usb' source: the filename to restore from the connected USB device. <span class="li-normal">type: string  required: False </span> </li>
                <li><span class="li-required">config_id</span> - When using 'revision' source: valid ID of configuration stored on disk to revert to.  <span class="li-normal">type: int  required: False </span> </li>
                <li><span class="li-required">password</span> - Password to decrypt configuration data. <span class="li-normal">type: string  required: False </span> </li>
                <li><span class="li-required">scope</span> - Specify global or VDOM only restore [global | vdom]. <span class="li-normal">type: string  required: True </span> </li>
                <li><span class="li-required">vdom</span> - If 'vdom' scope specified, the name of the VDOM to restore configuration. <span class="li-normal">type: string  required: False </span> </li>
                <li><span class="li-required">confirm_password_mask</span> - True to upload password mask config file. <span class="li-normal">type: boolean  required: False </span> </li>
                <li><span class="li-required">file_content</span> - Provided when uploading a file: base64 encoded file data. Must not contain whitespace or other invalid base64 characters. Must be included in HTTP body. <span class="li-normal">type: string  required: False </span> </li>
                
            </ul>
        
        </li>
        <li><span class="li-head">revoke.system.dhcp</span> - Revoke IPv4 DHCP leases. 
        <ul class="ul-self">
                <li><span class="li-required">ip</span> - Optional list of addresses to revoke. Defaults to all addresses if not provided. <span class="li-normal">type: array  required: False </span> </li>
                
            </ul>
        
        </li>
        <li><span class="li-head">revoke.system.dhcp6</span> - Revoke IPv6 DHCP leases. 
        <ul class="ul-self">
                <li><span class="li-required">ip</span> - Optional list of addresses to revoke. Defaults to all addresses if not provided. <span class="li-normal">type: array  required: False </span> </li>
                
            </ul>
        
        </li>
        <li><span class="li-head">run.system.compliance</span> - Immediately run compliance checks for the selected VDOM. 
        
        </li>
        <li><span class="li-head">run.system.config-script</span> - Run remote config scripts. 
        <ul class="ul-self">
                <li><span class="li-required">remote_script</span> - Name of remote config script to run. <span class="li-normal">type: string  required: True </span> </li>
                
            </ul>
        
        </li>
        <li><span class="li-head">save.system.config</span> - Explicitly save all configuration. 
        
        </li>
        <li><span class="li-head">save.system.config-revision</span> - Create a new config revision checkpoint. 
        <ul class="ul-self">
                <li><span class="li-required">comments</span> - Optional revision comments <span class="li-normal">type: string  required: False </span> </li>
                
            </ul>
        
        </li>
        <li><span class="li-head">scan.wifi.network</span> - When FortiWiFi is in client mode, start a scan for local WiFi networks. 
        
        </li>
        <li><span class="li-head">send-activation.user.fortitoken</span> - Send a FortiToken activation code to a user via SMS or Email. 
        <ul class="ul-self">
                <li><span class="li-required">token</span> - FortiToken serial number. The token must be assigned to a user/admin. <span class="li-normal">type: string  required: True </span> </li>
                <li><span class="li-required">method</span> - Method to send activation code [email|sms]. If not set, SMS will be attempted first, then email. <span class="li-normal">type: string  required: False </span> </li>
                <li><span class="li-required">email</span> - Override email address. <span class="li-normal">type: string  required: False </span> </li>
                <li><span class="li-required">sms_phone</span> - Override SMS phone number. SMS provider must be set in the assigned user/admin. <span class="li-normal">type: string  required: False </span> </li>
                
            </ul>
        
        </li>
        <li><span class="li-head">set-tier-plus.switch-controller.mclag-icl</span> - Setup a tier 2/3 MC-LAG link between a pair of FortiSwitches. 
        <ul class="ul-self">
                <li><span class="li-required">fortilink</span> - FortiLink interface name. <span class="li-normal">type: string  required: True </span> </li>
                <li><span class="li-required">parent_peer1</span> - FortiSwitch ID for MC-LAG parent peer 1. <span class="li-normal">type: string  required: True </span> </li>
                <li><span class="li-required">parent_peer2</span> - FortiSwitch ID for MC-LAG parent peer 2. <span class="li-normal">type: string  required: True </span> </li>
                <li><span class="li-required">peer1</span> - FortiSwitch ID for MC-LAG peer 1. <span class="li-normal">type: string  required: True </span> </li>
                <li><span class="li-required">peer2</span> - FortiSwitch ID for MC-LAG peer 2. <span class="li-normal">type: string  required: True </span> </li>
                <li><span class="li-required">isl_port_group</span> - ISL port group name. <span class="li-normal">type: string  required: True </span> </li>
                
            </ul>
        
        </li>
        <li><span class="li-head">set-tier1.switch-controller.mclag-icl</span> - Setup a tier-1 MC-LAG link between a pair of FortiSwitches. 
        <ul class="ul-self">
                <li><span class="li-required">fortilink</span> - FortiLink interface name. <span class="li-normal">type: string  required: True </span> </li>
                <li><span class="li-required">peer1</span> - FortiSwitch ID for MC-LAG peer 1. <span class="li-normal">type: string  required: True </span> </li>
                <li><span class="li-required">peer2</span> - FortiSwitch ID for MC-LAG peer 2. <span class="li-normal">type: string  required: True </span> </li>
                
            </ul>
        
        </li>
        <li><span class="li-head">set.system.private-data-encryption</span> - Sets private data encryption. 
        <ul class="ul-self">
                <li><span class="li-required">enable</span> - Enable private data encryption. <span class="li-normal">type: boolean  required: True </span> </li>
                <li><span class="li-required">password</span> - Admin password. <span class="li-normal">type: string  required: False </span> </li>
                
            </ul>
        
        </li>
        <li><span class="li-head">set.system.time</span> - Sets current system time stamp. 
        <ul class="ul-self">
                <li><span class="li-required">year</span> - Specifies the year for setting/updating time manually. <span class="li-normal">type: int  required: True </span> </li>
                <li><span class="li-required">month</span> - Specifies the month (0 - 11) for setting/updating time manually. <span class="li-normal">type: int  required: True </span> </li>
                <li><span class="li-required">day</span> - Specifies the day for setting/updating time manually. <span class="li-normal">type: int  required: True </span> </li>
                <li><span class="li-required">hour</span> - Specifies the hour (0 - 23) for setting/updating time manually. <span class="li-normal">type: int  required: True </span> </li>
                <li><span class="li-required">minute</span> - Specifies the minute (0 - 59) for setting/updating time manually. <span class="li-normal">type: int  required: True </span> </li>
                <li><span class="li-required">second</span> - Specifies the second (0 - 59) for setting/updating time manually. <span class="li-normal">type: int  required: True </span> </li>
                
            </ul>
        
        </li>
        <li><span class="li-head">set_status.wifi.managed_ap</span> - Update administrative state for a given FortiAP (enable or disable authorization). 
        <ul class="ul-self">
                <li><span class="li-required">wtpname</span> - FortiAP name. <span class="li-normal">type: string  required: False </span> </li>
                <li><span class="li-required">admin</span> - New FortiAP administrative state [enable|disable|discovered]. <span class="li-normal">type: string  required: False </span> </li>
                
            </ul>
        
        </li>
        <li><span class="li-head">set_status.wifi.rogue_ap</span> - Mark detected APs as rogue APs. 
        <ul class="ul-self">
                <li><span class="li-required">bssid</span> - List of rogue AP MAC addresses. <span class="li-normal">type: array  required: False </span> </li>
                <li><span class="li-required">ssid</span> - Corresponding list of rogue AP SSIDs. <span class="li-normal">type: array  required: False </span> </li>
                <li><span class="li-required">status</span> - Status to assign matching APs [unclassified|rogue|accepted|suppressed]. <span class="li-normal">type: string  required: False </span> </li>
                
            </ul>
        
        </li>
        <li><span class="li-head">shutdown.system.os</span> - Immediately shutdown this device. 
        <ul class="ul-self">
                <li><span class="li-required">event_log_message</span> - Message to be logged in event log. <span class="li-normal">type: string  required: False </span> </li>
                
            </ul>
        
        </li>
        <li><span class="li-head">sms.user.guest</span> - Sent guest login details via SMS. 
        <ul class="ul-self">
                <li><span class="li-required">group</span> - Guest group name. <span class="li-normal">type: string  required: True </span> </li>
                <li><span class="li-required">guest</span> - Guest user IDs. <span class="li-normal">type: array  required: True </span> </li>
                
            </ul>
        
        </li>
        <li><span class="li-head">soft-reset-neighbor.router.bgp</span> - BGP Neighbor soft reset. 
        <ul class="ul-self">
                <li><span class="li-required">ip</span> - IPv4 or IPv6 address of neighbor to perform soft reset on. <span class="li-normal">type: string  required: True </span> </li>
                
            </ul>
        
        </li>
        <li><span class="li-head">speed-test-trigger.system.interface</span> - Run a speed-test on the given interface. 
        <ul class="ul-self">
                <li><span class="li-required">mkey</span> - Name of the interface. <span class="li-normal">type: string  required: True </span> </li>
                
            </ul>
        
        </li>
        <li><span class="li-head">start.forticonverter.download</span> - Start download from FortiConverter for processed config. 
        <ul class="ul-self">
                <li><span class="li-required">ticket_id</span> - Service ticket ID. <span class="li-normal">type: string  required: True </span> </li>
                <li><span class="li-required">extension</span> - File extension [pdf|conf]. <span class="li-normal">type: string  required: True </span> </li>
                
            </ul>
        
        </li>
        <li><span class="li-head">start.network.debug-flow</span> - Start debug flow packet capture. 
        <ul class="ul-self">
                <li><span class="li-required">num_packets</span> - Number of packets. <span class="li-normal">type: int  required: True </span> </li>
                <li><span class="li-required">ipv6</span> - Whether we are debugging IPv6 traffic. <span class="li-normal">type: boolean  required: True </span> </li>
                <li><span class="li-required">negate</span> - Inverse IPv4 or IPv6 filter. <span class="li-normal">type: boolean  required: False </span> </li>
                <li><span class="li-required">addr_from</span> - IPv4 or IPv6 address start of range. <span class="li-normal">type: string  required: False </span> </li>
                <li><span class="li-required">addr_to</span> - IPv4 or IPv6 address end of range. <span class="li-normal">type: string  required: False </span> </li>
                <li><span class="li-required">daddr_from</span> - Destination IPv4 or IPv6 address start of range. <span class="li-normal">type: string  required: False </span> </li>
                <li><span class="li-required">daddr_to</span> - Destination IPv4 or IPv6 address end of range. <span class="li-normal">type: string  required: False </span> </li>
                <li><span class="li-required">saddr_from</span> - Source IPv4 or IPv6 address start of range. <span class="li-normal">type: string  required: False </span> </li>
                <li><span class="li-required">saddr_to</span> - Source IPv4 or IPv6 address end of range. <span class="li-normal">type: string  required: False </span> </li>
                <li><span class="li-required">port_from</span> - Port from. <span class="li-normal">type: int  required: False </span> </li>
                <li><span class="li-required">port_to</span> - Port to. <span class="li-normal">type: int  required: False </span> </li>
                <li><span class="li-required">dport_from</span> - Destination port from. <span class="li-normal">type: int  required: False </span> </li>
                <li><span class="li-required">dport_to</span> - Destination port to. <span class="li-normal">type: int  required: False </span> </li>
                <li><span class="li-required">sport_from</span> - Source port from. <span class="li-normal">type: int  required: False </span> </li>
                <li><span class="li-required">sport_to</span> - Source port to. <span class="li-normal">type: int  required: False </span> </li>
                <li><span class="li-required">proto</span> - Protocol number. <span class="li-normal">type: int  required: False </span> </li>
                
            </ul>
        
        </li>
        <li><span class="li-head">start.system.fsck</span> - Set file system check flag so that it will be executed on next device reboot. 
        
        </li>
        <li><span class="li-head">start.system.sniffer</span> - Start specified packet capture. 
        <ul class="ul-self">
                <li><span class="li-required">mkey</span> - ID of packet capture entry. <span class="li-normal">type: int  required: True </span> </li>
                
            </ul>
        
        </li>
        <li><span class="li-head">start.system.usb-log</span> - Start backup of logs from current VDOM to USB drive. 
        
        </li>
        <li><span class="li-head">start.wifi.spectrum</span> - Start spectrum analysis for a specific FortiAP for a duration of time. 
        <ul class="ul-self">
                <li><span class="li-required">wtp_id</span> - FortiAP ID. <span class="li-normal">type: string  required: True </span> </li>
                <li><span class="li-required">radio_id</span> - Radio ID. <span class="li-normal">type: int  required: True </span> </li>
                <li><span class="li-required">channels</span> - Channels. <span class="li-normal">type: array  required: True </span> </li>
                <li><span class="li-required">duration</span> - Duration in seconds. <span class="li-normal">type: int  required: True </span> </li>
                
            </ul>
        
        </li>
        <li><span class="li-head">start.wifi.vlan-probe</span> - Start a VLAN probe. 
        <ul class="ul-self">
                <li><span class="li-required">ap_interface</span> - FortiAP interface to send the probe on. <span class="li-normal">type: int  required: True </span> </li>
                <li><span class="li-required">wtp</span> - FortiAP ID. <span class="li-normal">type: string  required: True </span> </li>
                <li><span class="li-required">start_vlan_id</span> - The starting VLAN ID for the probe. <span class="li-normal">type: int  required: True </span> </li>
                <li><span class="li-required">end_vlan_id</span> - The ending VLAN ID for the probe. <span class="li-normal">type: int  required: True </span> </li>
                <li><span class="li-required">retries</span> - Number of times to retry a probe for a particular VLAN. <span class="li-normal">type: int  required: True </span> </li>
                <li><span class="li-required">timeout</span> - Timeout duration (in seconds) to wait for a VLAN probe response. <span class="li-normal">type: int  required: True </span> </li>
                
            </ul>
        
        </li>
        <li><span class="li-head">stop.network.debug-flow</span> - Stop debug flow packet capture. 
        
        </li>
        <li><span class="li-head">stop.system.sniffer</span> - Stop specified packet capture. 
        <ul class="ul-self">
                <li><span class="li-required">mkey</span> - ID of packet capture entry. <span class="li-normal">type: int  required: True </span> </li>
                
            </ul>
        
        </li>
        <li><span class="li-head">stop.system.usb-log</span> - Stop backup of logs to USB drive. 
        
        </li>
        <li><span class="li-head">stop.wifi.spectrum</span> - Stop spectrum analysis for a specific FortiAP. 
        <ul class="ul-self">
                <li><span class="li-required">wtp_id</span> - FortiAP ID. <span class="li-normal">type: string  required: True </span> </li>
                <li><span class="li-required">radio_id</span> - Radio ID. <span class="li-normal">type: int  required: True </span> </li>
                
            </ul>
        
        </li>
        <li><span class="li-head">stop.wifi.vlan-probe</span> - Stop a VLAN probe. 
        <ul class="ul-self">
                <li><span class="li-required">ap_interface</span> - FortiAP interface to send the probe on. <span class="li-normal">type: int  required: True </span> </li>
                <li><span class="li-required">wtp</span> - FortiAP ID. <span class="li-normal">type: string  required: True </span> </li>
                
            </ul>
        
        </li>
        <li><span class="li-head">submit.forticonverter.intf-mapping</span> - Submit physical interface mapping to FortiConverter. 
        <ul class="ul-self">
                <li><span class="li-required">intf_mapping</span> - Interface mapping from source to target. <span class="li-normal">type: object  required: True </span> </li>
                <li><span class="li-required">ticket_id</span> - Service ticket ID. <span class="li-normal">type: string  required: True </span> </li>
                
            </ul>
        
        </li>
        <li><span class="li-head">submit.forticonverter.mgmt-intf</span> - Submit management interface details to FortiConverter. 
        <ul class="ul-self">
                <li><span class="li-required">intf_details</span> - Management interface details. <span class="li-normal">type: object  required: True </span> </li>
                <li><span class="li-required">ticket_id</span> - Service ticket ID. <span class="li-normal">type: string  required: True </span> </li>
                
            </ul>
        
        </li>
        <li><span class="li-head">submit.forticonverter.notes</span> - Submit contact details and conversion notes to FortiConverter. 
        <ul class="ul-self">
                <li><span class="li-required">ticket_id</span> - Service ticket ID. <span class="li-normal">type: string  required: True </span> </li>
                <li><span class="li-required">contact_name</span> - Contact name. <span class="li-normal">type: string  required: True </span> </li>
                <li><span class="li-required">contact_email</span> - Contact email. <span class="li-normal">type: string  required: True </span> </li>
                <li><span class="li-required">contact_phone</span> - Contact phone. <span class="li-normal">type: string  required: True </span> </li>
                <li><span class="li-required">notes</span> - Conversion notes. <span class="li-normal">type: string  required: False </span> </li>
                
            </ul>
        
        </li>
        <li><span class="li-head">submit.forticonverter.ticket</span> - Submit FortiConverter ticket. 
        <ul class="ul-self">
                <li><span class="li-required">ticket_id</span> - Service ticket ID. <span class="li-normal">type: string  required: True </span> </li>
                
            </ul>
        
        </li>
        <li><span class="li-head">system.change-password</span> - Save admin and guest-admin passwords. 
        <ul class="ul-self">
                <li><span class="li-required">mkey</span> - User ID for password change. <span class="li-normal">type: string  required: False </span> </li>
                <li><span class="li-required">old_password</span> - Old password. <span class="li-normal">type: string  required: False </span> </li>
                <li><span class="li-required">new_password</span> - New password. <span class="li-normal">type: string  required: True </span> </li>
                
            </ul>
        
        </li>
        <li><span class="li-head">system.disconnect-admins</span> - Disconnects logged in administrators. 
        <ul class="ul-self">
                <li><span class="li-required">id</span> - Admin ID <span class="li-normal">type: int  required: False </span> </li>
                <li><span class="li-required">method</span> - Login method used to connect admin to FortiGate. <span class="li-normal">type: string  required: False </span> </li>
                <li><span class="li-required">admins</span> - List of objects with admin id and method. <span class="li-normal">type: array  required: True </span> </li>
                
            </ul>
        
        </li>
        <li><span class="li-head">system.password-policy-conform</span> - Check whether password conforms to the password policy. 
        <ul class="ul-self">
                <li><span class="li-required">mkey</span> - User ID for password change. <span class="li-normal">type: string  required: False </span> </li>
                <li><span class="li-required">apply_to</span> - Password Policy ID. <span class="li-normal">type: string  required: False </span> </li>
                <li><span class="li-required">password</span> - Password. <span class="li-normal">type: string  required: False </span> </li>
                <li><span class="li-required">old_password</span> - Old password. <span class="li-normal">type: string  required: False </span> </li>
                
            </ul>
        
        </li>
        <li><span class="li-head">test-availability.system.fortiguard</span> - Test availability of FortiGuard services. 
        <ul class="ul-self">
                <li><span class="li-required">protocol</span> - Protocol to check. [https | udp | http] <span class="li-normal">type: string  required: True </span> </li>
                <li><span class="li-required">port</span> - Port to check. <span class="li-normal">type: int  required: True </span> </li>
                <li><span class="li-required">service</span> - Service to check. [emailfilter | webfilter] <span class="li-normal">type: string  required: True </span> </li>
                
            </ul>
        
        </li>
        <li><span class="li-head">test-connect.user.radius</span> - Test the connectivity of the given RADIUS server and, optionally, the validity of a username & password. 
        <ul class="ul-self">
                <li><span class="li-required">mkey</span> - Name of FortiGate's RADIUS object whose settings to test. <span class="li-normal">type: string  required: False </span> </li>
                <li><span class="li-required">ordinal</span> - If 'mkey' is provided, the server-secret pair to use from the object: 'primary', 'secondary' or 'tertiary'. Defaults to 'primary'. <span class="li-normal">type: string  required: False </span> </li>
                <li><span class="li-required">server</span> - Host name or IP of a RADIUS server. If 'mkey' is provided, this overrides the 'server' value in the object. <span class="li-normal">type: string  required: False </span> </li>
                <li><span class="li-required">secret</span> - Secret password for the RADIUS server. If 'mkey' is provided, this overrides the 'secret' value in the object. <span class="li-normal">type: string  required: False </span> </li>
                <li><span class="li-required">auth_type</span> - Authentication protocol to use [auto|ms_chap_v2|ms_chap|chap|pap]. If 'mkey' is provided, this overrides the 'auth-type' value in the object. <span class="li-normal">type: string  required: False </span> </li>
                <li><span class="li-required">user</span> - User name whose access to check. <span class="li-normal">type: string  required: False </span> </li>
                <li><span class="li-required">password</span> - User's password. <span class="li-normal">type: string  required: False </span> </li>
                
            </ul>
        
        </li>
        <li><span class="li-head">test.system.automation-stitch</span> - Triggers an automation stitch for testing purposes. 
        <ul class="ul-self">
                <li><span class="li-required">mkey</span> - ID of automation stitch to trigger. <span class="li-normal">type: string  required: True </span> </li>
                <li><span class="li-required">log</span> - Message to store in the log buffer when triggering an event. For example, "logid=\"32102\" eventtime=1528840790000000000 logdesc=\"Sample description\" msg=\"Sample message\"". This parameter is required for the 'event-log' event type. For the test to run, the 'logid' argument value must match the trigger-defined value. If 'logid' is not provided, the test will use the trigger-defined value. <span class="li-normal">type: string  required: False </span> </li>
                
            </ul>
        
        </li>
        <li><span class="li-head">test.user.tacacs-plus</span> - Test the connectivity of the given TACACS+ server. 
        <ul class="ul-self">
                <li><span class="li-required">mkey</span> - Name of FortiGate's TACACS+ object whose settings to test. <span class="li-normal">type: string  required: False </span> </li>
                <li><span class="li-required">ordinal</span> - If 'mkey' is provided, the server-key pair to use from the object: 'primary', 'secondary' or 'tertiary'. Defaults to 'primary'. <span class="li-normal">type: string  required: False </span> </li>
                <li><span class="li-required">server</span> - Host name of IP of a TACACS+ server. If 'mkey' is provided, this overrides the 'server' value in the object. <span class="li-normal">type: string  required: False </span> </li>
                <li><span class="li-required">secret</span> - Secret key for the TACACS+ server. If 'mkey' is provided, this overrides the 'key' value in the object. <span class="li-normal">type: string  required: False </span> </li>
                <li><span class="li-required">port</span> - Port number of the TACACS+ server. If 'mkey' is provided, this overrides the 'port' value in the object. Defaults to 49. <span class="li-normal">type: int  required: False </span> </li>
                <li><span class="li-required">source_ip</span> - Source IP for communications to TACACS+ server. If 'mkey' is provided, this overrides the 'source-ip' value in the object. <span class="li-normal">type: string  required: False </span> </li>
                
            </ul>
        
        </li>
        <li><span class="li-head">toggle-vdom-mode.system.admin</span> - Toggles VDOM mode on/off. Enables or disables VDOM mode if it is disabled or enabled respectively. 
        
        </li>
        <li><span class="li-head">transfer.registration.forticare</span> - Transfer to a new FortiCare account. 
        <ul class="ul-self">
                <li><span class="li-required">email</span> - Account email. <span class="li-normal">type: string  required: True </span> </li>
                <li><span class="li-required">password</span> - Account password. <span class="li-normal">type: string  required: True </span> </li>
                <li><span class="li-required">old_email</span> - Old account email. <span class="li-normal">type: string  required: True </span> </li>
                <li><span class="li-required">old_password</span> - Old account password. <span class="li-normal">type: string  required: True </span> </li>
                <li><span class="li-required">is_government</span> - Set to true if the end-user is affiliated with a government. <span class="li-normal">type: boolean  required: False </span> </li>
                
            </ul>
        
        </li>
        <li><span class="li-head">trial.user.fortitoken-cloud</span> - Activate FortiToken Cloud trial. 
        
        </li>
        <li><span class="li-head">trigger.system.security-rating</span> - Run a Security Rating report. 
        <ul class="ul-self">
                <li><span class="li-required">report_type</span> - Security Rating report to run, run all reports when unspecified. <span class="li-normal">type: string  required: False </span> </li>
                <li><span class="li-required">report_types</span> - Multiple Security Rating reports to run, run all reports when unspecified. <span class="li-normal">type: array  required: False </span> </li>
                
            </ul>
        
        </li>
        <li><span class="li-head">tunnel_down.vpn.ipsec</span> - Bring down a specific IPsec VPN tunnel. 
        <ul class="ul-self">
                <li><span class="li-required">p1name</span> - IPsec phase1 name. <span class="li-normal">type: string  required: True </span> </li>
                <li><span class="li-required">p2name</span> - IPsec phase2 name. <span class="li-normal">type: string  required: True </span> </li>
                <li><span class="li-required">p2serial</span> - IPsec phase2 serial. <span class="li-normal">type: int  required: False </span> </li>
                
            </ul>
        
        </li>
        <li><span class="li-head">tunnel_reset_stats.vpn.ipsec</span> - Reset statistics for a specific IPsec VPN tunnel. 
        <ul class="ul-self">
                <li><span class="li-required">p1name</span> - IPsec phase1 name. <span class="li-normal">type: string  required: True </span> </li>
                
            </ul>
        
        </li>
        <li><span class="li-head">tunnel_up.vpn.ipsec</span> - Bring up a specific IPsec VPN tunnel. 
        <ul class="ul-self">
                <li><span class="li-required">p1name</span> - IPsec phase1 name. <span class="li-normal">type: string  required: True </span> </li>
                <li><span class="li-required">p2name</span> - IPsec phase2 name. <span class="li-normal">type: string  required: True </span> </li>
                <li><span class="li-required">p2serial</span> - IPsec phase2 serial. <span class="li-normal">type: int  required: False </span> </li>
                
            </ul>
        
        </li>
        <li><span class="li-head">unblock.endpoint-control.registration</span> - Unblock endpoint by FortiClient UID or MAC. 
        <ul class="ul-self">
                <li><span class="li-required">uid</span> - Single FortiClient UID to unblock. <span class="li-normal">type: string  required: False </span> </li>
                <li><span class="li-required">mac</span> - Single MAC to unblock. <span class="li-normal">type: string  required: False </span> </li>
                
            </ul>
        
        </li>
        <li><span class="li-head">unquarantine.endpoint-control.registration</span> - Unquarantine endpoint by FortiClient UID or MAC. 
        <ul class="ul-self">
                <li><span class="li-required">uid</span> - Single FortiClient UID to unquarantine. <span class="li-normal">type: string  required: False </span> </li>
                <li><span class="li-required">mac</span> - Single MAC to unquarantine. <span class="li-normal">type: string  required: False </span> </li>
                
            </ul>
        
        </li>
        <li><span class="li-head">unverify-cert.endpoint-control.ems</span> - Unverify EMS server certificate for a specific EMS. 
        <ul class="ul-self">
                <li><span class="li-required">ems_id</span> - EMS server ID (as defined in CLI table endpoint-control.fctems). <span class="li-normal">type: int  required: True </span> </li>
                <li><span class="li-required">scope</span> - Scope from which to retrieve EMS certificate status [vdom*|global]. <span class="li-normal">type: string  required: False </span> </li>
                
            </ul>
        
        </li>
        <li><span class="li-head">update-comments.system.config-revision</span> - Updates comments for a system configuration file. 
        <ul class="ul-self">
                <li><span class="li-required">config_id</span> - Configuration id. <span class="li-normal">type: int  required: False </span> </li>
                <li><span class="li-required">comments</span> - Configuration comments. <span class="li-normal">type: string  required: False </span> </li>
                
            </ul>
        
        </li>
        <li><span class="li-head">update-global-label.firewall.policy</span> - Update the global-label of group starting with the provided leading policy ID. 
        <ul class="ul-self">
                <li><span class="li-required">policyid</span> - Leading policy ID of the group to update. <span class="li-normal">type: string  required: True </span> </li>
                <li><span class="li-required">current-label</span> - The current global-label of the group. If not provided, will assume the current group's label is empty string. <span class="li-normal">type: string  required: False </span> </li>
                <li><span class="li-required">new-label</span> - The new global-label of the group. If not provided, the current group's label will be deleted <span class="li-normal">type: string  required: False </span> </li>
                
            </ul>
        
        </li>
        <li><span class="li-head">update-global-label.firewall.security-policy</span> - Update the global-label of group starting with the provided leading policy ID. 
        <ul class="ul-self">
                <li><span class="li-required">policyid</span> - Leading policy ID of the group to update. <span class="li-normal">type: string  required: True </span> </li>
                <li><span class="li-required">current-label</span> - The current global-label of the group. If not provided, will assume the current group's label is empty string. <span class="li-normal">type: string  required: False </span> </li>
                <li><span class="li-required">new-label</span> - The new global-label of the group. If not provided, the current group's label will be deleted <span class="li-normal">type: string  required: False </span> </li>
                
            </ul>
        
        </li>
        <li><span class="li-head">update.forticonverter.eligibility</span> - Force an immediate request to update eligibility and ticket info. 
        
        </li>
        <li><span class="li-head">update.forticonverter.intf-list</span> - Force an immediate request to update source interface list. 
        
        </li>
        <li><span class="li-head">update.forticonverter.sn-list</span> - Force an immediate request to update source device serials. 
        
        </li>
        <li><span class="li-head">update.forticonverter.submitted-info</span> - Force an immediate request to update all submitted info. 
        
        </li>
        <li><span class="li-head">update.switch-controller.isl-lockdown</span> - Enable/disable ISL lockdown. 
        <ul class="ul-self">
                <li><span class="li-required">fortilink</span> - FortiLink interface name. <span class="li-normal">type: string  required: True </span> </li>
                <li><span class="li-required">status</span> - To enable or disable lockdown. [enable|disable] <span class="li-normal">type: string  required: True </span> </li>
                
            </ul>
        
        </li>
        <li><span class="li-head">update.switch-controller.managed-switch</span> - Update administrative state for a given FortiSwitch (enable or disable authorization). 
        <ul class="ul-self">
                <li><span class="li-required">mkey</span> - FortiSwitch name. <span class="li-normal">type: string  required: False </span> </li>
                <li><span class="li-required">admin</span> - New FortiSwitch administrative state [enable|disable|discovered]. <span class="li-normal">type: string  required: False </span> </li>
                
            </ul>
        
        </li>
        <li><span class="li-head">update.system.fortiguard</span> - Immediately update status for FortiGuard services. 
        
        </li>
        <li><span class="li-head">update.system.ha-peer</span> - Update configuration of peer in HA cluster. 
        <ul class="ul-self">
                <li><span class="li-required">serial_no</span> - Serial number of the HA member. <span class="li-normal">type: string  required: True </span> </li>
                <li><span class="li-required">vcluster_id</span> - Virtual cluster number. <span class="li-normal">type: int  required: False </span> </li>
                <li><span class="li-required">priority</span> - Priority to assign to HA member. <span class="li-normal">type: int  required: False </span> </li>
                <li><span class="li-required">hostname</span> - Name to assign the HA member. <span class="li-normal">type: string  required: False </span> </li>
                
            </ul>
        
        </li>
        <li><span class="li-head">update.system.modem</span> - Update supported modem list from FortiGuard. 
        
        </li>
        <li><span class="li-head">update.system.sdn-connector</span> - Update an SDN connector's connection status. 
        <ul class="ul-self">
                <li><span class="li-required">mkey</span> - SDN connector name. <span class="li-normal">type: string  required: True </span> </li>
                
            </ul>
        
        </li>
        <li><span class="li-head">update.web-ui.custom-language</span> - Update custom language file to this Fortigate. 
        <ul class="ul-self">
                <li><span class="li-required">mkey</span> - Name of custom language entry. <span class="li-normal">type: string  required: True </span> </li>
                <li><span class="li-required">lang_name</span> - New name of custom language entry. <span class="li-normal">type: string  required: False </span> </li>
                <li><span class="li-required">lang_comments</span> - Comments of custom language entry. <span class="li-normal">type: string  required: False </span> </li>
                <li><span class="li-required">file_content</span> - Provided when uploading a file: base64 encoded file data. Must not contain whitespace or other invalid base64 characters. Must be included in HTTP body. <span class="li-normal">type: string  required: False </span> </li>
                
            </ul>
        
        </li>
        <li><span class="li-head">upgrade.extender-controller.extender</span> - Upgrade FortiExtender. 
        <ul class="ul-self">
                <li><span class="li-required">id</span> - FortiExtender ID to upgrade. <span class="li-normal">type: string  required: True </span> </li>
                <li><span class="li-required">file_content</span> - Provided when uploading a file: base64 encoded file data. Must not contain whitespace or other invalid base64 characters. Must be included in HTTP body. <span class="li-normal">type: string  required: False </span> </li>
                
            </ul>
        
        </li>
        <li><span class="li-head">upgrade.license.database</span> - Upgrade or downgrade UTM engine or signature package (IPS/AntiVirus/Application Control/Industrial database/Security Rating/Internet Service Database) using uploaded file. 
        <ul class="ul-self">
                <li><span class="li-required">db_name</span> - Security service database name [ips|appctrl|industrial_db|antivirus|security_rating|isdb|iotddb] <span class="li-normal">type: string  required: True </span> </li>
                <li><span class="li-required">confirm_not_signed</span> - Confirm whether unsigned pkg files may be uploaded. <span class="li-normal">type: boolean  required: False </span> </li>
                <li><span class="li-required">confirm_not_ga_certified</span> - Confirm whether non GA-certified pkg files may be uploaded. <span class="li-normal">type: boolean  required: False </span> </li>
                <li><span class="li-required">file_id</span> - File id of existing pkg file from a previous upload. <span class="li-normal">type: string  required: False </span> </li>
                <li><span class="li-required">file_content</span> - Provided when uploading a file: base64 encoded file data. Must not contain whitespace or other invalid base64 characters. Must be included in HTTP body. <span class="li-normal">type: string  required: False </span> </li>
                
            </ul>
        
        </li>
        <li><span class="li-head">upgrade.system.firmware</span> - Upgrade firmware image on this device. 
        <ul class="ul-self">
                <li><span class="li-required">source</span> - Firmware file data source [upload|usb|fortiguard|url]. <span class="li-normal">type: string  required: True </span> </li>
                <li><span class="li-required">url</span> - URL where the image should be retrieved from. <span class="li-normal">type: string  required: False </span> </li>
                <li><span class="li-required">passphrase</span> - Image encryption passphrase. <span class="li-normal">type: string  required: False </span> </li>
                <li><span class="li-required">force</span> - Bypass signature and validity checking. <span class="li-normal">type: boolean  required: False </span> </li>
                <li><span class="li-required">filename</span> - Name of file on USB disk to upgrade to, or ID from FortiGuard available firmware. <span class="li-normal">type: string  required: False </span> </li>
                <li><span class="li-required">format_partition</span> - Set to true to format boot partition before upgrade. <span class="li-normal">type: boolean  required: False </span> </li>
                <li><span class="li-required">ignore_invalid_signature</span> - Set to true to allow upgrade of firmware images with invalid signatures. <span class="li-normal">type: boolean  required: False </span> </li>
                <li><span class="li-required">file_id</span> - File ID of the uploaded firmware image to allow upgrade of firmware images with invalid signatures. <span class="li-normal">type: string  required: False </span> </li>
                <li><span class="li-required">ignore_admin_lockout_upon_downgrade</span> - Set to true to allow dowgrading if the firmware doesn't support safer password and there is at least 1 admin that will be locked out after upgrade. <span class="li-normal">type: boolean  required: False </span> </li>
                <li><span class="li-required">file_content</span> - Provided when uploading a file: base64 encoded file data. Must not contain whitespace or other invalid base64 characters. Must be included in HTTP body. <span class="li-normal">type: string  required: False </span> </li>
                
            </ul>
        
        </li>
        <li><span class="li-head">upgrade.system.lte-modem</span> - Upgrade LTE modem firmware image on this device using uploaded files. 
        
        </li>
        <li><span class="li-head">upload.forticonverter.config</span> - Upload config from target FortiGate to FortiConverter. 
        <ul class="ul-self">
                <li><span class="li-required">ticket_id</span> - Service ticket ID. <span class="li-normal">type: string  required: True </span> </li>
                <li><span class="li-required">file_content</span> - Provided when uploading a file: base64 encoded file data. Must not contain whitespace or other invalid base64 characters. Must be included in HTTP body. <span class="li-normal">type: string  required: False </span> </li>
                
            </ul>
        
        </li>
        <li><span class="li-head">upload.switch-controller.fsw-firmware</span> - Upload FortiSwitch firmware to the management FortiGate and then push to target FortiSwitches. 
        <ul class="ul-self">
                <li><span class="li-required">switch_ids</span> - The target device's switch ID. <span class="li-normal">type: string  required: False </span> </li>
                <li><span class="li-required">file_content</span> - Provided when uploading a file: base64 encoded file data. Must not contain whitespace or other invalid base64 characters. Must be included in HTTP body. <span class="li-normal">type: string  required: False </span> </li>
                
            </ul>
        
        </li>
        <li><span class="li-head">upload.system.config-script</span> - Upload and run a new configuration script file. 
        <ul class="ul-self">
                <li><span class="li-required">filename</span> - Name of configuration script file. <span class="li-normal">type: string  required: False </span> </li>
                <li><span class="li-required">file_content</span> - Provided when uploading a file: base64 encoded file data. Must not contain whitespace or other invalid base64 characters. Must be included in HTTP body. <span class="li-normal">type: string  required: False </span> </li>
                
            </ul>
        
        </li>
        <li><span class="li-head">upload.system.hscalefw-license</span> - Update Hyperscale firewall license for hardware acceleration using license key. 
        <ul class="ul-self">
                <li><span class="li-required">license_key</span> - License key. Format:0000-0000-0000-0000-0000-0000-00. <span class="li-normal">type: string  required: True </span> </li>
                
            </ul>
        
        </li>
        <li><span class="li-head">upload.system.lte-modem</span> - Upload the modem firmware upgrade files. 
        <ul class="ul-self">
                <li><span class="li-required">filename</span> - Firmware file being uploaded. <span class="li-normal">type: string  required: False </span> </li>
                <li><span class="li-required">file_content</span> - Provided when uploading a file: base64 encoded file data. Must not contain whitespace or other invalid base64 characters. Must be included in HTTP body. <span class="li-normal">type: string  required: False </span> </li>
                
            </ul>
        
        </li>
        <li><span class="li-head">upload.system.vmlicense</span> - Update VM license using uploaded file. Reboots immediately if successful. 
        <ul class="ul-self">
                <li><span class="li-required">file_content</span> - Provided when uploading a file: base64 encoded file data. Must not contain whitespace or other invalid base64 characters. Must be included in HTTP body. <span class="li-normal">type: string  required: False </span> </li>
                
            </ul>
        
        </li>
        <li><span class="li-head">upload.webproxy.pacfile</span> - Upload webproxy PAC file. 
        <ul class="ul-self">
                <li><span class="li-required">filename</span> - Name of PAC file. <span class="li-normal">type: string  required: False </span> </li>
                <li><span class="li-required">file_content</span> - Provided when uploading a file: base64 encoded file data. Must not contain whitespace or other invalid base64 characters. Must be included in HTTP body. <span class="li-normal">type: string  required: False </span> </li>
                
            </ul>
        
        </li>
        <li><span class="li-head">upload.wifi.firmware</span> - Upload FortiAP firmware to the management FortiGate and then push to target FortiAPs. 
        <ul class="ul-self">
                <li><span class="li-required">serials</span> - The target device's serial. <span class="li-normal">type: string  required: False </span> </li>
                <li><span class="li-required">file_content</span> - Provided when uploading a file: base64 encoded file data. Must not contain whitespace or other invalid base64 characters. Must be included in HTTP body. <span class="li-normal">type: string  required: False </span> </li>
                
            </ul>
        
        </li>
        <li><span class="li-head">upload.wifi.region-image</span> - Saves a floorplan/region image to an existing region. 
        <ul class="ul-self">
                <li><span class="li-required">region_name</span> - Region name to save image to. <span class="li-normal">type: string  required: True </span> </li>
                <li><span class="li-required">image_type</span> - MIME type of the image (png|jpeg|gif). <span class="li-normal">type: string  required: True </span> </li>
                <li><span class="li-required">file_content</span> - Provided when uploading a file: base64 encoded file data. Must not contain whitespace or other invalid base64 characters. Must be included in HTTP body. <span class="li-normal">type: string  required: False </span> </li>
                
            </ul>
        
        </li>
        <li><span class="li-head">user.password-policy-conform</span> - Check if password adheres to local user password policy. 
        <ul class="ul-self">
                <li><span class="li-required">username</span> - User name. <span class="li-normal">type: string  required: False </span> </li>
                <li><span class="li-required">password</span> - Password. <span class="li-normal">type: string  required: True </span> </li>
                
            </ul>
        
        </li>
        <li><span class="li-head">utm.rating-lookup</span> - Lookup FortiGuard rating for a specific URL. 
        <ul class="ul-self">
                <li><span class="li-required">url</span> - List of URLs to query. <span class="li-normal">type: array  required: False </span> </li>
                <li><span class="li-required">lang</span> - Language for the rating response. <span class="li-normal">type: string  required: False </span> </li>
                
            </ul>
        
        </li>
        <li><span class="li-head">validate-gcp-key.system.sdn-connector</span> - Validate a string representing a private key from GCP in PEM format. 
        <ul class="ul-self">
                <li><span class="li-required">private-key</span> - Private key in PEM format. <span class="li-normal">type: string  required: True </span> </li>
                
            </ul>
        
        </li>
        <li><span class="li-head">verify-cert.endpoint-control.ems</span> - Verify EMS server certificate for a specific EMS. 
        <ul class="ul-self">
                <li><span class="li-required">ems_id</span> - EMS server ID (as defined in CLI table endpoint-control.fctems). <span class="li-normal">type: int  required: True </span> </li>
                <li><span class="li-required">scope</span> - Scope from which to verify EMS [vdom*|global]. <span class="li-normal">type: string  required: False </span> </li>
                <li><span class="li-required">fingerprint</span> - EMS server certificate fingerprint to check with. <span class="li-normal">type: string  required: True </span> </li>
                
            </ul>
        
        </li>
        <li><span class="li-head">wake-on-lan.system.interface</span> - Send wake on lan packet to device. 
        <ul class="ul-self">
                <li><span class="li-required">mkey</span> - Name of the interface that will send out the packet. <span class="li-normal">type: string  required: True </span> </li>
                <li><span class="li-required">mac</span> - MAC of device to wake up. <span class="li-normal">type: string  required: True </span> </li>
                <li><span class="li-required">protocol_option</span> - protocol [wol | udp]. Default is udp <span class="li-normal">type: string  required: False </span> </li>
                <li><span class="li-required">port</span> - Port used by UDP WoL packets (0, 7, or 9). Port 9 will be used by default. <span class="li-normal">type: int  required: False </span> </li>
                <li><span class="li-required">address</span> - Broadcast IP address used by UDP WoL packets. <span class="li-normal">type: string  required: False </span> </li>
                <li><span class="li-required">secureon_password</span> - Password of the destination host if SecureOn is enabled. <span class="li-normal">type: string  required: False </span> </li>
                
            </ul>
        
        </li>
        <li><span class="li-head">webhook.system.automation-stitch</span> - Triggers an incoming webhook for an automation stitch. 
        <ul class="ul-self">
                <li><span class="li-required">mkey</span> - The incoming webhook name to trigger. <span class="li-normal">type: string  required: True </span> </li>
                
            </ul>
        
        </li>
        </ul>
        </div>
        </section>
    <li><span class="li-head">params</span> - the parameter for each action, see definition in above list.<span class="li-normal">type: dict</span></li>


Notes
-----

.. note::

   - Backup API varies across versions. For FOS 7.0.1 and earlier, utilize system_config_backup in fortios_monitor_fact. For FOS 7.0.2 and later, utilize backup.system.config in fortios_monitor.

   - Different ``selector`` may have different parameters, users are expected to look them up in the dropdown list above..

   - For some selectors, no ``params`` are allowed to appear.

   - Not all parameters are required for a selector.

   - This module is exclusivly for FortiOS monitor API.

   - The result of API request is stored in ``results``.


Examples
--------

.. code-block:: yaml+jinja

 - hosts: fortigates
   connection: httpapi
   collections:
   - fortinet.fortios
   vars:
    vdom: "root"
    ansible_httpapi_use_ssl: true
    ansible_httpapi_validate_certs: false
    ansible_httpapi_port: 443
   tasks:

   - name: Activate FortiToken
     fortios_monitor:
        vdom: "root"
        access_token: "<fortios_access_token>"
        selector: 'activate.user.fortitoken'
        params:
            tokens: '<token string>'

   - name: Reboot This Device
     fortios_monitor:
        vdom: "root"
        access_token: "<fortios_access_token>"
        selector: 'reboot.system.os'
        params:
            event_log_message: 'Reboot Request From Ansible'


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