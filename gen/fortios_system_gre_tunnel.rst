:source: fortios_system_gre_tunnel.py

:orphan:

.. _fortios_system_gre_tunnel:

fortios_system_gre_tunnel -- Configure GRE tunnel in Fortinet's FortiOS and FortiGate.
++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++

.. versionadded:: 2.9

.. contents::
   :local:
   :depth: 1


Synopsis
--------
- This module is able to configure a FortiGate or FortiOS (FOS) device by allowing the user to set and modify system feature and gre_tunnel category. Examples include all parameters and values need to be adjusted to datasources before usage. Tested with FOS v6.0.5


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
    <li><span class="li-head">state</span> - Indicates whether to create or remove the object. <span class="li-normal">type: str</span> <span class="li-required">required</span> <span class="li-normal">choices: present,  absent</span></li>
    <li><span class="li-head">system_gre_tunnel</span> - Configure GRE tunnel. <span class="li-normal">default: null</span> <span class="li-normal">type: dict</span></li>
            <ul class="ul-self">

            <li><span class="li-head">checksum_reception</span> - Enable/disable validating checksums in received GRE packets. <span class="li-normal">type: str</span> <span class="li-normal">choices: disable,  enable</span></li>
            <li><span class="li-head">checksum_transmission</span> - Enable/disable including checksums in transmitted GRE packets. <span class="li-normal">type: str</span> <span class="li-normal">choices: disable,  enable</span></li>
            <li><span class="li-head">dscp_copying</span> - Enable/disable DSCP copying. <span class="li-normal">type: str</span> <span class="li-normal">choices: disable,  enable</span></li>
            <li><span class="li-head">interface</span> - Interface name. Source system.interface.name. <span class="li-normal">type: str</span></li>
            <li><span class="li-head">ip_version</span> - IP version to use for VPN interface. <span class="li-normal">type: str</span> <span class="li-normal">choices: 4,  6</span></li>
            <li><span class="li-head">keepalive_failtimes</span> - Number of consecutive unreturned keepalive messages before a GRE connection is considered down (1 - 255). <span class="li-normal">type: int</span></li>
            <li><span class="li-head">keepalive_interval</span> - Keepalive message interval (0 - 32767, 0 = disabled). <span class="li-normal">type: int</span></li>
            <li><span class="li-head">key_inbound</span> - Require received GRE packets contain this key (0 - 4294967295). <span class="li-normal">type: int</span></li>
            <li><span class="li-head">key_outbound</span> - Include this key in transmitted GRE packets (0 - 4294967295). <span class="li-normal">type: int</span></li>
            <li><span class="li-head">local_gw</span> - IP address of the local gateway. <span class="li-normal">type: str</span></li>
            <li><span class="li-head">local_gw6</span> - IPv6 address of the local gateway. <span class="li-normal">type: str</span></li>
            <li><span class="li-head">name</span> - Tunnel name. <span class="li-required">required</span> <span class="li-normal">type: str</span></li>
            <li><span class="li-head">remote_gw</span> - IP address of the remote gateway. <span class="li-normal">type: str</span></li>
            <li><span class="li-head">remote_gw6</span> - IPv6 address of the remote gateway. <span class="li-normal">type: str</span></li>
            <li><span class="li-head">sequence_number_reception</span> - Enable/disable validating sequence numbers in received GRE packets. <span class="li-normal">type: str</span> <span class="li-normal">choices: disable,  enable</span></li>
            <li><span class="li-head">sequence_number_transmission</span> - Enable/disable including of sequence numbers in transmitted GRE packets. <span class="li-normal">type: str</span> <span class="li-normal">choices: disable,  enable</span>
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
      - name: Configure GRE tunnel.
        fortios_system_gre_tunnel:
          host:  "{{ host }}"
          username: "{{ username }}"
          password: "{{ password }}"
          vdom:  "{{ vdom }}"
          https: "False"
          state: "present"
          system_gre_tunnel:
            checksum_reception: "disable"
            checksum_transmission: "disable"
            dscp_copying: "disable"
            interface: "<your_own_value> (source system.interface.name)"
            ip_version: "4"
            keepalive_failtimes: "8"
            keepalive_interval: "9"
            key_inbound: "10"
            key_outbound: "11"
            local_gw: "<your_own_value>"
            local_gw6: "<your_own_value>"
            name: "default_name_14"
            remote_gw: "<your_own_value>"
            remote_gw6: "<your_own_value>"
            sequence_number_reception: "disable"
            sequence_number_transmission: "disable"



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