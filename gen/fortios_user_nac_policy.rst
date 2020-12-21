:source: fortios_user_nac_policy.py

:orphan:

.. fortios_user_nac_policy:

fortios_user_nac_policy -- Configure NAC policy matching pattern to identify matching NAC devices in Fortinet's FortiOS and FortiGate.
++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++

.. versionadded:: 2.10

.. contents::
   :local:
   :depth: 1


Synopsis
--------
- This module is able to configure a FortiGate or FortiOS (FOS) device by allowing the user to set and modify user feature and nac_policy category. Examples include all parameters and values need to be adjusted to datasources before usage. Tested with FOS v6.4.0



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
    <li> <span class="li-head">state</span> - Indicates whether to create or remove the object. <span class="li-normal">type: str</span> <span class="li-required">required: True</span> <span class="li-normal">choices: present, absent</span></li>
    <li> <span class="li-head">user_nac_policy</span> - Configure NAC policy matching pattern to identify matching NAC devices. <span class="li-normal">type: dict</span></li>
        <ul class="ul-self">
        <li> <span class="li-head">category</span> - Category of NAC policy. <span class="li-normal">type: str</span> <span class="li-normal">choices: device, firewall-user</span></li>
        <li> <span class="li-head">description</span> - Description for the NAC policy matching pattern. <span class="li-normal">type: str</span></li>
        <li> <span class="li-head">family</span> - NAC policy matching family. <span class="li-normal">type: str</span></li>
        <li> <span class="li-head">host</span> - NAC policy matching host. <span class="li-normal">type: str</span></li>
        <li> <span class="li-head">hw_vendor</span> - NAC policy matching hardware vendor. <span class="li-normal">type: str</span></li>
        <li> <span class="li-head">hw_version</span> - NAC policy matching hardware version. <span class="li-normal">type: str</span></li>
        <li> <span class="li-head">mac</span> - NAC policy matching MAC address. <span class="li-normal">type: str</span></li>
        <li> <span class="li-head">name</span> - NAC policy name. <span class="li-normal">type: str</span> <span class="li-required">required: True</span></li>
        <li> <span class="li-head">os</span> - NAC policy matching operating system. <span class="li-normal">type: str</span></li>
        <li> <span class="li-head">src</span> - NAC policy matching source. <span class="li-normal">type: str</span></li>
        <li> <span class="li-head">status</span> - Enable/disable NAC policy. <span class="li-normal">type: str</span> <span class="li-normal">choices: enable, disable</span></li>
        <li> <span class="li-head">sw_version</span> - NAC policy matching software version. <span class="li-normal">type: str</span></li>
        <li> <span class="li-head">switch_auto_auth</span> - NAC device auto authorization when discovered and nac-policy matched. <span class="li-normal">type: str</span> <span class="li-normal">choices: global, disable, enable</span></li>
        <li> <span class="li-head">switch_fortilink</span> - FortiLink interface for which this NAC policy belongs to. Source system.interface.name. <span class="li-normal">type: str</span></li>
        <li> <span class="li-head">switch_mac_policy</span> - switch-mac-policy to be applied on the matched NAC policy. Source switch-controller.mac-policy.name. <span class="li-normal">type: str</span></li>
        <li> <span class="li-head">switch_port_policy</span> - switch-port-policy to be applied on the matched NAC policy. Source switch-controller.port-policy.name. <span class="li-normal">type: str</span></li>
        <li> <span class="li-head">switch_scope</span> - List of managed FortiSwitches on which NAC policy can be applied. <span class="li-normal">type: list</span></li>
            <ul class="ul-self">
            <li> <span class="li-head">switch_id</span> - Managed FortiSwitch name from available options. Source switch-controller.managed-switch.switch-id. <span class="li-normal">type: str</span></li>
            </ul>
        <li> <span class="li-head">type</span> - NAC policy matching type. <span class="li-normal">type: str</span></li>
        <li> <span class="li-head">user</span> - NAC policy matching user. <span class="li-normal">type: str</span></li>
        <li> <span class="li-head">user_group</span> - NAC policy matching user group. Source user.group.name. <span class="li-normal">type: str</span></li>
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
      - name: Configure NAC policy matching pattern to identify matching NAC devices.
        fortios_user_nac_policy:
          vdom:  "{{ vdom }}"
          state: "present"
          access_token: "<your_own_value>"
          user_nac_policy:
            category: "device"
            description: "<your_own_value>"
            family: "<your_own_value>"
            host: "myhostname"
            hw_vendor: "<your_own_value>"
            hw_version: "<your_own_value>"
            mac: "<your_own_value>"
            name: "default_name_10"
            os: "<your_own_value>"
            src: "<your_own_value>"
            status: "enable"
            sw_version: "<your_own_value>"
            switch_auto_auth: "global"
            switch_fortilink: "<your_own_value> (source system.interface.name)"
            switch_mac_policy: "<your_own_value> (source switch-controller.mac-policy.name)"
            switch_port_policy: "<your_own_value> (source switch-controller.port-policy.name)"
            switch_scope:
             -
                switch_id: "<your_own_value> (source switch-controller.managed-switch.switch-id)"
            type: "<your_own_value>"
            user: "<your_own_value>"
            user_group: "<your_own_value> (source user.group.name)"
    


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
