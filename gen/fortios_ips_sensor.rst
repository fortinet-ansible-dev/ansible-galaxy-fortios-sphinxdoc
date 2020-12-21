:source: fortios_ips_sensor.py

:orphan:

.. fortios_ips_sensor:

fortios_ips_sensor -- Configure IPS sensor in Fortinet's FortiOS and FortiGate.
+++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++

.. versionadded:: 2.8

.. contents::
   :local:
   :depth: 1


Synopsis
--------
- This module is able to configure a FortiGate or FortiOS (FOS) device by allowing the user to set and modify ips feature and sensor category. Examples include all parameters and values need to be adjusted to datasources before usage. Tested with FOS v6.2.0



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
    <li> <span class="li-head">ips_sensor</span> - Configure IPS sensor. <span class="li-normal">type: dict</span></li>
        <ul class="ul-self">
        <li> <span class="li-head">state</span> - B(Deprecated) <span class="li-normal">type: str</span> <span class="li-required">required: False</span> <span class="li-normal">choices: present, absent</span></li>
        <li> <span class="li-head">block_malicious_url</span> - Enable/disable malicious URL blocking. <span class="li-normal">type: str</span> <span class="li-normal">choices: disable, enable</span></li>
        <li> <span class="li-head">comment</span> - Comment. <span class="li-normal">type: str</span></li>
        <li> <span class="li-head">entries</span> - IPS sensor filter. <span class="li-normal">type: list</span></li>
            <ul class="ul-self">
            <li> <span class="li-head">action</span> - Action taken with traffic in which signatures are detected. <span class="li-normal">type: str</span> <span class="li-normal">choices: pass, block, reset, default</span></li>
            <li> <span class="li-head">application</span> - Applications to be protected. set application ? lists available applications. all includes all applications. other includes all unlisted applications. <span class="li-normal">type: str</span></li>
            <li> <span class="li-head">exempt_ip</span> - Traffic from selected source or destination IP addresses is exempt from this signature. <span class="li-normal">type: list</span></li>
                <ul class="ul-self">
                <li> <span class="li-head">dst_ip</span> - Destination IP address and netmask. <span class="li-normal">type: str</span></li>
                <li> <span class="li-head">id</span> - Exempt IP ID. <span class="li-normal">type: int</span> <span class="li-required">required: True</span></li>
                <li> <span class="li-head">src_ip</span> - Source IP address and netmask. <span class="li-normal">type: str</span></li>
                </ul>
            <li> <span class="li-head">id</span> - Rule ID in IPS database (0 - 4294967295). <span class="li-normal">type: int</span> <span class="li-required">required: True</span></li>
            <li> <span class="li-head">location</span> - Protect client or server traffic. <span class="li-normal">type: str</span></li>
            <li> <span class="li-head">log</span> - Enable/disable logging of signatures included in filter. <span class="li-normal">type: str</span> <span class="li-normal">choices: disable, enable</span></li>
            <li> <span class="li-head">log_attack_context</span> - Enable/disable logging of attack context: URL buffer, header buffer, body buffer, packet buffer. <span class="li-normal">type: str</span> <span class="li-normal">choices: disable, enable</span></li>
            <li> <span class="li-head">log_packet</span> - Enable/disable packet logging. Enable to save the packet that triggers the filter. You can download the packets in pcap format for diagnostic use. <span class="li-normal">type: str</span> <span class="li-normal">choices: disable, enable</span></li>
            <li> <span class="li-head">os</span> - Operating systems to be protected.  all includes all operating systems. other includes all unlisted operating systems. <span class="li-normal">type: str</span></li>
            <li> <span class="li-head">protocol</span> - Protocols to be examined. set protocol ? lists available protocols. all includes all protocols. other includes all unlisted protocols. <span class="li-normal">type: str</span></li>
            <li> <span class="li-head">quarantine</span> - Quarantine method. <span class="li-normal">type: str</span> <span class="li-normal">choices: none, attacker</span></li>
            <li> <span class="li-head">quarantine_expiry</span> - Duration of quarantine. (Format <span class="li-normal">type: str</span></li>
            <li> <span class="li-head">quarantine_log</span> - Enable/disable quarantine logging. <span class="li-normal">type: str</span> <span class="li-normal">choices: disable, enable</span></li>
            <li> <span class="li-head">rate_count</span> - Count of the rate. <span class="li-normal">type: int</span></li>
            <li> <span class="li-head">rate_duration</span> - Duration (sec) of the rate. <span class="li-normal">type: int</span></li>
            <li> <span class="li-head">rate_mode</span> - Rate limit mode. <span class="li-normal">type: str</span> <span class="li-normal">choices: periodical, continuous</span></li>
            <li> <span class="li-head">rate_track</span> - Track the packet protocol field. <span class="li-normal">type: str</span> <span class="li-normal">choices: none, src-ip, dest-ip, dhcp-client-mac, dns-domain</span></li>
            <li> <span class="li-head">rule</span> - Identifies the predefined or custom IPS signatures to add to the sensor. <span class="li-normal">type: list</span></li>
                <ul class="ul-self">
                <li> <span class="li-head">id</span> - Rule IPS. <span class="li-normal">type: int</span> <span class="li-required">required: True</span></li>
                </ul>
            <li> <span class="li-head">severity</span> - Relative severity of the signature, from info to critical. Log messages generated by the signature include the severity. <span class="li-normal">type: str</span></li>
            <li> <span class="li-head">status</span> - Status of the signatures included in filter. default enables the filter and only use filters with default status of enable. Filters with default status of disable will not be used. <span class="li-normal">type: str</span> <span class="li-normal">choices: disable, enable, default</span></li>
            </ul>
        <li> <span class="li-head">extended_log</span> - Enable/disable extended logging. <span class="li-normal">type: str</span> <span class="li-normal">choices: enable, disable</span></li>
        <li> <span class="li-head">filter</span> - IPS sensor filter. <span class="li-normal">type: list</span></li>
            <ul class="ul-self">
            <li> <span class="li-head">action</span> - Action of selected rules. <span class="li-normal">type: str</span> <span class="li-normal">choices: pass, block, reset, default</span></li>
            <li> <span class="li-head">application</span> - Vulnerable application filter. <span class="li-normal">type: str</span></li>
            <li> <span class="li-head">location</span> - Vulnerability location filter. <span class="li-normal">type: str</span></li>
            <li> <span class="li-head">log</span> - Enable/disable logging of selected rules. <span class="li-normal">type: str</span> <span class="li-normal">choices: disable, enable</span></li>
            <li> <span class="li-head">log_packet</span> - Enable/disable packet logging of selected rules. <span class="li-normal">type: str</span> <span class="li-normal">choices: disable, enable</span></li>
            <li> <span class="li-head">name</span> - Filter name. <span class="li-normal">type: str</span> <span class="li-required">required: True</span></li>
            <li> <span class="li-head">os</span> - Vulnerable OS filter. <span class="li-normal">type: str</span></li>
            <li> <span class="li-head">protocol</span> - Vulnerable protocol filter. <span class="li-normal">type: str</span></li>
            <li> <span class="li-head">quarantine</span> - Quarantine IP or interface. <span class="li-normal">type: str</span> <span class="li-normal">choices: none, attacker</span></li>
            <li> <span class="li-head">quarantine_expiry</span> - Duration of quarantine in minute. <span class="li-normal">type: int</span></li>
            <li> <span class="li-head">quarantine_log</span> - Enable/disable logging of selected quarantine. <span class="li-normal">type: str</span> <span class="li-normal">choices: disable, enable</span></li>
            <li> <span class="li-head">severity</span> - Vulnerability severity filter. <span class="li-normal">type: str</span></li>
            <li> <span class="li-head">status</span> - Selected rules status. <span class="li-normal">type: str</span> <span class="li-normal">choices: disable, enable, default</span></li>
            </ul>
        <li> <span class="li-head">name</span> - Sensor name. <span class="li-normal">type: str</span> <span class="li-required">required: True</span></li>
        <li> <span class="li-head">override</span> - IPS override rule. <span class="li-normal">type: list</span></li>
            <ul class="ul-self">
            <li> <span class="li-head">action</span> - Action of override rule. <span class="li-normal">type: str</span> <span class="li-normal">choices: pass, block, reset</span></li>
            <li> <span class="li-head">exempt_ip</span> - Exempted IP. <span class="li-normal">type: list</span></li>
                <ul class="ul-self">
                <li> <span class="li-head">dst_ip</span> - Destination IP address and netmask. <span class="li-normal">type: str</span></li>
                <li> <span class="li-head">id</span> - Exempt IP ID. <span class="li-normal">type: int</span> <span class="li-required">required: True</span></li>
                <li> <span class="li-head">src_ip</span> - Source IP address and netmask. <span class="li-normal">type: str</span></li>
                </ul>
            <li> <span class="li-head">log</span> - Enable/disable logging. <span class="li-normal">type: str</span> <span class="li-normal">choices: disable, enable</span></li>
            <li> <span class="li-head">log_packet</span> - Enable/disable packet logging. <span class="li-normal">type: str</span> <span class="li-normal">choices: disable, enable</span></li>
            <li> <span class="li-head">quarantine</span> - Quarantine IP or interface. <span class="li-normal">type: str</span> <span class="li-normal">choices: none, attacker</span></li>
            <li> <span class="li-head">quarantine_expiry</span> - Duration of quarantine in minute. <span class="li-normal">type: int</span></li>
            <li> <span class="li-head">quarantine_log</span> - Enable/disable logging of selected quarantine. <span class="li-normal">type: str</span> <span class="li-normal">choices: disable, enable</span></li>
            <li> <span class="li-head">rule_id</span> - Override rule ID. <span class="li-normal">type: int</span></li>
            <li> <span class="li-head">status</span> - Enable/disable status of override rule. <span class="li-normal">type: str</span> <span class="li-normal">choices: disable, enable</span></li>
            </ul>
        <li> <span class="li-head">replacemsg_group</span> - Replacement message group. Source system.replacemsg-group.name. <span class="li-normal">type: str</span></li>
        <li> <span class="li-head">scan_botnet_connections</span> - Block or monitor connections to Botnet servers, or disable Botnet scanning. <span class="li-normal">type: str</span> <span class="li-normal">choices: disable, block, monitor</span></li>
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
      - name: Configure IPS sensor.
        fortios_ips_sensor:
          vdom:  "{{ vdom }}"
          state: "present"
          access_token: "<your_own_value>"
          ips_sensor:
            block_malicious_url: "disable"
            comment: "Comment."
            entries:
             -
                action: "pass"
                application: "<your_own_value>"
                exempt_ip:
                 -
                    dst_ip: "<your_own_value>"
                    id:  "10"
                    src_ip: "<your_own_value>"
                id:  "12"
                location: "<your_own_value>"
                log: "disable"
                log_attack_context: "disable"
                log_packet: "disable"
                os: "<your_own_value>"
                protocol: "<your_own_value>"
                quarantine: "none"
                quarantine_expiry: "<your_own_value>"
                quarantine_log: "disable"
                rate_count: "22"
                rate_duration: "23"
                rate_mode: "periodical"
                rate_track: "none"
                rule:
                 -
                    id:  "27"
                severity: "<your_own_value>"
                status: "disable"
            extended_log: "enable"
            filter:
             -
                action: "pass"
                application: "<your_own_value>"
                location: "<your_own_value>"
                log: "disable"
                log_packet: "disable"
                name: "default_name_37"
                os: "<your_own_value>"
                protocol: "<your_own_value>"
                quarantine: "none"
                quarantine_expiry: "41"
                quarantine_log: "disable"
                severity: "<your_own_value>"
                status: "disable"
            name: "default_name_45"
            override:
             -
                action: "pass"
                exempt_ip:
                 -
                    dst_ip: "<your_own_value>"
                    id:  "50"
                    src_ip: "<your_own_value>"
                log: "disable"
                log_packet: "disable"
                quarantine: "none"
                quarantine_expiry: "55"
                quarantine_log: "disable"
                rule_id: "57"
                status: "disable"
            replacemsg_group: "<your_own_value> (source system.replacemsg-group.name)"
            scan_botnet_connections: "disable"
    


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
