:source: fortios_log_fortianalyzer2_override_setting.py

:orphan:

.. fortios_log_fortianalyzer2_override_setting:

fortios_log_fortianalyzer2_override_setting -- Override FortiAnalyzer settings in Fortinet's FortiOS and FortiGate.
+++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++

.. versionadded:: 2.9

.. contents::
   :local:
   :depth: 1


Synopsis
--------
- This module is able to configure a FortiGate or FortiOS (FOS) device by allowing the user to set and modify log_fortianalyzer2 feature and override_setting category. Examples include all parameters and values need to be adjusted to datasources before usage. Tested with FOS v6.2.0



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
    <li> <span class="li-head">log_fortianalyzer2_override_setting</span> - Override FortiAnalyzer settings. <span class="li-normal">type: dict</span></li>
        <ul class="ul-self">
        <li> <span class="li-head">__change_ip</span> - Hidden attribute. <span class="li-normal">type: int</span></li>
        <li> <span class="li-head">access_config</span> - Enable/disable FortiAnalyzer access to configuration and data. <span class="li-normal">type: str</span> <span class="li-normal">choices: enable, disable</span></li>
        <li> <span class="li-head">certificate</span> - Certificate used to communicate with FortiAnalyzer. Source certificate.local.name. <span class="li-normal">type: str</span></li>
        <li> <span class="li-head">certificate_verification</span> - Enable/disable identity verification of FortiAnalyzer by use of certificate. <span class="li-normal">type: str</span> <span class="li-normal">choices: enable, disable</span></li>
        <li> <span class="li-head">conn_timeout</span> - FortiAnalyzer connection time-out in seconds (for status and log buffer). <span class="li-normal">type: int</span></li>
        <li> <span class="li-head">enc_algorithm</span> - Enable/disable sending FortiAnalyzer log data with SSL encryption. <span class="li-normal">type: str</span> <span class="li-normal">choices: high-medium, high, low</span></li>
        <li> <span class="li-head">faz_type</span> - Hidden setting index of FortiAnalyzer. <span class="li-normal">type: int</span></li>
        <li> <span class="li-head">hmac_algorithm</span> - FortiAnalyzer IPsec tunnel HMAC algorithm. <span class="li-normal">type: str</span> <span class="li-normal">choices: sha256, sha1</span></li>
        <li> <span class="li-head">ips_archive</span> - Enable/disable IPS packet archive logging. <span class="li-normal">type: str</span> <span class="li-normal">choices: enable, disable</span></li>
        <li> <span class="li-head">mgmt_name</span> - Hidden management name of FortiAnalyzer. <span class="li-normal">type: str</span></li>
        <li> <span class="li-head">monitor_failure_retry_period</span> - Time between FortiAnalyzer connection retries in seconds (for status and log buffer). <span class="li-normal">type: int</span></li>
        <li> <span class="li-head">monitor_keepalive_period</span> - Time between OFTP keepalives in seconds (for status and log buffer). <span class="li-normal">type: int</span></li>
        <li> <span class="li-head">override</span> - Enable/disable overriding FortiAnalyzer settings or use global settings. <span class="li-normal">type: str</span> <span class="li-normal">choices: enable, disable</span></li>
        <li> <span class="li-head">reliable</span> - Enable/disable reliable logging to FortiAnalyzer. <span class="li-normal">type: str</span> <span class="li-normal">choices: enable, disable</span></li>
        <li> <span class="li-head">serial</span> - Serial numbers of the FortiAnalyzer. <span class="li-normal">type: list</span></li>
            <ul class="ul-self">
            <li> <span class="li-head">name</span> - Serial Number. <span class="li-normal">type: str</span> <span class="li-required">required: True</span></li>
            </ul>
        <li> <span class="li-head">server</span> - The remote FortiAnalyzer. <span class="li-normal">type: str</span></li>
        <li> <span class="li-head">source_ip</span> - Source IPv4 or IPv6 address used to communicate with FortiAnalyzer. <span class="li-normal">type: str</span></li>
        <li> <span class="li-head">ssl_min_proto_version</span> - Minimum supported protocol version for SSL/TLS connections . <span class="li-normal">type: str</span> <span class="li-normal">choices: default, SSLv3, TLSv1, TLSv1-1, TLSv1-2</span></li>
        <li> <span class="li-head">status</span> - Enable/disable logging to FortiAnalyzer. <span class="li-normal">type: str</span> <span class="li-normal">choices: enable, disable</span></li>
        <li> <span class="li-head">upload_day</span> - Day of week (month) to upload logs. <span class="li-normal">type: str</span></li>
        <li> <span class="li-head">upload_interval</span> - Frequency to upload log files to FortiAnalyzer. <span class="li-normal">type: str</span> <span class="li-normal">choices: daily, weekly, monthly</span></li>
        <li> <span class="li-head">upload_option</span> - Enable/disable logging to hard disk and then uploading to FortiAnalyzer. <span class="li-normal">type: str</span> <span class="li-normal">choices: store-and-upload, realtime, 1-minute, 5-minute</span></li>
        <li> <span class="li-head">upload_time</span> - Time to upload logs (hh:mm). <span class="li-normal">type: str</span></li>
        <li> <span class="li-head">use_management_vdom</span> - Enable/disable use of management VDOM IP address as source IP for logs sent to FortiAnalyzer. <span class="li-normal">type: str</span> <span class="li-normal">choices: enable, disable</span></li>
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
      - name: Override FortiAnalyzer settings.
        fortios_log_fortianalyzer2_override_setting:
          vdom:  "{{ vdom }}"
          log_fortianalyzer2_override_setting:
            __change_ip: "3"
            access_config: "enable"
            certificate: "<your_own_value> (source certificate.local.name)"
            certificate_verification: "enable"
            conn_timeout: "7"
            enc_algorithm: "high-medium"
            faz_type: "9"
            hmac_algorithm: "sha256"
            ips_archive: "enable"
            mgmt_name: "<your_own_value>"
            monitor_failure_retry_period: "13"
            monitor_keepalive_period: "14"
            override: "enable"
            reliable: "enable"
            serial:
             -
                name: "default_name_18"
            server: "192.168.100.40"
            source_ip: "84.230.14.43"
            ssl_min_proto_version: "default"
            status: "enable"
            upload_day: "<your_own_value>"
            upload_interval: "daily"
            upload_option: "store-and-upload"
            upload_time: "<your_own_value>"
            use_management_vdom: "enable"


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
