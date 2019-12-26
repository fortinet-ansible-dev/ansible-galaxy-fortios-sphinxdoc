:source: fortios_system_firmware_upgrade.py

:orphan:

.. _fortios_system_firmware_upgrade:

fortios_system_firmware_upgrade -- Perform firmware upgrade on FortiGate or FortiOS (FOS) device.
+++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++

.. versionadded:: 2.9

.. contents::
   :local:
   :depth: 1


Synopsis
--------
- This module is able to perform firmware upgrade on FortiGate or FortiOS (FOS) device by specifying firmware upgrade source, filename and whether format boot partition before upgrade. Examples include all parameters and values need to be adjusted to datasources before usage. Tested with FOS v6.0.2


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
    <li><span class="li-head">vdom</span> - Virtual domain, among those defined previously. A vdom is a virtual instance of the FortiGate that can be configured and used as a different unit. <span class="li-normal">type: str</span> <span class="li-normal">default: root</span> <span class="li-required">required: false</span></li>
    <li><span class="li-head">https</span> - Indicates if the requests towards FortiGate must use HTTPS protocol. <span class="li-normal">type: bool</span> <span class="li-normal">default: true</span> <span class="li-required">required: false</span></li>
    <li><span class="li-head">ssl_verify</span> - Ensures FortiGate certificate must be verified by a proper CA. <span class="li-normal">type: bool</span> <span class="li-normal">default: true</span> <span class="li-required">required: false</span></li>
    <li><span class="li-head">system_firmware</span> - Possible parameters to go in the body for the request. Specify firmware upgrade source, filename and whether format boot partition before upgrade <span class="li-normal">default: null</span> <span class="li-normal">type: dict</span> <span class="li-required">required</span></li>
            <ul class="ul-self">

            <li><span class="li-head">file_content</span> - "Provided when uploading a file: base64 encoded file data. Must not contain whitespace or other invalid base64 characters. Must be included in HTTP body." <span class="li-normal">type: str</span> <span class="li-required">required: false</span></li>
            <li><span class="li-head">filename</span> - Name and path of the local firmware file. <span class="li-normal">type: str</span> <span class="li-required">required</span></li>
            <li><span class="li-head">format_partition</span> - Set to true to format boot partition before upgrade. <span class="li-normal">type: bool</span> <span class="li-required">required: false</span></li>
            <li><span class="li-head">source</span> - Firmware file data source [upload|usb|fortiguard]. <span class="li-normal">type: str</span> <span class="li-required">required</span> <span class="li-normal">choices: upload,  usb,  fortiguard</span>
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
      - name: Perform firmware upgrade with local firmware file.
        fortios_system_firmware:
          host:  "{{ host }}"
          username: "{{ username }}"
          password: "{{ password }}"
          vdom:  "{{ vdom }}"
          ssl_verify: "False"
          system_firmware:
            file_content: "<your_own_value>"
            filename: "<your_own_value>"
            format_partition: "<your_own_value>"
            source: "upload"
        register: fortios_system_firmware_upgrade_result

      - debug:
          var:
            # please check the following status to confirm
            fortios_system_firmware_upgrade_result.meta.results.status

      - name: Perform firmware upgrade with firmware file on USB.
        fortios_system_firmware_upgrade:
          host:  "{{ host }}"
          username: "{{ username }}"
          password: "{{ password }}"
          vdom:  "{{ vdom }}"
          ssl_verify: "False"
          system_firmware:
            filename: "<your_own_value>"
            format_partition: "<your_own_value>"
            source: "usb"
        register: fortios_system_firmware_upgrade_result

      - debug:
          var:
            # please check the following status to confirm
            fortios_system_firmware_upgrade_result.meta.results.status

      - name: Perform firmware upgrade from FortiGuard.
        fortios_system_firmware_upgrade:
          host:  "{{ host }}"
          username: "{{ username }}"
          password: "{{ password }}"
          vdom:  "{{ vdom }}"
          ssl_verify: "False"
          system_firmware:
            filename: "<your_own_value>"
            format_partition: "<your_own_value>"
            source: "fortiguard"
        register: fortios_system_firmware_upgrade_result

      - debug:
          var:
            # please check the following status to confirm
            fortios_system_firmware_upgrade_result.meta.results.status



Return Values
-------------
Common return values are documented: https://docs.ansible.com/ansible/latest/reference_appendices/common_return_values.html#common-return-values, the following are the fields unique to this module:

.. raw:: html

    <ul>

    <li><span class="li-return">build</span> - Build number of the fortigate image <span class="li-normal">returned: always</span> <span class="li-normal">type: str</span> <span class="li-normal">sample: '1547'</span></li>
    <li><span class="li-return">http_method</span> - Last method used to provision the content into FortiGate <span class="li-normal">returned: always</span> <span class="li-normal">type: str</span> <span class="li-normal">sample: 'POST'</span></li>
    <li><span class="li-return">name</span> - Name of the table used to fulfill the request <span class="li-normal">returned: always</span> <span class="li-normal">type: str</span> <span class="li-normal">sample: firmware</span></li>
    <li><span class="li-return">path</span> - Path of the table used to fulfill the request <span class="li-normal">returned: always</span> <span class="li-normal">type: str</span> <span class="li-normal">sample: system</span></li>
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

- Don Yao (@fortinetps)
- Miguel Angel Munoz (@mamunozgonzalez)
- Nicolas Thomas (@thomnico)



.. hint::
    If you notice any issues in this documentation, you can create a pull request to improve it.