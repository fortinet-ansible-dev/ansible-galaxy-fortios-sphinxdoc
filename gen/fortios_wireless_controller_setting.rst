:source: fortios_wireless_controller_setting.py

:orphan:

.. fortios_wireless_controller_setting:

fortios_wireless_controller_setting -- VDOM wireless controller configuration in Fortinet's FortiOS and FortiGate.
++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++

.. versionadded:: 2.8

.. contents::
   :local:
   :depth: 1


Synopsis
--------
- This module is able to configure a FortiGate or FortiOS (FOS) device by allowing the user to set and modify wireless_controller feature and setting category. Examples include all parameters and values need to be adjusted to datasources before usage. Tested with FOS v6.4.0



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
    <li> <span class="li-head">wireless_controller_setting</span> - VDOM wireless controller configuration. <span class="li-normal">type: dict</span></li>
        <ul class="ul-self">
        <li> <span class="li-head">account_id</span> - FortiCloud customer account ID. <span class="li-normal">type: str</span></li>
        <li> <span class="li-head">country</span> - Country or region in which the FortiGate is located. The country determines the 802.11 bands and channels that are available. <span class="li-normal">type: str</span> <span class="li-normal">choices: NA, AL, DZ, AO, AR, AM, AU, AT, AZ, BS, BH, BD, BB, BY, BE, BZ, BO, BA, BR, BN, BG, KH, CF, CL, CN, CO, CR, HR, CY, CZ, DK, DO, EC, EG, SV, EE, FI, FR, GE, DE, GR, GL, GD, GU, GT, HT, HN, HK, HU, IS, IN, ID, IR, IE, IL, IT, JM, JO, KZ, KE, KP, KR, KW, LV, LB, LI, LT, LU, MO, MK, MY, MT, MX, MC, MA, MZ, MM, NP, NL, AN, AW, NZ, False, OM, PK, PA, PG, PY, PE, PH, PL, PT, PR, QA, RO, RU, RW, SA, RS, ME, SG, SK, SI, ZA, ES, LK, SE, SD, CH, SY, TW, TZ, TH, TT, TN, TR, AE, UA, GB, US, PS, UY, UZ, VE, VN, YE, ZB, ZW, JP, CA</span></li>
        <li> <span class="li-head">darrp_optimize</span> - Time for running Dynamic Automatic Radio Resource Provisioning (DARRP) optimizations (0 - 86400 sec). <span class="li-normal">type: int</span></li>
        <li> <span class="li-head">darrp_optimize_schedules</span> - Firewall schedules for DARRP running time. DARRP will run periodically based on darrp-optimize within the schedules. Separate multiple schedule names with a space. <span class="li-normal">type: list</span></li>
            <ul class="ul-self">
            <li> <span class="li-head">name</span> - Schedule name. Source firewall.schedule.group.name firewall.schedule.recurring.name firewall.schedule.onetime.name. <span class="li-normal">type: str</span> <span class="li-required">required: True</span></li>
            </ul>
        <li> <span class="li-head">duplicate_ssid</span> - Enable/disable allowing Virtual Access Points (VAPs) to use the same SSID name in the same VDOM. <span class="li-normal">type: str</span> <span class="li-normal">choices: enable, disable</span></li>
        <li> <span class="li-head">fake_ssid_action</span> - Actions taken for detected fake SSID. <span class="li-normal">type: str</span> <span class="li-normal">choices: log, suppress</span></li>
        <li> <span class="li-head">fapc_compatibility</span> - Enable/disable FAP-C series compatibility. <span class="li-normal">type: str</span> <span class="li-normal">choices: enable, disable</span></li>
        <li> <span class="li-head">offending_ssid</span> - Configure offending SSID. <span class="li-normal">type: list</span></li>
            <ul class="ul-self">
            <li> <span class="li-head">action</span> - Actions taken for detected offending SSID. <span class="li-normal">type: str</span> <span class="li-normal">choices: log, suppress</span></li>
            <li> <span class="li-head">id</span> - ID. <span class="li-normal">type: int</span> <span class="li-required">required: True</span></li>
            <li> <span class="li-head">ssid_pattern</span> - Define offending SSID pattern (case insensitive), eg: word, word*, *word, wo*rd. <span class="li-normal">type: str</span></li>
            </ul>
        <li> <span class="li-head">phishing_ssid_detect</span> - Enable/disable phishing SSID detection. <span class="li-normal">type: str</span> <span class="li-normal">choices: enable, disable</span></li>
        <li> <span class="li-head">wfa_compatibility</span> - Enable/disable WFA compatibility. <span class="li-normal">type: str</span> <span class="li-normal">choices: enable, disable</span></li>
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
      - name: VDOM wireless controller configuration.
        fortios_wireless_controller_setting:
          vdom:  "{{ vdom }}"
          wireless_controller_setting:
            account_id: "<your_own_value>"
            country: "NA"
            darrp_optimize: "5"
            darrp_optimize_schedules:
             -
                name: "default_name_7 (source firewall.schedule.group.name firewall.schedule.recurring.name firewall.schedule.onetime.name)"
            duplicate_ssid: "enable"
            fake_ssid_action: "log"
            fapc_compatibility: "enable"
            offending_ssid:
             -
                action: "log"
                id:  "13"
                ssid_pattern: "<your_own_value>"
            phishing_ssid_detect: "enable"
            wfa_compatibility: "enable"


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
