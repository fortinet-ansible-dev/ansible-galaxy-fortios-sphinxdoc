:source: fortios_web_proxy_global.py

:orphan:

.. _fortios_web_proxy_global:

fortios_web_proxy_global -- Configure Web proxy global settings in Fortinet's FortiOS and FortiGate.
++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++

.. versionadded:: 2.8

.. contents::
   :local:
   :depth: 1


Synopsis
--------
- This module is able to configure a FortiGate or FortiOS (FOS) device by allowing the user to set and modify web_proxy feature and global category. Examples include all parameters and values need to be adjusted to datasources before usage. Tested with FOS v6.0.5


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
    <li><span class="li-head">web_proxy_global</span> - Configure Web proxy global settings. <span class="li-normal">default: null</span> <span class="li-normal">type: dict</span></li>
            <ul class="ul-self">

            <li><span class="li-head">fast_policy_match</span> - Enable/disable fast matching algorithm for explicit and transparent proxy policy. <span class="li-normal">type: str</span> <span class="li-normal">choices: enable,  disable</span></li>
            <li><span class="li-head">forward_proxy_auth</span> - Enable/disable forwarding proxy authentication headers. <span class="li-normal">type: str</span> <span class="li-normal">choices: enable,  disable</span></li>
            <li><span class="li-head">forward_server_affinity_timeout</span> - Period of time before the source IP's traffic is no longer assigned to the forwarding server (6 - 60 min). <span class="li-normal">type: int</span></li>
            <li><span class="li-head">learn_client_ip</span> - Enable/disable learning the client's IP address from headers. <span class="li-normal">type: str</span> <span class="li-normal">choices: enable,  disable</span></li>
            <li><span class="li-head">learn_client_ip_from_header</span> - Learn client IP address from the specified headers. <span class="li-normal">type: str</span> <span class="li-normal">choices: true-client-ip,  x-real-ip,  x-forwarded-for</span></li>
            <li><span class="li-head">learn_client_ip_srcaddr</span> - Source address name (srcaddr or srcaddr6 must be set). <span class="li-normal">type: list</span></li>
                    <ul class="ul-self">

                    <li><span class="li-head">name</span> - Address name. Source firewall.address.name firewall.addrgrp.name. <span class="li-required">required</span> <span class="li-normal">type: str</span>
                    </ul>

            <li><span class="li-head">learn_client_ip_srcaddr6</span> - IPv6 Source address name (srcaddr or srcaddr6 must be set). <span class="li-normal">type: list</span></li>
                    <ul class="ul-self">

                    <li><span class="li-head">name</span> - Address name. Source firewall.address6.name firewall.addrgrp6.name. <span class="li-required">required</span> <span class="li-normal">type: str</span>
                    </ul>

            <li><span class="li-head">max_message_length</span> - Maximum length of HTTP message, not including body (16 - 256 Kbytes). <span class="li-normal">type: int</span></li>
            <li><span class="li-head">max_request_length</span> - Maximum length of HTTP request line (2 - 64 Kbytes). <span class="li-normal">type: int</span></li>
            <li><span class="li-head">max_waf_body_cache_length</span> - Maximum length of HTTP messages processed by Web Application Firewall (WAF) (10 - 1024 Kbytes). <span class="li-normal">type: int</span></li>
            <li><span class="li-head">proxy_fqdn</span> - Fully Qualified Domain Name (FQDN) that clients connect to  to connect to the explicit web proxy. <span class="li-normal">type: str</span></li>
            <li><span class="li-head">strict_web_check</span> - Enable/disable strict web checking to block web sites that send incorrect headers that don't conform to HTTP 1.1. <span class="li-normal">type: str</span> <span class="li-normal">choices: enable,  disable</span></li>
            <li><span class="li-head">tunnel_non_http</span> - Enable/disable allowing non-HTTP traffic. Allowed non-HTTP traffic is tunneled. <span class="li-normal">type: str</span> <span class="li-normal">choices: enable,  disable</span></li>
            <li><span class="li-head">unknown_http_version</span> - "Action to take when an unknown version of HTTP is encountered: reject, allow (tunnel), or proceed with best-effort." <span class="li-normal">type: str</span> <span class="li-normal">choices: reject,  tunnel,  best-effort</span></li>
            <li><span class="li-head">webproxy_profile</span> - Name of the web proxy profile to apply when explicit proxy traffic is allowed by default and traffic is accepted that does not match an explicit proxy policy. Source web-proxy.profile.name. <span class="li-normal">type: str</span>
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
      - name: Configure Web proxy global settings.
        fortios_web_proxy_global:
          host:  "{{ host }}"
          username: "{{ username }}"
          password: "{{ password }}"
          vdom:  "{{ vdom }}"
          https: "False"
          web_proxy_global:
            fast_policy_match: "enable"
            forward_proxy_auth: "enable"
            forward_server_affinity_timeout: "5"
            learn_client_ip: "enable"
            learn_client_ip_from_header: "true-client-ip"
            learn_client_ip_srcaddr:
             -
                name: "default_name_9 (source firewall.address.name firewall.addrgrp.name)"
            learn_client_ip_srcaddr6:
             -
                name: "default_name_11 (source firewall.address6.name firewall.addrgrp6.name)"
            max_message_length: "12"
            max_request_length: "13"
            max_waf_body_cache_length: "14"
            proxy_fqdn: "<your_own_value>"
            strict_web_check: "enable"
            tunnel_non_http: "enable"
            unknown_http_version: "reject"
            webproxy_profile: "<your_own_value> (source web-proxy.profile.name)"



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