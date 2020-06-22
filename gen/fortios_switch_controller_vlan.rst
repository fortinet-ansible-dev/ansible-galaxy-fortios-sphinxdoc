:source: fortios_switch_controller_vlan.py

:orphan:

.. fortios_switch_controller_vlan:

fortios_switch_controller_vlan -- Configure VLANs for switch controller in Fortinet's FortiOS and FortiGate.
++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++

.. versionadded:: 2.9

.. contents::
   :local:
   :depth: 1


Synopsis
--------
- This module is able to configure a FortiGate or FortiOS (FOS) device by allowing the user to set and modify switch_controller feature and vlan category. Examples include all parameters and values need to be adjusted to datasources before usage. Tested with FOS v6.0.0



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
    <li> <span class="li-head">state</span> - Indicates whether to create or remove the object. <span class="li-normal">type: str</span> <span class="li-required">required: True</span> <span class="li-normal">choices: present, absent</span></li>
    <li> <span class="li-head">switch_controller_vlan</span> - Configure VLANs for switch controller. <span class="li-normal">type: dict</span></li>
        <ul class="ul-self">
        <li> <span class="li-head">auth</span> - Authentication. <span class="li-normal">type: str</span> <span class="li-normal">choices: radius, usergroup</span></li>
        <li> <span class="li-head">color</span> - Color of icon on the GUI. <span class="li-normal">type: int</span></li>
        <li> <span class="li-head">comments</span> - Comment. <span class="li-normal">type: str</span></li>
        <li> <span class="li-head">name</span> - Switch VLAN name. <span class="li-normal">type: str</span> <span class="li-required">required: True</span></li>
        <li> <span class="li-head">portal_message_override_group</span> - Specify captive portal replacement message override group. <span class="li-normal">type: str</span></li>
        <li> <span class="li-head">portal_message_overrides</span> - Individual message overrides. <span class="li-normal">type: dict</span></li>
            <ul class="ul-self">
            <li> <span class="li-head">auth_disclaimer_page</span> - Override auth-disclaimer-page message with message from portal-message-overrides group. <span class="li-normal">type: str</span></li>
            <li> <span class="li-head">auth_login_failed_page</span> - Override auth-login-failed-page message with message from portal-message-overrides group. <span class="li-normal">type: str</span></li>
            <li> <span class="li-head">auth_login_page</span> - Override auth-login-page message with message from portal-message-overrides group. <span class="li-normal">type: str</span></li>
            <li> <span class="li-head">auth_reject_page</span> - Override auth-reject-page message with message from portal-message-overrides group. <span class="li-normal">type: str</span></li>
            </ul>
        <li> <span class="li-head">radius_server</span> - Authentication radius server. Source user.radius.name. <span class="li-normal">type: str</span></li>
        <li> <span class="li-head">security</span> - Security. <span class="li-normal">type: str</span> <span class="li-normal">choices: open, captive-portal, 8021x</span></li>
        <li> <span class="li-head">selected_usergroups</span> - Selected user group. <span class="li-normal">type: list</span></li>
            <ul class="ul-self">
            <li> <span class="li-head">name</span> - User group name. Source user.group.name. <span class="li-normal">type: str</span> <span class="li-required">required: True</span></li>
            </ul>
        <li> <span class="li-head">usergroup</span> - Authentication usergroup. Source user.group.name. <span class="li-normal">type: str</span></li>
        <li> <span class="li-head">vdom</span> - Virtual domain, <span class="li-normal">type: str</span></li>
        <li> <span class="li-head">vlanid</span> - VLAN ID. <span class="li-normal">type: int</span></li>
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
      - name: Configure VLANs for switch controller.
        fortios_switch_controller_vlan:
          vdom:  "{{ vdom }}"
          state: "present"
          switch_controller_vlan:
            auth: "radius"
            color: "4"
            comments: "<your_own_value>"
            name: "default_name_6"
            portal_message_override_group: "<your_own_value>"
            portal_message_overrides:
                auth_disclaimer_page: "<your_own_value>"
                auth_login_failed_page: "<your_own_value>"
                auth_login_page: "<your_own_value>"
                auth_reject_page: "<your_own_value>"
            radius_server: "<your_own_value> (source user.radius.name)"
            security: "open"
            selected_usergroups:
             -
                name: "default_name_16 (source user.group.name)"
            usergroup: "<your_own_value> (source user.group.name)"
            vdom: "<your_own_value>"
            vlanid: "19"


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
