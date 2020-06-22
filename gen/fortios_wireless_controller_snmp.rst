:source: fortios_wireless_controller_snmp.py

:orphan:

.. fortios_wireless_controller_snmp:

fortios_wireless_controller_snmp -- Configure SNMP in Fortinet's FortiOS and FortiGate.
+++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++

.. versionadded:: 2.10

.. contents::
   :local:
   :depth: 1


Synopsis
--------
- This module is able to configure a FortiGate or FortiOS (FOS) device by allowing the user to set and modify wireless_controller feature and snmp category. Examples include all parameters and values need to be adjusted to datasources before usage. Tested with FOS v6.4.0



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
    <li> <span class="li-head">wireless_controller_snmp</span> - Configure SNMP. <span class="li-normal">type: dict</span></li>
        <ul class="ul-self">
        <li> <span class="li-head">community</span> - SNMP Community Configuration. <span class="li-normal">type: list</span></li>
            <ul class="ul-self">
            <li> <span class="li-head">hosts</span> - Configure IPv4 SNMP managers (hosts). <span class="li-normal">type: list</span></li>
                <ul class="ul-self">
                <li> <span class="li-head">id</span> - Host entry ID. <span class="li-normal">type: int</span> <span class="li-required">required: True</span></li>
                <li> <span class="li-head">ip</span> - IPv4 address of the SNMP manager (host). <span class="li-normal">type: str</span></li>
                </ul>
            <li> <span class="li-head">id</span> - Community ID. <span class="li-normal">type: int</span> <span class="li-required">required: True</span></li>
            <li> <span class="li-head">name</span> - Community name. <span class="li-normal">type: str</span></li>
            <li> <span class="li-head">query_v1_status</span> - Enable/disable SNMP v1 queries. <span class="li-normal">type: str</span> <span class="li-normal">choices: enable, disable</span></li>
            <li> <span class="li-head">query_v2c_status</span> - Enable/disable SNMP v2c queries. <span class="li-normal">type: str</span> <span class="li-normal">choices: enable, disable</span></li>
            <li> <span class="li-head">status</span> - Enable/disable this SNMP community. <span class="li-normal">type: str</span> <span class="li-normal">choices: enable, disable</span></li>
            <li> <span class="li-head">trap_v1_status</span> - Enable/disable SNMP v1 traps. <span class="li-normal">type: str</span> <span class="li-normal">choices: enable, disable</span></li>
            <li> <span class="li-head">trap_v2c_status</span> - Enable/disable SNMP v2c traps. <span class="li-normal">type: str</span> <span class="li-normal">choices: enable, disable</span></li>
            </ul>
        <li> <span class="li-head">contact_info</span> - Contact Information. <span class="li-normal">type: str</span></li>
        <li> <span class="li-head">engine_id</span> - AC SNMP engineId string (maximum 24 characters). <span class="li-normal">type: str</span></li>
        <li> <span class="li-head">trap_high_cpu_threshold</span> - CPU usage when trap is sent. <span class="li-normal">type: int</span></li>
        <li> <span class="li-head">trap_high_mem_threshold</span> - Memory usage when trap is sent. <span class="li-normal">type: int</span></li>
        <li> <span class="li-head">user</span> - SNMP User Configuration. <span class="li-normal">type: list</span></li>
            <ul class="ul-self">
            <li> <span class="li-head">auth_proto</span> - Authentication protocol. <span class="li-normal">type: str</span> <span class="li-normal">choices: md5, sha</span></li>
            <li> <span class="li-head">auth_pwd</span> - Password for authentication protocol. <span class="li-normal">type: str</span></li>
            <li> <span class="li-head">name</span> - SNMP User Name <span class="li-normal">type: str</span> <span class="li-required">required: True</span></li>
            <li> <span class="li-head">notify_hosts</span> - Configure SNMP User Notify Hosts. <span class="li-normal">type: str</span></li>
            <li> <span class="li-head">priv_proto</span> - Privacy (encryption) protocol. <span class="li-normal">type: str</span> <span class="li-normal">choices: aes, des, aes256, aes256cisco</span></li>
            <li> <span class="li-head">priv_pwd</span> - Password for privacy (encryption) protocol. <span class="li-normal">type: str</span></li>
            <li> <span class="li-head">queries</span> - Enable/disable SNMP queries for this user. <span class="li-normal">type: str</span> <span class="li-normal">choices: enable, disable</span></li>
            <li> <span class="li-head">security_level</span> - Security level for message authentication and encryption. <span class="li-normal">type: str</span> <span class="li-normal">choices: no-auth-no-priv, auth-no-priv, auth-priv</span></li>
            <li> <span class="li-head">status</span> - SNMP User Enable <span class="li-normal">type: str</span> <span class="li-normal">choices: enable, disable</span></li>
            <li> <span class="li-head">trap_status</span> - Enable/disable traps for this SNMP user. <span class="li-normal">type: str</span> <span class="li-normal">choices: enable, disable</span></li>
            </ul>
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
      - name: Configure SNMP.
        fortios_wireless_controller_snmp:
          vdom:  "{{ vdom }}"
          wireless_controller_snmp:
            community:
             -
                hosts:
                 -
                    id:  "5"
                    ip: "<your_own_value>"
                id:  "7"
                name: "default_name_8"
                query_v1_status: "enable"
                query_v2c_status: "enable"
                status: "enable"
                trap_v1_status: "enable"
                trap_v2c_status: "enable"
            contact_info: "<your_own_value>"
            engine_id: "<your_own_value>"
            trap_high_cpu_threshold: "16"
            trap_high_mem_threshold: "17"
            user:
             -
                auth_proto: "md5"
                auth_pwd: "<your_own_value>"
                name: "default_name_21"
                notify_hosts: "<your_own_value>"
                priv_proto: "aes"
                priv_pwd: "<your_own_value>"
                queries: "enable"
                security_level: "no-auth-no-priv"
                status: "enable"
                trap_status: "enable"


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
