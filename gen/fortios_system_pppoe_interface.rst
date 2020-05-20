:source: fortios_system_pppoe_interface.py

:orphan:

.. fortios_system_pppoe_interface:

fortios_system_pppoe_interface -- Configure the PPPoE interfaces in Fortinet's FortiOS and FortiGate.
+++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++

.. versionadded:: 2.9

.. contents::
   :local:
   :depth: 1


Synopsis
--------
- This module is able to configure a FortiGate or FortiOS (FOS) device by allowing the user to set and modify system feature and pppoe_interface category. Examples include all parameters and values need to be adjusted to datasources before usage. Tested with FOS v6.0.5



Requirements
------------
The below requirements are needed on the host that executes this module.

- ansible>=2.9.0


Parameters
----------


.. raw:: html

    <ul>
    <li> <span class="li-head">host</span> - FortiOS or FortiGate IP address. <span class="li-normal">type: str</span> <span class="li-required">required: False</span></li>
    <li> <span class="li-head">username</span> - FortiOS or FortiGate username. <span class="li-normal">type: str</span> <span class="li-required">required: False</span></li>
    <li> <span class="li-head">password</span> - FortiOS or FortiGate password. <span class="li-normal">type: str</span> <span class="li-normal">default: </span></li>
    <li> <span class="li-head">vdom</span> - Virtual domain, among those defined previously. A vdom is a virtual instance of the FortiGate that can be configured and used as a different unit. <span class="li-normal">type: str</span> <span class="li-normal">default: root</span></li>
    <li> <span class="li-head">https</span> - Indicates if the requests towards FortiGate must use HTTPS protocol. <span class="li-normal">type: bool</span> <span class="li-normal">default: True</span></li>
    <li> <span class="li-head">ssl_verify</span> - Ensures FortiGate certificate must be verified by a proper CA. <span class="li-normal">type: bool</span> <span class="li-normal">default: True</span></li>
    <li> <span class="li-head">state</span> - Indicates whether to create or remove the object. <span class="li-normal">type: str</span> <span class="li-required">required: True</span> <span class="li-normal">choices: present, absent</span></li>
    <li> <span class="li-head">system_pppoe_interface</span> - Configure the PPPoE interfaces. <span class="li-normal">type: dict</span></li>
        <ul class="ul-self">
        <li> <span class="li-head">ac_name</span> - PPPoE AC name. <span class="li-normal">type: str</span></li>
        <li> <span class="li-head">auth_type</span> - PPP authentication type to use. <span class="li-normal">type: str</span> <span class="li-normal">choices: auto, pap, chap, mschapv1, mschapv2</span></li>
        <li> <span class="li-head">device</span> - Name for the physical interface. Source system.interface.name. <span class="li-normal">type: str</span></li>
        <li> <span class="li-head">dial_on_demand</span> - Enable/disable dial on demand to dial the PPPoE interface when packets are routed to the PPPoE interface. <span class="li-normal">type: str</span> <span class="li-normal">choices: enable, disable</span></li>
        <li> <span class="li-head">disc_retry_timeout</span> - PPPoE discovery init timeout value in (0-4294967295 sec). <span class="li-normal">type: int</span></li>
        <li> <span class="li-head">idle_timeout</span> - PPPoE auto disconnect after idle timeout (0-4294967295 sec). <span class="li-normal">type: int</span></li>
        <li> <span class="li-head">ipunnumbered</span> - PPPoE unnumbered IP. <span class="li-normal">type: str</span></li>
        <li> <span class="li-head">ipv6</span> - Enable/disable IPv6 Control Protocol (IPv6CP). <span class="li-normal">type: str</span> <span class="li-normal">choices: enable, disable</span></li>
        <li> <span class="li-head">lcp_echo_interval</span> - PPPoE LCP echo interval in (0-4294967295 sec). <span class="li-normal">type: int</span></li>
        <li> <span class="li-head">lcp_max_echo_fails</span> - Maximum missed LCP echo messages before disconnect (0-4294967295). <span class="li-normal">type: int</span></li>
        <li> <span class="li-head">name</span> - Name of the PPPoE interface. <span class="li-normal">type: str</span> <span class="li-required">required: True</span></li>
        <li> <span class="li-head">padt_retry_timeout</span> - PPPoE terminate timeout value in (0-4294967295 sec). <span class="li-normal">type: int</span></li>
        <li> <span class="li-head">password</span> - Enter the password. <span class="li-normal">type: str</span></li>
        <li> <span class="li-head">pppoe_unnumbered_negotiate</span> - Enable/disable PPPoE unnumbered negotiation. <span class="li-normal">type: str</span> <span class="li-normal">choices: enable, disable</span></li>
        <li> <span class="li-head">service_name</span> - PPPoE service name. <span class="li-normal">type: str</span></li>
        <li> <span class="li-head">username</span> - User name. <span class="li-normal">type: str</span></li>
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
      - name: Configure the PPPoE interfaces.
        fortios_system_pppoe_interface:
          vdom:  "{{ vdom }}"
          state: "present"
          system_pppoe_interface:
            ac_name: "<your_own_value>"
            auth_type: "auto"
            device: "<your_own_value> (source system.interface.name)"
            dial_on_demand: "enable"
            disc_retry_timeout: "7"
            idle_timeout: "8"
            ipunnumbered: "<your_own_value>"
            ipv6: "enable"
            lcp_echo_interval: "11"
            lcp_max_echo_fails: "12"
            name: "default_name_13"
            padt_retry_timeout: "14"
            password: "<your_own_value>"
            pppoe_unnumbered_negotiate: "enable"
            service_name: "<your_own_value>"
            username: "<your_own_value>"


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
