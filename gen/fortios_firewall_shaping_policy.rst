:source: fortios_firewall_shaping_policy.py

:orphan:

.. fortios_firewall_shaping_policy:

fortios_firewall_shaping_policy -- Configure shaping policies in Fortinet's FortiOS and FortiGate.
++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++

.. versionadded:: 2.8

.. contents::
   :local:
   :depth: 1


Synopsis
--------
- This module is able to configure a FortiGate or FortiOS (FOS) device by allowing the user to set and modify firewall feature and shaping_policy category. Examples include all parameters and values need to be adjusted to datasources before usage. Tested with FOS v6.2.0



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
    <li> <span class="li-head">state</span> - Indicates whether to create or remove the object. This attribute was present already in previous version in a deeper level. It has been moved out to this outer level. <span class="li-normal">type: str</span> <span class="li-required">required: False</span> <span class="li-normal">choices: present, absent</span></li>
    <li> <span class="li-head">firewall_shaping_policy</span> - Configure shaping policies. <span class="li-normal">type: dict</span></li>
        <ul class="ul-self">
        <li> <span class="li-head">state</span> - B(Deprecated) <span class="li-normal">type: str</span> <span class="li-required">required: False</span> <span class="li-normal">choices: present, absent</span></li>
        <li> <span class="li-head">app_category</span> - IDs of one or more application categories that this shaper applies application control traffic shaping to. <span class="li-normal">type: list</span></li>
            <ul class="ul-self">
            <li> <span class="li-head">id</span> - Category IDs. <span class="li-normal">type: int</span> <span class="li-required">required: True</span></li>
            </ul>
        <li> <span class="li-head">app_group</span> - One or more application group names. <span class="li-normal">type: list</span></li>
            <ul class="ul-self">
            <li> <span class="li-head">name</span> - Application group name. Source application.group.name. <span class="li-normal">type: str</span> <span class="li-required">required: True</span></li>
            </ul>
        <li> <span class="li-head">application</span> - IDs of one or more applications that this shaper applies application control traffic shaping to. <span class="li-normal">type: list</span></li>
            <ul class="ul-self">
            <li> <span class="li-head">id</span> - Application IDs. <span class="li-normal">type: int</span> <span class="li-required">required: True</span></li>
            </ul>
        <li> <span class="li-head">class_id</span> - Traffic class ID. <span class="li-normal">type: int</span></li>
        <li> <span class="li-head">comment</span> - Comments. <span class="li-normal">type: str</span></li>
        <li> <span class="li-head">diffserv_forward</span> - Enable to change packet"s DiffServ values to the specified diffservcode-forward value. <span class="li-normal">type: str</span> <span class="li-normal">choices: enable, disable</span></li>
        <li> <span class="li-head">diffserv_reverse</span> - Enable to change packet"s reverse (reply) DiffServ values to the specified diffservcode-rev value. <span class="li-normal">type: str</span> <span class="li-normal">choices: enable, disable</span></li>
        <li> <span class="li-head">diffservcode_forward</span> - Change packet"s DiffServ to this value. <span class="li-normal">type: str</span></li>
        <li> <span class="li-head">diffservcode_rev</span> - Change packet"s reverse (reply) DiffServ to this value. <span class="li-normal">type: str</span></li>
        <li> <span class="li-head">dstaddr</span> - IPv4 destination address and address group names. <span class="li-normal">type: list</span></li>
            <ul class="ul-self">
            <li> <span class="li-head">name</span> - Address name. Source firewall.address.name firewall.addrgrp.name. <span class="li-normal">type: str</span> <span class="li-required">required: True</span></li>
            </ul>
        <li> <span class="li-head">dstaddr6</span> - IPv6 destination address and address group names. <span class="li-normal">type: list</span></li>
            <ul class="ul-self">
            <li> <span class="li-head">name</span> - Address name. Source firewall.address6.name firewall.addrgrp6.name. <span class="li-normal">type: str</span> <span class="li-required">required: True</span></li>
            </ul>
        <li> <span class="li-head">dstintf</span> - One or more outgoing (egress) interfaces. <span class="li-normal">type: list</span></li>
            <ul class="ul-self">
            <li> <span class="li-head">name</span> - Interface name. Source system.interface.name system.zone.name. <span class="li-normal">type: str</span> <span class="li-required">required: True</span></li>
            </ul>
        <li> <span class="li-head">groups</span> - Apply this traffic shaping policy to user groups that have authenticated with the FortiGate. <span class="li-normal">type: list</span></li>
            <ul class="ul-self">
            <li> <span class="li-head">name</span> - Group name. Source user.group.name. <span class="li-normal">type: str</span> <span class="li-required">required: True</span></li>
            </ul>
        <li> <span class="li-head">id</span> - Shaping policy ID (0 - 4294967295). <span class="li-normal">type: int</span> <span class="li-required">required: True</span></li>
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
        <li> <span class="li-head">internet_service_id</span> - Internet Service ID. <span class="li-normal">type: list</span></li>
            <ul class="ul-self">
            <li> <span class="li-head">id</span> - Internet Service ID. Source firewall.internet-service.id. <span class="li-normal">type: int</span> <span class="li-required">required: True</span></li>
            </ul>
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
        <li> <span class="li-head">internet_service_src_id</span> - Internet Service source ID. <span class="li-normal">type: list</span></li>
            <ul class="ul-self">
            <li> <span class="li-head">id</span> - Internet Service ID. Source firewall.internet-service.id. <span class="li-normal">type: int</span> <span class="li-required">required: True</span></li>
            </ul>
        <li> <span class="li-head">ip_version</span> - Apply this traffic shaping policy to IPv4 or IPv6 traffic. <span class="li-normal">type: str</span> <span class="li-normal">choices: 4, 6</span></li>
        <li> <span class="li-head">name</span> - Shaping policy name. <span class="li-normal">type: str</span></li>
        <li> <span class="li-head">per_ip_shaper</span> - Per-IP traffic shaper to apply with this policy. Source firewall.shaper.per-ip-shaper.name. <span class="li-normal">type: str</span></li>
        <li> <span class="li-head">schedule</span> - Schedule name. Source firewall.schedule.onetime.name firewall.schedule.recurring.name firewall.schedule.group.name. <span class="li-normal">type: str</span></li>
        <li> <span class="li-head">service</span> - Service and service group names. <span class="li-normal">type: list</span></li>
            <ul class="ul-self">
            <li> <span class="li-head">name</span> - Service name. Source firewall.service.custom.name firewall.service.group.name. <span class="li-normal">type: str</span> <span class="li-required">required: True</span></li>
            </ul>
        <li> <span class="li-head">srcaddr</span> - IPv4 source address and address group names. <span class="li-normal">type: list</span></li>
            <ul class="ul-self">
            <li> <span class="li-head">name</span> - Address name. Source firewall.address.name firewall.addrgrp.name. <span class="li-normal">type: str</span> <span class="li-required">required: True</span></li>
            </ul>
        <li> <span class="li-head">srcaddr6</span> - IPv6 source address and address group names. <span class="li-normal">type: list</span></li>
            <ul class="ul-self">
            <li> <span class="li-head">name</span> - Address name. Source firewall.address6.name firewall.addrgrp6.name. <span class="li-normal">type: str</span> <span class="li-required">required: True</span></li>
            </ul>
        <li> <span class="li-head">srcintf</span> - One or more incoming (ingress) interfaces. <span class="li-normal">type: list</span></li>
            <ul class="ul-self">
            <li> <span class="li-head">name</span> - Interface name. Source system.interface.name system.zone.name. <span class="li-normal">type: str</span> <span class="li-required">required: True</span></li>
            </ul>
        <li> <span class="li-head">status</span> - Enable/disable this traffic shaping policy. <span class="li-normal">type: str</span> <span class="li-normal">choices: enable, disable</span></li>
        <li> <span class="li-head">tos</span> - ToS (Type of Service) value used for comparison. <span class="li-normal">type: str</span></li>
        <li> <span class="li-head">tos_mask</span> - Non-zero bit positions are used for comparison while zero bit positions are ignored. <span class="li-normal">type: str</span></li>
        <li> <span class="li-head">tos_negate</span> - Enable negated TOS match. <span class="li-normal">type: str</span> <span class="li-normal">choices: enable, disable</span></li>
        <li> <span class="li-head">traffic_shaper</span> - Traffic shaper to apply to traffic forwarded by the firewall policy. Source firewall.shaper.traffic-shaper.name. <span class="li-normal">type: str</span></li>
        <li> <span class="li-head">traffic_shaper_reverse</span> - Traffic shaper to apply to response traffic received by the firewall policy. Source firewall.shaper.traffic-shaper.name. <span class="li-normal">type: str</span></li>
        <li> <span class="li-head">url_category</span> - IDs of one or more FortiGuard Web Filtering categories that this shaper applies traffic shaping to. <span class="li-normal">type: list</span></li>
            <ul class="ul-self">
            <li> <span class="li-head">id</span> - URL category ID. <span class="li-normal">type: int</span> <span class="li-required">required: True</span></li>
            </ul>
        <li> <span class="li-head">users</span> - Apply this traffic shaping policy to individual users that have authenticated with the FortiGate. <span class="li-normal">type: list</span></li>
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
      - name: Configure shaping policies.
        fortios_firewall_shaping_policy:
          vdom:  "{{ vdom }}"
          state: "present"
          access_token: "<your_own_value>"
          firewall_shaping_policy:
            app_category:
             -
                id:  "4"
            app_group:
             -
                name: "default_name_6 (source application.group.name)"
            application:
             -
                id:  "8"
            class_id: "9"
            comment: "Comments."
            diffserv_forward: "enable"
            diffserv_reverse: "enable"
            diffservcode_forward: "<your_own_value>"
            diffservcode_rev: "<your_own_value>"
            dstaddr:
             -
                name: "default_name_16 (source firewall.address.name firewall.addrgrp.name)"
            dstaddr6:
             -
                name: "default_name_18 (source firewall.address6.name firewall.addrgrp6.name)"
            dstintf:
             -
                name: "default_name_20 (source system.interface.name system.zone.name)"
            groups:
             -
                name: "default_name_22 (source user.group.name)"
            id:  "23"
            internet_service: "enable"
            internet_service_custom:
             -
                name: "default_name_26 (source firewall.internet-service-custom.name)"
            internet_service_custom_group:
             -
                name: "default_name_28 (source firewall.internet-service-custom-group.name)"
            internet_service_group:
             -
                name: "default_name_30 (source firewall.internet-service-group.name)"
            internet_service_id:
             -
                id:  "32 (source firewall.internet-service.id)"
            internet_service_src: "enable"
            internet_service_src_custom:
             -
                name: "default_name_35 (source firewall.internet-service-custom.name)"
            internet_service_src_custom_group:
             -
                name: "default_name_37 (source firewall.internet-service-custom-group.name)"
            internet_service_src_group:
             -
                name: "default_name_39 (source firewall.internet-service-group.name)"
            internet_service_src_id:
             -
                id:  "41 (source firewall.internet-service.id)"
            ip_version: "4"
            name: "default_name_43"
            per_ip_shaper: "<your_own_value> (source firewall.shaper.per-ip-shaper.name)"
            schedule: "<your_own_value> (source firewall.schedule.onetime.name firewall.schedule.recurring.name firewall.schedule.group.name)"
            service:
             -
                name: "default_name_47 (source firewall.service.custom.name firewall.service.group.name)"
            srcaddr:
             -
                name: "default_name_49 (source firewall.address.name firewall.addrgrp.name)"
            srcaddr6:
             -
                name: "default_name_51 (source firewall.address6.name firewall.addrgrp6.name)"
            srcintf:
             -
                name: "default_name_53 (source system.interface.name system.zone.name)"
            status: "enable"
            tos: "<your_own_value>"
            tos_mask: "<your_own_value>"
            tos_negate: "enable"
            traffic_shaper: "<your_own_value> (source firewall.shaper.traffic-shaper.name)"
            traffic_shaper_reverse: "<your_own_value> (source firewall.shaper.traffic-shaper.name)"
            url_category:
             -
                id:  "61"
            users:
             -
                name: "default_name_63 (source user.local.name)"
    


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
