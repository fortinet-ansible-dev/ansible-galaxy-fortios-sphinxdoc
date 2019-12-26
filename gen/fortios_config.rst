:source: fortios_config.py

:orphan:

.. _fortios_config:

fortios_config -- Manage config on Fortinet FortiOS firewall devices
++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++

.. versionadded:: 2.3

.. contents::
   :local:
   :depth: 1


Synopsis
--------
- This module provides management of FortiOS Devices configuration.


Requirements
------------
The below requirements are needed on the host that executes this module.

- pyFG


Parameters
----------

.. raw:: html

    <ul>

    <li><span class="li-head">src</span> - The I(src) argument provides a path to the configuration template to load into the remote device.</li>
    <li><span class="li-head">filter</span> - Only for partial backup, you can restrict by giving expected configuration path (ex. firewall address). <span class="li-normal">default: ""</span>
    </ul>




Notes
-----

.. note::


   - Requires fortiosapi library developed by Fortinet

   - Run as a local_action in your playbook



Examples
--------

.. code-block:: yaml+jinja

    - name: Backup current config
      fortios_config:
        host: 192.168.0.254
        username: admin
        password: password
        backup: yes

    - name: Backup only address objects
      fortios_config:
        host: 192.168.0.254
        username: admin
        password: password
        backup: yes
        backup_path: /tmp/forti_backup/
        filter: "firewall address"

    - name: Update configuration from file
      fortios_config:
        host: 192.168.0.254
        username: admin
        password: password
        src: new_configuration.conf.j2




Return Values
-------------
Common return values are documented: https://docs.ansible.com/ansible/latest/reference_appendices/common_return_values.html#common-return-values, the following are the fields unique to this module:

.. raw:: html

    <ul>

    <li><span class="li-return">running_config</span> - full config string <span class="li-normal">returned: always</span> <span class="li-normal">type: str</span></li>
    <li><span class="li-return">change_string</span> - The commands really executed by the module <span class="li-normal">returned: only if config changed</span> <span class="li-normal">type: str</span></li>
    </ul>



Status
------

- This module is not guaranteed to have a backwards compatible interface.



Authors
-------

- Benjamin Jolivot (@bjolivot)



.. hint::
    If you notice any issues in this documentation, you can create a pull request to improve it.