:source: fortios_system_fortiguard.py

:orphan:

.. fortios_system_fortiguard:

fortios_system_fortiguard -- Configure FortiGuard services in Fortinet's FortiOS and FortiGate.
+++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++

.. versionadded:: 2.9

.. contents::
   :local:
   :depth: 1


Synopsis
--------
- This module is able to configure a FortiGate or FortiOS (FOS) device by allowing the user to set and modify system feature and fortiguard category. Examples include all parameters and values need to be adjusted to datasources before usage. Tested with FOS v6.4.0



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
    <li> <span class="li-head">system_fortiguard</span> - Configure FortiGuard services. <span class="li-normal">type: dict</span></li>
        <ul class="ul-self">
        <li> <span class="li-head">antispam_cache</span> - Enable/disable FortiGuard antispam request caching. Uses a small amount of memory but improves performance. <span class="li-normal">type: str</span> <span class="li-normal">choices: enable, disable</span></li>
        <li> <span class="li-head">antispam_cache_mpercent</span> - Maximum percent of FortiGate memory the antispam cache is allowed to use (1 - 15%). <span class="li-normal">type: int</span></li>
        <li> <span class="li-head">antispam_cache_ttl</span> - Time-to-live for antispam cache entries in seconds (300 - 86400). Lower times reduce the cache size. Higher times may improve performance since the cache will have more entries. <span class="li-normal">type: int</span></li>
        <li> <span class="li-head">antispam_expiration</span> - Expiration date of the FortiGuard antispam contract. <span class="li-normal">type: int</span></li>
        <li> <span class="li-head">antispam_force_off</span> - Enable/disable turning off the FortiGuard antispam service. <span class="li-normal">type: str</span> <span class="li-normal">choices: enable, disable</span></li>
        <li> <span class="li-head">antispam_license</span> - Interval of time between license checks for the FortiGuard antispam contract. <span class="li-normal">type: int</span></li>
        <li> <span class="li-head">antispam_timeout</span> - Antispam query time out (1 - 30 sec). <span class="li-normal">type: int</span></li>
        <li> <span class="li-head">auto_join_forticloud</span> - Automatically connect to and login to FortiCloud. <span class="li-normal">type: str</span> <span class="li-normal">choices: enable, disable</span></li>
        <li> <span class="li-head">ddns_server_ip</span> - IP address of the FortiDDNS server. <span class="li-normal">type: str</span></li>
        <li> <span class="li-head">ddns_server_port</span> - Port used to communicate with FortiDDNS servers. <span class="li-normal">type: int</span></li>
        <li> <span class="li-head">fortiguard_anycast</span> - Enable/disable use of FortiGuard"s anycast network. <span class="li-normal">type: str</span> <span class="li-normal">choices: enable, disable</span></li>
        <li> <span class="li-head">fortiguard_anycast_source</span> - Configure which of Fortinet"s servers to provide FortiGuard services in FortiGuard"s anycast network. Default is Fortinet. <span class="li-normal">type: str</span> <span class="li-normal">choices: fortinet, aws, debug</span></li>
        <li> <span class="li-head">load_balance_servers</span> - Number of servers to alternate between as first FortiGuard option. <span class="li-normal">type: int</span></li>
        <li> <span class="li-head">outbreak_prevention_cache</span> - Enable/disable FortiGuard Virus Outbreak Prevention cache. <span class="li-normal">type: str</span> <span class="li-normal">choices: enable, disable</span></li>
        <li> <span class="li-head">outbreak_prevention_cache_mpercent</span> - Maximum percent of memory FortiGuard Virus Outbreak Prevention cache can use (1 - 15%). <span class="li-normal">type: int</span></li>
        <li> <span class="li-head">outbreak_prevention_cache_ttl</span> - Time-to-live for FortiGuard Virus Outbreak Prevention cache entries (300 - 86400 sec). <span class="li-normal">type: int</span></li>
        <li> <span class="li-head">outbreak_prevention_expiration</span> - Expiration date of FortiGuard Virus Outbreak Prevention contract. <span class="li-normal">type: int</span></li>
        <li> <span class="li-head">outbreak_prevention_force_off</span> - Turn off FortiGuard Virus Outbreak Prevention service. <span class="li-normal">type: str</span> <span class="li-normal">choices: enable, disable</span></li>
        <li> <span class="li-head">outbreak_prevention_license</span> - Interval of time between license checks for FortiGuard Virus Outbreak Prevention contract. <span class="li-normal">type: int</span></li>
        <li> <span class="li-head">outbreak_prevention_timeout</span> - FortiGuard Virus Outbreak Prevention time out (1 - 30 sec). <span class="li-normal">type: int</span></li>
        <li> <span class="li-head">port</span> - Port used to communicate with the FortiGuard servers. <span class="li-normal">type: str</span> <span class="li-normal">choices: 8888, 53, 80, 443</span></li>
        <li> <span class="li-head">protocol</span> - Protocol used to communicate with the FortiGuard servers. <span class="li-normal">type: str</span> <span class="li-normal">choices: udp, http, https</span></li>
        <li> <span class="li-head">proxy_password</span> - Proxy user password. <span class="li-normal">type: str</span></li>
        <li> <span class="li-head">proxy_server_ip</span> - IP address of the proxy server. <span class="li-normal">type: str</span></li>
        <li> <span class="li-head">proxy_server_port</span> - Port used to communicate with the proxy server. <span class="li-normal">type: int</span></li>
        <li> <span class="li-head">proxy_username</span> - Proxy user name. <span class="li-normal">type: str</span></li>
        <li> <span class="li-head">sandbox_region</span> - Cloud sandbox region. <span class="li-normal">type: str</span></li>
        <li> <span class="li-head">sdns_options</span> - Customization options for the FortiGuard DNS service. <span class="li-normal">type: str</span> <span class="li-normal">choices: include-question-section</span></li>
        <li> <span class="li-head">sdns_server_ip</span> - IP address of the FortiDNS server. <span class="li-normal">type: str</span></li>
        <li> <span class="li-head">sdns_server_port</span> - Port used to communicate with FortiDNS servers. <span class="li-normal">type: int</span></li>
        <li> <span class="li-head">source_ip</span> - Source IPv4 address used to communicate with FortiGuard. <span class="li-normal">type: str</span></li>
        <li> <span class="li-head">source_ip6</span> - Source IPv6 address used to communicate with FortiGuard. <span class="li-normal">type: str</span></li>
        <li> <span class="li-head">update_server_location</span> - Signature update server location. <span class="li-normal">type: str</span> <span class="li-normal">choices: usa, any</span></li>
        <li> <span class="li-head">webfilter_cache</span> - Enable/disable FortiGuard web filter caching. <span class="li-normal">type: str</span> <span class="li-normal">choices: enable, disable</span></li>
        <li> <span class="li-head">webfilter_cache_ttl</span> - Time-to-live for web filter cache entries in seconds (300 - 86400). <span class="li-normal">type: int</span></li>
        <li> <span class="li-head">webfilter_expiration</span> - Expiration date of the FortiGuard web filter contract. <span class="li-normal">type: int</span></li>
        <li> <span class="li-head">webfilter_force_off</span> - Enable/disable turning off the FortiGuard web filtering service. <span class="li-normal">type: str</span> <span class="li-normal">choices: enable, disable</span></li>
        <li> <span class="li-head">webfilter_license</span> - Interval of time between license checks for the FortiGuard web filter contract. <span class="li-normal">type: int</span></li>
        <li> <span class="li-head">webfilter_timeout</span> - Web filter query time out (1 - 30 sec). <span class="li-normal">type: int</span></li>
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
      - name: Configure FortiGuard services.
        fortios_system_fortiguard:
          vdom:  "{{ vdom }}"
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
            fortiguard_anycast: "enable"
            fortiguard_anycast_source: "fortinet"
            load_balance_servers: "15"
            outbreak_prevention_cache: "enable"
            outbreak_prevention_cache_mpercent: "17"
            outbreak_prevention_cache_ttl: "18"
            outbreak_prevention_expiration: "19"
            outbreak_prevention_force_off: "enable"
            outbreak_prevention_license: "21"
            outbreak_prevention_timeout: "22"
            port: "8888"
            protocol: "udp"
            proxy_password: "<your_own_value>"
            proxy_server_ip: "<your_own_value>"
            proxy_server_port: "27"
            proxy_username: "<your_own_value>"
            sandbox_region: "<your_own_value>"
            sdns_options: "include-question-section"
            sdns_server_ip: "<your_own_value>"
            sdns_server_port: "32"
            source_ip: "84.230.14.43"
            source_ip6: "<your_own_value>"
            update_server_location: "usa"
            webfilter_cache: "enable"
            webfilter_cache_ttl: "37"
            webfilter_expiration: "38"
            webfilter_force_off: "enable"
            webfilter_license: "40"
            webfilter_timeout: "41"


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
