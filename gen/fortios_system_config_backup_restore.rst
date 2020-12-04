:source: fortios_system_config_backup_restore.py

:orphan:

.. fortios_system_config_backup_restore:

fortios_system_config_backup_restore -- Backup/restore fortigate configuration
++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++

.. versionadded:: 2.10

.. contents::
   :local:
   :depth: 1


Synopsis
--------
- This module is able to backup or restore the global or particial settings of the fortigate Examples include all parameters and values need to be adjusted to datasources before usage. Tested with FOS v6.0.0



Requirements
------------
The below requirements are needed on the host that executes this module.

- ansible>=2.9.0


Parameters
----------


.. raw:: html

    <ul>
    <li> <span class="li-head">host</span> - host of fortigate <span class="li-normal">type: str</span> <span class="li-required">required: False</span></li>
    <li> <span class="li-head">password</span> - password of fortigate <span class="li-normal">type: str</span> <span class="li-required">required: False</span></li>
    <li> <span class="li-head">username</span> - username of fortigate <span class="li-normal">type: str</span> <span class="li-required">required: False</span></li>
    <li> <span class="li-head">description</span> - descriptive text <span class="li-normal">type: str</span> <span class="li-required">required: False</span></li>
    <li> <span class="li-head">vdom</span> - vdom to operate on <span class="li-normal">type: str</span> <span class="li-required">required: False</span> <span class="li-normal">default: root</span></li>
    <li> <span class="li-head">config</span> - configuration to restore <span class="li-normal">type: str</span> <span class="li-required">required: False</span></li>
    <li> <span class="li-head">mkey</span> - primary key <span class="li-normal">type: str</span> <span class="li-required">required: False</span></li>
    <li> <span class="li-head">https</span> - use https or not <span class="li-normal">type: bool</span> <span class="li-required">required: False</span> <span class="li-normal">default: True</span></li>
    <li> <span class="li-head">ssl_verify</span> - enable ssl verification or not <span class="li-normal">type: bool</span> <span class="li-required">required: False</span> <span class="li-normal">default: True</span></li>
    <li> <span class="li-head">backup</span> - content to backup <span class="li-normal">type: str</span> <span class="li-required">required: False</span></li>
    <li> <span class="li-head">scope</span> - scope to operation on <span class="li-normal">type: str</span> <span class="li-required">required: True</span></li>
    <li> <span class="li-head">filename</span> - the file name <span class="li-normal">type: str</span> <span class="li-required">required: True</span></li>
    <li> <span class="li-head">commands</span> - the command <span class="li-normal">type: str</span> <span class="li-required">required: False</span></li>
    </ul>


Notes
-----

.. note::

   - Legacy fortiosapi has been deprecated, httpapi is the preferred way to run playbooks

   - But this module relies on fortiosapi, please make sure fortiosapi is installed before using it



Examples
--------

.. code-block:: yaml+jinja
    
    - hosts: localhost
      connection: httpapi
      collections:
        - fortinet.fortios
      vars:
        vdom: "root"
        host: "192.168.122.60"
        username: "admin"
        password: ""
      tasks:
      - name: backup global or a_specific_vdom settings
        fortios_system_config_backup_restore:
         config: "system config backup"
         host:  "{{ host }}"
         username: "{{ username }}"
         password: "{{ password }}"
         vdom: "{{ vdom }}"
         backup: "yes"
         https: True
         ssl_verify: False
         scope: "global or vdom"
         filename: "/tmp/backup_test"
      - name: Restore global or a_specific_vdom settings
        fortios_system_config_backup_restore:
         config: "system config restore"
         host:  "{{ host }}"
         username: "{{ username }}"
         password: "{{ password }}"
         vdom:  "{{ vdom }}"
         https: True
         ssl_verify: False
         scope: "global or vdom"
         filename: "/tmp/backup_test"
    


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
