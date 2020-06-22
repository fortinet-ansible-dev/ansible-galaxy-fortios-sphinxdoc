:source: fortios_system_mobile_tunnel.py

:orphan:

.. fortios_system_mobile_tunnel:

fortios_system_mobile_tunnel -- Configure Mobile tunnels, an implementation of Network Mobility (NEMO) extensions for Mobile IPv4 RFC5177 in Fortinet's FortiOS and FortiGate.
++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++

.. versionadded:: 2.9

.. contents::
   :local:
   :depth: 1


Synopsis
--------
- This module is able to configure a FortiGate or FortiOS (FOS) device by allowing the user to set and modify system feature and mobile_tunnel category. Examples include all parameters and values need to be adjusted to datasources before usage. Tested with FOS v6.4.0



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
    <li> <span class="li-head">system_mobile_tunnel</span> - Configure Mobile tunnels, an implementation of Network Mobility (NEMO) extensions for Mobile IPv4 RFC5177. <span class="li-normal">type: dict</span></li>
        <ul class="ul-self">
        <li> <span class="li-head">hash_algorithm</span> - Hash Algorithm (Keyed MD5). <span class="li-normal">type: str</span> <span class="li-normal">choices: hmac-md5</span></li>
        <li> <span class="li-head">home_address</span> - Home IP address (Format: xxx.xxx.xxx.xxx). <span class="li-normal">type: str</span></li>
        <li> <span class="li-head">home_agent</span> - IPv4 address of the NEMO HA (Format: xxx.xxx.xxx.xxx). <span class="li-normal">type: str</span></li>
        <li> <span class="li-head">lifetime</span> - NMMO HA registration request lifetime (180 - 65535 sec). <span class="li-normal">type: int</span></li>
        <li> <span class="li-head">n_mhae_key</span> - NEMO authentication key. <span class="li-normal">type: str</span></li>
        <li> <span class="li-head">n_mhae_key_type</span> - NEMO authentication key type (ascii or base64). <span class="li-normal">type: str</span> <span class="li-normal">choices: ascii, base64</span></li>
        <li> <span class="li-head">n_mhae_spi</span> - NEMO authentication SPI . <span class="li-normal">type: int</span></li>
        <li> <span class="li-head">name</span> - Tunnel name. <span class="li-normal">type: str</span> <span class="li-required">required: True</span></li>
        <li> <span class="li-head">network</span> - NEMO network configuration. <span class="li-normal">type: list</span></li>
            <ul class="ul-self">
            <li> <span class="li-head">id</span> - Network entry ID. <span class="li-normal">type: int</span> <span class="li-required">required: True</span></li>
            <li> <span class="li-head">interface</span> - Select the associated interface name from available options. Source system.interface.name. <span class="li-normal">type: str</span></li>
            <li> <span class="li-head">prefix</span> - Class IP and Netmask with correction (Format:xxx.xxx.xxx.xxx xxx.xxx.xxx.xxx or xxx.xxx.xxx.xxx/x). <span class="li-normal">type: str</span></li>
            </ul>
        <li> <span class="li-head">reg_interval</span> - NMMO HA registration interval (5 - 300). <span class="li-normal">type: int</span></li>
        <li> <span class="li-head">reg_retry</span> - Maximum number of NMMO HA registration retries (1 to 30). <span class="li-normal">type: int</span></li>
        <li> <span class="li-head">renew_interval</span> - Time before lifetime expiraton to send NMMO HA re-registration (5 - 60). <span class="li-normal">type: int</span></li>
        <li> <span class="li-head">roaming_interface</span> - Select the associated interface name from available options. Source system.interface.name. <span class="li-normal">type: str</span></li>
        <li> <span class="li-head">status</span> - Enable/disable this mobile tunnel. <span class="li-normal">type: str</span> <span class="li-normal">choices: disable, enable</span></li>
        <li> <span class="li-head">tunnel_mode</span> - NEMO tunnnel mode (GRE tunnel). <span class="li-normal">type: str</span> <span class="li-normal">choices: gre</span></li>
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
      - name: Configure Mobile tunnels, an implementation of Network Mobility (NEMO) extensions for Mobile IPv4 RFC5177.
        fortios_system_mobile_tunnel:
          vdom:  "{{ vdom }}"
          state: "present"
          system_mobile_tunnel:
            hash_algorithm: "hmac-md5"
            home_address: "<your_own_value>"
            home_agent: "<your_own_value>"
            lifetime: "6"
            n_mhae_key: "<your_own_value>"
            n_mhae_key_type: "ascii"
            n_mhae_spi: "9"
            name: "default_name_10"
            network:
             -
                id:  "12"
                interface: "<your_own_value> (source system.interface.name)"
                prefix: "<your_own_value>"
            reg_interval: "15"
            reg_retry: "16"
            renew_interval: "17"
            roaming_interface: "<your_own_value> (source system.interface.name)"
            status: "disable"
            tunnel_mode: "gre"


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
