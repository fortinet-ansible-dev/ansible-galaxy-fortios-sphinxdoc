:source: fortios_report_chart.py

:orphan:

.. fortios_report_chart:

fortios_report_chart -- Report chart widget configuration in Fortinet's FortiOS and FortiGate.
++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++

.. versionadded:: 2.8

.. contents::
   :local:
   :depth: 1


Synopsis
--------
- This module is able to configure a FortiGate or FortiOS (FOS) device by allowing the user to set and modify report feature and chart category. Examples include all parameters and values need to be adjusted to datasources before usage. Tested with FOS v6.0.0



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
    <li> <span class="li-head">report_chart</span> - Report chart widget configuration. <span class="li-normal">type: dict</span></li>
        <ul class="ul-self">
        <li> <span class="li-head">state</span> - B(Deprecated) <span class="li-normal">type: str</span> <span class="li-required">required: False</span> <span class="li-normal">choices: present, absent</span></li>
        <li> <span class="li-head">background</span> - Chart background. <span class="li-normal">type: str</span></li>
        <li> <span class="li-head">category</span> - Category. <span class="li-normal">type: str</span> <span class="li-normal">choices: misc, traffic, event, virus, webfilter, attack, spam, dlp, app-ctrl, vulnerability</span></li>
        <li> <span class="li-head">category_series</span> - Category series of pie chart. <span class="li-normal">type: dict</span></li>
            <ul class="ul-self">
            <li> <span class="li-head">databind</span> - Category series value expression. <span class="li-normal">type: str</span></li>
            <li> <span class="li-head">font_size</span> - Font size of category-series title. <span class="li-normal">type: int</span></li>
            </ul>
        <li> <span class="li-head">color_palette</span> - Color palette (system will pick color automatically by default). <span class="li-normal">type: str</span></li>
        <li> <span class="li-head">column</span> - Table column definition. <span class="li-normal">type: list</span></li>
            <ul class="ul-self">
            <li> <span class="li-head">detail_unit</span> - Detail unit of column. <span class="li-normal">type: str</span></li>
            <li> <span class="li-head">detail_value</span> - Detail value of column. <span class="li-normal">type: str</span></li>
            <li> <span class="li-head">footer_unit</span> - Footer unit of column. <span class="li-normal">type: str</span></li>
            <li> <span class="li-head">footer_value</span> - Footer value of column. <span class="li-normal">type: str</span></li>
            <li> <span class="li-head">header_value</span> - Display name of table header. <span class="li-normal">type: str</span></li>
            <li> <span class="li-head">id</span> - ID. <span class="li-normal">type: int</span> <span class="li-required">required: True</span></li>
            <li> <span class="li-head">mapping</span> - Show detail in certain display value for certain condition. <span class="li-normal">type: list</span></li>
                <ul class="ul-self">
                <li> <span class="li-head">displayname</span> - Display name. <span class="li-normal">type: str</span></li>
                <li> <span class="li-head">id</span> - id <span class="li-normal">type: int</span> <span class="li-required">required: True</span></li>
                <li> <span class="li-head">op</span> - Comparision operater. <span class="li-normal">type: str</span> <span class="li-normal">choices: none, greater, greater-equal, less, less-equal, equal, between</span></li>
                <li> <span class="li-head">value_type</span> - Value type. <span class="li-normal">type: str</span> <span class="li-normal">choices: integer, string</span></li>
                <li> <span class="li-head">value1</span> - Value 1. <span class="li-normal">type: str</span></li>
                <li> <span class="li-head">value2</span> - Value 2. <span class="li-normal">type: str</span></li>
                </ul>
            </ul>
        <li> <span class="li-head">comments</span> - Comment. <span class="li-normal">type: str</span></li>
        <li> <span class="li-head">dataset</span> - Bind dataset to chart. <span class="li-normal">type: str</span></li>
        <li> <span class="li-head">dimension</span> - Dimension. <span class="li-normal">type: str</span> <span class="li-normal">choices: 2D, 3D</span></li>
        <li> <span class="li-head">drill_down_charts</span> - Drill down charts. <span class="li-normal">type: list</span></li>
            <ul class="ul-self">
            <li> <span class="li-head">chart_name</span> - Drill down chart name. <span class="li-normal">type: str</span></li>
            <li> <span class="li-head">id</span> - Drill down chart ID. <span class="li-normal">type: int</span> <span class="li-required">required: True</span></li>
            <li> <span class="li-head">status</span> - Enable/disable this drill down chart. <span class="li-normal">type: str</span> <span class="li-normal">choices: enable, disable</span></li>
            </ul>
        <li> <span class="li-head">favorite</span> - Favorite. <span class="li-normal">type: str</span> <span class="li-normal">choices: False, True</span></li>
        <li> <span class="li-head">graph_type</span> - Graph type. <span class="li-normal">type: str</span> <span class="li-normal">choices: none, bar, pie, line, flow</span></li>
        <li> <span class="li-head">legend</span> - Enable/Disable Legend area. <span class="li-normal">type: str</span> <span class="li-normal">choices: enable, disable</span></li>
        <li> <span class="li-head">legend_font_size</span> - Font size of legend area. <span class="li-normal">type: int</span></li>
        <li> <span class="li-head">name</span> - Chart Widget Name <span class="li-normal">type: str</span> <span class="li-required">required: True</span></li>
        <li> <span class="li-head">period</span> - Time period. <span class="li-normal">type: str</span> <span class="li-normal">choices: last24h, last7d</span></li>
        <li> <span class="li-head">policy</span> - Used by monitor policy. <span class="li-normal">type: int</span></li>
        <li> <span class="li-head">style</span> - Style. <span class="li-normal">type: str</span> <span class="li-normal">choices: auto, manual</span></li>
        <li> <span class="li-head">title</span> - Chart title. <span class="li-normal">type: str</span></li>
        <li> <span class="li-head">title_font_size</span> - Font size of chart title. <span class="li-normal">type: int</span></li>
        <li> <span class="li-head">type</span> - Chart type. <span class="li-normal">type: str</span> <span class="li-normal">choices: graph, table</span></li>
        <li> <span class="li-head">value_series</span> - Value series of pie chart. <span class="li-normal">type: dict</span></li>
            <ul class="ul-self">
            <li> <span class="li-head">databind</span> - Value series value expression. <span class="li-normal">type: str</span></li>
            </ul>
        <li> <span class="li-head">x_series</span> - X-series of chart. <span class="li-normal">type: dict</span></li>
            <ul class="ul-self">
            <li> <span class="li-head">caption</span> - X-series caption. <span class="li-normal">type: str</span></li>
            <li> <span class="li-head">caption_font_size</span> - X-series caption font size. <span class="li-normal">type: int</span></li>
            <li> <span class="li-head">databind</span> - X-series value expression. <span class="li-normal">type: str</span></li>
            <li> <span class="li-head">font_size</span> - X-series label font size. <span class="li-normal">type: int</span></li>
            <li> <span class="li-head">is_category</span> - X-series represent category or not. <span class="li-normal">type: str</span> <span class="li-normal">choices: True, False</span></li>
            <li> <span class="li-head">label_angle</span> - X-series label angle. <span class="li-normal">type: str</span> <span class="li-normal">choices: 45-degree, vertical, horizontal</span></li>
            <li> <span class="li-head">scale_direction</span> - Scale increase or decrease. <span class="li-normal">type: str</span> <span class="li-normal">choices: decrease, increase</span></li>
            <li> <span class="li-head">scale_format</span> - Date/time format. <span class="li-normal">type: str</span> <span class="li-normal">choices: YYYY-MM-DD-HH-MM, YYYY-MM-DD HH, YYYY-MM-DD, YYYY-MM, YYYY, HH-MM, MM-DD</span></li>
            <li> <span class="li-head">scale_step</span> - Scale step. <span class="li-normal">type: int</span></li>
            <li> <span class="li-head">scale_unit</span> - Scale unit. <span class="li-normal">type: str</span> <span class="li-normal">choices: minute, hour, day, month, year</span></li>
            <li> <span class="li-head">unit</span> - X-series unit. <span class="li-normal">type: str</span></li>
            </ul>
        <li> <span class="li-head">y_series</span> - Y-series of chart. <span class="li-normal">type: dict</span></li>
            <ul class="ul-self">
            <li> <span class="li-head">caption</span> - Y-series caption. <span class="li-normal">type: str</span></li>
            <li> <span class="li-head">caption_font_size</span> - Y-series caption font size. <span class="li-normal">type: int</span></li>
            <li> <span class="li-head">databind</span> - Y-series value expression. <span class="li-normal">type: str</span></li>
            <li> <span class="li-head">extra_databind</span> - Extra Y-series value. <span class="li-normal">type: str</span></li>
            <li> <span class="li-head">extra_y</span> - Allow another Y-series value <span class="li-normal">type: str</span> <span class="li-normal">choices: enable, disable</span></li>
            <li> <span class="li-head">extra_y_legend</span> - Extra Y-series legend type/name. <span class="li-normal">type: str</span></li>
            <li> <span class="li-head">font_size</span> - Y-series label font size. <span class="li-normal">type: int</span></li>
            <li> <span class="li-head">group</span> - Y-series group option. <span class="li-normal">type: str</span></li>
            <li> <span class="li-head">label_angle</span> - Y-series label angle. <span class="li-normal">type: str</span> <span class="li-normal">choices: 45-degree, vertical, horizontal</span></li>
            <li> <span class="li-head">unit</span> - Y-series unit. <span class="li-normal">type: str</span></li>
            <li> <span class="li-head">y_legend</span> - First Y-series legend type/name. <span class="li-normal">type: str</span></li>
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
      - name: Report chart widget configuration.
        fortios_report_chart:
          vdom:  "{{ vdom }}"
          state: "present"
          report_chart:
            background: "<your_own_value>"
            category: "misc"
            category_series:
                databind: "<your_own_value>"
                font_size: "7"
            color_palette: "<your_own_value>"
            column:
             -
                detail_unit: "<your_own_value>"
                detail_value: "<your_own_value>"
                footer_unit: "<your_own_value>"
                footer_value: "<your_own_value>"
                header_value: "<your_own_value>"
                id:  "15"
                mapping:
                 -
                    displayname: "<your_own_value>"
                    id:  "18"
                    op: "none"
                    value_type: "integer"
                    value1: "<your_own_value>"
                    value2: "<your_own_value>"
            comments: "<your_own_value>"
            dataset: "<your_own_value>"
            dimension: "2D"
            drill_down_charts:
             -
                chart_name: "<your_own_value>"
                id:  "28"
                status: "enable"
            favorite: "no"
            graph_type: "none"
            legend: "enable"
            legend_font_size: "33"
            name: "default_name_34"
            period: "last24h"
            policy: "36"
            style: "auto"
            title: "<your_own_value>"
            title_font_size: "39"
            type: "graph"
            value_series:
                databind: "<your_own_value>"
            x_series:
                caption: "<your_own_value>"
                caption_font_size: "45"
                databind: "<your_own_value>"
                font_size: "47"
                is_category: "yes"
                label_angle: "45-degree"
                scale_direction: "decrease"
                scale_format: "YYYY-MM-DD-HH-MM"
                scale_step: "52"
                scale_unit: "minute"
                unit: "<your_own_value>"
            y_series:
                caption: "<your_own_value>"
                caption_font_size: "57"
                databind: "<your_own_value>"
                extra_databind: "<your_own_value>"
                extra_y: "enable"
                extra_y_legend: "<your_own_value>"
                font_size: "62"
                group: "<your_own_value>"
                label_angle: "45-degree"
                unit: "<your_own_value>"
                y_legend: "<your_own_value>"


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
