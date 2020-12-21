:source: fortios_switch_controller_initial_config_vlans.py

:orphan:

.. fortios_switch_controller_initial_config_vlans:

fortios_switch_controller_initial_config_vlans -- Configure initial template for auto-generated VLAN interfaces in Fortinet's FortiOS and FortiGate.
++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++

.. versionadded:: 2.10

.. contents::
   :local:
   :depth: 1


Synopsis
--------
- This module is able to configure a FortiGate or FortiOS (FOS) device by allowing the user to set and modify switch_controller_initial_config feature and vlans category. Examples include all parameters and values need to be adjusted to datasources before usage. Tested with FOS v6.4.0



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
    <li> <span class="li-head">switch_controller_initial_config_vlans</span> - Configure initial template for auto-generated VLAN interfaces. <span class="li-normal">type: dict</span></li>
        <ul class="ul-self">
        <li> <span class="li-head">default_vlan</span> - Default VLAN (native) assigned to all switch ports upon discovery. Source switch-controller.initial-config.template.name. <span class="li-normal">type: str</span></li>
        <li> <span class="li-head">nac</span> - VLAN for NAC onboarding devices. Source switch-controller.initial-config.template.name. <span class="li-normal">type: str</span></li>
        <li> <span class="li-head">quarantine</span> - VLAN for quarantined traffic. Source switch-controller.initial-config.template.name. <span class="li-normal">type: str</span></li>
        <li> <span class="li-head">rspan</span> - VLAN for RSPAN/ERSPAN mirrored traffic. Source switch-controller.initial-config.template.name. <span class="li-normal">type: str</span></li>
        <li> <span class="li-head">video</span> - VLAN dedicated for video devices. Source switch-controller.initial-config.template.name. <span class="li-normal">type: str</span></li>
        <li> <span class="li-head">voice</span> - VLAN dedicated for voice devices. Source switch-controller.initial-config.template.name. <span class="li-normal">type: str</span></li>
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
      - name: Configure initial template for auto-generated VLAN interfaces.
        fortios_switch_controller_initial_config_vlans:
          vdom:  "{{ vdom }}"
          switch_controller_initial_config_vlans:
            default_vlan: "<your_own_value> (source switch-controller.initial-config.template.name)"
            nac: "<your_own_value> (source switch-controller.initial-config.template.name)"
            quarantine: "<your_own_value> (source switch-controller.initial-config.template.name)"
            rspan: "<your_own_value> (source switch-controller.initial-config.template.name)"
            video: "<your_own_value> (source switch-controller.initial-config.template.name)"
            voice: "<your_own_value> (source switch-controller.initial-config.template.name)"
    


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