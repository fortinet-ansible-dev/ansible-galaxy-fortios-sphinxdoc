:source: fortios_switch_controller_location.py

:orphan:

.. fortios_switch_controller_location:

fortios_switch_controller_location -- Configure FortiSwitch location services in Fortinet's FortiOS and FortiGate.
++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++

.. versionadded:: 2.10

.. contents::
   :local:
   :depth: 1


Synopsis
--------
- This module is able to configure a FortiGate or FortiOS (FOS) device by allowing the user to set and modify switch_controller feature and location category. Examples include all parameters and values need to be adjusted to datasources before usage. Tested with FOS v6.4.0



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
    <li> <span class="li-head">switch_controller_location</span> - Configure FortiSwitch location services. <span class="li-normal">type: dict</span></li>
        <ul class="ul-self">
        <li> <span class="li-head">address_civic</span> - Configure location civic address. <span class="li-normal">type: dict</span></li>
            <ul class="ul-self">
            <li> <span class="li-head">additional</span> - Location additional details. <span class="li-normal">type: str</span></li>
            <li> <span class="li-head">additional_code</span> - Location additional code details. <span class="li-normal">type: str</span></li>
            <li> <span class="li-head">block</span> - Location block details. <span class="li-normal">type: str</span></li>
            <li> <span class="li-head">branch_road</span> - Location branch road details. <span class="li-normal">type: str</span></li>
            <li> <span class="li-head">building</span> - Location building details. <span class="li-normal">type: str</span></li>
            <li> <span class="li-head">city</span> - Location city details. <span class="li-normal">type: str</span></li>
            <li> <span class="li-head">city_division</span> - Location city division details. <span class="li-normal">type: str</span></li>
            <li> <span class="li-head">country</span> - The two-letter ISO 3166 country code in capital ASCII letters eg. US, CA, DK, DE. <span class="li-normal">type: str</span></li>
            <li> <span class="li-head">country_subdivision</span> - National subdivisions (state, canton, region, province, or prefecture). <span class="li-normal">type: str</span></li>
            <li> <span class="li-head">county</span> - County, parish, gun (JP), or district (IN). <span class="li-normal">type: str</span></li>
            <li> <span class="li-head">direction</span> - Leading street direction. <span class="li-normal">type: str</span></li>
            <li> <span class="li-head">floor</span> - Floor. <span class="li-normal">type: str</span></li>
            <li> <span class="li-head">landmark</span> - Landmark or vanity address. <span class="li-normal">type: str</span></li>
            <li> <span class="li-head">language</span> - Language. <span class="li-normal">type: str</span></li>
            <li> <span class="li-head">name</span> - Name (residence and office occupant). <span class="li-normal">type: str</span></li>
            <li> <span class="li-head">number</span> - House number. <span class="li-normal">type: str</span></li>
            <li> <span class="li-head">number_suffix</span> - House number suffix. <span class="li-normal">type: str</span></li>
            <li> <span class="li-head">place_type</span> - Placetype. <span class="li-normal">type: str</span></li>
            <li> <span class="li-head">post_office_box</span> - Post office box (P.O. box). <span class="li-normal">type: str</span></li>
            <li> <span class="li-head">postal_community</span> - Postal community name. <span class="li-normal">type: str</span></li>
            <li> <span class="li-head">primary_road</span> - Primary road name. <span class="li-normal">type: str</span></li>
            <li> <span class="li-head">road_section</span> - Road section. <span class="li-normal">type: str</span></li>
            <li> <span class="li-head">room</span> - Room number. <span class="li-normal">type: str</span></li>
            <li> <span class="li-head">script</span> - Script used to present the address information. <span class="li-normal">type: str</span></li>
            <li> <span class="li-head">seat</span> - Seat number. <span class="li-normal">type: str</span></li>
            <li> <span class="li-head">street</span> - Street. <span class="li-normal">type: str</span></li>
            <li> <span class="li-head">street_name_post_mod</span> - Street name post modifier. <span class="li-normal">type: str</span></li>
            <li> <span class="li-head">street_name_pre_mod</span> - Street name pre modifier. <span class="li-normal">type: str</span></li>
            <li> <span class="li-head">street_suffix</span> - Street suffix. <span class="li-normal">type: str</span></li>
            <li> <span class="li-head">sub_branch_road</span> - Sub branch road name. <span class="li-normal">type: str</span></li>
            <li> <span class="li-head">trailing_str_suffix</span> - Trailing street suffix. <span class="li-normal">type: str</span></li>
            <li> <span class="li-head">unit</span> - Unit (apartment, suite). <span class="li-normal">type: str</span></li>
            <li> <span class="li-head">zip</span> - Postal/zip code. <span class="li-normal">type: str</span></li>
            </ul>
        <li> <span class="li-head">coordinates</span> - Configure location GPS coordinates. <span class="li-normal">type: dict</span></li>
            <ul class="ul-self">
            <li> <span class="li-head">altitude</span> - +/- Floating point no. eg. 117.47. <span class="li-normal">type: str</span></li>
            <li> <span class="li-head">altitude_unit</span> - m ( meters), f ( floors). <span class="li-normal">type: str</span> <span class="li-normal">choices: m, f</span></li>
            <li> <span class="li-head">datum</span> - WGS84, NAD83, NAD83/MLLW. <span class="li-normal">type: str</span> <span class="li-normal">choices: WGS84, NAD83, NAD83/MLLW</span></li>
            <li> <span class="li-head">latitude</span> - Floating point start with ( +/- )  or end with ( N or S ) eg. +/-16.67 or 16.67N. <span class="li-normal">type: str</span></li>
            <li> <span class="li-head">longitude</span> - Floating point start with ( +/- )  or end with ( E or W ) eg. +/-26.789 or 26.789E. <span class="li-normal">type: str</span></li>
            </ul>
        <li> <span class="li-head">elin_number</span> - Configure location ELIN number. <span class="li-normal">type: dict</span></li>
            <ul class="ul-self">
            <li> <span class="li-head">elin_num</span> - Configure ELIN callback number. <span class="li-normal">type: str</span></li>
            </ul>
        <li> <span class="li-head">name</span> - Unique location item name. <span class="li-normal">type: str</span> <span class="li-required">required: True</span></li>
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
      - name: Configure FortiSwitch location services.
        fortios_switch_controller_location:
          vdom:  "{{ vdom }}"
          state: "present"
          switch_controller_location:
            address_civic:
                additional: "<your_own_value>"
                additional_code: "<your_own_value>"
                block: "<your_own_value>"
                branch_road: "<your_own_value>"
                building: "<your_own_value>"
                city: "<your_own_value>"
                city_division: "<your_own_value>"
                country: "<your_own_value>"
                country_subdivision: "<your_own_value>"
                county: "<your_own_value>"
                direction: "<your_own_value>"
                floor: "<your_own_value>"
                landmark: "<your_own_value>"
                language: "<your_own_value>"
                name: "default_name_18"
                number: "<your_own_value>"
                number_suffix: "<your_own_value>"
                place_type: "<your_own_value>"
                post_office_box: "<your_own_value>"
                postal_community: "<your_own_value>"
                primary_road: "<your_own_value>"
                road_section: "<your_own_value>"
                room: "<your_own_value>"
                script: "<your_own_value>"
                seat: "<your_own_value>"
                street: "<your_own_value>"
                street_name_post_mod: "<your_own_value>"
                street_name_pre_mod: "<your_own_value>"
                street_suffix: "<your_own_value>"
                sub_branch_road: "<your_own_value>"
                trailing_str_suffix: "<your_own_value>"
                unit: "<your_own_value>"
                zip: "<your_own_value>"
            coordinates:
                altitude: "<your_own_value>"
                altitude_unit: "m"
                datum: "WGS84"
                latitude: "<your_own_value>"
                longitude: "<your_own_value>"
            elin_number:
                elin_num: "<your_own_value>"
            name: "default_name_45"


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
