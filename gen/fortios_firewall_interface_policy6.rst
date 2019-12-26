:source: fortios_firewall_interface_policy6.py

:orphan:

.. _fortios_firewall_interface_policy6:

fortios_firewall_interface_policy6 -- Configure IPv6 interface policies in Fortinet's FortiOS and FortiGate.
++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++

.. versionadded:: 2.8

.. contents::
   :local:
   :depth: 1


Synopsis
--------
- This module is able to configure a FortiGate or FortiOS (FOS) device by allowing the user to set and modify firewall feature and interface_policy6 category. Examples include all parameters and values need to be adjusted to datasources before usage. Tested with FOS v6.0.5


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
    <li><span class="li-head">firewall_interface_policy6</span> - Configure IPv6 interface policies. <span class="li-normal">default: null</span> <span class="li-normal">type: dict</span></li>
            <ul class="ul-self">

            <li><span class="li-head">state</span> - B(Deprecated) Starting with Ansible 2.9 we recommend using the top-level 'state' parameter. HORIZONTALLINE Indicates whether to create or remove the object. <span class="li-normal">type: str</span> <span class="li-required">required: false</span> <span class="li-normal">choices: present,  absent</span></li>
            <li><span class="li-head">address_type</span> - Policy address type (IPv4 or IPv6). <span class="li-normal">type: str</span> <span class="li-normal">choices: ipv4,  ipv6</span></li>
            <li><span class="li-head">application_list</span> - Application list name. Source application.list.name. <span class="li-normal">type: str</span></li>
            <li><span class="li-head">application_list_status</span> - Enable/disable application control. <span class="li-normal">type: str</span> <span class="li-normal">choices: enable,  disable</span></li>
            <li><span class="li-head">av_profile</span> - Antivirus profile. Source antivirus.profile.name. <span class="li-normal">type: str</span></li>
            <li><span class="li-head">av_profile_status</span> - Enable/disable antivirus. <span class="li-normal">type: str</span> <span class="li-normal">choices: enable,  disable</span></li>
            <li><span class="li-head">comments</span> - Comments. <span class="li-normal">type: str</span></li>
            <li><span class="li-head">dlp_sensor</span> - DLP sensor name. Source dlp.sensor.name. <span class="li-normal">type: str</span></li>
            <li><span class="li-head">dlp_sensor_status</span> - Enable/disable DLP. <span class="li-normal">type: str</span> <span class="li-normal">choices: enable,  disable</span></li>
            <li><span class="li-head">dsri</span> - Enable/disable DSRI. <span class="li-normal">type: str</span> <span class="li-normal">choices: enable,  disable</span></li>
            <li><span class="li-head">dstaddr6</span> - IPv6 address object to limit traffic monitoring to network traffic sent to the specified address or range. <span class="li-normal">type: list</span></li>
                    <ul class="ul-self">

                    <li><span class="li-head">name</span> - Address name. Source firewall.address6.name firewall.addrgrp6.name. <span class="li-required">required</span> <span class="li-normal">type: str</span>
                    </ul>

            <li><span class="li-head">interface</span> - Monitored interface name from available interfaces. Source system.zone.name system.interface.name. <span class="li-normal">type: str</span></li>
            <li><span class="li-head">ips_sensor</span> - IPS sensor name. Source ips.sensor.name. <span class="li-normal">type: str</span></li>
            <li><span class="li-head">ips_sensor_status</span> - Enable/disable IPS. <span class="li-normal">type: str</span> <span class="li-normal">choices: enable,  disable</span></li>
            <li><span class="li-head">label</span> - Label. <span class="li-normal">type: str</span></li>
            <li><span class="li-head">logtraffic</span> - "Logging type to be used in this policy (Options: all | utm | disable)." <span class="li-normal">type: str</span> <span class="li-normal">choices: all,  utm,  disable</span></li>
            <li><span class="li-head">policyid</span> - Policy ID. <span class="li-required">required</span> <span class="li-normal">type: int</span></li>
            <li><span class="li-head">scan_botnet_connections</span> - Enable/disable scanning for connections to Botnet servers. <span class="li-normal">type: str</span> <span class="li-normal">choices: disable,  block,  monitor</span></li>
            <li><span class="li-head">service6</span> - Service name. <span class="li-normal">type: list</span></li>
                    <ul class="ul-self">

                    <li><span class="li-head">name</span> - Address name. Source firewall.service.custom.name firewall.service.group.name. <span class="li-required">required</span> <span class="li-normal">type: str</span>
                    </ul>

            <li><span class="li-head">spamfilter_profile</span> - Antispam profile. Source spamfilter.profile.name. <span class="li-normal">type: str</span></li>
            <li><span class="li-head">spamfilter_profile_status</span> - Enable/disable antispam. <span class="li-normal">type: str</span> <span class="li-normal">choices: enable,  disable</span></li>
            <li><span class="li-head">srcaddr6</span> - IPv6 address object to limit traffic monitoring to network traffic sent from the specified address or range. <span class="li-normal">type: list</span></li>
                    <ul class="ul-self">

                    <li><span class="li-head">name</span> - Address name. Source firewall.address6.name firewall.addrgrp6.name. <span class="li-required">required</span> <span class="li-normal">type: str</span>
                    </ul>

            <li><span class="li-head">status</span> - Enable/disable this policy. <span class="li-normal">type: str</span> <span class="li-normal">choices: enable,  disable</span></li>
            <li><span class="li-head">webfilter_profile</span> - Web filter profile. Source webfilter.profile.name. <span class="li-normal">type: str</span></li>
            <li><span class="li-head">webfilter_profile_status</span> - Enable/disable web filtering. <span class="li-normal">type: str</span> <span class="li-normal">choices: enable,  disable</span>
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
      - name: Configure IPv6 interface policies.
        fortios_firewall_interface_policy6:
          host:  "{{ host }}"
          username: "{{ username }}"
          password: "{{ password }}"
          vdom:  "{{ vdom }}"
          https: "False"
          state: "present"
          firewall_interface_policy6:
            address_type: "ipv4"
            application_list: "<your_own_value> (source application.list.name)"
            application_list_status: "enable"
            av_profile: "<your_own_value> (source antivirus.profile.name)"
            av_profile_status: "enable"
            comments: "<your_own_value>"
            dlp_sensor: "<your_own_value> (source dlp.sensor.name)"
            dlp_sensor_status: "enable"
            dsri: "enable"
            dstaddr6:
             -
                name: "default_name_13 (source firewall.address6.name firewall.addrgrp6.name)"
            interface: "<your_own_value> (source system.zone.name system.interface.name)"
            ips_sensor: "<your_own_value> (source ips.sensor.name)"
            ips_sensor_status: "enable"
            label: "<your_own_value>"
            logtraffic: "all"
            policyid: "19"
            scan_botnet_connections: "disable"
            service6:
             -
                name: "default_name_22 (source firewall.service.custom.name firewall.service.group.name)"
            spamfilter_profile: "<your_own_value> (source spamfilter.profile.name)"
            spamfilter_profile_status: "enable"
            srcaddr6:
             -
                name: "default_name_26 (source firewall.address6.name firewall.addrgrp6.name)"
            status: "enable"
            webfilter_profile: "<your_own_value> (source webfilter.profile.name)"
            webfilter_profile_status: "enable"



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