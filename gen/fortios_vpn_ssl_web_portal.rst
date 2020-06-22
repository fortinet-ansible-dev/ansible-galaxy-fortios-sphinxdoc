:source: fortios_vpn_ssl_web_portal.py

:orphan:

.. fortios_vpn_ssl_web_portal:

fortios_vpn_ssl_web_portal -- Portal in Fortinet's FortiOS and FortiGate.
+++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++

.. versionadded:: 2.8

.. contents::
   :local:
   :depth: 1


Synopsis
--------
- This module is able to configure a FortiGate or FortiOS (FOS) device by allowing the user to set and modify vpn_ssl_web feature and portal category. Examples include all parameters and values need to be adjusted to datasources before usage. Tested with FOS v6.0.5



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
    <li> <span class="li-head">state</span> - Indicates whether to create or remove the object. This attribute was present already in previous version in a deeper level. It has been moved out to this outer level. <span class="li-normal">type: str</span> <span class="li-required">required: False</span> <span class="li-normal">choices: present, absent</span></li>
    <li> <span class="li-head">vpn_ssl_web_portal</span> - Portal. <span class="li-normal">type: dict</span></li>
        <ul class="ul-self">
        <li> <span class="li-head">state</span> - B(Deprecated) <span class="li-normal">type: str</span> <span class="li-required">required: False</span> <span class="li-normal">choices: present, absent</span></li>
        <li> <span class="li-head">allow_user_access</span> - Allow user access to SSL-VPN applications. <span class="li-normal">type: str</span> <span class="li-normal">choices: web, ftp, smb, telnet, ssh, vnc, rdp, ping, citrix, portforward</span></li>
        <li> <span class="li-head">auto_connect</span> - Enable/disable automatic connect by client when system is up. <span class="li-normal">type: str</span> <span class="li-normal">choices: enable, disable</span></li>
        <li> <span class="li-head">bookmark_group</span> - Portal bookmark group. <span class="li-normal">type: list</span></li>
            <ul class="ul-self">
            <li> <span class="li-head">bookmarks</span> - Bookmark table. <span class="li-normal">type: list</span></li>
                <ul class="ul-self">
                <li> <span class="li-head">additional_params</span> - Additional parameters. <span class="li-normal">type: str</span></li>
                <li> <span class="li-head">apptype</span> - Application type. <span class="li-normal">type: str</span> <span class="li-normal">choices: citrix, ftp, portforward, rdp, smb, ssh, telnet, vnc, web</span></li>
                <li> <span class="li-head">description</span> - Description. <span class="li-normal">type: str</span></li>
                <li> <span class="li-head">folder</span> - Network shared file folder parameter. <span class="li-normal">type: str</span></li>
                <li> <span class="li-head">form_data</span> - Form data. <span class="li-normal">type: list</span></li>
                    <ul class="ul-self">
                    <li> <span class="li-head">name</span> - Name. <span class="li-normal">type: str</span> <span class="li-required">required: True</span></li>
                    <li> <span class="li-head">value</span> - Value. <span class="li-normal">type: str</span></li>
                    </ul>
                <li> <span class="li-head">host</span> - Host name/IP parameter. <span class="li-normal">type: str</span></li>
                <li> <span class="li-head">listening_port</span> - Listening port (0 - 65535). <span class="li-normal">type: int</span></li>
                <li> <span class="li-head">load_balancing_info</span> - The load balancing information or cookie which should be provided to the connection broker. <span class="li-normal">type: str</span></li>
                <li> <span class="li-head">logon_password</span> - Logon password. <span class="li-normal">type: str</span></li>
                <li> <span class="li-head">logon_user</span> - Logon user. <span class="li-normal">type: str</span></li>
                <li> <span class="li-head">name</span> - Bookmark name. <span class="li-normal">type: str</span> <span class="li-required">required: True</span></li>
                <li> <span class="li-head">port</span> - Remote port. <span class="li-normal">type: int</span></li>
                <li> <span class="li-head">preconnection_blob</span> - An arbitrary string which identifies the RDP source. <span class="li-normal">type: str</span></li>
                <li> <span class="li-head">preconnection_id</span> - The numeric ID of the RDP source (0-2147483648). <span class="li-normal">type: int</span></li>
                <li> <span class="li-head">remote_port</span> - Remote port (0 - 65535). <span class="li-normal">type: int</span></li>
                <li> <span class="li-head">security</span> - Security mode for RDP connection. <span class="li-normal">type: str</span> <span class="li-normal">choices: rdp, nla, tls, any</span></li>
                <li> <span class="li-head">server_layout</span> - Server side keyboard layout. <span class="li-normal">type: str</span> <span class="li-normal">choices: de-de-qwertz, en-gb-qwerty, en-us-qwerty, es-es-qwerty, fr-fr-azerty, fr-ch-qwertz, it-it-qwerty, ja-jp-qwerty, pt-br-qwerty, sv-se-qwerty, tr-tr-qwerty, failsafe</span></li>
                <li> <span class="li-head">show_status_window</span> - Enable/disable showing of status window. <span class="li-normal">type: str</span> <span class="li-normal">choices: enable, disable</span></li>
                <li> <span class="li-head">sso</span> - Single Sign-On. <span class="li-normal">type: str</span> <span class="li-normal">choices: disable, static, auto</span></li>
                <li> <span class="li-head">sso_credential</span> - Single sign-on credentials. <span class="li-normal">type: str</span> <span class="li-normal">choices: sslvpn-login, alternative</span></li>
                <li> <span class="li-head">sso_credential_sent_once</span> - Single sign-on credentials are only sent once to remote server. <span class="li-normal">type: str</span> <span class="li-normal">choices: enable, disable</span></li>
                <li> <span class="li-head">sso_password</span> - SSO password. <span class="li-normal">type: str</span></li>
                <li> <span class="li-head">sso_username</span> - SSO user name. <span class="li-normal">type: str</span></li>
                <li> <span class="li-head">url</span> - URL parameter. <span class="li-normal">type: str</span></li>
                </ul>
            <li> <span class="li-head">name</span> - Bookmark group name. <span class="li-normal">type: str</span> <span class="li-required">required: True</span></li>
            </ul>
        <li> <span class="li-head">custom_lang</span> - Change the web portal display language. Overrides config system global set language. You can use config system custom-language and execute system custom-language to add custom language files. Source system.custom-language.name. <span class="li-normal">type: str</span></li>
        <li> <span class="li-head">customize_forticlient_download_url</span> - Enable support of customized download URL for FortiClient. <span class="li-normal">type: str</span> <span class="li-normal">choices: enable, disable</span></li>
        <li> <span class="li-head">display_bookmark</span> - Enable to display the web portal bookmark widget. <span class="li-normal">type: str</span> <span class="li-normal">choices: enable, disable</span></li>
        <li> <span class="li-head">display_connection_tools</span> - Enable to display the web portal connection tools widget. <span class="li-normal">type: str</span> <span class="li-normal">choices: enable, disable</span></li>
        <li> <span class="li-head">display_history</span> - Enable to display the web portal user login history widget. <span class="li-normal">type: str</span> <span class="li-normal">choices: enable, disable</span></li>
        <li> <span class="li-head">display_status</span> - Enable to display the web portal status widget. <span class="li-normal">type: str</span> <span class="li-normal">choices: enable, disable</span></li>
        <li> <span class="li-head">dns_server1</span> - IPv4 DNS server 1. <span class="li-normal">type: str</span></li>
        <li> <span class="li-head">dns_server2</span> - IPv4 DNS server 2. <span class="li-normal">type: str</span></li>
        <li> <span class="li-head">dns_suffix</span> - DNS suffix. <span class="li-normal">type: str</span></li>
        <li> <span class="li-head">exclusive_routing</span> - Enable/disable all traffic go through tunnel only. <span class="li-normal">type: str</span> <span class="li-normal">choices: enable, disable</span></li>
        <li> <span class="li-head">forticlient_download</span> - Enable/disable download option for FortiClient. <span class="li-normal">type: str</span> <span class="li-normal">choices: enable, disable</span></li>
        <li> <span class="li-head">forticlient_download_method</span> - FortiClient download method. <span class="li-normal">type: str</span> <span class="li-normal">choices: direct, ssl-vpn</span></li>
        <li> <span class="li-head">heading</span> - Web portal heading message. <span class="li-normal">type: str</span></li>
        <li> <span class="li-head">hide_sso_credential</span> - Enable to prevent SSO credential being sent to client. <span class="li-normal">type: str</span> <span class="li-normal">choices: enable, disable</span></li>
        <li> <span class="li-head">host_check</span> - Type of host checking performed on endpoints. <span class="li-normal">type: str</span> <span class="li-normal">choices: none, av, fw, av-fw, custom</span></li>
        <li> <span class="li-head">host_check_interval</span> - Periodic host check interval. Value of 0 means disabled and host checking only happens when the endpoint connects. <span class="li-normal">type: int</span></li>
        <li> <span class="li-head">host_check_policy</span> - One or more policies to require the endpoint to have specific security software. <span class="li-normal">type: list</span></li>
            <ul class="ul-self">
            <li> <span class="li-head">name</span> - Host check software list name. Source vpn.ssl.web.host-check-software.name. <span class="li-normal">type: str</span> <span class="li-required">required: True</span></li>
            </ul>
        <li> <span class="li-head">ip_mode</span> - Method by which users of this SSL-VPN tunnel obtain IP addresses. <span class="li-normal">type: str</span> <span class="li-normal">choices: range, user-group</span></li>
        <li> <span class="li-head">ip_pools</span> - IPv4 firewall source address objects reserved for SSL-VPN tunnel mode clients. <span class="li-normal">type: list</span></li>
            <ul class="ul-self">
            <li> <span class="li-head">name</span> - Address name. Source firewall.address.name firewall.addrgrp.name. <span class="li-normal">type: str</span> <span class="li-required">required: True</span></li>
            </ul>
        <li> <span class="li-head">ipv6_dns_server1</span> - IPv6 DNS server 1. <span class="li-normal">type: str</span></li>
        <li> <span class="li-head">ipv6_dns_server2</span> - IPv6 DNS server 2. <span class="li-normal">type: str</span></li>
        <li> <span class="li-head">ipv6_exclusive_routing</span> - Enable/disable all IPv6 traffic go through tunnel only. <span class="li-normal">type: str</span> <span class="li-normal">choices: enable, disable</span></li>
        <li> <span class="li-head">ipv6_pools</span> - IPv4 firewall source address objects reserved for SSL-VPN tunnel mode clients. <span class="li-normal">type: list</span></li>
            <ul class="ul-self">
            <li> <span class="li-head">name</span> - Address name. Source firewall.address6.name firewall.addrgrp6.name. <span class="li-normal">type: str</span> <span class="li-required">required: True</span></li>
            </ul>
        <li> <span class="li-head">ipv6_service_restriction</span> - Enable/disable IPv6 tunnel service restriction. <span class="li-normal">type: str</span> <span class="li-normal">choices: enable, disable</span></li>
        <li> <span class="li-head">ipv6_split_tunneling</span> - Enable/disable IPv6 split tunneling. <span class="li-normal">type: str</span> <span class="li-normal">choices: enable, disable</span></li>
        <li> <span class="li-head">ipv6_split_tunneling_routing_address</span> - IPv6 SSL-VPN tunnel mode firewall address objects that override firewall policy destination addresses to control split-tunneling access. <span class="li-normal">type: list</span></li>
            <ul class="ul-self">
            <li> <span class="li-head">name</span> - Address name. Source firewall.address6.name firewall.addrgrp6.name. <span class="li-normal">type: str</span> <span class="li-required">required: True</span></li>
            </ul>
        <li> <span class="li-head">ipv6_tunnel_mode</span> - Enable/disable IPv6 SSL-VPN tunnel mode. <span class="li-normal">type: str</span> <span class="li-normal">choices: enable, disable</span></li>
        <li> <span class="li-head">ipv6_wins_server1</span> - IPv6 WINS server 1. <span class="li-normal">type: str</span></li>
        <li> <span class="li-head">ipv6_wins_server2</span> - IPv6 WINS server 2. <span class="li-normal">type: str</span></li>
        <li> <span class="li-head">keep_alive</span> - Enable/disable automatic reconnect for FortiClient connections. <span class="li-normal">type: str</span> <span class="li-normal">choices: enable, disable</span></li>
        <li> <span class="li-head">limit_user_logins</span> - Enable to limit each user to one SSL-VPN session at a time. <span class="li-normal">type: str</span> <span class="li-normal">choices: enable, disable</span></li>
        <li> <span class="li-head">mac_addr_action</span> - Client MAC address action. <span class="li-normal">type: str</span> <span class="li-normal">choices: allow, deny</span></li>
        <li> <span class="li-head">mac_addr_check</span> - Enable/disable MAC address host checking. <span class="li-normal">type: str</span> <span class="li-normal">choices: enable, disable</span></li>
        <li> <span class="li-head">mac_addr_check_rule</span> - Client MAC address check rule. <span class="li-normal">type: list</span></li>
            <ul class="ul-self">
            <li> <span class="li-head">mac_addr_list</span> - Client MAC address list. <span class="li-normal">type: list</span></li>
                <ul class="ul-self">
                <li> <span class="li-head">addr</span> - Client MAC address. <span class="li-normal">type: str</span> <span class="li-required">required: True</span></li>
                </ul>
            <li> <span class="li-head">mac_addr_mask</span> - Client MAC address mask. <span class="li-normal">type: int</span></li>
            <li> <span class="li-head">name</span> - Client MAC address check rule name. <span class="li-normal">type: str</span> <span class="li-required">required: True</span></li>
            </ul>
        <li> <span class="li-head">macos_forticlient_download_url</span> - Download URL for Mac FortiClient. <span class="li-normal">type: str</span></li>
        <li> <span class="li-head">name</span> - Portal name. <span class="li-normal">type: str</span> <span class="li-required">required: True</span></li>
        <li> <span class="li-head">os_check</span> - Enable to let the FortiGate decide action based on client OS. <span class="li-normal">type: str</span> <span class="li-normal">choices: enable, disable</span></li>
        <li> <span class="li-head">os_check_list</span> - SSL VPN OS checks. <span class="li-normal">type: list</span></li>
            <ul class="ul-self">
            <li> <span class="li-head">action</span> - OS check options. <span class="li-normal">type: str</span> <span class="li-normal">choices: deny, allow, check-up-to-date</span></li>
            <li> <span class="li-head">latest_patch_level</span> - Latest OS patch level. <span class="li-normal">type: str</span></li>
            <li> <span class="li-head">name</span> - Name. <span class="li-normal">type: str</span> <span class="li-required">required: True</span></li>
            <li> <span class="li-head">tolerance</span> - OS patch level tolerance. <span class="li-normal">type: int</span></li>
            </ul>
        <li> <span class="li-head">redir_url</span> - Client login redirect URL. <span class="li-normal">type: str</span></li>
        <li> <span class="li-head">save_password</span> - Enable/disable FortiClient saving the user"s password. <span class="li-normal">type: str</span> <span class="li-normal">choices: enable, disable</span></li>
        <li> <span class="li-head">service_restriction</span> - Enable/disable tunnel service restriction. <span class="li-normal">type: str</span> <span class="li-normal">choices: enable, disable</span></li>
        <li> <span class="li-head">skip_check_for_unsupported_browser</span> - Enable to skip host check if browser does not support it. <span class="li-normal">type: str</span> <span class="li-normal">choices: enable, disable</span></li>
        <li> <span class="li-head">skip_check_for_unsupported_os</span> - Enable to skip host check if client OS does not support it. <span class="li-normal">type: str</span> <span class="li-normal">choices: enable, disable</span></li>
        <li> <span class="li-head">smb_ntlmv1_auth</span> - Enable support of NTLMv1 for Samba authentication. <span class="li-normal">type: str</span> <span class="li-normal">choices: enable, disable</span></li>
        <li> <span class="li-head">smbv1</span> - Enable/disable support of SMBv1 for Samba. <span class="li-normal">type: str</span> <span class="li-normal">choices: enable, disable</span></li>
        <li> <span class="li-head">split_dns</span> - Split DNS for SSL VPN. <span class="li-normal">type: list</span></li>
            <ul class="ul-self">
            <li> <span class="li-head">dns_server1</span> - DNS server 1. <span class="li-normal">type: str</span></li>
            <li> <span class="li-head">dns_server2</span> - DNS server 2. <span class="li-normal">type: str</span></li>
            <li> <span class="li-head">domains</span> - Split DNS domains used for SSL-VPN clients separated by comma(,). <span class="li-normal">type: str</span></li>
            <li> <span class="li-head">id</span> - ID. <span class="li-normal">type: int</span> <span class="li-required">required: True</span></li>
            <li> <span class="li-head">ipv6_dns_server1</span> - IPv6 DNS server 1. <span class="li-normal">type: str</span></li>
            <li> <span class="li-head">ipv6_dns_server2</span> - IPv6 DNS server 2. <span class="li-normal">type: str</span></li>
            </ul>
        <li> <span class="li-head">split_tunneling</span> - Enable/disable IPv4 split tunneling. <span class="li-normal">type: str</span> <span class="li-normal">choices: enable, disable</span></li>
        <li> <span class="li-head">split_tunneling_routing_address</span> - IPv4 SSL-VPN tunnel mode firewall address objects that override firewall policy destination addresses to control split-tunneling access. <span class="li-normal">type: list</span></li>
            <ul class="ul-self">
            <li> <span class="li-head">name</span> - Address name. Source firewall.address.name firewall.addrgrp.name. <span class="li-normal">type: str</span> <span class="li-required">required: True</span></li>
            </ul>
        <li> <span class="li-head">theme</span> - Web portal color scheme. <span class="li-normal">type: str</span> <span class="li-normal">choices: blue, green, red, melongene, mariner</span></li>
        <li> <span class="li-head">tunnel_mode</span> - Enable/disable IPv4 SSL-VPN tunnel mode. <span class="li-normal">type: str</span> <span class="li-normal">choices: enable, disable</span></li>
        <li> <span class="li-head">user_bookmark</span> - Enable to allow web portal users to create their own bookmarks. <span class="li-normal">type: str</span> <span class="li-normal">choices: enable, disable</span></li>
        <li> <span class="li-head">user_group_bookmark</span> - Enable to allow web portal users to create bookmarks for all users in the same user group. <span class="li-normal">type: str</span> <span class="li-normal">choices: enable, disable</span></li>
        <li> <span class="li-head">web_mode</span> - Enable/disable SSL VPN web mode. <span class="li-normal">type: str</span> <span class="li-normal">choices: enable, disable</span></li>
        <li> <span class="li-head">windows_forticlient_download_url</span> - Download URL for Windows FortiClient. <span class="li-normal">type: str</span></li>
        <li> <span class="li-head">wins_server1</span> - IPv4 WINS server 1. <span class="li-normal">type: str</span></li>
        <li> <span class="li-head">wins_server2</span> - IPv4 WINS server 1. <span class="li-normal">type: str</span></li>
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
      - name: Portal.
        fortios_vpn_ssl_web_portal:
          vdom:  "{{ vdom }}"
          state: "present"
          vpn_ssl_web_portal:
            allow_user_access: "web"
            auto_connect: "enable"
            bookmark_group:
             -
                bookmarks:
                 -
                    additional_params: "<your_own_value>"
                    apptype: "citrix"
                    description: "<your_own_value>"
                    folder: "<your_own_value>"
                    form_data:
                     -
                        name: "default_name_12"
                        value: "<your_own_value>"
                    host: "<your_own_value>"
                    listening_port: "15"
                    load_balancing_info: "<your_own_value>"
                    logon_password: "<your_own_value>"
                    logon_user: "<your_own_value>"
                    name: "default_name_19"
                    port: "20"
                    preconnection_blob: "<your_own_value>"
                    preconnection_id: "22"
                    remote_port: "23"
                    security: "rdp"
                    server_layout: "de-de-qwertz"
                    show_status_window: "enable"
                    sso: "disable"
                    sso_credential: "sslvpn-login"
                    sso_credential_sent_once: "enable"
                    sso_password: "<your_own_value>"
                    sso_username: "<your_own_value>"
                    url: "myurl.com"
                name: "default_name_33"
            custom_lang: "<your_own_value> (source system.custom-language.name)"
            customize_forticlient_download_url: "enable"
            display_bookmark: "enable"
            display_connection_tools: "enable"
            display_history: "enable"
            display_status: "enable"
            dns_server1: "<your_own_value>"
            dns_server2: "<your_own_value>"
            dns_suffix: "<your_own_value>"
            exclusive_routing: "enable"
            forticlient_download: "enable"
            forticlient_download_method: "direct"
            heading: "<your_own_value>"
            hide_sso_credential: "enable"
            host_check: "none"
            host_check_interval: "49"
            host_check_policy:
             -
                name: "default_name_51 (source vpn.ssl.web.host-check-software.name)"
            ip_mode: "range"
            ip_pools:
             -
                name: "default_name_54 (source firewall.address.name firewall.addrgrp.name)"
            ipv6_dns_server1: "<your_own_value>"
            ipv6_dns_server2: "<your_own_value>"
            ipv6_exclusive_routing: "enable"
            ipv6_pools:
             -
                name: "default_name_59 (source firewall.address6.name firewall.addrgrp6.name)"
            ipv6_service_restriction: "enable"
            ipv6_split_tunneling: "enable"
            ipv6_split_tunneling_routing_address:
             -
                name: "default_name_63 (source firewall.address6.name firewall.addrgrp6.name)"
            ipv6_tunnel_mode: "enable"
            ipv6_wins_server1: "<your_own_value>"
            ipv6_wins_server2: "<your_own_value>"
            keep_alive: "enable"
            limit_user_logins: "enable"
            mac_addr_action: "allow"
            mac_addr_check: "enable"
            mac_addr_check_rule:
             -
                mac_addr_list:
                 -
                    addr: "<your_own_value>"
                mac_addr_mask: "74"
                name: "default_name_75"
            macos_forticlient_download_url: "<your_own_value>"
            name: "default_name_77"
            os_check: "enable"
            os_check_list:
             -
                action: "deny"
                latest_patch_level: "<your_own_value>"
                name: "default_name_82"
                tolerance: "83"
            redir_url: "<your_own_value>"
            save_password: "enable"
            service_restriction: "enable"
            skip_check_for_unsupported_browser: "enable"
            skip_check_for_unsupported_os: "enable"
            smb_ntlmv1_auth: "enable"
            smbv1: "enable"
            split_dns:
             -
                dns_server1: "<your_own_value>"
                dns_server2: "<your_own_value>"
                domains: "<your_own_value>"
                id:  "95"
                ipv6_dns_server1: "<your_own_value>"
                ipv6_dns_server2: "<your_own_value>"
            split_tunneling: "enable"
            split_tunneling_routing_address:
             -
                name: "default_name_100 (source firewall.address.name firewall.addrgrp.name)"
            theme: "blue"
            tunnel_mode: "enable"
            user_bookmark: "enable"
            user_group_bookmark: "enable"
            web_mode: "enable"
            windows_forticlient_download_url: "<your_own_value>"
            wins_server1: "<your_own_value>"
            wins_server2: "<your_own_value>"


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
