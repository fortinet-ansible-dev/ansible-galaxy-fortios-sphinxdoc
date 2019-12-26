:source: fortios_firewall_sniffer.py

:orphan:

.. _fortios_firewall_sniffer:

fortios_firewall_sniffer -- Configure sniffer in Fortinet's FortiOS and FortiGate.
++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++

.. versionadded:: 2.8

.. contents::
   :local:
   :depth: 1


Synopsis
--------
- This module is able to configure a FortiGate or FortiOS (FOS) device by allowing the user to set and modify firewall feature and sniffer category. Examples include all parameters and values need to be adjusted to datasources before usage. Tested with FOS v6.0.5


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
    <li><span class="li-head">firewall_sniffer</span> - Configure sniffer. <span class="li-normal">default: null</span> <span class="li-normal">type: dict</span></li>
            <ul class="ul-self">

            <li><span class="li-head">state</span> - B(Deprecated) Starting with Ansible 2.9 we recommend using the top-level 'state' parameter. HORIZONTALLINE Indicates whether to create or remove the object. <span class="li-normal">type: str</span> <span class="li-required">required: false</span> <span class="li-normal">choices: present,  absent</span></li>
            <li><span class="li-head">anomaly</span> - Configuration method to edit Denial of Service (DoS) anomaly settings. <span class="li-normal">type: list</span></li>
                    <ul class="ul-self">

                    <li><span class="li-head">action</span> - Action taken when the threshold is reached. <span class="li-normal">type: str</span> <span class="li-normal">choices: pass,  block</span></li>
                    <li><span class="li-head">log</span> - Enable/disable anomaly logging. <span class="li-normal">type: str</span> <span class="li-normal">choices: enable,  disable</span></li>
                    <li><span class="li-head">name</span> - Anomaly name. <span class="li-required">required</span> <span class="li-normal">type: str</span></li>
                    <li><span class="li-head">quarantine</span> - Quarantine method. <span class="li-normal">type: str</span> <span class="li-normal">choices: none,  attacker</span></li>
                    <li><span class="li-head">quarantine_expiry</span> - Duration of quarantine. (Format ###d##h##m, minimum 1m, maximum 364d23h59m). Requires quarantine set to attacker. <span class="li-normal">type: str</span></li>
                    <li><span class="li-head">quarantine_log</span> - Enable/disable quarantine logging. <span class="li-normal">type: str</span> <span class="li-normal">choices: disable,  enable</span></li>
                    <li><span class="li-head">status</span> - Enable/disable this anomaly. <span class="li-normal">type: str</span> <span class="li-normal">choices: disable,  enable</span></li>
                    <li><span class="li-head">threshold</span> - Anomaly threshold. Number of detected instances per minute that triggers the anomaly action. <span class="li-normal">type: int</span></li>
                    <li><span class="li-head">threshold(default)</span> - Number of detected instances per minute which triggers action (1 - 2147483647). Note that each anomaly has a different threshold value assigned to it. <span class="li-normal">type: int</span>
                    </ul>

            <li><span class="li-head">application_list</span> - Name of an existing application list. Source application.list.name. <span class="li-normal">type: str</span></li>
            <li><span class="li-head">application_list_status</span> - Enable/disable application control profile. <span class="li-normal">type: str</span> <span class="li-normal">choices: enable,  disable</span></li>
            <li><span class="li-head">av_profile</span> - Name of an existing antivirus profile. Source antivirus.profile.name. <span class="li-normal">type: str</span></li>
            <li><span class="li-head">av_profile_status</span> - Enable/disable antivirus profile. <span class="li-normal">type: str</span> <span class="li-normal">choices: enable,  disable</span></li>
            <li><span class="li-head">dlp_sensor</span> - Name of an existing DLP sensor. Source dlp.sensor.name. <span class="li-normal">type: str</span></li>
            <li><span class="li-head">dlp_sensor_status</span> - Enable/disable DLP sensor. <span class="li-normal">type: str</span> <span class="li-normal">choices: enable,  disable</span></li>
            <li><span class="li-head">dsri</span> - Enable/disable DSRI. <span class="li-normal">type: str</span> <span class="li-normal">choices: enable,  disable</span></li>
            <li><span class="li-head">host</span> - "Hosts to filter for in sniffer traffic (Format examples: 1.1.1.1, 2.2.2.0/24, 3.3.3.3/255.255.255.0, 4.4.4.0-4.4.4.240)." <span class="li-normal">type: str</span></li>
            <li><span class="li-head">id</span> - Sniffer ID. <span class="li-required">required</span> <span class="li-normal">type: int</span></li>
            <li><span class="li-head">interface</span> - Interface name that traffic sniffing will take place on. Source system.interface.name. <span class="li-normal">type: str</span></li>
            <li><span class="li-head">ips_dos_status</span> - Enable/disable IPS DoS anomaly detection. <span class="li-normal">type: str</span> <span class="li-normal">choices: enable,  disable</span></li>
            <li><span class="li-head">ips_sensor</span> - Name of an existing IPS sensor. Source ips.sensor.name. <span class="li-normal">type: str</span></li>
            <li><span class="li-head">ips_sensor_status</span> - Enable/disable IPS sensor. <span class="li-normal">type: str</span> <span class="li-normal">choices: enable,  disable</span></li>
            <li><span class="li-head">ipv6</span> - Enable/disable sniffing IPv6 packets. <span class="li-normal">type: str</span> <span class="li-normal">choices: enable,  disable</span></li>
            <li><span class="li-head">logtraffic</span> - Either log all sessions, only sessions that have a security profile applied, or disable all logging for this policy. <span class="li-normal">type: str</span> <span class="li-normal">choices: all,  utm,  disable</span></li>
            <li><span class="li-head">max_packet_count</span> - Maximum packet count (1 - 1000000). <span class="li-normal">type: int</span></li>
            <li><span class="li-head">non_ip</span> - Enable/disable sniffing non-IP packets. <span class="li-normal">type: str</span> <span class="li-normal">choices: enable,  disable</span></li>
            <li><span class="li-head">port</span> - "Ports to sniff (Format examples: 10, :20, 30:40, 50-, 100-200)." <span class="li-normal">type: str</span></li>
            <li><span class="li-head">protocol</span> - Integer value for the protocol type as defined by IANA (0 - 255). <span class="li-normal">type: str</span></li>
            <li><span class="li-head">scan_botnet_connections</span> - Enable/disable scanning of connections to Botnet servers. <span class="li-normal">type: str</span> <span class="li-normal">choices: disable,  block,  monitor</span></li>
            <li><span class="li-head">spamfilter_profile</span> - Name of an existing spam filter profile. Source spamfilter.profile.name. <span class="li-normal">type: str</span></li>
            <li><span class="li-head">spamfilter_profile_status</span> - Enable/disable spam filter. <span class="li-normal">type: str</span> <span class="li-normal">choices: enable,  disable</span></li>
            <li><span class="li-head">status</span> - Enable/disable the active status of the sniffer. <span class="li-normal">type: str</span> <span class="li-normal">choices: enable,  disable</span></li>
            <li><span class="li-head">vlan</span> - List of VLANs to sniff. <span class="li-normal">type: str</span></li>
            <li><span class="li-head">webfilter_profile</span> - Name of an existing web filter profile. Source webfilter.profile.name. <span class="li-normal">type: str</span></li>
            <li><span class="li-head">webfilter_profile_status</span> - Enable/disable web filter profile. <span class="li-normal">type: str</span> <span class="li-normal">choices: enable,  disable</span>
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
      - name: Configure sniffer.
        fortios_firewall_sniffer:
          host:  "{{ host }}"
          username: "{{ username }}"
          password: "{{ password }}"
          vdom:  "{{ vdom }}"
          https: "False"
          state: "present"
          firewall_sniffer:
            anomaly:
             -
                action: "pass"
                log: "enable"
                name: "default_name_6"
                quarantine: "none"
                quarantine_expiry: "<your_own_value>"
                quarantine_log: "disable"
                status: "disable"
                threshold: "11"
                threshold(default): "12"
            application_list: "<your_own_value> (source application.list.name)"
            application_list_status: "enable"
            av_profile: "<your_own_value> (source antivirus.profile.name)"
            av_profile_status: "enable"
            dlp_sensor: "<your_own_value> (source dlp.sensor.name)"
            dlp_sensor_status: "enable"
            dsri: "enable"
            host: "myhostname"
            id:  "21"
            interface: "<your_own_value> (source system.interface.name)"
            ips_dos_status: "enable"
            ips_sensor: "<your_own_value> (source ips.sensor.name)"
            ips_sensor_status: "enable"
            ipv6: "enable"
            logtraffic: "all"
            max_packet_count: "28"
            non_ip: "enable"
            port: "<your_own_value>"
            protocol: "<your_own_value>"
            scan_botnet_connections: "disable"
            spamfilter_profile: "<your_own_value> (source spamfilter.profile.name)"
            spamfilter_profile_status: "enable"
            status: "enable"
            vlan: "<your_own_value>"
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