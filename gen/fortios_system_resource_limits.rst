:source: fortios_system_resource_limits.py

:orphan:

.. fortios_system_resource_limits:

fortios_system_resource_limits -- Configure resource limits in Fortinet's FortiOS and FortiGate.
++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++

.. versionadded:: 2.9

.. contents::
   :local:
   :depth: 1


Synopsis
--------
- This module is able to configure a FortiGate or FortiOS (FOS) device by allowing the user to set and modify system feature and resource_limits category. Examples include all parameters and values need to be adjusted to datasources before usage. Tested with FOS v6.4.0



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
    <li> <span class="li-head">system_resource_limits</span> - Configure resource limits. <span class="li-normal">type: dict</span></li>
        <ul class="ul-self">
        <li> <span class="li-head">custom_service</span> - Maximum number of firewall custom services. <span class="li-normal">type: int</span></li>
        <li> <span class="li-head">dialup_tunnel</span> - Maximum number of dial-up tunnels. <span class="li-normal">type: int</span></li>
        <li> <span class="li-head">firewall_address</span> - Maximum number of firewall addresses (IPv4, IPv6, multicast). <span class="li-normal">type: int</span></li>
        <li> <span class="li-head">firewall_addrgrp</span> - Maximum number of firewall address groups (IPv4, IPv6). <span class="li-normal">type: int</span></li>
        <li> <span class="li-head">firewall_policy</span> - Maximum number of firewall policies (policy, policy46, policy64, DoS-policy4, DoS-policy6, multicast). <span class="li-normal">type: int</span></li>
        <li> <span class="li-head">ipsec_phase1</span> - Maximum number of VPN IPsec phase1 tunnels. <span class="li-normal">type: int</span></li>
        <li> <span class="li-head">ipsec_phase1_interface</span> - Maximum number of VPN IPsec phase1 interface tunnels. <span class="li-normal">type: int</span></li>
        <li> <span class="li-head">ipsec_phase2</span> - Maximum number of VPN IPsec phase2 tunnels. <span class="li-normal">type: int</span></li>
        <li> <span class="li-head">ipsec_phase2_interface</span> - Maximum number of VPN IPsec phase2 interface tunnels. <span class="li-normal">type: int</span></li>
        <li> <span class="li-head">log_disk_quota</span> - Log disk quota in MB. <span class="li-normal">type: int</span></li>
        <li> <span class="li-head">onetime_schedule</span> - Maximum number of firewall one-time schedules. <span class="li-normal">type: int</span></li>
        <li> <span class="li-head">proxy</span> - Maximum number of concurrent proxy users. <span class="li-normal">type: int</span></li>
        <li> <span class="li-head">recurring_schedule</span> - Maximum number of firewall recurring schedules. <span class="li-normal">type: int</span></li>
        <li> <span class="li-head">service_group</span> - Maximum number of firewall service groups. <span class="li-normal">type: int</span></li>
        <li> <span class="li-head">session</span> - Maximum number of sessions. <span class="li-normal">type: int</span></li>
        <li> <span class="li-head">sslvpn</span> - Maximum number of SSL-VPN. <span class="li-normal">type: int</span></li>
        <li> <span class="li-head">user</span> - Maximum number of local users. <span class="li-normal">type: int</span></li>
        <li> <span class="li-head">user_group</span> - Maximum number of user groups. <span class="li-normal">type: int</span></li>
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
      - name: Configure resource limits.
        fortios_system_resource_limits:
          vdom:  "{{ vdom }}"
          system_resource_limits:
            custom_service: "3"
            dialup_tunnel: "4"
            firewall_address: "5"
            firewall_addrgrp: "6"
            firewall_policy: "7"
            ipsec_phase1: "8"
            ipsec_phase1_interface: "9"
            ipsec_phase2: "10"
            ipsec_phase2_interface: "11"
            log_disk_quota: "12"
            onetime_schedule: "13"
            proxy: "14"
            recurring_schedule: "15"
            service_group: "16"
            session: "17"
            sslvpn: "18"
            user: "19"
            user_group: "20"


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
