:source: fortios_report_layout.py

:orphan:

.. fortios_report_layout:

fortios_report_layout -- Report layout configuration in Fortinet's FortiOS and FortiGate.
+++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++

.. versionadded:: 2.8

.. contents::
   :local:
   :depth: 1


Synopsis
--------
- This module is able to configure a FortiGate or FortiOS (FOS) device by allowing the user to set and modify report feature and layout category. Examples include all parameters and values need to be adjusted to datasources before usage. Tested with FOS v6.2.0



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
    <li> <span class="li-head">state</span> - Indicates whether to create or remove the object. This attribute was present already in previous version in a deeper level. It has been moved out to this outer level. <span class="li-normal">type: str</span> <span class="li-required">required: False</span> <span class="li-normal">choices: present, absent</span></li>
    <li> <span class="li-head">report_layout</span> - Report layout configuration. <span class="li-normal">type: dict</span></li>
        <ul class="ul-self">
        <li> <span class="li-head">state</span> - B(Deprecated) <span class="li-normal">type: str</span> <span class="li-required">required: False</span> <span class="li-normal">choices: present, absent</span></li>
        <li> <span class="li-head">body_item</span> - Configure report body item. <span class="li-normal">type: list</span></li>
            <ul class="ul-self">
            <li> <span class="li-head">chart</span> - Report item chart name. <span class="li-normal">type: str</span></li>
            <li> <span class="li-head">chart_options</span> - Report chart options. <span class="li-normal">type: str</span> <span class="li-normal">choices: include-no-data, hide-title, show-caption</span></li>
            <li> <span class="li-head">column</span> - Report section column number. <span class="li-normal">type: int</span></li>
            <li> <span class="li-head">content</span> - Report item text content. <span class="li-normal">type: str</span></li>
            <li> <span class="li-head">description</span> - Description. <span class="li-normal">type: str</span></li>
            <li> <span class="li-head">drill_down_items</span> - Control how drill down charts are shown. <span class="li-normal">type: str</span></li>
            <li> <span class="li-head">drill_down_types</span> - Control whether keys from the parent being combined or not. <span class="li-normal">type: str</span></li>
            <li> <span class="li-head">hide</span> - Enable/disable hide item in report. <span class="li-normal">type: str</span> <span class="li-normal">choices: enable, disable</span></li>
            <li> <span class="li-head">id</span> - Report item ID. <span class="li-normal">type: int</span> <span class="li-required">required: True</span></li>
            <li> <span class="li-head">img_src</span> - Report item image file name. <span class="li-normal">type: str</span></li>
            <li> <span class="li-head">list</span> - Configure report list item. <span class="li-normal">type: list</span></li>
                <ul class="ul-self">
                <li> <span class="li-head">content</span> - List entry content. <span class="li-normal">type: str</span></li>
                <li> <span class="li-head">id</span> - List entry ID. <span class="li-normal">type: int</span> <span class="li-required">required: True</span></li>
                </ul>
            <li> <span class="li-head">list_component</span> - Report item list component. <span class="li-normal">type: str</span> <span class="li-normal">choices: bullet, numbered</span></li>
            <li> <span class="li-head">misc_component</span> - Report item miscellaneous component. <span class="li-normal">type: str</span> <span class="li-normal">choices: hline, page-break, column-break, section-start</span></li>
            <li> <span class="li-head">parameters</span> - Parameters. <span class="li-normal">type: list</span></li>
                <ul class="ul-self">
                <li> <span class="li-head">id</span> - ID. <span class="li-normal">type: int</span> <span class="li-required">required: True</span></li>
                <li> <span class="li-head">name</span> - Field name that match field of parameters defined in dataset. <span class="li-normal">type: str</span></li>
                <li> <span class="li-head">value</span> - Value to replace corresponding field of parameters defined in dataset. <span class="li-normal">type: str</span></li>
                </ul>
            <li> <span class="li-head">style</span> - Report item style. <span class="li-normal">type: str</span></li>
            <li> <span class="li-head">table_caption_style</span> - Table chart caption style. <span class="li-normal">type: str</span></li>
            <li> <span class="li-head">table_column_widths</span> - Report item table column widths. <span class="li-normal">type: str</span></li>
            <li> <span class="li-head">table_even_row_style</span> - Table chart even row style. <span class="li-normal">type: str</span></li>
            <li> <span class="li-head">table_head_style</span> - Table chart head style. <span class="li-normal">type: str</span></li>
            <li> <span class="li-head">table_odd_row_style</span> - Table chart odd row style. <span class="li-normal">type: str</span></li>
            <li> <span class="li-head">text_component</span> - Report item text component. <span class="li-normal">type: str</span> <span class="li-normal">choices: text, heading1, heading2, heading3</span></li>
            <li> <span class="li-head">title</span> - Report section title. <span class="li-normal">type: str</span></li>
            <li> <span class="li-head">top_n</span> - Value of top. <span class="li-normal">type: int</span></li>
            <li> <span class="li-head">type</span> - Report item type. <span class="li-normal">type: str</span> <span class="li-normal">choices: text, image, chart, misc</span></li>
            </ul>
        <li> <span class="li-head">cutoff_option</span> - Cutoff-option is either run-time or custom. <span class="li-normal">type: str</span> <span class="li-normal">choices: run-time, custom</span></li>
        <li> <span class="li-head">cutoff_time</span> - Custom cutoff time to generate report [hh:mm]. <span class="li-normal">type: str</span></li>
        <li> <span class="li-head">day</span> - Schedule days of week to generate report. <span class="li-normal">type: str</span> <span class="li-normal">choices: sunday, monday, tuesday, wednesday, thursday, friday, saturday</span></li>
        <li> <span class="li-head">description</span> - Description. <span class="li-normal">type: str</span></li>
        <li> <span class="li-head">email_recipients</span> - Email recipients for generated reports. <span class="li-normal">type: str</span></li>
        <li> <span class="li-head">email_send</span> - Enable/disable sending emails after reports are generated. <span class="li-normal">type: str</span> <span class="li-normal">choices: enable, disable</span></li>
        <li> <span class="li-head">format</span> - Report format. <span class="li-normal">type: str</span> <span class="li-normal">choices: pdf</span></li>
        <li> <span class="li-head">max_pdf_report</span> - Maximum number of PDF reports to keep at one time (oldest report is overwritten). <span class="li-normal">type: int</span></li>
        <li> <span class="li-head">name</span> - Report layout name. <span class="li-normal">type: str</span> <span class="li-required">required: True</span></li>
        <li> <span class="li-head">options</span> - Report layout options. <span class="li-normal">type: str</span> <span class="li-normal">choices: include-table-of-content, auto-numbering-heading, view-chart-as-heading, show-html-navbar-before-heading, dummy-option</span></li>
        <li> <span class="li-head">page</span> - Configure report page. <span class="li-normal">type: dict</span></li>
            <ul class="ul-self">
            <li> <span class="li-head">column_break_before</span> - Report page auto column break before heading. <span class="li-normal">type: str</span> <span class="li-normal">choices: heading1, heading2, heading3</span></li>
            <li> <span class="li-head">footer</span> - Configure report page footer. <span class="li-normal">type: dict</span></li>
                <ul class="ul-self">
                <li> <span class="li-head">footer_item</span> - Configure report footer item. <span class="li-normal">type: list</span></li>
                    <ul class="ul-self">
                    <li> <span class="li-head">content</span> - Report item text content. <span class="li-normal">type: str</span></li>
                    <li> <span class="li-head">description</span> - Description. <span class="li-normal">type: str</span></li>
                    <li> <span class="li-head">id</span> - Report item ID. <span class="li-normal">type: int</span> <span class="li-required">required: True</span></li>
                    <li> <span class="li-head">img_src</span> - Report item image file name. <span class="li-normal">type: str</span></li>
                    <li> <span class="li-head">style</span> - Report item style. <span class="li-normal">type: str</span></li>
                    <li> <span class="li-head">type</span> - Report item type. <span class="li-normal">type: str</span> <span class="li-normal">choices: text, image</span></li>
                    </ul>
                <li> <span class="li-head">style</span> - Report footer style. <span class="li-normal">type: str</span></li>
                </ul>
            <li> <span class="li-head">header</span> - Configure report page header. <span class="li-normal">type: dict</span></li>
                <ul class="ul-self">
                <li> <span class="li-head">header_item</span> - Configure report header item. <span class="li-normal">type: list</span></li>
                    <ul class="ul-self">
                    <li> <span class="li-head">content</span> - Report item text content. <span class="li-normal">type: str</span></li>
                    <li> <span class="li-head">description</span> - Description. <span class="li-normal">type: str</span></li>
                    <li> <span class="li-head">id</span> - Report item ID. <span class="li-normal">type: int</span> <span class="li-required">required: True</span></li>
                    <li> <span class="li-head">img_src</span> - Report item image file name. <span class="li-normal">type: str</span></li>
                    <li> <span class="li-head">style</span> - Report item style. <span class="li-normal">type: str</span></li>
                    <li> <span class="li-head">type</span> - Report item type. <span class="li-normal">type: str</span> <span class="li-normal">choices: text, image</span></li>
                    </ul>
                <li> <span class="li-head">style</span> - Report header style. <span class="li-normal">type: str</span></li>
                </ul>
            <li> <span class="li-head">options</span> - Report page options. <span class="li-normal">type: str</span> <span class="li-normal">choices: header-on-first-page, footer-on-first-page</span></li>
            <li> <span class="li-head">page_break_before</span> - Report page auto page break before heading. <span class="li-normal">type: str</span> <span class="li-normal">choices: heading1, heading2, heading3</span></li>
            <li> <span class="li-head">paper</span> - Report page paper. <span class="li-normal">type: str</span> <span class="li-normal">choices: a4, letter</span></li>
            </ul>
        <li> <span class="li-head">schedule_type</span> - Report schedule type. <span class="li-normal">type: str</span> <span class="li-normal">choices: demand, daily, weekly</span></li>
        <li> <span class="li-head">style_theme</span> - Report style theme. <span class="li-normal">type: str</span></li>
        <li> <span class="li-head">subtitle</span> - Report subtitle. <span class="li-normal">type: str</span></li>
        <li> <span class="li-head">time</span> - Schedule time to generate report [hh:mm]. <span class="li-normal">type: str</span></li>
        <li> <span class="li-head">title</span> - Report title. <span class="li-normal">type: str</span></li>
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
      - name: Report layout configuration.
        fortios_report_layout:
          vdom:  "{{ vdom }}"
          state: "present"
          access_token: "<your_own_value>"
          report_layout:
            body_item:
             -
                chart: "<your_own_value>"
                chart_options: "include-no-data"
                column: "6"
                content: "<your_own_value>"
                description: "<your_own_value>"
                drill_down_items: "<your_own_value>"
                drill_down_types: "<your_own_value>"
                hide: "enable"
                id:  "12"
                img_src: "<your_own_value>"
                list:
                 -
                    content: "<your_own_value>"
                    id:  "16"
                list_component: "bullet"
                misc_component: "hline"
                parameters:
                 -
                    id:  "20"
                    name: "default_name_21"
                    value: "<your_own_value>"
                style: "<your_own_value>"
                table_caption_style: "<your_own_value>"
                table_column_widths: "<your_own_value>"
                table_even_row_style: "<your_own_value>"
                table_head_style: "<your_own_value>"
                table_odd_row_style: "<your_own_value>"
                text_component: "text"
                title: "<your_own_value>"
                top_n: "31"
                type: "text"
            cutoff_option: "run-time"
            cutoff_time: "<your_own_value>"
            day: "sunday"
            description: "<your_own_value>"
            email_recipients: "<your_own_value>"
            email_send: "enable"
            format: "pdf"
            max_pdf_report: "40"
            name: "default_name_41"
            options: "include-table-of-content"
            page:
                column_break_before: "heading1"
                footer:
                    footer_item:
                     -
                        content: "<your_own_value>"
                        description: "<your_own_value>"
                        id:  "49"
                        img_src: "<your_own_value>"
                        style: "<your_own_value>"
                        type: "text"
                    style: "<your_own_value>"
                header:
                    header_item:
                     -
                        content: "<your_own_value>"
                        description: "<your_own_value>"
                        id:  "58"
                        img_src: "<your_own_value>"
                        style: "<your_own_value>"
                        type: "text"
                    style: "<your_own_value>"
                options: "header-on-first-page"
                page_break_before: "heading1"
                paper: "a4"
            schedule_type: "demand"
            style_theme: "<your_own_value>"
            subtitle: "<your_own_value>"
            time: "<your_own_value>"
            title: "<your_own_value>"
    


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
