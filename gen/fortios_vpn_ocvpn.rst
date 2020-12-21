:source: fortios_vpn_ocvpn.py

:orphan:

.. fortios_vpn_ocvpn:

fortios_vpn_ocvpn -- Configure Overlay Controller VPN settings in Fortinet's FortiOS and FortiGate.
+++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++

.. versionadded:: 2.9

.. contents::
   :local:
   :depth: 1


Synopsis
--------
- This module is able to configure a FortiGate or FortiOS (FOS) device by allowing the user to set and modify vpn feature and ocvpn category. Examples include all parameters and values need to be adjusted to datasources before usage. Tested with FOS v6.4.0



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
    <li> <span class="li-head">vpn_ocvpn</span> - Configure Overlay Controller VPN settings. <span class="li-normal">type: dict</span></li>
        <ul class="ul-self">
        <li> <span class="li-head">auto_discovery</span> - Enable/disable auto-discovery shortcuts. <span class="li-normal">type: str</span> <span class="li-normal">choices: enable, disable</span></li>
        <li> <span class="li-head">eap</span> - Enable/disable EAP client authentication. <span class="li-normal">type: str</span> <span class="li-normal">choices: enable, disable</span></li>
        <li> <span class="li-head">eap_users</span> - EAP authentication user group. Source user.group.name. <span class="li-normal">type: str</span></li>
        <li> <span class="li-head">forticlient_access</span> - Configure FortiClient settings. <span class="li-normal">type: dict</span></li>
            <ul class="ul-self">
            <li> <span class="li-head">auth_groups</span> - FortiClient user authentication groups. <span class="li-normal">type: list</span></li>
                <ul class="ul-self">
                <li> <span class="li-head">auth_group</span> - Authentication user group for FortiClient access. Source user.group.name. <span class="li-normal">type: str</span></li>
                <li> <span class="li-head">name</span> - Group name. <span class="li-normal">type: str</span> <span class="li-required">required: True</span></li>
                <li> <span class="li-head">overlays</span> - OCVPN overlays to allow access to. <span class="li-normal">type: list</span></li>
                    <ul class="ul-self">
                    <li> <span class="li-head">overlay_name</span> - Overlay name. Source vpn.ocvpn.overlays.overlay-name. <span class="li-normal">type: str</span></li>
                    </ul>
                </ul>
            <li> <span class="li-head">psksecret</span> - Pre-shared secret for FortiClient PSK authentication (ASCII string or hexadecimal encoded with a leading 0x). <span class="li-normal">type: str</span></li>
            <li> <span class="li-head">status</span> - Enable/disable FortiClient to access OCVPN networks. <span class="li-normal">type: str</span> <span class="li-normal">choices: enable, disable</span></li>
            </ul>
        <li> <span class="li-head">ip_allocation_block</span> - Class B subnet reserved for private IP address assignment. <span class="li-normal">type: str</span></li>
        <li> <span class="li-head">multipath</span> - Enable/disable multipath redundancy. <span class="li-normal">type: str</span> <span class="li-normal">choices: enable, disable</span></li>
        <li> <span class="li-head">nat</span> - Enable/disable inter-overlay source NAT. <span class="li-normal">type: str</span> <span class="li-normal">choices: enable, disable</span></li>
        <li> <span class="li-head">overlays</span> - Network overlays to register with Overlay Controller VPN service. <span class="li-normal">type: list</span></li>
            <ul class="ul-self">
            <li> <span class="li-head">assign_ip</span> - Enable/disable mode-cfg address assignment. <span class="li-normal">type: str</span> <span class="li-normal">choices: enable, disable</span></li>
            <li> <span class="li-head">inter_overlay</span> - Allow or deny traffic from other overlays. <span class="li-normal">type: str</span> <span class="li-normal">choices: allow, deny</span></li>
            <li> <span class="li-head">ipv4_end_ip</span> - End of IPv4 range. <span class="li-normal">type: str</span></li>
            <li> <span class="li-head">ipv4_start_ip</span> - Start of IPv4 range. <span class="li-normal">type: str</span></li>
            <li> <span class="li-head">overlay_name</span> - Overlay name. <span class="li-normal">type: str</span></li>
            <li> <span class="li-head">subnets</span> - Internal subnets to register with OCVPN service. <span class="li-normal">type: list</span></li>
                <ul class="ul-self">
                <li> <span class="li-head">id</span> - ID. <span class="li-normal">type: int</span> <span class="li-required">required: True</span></li>
                <li> <span class="li-head">interface</span> - LAN interface. Source system.interface.name. <span class="li-normal">type: str</span></li>
                <li> <span class="li-head">subnet</span> - IPv4 address and subnet mask. <span class="li-normal">type: str</span></li>
                <li> <span class="li-head">type</span> - Subnet type. <span class="li-normal">type: str</span> <span class="li-normal">choices: subnet, interface</span></li>
                </ul>
            </ul>
        <li> <span class="li-head">poll_interval</span> - Overlay Controller VPN polling interval. <span class="li-normal">type: int</span></li>
        <li> <span class="li-head">role</span> - Set device role. <span class="li-normal">type: str</span> <span class="li-normal">choices: spoke, primary-hub, secondary-hub</span></li>
        <li> <span class="li-head">sdwan</span> - Enable/disable adding OCVPN tunnels to SDWAN. <span class="li-normal">type: str</span> <span class="li-normal">choices: enable, disable</span></li>
        <li> <span class="li-head">status</span> - Enable/disable Overlay Controller cloud assisted VPN. <span class="li-normal">type: str</span> <span class="li-normal">choices: enable, disable</span></li>
        <li> <span class="li-head">wan_interface</span> - FortiGate WAN interfaces to use with OCVPN. <span class="li-normal">type: list</span></li>
            <ul class="ul-self">
            <li> <span class="li-head">name</span> - Interface name. Source system.interface.name. <span class="li-normal">type: str</span> <span class="li-required">required: True</span></li>
            </ul>
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
      - name: Configure Overlay Controller VPN settings.
        fortios_vpn_ocvpn:
          vdom:  "{{ vdom }}"
          vpn_ocvpn:
            auto_discovery: "enable"
            eap: "enable"
            eap_users: "<your_own_value> (source user.group.name)"
            forticlient_access:
                auth_groups:
                 -
                    auth_group: "<your_own_value> (source user.group.name)"
                    name: "default_name_9"
                    overlays:
                     -
                        overlay_name: "<your_own_value> (source vpn.ocvpn.overlays.overlay-name)"
                psksecret: "<your_own_value>"
                status: "enable"
            ip_allocation_block: "<your_own_value>"
            multipath: "enable"
            nat: "enable"
            overlays:
             -
                assign_ip: "enable"
                inter_overlay: "allow"
                ipv4_end_ip: "<your_own_value>"
                ipv4_start_ip: "<your_own_value>"
                overlay_name: "<your_own_value>"
                subnets:
                 -
                    id:  "24"
                    interface: "<your_own_value> (source system.interface.name)"
                    subnet: "<your_own_value>"
                    type: "subnet"
            poll_interval: "28"
            role: "spoke"
            sdwan: "enable"
            status: "enable"
            wan_interface:
             -
                name: "default_name_33 (source system.interface.name)"
    


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
