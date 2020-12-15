:source: fortios_switch_controller_security_policy_802_1x.py

:orphan:

.. fortios_switch_controller_security_policy_802_1x:

fortios_switch_controller_security_policy_802_1x -- Configure 802.1x MAC Authentication Bypass (MAB) policies in Fortinet's FortiOS and FortiGate.
++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++

.. versionadded:: 2.10

.. contents::
   :local:
   :depth: 1


Synopsis
--------
- This module is able to configure a FortiGate or FortiOS (FOS) device by allowing the user to set and modify switch_controller_security_policy feature and 802_1x category. Examples include all parameters and values need to be adjusted to datasources before usage. Tested with FOS v6.0.0



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
    <li> <span class="li-head">switch_controller_security_policy_802_1x</span> - Configure 802.1x MAC Authentication Bypass (MAB) policies. <span class="li-normal">type: dict</span></li>
        <ul class="ul-self">
        <li> <span class="li-head">auth_fail_vlan</span> - Enable to allow limited access to clients that cannot authenticate. <span class="li-normal">type: str</span> <span class="li-normal">choices: disable, enable</span></li>
        <li> <span class="li-head">auth_fail_vlan_id</span> - VLAN ID on which authentication failed. Source system.interface.name. <span class="li-normal">type: str</span></li>
        <li> <span class="li-head">auth_fail_vlanid</span> - VLAN ID on which authentication failed. <span class="li-normal">type: int</span></li>
        <li> <span class="li-head">eap_passthru</span> - Enable/disable EAP pass-through mode, allowing protocols (such as LLDP) to pass through ports for more flexible authentication. <span class="li-normal">type: str</span> <span class="li-normal">choices: disable, enable</span></li>
        <li> <span class="li-head">guest_auth_delay</span> - Guest authentication delay (1 - 900  sec). <span class="li-normal">type: int</span></li>
        <li> <span class="li-head">guest_vlan</span> - Enable the guest VLAN feature to allow limited access to non-802.1X-compliant clients. <span class="li-normal">type: str</span> <span class="li-normal">choices: disable, enable</span></li>
        <li> <span class="li-head">guest_vlan_id</span> - Guest VLAN name. Source system.interface.name. <span class="li-normal">type: str</span></li>
        <li> <span class="li-head">guest_vlanid</span> - Guest VLAN ID. <span class="li-normal">type: int</span></li>
        <li> <span class="li-head">mac_auth_bypass</span> - Enable/disable MAB for this policy. <span class="li-normal">type: str</span> <span class="li-normal">choices: disable, enable</span></li>
        <li> <span class="li-head">name</span> - Policy name. <span class="li-normal">type: str</span> <span class="li-required">required: True</span></li>
        <li> <span class="li-head">policy_type</span> - Policy type. <span class="li-normal">type: str</span> <span class="li-normal">choices: 802.1X</span></li>
        <li> <span class="li-head">radius_timeout_overwrite</span> - Enable to override the global RADIUS session timeout. <span class="li-normal">type: str</span> <span class="li-normal">choices: disable, enable</span></li>
        <li> <span class="li-head">security_mode</span> - Port or MAC based 802.1X security mode. <span class="li-normal">type: str</span> <span class="li-normal">choices: 802.1X, 802.1X-mac-based</span></li>
        <li> <span class="li-head">user_group</span> - Name of user-group to assign to this MAC Authentication Bypass (MAB) policy. <span class="li-normal">type: list</span></li>
            <ul class="ul-self">
            <li> <span class="li-head">name</span> - Group name. Source user.group.name. <span class="li-normal">type: str</span> <span class="li-required">required: True</span></li>
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
      - name: Configure 802.1x MAC Authentication Bypass (MAB) policies.
        fortios_switch_controller_security_policy_802_1x:
          vdom:  "{{ vdom }}"
          state: "present"
          access_token: "<your_own_value>"
          switch_controller_security_policy_802_1x:
            auth_fail_vlan: "disable"
            auth_fail_vlan_id: "<your_own_value> (source system.interface.name)"
            auth_fail_vlanid: "5"
            eap_passthru: "disable"
            guest_auth_delay: "7"
            guest_vlan: "disable"
            guest_vlan_id: "<your_own_value> (source system.interface.name)"
            guest_vlanid: "10"
            mac_auth_bypass: "disable"
            name: "default_name_12"
            policy_type: "802.1X"
            radius_timeout_overwrite: "disable"
            security_mode: "802.1X"
            user_group:
             -
                name: "default_name_17 (source user.group.name)"
    


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
