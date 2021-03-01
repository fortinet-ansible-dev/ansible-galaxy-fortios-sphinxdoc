:source: fortios_facts.py

:orphan:

.. fortios_facts:

fortios_facts -- Get facts about fortios devices (about to be deprecated).
++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++

.. versionadded:: 2.9

.. contents::
   :local:
   :depth: 1


Synopsis
--------
- Collects facts from network devices running the fortios operating system. This module places the facts gathered in the fact tree keyed by the respective resource name.  This facts module will only collect those facts which user specified in playbook.



Requirements
------------
The below requirements are needed on the host that executes this module.

- galaxy collection fortinet.fortios


Parameters
----------


.. raw:: html

    <ul>
    <li> <span class="li-head">host</span> - FortiOS or FortiGate IP address. <span class="li-normal">type: str</span> <span class="li-required">required: False</span></li>
    <li> <span class="li-head">username</span> - FortiOS or FortiGate username. <span class="li-normal">type: str</span> <span class="li-required">required: False</span></li>
    <li> <span class="li-head">password</span> - FortiOS or FortiGate password. <span class="li-normal">type: str</span> <span class="li-required">required: False</span> <span class="li-normal">default: </span></li>
    <li> <span class="li-head">vdom</span> - Virtual domain, among those defined previously. A vdom is a virtual instance of the FortiGate that can be configured and used as a different unit. <span class="li-normal">type: str</span> <span class="li-required">required: False</span> <span class="li-normal">default: root</span></li>
    <li> <span class="li-head">https</span> - Indicates if the requests towards FortiGate must use HTTPS protocol. <span class="li-normal">type: bool</span> <span class="li-required">required: False</span> <span class="li-normal">default: True</span></li>
    <li> <span class="li-head">ssl_verify</span> - Ensures FortiGate certificate must be verified by a proper CA. <span class="li-normal">type: bool</span> <span class="li-required">required: False</span> <span class="li-normal">default: False</span></li>
    <li> <span class="li-head">gather_subset</span> - When supplied, this argument will restrict the facts collected to a given subset.  Possible values for this argument include system_current-admins_select, system_firmware_select, system_fortimanager_status, system_ha-checksums_select, system_interface_select, system_status_select and system_time_select <span class="li-normal">type: list</span></li>
        <ul class="ul-self">
        <li> <span class="li-head">fact</span> - Name of the facts to gather <span class="li-normal">type: str</span> <span class="li-required">required: True</span></li>
        <li> <span class="li-head">filters</span> - Filters apply when gathering facts <span class="li-normal">type: list</span></li>
        </ul>
    </ul>


Notes
-----

.. note::

   - httpapi mode is the new recommended way for any network modules

   - the module is going to be deprecated in next major release.



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
      - name: gather basic system status facts
        fortios_facts:
          host:  "{{ host }}"
          username: "{{ username }}"
          password: "{{ password }}"
          vdom:  "{{ vdom }}"
          gather_subset:
            - fact: 'system_status_select'
    
      - name: gather all physical interfaces status facts
        fortios_facts:
          host:  "{{ host }}"
          username: "{{ username }}"
          password: "{{ password }}"
          vdom:  "{{ vdom }}"
          gather_subset:
            - fact: 'system_interface_select'
    
      - name: gather gather all physical and vlan interfaces status facts
        fortios_facts:
          host:  "{{ host }}"
          username: "{{ username }}"
          password: "{{ password }}"
          vdom:  "{{ vdom }}"
          gather_subset:
            - fact: 'system_interface_select'
              filters:
                - include_vlan: true
    
      - name: gather basic system info and physical interface port3 status facts
        fortios_facts:
          host:  "{{ host }}"
          username: "{{ username }}"
          password: "{{ password }}"
          vdom:  "{{ vdom }}"
          gather_subset:
            - fact: 'system_status_select'
            - fact: 'system_interface_select'
              filters:
                - interface_name: 'port3'


Return Values
-------------
Common return values are documented: https://docs.ansible.com/ansible/latest/reference_appendices/common_return_values.html#common-return-values, the following are the fields unique to this module:

.. raw:: html

    <ul>

    <li> <span class="li-return">build</span> - Build number of the fortigate image <span class="li-normal">returned: always</span> <span class="li-normal">type: str</span> <span class="li-normal">sample: 1547</span></li>
    <li> <span class="li-return">http_method</span> - Last method used to provision the content into FortiGate <span class="li-normal">returned: always</span> <span class="li-normal">type: str</span> <span class="li-normal">sample: GET</span></li>
    <li> <span class="li-return">name</span> - Name of the table used to fulfill the request <span class="li-normal">returned: always</span> <span class="li-normal">type: str</span> <span class="li-normal">sample: firmware</span></li>
    <li> <span class="li-return">path</span> - Path of the table used to fulfill the request <span class="li-normal">returned: always</span> <span class="li-normal">type: str</span> <span class="li-normal">sample: system</span></li>
    <li> <span class="li-return">revision</span> - Internal revision number <span class="li-normal">returned: always</span> <span class="li-normal">type: str</span> <span class="li-normal">sample: 17.0.2.10658</span></li>
    <li> <span class="li-return">serial</span> - Serial number of the unit <span class="li-normal">returned: always</span> <span class="li-normal">type: str</span> <span class="li-normal">sample: FGVMEVYYQT3AB5352</span></li>
    <li> <span class="li-return">status</span> - Indication of the operation's result <span class="li-normal">returned: always</span> <span class="li-normal">type: str</span> <span class="li-normal">sample: success</span></li>
    <li> <span class="li-return">vdom</span> - Virtual domain used <span class="li-normal">returned: always</span> <span class="li-normal">type: str</span> <span class="li-normal">sample: root</span></li>
    <li> <span class="li-return">version</span> - Version of the FortiGate <span class="li-normal">returned: always</span> <span class="li-normal">type: str</span> <span class="li-normal">sample: v5.6.3</span></li>
    <li> <span class="li-return">ansible_facts</span> - The list of fact subsets collected from the device <span class="li-normal">returned: always</span> <span class="li-normal">type: dict</span></li>
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
