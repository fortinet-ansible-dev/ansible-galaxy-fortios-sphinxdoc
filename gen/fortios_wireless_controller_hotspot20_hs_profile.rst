:source: fortios_wireless_controller_hotspot20_hs_profile.py

:orphan:

.. fortios_wireless_controller_hotspot20_hs_profile:

fortios_wireless_controller_hotspot20_hs_profile -- Configure hotspot profile in Fortinet's FortiOS and FortiGate.
++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++

.. versionadded:: 2.9

.. contents::
   :local:
   :depth: 1


Synopsis
--------
- This module is able to configure a FortiGate or FortiOS (FOS) device by allowing the user to set and modify wireless_controller_hotspot20 feature and hs_profile category. Examples include all parameters and values need to be adjusted to datasources before usage. Tested with FOS v6.0.0



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
    <li> <span class="li-head">state</span> - Indicates whether to create or remove the object. <span class="li-normal">type: str</span> <span class="li-required">required: True</span> <span class="li-normal">choices: present, absent</span></li>
    <li> <span class="li-head">wireless_controller_hotspot20_hs_profile</span> - Configure hotspot profile. <span class="li-normal">type: dict</span></li>
        <ul class="ul-self">
        <li> <span class="li-head">plmn_3gpp</span> - 3GPP PLMN name. Source wireless-controller.hotspot20.anqp-3gpp-cellular.name. <span class="li-normal">type: str</span></li>
        <li> <span class="li-head">access_network_asra</span> - Enable/disable additional step required for access (ASRA). <span class="li-normal">type: str</span> <span class="li-normal">choices: enable, disable</span></li>
        <li> <span class="li-head">access_network_esr</span> - Enable/disable emergency services reachable (ESR). <span class="li-normal">type: str</span> <span class="li-normal">choices: enable, disable</span></li>
        <li> <span class="li-head">access_network_internet</span> - Enable/disable connectivity to the Internet. <span class="li-normal">type: str</span> <span class="li-normal">choices: enable, disable</span></li>
        <li> <span class="li-head">access_network_type</span> - Access network type. <span class="li-normal">type: str</span> <span class="li-normal">choices: private-network, private-network-with-guest-access, chargeable-public-network, free-public-network, personal-device-network, emergency-services-only-network, test-or-experimental, wildcard</span></li>
        <li> <span class="li-head">access_network_uesa</span> - Enable/disable unauthenticated emergency service accessible (UESA). <span class="li-normal">type: str</span> <span class="li-normal">choices: enable, disable</span></li>
        <li> <span class="li-head">anqp_domain_id</span> - ANQP Domain ID (0-65535). <span class="li-normal">type: int</span></li>
        <li> <span class="li-head">bss_transition</span> - Enable/disable basic service set (BSS) transition Support. <span class="li-normal">type: str</span> <span class="li-normal">choices: enable, disable</span></li>
        <li> <span class="li-head">conn_cap</span> - Connection capability name. Source wireless-controller.hotspot20.h2qp-conn-capability.name. <span class="li-normal">type: str</span></li>
        <li> <span class="li-head">deauth_request_timeout</span> - Deauthentication request timeout (in seconds). <span class="li-normal">type: int</span></li>
        <li> <span class="li-head">dgaf</span> - Enable/disable downstream group-addressed forwarding (DGAF). <span class="li-normal">type: str</span> <span class="li-normal">choices: enable, disable</span></li>
        <li> <span class="li-head">domain_name</span> - Domain name. <span class="li-normal">type: str</span></li>
        <li> <span class="li-head">gas_comeback_delay</span> - GAS comeback delay (0 or 100 - 4000 milliseconds). <span class="li-normal">type: int</span></li>
        <li> <span class="li-head">gas_fragmentation_limit</span> - GAS fragmentation limit (512 - 4096). <span class="li-normal">type: int</span></li>
        <li> <span class="li-head">hessid</span> - Homogeneous extended service set identifier (HESSID). <span class="li-normal">type: str</span></li>
        <li> <span class="li-head">ip_addr_type</span> - IP address type name. Source wireless-controller.hotspot20.anqp-ip-address-type.name. <span class="li-normal">type: str</span></li>
        <li> <span class="li-head">l2tif</span> - Enable/disable Layer 2 traffic inspection and filtering. <span class="li-normal">type: str</span> <span class="li-normal">choices: enable, disable</span></li>
        <li> <span class="li-head">nai_realm</span> - NAI realm list name. Source wireless-controller.hotspot20.anqp-nai-realm.name. <span class="li-normal">type: str</span></li>
        <li> <span class="li-head">name</span> - Hotspot profile name. <span class="li-normal">type: str</span> <span class="li-required">required: True</span></li>
        <li> <span class="li-head">network_auth</span> - Network authentication name. Source wireless-controller.hotspot20.anqp-network-auth-type.name. <span class="li-normal">type: str</span></li>
        <li> <span class="li-head">oper_friendly_name</span> - Operator friendly name. Source wireless-controller.hotspot20.h2qp-operator-name.name. <span class="li-normal">type: str</span></li>
        <li> <span class="li-head">osu_provider</span> - Manually selected list of OSU provider(s). <span class="li-normal">type: list</span></li>
            <ul class="ul-self">
            <li> <span class="li-head">name</span> - OSU provider name. Source wireless-controller.hotspot20.h2qp-osu-provider.name. <span class="li-normal">type: str</span> <span class="li-required">required: True</span></li>
            </ul>
        <li> <span class="li-head">osu_ssid</span> - Online sign up (OSU) SSID. <span class="li-normal">type: str</span></li>
        <li> <span class="li-head">pame_bi</span> - Enable/disable Pre-Association Message Exchange BSSID Independent (PAME-BI). <span class="li-normal">type: str</span> <span class="li-normal">choices: disable, enable</span></li>
        <li> <span class="li-head">proxy_arp</span> - Enable/disable Proxy ARP. <span class="li-normal">type: str</span> <span class="li-normal">choices: enable, disable</span></li>
        <li> <span class="li-head">qos_map</span> - QoS MAP set ID. Source wireless-controller.hotspot20.qos-map.name. <span class="li-normal">type: str</span></li>
        <li> <span class="li-head">roaming_consortium</span> - Roaming consortium list name. Source wireless-controller.hotspot20.anqp-roaming-consortium.name. <span class="li-normal">type: str</span></li>
        <li> <span class="li-head">venue_group</span> - Venue group. <span class="li-normal">type: str</span> <span class="li-normal">choices: unspecified, assembly, business, educational, factory, institutional, mercantile, residential, storage, utility, vehicular, outdoor</span></li>
        <li> <span class="li-head">venue_name</span> - Venue name. Source wireless-controller.hotspot20.anqp-venue-name.name. <span class="li-normal">type: str</span></li>
        <li> <span class="li-head">venue_type</span> - Venue type. <span class="li-normal">type: str</span> <span class="li-normal">choices: unspecified, arena, stadium, passenger-terminal, amphitheater, amusement-park, place-of-worship, convention-center, library, museum, restaurant, theater, bar, coffee-shop, zoo-or-aquarium, emergency-center, doctor-office, bank, fire-station, police-station, post-office, professional-office, research-facility, attorney-office, primary-school, secondary-school, university-or-college, factory, hospital, long-term-care-facility, rehab-center, group-home, prison-or-jail, retail-store, grocery-market, auto-service-station, shopping-mall, gas-station, private, hotel-or-motel, dormitory, boarding-house, automobile, airplane, bus, ferry, ship-or-boat, train, motor-bike, muni-mesh-network, city-park, rest-area, traffic-control, bus-stop, kiosk</span></li>
        <li> <span class="li-head">wan_metrics</span> - WAN metric name. Source wireless-controller.hotspot20.h2qp-wan-metric.name. <span class="li-normal">type: str</span></li>
        <li> <span class="li-head">wnm_sleep_mode</span> - Enable/disable wireless network management (WNM) sleep mode. <span class="li-normal">type: str</span> <span class="li-normal">choices: enable, disable</span></li>
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
      - name: Configure hotspot profile.
        fortios_wireless_controller_hotspot20_hs_profile:
          vdom:  "{{ vdom }}"
          state: "present"
          access_token: "<your_own_value>"
          wireless_controller_hotspot20_hs_profile:
            plmn_3gpp: "<your_own_value> (source wireless-controller.hotspot20.anqp-3gpp-cellular.name)"
            access_network_asra: "enable"
            access_network_esr: "enable"
            access_network_internet: "enable"
            access_network_type: "private-network"
            access_network_uesa: "enable"
            anqp_domain_id: "9"
            bss_transition: "enable"
            conn_cap: "<your_own_value> (source wireless-controller.hotspot20.h2qp-conn-capability.name)"
            deauth_request_timeout: "12"
            dgaf: "enable"
            domain_name: "<your_own_value>"
            gas_comeback_delay: "15"
            gas_fragmentation_limit: "16"
            hessid: "<your_own_value>"
            ip_addr_type: "<your_own_value> (source wireless-controller.hotspot20.anqp-ip-address-type.name)"
            l2tif: "enable"
            nai_realm: "<your_own_value> (source wireless-controller.hotspot20.anqp-nai-realm.name)"
            name: "default_name_21"
            network_auth: "<your_own_value> (source wireless-controller.hotspot20.anqp-network-auth-type.name)"
            oper_friendly_name: "<your_own_value> (source wireless-controller.hotspot20.h2qp-operator-name.name)"
            osu_provider:
             -
                name: "default_name_25 (source wireless-controller.hotspot20.h2qp-osu-provider.name)"
            osu_ssid: "<your_own_value>"
            pame_bi: "disable"
            proxy_arp: "enable"
            qos_map: "<your_own_value> (source wireless-controller.hotspot20.qos-map.name)"
            roaming_consortium: "<your_own_value> (source wireless-controller.hotspot20.anqp-roaming-consortium.name)"
            venue_group: "unspecified"
            venue_name: "<your_own_value> (source wireless-controller.hotspot20.anqp-venue-name.name)"
            venue_type: "unspecified"
            wan_metrics: "<your_own_value> (source wireless-controller.hotspot20.h2qp-wan-metric.name)"
            wnm_sleep_mode: "enable"
    


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
