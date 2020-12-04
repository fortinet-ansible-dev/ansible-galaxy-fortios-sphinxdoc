:source: fortios_system_wccp.py

:orphan:

.. fortios_system_wccp:

fortios_system_wccp -- Configure WCCP in Fortinet's FortiOS and FortiGate.
++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++

.. versionadded:: 2.9

.. contents::
   :local:
   :depth: 1


Synopsis
--------
- This module is able to configure a FortiGate or FortiOS (FOS) device by allowing the user to set and modify system feature and wccp category. Examples include all parameters and values need to be adjusted to datasources before usage. Tested with FOS v6.2.0



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
    <li> <span class="li-head">system_wccp</span> - Configure WCCP. <span class="li-normal">type: dict</span></li>
        <ul class="ul-self">
        <li> <span class="li-head">assignment_bucket_format</span> - Assignment bucket format for the WCCP cache engine. <span class="li-normal">type: str</span> <span class="li-normal">choices: wccp-v2, cisco-implementation</span></li>
        <li> <span class="li-head">assignment_dstaddr_mask</span> - Assignment destination address mask. <span class="li-normal">type: str</span></li>
        <li> <span class="li-head">assignment_method</span> - Hash key assignment preference. <span class="li-normal">type: str</span> <span class="li-normal">choices: HASH, MASK, any</span></li>
        <li> <span class="li-head">assignment_srcaddr_mask</span> - Assignment source address mask. <span class="li-normal">type: str</span></li>
        <li> <span class="li-head">assignment_weight</span> - Assignment of hash weight/ratio for the WCCP cache engine. <span class="li-normal">type: int</span></li>
        <li> <span class="li-head">authentication</span> - Enable/disable MD5 authentication. <span class="li-normal">type: str</span> <span class="li-normal">choices: enable, disable</span></li>
        <li> <span class="li-head">cache_engine_method</span> - Method used to forward traffic to the routers or to return to the cache engine. <span class="li-normal">type: str</span> <span class="li-normal">choices: GRE, L2</span></li>
        <li> <span class="li-head">cache_id</span> - IP address known to all routers. If the addresses are the same, use the default 0.0.0.0. <span class="li-normal">type: str</span></li>
        <li> <span class="li-head">forward_method</span> - Method used to forward traffic to the cache servers. <span class="li-normal">type: str</span> <span class="li-normal">choices: GRE, L2, any</span></li>
        <li> <span class="li-head">group_address</span> - IP multicast address used by the cache routers. For the FortiGate to ignore multicast WCCP traffic, use the default 0.0.0.0. <span class="li-normal">type: str</span></li>
        <li> <span class="li-head">password</span> - Password for MD5 authentication. <span class="li-normal">type: str</span></li>
        <li> <span class="li-head">ports</span> - Service ports. <span class="li-normal">type: str</span></li>
        <li> <span class="li-head">ports_defined</span> - Match method. <span class="li-normal">type: str</span> <span class="li-normal">choices: source, destination</span></li>
        <li> <span class="li-head">primary_hash</span> - Hash method. <span class="li-normal">type: str</span> <span class="li-normal">choices: src-ip, dst-ip, src-port, dst-port</span></li>
        <li> <span class="li-head">priority</span> - Service priority. <span class="li-normal">type: int</span></li>
        <li> <span class="li-head">protocol</span> - Service protocol. <span class="li-normal">type: int</span></li>
        <li> <span class="li-head">return_method</span> - Method used to decline a redirected packet and return it to the FortiGate. <span class="li-normal">type: str</span> <span class="li-normal">choices: GRE, L2, any</span></li>
        <li> <span class="li-head">router_id</span> - IP address known to all cache engines. If all cache engines connect to the same FortiGate interface, use the default 0.0.0.0. <span class="li-normal">type: str</span></li>
        <li> <span class="li-head">router_list</span> - IP addresses of one or more WCCP routers. <span class="li-normal">type: str</span></li>
        <li> <span class="li-head">server_list</span> - IP addresses and netmasks for up to four cache servers. <span class="li-normal">type: str</span></li>
        <li> <span class="li-head">server_type</span> - Cache server type. <span class="li-normal">type: str</span> <span class="li-normal">choices: forward, proxy</span></li>
        <li> <span class="li-head">service_id</span> - Service ID. <span class="li-normal">type: str</span></li>
        <li> <span class="li-head">service_type</span> - WCCP service type used by the cache server for logical interception and redirection of traffic. <span class="li-normal">type: str</span> <span class="li-normal">choices: auto, standard, dynamic</span></li>
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
      - name: Configure WCCP.
        fortios_system_wccp:
          vdom:  "{{ vdom }}"
          state: "present"
          access_token: "<your_own_value>"
          system_wccp:
            assignment_bucket_format: "wccp-v2"
            assignment_dstaddr_mask: "<your_own_value>"
            assignment_method: "HASH"
            assignment_srcaddr_mask: "<your_own_value>"
            assignment_weight: "7"
            authentication: "enable"
            cache_engine_method: "GRE"
            cache_id: "<your_own_value>"
            forward_method: "GRE"
            group_address: "<your_own_value>"
            password: "<your_own_value>"
            ports: "<your_own_value>"
            ports_defined: "source"
            primary_hash: "src-ip"
            priority: "17"
            protocol: "18"
            return_method: "GRE"
            router_id: "<your_own_value>"
            router_list: "<your_own_value>"
            server_list: "<your_own_value>"
            server_type: "forward"
            service_id: "<your_own_value>"
            service_type: "auto"
    


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
