:source: fortios_dnsfilter_profile.py

:orphan:

.. fortios_dnsfilter_profile:

fortios_dnsfilter_profile -- Configure DNS domain filter profiles in Fortinet's FortiOS and FortiGate.
++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++

.. versionadded:: 2.8

.. contents::
   :local:
   :depth: 1


Synopsis
--------
- This module is able to configure a FortiGate or FortiOS (FOS) device by allowing the user to set and modify dnsfilter feature and profile category. Examples include all parameters and values need to be adjusted to datasources before usage. Tested with FOS v6.4.0



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
    <li> <span class="li-head">dnsfilter_profile</span> - Configure DNS domain filter profiles. <span class="li-normal">type: dict</span></li>
        <ul class="ul-self">
        <li> <span class="li-head">state</span> - B(Deprecated) <span class="li-normal">type: str</span> <span class="li-required">required: False</span> <span class="li-normal">choices: present, absent</span></li>
        <li> <span class="li-head">block_action</span> - Action to take for blocked domains. <span class="li-normal">type: str</span> <span class="li-normal">choices: block, redirect</span></li>
        <li> <span class="li-head">block_botnet</span> - Enable/disable blocking botnet C&C DNS lookups. <span class="li-normal">type: str</span> <span class="li-normal">choices: disable, enable</span></li>
        <li> <span class="li-head">comment</span> - Comment. <span class="li-normal">type: str</span></li>
        <li> <span class="li-head">dns_translation</span> - DNS translation settings. <span class="li-normal">type: list</span></li>
            <ul class="ul-self">
            <li> <span class="li-head">addr_type</span> - DNS translation type (IPv4 or IPv6). <span class="li-normal">type: str</span> <span class="li-normal">choices: ipv4, ipv6</span></li>
            <li> <span class="li-head">dst</span> - IPv4 address or subnet on the external network to substitute for the resolved address in DNS query replies. Can be single IP address or subnet on the external network, but number of addresses must equal number of mapped IP addresses in src. <span class="li-normal">type: str</span></li>
            <li> <span class="li-head">dst6</span> - IPv6 address or subnet on the external network to substitute for the resolved address in DNS query replies. Can be single IP address or subnet on the external network, but number of addresses must equal number of mapped IP addresses in src6. <span class="li-normal">type: str</span></li>
            <li> <span class="li-head">id</span> - ID. <span class="li-normal">type: int</span> <span class="li-required">required: True</span></li>
            <li> <span class="li-head">netmask</span> - If src and dst are subnets rather than single IP addresses, enter the netmask for both src and dst. <span class="li-normal">type: str</span></li>
            <li> <span class="li-head">prefix</span> - If src6 and dst6 are subnets rather than single IP addresses, enter the prefix for both src6 and dst6 (1 - 128). <span class="li-normal">type: int</span></li>
            <li> <span class="li-head">src</span> - IPv4 address or subnet on the internal network to compare with the resolved address in DNS query replies. If the resolved address matches, the resolved address is substituted with dst. <span class="li-normal">type: str</span></li>
            <li> <span class="li-head">src6</span> - IPv6 address or subnet on the internal network to compare with the resolved address in DNS query replies. If the resolved address matches, the resolved address is substituted with dst6. <span class="li-normal">type: str</span></li>
            <li> <span class="li-head">status</span> - Enable/disable this DNS translation entry. <span class="li-normal">type: str</span> <span class="li-normal">choices: enable, disable</span></li>
            </ul>
        <li> <span class="li-head">domain_filter</span> - Domain filter settings. <span class="li-normal">type: dict</span></li>
            <ul class="ul-self">
            <li> <span class="li-head">domain_filter_table</span> - DNS domain filter table ID. Source dnsfilter.domain-filter.id. <span class="li-normal">type: int</span></li>
            </ul>
        <li> <span class="li-head">external_ip_blocklist</span> - One or more external IP block lists. <span class="li-normal">type: list</span></li>
            <ul class="ul-self">
            <li> <span class="li-head">name</span> - External domain block list name. Source system.external-resource.name. <span class="li-normal">type: str</span> <span class="li-required">required: True</span></li>
            </ul>
        <li> <span class="li-head">ftgd_dns</span> - FortiGuard DNS Filter settings. <span class="li-normal">type: dict</span></li>
            <ul class="ul-self">
            <li> <span class="li-head">filters</span> - FortiGuard DNS domain filters. <span class="li-normal">type: list</span></li>
                <ul class="ul-self">
                <li> <span class="li-head">action</span> - Action to take for DNS requests matching the category. <span class="li-normal">type: str</span> <span class="li-normal">choices: block, monitor</span></li>
                <li> <span class="li-head">category</span> - Category number. <span class="li-normal">type: int</span></li>
                <li> <span class="li-head">id</span> - ID number. <span class="li-normal">type: int</span> <span class="li-required">required: True</span></li>
                <li> <span class="li-head">log</span> - Enable/disable DNS filter logging for this DNS profile. <span class="li-normal">type: str</span> <span class="li-normal">choices: enable, disable</span></li>
                </ul>
            <li> <span class="li-head">options</span> - FortiGuard DNS filter options. <span class="li-normal">type: str</span> <span class="li-normal">choices: error-allow, ftgd-disable</span></li>
            </ul>
        <li> <span class="li-head">log_all_domain</span> - Enable/disable logging of all domains visited (detailed DNS logging). <span class="li-normal">type: str</span> <span class="li-normal">choices: enable, disable</span></li>
        <li> <span class="li-head">name</span> - Profile name. <span class="li-normal">type: str</span> <span class="li-required">required: True</span></li>
        <li> <span class="li-head">redirect_portal</span> - IPv4 address of the SDNS redirect portal. <span class="li-normal">type: str</span></li>
        <li> <span class="li-head">redirect_portal6</span> - IPv6 address of the SDNS redirect portal. <span class="li-normal">type: str</span></li>
        <li> <span class="li-head">safe_search</span> - Enable/disable Google, Bing, and YouTube safe search. <span class="li-normal">type: str</span> <span class="li-normal">choices: disable, enable</span></li>
        <li> <span class="li-head">sdns_domain_log</span> - Enable/disable domain filtering and botnet domain logging. <span class="li-normal">type: str</span> <span class="li-normal">choices: enable, disable</span></li>
        <li> <span class="li-head">sdns_ftgd_err_log</span> - Enable/disable FortiGuard SDNS rating error logging. <span class="li-normal">type: str</span> <span class="li-normal">choices: enable, disable</span></li>
        <li> <span class="li-head">youtube_restrict</span> - Set safe search for YouTube restriction level. <span class="li-normal">type: str</span> <span class="li-normal">choices: strict, moderate</span></li>
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
      - name: Configure DNS domain filter profiles.
        fortios_dnsfilter_profile:
          vdom:  "{{ vdom }}"
          state: "present"
          dnsfilter_profile:
            block_action: "block"
            block_botnet: "disable"
            comment: "Comment."
            dns_translation:
             -
                addr_type: "ipv4"
                dst: "<your_own_value>"
                dst6: "<your_own_value>"
                id:  "10"
                netmask: "<your_own_value>"
                prefix: "12"
                src: "<your_own_value>"
                src6: "<your_own_value>"
                status: "enable"
            domain_filter:
                domain_filter_table: "17 (source dnsfilter.domain-filter.id)"
            external_ip_blocklist:
             -
                name: "default_name_19 (source system.external-resource.name)"
            ftgd_dns:
                filters:
                 -
                    action: "block"
                    category: "23"
                    id:  "24"
                    log: "enable"
                options: "error-allow"
            log_all_domain: "enable"
            name: "default_name_28"
            redirect_portal: "<your_own_value>"
            redirect_portal6: "<your_own_value>"
            safe_search: "disable"
            sdns_domain_log: "enable"
            sdns_ftgd_err_log: "enable"
            youtube_restrict: "strict"


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
