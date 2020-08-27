:source: fortios_webfilter_urlfilter.py

:orphan:

.. fortios_webfilter_urlfilter:

fortios_webfilter_urlfilter -- Configure URL filter lists in Fortinet's FortiOS and FortiGate.
++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++

.. versionadded:: 2.8

.. contents::
   :local:
   :depth: 1


Synopsis
--------
- This module is able to configure a FortiGate or FortiOS (FOS) device by allowing the user to set and modify webfilter feature and urlfilter category. Examples include all parameters and values need to be adjusted to datasources before usage. Tested with FOS v6.0.0



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
    <li> <span class="li-head">webfilter_urlfilter</span> - Configure URL filter lists. <span class="li-normal">type: dict</span></li>
        <ul class="ul-self">
        <li> <span class="li-head">state</span> - B(Deprecated) <span class="li-normal">type: str</span> <span class="li-required">required: False</span> <span class="li-normal">choices: present, absent</span></li>
        <li> <span class="li-head">comment</span> - Optional comments. <span class="li-normal">type: str</span></li>
        <li> <span class="li-head">entries</span> - URL filter entries. <span class="li-normal">type: list</span></li>
            <ul class="ul-self">
            <li> <span class="li-head">action</span> - Action to take for URL filter matches. <span class="li-normal">type: str</span> <span class="li-normal">choices: exempt, block, allow, monitor</span></li>
            <li> <span class="li-head">dns_address_family</span> - Resolve IPv4 address, IPv6 address, or both from DNS server. <span class="li-normal">type: str</span> <span class="li-normal">choices: ipv4, ipv6, both</span></li>
            <li> <span class="li-head">exempt</span> - If action is set to exempt, select the security profile operations that exempt URLs skip. Separate multiple options with a space. <span class="li-normal">type: str</span> <span class="li-normal">choices: av, web-content, activex-java-cookie, dlp, fortiguard, range-block, pass, all</span></li>
            <li> <span class="li-head">id</span> - Id. <span class="li-normal">type: int</span> <span class="li-required">required: True</span></li>
            <li> <span class="li-head">referrer_host</span> - Referrer host name. <span class="li-normal">type: str</span></li>
            <li> <span class="li-head">status</span> - Enable/disable this URL filter. <span class="li-normal">type: str</span> <span class="li-normal">choices: enable, disable</span></li>
            <li> <span class="li-head">type</span> - Filter type (simple, regex, or wildcard). <span class="li-normal">type: str</span> <span class="li-normal">choices: simple, regex, wildcard</span></li>
            <li> <span class="li-head">url</span> - URL to be filtered. <span class="li-normal">type: str</span></li>
            <li> <span class="li-head">web_proxy_profile</span> - Web proxy profile. Source web-proxy.profile.name. <span class="li-normal">type: str</span></li>
            </ul>
        <li> <span class="li-head">id</span> - ID. <span class="li-normal">type: int</span> <span class="li-required">required: True</span></li>
        <li> <span class="li-head">ip_addr_block</span> - Enable/disable blocking URLs when the hostname appears as an IP address. <span class="li-normal">type: str</span> <span class="li-normal">choices: enable, disable</span></li>
        <li> <span class="li-head">name</span> - Name of URL filter list. <span class="li-normal">type: str</span></li>
        <li> <span class="li-head">one_arm_ips_urlfilter</span> - Enable/disable DNS resolver for one-arm IPS URL filter operation. <span class="li-normal">type: str</span> <span class="li-normal">choices: enable, disable</span></li>
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
      - name: Configure URL filter lists.
        fortios_webfilter_urlfilter:
          vdom:  "{{ vdom }}"
          state: "present"
          webfilter_urlfilter:
            comment: "Optional comments."
            entries:
             -
                action: "exempt"
                dns_address_family: "ipv4"
                exempt: "av"
                id:  "8"
                referrer_host: "myhostname"
                status: "enable"
                type: "simple"
                url: "myurl.com"
                web_proxy_profile: "<your_own_value> (source web-proxy.profile.name)"
            id:  "14"
            ip_addr_block: "enable"
            name: "default_name_16"
            one_arm_ips_urlfilter: "enable"


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
