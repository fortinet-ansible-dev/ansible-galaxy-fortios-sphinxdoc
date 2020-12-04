:source: fortios_waf_profile.py

:orphan:

.. fortios_waf_profile:

fortios_waf_profile -- Web application firewall configuration in Fortinet's FortiOS and FortiGate.
++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++

.. versionadded:: 2.8

.. contents::
   :local:
   :depth: 1


Synopsis
--------
- This module is able to configure a FortiGate or FortiOS (FOS) device by allowing the user to set and modify waf feature and profile category. Examples include all parameters and values need to be adjusted to datasources before usage. Tested with FOS v6.2.0



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
    <li> <span class="li-head">state</span> - Indicates whether to create or remove the object. This attribute was present already in previous version in a deeper level. It has been moved out to this outer level. <span class="li-normal">type: str</span> <span class="li-required">required: False</span> <span class="li-normal">choices: present, absent</span></li>
    <li> <span class="li-head">waf_profile</span> - Web application firewall configuration. <span class="li-normal">type: dict</span></li>
        <ul class="ul-self">
        <li> <span class="li-head">state</span> - B(Deprecated) <span class="li-normal">type: str</span> <span class="li-required">required: False</span> <span class="li-normal">choices: present, absent</span></li>
        <li> <span class="li-head">address_list</span> - Black address list and white address list. <span class="li-normal">type: dict</span></li>
            <ul class="ul-self">
            <li> <span class="li-head">blocked_address</span> - Blocked address. <span class="li-normal">type: list</span></li>
                <ul class="ul-self">
                <li> <span class="li-head">name</span> - Address name. Source firewall.address.name firewall.addrgrp.name. <span class="li-normal">type: str</span> <span class="li-required">required: True</span></li>
                </ul>
            <li> <span class="li-head">blocked_log</span> - Enable/disable logging on blocked addresses. <span class="li-normal">type: str</span> <span class="li-normal">choices: enable, disable</span></li>
            <li> <span class="li-head">severity</span> - Severity. <span class="li-normal">type: str</span> <span class="li-normal">choices: high, medium, low</span></li>
            <li> <span class="li-head">status</span> - Status. <span class="li-normal">type: str</span> <span class="li-normal">choices: enable, disable</span></li>
            <li> <span class="li-head">trusted_address</span> - Trusted address. <span class="li-normal">type: list</span></li>
                <ul class="ul-self">
                <li> <span class="li-head">name</span> - Address name. Source firewall.address.name firewall.addrgrp.name. <span class="li-normal">type: str</span> <span class="li-required">required: True</span></li>
                </ul>
            </ul>
        <li> <span class="li-head">comment</span> - Comment. <span class="li-normal">type: str</span></li>
        <li> <span class="li-head">constraint</span> - WAF HTTP protocol restrictions. <span class="li-normal">type: dict</span></li>
            <ul class="ul-self">
            <li> <span class="li-head">content_length</span> - HTTP content length in request. <span class="li-normal">type: dict</span></li>
                <ul class="ul-self">
                <li> <span class="li-head">action</span> - Action. <span class="li-normal">type: str</span> <span class="li-normal">choices: allow, block</span></li>
                <li> <span class="li-head">length</span> - Length of HTTP content in bytes (0 to 2147483647). <span class="li-normal">type: int</span></li>
                <li> <span class="li-head">log</span> - Enable/disable logging. <span class="li-normal">type: str</span> <span class="li-normal">choices: enable, disable</span></li>
                <li> <span class="li-head">severity</span> - Severity. <span class="li-normal">type: str</span> <span class="li-normal">choices: high, medium, low</span></li>
                <li> <span class="li-head">status</span> - Enable/disable the constraint. <span class="li-normal">type: str</span> <span class="li-normal">choices: enable, disable</span></li>
                </ul>
            <li> <span class="li-head">exception</span> - HTTP constraint exception. <span class="li-normal">type: list</span></li>
                <ul class="ul-self">
                <li> <span class="li-head">address</span> - Host address. Source firewall.address.name firewall.addrgrp.name. <span class="li-normal">type: str</span></li>
                <li> <span class="li-head">content_length</span> - HTTP content length in request. <span class="li-normal">type: str</span> <span class="li-normal">choices: enable, disable</span></li>
                <li> <span class="li-head">header_length</span> - HTTP header length in request. <span class="li-normal">type: str</span> <span class="li-normal">choices: enable, disable</span></li>
                <li> <span class="li-head">hostname</span> - Enable/disable hostname check. <span class="li-normal">type: str</span> <span class="li-normal">choices: enable, disable</span></li>
                <li> <span class="li-head">id</span> - Exception ID. <span class="li-normal">type: int</span> <span class="li-required">required: True</span></li>
                <li> <span class="li-head">line_length</span> - HTTP line length in request. <span class="li-normal">type: str</span> <span class="li-normal">choices: enable, disable</span></li>
                <li> <span class="li-head">malformed</span> - Enable/disable malformed HTTP request check. <span class="li-normal">type: str</span> <span class="li-normal">choices: enable, disable</span></li>
                <li> <span class="li-head">max_cookie</span> - Maximum number of cookies in HTTP request. <span class="li-normal">type: str</span> <span class="li-normal">choices: enable, disable</span></li>
                <li> <span class="li-head">max_header_line</span> - Maximum number of HTTP header line. <span class="li-normal">type: str</span> <span class="li-normal">choices: enable, disable</span></li>
                <li> <span class="li-head">max_range_segment</span> - Maximum number of range segments in HTTP range line. <span class="li-normal">type: str</span> <span class="li-normal">choices: enable, disable</span></li>
                <li> <span class="li-head">max_url_param</span> - Maximum number of parameters in URL. <span class="li-normal">type: str</span> <span class="li-normal">choices: enable, disable</span></li>
                <li> <span class="li-head">method</span> - Enable/disable HTTP method check. <span class="li-normal">type: str</span> <span class="li-normal">choices: enable, disable</span></li>
                <li> <span class="li-head">param_length</span> - Maximum length of parameter in URL, HTTP POST request or HTTP body. <span class="li-normal">type: str</span> <span class="li-normal">choices: enable, disable</span></li>
                <li> <span class="li-head">pattern</span> - URL pattern. <span class="li-normal">type: str</span></li>
                <li> <span class="li-head">regex</span> - Enable/disable regular expression based pattern match. <span class="li-normal">type: str</span> <span class="li-normal">choices: enable, disable</span></li>
                <li> <span class="li-head">url_param_length</span> - Maximum length of parameter in URL. <span class="li-normal">type: str</span> <span class="li-normal">choices: enable, disable</span></li>
                <li> <span class="li-head">version</span> - Enable/disable HTTP version check. <span class="li-normal">type: str</span> <span class="li-normal">choices: enable, disable</span></li>
                </ul>
            <li> <span class="li-head">header_length</span> - HTTP header length in request. <span class="li-normal">type: dict</span></li>
                <ul class="ul-self">
                <li> <span class="li-head">action</span> - Action. <span class="li-normal">type: str</span> <span class="li-normal">choices: allow, block</span></li>
                <li> <span class="li-head">length</span> - Length of HTTP header in bytes (0 to 2147483647). <span class="li-normal">type: int</span></li>
                <li> <span class="li-head">log</span> - Enable/disable logging. <span class="li-normal">type: str</span> <span class="li-normal">choices: enable, disable</span></li>
                <li> <span class="li-head">severity</span> - Severity. <span class="li-normal">type: str</span> <span class="li-normal">choices: high, medium, low</span></li>
                <li> <span class="li-head">status</span> - Enable/disable the constraint. <span class="li-normal">type: str</span> <span class="li-normal">choices: enable, disable</span></li>
                </ul>
            <li> <span class="li-head">hostname</span> - Enable/disable hostname check. <span class="li-normal">type: dict</span></li>
                <ul class="ul-self">
                <li> <span class="li-head">action</span> - Action. <span class="li-normal">type: str</span> <span class="li-normal">choices: allow, block</span></li>
                <li> <span class="li-head">log</span> - Enable/disable logging. <span class="li-normal">type: str</span> <span class="li-normal">choices: enable, disable</span></li>
                <li> <span class="li-head">severity</span> - Severity. <span class="li-normal">type: str</span> <span class="li-normal">choices: high, medium, low</span></li>
                <li> <span class="li-head">status</span> - Enable/disable the constraint. <span class="li-normal">type: str</span> <span class="li-normal">choices: enable, disable</span></li>
                </ul>
            <li> <span class="li-head">line_length</span> - HTTP line length in request. <span class="li-normal">type: dict</span></li>
                <ul class="ul-self">
                <li> <span class="li-head">action</span> - Action. <span class="li-normal">type: str</span> <span class="li-normal">choices: allow, block</span></li>
                <li> <span class="li-head">length</span> - Length of HTTP line in bytes (0 to 2147483647). <span class="li-normal">type: int</span></li>
                <li> <span class="li-head">log</span> - Enable/disable logging. <span class="li-normal">type: str</span> <span class="li-normal">choices: enable, disable</span></li>
                <li> <span class="li-head">severity</span> - Severity. <span class="li-normal">type: str</span> <span class="li-normal">choices: high, medium, low</span></li>
                <li> <span class="li-head">status</span> - Enable/disable the constraint. <span class="li-normal">type: str</span> <span class="li-normal">choices: enable, disable</span></li>
                </ul>
            <li> <span class="li-head">malformed</span> - Enable/disable malformed HTTP request check. <span class="li-normal">type: dict</span></li>
                <ul class="ul-self">
                <li> <span class="li-head">action</span> - Action. <span class="li-normal">type: str</span> <span class="li-normal">choices: allow, block</span></li>
                <li> <span class="li-head">log</span> - Enable/disable logging. <span class="li-normal">type: str</span> <span class="li-normal">choices: enable, disable</span></li>
                <li> <span class="li-head">severity</span> - Severity. <span class="li-normal">type: str</span> <span class="li-normal">choices: high, medium, low</span></li>
                <li> <span class="li-head">status</span> - Enable/disable the constraint. <span class="li-normal">type: str</span> <span class="li-normal">choices: enable, disable</span></li>
                </ul>
            <li> <span class="li-head">max_cookie</span> - Maximum number of cookies in HTTP request. <span class="li-normal">type: dict</span></li>
                <ul class="ul-self">
                <li> <span class="li-head">action</span> - Action. <span class="li-normal">type: str</span> <span class="li-normal">choices: allow, block</span></li>
                <li> <span class="li-head">log</span> - Enable/disable logging. <span class="li-normal">type: str</span> <span class="li-normal">choices: enable, disable</span></li>
                <li> <span class="li-head">max_cookie</span> - Maximum number of cookies in HTTP request (0 to 2147483647). <span class="li-normal">type: int</span></li>
                <li> <span class="li-head">severity</span> - Severity. <span class="li-normal">type: str</span> <span class="li-normal">choices: high, medium, low</span></li>
                <li> <span class="li-head">status</span> - Enable/disable the constraint. <span class="li-normal">type: str</span> <span class="li-normal">choices: enable, disable</span></li>
                </ul>
            <li> <span class="li-head">max_header_line</span> - Maximum number of HTTP header line. <span class="li-normal">type: dict</span></li>
                <ul class="ul-self">
                <li> <span class="li-head">action</span> - Action. <span class="li-normal">type: str</span> <span class="li-normal">choices: allow, block</span></li>
                <li> <span class="li-head">log</span> - Enable/disable logging. <span class="li-normal">type: str</span> <span class="li-normal">choices: enable, disable</span></li>
                <li> <span class="li-head">max_header_line</span> - Maximum number HTTP header lines (0 to 2147483647). <span class="li-normal">type: int</span></li>
                <li> <span class="li-head">severity</span> - Severity. <span class="li-normal">type: str</span> <span class="li-normal">choices: high, medium, low</span></li>
                <li> <span class="li-head">status</span> - Enable/disable the constraint. <span class="li-normal">type: str</span> <span class="li-normal">choices: enable, disable</span></li>
                </ul>
            <li> <span class="li-head">max_range_segment</span> - Maximum number of range segments in HTTP range line. <span class="li-normal">type: dict</span></li>
                <ul class="ul-self">
                <li> <span class="li-head">action</span> - Action. <span class="li-normal">type: str</span> <span class="li-normal">choices: allow, block</span></li>
                <li> <span class="li-head">log</span> - Enable/disable logging. <span class="li-normal">type: str</span> <span class="li-normal">choices: enable, disable</span></li>
                <li> <span class="li-head">max_range_segment</span> - Maximum number of range segments in HTTP range line (0 to 2147483647). <span class="li-normal">type: int</span></li>
                <li> <span class="li-head">severity</span> - Severity. <span class="li-normal">type: str</span> <span class="li-normal">choices: high, medium, low</span></li>
                <li> <span class="li-head">status</span> - Enable/disable the constraint. <span class="li-normal">type: str</span> <span class="li-normal">choices: enable, disable</span></li>
                </ul>
            <li> <span class="li-head">max_url_param</span> - Maximum number of parameters in URL. <span class="li-normal">type: dict</span></li>
                <ul class="ul-self">
                <li> <span class="li-head">action</span> - Action. <span class="li-normal">type: str</span> <span class="li-normal">choices: allow, block</span></li>
                <li> <span class="li-head">log</span> - Enable/disable logging. <span class="li-normal">type: str</span> <span class="li-normal">choices: enable, disable</span></li>
                <li> <span class="li-head">max_url_param</span> - Maximum number of parameters in URL (0 to 2147483647). <span class="li-normal">type: int</span></li>
                <li> <span class="li-head">severity</span> - Severity. <span class="li-normal">type: str</span> <span class="li-normal">choices: high, medium, low</span></li>
                <li> <span class="li-head">status</span> - Enable/disable the constraint. <span class="li-normal">type: str</span> <span class="li-normal">choices: enable, disable</span></li>
                </ul>
            <li> <span class="li-head">method</span> - Enable/disable HTTP method check. <span class="li-normal">type: dict</span></li>
                <ul class="ul-self">
                <li> <span class="li-head">action</span> - Action. <span class="li-normal">type: str</span> <span class="li-normal">choices: allow, block</span></li>
                <li> <span class="li-head">log</span> - Enable/disable logging. <span class="li-normal">type: str</span> <span class="li-normal">choices: enable, disable</span></li>
                <li> <span class="li-head">severity</span> - Severity. <span class="li-normal">type: str</span> <span class="li-normal">choices: high, medium, low</span></li>
                <li> <span class="li-head">status</span> - Enable/disable the constraint. <span class="li-normal">type: str</span> <span class="li-normal">choices: enable, disable</span></li>
                </ul>
            <li> <span class="li-head">param_length</span> - Maximum length of parameter in URL, HTTP POST request or HTTP body. <span class="li-normal">type: dict</span></li>
                <ul class="ul-self">
                <li> <span class="li-head">action</span> - Action. <span class="li-normal">type: str</span> <span class="li-normal">choices: allow, block</span></li>
                <li> <span class="li-head">length</span> - Maximum length of parameter in URL, HTTP POST request or HTTP body in bytes (0 to 2147483647). <span class="li-normal">type: int</span></li>
                <li> <span class="li-head">log</span> - Enable/disable logging. <span class="li-normal">type: str</span> <span class="li-normal">choices: enable, disable</span></li>
                <li> <span class="li-head">severity</span> - Severity. <span class="li-normal">type: str</span> <span class="li-normal">choices: high, medium, low</span></li>
                <li> <span class="li-head">status</span> - Enable/disable the constraint. <span class="li-normal">type: str</span> <span class="li-normal">choices: enable, disable</span></li>
                </ul>
            <li> <span class="li-head">url_param_length</span> - Maximum length of parameter in URL. <span class="li-normal">type: dict</span></li>
                <ul class="ul-self">
                <li> <span class="li-head">action</span> - Action. <span class="li-normal">type: str</span> <span class="li-normal">choices: allow, block</span></li>
                <li> <span class="li-head">length</span> - Maximum length of URL parameter in bytes (0 to 2147483647). <span class="li-normal">type: int</span></li>
                <li> <span class="li-head">log</span> - Enable/disable logging. <span class="li-normal">type: str</span> <span class="li-normal">choices: enable, disable</span></li>
                <li> <span class="li-head">severity</span> - Severity. <span class="li-normal">type: str</span> <span class="li-normal">choices: high, medium, low</span></li>
                <li> <span class="li-head">status</span> - Enable/disable the constraint. <span class="li-normal">type: str</span> <span class="li-normal">choices: enable, disable</span></li>
                </ul>
            <li> <span class="li-head">version</span> - Enable/disable HTTP version check. <span class="li-normal">type: dict</span></li>
                <ul class="ul-self">
                <li> <span class="li-head">action</span> - Action. <span class="li-normal">type: str</span> <span class="li-normal">choices: allow, block</span></li>
                <li> <span class="li-head">log</span> - Enable/disable logging. <span class="li-normal">type: str</span> <span class="li-normal">choices: enable, disable</span></li>
                <li> <span class="li-head">severity</span> - Severity. <span class="li-normal">type: str</span> <span class="li-normal">choices: high, medium, low</span></li>
                <li> <span class="li-head">status</span> - Enable/disable the constraint. <span class="li-normal">type: str</span> <span class="li-normal">choices: enable, disable</span></li>
                </ul>
            </ul>
        <li> <span class="li-head">extended_log</span> - Enable/disable extended logging. <span class="li-normal">type: str</span> <span class="li-normal">choices: enable, disable</span></li>
        <li> <span class="li-head">external</span> - Disable/Enable external HTTP Inspection. <span class="li-normal">type: str</span> <span class="li-normal">choices: disable, enable</span></li>
        <li> <span class="li-head">method</span> - Method restriction. <span class="li-normal">type: dict</span></li>
            <ul class="ul-self">
            <li> <span class="li-head">default_allowed_methods</span> - Methods. <span class="li-normal">type: str</span> <span class="li-normal">choices: get, post, put, head, connect, trace, options, delete, others</span></li>
            <li> <span class="li-head">log</span> - Enable/disable logging. <span class="li-normal">type: str</span> <span class="li-normal">choices: enable, disable</span></li>
            <li> <span class="li-head">method_policy</span> - HTTP method policy. <span class="li-normal">type: list</span></li>
                <ul class="ul-self">
                <li> <span class="li-head">address</span> - Host address. Source firewall.address.name firewall.addrgrp.name. <span class="li-normal">type: str</span></li>
                <li> <span class="li-head">allowed_methods</span> - Allowed Methods. <span class="li-normal">type: str</span> <span class="li-normal">choices: get, post, put, head, connect, trace, options, delete, others</span></li>
                <li> <span class="li-head">id</span> - HTTP method policy ID. <span class="li-normal">type: int</span> <span class="li-required">required: True</span></li>
                <li> <span class="li-head">pattern</span> - URL pattern. <span class="li-normal">type: str</span></li>
                <li> <span class="li-head">regex</span> - Enable/disable regular expression based pattern match. <span class="li-normal">type: str</span> <span class="li-normal">choices: enable, disable</span></li>
                </ul>
            <li> <span class="li-head">severity</span> - Severity. <span class="li-normal">type: str</span> <span class="li-normal">choices: high, medium, low</span></li>
            <li> <span class="li-head">status</span> - Status. <span class="li-normal">type: str</span> <span class="li-normal">choices: enable, disable</span></li>
            </ul>
        <li> <span class="li-head">name</span> - WAF Profile name. <span class="li-normal">type: str</span> <span class="li-required">required: True</span></li>
        <li> <span class="li-head">signature</span> - WAF signatures. <span class="li-normal">type: dict</span></li>
            <ul class="ul-self">
            <li> <span class="li-head">credit_card_detection_threshold</span> - The minimum number of Credit cards to detect violation. <span class="li-normal">type: int</span></li>
            <li> <span class="li-head">custom_signature</span> - Custom signature. <span class="li-normal">type: list</span></li>
                <ul class="ul-self">
                <li> <span class="li-head">action</span> - Action. <span class="li-normal">type: str</span> <span class="li-normal">choices: allow, block, erase</span></li>
                <li> <span class="li-head">case_sensitivity</span> - Case sensitivity in pattern. <span class="li-normal">type: str</span> <span class="li-normal">choices: disable, enable</span></li>
                <li> <span class="li-head">direction</span> - Traffic direction. <span class="li-normal">type: str</span> <span class="li-normal">choices: request, response</span></li>
                <li> <span class="li-head">log</span> - Enable/disable logging. <span class="li-normal">type: str</span> <span class="li-normal">choices: enable, disable</span></li>
                <li> <span class="li-head">name</span> - Signature name. <span class="li-normal">type: str</span> <span class="li-required">required: True</span></li>
                <li> <span class="li-head">pattern</span> - Match pattern. <span class="li-normal">type: str</span></li>
                <li> <span class="li-head">severity</span> - Severity. <span class="li-normal">type: str</span> <span class="li-normal">choices: high, medium, low</span></li>
                <li> <span class="li-head">status</span> - Status. <span class="li-normal">type: str</span> <span class="li-normal">choices: enable, disable</span></li>
                <li> <span class="li-head">target</span> - Match HTTP target. <span class="li-normal">type: str</span> <span class="li-normal">choices: arg, arg-name, req-body, req-cookie, req-cookie-name, req-filename, req-header, req-header-name, req-raw-uri, req-uri, resp-body, resp-hdr, resp-status</span></li>
                </ul>
            <li> <span class="li-head">disabled_signature</span> - Disabled signatures <span class="li-normal">type: list</span></li>
                <ul class="ul-self">
                <li> <span class="li-head">id</span> - Signature ID. Source waf.signature.id. <span class="li-normal">type: int</span> <span class="li-required">required: True</span></li>
                </ul>
            <li> <span class="li-head">disabled_sub_class</span> - Disabled signature subclasses. <span class="li-normal">type: list</span></li>
                <ul class="ul-self">
                <li> <span class="li-head">id</span> - Signature subclass ID. Source waf.sub-class.id. <span class="li-normal">type: int</span> <span class="li-required">required: True</span></li>
                </ul>
            <li> <span class="li-head">main_class</span> - Main signature class. <span class="li-normal">type: list</span></li>
                <ul class="ul-self">
                <li> <span class="li-head">action</span> - Action. <span class="li-normal">type: str</span> <span class="li-normal">choices: allow, block, erase</span></li>
                <li> <span class="li-head">id</span> - Main signature class ID. Source waf.main-class.id. <span class="li-normal">type: int</span> <span class="li-required">required: True</span></li>
                <li> <span class="li-head">log</span> - Enable/disable logging. <span class="li-normal">type: str</span> <span class="li-normal">choices: enable, disable</span></li>
                <li> <span class="li-head">severity</span> - Severity. <span class="li-normal">type: str</span> <span class="li-normal">choices: high, medium, low</span></li>
                <li> <span class="li-head">status</span> - Status. <span class="li-normal">type: str</span> <span class="li-normal">choices: enable, disable</span></li>
                </ul>
            </ul>
        <li> <span class="li-head">url_access</span> - URL access list <span class="li-normal">type: list</span></li>
            <ul class="ul-self">
            <li> <span class="li-head">access_pattern</span> - URL access pattern. <span class="li-normal">type: list</span></li>
                <ul class="ul-self">
                <li> <span class="li-head">id</span> - URL access pattern ID. <span class="li-normal">type: int</span> <span class="li-required">required: True</span></li>
                <li> <span class="li-head">negate</span> - Enable/disable match negation. <span class="li-normal">type: str</span> <span class="li-normal">choices: enable, disable</span></li>
                <li> <span class="li-head">pattern</span> - URL pattern. <span class="li-normal">type: str</span></li>
                <li> <span class="li-head">regex</span> - Enable/disable regular expression based pattern match. <span class="li-normal">type: str</span> <span class="li-normal">choices: enable, disable</span></li>
                <li> <span class="li-head">srcaddr</span> - Source address. Source firewall.address.name firewall.addrgrp.name. <span class="li-normal">type: str</span></li>
                </ul>
            <li> <span class="li-head">action</span> - Action. <span class="li-normal">type: str</span> <span class="li-normal">choices: bypass, permit, block</span></li>
            <li> <span class="li-head">address</span> - Host address. Source firewall.address.name firewall.addrgrp.name. <span class="li-normal">type: str</span></li>
            <li> <span class="li-head">id</span> - URL access ID. <span class="li-normal">type: int</span> <span class="li-required">required: True</span></li>
            <li> <span class="li-head">log</span> - Enable/disable logging. <span class="li-normal">type: str</span> <span class="li-normal">choices: enable, disable</span></li>
            <li> <span class="li-head">severity</span> - Severity. <span class="li-normal">type: str</span> <span class="li-normal">choices: high, medium, low</span></li>
            </ul>
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
      - name: Web application firewall configuration.
        fortios_waf_profile:
          vdom:  "{{ vdom }}"
          state: "present"
          access_token: "<your_own_value>"
          waf_profile:
            address_list:
                blocked_address:
                 -
                    name: "default_name_5 (source firewall.address.name firewall.addrgrp.name)"
                blocked_log: "enable"
                severity: "high"
                status: "enable"
                trusted_address:
                 -
                    name: "default_name_10 (source firewall.address.name firewall.addrgrp.name)"
            comment: "Comment."
            constraint:
                content_length:
                    action: "allow"
                    length: "15"
                    log: "enable"
                    severity: "high"
                    status: "enable"
                exception:
                 -
                    address: "<your_own_value> (source firewall.address.name firewall.addrgrp.name)"
                    content_length: "enable"
                    header_length: "enable"
                    hostname: "enable"
                    id:  "24"
                    line_length: "enable"
                    malformed: "enable"
                    max_cookie: "enable"
                    max_header_line: "enable"
                    max_range_segment: "enable"
                    max_url_param: "enable"
                    method: "enable"
                    param_length: "enable"
                    pattern: "<your_own_value>"
                    regex: "enable"
                    url_param_length: "enable"
                    version: "enable"
                header_length:
                    action: "allow"
                    length: "39"
                    log: "enable"
                    severity: "high"
                    status: "enable"
                hostname:
                    action: "allow"
                    log: "enable"
                    severity: "high"
                    status: "enable"
                line_length:
                    action: "allow"
                    length: "50"
                    log: "enable"
                    severity: "high"
                    status: "enable"
                malformed:
                    action: "allow"
                    log: "enable"
                    severity: "high"
                    status: "enable"
                max_cookie:
                    action: "allow"
                    log: "enable"
                    max_cookie: "62"
                    severity: "high"
                    status: "enable"
                max_header_line:
                    action: "allow"
                    log: "enable"
                    max_header_line: "68"
                    severity: "high"
                    status: "enable"
                max_range_segment:
                    action: "allow"
                    log: "enable"
                    max_range_segment: "74"
                    severity: "high"
                    status: "enable"
                max_url_param:
                    action: "allow"
                    log: "enable"
                    max_url_param: "80"
                    severity: "high"
                    status: "enable"
                method:
                    action: "allow"
                    log: "enable"
                    severity: "high"
                    status: "enable"
                param_length:
                    action: "allow"
                    length: "90"
                    log: "enable"
                    severity: "high"
                    status: "enable"
                url_param_length:
                    action: "allow"
                    length: "96"
                    log: "enable"
                    severity: "high"
                    status: "enable"
                version:
                    action: "allow"
                    log: "enable"
                    severity: "high"
                    status: "enable"
            extended_log: "enable"
            external: "disable"
            method:
                default_allowed_methods: "get"
                log: "enable"
                method_policy:
                 -
                    address: "<your_own_value> (source firewall.address.name firewall.addrgrp.name)"
                    allowed_methods: "get"
                    id:  "113"
                    pattern: "<your_own_value>"
                    regex: "enable"
                severity: "high"
                status: "enable"
            name: "default_name_118"
            signature:
                credit_card_detection_threshold: "120"
                custom_signature:
                 -
                    action: "allow"
                    case_sensitivity: "disable"
                    direction: "request"
                    log: "enable"
                    name: "default_name_126"
                    pattern: "<your_own_value>"
                    severity: "high"
                    status: "enable"
                    target: "arg"
                disabled_signature:
                 -
                    id:  "132 (source waf.signature.id)"
                disabled_sub_class:
                 -
                    id:  "134 (source waf.sub-class.id)"
                main_class:
                 -
                    action: "allow"
                    id:  "137 (source waf.main-class.id)"
                    log: "enable"
                    severity: "high"
                    status: "enable"
            url_access:
             -
                access_pattern:
                 -
                    id:  "143"
                    negate: "enable"
                    pattern: "<your_own_value>"
                    regex: "enable"
                    srcaddr: "<your_own_value> (source firewall.address.name firewall.addrgrp.name)"
                action: "bypass"
                address: "<your_own_value> (source firewall.address.name firewall.addrgrp.name)"
                id:  "150"
                log: "enable"
                severity: "high"
    


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
