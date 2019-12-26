:source: fortios_system_fortiguard.py

:orphan:

.. _fortios_system_fortiguard:

fortios_system_fortiguard -- Configure FortiGuard services in Fortinet's FortiOS and FortiGate.
+++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++

.. versionadded:: 2.9

.. contents::
   :local:
   :depth: 1


Synopsis
--------
- This module is able to configure a FortiGate or FortiOS (FOS) device by allowing the user to set and modify system feature and fortiguard category. Examples include all parameters and values need to be adjusted to datasources before usage. Tested with FOS v6.0.5


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
    <li><span class="li-head">system_fortiguard</span> - Configure FortiGuard services. <span class="li-normal">default: null</span> <span class="li-normal">type: dict</span></li>
            <ul class="ul-self">

            <li><span class="li-head">antispam_cache</span> - Enable/disable FortiGuard antispam request caching. Uses a small amount of memory but improves performance. <span class="li-normal">type: str</span> <span class="li-normal">choices: enable,  disable</span></li>
            <li><span class="li-head">antispam_cache_mpercent</span> - Maximum percent of FortiGate memory the antispam cache is allowed to use (1 - 15%). <span class="li-normal">type: int</span></li>
            <li><span class="li-head">antispam_cache_ttl</span> - Time-to-live for antispam cache entries in seconds (300 - 86400). Lower times reduce the cache size. Higher times may improve performance since the cache will have more entries. <span class="li-normal">type: int</span></li>
            <li><span class="li-head">antispam_expiration</span> - Expiration date of the FortiGuard antispam contract. <span class="li-normal">type: int</span></li>
            <li><span class="li-head">antispam_force_off</span> - Enable/disable turning off the FortiGuard antispam service. <span class="li-normal">type: str</span> <span class="li-normal">choices: enable,  disable</span></li>
            <li><span class="li-head">antispam_license</span> - Interval of time between license checks for the FortiGuard antispam contract. <span class="li-normal">type: int</span></li>
            <li><span class="li-head">antispam_timeout</span> - Antispam query time out (1 - 30 sec). <span class="li-normal">type: int</span></li>
            <li><span class="li-head">auto_join_forticloud</span> - Automatically connect to and login to FortiCloud. <span class="li-normal">type: str</span> <span class="li-normal">choices: enable,  disable</span></li>
            <li><span class="li-head">ddns_server_ip</span> - IP address of the FortiDDNS server. <span class="li-normal">type: str</span></li>
            <li><span class="li-head">ddns_server_port</span> - Port used to communicate with FortiDDNS servers. <span class="li-normal">type: int</span></li>
            <li><span class="li-head">load_balance_servers</span> - Number of servers to alternate between as first FortiGuard option. <span class="li-normal">type: int</span></li>
            <li><span class="li-head">outbreak_prevention_cache</span> - Enable/disable FortiGuard Virus Outbreak Prevention cache. <span class="li-normal">type: str</span> <span class="li-normal">choices: enable,  disable</span></li>
            <li><span class="li-head">outbreak_prevention_cache_mpercent</span> - Maximum percent of memory FortiGuard Virus Outbreak Prevention cache can use (1 - 15%). <span class="li-normal">type: int</span></li>
            <li><span class="li-head">outbreak_prevention_cache_ttl</span> - Time-to-live for FortiGuard Virus Outbreak Prevention cache entries (300 - 86400 sec). <span class="li-normal">type: int</span></li>
            <li><span class="li-head">outbreak_prevention_expiration</span> - Expiration date of FortiGuard Virus Outbreak Prevention contract. <span class="li-normal">type: int</span></li>
            <li><span class="li-head">outbreak_prevention_force_off</span> - Turn off FortiGuard Virus Outbreak Prevention service. <span class="li-normal">type: str</span> <span class="li-normal">choices: enable,  disable</span></li>
            <li><span class="li-head">outbreak_prevention_license</span> - Interval of time between license checks for FortiGuard Virus Outbreak Prevention contract. <span class="li-normal">type: int</span></li>
            <li><span class="li-head">outbreak_prevention_timeout</span> - FortiGuard Virus Outbreak Prevention time out (1 - 30 sec). <span class="li-normal">type: int</span></li>
            <li><span class="li-head">port</span> - Port used to communicate with the FortiGuard servers. <span class="li-normal">type: str</span> <span class="li-normal">choices: 53,  8888,  80</span></li>
            <li><span class="li-head">sdns_server_ip</span> - IP address of the FortiDNS server. <span class="li-normal">type: str</span></li>
            <li><span class="li-head">sdns_server_port</span> - Port used to communicate with FortiDNS servers. <span class="li-normal">type: int</span></li>
            <li><span class="li-head">service_account_id</span> - Service account ID. <span class="li-normal">type: str</span></li>
            <li><span class="li-head">source_ip</span> - Source IPv4 address used to communicate with FortiGuard. <span class="li-normal">type: str</span></li>
            <li><span class="li-head">source_ip6</span> - Source IPv6 address used to communicate with FortiGuard. <span class="li-normal">type: str</span></li>
            <li><span class="li-head">update_server_location</span> - Signature update server location. <span class="li-normal">type: str</span> <span class="li-normal">choices: usa,  any</span></li>
            <li><span class="li-head">webfilter_cache</span> - Enable/disable FortiGuard web filter caching. <span class="li-normal">type: str</span> <span class="li-normal">choices: enable,  disable</span></li>
            <li><span class="li-head">webfilter_cache_ttl</span> - Time-to-live for web filter cache entries in seconds (300 - 86400). <span class="li-normal">type: int</span></li>
            <li><span class="li-head">webfilter_expiration</span> - Expiration date of the FortiGuard web filter contract. <span class="li-normal">type: int</span></li>
            <li><span class="li-head">webfilter_force_off</span> - Enable/disable turning off the FortiGuard web filtering service. <span class="li-normal">type: str</span> <span class="li-normal">choices: enable,  disable</span></li>
            <li><span class="li-head">webfilter_license</span> - Interval of time between license checks for the FortiGuard web filter contract. <span class="li-normal">type: int</span></li>
            <li><span class="li-head">webfilter_timeout</span> - Web filter query time out (1 - 30 sec). <span class="li-normal">type: int</span>
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
      - name: Configure FortiGuard services.
        fortios_system_fortiguard:
          host:  "{{ host }}"
          username: "{{ username }}"
          password: "{{ password }}"
          vdom:  "{{ vdom }}"
          https: "False"
          system_fortiguard:
            antispam_cache: "enable"
            antispam_cache_mpercent: "4"
            antispam_cache_ttl: "5"
            antispam_expiration: "6"
            antispam_force_off: "enable"
            antispam_license: "8"
            antispam_timeout: "9"
            auto_join_forticloud: "enable"
            ddns_server_ip: "<your_own_value>"
            ddns_server_port: "12"
            load_balance_servers: "13"
            outbreak_prevention_cache: "enable"
            outbreak_prevention_cache_mpercent: "15"
            outbreak_prevention_cache_ttl: "16"
            outbreak_prevention_expiration: "17"
            outbreak_prevention_force_off: "enable"
            outbreak_prevention_license: "19"
            outbreak_prevention_timeout: "20"
            port: "53"
            sdns_server_ip: "<your_own_value>"
            sdns_server_port: "23"
            service_account_id: "<your_own_value>"
            source_ip: "84.230.14.43"
            source_ip6: "<your_own_value>"
            update_server_location: "usa"
            webfilter_cache: "enable"
            webfilter_cache_ttl: "29"
            webfilter_expiration: "30"
            webfilter_force_off: "enable"
            webfilter_license: "32"
            webfilter_timeout: "33"



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