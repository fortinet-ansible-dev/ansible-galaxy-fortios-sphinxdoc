:source: fortios_address.py

:orphan:

.. _fortios_address:

fortios_address -- Manage fortios firewall address objects.
+++++++++++++++++++++++++++++++++++++++++++++++++++++++++++

.. versionadded:: 2.4

.. contents::
   :local:
   :depth: 1


Synopsis
--------
- This module provide management of firewall addresses on FortiOS devices.


Requirements
------------
The below requirements are needed on the host that executes this module.

- fortiosapi>=0.9.8


Parameters
----------

.. raw:: html

    <ul>

    <li><span class="li-head">state</span> - Specifies if address need to be added or deleted. <span class="li-required">required</span> <span class="li-normal">choices: ['present', 'absent']</li>
    <li><span class="li-head">name</span> - Name of the address to add or delete. <span class="li-required">required</span> <span class="li-normal">type:</span> Type of the address. <span class="li-normal">choices: ['iprange', 'fqdn', 'ipmask', 'geography']</li>
    <li><span class="li-head">value</span> - Address value, based on type. If type=fqdn, something like www.google.com. If type=ipmask, you can use simple ip (192.168.0.1), ip+mask (192.168.0.1 255.255.255.0) or CIDR (192.168.0.1/32).</li>
    <li><span class="li-head">start_ip</span> - First ip in range (used only with type=iprange).</li>
    <li><span class="li-head">end_ip</span> - Last ip in range (used only with type=iprange).</li>
    <li><span class="li-head">country</span> - 2 letter country code (like FR).</li>
    <li><span class="li-head">interface</span> - interface name the address apply to. <span class="li-normal">default: any</span></li>
    <li><span class="li-head">comment</span> - free text to describe address.
    </ul>




Notes
-----

.. note::


   - This module requires netaddr python library.



Examples
--------

.. code-block:: yaml+jinja

    - name: Register french addresses
      fortios_address:
        host: 192.168.0.254
        username: admin
        password: p4ssw0rd
        state: present
        name: "fromfrance"
        type: geography
        country: FR
        comment: "French geoip address"

    - name: Register some fqdn
      fortios_address:
        host: 192.168.0.254
        username: admin
        password: p4ssw0rd
        state: present
        name: "Ansible"
        type: fqdn
        value: www.ansible.com
        comment: "Ansible website"

    - name: Register google DNS
      fortios_address:
        host: 192.168.0.254
        username: admin
        password: p4ssw0rd
        state: present
        name: "google_dns"
        type: ipmask
        value: 8.8.8.8




Return Values
-------------
Common return values are documented: https://docs.ansible.com/ansible/latest/reference_appendices/common_return_values.html#common-return-values, the following are the fields unique to this module:

.. raw:: html

    <ul>

    <li><span class="li-return">firewall_address_config</span> - full firewall addresses config string. <span class="li-normal">returned: always</span> <span class="li-normal">type: str</span></li>
    <li><span class="li-return">change_string</span> - The commands executed by the module. <span class="li-normal">returned: only if config changed</span> <span class="li-normal">type: str</span></li>
    </ul>



Status
------

- This module is not guaranteed to have a backwards compatible interface.



Authors
-------

- Benjamin Jolivot (@bjolivot)



.. hint::
    If you notice any issues in this documentation, you can create a pull request to improve it.