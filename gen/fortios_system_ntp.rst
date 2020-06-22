:source: fortios_system_ntp.py

:orphan:

.. fortios_system_ntp:

fortios_system_ntp -- Configure system NTP information in Fortinet's FortiOS and FortiGate.
+++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++

.. versionadded:: 2.9

.. contents::
   :local:
   :depth: 1


Synopsis
--------
- This module is able to configure a FortiGate or FortiOS (FOS) device by allowing the user to set and modify system feature and ntp category. Examples include all parameters and values need to be adjusted to datasources before usage. Tested with FOS v6.4.0



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
    <li> <span class="li-head">system_ntp</span> - Configure system NTP information. <span class="li-normal">type: dict</span></li>
        <ul class="ul-self">
        <li> <span class="li-head">authentication</span> - Enable/disable authentication. <span class="li-normal">type: str</span> <span class="li-normal">choices: enable, disable</span></li>
        <li> <span class="li-head">interface</span> - FortiGate interface(s) with NTP server mode enabled. Devices on your network can contact these interfaces for NTP services. <span class="li-normal">type: list</span></li>
            <ul class="ul-self">
            <li> <span class="li-head">interface_name</span> - Interface name. Source system.interface.name. <span class="li-normal">type: str</span></li>
            </ul>
        <li> <span class="li-head">key</span> - Key for authentication. <span class="li-normal">type: str</span></li>
        <li> <span class="li-head">key_id</span> - Key ID for authentication. <span class="li-normal">type: int</span></li>
        <li> <span class="li-head">key_type</span> - Key type for authentication (MD5, SHA1). <span class="li-normal">type: str</span> <span class="li-normal">choices: MD5, SHA1</span></li>
        <li> <span class="li-head">ntpserver</span> - Configure the FortiGate to connect to any available third-party NTP server. <span class="li-normal">type: list</span></li>
            <ul class="ul-self">
            <li> <span class="li-head">authentication</span> - Enable/disable MD5(NTPv3)/SHA1(NTPv4) authentication. <span class="li-normal">type: str</span> <span class="li-normal">choices: enable, disable</span></li>
            <li> <span class="li-head">id</span> - NTP server ID. <span class="li-normal">type: int</span> <span class="li-required">required: True</span></li>
            <li> <span class="li-head">key</span> - Key for MD5(NTPv3)/SHA1(NTPv4) authentication. <span class="li-normal">type: str</span></li>
            <li> <span class="li-head">key_id</span> - Key ID for authentication. <span class="li-normal">type: int</span></li>
            <li> <span class="li-head">ntpv3</span> - Enable to use NTPv3 instead of NTPv4. <span class="li-normal">type: str</span> <span class="li-normal">choices: enable, disable</span></li>
            <li> <span class="li-head">server</span> - IP address or hostname of the NTP Server. <span class="li-normal">type: str</span></li>
            </ul>
        <li> <span class="li-head">ntpsync</span> - Enable/disable setting the FortiGate system time by synchronizing with an NTP Server. <span class="li-normal">type: str</span> <span class="li-normal">choices: enable, disable</span></li>
        <li> <span class="li-head">server_mode</span> - Enable/disable FortiGate NTP Server Mode. Your FortiGate becomes an NTP server for other devices on your network. The FortiGate relays NTP requests to its configured NTP server. <span class="li-normal">type: str</span> <span class="li-normal">choices: enable, disable</span></li>
        <li> <span class="li-head">source_ip</span> - Source IP address for communication to the NTP server. <span class="li-normal">type: str</span></li>
        <li> <span class="li-head">source_ip6</span> - Source IPv6 address for communication to the NTP server. <span class="li-normal">type: str</span></li>
        <li> <span class="li-head">syncinterval</span> - NTP synchronization interval (1 - 1440 min). <span class="li-normal">type: int</span></li>
        <li> <span class="li-head">type</span> - Use the FortiGuard NTP server or any other available NTP Server. <span class="li-normal">type: str</span> <span class="li-normal">choices: fortiguard, custom</span></li>
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
      - name: Configure system NTP information.
        fortios_system_ntp:
          vdom:  "{{ vdom }}"
          system_ntp:
            authentication: "enable"
            interface:
             -
                interface_name: "<your_own_value> (source system.interface.name)"
            key: "<your_own_value>"
            key_id: "7"
            key_type: "MD5"
            ntpserver:
             -
                authentication: "enable"
                id:  "11"
                key: "<your_own_value>"
                key_id: "13"
                ntpv3: "enable"
                server: "192.168.100.40"
            ntpsync: "enable"
            server_mode: "enable"
            source_ip: "84.230.14.43"
            source_ip6: "<your_own_value>"
            syncinterval: "20"
            type: "fortiguard"


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
