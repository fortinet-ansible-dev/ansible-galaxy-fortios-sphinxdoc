:source: fortios_firewall_profile_protocol_options.py

:orphan:

.. fortios_firewall_profile_protocol_options:

fortios_firewall_profile_protocol_options -- Configure protocol options in Fortinet's FortiOS and FortiGate.
++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++

.. versionadded:: 2.8

.. contents::
   :local:
   :depth: 1


Synopsis
--------
- This module is able to configure a FortiGate or FortiOS (FOS) device by allowing the user to set and modify firewall feature and profile_protocol_options category. Examples include all parameters and values need to be adjusted to datasources before usage. Tested with FOS v6.4.0



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
    <li> <span class="li-head">firewall_profile_protocol_options</span> - Configure protocol options. <span class="li-normal">type: dict</span></li>
        <ul class="ul-self">
        <li> <span class="li-head">state</span> - B(Deprecated) <span class="li-normal">type: str</span> <span class="li-required">required: False</span> <span class="li-normal">choices: present, absent</span></li>
        <li> <span class="li-head">cifs</span> - Configure CIFS protocol options. <span class="li-normal">type: dict</span></li>
            <ul class="ul-self">
            <li> <span class="li-head">options</span> - One or more options that can be applied to the session. <span class="li-normal">type: str</span> <span class="li-normal">choices: oversize</span></li>
            <li> <span class="li-head">oversize_limit</span> - Maximum in-memory file size that can be scanned (1 - 383 MB). <span class="li-normal">type: int</span></li>
            <li> <span class="li-head">ports</span> - Ports to scan for content (1 - 65535). <span class="li-normal">type: int</span></li>
            <li> <span class="li-head">scan_bzip2</span> - Enable/disable scanning of BZip2 compressed files. <span class="li-normal">type: str</span> <span class="li-normal">choices: enable, disable</span></li>
            <li> <span class="li-head">status</span> - Enable/disable the active status of scanning for this protocol. <span class="li-normal">type: str</span> <span class="li-normal">choices: enable, disable</span></li>
            <li> <span class="li-head">tcp_window_maximum</span> - Maximum dynamic TCP window size . <span class="li-normal">type: int</span></li>
            <li> <span class="li-head">tcp_window_minimum</span> - Minimum dynamic TCP window size . <span class="li-normal">type: int</span></li>
            <li> <span class="li-head">tcp_window_size</span> - Set TCP static window size . <span class="li-normal">type: int</span></li>
            <li> <span class="li-head">tcp_window_type</span> - Specify type of TCP window to use for this protocol. <span class="li-normal">type: str</span> <span class="li-normal">choices: system, static, dynamic</span></li>
            <li> <span class="li-head">uncompressed_nest_limit</span> - Maximum nested levels of compression that can be uncompressed and scanned (2 - 100). <span class="li-normal">type: int</span></li>
            <li> <span class="li-head">uncompressed_oversize_limit</span> - Maximum in-memory uncompressed file size that can be scanned (0 - 383 MB, 0 = unlimited). <span class="li-normal">type: int</span></li>
            </ul>
        <li> <span class="li-head">comment</span> - Optional comments. <span class="li-normal">type: str</span></li>
        <li> <span class="li-head">dns</span> - Configure DNS protocol options. <span class="li-normal">type: dict</span></li>
            <ul class="ul-self">
            <li> <span class="li-head">ports</span> - Ports to scan for content (1 - 65535). <span class="li-normal">type: int</span></li>
            <li> <span class="li-head">status</span> - Enable/disable the active status of scanning for this protocol. <span class="li-normal">type: str</span> <span class="li-normal">choices: enable, disable</span></li>
            </ul>
        <li> <span class="li-head">feature_set</span> - Flow/proxy feature set. <span class="li-normal">type: str</span> <span class="li-normal">choices: flow, proxy</span></li>
        <li> <span class="li-head">ftp</span> - Configure FTP protocol options. <span class="li-normal">type: dict</span></li>
            <ul class="ul-self">
            <li> <span class="li-head">comfort_amount</span> - Amount of data to send in a transmission for client comforting (1 - 65535 bytes). <span class="li-normal">type: int</span></li>
            <li> <span class="li-head">comfort_interval</span> - Period of time between start, or last transmission, and the next client comfort transmission of data (1 - 900 sec). <span class="li-normal">type: int</span></li>
            <li> <span class="li-head">inspect_all</span> - Enable/disable the inspection of all ports for the protocol. <span class="li-normal">type: str</span> <span class="li-normal">choices: enable, disable</span></li>
            <li> <span class="li-head">options</span> - One or more options that can be applied to the session. <span class="li-normal">type: str</span> <span class="li-normal">choices: clientcomfort, oversize, splice, bypass-rest-command, bypass-mode-command</span></li>
            <li> <span class="li-head">oversize_limit</span> - Maximum in-memory file size that can be scanned (1 - 383 MB). <span class="li-normal">type: int</span></li>
            <li> <span class="li-head">ports</span> - Ports to scan for content (1 - 65535). <span class="li-normal">type: int</span></li>
            <li> <span class="li-head">scan_bzip2</span> - Enable/disable scanning of BZip2 compressed files. <span class="li-normal">type: str</span> <span class="li-normal">choices: enable, disable</span></li>
            <li> <span class="li-head">ssl_offloaded</span> - SSL decryption and encryption performed by an external device. <span class="li-normal">type: str</span> <span class="li-normal">choices: False, True</span></li>
            <li> <span class="li-head">status</span> - Enable/disable the active status of scanning for this protocol. <span class="li-normal">type: str</span> <span class="li-normal">choices: enable, disable</span></li>
            <li> <span class="li-head">uncompressed_nest_limit</span> - Maximum nested levels of compression that can be uncompressed and scanned (2 - 100). <span class="li-normal">type: int</span></li>
            <li> <span class="li-head">uncompressed_oversize_limit</span> - Maximum in-memory uncompressed file size that can be scanned (0 - 383 MB, 0 = unlimited). <span class="li-normal">type: int</span></li>
            </ul>
        <li> <span class="li-head">http</span> - Configure HTTP protocol options. <span class="li-normal">type: dict</span></li>
            <ul class="ul-self">
            <li> <span class="li-head">block_page_status_code</span> - Code number returned for blocked HTTP pages (non-FortiGuard only) (100 - 599). <span class="li-normal">type: int</span></li>
            <li> <span class="li-head">comfort_amount</span> - Amount of data to send in a transmission for client comforting (1 - 65535 bytes). <span class="li-normal">type: int</span></li>
            <li> <span class="li-head">comfort_interval</span> - Period of time between start, or last transmission, and the next client comfort transmission of data (1 - 900 sec). <span class="li-normal">type: int</span></li>
            <li> <span class="li-head">fortinet_bar</span> - Enable/disable Fortinet bar on HTML content. <span class="li-normal">type: str</span> <span class="li-normal">choices: enable, disable</span></li>
            <li> <span class="li-head">fortinet_bar_port</span> - Port for use by Fortinet Bar (1 - 65535). <span class="li-normal">type: int</span></li>
            <li> <span class="li-head">inspect_all</span> - Enable/disable the inspection of all ports for the protocol. <span class="li-normal">type: str</span> <span class="li-normal">choices: enable, disable</span></li>
            <li> <span class="li-head">options</span> - One or more options that can be applied to the session. <span class="li-normal">type: str</span> <span class="li-normal">choices: clientcomfort, servercomfort, oversize, chunkedbypass</span></li>
            <li> <span class="li-head">oversize_limit</span> - Maximum in-memory file size that can be scanned (1 - 383 MB). <span class="li-normal">type: int</span></li>
            <li> <span class="li-head">ports</span> - Ports to scan for content (1 - 65535). <span class="li-normal">type: int</span></li>
            <li> <span class="li-head">post_lang</span> - ID codes for character sets to be used to convert to UTF-8 for banned words and DLP on HTTP posts (maximum of 5 character sets). <span class="li-normal">type: str</span> <span class="li-normal">choices: jisx0201, jisx0208, jisx0212, gb2312, ksc5601-ex, euc-jp, sjis, iso2022-jp, iso2022-jp-1, iso2022-jp-2, euc-cn, ces-gbk, hz, ces-big5, euc-kr, iso2022-jp-3, iso8859-1, tis620, cp874, cp1252, cp1251</span></li>
            <li> <span class="li-head">proxy_after_tcp_handshake</span> - Proxy traffic after the TCP 3-way handshake has been established (not before). <span class="li-normal">type: str</span> <span class="li-normal">choices: enable, disable</span></li>
            <li> <span class="li-head">range_block</span> - Enable/disable blocking of partial downloads. <span class="li-normal">type: str</span> <span class="li-normal">choices: disable, enable</span></li>
            <li> <span class="li-head">retry_count</span> - Number of attempts to retry HTTP connection (0 - 100). <span class="li-normal">type: int</span></li>
            <li> <span class="li-head">scan_bzip2</span> - Enable/disable scanning of BZip2 compressed files. <span class="li-normal">type: str</span> <span class="li-normal">choices: enable, disable</span></li>
            <li> <span class="li-head">ssl_offloaded</span> - SSL decryption and encryption performed by an external device. <span class="li-normal">type: str</span> <span class="li-normal">choices: False, True</span></li>
            <li> <span class="li-head">status</span> - Enable/disable the active status of scanning for this protocol. <span class="li-normal">type: str</span> <span class="li-normal">choices: enable, disable</span></li>
            <li> <span class="li-head">stream_based_uncompressed_limit</span> - Maximum stream-based uncompressed data size that will be scanned (MB, 0 = unlimited (default).  Stream-based uncompression used only under certain conditions.). <span class="li-normal">type: int</span></li>
            <li> <span class="li-head">streaming_content_bypass</span> - Enable/disable bypassing of streaming content from buffering. <span class="li-normal">type: str</span> <span class="li-normal">choices: enable, disable</span></li>
            <li> <span class="li-head">strip_x_forwarded_for</span> - Enable/disable stripping of HTTP X-Forwarded-For header. <span class="li-normal">type: str</span> <span class="li-normal">choices: disable, enable</span></li>
            <li> <span class="li-head">switching_protocols</span> - Bypass from scanning, or block a connection that attempts to switch protocol. <span class="li-normal">type: str</span> <span class="li-normal">choices: bypass, block</span></li>
            <li> <span class="li-head">tcp_window_maximum</span> - Maximum dynamic TCP window size . <span class="li-normal">type: int</span></li>
            <li> <span class="li-head">tcp_window_minimum</span> - Minimum dynamic TCP window size . <span class="li-normal">type: int</span></li>
            <li> <span class="li-head">tcp_window_size</span> - Set TCP static window size . <span class="li-normal">type: int</span></li>
            <li> <span class="li-head">tcp_window_type</span> - Specify type of TCP window to use for this protocol. <span class="li-normal">type: str</span> <span class="li-normal">choices: system, static, dynamic</span></li>
            <li> <span class="li-head">tunnel_non_http</span> - Configure how to process non-HTTP traffic when a profile configured for HTTP traffic accepts a non-HTTP session. Can occur if an application sends non-HTTP traffic using an HTTP destination port. <span class="li-normal">type: str</span> <span class="li-normal">choices: enable, disable</span></li>
            <li> <span class="li-head">uncompressed_nest_limit</span> - Maximum nested levels of compression that can be uncompressed and scanned (2 - 100). <span class="li-normal">type: int</span></li>
            <li> <span class="li-head">uncompressed_oversize_limit</span> - Maximum in-memory uncompressed file size that can be scanned (0 - 383 MB, 0 = unlimited). <span class="li-normal">type: int</span></li>
            <li> <span class="li-head">unknown_http_version</span> - How to handle HTTP sessions that do not comply with HTTP 0.9, 1.0, or 1.1. <span class="li-normal">type: str</span> <span class="li-normal">choices: reject, tunnel, best-effort</span></li>
            </ul>
        <li> <span class="li-head">imap</span> - Configure IMAP protocol options. <span class="li-normal">type: dict</span></li>
            <ul class="ul-self">
            <li> <span class="li-head">inspect_all</span> - Enable/disable the inspection of all ports for the protocol. <span class="li-normal">type: str</span> <span class="li-normal">choices: enable, disable</span></li>
            <li> <span class="li-head">options</span> - One or more options that can be applied to the session. <span class="li-normal">type: str</span> <span class="li-normal">choices: fragmail, oversize</span></li>
            <li> <span class="li-head">oversize_limit</span> - Maximum in-memory file size that can be scanned (1 - 383 MB). <span class="li-normal">type: int</span></li>
            <li> <span class="li-head">ports</span> - Ports to scan for content (1 - 65535). <span class="li-normal">type: int</span></li>
            <li> <span class="li-head">proxy_after_tcp_handshake</span> - Proxy traffic after the TCP 3-way handshake has been established (not before). <span class="li-normal">type: str</span> <span class="li-normal">choices: enable, disable</span></li>
            <li> <span class="li-head">scan_bzip2</span> - Enable/disable scanning of BZip2 compressed files. <span class="li-normal">type: str</span> <span class="li-normal">choices: enable, disable</span></li>
            <li> <span class="li-head">ssl_offloaded</span> - SSL decryption and encryption performed by an external device. <span class="li-normal">type: str</span> <span class="li-normal">choices: False, True</span></li>
            <li> <span class="li-head">status</span> - Enable/disable the active status of scanning for this protocol. <span class="li-normal">type: str</span> <span class="li-normal">choices: enable, disable</span></li>
            <li> <span class="li-head">uncompressed_nest_limit</span> - Maximum nested levels of compression that can be uncompressed and scanned (2 - 100). <span class="li-normal">type: int</span></li>
            <li> <span class="li-head">uncompressed_oversize_limit</span> - Maximum in-memory uncompressed file size that can be scanned (0 - 383 MB, 0 = unlimited). <span class="li-normal">type: int</span></li>
            </ul>
        <li> <span class="li-head">mail_signature</span> - Configure Mail signature. <span class="li-normal">type: dict</span></li>
            <ul class="ul-self">
            <li> <span class="li-head">signature</span> - Email signature to be added to outgoing email (if the signature contains spaces, enclose with quotation marks). <span class="li-normal">type: str</span></li>
            <li> <span class="li-head">status</span> - Enable/disable adding an email signature to SMTP email messages as they pass through the FortiGate. <span class="li-normal">type: str</span> <span class="li-normal">choices: disable, enable</span></li>
            </ul>
        <li> <span class="li-head">mapi</span> - Configure MAPI protocol options. <span class="li-normal">type: dict</span></li>
            <ul class="ul-self">
            <li> <span class="li-head">options</span> - One or more options that can be applied to the session. <span class="li-normal">type: str</span> <span class="li-normal">choices: fragmail, oversize</span></li>
            <li> <span class="li-head">oversize_limit</span> - Maximum in-memory file size that can be scanned (1 - 383 MB). <span class="li-normal">type: int</span></li>
            <li> <span class="li-head">ports</span> - Ports to scan for content (1 - 65535). <span class="li-normal">type: int</span></li>
            <li> <span class="li-head">scan_bzip2</span> - Enable/disable scanning of BZip2 compressed files. <span class="li-normal">type: str</span> <span class="li-normal">choices: enable, disable</span></li>
            <li> <span class="li-head">status</span> - Enable/disable the active status of scanning for this protocol. <span class="li-normal">type: str</span> <span class="li-normal">choices: enable, disable</span></li>
            <li> <span class="li-head">uncompressed_nest_limit</span> - Maximum nested levels of compression that can be uncompressed and scanned (2 - 100). <span class="li-normal">type: int</span></li>
            <li> <span class="li-head">uncompressed_oversize_limit</span> - Maximum in-memory uncompressed file size that can be scanned (0 - 383 MB, 0 = unlimited). <span class="li-normal">type: int</span></li>
            </ul>
        <li> <span class="li-head">name</span> - Name. <span class="li-normal">type: str</span> <span class="li-required">required: True</span></li>
        <li> <span class="li-head">nntp</span> - Configure NNTP protocol options. <span class="li-normal">type: dict</span></li>
            <ul class="ul-self">
            <li> <span class="li-head">inspect_all</span> - Enable/disable the inspection of all ports for the protocol. <span class="li-normal">type: str</span> <span class="li-normal">choices: enable, disable</span></li>
            <li> <span class="li-head">options</span> - One or more options that can be applied to the session. <span class="li-normal">type: str</span> <span class="li-normal">choices: oversize, splice</span></li>
            <li> <span class="li-head">oversize_limit</span> - Maximum in-memory file size that can be scanned (1 - 383 MB). <span class="li-normal">type: int</span></li>
            <li> <span class="li-head">ports</span> - Ports to scan for content (1 - 65535). <span class="li-normal">type: int</span></li>
            <li> <span class="li-head">proxy_after_tcp_handshake</span> - Proxy traffic after the TCP 3-way handshake has been established (not before). <span class="li-normal">type: str</span> <span class="li-normal">choices: enable, disable</span></li>
            <li> <span class="li-head">scan_bzip2</span> - Enable/disable scanning of BZip2 compressed files. <span class="li-normal">type: str</span> <span class="li-normal">choices: enable, disable</span></li>
            <li> <span class="li-head">status</span> - Enable/disable the active status of scanning for this protocol. <span class="li-normal">type: str</span> <span class="li-normal">choices: enable, disable</span></li>
            <li> <span class="li-head">uncompressed_nest_limit</span> - Maximum nested levels of compression that can be uncompressed and scanned (2 - 100). <span class="li-normal">type: int</span></li>
            <li> <span class="li-head">uncompressed_oversize_limit</span> - Maximum in-memory uncompressed file size that can be scanned (0 - 383 MB, 0 = unlimited). <span class="li-normal">type: int</span></li>
            </ul>
        <li> <span class="li-head">oversize_log</span> - Enable/disable logging for antivirus oversize file blocking. <span class="li-normal">type: str</span> <span class="li-normal">choices: disable, enable</span></li>
        <li> <span class="li-head">pop3</span> - Configure POP3 protocol options. <span class="li-normal">type: dict</span></li>
            <ul class="ul-self">
            <li> <span class="li-head">inspect_all</span> - Enable/disable the inspection of all ports for the protocol. <span class="li-normal">type: str</span> <span class="li-normal">choices: enable, disable</span></li>
            <li> <span class="li-head">options</span> - One or more options that can be applied to the session. <span class="li-normal">type: str</span> <span class="li-normal">choices: fragmail, oversize</span></li>
            <li> <span class="li-head">oversize_limit</span> - Maximum in-memory file size that can be scanned (1 - 383 MB). <span class="li-normal">type: int</span></li>
            <li> <span class="li-head">ports</span> - Ports to scan for content (1 - 65535). <span class="li-normal">type: int</span></li>
            <li> <span class="li-head">proxy_after_tcp_handshake</span> - Proxy traffic after the TCP 3-way handshake has been established (not before). <span class="li-normal">type: str</span> <span class="li-normal">choices: enable, disable</span></li>
            <li> <span class="li-head">scan_bzip2</span> - Enable/disable scanning of BZip2 compressed files. <span class="li-normal">type: str</span> <span class="li-normal">choices: enable, disable</span></li>
            <li> <span class="li-head">ssl_offloaded</span> - SSL decryption and encryption performed by an external device. <span class="li-normal">type: str</span> <span class="li-normal">choices: False, True</span></li>
            <li> <span class="li-head">status</span> - Enable/disable the active status of scanning for this protocol. <span class="li-normal">type: str</span> <span class="li-normal">choices: enable, disable</span></li>
            <li> <span class="li-head">uncompressed_nest_limit</span> - Maximum nested levels of compression that can be uncompressed and scanned (2 - 100). <span class="li-normal">type: int</span></li>
            <li> <span class="li-head">uncompressed_oversize_limit</span> - Maximum in-memory uncompressed file size that can be scanned (0 - 383 MB, 0 = unlimited). <span class="li-normal">type: int</span></li>
            </ul>
        <li> <span class="li-head">replacemsg_group</span> - Name of the replacement message group to be used Source system.replacemsg-group.name. <span class="li-normal">type: str</span></li>
        <li> <span class="li-head">rpc_over_http</span> - Enable/disable inspection of RPC over HTTP. <span class="li-normal">type: str</span> <span class="li-normal">choices: enable, disable</span></li>
        <li> <span class="li-head">smtp</span> - Configure SMTP protocol options. <span class="li-normal">type: dict</span></li>
            <ul class="ul-self">
            <li> <span class="li-head">inspect_all</span> - Enable/disable the inspection of all ports for the protocol. <span class="li-normal">type: str</span> <span class="li-normal">choices: enable, disable</span></li>
            <li> <span class="li-head">options</span> - One or more options that can be applied to the session. <span class="li-normal">type: str</span> <span class="li-normal">choices: fragmail, oversize, splice</span></li>
            <li> <span class="li-head">oversize_limit</span> - Maximum in-memory file size that can be scanned (1 - 383 MB). <span class="li-normal">type: int</span></li>
            <li> <span class="li-head">ports</span> - Ports to scan for content (1 - 65535). <span class="li-normal">type: int</span></li>
            <li> <span class="li-head">proxy_after_tcp_handshake</span> - Proxy traffic after the TCP 3-way handshake has been established (not before). <span class="li-normal">type: str</span> <span class="li-normal">choices: enable, disable</span></li>
            <li> <span class="li-head">scan_bzip2</span> - Enable/disable scanning of BZip2 compressed files. <span class="li-normal">type: str</span> <span class="li-normal">choices: enable, disable</span></li>
            <li> <span class="li-head">server_busy</span> - Enable/disable SMTP server busy when server not available. <span class="li-normal">type: str</span> <span class="li-normal">choices: enable, disable</span></li>
            <li> <span class="li-head">ssl_offloaded</span> - SSL decryption and encryption performed by an external device. <span class="li-normal">type: str</span> <span class="li-normal">choices: False, True</span></li>
            <li> <span class="li-head">status</span> - Enable/disable the active status of scanning for this protocol. <span class="li-normal">type: str</span> <span class="li-normal">choices: enable, disable</span></li>
            <li> <span class="li-head">uncompressed_nest_limit</span> - Maximum nested levels of compression that can be uncompressed and scanned (2 - 100). <span class="li-normal">type: int</span></li>
            <li> <span class="li-head">uncompressed_oversize_limit</span> - Maximum in-memory uncompressed file size that can be scanned (0 - 383 MB, 0 = unlimited). <span class="li-normal">type: int</span></li>
            </ul>
        <li> <span class="li-head">ssh</span> - Configure SFTP and SCP protocol options. <span class="li-normal">type: dict</span></li>
            <ul class="ul-self">
            <li> <span class="li-head">comfort_amount</span> - Amount of data to send in a transmission for client comforting (1 - 65535 bytes). <span class="li-normal">type: int</span></li>
            <li> <span class="li-head">comfort_interval</span> - Period of time between start, or last transmission, and the next client comfort transmission of data (1 - 900 sec). <span class="li-normal">type: int</span></li>
            <li> <span class="li-head">options</span> - One or more options that can be applied to the session. <span class="li-normal">type: str</span> <span class="li-normal">choices: oversize, clientcomfort, servercomfort</span></li>
            <li> <span class="li-head">oversize_limit</span> - Maximum in-memory file size that can be scanned (1 - 383 MB). <span class="li-normal">type: int</span></li>
            <li> <span class="li-head">scan_bzip2</span> - Enable/disable scanning of BZip2 compressed files. <span class="li-normal">type: str</span> <span class="li-normal">choices: enable, disable</span></li>
            <li> <span class="li-head">uncompressed_nest_limit</span> - Maximum nested levels of compression that can be uncompressed and scanned (2 - 100). <span class="li-normal">type: int</span></li>
            <li> <span class="li-head">uncompressed_oversize_limit</span> - Maximum in-memory uncompressed file size that can be scanned (0 - 383 MB, 0 = unlimited). <span class="li-normal">type: int</span></li>
            </ul>
        <li> <span class="li-head">switching_protocols_log</span> - Enable/disable logging for HTTP/HTTPS switching protocols. <span class="li-normal">type: str</span> <span class="li-normal">choices: disable, enable</span></li>
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
      - name: Configure protocol options.
        fortios_firewall_profile_protocol_options:
          vdom:  "{{ vdom }}"
          state: "present"
          access_token: "<your_own_value>"
          firewall_profile_protocol_options:
            cifs:
                options: "oversize"
                oversize_limit: "5"
                ports: "6"
                scan_bzip2: "enable"
                status: "enable"
                tcp_window_maximum: "9"
                tcp_window_minimum: "10"
                tcp_window_size: "11"
                tcp_window_type: "system"
                uncompressed_nest_limit: "13"
                uncompressed_oversize_limit: "14"
            comment: "Optional comments."
            dns:
                ports: "17"
                status: "enable"
            feature_set: "flow"
            ftp:
                comfort_amount: "21"
                comfort_interval: "22"
                inspect_all: "enable"
                options: "clientcomfort"
                oversize_limit: "25"
                ports: "26"
                scan_bzip2: "enable"
                ssl_offloaded: "no"
                status: "enable"
                uncompressed_nest_limit: "30"
                uncompressed_oversize_limit: "31"
            http:
                block_page_status_code: "33"
                comfort_amount: "34"
                comfort_interval: "35"
                fortinet_bar: "enable"
                fortinet_bar_port: "37"
                inspect_all: "enable"
                options: "clientcomfort"
                oversize_limit: "40"
                ports: "41"
                post_lang: "jisx0201"
                proxy_after_tcp_handshake: "enable"
                range_block: "disable"
                retry_count: "45"
                scan_bzip2: "enable"
                ssl_offloaded: "no"
                status: "enable"
                stream_based_uncompressed_limit: "49"
                streaming_content_bypass: "enable"
                strip_x_forwarded_for: "disable"
                switching_protocols: "bypass"
                tcp_window_maximum: "53"
                tcp_window_minimum: "54"
                tcp_window_size: "55"
                tcp_window_type: "system"
                tunnel_non_http: "enable"
                uncompressed_nest_limit: "58"
                uncompressed_oversize_limit: "59"
                unknown_http_version: "reject"
            imap:
                inspect_all: "enable"
                options: "fragmail"
                oversize_limit: "64"
                ports: "65"
                proxy_after_tcp_handshake: "enable"
                scan_bzip2: "enable"
                ssl_offloaded: "no"
                status: "enable"
                uncompressed_nest_limit: "70"
                uncompressed_oversize_limit: "71"
            mail_signature:
                signature: "<your_own_value>"
                status: "disable"
            mapi:
                options: "fragmail"
                oversize_limit: "77"
                ports: "78"
                scan_bzip2: "enable"
                status: "enable"
                uncompressed_nest_limit: "81"
                uncompressed_oversize_limit: "82"
            name: "default_name_83"
            nntp:
                inspect_all: "enable"
                options: "oversize"
                oversize_limit: "87"
                ports: "88"
                proxy_after_tcp_handshake: "enable"
                scan_bzip2: "enable"
                status: "enable"
                uncompressed_nest_limit: "92"
                uncompressed_oversize_limit: "93"
            oversize_log: "disable"
            pop3:
                inspect_all: "enable"
                options: "fragmail"
                oversize_limit: "98"
                ports: "99"
                proxy_after_tcp_handshake: "enable"
                scan_bzip2: "enable"
                ssl_offloaded: "no"
                status: "enable"
                uncompressed_nest_limit: "104"
                uncompressed_oversize_limit: "105"
            replacemsg_group: "<your_own_value> (source system.replacemsg-group.name)"
            rpc_over_http: "enable"
            smtp:
                inspect_all: "enable"
                options: "fragmail"
                oversize_limit: "111"
                ports: "112"
                proxy_after_tcp_handshake: "enable"
                scan_bzip2: "enable"
                server_busy: "enable"
                ssl_offloaded: "no"
                status: "enable"
                uncompressed_nest_limit: "118"
                uncompressed_oversize_limit: "119"
            ssh:
                comfort_amount: "121"
                comfort_interval: "122"
                options: "oversize"
                oversize_limit: "124"
                scan_bzip2: "enable"
                uncompressed_nest_limit: "126"
                uncompressed_oversize_limit: "127"
            switching_protocols_log: "disable"
    


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
