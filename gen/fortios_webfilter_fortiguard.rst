:source: fortios_webfilter_fortiguard.py

:orphan:

.. fortios_webfilter_fortiguard:

fortios_webfilter_fortiguard -- Configure FortiGuard Web Filter service in Fortinet's FortiOS and FortiGate.
++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++

.. versionadded:: 2.8

.. contents::
   :local:
   :depth: 1


Synopsis
--------
- This module is able to configure a FortiGate or FortiOS (FOS) device by allowing the user to set and modify webfilter feature and fortiguard category. Examples include all parameters and values need to be adjusted to datasources before usage. Tested with FOS v6.4.0



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
    <li> <span class="li-head">webfilter_fortiguard</span> - Configure FortiGuard Web Filter service. <span class="li-normal">type: dict</span></li>
        <ul class="ul-self">
        <li> <span class="li-head">cache_mem_percent</span> - Maximum percentage of available memory allocated to caching (1 - 15%). <span class="li-normal">type: int</span></li>
        <li> <span class="li-head">cache_mode</span> - Cache entry expiration mode. <span class="li-normal">type: str</span> <span class="li-normal">choices: ttl, db-ver</span></li>
        <li> <span class="li-head">cache_prefix_match</span> - Enable/disable prefix matching in the cache. <span class="li-normal">type: str</span> <span class="li-normal">choices: enable, disable</span></li>
        <li> <span class="li-head">close_ports</span> - Close ports used for HTTP/HTTPS override authentication and disable user overrides. <span class="li-normal">type: str</span> <span class="li-normal">choices: enable, disable</span></li>
        <li> <span class="li-head">ovrd_auth_https</span> - Enable/disable use of HTTPS for override authentication. <span class="li-normal">type: str</span> <span class="li-normal">choices: enable, disable</span></li>
        <li> <span class="li-head">ovrd_auth_port_http</span> - Port to use for FortiGuard Web Filter HTTP override authentication <span class="li-normal">type: int</span></li>
        <li> <span class="li-head">ovrd_auth_port_https</span> - Port to use for FortiGuard Web Filter HTTPS override authentication in proxy mode. <span class="li-normal">type: int</span></li>
        <li> <span class="li-head">ovrd_auth_port_https_flow</span> - Port to use for FortiGuard Web Filter HTTPS override authentication in flow mode. <span class="li-normal">type: int</span></li>
        <li> <span class="li-head">ovrd_auth_port_warning</span> - Port to use for FortiGuard Web Filter Warning override authentication. <span class="li-normal">type: int</span></li>
        <li> <span class="li-head">request_packet_size_limit</span> - Limit size of URL request packets sent to FortiGuard server (0 for default). <span class="li-normal">type: int</span></li>
        <li> <span class="li-head">warn_auth_https</span> - Enable/disable use of HTTPS for warning and authentication. <span class="li-normal">type: str</span> <span class="li-normal">choices: enable, disable</span></li>
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
      - name: Configure FortiGuard Web Filter service.
        fortios_webfilter_fortiguard:
          vdom:  "{{ vdom }}"
          webfilter_fortiguard:
            cache_mem_percent: "3"
            cache_mode: "ttl"
            cache_prefix_match: "enable"
            close_ports: "enable"
            ovrd_auth_https: "enable"
            ovrd_auth_port_http: "8"
            ovrd_auth_port_https: "9"
            ovrd_auth_port_https_flow: "10"
            ovrd_auth_port_warning: "11"
            request_packet_size_limit: "12"
            warn_auth_https: "enable"
    


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
