:source: fortios_user_exchange.py

:orphan:

.. fortios_user_exchange:

fortios_user_exchange -- Configure MS Exchange server entries in Fortinet's FortiOS and FortiGate.
++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++

.. versionadded:: 2.9

.. contents::
   :local:
   :depth: 1


Synopsis
--------
- This module is able to configure a FortiGate or FortiOS (FOS) device by allowing the user to set and modify user feature and exchange category. Examples include all parameters and values need to be adjusted to datasources before usage. Tested with FOS v6.4.0



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
    <li> <span class="li-head">user_exchange</span> - Configure MS Exchange server entries. <span class="li-normal">type: dict</span></li>
        <ul class="ul-self">
        <li> <span class="li-head">auth_level</span> - Authentication security level used for the RPC protocol layer. <span class="li-normal">type: str</span> <span class="li-normal">choices: connect, call, packet, integrity, privacy</span></li>
        <li> <span class="li-head">auth_type</span> - Authentication security type used for the RPC protocol layer. <span class="li-normal">type: str</span> <span class="li-normal">choices: spnego, ntlm, kerberos</span></li>
        <li> <span class="li-head">auto_discover_kdc</span> - Enable/disable automatic discovery of KDC IP addresses. <span class="li-normal">type: str</span> <span class="li-normal">choices: enable, disable</span></li>
        <li> <span class="li-head">connect_protocol</span> - Connection protocol used to connect to MS Exchange service. <span class="li-normal">type: str</span> <span class="li-normal">choices: rpc-over-tcp, rpc-over-http, rpc-over-https</span></li>
        <li> <span class="li-head">domain_name</span> - MS Exchange server fully qualified domain name. <span class="li-normal">type: str</span></li>
        <li> <span class="li-head">http_auth_type</span> - Authentication security type used for the HTTP transport. <span class="li-normal">type: str</span> <span class="li-normal">choices: basic, ntlm</span></li>
        <li> <span class="li-head">ip</span> - Server IPv4 address. <span class="li-normal">type: str</span></li>
        <li> <span class="li-head">kdc_ip</span> - KDC IPv4 addresses for Kerberos authentication. <span class="li-normal">type: list</span></li>
            <ul class="ul-self">
            <li> <span class="li-head">ipv4</span> - KDC IPv4 addresses for Kerberos authentication. <span class="li-normal">type: str</span> <span class="li-required">required: True</span></li>
            </ul>
        <li> <span class="li-head">name</span> - MS Exchange server entry name. <span class="li-normal">type: str</span> <span class="li-required">required: True</span></li>
        <li> <span class="li-head">password</span> - Password for the specified username. <span class="li-normal">type: str</span></li>
        <li> <span class="li-head">server_name</span> - MS Exchange server hostname. <span class="li-normal">type: str</span></li>
        <li> <span class="li-head">ssl_min_proto_version</span> - Minimum SSL/TLS protocol version for HTTPS transport . <span class="li-normal">type: str</span> <span class="li-normal">choices: default, SSLv3, TLSv1, TLSv1-1, TLSv1-2</span></li>
        <li> <span class="li-head">username</span> - User name used to sign in to the server. Must have proper permissions for service. <span class="li-normal">type: str</span></li>
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
      - name: Configure MS Exchange server entries.
        fortios_user_exchange:
          vdom:  "{{ vdom }}"
          state: "present"
          user_exchange:
            auth_level: "connect"
            auth_type: "spnego"
            auto_discover_kdc: "enable"
            connect_protocol: "rpc-over-tcp"
            domain_name: "<your_own_value>"
            http_auth_type: "basic"
            ip: "<your_own_value>"
            kdc_ip:
             -
                ipv4: "<your_own_value>"
            name: "default_name_12"
            password: "<your_own_value>"
            server_name: "<your_own_value>"
            ssl_min_proto_version: "default"
            username: "<your_own_value>"


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
