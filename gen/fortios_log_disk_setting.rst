:source: fortios_log_disk_setting.py

:orphan:

.. fortios_log_disk_setting:

fortios_log_disk_setting -- Settings for local disk logging in Fortinet's FortiOS and FortiGate.
++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++

.. versionadded:: 2.8

.. contents::
   :local:
   :depth: 1


Synopsis
--------
- This module is able to configure a FortiGate or FortiOS (FOS) device by allowing the user to set and modify log_disk feature and setting category. Examples include all parameters and values need to be adjusted to datasources before usage. Tested with FOS v6.0.5



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
    <li> <span class="li-head">log_disk_setting</span> - Settings for local disk logging. <span class="li-normal">type: dict</span></li>
        <ul class="ul-self">
        <li> <span class="li-head">diskfull</span> - Action to take when disk is full. The system can overwrite the oldest log messages or stop logging when the disk is full . <span class="li-normal">type: str</span> <span class="li-normal">choices: overwrite, nolog</span></li>
        <li> <span class="li-head">dlp_archive_quota</span> - DLP archive quota (MB). <span class="li-normal">type: int</span></li>
        <li> <span class="li-head">full_final_warning_threshold</span> - Log full final warning threshold as a percent (3 - 100). <span class="li-normal">type: int</span></li>
        <li> <span class="li-head">full_first_warning_threshold</span> - Log full first warning threshold as a percent (1 - 98). <span class="li-normal">type: int</span></li>
        <li> <span class="li-head">full_second_warning_threshold</span> - Log full second warning threshold as a percent (2 - 99). <span class="li-normal">type: int</span></li>
        <li> <span class="li-head">ips_archive</span> - Enable/disable IPS packet archiving to the local disk. <span class="li-normal">type: str</span> <span class="li-normal">choices: enable, disable</span></li>
        <li> <span class="li-head">log_quota</span> - Disk log quota (MB). <span class="li-normal">type: int</span></li>
        <li> <span class="li-head">max_log_file_size</span> - Maximum log file size before rolling (1 - 100 Mbytes). <span class="li-normal">type: int</span></li>
        <li> <span class="li-head">max_policy_packet_capture_size</span> - Maximum size of policy sniffer in MB (0 means unlimited). <span class="li-normal">type: int</span></li>
        <li> <span class="li-head">maximum_log_age</span> - Delete log files older than (days). <span class="li-normal">type: int</span></li>
        <li> <span class="li-head">report_quota</span> - Report quota (MB). <span class="li-normal">type: int</span></li>
        <li> <span class="li-head">roll_day</span> - Day of week on which to roll log file. <span class="li-normal">type: str</span> <span class="li-normal">choices: sunday, monday, tuesday, wednesday, thursday, friday, saturday</span></li>
        <li> <span class="li-head">roll_schedule</span> - Frequency to check log file for rolling. <span class="li-normal">type: str</span> <span class="li-normal">choices: daily, weekly</span></li>
        <li> <span class="li-head">roll_time</span> - Time of day to roll the log file (hh:mm). <span class="li-normal">type: str</span></li>
        <li> <span class="li-head">source_ip</span> - Source IP address to use for uploading disk log files. <span class="li-normal">type: str</span></li>
        <li> <span class="li-head">status</span> - Enable/disable local disk logging. <span class="li-normal">type: str</span> <span class="li-normal">choices: enable, disable</span></li>
        <li> <span class="li-head">upload</span> - Enable/disable uploading log files when they are rolled. <span class="li-normal">type: str</span> <span class="li-normal">choices: enable, disable</span></li>
        <li> <span class="li-head">upload_delete_files</span> - Delete log files after uploading . <span class="li-normal">type: str</span> <span class="li-normal">choices: enable, disable</span></li>
        <li> <span class="li-head">upload_destination</span> - The type of server to upload log files to. Only FTP is currently supported. <span class="li-normal">type: str</span> <span class="li-normal">choices: ftp-server</span></li>
        <li> <span class="li-head">upload_ssl_conn</span> - Enable/disable encrypted FTPS communication to upload log files. <span class="li-normal">type: str</span> <span class="li-normal">choices: default, high, low, disable</span></li>
        <li> <span class="li-head">uploaddir</span> - The remote directory on the FTP server to upload log files to. <span class="li-normal">type: str</span></li>
        <li> <span class="li-head">uploadip</span> - IP address of the FTP server to upload log files to. <span class="li-normal">type: str</span></li>
        <li> <span class="li-head">uploadpass</span> - Password required to log into the FTP server to upload disk log files. <span class="li-normal">type: str</span></li>
        <li> <span class="li-head">uploadport</span> - TCP port to use for communicating with the FTP server . <span class="li-normal">type: int</span></li>
        <li> <span class="li-head">uploadsched</span> - Set the schedule for uploading log files to the FTP server . <span class="li-normal">type: str</span> <span class="li-normal">choices: disable, enable</span></li>
        <li> <span class="li-head">uploadtime</span> - Time of day at which log files are uploaded if uploadsched is enabled (hh:mm or hh). <span class="li-normal">type: str</span></li>
        <li> <span class="li-head">uploadtype</span> - Types of log files to upload. Separate multiple entries with a space. <span class="li-normal">type: str</span> <span class="li-normal">choices: traffic, event, virus, webfilter, IPS, spamfilter, dlp-archive, anomaly, voip, dlp, app-ctrl, waf, netscan, gtp, dns</span></li>
        <li> <span class="li-head">uploaduser</span> - Username required to log into the FTP server to upload disk log files. <span class="li-normal">type: str</span></li>
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
      - name: Settings for local disk logging.
        fortios_log_disk_setting:
          vdom:  "{{ vdom }}"
          log_disk_setting:
            diskfull: "overwrite"
            dlp_archive_quota: "4"
            full_final_warning_threshold: "5"
            full_first_warning_threshold: "6"
            full_second_warning_threshold: "7"
            ips_archive: "enable"
            log_quota: "9"
            max_log_file_size: "10"
            max_policy_packet_capture_size: "11"
            maximum_log_age: "12"
            report_quota: "13"
            roll_day: "sunday"
            roll_schedule: "daily"
            roll_time: "<your_own_value>"
            source_ip: "84.230.14.43"
            status: "enable"
            upload: "enable"
            upload_delete_files: "enable"
            upload_destination: "ftp-server"
            upload_ssl_conn: "default"
            uploaddir: "<your_own_value>"
            uploadip: "<your_own_value>"
            uploadpass: "<your_own_value>"
            uploadport: "26"
            uploadsched: "disable"
            uploadtime: "<your_own_value>"
            uploadtype: "traffic"
            uploaduser: "<your_own_value>"


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
