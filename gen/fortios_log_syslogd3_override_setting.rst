:source: fortios_log_syslogd3_override_setting.py

:orphan:

.. fortios_log_syslogd3_override_setting:

fortios_log_syslogd3_override_setting -- Override settings for remote syslog server in Fortinet's FortiOS and FortiGate.
++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++

.. versionadded:: 2.9

.. contents::
   :local:
   :depth: 1


Synopsis
--------
- This module is able to configure a FortiGate or FortiOS (FOS) device by allowing the user to set and modify log_syslogd3 feature and override_setting category. Examples include all parameters and values need to be adjusted to datasources before usage. Tested with FOS v6.2.0



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
    <li> <span class="li-head">log_syslogd3_override_setting</span> - Override settings for remote syslog server. <span class="li-normal">type: dict</span></li>
        <ul class="ul-self">
        <li> <span class="li-head">certificate</span> - Certificate used to communicate with Syslog server. Source certificate.local.name. <span class="li-normal">type: str</span></li>
        <li> <span class="li-head">custom_field_name</span> - Custom field name for CEF format logging. <span class="li-normal">type: list</span></li>
            <ul class="ul-self">
            <li> <span class="li-head">custom</span> - Field custom name. <span class="li-normal">type: str</span></li>
            <li> <span class="li-head">id</span> - Entry ID. <span class="li-normal">type: int</span> <span class="li-required">required: True</span></li>
            <li> <span class="li-head">name</span> - Field name. <span class="li-normal">type: str</span></li>
            </ul>
        <li> <span class="li-head">enc_algorithm</span> - Enable/disable reliable syslogging with TLS encryption. <span class="li-normal">type: str</span> <span class="li-normal">choices: high-medium, high, low, disable</span></li>
        <li> <span class="li-head">facility</span> - Remote syslog facility. <span class="li-normal">type: str</span> <span class="li-normal">choices: kernel, user, mail, daemon, auth, syslog, lpr, news, uucp, cron, authpriv, ftp, ntp, audit, alert, clock, local0, local1, local2, local3, local4, local5, local6, local7</span></li>
        <li> <span class="li-head">format</span> - Log format. <span class="li-normal">type: str</span> <span class="li-normal">choices: default, csv, cef</span></li>
        <li> <span class="li-head">mode</span> - Remote syslog logging over UDP/Reliable TCP. <span class="li-normal">type: str</span> <span class="li-normal">choices: udp, legacy-reliable, reliable</span></li>
        <li> <span class="li-head">override</span> - Enable/disable override syslog settings. <span class="li-normal">type: str</span> <span class="li-normal">choices: enable, disable</span></li>
        <li> <span class="li-head">port</span> - Server listen port. <span class="li-normal">type: int</span></li>
        <li> <span class="li-head">server</span> - Address of remote syslog server. <span class="li-normal">type: str</span></li>
        <li> <span class="li-head">source_ip</span> - Source IP address of syslog. <span class="li-normal">type: str</span></li>
        <li> <span class="li-head">ssl_min_proto_version</span> - Minimum supported protocol version for SSL/TLS connections . <span class="li-normal">type: str</span> <span class="li-normal">choices: default, SSLv3, TLSv1, TLSv1-1, TLSv1-2</span></li>
        <li> <span class="li-head">status</span> - Enable/disable remote syslog logging. <span class="li-normal">type: str</span> <span class="li-normal">choices: enable, disable</span></li>
        <li> <span class="li-head">syslog_type</span> - Hidden setting index of Syslog. <span class="li-normal">type: int</span></li>
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
      - name: Override settings for remote syslog server.
        fortios_log_syslogd3_override_setting:
          vdom:  "{{ vdom }}"
          log_syslogd3_override_setting:
            certificate: "<your_own_value> (source certificate.local.name)"
            custom_field_name:
             -
                custom: "<your_own_value>"
                id:  "6"
                name: "default_name_7"
            enc_algorithm: "high-medium"
            facility: "kernel"
            format: "default"
            mode: "udp"
            override: "enable"
            port: "13"
            server: "192.168.100.40"
            source_ip: "84.230.14.43"
            ssl_min_proto_version: "default"
            status: "enable"
            syslog_type: "18"
    


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
