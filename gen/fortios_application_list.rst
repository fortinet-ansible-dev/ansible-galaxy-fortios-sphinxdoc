:source: fortios_application_list.py

:orphan:

.. fortios_application_list:

fortios_application_list -- Configure application control lists in Fortinet's FortiOS and FortiGate.
++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++

.. versionadded:: 2.8

.. contents::
   :local:
   :depth: 1


Synopsis
--------
- This module is able to configure a FortiGate or FortiOS (FOS) device by allowing the user to set and modify application feature and list category. Examples include all parameters and values need to be adjusted to datasources before usage. Tested with FOS v6.0.5



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
    <li> <span class="li-head">application_list</span> - Configure application control lists. <span class="li-normal">type: dict</span></li>
        <ul class="ul-self">
        <li> <span class="li-head">state</span> - B(Deprecated) <span class="li-normal">type: str</span> <span class="li-required">required: False</span> <span class="li-normal">choices: present, absent</span></li>
        <li> <span class="li-head">app_replacemsg</span> - Enable/disable replacement messages for blocked applications. <span class="li-normal">type: str</span> <span class="li-normal">choices: disable, enable</span></li>
        <li> <span class="li-head">comment</span> - comments <span class="li-normal">type: str</span></li>
        <li> <span class="li-head">deep_app_inspection</span> - Enable/disable deep application inspection. <span class="li-normal">type: str</span> <span class="li-normal">choices: disable, enable</span></li>
        <li> <span class="li-head">entries</span> - Application list entries. <span class="li-normal">type: list</span></li>
            <ul class="ul-self">
            <li> <span class="li-head">action</span> - Pass or block traffic, or reset connection for traffic from this application. <span class="li-normal">type: str</span> <span class="li-normal">choices: pass, block, reset</span></li>
            <li> <span class="li-head">application</span> - ID of allowed applications. <span class="li-normal">type: list</span></li>
                <ul class="ul-self">
                <li> <span class="li-head">id</span> - Application IDs. <span class="li-normal">type: int</span> <span class="li-required">required: True</span></li>
                </ul>
            <li> <span class="li-head">behavior</span> - Application behavior filter. <span class="li-normal">type: str</span></li>
            <li> <span class="li-head">category</span> - Category ID list. <span class="li-normal">type: list</span></li>
                <ul class="ul-self">
                <li> <span class="li-head">id</span> - Application category ID. <span class="li-normal">type: int</span> <span class="li-required">required: True</span></li>
                </ul>
            <li> <span class="li-head">id</span> - Entry ID. <span class="li-normal">type: int</span> <span class="li-required">required: True</span></li>
            <li> <span class="li-head">log</span> - Enable/disable logging for this application list. <span class="li-normal">type: str</span> <span class="li-normal">choices: disable, enable</span></li>
            <li> <span class="li-head">log_packet</span> - Enable/disable packet logging. <span class="li-normal">type: str</span> <span class="li-normal">choices: disable, enable</span></li>
            <li> <span class="li-head">parameters</span> - Application parameters. <span class="li-normal">type: list</span></li>
                <ul class="ul-self">
                <li> <span class="li-head">id</span> - Parameter ID. <span class="li-normal">type: int</span> <span class="li-required">required: True</span></li>
                <li> <span class="li-head">value</span> - Parameter value. <span class="li-normal">type: str</span></li>
                </ul>
            <li> <span class="li-head">per_ip_shaper</span> - Per-IP traffic shaper. Source firewall.shaper.per-ip-shaper.name. <span class="li-normal">type: str</span></li>
            <li> <span class="li-head">popularity</span> - Application popularity filter (1 - 5, from least to most popular). <span class="li-normal">type: str</span> <span class="li-normal">choices: 1, 2, 3, 4, 5</span></li>
            <li> <span class="li-head">protocols</span> - Application protocol filter. <span class="li-normal">type: str</span></li>
            <li> <span class="li-head">quarantine</span> - Quarantine method. <span class="li-normal">type: str</span> <span class="li-normal">choices: none, attacker</span></li>
            <li> <span class="li-head">quarantine_expiry</span> - Duration of quarantine. (Format <span class="li-normal">type: str</span></li>
            <li> <span class="li-head">quarantine_log</span> - Enable/disable quarantine logging. <span class="li-normal">type: str</span> <span class="li-normal">choices: disable, enable</span></li>
            <li> <span class="li-head">rate_count</span> - Count of the rate. <span class="li-normal">type: int</span></li>
            <li> <span class="li-head">rate_duration</span> - Duration (sec) of the rate. <span class="li-normal">type: int</span></li>
            <li> <span class="li-head">rate_mode</span> - Rate limit mode. <span class="li-normal">type: str</span> <span class="li-normal">choices: periodical, continuous</span></li>
            <li> <span class="li-head">rate_track</span> - Track the packet protocol field. <span class="li-normal">type: str</span> <span class="li-normal">choices: none, src-ip, dest-ip, dhcp-client-mac, dns-domain</span></li>
            <li> <span class="li-head">risk</span> - Risk, or impact, of allowing traffic from this application to occur (1 - 5; Low, Elevated, Medium, High, and Critical). <span class="li-normal">type: list</span></li>
                <ul class="ul-self">
                <li> <span class="li-head">level</span> - Risk, or impact, of allowing traffic from this application to occur (1 - 5; Low, Elevated, Medium, High, and Critical). <span class="li-normal">type: int</span> <span class="li-required">required: True</span></li>
                </ul>
            <li> <span class="li-head">session_ttl</span> - Session TTL (0 = default). <span class="li-normal">type: int</span></li>
            <li> <span class="li-head">shaper</span> - Traffic shaper. Source firewall.shaper.traffic-shaper.name. <span class="li-normal">type: str</span></li>
            <li> <span class="li-head">shaper_reverse</span> - Reverse traffic shaper. Source firewall.shaper.traffic-shaper.name. <span class="li-normal">type: str</span></li>
            <li> <span class="li-head">sub_category</span> - Application Sub-category ID list. <span class="li-normal">type: list</span></li>
                <ul class="ul-self">
                <li> <span class="li-head">id</span> - Application sub-category ID. <span class="li-normal">type: int</span> <span class="li-required">required: True</span></li>
                </ul>
            <li> <span class="li-head">technology</span> - Application technology filter. <span class="li-normal">type: str</span></li>
            <li> <span class="li-head">vendor</span> - Application vendor filter. <span class="li-normal">type: str</span></li>
            </ul>
        <li> <span class="li-head">extended_log</span> - Enable/disable extended logging. <span class="li-normal">type: str</span> <span class="li-normal">choices: enable, disable</span></li>
        <li> <span class="li-head">name</span> - List name. <span class="li-normal">type: str</span> <span class="li-required">required: True</span></li>
        <li> <span class="li-head">options</span> - Basic application protocol signatures allowed by default. <span class="li-normal">type: str</span> <span class="li-normal">choices: allow-dns, allow-icmp, allow-http, allow-ssl, allow-quic</span></li>
        <li> <span class="li-head">other_application_action</span> - Action for other applications. <span class="li-normal">type: str</span> <span class="li-normal">choices: pass, block</span></li>
        <li> <span class="li-head">other_application_log</span> - Enable/disable logging for other applications. <span class="li-normal">type: str</span> <span class="li-normal">choices: disable, enable</span></li>
        <li> <span class="li-head">p2p_black_list</span> - P2P applications to be black listed. <span class="li-normal">type: str</span> <span class="li-normal">choices: skype, edonkey, bittorrent</span></li>
        <li> <span class="li-head">replacemsg_group</span> - Replacement message group. Source system.replacemsg-group.name. <span class="li-normal">type: str</span></li>
        <li> <span class="li-head">unknown_application_action</span> - Pass or block traffic from unknown applications. <span class="li-normal">type: str</span> <span class="li-normal">choices: pass, block</span></li>
        <li> <span class="li-head">unknown_application_log</span> - Enable/disable logging for unknown applications. <span class="li-normal">type: str</span> <span class="li-normal">choices: disable, enable</span></li>
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
      - name: Configure application control lists.
        fortios_application_list:
          vdom:  "{{ vdom }}"
          state: "present"
          application_list:
            app_replacemsg: "disable"
            comment: "comments"
            deep_app_inspection: "disable"
            entries:
             -
                action: "pass"
                application:
                 -
                    id:  "9"
                behavior: "<your_own_value>"
                category:
                 -
                    id:  "12"
                id:  "13"
                log: "disable"
                log_packet: "disable"
                parameters:
                 -
                    id:  "17"
                    value: "<your_own_value>"
                per_ip_shaper: "<your_own_value> (source firewall.shaper.per-ip-shaper.name)"
                popularity: "1"
                protocols: "<your_own_value>"
                quarantine: "none"
                quarantine_expiry: "<your_own_value>"
                quarantine_log: "disable"
                rate_count: "25"
                rate_duration: "26"
                rate_mode: "periodical"
                rate_track: "none"
                risk:
                 -
                    level: "30"
                session_ttl: "31"
                shaper: "<your_own_value> (source firewall.shaper.traffic-shaper.name)"
                shaper_reverse: "<your_own_value> (source firewall.shaper.traffic-shaper.name)"
                sub_category:
                 -
                    id:  "35"
                technology: "<your_own_value>"
                vendor: "<your_own_value>"
            extended_log: "enable"
            name: "default_name_39"
            options: "allow-dns"
            other_application_action: "pass"
            other_application_log: "disable"
            p2p_black_list: "skype"
            replacemsg_group: "<your_own_value> (source system.replacemsg-group.name)"
            unknown_application_action: "pass"
            unknown_application_log: "disable"


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
