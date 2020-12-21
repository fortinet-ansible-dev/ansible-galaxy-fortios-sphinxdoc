:source: fortios_system_modem.py

:orphan:

.. fortios_system_modem:

fortios_system_modem -- Configure MODEM in Fortinet's FortiOS and FortiGate.
++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++

.. versionadded:: 2.10

.. contents::
   :local:
   :depth: 1


Synopsis
--------
- This module is able to configure a FortiGate or FortiOS (FOS) device by allowing the user to set and modify system feature and modem category. Examples include all parameters and values need to be adjusted to datasources before usage. Tested with FOS v6.0.0



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
    <li> <span class="li-head">system_modem</span> - Configure MODEM. <span class="li-normal">type: dict</span></li>
        <ul class="ul-self">
        <li> <span class="li-head">action</span> - Dial up/stop MODEM. <span class="li-normal">type: str</span> <span class="li-normal">choices: dial, stop, none</span></li>
        <li> <span class="li-head">altmode</span> - Enable/disable altmode for installations using PPP in China. <span class="li-normal">type: str</span> <span class="li-normal">choices: enable, disable</span></li>
        <li> <span class="li-head">authtype1</span> - Allowed authentication types for ISP 1. <span class="li-normal">type: str</span> <span class="li-normal">choices: pap, chap, mschap, mschapv2</span></li>
        <li> <span class="li-head">authtype2</span> - Allowed authentication types for ISP 2. <span class="li-normal">type: str</span> <span class="li-normal">choices: pap, chap, mschap, mschapv2</span></li>
        <li> <span class="li-head">authtype3</span> - Allowed authentication types for ISP 3. <span class="li-normal">type: str</span> <span class="li-normal">choices: pap, chap, mschap, mschapv2</span></li>
        <li> <span class="li-head">auto_dial</span> - Enable/disable auto-dial after a reboot or disconnection. <span class="li-normal">type: str</span> <span class="li-normal">choices: enable, disable</span></li>
        <li> <span class="li-head">connect_timeout</span> - Connection completion timeout (30 - 255 sec). <span class="li-normal">type: int</span></li>
        <li> <span class="li-head">dial_cmd1</span> - Dial command (this is often an ATD or ATDT command). <span class="li-normal">type: str</span></li>
        <li> <span class="li-head">dial_cmd2</span> - Dial command (this is often an ATD or ATDT command). <span class="li-normal">type: str</span></li>
        <li> <span class="li-head">dial_cmd3</span> - Dial command (this is often an ATD or ATDT command). <span class="li-normal">type: str</span></li>
        <li> <span class="li-head">dial_on_demand</span> - Enable/disable to dial the modem when packets are routed to the modem interface. <span class="li-normal">type: str</span> <span class="li-normal">choices: enable, disable</span></li>
        <li> <span class="li-head">distance</span> - Distance of learned routes (1 - 255). <span class="li-normal">type: int</span></li>
        <li> <span class="li-head">dont_send_CR1</span> - Do not send CR when connected (ISP1). <span class="li-normal">type: str</span> <span class="li-normal">choices: enable, disable</span></li>
        <li> <span class="li-head">dont_send_CR2</span> - Do not send CR when connected (ISP2). <span class="li-normal">type: str</span> <span class="li-normal">choices: enable, disable</span></li>
        <li> <span class="li-head">dont_send_CR3</span> - Do not send CR when connected (ISP3). <span class="li-normal">type: str</span> <span class="li-normal">choices: enable, disable</span></li>
        <li> <span class="li-head">extra_init1</span> - Extra initialization string to ISP 1. <span class="li-normal">type: str</span></li>
        <li> <span class="li-head">extra_init2</span> - Extra initialization string to ISP 2. <span class="li-normal">type: str</span></li>
        <li> <span class="li-head">extra_init3</span> - Extra initialization string to ISP 3. <span class="li-normal">type: str</span></li>
        <li> <span class="li-head">holddown_timer</span> - Hold down timer in seconds (1 - 60 sec). <span class="li-normal">type: int</span></li>
        <li> <span class="li-head">idle_timer</span> - MODEM connection idle time (1 - 9999 min). <span class="li-normal">type: int</span></li>
        <li> <span class="li-head">interface</span> - Name of redundant interface. Source system.interface.name. <span class="li-normal">type: str</span></li>
        <li> <span class="li-head">lockdown_lac</span> - Allow connection only to the specified Location Area Code (LAC). <span class="li-normal">type: str</span></li>
        <li> <span class="li-head">mode</span> - Set MODEM operation mode to redundant or standalone. <span class="li-normal">type: str</span> <span class="li-normal">choices: standalone, redundant</span></li>
        <li> <span class="li-head">network_init</span> - AT command to set the Network name/type (AT+COPS=<mode>,[<format>,<oper>[,<AcT>]]). <span class="li-normal">type: str</span></li>
        <li> <span class="li-head">passwd1</span> - Password to access the specified dialup account. <span class="li-normal">type: str</span></li>
        <li> <span class="li-head">passwd2</span> - Password to access the specified dialup account. <span class="li-normal">type: str</span></li>
        <li> <span class="li-head">passwd3</span> - Password to access the specified dialup account. <span class="li-normal">type: str</span></li>
        <li> <span class="li-head">peer_modem1</span> - Specify peer MODEM type for phone1. <span class="li-normal">type: str</span> <span class="li-normal">choices: generic, actiontec, ascend_TNT</span></li>
        <li> <span class="li-head">peer_modem2</span> - Specify peer MODEM type for phone2. <span class="li-normal">type: str</span> <span class="li-normal">choices: generic, actiontec, ascend_TNT</span></li>
        <li> <span class="li-head">peer_modem3</span> - Specify peer MODEM type for phone3. <span class="li-normal">type: str</span> <span class="li-normal">choices: generic, actiontec, ascend_TNT</span></li>
        <li> <span class="li-head">phone1</span> - Phone number to connect to the dialup account (must not contain spaces, and should include standard special characters). <span class="li-normal">type: str</span></li>
        <li> <span class="li-head">phone2</span> - Phone number to connect to the dialup account (must not contain spaces, and should include standard special characters). <span class="li-normal">type: str</span></li>
        <li> <span class="li-head">phone3</span> - Phone number to connect to the dialup account (must not contain spaces, and should include standard special characters). <span class="li-normal">type: str</span></li>
        <li> <span class="li-head">pin_init</span> - AT command to set the PIN (AT+PIN=<pin>). <span class="li-normal">type: str</span></li>
        <li> <span class="li-head">ppp_echo_request1</span> - Enable/disable PPP echo-request to ISP 1. <span class="li-normal">type: str</span> <span class="li-normal">choices: enable, disable</span></li>
        <li> <span class="li-head">ppp_echo_request2</span> - Enable/disable PPP echo-request to ISP 2. <span class="li-normal">type: str</span> <span class="li-normal">choices: enable, disable</span></li>
        <li> <span class="li-head">ppp_echo_request3</span> - Enable/disable PPP echo-request to ISP 3. <span class="li-normal">type: str</span> <span class="li-normal">choices: enable, disable</span></li>
        <li> <span class="li-head">priority</span> - Priority of learned routes (0 - 4294967295). <span class="li-normal">type: int</span></li>
        <li> <span class="li-head">redial</span> - Redial limit (1 - 10 attempts, none = redial forever). <span class="li-normal">type: str</span> <span class="li-normal">choices: none, 1, 2, 3, 4, 5, 6, 7, 8, 9, 10</span></li>
        <li> <span class="li-head">reset</span> - Number of dial attempts before resetting modem (0 = never reset). <span class="li-normal">type: int</span></li>
        <li> <span class="li-head">status</span> - Enable/disable Modem support (equivalent to bringing an interface up or down). <span class="li-normal">type: str</span> <span class="li-normal">choices: enable, disable</span></li>
        <li> <span class="li-head">traffic_check</span> - Enable/disable traffic-check. <span class="li-normal">type: str</span> <span class="li-normal">choices: enable, disable</span></li>
        <li> <span class="li-head">username1</span> - User name to access the specified dialup account. <span class="li-normal">type: str</span></li>
        <li> <span class="li-head">username2</span> - User name to access the specified dialup account. <span class="li-normal">type: str</span></li>
        <li> <span class="li-head">username3</span> - User name to access the specified dialup account. <span class="li-normal">type: str</span></li>
        <li> <span class="li-head">wireless_port</span> - Enter wireless port number, 0 for default, 1 for first port, ... (0 - 4294967295) <span class="li-normal">type: int</span></li>
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
      - name: Configure MODEM.
        fortios_system_modem:
          vdom:  "{{ vdom }}"
          system_modem:
            action: "dial"
            altmode: "enable"
            authtype1: "pap"
            authtype2: "pap"
            authtype3: "pap"
            auto_dial: "enable"
            connect_timeout: "9"
            dial_cmd1: "<your_own_value>"
            dial_cmd2: "<your_own_value>"
            dial_cmd3: "<your_own_value>"
            dial_on_demand: "enable"
            distance: "14"
            dont_send_CR1: "enable"
            dont_send_CR2: "enable"
            dont_send_CR3: "enable"
            extra_init1: "<your_own_value>"
            extra_init2: "<your_own_value>"
            extra_init3: "<your_own_value>"
            holddown_timer: "21"
            idle_timer: "22"
            interface: "<your_own_value> (source system.interface.name)"
            lockdown_lac: "<your_own_value>"
            mode: "standalone"
            network_init: "<your_own_value>"
            passwd1: "<your_own_value>"
            passwd2: "<your_own_value>"
            passwd3: "<your_own_value>"
            peer_modem1: "generic"
            peer_modem2: "generic"
            peer_modem3: "generic"
            phone1: "<your_own_value>"
            phone2: "<your_own_value>"
            phone3: "<your_own_value>"
            pin_init: "<your_own_value>"
            ppp_echo_request1: "enable"
            ppp_echo_request2: "enable"
            ppp_echo_request3: "enable"
            priority: "40"
            redial: "none"
            reset: "42"
            status: "enable"
            traffic_check: "enable"
            username1: "<your_own_value>"
            username2: "<your_own_value>"
            username3: "<your_own_value>"
            wireless_port: "48"
    


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
