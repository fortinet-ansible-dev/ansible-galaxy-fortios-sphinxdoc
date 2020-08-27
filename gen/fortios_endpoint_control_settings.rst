:source: fortios_endpoint_control_settings.py

:orphan:

.. fortios_endpoint_control_settings:

fortios_endpoint_control_settings -- Configure endpoint control settings in Fortinet's FortiOS and FortiGate.
+++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++

.. versionadded:: 2.8

.. contents::
   :local:
   :depth: 1


Synopsis
--------
- This module is able to configure a FortiGate or FortiOS (FOS) device by allowing the user to set and modify endpoint_control feature and settings category. Examples include all parameters and values need to be adjusted to datasources before usage. Tested with FOS v6.0.0



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
    <li> <span class="li-head">endpoint_control_settings</span> - Configure endpoint control settings. <span class="li-normal">type: dict</span></li>
        <ul class="ul-self">
        <li> <span class="li-head">download_custom_link</span> - Customized URL for downloading FortiClient. <span class="li-normal">type: str</span></li>
        <li> <span class="li-head">download_location</span> - FortiClient download location (FortiGuard or custom). <span class="li-normal">type: str</span> <span class="li-normal">choices: fortiguard, custom</span></li>
        <li> <span class="li-head">forticlient_avdb_update_interval</span> - Period of time between FortiClient AntiVirus database updates (0 - 24 hours). <span class="li-normal">type: int</span></li>
        <li> <span class="li-head">forticlient_dereg_unsupported_client</span> - Enable/disable deregistering unsupported FortiClient endpoints. <span class="li-normal">type: str</span> <span class="li-normal">choices: enable, disable</span></li>
        <li> <span class="li-head">forticlient_ems_rest_api_call_timeout</span> - FortiClient EMS call timeout in milliseconds (500 - 30000 milliseconds). <span class="li-normal">type: int</span></li>
        <li> <span class="li-head">forticlient_keepalive_interval</span> - Interval between two KeepAlive messages from FortiClient (20 - 300 sec). <span class="li-normal">type: int</span></li>
        <li> <span class="li-head">forticlient_offline_grace</span> - Enable/disable grace period for offline registered clients. <span class="li-normal">type: str</span> <span class="li-normal">choices: enable, disable</span></li>
        <li> <span class="li-head">forticlient_offline_grace_interval</span> - Grace period for offline registered FortiClient (60 - 600 sec). <span class="li-normal">type: int</span></li>
        <li> <span class="li-head">forticlient_reg_key</span> - FortiClient registration key. <span class="li-normal">type: str</span></li>
        <li> <span class="li-head">forticlient_reg_key_enforce</span> - Enable/disable requiring or enforcing FortiClient registration keys. <span class="li-normal">type: str</span> <span class="li-normal">choices: enable, disable</span></li>
        <li> <span class="li-head">forticlient_reg_timeout</span> - FortiClient registration license timeout (days, min = 1, max = 180, 0 means unlimited). <span class="li-normal">type: int</span></li>
        <li> <span class="li-head">forticlient_sys_update_interval</span> - Interval between two system update messages from FortiClient (30 - 1440 min). <span class="li-normal">type: int</span></li>
        <li> <span class="li-head">forticlient_user_avatar</span> - Enable/disable uploading FortiClient user avatars. <span class="li-normal">type: str</span> <span class="li-normal">choices: enable, disable</span></li>
        <li> <span class="li-head">forticlient_warning_interval</span> - Period of time between FortiClient portal warnings (0 - 24 hours). <span class="li-normal">type: int</span></li>
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
      - name: Configure endpoint control settings.
        fortios_endpoint_control_settings:
          vdom:  "{{ vdom }}"
          endpoint_control_settings:
            download_custom_link: "<your_own_value>"
            download_location: "fortiguard"
            forticlient_avdb_update_interval: "5"
            forticlient_dereg_unsupported_client: "enable"
            forticlient_ems_rest_api_call_timeout: "7"
            forticlient_keepalive_interval: "8"
            forticlient_offline_grace: "enable"
            forticlient_offline_grace_interval: "10"
            forticlient_reg_key: "<your_own_value>"
            forticlient_reg_key_enforce: "enable"
            forticlient_reg_timeout: "13"
            forticlient_sys_update_interval: "14"
            forticlient_user_avatar: "enable"
            forticlient_warning_interval: "16"


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
