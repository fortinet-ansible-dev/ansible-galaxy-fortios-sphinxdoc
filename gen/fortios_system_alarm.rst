:source: fortios_system_alarm.py

:orphan:

.. fortios_system_alarm:

fortios_system_alarm -- Configure alarm in Fortinet's FortiOS and FortiGate.
++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++

.. versionadded:: 2.9

.. contents::
   :local:
   :depth: 1


Synopsis
--------
- This module is able to configure a FortiGate or FortiOS (FOS) device by allowing the user to set and modify system feature and alarm category. Examples include all parameters and values need to be adjusted to datasources before usage. Tested with FOS v6.4.0



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
    <li> <span class="li-head">system_alarm</span> - Configure alarm. <span class="li-normal">type: dict</span></li>
        <ul class="ul-self">
        <li> <span class="li-head">audible</span> - Enable/disable audible alarm. <span class="li-normal">type: str</span> <span class="li-normal">choices: enable, disable</span></li>
        <li> <span class="li-head">groups</span> - Alarm groups. <span class="li-normal">type: list</span></li>
            <ul class="ul-self">
            <li> <span class="li-head">admin_auth_failure_threshold</span> - Admin authentication failure threshold. <span class="li-normal">type: int</span></li>
            <li> <span class="li-head">admin_auth_lockout_threshold</span> - Admin authentication lockout threshold. <span class="li-normal">type: int</span></li>
            <li> <span class="li-head">decryption_failure_threshold</span> - Decryption failure threshold. <span class="li-normal">type: int</span></li>
            <li> <span class="li-head">encryption_failure_threshold</span> - Encryption failure threshold. <span class="li-normal">type: int</span></li>
            <li> <span class="li-head">fw_policy_id</span> - Firewall policy ID. <span class="li-normal">type: int</span></li>
            <li> <span class="li-head">fw_policy_id_threshold</span> - Firewall policy ID threshold. <span class="li-normal">type: int</span></li>
            <li> <span class="li-head">fw_policy_violations</span> - Firewall policy violations. <span class="li-normal">type: list</span></li>
                <ul class="ul-self">
                <li> <span class="li-head">dst_ip</span> - Destination IP (0=all). <span class="li-normal">type: str</span></li>
                <li> <span class="li-head">dst_port</span> - Destination port (0=all). <span class="li-normal">type: int</span></li>
                <li> <span class="li-head">id</span> - Firewall policy violations ID. <span class="li-normal">type: int</span> <span class="li-required">required: True</span></li>
                <li> <span class="li-head">src_ip</span> - Source IP (0=all). <span class="li-normal">type: str</span></li>
                <li> <span class="li-head">src_port</span> - Source port (0=all). <span class="li-normal">type: int</span></li>
                <li> <span class="li-head">threshold</span> - Firewall policy violation threshold. <span class="li-normal">type: int</span></li>
                </ul>
            <li> <span class="li-head">id</span> - Group ID. <span class="li-normal">type: int</span> <span class="li-required">required: True</span></li>
            <li> <span class="li-head">log_full_warning_threshold</span> - Log full warning threshold. <span class="li-normal">type: int</span></li>
            <li> <span class="li-head">period</span> - Time period in seconds (0 = from start up). <span class="li-normal">type: int</span></li>
            <li> <span class="li-head">replay_attempt_threshold</span> - Replay attempt threshold. <span class="li-normal">type: int</span></li>
            <li> <span class="li-head">self_test_failure_threshold</span> - Self-test failure threshold. <span class="li-normal">type: int</span></li>
            <li> <span class="li-head">user_auth_failure_threshold</span> - User authentication failure threshold. <span class="li-normal">type: int</span></li>
            <li> <span class="li-head">user_auth_lockout_threshold</span> - User authentication lockout threshold. <span class="li-normal">type: int</span></li>
            </ul>
        <li> <span class="li-head">status</span> - Enable/disable alarm. <span class="li-normal">type: str</span> <span class="li-normal">choices: enable, disable</span></li>
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
      - name: Configure alarm.
        fortios_system_alarm:
          vdom:  "{{ vdom }}"
          system_alarm:
            audible: "enable"
            groups:
             -
                admin_auth_failure_threshold: "5"
                admin_auth_lockout_threshold: "6"
                decryption_failure_threshold: "7"
                encryption_failure_threshold: "8"
                fw_policy_id: "9"
                fw_policy_id_threshold: "10"
                fw_policy_violations:
                 -
                    dst_ip: "<your_own_value>"
                    dst_port: "13"
                    id:  "14"
                    src_ip: "<your_own_value>"
                    src_port: "16"
                    threshold: "17"
                id:  "18"
                log_full_warning_threshold: "19"
                period: "20"
                replay_attempt_threshold: "21"
                self_test_failure_threshold: "22"
                user_auth_failure_threshold: "23"
                user_auth_lockout_threshold: "24"
            status: "enable"


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
