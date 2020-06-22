:source: fortios_system_automation_trigger.py

:orphan:

.. fortios_system_automation_trigger:

fortios_system_automation_trigger -- Trigger for automation stitches in Fortinet's FortiOS and FortiGate.
+++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++

.. versionadded:: 2.9

.. contents::
   :local:
   :depth: 1


Synopsis
--------
- This module is able to configure a FortiGate or FortiOS (FOS) device by allowing the user to set and modify system feature and automation_trigger category. Examples include all parameters and values need to be adjusted to datasources before usage. Tested with FOS v6.4.0



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
    <li> <span class="li-head">state</span> - Indicates whether to create or remove the object. <span class="li-normal">type: str</span> <span class="li-required">required: True</span> <span class="li-normal">choices: present, absent</span></li>
    <li> <span class="li-head">system_automation_trigger</span> - Trigger for automation stitches. <span class="li-normal">type: dict</span></li>
        <ul class="ul-self">
        <li> <span class="li-head">event_type</span> - Event type. <span class="li-normal">type: str</span> <span class="li-normal">choices: ioc, event-log, reboot, low-memory, high-cpu, license-near-expiry, ha-failover, config-change, security-rating-summary, virus-ips-db-updated, faz-event, incoming-webhook</span></li>
        <li> <span class="li-head">faz_event_name</span> - FortiAnalyzer event handler name. <span class="li-normal">type: str</span></li>
        <li> <span class="li-head">faz_event_severity</span> - FortiAnalyzer event severity. <span class="li-normal">type: str</span></li>
        <li> <span class="li-head">faz_event_tags</span> - FortiAnalyzer event tags. <span class="li-normal">type: str</span></li>
        <li> <span class="li-head">fields</span> - Customized trigger field settings. <span class="li-normal">type: list</span></li>
            <ul class="ul-self">
            <li> <span class="li-head">id</span> - Entry ID. <span class="li-normal">type: int</span> <span class="li-required">required: True</span></li>
            <li> <span class="li-head">name</span> - Name. <span class="li-normal">type: str</span></li>
            <li> <span class="li-head">value</span> - Value. <span class="li-normal">type: str</span></li>
            </ul>
        <li> <span class="li-head">ioc_level</span> - IOC threat level. <span class="li-normal">type: str</span> <span class="li-normal">choices: medium, high</span></li>
        <li> <span class="li-head">license_type</span> - License type. <span class="li-normal">type: str</span> <span class="li-normal">choices: forticare-support, fortiguard-webfilter, fortiguard-antispam, fortiguard-antivirus, fortiguard-ips, fortiguard-management, forticloud, any</span></li>
        <li> <span class="li-head">logid</span> - Log ID to trigger event. <span class="li-normal">type: int</span></li>
        <li> <span class="li-head">name</span> - Name. <span class="li-normal">type: str</span> <span class="li-required">required: True</span></li>
        <li> <span class="li-head">report_type</span> - Security Rating report. <span class="li-normal">type: str</span> <span class="li-normal">choices: PostureReport, CoverageReport, OptimizationReport</span></li>
        <li> <span class="li-head">trigger_day</span> - Day within a month to trigger. <span class="li-normal">type: int</span></li>
        <li> <span class="li-head">trigger_frequency</span> - Scheduled trigger frequency . <span class="li-normal">type: str</span> <span class="li-normal">choices: hourly, daily, weekly, monthly</span></li>
        <li> <span class="li-head">trigger_hour</span> - Hour of the day on which to trigger (0 - 23). <span class="li-normal">type: int</span></li>
        <li> <span class="li-head">trigger_minute</span> - Minute of the hour on which to trigger (0 - 59). <span class="li-normal">type: int</span></li>
        <li> <span class="li-head">trigger_type</span> - Trigger type. <span class="li-normal">type: str</span> <span class="li-normal">choices: event-based, scheduled</span></li>
        <li> <span class="li-head">trigger_weekday</span> - Day of week for trigger. <span class="li-normal">type: str</span> <span class="li-normal">choices: sunday, monday, tuesday, wednesday, thursday, friday, saturday</span></li>
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
      - name: Trigger for automation stitches.
        fortios_system_automation_trigger:
          vdom:  "{{ vdom }}"
          state: "present"
          system_automation_trigger:
            event_type: "ioc"
            faz_event_name: "<your_own_value>"
            faz_event_severity: "<your_own_value>"
            faz_event_tags: "<your_own_value>"
            fields:
             -
                id:  "8"
                name: "default_name_9"
                value: "<your_own_value>"
            ioc_level: "medium"
            license_type: "forticare-support"
            logid: "13"
            name: "default_name_14"
            report_type: "PostureReport"
            trigger_day: "16"
            trigger_frequency: "hourly"
            trigger_hour: "18"
            trigger_minute: "19"
            trigger_type: "event-based"
            trigger_weekday: "sunday"


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
