:source: fortios_system_accprofile.py

:orphan:

.. _fortios_system_accprofile:

fortios_system_accprofile -- Configure access profiles for system administrators in Fortinet's FortiOS and FortiGate.
+++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++

.. versionadded:: 2.8

.. contents::
   :local:
   :depth: 1


Synopsis
--------
- This module is able to configure a FortiGate or FortiOS (FOS) device by allowing the user to set and modify system feature and accprofile category. Examples include all parameters and values need to be adjusted to datasources before usage. Tested with FOS v6.0.5


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
    <li><span class="li-head">system_accprofile</span> - Configure access profiles for system administrators. <span class="li-normal">default: null</span> <span class="li-normal">type: dict</span></li>
            <ul class="ul-self">

            <li><span class="li-head">state</span> - B(Deprecated) Starting with Ansible 2.9 we recommend using the top-level 'state' parameter. HORIZONTALLINE Indicates whether to create or remove the object. <span class="li-normal">type: str</span> <span class="li-required">required: false</span> <span class="li-normal">choices: present,  absent</span></li>
            <li><span class="li-head">admintimeout</span> - Administrator timeout for this access profile (0 - 480 min). <span class="li-normal">type: int</span></li>
            <li><span class="li-head">admintimeout_override</span> - Enable/disable overriding the global administrator idle timeout. <span class="li-normal">type: str</span> <span class="li-normal">choices: enable,  disable</span></li>
            <li><span class="li-head">authgrp</span> - Administrator access to Users and Devices. <span class="li-normal">type: str</span> <span class="li-normal">choices: none,  read,  read-write</span></li>
            <li><span class="li-head">comments</span> - Comment. <span class="li-normal">type: str</span></li>
            <li><span class="li-head">ftviewgrp</span> - FortiView. <span class="li-normal">type: str</span> <span class="li-normal">choices: none,  read,  read-write</span></li>
            <li><span class="li-head">fwgrp</span> - Administrator access to the Firewall configuration. <span class="li-normal">type: str</span> <span class="li-normal">choices: none,  read,  read-write,  custom</span></li>
            <li><span class="li-head">fwgrp_permission</span> - Custom firewall permission. <span class="li-normal">type: dict</span></li>
                    <ul class="ul-self">

                    <li><span class="li-head">address</span> - Address Configuration. <span class="li-normal">type: str</span> <span class="li-normal">choices: none,  read,  read-write</span></li>
                    <li><span class="li-head">policy</span> - Policy Configuration. <span class="li-normal">type: str</span> <span class="li-normal">choices: none,  read,  read-write</span></li>
                    <li><span class="li-head">schedule</span> - Schedule Configuration. <span class="li-normal">type: str</span> <span class="li-normal">choices: none,  read,  read-write</span></li>
                    <li><span class="li-head">service</span> - Service Configuration. <span class="li-normal">type: str</span> <span class="li-normal">choices: none,  read,  read-write</span>
                    </ul>

            <li><span class="li-head">loggrp</span> - Administrator access to Logging and Reporting including viewing log messages. <span class="li-normal">type: str</span> <span class="li-normal">choices: none,  read,  read-write,  custom</span></li>
            <li><span class="li-head">loggrp_permission</span> - Custom Log & Report permission. <span class="li-normal">type: dict</span></li>
                    <ul class="ul-self">

                    <li><span class="li-head">config</span> - Log & Report configuration. <span class="li-normal">type: str</span> <span class="li-normal">choices: none,  read,  read-write</span></li>
                    <li><span class="li-head">data_access</span> - Log & Report Data Access. <span class="li-normal">type: str</span> <span class="li-normal">choices: none,  read,  read-write</span></li>
                    <li><span class="li-head">report_access</span> - Log & Report Report Access. <span class="li-normal">type: str</span> <span class="li-normal">choices: none,  read,  read-write</span></li>
                    <li><span class="li-head">threat_weight</span> - Log & Report Threat Weight. <span class="li-normal">type: str</span> <span class="li-normal">choices: none,  read,  read-write</span>
                    </ul>

            <li><span class="li-head">name</span> - Profile name. <span class="li-required">required</span> <span class="li-normal">type: str</span></li>
            <li><span class="li-head">netgrp</span> - Network Configuration. <span class="li-normal">type: str</span> <span class="li-normal">choices: none,  read,  read-write,  custom</span></li>
            <li><span class="li-head">netgrp_permission</span> - Custom network permission. <span class="li-normal">type: dict</span></li>
                    <ul class="ul-self">

                    <li><span class="li-head">cfg</span> - Network Configuration. <span class="li-normal">type: str</span> <span class="li-normal">choices: none,  read,  read-write</span></li>
                    <li><span class="li-head">packet_capture</span> - Packet Capture Configuration. <span class="li-normal">type: str</span> <span class="li-normal">choices: none,  read,  read-write</span></li>
                    <li><span class="li-head">route_cfg</span> - Router Configuration. <span class="li-normal">type: str</span> <span class="li-normal">choices: none,  read,  read-write</span>
                    </ul>

            <li><span class="li-head">scope</span> - "Scope of admin access: global or specific VDOM(s)." <span class="li-normal">type: str</span> <span class="li-normal">choices: vdom,  global</span></li>
            <li><span class="li-head">secfabgrp</span> - Security Fabric. <span class="li-normal">type: str</span> <span class="li-normal">choices: none,  read,  read-write</span></li>
            <li><span class="li-head">sysgrp</span> - System Configuration. <span class="li-normal">type: str</span> <span class="li-normal">choices: none,  read,  read-write,  custom</span></li>
            <li><span class="li-head">sysgrp_permission</span> - Custom system permission. <span class="li-normal">type: dict</span></li>
                    <ul class="ul-self">

                    <li><span class="li-head">admin</span> - Administrator Users. <span class="li-normal">type: str</span> <span class="li-normal">choices: none,  read,  read-write</span></li>
                    <li><span class="li-head">cfg</span> - System Configuration. <span class="li-normal">type: str</span> <span class="li-normal">choices: none,  read,  read-write</span></li>
                    <li><span class="li-head">mnt</span> - Maintenance. <span class="li-normal">type: str</span> <span class="li-normal">choices: none,  read,  read-write</span></li>
                    <li><span class="li-head">upd</span> - FortiGuard Updates. <span class="li-normal">type: str</span> <span class="li-normal">choices: none,  read,  read-write</span>
                    </ul>

            <li><span class="li-head">utmgrp</span> - Administrator access to Security Profiles. <span class="li-normal">type: str</span> <span class="li-normal">choices: none,  read,  read-write,  custom</span></li>
            <li><span class="li-head">utmgrp_permission</span> - Custom Security Profile permissions. <span class="li-normal">type: dict</span></li>
                    <ul class="ul-self">

                    <li><span class="li-head">antivirus</span> - Antivirus profiles and settings. <span class="li-normal">type: str</span> <span class="li-normal">choices: none,  read,  read-write</span></li>
                    <li><span class="li-head">application_control</span> - Application Control profiles and settings. <span class="li-normal">type: str</span> <span class="li-normal">choices: none,  read,  read-write</span></li>
                    <li><span class="li-head">data_loss_prevention</span> - DLP profiles and settings. <span class="li-normal">type: str</span> <span class="li-normal">choices: none,  read,  read-write</span></li>
                    <li><span class="li-head">dnsfilter</span> - DNS Filter profiles and settings. <span class="li-normal">type: str</span> <span class="li-normal">choices: none,  read,  read-write</span></li>
                    <li><span class="li-head">endpoint_control</span> - FortiClient Profiles. <span class="li-normal">type: str</span> <span class="li-normal">choices: none,  read,  read-write</span></li>
                    <li><span class="li-head">icap</span> - ICAP profiles and settings. <span class="li-normal">type: str</span> <span class="li-normal">choices: none,  read,  read-write</span></li>
                    <li><span class="li-head">ips</span> - IPS profiles and settings. <span class="li-normal">type: str</span> <span class="li-normal">choices: none,  read,  read-write</span></li>
                    <li><span class="li-head">spamfilter</span> - AntiSpam filter and settings. <span class="li-normal">type: str</span> <span class="li-normal">choices: none,  read,  read-write</span></li>
                    <li><span class="li-head">voip</span> - VoIP profiles and settings. <span class="li-normal">type: str</span> <span class="li-normal">choices: none,  read,  read-write</span></li>
                    <li><span class="li-head">waf</span> - Web Application Firewall profiles and settings. <span class="li-normal">type: str</span> <span class="li-normal">choices: none,  read,  read-write</span></li>
                    <li><span class="li-head">webfilter</span> - Web Filter profiles and settings. <span class="li-normal">type: str</span> <span class="li-normal">choices: none,  read,  read-write</span>
                    </ul>

            <li><span class="li-head">vpngrp</span> - Administrator access to IPsec, SSL, PPTP, and L2TP VPN. <span class="li-normal">type: str</span> <span class="li-normal">choices: none,  read,  read-write</span></li>
            <li><span class="li-head">wanoptgrp</span> - Administrator access to WAN Opt & Cache. <span class="li-normal">type: str</span> <span class="li-normal">choices: none,  read,  read-write</span></li>
            <li><span class="li-head">wifi</span> - Administrator access to the WiFi controller and Switch controller. <span class="li-normal">type: str</span> <span class="li-normal">choices: none,  read,  read-write</span>
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
      - name: Configure access profiles for system administrators.
        fortios_system_accprofile:
          host:  "{{ host }}"
          username: "{{ username }}"
          password: "{{ password }}"
          vdom:  "{{ vdom }}"
          https: "False"
          state: "present"
          system_accprofile:
            admintimeout: "3"
            admintimeout_override: "enable"
            authgrp: "none"
            comments: "<your_own_value>"
            ftviewgrp: "none"
            fwgrp: "none"
            fwgrp_permission:
                address: "none"
                policy: "none"
                schedule: "none"
                service: "none"
            loggrp: "none"
            loggrp_permission:
                config: "none"
                data_access: "none"
                report_access: "none"
                threat_weight: "none"
            name: "default_name_20"
            netgrp: "none"
            netgrp_permission:
                cfg: "none"
                packet_capture: "none"
                route_cfg: "none"
            scope: "vdom"
            secfabgrp: "none"
            sysgrp: "none"
            sysgrp_permission:
                admin: "none"
                cfg: "none"
                mnt: "none"
                upd: "none"
            utmgrp: "none"
            utmgrp_permission:
                antivirus: "none"
                application_control: "none"
                data_loss_prevention: "none"
                dnsfilter: "none"
                endpoint_control: "none"
                icap: "none"
                ips: "none"
                spamfilter: "none"
                voip: "none"
                waf: "none"
                webfilter: "none"
            vpngrp: "none"
            wanoptgrp: "none"
            wifi: "none"



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