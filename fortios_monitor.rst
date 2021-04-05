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
        <li><span class="li-head">activate.user.fortitoken</span> - Activate a set of FortiTokens by serial number. 
        <ul class="ul-self">
                <li><span class="li-required">tokens</span> - List of FortiToken serial numbers to activate. If omitted, all tokens will be used. <span class="li-normal">type: array </span> </li>
                
            </ul>
        
        </li>
        <li><span class="li-head">add-license.registration.forticare</span> - Add a FortiCare license. 
        <ul class="ul-self">
                <li><span class="li-required">registration_code</span> - FortiCare contract number. <span class="li-normal">type: string </span> </li>
                
            </ul>
        
        </li>
        <li><span class="li-head">add-license.registration.vdom</span> - Add a VDOM license. 
        <ul class="ul-self">
                <li><span class="li-required">license</span> - VDOM license key. <span class="li-normal">type: string </span> </li>
                
            </ul>
        
        </li>
        <li><span class="li-head">add.firewall.clearpass-address</span> - Add ClearPass address with SPT (System Posture Token) value. 
        <ul class="ul-self">
                <li><span class="li-required">endpoint_ip</span> - Endpoint IPv4 address. <span class="li-normal">type: array </span> </li>
                <li><span class="li-required">spt</span> - SPT value [healthy|checkup|transient|quarantine|infected|unknown*]. <span class="li-normal">type: string </span> </li>
                
            </ul>
        
        </li>
        <li><span class="li-head">add.nsx.service</span> - Add NSX service to connector. 
        <ul class="ul-self">
                <li><span class="li-required">mkey</span> - NSX connector name. <span class="li-normal">type: string </span> </li>
                
            </ul>
        
        </li>
        <li><span class="li-head">add_users.user.banned</span> - Immediately add one or more users to the banned list. 
        <ul class="ul-self">
                <li><span class="li-required">ip_addresses</span> - List of IP Addresses to ban. IPv4 and IPv6 addresses are allowed. <span class="li-normal">type: array </span> </li>
                <li><span class="li-required">expiry</span> - Time until expiry in seconds. 0 for indefinite ban. <span class="li-normal">type: int </span> </li>
                
            </ul>
        
        </li>
        <li><span class="li-head">backup-action.system.fortimanager</span> - Import or update from FortiManager objects. 
        <ul class="ul-self">
                <li><span class="li-required">operation</span> - Operation to perform on the given CMDB objects [import|update]. <span class="li-normal">type: string </span> </li>
                <li><span class="li-required">objects</span> - Array of CMDB tables and mkeys. <span class="li-normal">type: array </span> </li>
                
            </ul>
        
        </li>
        <li><span class="li-head">cancel.fortiview.session</span> - Cancel a FortiView request session. 
        <ul class="ul-self">
                <li><span class="li-required">device</span> - FortiView request session's device. [disk|faz] <span class="li-normal">type: string </span> </li>
                <li><span class="li-required">sessionid</span> - Session ID to cancel. <span class="li-normal">type: int </span> </li>
                <li><span class="li-required">view_level</span> - FortiView View level. <span class="li-normal">type: string </span> </li>
                <li><span class="li-required">report_by</span> - Report by field. <span class="li-normal">type: string </span> </li>
                
            </ul>
        
        </li>
        <li><span class="li-head">change-vdom-mode.system.admin</span> - Switch between VDOM modes. 
        <ul class="ul-self">
                <li><span class="li-required">vdom-mode</span> - VDOM mode [no-vdom|split-vdom|multi-vdom] <span class="li-normal">type: string </span> </li>
                
            </ul>
        
        </li>
        <li><span class="li-head">clear-statistics.system.fortiguard</span> - Immediately clear all FortiGuard statistics. 
        
        </li>
        <li><span class="li-head">clear.system.sniffer</span> - Clear the results of a specified packet capture. 
        <ul class="ul-self">
                <li><span class="li-required">mkey</span> - ID of packet capture entry. <span class="li-normal">type: int </span> </li>
                
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
                <li><span class="li-required">policy</span> - Single policy ID to reset. <span class="li-normal">type: int </span> </li>
                
            </ul>
        
        </li>
        <li><span class="li-head">clear_counters.firewall.acl6</span> - Reset counters for one or more IPv6 ACLs by policy ID. 
        <ul class="ul-self">
                <li><span class="li-required">policy</span> - Single policy ID to reset. <span class="li-normal">type: int </span> </li>
                
            </ul>
        
        </li>
        <li><span class="li-head">clear_counters.firewall.policy</span> - Reset traffic statistics for one or more firewall policies by policy ID. 
        <ul class="ul-self">
                <li><span class="li-required">policy</span> - Single policy ID to reset. <span class="li-normal">type: int </span> </li>
                
            </ul>
        
        </li>
        <li><span class="li-head">clear_counters.firewall.proxy-policy</span> - Reset traffic statistics for one or more explicit proxy policies by policy ID. 
        <ul class="ul-self">
                <li><span class="li-required">policy</span> - Single policy ID to reset. <span class="li-normal">type: int </span> </li>
                
            </ul>
        
        </li>
        <li><span class="li-head">clear_counters.firewall.security-policy</span> - Reset traffic statistics for one or more security policies by policy ID. 
        <ul class="ul-self">
                <li><span class="li-required">policy</span> - Single policy ID to reset. <span class="li-normal">type: int </span> </li>
                
            </ul>
        
        </li>
        <li><span class="li-head">clear_tunnel.vpn.ssl</span> - Remove all active tunnel sessions in current virtual domain. 
        
        </li>
        <li><span class="li-head">clear_users.user.banned</span> - Immediately clear a list of specific banned users by IP. 
        <ul class="ul-self">
                <li><span class="li-required">ip_addresses</span> - List of banned user IPs to clear. IPv4 and IPv6 addresses are allowed. <span class="li-normal">type: array </span> </li>
                
            </ul>
        
        </li>
        <li><span class="li-head">close.firewall.session</span> - Close a specific firewall session that matches all provided criteria. 
        <ul class="ul-self">
                <li><span class="li-required">daddr</span> - Destination address. <span class="li-normal">type: string </span> </li>
                <li><span class="li-required">dport</span> - Destination port. <span class="li-normal">type: int </span> </li>
                <li><span class="li-required">pro</span> - Protocol name [tcp|udp|icmp|...]. <span class="li-normal">type: string </span> </li>
                <li><span class="li-required">sport</span> - Source port. <span class="li-normal">type: int </span> </li>
                <li><span class="li-required">saddr</span> - Source address. <span class="li-normal">type: string </span> </li>
                
            </ul>
        
        </li>
        <li><span class="li-head">config.system.fortimanager</span> - Configure FortiManager IP. Register FortiManager if 'fortimanager_ip' is provided.       Unregister FortiManager if only 'unregister' parameter is specified and set to true. 
        <ul class="ul-self">
                <li><span class="li-required">unregister</span> - Unregister the FortiManager (default=false). <span class="li-normal">type: boolean </span> </li>
                <li><span class="li-required">fortimanager_ip</span> - FortiManager IP address. <span class="li-normal">type: string </span> </li>
                
            </ul>
        
        </li>
        <li><span class="li-head">connect.system.modem</span> - Trigger a connect for the configured modem. 
        
        </li>
        <li><span class="li-head">connect.wifi.network</span> - When FortiWiFi is in client mode, connect to the specified network, if configured in the 'wifi' interface. 
        <ul class="ul-self">
                <li><span class="li-required">ssid</span> - SSID of network to connect to. <span class="li-normal">type: string </span> </li>
                
            </ul>
        
        </li>
        <li><span class="li-head">create.registration.forticare</span> - Create a new FortiCare account. 
        <ul class="ul-self">
                <li><span class="li-required">city</span> - City. <span class="li-normal">type: string </span> </li>
                <li><span class="li-required">first_name</span> - First name. <span class="li-normal">type: string </span> </li>
                <li><span class="li-required">last_name</span> - Last name. <span class="li-normal">type: string </span> </li>
                <li><span class="li-required">industry_id</span> - Industry ID. <span class="li-normal">type: int </span> </li>
                <li><span class="li-required">orgsize_id</span> - Organization size ID. <span class="li-normal">type: int </span> </li>
                <li><span class="li-required">title</span> - Title. <span class="li-normal">type: string </span> </li>
                <li><span class="li-required">industry</span> - Industry. <span class="li-normal">type: string </span> </li>
                <li><span class="li-required">company</span> - Company. <span class="li-normal">type: string </span> </li>
                <li><span class="li-required">reseller_id</span> - Reseller ID. <span class="li-normal">type: int </span> </li>
                <li><span class="li-required">state_code</span> - State/Province code. <span class="li-normal">type: string </span> </li>
                <li><span class="li-required">phone</span> - Phone number. <span class="li-normal">type: string </span> </li>
                <li><span class="li-required">state</span> - State/Province. <span class="li-normal">type: string </span> </li>
                <li><span class="li-required">postal_code</span> - Postal code. <span class="li-normal">type: string </span> </li>
                <li><span class="li-required">country_code</span> - Country code. <span class="li-normal">type: int </span> </li>
                <li><span class="li-required">address</span> - Address. <span class="li-normal">type: string </span> </li>
                <li><span class="li-required">reseller_name</span> - Reseller name. <span class="li-normal">type: string </span> </li>
                <li><span class="li-required">password</span> - Account password. <span class="li-normal">type: string </span> </li>
                <li><span class="li-required">email</span> - Account email. <span class="li-normal">type: string </span> </li>
                
            </ul>
        
        </li>
        <li><span class="li-head">create.registration.forticloud</span> - Create a FortiCloud account. 
        <ul class="ul-self">
                <li><span class="li-required">send_logs</span> - Send logs to FortiCloud. <span class="li-normal">type: boolean </span> </li>
                <li><span class="li-required">password</span> - Account password. <span class="li-normal">type: string </span> </li>
                <li><span class="li-required">email</span> - Account email. <span class="li-normal">type: string </span> </li>
                
            </ul>
        
        </li>
        <li><span class="li-head">create.web-ui.custom-language</span> - Upload custom language file to this Fortigate. 
        <ul class="ul-self">
                <li><span class="li-required">file_content</span> - Provided when uploading a file: base64 encoded file data. Must not contain whitespace or other invalid base64 characters. Must be included in HTTP body. <span class="li-normal">type: string </span> </li>
                <li><span class="li-required">lang_name</span> - Name of custom language entry. <span class="li-normal">type: string </span> </li>
                <li><span class="li-required">lang_comments</span> - Comments of custom language entry. <span class="li-normal">type: string </span> </li>
                <li><span class="li-required">filename</span> - Name of custom language file. <span class="li-normal">type: string </span> </li>
                
            </ul>
        
        </li>
        <li><span class="li-head">deauth.user.firewall</span> - Deauthenticate single, multiple, or all firewall users. 
        <ul class="ul-self">
                <li><span class="li-required">all</span> - Set to true to deauthenticate all users. Other parameters will be ignored. <span class="li-normal">type: boolean </span> </li>
                <li><span class="li-required">users</span> - Array of user objects to deauthenticate. Use this to deauthenticate multiple users at once. Each object should include the above properties. <span class="li-normal">type: array </span> </li>
                <li><span class="li-required">ip</span> - User IP address. Required for both proxy and firewall users. <span class="li-normal">type: string </span> </li>
                <li><span class="li-required">user_type</span> - User type [proxy|firewall]. Required for both proxy and firewall users. <span class="li-normal">type: string </span> </li>
                <li><span class="li-required">id</span> - User ID. Required for both proxy and firewall users. <span class="li-normal">type: int </span> </li>
                <li><span class="li-required">ip_version</span> - IP version [ip4|ip6]. Only required if user_type is firewall. <span class="li-normal">type: string </span> </li>
                <li><span class="li-required">method</span> - Authentication method [fsso|rsso|ntlm|firewall|wsso|fsso_citrix|sso_guest]. Only required if user_type is firewall. <span class="li-normal">type: string </span> </li>
                
            </ul>
        
        </li>
        <li><span class="li-head">delete.firewall.clearpass-address</span> - Delete ClearPass address with SPT (System Posture Token) value. 
        <ul class="ul-self">
                <li><span class="li-required">endpoint_ip</span> - Endpoint IPv4 address. <span class="li-normal">type: array </span> </li>
                <li><span class="li-required">spt</span> - SPT value [healthy|checkup|transient|quarantine|infected|unknown*]. <span class="li-normal">type: string </span> </li>
                
            </ul>
        
        </li>
        <li><span class="li-head">delete.log.local-report</span> - Delete a local report. 
        <ul class="ul-self">
                <li><span class="li-required">mkeys</span> - Local Report Name. <span class="li-normal">type: array </span> </li>
                
            </ul>
        
        </li>
        <li><span class="li-head">delete.system.config-revision</span> - Deletes one or more system configuration revisions. 
        <ul class="ul-self">
                <li><span class="li-required">config_ids</span> - List of configuration ids. <span class="li-normal">type: array </span> </li>
                
            </ul>
        
        </li>
        <li><span class="li-head">delete.system.config-script</span> - Delete the history of config scripts. 
        <ul class="ul-self">
                <li><span class="li-required">id_list</span> - List of config script history ids to delete. <span class="li-normal">type: array </span> </li>
                
            </ul>
        
        </li>
        <li><span class="li-head">delete.vpn.ssl</span> - Terminate the provided SSL-VPN session. 
        <ul class="ul-self">
                <li><span class="li-required">index</span> - The session index. <span class="li-normal">type: int </span> </li>
                <li><span class="li-required">type</span> - The session type [websession|subsession]. <span class="li-normal">type: string </span> </li>
                
            </ul>
        
        </li>
        <li><span class="li-head">delete.webfilter.override</span> - Delete a configured webfilter override. 
        <ul class="ul-self">
                <li><span class="li-required">mkey</span> - ID of webfilter override to delete. <span class="li-normal">type: string </span> </li>
                
            </ul>
        
        </li>
        <li><span class="li-head">dhcp-renew.system.interface</span> - Renew DHCP lease of an interface. 
        <ul class="ul-self">
                <li><span class="li-required">mkey</span> - Name of the interface. <span class="li-normal">type: string </span> </li>
                
            </ul>
        
        </li>
        <li><span class="li-head">diagnose.extender-controller.extender</span> - Execute diagnotic commands. 
        <ul class="ul-self">
                <li><span class="li-required">cmd</span> - Command to execute. <span class="li-normal">type: string </span> </li>
                <li><span class="li-required">id</span> - FortiExtender ID. <span class="li-normal">type: string </span> </li>
                
            </ul>
        
        </li>
        <li><span class="li-head">disassociate.wifi.client</span> - Disassociate a WiFi client from the FortiAP it's currently connected to. The client will need to reassociate with the same FortiAP or another to resume connectivity. 
        <ul class="ul-self">
                <li><span class="li-required">mac</span> - MAC address. <span class="li-normal">type: string </span> </li>
                
            </ul>
        
        </li>
        <li><span class="li-head">disconnect.system.ha-peer</span> - Update configuration of peer in HA cluster. 
        <ul class="ul-self">
                <li><span class="li-required">interface</span> - Name of the interface which should be assigned for management. <span class="li-normal">type: string </span> </li>
                <li><span class="li-required">ip</span> - IP to assign to the selected interface. <span class="li-normal">type: string </span> </li>
                <li><span class="li-required">serial_no</span> - Serial number of the HA member. <span class="li-normal">type: string </span> </li>
                <li><span class="li-required">mask</span> - Full network mask to assign to the selected interface. <span class="li-normal">type: string </span> </li>
                
            </ul>
        
        </li>
        <li><span class="li-head">disconnect.system.modem</span> - Trigger a disconnect for the configured modem. 
        
        </li>
        <li><span class="li-head">download.switch-controller.fsw-firmware</span> - Download FortiSwitch firmware from FortiGuard to the FortiGate according to FortiSwitch image ID. 
        <ul class="ul-self">
                <li><span class="li-required">image_id</span> - FortiSwitch image ID. <span class="li-normal">type: string </span> </li>
                
            </ul>
        
        </li>
        <li><span class="li-head">download.wifi.firmware</span> - Download FortiAP firmware from FortiGuard to the FortiGate according to FortiAP image ID. 
        <ul class="ul-self">
                <li><span class="li-required">image_id</span> - FortiAP image ID. <span class="li-normal">type: string </span> </li>
                
            </ul>
        
        </li>
        <li><span class="li-head">dump.system.com-log</span> - Dump system com-log to file. 
        
        </li>
        <li><span class="li-head">eject.system.usb-device</span> - Eject USB drives for safe removal. 
        
        </li>
        <li><span class="li-head">email.user.guest</span> - Sent guest login details via email. 
        <ul class="ul-self">
                <li><span class="li-required">group</span> - Guest group name. <span class="li-normal">type: string </span> </li>
                <li><span class="li-required">guest</span> - Guest user IDs. <span class="li-normal">type: array </span> </li>
                
            </ul>
        
        </li>
        <li><span class="li-head">factory-reset.switch-controller.managed-switch</span> - Send 'Factory Reset' command to a given FortiSwitch. 
        <ul class="ul-self">
                <li><span class="li-required">mkey</span> - Name of managed FortiSwitch. <span class="li-normal">type: string </span> </li>
                
            </ul>
        
        </li>
        <li><span class="li-head">generate-key.system.api-user</span> - Generate a new api-key for the specified api-key-auth admin. The old api-key will be replaced. The response contains the only chance to read the new api-key plaintext in the api_key field. 
        <ul class="ul-self">
                <li><span class="li-required">api-user</span> - Generate a new token for this api-user. <span class="li-normal">type: string </span> </li>
                
            </ul>
        
        </li>
        <li><span class="li-head">generate.vpn-certificate.csr</span> - Generate a certificate signing request (CSR) and a private key. The CSR can be retrieved / downloaded from CLI, GUI and REST API. 
        <ul class="ul-self">
                <li><span class="li-required">city</span> - Locality (L) of the certificate subject. <span class="li-normal">type: string </span> </li>
                <li><span class="li-required">orgunits</span> - List of organization units. Organization Units (OU) of the certificate subject. <span class="li-normal">type: array </span> </li>
                <li><span class="li-required">countrycode</span> - Country (C) of the certificate subject. <span class="li-normal">type: string </span> </li>
                <li><span class="li-required">scep_url</span> - SCEP server URL. If provided, use the url to enroll the csr through SCEP. <span class="li-normal">type: string </span> </li>
                <li><span class="li-required">curvename</span> - Elliptic curve name. [secp256r1|secp384r1|secp521r1]. Unavailable if the FortiGate is a Low Encryption Device (LENC). Required when keytype is ec. <span class="li-normal">type: string </span> </li>
                <li><span class="li-required">keytype</span> - Generate a RSA or an elliptic curve certificate request [rsa|ec]. The Elliptic Curve option is unavailable if the FortiGate is a Low Encryption Device (LENC) <span class="li-normal">type: string </span> </li>
                <li><span class="li-required">certname</span> - Certicate name. Used to retrieve / download the CSR. Not included in CSR and key content. <span class="li-normal">type: string </span> </li>
                <li><span class="li-required">scep_password</span> - SCEP challenge password. Some SCEP servers may require challege password. Provide it when SCEP server requires. <span class="li-normal">type: string </span> </li>
                <li><span class="li-required">state</span> - State (ST) of the certificate subject. <span class="li-normal">type: string </span> </li>
                <li><span class="li-required">keysize</span> - Key size.[1024|1536|2048|4096]. 512 only if the FortiGate is a Low Encryption Device (LENC). Required when keytype is RSA. <span class="li-normal">type: int </span> </li>
                <li><span class="li-required">scope</span> - Scope of CSR [vdom*|global]. Global scope is only accessible for global administrators <span class="li-normal">type: string </span> </li>
                <li><span class="li-required">sub_alt_name</span> - Subject alternative name (SAN) of the certificate. <span class="li-normal">type: string </span> </li>
                <li><span class="li-required">org</span> - Organization (O) of the certificate subject. <span class="li-normal">type: string </span> </li>
                <li><span class="li-required">password</span> - Password / pass phrase for the private key. If not provided, FortiGate generates a random one. <span class="li-normal">type: string </span> </li>
                <li><span class="li-required">email</span> - Email of the certificate subject. <span class="li-normal">type: string </span> </li>
                <li><span class="li-required">subject</span> - Subject (Host IP/Domain Name/E-Mail). Common Name (CN) of the certificate subject. <span class="li-normal">type: string </span> </li>
                
            </ul>
        
        </li>
        <li><span class="li-head">geoip.geoip-query</span> - Retrieve location details for IPs queried against FortiGuard's geoip service. 
        <ul class="ul-self">
                <li><span class="li-required">ip_addresses</span> - One or more IP address strings to query for location details. <span class="li-normal">type: array </span> </li>
                
            </ul>
        
        </li>
        <li><span class="li-head">import-mobile.user.fortitoken</span> - Import a list of tokens from FortiGuard to the FortiGate unit. 
        <ul class="ul-self">
                <li><span class="li-required">code</span> - Activation code on redemption certificate. <span class="li-normal">type: string </span> </li>
                
            </ul>
        
        </li>
        <li><span class="li-head">import-seed.user.fortitoken</span> - Import a FortiToken seed file. 
        <ul class="ul-self">
                <li><span class="li-required">file_content</span> - Provided when uploading a file: base64 encoded file data. Must not contain whitespace or other invalid base64 characters. Must be included in HTTP body. <span class="li-normal">type: string </span> </li>
                
            </ul>
        
        </li>
        <li><span class="li-head">import-trial.user.fortitoken</span> - Import trial mobile FortiTokens. 
        
        </li>
        <li><span class="li-head">import.vpn-certificate.ca</span> - Import CA certificate. 
        <ul class="ul-self">
                <li><span class="li-required">file_content</span> - Provided when uploading a file: base64 encoded file data. Must not contain whitespace or other invalid base64 characters. Must be included in HTTP body. <span class="li-normal">type: string </span> </li>
                <li><span class="li-required">scope</span> - Scope of CA certificate [vdom*|global]. Global scope is only accessible for global administrators <span class="li-normal">type: string </span> </li>
                <li><span class="li-required">import_method</span> - Method of importing CA certificate.[file|scep] <span class="li-normal">type: string </span> </li>
                <li><span class="li-required">scep_ca_id</span> - SCEP server CA identifier for import via SCEP. <span class="li-normal">type: string </span> </li>
                <li><span class="li-required">scep_url</span> - SCEP server URL. Required for import via SCEP <span class="li-normal">type: string </span> </li>
                
            </ul>
        
        </li>
        <li><span class="li-head">import.vpn-certificate.crl</span> - Import certificate revocation lists (CRL) from file content. 
        <ul class="ul-self">
                <li><span class="li-required">file_content</span> - Provided when uploading a file: base64 encoded file data. Must not contain whitespace or other invalid base64 characters. Must be included in HTTP body. <span class="li-normal">type: string </span> </li>
                <li><span class="li-required">scope</span> - Scope of CRL [vdom*|global]. Global scope is only accessible for global administrators <span class="li-normal">type: string </span> </li>
                
            </ul>
        
        </li>
        <li><span class="li-head">import.vpn-certificate.local</span> - Import local certificate. 
        <ul class="ul-self">
                <li><span class="li-required">file_content</span> - Provided when uploading a file: base64 encoded file data. Must not contain whitespace or other invalid base64 characters. Must be included in HTTP body. <span class="li-normal">type: string </span> </li>
                <li><span class="li-required">certname</span> - Certificate name for pkcs12 and regular certificate types. <span class="li-normal">type: string </span> </li>
                <li><span class="li-required">key_file_content</span> - Key content encoded in BASE64 for regular certificate type. <span class="li-normal">type: string </span> </li>
                <li><span class="li-required">scope</span> - Scope of local certificate [vdom*|global]. Global scope is only accessible for global administrators <span class="li-normal">type: string </span> </li>
                <li><span class="li-required">password</span> - Optional password for pkcs12 and regular certificate types. <span class="li-normal">type: string </span> </li>
                <li><span class="li-required">type</span> - Type of certificate.[local|pkcs12|regular] <span class="li-normal">type: string </span> </li>
                
            </ul>
        
        </li>
        <li><span class="li-head">import.vpn-certificate.remote</span> - Import remote certificate. 
        <ul class="ul-self">
                <li><span class="li-required">file_content</span> - Provided when uploading a file: base64 encoded file data. Must not contain whitespace or other invalid base64 characters. Must be included in HTTP body. <span class="li-normal">type: string </span> </li>
                <li><span class="li-required">scope</span> - Scope of CRL [vdom*|global]. Global scope is only accessible for global administrators <span class="li-normal">type: string </span> </li>
                
            </ul>
        
        </li>
        <li><span class="li-head">import.web-ui.language</span> - Import localization language file to this FortiGate. 
        <ul class="ul-self">
                <li><span class="li-required">file_content</span> - Provided when uploading a file: base64 encoded file data. Must not contain whitespace or other invalid base64 characters. Must be included in HTTP body. <span class="li-normal">type: string </span> </li>
                
            </ul>
        
        </li>
        <li><span class="li-head">keep-alive.wifi.spectrum</span> - Extend duration of an existing spectrum analysis for a specific FortiAP. 
        <ul class="ul-self">
                <li><span class="li-required">radio_id</span> - Radio ID. <span class="li-normal">type: int </span> </li>
                <li><span class="li-required">duration</span> - Duration in seconds. <span class="li-normal">type: int </span> </li>
                <li><span class="li-required">wtp_id</span> - FortiAP ID. <span class="li-normal">type: string </span> </li>
                
            </ul>
        
        </li>
        <li><span class="li-head">login.registration.forticare</span> - Login to FortiCare. 
        <ul class="ul-self">
                <li><span class="li-required">reseller_name</span> - Reseller name. <span class="li-normal">type: string </span> </li>
                <li><span class="li-required">password</span> - Account password. <span class="li-normal">type: string </span> </li>
                <li><span class="li-required">email</span> - Account email. <span class="li-normal">type: string </span> </li>
                <li><span class="li-required">reseller_id</span> - Reseller ID. <span class="li-normal">type: int </span> </li>
                
            </ul>
        
        </li>
        <li><span class="li-head">login.registration.forticloud</span> - Login to FortiCloud. 
        <ul class="ul-self">
                <li><span class="li-required">send_logs</span> - Send logs to FortiCloud. <span class="li-normal">type: boolean </span> </li>
                <li><span class="li-required">domain</span> - FortiCloud domain. <span class="li-normal">type: string </span> </li>
                <li><span class="li-required">password</span> - Account password. <span class="li-normal">type: string </span> </li>
                <li><span class="li-required">email</span> - Account email. <span class="li-normal">type: string </span> </li>
                
            </ul>
        
        </li>
        <li><span class="li-head">logout.registration.forticloud</span> - Logout from FortiCloud. 
        
        </li>
        <li><span class="li-head">migrate.registration.forticloud</span> - Migrate standalone FortiGate Cloud account to FortiCloud. 
        <ul class="ul-self">
                <li><span class="li-required">password</span> - Account password. <span class="li-normal">type: string </span> </li>
                <li><span class="li-required">email</span> - Account email. <span class="li-normal">type: string </span> </li>
                
            </ul>
        
        </li>
        <li><span class="li-head">poe-reset.switch-controller.managed-switch</span> - Reset PoE on a given FortiSwitch's port. 
        <ul class="ul-self">
                <li><span class="li-required">port</span> - Name of port to reset PoE on. <span class="li-normal">type: string </span> </li>
                <li><span class="li-required">mkey</span> - Name of managed FortiSwitch. <span class="li-normal">type: string </span> </li>
                
            </ul>
        
        </li>
        <li><span class="li-head">provision.user.fortitoken</span> - Provision a set of FortiTokens by serial number. 
        <ul class="ul-self">
                <li><span class="li-required">tokens</span> - List of FortiToken serial numbers to provision. If omitted, all tokens will be used. <span class="li-normal">type: array </span> </li>
                
            </ul>
        
        </li>
        <li><span class="li-head">push.switch-controller.fsw-firmware</span> - Push FortiSwitch firmware to the given device. 
        <ul class="ul-self">
                <li><span class="li-required">image_id</span> - FortiSwitch image ID. <span class="li-normal">type: string </span> </li>
                <li><span class="li-required">serial</span> - The target device's serial. <span class="li-normal">type: string </span> </li>
                
            </ul>
        
        </li>
        <li><span class="li-head">push.wifi.firmware</span> - Push FortiAP firmware to the given device. 
        <ul class="ul-self">
                <li><span class="li-required">image_id</span> - FortiAP image ID. <span class="li-normal">type: string </span> </li>
                <li><span class="li-required">serial</span> - The target device's serial. <span class="li-normal">type: string </span> </li>
                
            </ul>
        
        </li>
        <li><span class="li-head">reboot.system.os</span> - Immediately reboot this device. 
        <ul class="ul-self">
                <li><span class="li-required">event_log_message</span> - Message to be logged in event log. <span class="li-normal">type: string </span> </li>
                
            </ul>
        
        </li>
        <li><span class="li-head">refresh-server.user.fsso</span> - Refresh remote agent group list for all fsso agents. 
        
        </li>
        <li><span class="li-head">refresh.user.fortitoken</span> - Refresh a set of FortiTokens by serial number. 
        <ul class="ul-self">
                <li><span class="li-required">tokens</span> - List of FortiToken serial numbers to refresh. If omitted, all tokens will be used. <span class="li-normal">type: array </span> </li>
                
            </ul>
        
        </li>
        <li><span class="li-head">register-appliance.system.csf</span> - Register appliance to Security Fabric. 
        <ul class="ul-self">
                <li><span class="li-required">mgmt_ip</span> - Management IP or FQDN. <span class="li-normal">type: string </span> </li>
                <li><span class="li-required">mgmt_port</span> - Management port. <span class="li-normal">type: int </span> </li>
                <li><span class="li-required">hostname</span> - Host name. <span class="li-normal">type: string </span> </li>
                <li><span class="li-required">mgmt_url_parameters</span> - Array of URL parameters. Each item is a key/value pair. If provided, the URL parameters will be included in the management IP URL. <span class="li-normal">type: array </span> </li>
                <li><span class="li-required">serial</span> - Serial number. <span class="li-normal">type: string </span> </li>
                <li><span class="li-required">type</span> - Appliance type (Example: 'faz'). <span class="li-normal">type: string </span> </li>
                
            </ul>
        
        </li>
        <li><span class="li-head">register-device.registration.forticloud</span> - Register a device to FortiCloud through FortiGate. Currently FortiSwitch and FortiAP are supported. 
        <ul class="ul-self">
                <li><span class="li-required">country</span> - Country. <span class="li-normal">type: string </span> </li>
                <li><span class="li-required">serial</span> - Device serial number <span class="li-normal">type: string </span> </li>
                <li><span class="li-required">password</span> - Password. <span class="li-normal">type: string </span> </li>
                <li><span class="li-required">email</span> - FortiCloud email. <span class="li-normal">type: string </span> </li>
                <li><span class="li-required">reseller</span> - Reseller. <span class="li-normal">type: string </span> </li>
                
            </ul>
        
        </li>
        <li><span class="li-head">reset.extender-controller.extender</span> - Reset a specific FortiExtender unit. 
        <ul class="ul-self">
                <li><span class="li-required">id</span> - FortiExtender ID to reset. <span class="li-normal">type: string </span> </li>
                
            </ul>
        
        </li>
        <li><span class="li-head">reset.firewall.per-ip-shaper</span> - Reset statistics for all configured firewall per-IP traffic shapers. 
        
        </li>
        <li><span class="li-head">reset.firewall.policy</span> - Reset traffic statistics for all firewall policies. 
        
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
                <li><span class="li-required">profile</span> - Webfilter profile to reset. <span class="li-normal">type: string </span> </li>
                <li><span class="li-required">user</span> - User or IP to reset with. <span class="li-normal">type: string </span> </li>
                
            </ul>
        
        </li>
        <li><span class="li-head">reset.wifi.euclid</span> - Reset presence analytics statistics. 
        
        </li>
        <li><span class="li-head">restart.switch-controller.managed-switch</span> - Restart a given FortiSwitch. 
        <ul class="ul-self">
                <li><span class="li-required">mkey</span> - Name of managed FortiSwitch. <span class="li-normal">type: string </span> </li>
                
            </ul>
        
        </li>
        <li><span class="li-head">restart.system.sniffer</span> - Restart specified packet capture. 
        <ul class="ul-self">
                <li><span class="li-required">mkey</span> - ID of packet capture entry. <span class="li-normal">type: int </span> </li>
                
            </ul>
        
        </li>
        <li><span class="li-head">restart.wifi.managed_ap</span> - Restart a given FortiAP. 
        <ul class="ul-self">
                <li><span class="li-required">wtpname</span> - FortiAP name. <span class="li-normal">type: string </span> </li>
                
            </ul>
        
        </li>
        <li><span class="li-head">restore.system.config</span> - Restore system configuration from uploaded file or from USB. 
        <ul class="ul-self">
                <li><span class="li-required">config_id</span> - When using 'revision' source: valid ID of configuration stored on disk to revert to.  <span class="li-normal">type: int </span> </li>
                <li><span class="li-required">file_content</span> - Provided when uploading a file: base64 encoded file data. Must not contain whitespace or other invalid base64 characters. Must be included in HTTP body. <span class="li-normal">type: string </span> </li>
                <li><span class="li-required">usb_filename</span> - When using 'usb' source: the filename to restore from the connected USB device. <span class="li-normal">type: string </span> </li>
                <li><span class="li-required">source</span> - Configuration file data source [upload | usb | revision]. <span class="li-normal">type: string </span> </li>
                <li><span class="li-required">scope</span> - Specify global or VDOM only restore [global | vdom]. <span class="li-normal">type: string </span> </li>
                <li><span class="li-required">password</span> - Password to decrypt configuration data. <span class="li-normal">type: string </span> </li>
                <li><span class="li-required">vdom</span> - If 'vdom' scope specified, the name of the VDOM to restore configuration. <span class="li-normal">type: string </span> </li>
                
            </ul>
        
        </li>
        <li><span class="li-head">revoke.system.dhcp</span> - Revoke IPv4 DHCP leases. 
        <ul class="ul-self">
                <li><span class="li-required">ip</span> - Optional list of addresses to revoke. Defaults to all addresses if not provided. <span class="li-normal">type: array </span> </li>
                
            </ul>
        
        </li>
        <li><span class="li-head">revoke.system.dhcp6</span> - Revoke IPv6 DHCP leases. 
        <ul class="ul-self">
                <li><span class="li-required">ip</span> - Optional list of addresses to revoke. Defaults to all addresses if not provided. <span class="li-normal">type: array </span> </li>
                
            </ul>
        
        </li>
        <li><span class="li-head">run.system.config-script</span> - Run remote config scripts. 
        <ul class="ul-self">
                <li><span class="li-required">remote_script</span> - Name of remote config script to run. <span class="li-normal">type: string </span> </li>
                
            </ul>
        
        </li>
        <li><span class="li-head">save.system.config-revision</span> - Create a new config revision checkpoint. 
        <ul class="ul-self">
                <li><span class="li-required">comments</span> - Optional revision comments <span class="li-normal">type: string </span> </li>
                
            </ul>
        
        </li>
        <li><span class="li-head">scan.wifi.network</span> - When FortiWiFi is in client mode, start a scan for local WiFi networks. 
        
        </li>
        <li><span class="li-head">send-activation.user.fortitoken</span> - Send a FortiToken activation code to a user via SMS or Email. 
        <ul class="ul-self">
                <li><span class="li-required">token</span> - FortiToken serial number. The token must be assigned to a user/admin. <span class="li-normal">type: string </span> </li>
                <li><span class="li-required">sms_phone</span> - Override SMS phone number. SMS provider must be set in the assigned user/admin. <span class="li-normal">type: string </span> </li>
                <li><span class="li-required">method</span> - Method to send activation code [email|sms]. If not set, SMS will be attempted first, then email. <span class="li-normal">type: string </span> </li>
                <li><span class="li-required">email</span> - Override email address. <span class="li-normal">type: string </span> </li>
                
            </ul>
        
        </li>
        <li><span class="li-head">set.system.time</span> - Sets current system time stamp. 
        <ul class="ul-self">
                <li><span class="li-required">hour</span> - Specifies the hour (0 - 23) for setting/updating time manually. <span class="li-normal">type: int </span> </li>
                <li><span class="li-required">month</span> - Specifies the month (0 - 11) for setting/updating time manually. <span class="li-normal">type: int </span> </li>
                <li><span class="li-required">second</span> - Specifies the second (0 - 59) for setting/updating time manually. <span class="li-normal">type: int </span> </li>
                <li><span class="li-required">year</span> - Specifies the year for setting/updating time manually. <span class="li-normal">type: int </span> </li>
                <li><span class="li-required">day</span> - Specifies the day for setting/updating time manually. <span class="li-normal">type: int </span> </li>
                <li><span class="li-required">minute</span> - Specifies the minute (0 - 59) for setting/updating time manually. <span class="li-normal">type: int </span> </li>
                
            </ul>
        
        </li>
        <li><span class="li-head">set_status.wifi.managed_ap</span> - Update administrative state for a given FortiAP (enable or disable authorization). 
        <ul class="ul-self">
                <li><span class="li-required">admin</span> - New FortiAP administrative state [enable|disable|discovered]. <span class="li-normal">type: string </span> </li>
                <li><span class="li-required">wtpname</span> - FortiAP name. <span class="li-normal">type: string </span> </li>
                
            </ul>
        
        </li>
        <li><span class="li-head">set_status.wifi.rogue_ap</span> - Mark detected APs as rogue APs. 
        <ul class="ul-self">
                <li><span class="li-required">status</span> - Status to assign matching APs [unclassified|rogue|accepted|suppressed]. <span class="li-normal">type: string </span> </li>
                <li><span class="li-required">ssid</span> - Corresponding list of rogue AP SSIDs. <span class="li-normal">type: array </span> </li>
                <li><span class="li-required">bssid</span> - List of rogue AP MAC addresses. <span class="li-normal">type: array </span> </li>
                
            </ul>
        
        </li>
        <li><span class="li-head">shutdown.system.os</span> - Immediately shutdown this device. 
        <ul class="ul-self">
                <li><span class="li-required">event_log_message</span> - Message to be logged in event log. <span class="li-normal">type: string </span> </li>
                
            </ul>
        
        </li>
        <li><span class="li-head">sms.user.guest</span> - Sent guest login details via SMS. 
        <ul class="ul-self">
                <li><span class="li-required">group</span> - Guest group name. <span class="li-normal">type: string </span> </li>
                <li><span class="li-required">guest</span> - Guest user IDs. <span class="li-normal">type: array </span> </li>
                
            </ul>
        
        </li>
        <li><span class="li-head">speed-test-trigger.system.interface</span> - Run a speed-test on the given interface. 
        <ul class="ul-self">
                <li><span class="li-required">mkey</span> - Name of the interface. <span class="li-normal">type: string </span> </li>
                
            </ul>
        
        </li>
        <li><span class="li-head">start.system.fsck</span> - Set file system check flag so that it will be executed on next device reboot. 
        
        </li>
        <li><span class="li-head">start.system.sniffer</span> - Start specified packet capture. 
        <ul class="ul-self">
                <li><span class="li-required">mkey</span> - ID of packet capture entry. <span class="li-normal">type: int </span> </li>
                
            </ul>
        
        </li>
        <li><span class="li-head">start.system.usb-log</span> - Start backup of logs from current VDOM to USB drive. 
        
        </li>
        <li><span class="li-head">start.wifi.spectrum</span> - Start spectrum analysis for a specific FortiAP for a duration of time. 
        <ul class="ul-self">
                <li><span class="li-required">radio_id</span> - Radio ID. <span class="li-normal">type: int </span> </li>
                <li><span class="li-required">channels</span> - Channels. <span class="li-normal">type: array </span> </li>
                <li><span class="li-required">duration</span> - Duration in seconds. <span class="li-normal">type: int </span> </li>
                <li><span class="li-required">wtp_id</span> - FortiAP ID. <span class="li-normal">type: string </span> </li>
                
            </ul>
        
        </li>
        <li><span class="li-head">start.wifi.vlan-probe</span> - Start a VLAN probe. 
        <ul class="ul-self">
                <li><span class="li-required">wtp</span> - FortiAP ID. <span class="li-normal">type: string </span> </li>
                <li><span class="li-required">retries</span> - Number of times to retry a probe for a particular VLAN. <span class="li-normal">type: int </span> </li>
                <li><span class="li-required">start_vlan_id</span> - The starting VLAN ID for the probe. <span class="li-normal">type: int </span> </li>
                <li><span class="li-required">end_vlan_id</span> - The ending VLAN ID for the probe. <span class="li-normal">type: int </span> </li>
                <li><span class="li-required">timeout</span> - Timeout duration (in seconds) to wait for a VLAN probe response. <span class="li-normal">type: int </span> </li>
                <li><span class="li-required">ap_interface</span> - FortiAP interface to send the probe on. <span class="li-normal">type: int </span> </li>
                
            </ul>
        
        </li>
        <li><span class="li-head">stop.system.sniffer</span> - Stop specified packet capture. 
        <ul class="ul-self">
                <li><span class="li-required">mkey</span> - ID of packet capture entry. <span class="li-normal">type: int </span> </li>
                
            </ul>
        
        </li>
        <li><span class="li-head">stop.system.usb-log</span> - Stop backup of logs to USB drive. 
        
        </li>
        <li><span class="li-head">stop.wifi.spectrum</span> - Stop spectrum analysis for a specific FortiAP. 
        <ul class="ul-self">
                <li><span class="li-required">radio_id</span> - Radio ID. <span class="li-normal">type: int </span> </li>
                <li><span class="li-required">wtp_id</span> - FortiAP ID. <span class="li-normal">type: string </span> </li>
                
            </ul>
        
        </li>
        <li><span class="li-head">stop.wifi.vlan-probe</span> - Stop a VLAN probe. 
        <ul class="ul-self">
                <li><span class="li-required">wtp</span> - FortiAP ID. <span class="li-normal">type: string </span> </li>
                <li><span class="li-required">ap_interface</span> - FortiAP interface to send the probe on. <span class="li-normal">type: int </span> </li>
                
            </ul>
        
        </li>
        <li><span class="li-head">system.change-password</span> - Save admin and guest-admin passwords. 
        <ul class="ul-self">
                <li><span class="li-required">new_password</span> - New password. <span class="li-normal">type: string </span> </li>
                <li><span class="li-required">old_password</span> - Old password. <span class="li-normal">type: string </span> </li>
                <li><span class="li-required">mkey</span> - User ID for password change. <span class="li-normal">type: string </span> </li>
                
            </ul>
        
        </li>
        <li><span class="li-head">system.disconnect-admins</span> - Disconnects logged in administrators. 
        <ul class="ul-self">
                <li><span class="li-required">admins</span> - List of objects with admin id and method. <span class="li-normal">type: array </span> </li>
                <li><span class="li-required">id</span> - Admin ID <span class="li-normal">type: int </span> </li>
                <li><span class="li-required">method</span> - Login method used to connect admin to FortiGate. <span class="li-normal">type: string </span> </li>
                
            </ul>
        
        </li>
        <li><span class="li-head">system.password-policy-conform</span> - Check whether password conforms to the password policy. 
        <ul class="ul-self">
                <li><span class="li-required">apply_to</span> - Password Policy ID. <span class="li-normal">type: string </span> </li>
                <li><span class="li-required">password</span> - Password. <span class="li-normal">type: string </span> </li>
                <li><span class="li-required">old_password</span> - Old password. <span class="li-normal">type: string </span> </li>
                <li><span class="li-required">mkey</span> - User ID for password change. <span class="li-normal">type: string </span> </li>
                
            </ul>
        
        </li>
        <li><span class="li-head">test-availability.system.fortiguard</span> - Test availability of FortiGuard services. 
        <ul class="ul-self">
                <li><span class="li-required">protocol</span> - Protocol to check. [https | udp | http] <span class="li-normal">type: string </span> </li>
                <li><span class="li-required">port</span> - Port to check. <span class="li-normal">type: int </span> </li>
                <li><span class="li-required">service</span> - Service to check. [emailfilter | webfilter] <span class="li-normal">type: string </span> </li>
                
            </ul>
        
        </li>
        <li><span class="li-head">test-connect.user.radius</span> - Test the connectivity of the given RADIUS server and, optionally, the validity of a username & password. 
        <ul class="ul-self">
                <li><span class="li-required">ordinal</span> - If 'mkey' is provided, the server-secret pair to use from the object: 'primary', 'secondary' or 'tertiary'. Defaults to 'primary'. <span class="li-normal">type: string </span> </li>
                <li><span class="li-required">server</span> - Host name or IP of a RADIUS server. If 'mkey' is provided, this overrides the 'server' value in the object. <span class="li-normal">type: string </span> </li>
                <li><span class="li-required">secret</span> - Secret password for the RADIUS server. If 'mkey' is provided, this overrides the 'secret' value in the object. <span class="li-normal">type: string </span> </li>
                <li><span class="li-required">user</span> - User name whose access to check. <span class="li-normal">type: string </span> </li>
                <li><span class="li-required">password</span> - User's password. <span class="li-normal">type: string </span> </li>
                <li><span class="li-required">mkey</span> - Name of FortiGate's RADIUS object whose settings to test. <span class="li-normal">type: string </span> </li>
                
            </ul>
        
        </li>
        <li><span class="li-head">test.system.automation-stitch</span> - Triggers an automation stitch for testing purposes. 
        <ul class="ul-self">
                <li><span class="li-required">log</span> - Message to store in the log buffer when triggering an event. For example, "logid=\"32102\" eventtime=1528840790000000000 logdesc=\"Sample description\" msg=\"Sample message\"". This parameter is required for the 'event-log' event type. For the test to run, the 'logid' argument value must match the trigger-defined value. If 'logid' is not provided, the test will use the trigger-defined value. <span class="li-normal">type: string </span> </li>
                <li><span class="li-required">mkey</span> - ID of automation stitch to trigger. <span class="li-normal">type: string </span> </li>
                
            </ul>
        
        </li>
        <li><span class="li-head">test.user.tacacs-plus</span> - Test the connectivity of the given TACACS+ server. 
        <ul class="ul-self">
                <li><span class="li-required">ordinal</span> - If 'mkey' is provided, the server-key pair to use from the object: 'primary', 'secondary' or 'tertiary'. Defaults to 'primary'. <span class="li-normal">type: string </span> </li>
                <li><span class="li-required">source_ip</span> - Source IP for communications to TACACS+ server. If 'mkey' is provided, this overrides the 'source-ip' value in the object. <span class="li-normal">type: string </span> </li>
                <li><span class="li-required">server</span> - Host name of IP of a TACACS+ server. If 'mkey' is provided, this overrides the 'server' value in the object. <span class="li-normal">type: string </span> </li>
                <li><span class="li-required">secret</span> - Secret key for the TACACS+ server. If 'mkey' is provided, this overrides the 'key' value in the object. <span class="li-normal">type: string </span> </li>
                <li><span class="li-required">port</span> - Port number of the TACACS+ server. If 'mkey' is provided, this overrides the 'port' value in the object. Defaults to 49. <span class="li-normal">type: int </span> </li>
                <li><span class="li-required">mkey</span> - Name of FortiGate's TACACS+ object whose settings to test. <span class="li-normal">type: string </span> </li>
                
            </ul>
        
        </li>
        <li><span class="li-head">transfer.registration.forticare</span> - Transfer to a new FortiCare account. 
        <ul class="ul-self">
                <li><span class="li-required">password</span> - Account password. <span class="li-normal">type: string </span> </li>
                <li><span class="li-required">old_password</span> - Old account password. <span class="li-normal">type: string </span> </li>
                <li><span class="li-required">email</span> - Account email. <span class="li-normal">type: string </span> </li>
                <li><span class="li-required">old_email</span> - Old account email. <span class="li-normal">type: string </span> </li>
                
            </ul>
        
        </li>
        <li><span class="li-head">trigger.system.security-rating</span> - Run a Security Rating report. 
        <ul class="ul-self">
                <li><span class="li-required">report_types</span> - Multiple Security Rating reports to run, run all reports when unspecified. <span class="li-normal">type: array </span> </li>
                <li><span class="li-required">report_type</span> - Security Rating report to run, run all reports when unspecified. <span class="li-normal">type: string </span> </li>
                
            </ul>
        
        </li>
        <li><span class="li-head">tunnel_down.vpn.ipsec</span> - Bring down a specific IPsec VPN tunnel. 
        <ul class="ul-self">
                <li><span class="li-required">p2name</span> - IPsec phase2 name. <span class="li-normal">type: string </span> </li>
                <li><span class="li-required">p2serial</span> - IPsec phase2 serial. <span class="li-normal">type: int </span> </li>
                <li><span class="li-required">p1name</span> - IPsec phase1 name. <span class="li-normal">type: string </span> </li>
                
            </ul>
        
        </li>
        <li><span class="li-head">tunnel_reset_stats.vpn.ipsec</span> - Reset statistics for a specific IPsec VPN tunnel. 
        <ul class="ul-self">
                <li><span class="li-required">p1name</span> - IPsec phase1 name. <span class="li-normal">type: string </span> </li>
                
            </ul>
        
        </li>
        <li><span class="li-head">tunnel_up.vpn.ipsec</span> - Bring up a specific IPsec VPN tunnel. 
        <ul class="ul-self">
                <li><span class="li-required">p2name</span> - IPsec phase2 name. <span class="li-normal">type: string </span> </li>
                <li><span class="li-required">p2serial</span> - IPsec phase2 serial. <span class="li-normal">type: int </span> </li>
                <li><span class="li-required">p1name</span> - IPsec phase1 name. <span class="li-normal">type: string </span> </li>
                
            </ul>
        
        </li>
        <li><span class="li-head">update-comments.system.config-revision</span> - Updates comments for a system configuration file. 
        <ul class="ul-self">
                <li><span class="li-required">config_id</span> - Configuration id. <span class="li-normal">type: int </span> </li>
                <li><span class="li-required">comments</span> - Configuration comments. <span class="li-normal">type: string </span> </li>
                
            </ul>
        
        </li>
        <li><span class="li-head">update.switch-controller.managed-switch</span> - Update administrative state for a given FortiSwitch (enable or disable authorization). 
        <ul class="ul-self">
                <li><span class="li-required">admin</span> - New FortiSwitch administrative state [enable|disable|discovered]. <span class="li-normal">type: string </span> </li>
                <li><span class="li-required">fswname</span> - DEPRECATED since 5.6.1, will be removed in 6.4. Please use mkey instead. <span class="li-normal">type: string </span> </li>
                <li><span class="li-required">mkey</span> - FortiSwitch name. <span class="li-normal">type: string </span> </li>
                
            </ul>
        
        </li>
        <li><span class="li-head">update.system.fortiguard</span> - Immediately update status for FortiGuard services. 
        
        </li>
        <li><span class="li-head">update.system.ha-peer</span> - Update configuration of peer in HA cluster. 
        <ul class="ul-self">
                <li><span class="li-required">priority</span> - Priority to assign to HA member. <span class="li-normal">type: int </span> </li>
                <li><span class="li-required">serial_no</span> - Serial number of the HA member. <span class="li-normal">type: string </span> </li>
                <li><span class="li-required">hostname</span> - Name to assign the HA member. <span class="li-normal">type: string </span> </li>
                <li><span class="li-required">vcluster_id</span> - Virtual cluster number. <span class="li-normal">type: int </span> </li>
                
            </ul>
        
        </li>
        <li><span class="li-head">update.system.modem</span> - Update supported modem list from FortiGuard. 
        
        </li>
        <li><span class="li-head">update.system.sdn-connector</span> - Update an SDN connector's connection status. 
        <ul class="ul-self">
                <li><span class="li-required">mkey</span> - SDN connector name. <span class="li-normal">type: string </span> </li>
                
            </ul>
        
        </li>
        <li><span class="li-head">update.web-ui.custom-language</span> - Update custom language file to this Fortigate. 
        <ul class="ul-self">
                <li><span class="li-required">file_content</span> - Provided when uploading a file: base64 encoded file data. Must not contain whitespace or other invalid base64 characters. Must be included in HTTP body. <span class="li-normal">type: string </span> </li>
                <li><span class="li-required">filename</span> - Name of custom language file. <span class="li-normal">type: string </span> </li>
                <li><span class="li-required">lang_comments</span> - Comments of custom language entry. <span class="li-normal">type: string </span> </li>
                <li><span class="li-required">mkey</span> - Name of custom language entry. <span class="li-normal">type: string </span> </li>
                <li><span class="li-required">lang_name</span> - New name of custom language entry. <span class="li-normal">type: string </span> </li>
                
            </ul>
        
        </li>
        <li><span class="li-head">upgrade.extender-controller.extender</span> - Upgrade FortiExtender. 
        <ul class="ul-self">
                <li><span class="li-required">file_content</span> - Provided when uploading a file: base64 encoded file data. Must not contain whitespace or other invalid base64 characters. Must be included in HTTP body. <span class="li-normal">type: string </span> </li>
                <li><span class="li-required">id</span> - FortiExtender ID to upgrade. <span class="li-normal">type: string </span> </li>
                
            </ul>
        
        </li>
        <li><span class="li-head">upgrade.license.database</span> - Upgrade or downgrade UTM engine or signature package (IPS/AntiVirus/Application Control/Industrial database/Security Rating) using uploaded file. 
        <ul class="ul-self">
                <li><span class="li-required">file_content</span> - Provided when uploading a file: base64 encoded file data. Must not contain whitespace or other invalid base64 characters. Must be included in HTTP body. <span class="li-normal">type: string </span> </li>
                <li><span class="li-required">db_name</span> - Security service database name [ips|appctrl|industrial_db|antivirus|security_rating] <span class="li-normal">type: string </span> </li>
                
            </ul>
        
        </li>
        <li><span class="li-head">upgrade.system.firmware</span> - Upgrade firmware image on this device using uploaded file. 
        <ul class="ul-self">
                <li><span class="li-required">file_content</span> - Provided when uploading a file: base64 encoded file data. Must not contain whitespace or other invalid base64 characters. Must be included in HTTP body. <span class="li-normal">type: string </span> </li>
                <li><span class="li-required">source</span> - Firmware file data source [upload|usb|fortiguard]. <span class="li-normal">type: string </span> </li>
                <li><span class="li-required">ignore_invalid_signature</span> - Set to true to allow upgrade of firmware images with invalid signatures. <span class="li-normal">type: boolean </span> </li>
                <li><span class="li-required">format_partition</span> - Set to true to format boot partition before upgrade. <span class="li-normal">type: boolean </span> </li>
                <li><span class="li-required">filename</span> - Name of file on fortiguard or USB disk to upgrade to. <span class="li-normal">type: string </span> </li>
                
            </ul>
        
        </li>
        <li><span class="li-head">upload.switch-controller.fsw-firmware</span> - Upload FortiSwitch firmware to the management FortiGate and then push to target FortiSwitches. 
        <ul class="ul-self">
                <li><span class="li-required">serials</span> - The target device's serial. <span class="li-normal">type: string </span> </li>
                <li><span class="li-required">file_content</span> - Provided when uploading a file: base64 encoded file data. Must not contain whitespace or other invalid base64 characters. Must be included in HTTP body. <span class="li-normal">type: string </span> </li>
                
            </ul>
        
        </li>
        <li><span class="li-head">upload.system.config-script</span> - Upload and run a new configuration script file. 
        <ul class="ul-self">
                <li><span class="li-required">file_content</span> - Provided when uploading a file: base64 encoded file data. Must not contain whitespace or other invalid base64 characters. Must be included in HTTP body. <span class="li-normal">type: string </span> </li>
                <li><span class="li-required">filename</span> - Name of configuration script file. <span class="li-normal">type: string </span> </li>
                
            </ul>
        
        </li>
        <li><span class="li-head">upload.system.vmlicense</span> - Update VM license using uploaded file. Reboots immediately if successful. 
        <ul class="ul-self">
                <li><span class="li-required">file_content</span> - Provided when uploading a file: base64 encoded file data. Must not contain whitespace or other invalid base64 characters. Must be included in HTTP body. <span class="li-normal">type: string </span> </li>
                
            </ul>
        
        </li>
        <li><span class="li-head">upload.wifi.firmware</span> - Upload FortiAP firmware to the management FortiGate and then push to target FortiAPs. 
        <ul class="ul-self">
                <li><span class="li-required">serials</span> - The target device's serial. <span class="li-normal">type: string </span> </li>
                <li><span class="li-required">file_content</span> - Provided when uploading a file: base64 encoded file data. Must not contain whitespace or other invalid base64 characters. Must be included in HTTP body. <span class="li-normal">type: string </span> </li>
                
            </ul>
        
        </li>
        <li><span class="li-head">upload.wifi.region-image</span> - Saves a floorplan/region image to an existing region. 
        <ul class="ul-self">
                <li><span class="li-required">image_type</span> - MIME type of the image (png|jpeg|gif). <span class="li-normal">type: string </span> </li>
                <li><span class="li-required">file_content</span> - Provided when uploading a file: base64 encoded file data. Must not contain whitespace or other invalid base64 characters. Must be included in HTTP body. <span class="li-normal">type: string </span> </li>
                <li><span class="li-required">region_name</span> - Region name to save image to. <span class="li-normal">type: string </span> </li>
                
            </ul>
        
        </li>
        <li><span class="li-head">utm.rating-lookup</span> - Lookup FortiGuard rating for a specific URL. 
        <ul class="ul-self">
                <li><span class="li-required">url</span> - List of URLs to query. <span class="li-normal">type: array </span> </li>
                <li><span class="li-required">lang</span> - Language for the rating response. <span class="li-normal">type: string </span> </li>
                
            </ul>
        
        </li>
        <li><span class="li-head">validate-gcp-key.system.sdn-connector</span> - Validate a string representing a private key from GCP in PEM format. 
        <ul class="ul-self">
                <li><span class="li-required">private-key</span> - Private key in PEM format. <span class="li-normal">type: string </span> </li>
                
            </ul>
        
        </li>
        <li><span class="li-head">verify-cert.endpoint-control.ems</span> - Verify EMS server certificate for a specific EMS. 
        <ul class="ul-self">
                <li><span class="li-required">ems_name</span> - EMS server name (as defined in CLI table endpoint-control.fctems). <span class="li-normal">type: string </span> </li>
                <li><span class="li-required">fingerprint</span> - EMS server certificate fingerprint to check with. <span class="li-normal">type: string </span> </li>
                
            </ul>
        
        </li>
        <li><span class="li-head">webhook.system.automation-stitch</span> - Triggers an incoming webhook for an automation stitch. 
        <ul class="ul-self">
                <li><span class="li-required">mkey</span> - The incoming webhook name to trigger. <span class="li-normal">type: string </span> </li>
                
            </ul>
        
        </li>
        </ul>
        </div>
        </section>
    <li><span class="li-head">params</span> - the parameter for each action, see definition in above list.<span class="li-normal">type: dict</span></li>


Notes
-----

.. note::

   - Different ``selector`` may have different parameters, users are expected to look up them in the dropdown list above..

   - For some selectors, no ``params`` are allowed to appear.

   - Not all parameters are required for a selector.

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