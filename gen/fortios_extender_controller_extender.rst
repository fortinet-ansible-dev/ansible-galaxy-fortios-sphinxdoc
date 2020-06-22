:source: fortios_extender_controller_extender.py

:orphan:

.. fortios_extender_controller_extender:

fortios_extender_controller_extender -- Extender controller configuration in Fortinet's FortiOS and FortiGate.
++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++

.. versionadded:: 2.8

.. contents::
   :local:
   :depth: 1


Synopsis
--------
- This module is able to configure a FortiGate or FortiOS (FOS) device by allowing the user to set and modify extender_controller feature and extender category. Examples include all parameters and values need to be adjusted to datasources before usage. Tested with FOS v6.0.5



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
    <li> <span class="li-head">state</span> - Indicates whether to create or remove the object. This attribute was present already in previous version in a deeper level. It has been moved out to this outer level. <span class="li-normal">type: str</span> <span class="li-required">required: False</span> <span class="li-normal">choices: present, absent</span></li>
    <li> <span class="li-head">extender_controller_extender</span> - Extender controller configuration. <span class="li-normal">type: dict</span></li>
        <ul class="ul-self">
        <li> <span class="li-head">state</span> - B(Deprecated) <span class="li-normal">type: str</span> <span class="li-required">required: False</span> <span class="li-normal">choices: present, absent</span></li>
        <li> <span class="li-head">aaa_shared_secret</span> - AAA shared secret. <span class="li-normal">type: str</span></li>
        <li> <span class="li-head">access_point_name</span> - Access point name(APN). <span class="li-normal">type: str</span></li>
        <li> <span class="li-head">admin</span> - FortiExtender Administration (enable or disable). <span class="li-normal">type: str</span> <span class="li-normal">choices: disable, discovered, enable</span></li>
        <li> <span class="li-head">at_dial_script</span> - Initialization AT commands specific to the MODEM. <span class="li-normal">type: str</span></li>
        <li> <span class="li-head">billing_start_day</span> - Billing start day. <span class="li-normal">type: int</span></li>
        <li> <span class="li-head">cdma_aaa_spi</span> - CDMA AAA SPI. <span class="li-normal">type: str</span></li>
        <li> <span class="li-head">cdma_ha_spi</span> - CDMA HA SPI. <span class="li-normal">type: str</span></li>
        <li> <span class="li-head">cdma_nai</span> - NAI for CDMA MODEMS. <span class="li-normal">type: str</span></li>
        <li> <span class="li-head">conn_status</span> - Connection status. <span class="li-normal">type: int</span></li>
        <li> <span class="li-head">description</span> - Description. <span class="li-normal">type: str</span></li>
        <li> <span class="li-head">dial_mode</span> - Dial mode (dial-on-demand or always-connect). <span class="li-normal">type: str</span> <span class="li-normal">choices: dial-on-demand, always-connect</span></li>
        <li> <span class="li-head">dial_status</span> - Dial status. <span class="li-normal">type: int</span></li>
        <li> <span class="li-head">ext_name</span> - FortiExtender name. <span class="li-normal">type: str</span></li>
        <li> <span class="li-head">ha_shared_secret</span> - HA shared secret. <span class="li-normal">type: str</span></li>
        <li> <span class="li-head">id</span> - FortiExtender serial number. <span class="li-normal">type: str</span> <span class="li-required">required: True</span></li>
        <li> <span class="li-head">ifname</span> - FortiExtender interface name. <span class="li-normal">type: str</span></li>
        <li> <span class="li-head">initiated_update</span> - Allow/disallow network initiated updates to the MODEM. <span class="li-normal">type: str</span> <span class="li-normal">choices: enable, disable</span></li>
        <li> <span class="li-head">mode</span> - FortiExtender mode. <span class="li-normal">type: str</span> <span class="li-normal">choices: standalone, redundant</span></li>
        <li> <span class="li-head">modem_passwd</span> - MODEM password. <span class="li-normal">type: str</span></li>
        <li> <span class="li-head">modem_type</span> - MODEM type (CDMA, GSM/LTE or WIMAX). <span class="li-normal">type: str</span> <span class="li-normal">choices: cdma, gsm/lte, wimax</span></li>
        <li> <span class="li-head">multi_mode</span> - MODEM mode of operation(3G,LTE,etc). <span class="li-normal">type: str</span> <span class="li-normal">choices: auto, auto-3g, force-lte, force-3g, force-2g</span></li>
        <li> <span class="li-head">ppp_auth_protocol</span> - PPP authentication protocol (PAP,CHAP or auto). <span class="li-normal">type: str</span> <span class="li-normal">choices: auto, pap, chap</span></li>
        <li> <span class="li-head">ppp_echo_request</span> - Enable/disable PPP echo request. <span class="li-normal">type: str</span> <span class="li-normal">choices: enable, disable</span></li>
        <li> <span class="li-head">ppp_password</span> - PPP password. <span class="li-normal">type: str</span></li>
        <li> <span class="li-head">ppp_username</span> - PPP username. <span class="li-normal">type: str</span></li>
        <li> <span class="li-head">primary_ha</span> - Primary HA. <span class="li-normal">type: str</span></li>
        <li> <span class="li-head">quota_limit_mb</span> - Monthly quota limit (MB). <span class="li-normal">type: int</span></li>
        <li> <span class="li-head">redial</span> - Number of redials allowed based on failed attempts. <span class="li-normal">type: str</span> <span class="li-normal">choices: none, 1, 2, 3, 4, 5, 6, 7, 8, 9, 10</span></li>
        <li> <span class="li-head">redundant_intf</span> - Redundant interface. <span class="li-normal">type: str</span></li>
        <li> <span class="li-head">roaming</span> - Enable/disable MODEM roaming. <span class="li-normal">type: str</span> <span class="li-normal">choices: enable, disable</span></li>
        <li> <span class="li-head">role</span> - FortiExtender work role(Primary, Secondary, None). <span class="li-normal">type: str</span> <span class="li-normal">choices: none, primary, secondary</span></li>
        <li> <span class="li-head">secondary_ha</span> - Secondary HA. <span class="li-normal">type: str</span></li>
        <li> <span class="li-head">sim_pin</span> - SIM PIN. <span class="li-normal">type: str</span></li>
        <li> <span class="li-head">vdom</span> - VDOM <span class="li-normal">type: int</span></li>
        <li> <span class="li-head">wimax_auth_protocol</span> - WiMax authentication protocol(TLS or TTLS). <span class="li-normal">type: str</span> <span class="li-normal">choices: tls, ttls</span></li>
        <li> <span class="li-head">wimax_carrier</span> - WiMax carrier. <span class="li-normal">type: str</span></li>
        <li> <span class="li-head">wimax_realm</span> - WiMax realm. <span class="li-normal">type: str</span></li>
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
      - name: Extender controller configuration.
        fortios_extender_controller_extender:
          vdom:  "{{ vdom }}"
          state: "present"
          extender_controller_extender:
            aaa_shared_secret: "<your_own_value>"
            access_point_name: "<your_own_value>"
            admin: "disable"
            at_dial_script: "<your_own_value>"
            billing_start_day: "7"
            cdma_aaa_spi: "<your_own_value>"
            cdma_ha_spi: "<your_own_value>"
            cdma_nai: "<your_own_value>"
            conn_status: "11"
            description: "<your_own_value>"
            dial_mode: "dial-on-demand"
            dial_status: "14"
            ext_name: "<your_own_value>"
            ha_shared_secret: "<your_own_value>"
            id:  "17"
            ifname: "<your_own_value>"
            initiated_update: "enable"
            mode: "standalone"
            modem_passwd: "<your_own_value>"
            modem_type: "cdma"
            multi_mode: "auto"
            ppp_auth_protocol: "auto"
            ppp_echo_request: "enable"
            ppp_password: "<your_own_value>"
            ppp_username: "<your_own_value>"
            primary_ha: "<your_own_value>"
            quota_limit_mb: "29"
            redial: "none"
            redundant_intf: "<your_own_value>"
            roaming: "enable"
            role: "none"
            secondary_ha: "<your_own_value>"
            sim_pin: "<your_own_value>"
            vdom: "36"
            wimax_auth_protocol: "tls"
            wimax_carrier: "<your_own_value>"
            wimax_realm: "<your_own_value>"


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
