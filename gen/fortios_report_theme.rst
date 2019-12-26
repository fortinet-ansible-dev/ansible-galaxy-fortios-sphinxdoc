:source: fortios_report_theme.py

:orphan:

.. _fortios_report_theme:

fortios_report_theme -- Report themes configuration in Fortinet's FortiOS and FortiGate.
++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++

.. versionadded:: 2.8

.. contents::
   :local:
   :depth: 1


Synopsis
--------
- This module is able to configure a FortiGate or FortiOS (FOS) device by allowing the user to set and modify report feature and theme category. Examples include all parameters and values need to be adjusted to datasources before usage. Tested with FOS v6.0.5


Requirements
------------
The below requirements are needed on the host that executes this module.

- fortiosapi>=0.9.8


Parameters
----------

.. raw:: html

    <ul>

    <li><span class="li-head">host</span> - FortiOS or FortiGate IP address. <span class="li-normal">type: str</span> <span class="li-required">required: false</span></li>
    <li><span class="li-head">username</span> - FortiOS or FortiGate username. <span class="li-normal">type: str</span> <span class="li-required">required: false</span></li>
    <li><span class="li-head">password</span> - FortiOS or FortiGate password. <span class="li-normal">type: str</span> <span class="li-normal">default: ""</span></li>
    <li><span class="li-head">vdom</span> - Virtual domain, among those defined previously. A vdom is a virtual instance of the FortiGate that can be configured and used as a different unit. <span class="li-normal">type: str</span> <span class="li-normal">default: root</span></li>
    <li><span class="li-head">https</span> - Indicates if the requests towards FortiGate must use HTTPS protocol. <span class="li-normal">type: bool</span> <span class="li-normal">default: true</span></li>
    <li><span class="li-head">ssl_verify</span> - Ensures FortiGate certificate must be verified by a proper CA. <span class="li-normal">type: bool</span> <span class="li-normal">default: true</span></li>
    <li><span class="li-head">state</span> - Indicates whether to create or remove the object. This attribute was present already in previous version in a deeper level. It has been moved out to this outer level. <span class="li-normal">type: str</span> <span class="li-required">required: false</span> <span class="li-normal">choices: present,  absent</span></li>
    <li><span class="li-head">report_theme</span> - Report themes configuration <span class="li-normal">default: null</span> <span class="li-normal">type: dict</span></li>
            <ul class="ul-self">

            <li><span class="li-head">state</span> - B(Deprecated) Starting with Ansible 2.9 we recommend using the top-level 'state' parameter. HORIZONTALLINE Indicates whether to create or remove the object. <span class="li-normal">type: str</span> <span class="li-required">required: false</span> <span class="li-normal">choices: present,  absent</span></li>
            <li><span class="li-head">bullet_list_style</span> - Bullet list style. <span class="li-normal">type: str</span></li>
            <li><span class="li-head">column_count</span> - Report page column count. <span class="li-normal">type: str</span> <span class="li-normal">choices: 1,  2,  3</span></li>
            <li><span class="li-head">default_html_style</span> - Default HTML report style. <span class="li-normal">type: str</span></li>
            <li><span class="li-head">default_pdf_style</span> - Default PDF report style. <span class="li-normal">type: str</span></li>
            <li><span class="li-head">graph_chart_style</span> - Graph chart style. <span class="li-normal">type: str</span></li>
            <li><span class="li-head">heading1_style</span> - Report heading style. <span class="li-normal">type: str</span></li>
            <li><span class="li-head">heading2_style</span> - Report heading style. <span class="li-normal">type: str</span></li>
            <li><span class="li-head">heading3_style</span> - Report heading style. <span class="li-normal">type: str</span></li>
            <li><span class="li-head">heading4_style</span> - Report heading style. <span class="li-normal">type: str</span></li>
            <li><span class="li-head">hline_style</span> - Horizontal line style. <span class="li-normal">type: str</span></li>
            <li><span class="li-head">image_style</span> - Image style. <span class="li-normal">type: str</span></li>
            <li><span class="li-head">name</span> - Report theme name. <span class="li-required">required</span> <span class="li-normal">type: str</span></li>
            <li><span class="li-head">normal_text_style</span> - Normal text style. <span class="li-normal">type: str</span></li>
            <li><span class="li-head">numbered_list_style</span> - Numbered list style. <span class="li-normal">type: str</span></li>
            <li><span class="li-head">page_footer_style</span> - Report page footer style. <span class="li-normal">type: str</span></li>
            <li><span class="li-head">page_header_style</span> - Report page header style. <span class="li-normal">type: str</span></li>
            <li><span class="li-head">page_orient</span> - Report page orientation. <span class="li-normal">type: str</span> <span class="li-normal">choices: portrait,  landscape</span></li>
            <li><span class="li-head">page_style</span> - Report page style. <span class="li-normal">type: str</span></li>
            <li><span class="li-head">report_subtitle_style</span> - Report subtitle style. <span class="li-normal">type: str</span></li>
            <li><span class="li-head">report_title_style</span> - Report title style. <span class="li-normal">type: str</span></li>
            <li><span class="li-head">table_chart_caption_style</span> - Table chart caption style. <span class="li-normal">type: str</span></li>
            <li><span class="li-head">table_chart_even_row_style</span> - Table chart even row style. <span class="li-normal">type: str</span></li>
            <li><span class="li-head">table_chart_head_style</span> - Table chart head row style. <span class="li-normal">type: str</span></li>
            <li><span class="li-head">table_chart_odd_row_style</span> - Table chart odd row style. <span class="li-normal">type: str</span></li>
            <li><span class="li-head">table_chart_style</span> - Table chart style. <span class="li-normal">type: str</span></li>
            <li><span class="li-head">toc_heading1_style</span> - Table of contents heading style. <span class="li-normal">type: str</span></li>
            <li><span class="li-head">toc_heading2_style</span> - Table of contents heading style. <span class="li-normal">type: str</span></li>
            <li><span class="li-head">toc_heading3_style</span> - Table of contents heading style. <span class="li-normal">type: str</span></li>
            <li><span class="li-head">toc_heading4_style</span> - Table of contents heading style. <span class="li-normal">type: str</span></li>
            <li><span class="li-head">toc_title_style</span> - Table of contents title style. <span class="li-normal">type: str</span>
            </ul>

    </ul>




Notes
-----

.. note::


   - Requires fortiosapi library developed by Fortinet

   - Run as a local_action in your playbook



Examples
--------

.. code-block:: yaml+jinja

    - hosts: localhost
      vars:
       host: "192.168.122.40"
       username: "admin"
       password: ""
       vdom: "root"
       ssl_verify: "False"
      tasks:
      - name: Report themes configuration
        fortios_report_theme:
          host:  "{{ host }}"
          username: "{{ username }}"
          password: "{{ password }}"
          vdom:  "{{ vdom }}"
          https: "False"
          state: "present"
          report_theme:
            bullet_list_style: "<your_own_value>"
            column_count: "1"
            default_html_style: "<your_own_value>"
            default_pdf_style: "<your_own_value>"
            graph_chart_style: "<your_own_value>"
            heading1_style: "<your_own_value>"
            heading2_style: "<your_own_value>"
            heading3_style: "<your_own_value>"
            heading4_style: "<your_own_value>"
            hline_style: "<your_own_value>"
            image_style: "<your_own_value>"
            name: "default_name_14"
            normal_text_style: "<your_own_value>"
            numbered_list_style: "<your_own_value>"
            page_footer_style: "<your_own_value>"
            page_header_style: "<your_own_value>"
            page_orient: "portrait"
            page_style: "<your_own_value>"
            report_subtitle_style: "<your_own_value>"
            report_title_style: "<your_own_value>"
            table_chart_caption_style: "<your_own_value>"
            table_chart_even_row_style: "<your_own_value>"
            table_chart_head_style: "<your_own_value>"
            table_chart_odd_row_style: "<your_own_value>"
            table_chart_style: "<your_own_value>"
            toc_heading1_style: "<your_own_value>"
            toc_heading2_style: "<your_own_value>"
            toc_heading3_style: "<your_own_value>"
            toc_heading4_style: "<your_own_value>"
            toc_title_style: "<your_own_value>"



Return Values
-------------
Common return values are documented: https://docs.ansible.com/ansible/latest/reference_appendices/common_return_values.html#common-return-values, the following are the fields unique to this module:

.. raw:: html

    <ul>

    <li><span class="li-return">build</span> - Build number of the fortigate image <span class="li-normal">returned: always</span> <span class="li-normal">type: str</span> <span class="li-normal">sample: '1547'</span></li>
    <li><span class="li-return">http_method</span> - Last method used to provision the content into FortiGate <span class="li-normal">returned: always</span> <span class="li-normal">type: str</span> <span class="li-normal">sample: 'PUT'</span></li>
    <li><span class="li-return">http_status</span> - Last result given by FortiGate on last operation applied <span class="li-normal">returned: always</span> <span class="li-normal">type: str</span> <span class="li-normal">sample: 200</span></li>
    <li><span class="li-return">mkey</span> - Master key (id) used in the last call to FortiGate <span class="li-normal">returned: success</span> <span class="li-normal">type: str</span> <span class="li-normal">sample: id</span></li>
    <li><span class="li-return">name</span> - Name of the table used to fulfill the request <span class="li-normal">returned: always</span> <span class="li-normal">type: str</span> <span class="li-normal">sample: urlfilter</span></li>
    <li><span class="li-return">path</span> - Path of the table used to fulfill the request <span class="li-normal">returned: always</span> <span class="li-normal">type: str</span> <span class="li-normal">sample: webfilter</span></li>
    <li><span class="li-return">revision</span> - Internal revision number <span class="li-normal">returned: always</span> <span class="li-normal">type: str</span> <span class="li-normal">sample: 17.0.2.10658</span></li>
    <li><span class="li-return">serial</span> - Serial number of the unit <span class="li-normal">returned: always</span> <span class="li-normal">type: str</span> <span class="li-normal">sample: FGVMEVYYQT3AB5352</span></li>
    <li><span class="li-return">status</span> - Indication of the operation's result <span class="li-normal">returned: always</span> <span class="li-normal">type: str</span> <span class="li-normal">sample: success</span></li>
    <li><span class="li-return">vdom</span> - Virtual domain used <span class="li-normal">returned: always</span> <span class="li-normal">type: str</span> <span class="li-normal">sample: root</span></li>
    <li><span class="li-return">version</span> - Version of the FortiGate <span class="li-normal">returned: always</span> <span class="li-normal">type: str</span> <span class="li-normal">sample: v5.6.3</span></li>
    </ul>



Status
------

- This module is not guaranteed to have a backwards compatible interface.



Authors
-------

- Miguel Angel Munoz (@mamunozgonzalez)
- Nicolas Thomas (@thomnico)



.. hint::
    If you notice any issues in this documentation, you can create a pull request to improve it.