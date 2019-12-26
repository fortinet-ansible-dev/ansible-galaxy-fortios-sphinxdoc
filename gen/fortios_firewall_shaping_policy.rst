:source: fortios_firewall_shaping_policy.py

:orphan:

.. _fortios_firewall_shaping_policy:

fortios_firewall_shaping_policy -- Configure shaping policies in Fortinet's FortiOS and FortiGate.
++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++

.. versionadded:: 2.8

.. contents::
   :local:
   :depth: 1


Synopsis
--------
- This module is able to configure a FortiGate or FortiOS (FOS) device by allowing the user to set and modify firewall feature and shaping_policy category. Examples include all parameters and values need to be adjusted to datasources before usage. Tested with FOS v6.0.5


Requirements
------------
The below requirements are needed on the host that executes this module.

- fortiosapi>=0.9.8


Parameters
----------

.. raw:: html

    <ul>

    <li><span class="li-head">host</span> - FortiOS or FortiGate IP address. <span class="li-normal">type: str</span> <span class="li-required">required: false</span></li>
    <li><span class="li-head">username</span> - FortiOS or FortiGate username. <span class="li-normal">type: str</span> <span class="li-required">required: false</span></li>
    <li><span class="li-head">password</span> - FortiOS or FortiGate password. <span class="li-normal">type: str</span> <span class="li-normal">default: ""</span></li>
    <li><span class="li-head">vdom</span> - Virtual domain, among those defined previously. A vdom is a virtual instance of the FortiGate that can be configured and used as a different unit. <span class="li-normal">type: str</span> <span class="li-normal">default: root</span></li>
    <li><span class="li-head">https</span> - Indicates if the requests towards FortiGate must use HTTPS protocol. <span class="li-normal">type: bool</span> <span class="li-normal">default: true</span></li>
    <li><span class="li-head">ssl_verify</span> - Ensures FortiGate certificate must be verified by a proper CA. <span class="li-normal">type: bool</span> <span class="li-normal">default: true</span></li>
    <li><span class="li-head">state</span> - Indicates whether to create or remove the object. This attribute was present already in previous version in a deeper level. It has been moved out to this outer level. <span class="li-normal">type: str</span> <span class="li-required">required: false</span> <span class="li-normal">choices: present,  absent</span></li>
    <li><span class="li-head">firewall_shaping_policy</span> - Configure shaping policies. <span class="li-normal">default: null</span> <span class="li-normal">type: dict</span></li>
            <ul class="ul-self">

            <li><span class="li-head">state</span> - B(Deprecated) Starting with Ansible 2.9 we recommend using the top-level 'state' parameter. HORIZONTALLINE Indicates whether to create or remove the object. <span class="li-normal">type: str</span> <span class="li-required">required: false</span> <span class="li-normal">choices: present,  absent</span></li>
            <li><span class="li-head">app_category</span> - IDs of one or more application categories that this shaper applies application control traffic shaping to. <span class="li-normal">type: list</span></li>
                    <ul class="ul-self">

                    <li><span class="li-head">id</span> - Category IDs. <span class="li-required">required</span> <span class="li-normal">type: int</span>
                    </ul>

            <li><span class="li-head">application</span> - IDs of one or more applications that this shaper applies application control traffic shaping to. <span class="li-normal">type: list</span></li>
                    <ul class="ul-self">

                    <li><span class="li-head">id</span> - Application IDs. <span class="li-required">required</span> <span class="li-normal">type: int</span>
                    </ul>

            <li><span class="li-head">class_id</span> - Traffic class ID. <span class="li-normal">type: int</span></li>
            <li><span class="li-head">comment</span> - Comments. <span class="li-normal">type: str</span></li>
            <li><span class="li-head">dstaddr</span> - IPv4 destination address and address group names. <span class="li-normal">type: list</span></li>
                    <ul class="ul-self">

                    <li><span class="li-head">name</span> - Address name. Source firewall.address.name firewall.addrgrp.name. <span class="li-required">required</span> <span class="li-normal">type: str</span>
                    </ul>

            <li><span class="li-head">dstaddr6</span> - IPv6 destination address and address group names. <span class="li-normal">type: list</span></li>
                    <ul class="ul-self">

                    <li><span class="li-head">name</span> - Address name. Source firewall.address6.name firewall.addrgrp6.name. <span class="li-required">required</span> <span class="li-normal">type: str</span>
                    </ul>

            <li><span class="li-head">dstintf</span> - One or more outgoing (egress) interfaces. <span class="li-normal">type: list</span></li>
                    <ul class="ul-self">

                    <li><span class="li-head">name</span> - Interface name. Source system.interface.name system.zone.name. <span class="li-required">required</span> <span class="li-normal">type: str</span>
                    </ul>

            <li><span class="li-head">groups</span> - Apply this traffic shaping policy to user groups that have authenticated with the FortiGate. <span class="li-normal">type: list</span></li>
                    <ul class="ul-self">

                    <li><span class="li-head">name</span> - Group name. Source user.group.name. <span class="li-required">required</span> <span class="li-normal">type: str</span>
                    </ul>

            <li><span class="li-head">id</span> - Shaping policy ID. <span class="li-required">required</span> <span class="li-normal">type: int</span></li>
            <li><span class="li-head">internet_service</span> - Enable/disable use of Internet Services for this policy. If enabled, destination address and service are not used. <span class="li-normal">type: str</span> <span class="li-normal">choices: enable,  disable</span></li>
            <li><span class="li-head">internet_service_custom</span> - Custom Internet Service name. <span class="li-normal">type: list</span></li>
                    <ul class="ul-self">

                    <li><span class="li-head">name</span> - Custom Internet Service name. Source firewall.internet-service-custom.name. <span class="li-required">required</span> <span class="li-normal">type: str</span>
                    </ul>

            <li><span class="li-head">internet_service_id</span> - Internet Service ID. <span class="li-normal">type: list</span></li>
                    <ul class="ul-self">

                    <li><span class="li-head">id</span> - Internet Service ID. Source firewall.internet-service.id. <span class="li-required">required</span> <span class="li-normal">type: int</span>
                    </ul>

            <li><span class="li-head">internet_service_src</span> - Enable/disable use of Internet Services in source for this policy. If enabled, source address is not used. <span class="li-normal">type: str</span> <span class="li-normal">choices: enable,  disable</span></li>
            <li><span class="li-head">internet_service_src_custom</span> - Custom Internet Service source name. <span class="li-normal">type: list</span></li>
                    <ul class="ul-self">

                    <li><span class="li-head">name</span> - Custom Internet Service name. Source firewall.internet-service-custom.name. <span class="li-required">required</span> <span class="li-normal">type: str</span>
                    </ul>

            <li><span class="li-head">internet_service_src_id</span> - Internet Service source ID. <span class="li-normal">type: list</span></li>
                    <ul class="ul-self">

                    <li><span class="li-head">id</span> - Internet Service ID. Source firewall.internet-service.id. <span class="li-required">required</span> <span class="li-normal">type: int</span>
                    </ul>

            <li><span class="li-head">ip_version</span> - Apply this traffic shaping policy to IPv4 or IPv6 traffic. <span class="li-normal">type: str</span> <span class="li-normal">choices: 4,  6</span></li>
            <li><span class="li-head">per_ip_shaper</span> - Per-IP traffic shaper to apply with this policy. Source firewall.shaper.per-ip-shaper.name. <span class="li-normal">type: str</span></li>
            <li><span class="li-head">schedule</span> - Schedule name. Source firewall.schedule.onetime.name firewall.schedule.recurring.name firewall.schedule.group.name. <span class="li-normal">type: str</span></li>
            <li><span class="li-head">service</span> - Service and service group names. <span class="li-normal">type: list</span></li>
                    <ul class="ul-self">

                    <li><span class="li-head">name</span> - Service name. Source firewall.service.custom.name firewall.service.group.name. <span class="li-required">required</span> <span class="li-normal">type: str</span>
                    </ul>

            <li><span class="li-head">srcaddr</span> - IPv4 source address and address group names. <span class="li-normal">type: list</span></li>
                    <ul class="ul-self">

                    <li><span class="li-head">name</span> - Address name. Source firewall.address.name firewall.addrgrp.name. <span class="li-required">required</span> <span class="li-normal">type: str</span>
                    </ul>

            <li><span class="li-head">srcaddr6</span> - IPv6 source address and address group names. <span class="li-normal">type: list</span></li>
                    <ul class="ul-self">

                    <li><span class="li-head">name</span> - Address name. Source firewall.address6.name firewall.addrgrp6.name. <span class="li-required">required</span> <span class="li-normal">type: str</span>
                    </ul>

            <li><span class="li-head">status</span> - Enable/disable this traffic shaping policy. <span class="li-normal">type: str</span> <span class="li-normal">choices: enable,  disable</span></li>
            <li><span class="li-head">traffic_shaper</span> - Traffic shaper to apply to traffic forwarded by the firewall policy. Source firewall.shaper.traffic-shaper.name. <span class="li-normal">type: str</span></li>
            <li><span class="li-head">traffic_shaper_reverse</span> - Traffic shaper to apply to response traffic received by the firewall policy. Source firewall.shaper.traffic-shaper.name. <span class="li-normal">type: str</span></li>
            <li><span class="li-head">url_category</span> - IDs of one or more FortiGuard Web Filtering categories that this shaper applies traffic shaping to. <span class="li-normal">type: list</span></li>
                    <ul class="ul-self">

                    <li><span class="li-head">id</span> - URL category ID. <span class="li-required">required</span> <span class="li-normal">type: int</span>
                    </ul>

            <li><span class="li-head">users</span> - Apply this traffic shaping policy to individual users that have authenticated with the FortiGate. <span class="li-normal">type: list</span></li>
                    <ul class="ul-self">

                    <li><span class="li-head">name</span> - User name. Source user.local.name. <span class="li-required">required</span> <span class="li-normal">type: str</span>
                    </ul>

            </ul>

    </ul>




Notes
-----

.. note::


   - Requires fortiosapi library developed by Fortinet

   - Run as a local_action in your playbook



Examples
--------

.. code-block:: yaml+jinja

    - hosts: localhost
      vars:
       host: "192.168.122.40"
       username: "admin"
       password: ""
       vdom: "root"
       ssl_verify: "False"
      tasks:
      - name: Configure shaping policies.
        fortios_firewall_shaping_policy:
          host:  "{{ host }}"
          username: "{{ username }}"
          password: "{{ password }}"
          vdom:  "{{ vdom }}"
          https: "False"
          state: "present"
          firewall_shaping_policy:
            app_category:
             -
                id:  "4"
            application:
             -
                id:  "6"
            class_id: "7"
            comment: "Comments."
            dstaddr:
             -
                name: "default_name_10 (source firewall.address.name firewall.addrgrp.name)"
            dstaddr6:
             -
                name: "default_name_12 (source firewall.address6.name firewall.addrgrp6.name)"
            dstintf:
             -
                name: "default_name_14 (source system.interface.name system.zone.name)"
            groups:
             -
                name: "default_name_16 (source user.group.name)"
            id:  "17"
            internet_service: "enable"
            internet_service_custom:
             -
                name: "default_name_20 (source firewall.internet-service-custom.name)"
            internet_service_id:
             -
                id:  "22 (source firewall.internet-service.id)"
            internet_service_src: "enable"
            internet_service_src_custom:
             -
                name: "default_name_25 (source firewall.internet-service-custom.name)"
            internet_service_src_id:
             -
                id:  "27 (source firewall.internet-service.id)"
            ip_version: "4"
            per_ip_shaper: "<your_own_value> (source firewall.shaper.per-ip-shaper.name)"
            schedule: "<your_own_value> (source firewall.schedule.onetime.name firewall.schedule.recurring.name firewall.schedule.group.name)"
            service:
             -
                name: "default_name_32 (source firewall.service.custom.name firewall.service.group.name)"
            srcaddr:
             -
                name: "default_name_34 (source firewall.address.name firewall.addrgrp.name)"
            srcaddr6:
             -
                name: "default_name_36 (source firewall.address6.name firewall.addrgrp6.name)"
            status: "enable"
            traffic_shaper: "<your_own_value> (source firewall.shaper.traffic-shaper.name)"
            traffic_shaper_reverse: "<your_own_value> (source firewall.shaper.traffic-shaper.name)"
            url_category:
             -
                id:  "41"
            users:
             -
                name: "default_name_43 (source user.local.name)"



Return Values
-------------
Common return values are documented: https://docs.ansible.com/ansible/latest/reference_appendices/common_return_values.html#common-return-values, the following are the fields unique to this module:

.. raw:: html

    <ul>

    <li><span class="li-return">build</span> - Build number of the fortigate image <span class="li-normal">returned: always</span> <span class="li-normal">type: str</span> <span class="li-normal">sample: '1547'</span></li>
    <li><span class="li-return">http_method</span> - Last method used to provision the content into FortiGate <span class="li-normal">returned: always</span> <span class="li-normal">type: str</span> <span class="li-normal">sample: 'PUT'</span></li>
    <li><span class="li-return">http_status</span> - Last result given by FortiGate on last operation applied <span class="li-normal">returned: always</span> <span class="li-normal">type: str</span> <span class="li-normal">sample: 200</span></li>
    <li><span class="li-return">mkey</span> - Master key (id) used in the last call to FortiGate <span class="li-normal">returned: success</span> <span class="li-normal">type: str</span> <span class="li-normal">sample: id</span></li>
    <li><span class="li-return">name</span> - Name of the table used to fulfill the request <span class="li-normal">returned: always</span> <span class="li-normal">type: str</span> <span class="li-normal">sample: urlfilter</span></li>
    <li><span class="li-return">path</span> - Path of the table used to fulfill the request <span class="li-normal">returned: always</span> <span class="li-normal">type: str</span> <span class="li-normal">sample: webfilter</span></li>
    <li><span class="li-return">revision</span> - Internal revision number <span class="li-normal">returned: always</span> <span class="li-normal">type: str</span> <span class="li-normal">sample: 17.0.2.10658</span></li>
    <li><span class="li-return">serial</span> - Serial number of the unit <span class="li-normal">returned: always</span> <span class="li-normal">type: str</span> <span class="li-normal">sample: FGVMEVYYQT3AB5352</span></li>
    <li><span class="li-return">status</span> - Indication of the operation's result <span class="li-normal">returned: always</span> <span class="li-normal">type: str</span> <span class="li-normal">sample: success</span></li>
    <li><span class="li-return">vdom</span> - Virtual domain used <span class="li-normal">returned: always</span> <span class="li-normal">type: str</span> <span class="li-normal">sample: root</span></li>
    <li><span class="li-return">version</span> - Version of the FortiGate <span class="li-normal">returned: always</span> <span class="li-normal">type: str</span> <span class="li-normal">sample: v5.6.3</span></li>
    </ul>



Status
------

- This module is not guaranteed to have a backwards compatible interface.



Authors
-------

- Miguel Angel Munoz (@mamunozgonzalez)
- Nicolas Thomas (@thomnico)



.. hint::
    If you notice any issues in this documentation, you can create a pull request to improve it.