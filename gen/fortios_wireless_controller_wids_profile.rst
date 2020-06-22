:source: fortios_wireless_controller_wids_profile.py

:orphan:

.. fortios_wireless_controller_wids_profile:

fortios_wireless_controller_wids_profile -- Configure wireless intrusion detection system (WIDS) profiles in Fortinet's FortiOS and FortiGate.
++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++

.. versionadded:: 2.8

.. contents::
   :local:
   :depth: 1


Synopsis
--------
- This module is able to configure a FortiGate or FortiOS (FOS) device by allowing the user to set and modify wireless_controller feature and wids_profile category. Examples include all parameters and values need to be adjusted to datasources before usage. Tested with FOS v6.2.0



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
    <li> <span class="li-head">state</span> - Indicates whether to create or remove the object. This attribute was present already in previous version in a deeper level. It has been moved out to this outer level. <span class="li-normal">type: str</span> <span class="li-required">required: False</span> <span class="li-normal">choices: present, absent</span></li>
    <li> <span class="li-head">wireless_controller_wids_profile</span> - Configure wireless intrusion detection system (WIDS) profiles. <span class="li-normal">type: dict</span></li>
        <ul class="ul-self">
        <li> <span class="li-head">state</span> - B(Deprecated) <span class="li-normal">type: str</span> <span class="li-required">required: False</span> <span class="li-normal">choices: present, absent</span></li>
        <li> <span class="li-head">ap_auto_suppress</span> - Enable/disable on-wire rogue AP auto-suppression . <span class="li-normal">type: str</span> <span class="li-normal">choices: enable, disable</span></li>
        <li> <span class="li-head">ap_bgscan_disable_day</span> - Optionally turn off scanning for one or more days of the week. Separate the days with a space. By default, no days are set. <span class="li-normal">type: str</span> <span class="li-normal">choices: sunday, monday, tuesday, wednesday, thursday, friday, saturday</span></li>
        <li> <span class="li-head">ap_bgscan_disable_end</span> - End time, using a 24-hour clock in the format of hh:mm, for disabling background scanning . <span class="li-normal">type: str</span></li>
        <li> <span class="li-head">ap_bgscan_disable_start</span> - Start time, using a 24-hour clock in the format of hh:mm, for disabling background scanning . <span class="li-normal">type: str</span></li>
        <li> <span class="li-head">ap_bgscan_duration</span> - Listening time on a scanning channel (10 - 1000 msec). <span class="li-normal">type: int</span></li>
        <li> <span class="li-head">ap_bgscan_idle</span> - Waiting time for channel inactivity before scanning this channel (0 - 1000 msec). <span class="li-normal">type: int</span></li>
        <li> <span class="li-head">ap_bgscan_intv</span> - Period of time between scanning two channels (1 - 600 sec). <span class="li-normal">type: int</span></li>
        <li> <span class="li-head">ap_bgscan_period</span> - Period of time between background scans (60 - 3600 sec). <span class="li-normal">type: int</span></li>
        <li> <span class="li-head">ap_bgscan_report_intv</span> - Period of time between background scan reports (15 - 600 sec). <span class="li-normal">type: int</span></li>
        <li> <span class="li-head">ap_fgscan_report_intv</span> - Period of time between foreground scan reports (15 - 600 sec). <span class="li-normal">type: int</span></li>
        <li> <span class="li-head">ap_scan</span> - Enable/disable rogue AP detection. <span class="li-normal">type: str</span> <span class="li-normal">choices: disable, enable</span></li>
        <li> <span class="li-head">ap_scan_passive</span> - Enable/disable passive scanning. Enable means do not send probe request on any channels . <span class="li-normal">type: str</span> <span class="li-normal">choices: enable, disable</span></li>
        <li> <span class="li-head">asleap_attack</span> - Enable/disable asleap attack detection . <span class="li-normal">type: str</span> <span class="li-normal">choices: enable, disable</span></li>
        <li> <span class="li-head">assoc_flood_thresh</span> - The threshold value for association frame flooding. <span class="li-normal">type: int</span></li>
        <li> <span class="li-head">assoc_flood_time</span> - Number of seconds after which a station is considered not connected. <span class="li-normal">type: int</span></li>
        <li> <span class="li-head">assoc_frame_flood</span> - Enable/disable association frame flooding detection . <span class="li-normal">type: str</span> <span class="li-normal">choices: enable, disable</span></li>
        <li> <span class="li-head">auth_flood_thresh</span> - The threshold value for authentication frame flooding. <span class="li-normal">type: int</span></li>
        <li> <span class="li-head">auth_flood_time</span> - Number of seconds after which a station is considered not connected. <span class="li-normal">type: int</span></li>
        <li> <span class="li-head">auth_frame_flood</span> - Enable/disable authentication frame flooding detection . <span class="li-normal">type: str</span> <span class="li-normal">choices: enable, disable</span></li>
        <li> <span class="li-head">comment</span> - Comment. <span class="li-normal">type: str</span></li>
        <li> <span class="li-head">deauth_broadcast</span> - Enable/disable broadcasting de-authentication detection . <span class="li-normal">type: str</span> <span class="li-normal">choices: enable, disable</span></li>
        <li> <span class="li-head">deauth_unknown_src_thresh</span> - Threshold value per second to deauth unknown src for DoS attack (0: no limit). <span class="li-normal">type: int</span></li>
        <li> <span class="li-head">eapol_fail_flood</span> - Enable/disable EAPOL-Failure flooding (to AP) detection . <span class="li-normal">type: str</span> <span class="li-normal">choices: enable, disable</span></li>
        <li> <span class="li-head">eapol_fail_intv</span> - The detection interval for EAPOL-Failure flooding (1 - 3600 sec). <span class="li-normal">type: int</span></li>
        <li> <span class="li-head">eapol_fail_thresh</span> - The threshold value for EAPOL-Failure flooding in specified interval. <span class="li-normal">type: int</span></li>
        <li> <span class="li-head">eapol_logoff_flood</span> - Enable/disable EAPOL-Logoff flooding (to AP) detection . <span class="li-normal">type: str</span> <span class="li-normal">choices: enable, disable</span></li>
        <li> <span class="li-head">eapol_logoff_intv</span> - The detection interval for EAPOL-Logoff flooding (1 - 3600 sec). <span class="li-normal">type: int</span></li>
        <li> <span class="li-head">eapol_logoff_thresh</span> - The threshold value for EAPOL-Logoff flooding in specified interval. <span class="li-normal">type: int</span></li>
        <li> <span class="li-head">eapol_pre_fail_flood</span> - Enable/disable premature EAPOL-Failure flooding (to STA) detection . <span class="li-normal">type: str</span> <span class="li-normal">choices: enable, disable</span></li>
        <li> <span class="li-head">eapol_pre_fail_intv</span> - The detection interval for premature EAPOL-Failure flooding (1 - 3600 sec). <span class="li-normal">type: int</span></li>
        <li> <span class="li-head">eapol_pre_fail_thresh</span> - The threshold value for premature EAPOL-Failure flooding in specified interval. <span class="li-normal">type: int</span></li>
        <li> <span class="li-head">eapol_pre_succ_flood</span> - Enable/disable premature EAPOL-Success flooding (to STA) detection . <span class="li-normal">type: str</span> <span class="li-normal">choices: enable, disable</span></li>
        <li> <span class="li-head">eapol_pre_succ_intv</span> - The detection interval for premature EAPOL-Success flooding (1 - 3600 sec). <span class="li-normal">type: int</span></li>
        <li> <span class="li-head">eapol_pre_succ_thresh</span> - The threshold value for premature EAPOL-Success flooding in specified interval. <span class="li-normal">type: int</span></li>
        <li> <span class="li-head">eapol_start_flood</span> - Enable/disable EAPOL-Start flooding (to AP) detection . <span class="li-normal">type: str</span> <span class="li-normal">choices: enable, disable</span></li>
        <li> <span class="li-head">eapol_start_intv</span> - The detection interval for EAPOL-Start flooding (1 - 3600 sec). <span class="li-normal">type: int</span></li>
        <li> <span class="li-head">eapol_start_thresh</span> - The threshold value for EAPOL-Start flooding in specified interval. <span class="li-normal">type: int</span></li>
        <li> <span class="li-head">eapol_succ_flood</span> - Enable/disable EAPOL-Success flooding (to AP) detection . <span class="li-normal">type: str</span> <span class="li-normal">choices: enable, disable</span></li>
        <li> <span class="li-head">eapol_succ_intv</span> - The detection interval for EAPOL-Success flooding (1 - 3600 sec). <span class="li-normal">type: int</span></li>
        <li> <span class="li-head">eapol_succ_thresh</span> - The threshold value for EAPOL-Success flooding in specified interval. <span class="li-normal">type: int</span></li>
        <li> <span class="li-head">invalid_mac_oui</span> - Enable/disable invalid MAC OUI detection. <span class="li-normal">type: str</span> <span class="li-normal">choices: enable, disable</span></li>
        <li> <span class="li-head">long_duration_attack</span> - Enable/disable long duration attack detection based on user configured threshold . <span class="li-normal">type: str</span> <span class="li-normal">choices: enable, disable</span></li>
        <li> <span class="li-head">long_duration_thresh</span> - Threshold value for long duration attack detection (1000 - 32767 usec). <span class="li-normal">type: int</span></li>
        <li> <span class="li-head">name</span> - WIDS profile name. <span class="li-normal">type: str</span> <span class="li-required">required: True</span></li>
        <li> <span class="li-head">null_ssid_probe_resp</span> - Enable/disable null SSID probe response detection . <span class="li-normal">type: str</span> <span class="li-normal">choices: enable, disable</span></li>
        <li> <span class="li-head">sensor_mode</span> - Scan nearby WiFi stations . <span class="li-normal">type: str</span> <span class="li-normal">choices: disable, foreign, both</span></li>
        <li> <span class="li-head">spoofed_deauth</span> - Enable/disable spoofed de-authentication attack detection . <span class="li-normal">type: str</span> <span class="li-normal">choices: enable, disable</span></li>
        <li> <span class="li-head">weak_wep_iv</span> - Enable/disable weak WEP IV (Initialization Vector) detection . <span class="li-normal">type: str</span> <span class="li-normal">choices: enable, disable</span></li>
        <li> <span class="li-head">wireless_bridge</span> - Enable/disable wireless bridge detection . <span class="li-normal">type: str</span> <span class="li-normal">choices: enable, disable</span></li>
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
      - name: Configure wireless intrusion detection system (WIDS) profiles.
        fortios_wireless_controller_wids_profile:
          vdom:  "{{ vdom }}"
          state: "present"
          wireless_controller_wids_profile:
            ap_auto_suppress: "enable"
            ap_bgscan_disable_day: "sunday"
            ap_bgscan_disable_end: "<your_own_value>"
            ap_bgscan_disable_start: "<your_own_value>"
            ap_bgscan_duration: "7"
            ap_bgscan_idle: "8"
            ap_bgscan_intv: "9"
            ap_bgscan_period: "10"
            ap_bgscan_report_intv: "11"
            ap_fgscan_report_intv: "12"
            ap_scan: "disable"
            ap_scan_passive: "enable"
            asleap_attack: "enable"
            assoc_flood_thresh: "16"
            assoc_flood_time: "17"
            assoc_frame_flood: "enable"
            auth_flood_thresh: "19"
            auth_flood_time: "20"
            auth_frame_flood: "enable"
            comment: "Comment."
            deauth_broadcast: "enable"
            deauth_unknown_src_thresh: "24"
            eapol_fail_flood: "enable"
            eapol_fail_intv: "26"
            eapol_fail_thresh: "27"
            eapol_logoff_flood: "enable"
            eapol_logoff_intv: "29"
            eapol_logoff_thresh: "30"
            eapol_pre_fail_flood: "enable"
            eapol_pre_fail_intv: "32"
            eapol_pre_fail_thresh: "33"
            eapol_pre_succ_flood: "enable"
            eapol_pre_succ_intv: "35"
            eapol_pre_succ_thresh: "36"
            eapol_start_flood: "enable"
            eapol_start_intv: "38"
            eapol_start_thresh: "39"
            eapol_succ_flood: "enable"
            eapol_succ_intv: "41"
            eapol_succ_thresh: "42"
            invalid_mac_oui: "enable"
            long_duration_attack: "enable"
            long_duration_thresh: "45"
            name: "default_name_46"
            null_ssid_probe_resp: "enable"
            sensor_mode: "disable"
            spoofed_deauth: "enable"
            weak_wep_iv: "enable"
            wireless_bridge: "enable"


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
