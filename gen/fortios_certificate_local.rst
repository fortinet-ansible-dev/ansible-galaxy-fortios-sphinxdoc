:source: fortios_certificate_local.py

:orphan:

.. fortios_certificate_local:

fortios_certificate_local -- Local keys and certificates in Fortinet's FortiOS and FortiGate.
+++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++

.. versionadded:: 2.9

.. contents::
   :local:
   :depth: 1


Synopsis
--------
- This module is able to configure a FortiGate or FortiOS (FOS) device by allowing the user to set and modify certificate feature and local category. Examples include all parameters and values need to be adjusted to datasources before usage. Tested with FOS v6.4.0



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
    <li> <span class="li-head">state</span> - Indicates whether to create or remove the object. <span class="li-normal">type: str</span> <span class="li-required">required: True</span> <span class="li-normal">choices: present, absent</span></li>
    <li> <span class="li-head">certificate_local</span> - Local keys and certificates. <span class="li-normal">type: dict</span></li>
        <ul class="ul-self">
        <li> <span class="li-head">auto_regenerate_days</span> - Number of days to wait before expiry of an updated local certificate is requested (0 = disabled). <span class="li-normal">type: int</span></li>
        <li> <span class="li-head">auto_regenerate_days_warning</span> - Number of days to wait before an expiry warning message is generated (0 = disabled). <span class="li-normal">type: int</span></li>
        <li> <span class="li-head">ca_identifier</span> - CA identifier of the CA server for signing via SCEP. <span class="li-normal">type: str</span></li>
        <li> <span class="li-head">certificate</span> - PEM format certificate. <span class="li-normal">type: str</span></li>
        <li> <span class="li-head">cmp_path</span> - Path location inside CMP server. <span class="li-normal">type: str</span></li>
        <li> <span class="li-head">cmp_regeneration_method</span> - CMP auto-regeneration method. <span class="li-normal">type: str</span> <span class="li-normal">choices: keyupate, renewal</span></li>
        <li> <span class="li-head">cmp_server</span> - "ADDRESS:PORT" for CMP server. <span class="li-normal">type: str</span></li>
        <li> <span class="li-head">cmp_server_cert</span> - CMP server certificate. Source certificate.ca.name. <span class="li-normal">type: str</span></li>
        <li> <span class="li-head">comments</span> - Comment. <span class="li-normal">type: str</span></li>
        <li> <span class="li-head">csr</span> - Certificate Signing Request. <span class="li-normal">type: str</span></li>
        <li> <span class="li-head">enroll_protocol</span> - Certificate enrollment protocol. <span class="li-normal">type: str</span> <span class="li-normal">choices: none, scep, cmpv2</span></li>
        <li> <span class="li-head">ike_localid</span> - Local ID the FortiGate uses for authentication as a VPN client. <span class="li-normal">type: str</span></li>
        <li> <span class="li-head">ike_localid_type</span> - IKE local ID type. <span class="li-normal">type: str</span> <span class="li-normal">choices: asn1dn, fqdn</span></li>
        <li> <span class="li-head">name</span> - Name. <span class="li-normal">type: str</span> <span class="li-required">required: True</span></li>
        <li> <span class="li-head">name_encoding</span> - Name encoding method for auto-regeneration. <span class="li-normal">type: str</span> <span class="li-normal">choices: printable, utf8</span></li>
        <li> <span class="li-head">password</span> - Password as a PEM file. <span class="li-normal">type: str</span></li>
        <li> <span class="li-head">private_key</span> - PEM format key, encrypted with a password. <span class="li-normal">type: str</span></li>
        <li> <span class="li-head">range</span> - Either a global or VDOM IP address range for the certificate. <span class="li-normal">type: str</span> <span class="li-normal">choices: global, vdom</span></li>
        <li> <span class="li-head">scep_password</span> - SCEP server challenge password for auto-regeneration. <span class="li-normal">type: str</span></li>
        <li> <span class="li-head">scep_url</span> - SCEP server URL. <span class="li-normal">type: str</span></li>
        <li> <span class="li-head">source</span> - Certificate source type. <span class="li-normal">type: str</span> <span class="li-normal">choices: factory, user, bundle</span></li>
        <li> <span class="li-head">source_ip</span> - Source IP address for communications to the SCEP server. <span class="li-normal">type: str</span></li>
        <li> <span class="li-head">state</span> - Certificate Signing Request State. <span class="li-normal">type: str</span></li>
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
      - name: Local keys and certificates.
        fortios_certificate_local:
          vdom:  "{{ vdom }}"
          state: "present"
          access_token: "<your_own_value>"
          certificate_local:
            auto_regenerate_days: "3"
            auto_regenerate_days_warning: "4"
            ca_identifier:  "myId_5"
            certificate: "<your_own_value>"
            cmp_path: "<your_own_value>"
            cmp_regeneration_method: "keyupate"
            cmp_server: "<your_own_value>"
            cmp_server_cert: "<your_own_value> (source certificate.ca.name)"
            comments: "<your_own_value>"
            csr: "<your_own_value>"
            enroll_protocol: "none"
            ike_localid: "<your_own_value>"
            ike_localid_type: "asn1dn"
            name: "default_name_16"
            name_encoding: "printable"
            password: "<your_own_value>"
            private_key: "<your_own_value>"
            range: "global"
            scep_password: "<your_own_value>"
            scep_url: "<your_own_value>"
            source: "factory"
            source_ip: "84.230.14.43"
            state: "<your_own_value>"
    


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
