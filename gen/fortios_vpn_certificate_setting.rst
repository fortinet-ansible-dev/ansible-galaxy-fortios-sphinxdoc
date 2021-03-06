:source: fortios_vpn_certificate_setting.py

:orphan:

.. _fortios_vpn_certificate_setting:

fortios_vpn_certificate_setting -- VPN certificate setting in Fortinet's FortiOS and FortiGate.
+++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++

.. versionadded:: 2.9

.. contents::
   :local:
   :depth: 1


Synopsis
--------
- This module is able to configure a FortiGate or FortiOS (FOS) device by allowing the user to set and modify vpn_certificate feature and setting category. Examples include all parameters and values need to be adjusted to datasources before usage. Tested with FOS v6.0.5


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
    <li><span class="li-head">vpn_certificate_setting</span> - VPN certificate setting. <span class="li-normal">default: null</span> <span class="li-normal">type: dict</span></li>
            <ul class="ul-self">

            <li><span class="li-head">certname_dsa1024</span> - 1024 bit DSA key certificate for re-signing server certificates for SSL inspection. Source vpn.certificate.local.name. <span class="li-normal">type: str</span></li>
            <li><span class="li-head">certname_dsa2048</span> - 2048 bit DSA key certificate for re-signing server certificates for SSL inspection. Source vpn.certificate.local.name. <span class="li-normal">type: str</span></li>
            <li><span class="li-head">certname_ecdsa256</span> - 256 bit ECDSA key certificate for re-signing server certificates for SSL inspection. Source vpn.certificate.local.name. <span class="li-normal">type: str</span></li>
            <li><span class="li-head">certname_ecdsa384</span> - 384 bit ECDSA key certificate for re-signing server certificates for SSL inspection. Source vpn.certificate.local.name. <span class="li-normal">type: str</span></li>
            <li><span class="li-head">certname_rsa1024</span> - 1024 bit RSA key certificate for re-signing server certificates for SSL inspection. Source vpn.certificate.local.name. <span class="li-normal">type: str</span></li>
            <li><span class="li-head">certname_rsa2048</span> - 2048 bit RSA key certificate for re-signing server certificates for SSL inspection. Source vpn.certificate.local.name. <span class="li-normal">type: str</span></li>
            <li><span class="li-head">check_ca_cert</span> - Enable/disable verification of the user certificate and pass authentication if any CA in the chain is trusted . <span class="li-normal">type: str</span> <span class="li-normal">choices: enable,  disable</span></li>
            <li><span class="li-head">check_ca_chain</span> - Enable/disable verification of the entire certificate chain and pass authentication only if the chain is complete and all of the CAs in the chain are trusted . <span class="li-normal">type: str</span> <span class="li-normal">choices: enable,  disable</span></li>
            <li><span class="li-head">cmp_save_extra_certs</span> - Enable/disable saving extra certificates in CMP mode. <span class="li-normal">type: str</span> <span class="li-normal">choices: enable,  disable</span></li>
            <li><span class="li-head">cn_match</span> - When searching for a matching certificate, control how to find matches in the cn attribute of the certificate subject name. <span class="li-normal">type: str</span> <span class="li-normal">choices: substring,  value</span></li>
            <li><span class="li-head">ocsp_default_server</span> - Default OCSP server. Source vpn.certificate.ocsp-server.name. <span class="li-normal">type: str</span></li>
            <li><span class="li-head">ocsp_status</span> - Enable/disable receiving certificates using the OCSP. <span class="li-normal">type: str</span> <span class="li-normal">choices: enable,  disable</span></li>
            <li><span class="li-head">ssl_min_proto_version</span> - Minimum supported protocol version for SSL/TLS connections . <span class="li-normal">type: str</span> <span class="li-normal">choices: default,  SSLv3,  TLSv1,  TLSv1-1,  TLSv1-2</span></li>
            <li><span class="li-head">ssl_ocsp_option</span> - Specify whether the OCSP URL is from the certificate or the default OCSP server. <span class="li-normal">type: str</span> <span class="li-normal">choices: certificate,  server</span></li>
            <li><span class="li-head">ssl_ocsp_status</span> - Enable/disable SSL OCSP. <span class="li-normal">type: str</span> <span class="li-normal">choices: enable,  disable</span></li>
            <li><span class="li-head">strict_crl_check</span> - Enable/disable strict mode CRL checking. <span class="li-normal">type: str</span> <span class="li-normal">choices: enable,  disable</span></li>
            <li><span class="li-head">strict_ocsp_check</span> - Enable/disable strict mode OCSP checking. <span class="li-normal">type: str</span> <span class="li-normal">choices: enable,  disable</span></li>
            <li><span class="li-head">subject_match</span> - When searching for a matching certificate, control how to find matches in the certificate subject name. <span class="li-normal">type: str</span> <span class="li-normal">choices: substring,  value</span>
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
      - name: VPN certificate setting.
        fortios_vpn_certificate_setting:
          host:  "{{ host }}"
          username: "{{ username }}"
          password: "{{ password }}"
          vdom:  "{{ vdom }}"
          https: "False"
          vpn_certificate_setting:
            certname_dsa1024: "<your_own_value> (source vpn.certificate.local.name)"
            certname_dsa2048: "<your_own_value> (source vpn.certificate.local.name)"
            certname_ecdsa256: "<your_own_value> (source vpn.certificate.local.name)"
            certname_ecdsa384: "<your_own_value> (source vpn.certificate.local.name)"
            certname_rsa1024: "<your_own_value> (source vpn.certificate.local.name)"
            certname_rsa2048: "<your_own_value> (source vpn.certificate.local.name)"
            check_ca_cert: "enable"
            check_ca_chain: "enable"
            cmp_save_extra_certs: "enable"
            cn_match: "substring"
            ocsp_default_server: "<your_own_value> (source vpn.certificate.ocsp-server.name)"
            ocsp_status: "enable"
            ssl_min_proto_version: "default"
            ssl_ocsp_option: "certificate"
            ssl_ocsp_status: "enable"
            strict_crl_check: "enable"
            strict_ocsp_check: "enable"
            subject_match: "substring"



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