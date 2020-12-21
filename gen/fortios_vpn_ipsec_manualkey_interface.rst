:source: fortios_vpn_ipsec_manualkey_interface.py

:orphan:

.. fortios_vpn_ipsec_manualkey_interface:

fortios_vpn_ipsec_manualkey_interface -- Configure IPsec manual keys in Fortinet's FortiOS and FortiGate.
+++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++

.. versionadded:: 2.8

.. contents::
   :local:
   :depth: 1


Synopsis
--------
- This module is able to configure a FortiGate or FortiOS (FOS) device by allowing the user to set and modify vpn_ipsec feature and manualkey_interface category. Examples include all parameters and values need to be adjusted to datasources before usage. Tested with FOS v6.4.0



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
    <li> <span class="li-head">vpn_ipsec_manualkey_interface</span> - Configure IPsec manual keys. <span class="li-normal">type: dict</span></li>
        <ul class="ul-self">
        <li> <span class="li-head">state</span> - B(Deprecated) <span class="li-normal">type: str</span> <span class="li-required">required: False</span> <span class="li-normal">choices: present, absent</span></li>
        <li> <span class="li-head">addr_type</span> - IP version to use for IP packets. <span class="li-normal">type: str</span> <span class="li-normal">choices: 4, 6</span></li>
        <li> <span class="li-head">auth_alg</span> - Authentication algorithm. Must be the same for both ends of the tunnel. <span class="li-normal">type: str</span> <span class="li-normal">choices: None, md5, sha1, sha256, sha384, sha512</span></li>
        <li> <span class="li-head">auth_key</span> - Hexadecimal authentication key in 16-digit (8-byte) segments separated by hyphens. <span class="li-normal">type: str</span></li>
        <li> <span class="li-head">enc_alg</span> - Encryption algorithm. Must be the same for both ends of the tunnel. <span class="li-normal">type: str</span> <span class="li-normal">choices: None, des, 3des, aes128, aes192, aes256, aria128, aria192, aria256, seed</span></li>
        <li> <span class="li-head">enc_key</span> - Hexadecimal encryption key in 16-digit (8-byte) segments separated by hyphens. <span class="li-normal">type: str</span></li>
        <li> <span class="li-head">interface</span> - Name of the physical, aggregate, or VLAN interface. Source system.interface.name. <span class="li-normal">type: str</span></li>
        <li> <span class="li-head">ip_version</span> - IP version to use for VPN interface. <span class="li-normal">type: str</span> <span class="li-normal">choices: 4, 6</span></li>
        <li> <span class="li-head">local_gw</span> - IPv4 address of the local gateway"s external interface. <span class="li-normal">type: str</span></li>
        <li> <span class="li-head">local_gw6</span> - Local IPv6 address of VPN gateway. <span class="li-normal">type: str</span></li>
        <li> <span class="li-head">local_spi</span> - Local SPI, a hexadecimal 8-digit (4-byte) tag. Discerns between two traffic streams with different encryption rules. <span class="li-normal">type: str</span></li>
        <li> <span class="li-head">name</span> - IPsec tunnel name. <span class="li-normal">type: str</span> <span class="li-required">required: True</span></li>
        <li> <span class="li-head">remote_gw</span> - IPv4 address of the remote gateway"s external interface. <span class="li-normal">type: str</span></li>
        <li> <span class="li-head">remote_gw6</span> - Remote IPv6 address of VPN gateway. <span class="li-normal">type: str</span></li>
        <li> <span class="li-head">remote_spi</span> - Remote SPI, a hexadecimal 8-digit (4-byte) tag. Discerns between two traffic streams with different encryption rules. <span class="li-normal">type: str</span></li>
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
      - name: Configure IPsec manual keys.
        fortios_vpn_ipsec_manualkey_interface:
          vdom:  "{{ vdom }}"
          state: "present"
          access_token: "<your_own_value>"
          vpn_ipsec_manualkey_interface:
            addr_type: "4"
            auth_alg: "null"
            auth_key: "<your_own_value>"
            enc_alg: "null"
            enc_key: "<your_own_value>"
            interface: "<your_own_value> (source system.interface.name)"
            ip_version: "4"
            local_gw: "<your_own_value>"
            local_gw6: "<your_own_value>"
            local_spi: "<your_own_value>"
            name: "default_name_13"
            remote_gw: "<your_own_value>"
            remote_gw6: "<your_own_value>"
            remote_spi: "<your_own_value>"
    


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
