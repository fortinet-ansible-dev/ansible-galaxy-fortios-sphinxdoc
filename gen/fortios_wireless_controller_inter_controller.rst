:source: fortios_wireless_controller_inter_controller.py

:orphan:

.. fortios_wireless_controller_inter_controller:

fortios_wireless_controller_inter_controller -- Configure inter wireless controller operation in Fortinet's FortiOS and FortiGate.
++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++

.. versionadded:: 2.9

.. contents::
   :local:
   :depth: 1


Synopsis
--------
- This module is able to configure a FortiGate or FortiOS (FOS) device by allowing the user to set and modify wireless_controller feature and inter_controller category. Examples include all parameters and values need to be adjusted to datasources before usage. Tested with FOS v6.4.0



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
    <li> <span class="li-head">wireless_controller_inter_controller</span> - Configure inter wireless controller operation. <span class="li-normal">type: dict</span></li>
        <ul class="ul-self">
        <li> <span class="li-head">fast_failover_max</span> - Maximum number of retransmissions for fast failover HA messages between peer wireless controllers (3 - 64). <span class="li-normal">type: int</span></li>
        <li> <span class="li-head">fast_failover_wait</span> - Minimum wait time before an AP transitions from secondary controller to primary controller (10 - 86400 sec). <span class="li-normal">type: int</span></li>
        <li> <span class="li-head">inter_controller_key</span> - Secret key for inter-controller communications. <span class="li-normal">type: str</span></li>
        <li> <span class="li-head">inter_controller_mode</span> - Configure inter-controller mode (disable, l2-roaming, 1+1). <span class="li-normal">type: str</span> <span class="li-normal">choices: disable, l2-roaming, 1+1</span></li>
        <li> <span class="li-head">inter_controller_peer</span> - Fast failover peer wireless controller list. <span class="li-normal">type: list</span></li>
            <ul class="ul-self">
            <li> <span class="li-head">id</span> - ID. <span class="li-normal">type: int</span> <span class="li-required">required: True</span></li>
            <li> <span class="li-head">peer_ip</span> - Peer wireless controller"s IP address. <span class="li-normal">type: str</span></li>
            <li> <span class="li-head">peer_port</span> - Port used by the wireless controller"s for inter-controller communications (1024 - 49150). <span class="li-normal">type: int</span></li>
            <li> <span class="li-head">peer_priority</span> - Peer wireless controller"s priority (primary or secondary). <span class="li-normal">type: str</span> <span class="li-normal">choices: primary, secondary</span></li>
            </ul>
        <li> <span class="li-head">inter_controller_pri</span> - Configure inter-controller"s priority (primary or secondary). <span class="li-normal">type: str</span> <span class="li-normal">choices: primary, secondary</span></li>
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
      - name: Configure inter wireless controller operation.
        fortios_wireless_controller_inter_controller:
          vdom:  "{{ vdom }}"
          wireless_controller_inter_controller:
            fast_failover_max: "3"
            fast_failover_wait: "4"
            inter_controller_key: "<your_own_value>"
            inter_controller_mode: "disable"
            inter_controller_peer:
             -
                id:  "8"
                peer_ip: "<your_own_value>"
                peer_port: "10"
                peer_priority: "primary"
            inter_controller_pri: "primary"
    


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
