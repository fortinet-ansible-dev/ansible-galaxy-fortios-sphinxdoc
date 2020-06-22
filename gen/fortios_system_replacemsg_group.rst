:source: fortios_system_replacemsg_group.py

:orphan:

.. fortios_system_replacemsg_group:

fortios_system_replacemsg_group -- Configure replacement message groups in Fortinet's FortiOS and FortiGate.
++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++

.. versionadded:: 2.9

.. contents::
   :local:
   :depth: 1


Synopsis
--------
- This module is able to configure a FortiGate or FortiOS (FOS) device by allowing the user to set and modify system feature and replacemsg_group category. Examples include all parameters and values need to be adjusted to datasources before usage. Tested with FOS v6.0.5



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
    <li> <span class="li-head">system_replacemsg_group</span> - Configure replacement message groups. <span class="li-normal">type: dict</span></li>
        <ul class="ul-self">
        <li> <span class="li-head">admin</span> - Replacement message table entries. <span class="li-normal">type: list</span></li>
            <ul class="ul-self">
            <li> <span class="li-head">buffer</span> - Message string. <span class="li-normal">type: str</span></li>
            <li> <span class="li-head">format</span> - Format flag. <span class="li-normal">type: str</span> <span class="li-normal">choices: none, text, html, wml</span></li>
            <li> <span class="li-head">header</span> - Header flag. <span class="li-normal">type: str</span> <span class="li-normal">choices: none, http, 8bit</span></li>
            <li> <span class="li-head">msg_type</span> - Message type. <span class="li-normal">type: str</span></li>
            </ul>
        <li> <span class="li-head">alertmail</span> - Replacement message table entries. <span class="li-normal">type: list</span></li>
            <ul class="ul-self">
            <li> <span class="li-head">buffer</span> - Message string. <span class="li-normal">type: str</span></li>
            <li> <span class="li-head">format</span> - Format flag. <span class="li-normal">type: str</span> <span class="li-normal">choices: none, text, html, wml</span></li>
            <li> <span class="li-head">header</span> - Header flag. <span class="li-normal">type: str</span> <span class="li-normal">choices: none, http, 8bit</span></li>
            <li> <span class="li-head">msg_type</span> - Message type. <span class="li-normal">type: str</span></li>
            </ul>
        <li> <span class="li-head">auth</span> - Replacement message table entries. <span class="li-normal">type: list</span></li>
            <ul class="ul-self">
            <li> <span class="li-head">buffer</span> - Message string. <span class="li-normal">type: str</span></li>
            <li> <span class="li-head">format</span> - Format flag. <span class="li-normal">type: str</span> <span class="li-normal">choices: none, text, html, wml</span></li>
            <li> <span class="li-head">header</span> - Header flag. <span class="li-normal">type: str</span> <span class="li-normal">choices: none, http, 8bit</span></li>
            <li> <span class="li-head">msg_type</span> - Message type. <span class="li-normal">type: str</span></li>
            </ul>
        <li> <span class="li-head">comment</span> - Comment. <span class="li-normal">type: str</span></li>
        <li> <span class="li-head">custom_message</span> - Replacement message table entries. <span class="li-normal">type: list</span></li>
            <ul class="ul-self">
            <li> <span class="li-head">buffer</span> - Message string. <span class="li-normal">type: str</span></li>
            <li> <span class="li-head">format</span> - Format flag. <span class="li-normal">type: str</span> <span class="li-normal">choices: none, text, html, wml</span></li>
            <li> <span class="li-head">header</span> - Header flag. <span class="li-normal">type: str</span> <span class="li-normal">choices: none, http, 8bit</span></li>
            <li> <span class="li-head">msg_type</span> - Message type. <span class="li-normal">type: str</span></li>
            </ul>
        <li> <span class="li-head">device_detection_portal</span> - Replacement message table entries. <span class="li-normal">type: list</span></li>
            <ul class="ul-self">
            <li> <span class="li-head">buffer</span> - Message string. <span class="li-normal">type: str</span></li>
            <li> <span class="li-head">format</span> - Format flag. <span class="li-normal">type: str</span> <span class="li-normal">choices: none, text, html, wml</span></li>
            <li> <span class="li-head">header</span> - Header flag. <span class="li-normal">type: str</span> <span class="li-normal">choices: none, http, 8bit</span></li>
            <li> <span class="li-head">msg_type</span> - Message type. <span class="li-normal">type: str</span></li>
            </ul>
        <li> <span class="li-head">ec</span> - Replacement message table entries. <span class="li-normal">type: list</span></li>
            <ul class="ul-self">
            <li> <span class="li-head">buffer</span> - Message string. <span class="li-normal">type: str</span></li>
            <li> <span class="li-head">format</span> - Format flag. <span class="li-normal">type: str</span> <span class="li-normal">choices: none, text, html, wml</span></li>
            <li> <span class="li-head">header</span> - Header flag. <span class="li-normal">type: str</span> <span class="li-normal">choices: none, http, 8bit</span></li>
            <li> <span class="li-head">msg_type</span> - Message type. <span class="li-normal">type: str</span></li>
            </ul>
        <li> <span class="li-head">fortiguard_wf</span> - Replacement message table entries. <span class="li-normal">type: list</span></li>
            <ul class="ul-self">
            <li> <span class="li-head">buffer</span> - Message string. <span class="li-normal">type: str</span></li>
            <li> <span class="li-head">format</span> - Format flag. <span class="li-normal">type: str</span> <span class="li-normal">choices: none, text, html, wml</span></li>
            <li> <span class="li-head">header</span> - Header flag. <span class="li-normal">type: str</span> <span class="li-normal">choices: none, http, 8bit</span></li>
            <li> <span class="li-head">msg_type</span> - Message type. <span class="li-normal">type: str</span></li>
            </ul>
        <li> <span class="li-head">ftp</span> - Replacement message table entries. <span class="li-normal">type: list</span></li>
            <ul class="ul-self">
            <li> <span class="li-head">buffer</span> - Message string. <span class="li-normal">type: str</span></li>
            <li> <span class="li-head">format</span> - Format flag. <span class="li-normal">type: str</span> <span class="li-normal">choices: none, text, html, wml</span></li>
            <li> <span class="li-head">header</span> - Header flag. <span class="li-normal">type: str</span> <span class="li-normal">choices: none, http, 8bit</span></li>
            <li> <span class="li-head">msg_type</span> - Message type. <span class="li-normal">type: str</span></li>
            </ul>
        <li> <span class="li-head">group_type</span> - Group type. <span class="li-normal">type: str</span> <span class="li-normal">choices: default, utm, auth, ec</span></li>
        <li> <span class="li-head">http</span> - Replacement message table entries. <span class="li-normal">type: list</span></li>
            <ul class="ul-self">
            <li> <span class="li-head">buffer</span> - Message string. <span class="li-normal">type: str</span></li>
            <li> <span class="li-head">format</span> - Format flag. <span class="li-normal">type: str</span> <span class="li-normal">choices: none, text, html, wml</span></li>
            <li> <span class="li-head">header</span> - Header flag. <span class="li-normal">type: str</span> <span class="li-normal">choices: none, http, 8bit</span></li>
            <li> <span class="li-head">msg_type</span> - Message type. <span class="li-normal">type: str</span></li>
            </ul>
        <li> <span class="li-head">icap</span> - Replacement message table entries. <span class="li-normal">type: list</span></li>
            <ul class="ul-self">
            <li> <span class="li-head">buffer</span> - Message string. <span class="li-normal">type: str</span></li>
            <li> <span class="li-head">format</span> - Format flag. <span class="li-normal">type: str</span> <span class="li-normal">choices: none, text, html, wml</span></li>
            <li> <span class="li-head">header</span> - Header flag. <span class="li-normal">type: str</span> <span class="li-normal">choices: none, http, 8bit</span></li>
            <li> <span class="li-head">msg_type</span> - Message type. <span class="li-normal">type: str</span></li>
            </ul>
        <li> <span class="li-head">mail</span> - Replacement message table entries. <span class="li-normal">type: list</span></li>
            <ul class="ul-self">
            <li> <span class="li-head">buffer</span> - Message string. <span class="li-normal">type: str</span></li>
            <li> <span class="li-head">format</span> - Format flag. <span class="li-normal">type: str</span> <span class="li-normal">choices: none, text, html, wml</span></li>
            <li> <span class="li-head">header</span> - Header flag. <span class="li-normal">type: str</span> <span class="li-normal">choices: none, http, 8bit</span></li>
            <li> <span class="li-head">msg_type</span> - Message type. <span class="li-normal">type: str</span></li>
            </ul>
        <li> <span class="li-head">nac_quar</span> - Replacement message table entries. <span class="li-normal">type: list</span></li>
            <ul class="ul-self">
            <li> <span class="li-head">buffer</span> - Message string. <span class="li-normal">type: str</span></li>
            <li> <span class="li-head">format</span> - Format flag. <span class="li-normal">type: str</span> <span class="li-normal">choices: none, text, html, wml</span></li>
            <li> <span class="li-head">header</span> - Header flag. <span class="li-normal">type: str</span> <span class="li-normal">choices: none, http, 8bit</span></li>
            <li> <span class="li-head">msg_type</span> - Message type. <span class="li-normal">type: str</span></li>
            </ul>
        <li> <span class="li-head">name</span> - Group name. <span class="li-normal">type: str</span> <span class="li-required">required: True</span></li>
        <li> <span class="li-head">nntp</span> - Replacement message table entries. <span class="li-normal">type: list</span></li>
            <ul class="ul-self">
            <li> <span class="li-head">buffer</span> - Message string. <span class="li-normal">type: str</span></li>
            <li> <span class="li-head">format</span> - Format flag. <span class="li-normal">type: str</span> <span class="li-normal">choices: none, text, html, wml</span></li>
            <li> <span class="li-head">header</span> - Header flag. <span class="li-normal">type: str</span> <span class="li-normal">choices: none, http, 8bit</span></li>
            <li> <span class="li-head">msg_type</span> - Message type. <span class="li-normal">type: str</span></li>
            </ul>
        <li> <span class="li-head">spam</span> - Replacement message table entries. <span class="li-normal">type: list</span></li>
            <ul class="ul-self">
            <li> <span class="li-head">buffer</span> - Message string. <span class="li-normal">type: str</span></li>
            <li> <span class="li-head">format</span> - Format flag. <span class="li-normal">type: str</span> <span class="li-normal">choices: none, text, html, wml</span></li>
            <li> <span class="li-head">header</span> - Header flag. <span class="li-normal">type: str</span> <span class="li-normal">choices: none, http, 8bit</span></li>
            <li> <span class="li-head">msg_type</span> - Message type. <span class="li-normal">type: str</span></li>
            </ul>
        <li> <span class="li-head">sslvpn</span> - Replacement message table entries. <span class="li-normal">type: list</span></li>
            <ul class="ul-self">
            <li> <span class="li-head">buffer</span> - Message string. <span class="li-normal">type: str</span></li>
            <li> <span class="li-head">format</span> - Format flag. <span class="li-normal">type: str</span> <span class="li-normal">choices: none, text, html, wml</span></li>
            <li> <span class="li-head">header</span> - Header flag. <span class="li-normal">type: str</span> <span class="li-normal">choices: none, http, 8bit</span></li>
            <li> <span class="li-head">msg_type</span> - Message type. <span class="li-normal">type: str</span></li>
            </ul>
        <li> <span class="li-head">traffic_quota</span> - Replacement message table entries. <span class="li-normal">type: list</span></li>
            <ul class="ul-self">
            <li> <span class="li-head">buffer</span> - Message string. <span class="li-normal">type: str</span></li>
            <li> <span class="li-head">format</span> - Format flag. <span class="li-normal">type: str</span> <span class="li-normal">choices: none, text, html, wml</span></li>
            <li> <span class="li-head">header</span> - Header flag. <span class="li-normal">type: str</span> <span class="li-normal">choices: none, http, 8bit</span></li>
            <li> <span class="li-head">msg_type</span> - Message type. <span class="li-normal">type: str</span></li>
            </ul>
        <li> <span class="li-head">utm</span> - Replacement message table entries. <span class="li-normal">type: list</span></li>
            <ul class="ul-self">
            <li> <span class="li-head">buffer</span> - Message string. <span class="li-normal">type: str</span></li>
            <li> <span class="li-head">format</span> - Format flag. <span class="li-normal">type: str</span> <span class="li-normal">choices: none, text, html, wml</span></li>
            <li> <span class="li-head">header</span> - Header flag. <span class="li-normal">type: str</span> <span class="li-normal">choices: none, http, 8bit</span></li>
            <li> <span class="li-head">msg_type</span> - Message type. <span class="li-normal">type: str</span></li>
            </ul>
        <li> <span class="li-head">webproxy</span> - Replacement message table entries. <span class="li-normal">type: list</span></li>
            <ul class="ul-self">
            <li> <span class="li-head">buffer</span> - Message string. <span class="li-normal">type: str</span></li>
            <li> <span class="li-head">format</span> - Format flag. <span class="li-normal">type: str</span> <span class="li-normal">choices: none, text, html, wml</span></li>
            <li> <span class="li-head">header</span> - Header flag. <span class="li-normal">type: str</span> <span class="li-normal">choices: none, http, 8bit</span></li>
            <li> <span class="li-head">msg_type</span> - Message type. <span class="li-normal">type: str</span></li>
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
      - name: Configure replacement message groups.
        fortios_system_replacemsg_group:
          vdom:  "{{ vdom }}"
          state: "present"
          system_replacemsg_group:
            admin:
             -
                buffer: "<your_own_value>"
                format: "none"
                header: "none"
                msg_type: "<your_own_value>"
            alertmail:
             -
                buffer: "<your_own_value>"
                format: "none"
                header: "none"
                msg_type: "<your_own_value>"
            auth:
             -
                buffer: "<your_own_value>"
                format: "none"
                header: "none"
                msg_type: "<your_own_value>"
            comment: "Comment."
            custom_message:
             -
                buffer: "<your_own_value>"
                format: "none"
                header: "none"
                msg_type: "<your_own_value>"
            device_detection_portal:
             -
                buffer: "<your_own_value>"
                format: "none"
                header: "none"
                msg_type: "<your_own_value>"
            ec:
             -
                buffer: "<your_own_value>"
                format: "none"
                header: "none"
                msg_type: "<your_own_value>"
            fortiguard_wf:
             -
                buffer: "<your_own_value>"
                format: "none"
                header: "none"
                msg_type: "<your_own_value>"
            ftp:
             -
                buffer: "<your_own_value>"
                format: "none"
                header: "none"
                msg_type: "<your_own_value>"
            group_type: "default"
            http:
             -
                buffer: "<your_own_value>"
                format: "none"
                header: "none"
                msg_type: "<your_own_value>"
            icap:
             -
                buffer: "<your_own_value>"
                format: "none"
                header: "none"
                msg_type: "<your_own_value>"
            mail:
             -
                buffer: "<your_own_value>"
                format: "none"
                header: "none"
                msg_type: "<your_own_value>"
            nac_quar:
             -
                buffer: "<your_own_value>"
                format: "none"
                header: "none"
                msg_type: "<your_own_value>"
            name: "default_name_65"
            nntp:
             -
                buffer: "<your_own_value>"
                format: "none"
                header: "none"
                msg_type: "<your_own_value>"
            spam:
             -
                buffer: "<your_own_value>"
                format: "none"
                header: "none"
                msg_type: "<your_own_value>"
            sslvpn:
             -
                buffer: "<your_own_value>"
                format: "none"
                header: "none"
                msg_type: "<your_own_value>"
            traffic_quota:
             -
                buffer: "<your_own_value>"
                format: "none"
                header: "none"
                msg_type: "<your_own_value>"
            utm:
             -
                buffer: "<your_own_value>"
                format: "none"
                header: "none"
                msg_type: "<your_own_value>"
            webproxy:
             -
                buffer: "<your_own_value>"
                format: "none"
                header: "none"
                msg_type: "<your_own_value>"


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