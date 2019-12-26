:source: fortios_user_fsso.py

:orphan:

.. _fortios_user_fsso:

fortios_user_fsso -- Configure Fortinet Single Sign On (FSSO) agents in Fortinet's FortiOS and FortiGate.
+++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++

.. versionadded:: 2.9

.. contents::
   :local:
   :depth: 1


Synopsis
--------
- This module is able to configure a FortiGate or FortiOS (FOS) device by allowing the user to set and modify user feature and fsso category. Examples include all parameters and values need to be adjusted to datasources before usage. Tested with FOS v6.0.5


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
    <li><span class="li-head">user_fsso</span> - Configure Fortinet Single Sign On (FSSO) agents. <span class="li-normal">default: null</span> <span class="li-normal">type: dict</span></li>
            <ul class="ul-self">

            <li><span class="li-head">ldap_server</span> - LDAP server to get group information. Source user.ldap.name. <span class="li-normal">type: str</span></li>
            <li><span class="li-head">name</span> - Name. <span class="li-required">required</span> <span class="li-normal">type: str</span></li>
            <li><span class="li-head">password</span> - Password of the first FSSO collector agent. <span class="li-normal">type: str</span></li>
            <li><span class="li-head">password2</span> - Password of the second FSSO collector agent. <span class="li-normal">type: str</span></li>
            <li><span class="li-head">password3</span> - Password of the third FSSO collector agent. <span class="li-normal">type: str</span></li>
            <li><span class="li-head">password4</span> - Password of the fourth FSSO collector agent. <span class="li-normal">type: str</span></li>
            <li><span class="li-head">password5</span> - Password of the fifth FSSO collector agent. <span class="li-normal">type: str</span></li>
            <li><span class="li-head">port</span> - Port of the first FSSO collector agent. <span class="li-normal">type: int</span></li>
            <li><span class="li-head">port2</span> - Port of the second FSSO collector agent. <span class="li-normal">type: int</span></li>
            <li><span class="li-head">port3</span> - Port of the third FSSO collector agent. <span class="li-normal">type: int</span></li>
            <li><span class="li-head">port4</span> - Port of the fourth FSSO collector agent. <span class="li-normal">type: int</span></li>
            <li><span class="li-head">port5</span> - Port of the fifth FSSO collector agent. <span class="li-normal">type: int</span></li>
            <li><span class="li-head">server</span> - Domain name or IP address of the first FSSO collector agent. <span class="li-normal">type: str</span></li>
            <li><span class="li-head">server2</span> - Domain name or IP address of the second FSSO collector agent. <span class="li-normal">type: str</span></li>
            <li><span class="li-head">server3</span> - Domain name or IP address of the third FSSO collector agent. <span class="li-normal">type: str</span></li>
            <li><span class="li-head">server4</span> - Domain name or IP address of the fourth FSSO collector agent. <span class="li-normal">type: str</span></li>
            <li><span class="li-head">server5</span> - Domain name or IP address of the fifth FSSO collector agent. <span class="li-normal">type: str</span></li>
            <li><span class="li-head">source_ip</span> - Source IP for communications to FSSO agent. <span class="li-normal">type: str</span></li>
            <li><span class="li-head">source_ip6</span> - IPv6 source for communications to FSSO agent. <span class="li-normal">type: str</span>
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
      - name: Configure Fortinet Single Sign On (FSSO) agents.
        fortios_user_fsso:
          host:  "{{ host }}"
          username: "{{ username }}"
          password: "{{ password }}"
          vdom:  "{{ vdom }}"
          https: "False"
          state: "present"
          user_fsso:
            ldap_server: "<your_own_value> (source user.ldap.name)"
            name: "default_name_4"
            password: "<your_own_value>"
            password2: "<your_own_value>"
            password3: "<your_own_value>"
            password4: "<your_own_value>"
            password5: "<your_own_value>"
            port: "10"
            port2: "11"
            port3: "12"
            port4: "13"
            port5: "14"
            server: "192.168.100.40"
            server2: "<your_own_value>"
            server3: "<your_own_value>"
            server4: "<your_own_value>"
            server5: "<your_own_value>"
            source_ip: "84.230.14.43"
            source_ip6: "<your_own_value>"



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