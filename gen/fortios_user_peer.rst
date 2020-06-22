:source: fortios_user_peer.py

:orphan:

.. fortios_user_peer:

fortios_user_peer -- Configure peer users in Fortinet's FortiOS and FortiGate.
++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++

.. versionadded:: 2.9

.. contents::
   :local:
   :depth: 1


Synopsis
--------
- This module is able to configure a FortiGate or FortiOS (FOS) device by allowing the user to set and modify user feature and peer category. Examples include all parameters and values need to be adjusted to datasources before usage. Tested with FOS v6.0.0



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
    <li> <span class="li-head">state</span> - Indicates whether to create or remove the object. <span class="li-normal">type: str</span> <span class="li-required">required: True</span> <span class="li-normal">choices: present, absent</span></li>
    <li> <span class="li-head">user_peer</span> - Configure peer users. <span class="li-normal">type: dict</span></li>
        <ul class="ul-self">
        <li> <span class="li-head">ca</span> - Name of the CA certificate as returned by the execute vpn certificate ca list command. Source vpn.certificate.ca.name. <span class="li-normal">type: str</span></li>
        <li> <span class="li-head">cn</span> - Peer certificate common name. <span class="li-normal">type: str</span></li>
        <li> <span class="li-head">cn_type</span> - Peer certificate common name type. <span class="li-normal">type: str</span> <span class="li-normal">choices: string, email, FQDN, ipv4, ipv6</span></li>
        <li> <span class="li-head">ldap_mode</span> - Mode for LDAP peer authentication. <span class="li-normal">type: str</span> <span class="li-normal">choices: password, principal-name</span></li>
        <li> <span class="li-head">ldap_password</span> - Password for LDAP server bind. <span class="li-normal">type: str</span></li>
        <li> <span class="li-head">ldap_server</span> - Name of an LDAP server defined under the user ldap command. Performs client access rights check. Source user.ldap.name. <span class="li-normal">type: str</span></li>
        <li> <span class="li-head">ldap_username</span> - Username for LDAP server bind. <span class="li-normal">type: str</span></li>
        <li> <span class="li-head">mandatory_ca_verify</span> - Determine what happens to the peer if the CA certificate is not installed. Disable to automatically consider the peer certificate as valid. <span class="li-normal">type: str</span> <span class="li-normal">choices: enable, disable</span></li>
        <li> <span class="li-head">name</span> - Peer name. <span class="li-normal">type: str</span> <span class="li-required">required: True</span></li>
        <li> <span class="li-head">ocsp_override_server</span> - Online Certificate Status Protocol (OCSP) server for certificate retrieval. Source vpn.certificate.ocsp-server.name. <span class="li-normal">type: str</span></li>
        <li> <span class="li-head">passwd</span> - Peer"s password used for two-factor authentication. <span class="li-normal">type: str</span></li>
        <li> <span class="li-head">subject</span> - Peer certificate name constraints. <span class="li-normal">type: str</span></li>
        <li> <span class="li-head">two_factor</span> - Enable/disable two-factor authentication, applying certificate and password-based authentication. <span class="li-normal">type: str</span> <span class="li-normal">choices: enable, disable</span></li>
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
      - name: Configure peer users.
        fortios_user_peer:
          vdom:  "{{ vdom }}"
          state: "present"
          user_peer:
            ca: "<your_own_value> (source vpn.certificate.ca.name)"
            cn: "<your_own_value>"
            cn_type: "string"
            ldap_mode: "password"
            ldap_password: "<your_own_value>"
            ldap_server: "<your_own_value> (source user.ldap.name)"
            ldap_username: "<your_own_value>"
            mandatory_ca_verify: "enable"
            name: "default_name_11"
            ocsp_override_server: "<your_own_value> (source vpn.certificate.ocsp-server.name)"
            passwd: "<your_own_value>"
            subject: "<your_own_value>"
            two_factor: "enable"


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
