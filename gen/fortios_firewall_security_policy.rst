:source: fortios_firewall_security_policy.py

:orphan:

.. fortios_firewall_security_policy:

fortios_firewall_security_policy -- Configure NGFW IPv4/IPv6 application policies in Fortinet's FortiOS and FortiGate.
++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++

.. versionadded:: 2.10

.. contents::
   :local:
   :depth: 1


Synopsis
--------
- This module is able to configure a FortiGate or FortiOS (FOS) device by allowing the user to set and modify firewall feature and security_policy category. Examples include all parameters and values need to be adjusted to datasources before usage. Tested with FOS v6.4.0



Requirements
------------
The below requirements are needed on the host that executes this module.

- ansible>=2.9.0


Parameters
----------


.. raw:: html

    <ul>
    <li> <span class="li-head">access_token</span> - Token-based authentication. Generated from GUI of Fortigate. <span class="li-normal">type: str</span> <span class="li-required">required: False</span></li>
    <li> <span class="li-head">vdom</span> - Virtual domain, among those defined previously. A vdom is a virtual instance of the FortiGate that can be configured and used as a different unit. <span class="li-normal">type: str</span> <span class="li-normal">default: root</span></li>
    <li> <span class="li-head">state</span> - Indicates whether to create or remove the object. <span class="li-normal">type: str</span> <span class="li-required">required: True</span> <span class="li-normal">choices: present, absent</span></li>
    <li> <span class="li-head">firewall_security_policy</span> - Configure NGFW IPv4/IPv6 application policies. <span class="li-normal">type: dict</span></li>
        <ul class="ul-self">
        <li> <span class="li-head">action</span> - Policy action (accept/deny). <span class="li-normal">type: str</span> <span class="li-normal">choices: accept, deny</span></li>
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
        <li> <span class="li-head">cifs_profile</span> - Name of an existing CIFS profile. Source cifs.profile.name. <span class="li-normal">type: str</span></li>
        <li> <span class="li-head">comments</span> - Comment. <span class="li-normal">type: str</span></li>
        <li> <span class="li-head">dlp_sensor</span> - Name of an existing DLP sensor. Source dlp.sensor.name. <span class="li-normal">type: str</span></li>
        <li> <span class="li-head">dnsfilter_profile</span> - Name of an existing DNS filter profile. Source dnsfilter.profile.name. <span class="li-normal">type: str</span></li>
        <li> <span class="li-head">dstaddr</span> - Destination IPv4 address name and address group names. <span class="li-normal">type: list</span></li>
            <ul class="ul-self">
            <li> <span class="li-head">name</span> - Address name. Source firewall.address.name firewall.addrgrp.name firewall.vip.name firewall.vipgrp.name system.external-resource .name. <span class="li-normal">type: str</span> <span class="li-required">required: True</span></li>
            </ul>
        <li> <span class="li-head">dstaddr6</span> - Destination IPv6 address name and address group names. <span class="li-normal">type: list</span></li>
            <ul class="ul-self">
            <li> <span class="li-head">name</span> - Address name. Source firewall.address6.name firewall.addrgrp6.name firewall.vip6.name firewall.vipgrp6.name system .external-resource.name. <span class="li-normal">type: str</span> <span class="li-required">required: True</span></li>
            </ul>
        <li> <span class="li-head">dstintf</span> - Outgoing (egress) interface. <span class="li-normal">type: list</span></li>
            <ul class="ul-self">
            <li> <span class="li-head">name</span> - Interface name. Source system.interface.name system.zone.name. <span class="li-normal">type: str</span> <span class="li-required">required: True</span></li>
            </ul>
        <li> <span class="li-head">emailfilter_profile</span> - Name of an existing email filter profile. Source emailfilter.profile.name. <span class="li-normal">type: str</span></li>
        <li> <span class="li-head">enforce_default_app_port</span> - Enable/disable default application port enforcement for allowed applications. <span class="li-normal">type: str</span> <span class="li-normal">choices: enable, disable</span></li>
        <li> <span class="li-head">fsso_groups</span> - Names of FSSO groups. <span class="li-normal">type: list</span></li>
            <ul class="ul-self">
            <li> <span class="li-head">name</span> - Names of FSSO groups. Source user.adgrp.name. <span class="li-normal">type: str</span> <span class="li-required">required: True</span></li>
            </ul>
        <li> <span class="li-head">groups</span> - Names of user groups that can authenticate with this policy. <span class="li-normal">type: list</span></li>
            <ul class="ul-self">
            <li> <span class="li-head">name</span> - User group name. Source user.group.name. <span class="li-normal">type: str</span> <span class="li-required">required: True</span></li>
            </ul>
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
        <li> <span class="li-head">internet_service_negate</span> - When enabled internet-service specifies what the service must NOT be. <span class="li-normal">type: str</span> <span class="li-normal">choices: enable, disable</span></li>
        <li> <span class="li-head">internet_service_src</span> - Enable/disable use of Internet Services in source for this policy. If enabled, source address is not used. <span class="li-normal">type: str</span> <span class="li-normal">choices: enable, disable</span></li>
        <li> <span class="li-head">internet_service_src_custom</span> - Custom Internet Service source name. <span class="li-normal">type: list</span></li>
            <ul class="ul-self">
            <li> <span class="li-head">name</span> - Custom Internet Service name. Source firewall.internet-service-custom.name. <span class="li-normal">type: str</span> <span class="li-required">required: True</span></li>
            </ul>
        <li> <span class="li-head">internet_service_src_custom_group</span> - Custom Internet Service source group name. <span class="li-normal">type: list</span></li>
            <ul class="ul-self">
            <li> <span class="li-head">name</span> - Custom Internet Service group name. Source firewall.internet-service-custom-group.name. <span class="li-normal">type: str</span> <span class="li-required">required: True</span></li>
            </ul>
        <li> <span class="li-head">internet_service_src_group</span> - Internet Service source group name. <span class="li-normal">type: list</span></li>
            <ul class="ul-self">
            <li> <span class="li-head">name</span> - Internet Service group name. Source firewall.internet-service-group.name. <span class="li-normal">type: str</span> <span class="li-required">required: True</span></li>
            </ul>
        <li> <span class="li-head">internet_service_src_name</span> - Internet Service source name. <span class="li-normal">type: list</span></li>
            <ul class="ul-self">
            <li> <span class="li-head">name</span> - Internet Service name. Source firewall.internet-service-name.name. <span class="li-normal">type: str</span> <span class="li-required">required: True</span></li>
            </ul>
        <li> <span class="li-head">internet_service_src_negate</span> - When enabled internet-service-src specifies what the service must NOT be. <span class="li-normal">type: str</span> <span class="li-normal">choices: enable, disable</span></li>
        <li> <span class="li-head">ips_sensor</span> - Name of an existing IPS sensor. Source ips.sensor.name. <span class="li-normal">type: str</span></li>
        <li> <span class="li-head">logtraffic</span> - Enable or disable logging. Log all sessions or security profile sessions. <span class="li-normal">type: str</span> <span class="li-normal">choices: all, utm, disable</span></li>
        <li> <span class="li-head">name</span> - Policy name. <span class="li-normal">type: str</span></li>
        <li> <span class="li-head">policyid</span> - Policy ID. <span class="li-normal">type: int</span> <span class="li-required">required: True</span></li>
        <li> <span class="li-head">profile_group</span> - Name of profile group. Source firewall.profile-group.name. <span class="li-normal">type: str</span></li>
        <li> <span class="li-head">profile_protocol_options</span> - Name of an existing Protocol options profile. Source firewall.profile-protocol-options.name. <span class="li-normal">type: str</span></li>
        <li> <span class="li-head">profile_type</span> - Determine whether the firewall policy allows security profile groups or single profiles only. <span class="li-normal">type: str</span> <span class="li-normal">choices: single, group</span></li>
        <li> <span class="li-head">schedule</span> - Schedule name. Source firewall.schedule.onetime.name firewall.schedule.recurring.name firewall.schedule.group.name. <span class="li-normal">type: str</span></li>
        <li> <span class="li-head">send_deny_packet</span> - Enable to send a reply when a session is denied or blocked by a firewall policy. <span class="li-normal">type: str</span> <span class="li-normal">choices: disable, enable</span></li>
        <li> <span class="li-head">service</span> - Service and service group names. <span class="li-normal">type: list</span></li>
            <ul class="ul-self">
            <li> <span class="li-head">name</span> - Service name. Source firewall.service.custom.name firewall.service.group.name. <span class="li-normal">type: str</span> <span class="li-required">required: True</span></li>
            </ul>
        <li> <span class="li-head">service_negate</span> - When enabled service specifies what the service must NOT be. <span class="li-normal">type: str</span> <span class="li-normal">choices: enable, disable</span></li>
        <li> <span class="li-head">srcaddr</span> - Source IPv4 address name and address group names. <span class="li-normal">type: list</span></li>
            <ul class="ul-self">
            <li> <span class="li-head">name</span> - Address name. Source firewall.address.name firewall.addrgrp.name system.external-resource.name. <span class="li-normal">type: str</span> <span class="li-required">required: True</span></li>
            </ul>
        <li> <span class="li-head">srcaddr6</span> - Source IPv6 address name and address group names. <span class="li-normal">type: list</span></li>
            <ul class="ul-self">
            <li> <span class="li-head">name</span> - Address name. Source firewall.address6.name firewall.addrgrp6.name system.external-resource.name. <span class="li-normal">type: str</span> <span class="li-required">required: True</span></li>
            </ul>
        <li> <span class="li-head">srcintf</span> - Incoming (ingress) interface. <span class="li-normal">type: list</span></li>
            <ul class="ul-self">
            <li> <span class="li-head">name</span> - Interface name. Source system.interface.name system.zone.name. <span class="li-normal">type: str</span> <span class="li-required">required: True</span></li>
            </ul>
        <li> <span class="li-head">ssh_filter_profile</span> - Name of an existing SSH filter profile. Source ssh-filter.profile.name. <span class="li-normal">type: str</span></li>
        <li> <span class="li-head">ssl_ssh_profile</span> - Name of an existing SSL SSH profile. Source firewall.ssl-ssh-profile.name. <span class="li-normal">type: str</span></li>
        <li> <span class="li-head">status</span> - Enable or disable this policy. <span class="li-normal">type: str</span> <span class="li-normal">choices: enable, disable</span></li>
        <li> <span class="li-head">url_category</span> - URL category ID list. <span class="li-normal">type: list</span></li>
            <ul class="ul-self">
            <li> <span class="li-head">id</span> - URL category ID. <span class="li-normal">type: int</span> <span class="li-required">required: True</span></li>
            </ul>
        <li> <span class="li-head">users</span> - Names of individual users that can authenticate with this policy. <span class="li-normal">type: list</span></li>
            <ul class="ul-self">
            <li> <span class="li-head">name</span> - User name. Source user.local.name. <span class="li-normal">type: str</span> <span class="li-required">required: True</span></li>
            </ul>
        <li> <span class="li-head">uuid</span> - Universally Unique Identifier (UUID; automatically assigned but can be manually reset). <span class="li-normal">type: str</span></li>
        <li> <span class="li-head">voip_profile</span> - Name of an existing VoIP profile. Source voip.profile.name. <span class="li-normal">type: str</span></li>
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
      - name: Configure NGFW IPv4/IPv6 application policies.
        fortios_firewall_security_policy:
          vdom:  "{{ vdom }}"
          state: "present"
          access_token: "<your_own_value>"
          firewall_security_policy:
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
            cifs_profile: "<your_own_value> (source cifs.profile.name)"
            comments: "<your_own_value>"
            dlp_sensor: "<your_own_value> (source dlp.sensor.name)"
            dnsfilter_profile: "<your_own_value> (source dnsfilter.profile.name)"
            dstaddr:
             -
                name: "default_name_17 (source firewall.address.name firewall.addrgrp.name firewall.vip.name firewall.vipgrp.name system.external-resource.name)"
            dstaddr6:
             -
                name: "default_name_19 (source firewall.address6.name firewall.addrgrp6.name firewall.vip6.name firewall.vipgrp6.name system.external-resource
                  .name)"
            dstintf:
             -
                name: "default_name_21 (source system.interface.name system.zone.name)"
            emailfilter_profile: "<your_own_value> (source emailfilter.profile.name)"
            enforce_default_app_port: "enable"
            fsso_groups:
             -
                name: "default_name_25 (source user.adgrp.name)"
            groups:
             -
                name: "default_name_27 (source user.group.name)"
            icap_profile: "<your_own_value> (source icap.profile.name)"
            internet_service: "enable"
            internet_service_custom:
             -
                name: "default_name_31 (source firewall.internet-service-custom.name)"
            internet_service_custom_group:
             -
                name: "default_name_33 (source firewall.internet-service-custom-group.name)"
            internet_service_group:
             -
                name: "default_name_35 (source firewall.internet-service-group.name)"
            internet_service_name:
             -
                name: "default_name_37 (source firewall.internet-service-name.name)"
            internet_service_negate: "enable"
            internet_service_src: "enable"
            internet_service_src_custom:
             -
                name: "default_name_41 (source firewall.internet-service-custom.name)"
            internet_service_src_custom_group:
             -
                name: "default_name_43 (source firewall.internet-service-custom-group.name)"
            internet_service_src_group:
             -
                name: "default_name_45 (source firewall.internet-service-group.name)"
            internet_service_src_name:
             -
                name: "default_name_47 (source firewall.internet-service-name.name)"
            internet_service_src_negate: "enable"
            ips_sensor: "<your_own_value> (source ips.sensor.name)"
            logtraffic: "all"
            name: "default_name_51"
            policyid: "52"
            profile_group: "<your_own_value> (source firewall.profile-group.name)"
            profile_protocol_options: "<your_own_value> (source firewall.profile-protocol-options.name)"
            profile_type: "single"
            schedule: "<your_own_value> (source firewall.schedule.onetime.name firewall.schedule.recurring.name firewall.schedule.group.name)"
            send_deny_packet: "disable"
            service:
             -
                name: "default_name_59 (source firewall.service.custom.name firewall.service.group.name)"
            service_negate: "enable"
            srcaddr:
             -
                name: "default_name_62 (source firewall.address.name firewall.addrgrp.name system.external-resource.name)"
            srcaddr6:
             -
                name: "default_name_64 (source firewall.address6.name firewall.addrgrp6.name system.external-resource.name)"
            srcintf:
             -
                name: "default_name_66 (source system.interface.name system.zone.name)"
            ssh_filter_profile: "<your_own_value> (source ssh-filter.profile.name)"
            ssl_ssh_profile: "<your_own_value> (source firewall.ssl-ssh-profile.name)"
            status: "enable"
            url_category:
             -
                id:  "71"
            users:
             -
                name: "default_name_73 (source user.local.name)"
            uuid: "<your_own_value>"
            voip_profile: "<your_own_value> (source voip.profile.name)"
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
- Jie Xue (@JieX19)
- Hongbin Lu (@fgtdev-hblu)
- Frank Shen (@frankshen01)
- Miguel Angel Munoz (@mamunozgonzalez)
- Nicolas Thomas (@thomnico)


.. hint::
    If you notice any issues in this documentation, you can create a pull request to improve it.
