:source: fortios_endpoint_control_profile.py

:orphan:

.. fortios_endpoint_control_profile:

fortios_endpoint_control_profile -- Configure FortiClient endpoint control profiles in Fortinet's FortiOS and FortiGate.
++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++

.. versionadded:: 2.8

.. contents::
   :local:
   :depth: 1


Synopsis
--------
- This module is able to configure a FortiGate or FortiOS (FOS) device by allowing the user to set and modify endpoint_control feature and profile category. Examples include all parameters and values need to be adjusted to datasources before usage. Tested with FOS v6.0.0



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
    <li> <span class="li-head">endpoint_control_profile</span> - Configure FortiClient endpoint control profiles. <span class="li-normal">type: dict</span></li>
        <ul class="ul-self">
        <li> <span class="li-head">state</span> - B(Deprecated) <span class="li-normal">type: str</span> <span class="li-required">required: False</span> <span class="li-normal">choices: present, absent</span></li>
        <li> <span class="li-head">description</span> - Description. <span class="li-normal">type: str</span></li>
        <li> <span class="li-head">device_groups</span> - Device groups. <span class="li-normal">type: list</span></li>
            <ul class="ul-self">
            <li> <span class="li-head">name</span> - Device group object from available options. Source user.device-group.name user.device-category.name. <span class="li-normal">type: str</span> <span class="li-required">required: True</span></li>
            </ul>
        <li> <span class="li-head">forticlient_android_settings</span> - FortiClient settings for Android platform. <span class="li-normal">type: dict</span></li>
            <ul class="ul-self">
            <li> <span class="li-head">disable_wf_when_protected</span> - Enable/disable FortiClient web category filtering when protected by FortiGate. <span class="li-normal">type: str</span> <span class="li-normal">choices: enable, disable</span></li>
            <li> <span class="li-head">forticlient_advanced_vpn</span> - Enable/disable advanced FortiClient VPN configuration. <span class="li-normal">type: str</span> <span class="li-normal">choices: enable, disable</span></li>
            <li> <span class="li-head">forticlient_advanced_vpn_buffer</span> - Advanced FortiClient VPN configuration. <span class="li-normal">type: str</span></li>
            <li> <span class="li-head">forticlient_vpn_provisioning</span> - Enable/disable FortiClient VPN provisioning. <span class="li-normal">type: str</span> <span class="li-normal">choices: enable, disable</span></li>
            <li> <span class="li-head">forticlient_vpn_settings</span> - FortiClient VPN settings. <span class="li-normal">type: list</span></li>
                <ul class="ul-self">
                <li> <span class="li-head">auth_method</span> - Authentication method. <span class="li-normal">type: str</span> <span class="li-normal">choices: psk, certificate</span></li>
                <li> <span class="li-head">name</span> - VPN name. <span class="li-normal">type: str</span> <span class="li-required">required: True</span></li>
                <li> <span class="li-head">preshared_key</span> - Pre-shared secret for PSK authentication. <span class="li-normal">type: str</span></li>
                <li> <span class="li-head">remote_gw</span> - IP address or FQDN of the remote VPN gateway. <span class="li-normal">type: str</span></li>
                <li> <span class="li-head">sslvpn_access_port</span> - SSL VPN access port (1 - 65535). <span class="li-normal">type: int</span></li>
                <li> <span class="li-head">sslvpn_require_certificate</span> - Enable/disable requiring SSL VPN client certificate. <span class="li-normal">type: str</span> <span class="li-normal">choices: enable, disable</span></li>
                <li> <span class="li-head">type</span> - VPN type (IPsec or SSL VPN). <span class="li-normal">type: str</span> <span class="li-normal">choices: ipsec, ssl</span></li>
                </ul>
            <li> <span class="li-head">forticlient_wf</span> - Enable/disable FortiClient web filtering. <span class="li-normal">type: str</span> <span class="li-normal">choices: enable, disable</span></li>
            <li> <span class="li-head">forticlient_wf_profile</span> - The FortiClient web filter profile to apply. Source webfilter.profile.name. <span class="li-normal">type: str</span></li>
            </ul>
        <li> <span class="li-head">forticlient_ios_settings</span> - FortiClient settings for iOS platform. <span class="li-normal">type: dict</span></li>
            <ul class="ul-self">
            <li> <span class="li-head">client_vpn_provisioning</span> - FortiClient VPN provisioning. <span class="li-normal">type: str</span> <span class="li-normal">choices: enable, disable</span></li>
            <li> <span class="li-head">client_vpn_settings</span> - FortiClient VPN settings. <span class="li-normal">type: list</span></li>
                <ul class="ul-self">
                <li> <span class="li-head">auth_method</span> - Authentication method. <span class="li-normal">type: str</span> <span class="li-normal">choices: psk, certificate</span></li>
                <li> <span class="li-head">name</span> - VPN name. <span class="li-normal">type: str</span> <span class="li-required">required: True</span></li>
                <li> <span class="li-head">preshared_key</span> - Pre-shared secret for PSK authentication. <span class="li-normal">type: str</span></li>
                <li> <span class="li-head">remote_gw</span> - IP address or FQDN of the remote VPN gateway. <span class="li-normal">type: str</span></li>
                <li> <span class="li-head">sslvpn_access_port</span> - SSL VPN access port (1 - 65535). <span class="li-normal">type: int</span></li>
                <li> <span class="li-head">sslvpn_require_certificate</span> - Enable/disable requiring SSL VPN client certificate. <span class="li-normal">type: str</span> <span class="li-normal">choices: enable, disable</span></li>
                <li> <span class="li-head">type</span> - VPN type (IPsec or SSL VPN). <span class="li-normal">type: str</span> <span class="li-normal">choices: ipsec, ssl</span></li>
                <li> <span class="li-head">vpn_configuration_content</span> - Content of VPN configuration. <span class="li-normal">type: str</span></li>
                <li> <span class="li-head">vpn_configuration_name</span> - Name of VPN configuration. <span class="li-normal">type: str</span></li>
                </ul>
            <li> <span class="li-head">configuration_content</span> - Content of configuration profile. <span class="li-normal">type: str</span></li>
            <li> <span class="li-head">configuration_name</span> - Name of configuration profile. <span class="li-normal">type: str</span></li>
            <li> <span class="li-head">disable_wf_when_protected</span> - Enable/disable FortiClient web category filtering when protected by FortiGate. <span class="li-normal">type: str</span> <span class="li-normal">choices: enable, disable</span></li>
            <li> <span class="li-head">distribute_configuration_profile</span> - Enable/disable configuration profile (.mobileconfig file) distribution. <span class="li-normal">type: str</span> <span class="li-normal">choices: enable, disable</span></li>
            <li> <span class="li-head">forticlient_wf</span> - Enable/disable FortiClient web filtering. <span class="li-normal">type: str</span> <span class="li-normal">choices: enable, disable</span></li>
            <li> <span class="li-head">forticlient_wf_profile</span> - The FortiClient web filter profile to apply. Source webfilter.profile.name. <span class="li-normal">type: str</span></li>
            </ul>
        <li> <span class="li-head">forticlient_winmac_settings</span> - FortiClient settings for Windows/Mac platform. <span class="li-normal">type: dict</span></li>
            <ul class="ul-self">
            <li> <span class="li-head">av_realtime_protection</span> - Enable/disable FortiClient AntiVirus real-time protection. <span class="li-normal">type: str</span> <span class="li-normal">choices: enable, disable</span></li>
            <li> <span class="li-head">av_signature_up_to_date</span> - Enable/disable FortiClient AV signature updates. <span class="li-normal">type: str</span> <span class="li-normal">choices: enable, disable</span></li>
            <li> <span class="li-head">forticlient_application_firewall</span> - Enable/disable the FortiClient application firewall. <span class="li-normal">type: str</span> <span class="li-normal">choices: enable, disable</span></li>
            <li> <span class="li-head">forticlient_application_firewall_list</span> - FortiClient application firewall rule list. Source application.list.name. <span class="li-normal">type: str</span></li>
            <li> <span class="li-head">forticlient_av</span> - Enable/disable FortiClient AntiVirus scanning. <span class="li-normal">type: str</span> <span class="li-normal">choices: enable, disable</span></li>
            <li> <span class="li-head">forticlient_ems_compliance</span> - Enable/disable FortiClient Enterprise Management Server (EMS) compliance. <span class="li-normal">type: str</span> <span class="li-normal">choices: enable, disable</span></li>
            <li> <span class="li-head">forticlient_ems_compliance_action</span> - FortiClient EMS compliance action. <span class="li-normal">type: str</span> <span class="li-normal">choices: block, warning</span></li>
            <li> <span class="li-head">forticlient_ems_entries</span> - FortiClient EMS entries. <span class="li-normal">type: list</span></li>
                <ul class="ul-self">
                <li> <span class="li-head">name</span> - FortiClient EMS name. Source endpoint-control.forticlient-ems.name. <span class="li-normal">type: str</span> <span class="li-required">required: True</span></li>
                </ul>
            <li> <span class="li-head">forticlient_linux_ver</span> - Minimum FortiClient Linux version. <span class="li-normal">type: str</span></li>
            <li> <span class="li-head">forticlient_log_upload</span> - Enable/disable uploading FortiClient logs. <span class="li-normal">type: str</span> <span class="li-normal">choices: enable, disable</span></li>
            <li> <span class="li-head">forticlient_log_upload_level</span> - Select the FortiClient logs to upload. <span class="li-normal">type: str</span> <span class="li-normal">choices: traffic, vulnerability, event</span></li>
            <li> <span class="li-head">forticlient_log_upload_server</span> - IP address or FQDN of the server to which to upload FortiClient logs. <span class="li-normal">type: str</span></li>
            <li> <span class="li-head">forticlient_mac_ver</span> - Minimum FortiClient Mac OS version. <span class="li-normal">type: str</span></li>
            <li> <span class="li-head">forticlient_minimum_software_version</span> - Enable/disable requiring clients to run FortiClient with a minimum software version number. <span class="li-normal">type: str</span> <span class="li-normal">choices: enable, disable</span></li>
            <li> <span class="li-head">forticlient_operating_system</span> - FortiClient operating system. <span class="li-normal">type: list</span></li>
                <ul class="ul-self">
                <li> <span class="li-head">id</span> - Operating system entry ID. <span class="li-normal">type: int</span> <span class="li-required">required: True</span></li>
                <li> <span class="li-head">os_name</span> - Customize operating system name or Mac OS format:x.x.x <span class="li-normal">type: str</span></li>
                <li> <span class="li-head">os_type</span> - Operating system type. <span class="li-normal">type: str</span> <span class="li-normal">choices: custom, mac-os, win-7, win-80, win-81, win-10, win-2000, win-home-svr, win-svr-10, win-svr-2003, win-svr-2003-r2, win-svr-2008, win-svr-2008-r2, win-svr-2012, win-svr-2012-r2, win-sto-svr-2003, win-vista, win-xp, ubuntu-linux, centos-linux, redhat-linux, fedora-linux</span></li>
                </ul>
            <li> <span class="li-head">forticlient_own_file</span> - Checking the path and filename of the FortiClient application. <span class="li-normal">type: list</span></li>
                <ul class="ul-self">
                <li> <span class="li-head">file</span> - File path and name. <span class="li-normal">type: str</span></li>
                <li> <span class="li-head">id</span> - File ID. <span class="li-normal">type: int</span> <span class="li-required">required: True</span></li>
                </ul>
            <li> <span class="li-head">forticlient_registration_compliance_action</span> - FortiClient registration compliance action. <span class="li-normal">type: str</span> <span class="li-normal">choices: block, warning</span></li>
            <li> <span class="li-head">forticlient_registry_entry</span> - FortiClient registry entry. <span class="li-normal">type: list</span></li>
                <ul class="ul-self">
                <li> <span class="li-head">id</span> - Registry entry ID. <span class="li-normal">type: int</span> <span class="li-required">required: True</span></li>
                <li> <span class="li-head">registry_entry</span> - Registry entry. <span class="li-normal">type: str</span></li>
                </ul>
            <li> <span class="li-head">forticlient_running_app</span> - Use FortiClient to verify if the listed applications are running on the client. <span class="li-normal">type: list</span></li>
                <ul class="ul-self">
                <li> <span class="li-head">app_name</span> - Application name. <span class="li-normal">type: str</span></li>
                <li> <span class="li-head">app_sha256_signature</span> - App"s SHA256 signature. <span class="li-normal">type: str</span></li>
                <li> <span class="li-head">app_sha256_signature2</span> - App"s SHA256 Signature. <span class="li-normal">type: str</span></li>
                <li> <span class="li-head">app_sha256_signature3</span> - App"s SHA256 Signature. <span class="li-normal">type: str</span></li>
                <li> <span class="li-head">app_sha256_signature4</span> - App"s SHA256 Signature. <span class="li-normal">type: str</span></li>
                <li> <span class="li-head">application_check_rule</span> - Application check rule. <span class="li-normal">type: str</span> <span class="li-normal">choices: present, absent</span></li>
                <li> <span class="li-head">id</span> - Application ID. <span class="li-normal">type: int</span> <span class="li-required">required: True</span></li>
                <li> <span class="li-head">process_name</span> - Process name. <span class="li-normal">type: str</span></li>
                <li> <span class="li-head">process_name2</span> - Process name. <span class="li-normal">type: str</span></li>
                <li> <span class="li-head">process_name3</span> - Process name. <span class="li-normal">type: str</span></li>
                <li> <span class="li-head">process_name4</span> - Process name. <span class="li-normal">type: str</span></li>
                </ul>
            <li> <span class="li-head">forticlient_security_posture</span> - Enable/disable FortiClient security posture check options. <span class="li-normal">type: str</span> <span class="li-normal">choices: enable, disable</span></li>
            <li> <span class="li-head">forticlient_security_posture_compliance_action</span> - FortiClient security posture compliance action. <span class="li-normal">type: str</span> <span class="li-normal">choices: block, warning</span></li>
            <li> <span class="li-head">forticlient_system_compliance</span> - Enable/disable enforcement of FortiClient system compliance. <span class="li-normal">type: str</span> <span class="li-normal">choices: enable, disable</span></li>
            <li> <span class="li-head">forticlient_system_compliance_action</span> - Block or warn clients not compliant with FortiClient requirements. <span class="li-normal">type: str</span> <span class="li-normal">choices: block, warning</span></li>
            <li> <span class="li-head">forticlient_vuln_scan</span> - Enable/disable FortiClient vulnerability scanning. <span class="li-normal">type: str</span> <span class="li-normal">choices: enable, disable</span></li>
            <li> <span class="li-head">forticlient_vuln_scan_compliance_action</span> - FortiClient vulnerability compliance action. <span class="li-normal">type: str</span> <span class="li-normal">choices: block, warning</span></li>
            <li> <span class="li-head">forticlient_vuln_scan_enforce</span> - Configure the level of the vulnerability found that causes a FortiClient vulnerability compliance action. <span class="li-normal">type: str</span> <span class="li-normal">choices: critical, high, medium, low, info</span></li>
            <li> <span class="li-head">forticlient_vuln_scan_enforce_grace</span> - FortiClient vulnerability scan enforcement grace period (0 - 30 days). <span class="li-normal">type: int</span></li>
            <li> <span class="li-head">forticlient_vuln_scan_exempt</span> - Enable/disable compliance exemption for vulnerabilities that cannot be patched automatically. <span class="li-normal">type: str</span> <span class="li-normal">choices: enable, disable</span></li>
            <li> <span class="li-head">forticlient_wf</span> - Enable/disable FortiClient web filtering. <span class="li-normal">type: str</span> <span class="li-normal">choices: enable, disable</span></li>
            <li> <span class="li-head">forticlient_wf_profile</span> - The FortiClient web filter profile to apply. Source webfilter.profile.name. <span class="li-normal">type: str</span></li>
            <li> <span class="li-head">forticlient_win_ver</span> - Minimum FortiClient Windows version. <span class="li-normal">type: str</span></li>
            <li> <span class="li-head">os_av_software_installed</span> - Enable/disable checking for OS recognized AntiVirus software. <span class="li-normal">type: str</span> <span class="li-normal">choices: enable, disable</span></li>
            <li> <span class="li-head">sandbox_address</span> - FortiSandbox address. <span class="li-normal">type: str</span></li>
            <li> <span class="li-head">sandbox_analysis</span> - Enable/disable sending files to FortiSandbox for analysis. <span class="li-normal">type: str</span> <span class="li-normal">choices: enable, disable</span></li>
            </ul>
        <li> <span class="li-head">on_net_addr</span> - Addresses for on-net detection. <span class="li-normal">type: list</span></li>
            <ul class="ul-self">
            <li> <span class="li-head">name</span> - Address object from available options. Source firewall.address.name firewall.addrgrp.name. <span class="li-normal">type: str</span> <span class="li-required">required: True</span></li>
            </ul>
        <li> <span class="li-head">profile_name</span> - Profile name. <span class="li-normal">type: str</span></li>
        <li> <span class="li-head">replacemsg_override_group</span> - Select an endpoint control replacement message override group from available options. Source system.replacemsg-group.name. <span class="li-normal">type: str</span></li>
        <li> <span class="li-head">src_addr</span> - Source addresses. <span class="li-normal">type: list</span></li>
            <ul class="ul-self">
            <li> <span class="li-head">name</span> - Address object from available options. Source firewall.address.name firewall.addrgrp.name. <span class="li-normal">type: str</span> <span class="li-required">required: True</span></li>
            </ul>
        <li> <span class="li-head">user_groups</span> - User groups. <span class="li-normal">type: list</span></li>
            <ul class="ul-self">
            <li> <span class="li-head">name</span> - User group name. Source user.group.name. <span class="li-normal">type: str</span> <span class="li-required">required: True</span></li>
            </ul>
        <li> <span class="li-head">users</span> - Users. <span class="li-normal">type: list</span></li>
            <ul class="ul-self">
            <li> <span class="li-head">name</span> - User name. Source user.local.name. <span class="li-normal">type: str</span> <span class="li-required">required: True</span></li>
            </ul>
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
      - name: Configure FortiClient endpoint control profiles.
        fortios_endpoint_control_profile:
          vdom:  "{{ vdom }}"
          state: "present"
          endpoint_control_profile:
            description: "<your_own_value>"
            device_groups:
             -
                name: "default_name_5 (source user.device-group.name user.device-category.name)"
            forticlient_android_settings:
                disable_wf_when_protected: "enable"
                forticlient_advanced_vpn: "enable"
                forticlient_advanced_vpn_buffer: "<your_own_value>"
                forticlient_vpn_provisioning: "enable"
                forticlient_vpn_settings:
                 -
                    auth_method: "psk"
                    name: "default_name_13"
                    preshared_key: "<your_own_value>"
                    remote_gw: "<your_own_value>"
                    sslvpn_access_port: "16"
                    sslvpn_require_certificate: "enable"
                    type: "ipsec"
                forticlient_wf: "enable"
                forticlient_wf_profile: "<your_own_value> (source webfilter.profile.name)"
            forticlient_ios_settings:
                client_vpn_provisioning: "enable"
                client_vpn_settings:
                 -
                    auth_method: "psk"
                    name: "default_name_25"
                    preshared_key: "<your_own_value>"
                    remote_gw: "<your_own_value>"
                    sslvpn_access_port: "28"
                    sslvpn_require_certificate: "enable"
                    type: "ipsec"
                    vpn_configuration_content: "<your_own_value>"
                    vpn_configuration_name: "<your_own_value>"
                configuration_content: "<your_own_value>"
                configuration_name: "<your_own_value>"
                disable_wf_when_protected: "enable"
                distribute_configuration_profile: "enable"
                forticlient_wf: "enable"
                forticlient_wf_profile: "<your_own_value> (source webfilter.profile.name)"
            forticlient_winmac_settings:
                av_realtime_protection: "enable"
                av_signature_up_to_date: "enable"
                forticlient_application_firewall: "enable"
                forticlient_application_firewall_list: "<your_own_value> (source application.list.name)"
                forticlient_av: "enable"
                forticlient_ems_compliance: "enable"
                forticlient_ems_compliance_action: "block"
                forticlient_ems_entries:
                 -
                    name: "default_name_48 (source endpoint-control.forticlient-ems.name)"
                forticlient_linux_ver: "<your_own_value>"
                forticlient_log_upload: "enable"
                forticlient_log_upload_level: "traffic"
                forticlient_log_upload_server: "<your_own_value>"
                forticlient_mac_ver: "<your_own_value>"
                forticlient_minimum_software_version: "enable"
                forticlient_operating_system:
                 -
                    id:  "56"
                    os_name: "<your_own_value>"
                    os_type: "custom"
                forticlient_own_file:
                 -
                    file: "<your_own_value>"
                    id:  "61"
                forticlient_registration_compliance_action: "block"
                forticlient_registry_entry:
                 -
                    id:  "64"
                    registry_entry: "<your_own_value>"
                forticlient_running_app:
                 -
                    app_name: "<your_own_value>"
                    app_sha256_signature: "<your_own_value>"
                    app_sha256_signature2: "<your_own_value>"
                    app_sha256_signature3: "<your_own_value>"
                    app_sha256_signature4: "<your_own_value>"
                    application_check_rule: "present"
                    id:  "73"
                    process_name: "<your_own_value>"
                    process_name2: "<your_own_value>"
                    process_name3: "<your_own_value>"
                    process_name4: "<your_own_value>"
                forticlient_security_posture: "enable"
                forticlient_security_posture_compliance_action: "block"
                forticlient_system_compliance: "enable"
                forticlient_system_compliance_action: "block"
                forticlient_vuln_scan: "enable"
                forticlient_vuln_scan_compliance_action: "block"
                forticlient_vuln_scan_enforce: "critical"
                forticlient_vuln_scan_enforce_grace: "85"
                forticlient_vuln_scan_exempt: "enable"
                forticlient_wf: "enable"
                forticlient_wf_profile: "<your_own_value> (source webfilter.profile.name)"
                forticlient_win_ver: "<your_own_value>"
                os_av_software_installed: "enable"
                sandbox_address: "<your_own_value>"
                sandbox_analysis: "enable"
            on_net_addr:
             -
                name: "default_name_94 (source firewall.address.name firewall.addrgrp.name)"
            profile_name: "<your_own_value>"
            replacemsg_override_group: "<your_own_value> (source system.replacemsg-group.name)"
            src_addr:
             -
                name: "default_name_98 (source firewall.address.name firewall.addrgrp.name)"
            user_groups:
             -
                name: "default_name_100 (source user.group.name)"
            users:
             -
                name: "default_name_102 (source user.local.name)"


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
