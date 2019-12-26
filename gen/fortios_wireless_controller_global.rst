:source: fortios_wireless_controller_global.py

:orphan:

.. _fortios_wireless_controller_global:

fortios_wireless_controller_global -- Configure wireless controller global settings in Fortinet's FortiOS and FortiGate.
++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++

.. versionadded:: 2.8

.. contents::
   :local:
   :depth: 1


Synopsis
--------
- This module is able to configure a FortiGate or FortiOS (FOS) device by allowing the user to set and modify wireless_controller feature and global category. Examples include all parameters and values need to be adjusted to datasources before usage. Tested with FOS v6.0.5


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
    <li><span class="li-head">wireless_controller_global</span> - Configure wireless controller global settings. <span class="li-normal">default: null</span> <span class="li-normal">type: dict</span></li>
            <ul class="ul-self">

            <li><span class="li-head">ap_log_server</span> - Enable/disable configuring APs or FortiAPs to send log messages to a syslog server . <span class="li-normal">type: str</span> <span class="li-normal">choices: enable,  disable</span></li>
            <li><span class="li-head">ap_log_server_ip</span> - IP address that APs or FortiAPs send log messages to. <span class="li-normal">type: str</span></li>
            <li><span class="li-head">ap_log_server_port</span> - Port that APs or FortiAPs send log messages to. <span class="li-normal">type: int</span></li>
            <li><span class="li-head">control_message_offload</span> - Configure CAPWAP control message data channel offload. <span class="li-normal">type: str</span> <span class="li-normal">choices: ebp-frame,  aeroscout-tag,  ap-list,  sta-list,  sta-cap-list,  stats,  aeroscout-mu</span></li>
            <li><span class="li-head">data_ethernet_II</span> - Configure the wireless controller to use Ethernet II or 802.3 frames with 802.3 data tunnel mode . <span class="li-normal">type: str</span> <span class="li-normal">choices: enable,  disable</span></li>
            <li><span class="li-head">discovery_mc_addr</span> - Multicast IP address for AP discovery . <span class="li-normal">type: str</span></li>
            <li><span class="li-head">fiapp_eth_type</span> - Ethernet type for Fortinet Inter-Access Point Protocol (IAPP), or IEEE 802.11f, packets (0 - 65535). <span class="li-normal">type: int</span></li>
            <li><span class="li-head">image_download</span> - Enable/disable WTP image download at join time. <span class="li-normal">type: str</span> <span class="li-normal">choices: enable,  disable</span></li>
            <li><span class="li-head">ipsec_base_ip</span> - Base IP address for IPsec VPN tunnels between the access points and the wireless controller . <span class="li-normal">type: str</span></li>
            <li><span class="li-head">link_aggregation</span> - Enable/disable calculating the CAPWAP transmit hash to load balance sessions to link aggregation nodes . <span class="li-normal">type: str</span> <span class="li-normal">choices: enable,  disable</span></li>
            <li><span class="li-head">location</span> - Description of the location of the wireless controller. <span class="li-normal">type: str</span></li>
            <li><span class="li-head">max_clients</span> - Maximum number of clients that can connect simultaneously . <span class="li-normal">type: int</span></li>
            <li><span class="li-head">max_retransmit</span> - Maximum number of tunnel packet retransmissions (0 - 64). <span class="li-normal">type: int</span></li>
            <li><span class="li-head">mesh_eth_type</span> - Mesh Ethernet identifier included in backhaul packets (0 - 65535). <span class="li-normal">type: int</span></li>
            <li><span class="li-head">name</span> - Name of the wireless controller. <span class="li-normal">type: str</span></li>
            <li><span class="li-head">rogue_scan_mac_adjacency</span> - Maximum numerical difference between an AP's Ethernet and wireless MAC values to match for rogue detection (0 - 31). <span class="li-normal">type: int</span></li>
            <li><span class="li-head">wtp_share</span> - Enable/disable sharing of WTPs between VDOMs. <span class="li-normal">type: str</span> <span class="li-normal">choices: enable,  disable</span>
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
      - name: Configure wireless controller global settings.
        fortios_wireless_controller_global:
          host:  "{{ host }}"
          username: "{{ username }}"
          password: "{{ password }}"
          vdom:  "{{ vdom }}"
          https: "False"
          wireless_controller_global:
            ap_log_server: "enable"
            ap_log_server_ip: "<your_own_value>"
            ap_log_server_port: "5"
            control_message_offload: "ebp-frame"
            data_ethernet_II: "enable"
            discovery_mc_addr: "<your_own_value>"
            fiapp_eth_type: "9"
            image_download: "enable"
            ipsec_base_ip: "<your_own_value>"
            link_aggregation: "enable"
            location: "<your_own_value>"
            max_clients: "14"
            max_retransmit: "15"
            mesh_eth_type: "16"
            name: "default_name_17"
            rogue_scan_mac_adjacency: "18"
            wtp_share: "enable"



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