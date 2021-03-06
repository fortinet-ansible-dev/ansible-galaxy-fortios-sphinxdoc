:source: fortios_firewall_internet_service_custom.py

:orphan:

.. _fortios_firewall_internet_service_custom:

fortios_firewall_internet_service_custom -- Configure custom Internet Services in Fortinet's FortiOS and FortiGate.
+++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++

.. versionadded:: 2.8

.. contents::
   :local:
   :depth: 1


Synopsis
--------
- This module is able to configure a FortiGate or FortiOS (FOS) device by allowing the user to set and modify firewall feature and internet_service_custom category. Examples include all parameters and values need to be adjusted to datasources before usage. Tested with FOS v6.0.5


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
    <li><span class="li-head">vdom</span> - Virtual domain, among those defined previously. A vdom is a virtual instance of the FortiGate that can be configured and used as a different unit. <span class="li-normal">type: str</span> <span class="li-normal">default: root</span></li>
    <li><span class="li-head">https</span> - Indicates if the requests towards FortiGate must use HTTPS protocol. <span class="li-normal">type: bool</span> <span class="li-normal">default: true</span></li>
    <li><span class="li-head">ssl_verify</span> - Ensures FortiGate certificate must be verified by a proper CA. <span class="li-normal">type: bool</span> <span class="li-normal">default: true</span></li>
    <li><span class="li-head">state</span> - Indicates whether to create or remove the object. This attribute was present already in previous version in a deeper level. It has been moved out to this outer level. <span class="li-normal">type: str</span> <span class="li-required">required: false</span> <span class="li-normal">choices: present,  absent</span></li>
    <li><span class="li-head">firewall_internet_service_custom</span> - Configure custom Internet Services. <span class="li-normal">default: null</span> <span class="li-normal">type: dict</span></li>
            <ul class="ul-self">

            <li><span class="li-head">state</span> - B(Deprecated) Starting with Ansible 2.9 we recommend using the top-level 'state' parameter. HORIZONTALLINE Indicates whether to create or remove the object. <span class="li-normal">type: str</span> <span class="li-required">required: false</span> <span class="li-normal">choices: present,  absent</span></li>
            <li><span class="li-head">comment</span> - Comment. <span class="li-normal">type: str</span></li>
            <li><span class="li-head">disable_entry</span> - Disable entries in the Internet Service database. <span class="li-normal">type: list</span></li>
                    <ul class="ul-self">

                    <li><span class="li-head">id</span> - Disable entry ID. <span class="li-required">required</span> <span class="li-normal">type: int</span></li>
                    <li><span class="li-head">ip_range</span> - IP ranges in the disable entry. <span class="li-normal">type: list</span></li>
                            <ul class="ul-self">

                            <li><span class="li-head">end_ip</span> - End IP address. <span class="li-normal">type: str</span></li>
                            <li><span class="li-head">id</span> - Disable entry range ID. <span class="li-required">required</span> <span class="li-normal">type: int</span></li>
                            <li><span class="li-head">start_ip</span> - Start IP address. <span class="li-normal">type: str</span>
                            </ul>

                    <li><span class="li-head">port</span> - Integer value for the TCP/IP port (0 - 65535). <span class="li-normal">type: int</span></li>
                    <li><span class="li-head">protocol</span> - Integer value for the protocol type as defined by IANA (0 - 255). <span class="li-normal">type: int</span>
                    </ul>

            <li><span class="li-head">entry</span> - Entries added to the Internet Service database and custom database. <span class="li-normal">type: list</span></li>
                    <ul class="ul-self">

                    <li><span class="li-head">dst</span> - Destination address or address group name. <span class="li-normal">type: list</span></li>
                            <ul class="ul-self">

                            <li><span class="li-head">name</span> - Select the destination address or address group object from available options. Source firewall.address.name firewall .addrgrp.name. <span class="li-required">required</span> <span class="li-normal">type: str</span>
                            </ul>

                    <li><span class="li-head">id</span> - Entry ID(1-255). <span class="li-required">required</span> <span class="li-normal">type: int</span></li>
                    <li><span class="li-head">port_range</span> - Port ranges in the custom entry. <span class="li-normal">type: list</span></li>
                            <ul class="ul-self">

                            <li><span class="li-head">end_port</span> - Integer value for ending TCP/UDP/SCTP destination port in range (1 to 65535). <span class="li-normal">type: int</span></li>
                            <li><span class="li-head">id</span> - Custom entry port range ID. <span class="li-required">required</span> <span class="li-normal">type: int</span></li>
                            <li><span class="li-head">start_port</span> - Integer value for starting TCP/UDP/SCTP destination port in range (1 to 65535). <span class="li-normal">type: int</span>
                            </ul>

                    <li><span class="li-head">protocol</span> - Integer value for the protocol type as defined by IANA (0 - 255). <span class="li-normal">type: int</span>
                    </ul>

            <li><span class="li-head">master_service_id</span> - Internet Service ID in the Internet Service database. Source firewall.internet-service.id. <span class="li-normal">type: int</span></li>
            <li><span class="li-head">name</span> - Internet Service name. <span class="li-required">required</span> <span class="li-normal">type: str</span>
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
      - name: Configure custom Internet Services.
        fortios_firewall_internet_service_custom:
          host:  "{{ host }}"
          username: "{{ username }}"
          password: "{{ password }}"
          vdom:  "{{ vdom }}"
          https: "False"
          state: "present"
          firewall_internet_service_custom:
            comment: "Comment."
            disable_entry:
             -
                id:  "5"
                ip_range:
                 -
                    end_ip: "<your_own_value>"
                    id:  "8"
                    start_ip: "<your_own_value>"
                port: "10"
                protocol: "11"
            entry:
             -
                dst:
                 -
                    name: "default_name_14 (source firewall.address.name firewall.addrgrp.name)"
                id:  "15"
                port_range:
                 -
                    end_port: "17"
                    id:  "18"
                    start_port: "19"
                protocol: "20"
            master_service_id: "21 (source firewall.internet-service.id)"
            name: "default_name_22"



Return Values
-------------
Common return values are documented: https://docs.ansible.com/ansible/latest/reference_appendices/common_return_values.html#common-return-values, the following are the fields unique to this module:

.. raw:: html

    <ul>

    <li><span class="li-return">build</span> - Build number of the fortigate image <span class="li-normal">returned: always</span> <span class="li-normal">type: str</span> <span class="li-normal">sample: '1547'</span></li>
    <li><span class="li-return">http_method</span> - Last method used to provision the content into FortiGate <span class="li-normal">returned: always</span> <span class="li-normal">type: str</span> <span class="li-normal">sample: 'PUT'</span></li>
    <li><span class="li-return">http_status</span> - Last result given by FortiGate on last operation applied <span class="li-normal">returned: always</span> <span class="li-normal">type: str</span> <span class="li-normal">sample: 200</span></li>
    <li><span class="li-return">mkey</span> - Master key (id) used in the last call to FortiGate <span class="li-normal">returned: success</span> <span class="li-normal">type: str</span> <span class="li-normal">sample: id</span></li>
    <li><span class="li-return">name</span> - Name of the table used to fulfill the request <span class="li-normal">returned: always</span> <span class="li-normal">type: str</span> <span class="li-normal">sample: urlfilter</span></li>
    <li><span class="li-return">path</span> - Path of the table used to fulfill the request <span class="li-normal">returned: always</span> <span class="li-normal">type: str</span> <span class="li-normal">sample: webfilter</span></li>
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

- Miguel Angel Munoz (@mamunozgonzalez)
- Nicolas Thomas (@thomnico)



.. hint::
    If you notice any issues in this documentation, you can create a pull request to improve it.