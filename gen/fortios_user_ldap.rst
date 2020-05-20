:source: fortios_user_ldap.py

:orphan:

.. fortios_user_ldap:

fortios_user_ldap -- Configure LDAP server entries in Fortinet's FortiOS and FortiGate.
+++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++

.. versionadded:: 2.9

.. contents::
   :local:
   :depth: 1


Synopsis
--------
- This module is able to configure a FortiGate or FortiOS (FOS) device by allowing the user to set and modify user feature and ldap category. Examples include all parameters and values need to be adjusted to datasources before usage. Tested with FOS v6.0.5



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
    <li> <span class="li-head">user_ldap</span> - Configure LDAP server entries. <span class="li-normal">type: dict</span></li>
        <ul class="ul-self">
        <li> <span class="li-head">account_key_filter</span> - Account key filter, using the UPN as the search filter. <span class="li-normal">type: str</span></li>
        <li> <span class="li-head">account_key_processing</span> - Account key processing operation, either keep or strip domain string of UPN in the token. <span class="li-normal">type: str</span> <span class="li-normal">choices: same, strip</span></li>
        <li> <span class="li-head">ca_cert</span> - CA certificate name. Source vpn.certificate.ca.name. <span class="li-normal">type: str</span></li>
        <li> <span class="li-head">cnid</span> - Common name identifier for the LDAP server. The common name identifier for most LDAP servers is "cn". <span class="li-normal">type: str</span></li>
        <li> <span class="li-head">dn</span> - Distinguished name used to look up entries on the LDAP server. <span class="li-normal">type: str</span></li>
        <li> <span class="li-head">group_filter</span> - Filter used for group matching. <span class="li-normal">type: str</span></li>
        <li> <span class="li-head">group_member_check</span> - Group member checking methods. <span class="li-normal">type: str</span> <span class="li-normal">choices: user-attr, group-object, posix-group-object</span></li>
        <li> <span class="li-head">group_object_filter</span> - Filter used for group searching. <span class="li-normal">type: str</span></li>
        <li> <span class="li-head">group_search_base</span> - Search base used for group searching. <span class="li-normal">type: str</span></li>
        <li> <span class="li-head">member_attr</span> - Name of attribute from which to get group membership. <span class="li-normal">type: str</span></li>
        <li> <span class="li-head">name</span> - LDAP server entry name. <span class="li-normal">type: str</span> <span class="li-required">required: True</span></li>
        <li> <span class="li-head">password</span> - Password for initial binding. <span class="li-normal">type: str</span></li>
        <li> <span class="li-head">password_expiry_warning</span> - Enable/disable password expiry warnings. <span class="li-normal">type: str</span> <span class="li-normal">choices: enable, disable</span></li>
        <li> <span class="li-head">password_renewal</span> - Enable/disable online password renewal. <span class="li-normal">type: str</span> <span class="li-normal">choices: enable, disable</span></li>
        <li> <span class="li-head">port</span> - Port to be used for communication with the LDAP server . <span class="li-normal">type: int</span></li>
        <li> <span class="li-head">secondary_server</span> - Secondary LDAP server CN domain name or IP. <span class="li-normal">type: str</span></li>
        <li> <span class="li-head">secure</span> - Port to be used for authentication. <span class="li-normal">type: str</span> <span class="li-normal">choices: disable, starttls, ldaps</span></li>
        <li> <span class="li-head">server</span> - LDAP server CN domain name or IP. <span class="li-normal">type: str</span></li>
        <li> <span class="li-head">server_identity_check</span> - Enable/disable LDAP server identity check (verify server domain name/IP address against the server certificate). <span class="li-normal">type: str</span> <span class="li-normal">choices: enable, disable</span></li>
        <li> <span class="li-head">source_ip</span> - Source IP for communications to LDAP server. <span class="li-normal">type: str</span></li>
        <li> <span class="li-head">ssl_min_proto_version</span> - Minimum supported protocol version for SSL/TLS connections . <span class="li-normal">type: str</span> <span class="li-normal">choices: default, SSLv3, TLSv1, TLSv1-1, TLSv1-2</span></li>
        <li> <span class="li-head">tertiary_server</span> - Tertiary LDAP server CN domain name or IP. <span class="li-normal">type: str</span></li>
        <li> <span class="li-head">type</span> - Authentication type for LDAP searches. <span class="li-normal">type: str</span> <span class="li-normal">choices: simple, anonymous, regular</span></li>
        <li> <span class="li-head">username</span> - Username (full DN) for initial binding. <span class="li-normal">type: str</span></li>
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
      - name: Configure LDAP server entries.
        fortios_user_ldap:
          vdom:  "{{ vdom }}"
          state: "present"
          user_ldap:
            account_key_filter: "<your_own_value>"
            account_key_processing: "same"
            ca_cert: "<your_own_value> (source vpn.certificate.ca.name)"
            cnid: "<your_own_value>"
            dn: "<your_own_value>"
            group_filter: "<your_own_value>"
            group_member_check: "user-attr"
            group_object_filter: "<your_own_value>"
            group_search_base: "<your_own_value>"
            member_attr: "<your_own_value>"
            name: "default_name_13"
            password: "<your_own_value>"
            password_expiry_warning: "enable"
            password_renewal: "enable"
            port: "17"
            secondary_server: "<your_own_value>"
            secure: "disable"
            server: "192.168.100.40"
            server_identity_check: "enable"
            source_ip: "84.230.14.43"
            ssl_min_proto_version: "default"
            tertiary_server: "<your_own_value>"
            type: "simple"
            username: "<your_own_value>"


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
