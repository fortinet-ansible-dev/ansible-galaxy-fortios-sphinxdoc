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
- This module is able to configure a FortiGate or FortiOS (FOS) device by allowing the user to set and modify firewall feature and profile_protocol_options category. Examples include all parameters and values need to be adjusted to datasources before usage. Tested with FOS v6.0.5



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
    <li> <span class="li-head">firewall_profile_protocol_options</span> - Configure protocol options. <span class="li-normal">type: dict</span></li>
        <ul class="ul-self">
        <li> <span class="li-head">state</span> - B(Deprecated) <span class="li-normal">type: str</span> <span class="li-required">required: False</span> <span class="li-normal">choices: present, absent</span></li>
        <li> <span class="li-head">comment</span> - Optional comments. <span class="li-normal">type: str</span></li>
        <li> <span class="li-head">dns</span> - Configure DNS protocol options. <span class="li-normal">type: dict</span></li>
            <ul class="ul-self">
            <li> <span class="li-head">ports</span> - Ports to scan for content (1 - 65535). <span class="li-normal">type: int</span></li>
            <li> <span class="li-head">status</span> - Enable/disable the active status of scanning for this protocol. <span class="li-normal">type: str</span> <span class="li-normal">choices: enable, disable</span></li>
            </ul>
        <li> <span class="li-head">ftp</span> - Configure FTP protocol options. <span class="li-normal">type: dict</span></li>
            <ul class="ul-self">
            <li> <span class="li-head">comfort_amount</span> - Amount of data to send in a transmission for client comforting (1 - 10240 bytes). <span class="li-normal">type: int</span></li>
            <li> <span class="li-head">comfort_interval</span> - Period of time between start, or last transmission, and the next client comfort transmission of data (1 - 900 sec). <span class="li-normal">type: int</span></li>
            <li> <span class="li-head">inspect_all</span> - Enable/disable the inspection of all ports for the protocol. <span class="li-normal">type: str</span> <span class="li-normal">choices: enable, disable</span></li>
            <li> <span class="li-head">options</span> - One or more options that can be applied to the session. <span class="li-normal">type: str</span> <span class="li-normal">choices: clientcomfort, oversize, splice, bypass-rest-command, bypass-mode-command</span></li>
            <li> <span class="li-head">oversize_limit</span> - Maximum in-memory file size that can be scanned (1 - 383 MB). <span class="li-normal">type: int</span></li>
            <li> <span class="li-head">ports</span> - Ports to scan for content (1 - 65535). <span class="li-normal">type: int</span></li>
            <li> <span class="li-head">scan_bzip2</span> - Enable/disable scanning of BZip2 compressed files. <span class="li-normal">type: str</span> <span class="li-normal">choices: enable, disable</span></li>
            <li> <span class="li-head">status</span> - Enable/disable the active status of scanning for this protocol. <span class="li-normal">type: str</span> <span class="li-normal">choices: enable, disable</span></li>
            <li> <span class="li-head">uncompressed_nest_limit</span> - Maximum nested levels of compression that can be uncompressed and scanned (2 - 100). <span class="li-normal">type: int</span></li>
            <li> <span class="li-head">uncompressed_oversize_limit</span> - Maximum in-memory uncompressed file size that can be scanned (0 - 383 MB, 0 = unlimited). <span class="li-normal">type: int</span></li>
            </ul>
        <li> <span class="li-head">http</span> - Configure HTTP protocol options. <span class="li-normal">type: dict</span></li>
            <ul class="ul-self">
            <li> <span class="li-head">block_page_status_code</span> - Code number returned for blocked HTTP pages (non-FortiGuard only) (100 - 599). <span class="li-normal">type: int</span></li>
            <li> <span class="li-head">comfort_amount</span> - Amount of data to send in a transmission for client comforting (1 - 10240 bytes). <span class="li-normal">type: int</span></li>
            <li> <span class="li-head">comfort_interval</span> - Period of time between start, or last transmission, and the next client comfort transmission of data (1 - 900 sec). <span class="li-normal">type: int</span></li>
            <li> <span class="li-head">fortinet_bar</span> - Enable/disable Fortinet bar on HTML content. <span class="li-normal">type: str</span> <span class="li-normal">choices: enable, disable</span></li>
            <li> <span class="li-head">fortinet_bar_port</span> - Port for use by Fortinet Bar (1 - 65535). <span class="li-normal">type: int</span></li>
            <li> <span class="li-head">http_policy</span> - Enable/disable HTTP policy check. <span class="li-normal">type: str</span> <span class="li-normal">choices: disable, enable</span></li>
            <li> <span class="li-head">inspect_all</span> - Enable/disable the inspection of all ports for the protocol. <span class="li-normal">type: str</span> <span class="li-normal">choices: enable, disable</span></li>
            <li> <span class="li-head">options</span> - One or more options that can be applied to the session. <span class="li-normal">type: str</span> <span class="li-normal">choices: clientcomfort, servercomfort, oversize, chunkedbypass</span></li>
            <li> <span class="li-head">oversize_limit</span> - Maximum in-memory file size that can be scanned (1 - 383 MB). <span class="li-normal">type: int</span></li>
            <li> <span class="li-head">ports</span> - Ports to scan for content (1 - 65535). <span class="li-normal">type: int</span></li>
            <li> <span class="li-head">post_lang</span> - ID codes for character sets to be used to convert to UTF-8 for banned words and DLP on HTTP posts (maximum of 5 character sets). <span class="li-normal">type: str</span> <span class="li-normal">choices: jisx0201, jisx0208, jisx0212, gb2312, ksc5601-ex, euc-jp, sjis, iso2022-jp, iso2022-jp-1, iso2022-jp-2, euc-cn, ces-gbk, hz, ces-big5, euc-kr, iso2022-jp-3, iso8859-1, tis620, cp874, cp1252, cp1251</span></li>
            <li> <span class="li-head">range_block</span> - Enable/disable blocking of partial downloads. <span class="li-normal">type: str</span> <span class="li-normal">choices: disable, enable</span></li>
            <li> <span class="li-head">retry_count</span> - Number of attempts to retry HTTP connection (0 - 100). <span class="li-normal">type: int</span></li>
            <li> <span class="li-head">scan_bzip2</span> - Enable/disable scanning of BZip2 compressed files. <span class="li-normal">type: str</span> <span class="li-normal">choices: enable, disable</span></li>
            <li> <span class="li-head">status</span> - Enable/disable the active status of scanning for this protocol. <span class="li-normal">type: str</span> <span class="li-normal">choices: enable, disable</span></li>
            <li> <span class="li-head">streaming_content_bypass</span> - Enable/disable bypassing of streaming content from buffering. <span class="li-normal">type: str</span> <span class="li-normal">choices: enable, disable</span></li>
            <li> <span class="li-head">strip_x_forwarded_for</span> - Enable/disable stripping of HTTP X-Forwarded-For header. <span class="li-normal">type: str</span> <span class="li-normal">choices: disable, enable</span></li>
            <li> <span class="li-head">switching_protocols</span> - Bypass from scanning, or block a connection that attempts to switch protocol. <span class="li-normal">type: str</span> <span class="li-normal">choices: bypass, block</span></li>
            <li> <span class="li-head">uncompressed_nest_limit</span> - Maximum nested levels of compression that can be uncompressed and scanned (2 - 100). <span class="li-normal">type: int</span></li>
            <li> <span class="li-head">uncompressed_oversize_limit</span> - Maximum in-memory uncompressed file size that can be scanned (0 - 383 MB, 0 = unlimited). <span class="li-normal">type: int</span></li>
            </ul>
        <li> <span class="li-head">imap</span> - Configure IMAP protocol options. <span class="li-normal">type: dict</span></li>
            <ul class="ul-self">
            <li> <span class="li-head">inspect_all</span> - Enable/disable the inspection of all ports for the protocol. <span class="li-normal">type: str</span> <span class="li-normal">choices: enable, disable</span></li>
            <li> <span class="li-head">options</span> - One or more options that can be applied to the session. <span class="li-normal">type: str</span> <span class="li-normal">choices: fragmail, oversize</span></li>
            <li> <span class="li-head">oversize_limit</span> - Maximum in-memory file size that can be scanned (1 - 383 MB). <span class="li-normal">type: int</span></li>
            <li> <span class="li-head">ports</span> - Ports to scan for content (1 - 65535). <span class="li-normal">type: int</span></li>
            <li> <span class="li-head">scan_bzip2</span> - Enable/disable scanning of BZip2 compressed files. <span class="li-normal">type: str</span> <span class="li-normal">choices: enable, disable</span></li>
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
            <li> <span class="li-head">scan_bzip2</span> - Enable/disable scanning of BZip2 compressed files. <span class="li-normal">type: str</span> <span class="li-normal">choices: enable, disable</span></li>
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
            <li> <span class="li-head">scan_bzip2</span> - Enable/disable scanning of BZip2 compressed files. <span class="li-normal">type: str</span> <span class="li-normal">choices: enable, disable</span></li>
            <li> <span class="li-head">server_busy</span> - Enable/disable SMTP server busy when server not available. <span class="li-normal">type: str</span> <span class="li-normal">choices: enable, disable</span></li>
            <li> <span class="li-head">status</span> - Enable/disable the active status of scanning for this protocol. <span class="li-normal">type: str</span> <span class="li-normal">choices: enable, disable</span></li>
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
          firewall_profile_protocol_options:
            comment: "Optional comments."
            dns:
                ports: "5"
                status: "enable"
            ftp:
                comfort_amount: "8"
                comfort_interval: "9"
                inspect_all: "enable"
                options: "clientcomfort"
                oversize_limit: "12"
                ports: "13"
                scan_bzip2: "enable"
                status: "enable"
                uncompressed_nest_limit: "16"
                uncompressed_oversize_limit: "17"
            http:
                block_page_status_code: "19"
                comfort_amount: "20"
                comfort_interval: "21"
                fortinet_bar: "enable"
                fortinet_bar_port: "23"
                http_policy: "disable"
                inspect_all: "enable"
                options: "clientcomfort"
                oversize_limit: "27"
                ports: "28"
                post_lang: "jisx0201"
                range_block: "disable"
                retry_count: "31"
                scan_bzip2: "enable"
                status: "enable"
                streaming_content_bypass: "enable"
                strip_x_forwarded_for: "disable"
                switching_protocols: "bypass"
                uncompressed_nest_limit: "37"
                uncompressed_oversize_limit: "38"
            imap:
                inspect_all: "enable"
                options: "fragmail"
                oversize_limit: "42"
                ports: "43"
                scan_bzip2: "enable"
                status: "enable"
                uncompressed_nest_limit: "46"
                uncompressed_oversize_limit: "47"
            mail_signature:
                signature: "<your_own_value>"
                status: "disable"
            mapi:
                options: "fragmail"
                oversize_limit: "53"
                ports: "54"
                scan_bzip2: "enable"
                status: "enable"
                uncompressed_nest_limit: "57"
                uncompressed_oversize_limit: "58"
            name: "default_name_59"
            nntp:
                inspect_all: "enable"
                options: "oversize"
                oversize_limit: "63"
                ports: "64"
                scan_bzip2: "enable"
                status: "enable"
                uncompressed_nest_limit: "67"
                uncompressed_oversize_limit: "68"
            oversize_log: "disable"
            pop3:
                inspect_all: "enable"
                options: "fragmail"
                oversize_limit: "73"
                ports: "74"
                scan_bzip2: "enable"
                status: "enable"
                uncompressed_nest_limit: "77"
                uncompressed_oversize_limit: "78"
            replacemsg_group: "<your_own_value> (source system.replacemsg-group.name)"
            rpc_over_http: "enable"
            smtp:
                inspect_all: "enable"
                options: "fragmail"
                oversize_limit: "84"
                ports: "85"
                scan_bzip2: "enable"
                server_busy: "enable"
                status: "enable"
                uncompressed_nest_limit: "89"
                uncompressed_oversize_limit: "90"
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
- Hongbin Lu (@fgtdev-hblu)
- Frank Shen (@frankshen01)
- Jie Xue (@JieX19)
- Miguel Angel Munoz (@mamunozgonzalez)
- Nicolas Thomas (@thomnico)


.. hint::
    If you notice any issues in this documentation, you can create a pull request to improve it.
