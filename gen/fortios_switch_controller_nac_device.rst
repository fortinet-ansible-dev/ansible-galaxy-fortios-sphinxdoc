:source: fortios_switch_controller_nac_device.py

:orphan:

.. fortios_switch_controller_nac_device:

fortios_switch_controller_nac_device -- Configure/list NAC devices learned on the managed FortiSwitch ports which matches NAC policy in Fortinet's FortiOS and FortiGate.
+++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++

.. versionadded:: 2.10

.. contents::
   :local:
   :depth: 1


Synopsis
--------
- This module is able to configure a FortiGate or FortiOS (FOS) device by allowing the user to set and modify switch_controller feature and nac_device category. Examples include all parameters and values need to be adjusted to datasources before usage. Tested with FOS v6.4.0



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
    <li> <span class="li-head">switch_controller_nac_device</span> - Configure/list NAC devices learned on the managed FortiSwitch ports which matches NAC policy. <span class="li-normal">type: dict</span></li>
        <ul class="ul-self">
        <li> <span class="li-head">description</span> - Description for the learned NAC device. <span class="li-normal">type: str</span></li>
        <li> <span class="li-head">id</span> - Device ID. <span class="li-normal">type: int</span> <span class="li-required">required: True</span></li>
        <li> <span class="li-head">last_known_port</span> - Managed FortiSwitch port where NAC device is last learned. <span class="li-normal">type: str</span></li>
        <li> <span class="li-head">last_known_switch</span> - Managed FortiSwitch where NAC device is last learned. Source switch-controller.managed-switch.switch-id. <span class="li-normal">type: str</span></li>
        <li> <span class="li-head">last_seen</span> - Device last seen. <span class="li-normal">type: int</span></li>
        <li> <span class="li-head">mac</span> - MAC address of the learned NAC device. <span class="li-normal">type: str</span></li>
        <li> <span class="li-head">mac_policy</span> - MAC policy to be applied on this learned NAC device. Source switch-controller.mac-policy.name. <span class="li-normal">type: str</span></li>
        <li> <span class="li-head">matched_nac_policy</span> - Matched NAC policy for the learned NAC device. Source user.nac-policy.name. <span class="li-normal">type: str</span></li>
        <li> <span class="li-head">port_policy</span> - Port policy to be applied on this learned NAC device. Source switch-controller.port-policy.name. <span class="li-normal">type: str</span></li>
        <li> <span class="li-head">status</span> - Status of the learned NAC device. Set enable to authorize the NAC device. <span class="li-normal">type: str</span> <span class="li-normal">choices: enable, disable</span></li>
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
      - name: Configure/list NAC devices learned on the managed FortiSwitch ports which matches NAC policy.
        fortios_switch_controller_nac_device:
          vdom:  "{{ vdom }}"
          state: "present"
          access_token: "<your_own_value>"
          switch_controller_nac_device:
            description: "<your_own_value>"
            id:  "4"
            last_known_port: "<your_own_value>"
            last_known_switch: "<your_own_value> (source switch-controller.managed-switch.switch-id)"
            last_seen: "7"
            mac: "<your_own_value>"
            mac_policy: "<your_own_value> (source switch-controller.mac-policy.name)"
            matched_nac_policy: "<your_own_value> (source user.nac-policy.name)"
            port_policy: "<your_own_value> (source switch-controller.port-policy.name)"
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
- Jie Xue (@JieX19)
- Hongbin Lu (@fgtdev-hblu)
- Frank Shen (@frankshen01)
- Miguel Angel Munoz (@mamunozgonzalez)
- Nicolas Thomas (@thomnico)


.. hint::
    If you notice any issues in this documentation, you can create a pull request to improve it.
