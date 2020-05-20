:source: fortios_wireless_controller_timers.py

:orphan:

.. fortios_wireless_controller_timers:

fortios_wireless_controller_timers -- Configure CAPWAP timers in Fortinet's FortiOS and FortiGate.
++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++

.. versionadded:: 2.9

.. contents::
   :local:
   :depth: 1


Synopsis
--------
- This module is able to configure a FortiGate or FortiOS (FOS) device by allowing the user to set and modify wireless_controller feature and timers category. Examples include all parameters and values need to be adjusted to datasources before usage. Tested with FOS v6.0.0



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
    <li> <span class="li-head">wireless_controller_timers</span> - Configure CAPWAP timers. <span class="li-normal">type: dict</span></li>
        <ul class="ul-self">
        <li> <span class="li-head">ble_scan_report_intv</span> - Time between running Bluetooth Low Energy (BLE) reports (10 - 3600 sec). <span class="li-normal">type: int</span></li>
        <li> <span class="li-head">client_idle_timeout</span> - Time after which a client is considered idle and times out (20 - 3600 sec). <span class="li-normal">type: int</span></li>
        <li> <span class="li-head">darrp_day</span> - Weekday on which to run DARRP optimization. <span class="li-normal">type: str</span> <span class="li-normal">choices: sunday, monday, tuesday, wednesday, thursday, friday, saturday</span></li>
        <li> <span class="li-head">darrp_optimize</span> - Time for running Dynamic Automatic Radio Resource Provisioning (DARRP) optimizations (0 - 86400 sec). <span class="li-normal">type: int</span></li>
        <li> <span class="li-head">darrp_time</span> - Time at which DARRP optimizations run (you can add up to 8 times). <span class="li-normal">type: list</span></li>
            <ul class="ul-self">
            <li> <span class="li-head">time</span> - Time. <span class="li-normal">type: str</span> <span class="li-required">required: True</span></li>
            </ul>
        <li> <span class="li-head">discovery_interval</span> - Time between discovery requests (2 - 180 sec). <span class="li-normal">type: int</span></li>
        <li> <span class="li-head">echo_interval</span> - Time between echo requests sent by the managed WTP, AP, or FortiAP (1 - 255 sec). <span class="li-normal">type: int</span></li>
        <li> <span class="li-head">fake_ap_log</span> - Time between recording logs about fake APs if periodic fake AP logging is configured (0 - 1440 min). <span class="li-normal">type: int</span></li>
        <li> <span class="li-head">ipsec_intf_cleanup</span> - Time period to keep IPsec VPN interfaces up after WTP sessions are disconnected (30 - 3600 sec). <span class="li-normal">type: int</span></li>
        <li> <span class="li-head">radio_stats_interval</span> - Time between running radio reports (1 - 255 sec). <span class="li-normal">type: int</span></li>
        <li> <span class="li-head">rogue_ap_log</span> - Time between logging rogue AP messages if periodic rogue AP logging is configured (0 - 1440 min). <span class="li-normal">type: int</span></li>
        <li> <span class="li-head">sta_capability_interval</span> - Time between running station capability reports (1 - 255 sec). <span class="li-normal">type: int</span></li>
        <li> <span class="li-head">sta_locate_timer</span> - Time between running client presence flushes to remove clients that are listed but no longer present (0 - 86400 sec). <span class="li-normal">type: int</span></li>
        <li> <span class="li-head">sta_stats_interval</span> - Time between running client (station) reports (1 - 255 sec). <span class="li-normal">type: int</span></li>
        <li> <span class="li-head">vap_stats_interval</span> - Time between running Virtual Access Point (VAP) reports (1 - 255 sec). <span class="li-normal">type: int</span></li>
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
      - name: Configure CAPWAP timers.
        fortios_wireless_controller_timers:
          vdom:  "{{ vdom }}"
          wireless_controller_timers:
            ble_scan_report_intv: "3"
            client_idle_timeout: "4"
            darrp_day: "sunday"
            darrp_optimize: "6"
            darrp_time:
             -
                time: "<your_own_value>"
            discovery_interval: "9"
            echo_interval: "10"
            fake_ap_log: "11"
            ipsec_intf_cleanup: "12"
            radio_stats_interval: "13"
            rogue_ap_log: "14"
            sta_capability_interval: "15"
            sta_locate_timer: "16"
            sta_stats_interval: "17"
            vap_stats_interval: "18"


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
