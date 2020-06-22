:source: fortios_firewall_proxy_address.py

:orphan:

.. fortios_firewall_proxy_address:

fortios_firewall_proxy_address -- Configure web proxy address in Fortinet's FortiOS and FortiGate.
++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++

.. versionadded:: 2.8

.. contents::
   :local:
   :depth: 1


Synopsis
--------
- This module is able to configure a FortiGate or FortiOS (FOS) device by allowing the user to set and modify firewall feature and proxy_address category. Examples include all parameters and values need to be adjusted to datasources before usage. Tested with FOS v6.2.0



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
    <li> <span class="li-head">firewall_proxy_address</span> - Configure web proxy address. <span class="li-normal">type: dict</span></li>
        <ul class="ul-self">
        <li> <span class="li-head">state</span> - B(Deprecated) <span class="li-normal">type: str</span> <span class="li-required">required: False</span> <span class="li-normal">choices: present, absent</span></li>
        <li> <span class="li-head">case_sensitivity</span> - Enable to make the pattern case sensitive. <span class="li-normal">type: str</span> <span class="li-normal">choices: disable, enable</span></li>
        <li> <span class="li-head">category</span> - FortiGuard category ID. <span class="li-normal">type: list</span></li>
            <ul class="ul-self">
            <li> <span class="li-head">id</span> - Fortiguard category id. <span class="li-normal">type: int</span> <span class="li-required">required: True</span></li>
            </ul>
        <li> <span class="li-head">color</span> - Integer value to determine the color of the icon in the GUI (1 - 32). <span class="li-normal">type: int</span></li>
        <li> <span class="li-head">comment</span> - Optional comments. <span class="li-normal">type: str</span></li>
        <li> <span class="li-head">header</span> - HTTP header name as a regular expression. <span class="li-normal">type: str</span></li>
        <li> <span class="li-head">header_group</span> - HTTP header group. <span class="li-normal">type: list</span></li>
            <ul class="ul-self">
            <li> <span class="li-head">case_sensitivity</span> - Case sensitivity in pattern. <span class="li-normal">type: str</span> <span class="li-normal">choices: disable, enable</span></li>
            <li> <span class="li-head">header</span> - HTTP header regular expression. <span class="li-normal">type: str</span></li>
            <li> <span class="li-head">header_name</span> - HTTP header. <span class="li-normal">type: str</span></li>
            <li> <span class="li-head">id</span> - ID. <span class="li-normal">type: int</span> <span class="li-required">required: True</span></li>
            </ul>
        <li> <span class="li-head">header_name</span> - Name of HTTP header. <span class="li-normal">type: str</span></li>
        <li> <span class="li-head">host</span> - Address object for the host. Source firewall.address.name firewall.addrgrp.name firewall.proxy-address.name. <span class="li-normal">type: str</span></li>
        <li> <span class="li-head">host_regex</span> - Host name as a regular expression. <span class="li-normal">type: str</span></li>
        <li> <span class="li-head">method</span> - HTTP request methods to be used. <span class="li-normal">type: str</span> <span class="li-normal">choices: get, post, put, head, connect, trace, options, delete</span></li>
        <li> <span class="li-head">name</span> - Address name. <span class="li-normal">type: str</span> <span class="li-required">required: True</span></li>
        <li> <span class="li-head">path</span> - URL path as a regular expression. <span class="li-normal">type: str</span></li>
        <li> <span class="li-head">query</span> - Match the query part of the URL as a regular expression. <span class="li-normal">type: str</span></li>
        <li> <span class="li-head">referrer</span> - Enable/disable use of referrer field in the HTTP header to match the address. <span class="li-normal">type: str</span> <span class="li-normal">choices: enable, disable</span></li>
        <li> <span class="li-head">tagging</span> - Config object tagging. <span class="li-normal">type: list</span></li>
            <ul class="ul-self">
            <li> <span class="li-head">category</span> - Tag category. Source system.object-tagging.category. <span class="li-normal">type: str</span></li>
            <li> <span class="li-head">name</span> - Tagging entry name. <span class="li-normal">type: str</span> <span class="li-required">required: True</span></li>
            <li> <span class="li-head">tags</span> - Tags. <span class="li-normal">type: list</span></li>
                <ul class="ul-self">
                <li> <span class="li-head">name</span> - Tag name. Source system.object-tagging.tags.name. <span class="li-normal">type: str</span> <span class="li-required">required: True</span></li>
                </ul>
            </ul>
        <li> <span class="li-head">type</span> - Proxy address type. <span class="li-normal">type: str</span> <span class="li-normal">choices: host-regex, url, category, method, ua, header, src-advanced, dst-advanced</span></li>
        <li> <span class="li-head">ua</span> - Names of browsers to be used as user agent. <span class="li-normal">type: str</span> <span class="li-normal">choices: chrome, ms, firefox, safari, other</span></li>
        <li> <span class="li-head">uuid</span> - Universally Unique Identifier (UUID; automatically assigned but can be manually reset). <span class="li-normal">type: str</span></li>
        <li> <span class="li-head">visibility</span> - Enable/disable visibility of the object in the GUI. <span class="li-normal">type: str</span> <span class="li-normal">choices: enable, disable</span></li>
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
      - name: Configure web proxy address.
        fortios_firewall_proxy_address:
          vdom:  "{{ vdom }}"
          state: "present"
          firewall_proxy_address:
            case_sensitivity: "disable"
            category:
             -
                id:  "5"
            color: "6"
            comment: "Optional comments."
            header: "<your_own_value>"
            header_group:
             -
                case_sensitivity: "disable"
                header: "<your_own_value>"
                header_name: "<your_own_value>"
                id:  "13"
            header_name: "<your_own_value>"
            host: "myhostname (source firewall.address.name firewall.addrgrp.name firewall.proxy-address.name)"
            host_regex: "myhostname"
            method: "get"
            name: "default_name_18"
            path: "<your_own_value>"
            query: "<your_own_value>"
            referrer: "enable"
            tagging:
             -
                category: "<your_own_value> (source system.object-tagging.category)"
                name: "default_name_24"
                tags:
                 -
                    name: "default_name_26 (source system.object-tagging.tags.name)"
            type: "host-regex"
            ua: "chrome"
            uuid: "<your_own_value>"
            visibility: "enable"


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
