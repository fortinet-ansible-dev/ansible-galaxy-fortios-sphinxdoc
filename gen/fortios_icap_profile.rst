:source: fortios_icap_profile.py

:orphan:

.. fortios_icap_profile:

fortios_icap_profile -- Configure ICAP profiles in Fortinet's FortiOS and FortiGate.
++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++

.. versionadded:: 2.8

.. contents::
   :local:
   :depth: 1


Synopsis
--------
- This module is able to configure a FortiGate or FortiOS (FOS) device by allowing the user to set and modify icap feature and profile category. Examples include all parameters and values need to be adjusted to datasources before usage. Tested with FOS v6.2.0



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
    <li> <span class="li-head">icap_profile</span> - Configure ICAP profiles. <span class="li-normal">type: dict</span></li>
        <ul class="ul-self">
        <li> <span class="li-head">state</span> - B(Deprecated) <span class="li-normal">type: str</span> <span class="li-required">required: False</span> <span class="li-normal">choices: present, absent</span></li>
        <li> <span class="li-head">icap_headers</span> - Configure ICAP forwarded request headers. <span class="li-normal">type: list</span></li>
            <ul class="ul-self">
            <li> <span class="li-head">base64_encoding</span> - Enable/disable use of base64 encoding of HTTP content. <span class="li-normal">type: str</span> <span class="li-normal">choices: disable, enable</span></li>
            <li> <span class="li-head">content</span> - HTTP header content. <span class="li-normal">type: str</span></li>
            <li> <span class="li-head">id</span> - HTTP forwarded header ID. <span class="li-normal">type: int</span> <span class="li-required">required: True</span></li>
            <li> <span class="li-head">name</span> - HTTP forwarded header name. <span class="li-normal">type: str</span></li>
            </ul>
        <li> <span class="li-head">methods</span> - The allowed HTTP methods that will be sent to ICAP server for further processing. <span class="li-normal">type: str</span> <span class="li-normal">choices: delete, get, head, options, post, put, trace, other</span></li>
        <li> <span class="li-head">name</span> - ICAP profile name. <span class="li-normal">type: str</span> <span class="li-required">required: True</span></li>
        <li> <span class="li-head">preview</span> - Enable/disable preview of data to ICAP server. <span class="li-normal">type: str</span> <span class="li-normal">choices: disable, enable</span></li>
        <li> <span class="li-head">preview_data_length</span> - Preview data length to be sent to ICAP server. <span class="li-normal">type: int</span></li>
        <li> <span class="li-head">replacemsg_group</span> - Replacement message group. Source system.replacemsg-group.name. <span class="li-normal">type: str</span></li>
        <li> <span class="li-head">request</span> - Enable/disable whether an HTTP request is passed to an ICAP server. <span class="li-normal">type: str</span> <span class="li-normal">choices: disable, enable</span></li>
        <li> <span class="li-head">request_failure</span> - Action to take if the ICAP server cannot be contacted when processing an HTTP request. <span class="li-normal">type: str</span> <span class="li-normal">choices: error, bypass</span></li>
        <li> <span class="li-head">request_path</span> - Path component of the ICAP URI that identifies the HTTP request processing service. <span class="li-normal">type: str</span></li>
        <li> <span class="li-head">request_server</span> - ICAP server to use for an HTTP request. Source icap.server.name. <span class="li-normal">type: str</span></li>
        <li> <span class="li-head">response</span> - Enable/disable whether an HTTP response is passed to an ICAP server. <span class="li-normal">type: str</span> <span class="li-normal">choices: disable, enable</span></li>
        <li> <span class="li-head">response_failure</span> - Action to take if the ICAP server cannot be contacted when processing an HTTP response. <span class="li-normal">type: str</span> <span class="li-normal">choices: error, bypass</span></li>
        <li> <span class="li-head">response_path</span> - Path component of the ICAP URI that identifies the HTTP response processing service. <span class="li-normal">type: str</span></li>
        <li> <span class="li-head">response_req_hdr</span> - Enable/disable addition of req-hdr for ICAP response modification (respmod) processing. <span class="li-normal">type: str</span> <span class="li-normal">choices: disable, enable</span></li>
        <li> <span class="li-head">response_server</span> - ICAP server to use for an HTTP response. Source icap.server.name. <span class="li-normal">type: str</span></li>
        <li> <span class="li-head">streaming_content_bypass</span> - Enable/disable bypassing of ICAP server for streaming content. <span class="li-normal">type: str</span> <span class="li-normal">choices: disable, enable</span></li>
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
      - name: Configure ICAP profiles.
        fortios_icap_profile:
          vdom:  "{{ vdom }}"
          state: "present"
          access_token: "<your_own_value>"
          icap_profile:
            icap_headers:
             -
                base64_encoding: "disable"
                content: "<your_own_value>"
                id:  "6"
                name: "default_name_7"
            methods: "delete"
            name: "default_name_9"
            preview: "disable"
            preview_data_length: "11"
            replacemsg_group: "<your_own_value> (source system.replacemsg-group.name)"
            request: "disable"
            request_failure: "error"
            request_path: "<your_own_value>"
            request_server: "<your_own_value> (source icap.server.name)"
            response: "disable"
            response_failure: "error"
            response_path: "<your_own_value>"
            response_req_hdr: "disable"
            response_server: "<your_own_value> (source icap.server.name)"
            streaming_content_bypass: "disable"
    


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
