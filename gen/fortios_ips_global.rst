:source: fortios_ips_global.py

:orphan:

.. fortios_ips_global:

fortios_ips_global -- Configure IPS global parameter in Fortinet's FortiOS and FortiGate.
+++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++

.. versionadded:: 2.8

.. contents::
   :local:
   :depth: 1


Synopsis
--------
- This module is able to configure a FortiGate or FortiOS (FOS) device by allowing the user to set and modify ips feature and global category. Examples include all parameters and values need to be adjusted to datasources before usage. Tested with FOS v6.2.0



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
    <li> <span class="li-head">ips_global</span> - Configure IPS global parameter. <span class="li-normal">type: dict</span></li>
        <ul class="ul-self">
        <li> <span class="li-head">anomaly_mode</span> - Global blocking mode for rate-based anomalies. <span class="li-normal">type: str</span> <span class="li-normal">choices: periodical, continuous</span></li>
        <li> <span class="li-head">database</span> - Regular or extended IPS database. Regular protects against the latest common and in-the-wild attacks. Extended includes protection from legacy attacks. <span class="li-normal">type: str</span> <span class="li-normal">choices: regular, extended</span></li>
        <li> <span class="li-head">deep_app_insp_db_limit</span> - Limit on number of entries in deep application inspection database (1 - 2147483647, 0 = use recommended setting) <span class="li-normal">type: int</span></li>
        <li> <span class="li-head">deep_app_insp_timeout</span> - Timeout for Deep application inspection (1 - 2147483647 sec., 0 = use recommended setting). <span class="li-normal">type: int</span></li>
        <li> <span class="li-head">engine_count</span> - Number of IPS engines running. If set to the default value of 0, FortiOS sets the number to optimize performance depending on the number of CPU cores. <span class="li-normal">type: int</span></li>
        <li> <span class="li-head">exclude_signatures</span> - Excluded signatures. <span class="li-normal">type: str</span> <span class="li-normal">choices: none, industrial</span></li>
        <li> <span class="li-head">fail_open</span> - Enable to allow traffic if the IPS process crashes. Default is disable and IPS traffic is blocked when the IPS process crashes. <span class="li-normal">type: str</span> <span class="li-normal">choices: enable, disable</span></li>
        <li> <span class="li-head">intelligent_mode</span> - Enable/disable IPS adaptive scanning (intelligent mode). Intelligent mode optimizes the scanning method for the type of traffic. <span class="li-normal">type: str</span> <span class="li-normal">choices: enable, disable</span></li>
        <li> <span class="li-head">session_limit_mode</span> - Method of counting concurrent sessions used by session limit anomalies. Choose between greater accuracy (accurate) or improved performance (heuristics). <span class="li-normal">type: str</span> <span class="li-normal">choices: accurate, heuristic</span></li>
        <li> <span class="li-head">skype_client_public_ipaddr</span> - Public IP addresses of your network that receive Skype sessions. Helps identify Skype sessions. Separate IP addresses with commas. <span class="li-normal">type: str</span></li>
        <li> <span class="li-head">socket_size</span> - IPS socket buffer size (0 - 256 MB). Default depends on available memory. Can be changed to tune performance. <span class="li-normal">type: int</span></li>
        <li> <span class="li-head">sync_session_ttl</span> - Enable/disable use of kernel session TTL for IPS sessions. <span class="li-normal">type: str</span> <span class="li-normal">choices: enable, disable</span></li>
        <li> <span class="li-head">traffic_submit</span> - Enable/disable submitting attack data found by this FortiGate to FortiGuard. <span class="li-normal">type: str</span> <span class="li-normal">choices: enable, disable</span></li>
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
      - name: Configure IPS global parameter.
        fortios_ips_global:
          vdom:  "{{ vdom }}"
          ips_global:
            anomaly_mode: "periodical"
            database: "regular"
            deep_app_insp_db_limit: "5"
            deep_app_insp_timeout: "6"
            engine_count: "7"
            exclude_signatures: "none"
            fail_open: "enable"
            intelligent_mode: "enable"
            session_limit_mode: "accurate"
            skype_client_public_ipaddr: "<your_own_value>"
            socket_size: "13"
            sync_session_ttl: "enable"
            traffic_submit: "enable"
    


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
