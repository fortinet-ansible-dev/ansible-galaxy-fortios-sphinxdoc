:source: fortios_log_threat_weight.py

:orphan:

.. fortios_log_threat_weight:

fortios_log_threat_weight -- Configure threat weight settings in Fortinet's FortiOS and FortiGate.
++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++

.. versionadded:: 2.8

.. contents::
   :local:
   :depth: 1


Synopsis
--------
- This module is able to configure a FortiGate or FortiOS (FOS) device by allowing the user to set and modify log feature and threat_weight category. Examples include all parameters and values need to be adjusted to datasources before usage. Tested with FOS v6.0.5



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
    <li> <span class="li-head">log_threat_weight</span> - Configure threat weight settings. <span class="li-normal">type: dict</span></li>
        <ul class="ul-self">
        <li> <span class="li-head">application</span> - Application-control threat weight settings. <span class="li-normal">type: list</span></li>
            <ul class="ul-self">
            <li> <span class="li-head">category</span> - Application category. <span class="li-normal">type: int</span></li>
            <li> <span class="li-head">id</span> - Entry ID. <span class="li-normal">type: int</span> <span class="li-required">required: True</span></li>
            <li> <span class="li-head">level</span> - Threat weight score for Application events. <span class="li-normal">type: str</span> <span class="li-normal">choices: disable, low, medium, high, critical</span></li>
            </ul>
        <li> <span class="li-head">blocked_connection</span> - Threat weight score for blocked connections. <span class="li-normal">type: str</span> <span class="li-normal">choices: disable, low, medium, high, critical</span></li>
        <li> <span class="li-head">failed_connection</span> - Threat weight score for failed connections. <span class="li-normal">type: str</span> <span class="li-normal">choices: disable, low, medium, high, critical</span></li>
        <li> <span class="li-head">geolocation</span> - Geolocation-based threat weight settings. <span class="li-normal">type: list</span></li>
            <ul class="ul-self">
            <li> <span class="li-head">country</span> - Country code. <span class="li-normal">type: str</span></li>
            <li> <span class="li-head">id</span> - Entry ID. <span class="li-normal">type: int</span> <span class="li-required">required: True</span></li>
            <li> <span class="li-head">level</span> - Threat weight score for Geolocation-based events. <span class="li-normal">type: str</span> <span class="li-normal">choices: disable, low, medium, high, critical</span></li>
            </ul>
        <li> <span class="li-head">ips</span> - IPS threat weight settings. <span class="li-normal">type: dict</span></li>
            <ul class="ul-self">
            <li> <span class="li-head">critical_severity</span> - Threat weight score for IPS critical severity events. <span class="li-normal">type: str</span> <span class="li-normal">choices: disable, low, medium, high, critical</span></li>
            <li> <span class="li-head">high_severity</span> - Threat weight score for IPS high severity events. <span class="li-normal">type: str</span> <span class="li-normal">choices: disable, low, medium, high, critical</span></li>
            <li> <span class="li-head">info_severity</span> - Threat weight score for IPS info severity events. <span class="li-normal">type: str</span> <span class="li-normal">choices: disable, low, medium, high, critical</span></li>
            <li> <span class="li-head">low_severity</span> - Threat weight score for IPS low severity events. <span class="li-normal">type: str</span> <span class="li-normal">choices: disable, low, medium, high, critical</span></li>
            <li> <span class="li-head">medium_severity</span> - Threat weight score for IPS medium severity events. <span class="li-normal">type: str</span> <span class="li-normal">choices: disable, low, medium, high, critical</span></li>
            </ul>
        <li> <span class="li-head">level</span> - Score mapping for threat weight levels. <span class="li-normal">type: dict</span></li>
            <ul class="ul-self">
            <li> <span class="li-head">critical</span> - Critical level score value (1 - 100). <span class="li-normal">type: int</span></li>
            <li> <span class="li-head">high</span> - High level score value (1 - 100). <span class="li-normal">type: int</span></li>
            <li> <span class="li-head">low</span> - Low level score value (1 - 100). <span class="li-normal">type: int</span></li>
            <li> <span class="li-head">medium</span> - Medium level score value (1 - 100). <span class="li-normal">type: int</span></li>
            </ul>
        <li> <span class="li-head">malware</span> - Anti-virus malware threat weight settings. <span class="li-normal">type: dict</span></li>
            <ul class="ul-self">
            <li> <span class="li-head">botnet_connection</span> - Threat weight score for detected botnet connections. <span class="li-normal">type: str</span> <span class="li-normal">choices: disable, low, medium, high, critical</span></li>
            <li> <span class="li-head">command_blocked</span> - Threat weight score for blocked command detected. <span class="li-normal">type: str</span> <span class="li-normal">choices: disable, low, medium, high, critical</span></li>
            <li> <span class="li-head">content_disarm</span> - Threat weight score for virus (content disarm) detected. <span class="li-normal">type: str</span> <span class="li-normal">choices: disable, low, medium, high, critical</span></li>
            <li> <span class="li-head">mimefragmented</span> - Threat weight score for mimefragmented detected. <span class="li-normal">type: str</span> <span class="li-normal">choices: disable, low, medium, high, critical</span></li>
            <li> <span class="li-head">oversized</span> - Threat weight score for oversized file detected. <span class="li-normal">type: str</span> <span class="li-normal">choices: disable, low, medium, high, critical</span></li>
            <li> <span class="li-head">switch_proto</span> - Threat weight score for switch proto detected. <span class="li-normal">type: str</span> <span class="li-normal">choices: disable, low, medium, high, critical</span></li>
            <li> <span class="li-head">virus_blocked</span> - Threat weight score for virus (blocked) detected. <span class="li-normal">type: str</span> <span class="li-normal">choices: disable, low, medium, high, critical</span></li>
            <li> <span class="li-head">virus_file_type_executable</span> - Threat weight score for virus (filetype executable) detected. <span class="li-normal">type: str</span> <span class="li-normal">choices: disable, low, medium, high, critical</span></li>
            <li> <span class="li-head">virus_infected</span> - Threat weight score for virus (infected) detected. <span class="li-normal">type: str</span> <span class="li-normal">choices: disable, low, medium, high, critical</span></li>
            <li> <span class="li-head">virus_outbreak_prevention</span> - Threat weight score for virus (outbreak prevention) event. <span class="li-normal">type: str</span> <span class="li-normal">choices: disable, low, medium, high, critical</span></li>
            <li> <span class="li-head">virus_scan_error</span> - Threat weight score for virus (scan error) detected. <span class="li-normal">type: str</span> <span class="li-normal">choices: disable, low, medium, high, critical</span></li>
            </ul>
        <li> <span class="li-head">status</span> - Enable/disable the threat weight feature. <span class="li-normal">type: str</span> <span class="li-normal">choices: enable, disable</span></li>
        <li> <span class="li-head">url_block_detected</span> - Threat weight score for URL blocking. <span class="li-normal">type: str</span> <span class="li-normal">choices: disable, low, medium, high, critical</span></li>
        <li> <span class="li-head">web</span> - Web filtering threat weight settings. <span class="li-normal">type: list</span></li>
            <ul class="ul-self">
            <li> <span class="li-head">category</span> - Threat weight score for web category filtering matches. <span class="li-normal">type: int</span></li>
            <li> <span class="li-head">id</span> - Entry ID. <span class="li-normal">type: int</span> <span class="li-required">required: True</span></li>
            <li> <span class="li-head">level</span> - Threat weight score for web category filtering matches. <span class="li-normal">type: str</span> <span class="li-normal">choices: disable, low, medium, high, critical</span></li>
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
      - name: Configure threat weight settings.
        fortios_log_threat_weight:
          vdom:  "{{ vdom }}"
          log_threat_weight:
            application:
             -
                category: "4"
                id:  "5"
                level: "disable"
            blocked_connection: "disable"
            failed_connection: "disable"
            geolocation:
             -
                country: "<your_own_value>"
                id:  "11"
                level: "disable"
            ips:
                critical_severity: "disable"
                high_severity: "disable"
                info_severity: "disable"
                low_severity: "disable"
                medium_severity: "disable"
            level:
                critical: "20"
                high: "21"
                low: "22"
                medium: "23"
            malware:
                botnet_connection: "disable"
                command_blocked: "disable"
                content_disarm: "disable"
                mimefragmented: "disable"
                oversized: "disable"
                switch_proto: "disable"
                virus_blocked: "disable"
                virus_file_type_executable: "disable"
                virus_infected: "disable"
                virus_outbreak_prevention: "disable"
                virus_scan_error: "disable"
            status: "enable"
            url_block_detected: "disable"
            web:
             -
                category: "39"
                id:  "40"
                level: "disable"


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
