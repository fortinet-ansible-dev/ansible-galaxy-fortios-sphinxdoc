:source: fortios_system_sso_admin.py

:orphan:

.. fortios_system_sso_admin:

fortios_system_sso_admin -- Configure SSO admin users in Fortinet's FortiOS and FortiGate.
++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++

.. versionadded:: 2.10

.. contents::
   :local:
   :depth: 1


Synopsis
--------
- This module is able to configure a FortiGate or FortiOS (FOS) device by allowing the user to set and modify system feature and sso_admin category. Examples include all parameters and values need to be adjusted to datasources before usage. Tested with FOS v6.2.0



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
    <li> <span class="li-head">system_sso_admin</span> - Configure SSO admin users. <span class="li-normal">type: dict</span></li>
        <ul class="ul-self">
        <li> <span class="li-head">accprofile</span> - SSO admin user access profile. Source system.accprofile.name. <span class="li-normal">type: str</span></li>
        <li> <span class="li-head">gui_dashboard</span> - GUI dashboards. <span class="li-normal">type: list</span></li>
            <ul class="ul-self">
            <li> <span class="li-head">columns</span> - Number of columns. <span class="li-normal">type: int</span></li>
            <li> <span class="li-head">id</span> - Dashboard ID. <span class="li-normal">type: int</span> <span class="li-required">required: True</span></li>
            <li> <span class="li-head">layout_type</span> - Layout type. <span class="li-normal">type: str</span> <span class="li-normal">choices: responsive, fixed</span></li>
            <li> <span class="li-head">name</span> - Dashboard name. <span class="li-normal">type: str</span></li>
            <li> <span class="li-head">permanent</span> - Permanent dashboard (can"t be removed via the GUI). <span class="li-normal">type: str</span> <span class="li-normal">choices: disable, enable</span></li>
            <li> <span class="li-head">vdom</span> - Virtual domain. Source system.vdom.name. <span class="li-normal">type: str</span></li>
            <li> <span class="li-head">widget</span> - Dashboard widgets. <span class="li-normal">type: list</span></li>
                <ul class="ul-self">
                <li> <span class="li-head">fabric_device</span> - Fabric device to monitor. <span class="li-normal">type: str</span></li>
                <li> <span class="li-head">fabric_device_widget_name</span> - Fabric device widget name. <span class="li-normal">type: str</span></li>
                <li> <span class="li-head">fabric_device_widget_visualization_type</span> - Visualization type for fabric device widget. <span class="li-normal">type: str</span></li>
                <li> <span class="li-head">fortiview_device</span> - FortiView device. <span class="li-normal">type: str</span></li>
                <li> <span class="li-head">fortiview_filters</span> - FortiView filters. <span class="li-normal">type: list</span></li>
                    <ul class="ul-self">
                    <li> <span class="li-head">id</span> - FortiView Filter ID. <span class="li-normal">type: int</span> <span class="li-required">required: True</span></li>
                    <li> <span class="li-head">key</span> - Filter key. <span class="li-normal">type: str</span></li>
                    <li> <span class="li-head">value</span> - Filter value. <span class="li-normal">type: str</span></li>
                    </ul>
                <li> <span class="li-head">fortiview_sort_by</span> - FortiView sort by. <span class="li-normal">type: str</span></li>
                <li> <span class="li-head">fortiview_timeframe</span> - FortiView timeframe. <span class="li-normal">type: str</span></li>
                <li> <span class="li-head">fortiview_type</span> - FortiView type. <span class="li-normal">type: str</span></li>
                <li> <span class="li-head">fortiview_visualization</span> - FortiView visualization. <span class="li-normal">type: str</span></li>
                <li> <span class="li-head">height</span> - Height. <span class="li-normal">type: int</span></li>
                <li> <span class="li-head">id</span> - Widget ID. <span class="li-normal">type: int</span> <span class="li-required">required: True</span></li>
                <li> <span class="li-head">industry</span> - Security Audit Rating industry. <span class="li-normal">type: str</span> <span class="li-normal">choices: default, custom</span></li>
                <li> <span class="li-head">interface</span> - Interface to monitor. Source system.interface.name. <span class="li-normal">type: str</span></li>
                <li> <span class="li-head">region</span> - Security Audit Rating region. <span class="li-normal">type: str</span> <span class="li-normal">choices: default, custom</span></li>
                <li> <span class="li-head">title</span> - Widget title. <span class="li-normal">type: str</span></li>
                <li> <span class="li-head">type</span> - Widget type. <span class="li-normal">type: str</span> <span class="li-normal">choices: sysinfo, licinfo, vminfo, forticloud, cpu-usage, memory-usage, disk-usage, log-rate, sessions, session-rate, tr-history, analytics, usb-modem, admins, security-fabric, security-fabric-ranking, ha-status, vulnerability-summary, host-scan-summary, fortiview, botnet-activity, fabric-device</span></li>
                <li> <span class="li-head">width</span> - Width. <span class="li-normal">type: int</span></li>
                <li> <span class="li-head">x_pos</span> - X position. <span class="li-normal">type: int</span></li>
                <li> <span class="li-head">y_pos</span> - Y position. <span class="li-normal">type: int</span></li>
                </ul>
            </ul>
        <li> <span class="li-head">gui_global_menu_favorites</span> - Favorite GUI menu IDs for the global VDOM. <span class="li-normal">type: list</span></li>
            <ul class="ul-self">
            <li> <span class="li-head">id</span> - Select menu ID. <span class="li-normal">type: str</span> <span class="li-required">required: True</span></li>
            </ul>
        <li> <span class="li-head">gui_new_feature_acknowledge</span> - Acknowledgement of new features. <span class="li-normal">type: list</span></li>
            <ul class="ul-self">
            <li> <span class="li-head">id</span> - Select menu ID. <span class="li-normal">type: str</span> <span class="li-required">required: True</span></li>
            </ul>
        <li> <span class="li-head">gui_vdom_menu_favorites</span> - Favorite GUI menu IDs for VDOMs. <span class="li-normal">type: list</span></li>
            <ul class="ul-self">
            <li> <span class="li-head">id</span> - Select menu ID. <span class="li-normal">type: str</span> <span class="li-required">required: True</span></li>
            </ul>
        <li> <span class="li-head">name</span> - SSO admin name. <span class="li-normal">type: str</span> <span class="li-required">required: True</span></li>
        <li> <span class="li-head">vdom</span> - Virtual domain(s) that the administrator can access. <span class="li-normal">type: list</span></li>
            <ul class="ul-self">
            <li> <span class="li-head">name</span> - Virtual domain name. Source system.vdom.name. <span class="li-normal">type: str</span> <span class="li-required">required: True</span></li>
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
      - name: Configure SSO admin users.
        fortios_system_sso_admin:
          vdom:  "{{ vdom }}"
          state: "present"
          access_token: "<your_own_value>"
          system_sso_admin:
            accprofile: "<your_own_value> (source system.accprofile.name)"
            gui_dashboard:
             -
                columns: "5"
                id:  "6"
                layout_type: "responsive"
                name: "default_name_8"
                permanent: "disable"
                vdom: "<your_own_value> (source system.vdom.name)"
                widget:
                 -
                    fabric_device: "<your_own_value>"
                    fabric_device_widget_name: "<your_own_value>"
                    fabric_device_widget_visualization_type: "<your_own_value>"
                    fortiview_device: "<your_own_value>"
                    fortiview_filters:
                     -
                        id:  "17"
                        key: "<your_own_value>"
                        value: "<your_own_value>"
                    fortiview_sort_by: "<your_own_value>"
                    fortiview_timeframe: "<your_own_value>"
                    fortiview_type: "<your_own_value>"
                    fortiview_visualization: "<your_own_value>"
                    height: "24"
                    id:  "25"
                    industry: "default"
                    interface: "<your_own_value> (source system.interface.name)"
                    region: "default"
                    title: "<your_own_value>"
                    type: "sysinfo"
                    width: "31"
                    x_pos: "32"
                    y_pos: "33"
            gui_global_menu_favorites:
             -
                id:  "35"
            gui_new_feature_acknowledge:
             -
                id:  "37"
            gui_vdom_menu_favorites:
             -
                id:  "39"
            name: "default_name_40"
            vdom:
             -
                name: "default_name_42 (source system.vdom.name)"
    


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
