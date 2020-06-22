:source: fortios_web_proxy_explicit.py

:orphan:

.. fortios_web_proxy_explicit:

fortios_web_proxy_explicit -- Configure explicit Web proxy settings in Fortinet's FortiOS and FortiGate.
++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++

.. versionadded:: 2.8

.. contents::
   :local:
   :depth: 1


Synopsis
--------
- This module is able to configure a FortiGate or FortiOS (FOS) device by allowing the user to set and modify web_proxy feature and explicit category. Examples include all parameters and values need to be adjusted to datasources before usage. Tested with FOS v6.0.0



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
    <li> <span class="li-head">web_proxy_explicit</span> - Configure explicit Web proxy settings. <span class="li-normal">type: dict</span></li>
        <ul class="ul-self">
        <li> <span class="li-head">ftp_incoming_port</span> - Accept incoming FTP-over-HTTP requests on one or more ports (0 - 65535). <span class="li-normal">type: str</span></li>
        <li> <span class="li-head">ftp_over_http</span> - Enable to proxy FTP-over-HTTP sessions sent from a web browser. <span class="li-normal">type: str</span> <span class="li-normal">choices: enable, disable</span></li>
        <li> <span class="li-head">http_incoming_port</span> - Accept incoming HTTP requests on one or more ports (0 - 65535). <span class="li-normal">type: str</span></li>
        <li> <span class="li-head">https_incoming_port</span> - Accept incoming HTTPS requests on one or more ports (0 - 65535). <span class="li-normal">type: str</span></li>
        <li> <span class="li-head">https_replacement_message</span> - Enable/disable sending the client a replacement message for HTTPS requests. <span class="li-normal">type: str</span> <span class="li-normal">choices: enable, disable</span></li>
        <li> <span class="li-head">incoming_ip</span> - Restrict the explicit HTTP proxy to only accept sessions from this IP address. An interface must have this IP address. <span class="li-normal">type: str</span></li>
        <li> <span class="li-head">incoming_ip6</span> - Restrict the explicit web proxy to only accept sessions from this IPv6 address. An interface must have this IPv6 address. <span class="li-normal">type: str</span></li>
        <li> <span class="li-head">ipv6_status</span> - Enable/disable allowing an IPv6 web proxy destination in policies and all IPv6 related entries in this command. <span class="li-normal">type: str</span> <span class="li-normal">choices: enable, disable</span></li>
        <li> <span class="li-head">message_upon_server_error</span> - Enable/disable displaying a replacement message when a server error is detected. <span class="li-normal">type: str</span> <span class="li-normal">choices: enable, disable</span></li>
        <li> <span class="li-head">outgoing_ip</span> - Outgoing HTTP requests will have this IP address as their source address. An interface must have this IP address. <span class="li-normal">type: str</span></li>
        <li> <span class="li-head">outgoing_ip6</span> - Outgoing HTTP requests will leave this IPv6. Multiple interfaces can be specified. Interfaces must have these IPv6 addresses. <span class="li-normal">type: str</span></li>
        <li> <span class="li-head">pac_file_data</span> - PAC file contents enclosed in quotes (maximum of 256K bytes). <span class="li-normal">type: str</span></li>
        <li> <span class="li-head">pac_file_name</span> - Pac file name. <span class="li-normal">type: str</span></li>
        <li> <span class="li-head">pac_file_server_port</span> - Port number that PAC traffic from client web browsers uses to connect to the explicit web proxy (0 - 65535). <span class="li-normal">type: str</span></li>
        <li> <span class="li-head">pac_file_server_status</span> - Enable/disable Proxy Auto-Configuration (PAC) for users of this explicit proxy profile. <span class="li-normal">type: str</span> <span class="li-normal">choices: enable, disable</span></li>
        <li> <span class="li-head">pac_file_url</span> - PAC file access URL. <span class="li-normal">type: str</span></li>
        <li> <span class="li-head">pac_policy</span> - PAC policies. <span class="li-normal">type: list</span></li>
            <ul class="ul-self">
            <li> <span class="li-head">comments</span> - Optional comments. <span class="li-normal">type: str</span></li>
            <li> <span class="li-head">dstaddr</span> - Destination address objects. <span class="li-normal">type: list</span></li>
                <ul class="ul-self">
                <li> <span class="li-head">name</span> - Address name. Source firewall.address.name firewall.addrgrp.name. <span class="li-normal">type: str</span> <span class="li-required">required: True</span></li>
                </ul>
            <li> <span class="li-head">pac_file_data</span> - PAC file contents enclosed in quotes (maximum of 256K bytes). <span class="li-normal">type: str</span></li>
            <li> <span class="li-head">pac_file_name</span> - Pac file name. <span class="li-normal">type: str</span></li>
            <li> <span class="li-head">policyid</span> - Policy ID. <span class="li-normal">type: int</span> <span class="li-required">required: True</span></li>
            <li> <span class="li-head">srcaddr</span> - Source address objects. <span class="li-normal">type: list</span></li>
                <ul class="ul-self">
                <li> <span class="li-head">name</span> - Address name. Source firewall.address.name firewall.addrgrp.name firewall.proxy-address.name firewall.proxy-addrgrp.name. <span class="li-normal">type: str</span> <span class="li-required">required: True</span></li>
                </ul>
            <li> <span class="li-head">srcaddr6</span> - Source address6 objects. <span class="li-normal">type: list</span></li>
                <ul class="ul-self">
                <li> <span class="li-head">name</span> - Address name. Source firewall.address6.name firewall.addrgrp6.name. <span class="li-normal">type: str</span> <span class="li-required">required: True</span></li>
                </ul>
            <li> <span class="li-head">status</span> - Enable/disable policy. <span class="li-normal">type: str</span> <span class="li-normal">choices: enable, disable</span></li>
            </ul>
        <li> <span class="li-head">pref_dns_result</span> - Prefer resolving addresses using the configured IPv4 or IPv6 DNS server . <span class="li-normal">type: str</span> <span class="li-normal">choices: ipv4, ipv6</span></li>
        <li> <span class="li-head">realm</span> - Authentication realm used to identify the explicit web proxy (maximum of 63 characters). <span class="li-normal">type: str</span></li>
        <li> <span class="li-head">sec_default_action</span> - Accept or deny explicit web proxy sessions when no web proxy firewall policy exists. <span class="li-normal">type: str</span> <span class="li-normal">choices: accept, deny</span></li>
        <li> <span class="li-head">socks</span> - Enable/disable the SOCKS proxy. <span class="li-normal">type: str</span> <span class="li-normal">choices: enable, disable</span></li>
        <li> <span class="li-head">socks_incoming_port</span> - Accept incoming SOCKS proxy requests on one or more ports (0 - 65535). <span class="li-normal">type: str</span></li>
        <li> <span class="li-head">ssl_algorithm</span> - Relative strength of encryption algorithms accepted in HTTPS deep scan: high, medium, or low. <span class="li-normal">type: str</span> <span class="li-normal">choices: high, medium, low</span></li>
        <li> <span class="li-head">status</span> - Enable/disable the explicit Web proxy for HTTP and HTTPS session. <span class="li-normal">type: str</span> <span class="li-normal">choices: enable, disable</span></li>
        <li> <span class="li-head">strict_guest</span> - Enable/disable strict guest user checking by the explicit web proxy. <span class="li-normal">type: str</span> <span class="li-normal">choices: enable, disable</span></li>
        <li> <span class="li-head">trace_auth_no_rsp</span> - Enable/disable logging timed-out authentication requests. <span class="li-normal">type: str</span> <span class="li-normal">choices: enable, disable</span></li>
        <li> <span class="li-head">unknown_http_version</span> - Either reject unknown HTTP traffic as malformed or handle unknown HTTP traffic as best as the proxy server can. <span class="li-normal">type: str</span> <span class="li-normal">choices: reject, best-effort</span></li>
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
      - name: Configure explicit Web proxy settings.
        fortios_web_proxy_explicit:
          vdom:  "{{ vdom }}"
          web_proxy_explicit:
            ftp_incoming_port: "<your_own_value>"
            ftp_over_http: "enable"
            http_incoming_port: "<your_own_value>"
            https_incoming_port: "<your_own_value>"
            https_replacement_message: "enable"
            incoming_ip: "<your_own_value>"
            incoming_ip6: "<your_own_value>"
            ipv6_status: "enable"
            message_upon_server_error: "enable"
            outgoing_ip: "<your_own_value>"
            outgoing_ip6: "<your_own_value>"
            pac_file_data: "<your_own_value>"
            pac_file_name: "<your_own_value>"
            pac_file_server_port: "<your_own_value>"
            pac_file_server_status: "enable"
            pac_file_url: "<your_own_value>"
            pac_policy:
             -
                comments: "<your_own_value>"
                dstaddr:
                 -
                    name: "default_name_22 (source firewall.address.name firewall.addrgrp.name)"
                pac_file_data: "<your_own_value>"
                pac_file_name: "<your_own_value>"
                policyid: "25"
                srcaddr:
                 -
                    name: "default_name_27 (source firewall.address.name firewall.addrgrp.name firewall.proxy-address.name firewall.proxy-addrgrp.name)"
                srcaddr6:
                 -
                    name: "default_name_29 (source firewall.address6.name firewall.addrgrp6.name)"
                status: "enable"
            pref_dns_result: "ipv4"
            realm: "<your_own_value>"
            sec_default_action: "accept"
            socks: "enable"
            socks_incoming_port: "<your_own_value>"
            ssl_algorithm: "high"
            status: "enable"
            strict_guest: "enable"
            trace_auth_no_rsp: "enable"
            unknown_http_version: "reject"


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
