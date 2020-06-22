:source: fortios_wireless_controller_log.py

:orphan:

.. fortios_wireless_controller_log:

fortios_wireless_controller_log -- Configure wireless controller event log filters in Fortinet's FortiOS and FortiGate.
+++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++

.. versionadded:: 2.10

.. contents::
   :local:
   :depth: 1


Synopsis
--------
- This module is able to configure a FortiGate or FortiOS (FOS) device by allowing the user to set and modify wireless_controller feature and log category. Examples include all parameters and values need to be adjusted to datasources before usage. Tested with FOS v6.2.0



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
    <li> <span class="li-head">wireless_controller_log</span> - Configure wireless controller event log filters. <span class="li-normal">type: dict</span></li>
        <ul class="ul-self">
        <li> <span class="li-head">addrgrp_log</span> - Lowest severity level to log address group message. <span class="li-normal">type: str</span> <span class="li-normal">choices: emergency, alert, critical, error, warning, notification, information, debug</span></li>
        <li> <span class="li-head">ble_log</span> - Lowest severity level to log BLE detection message. <span class="li-normal">type: str</span> <span class="li-normal">choices: emergency, alert, critical, error, warning, notification, information, debug</span></li>
        <li> <span class="li-head">clb_log</span> - Lowest severity level to log client load balancing message. <span class="li-normal">type: str</span> <span class="li-normal">choices: emergency, alert, critical, error, warning, notification, information, debug</span></li>
        <li> <span class="li-head">dhcp_starv_log</span> - Lowest severity level to log DHCP starvation event message. <span class="li-normal">type: str</span> <span class="li-normal">choices: emergency, alert, critical, error, warning, notification, information, debug</span></li>
        <li> <span class="li-head">led_sched_log</span> - Lowest severity level to log LED schedule event message. <span class="li-normal">type: str</span> <span class="li-normal">choices: emergency, alert, critical, error, warning, notification, information, debug</span></li>
        <li> <span class="li-head">radio_event_log</span> - Lowest severity level to log radio event message. <span class="li-normal">type: str</span> <span class="li-normal">choices: emergency, alert, critical, error, warning, notification, information, debug</span></li>
        <li> <span class="li-head">rogue_event_log</span> - Lowest severity level to log rogue AP event message. <span class="li-normal">type: str</span> <span class="li-normal">choices: emergency, alert, critical, error, warning, notification, information, debug</span></li>
        <li> <span class="li-head">sta_event_log</span> - Lowest severity level to log station event message. <span class="li-normal">type: str</span> <span class="li-normal">choices: emergency, alert, critical, error, warning, notification, information, debug</span></li>
        <li> <span class="li-head">sta_locate_log</span> - Lowest severity level to log station locate message. <span class="li-normal">type: str</span> <span class="li-normal">choices: emergency, alert, critical, error, warning, notification, information, debug</span></li>
        <li> <span class="li-head">status</span> - Enable/disable wireless event logging. <span class="li-normal">type: str</span> <span class="li-normal">choices: enable, disable</span></li>
        <li> <span class="li-head">wids_log</span> - Lowest severity level to log WIDS message. <span class="li-normal">type: str</span> <span class="li-normal">choices: emergency, alert, critical, error, warning, notification, information, debug</span></li>
        <li> <span class="li-head">wtp_event_log</span> - Lowest severity level to log WTP event message. <span class="li-normal">type: str</span> <span class="li-normal">choices: emergency, alert, critical, error, warning, notification, information, debug</span></li>
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
      - name: Configure wireless controller event log filters.
        fortios_wireless_controller_log:
          vdom:  "{{ vdom }}"
          wireless_controller_log:
            addrgrp_log: "emergency"
            ble_log: "emergency"
            clb_log: "emergency"
            dhcp_starv_log: "emergency"
            led_sched_log: "emergency"
            radio_event_log: "emergency"
            rogue_event_log: "emergency"
            sta_event_log: "emergency"
            sta_locate_log: "emergency"
            status: "enable"
            wids_log: "emergency"
            wtp_event_log: "emergency"


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