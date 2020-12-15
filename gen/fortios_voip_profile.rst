:source: fortios_voip_profile.py

:orphan:

.. fortios_voip_profile:

fortios_voip_profile -- Configure VoIP profiles in Fortinet's FortiOS and FortiGate.
++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++

.. versionadded:: 2.8

.. contents::
   :local:
   :depth: 1


Synopsis
--------
- This module is able to configure a FortiGate or FortiOS (FOS) device by allowing the user to set and modify voip feature and profile category. Examples include all parameters and values need to be adjusted to datasources before usage. Tested with FOS v6.0.0



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
    <li> <span class="li-head">voip_profile</span> - Configure VoIP profiles. <span class="li-normal">type: dict</span></li>
        <ul class="ul-self">
        <li> <span class="li-head">state</span> - B(Deprecated) <span class="li-normal">type: str</span> <span class="li-required">required: False</span> <span class="li-normal">choices: present, absent</span></li>
        <li> <span class="li-head">comment</span> - Comment. <span class="li-normal">type: str</span></li>
        <li> <span class="li-head">name</span> - Profile name. <span class="li-normal">type: str</span> <span class="li-required">required: True</span></li>
        <li> <span class="li-head">sccp</span> - SCCP. <span class="li-normal">type: dict</span></li>
            <ul class="ul-self">
            <li> <span class="li-head">block_mcast</span> - Enable/disable block multicast RTP connections. <span class="li-normal">type: str</span> <span class="li-normal">choices: disable, enable</span></li>
            <li> <span class="li-head">log_call_summary</span> - Enable/disable log summary of SCCP calls. <span class="li-normal">type: str</span> <span class="li-normal">choices: disable, enable</span></li>
            <li> <span class="li-head">log_violations</span> - Enable/disable logging of SCCP violations. <span class="li-normal">type: str</span> <span class="li-normal">choices: disable, enable</span></li>
            <li> <span class="li-head">max_calls</span> - Maximum calls per minute per SCCP client (max 65535). <span class="li-normal">type: int</span></li>
            <li> <span class="li-head">status</span> - Enable/disable SCCP. <span class="li-normal">type: str</span> <span class="li-normal">choices: disable, enable</span></li>
            <li> <span class="li-head">verify_header</span> - Enable/disable verify SCCP header content. <span class="li-normal">type: str</span> <span class="li-normal">choices: disable, enable</span></li>
            </ul>
        <li> <span class="li-head">sip</span> - SIP. <span class="li-normal">type: dict</span></li>
            <ul class="ul-self">
            <li> <span class="li-head">ack_rate</span> - ACK request rate limit (per second, per policy). <span class="li-normal">type: int</span></li>
            <li> <span class="li-head">block_ack</span> - Enable/disable block ACK requests. <span class="li-normal">type: str</span> <span class="li-normal">choices: disable, enable</span></li>
            <li> <span class="li-head">block_bye</span> - Enable/disable block BYE requests. <span class="li-normal">type: str</span> <span class="li-normal">choices: disable, enable</span></li>
            <li> <span class="li-head">block_cancel</span> - Enable/disable block CANCEL requests. <span class="li-normal">type: str</span> <span class="li-normal">choices: disable, enable</span></li>
            <li> <span class="li-head">block_geo_red_options</span> - Enable/disable block OPTIONS requests, but OPTIONS requests still notify for redundancy. <span class="li-normal">type: str</span> <span class="li-normal">choices: disable, enable</span></li>
            <li> <span class="li-head">block_info</span> - Enable/disable block INFO requests. <span class="li-normal">type: str</span> <span class="li-normal">choices: disable, enable</span></li>
            <li> <span class="li-head">block_invite</span> - Enable/disable block INVITE requests. <span class="li-normal">type: str</span> <span class="li-normal">choices: disable, enable</span></li>
            <li> <span class="li-head">block_long_lines</span> - Enable/disable block requests with headers exceeding max-line-length. <span class="li-normal">type: str</span> <span class="li-normal">choices: disable, enable</span></li>
            <li> <span class="li-head">block_message</span> - Enable/disable block MESSAGE requests. <span class="li-normal">type: str</span> <span class="li-normal">choices: disable, enable</span></li>
            <li> <span class="li-head">block_notify</span> - Enable/disable block NOTIFY requests. <span class="li-normal">type: str</span> <span class="li-normal">choices: disable, enable</span></li>
            <li> <span class="li-head">block_options</span> - Enable/disable block OPTIONS requests and no OPTIONS as notifying message for redundancy either. <span class="li-normal">type: str</span> <span class="li-normal">choices: disable, enable</span></li>
            <li> <span class="li-head">block_prack</span> - Enable/disable block prack requests. <span class="li-normal">type: str</span> <span class="li-normal">choices: disable, enable</span></li>
            <li> <span class="li-head">block_publish</span> - Enable/disable block PUBLISH requests. <span class="li-normal">type: str</span> <span class="li-normal">choices: disable, enable</span></li>
            <li> <span class="li-head">block_refer</span> - Enable/disable block REFER requests. <span class="li-normal">type: str</span> <span class="li-normal">choices: disable, enable</span></li>
            <li> <span class="li-head">block_register</span> - Enable/disable block REGISTER requests. <span class="li-normal">type: str</span> <span class="li-normal">choices: disable, enable</span></li>
            <li> <span class="li-head">block_subscribe</span> - Enable/disable block SUBSCRIBE requests. <span class="li-normal">type: str</span> <span class="li-normal">choices: disable, enable</span></li>
            <li> <span class="li-head">block_unknown</span> - Block unrecognized SIP requests (enabled by default). <span class="li-normal">type: str</span> <span class="li-normal">choices: disable, enable</span></li>
            <li> <span class="li-head">block_update</span> - Enable/disable block UPDATE requests. <span class="li-normal">type: str</span> <span class="li-normal">choices: disable, enable</span></li>
            <li> <span class="li-head">bye_rate</span> - BYE request rate limit (per second, per policy). <span class="li-normal">type: int</span></li>
            <li> <span class="li-head">call_keepalive</span> - Continue tracking calls with no RTP for this many minutes. <span class="li-normal">type: int</span></li>
            <li> <span class="li-head">cancel_rate</span> - CANCEL request rate limit (per second, per policy). <span class="li-normal">type: int</span></li>
            <li> <span class="li-head">contact_fixup</span> - Fixup contact anyway even if contact"s IP:port doesn"t match session"s IP:port. <span class="li-normal">type: str</span> <span class="li-normal">choices: disable, enable</span></li>
            <li> <span class="li-head">hnt_restrict_source_ip</span> - Enable/disable restrict RTP source IP to be the same as SIP source IP when HNT is enabled. <span class="li-normal">type: str</span> <span class="li-normal">choices: disable, enable</span></li>
            <li> <span class="li-head">hosted_nat_traversal</span> - Hosted NAT Traversal (HNT). <span class="li-normal">type: str</span> <span class="li-normal">choices: disable, enable</span></li>
            <li> <span class="li-head">info_rate</span> - INFO request rate limit (per second, per policy). <span class="li-normal">type: int</span></li>
            <li> <span class="li-head">invite_rate</span> - INVITE request rate limit (per second, per policy). <span class="li-normal">type: int</span></li>
            <li> <span class="li-head">ips_rtp</span> - Enable/disable allow IPS on RTP. <span class="li-normal">type: str</span> <span class="li-normal">choices: disable, enable</span></li>
            <li> <span class="li-head">log_call_summary</span> - Enable/disable logging of SIP call summary. <span class="li-normal">type: str</span> <span class="li-normal">choices: disable, enable</span></li>
            <li> <span class="li-head">log_violations</span> - Enable/disable logging of SIP violations. <span class="li-normal">type: str</span> <span class="li-normal">choices: disable, enable</span></li>
            <li> <span class="li-head">malformed_header_allow</span> - Action for malformed Allow header. <span class="li-normal">type: str</span> <span class="li-normal">choices: discard, pass, respond</span></li>
            <li> <span class="li-head">malformed_header_call_id</span> - Action for malformed Call-ID header. <span class="li-normal">type: str</span> <span class="li-normal">choices: discard, pass, respond</span></li>
            <li> <span class="li-head">malformed_header_contact</span> - Action for malformed Contact header. <span class="li-normal">type: str</span> <span class="li-normal">choices: discard, pass, respond</span></li>
            <li> <span class="li-head">malformed_header_content_length</span> - Action for malformed Content-Length header. <span class="li-normal">type: str</span> <span class="li-normal">choices: discard, pass, respond</span></li>
            <li> <span class="li-head">malformed_header_content_type</span> - Action for malformed Content-Type header. <span class="li-normal">type: str</span> <span class="li-normal">choices: discard, pass, respond</span></li>
            <li> <span class="li-head">malformed_header_cseq</span> - Action for malformed CSeq header. <span class="li-normal">type: str</span> <span class="li-normal">choices: discard, pass, respond</span></li>
            <li> <span class="li-head">malformed_header_expires</span> - Action for malformed Expires header. <span class="li-normal">type: str</span> <span class="li-normal">choices: discard, pass, respond</span></li>
            <li> <span class="li-head">malformed_header_from</span> - Action for malformed From header. <span class="li-normal">type: str</span> <span class="li-normal">choices: discard, pass, respond</span></li>
            <li> <span class="li-head">malformed_header_max_forwards</span> - Action for malformed Max-Forwards header. <span class="li-normal">type: str</span> <span class="li-normal">choices: discard, pass, respond</span></li>
            <li> <span class="li-head">malformed_header_p_asserted_identity</span> - Action for malformed P-Asserted-Identity header. <span class="li-normal">type: str</span> <span class="li-normal">choices: discard, pass, respond</span></li>
            <li> <span class="li-head">malformed_header_rack</span> - Action for malformed RAck header. <span class="li-normal">type: str</span> <span class="li-normal">choices: discard, pass, respond</span></li>
            <li> <span class="li-head">malformed_header_record_route</span> - Action for malformed Record-Route header. <span class="li-normal">type: str</span> <span class="li-normal">choices: discard, pass, respond</span></li>
            <li> <span class="li-head">malformed_header_route</span> - Action for malformed Route header. <span class="li-normal">type: str</span> <span class="li-normal">choices: discard, pass, respond</span></li>
            <li> <span class="li-head">malformed_header_rseq</span> - Action for malformed RSeq header. <span class="li-normal">type: str</span> <span class="li-normal">choices: discard, pass, respond</span></li>
            <li> <span class="li-head">malformed_header_sdp_a</span> - Action for malformed SDP a line. <span class="li-normal">type: str</span> <span class="li-normal">choices: discard, pass, respond</span></li>
            <li> <span class="li-head">malformed_header_sdp_b</span> - Action for malformed SDP b line. <span class="li-normal">type: str</span> <span class="li-normal">choices: discard, pass, respond</span></li>
            <li> <span class="li-head">malformed_header_sdp_c</span> - Action for malformed SDP c line. <span class="li-normal">type: str</span> <span class="li-normal">choices: discard, pass, respond</span></li>
            <li> <span class="li-head">malformed_header_sdp_i</span> - Action for malformed SDP i line. <span class="li-normal">type: str</span> <span class="li-normal">choices: discard, pass, respond</span></li>
            <li> <span class="li-head">malformed_header_sdp_k</span> - Action for malformed SDP k line. <span class="li-normal">type: str</span> <span class="li-normal">choices: discard, pass, respond</span></li>
            <li> <span class="li-head">malformed_header_sdp_m</span> - Action for malformed SDP m line. <span class="li-normal">type: str</span> <span class="li-normal">choices: discard, pass, respond</span></li>
            <li> <span class="li-head">malformed_header_sdp_o</span> - Action for malformed SDP o line. <span class="li-normal">type: str</span> <span class="li-normal">choices: discard, pass, respond</span></li>
            <li> <span class="li-head">malformed_header_sdp_r</span> - Action for malformed SDP r line. <span class="li-normal">type: str</span> <span class="li-normal">choices: discard, pass, respond</span></li>
            <li> <span class="li-head">malformed_header_sdp_s</span> - Action for malformed SDP s line. <span class="li-normal">type: str</span> <span class="li-normal">choices: discard, pass, respond</span></li>
            <li> <span class="li-head">malformed_header_sdp_t</span> - Action for malformed SDP t line. <span class="li-normal">type: str</span> <span class="li-normal">choices: discard, pass, respond</span></li>
            <li> <span class="li-head">malformed_header_sdp_v</span> - Action for malformed SDP v line. <span class="li-normal">type: str</span> <span class="li-normal">choices: discard, pass, respond</span></li>
            <li> <span class="li-head">malformed_header_sdp_z</span> - Action for malformed SDP z line. <span class="li-normal">type: str</span> <span class="li-normal">choices: discard, pass, respond</span></li>
            <li> <span class="li-head">malformed_header_to</span> - Action for malformed To header. <span class="li-normal">type: str</span> <span class="li-normal">choices: discard, pass, respond</span></li>
            <li> <span class="li-head">malformed_header_via</span> - Action for malformed VIA header. <span class="li-normal">type: str</span> <span class="li-normal">choices: discard, pass, respond</span></li>
            <li> <span class="li-head">malformed_request_line</span> - Action for malformed request line. <span class="li-normal">type: str</span> <span class="li-normal">choices: discard, pass, respond</span></li>
            <li> <span class="li-head">max_body_length</span> - Maximum SIP message body length (0 meaning no limit). <span class="li-normal">type: int</span></li>
            <li> <span class="li-head">max_dialogs</span> - Maximum number of concurrent calls/dialogs (per policy). <span class="li-normal">type: int</span></li>
            <li> <span class="li-head">max_idle_dialogs</span> - Maximum number established but idle dialogs to retain (per policy). <span class="li-normal">type: int</span></li>
            <li> <span class="li-head">max_line_length</span> - Maximum SIP header line length (78-4096). <span class="li-normal">type: int</span></li>
            <li> <span class="li-head">message_rate</span> - MESSAGE request rate limit (per second, per policy). <span class="li-normal">type: int</span></li>
            <li> <span class="li-head">nat_trace</span> - Enable/disable preservation of original IP in SDP i line. <span class="li-normal">type: str</span> <span class="li-normal">choices: disable, enable</span></li>
            <li> <span class="li-head">no_sdp_fixup</span> - Enable/disable no SDP fix-up. <span class="li-normal">type: str</span> <span class="li-normal">choices: disable, enable</span></li>
            <li> <span class="li-head">notify_rate</span> - NOTIFY request rate limit (per second, per policy). <span class="li-normal">type: int</span></li>
            <li> <span class="li-head">open_contact_pinhole</span> - Enable/disable open pinhole for non-REGISTER Contact port. <span class="li-normal">type: str</span> <span class="li-normal">choices: disable, enable</span></li>
            <li> <span class="li-head">open_record_route_pinhole</span> - Enable/disable open pinhole for Record-Route port. <span class="li-normal">type: str</span> <span class="li-normal">choices: disable, enable</span></li>
            <li> <span class="li-head">open_register_pinhole</span> - Enable/disable open pinhole for REGISTER Contact port. <span class="li-normal">type: str</span> <span class="li-normal">choices: disable, enable</span></li>
            <li> <span class="li-head">open_via_pinhole</span> - Enable/disable open pinhole for Via port. <span class="li-normal">type: str</span> <span class="li-normal">choices: disable, enable</span></li>
            <li> <span class="li-head">options_rate</span> - OPTIONS request rate limit (per second, per policy). <span class="li-normal">type: int</span></li>
            <li> <span class="li-head">prack_rate</span> - PRACK request rate limit (per second, per policy). <span class="li-normal">type: int</span></li>
            <li> <span class="li-head">preserve_override</span> - Override i line to preserve original IPS . <span class="li-normal">type: str</span> <span class="li-normal">choices: disable, enable</span></li>
            <li> <span class="li-head">provisional_invite_expiry_time</span> - Expiry time for provisional INVITE (10 - 3600 sec). <span class="li-normal">type: int</span></li>
            <li> <span class="li-head">publish_rate</span> - PUBLISH request rate limit (per second, per policy). <span class="li-normal">type: int</span></li>
            <li> <span class="li-head">refer_rate</span> - REFER request rate limit (per second, per policy). <span class="li-normal">type: int</span></li>
            <li> <span class="li-head">register_contact_trace</span> - Enable/disable trace original IP/port within the contact header of REGISTER requests. <span class="li-normal">type: str</span> <span class="li-normal">choices: disable, enable</span></li>
            <li> <span class="li-head">register_rate</span> - REGISTER request rate limit (per second, per policy). <span class="li-normal">type: int</span></li>
            <li> <span class="li-head">rfc2543_branch</span> - Enable/disable support via branch compliant with RFC 2543. <span class="li-normal">type: str</span> <span class="li-normal">choices: disable, enable</span></li>
            <li> <span class="li-head">rtp</span> - Enable/disable create pinholes for RTP traffic to traverse firewall. <span class="li-normal">type: str</span> <span class="li-normal">choices: disable, enable</span></li>
            <li> <span class="li-head">ssl_algorithm</span> - Relative strength of encryption algorithms accepted in negotiation. <span class="li-normal">type: str</span> <span class="li-normal">choices: high, medium, low</span></li>
            <li> <span class="li-head">ssl_auth_client</span> - Require a client certificate and authenticate it with the peer/peergrp. Source user.peer.name user.peergrp.name. <span class="li-normal">type: str</span></li>
            <li> <span class="li-head">ssl_auth_server</span> - Authenticate the server"s certificate with the peer/peergrp. Source user.peer.name user.peergrp.name. <span class="li-normal">type: str</span></li>
            <li> <span class="li-head">ssl_client_certificate</span> - Name of Certificate to offer to server if requested. Source vpn.certificate.local.name. <span class="li-normal">type: str</span></li>
            <li> <span class="li-head">ssl_client_renegotiation</span> - Allow/block client renegotiation by server. <span class="li-normal">type: str</span> <span class="li-normal">choices: allow, deny, secure</span></li>
            <li> <span class="li-head">ssl_max_version</span> - Highest SSL/TLS version to negotiate. <span class="li-normal">type: str</span> <span class="li-normal">choices: ssl-3.0, tls-1.0, tls-1.1, tls-1.2</span></li>
            <li> <span class="li-head">ssl_min_version</span> - Lowest SSL/TLS version to negotiate. <span class="li-normal">type: str</span> <span class="li-normal">choices: ssl-3.0, tls-1.0, tls-1.1, tls-1.2</span></li>
            <li> <span class="li-head">ssl_mode</span> - SSL/TLS mode for encryption & decryption of traffic. <span class="li-normal">type: str</span> <span class="li-normal">choices: False, full</span></li>
            <li> <span class="li-head">ssl_pfs</span> - SSL Perfect Forward Secrecy. <span class="li-normal">type: str</span> <span class="li-normal">choices: require, deny, allow</span></li>
            <li> <span class="li-head">ssl_send_empty_frags</span> - Send empty fragments to avoid attack on CBC IV (SSL 3.0 & TLS 1.0 only). <span class="li-normal">type: str</span> <span class="li-normal">choices: enable, disable</span></li>
            <li> <span class="li-head">ssl_server_certificate</span> - Name of Certificate return to the client in every SSL connection. Source vpn.certificate.local.name. <span class="li-normal">type: str</span></li>
            <li> <span class="li-head">status</span> - Enable/disable SIP. <span class="li-normal">type: str</span> <span class="li-normal">choices: disable, enable</span></li>
            <li> <span class="li-head">strict_register</span> - Enable/disable only allow the registrar to connect. <span class="li-normal">type: str</span> <span class="li-normal">choices: disable, enable</span></li>
            <li> <span class="li-head">subscribe_rate</span> - SUBSCRIBE request rate limit (per second, per policy). <span class="li-normal">type: int</span></li>
            <li> <span class="li-head">unknown_header</span> - Action for unknown SIP header. <span class="li-normal">type: str</span> <span class="li-normal">choices: discard, pass, respond</span></li>
            <li> <span class="li-head">update_rate</span> - UPDATE request rate limit (per second, per policy). <span class="li-normal">type: int</span></li>
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
      - name: Configure VoIP profiles.
        fortios_voip_profile:
          vdom:  "{{ vdom }}"
          state: "present"
          access_token: "<your_own_value>"
          voip_profile:
            comment: "Comment."
            name: "default_name_4"
            sccp:
                block_mcast: "disable"
                log_call_summary: "disable"
                log_violations: "disable"
                max_calls: "9"
                status: "disable"
                verify_header: "disable"
            sip:
                ack_rate: "13"
                block_ack: "disable"
                block_bye: "disable"
                block_cancel: "disable"
                block_geo_red_options: "disable"
                block_info: "disable"
                block_invite: "disable"
                block_long_lines: "disable"
                block_message: "disable"
                block_notify: "disable"
                block_options: "disable"
                block_prack: "disable"
                block_publish: "disable"
                block_refer: "disable"
                block_register: "disable"
                block_subscribe: "disable"
                block_unknown: "disable"
                block_update: "disable"
                bye_rate: "31"
                call_keepalive: "32"
                cancel_rate: "33"
                contact_fixup: "disable"
                hnt_restrict_source_ip: "disable"
                hosted_nat_traversal: "disable"
                info_rate: "37"
                invite_rate: "38"
                ips_rtp: "disable"
                log_call_summary: "disable"
                log_violations: "disable"
                malformed_header_allow: "discard"
                malformed_header_call_id: "discard"
                malformed_header_contact: "discard"
                malformed_header_content_length: "discard"
                malformed_header_content_type: "discard"
                malformed_header_cseq: "discard"
                malformed_header_expires: "discard"
                malformed_header_from: "discard"
                malformed_header_max_forwards: "discard"
                malformed_header_p_asserted_identity: "discard"
                malformed_header_rack: "discard"
                malformed_header_record_route: "discard"
                malformed_header_route: "discard"
                malformed_header_rseq: "discard"
                malformed_header_sdp_a: "discard"
                malformed_header_sdp_b: "discard"
                malformed_header_sdp_c: "discard"
                malformed_header_sdp_i: "discard"
                malformed_header_sdp_k: "discard"
                malformed_header_sdp_m: "discard"
                malformed_header_sdp_o: "discard"
                malformed_header_sdp_r: "discard"
                malformed_header_sdp_s: "discard"
                malformed_header_sdp_t: "discard"
                malformed_header_sdp_v: "discard"
                malformed_header_sdp_z: "discard"
                malformed_header_to: "discard"
                malformed_header_via: "discard"
                malformed_request_line: "discard"
                max_body_length: "71"
                max_dialogs: "72"
                max_idle_dialogs: "73"
                max_line_length: "74"
                message_rate: "75"
                nat_trace: "disable"
                no_sdp_fixup: "disable"
                notify_rate: "78"
                open_contact_pinhole: "disable"
                open_record_route_pinhole: "disable"
                open_register_pinhole: "disable"
                open_via_pinhole: "disable"
                options_rate: "83"
                prack_rate: "84"
                preserve_override: "disable"
                provisional_invite_expiry_time: "86"
                publish_rate: "87"
                refer_rate: "88"
                register_contact_trace: "disable"
                register_rate: "90"
                rfc2543_branch: "disable"
                rtp: "disable"
                ssl_algorithm: "high"
                ssl_auth_client: "<your_own_value> (source user.peer.name user.peergrp.name)"
                ssl_auth_server: "<your_own_value> (source user.peer.name user.peergrp.name)"
                ssl_client_certificate: "<your_own_value> (source vpn.certificate.local.name)"
                ssl_client_renegotiation: "allow"
                ssl_max_version: "ssl-3.0"
                ssl_min_version: "ssl-3.0"
                ssl_mode: "off"
                ssl_pfs: "require"
                ssl_send_empty_frags: "enable"
                ssl_server_certificate: "<your_own_value> (source vpn.certificate.local.name)"
                status: "disable"
                strict_register: "disable"
                subscribe_rate: "106"
                unknown_header: "discard"
                update_rate: "108"
    


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
