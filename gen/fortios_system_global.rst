:source: fortios_system_global.py

:orphan:

.. fortios_system_global:

fortios_system_global -- Configure global attributes in Fortinet's FortiOS and FortiGate.
+++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++

.. versionadded:: 2.8

.. contents::
   :local:
   :depth: 1


Synopsis
--------
- This module is able to configure a FortiGate or FortiOS (FOS) device by allowing the user to set and modify system feature and global category. Examples include all parameters and values need to be adjusted to datasources before usage. Tested with FOS v6.0.5



Requirements
------------
The below requirements are needed on the host that executes this module.

- ansible>=2.9.0


Parameters
----------


.. raw:: html

    <ul>
    <li> <span class="li-head">host</span> - FortiOS or FortiGate IP address. <span class="li-normal">type: str</span> <span class="li-required">required: False</span></li>
    <li> <span class="li-head">username</span> - FortiOS or FortiGate username. <span class="li-normal">type: str</span> <span class="li-required">required: False</span></li>
    <li> <span class="li-head">password</span> - FortiOS or FortiGate password. <span class="li-normal">type: str</span> <span class="li-normal">default: </span></li>
    <li> <span class="li-head">vdom</span> - Virtual domain, among those defined previously. A vdom is a virtual instance of the FortiGate that can be configured and used as a different unit. <span class="li-normal">type: str</span> <span class="li-normal">default: root</span></li>
    <li> <span class="li-head">https</span> - Indicates if the requests towards FortiGate must use HTTPS protocol. <span class="li-normal">type: bool</span> <span class="li-normal">default: True</span></li>
    <li> <span class="li-head">ssl_verify</span> - Ensures FortiGate certificate must be verified by a proper CA. <span class="li-normal">type: bool</span> <span class="li-normal">default: True</span></li>
    <li> <span class="li-head">system_global</span> - Configure global attributes. <span class="li-normal">type: dict</span></li>
        <ul class="ul-self">
        <li> <span class="li-head">admin_concurrent</span> - Enable/disable concurrent administrator logins. (Use policy-auth-concurrent for firewall authenticated users.) <span class="li-normal">type: str</span> <span class="li-normal">choices: enable, disable</span></li>
        <li> <span class="li-head">admin_console_timeout</span> - Console login timeout that overrides the admintimeout value. (15 - 300 seconds) (15 seconds to 5 minutes). 0 the default, disables this timeout. <span class="li-normal">type: int</span></li>
        <li> <span class="li-head">admin_hsts_max_age</span> - HTTPS Strict-Transport-Security header max-age in seconds. A value of 0 will reset any HSTS records in the browser.When admin-https-redirect is disabled the header max-age will be 0. <span class="li-normal">type: int</span></li>
        <li> <span class="li-head">admin_https_pki_required</span> - Enable/disable admin login method. Enable to force administrators to provide a valid certificate to log in if PKI is enabled. Disable to allow administrators to log in with a certificate or password. <span class="li-normal">type: str</span> <span class="li-normal">choices: enable, disable</span></li>
        <li> <span class="li-head">admin_https_redirect</span> - Enable/disable redirection of HTTP administration access to HTTPS. <span class="li-normal">type: str</span> <span class="li-normal">choices: enable, disable</span></li>
        <li> <span class="li-head">admin_https_ssl_versions</span> - Allowed TLS versions for web administration. <span class="li-normal">type: list</span> <span class="li-normal">choices: tlsv1-0, tlsv1-1, tlsv1-2</span></li>
        <li> <span class="li-head">admin_lockout_duration</span> - Amount of time in seconds that an administrator account is locked out after reaching the admin-lockout-threshold for repeated failed login attempts. <span class="li-normal">type: int</span></li>
        <li> <span class="li-head">admin_lockout_threshold</span> - Number of failed login attempts before an administrator account is locked out for the admin-lockout-duration. <span class="li-normal">type: int</span></li>
        <li> <span class="li-head">admin_login_max</span> - Maximum number of administrators who can be logged in at the same time (1 - 100) <span class="li-normal">type: int</span></li>
        <li> <span class="li-head">admin_maintainer</span> - Enable/disable maintainer administrator login. When enabled, the maintainer account can be used to log in from the console after a hard reboot. The password is "bcpb" followed by the FortiGate unit serial number. You have limited time to complete this login. <span class="li-normal">type: str</span> <span class="li-normal">choices: enable, disable</span></li>
        <li> <span class="li-head">admin_port</span> - Administrative access port for HTTP. (1 - 65535). <span class="li-normal">type: int</span></li>
        <li> <span class="li-head">admin_restrict_local</span> - Enable/disable local admin authentication restriction when remote authenticator is up and running. <span class="li-normal">type: str</span> <span class="li-normal">choices: enable, disable</span></li>
        <li> <span class="li-head">admin_scp</span> - Enable/disable using SCP to download the system configuration. You can use SCP as an alternative method for backing up the configuration. <span class="li-normal">type: str</span> <span class="li-normal">choices: enable, disable</span></li>
        <li> <span class="li-head">admin_server_cert</span> - Server certificate that the FortiGate uses for HTTPS administrative connections. Source certificate.local.name. <span class="li-normal">type: str</span></li>
        <li> <span class="li-head">admin_sport</span> - Administrative access port for HTTPS. (1 - 65535). <span class="li-normal">type: int</span></li>
        <li> <span class="li-head">admin_ssh_grace_time</span> - Maximum time in seconds permitted between making an SSH connection to the FortiGate unit and authenticating (10 - 3600 sec (1 hour)). <span class="li-normal">type: int</span></li>
        <li> <span class="li-head">admin_ssh_password</span> - Enable/disable password authentication for SSH admin access. <span class="li-normal">type: str</span> <span class="li-normal">choices: enable, disable</span></li>
        <li> <span class="li-head">admin_ssh_port</span> - Administrative access port for SSH. (1 - 65535). <span class="li-normal">type: int</span></li>
        <li> <span class="li-head">admin_ssh_v1</span> - Enable/disable SSH v1 compatibility. <span class="li-normal">type: str</span> <span class="li-normal">choices: enable, disable</span></li>
        <li> <span class="li-head">admin_telnet_port</span> - Administrative access port for TELNET. (1 - 65535). <span class="li-normal">type: int</span></li>
        <li> <span class="li-head">admintimeout</span> - Number of minutes before an idle administrator session times out (5 - 480 minutes (8 hours)). A shorter idle timeout is more secure. <span class="li-normal">type: int</span></li>
        <li> <span class="li-head">alias</span> - Alias for your FortiGate unit. <span class="li-normal">type: str</span></li>
        <li> <span class="li-head">allow_traffic_redirect</span> - Disable to allow traffic to be routed back on a different interface. <span class="li-normal">type: str</span> <span class="li-normal">choices: enable, disable</span></li>
        <li> <span class="li-head">anti_replay</span> - Level of checking for packet replay and TCP sequence checking. <span class="li-normal">type: str</span> <span class="li-normal">choices: disable, loose, strict</span></li>
        <li> <span class="li-head">arp_max_entry</span> - Maximum number of dynamically learned MAC addresses that can be added to the ARP table (131072 - 2147483647). <span class="li-normal">type: int</span></li>
        <li> <span class="li-head">asymroute</span> - Enable/disable asymmetric route. <span class="li-normal">type: str</span> <span class="li-normal">choices: enable, disable</span></li>
        <li> <span class="li-head">auth_cert</span> - Server certificate that the FortiGate uses for HTTPS firewall authentication connections. Source certificate.local.name. <span class="li-normal">type: str</span></li>
        <li> <span class="li-head">auth_http_port</span> - User authentication HTTP port. (1 - 65535). <span class="li-normal">type: int</span></li>
        <li> <span class="li-head">auth_https_port</span> - User authentication HTTPS port. (1 - 65535). <span class="li-normal">type: int</span></li>
        <li> <span class="li-head">auth_keepalive</span> - Enable to prevent user authentication sessions from timing out when idle. <span class="li-normal">type: str</span> <span class="li-normal">choices: enable, disable</span></li>
        <li> <span class="li-head">auth_session_limit</span> - Action to take when the number of allowed user authenticated sessions is reached. <span class="li-normal">type: str</span> <span class="li-normal">choices: block-new, logout-inactive</span></li>
        <li> <span class="li-head">auto_auth_extension_device</span> - Enable/disable automatic authorization of dedicated Fortinet extension devices. <span class="li-normal">type: str</span> <span class="li-normal">choices: enable, disable</span></li>
        <li> <span class="li-head">av_affinity</span> - Affinity setting for AV scanning (hexadecimal value up to 256 bits in the format of xxxxxxxxxxxxxxxx). <span class="li-normal">type: str</span></li>
        <li> <span class="li-head">av_failopen</span> - Set the action to take if the FortiGate is running low on memory or the proxy connection limit has been reached. <span class="li-normal">type: str</span> <span class="li-normal">choices: pass, False, one-shot</span></li>
        <li> <span class="li-head">av_failopen_session</span> - When enabled and a proxy for a protocol runs out of room in its session table, that protocol goes into failopen mode and enacts the action specified by av-failopen. <span class="li-normal">type: str</span> <span class="li-normal">choices: enable, disable</span></li>
        <li> <span class="li-head">batch_cmdb</span> - Enable/disable batch mode, allowing you to enter a series of CLI commands that will execute as a group once they are loaded. <span class="li-normal">type: str</span> <span class="li-normal">choices: enable, disable</span></li>
        <li> <span class="li-head">block_session_timer</span> - Duration in seconds for blocked sessions (1 - 300 sec  (5 minutes)). <span class="li-normal">type: int</span></li>
        <li> <span class="li-head">br_fdb_max_entry</span> - Maximum number of bridge forwarding database (FDB) entries. <span class="li-normal">type: int</span></li>
        <li> <span class="li-head">cert_chain_max</span> - Maximum number of certificates that can be traversed in a certificate chain. <span class="li-normal">type: int</span></li>
        <li> <span class="li-head">cfg_revert_timeout</span> - Time-out for reverting to the last saved configuration. <span class="li-normal">type: int</span></li>
        <li> <span class="li-head">cfg_save</span> - Configuration file save mode for CLI changes. <span class="li-normal">type: str</span> <span class="li-normal">choices: automatic, manual, revert</span></li>
        <li> <span class="li-head">check_protocol_header</span> - Level of checking performed on protocol headers. Strict checking is more thorough but may affect performance. Loose checking is ok in most cases. <span class="li-normal">type: str</span> <span class="li-normal">choices: loose, strict</span></li>
        <li> <span class="li-head">check_reset_range</span> - Configure ICMP error message verification. You can either apply strict RST range checking or disable it. <span class="li-normal">type: str</span> <span class="li-normal">choices: strict, disable</span></li>
        <li> <span class="li-head">cli_audit_log</span> - Enable/disable CLI audit log. <span class="li-normal">type: str</span> <span class="li-normal">choices: enable, disable</span></li>
        <li> <span class="li-head">clt_cert_req</span> - Enable/disable requiring administrators to have a client certificate to log into the GUI using HTTPS. <span class="li-normal">type: str</span> <span class="li-normal">choices: enable, disable</span></li>
        <li> <span class="li-head">compliance_check</span> - Enable/disable global PCI DSS compliance check. <span class="li-normal">type: str</span> <span class="li-normal">choices: enable, disable</span></li>
        <li> <span class="li-head">compliance_check_time</span> - Time of day to run scheduled PCI DSS compliance checks. <span class="li-normal">type: str</span></li>
        <li> <span class="li-head">cpu_use_threshold</span> - Threshold at which CPU usage is reported. (% of total CPU). <span class="li-normal">type: int</span></li>
        <li> <span class="li-head">csr_ca_attribute</span> - Enable/disable the CA attribute in certificates. Some CA servers reject CSRs that have the CA attribute. <span class="li-normal">type: str</span> <span class="li-normal">choices: enable, disable</span></li>
        <li> <span class="li-head">daily_restart</span> - Enable/disable daily restart of FortiGate unit. Use the restart-time option to set the time of day for the restart. <span class="li-normal">type: str</span> <span class="li-normal">choices: enable, disable</span></li>
        <li> <span class="li-head">device_identification_active_scan_delay</span> - Number of seconds to passively scan a device before performing an active scan. (20 - 3600 sec, (20 sec to 1 hour)). <span class="li-normal">type: int</span></li>
        <li> <span class="li-head">device_idle_timeout</span> - Time in seconds that a device must be idle to automatically log the device user out. (30 - 31536000 sec (30 sec to 1 year)). <span class="li-normal">type: int</span></li>
        <li> <span class="li-head">dh_params</span> - Number of bits to use in the Diffie-Hellman exchange for HTTPS/SSH protocols. <span class="li-normal">type: str</span> <span class="li-normal">choices: 1024, 1536, 2048, 3072, 4096, 6144, 8192</span></li>
        <li> <span class="li-head">dnsproxy_worker_count</span> - DNS proxy worker count. <span class="li-normal">type: int</span></li>
        <li> <span class="li-head">dst</span> - Enable/disable daylight saving time. <span class="li-normal">type: str</span> <span class="li-normal">choices: enable, disable</span></li>
        <li> <span class="li-head">endpoint_control_fds_access</span> - Enable/disable access to the FortiGuard network for non-compliant endpoints. <span class="li-normal">type: str</span> <span class="li-normal">choices: enable, disable</span></li>
        <li> <span class="li-head">endpoint_control_portal_port</span> - Endpoint control portal port (1 - 65535). <span class="li-normal">type: int</span></li>
        <li> <span class="li-head">failtime</span> - Fail-time for server lost. <span class="li-normal">type: int</span></li>
        <li> <span class="li-head">fds_statistics</span> - Enable/disable sending IPS, Application Control, and AntiVirus data to FortiGuard. This data is used to improve FortiGuard services and is not shared with external parties and is protected by Fortinet"s privacy policy. <span class="li-normal">type: str</span> <span class="li-normal">choices: enable, disable</span></li>
        <li> <span class="li-head">fds_statistics_period</span> - FortiGuard statistics collection period in minutes. (1 - 1440 min (1 min to 24 hours)). <span class="li-normal">type: int</span></li>
        <li> <span class="li-head">fgd_alert_subscription</span> - Type of alert to retrieve from FortiGuard. <span class="li-normal">type: list</span> <span class="li-normal">choices: advisory, latest-threat, latest-virus, latest-attack, new-antivirus-db, new-attack-db</span></li>
        <li> <span class="li-head">fortiextender</span> - Enable/disable FortiExtender. <span class="li-normal">type: str</span> <span class="li-normal">choices: enable, disable</span></li>
        <li> <span class="li-head">fortiextender_data_port</span> - FortiExtender data port (1024 - 49150). <span class="li-normal">type: int</span></li>
        <li> <span class="li-head">fortiextender_vlan_mode</span> - Enable/disable FortiExtender VLAN mode. <span class="li-normal">type: str</span> <span class="li-normal">choices: enable, disable</span></li>
        <li> <span class="li-head">fortiservice_port</span> - FortiService port (1 - 65535). Used by FortiClient endpoint compliance. Older versions of FortiClient used a different port. <span class="li-normal">type: int</span></li>
        <li> <span class="li-head">gui_certificates</span> - Enable/disable the System > Certificate GUI page, allowing you to add and configure certificates from the GUI. <span class="li-normal">type: str</span> <span class="li-normal">choices: enable, disable</span></li>
        <li> <span class="li-head">gui_custom_language</span> - Enable/disable custom languages in GUI. <span class="li-normal">type: str</span> <span class="li-normal">choices: enable, disable</span></li>
        <li> <span class="li-head">gui_date_format</span> - Default date format used throughout GUI. <span class="li-normal">type: str</span> <span class="li-normal">choices: yyyy/MM/dd, dd/MM/yyyy, MM/dd/yyyy, yyyy-MM-dd, dd-MM-yyyy, MM-dd-yyyy</span></li>
        <li> <span class="li-head">gui_device_latitude</span> - Add the latitude of the location of this FortiGate to position it on the Threat Map. <span class="li-normal">type: str</span></li>
        <li> <span class="li-head">gui_device_longitude</span> - Add the longitude of the location of this FortiGate to position it on the Threat Map. <span class="li-normal">type: str</span></li>
        <li> <span class="li-head">gui_display_hostname</span> - Enable/disable displaying the FortiGate"s hostname on the GUI login page. <span class="li-normal">type: str</span> <span class="li-normal">choices: enable, disable</span></li>
        <li> <span class="li-head">gui_ipv6</span> - Enable/disable IPv6 settings on the GUI. <span class="li-normal">type: str</span> <span class="li-normal">choices: enable, disable</span></li>
        <li> <span class="li-head">gui_lines_per_page</span> - Number of lines to display per page for web administration. <span class="li-normal">type: int</span></li>
        <li> <span class="li-head">gui_theme</span> - Color scheme for the administration GUI. <span class="li-normal">type: str</span> <span class="li-normal">choices: green, red, blue, melongene, mariner</span></li>
        <li> <span class="li-head">gui_wireless_opensecurity</span> - Enable/disable wireless open security option on the GUI. <span class="li-normal">type: str</span> <span class="li-normal">choices: enable, disable</span></li>
        <li> <span class="li-head">honor_df</span> - Enable/disable honoring of Don"t-Fragment (DF) flag. <span class="li-normal">type: str</span> <span class="li-normal">choices: enable, disable</span></li>
        <li> <span class="li-head">hostname</span> - FortiGate unit"s hostname. Most models will truncate names longer than 24 characters. Some models support hostnames up to 35 characters. <span class="li-normal">type: str</span></li>
        <li> <span class="li-head">igmp_state_limit</span> - Maximum number of IGMP memberships (96 - 64000). <span class="li-normal">type: int</span></li>
        <li> <span class="li-head">interval</span> - Dead gateway detection interval. <span class="li-normal">type: int</span></li>
        <li> <span class="li-head">ip_src_port_range</span> - IP source port range used for traffic originating from the FortiGate unit. <span class="li-normal">type: str</span></li>
        <li> <span class="li-head">ips_affinity</span> - Affinity setting for IPS (hexadecimal value up to 256 bits in the format of xxxxxxxxxxxxxxxx; allowed CPUs must be less than total number of IPS engine daemons). <span class="li-normal">type: str</span></li>
        <li> <span class="li-head">ipsec_asic_offload</span> - Enable/disable ASIC offloading (hardware acceleration) for IPsec VPN traffic. Hardware acceleration can offload IPsec VPN sessions and accelerate encryption and decryption. <span class="li-normal">type: str</span> <span class="li-normal">choices: enable, disable</span></li>
        <li> <span class="li-head">ipsec_hmac_offload</span> - Enable/disable offloading (hardware acceleration) of HMAC processing for IPsec VPN. <span class="li-normal">type: str</span> <span class="li-normal">choices: enable, disable</span></li>
        <li> <span class="li-head">ipsec_soft_dec_async</span> - Enable/disable software decryption asynchronization (using multiple CPUs to do decryption) for IPsec VPN traffic. <span class="li-normal">type: str</span> <span class="li-normal">choices: enable, disable</span></li>
        <li> <span class="li-head">ipv6_accept_dad</span> - Enable/disable acceptance of IPv6 Duplicate Address Detection (DAD). <span class="li-normal">type: int</span></li>
        <li> <span class="li-head">ipv6_allow_anycast_probe</span> - Enable/disable IPv6 address probe through Anycast. <span class="li-normal">type: str</span> <span class="li-normal">choices: enable, disable</span></li>
        <li> <span class="li-head">language</span> - GUI display language. <span class="li-normal">type: str</span> <span class="li-normal">choices: english, french, spanish, portuguese, japanese, trach, simch, korean</span></li>
        <li> <span class="li-head">ldapconntimeout</span> - Global timeout for connections with remote LDAP servers in milliseconds (1 - 300000). <span class="li-normal">type: int</span></li>
        <li> <span class="li-head">lldp_transmission</span> - Enable/disable Link Layer Discovery Protocol (LLDP) transmission. <span class="li-normal">type: str</span> <span class="li-normal">choices: enable, disable</span></li>
        <li> <span class="li-head">log_ssl_connection</span> - Enable/disable logging of SSL connection events. <span class="li-normal">type: str</span> <span class="li-normal">choices: enable, disable</span></li>
        <li> <span class="li-head">log_uuid</span> - Whether UUIDs are added to traffic logs. You can disable UUIDs, add firewall policy UUIDs to traffic logs, or add all UUIDs to traffic logs. <span class="li-normal">type: str</span> <span class="li-normal">choices: disable, policy-only, extended</span></li>
        <li> <span class="li-head">login_timestamp</span> - Enable/disable login time recording. <span class="li-normal">type: str</span> <span class="li-normal">choices: enable, disable</span></li>
        <li> <span class="li-head">long_vdom_name</span> - Enable/disable long VDOM name support. <span class="li-normal">type: str</span> <span class="li-normal">choices: enable, disable</span></li>
        <li> <span class="li-head">management_vdom</span> - Management virtual domain name. Source system.vdom.name. <span class="li-normal">type: str</span></li>
        <li> <span class="li-head">max_dlpstat_memory</span> - Maximum DLP stat memory (0 - 4294967295). <span class="li-normal">type: int</span></li>
        <li> <span class="li-head">max_route_cache_size</span> - Maximum number of IP route cache entries (0 - 2147483647). <span class="li-normal">type: int</span></li>
        <li> <span class="li-head">mc_ttl_notchange</span> - Enable/disable no modification of multicast TTL. <span class="li-normal">type: str</span> <span class="li-normal">choices: enable, disable</span></li>
        <li> <span class="li-head">memory_use_threshold_extreme</span> - Threshold at which memory usage is considered extreme (new sessions are dropped) (% of total RAM). <span class="li-normal">type: int</span></li>
        <li> <span class="li-head">memory_use_threshold_green</span> - Threshold at which memory usage forces the FortiGate to exit conserve mode (% of total RAM). <span class="li-normal">type: int</span></li>
        <li> <span class="li-head">memory_use_threshold_red</span> - Threshold at which memory usage forces the FortiGate to enter conserve mode (% of total RAM). <span class="li-normal">type: int</span></li>
        <li> <span class="li-head">miglog_affinity</span> - Affinity setting for logging (64-bit hexadecimal value in the format of xxxxxxxxxxxxxxxx). <span class="li-normal">type: str</span></li>
        <li> <span class="li-head">miglogd_children</span> - Number of logging (miglogd) processes to be allowed to run. Higher number can reduce performance; lower number can slow log processing time. No logs will be dropped or lost if the number is changed. <span class="li-normal">type: int</span></li>
        <li> <span class="li-head">multi_factor_authentication</span> - Enforce all login methods to require an additional authentication factor . <span class="li-normal">type: str</span> <span class="li-normal">choices: optional, mandatory</span></li>
        <li> <span class="li-head">multicast_forward</span> - Enable/disable multicast forwarding. <span class="li-normal">type: str</span> <span class="li-normal">choices: enable, disable</span></li>
        <li> <span class="li-head">ndp_max_entry</span> - Maximum number of NDP table entries (set to 65,536 or higher; if set to 0, kernel holds 65,536 entries). <span class="li-normal">type: int</span></li>
        <li> <span class="li-head">per_user_bwl</span> - Enable/disable per-user black/white list filter. <span class="li-normal">type: str</span> <span class="li-normal">choices: enable, disable</span></li>
        <li> <span class="li-head">policy_auth_concurrent</span> - Number of concurrent firewall use logins from the same user (1 - 100). <span class="li-normal">type: int</span></li>
        <li> <span class="li-head">post_login_banner</span> - Enable/disable displaying the administrator access disclaimer message after an administrator successfully logs in. <span class="li-normal">type: str</span> <span class="li-normal">choices: disable, enable</span></li>
        <li> <span class="li-head">pre_login_banner</span> - Enable/disable displaying the administrator access disclaimer message on the login page before an administrator logs in. <span class="li-normal">type: str</span> <span class="li-normal">choices: enable, disable</span></li>
        <li> <span class="li-head">private_data_encryption</span> - Enable/disable private data encryption using an AES 128-bit key. <span class="li-normal">type: str</span> <span class="li-normal">choices: disable, enable</span></li>
        <li> <span class="li-head">proxy_auth_lifetime</span> - Enable/disable authenticated users lifetime control.  This is a cap on the total time a proxy user can be authenticated for after which re-authentication will take place. <span class="li-normal">type: str</span> <span class="li-normal">choices: enable, disable</span></li>
        <li> <span class="li-head">proxy_auth_lifetime_timeout</span> - Lifetime timeout in minutes for authenticated users (5  - 65535 min). <span class="li-normal">type: int</span></li>
        <li> <span class="li-head">proxy_auth_timeout</span> - Authentication timeout in minutes for authenticated users (1 - 300 min). <span class="li-normal">type: int</span></li>
        <li> <span class="li-head">proxy_cipher_hardware_acceleration</span> - Enable/disable using content processor (CP8 or CP9) hardware acceleration to encrypt and decrypt IPsec and SSL traffic. <span class="li-normal">type: str</span> <span class="li-normal">choices: disable, enable</span></li>
        <li> <span class="li-head">proxy_kxp_hardware_acceleration</span> - Enable/disable using the content processor to accelerate KXP traffic. <span class="li-normal">type: str</span> <span class="li-normal">choices: disable, enable</span></li>
        <li> <span class="li-head">proxy_re_authentication_mode</span> - Control if users must re-authenticate after a session is closed, traffic has been idle, or from the point at which the user was first created. <span class="li-normal">type: str</span> <span class="li-normal">choices: session, traffic, absolute</span></li>
        <li> <span class="li-head">proxy_worker_count</span> - Proxy worker count. <span class="li-normal">type: int</span></li>
        <li> <span class="li-head">radius_port</span> - RADIUS service port number. <span class="li-normal">type: int</span></li>
        <li> <span class="li-head">reboot_upon_config_restore</span> - Enable/disable reboot of system upon restoring configuration. <span class="li-normal">type: str</span> <span class="li-normal">choices: enable, disable</span></li>
        <li> <span class="li-head">refresh</span> - Statistics refresh interval in GUI. <span class="li-normal">type: int</span></li>
        <li> <span class="li-head">remoteauthtimeout</span> - Number of seconds that the FortiGate waits for responses from remote RADIUS, LDAP, or TACACS+ authentication servers. (0-300 sec). <span class="li-normal">type: int</span></li>
        <li> <span class="li-head">reset_sessionless_tcp</span> - Action to perform if the FortiGate receives a TCP packet but cannot find a corresponding session in its session table. NAT/Route mode only. <span class="li-normal">type: str</span> <span class="li-normal">choices: enable, disable</span></li>
        <li> <span class="li-head">restart_time</span> - Daily restart time (hh:mm). <span class="li-normal">type: str</span></li>
        <li> <span class="li-head">revision_backup_on_logout</span> - Enable/disable back-up of the latest configuration revision when an administrator logs out of the CLI or GUI. <span class="li-normal">type: str</span> <span class="li-normal">choices: enable, disable</span></li>
        <li> <span class="li-head">revision_image_auto_backup</span> - Enable/disable back-up of the latest configuration revision after the firmware is upgraded. <span class="li-normal">type: str</span> <span class="li-normal">choices: enable, disable</span></li>
        <li> <span class="li-head">scanunit_count</span> - Number of scanunits. The range and the default depend on the number of CPUs. Only available on FortiGate units with multiple CPUs. <span class="li-normal">type: int</span></li>
        <li> <span class="li-head">security_rating_result_submission</span> - Enable/disable the submission of Security Rating results to FortiGuard. <span class="li-normal">type: str</span> <span class="li-normal">choices: enable, disable</span></li>
        <li> <span class="li-head">security_rating_run_on_schedule</span> - Enable/disable scheduled runs of Security Rating. <span class="li-normal">type: str</span> <span class="li-normal">choices: enable, disable</span></li>
        <li> <span class="li-head">send_pmtu_icmp</span> - Enable/disable sending of path maximum transmission unit (PMTU) - ICMP destination unreachable packet and to support PMTUD protocol on your network to reduce fragmentation of packets. <span class="li-normal">type: str</span> <span class="li-normal">choices: enable, disable</span></li>
        <li> <span class="li-head">snat_route_change</span> - Enable/disable the ability to change the static NAT route. <span class="li-normal">type: str</span> <span class="li-normal">choices: enable, disable</span></li>
        <li> <span class="li-head">special_file_23_support</span> - Enable/disable IPS detection of HIBUN format files when using Data Leak Protection. <span class="li-normal">type: str</span> <span class="li-normal">choices: disable, enable</span></li>
        <li> <span class="li-head">ssd_trim_date</span> - Date within a month to run ssd trim. <span class="li-normal">type: int</span></li>
        <li> <span class="li-head">ssd_trim_freq</span> - How often to run SSD Trim . SSD Trim prevents SSD drive data loss by finding and isolating errors. <span class="li-normal">type: str</span> <span class="li-normal">choices: never, hourly, daily, weekly, monthly</span></li>
        <li> <span class="li-head">ssd_trim_hour</span> - Hour of the day on which to run SSD Trim (0 - 23). <span class="li-normal">type: int</span></li>
        <li> <span class="li-head">ssd_trim_min</span> - Minute of the hour on which to run SSD Trim (0 - 59, 60 for random). <span class="li-normal">type: int</span></li>
        <li> <span class="li-head">ssd_trim_weekday</span> - Day of week to run SSD Trim. <span class="li-normal">type: str</span> <span class="li-normal">choices: sunday, monday, tuesday, wednesday, thursday, friday, saturday</span></li>
        <li> <span class="li-head">ssh_cbc_cipher</span> - Enable/disable CBC cipher for SSH access. <span class="li-normal">type: str</span> <span class="li-normal">choices: enable, disable</span></li>
        <li> <span class="li-head">ssh_hmac_md5</span> - Enable/disable HMAC-MD5 for SSH access. <span class="li-normal">type: str</span> <span class="li-normal">choices: enable, disable</span></li>
        <li> <span class="li-head">ssh_kex_sha1</span> - Enable/disable SHA1 key exchange for SSH access. <span class="li-normal">type: str</span> <span class="li-normal">choices: enable, disable</span></li>
        <li> <span class="li-head">ssl_min_proto_version</span> - Minimum supported protocol version for SSL/TLS connections . <span class="li-normal">type: str</span> <span class="li-normal">choices: SSLv3, TLSv1, TLSv1-1, TLSv1-2</span></li>
        <li> <span class="li-head">ssl_static_key_ciphers</span> - Enable/disable static key ciphers in SSL/TLS connections (e.g. AES128-SHA, AES256-SHA, AES128-SHA256, AES256-SHA256). <span class="li-normal">type: str</span> <span class="li-normal">choices: enable, disable</span></li>
        <li> <span class="li-head">sslvpn_cipher_hardware_acceleration</span> - Enable/disable SSL VPN hardware acceleration. <span class="li-normal">type: str</span> <span class="li-normal">choices: enable, disable</span></li>
        <li> <span class="li-head">sslvpn_kxp_hardware_acceleration</span> - Enable/disable SSL VPN KXP hardware acceleration. <span class="li-normal">type: str</span> <span class="li-normal">choices: enable, disable</span></li>
        <li> <span class="li-head">sslvpn_max_worker_count</span> - Maximum number of SSL VPN processes. Upper limit for this value is the number of CPUs and depends on the model. <span class="li-normal">type: int</span></li>
        <li> <span class="li-head">sslvpn_plugin_version_check</span> - Enable/disable checking browser"s plugin version by SSL VPN. <span class="li-normal">type: str</span> <span class="li-normal">choices: enable, disable</span></li>
        <li> <span class="li-head">strict_dirty_session_check</span> - Enable to check the session against the original policy when revalidating. This can prevent dropping of redirected sessions when web-filtering and authentication are enabled together. If this option is enabled, the FortiGate unit deletes a session if a routing or policy change causes the session to no longer match the policy that originally allowed the session. <span class="li-normal">type: str</span> <span class="li-normal">choices: enable, disable</span></li>
        <li> <span class="li-head">strong_crypto</span> - Enable to use strong encryption and only allow strong ciphers (AES, 3DES) and digest (SHA1) for HTTPS/SSH/TLS/SSL functions. <span class="li-normal">type: str</span> <span class="li-normal">choices: enable, disable</span></li>
        <li> <span class="li-head">switch_controller</span> - Enable/disable switch controller feature. Switch controller allows you to manage FortiSwitch from the FortiGate itself. <span class="li-normal">type: str</span> <span class="li-normal">choices: disable, enable</span></li>
        <li> <span class="li-head">switch_controller_reserved_network</span> - Enable reserved network subnet for controlled switches. This is available when the switch controller is enabled. <span class="li-normal">type: str</span></li>
        <li> <span class="li-head">sys_perf_log_interval</span> - Time in minutes between updates of performance statistics logging. (1 - 15 min). <span class="li-normal">type: int</span></li>
        <li> <span class="li-head">tcp_halfclose_timer</span> - Number of seconds the FortiGate unit should wait to close a session after one peer has sent a FIN packet but the other has not responded (1 - 86400 sec (1 day)). <span class="li-normal">type: int</span></li>
        <li> <span class="li-head">tcp_halfopen_timer</span> - Number of seconds the FortiGate unit should wait to close a session after one peer has sent an open session packet but the other has not responded (1 - 86400 sec (1 day)). <span class="li-normal">type: int</span></li>
        <li> <span class="li-head">tcp_option</span> - Enable SACK, timestamp and MSS TCP options. <span class="li-normal">type: str</span> <span class="li-normal">choices: enable, disable</span></li>
        <li> <span class="li-head">tcp_timewait_timer</span> - Length of the TCP TIME-WAIT state in seconds. <span class="li-normal">type: int</span></li>
        <li> <span class="li-head">tftp</span> - Enable/disable TFTP. <span class="li-normal">type: str</span> <span class="li-normal">choices: enable, disable</span></li>
        <li> <span class="li-head">timezone</span> - Number corresponding to your time zone from 00 to 86. Enter set timezone ? to view the list of time zones and the numbers that represent them. <span class="li-normal">type: str</span> <span class="li-normal">choices: 1, 2, 3, 4, 5, 81, 6, 7, 08, 09, 10, 11, 12, 13, 74, 14, 77, 15, 87, 16, 17, 18, 19, 20, 75, 21, 22, 23, 24, 80, 79, 25, 26, 27, 28, 78, 29, 30, 31, 32, 33, 34, 35, 36, 37, 38, 83, 84, 40, 85, 41, 42, 43, 39, 44, 46, 47, 51, 48, 45, 49, 50, 52, 53, 54, 55, 56, 57, 58, 59, 60, 62, 63, 61, 64, 65, 66, 67, 68, 69, 70, 71, 72, 0, 82, 73, 86, 76</span></li>
        <li> <span class="li-head">tp_mc_skip_policy</span> - Enable/disable skip policy check and allow multicast through. <span class="li-normal">type: str</span> <span class="li-normal">choices: enable, disable</span></li>
        <li> <span class="li-head">traffic_priority</span> - Choose Type of Service (ToS) or Differentiated Services Code Point (DSCP) for traffic prioritization in traffic shaping. <span class="li-normal">type: str</span> <span class="li-normal">choices: tos, dscp</span></li>
        <li> <span class="li-head">traffic_priority_level</span> - Default system-wide level of priority for traffic prioritization. <span class="li-normal">type: str</span> <span class="li-normal">choices: low, medium, high</span></li>
        <li> <span class="li-head">two_factor_email_expiry</span> - Email-based two-factor authentication session timeout (30 - 300 seconds (5 minutes)). <span class="li-normal">type: int</span></li>
        <li> <span class="li-head">two_factor_fac_expiry</span> - FortiAuthenticator token authentication session timeout (10 - 3600 seconds (1 hour)). <span class="li-normal">type: int</span></li>
        <li> <span class="li-head">two_factor_ftk_expiry</span> - FortiToken authentication session timeout (60 - 600 sec (10 minutes)). <span class="li-normal">type: int</span></li>
        <li> <span class="li-head">two_factor_ftm_expiry</span> - FortiToken Mobile session timeout (1 - 168 hours (7 days)). <span class="li-normal">type: int</span></li>
        <li> <span class="li-head">two_factor_sms_expiry</span> - SMS-based two-factor authentication session timeout (30 - 300 sec). <span class="li-normal">type: int</span></li>
        <li> <span class="li-head">udp_idle_timer</span> - UDP connection session timeout. This command can be useful in managing CPU and memory resources (1 - 86400 seconds (1 day)). <span class="li-normal">type: int</span></li>
        <li> <span class="li-head">user_server_cert</span> - Certificate to use for https user authentication. Source certificate.local.name. <span class="li-normal">type: str</span></li>
        <li> <span class="li-head">vdom_admin</span> - Enable/disable support for multiple virtual domains (VDOMs). <span class="li-normal">type: str</span> <span class="li-normal">choices: enable, disable</span></li>
        <li> <span class="li-head">vip_arp_range</span> - Controls the number of ARPs that the FortiGate sends for a Virtual IP (VIP) address range. <span class="li-normal">type: str</span> <span class="li-normal">choices: unlimited, restricted</span></li>
        <li> <span class="li-head">virtual_server_count</span> - Maximum number of virtual server processes to create. The maximum is the number of CPU cores. This is not available on single-core CPUs. <span class="li-normal">type: int</span></li>
        <li> <span class="li-head">virtual_server_hardware_acceleration</span> - Enable/disable virtual server hardware acceleration. <span class="li-normal">type: str</span> <span class="li-normal">choices: disable, enable</span></li>
        <li> <span class="li-head">wad_affinity</span> - Affinity setting for wad (hexadecimal value up to 256 bits in the format of xxxxxxxxxxxxxxxx). <span class="li-normal">type: str</span></li>
        <li> <span class="li-head">wad_csvc_cs_count</span> - Number of concurrent WAD-cache-service object-cache processes. <span class="li-normal">type: int</span></li>
        <li> <span class="li-head">wad_csvc_db_count</span> - Number of concurrent WAD-cache-service byte-cache processes. <span class="li-normal">type: int</span></li>
        <li> <span class="li-head">wad_source_affinity</span> - Enable/disable dispatching traffic to WAD workers based on source affinity. <span class="li-normal">type: str</span> <span class="li-normal">choices: disable, enable</span></li>
        <li> <span class="li-head">wad_worker_count</span> - Number of explicit proxy WAN optimization daemon (WAD) processes. By default WAN optimization, explicit proxy, and web caching is handled by all of the CPU cores in a FortiGate unit. <span class="li-normal">type: int</span></li>
        <li> <span class="li-head">wifi_ca_certificate</span> - CA certificate that verifies the WiFi certificate. Source certificate.ca.name. <span class="li-normal">type: str</span></li>
        <li> <span class="li-head">wifi_certificate</span> - Certificate to use for WiFi authentication. Source certificate.local.name. <span class="li-normal">type: str</span></li>
        <li> <span class="li-head">wimax_4g_usb</span> - Enable/disable comparability with WiMAX 4G USB devices. <span class="li-normal">type: str</span> <span class="li-normal">choices: enable, disable</span></li>
        <li> <span class="li-head">wireless_controller</span> - Enable/disable the wireless controller feature to use the FortiGate unit to manage FortiAPs. <span class="li-normal">type: str</span> <span class="li-normal">choices: enable, disable</span></li>
        <li> <span class="li-head">wireless_controller_port</span> - Port used for the control channel in wireless controller mode (wireless-mode is ac). The data channel port is the control channel port number plus one (1024 - 49150). <span class="li-normal">type: int</span></li>
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
      - name: Configure global attributes.
        fortios_system_global:
          vdom:  "{{ vdom }}"
          system_global:
            admin_concurrent: "enable"
            admin_console_timeout: "4"
            admin_hsts_max_age: "5"
            admin_https_pki_required: "enable"
            admin_https_redirect: "enable"
            admin_https_ssl_versions: "tlsv1-0"
            admin_lockout_duration: "9"
            admin_lockout_threshold: "10"
            admin_login_max: "11"
            admin_maintainer: "enable"
            admin_port: "13"
            admin_restrict_local: "enable"
            admin_scp: "enable"
            admin_server_cert: "<your_own_value> (source certificate.local.name)"
            admin_sport: "17"
            admin_ssh_grace_time: "18"
            admin_ssh_password: "enable"
            admin_ssh_port: "20"
            admin_ssh_v1: "enable"
            admin_telnet_port: "22"
            admintimeout: "23"
            alias: "<your_own_value>"
            allow_traffic_redirect: "enable"
            anti_replay: "disable"
            arp_max_entry: "27"
            asymroute: "enable"
            auth_cert: "<your_own_value> (source certificate.local.name)"
            auth_http_port: "30"
            auth_https_port: "31"
            auth_keepalive: "enable"
            auth_session_limit: "block-new"
            auto_auth_extension_device: "enable"
            av_affinity: "<your_own_value>"
            av_failopen: "pass"
            av_failopen_session: "enable"
            batch_cmdb: "enable"
            block_session_timer: "39"
            br_fdb_max_entry: "40"
            cert_chain_max: "41"
            cfg_revert_timeout: "42"
            cfg_save: "automatic"
            check_protocol_header: "loose"
            check_reset_range: "strict"
            cli_audit_log: "enable"
            clt_cert_req: "enable"
            compliance_check: "enable"
            compliance_check_time: "<your_own_value>"
            cpu_use_threshold: "50"
            csr_ca_attribute: "enable"
            daily_restart: "enable"
            device_identification_active_scan_delay: "53"
            device_idle_timeout: "54"
            dh_params: "1024"
            dnsproxy_worker_count: "56"
            dst: "enable"
            endpoint_control_fds_access: "enable"
            endpoint_control_portal_port: "59"
            failtime: "60"
            fds_statistics: "enable"
            fds_statistics_period: "62"
            fgd_alert_subscription: "advisory"
            fortiextender: "enable"
            fortiextender_data_port: "65"
            fortiextender_vlan_mode: "enable"
            fortiservice_port: "67"
            gui_certificates: "enable"
            gui_custom_language: "enable"
            gui_date_format: "yyyy/MM/dd"
            gui_device_latitude: "<your_own_value>"
            gui_device_longitude: "<your_own_value>"
            gui_display_hostname: "enable"
            gui_ipv6: "enable"
            gui_lines_per_page: "75"
            gui_theme: "green"
            gui_wireless_opensecurity: "enable"
            honor_df: "enable"
            hostname: "myhostname"
            igmp_state_limit: "80"
            interval: "81"
            ip_src_port_range: "<your_own_value>"
            ips_affinity: "<your_own_value>"
            ipsec_asic_offload: "enable"
            ipsec_hmac_offload: "enable"
            ipsec_soft_dec_async: "enable"
            ipv6_accept_dad: "87"
            ipv6_allow_anycast_probe: "enable"
            language: "english"
            ldapconntimeout: "90"
            lldp_transmission: "enable"
            log_ssl_connection: "enable"
            log_uuid: "disable"
            login_timestamp: "enable"
            long_vdom_name: "enable"
            management_vdom: "<your_own_value> (source system.vdom.name)"
            max_dlpstat_memory: "97"
            max_route_cache_size: "98"
            mc_ttl_notchange: "enable"
            memory_use_threshold_extreme: "100"
            memory_use_threshold_green: "101"
            memory_use_threshold_red: "102"
            miglog_affinity: "<your_own_value>"
            miglogd_children: "104"
            multi_factor_authentication: "optional"
            multicast_forward: "enable"
            ndp_max_entry: "107"
            per_user_bwl: "enable"
            policy_auth_concurrent: "109"
            post_login_banner: "disable"
            pre_login_banner: "enable"
            private_data_encryption: "disable"
            proxy_auth_lifetime: "enable"
            proxy_auth_lifetime_timeout: "114"
            proxy_auth_timeout: "115"
            proxy_cipher_hardware_acceleration: "disable"
            proxy_kxp_hardware_acceleration: "disable"
            proxy_re_authentication_mode: "session"
            proxy_worker_count: "119"
            radius_port: "120"
            reboot_upon_config_restore: "enable"
            refresh: "122"
            remoteauthtimeout: "123"
            reset_sessionless_tcp: "enable"
            restart_time: "<your_own_value>"
            revision_backup_on_logout: "enable"
            revision_image_auto_backup: "enable"
            scanunit_count: "128"
            security_rating_result_submission: "enable"
            security_rating_run_on_schedule: "enable"
            send_pmtu_icmp: "enable"
            snat_route_change: "enable"
            special_file_23_support: "disable"
            ssd_trim_date: "134"
            ssd_trim_freq: "never"
            ssd_trim_hour: "136"
            ssd_trim_min: "137"
            ssd_trim_weekday: "sunday"
            ssh_cbc_cipher: "enable"
            ssh_hmac_md5: "enable"
            ssh_kex_sha1: "enable"
            ssl_min_proto_version: "SSLv3"
            ssl_static_key_ciphers: "enable"
            sslvpn_cipher_hardware_acceleration: "enable"
            sslvpn_kxp_hardware_acceleration: "enable"
            sslvpn_max_worker_count: "146"
            sslvpn_plugin_version_check: "enable"
            strict_dirty_session_check: "enable"
            strong_crypto: "enable"
            switch_controller: "disable"
            switch_controller_reserved_network: "<your_own_value>"
            sys_perf_log_interval: "152"
            tcp_halfclose_timer: "153"
            tcp_halfopen_timer: "154"
            tcp_option: "enable"
            tcp_timewait_timer: "156"
            tftp: "enable"
            timezone: "01"
            tp_mc_skip_policy: "enable"
            traffic_priority: "tos"
            traffic_priority_level: "low"
            two_factor_email_expiry: "162"
            two_factor_fac_expiry: "163"
            two_factor_ftk_expiry: "164"
            two_factor_ftm_expiry: "165"
            two_factor_sms_expiry: "166"
            udp_idle_timer: "167"
            user_server_cert: "<your_own_value> (source certificate.local.name)"
            vdom_admin: "enable"
            vip_arp_range: "unlimited"
            virtual_server_count: "171"
            virtual_server_hardware_acceleration: "disable"
            wad_affinity: "<your_own_value>"
            wad_csvc_cs_count: "174"
            wad_csvc_db_count: "175"
            wad_source_affinity: "disable"
            wad_worker_count: "177"
            wifi_ca_certificate: "<your_own_value> (source certificate.ca.name)"
            wifi_certificate: "<your_own_value> (source certificate.local.name)"
            wimax_4g_usb: "enable"
            wireless_controller: "enable"
            wireless_controller_port: "182"


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
- Hongbin Lu (@fgtdev-hblu)
- Frank Shen (@frankshen01)
- Jie Xue (@JieX19)
- Miguel Angel Munoz (@mamunozgonzalez)
- Nicolas Thomas (@thomnico)


.. hint::
    If you notice any issues in this documentation, you can create a pull request to improve it.
