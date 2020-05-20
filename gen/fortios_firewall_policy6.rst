:source: fortios_firewall_policy6.py

:orphan:

.. fortios_firewall_policy6:

fortios_firewall_policy6 -- Configure IPv6 policies in Fortinet's FortiOS and FortiGate.
++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++

.. versionadded:: 2.8

.. contents::
   :local:
   :depth: 1


Synopsis
--------
- This module is able to configure a FortiGate or FortiOS (FOS) device by allowing the user to set and modify firewall feature and policy6 category. Examples include all parameters and values need to be adjusted to datasources before usage. Tested with FOS v6.0.0



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
    <li> <span class="li-head">firewall_policy6</span> - Configure IPv6 policies. <span class="li-normal">type: dict</span></li>
        <ul class="ul-self">
        <li> <span class="li-head">state</span> - B(Deprecated) <span class="li-normal">type: str</span> <span class="li-required">required: False</span> <span class="li-normal">choices: present, absent</span></li>
        <li> <span class="li-head">action</span> - Policy action (allow/deny/ipsec). <span class="li-normal">type: str</span> <span class="li-normal">choices: accept, deny, ipsec</span></li>
        <li> <span class="li-head">app_category</span> - Application category ID list. <span class="li-normal">type: list</span></li>
            <ul class="ul-self">
            <li> <span class="li-head">id</span> - Category IDs. <span class="li-normal">type: int</span> <span class="li-required">required: True</span></li>
            </ul>
        <li> <span class="li-head">app_group</span> - Application group names. <span class="li-normal">type: list</span></li>
            <ul class="ul-self">
            <li> <span class="li-head">name</span> - Application group names. Source application.group.name. <span class="li-normal">type: str</span> <span class="li-required">required: True</span></li>
            </ul>
        <li> <span class="li-head">application</span> - Application ID list. <span class="li-normal">type: list</span></li>
            <ul class="ul-self">
            <li> <span class="li-head">id</span> - Application IDs. <span class="li-normal">type: int</span> <span class="li-required">required: True</span></li>
            </ul>
        <li> <span class="li-head">application_list</span> - Name of an existing Application list. Source application.list.name. <span class="li-normal">type: str</span></li>
        <li> <span class="li-head">av_profile</span> - Name of an existing Antivirus profile. Source antivirus.profile.name. <span class="li-normal">type: str</span></li>
        <li> <span class="li-head">comments</span> - Comment. <span class="li-normal">type: str</span></li>
        <li> <span class="li-head">custom_log_fields</span> - Log field index numbers to append custom log fields to log messages for this policy. <span class="li-normal">type: list</span></li>
            <ul class="ul-self">
            <li> <span class="li-head">field_id</span> - Custom log field. Source log.custom-field.id. <span class="li-normal">type: str</span></li>
            </ul>
        <li> <span class="li-head">devices</span> - Names of devices or device groups that can be matched by the policy. <span class="li-normal">type: list</span></li>
            <ul class="ul-self">
            <li> <span class="li-head">name</span> - Device or group name. Source user.device.alias user.device-group.name user.device-category.name. <span class="li-normal">type: str</span> <span class="li-required">required: True</span></li>
            </ul>
        <li> <span class="li-head">diffserv_forward</span> - Enable to change packet"s DiffServ values to the specified diffservcode-forward value. <span class="li-normal">type: str</span> <span class="li-normal">choices: enable, disable</span></li>
        <li> <span class="li-head">diffserv_reverse</span> - Enable to change packet"s reverse (reply) DiffServ values to the specified diffservcode-rev value. <span class="li-normal">type: str</span> <span class="li-normal">choices: enable, disable</span></li>
        <li> <span class="li-head">diffservcode_forward</span> - Change packet"s DiffServ to this value. <span class="li-normal">type: str</span></li>
        <li> <span class="li-head">diffservcode_rev</span> - Change packet"s reverse (reply) DiffServ to this value. <span class="li-normal">type: str</span></li>
        <li> <span class="li-head">dlp_sensor</span> - Name of an existing DLP sensor. Source dlp.sensor.name. <span class="li-normal">type: str</span></li>
        <li> <span class="li-head">dscp_match</span> - Enable DSCP check. <span class="li-normal">type: str</span> <span class="li-normal">choices: enable, disable</span></li>
        <li> <span class="li-head">dscp_negate</span> - Enable negated DSCP match. <span class="li-normal">type: str</span> <span class="li-normal">choices: enable, disable</span></li>
        <li> <span class="li-head">dscp_value</span> - DSCP value. <span class="li-normal">type: str</span></li>
        <li> <span class="li-head">dsri</span> - Enable DSRI to ignore HTTP server responses. <span class="li-normal">type: str</span> <span class="li-normal">choices: enable, disable</span></li>
        <li> <span class="li-head">dstaddr</span> - Destination address and address group names. <span class="li-normal">type: list</span></li>
            <ul class="ul-self">
            <li> <span class="li-head">name</span> - Address name. Source firewall.address6.name firewall.addrgrp6.name firewall.vip6.name firewall.vipgrp6.name. <span class="li-normal">type: str</span> <span class="li-required">required: True</span></li>
            </ul>
        <li> <span class="li-head">dstaddr_negate</span> - When enabled dstaddr specifies what the destination address must NOT be. <span class="li-normal">type: str</span> <span class="li-normal">choices: enable, disable</span></li>
        <li> <span class="li-head">dstintf</span> - Outgoing (egress) interface. <span class="li-normal">type: list</span></li>
            <ul class="ul-self">
            <li> <span class="li-head">name</span> - Interface name. Source system.interface.name system.zone.name. <span class="li-normal">type: str</span> <span class="li-required">required: True</span></li>
            </ul>
        <li> <span class="li-head">firewall_session_dirty</span> - How to handle sessions if the configuration of this firewall policy changes. <span class="li-normal">type: str</span> <span class="li-normal">choices: check-all, check-new</span></li>
        <li> <span class="li-head">fixedport</span> - Enable to prevent source NAT from changing a session"s source port. <span class="li-normal">type: str</span> <span class="li-normal">choices: enable, disable</span></li>
        <li> <span class="li-head">global_label</span> - Label for the policy that appears when the GUI is in Global View mode. <span class="li-normal">type: str</span></li>
        <li> <span class="li-head">groups</span> - Names of user groups that can authenticate with this policy. <span class="li-normal">type: list</span></li>
            <ul class="ul-self">
            <li> <span class="li-head">name</span> - Group name. Source user.group.name. <span class="li-normal">type: str</span> <span class="li-required">required: True</span></li>
            </ul>
        <li> <span class="li-head">icap_profile</span> - Name of an existing ICAP profile. Source icap.profile.name. <span class="li-normal">type: str</span></li>
        <li> <span class="li-head">inbound</span> - Policy-based IPsec VPN: only traffic from the remote network can initiate a VPN. <span class="li-normal">type: str</span> <span class="li-normal">choices: enable, disable</span></li>
        <li> <span class="li-head">ippool</span> - Enable to use IP Pools for source NAT. <span class="li-normal">type: str</span> <span class="li-normal">choices: enable, disable</span></li>
        <li> <span class="li-head">ips_sensor</span> - Name of an existing IPS sensor. Source ips.sensor.name. <span class="li-normal">type: str</span></li>
        <li> <span class="li-head">label</span> - Label for the policy that appears when the GUI is in Section View mode. <span class="li-normal">type: str</span></li>
        <li> <span class="li-head">logtraffic</span> - Enable or disable logging. Log all sessions or security profile sessions. <span class="li-normal">type: str</span> <span class="li-normal">choices: all, utm, disable</span></li>
        <li> <span class="li-head">logtraffic_start</span> - Record logs when a session starts and ends. <span class="li-normal">type: str</span> <span class="li-normal">choices: enable, disable</span></li>
        <li> <span class="li-head">name</span> - Policy name. <span class="li-normal">type: str</span></li>
        <li> <span class="li-head">nat</span> - Enable/disable source NAT. <span class="li-normal">type: str</span> <span class="li-normal">choices: enable, disable</span></li>
        <li> <span class="li-head">natinbound</span> - Policy-based IPsec VPN: apply destination NAT to inbound traffic. <span class="li-normal">type: str</span> <span class="li-normal">choices: enable, disable</span></li>
        <li> <span class="li-head">natoutbound</span> - Policy-based IPsec VPN: apply source NAT to outbound traffic. <span class="li-normal">type: str</span> <span class="li-normal">choices: enable, disable</span></li>
        <li> <span class="li-head">outbound</span> - Policy-based IPsec VPN: only traffic from the internal network can initiate a VPN. <span class="li-normal">type: str</span> <span class="li-normal">choices: enable, disable</span></li>
        <li> <span class="li-head">per_ip_shaper</span> - Per-IP traffic shaper. Source firewall.shaper.per-ip-shaper.name. <span class="li-normal">type: str</span></li>
        <li> <span class="li-head">policyid</span> - Policy ID. <span class="li-normal">type: int</span> <span class="li-required">required: True</span></li>
        <li> <span class="li-head">poolname</span> - IP Pool names. <span class="li-normal">type: list</span></li>
            <ul class="ul-self">
            <li> <span class="li-head">name</span> - IP pool name. Source firewall.ippool6.name. <span class="li-normal">type: str</span> <span class="li-required">required: True</span></li>
            </ul>
        <li> <span class="li-head">profile_group</span> - Name of profile group. Source firewall.profile-group.name. <span class="li-normal">type: str</span></li>
        <li> <span class="li-head">profile_protocol_options</span> - Name of an existing Protocol options profile. Source firewall.profile-protocol-options.name. <span class="li-normal">type: str</span></li>
        <li> <span class="li-head">profile_type</span> - Determine whether the firewall policy allows security profile groups or single profiles only. <span class="li-normal">type: str</span> <span class="li-normal">choices: single, group</span></li>
        <li> <span class="li-head">replacemsg_override_group</span> - Override the default replacement message group for this policy. Source system.replacemsg-group.name. <span class="li-normal">type: str</span></li>
        <li> <span class="li-head">rsso</span> - Enable/disable RADIUS single sign-on (RSSO). <span class="li-normal">type: str</span> <span class="li-normal">choices: enable, disable</span></li>
        <li> <span class="li-head">schedule</span> - Schedule name. Source firewall.schedule.onetime.name firewall.schedule.recurring.name firewall.schedule.group.name. <span class="li-normal">type: str</span></li>
        <li> <span class="li-head">send_deny_packet</span> - Enable/disable return of deny-packet. <span class="li-normal">type: str</span> <span class="li-normal">choices: enable, disable</span></li>
        <li> <span class="li-head">service</span> - Service and service group names. <span class="li-normal">type: list</span></li>
            <ul class="ul-self">
            <li> <span class="li-head">name</span> - Address name. Source firewall.service.custom.name firewall.service.group.name. <span class="li-normal">type: str</span> <span class="li-required">required: True</span></li>
            </ul>
        <li> <span class="li-head">service_negate</span> - When enabled service specifies what the service must NOT be. <span class="li-normal">type: str</span> <span class="li-normal">choices: enable, disable</span></li>
        <li> <span class="li-head">session_ttl</span> - Session TTL in seconds for sessions accepted by this policy. 0 means use the system default session TTL. <span class="li-normal">type: int</span></li>
        <li> <span class="li-head">spamfilter_profile</span> - Name of an existing Spam filter profile. Source spamfilter.profile.name. <span class="li-normal">type: str</span></li>
        <li> <span class="li-head">srcaddr</span> - Source address and address group names. <span class="li-normal">type: list</span></li>
            <ul class="ul-self">
            <li> <span class="li-head">name</span> - Address name. Source firewall.address6.name firewall.addrgrp6.name. <span class="li-normal">type: str</span> <span class="li-required">required: True</span></li>
            </ul>
        <li> <span class="li-head">srcaddr_negate</span> - When enabled srcaddr specifies what the source address must NOT be. <span class="li-normal">type: str</span> <span class="li-normal">choices: enable, disable</span></li>
        <li> <span class="li-head">srcintf</span> - Incoming (ingress) interface. <span class="li-normal">type: list</span></li>
            <ul class="ul-self">
            <li> <span class="li-head">name</span> - Interface name. Source system.zone.name system.interface.name. <span class="li-normal">type: str</span> <span class="li-required">required: True</span></li>
            </ul>
        <li> <span class="li-head">ssh_filter_profile</span> - Name of an existing SSH filter profile. Source ssh-filter.profile.name. <span class="li-normal">type: str</span></li>
        <li> <span class="li-head">ssl_mirror</span> - Enable to copy decrypted SSL traffic to a FortiGate interface (called SSL mirroring). <span class="li-normal">type: str</span> <span class="li-normal">choices: enable, disable</span></li>
        <li> <span class="li-head">ssl_mirror_intf</span> - SSL mirror interface name. <span class="li-normal">type: list</span></li>
            <ul class="ul-self">
            <li> <span class="li-head">name</span> - Interface name. Source system.zone.name system.interface.name. <span class="li-normal">type: str</span> <span class="li-required">required: True</span></li>
            </ul>
        <li> <span class="li-head">ssl_ssh_profile</span> - Name of an existing SSL SSH profile. Source firewall.ssl-ssh-profile.name. <span class="li-normal">type: str</span></li>
        <li> <span class="li-head">status</span> - Enable or disable this policy. <span class="li-normal">type: str</span> <span class="li-normal">choices: enable, disable</span></li>
        <li> <span class="li-head">tcp_mss_receiver</span> - Receiver TCP maximum segment size (MSS). <span class="li-normal">type: int</span></li>
        <li> <span class="li-head">tcp_mss_sender</span> - Sender TCP maximum segment size (MSS). <span class="li-normal">type: int</span></li>
        <li> <span class="li-head">tcp_session_without_syn</span> - Enable/disable creation of TCP session without SYN flag. <span class="li-normal">type: str</span> <span class="li-normal">choices: all, data-only, disable</span></li>
        <li> <span class="li-head">timeout_send_rst</span> - Enable/disable sending RST packets when TCP sessions expire. <span class="li-normal">type: str</span> <span class="li-normal">choices: enable, disable</span></li>
        <li> <span class="li-head">traffic_shaper</span> - Reverse traffic shaper. Source firewall.shaper.traffic-shaper.name. <span class="li-normal">type: str</span></li>
        <li> <span class="li-head">traffic_shaper_reverse</span> - Reverse traffic shaper. Source firewall.shaper.traffic-shaper.name. <span class="li-normal">type: str</span></li>
        <li> <span class="li-head">url_category</span> - URL category ID list. <span class="li-normal">type: list</span></li>
            <ul class="ul-self">
            <li> <span class="li-head">id</span> - URL category ID. <span class="li-normal">type: int</span> <span class="li-required">required: True</span></li>
            </ul>
        <li> <span class="li-head">users</span> - Names of individual users that can authenticate with this policy. <span class="li-normal">type: list</span></li>
            <ul class="ul-self">
            <li> <span class="li-head">name</span> - Names of individual users that can authenticate with this policy. Source user.local.name. <span class="li-normal">type: str</span> <span class="li-required">required: True</span></li>
            </ul>
        <li> <span class="li-head">utm_status</span> - Enable AV/web/ips protection profile. <span class="li-normal">type: str</span> <span class="li-normal">choices: enable, disable</span></li>
        <li> <span class="li-head">uuid</span> - Universally Unique Identifier (UUID; automatically assigned but can be manually reset). <span class="li-normal">type: str</span></li>
        <li> <span class="li-head">vlan_cos_fwd</span> - VLAN forward direction user priority: 255 passthrough, 0 lowest, 7 highest <span class="li-normal">type: int</span></li>
        <li> <span class="li-head">vlan_cos_rev</span> - VLAN reverse direction user priority: 255 passthrough, 0 lowest, 7 highest <span class="li-normal">type: int</span></li>
        <li> <span class="li-head">vlan_filter</span> - Set VLAN filters. <span class="li-normal">type: str</span></li>
        <li> <span class="li-head">voip_profile</span> - Name of an existing VoIP profile. Source voip.profile.name. <span class="li-normal">type: str</span></li>
        <li> <span class="li-head">vpntunnel</span> - Policy-based IPsec VPN: name of the IPsec VPN Phase 1. Source vpn.ipsec.phase1.name vpn.ipsec.manualkey.name. <span class="li-normal">type: str</span></li>
        <li> <span class="li-head">webfilter_profile</span> - Name of an existing Web filter profile. Source webfilter.profile.name. <span class="li-normal">type: str</span></li>
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
      - name: Configure IPv6 policies.
        fortios_firewall_policy6:
          vdom:  "{{ vdom }}"
          state: "present"
          firewall_policy6:
            action: "accept"
            app_category:
             -
                id:  "5"
            app_group:
             -
                name: "default_name_7 (source application.group.name)"
            application:
             -
                id:  "9"
            application_list: "<your_own_value> (source application.list.name)"
            av_profile: "<your_own_value> (source antivirus.profile.name)"
            comments: "<your_own_value>"
            custom_log_fields:
             -
                field_id: "<your_own_value> (source log.custom-field.id)"
            devices:
             -
                name: "default_name_16 (source user.device.alias user.device-group.name user.device-category.name)"
            diffserv_forward: "enable"
            diffserv_reverse: "enable"
            diffservcode_forward: "<your_own_value>"
            diffservcode_rev: "<your_own_value>"
            dlp_sensor: "<your_own_value> (source dlp.sensor.name)"
            dscp_match: "enable"
            dscp_negate: "enable"
            dscp_value: "<your_own_value>"
            dsri: "enable"
            dstaddr:
             -
                name: "default_name_27 (source firewall.address6.name firewall.addrgrp6.name firewall.vip6.name firewall.vipgrp6.name)"
            dstaddr_negate: "enable"
            dstintf:
             -
                name: "default_name_30 (source system.interface.name system.zone.name)"
            firewall_session_dirty: "check-all"
            fixedport: "enable"
            global_label: "<your_own_value>"
            groups:
             -
                name: "default_name_35 (source user.group.name)"
            icap_profile: "<your_own_value> (source icap.profile.name)"
            inbound: "enable"
            ippool: "enable"
            ips_sensor: "<your_own_value> (source ips.sensor.name)"
            label: "<your_own_value>"
            logtraffic: "all"
            logtraffic_start: "enable"
            name: "default_name_43"
            nat: "enable"
            natinbound: "enable"
            natoutbound: "enable"
            outbound: "enable"
            per_ip_shaper: "<your_own_value> (source firewall.shaper.per-ip-shaper.name)"
            policyid: "49"
            poolname:
             -
                name: "default_name_51 (source firewall.ippool6.name)"
            profile_group: "<your_own_value> (source firewall.profile-group.name)"
            profile_protocol_options: "<your_own_value> (source firewall.profile-protocol-options.name)"
            profile_type: "single"
            replacemsg_override_group: "<your_own_value> (source system.replacemsg-group.name)"
            rsso: "enable"
            schedule: "<your_own_value> (source firewall.schedule.onetime.name firewall.schedule.recurring.name firewall.schedule.group.name)"
            send_deny_packet: "enable"
            service:
             -
                name: "default_name_60 (source firewall.service.custom.name firewall.service.group.name)"
            service_negate: "enable"
            session_ttl: "62"
            spamfilter_profile: "<your_own_value> (source spamfilter.profile.name)"
            srcaddr:
             -
                name: "default_name_65 (source firewall.address6.name firewall.addrgrp6.name)"
            srcaddr_negate: "enable"
            srcintf:
             -
                name: "default_name_68 (source system.zone.name system.interface.name)"
            ssh_filter_profile: "<your_own_value> (source ssh-filter.profile.name)"
            ssl_mirror: "enable"
            ssl_mirror_intf:
             -
                name: "default_name_72 (source system.zone.name system.interface.name)"
            ssl_ssh_profile: "<your_own_value> (source firewall.ssl-ssh-profile.name)"
            status: "enable"
            tcp_mss_receiver: "75"
            tcp_mss_sender: "76"
            tcp_session_without_syn: "all"
            timeout_send_rst: "enable"
            traffic_shaper: "<your_own_value> (source firewall.shaper.traffic-shaper.name)"
            traffic_shaper_reverse: "<your_own_value> (source firewall.shaper.traffic-shaper.name)"
            url_category:
             -
                id:  "82"
            users:
             -
                name: "default_name_84 (source user.local.name)"
            utm_status: "enable"
            uuid: "<your_own_value>"
            vlan_cos_fwd: "87"
            vlan_cos_rev: "88"
            vlan_filter: "<your_own_value>"
            voip_profile: "<your_own_value> (source voip.profile.name)"
            vpntunnel: "<your_own_value> (source vpn.ipsec.phase1.name vpn.ipsec.manualkey.name)"
            webfilter_profile: "<your_own_value> (source webfilter.profile.name)"


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
