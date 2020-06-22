:source: fortios_report_style.py

:orphan:

.. fortios_report_style:

fortios_report_style -- Report style configuration in Fortinet's FortiOS and FortiGate.
+++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++

.. versionadded:: 2.8

.. contents::
   :local:
   :depth: 1


Synopsis
--------
- This module is able to configure a FortiGate or FortiOS (FOS) device by allowing the user to set and modify report feature and style category. Examples include all parameters and values need to be adjusted to datasources before usage. Tested with FOS v6.4.0



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
    <li> <span class="li-head">state</span> - Indicates whether to create or remove the object. This attribute was present already in previous version in a deeper level. It has been moved out to this outer level. <span class="li-normal">type: str</span> <span class="li-required">required: False</span> <span class="li-normal">choices: present, absent</span></li>
    <li> <span class="li-head">report_style</span> - Report style configuration. <span class="li-normal">type: dict</span></li>
        <ul class="ul-self">
        <li> <span class="li-head">state</span> - B(Deprecated) <span class="li-normal">type: str</span> <span class="li-required">required: False</span> <span class="li-normal">choices: present, absent</span></li>
        <li> <span class="li-head">align</span> - Alignment. <span class="li-normal">type: str</span> <span class="li-normal">choices: left, center, right, justify</span></li>
        <li> <span class="li-head">bg_color</span> - Background color. <span class="li-normal">type: str</span></li>
        <li> <span class="li-head">border_bottom</span> - Border bottom. <span class="li-normal">type: str</span></li>
        <li> <span class="li-head">border_left</span> - Border left. <span class="li-normal">type: str</span></li>
        <li> <span class="li-head">border_right</span> - Border right. <span class="li-normal">type: str</span></li>
        <li> <span class="li-head">border_top</span> - Border top. <span class="li-normal">type: str</span></li>
        <li> <span class="li-head">column_gap</span> - Column gap. <span class="li-normal">type: str</span></li>
        <li> <span class="li-head">column_span</span> - Column span. <span class="li-normal">type: str</span> <span class="li-normal">choices: none, all</span></li>
        <li> <span class="li-head">fg_color</span> - Foreground color. <span class="li-normal">type: str</span></li>
        <li> <span class="li-head">font_family</span> - Font family. <span class="li-normal">type: str</span> <span class="li-normal">choices: Verdana, Arial, Helvetica, Courier, Times</span></li>
        <li> <span class="li-head">font_size</span> - Font size. <span class="li-normal">type: str</span></li>
        <li> <span class="li-head">font_style</span> - Font style. <span class="li-normal">type: str</span> <span class="li-normal">choices: normal, italic</span></li>
        <li> <span class="li-head">font_weight</span> - Font weight. <span class="li-normal">type: str</span> <span class="li-normal">choices: normal, bold</span></li>
        <li> <span class="li-head">height</span> - Height. <span class="li-normal">type: str</span></li>
        <li> <span class="li-head">line_height</span> - Text line height. <span class="li-normal">type: str</span></li>
        <li> <span class="li-head">margin_bottom</span> - Margin bottom. <span class="li-normal">type: str</span></li>
        <li> <span class="li-head">margin_left</span> - Margin left. <span class="li-normal">type: str</span></li>
        <li> <span class="li-head">margin_right</span> - Margin right. <span class="li-normal">type: str</span></li>
        <li> <span class="li-head">margin_top</span> - Margin top. <span class="li-normal">type: str</span></li>
        <li> <span class="li-head">name</span> - Report style name. <span class="li-normal">type: str</span> <span class="li-required">required: True</span></li>
        <li> <span class="li-head">options</span> - Report style options. <span class="li-normal">type: str</span> <span class="li-normal">choices: font, text, color, align, size, margin, border, padding, column</span></li>
        <li> <span class="li-head">padding_bottom</span> - Padding bottom. <span class="li-normal">type: str</span></li>
        <li> <span class="li-head">padding_left</span> - Padding left. <span class="li-normal">type: str</span></li>
        <li> <span class="li-head">padding_right</span> - Padding right. <span class="li-normal">type: str</span></li>
        <li> <span class="li-head">padding_top</span> - Padding top. <span class="li-normal">type: str</span></li>
        <li> <span class="li-head">width</span> - Width. <span class="li-normal">type: str</span></li>
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
      - name: Report style configuration.
        fortios_report_style:
          vdom:  "{{ vdom }}"
          state: "present"
          report_style:
            align: "left"
            bg_color: "<your_own_value>"
            border_bottom: "<your_own_value>"
            border_left: "<your_own_value>"
            border_right: "<your_own_value>"
            border_top: "<your_own_value>"
            column_gap: "<your_own_value>"
            column_span: "none"
            fg_color: "<your_own_value>"
            font_family: "Verdana"
            font_size: "<your_own_value>"
            font_style: "normal"
            font_weight: "normal"
            height: "<your_own_value>"
            line_height: "<your_own_value>"
            margin_bottom: "<your_own_value>"
            margin_left: "<your_own_value>"
            margin_right: "<your_own_value>"
            margin_top: "<your_own_value>"
            name: "default_name_22"
            options: "font"
            padding_bottom: "<your_own_value>"
            padding_left: "<your_own_value>"
            padding_right: "<your_own_value>"
            padding_top: "<your_own_value>"
            width: "<your_own_value>"


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
