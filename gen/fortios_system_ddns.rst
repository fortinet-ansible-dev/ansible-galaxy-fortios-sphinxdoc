:source: fortios_system_ddns.py

:orphan:

.. fortios_system_ddns:

fortios_system_ddns -- Configure DDNS in Fortinet's FortiOS and FortiGate.
++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++

.. versionadded:: 2.9

.. contents::
   :local:
   :depth: 1


Synopsis
--------
- This module is able to configure a FortiGate or FortiOS (FOS) device by allowing the user to set and modify system feature and ddns category. Examples include all parameters and values need to be adjusted to datasources before usage. Tested with FOS v6.2.0



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
    <li> <span class="li-head">system_ddns</span> - Configure DDNS. <span class="li-normal">type: dict</span></li>
        <ul class="ul-self">
        <li> <span class="li-head">bound_ip</span> - Bound IP address. <span class="li-normal">type: str</span></li>
        <li> <span class="li-head">clear_text</span> - Enable/disable use of clear text connections. <span class="li-normal">type: str</span> <span class="li-normal">choices: disable, enable</span></li>
        <li> <span class="li-head">ddns_auth</span> - Enable/disable TSIG authentication for your DDNS server. <span class="li-normal">type: str</span> <span class="li-normal">choices: disable, tsig</span></li>
        <li> <span class="li-head">ddns_domain</span> - Your fully qualified domain name (for example, yourname.DDNS.com). <span class="li-normal">type: str</span></li>
        <li> <span class="li-head">ddns_key</span> - DDNS update key (base 64 encoding). <span class="li-normal">type: str</span></li>
        <li> <span class="li-head">ddns_keyname</span> - DDNS update key name. <span class="li-normal">type: str</span></li>
        <li> <span class="li-head">ddns_password</span> - DDNS password. <span class="li-normal">type: str</span></li>
        <li> <span class="li-head">ddns_server</span> - Select a DDNS service provider. <span class="li-normal">type: str</span> <span class="li-normal">choices: dyndns.org, dyns.net, tzo.com, vavic.com, dipdns.net, now.net.cn, dhs.org, easydns.com, genericDDNS, FortiGuardDDNS, noip.com</span></li>
        <li> <span class="li-head">ddns_server_ip</span> - Generic DDNS server IP. <span class="li-normal">type: str</span></li>
        <li> <span class="li-head">ddns_sn</span> - DDNS Serial Number. <span class="li-normal">type: str</span></li>
        <li> <span class="li-head">ddns_ttl</span> - Time-to-live for DDNS packets. <span class="li-normal">type: int</span></li>
        <li> <span class="li-head">ddns_username</span> - DDNS user name. <span class="li-normal">type: str</span></li>
        <li> <span class="li-head">ddns_zone</span> - Zone of your domain name (for example, DDNS.com). <span class="li-normal">type: str</span></li>
        <li> <span class="li-head">ddnsid</span> - DDNS ID. <span class="li-normal">type: int</span> <span class="li-required">required: True</span></li>
        <li> <span class="li-head">monitor_interface</span> - Monitored interface. <span class="li-normal">type: list</span></li>
            <ul class="ul-self">
            <li> <span class="li-head">interface_name</span> - Interface name. Source system.interface.name. <span class="li-normal">type: str</span></li>
            </ul>
        <li> <span class="li-head">ssl_certificate</span> - Name of local certificate for SSL connections. Source certificate.local.name. <span class="li-normal">type: str</span></li>
        <li> <span class="li-head">update_interval</span> - DDNS update interval (60 - 2592000 sec). <span class="li-normal">type: int</span></li>
        <li> <span class="li-head">use_public_ip</span> - Enable/disable use of public IP address. <span class="li-normal">type: str</span> <span class="li-normal">choices: disable, enable</span></li>
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
      - name: Configure DDNS.
        fortios_system_ddns:
          vdom:  "{{ vdom }}"
          state: "present"
          system_ddns:
            bound_ip: "<your_own_value>"
            clear_text: "disable"
            ddns_auth: "disable"
            ddns_domain: "<your_own_value>"
            ddns_key: "<your_own_value>"
            ddns_keyname: "<your_own_value>"
            ddns_password: "<your_own_value>"
            ddns_server: "dyndns.org"
            ddns_server_ip: "<your_own_value>"
            ddns_sn: "<your_own_value>"
            ddns_ttl: "13"
            ddns_username: "<your_own_value>"
            ddns_zone: "<your_own_value>"
            ddnsid: "16"
            monitor_interface:
             -
                interface_name: "<your_own_value> (source system.interface.name)"
            ssl_certificate: "<your_own_value> (source certificate.local.name)"
            update_interval: "20"
            use_public_ip: "disable"


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
