:source: fortios_system_dns_database.py

:orphan:

.. fortios_system_dns_database:

fortios_system_dns_database -- Configure DNS databases in Fortinet's FortiOS and FortiGate.
+++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++

.. versionadded:: 2.9

.. contents::
   :local:
   :depth: 1


Synopsis
--------
- This module is able to configure a FortiGate or FortiOS (FOS) device by allowing the user to set and modify system feature and dns_database category. Examples include all parameters and values need to be adjusted to datasources before usage. Tested with FOS v6.2.0



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
    <li> <span class="li-head">system_dns_database</span> - Configure DNS databases. <span class="li-normal">type: dict</span></li>
        <ul class="ul-self">
        <li> <span class="li-head">allow_transfer</span> - DNS zone transfer IP address list. <span class="li-normal">type: str</span></li>
        <li> <span class="li-head">authoritative</span> - Enable/disable authoritative zone. <span class="li-normal">type: str</span> <span class="li-normal">choices: enable, disable</span></li>
        <li> <span class="li-head">contact</span> - Email address of the administrator for this zone.  You can specify only the username (e.g. admin) or full email address (e.g. admin@test .com)   When using a simple username, the domain of the email will be this zone. <span class="li-normal">type: str</span></li>
        <li> <span class="li-head">dns_entry</span> - DNS entry. <span class="li-normal">type: list</span></li>
            <ul class="ul-self">
            <li> <span class="li-head">canonical_name</span> - Canonical name of the host. <span class="li-normal">type: str</span></li>
            <li> <span class="li-head">hostname</span> - Name of the host. <span class="li-normal">type: str</span></li>
            <li> <span class="li-head">id</span> - DNS entry ID. <span class="li-normal">type: int</span> <span class="li-required">required: True</span></li>
            <li> <span class="li-head">ip</span> - IPv4 address of the host. <span class="li-normal">type: str</span></li>
            <li> <span class="li-head">ipv6</span> - IPv6 address of the host. <span class="li-normal">type: str</span></li>
            <li> <span class="li-head">preference</span> - DNS entry preference, 0 is the highest preference (0 - 65535) <span class="li-normal">type: int</span></li>
            <li> <span class="li-head">status</span> - Enable/disable resource record status. <span class="li-normal">type: str</span> <span class="li-normal">choices: enable, disable</span></li>
            <li> <span class="li-head">ttl</span> - Time-to-live for this entry (0 to 2147483647 sec). <span class="li-normal">type: int</span></li>
            <li> <span class="li-head">type</span> - Resource record type. <span class="li-normal">type: str</span> <span class="li-normal">choices: A, NS, CNAME, MX, AAAA, PTR, PTR_V6</span></li>
            </ul>
        <li> <span class="li-head">domain</span> - Domain name. <span class="li-normal">type: str</span></li>
        <li> <span class="li-head">forwarder</span> - DNS zone forwarder IP address list. <span class="li-normal">type: str</span></li>
        <li> <span class="li-head">ip_master</span> - IP address of master DNS server. Entries in this master DNS server and imported into the DNS zone. <span class="li-normal">type: str</span></li>
        <li> <span class="li-head">name</span> - Zone name. <span class="li-normal">type: str</span> <span class="li-required">required: True</span></li>
        <li> <span class="li-head">primary_name</span> - Domain name of the default DNS server for this zone. <span class="li-normal">type: str</span></li>
        <li> <span class="li-head">source_ip</span> - Source IP for forwarding to DNS server. <span class="li-normal">type: str</span></li>
        <li> <span class="li-head">status</span> - Enable/disable this DNS zone. <span class="li-normal">type: str</span> <span class="li-normal">choices: enable, disable</span></li>
        <li> <span class="li-head">ttl</span> - Default time-to-live value for the entries of this DNS zone (0 - 2147483647 sec). <span class="li-normal">type: int</span></li>
        <li> <span class="li-head">type</span> - Zone type (master to manage entries directly, slave to import entries from other zones). <span class="li-normal">type: str</span> <span class="li-normal">choices: master, slave</span></li>
        <li> <span class="li-head">view</span> - Zone view (public to serve public clients, shadow to serve internal clients). <span class="li-normal">type: str</span> <span class="li-normal">choices: shadow, public</span></li>
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
      - name: Configure DNS databases.
        fortios_system_dns_database:
          vdom:  "{{ vdom }}"
          state: "present"
          access_token: "<your_own_value>"
          system_dns_database:
            allow_transfer: "<your_own_value>"
            authoritative: "enable"
            contact: "<your_own_value>"
            dns_entry:
             -
                canonical_name: "<your_own_value>"
                hostname: "myhostname"
                id:  "9"
                ip: "<your_own_value>"
                ipv6: "<your_own_value>"
                preference: "12"
                status: "enable"
                ttl: "14"
                type: "A"
            domain: "<your_own_value>"
            forwarder: "<your_own_value>"
            ip_master: "<your_own_value>"
            name: "default_name_19"
            primary_name: "<your_own_value>"
            source_ip: "84.230.14.43"
            status: "enable"
            ttl: "23"
            type: "master"
            view: "shadow"
    


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
