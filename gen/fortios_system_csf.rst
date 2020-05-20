:source: fortios_system_csf.py

:orphan:

.. fortios_system_csf:

fortios_system_csf -- Add this FortiGate to a Security Fabric or set up a new Security Fabric on this FortiGate in Fortinet's FortiOS and FortiGate.
++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++

.. versionadded:: 2.9

.. contents::
   :local:
   :depth: 1


Synopsis
--------
- This module is able to configure a FortiGate or FortiOS (FOS) device by allowing the user to set and modify system feature and csf category. Examples include all parameters and values need to be adjusted to datasources before usage. Tested with FOS v6.0.5



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
    <li> <span class="li-head">system_csf</span> - Add this FortiGate to a Security Fabric or set up a new Security Fabric on this FortiGate. <span class="li-normal">type: dict</span></li>
        <ul class="ul-self">
        <li> <span class="li-head">configuration_sync</span> - Configuration sync mode. <span class="li-normal">type: str</span> <span class="li-normal">choices: default, local</span></li>
        <li> <span class="li-head">fabric_device</span> - Fabric device configuration. <span class="li-normal">type: list</span></li>
            <ul class="ul-self">
            <li> <span class="li-head">device_ip</span> - Device IP. <span class="li-normal">type: str</span></li>
            <li> <span class="li-head">device_type</span> - Device type. <span class="li-normal">type: str</span> <span class="li-normal">choices: fortimail</span></li>
            <li> <span class="li-head">login</span> - Device login name. <span class="li-normal">type: str</span></li>
            <li> <span class="li-head">name</span> - Device name. <span class="li-normal">type: str</span> <span class="li-required">required: True</span></li>
            <li> <span class="li-head">password</span> - Device login password. <span class="li-normal">type: str</span></li>
            </ul>
        <li> <span class="li-head">fixed_key</span> - Auto-generated fixed key used when this device is the root. (Will automatically be generated if not set.) <span class="li-normal">type: str</span></li>
        <li> <span class="li-head">group_name</span> - Security Fabric group name. All FortiGates in a Security Fabric must have the same group name. <span class="li-normal">type: str</span></li>
        <li> <span class="li-head">group_password</span> - Security Fabric group password. All FortiGates in a Security Fabric must have the same group password. <span class="li-normal">type: str</span></li>
        <li> <span class="li-head">management_ip</span> - Management IP address of this FortiGate. Used to log into this FortiGate from another FortiGate in the Security Fabric. <span class="li-normal">type: str</span></li>
        <li> <span class="li-head">management_port</span> - Overriding port for management connection (Overrides admin port). <span class="li-normal">type: int</span></li>
        <li> <span class="li-head">status</span> - Enable/disable Security Fabric. <span class="li-normal">type: str</span> <span class="li-normal">choices: enable, disable</span></li>
        <li> <span class="li-head">trusted_list</span> - Pre-authorized and blocked security fabric nodes. <span class="li-normal">type: list</span></li>
            <ul class="ul-self">
            <li> <span class="li-head">action</span> - Security fabric authorization action. <span class="li-normal">type: str</span> <span class="li-normal">choices: accept, deny</span></li>
            <li> <span class="li-head">downstream_authorization</span> - Trust authorizations by this node"s administrator. <span class="li-normal">type: str</span> <span class="li-normal">choices: enable, disable</span></li>
            <li> <span class="li-head">ha_members</span> - HA members. <span class="li-normal">type: str</span></li>
            <li> <span class="li-head">serial</span> - Serial. <span class="li-normal">type: str</span> <span class="li-required">required: True</span></li>
            </ul>
        <li> <span class="li-head">upstream_ip</span> - IP address of the FortiGate upstream from this FortiGate in the Security Fabric. <span class="li-normal">type: str</span></li>
        <li> <span class="li-head">upstream_port</span> - The port number to use to communicate with the FortiGate upstream from this FortiGate in the Security Fabric . <span class="li-normal">type: int</span></li>
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
      - name: Add this FortiGate to a Security Fabric or set up a new Security Fabric on this FortiGate.
        fortios_system_csf:
          vdom:  "{{ vdom }}"
          system_csf:
            configuration_sync: "default"
            fabric_device:
             -
                device_ip: "<your_own_value>"
                device_type: "fortimail"
                login: "<your_own_value>"
                name: "default_name_8"
                password: "<your_own_value>"
            fixed_key: "<your_own_value>"
            group_name: "<your_own_value>"
            group_password: "<your_own_value>"
            management_ip: "<your_own_value>"
            management_port: "14"
            status: "enable"
            trusted_list:
             -
                action: "accept"
                downstream_authorization: "enable"
                ha_members: "<your_own_value>"
                serial: "<your_own_value>"
            upstream_ip: "<your_own_value>"
            upstream_port: "22"


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
