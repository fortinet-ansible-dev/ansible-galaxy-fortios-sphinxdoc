:source: fortios_system_npu.py

:orphan:

.. fortios_system_npu:

fortios_system_npu -- Configure NPU attributes in Fortinet's FortiOS and FortiGate.
+++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++

.. versionadded:: 2.10

.. contents::
   :local:
   :depth: 1


Synopsis
--------
- This module is able to configure a FortiGate or FortiOS (FOS) device by allowing the user to set and modify system feature and npu category. Examples include all parameters and values need to be adjusted to datasources before usage. Tested with FOS v6.4.0



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
    <li> <span class="li-head">system_npu</span> - Configure NPU attributes. <span class="li-normal">type: dict</span></li>
        <ul class="ul-self">
        <li> <span class="li-head">fp_anomaly</span> - NP6Lite anomaly protection (packet drop or send trap to host). <span class="li-normal">type: dict</span></li>
            <ul class="ul-self">
            <li> <span class="li-head">esp_minlen_err</span> - Invalid IPv4 ESP short packet anomalies. <span class="li-normal">type: str</span> <span class="li-normal">choices: drop, trap-to-host</span></li>
            <li> <span class="li-head">icmp_csum_err</span> - Invalid IPv4 ICMP packet checksum anomalies. <span class="li-normal">type: str</span> <span class="li-normal">choices: drop, trap-to-host</span></li>
            <li> <span class="li-head">icmp_minlen_err</span> - Invalid IPv4 ICMP short packet anomalies. <span class="li-normal">type: str</span> <span class="li-normal">choices: drop, trap-to-host</span></li>
            <li> <span class="li-head">ipv4_csum_err</span> - Invalid IPv4 packet checksum anomalies. <span class="li-normal">type: str</span> <span class="li-normal">choices: drop, trap-to-host</span></li>
            <li> <span class="li-head">ipv4_ihl_err</span> - Invalid IPv4 header length anomalies. <span class="li-normal">type: str</span> <span class="li-normal">choices: drop, trap-to-host</span></li>
            <li> <span class="li-head">ipv4_len_err</span> - Invalid IPv4 packet length anomalies. <span class="li-normal">type: str</span> <span class="li-normal">choices: drop, trap-to-host</span></li>
            <li> <span class="li-head">ipv4_opt_err</span> - Invalid IPv4 option parsing anomalies. <span class="li-normal">type: str</span> <span class="li-normal">choices: drop, trap-to-host</span></li>
            <li> <span class="li-head">ipv4_ttlzero_err</span> - Invalid IPv4 TTL field zero anomalies. <span class="li-normal">type: str</span> <span class="li-normal">choices: drop, trap-to-host</span></li>
            <li> <span class="li-head">ipv4_ver_err</span> - Invalid IPv4 header version anomalies. <span class="li-normal">type: str</span> <span class="li-normal">choices: drop, trap-to-host</span></li>
            <li> <span class="li-head">ipv6_exthdr_len_err</span> - Invalid IPv6 packet chain extension header total length anomalies. <span class="li-normal">type: str</span> <span class="li-normal">choices: drop, trap-to-host</span></li>
            <li> <span class="li-head">ipv6_exthdr_order_err</span> - Invalid IPv6 packet extension header ordering anomalies. <span class="li-normal">type: str</span> <span class="li-normal">choices: drop, trap-to-host</span></li>
            <li> <span class="li-head">ipv6_ihl_err</span> - Invalid IPv6 packet length anomalies. <span class="li-normal">type: str</span> <span class="li-normal">choices: drop, trap-to-host</span></li>
            <li> <span class="li-head">ipv6_plen_zero</span> - Invalid IPv6 packet payload length zero anomalies. <span class="li-normal">type: str</span> <span class="li-normal">choices: drop, trap-to-host</span></li>
            <li> <span class="li-head">ipv6_ver_err</span> - Invalid IPv6 packet version anomalies. <span class="li-normal">type: str</span> <span class="li-normal">choices: drop, trap-to-host</span></li>
            <li> <span class="li-head">tcp_csum_err</span> - Invalid IPv4 TCP packet checksum anomalies. <span class="li-normal">type: str</span> <span class="li-normal">choices: drop, trap-to-host</span></li>
            <li> <span class="li-head">tcp_hlen_err</span> - Invalid IPv4 TCP header length anomalies. <span class="li-normal">type: str</span> <span class="li-normal">choices: drop, trap-to-host</span></li>
            <li> <span class="li-head">tcp_plen_err</span> - Invalid IPv4 TCP packet length anomalies. <span class="li-normal">type: str</span> <span class="li-normal">choices: drop, trap-to-host</span></li>
            <li> <span class="li-head">udp_csum_err</span> - Invalid IPv4 UDP packet checksum anomalies. <span class="li-normal">type: str</span> <span class="li-normal">choices: drop, trap-to-host</span></li>
            <li> <span class="li-head">udp_hlen_err</span> - Invalid IPv4 UDP packet header length anomalies. <span class="li-normal">type: str</span> <span class="li-normal">choices: drop, trap-to-host</span></li>
            <li> <span class="li-head">udp_len_err</span> - Invalid IPv4 UDP packet length anomalies. <span class="li-normal">type: str</span> <span class="li-normal">choices: drop, trap-to-host</span></li>
            <li> <span class="li-head">udp_plen_err</span> - Invalid IPv4 UDP packet minimum length anomalies. <span class="li-normal">type: str</span> <span class="li-normal">choices: drop, trap-to-host</span></li>
            <li> <span class="li-head">udplite_cover_err</span> - Invalid IPv4 UDP-Lite packet coverage anomalies. <span class="li-normal">type: str</span> <span class="li-normal">choices: drop, trap-to-host</span></li>
            <li> <span class="li-head">udplite_csum_err</span> - Invalid IPv4 UDP-Lite packet checksum anomalies. <span class="li-normal">type: str</span> <span class="li-normal">choices: drop, trap-to-host</span></li>
            <li> <span class="li-head">unknproto_minlen_err</span> - Invalid IPv4 L4 unknown protocol short packet anomalies. <span class="li-normal">type: str</span> <span class="li-normal">choices: drop, trap-to-host</span></li>
            </ul>
        <li> <span class="li-head">iph_rsvd_re_cksum</span> - Enable/disable IP checksum re-calculation for packets with iph.reserved bit set. <span class="li-normal">type: str</span> <span class="li-normal">choices: enable, disable</span></li>
        <li> <span class="li-head">per_session_accounting</span> - Enable/disable per-session accounting. <span class="li-normal">type: str</span> <span class="li-normal">choices: disable, traffic-log-only, enable</span></li>
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
      - name: Configure NPU attributes.
        fortios_system_npu:
          vdom:  "{{ vdom }}"
          system_npu:
            fp_anomaly:
                esp_minlen_err: "drop"
                icmp_csum_err: "drop"
                icmp_minlen_err: "drop"
                ipv4_csum_err: "drop"
                ipv4_ihl_err: "drop"
                ipv4_len_err: "drop"
                ipv4_opt_err: "drop"
                ipv4_ttlzero_err: "drop"
                ipv4_ver_err: "drop"
                ipv6_exthdr_len_err: "drop"
                ipv6_exthdr_order_err: "drop"
                ipv6_ihl_err: "drop"
                ipv6_plen_zero: "drop"
                ipv6_ver_err: "drop"
                tcp_csum_err: "drop"
                tcp_hlen_err: "drop"
                tcp_plen_err: "drop"
                udp_csum_err: "drop"
                udp_hlen_err: "drop"
                udp_len_err: "drop"
                udp_plen_err: "drop"
                udplite_cover_err: "drop"
                udplite_csum_err: "drop"
                unknproto_minlen_err: "drop"
            iph_rsvd_re_cksum: "enable"
            per_session_accounting: "disable"


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
