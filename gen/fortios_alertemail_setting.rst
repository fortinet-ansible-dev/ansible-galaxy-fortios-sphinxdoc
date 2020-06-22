:source: fortios_alertemail_setting.py

:orphan:

.. fortios_alertemail_setting:

fortios_alertemail_setting -- Configure alert email settings in Fortinet's FortiOS and FortiGate.
+++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++

.. versionadded:: 2.9

.. contents::
   :local:
   :depth: 1


Synopsis
--------
- This module is able to configure a FortiGate or FortiOS (FOS) device by allowing the user to set and modify alertemail feature and setting category. Examples include all parameters and values need to be adjusted to datasources before usage. Tested with FOS v6.0.5



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
    <li> <span class="li-head">alertemail_setting</span> - Configure alert email settings. <span class="li-normal">type: dict</span></li>
        <ul class="ul-self">
        <li> <span class="li-head">admin_login_logs</span> - Enable/disable administrator login/logout logs in alert email. <span class="li-normal">type: str</span> <span class="li-normal">choices: enable, disable</span></li>
        <li> <span class="li-head">alert_interval</span> - Alert alert interval in minutes. <span class="li-normal">type: int</span></li>
        <li> <span class="li-head">amc_interface_bypass_mode</span> - Enable/disable Fortinet Advanced Mezzanine Card (AMC) interface bypass mode logs in alert email. <span class="li-normal">type: str</span> <span class="li-normal">choices: enable, disable</span></li>
        <li> <span class="li-head">antivirus_logs</span> - Enable/disable antivirus logs in alert email. <span class="li-normal">type: str</span> <span class="li-normal">choices: enable, disable</span></li>
        <li> <span class="li-head">configuration_changes_logs</span> - Enable/disable configuration change logs in alert email. <span class="li-normal">type: str</span> <span class="li-normal">choices: enable, disable</span></li>
        <li> <span class="li-head">critical_interval</span> - Critical alert interval in minutes. <span class="li-normal">type: int</span></li>
        <li> <span class="li-head">debug_interval</span> - Debug alert interval in minutes. <span class="li-normal">type: int</span></li>
        <li> <span class="li-head">email_interval</span> - Interval between sending alert emails (1 - 99999 min). <span class="li-normal">type: int</span></li>
        <li> <span class="li-head">emergency_interval</span> - Emergency alert interval in minutes. <span class="li-normal">type: int</span></li>
        <li> <span class="li-head">error_interval</span> - Error alert interval in minutes. <span class="li-normal">type: int</span></li>
        <li> <span class="li-head">FDS_license_expiring_days</span> - Number of days to send alert email prior to FortiGuard license expiration (1 - 100 days). <span class="li-normal">type: int</span></li>
        <li> <span class="li-head">FDS_license_expiring_warning</span> - Enable/disable FortiGuard license expiration warnings in alert email. <span class="li-normal">type: str</span> <span class="li-normal">choices: enable, disable</span></li>
        <li> <span class="li-head">FDS_update_logs</span> - Enable/disable FortiGuard update logs in alert email. <span class="li-normal">type: str</span> <span class="li-normal">choices: enable, disable</span></li>
        <li> <span class="li-head">filter_mode</span> - How to filter log messages that are sent to alert emails. <span class="li-normal">type: str</span> <span class="li-normal">choices: category, threshold</span></li>
        <li> <span class="li-head">FIPS_CC_errors</span> - Enable/disable FIPS and Common Criteria error logs in alert email. <span class="li-normal">type: str</span> <span class="li-normal">choices: enable, disable</span></li>
        <li> <span class="li-head">firewall_authentication_failure_logs</span> - Enable/disable firewall authentication failure logs in alert email. <span class="li-normal">type: str</span> <span class="li-normal">choices: enable, disable</span></li>
        <li> <span class="li-head">fortiguard_log_quota_warning</span> - Enable/disable FortiCloud log quota warnings in alert email. <span class="li-normal">type: str</span> <span class="li-normal">choices: enable, disable</span></li>
        <li> <span class="li-head">FSSO_disconnect_logs</span> - Enable/disable logging of FSSO collector agent disconnect. <span class="li-normal">type: str</span> <span class="li-normal">choices: enable, disable</span></li>
        <li> <span class="li-head">HA_logs</span> - Enable/disable HA logs in alert email. <span class="li-normal">type: str</span> <span class="li-normal">choices: enable, disable</span></li>
        <li> <span class="li-head">information_interval</span> - Information alert interval in minutes. <span class="li-normal">type: int</span></li>
        <li> <span class="li-head">IPS_logs</span> - Enable/disable IPS logs in alert email. <span class="li-normal">type: str</span> <span class="li-normal">choices: enable, disable</span></li>
        <li> <span class="li-head">IPsec_errors_logs</span> - Enable/disable IPsec error logs in alert email. <span class="li-normal">type: str</span> <span class="li-normal">choices: enable, disable</span></li>
        <li> <span class="li-head">local_disk_usage</span> - Disk usage percentage at which to send alert email (1 - 99 percent). <span class="li-normal">type: int</span></li>
        <li> <span class="li-head">log_disk_usage_warning</span> - Enable/disable disk usage warnings in alert email. <span class="li-normal">type: str</span> <span class="li-normal">choices: enable, disable</span></li>
        <li> <span class="li-head">mailto1</span> - Email address to send alert email to (usually a system administrator) (max. 64 characters). <span class="li-normal">type: str</span></li>
        <li> <span class="li-head">mailto2</span> - Optional second email address to send alert email to (max. 64 characters). <span class="li-normal">type: str</span></li>
        <li> <span class="li-head">mailto3</span> - Optional third email address to send alert email to (max. 64 characters). <span class="li-normal">type: str</span></li>
        <li> <span class="li-head">notification_interval</span> - Notification alert interval in minutes. <span class="li-normal">type: int</span></li>
        <li> <span class="li-head">PPP_errors_logs</span> - Enable/disable PPP error logs in alert email. <span class="li-normal">type: str</span> <span class="li-normal">choices: enable, disable</span></li>
        <li> <span class="li-head">severity</span> - Lowest severity level to log. <span class="li-normal">type: str</span> <span class="li-normal">choices: emergency, alert, critical, error, warning, notification, information, debug</span></li>
        <li> <span class="li-head">ssh_logs</span> - Enable/disable SSH logs in alert email. <span class="li-normal">type: str</span> <span class="li-normal">choices: enable, disable</span></li>
        <li> <span class="li-head">sslvpn_authentication_errors_logs</span> - Enable/disable SSL-VPN authentication error logs in alert email. <span class="li-normal">type: str</span> <span class="li-normal">choices: enable, disable</span></li>
        <li> <span class="li-head">username</span> - Name that appears in the From: field of alert emails (max. 36 characters). <span class="li-normal">type: str</span></li>
        <li> <span class="li-head">violation_traffic_logs</span> - Enable/disable violation traffic logs in alert email. <span class="li-normal">type: str</span> <span class="li-normal">choices: enable, disable</span></li>
        <li> <span class="li-head">warning_interval</span> - Warning alert interval in minutes. <span class="li-normal">type: int</span></li>
        <li> <span class="li-head">webfilter_logs</span> - Enable/disable web filter logs in alert email. <span class="li-normal">type: str</span> <span class="li-normal">choices: enable, disable</span></li>
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
      - name: Configure alert email settings.
        fortios_alertemail_setting:
          vdom:  "{{ vdom }}"
          alertemail_setting:
            admin_login_logs: "enable"
            alert_interval: "4"
            amc_interface_bypass_mode: "enable"
            antivirus_logs: "enable"
            configuration_changes_logs: "enable"
            critical_interval: "8"
            debug_interval: "9"
            email_interval: "10"
            emergency_interval: "11"
            error_interval: "12"
            FDS_license_expiring_days: "13"
            FDS_license_expiring_warning: "enable"
            FDS_update_logs: "enable"
            filter_mode: "category"
            FIPS_CC_errors: "enable"
            firewall_authentication_failure_logs: "enable"
            fortiguard_log_quota_warning: "enable"
            FSSO_disconnect_logs: "enable"
            HA_logs: "enable"
            information_interval: "22"
            IPS_logs: "enable"
            IPsec_errors_logs: "enable"
            local_disk_usage: "25"
            log_disk_usage_warning: "enable"
            mailto1: "<your_own_value>"
            mailto2: "<your_own_value>"
            mailto3: "<your_own_value>"
            notification_interval: "30"
            PPP_errors_logs: "enable"
            severity: "emergency"
            ssh_logs: "enable"
            sslvpn_authentication_errors_logs: "enable"
            username: "<your_own_value>"
            violation_traffic_logs: "enable"
            warning_interval: "37"
            webfilter_logs: "enable"


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
