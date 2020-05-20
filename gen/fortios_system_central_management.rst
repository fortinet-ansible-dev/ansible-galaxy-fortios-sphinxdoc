:source: fortios_system_central_management.py

:orphan:

.. fortios_system_central_management:

fortios_system_central_management -- Configure central management in Fortinet's FortiOS and FortiGate.
++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++

.. versionadded:: 2.8

.. contents::
   :local:
   :depth: 1


Synopsis
--------
- This module is able to configure a FortiGate or FortiOS (FOS) device by allowing the user to set and modify system feature and central_management category. Examples include all parameters and values need to be adjusted to datasources before usage. Tested with FOS v6.0.5



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
    <li> <span class="li-head">system_central_management</span> - Configure central management. <span class="li-normal">type: dict</span></li>
        <ul class="ul-self">
        <li> <span class="li-head">allow_monitor</span> - Enable/disable allowing the central management server to remotely monitor this FortiGate <span class="li-normal">type: str</span> <span class="li-normal">choices: enable, disable</span></li>
        <li> <span class="li-head">allow_push_configuration</span> - Enable/disable allowing the central management server to push configuration changes to this FortiGate. <span class="li-normal">type: str</span> <span class="li-normal">choices: enable, disable</span></li>
        <li> <span class="li-head">allow_push_firmware</span> - Enable/disable allowing the central management server to push firmware updates to this FortiGate. <span class="li-normal">type: str</span> <span class="li-normal">choices: enable, disable</span></li>
        <li> <span class="li-head">allow_remote_firmware_upgrade</span> - Enable/disable remotely upgrading the firmware on this FortiGate from the central management server. <span class="li-normal">type: str</span> <span class="li-normal">choices: enable, disable</span></li>
        <li> <span class="li-head">enc_algorithm</span> - Encryption strength for communications between the FortiGate and central management. <span class="li-normal">type: str</span> <span class="li-normal">choices: default, high, low</span></li>
        <li> <span class="li-head">fmg</span> - IP address or FQDN of the FortiManager. <span class="li-normal">type: str</span></li>
        <li> <span class="li-head">fmg_source_ip</span> - IPv4 source address that this FortiGate uses when communicating with FortiManager. <span class="li-normal">type: str</span></li>
        <li> <span class="li-head">fmg_source_ip6</span> - IPv6 source address that this FortiGate uses when communicating with FortiManager. <span class="li-normal">type: str</span></li>
        <li> <span class="li-head">include_default_servers</span> - Enable/disable inclusion of public FortiGuard servers in the override server list. <span class="li-normal">type: str</span> <span class="li-normal">choices: enable, disable</span></li>
        <li> <span class="li-head">mode</span> - Central management mode. <span class="li-normal">type: str</span> <span class="li-normal">choices: normal, backup</span></li>
        <li> <span class="li-head">schedule_config_restore</span> - Enable/disable allowing the central management server to restore the configuration of this FortiGate. <span class="li-normal">type: str</span> <span class="li-normal">choices: enable, disable</span></li>
        <li> <span class="li-head">schedule_script_restore</span> - Enable/disable allowing the central management server to restore the scripts stored on this FortiGate. <span class="li-normal">type: str</span> <span class="li-normal">choices: enable, disable</span></li>
        <li> <span class="li-head">serial_number</span> - Serial number. <span class="li-normal">type: str</span></li>
        <li> <span class="li-head">server_list</span> - Additional severs that the FortiGate can use for updates (for AV, IPS, updates) and ratings (for web filter and antispam ratings) servers. <span class="li-normal">type: list</span></li>
            <ul class="ul-self">
            <li> <span class="li-head">addr_type</span> - Indicate whether the FortiGate communicates with the override server using an IPv4 address, an IPv6 address or a FQDN. <span class="li-normal">type: str</span> <span class="li-normal">choices: ipv4, ipv6, fqdn</span></li>
            <li> <span class="li-head">fqdn</span> - FQDN address of override server. <span class="li-normal">type: str</span></li>
            <li> <span class="li-head">id</span> - ID. <span class="li-normal">type: int</span> <span class="li-required">required: True</span></li>
            <li> <span class="li-head">server_address</span> - IPv4 address of override server. <span class="li-normal">type: str</span></li>
            <li> <span class="li-head">server_address6</span> - IPv6 address of override server. <span class="li-normal">type: str</span></li>
            <li> <span class="li-head">server_type</span> - FortiGuard service type. <span class="li-normal">type: str</span> <span class="li-normal">choices: update, rating</span></li>
            </ul>
        <li> <span class="li-head">type</span> - Central management type. <span class="li-normal">type: str</span> <span class="li-normal">choices: fortimanager, fortiguard, none</span></li>
        <li> <span class="li-head">vdom</span> - Virtual domain (VDOM) name to use when communicating with FortiManager. Source system.vdom.name. <span class="li-normal">type: str</span></li>
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
      - name: Configure central management.
        fortios_system_central_management:
          vdom:  "{{ vdom }}"
          system_central_management:
            allow_monitor: "enable"
            allow_push_configuration: "enable"
            allow_push_firmware: "enable"
            allow_remote_firmware_upgrade: "enable"
            enc_algorithm: "default"
            fmg: "<your_own_value>"
            fmg_source_ip: "<your_own_value>"
            fmg_source_ip6: "<your_own_value>"
            include_default_servers: "enable"
            mode: "normal"
            schedule_config_restore: "enable"
            schedule_script_restore: "enable"
            serial_number: "<your_own_value>"
            server_list:
             -
                addr_type: "ipv4"
                fqdn: "<your_own_value>"
                id:  "19"
                server_address: "<your_own_value>"
                server_address6: "<your_own_value>"
                server_type: "update"
            type: "fortimanager"
            vdom: "<your_own_value> (source system.vdom.name)"


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
