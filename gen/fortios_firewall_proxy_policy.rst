:source: fortios_firewall_proxy_policy.py

:orphan:

.. fortios_firewall_proxy_policy:

fortios_firewall_proxy_policy -- Configure proxy policies in Fortinet's FortiOS and FortiGate.
++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++

.. versionadded:: 2.8

.. contents::
   :local:
   :depth: 1


Synopsis
--------
- This module is able to configure a FortiGate or FortiOS (FOS) device by allowing the user to set and modify firewall feature and proxy_policy category. Examples include all parameters and values need to be adjusted to datasources before usage. Tested with FOS v6.4.0



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
    <li> <span class="li-head">firewall_proxy_policy</span> - Configure proxy policies. <span class="li-normal">type: dict</span></li>
        <ul class="ul-self">
        <li> <span class="li-head">state</span> - B(Deprecated) <span class="li-normal">type: str</span> <span class="li-required">required: False</span> <span class="li-normal">choices: present, absent</span></li>
        <li> <span class="li-head">action</span> - Accept or deny traffic matching the policy parameters. <span class="li-normal">type: str</span> <span class="li-normal">choices: accept, deny, redirect</span></li>
        <li> <span class="li-head">application_list</span> - Name of an existing Application list. Source application.list.name. <span class="li-normal">type: str</span></li>
        <li> <span class="li-head">av_profile</span> - Name of an existing Antivirus profile. Source antivirus.profile.name. <span class="li-normal">type: str</span></li>
        <li> <span class="li-head">cifs_profile</span> - Name of an existing CIFS profile. Source cifs.profile.name. <span class="li-normal">type: str</span></li>
        <li> <span class="li-head">comments</span> - Optional comments. <span class="li-normal">type: str</span></li>
        <li> <span class="li-head">decrypted_traffic_mirror</span> - Decrypted traffic mirror. Source firewall.decrypted-traffic-mirror.name. <span class="li-normal">type: str</span></li>
        <li> <span class="li-head">disclaimer</span> - Web proxy disclaimer setting: by domain, policy, or user. <span class="li-normal">type: str</span> <span class="li-normal">choices: disable, domain, policy, user</span></li>
        <li> <span class="li-head">dlp_sensor</span> - Name of an existing DLP sensor. Source dlp.sensor.name. <span class="li-normal">type: str</span></li>
        <li> <span class="li-head">dstaddr</span> - Destination address objects. <span class="li-normal">type: list</span></li>
            <ul class="ul-self">
            <li> <span class="li-head">name</span> - Address name. Source firewall.address.name firewall.addrgrp.name firewall.proxy-address.name firewall.proxy-addrgrp.name firewall.vip.name firewall.vipgrp.name firewall.vip46.name firewall.vipgrp46.name system.external-resource.name. <span class="li-normal">type: str</span> <span class="li-required">required: True</span></li>
            </ul>
        <li> <span class="li-head">dstaddr_negate</span> - When enabled, destination addresses match against any address EXCEPT the specified destination addresses. <span class="li-normal">type: str</span> <span class="li-normal">choices: enable, disable</span></li>
        <li> <span class="li-head">dstaddr6</span> - IPv6 destination address objects. <span class="li-normal">type: list</span></li>
            <ul class="ul-self">
            <li> <span class="li-head">name</span> - Address name. Source firewall.address6.name firewall.addrgrp6.name firewall.vip6.name firewall.vipgrp6.name firewall.vip64.name firewall.vipgrp64.name system.external-resource.name. <span class="li-normal">type: str</span> <span class="li-required">required: True</span></li>
            </ul>
        <li> <span class="li-head">dstintf</span> - Destination interface names. <span class="li-normal">type: list</span></li>
            <ul class="ul-self">
            <li> <span class="li-head">name</span> - Interface name. Source system.interface.name system.zone.name. <span class="li-normal">type: str</span> <span class="li-required">required: True</span></li>
            </ul>
        <li> <span class="li-head">emailfilter_profile</span> - Name of an existing email filter profile. Source emailfilter.profile.name. <span class="li-normal">type: str</span></li>
        <li> <span class="li-head">groups</span> - Names of group objects. <span class="li-normal">type: list</span></li>
            <ul class="ul-self">
            <li> <span class="li-head">name</span> - Group name. Source user.group.name. <span class="li-normal">type: str</span> <span class="li-required">required: True</span></li>
            </ul>
        <li> <span class="li-head">http_tunnel_auth</span> - Enable/disable HTTP tunnel authentication. <span class="li-normal">type: str</span> <span class="li-normal">choices: enable, disable</span></li>
        <li> <span class="li-head">icap_profile</span> - Name of an existing ICAP profile. Source icap.profile.name. <span class="li-normal">type: str</span></li>
        <li> <span class="li-head">internet_service</span> - Enable/disable use of Internet Services for this policy. If enabled, destination address and service are not used. <span class="li-normal">type: str</span> <span class="li-normal">choices: enable, disable</span></li>
        <li> <span class="li-head">internet_service_custom</span> - Custom Internet Service name. <span class="li-normal">type: list</span></li>
            <ul class="ul-self">
            <li> <span class="li-head">name</span> - Custom Internet Service name. Source firewall.internet-service-custom.name. <span class="li-normal">type: str</span> <span class="li-required">required: True</span></li>
            </ul>
        <li> <span class="li-head">internet_service_custom_group</span> - Custom Internet Service group name. <span class="li-normal">type: list</span></li>
            <ul class="ul-self">
            <li> <span class="li-head">name</span> - Custom Internet Service group name. Source firewall.internet-service-custom-group.name. <span class="li-normal">type: str</span> <span class="li-required">required: True</span></li>
            </ul>
        <li> <span class="li-head">internet_service_group</span> - Internet Service group name. <span class="li-normal">type: list</span></li>
            <ul class="ul-self">
            <li> <span class="li-head">name</span> - Internet Service group name. Source firewall.internet-service-group.name. <span class="li-normal">type: str</span> <span class="li-required">required: True</span></li>
            </ul>
        <li> <span class="li-head">internet_service_name</span> - Internet Service name. <span class="li-normal">type: list</span></li>
            <ul class="ul-self">
            <li> <span class="li-head">name</span> - Internet Service name. Source firewall.internet-service-name.name. <span class="li-normal">type: str</span> <span class="li-required">required: True</span></li>
            </ul>
        <li> <span class="li-head">internet_service_negate</span> - When enabled, Internet Services match against any internet service EXCEPT the selected Internet Service. <span class="li-normal">type: str</span> <span class="li-normal">choices: enable, disable</span></li>
        <li> <span class="li-head">ips_sensor</span> - Name of an existing IPS sensor. Source ips.sensor.name. <span class="li-normal">type: str</span></li>
        <li> <span class="li-head">logtraffic</span> - Enable/disable logging traffic through the policy. <span class="li-normal">type: str</span> <span class="li-normal">choices: all, utm, disable</span></li>
        <li> <span class="li-head">logtraffic_start</span> - Enable/disable policy log traffic start. <span class="li-normal">type: str</span> <span class="li-normal">choices: enable, disable</span></li>
        <li> <span class="li-head">policyid</span> - Policy ID. <span class="li-normal">type: int</span> <span class="li-required">required: True</span></li>
        <li> <span class="li-head">poolname</span> - Name of IP pool object. <span class="li-normal">type: list</span></li>
            <ul class="ul-self">
            <li> <span class="li-head">name</span> - IP pool name. Source firewall.ippool.name. <span class="li-normal">type: str</span> <span class="li-required">required: True</span></li>
            </ul>
        <li> <span class="li-head">profile_group</span> - Name of profile group. Source firewall.profile-group.name. <span class="li-normal">type: str</span></li>
        <li> <span class="li-head">profile_protocol_options</span> - Name of an existing Protocol options profile. Source firewall.profile-protocol-options.name. <span class="li-normal">type: str</span></li>
        <li> <span class="li-head">profile_type</span> - Determine whether the firewall policy allows security profile groups or single profiles only. <span class="li-normal">type: str</span> <span class="li-normal">choices: single, group</span></li>
        <li> <span class="li-head">proxy</span> - Type of explicit proxy. <span class="li-normal">type: str</span> <span class="li-normal">choices: explicit-web, transparent-web, ftp, ssh, ssh-tunnel, wanopt</span></li>
        <li> <span class="li-head">redirect_url</span> - Redirect URL for further explicit web proxy processing. <span class="li-normal">type: str</span></li>
        <li> <span class="li-head">replacemsg_override_group</span> - Authentication replacement message override group. Source system.replacemsg-group.name. <span class="li-normal">type: str</span></li>
        <li> <span class="li-head">schedule</span> - Name of schedule object. Source firewall.schedule.onetime.name firewall.schedule.recurring.name firewall.schedule.group.name. <span class="li-normal">type: str</span></li>
        <li> <span class="li-head">service</span> - Name of service objects. <span class="li-normal">type: list</span></li>
            <ul class="ul-self">
            <li> <span class="li-head">name</span> - Service name. Source firewall.service.custom.name firewall.service.group.name. <span class="li-normal">type: str</span> <span class="li-required">required: True</span></li>
            </ul>
        <li> <span class="li-head">service_negate</span> - When enabled, services match against any service EXCEPT the specified destination services. <span class="li-normal">type: str</span> <span class="li-normal">choices: enable, disable</span></li>
        <li> <span class="li-head">session_ttl</span> - TTL in seconds for sessions accepted by this policy (0 means use the system ). <span class="li-normal">type: int</span></li>
        <li> <span class="li-head">srcaddr</span> - Source address objects. <span class="li-normal">type: list</span></li>
            <ul class="ul-self">
            <li> <span class="li-head">name</span> - Address name. Source firewall.address.name firewall.addrgrp.name firewall.proxy-address.name firewall.proxy-addrgrp.name system .external-resource.name. <span class="li-normal">type: str</span> <span class="li-required">required: True</span></li>
            </ul>
        <li> <span class="li-head">srcaddr_negate</span> - When enabled, source addresses match against any address EXCEPT the specified source addresses. <span class="li-normal">type: str</span> <span class="li-normal">choices: enable, disable</span></li>
        <li> <span class="li-head">srcaddr6</span> - IPv6 source address objects. <span class="li-normal">type: list</span></li>
            <ul class="ul-self">
            <li> <span class="li-head">name</span> - Address name. Source firewall.address6.name firewall.addrgrp6.name system.external-resource.name. <span class="li-normal">type: str</span> <span class="li-required">required: True</span></li>
            </ul>
        <li> <span class="li-head">srcintf</span> - Source interface names. <span class="li-normal">type: list</span></li>
            <ul class="ul-self">
            <li> <span class="li-head">name</span> - Interface name. Source system.interface.name system.zone.name. <span class="li-normal">type: str</span> <span class="li-required">required: True</span></li>
            </ul>
        <li> <span class="li-head">ssh_filter_profile</span> - Name of an existing SSH filter profile. Source ssh-filter.profile.name. <span class="li-normal">type: str</span></li>
        <li> <span class="li-head">ssh_policy_redirect</span> - Redirect SSH traffic to matching transparent proxy policy. <span class="li-normal">type: str</span> <span class="li-normal">choices: enable, disable</span></li>
        <li> <span class="li-head">ssl_ssh_profile</span> - Name of an existing SSL SSH profile. Source firewall.ssl-ssh-profile.name. <span class="li-normal">type: str</span></li>
        <li> <span class="li-head">status</span> - Enable/disable the active status of the policy. <span class="li-normal">type: str</span> <span class="li-normal">choices: enable, disable</span></li>
        <li> <span class="li-head">transparent</span> - Enable to use the IP address of the client to connect to the server. <span class="li-normal">type: str</span> <span class="li-normal">choices: enable, disable</span></li>
        <li> <span class="li-head">users</span> - Names of user objects. <span class="li-normal">type: list</span></li>
            <ul class="ul-self">
            <li> <span class="li-head">name</span> - Group name. Source user.local.name. <span class="li-normal">type: str</span> <span class="li-required">required: True</span></li>
            </ul>
        <li> <span class="li-head">utm_status</span> - Enable the use of UTM profiles/sensors/lists. <span class="li-normal">type: str</span> <span class="li-normal">choices: enable, disable</span></li>
        <li> <span class="li-head">uuid</span> - Universally Unique Identifier (UUID; automatically assigned but can be manually reset). <span class="li-normal">type: str</span></li>
        <li> <span class="li-head">waf_profile</span> - Name of an existing Web application firewall profile. Source waf.profile.name. <span class="li-normal">type: str</span></li>
        <li> <span class="li-head">webcache</span> - Enable/disable web caching. <span class="li-normal">type: str</span> <span class="li-normal">choices: enable, disable</span></li>
        <li> <span class="li-head">webcache_https</span> - Enable/disable web caching for HTTPS (Requires deep-inspection enabled in ssl-ssh-profile). <span class="li-normal">type: str</span> <span class="li-normal">choices: disable, enable</span></li>
        <li> <span class="li-head">webfilter_profile</span> - Name of an existing Web filter profile. Source webfilter.profile.name. <span class="li-normal">type: str</span></li>
        <li> <span class="li-head">webproxy_forward_server</span> - Web proxy forward server name. Source web-proxy.forward-server.name web-proxy.forward-server-group.name. <span class="li-normal">type: str</span></li>
        <li> <span class="li-head">webproxy_profile</span> - Name of web proxy profile. Source web-proxy.profile.name. <span class="li-normal">type: str</span></li>
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
      - name: Configure proxy policies.
        fortios_firewall_proxy_policy:
          vdom:  "{{ vdom }}"
          state: "present"
          firewall_proxy_policy:
            action: "accept"
            application_list: "<your_own_value> (source application.list.name)"
            av_profile: "<your_own_value> (source antivirus.profile.name)"
            cifs_profile: "<your_own_value> (source cifs.profile.name)"
            comments: "<your_own_value>"
            decrypted_traffic_mirror: "<your_own_value> (source firewall.decrypted-traffic-mirror.name)"
            disclaimer: "disable"
            dlp_sensor: "<your_own_value> (source dlp.sensor.name)"
            dstaddr:
             -
                name: "default_name_12 (source firewall.address.name firewall.addrgrp.name firewall.proxy-address.name firewall.proxy-addrgrp.name firewall.vip
                  .name firewall.vipgrp.name firewall.vip46.name firewall.vipgrp46.name system.external-resource.name)"
            dstaddr_negate: "enable"
            dstaddr6:
             -
                name: "default_name_15 (source firewall.address6.name firewall.addrgrp6.name firewall.vip6.name firewall.vipgrp6.name firewall.vip64.name firewall
                  .vipgrp64.name system.external-resource.name)"
            dstintf:
             -
                name: "default_name_17 (source system.interface.name system.zone.name)"
            emailfilter_profile: "<your_own_value> (source emailfilter.profile.name)"
            groups:
             -
                name: "default_name_20 (source user.group.name)"
            http_tunnel_auth: "enable"
            icap_profile: "<your_own_value> (source icap.profile.name)"
            internet_service: "enable"
            internet_service_custom:
             -
                name: "default_name_25 (source firewall.internet-service-custom.name)"
            internet_service_custom_group:
             -
                name: "default_name_27 (source firewall.internet-service-custom-group.name)"
            internet_service_group:
             -
                name: "default_name_29 (source firewall.internet-service-group.name)"
            internet_service_name:
             -
                name: "default_name_31 (source firewall.internet-service-name.name)"
            internet_service_negate: "enable"
            ips_sensor: "<your_own_value> (source ips.sensor.name)"
            logtraffic: "all"
            logtraffic_start: "enable"
            policyid: "36"
            poolname:
             -
                name: "default_name_38 (source firewall.ippool.name)"
            profile_group: "<your_own_value> (source firewall.profile-group.name)"
            profile_protocol_options: "<your_own_value> (source firewall.profile-protocol-options.name)"
            profile_type: "single"
            proxy: "explicit-web"
            redirect_url: "<your_own_value>"
            replacemsg_override_group: "<your_own_value> (source system.replacemsg-group.name)"
            schedule: "<your_own_value> (source firewall.schedule.onetime.name firewall.schedule.recurring.name firewall.schedule.group.name)"
            service:
             -
                name: "default_name_47 (source firewall.service.custom.name firewall.service.group.name)"
            service_negate: "enable"
            session_ttl: "49"
            srcaddr:
             -
                name: "default_name_51 (source firewall.address.name firewall.addrgrp.name firewall.proxy-address.name firewall.proxy-addrgrp.name system
                  .external-resource.name)"
            srcaddr_negate: "enable"
            srcaddr6:
             -
                name: "default_name_54 (source firewall.address6.name firewall.addrgrp6.name system.external-resource.name)"
            srcintf:
             -
                name: "default_name_56 (source system.interface.name system.zone.name)"
            ssh_filter_profile: "<your_own_value> (source ssh-filter.profile.name)"
            ssh_policy_redirect: "enable"
            ssl_ssh_profile: "<your_own_value> (source firewall.ssl-ssh-profile.name)"
            status: "enable"
            transparent: "enable"
            users:
             -
                name: "default_name_63 (source user.local.name)"
            utm_status: "enable"
            uuid: "<your_own_value>"
            waf_profile: "<your_own_value> (source waf.profile.name)"
            webcache: "enable"
            webcache_https: "disable"
            webfilter_profile: "<your_own_value> (source webfilter.profile.name)"
            webproxy_forward_server: "<your_own_value> (source web-proxy.forward-server.name web-proxy.forward-server-group.name)"
            webproxy_profile: "<your_own_value> (source web-proxy.profile.name)"


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
