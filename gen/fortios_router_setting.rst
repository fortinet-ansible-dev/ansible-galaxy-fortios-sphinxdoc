:source: fortios_router_setting.py

:orphan:

.. fortios_router_setting:

fortios_router_setting -- Configure router settings in Fortinet's FortiOS and FortiGate.
++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++

.. versionadded:: 2.8

.. contents::
   :local:
   :depth: 1


Synopsis
--------
- This module is able to configure a FortiGate or FortiOS (FOS) device by allowing the user to set and modify router feature and setting category. Examples include all parameters and values need to be adjusted to datasources before usage. Tested with FOS v6.2.0



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
    <li> <span class="li-head">router_setting</span> - Configure router settings. <span class="li-normal">type: dict</span></li>
        <ul class="ul-self">
        <li> <span class="li-head">bgp_debug_flags</span> - bgp_debug_flags <span class="li-normal">type: str</span></li>
        <li> <span class="li-head">hostname</span> - Hostname for this virtual domain router. <span class="li-normal">type: str</span></li>
        <li> <span class="li-head">igmp_debug_flags</span> - igmp_debug_flags <span class="li-normal">type: str</span></li>
        <li> <span class="li-head">imi_debug_flags</span> - imi_debug_flags <span class="li-normal">type: str</span></li>
        <li> <span class="li-head">isis_debug_flags</span> - isis_debug_flags <span class="li-normal">type: str</span></li>
        <li> <span class="li-head">ospf6_debug_events_flags</span> - ospf6_debug_events_flags <span class="li-normal">type: str</span></li>
        <li> <span class="li-head">ospf6_debug_ifsm_flags</span> - ospf6_debug_ifsm_flags <span class="li-normal">type: str</span></li>
        <li> <span class="li-head">ospf6_debug_lsa_flags</span> - ospf6_debug_lsa_flags <span class="li-normal">type: str</span></li>
        <li> <span class="li-head">ospf6_debug_nfsm_flags</span> - ospf6_debug_nfsm_flags <span class="li-normal">type: str</span></li>
        <li> <span class="li-head">ospf6_debug_nsm_flags</span> - ospf6_debug_nsm_flags <span class="li-normal">type: str</span></li>
        <li> <span class="li-head">ospf6_debug_packet_flags</span> - ospf6_debug_packet_flags <span class="li-normal">type: str</span></li>
        <li> <span class="li-head">ospf6_debug_route_flags</span> - ospf6_debug_route_flags <span class="li-normal">type: str</span></li>
        <li> <span class="li-head">ospf_debug_events_flags</span> - ospf_debug_events_flags <span class="li-normal">type: str</span></li>
        <li> <span class="li-head">ospf_debug_ifsm_flags</span> - ospf_debug_ifsm_flags <span class="li-normal">type: str</span></li>
        <li> <span class="li-head">ospf_debug_lsa_flags</span> - ospf_debug_lsa_flags <span class="li-normal">type: str</span></li>
        <li> <span class="li-head">ospf_debug_nfsm_flags</span> - ospf_debug_nfsm_flags <span class="li-normal">type: str</span></li>
        <li> <span class="li-head">ospf_debug_nsm_flags</span> - ospf_debug_nsm_flags <span class="li-normal">type: str</span></li>
        <li> <span class="li-head">ospf_debug_packet_flags</span> - ospf_debug_packet_flags <span class="li-normal">type: str</span></li>
        <li> <span class="li-head">ospf_debug_route_flags</span> - ospf_debug_route_flags <span class="li-normal">type: str</span></li>
        <li> <span class="li-head">pimdm_debug_flags</span> - pimdm_debug_flags <span class="li-normal">type: str</span></li>
        <li> <span class="li-head">pimsm_debug_joinprune_flags</span> - pimsm_debug_joinprune_flags <span class="li-normal">type: str</span></li>
        <li> <span class="li-head">pimsm_debug_simple_flags</span> - pimsm_debug_simple_flags <span class="li-normal">type: str</span></li>
        <li> <span class="li-head">pimsm_debug_timer_flags</span> - pimsm_debug_timer_flags <span class="li-normal">type: str</span></li>
        <li> <span class="li-head">rip_debug_flags</span> - rip_debug_flags <span class="li-normal">type: str</span></li>
        <li> <span class="li-head">ripng_debug_flags</span> - ripng_debug_flags <span class="li-normal">type: str</span></li>
        <li> <span class="li-head">show_filter</span> - Prefix-list as filter for showing routes. Source router.prefix-list.name. <span class="li-normal">type: str</span></li>
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
      - name: Configure router settings.
        fortios_router_setting:
          vdom:  "{{ vdom }}"
          router_setting:
            bgp_debug_flags: "<your_own_value>"
            hostname: "myhostname"
            igmp_debug_flags: "<your_own_value>"
            imi_debug_flags: "<your_own_value>"
            isis_debug_flags: "<your_own_value>"
            ospf6_debug_events_flags: "<your_own_value>"
            ospf6_debug_ifsm_flags: "<your_own_value>"
            ospf6_debug_lsa_flags: "<your_own_value>"
            ospf6_debug_nfsm_flags: "<your_own_value>"
            ospf6_debug_nsm_flags: "<your_own_value>"
            ospf6_debug_packet_flags: "<your_own_value>"
            ospf6_debug_route_flags: "<your_own_value>"
            ospf_debug_events_flags: "<your_own_value>"
            ospf_debug_ifsm_flags: "<your_own_value>"
            ospf_debug_lsa_flags: "<your_own_value>"
            ospf_debug_nfsm_flags: "<your_own_value>"
            ospf_debug_nsm_flags: "<your_own_value>"
            ospf_debug_packet_flags: "<your_own_value>"
            ospf_debug_route_flags: "<your_own_value>"
            pimdm_debug_flags: "<your_own_value>"
            pimsm_debug_joinprune_flags: "<your_own_value>"
            pimsm_debug_simple_flags: "<your_own_value>"
            pimsm_debug_timer_flags: "<your_own_value>"
            rip_debug_flags: "<your_own_value>"
            ripng_debug_flags: "<your_own_value>"
            show_filter: "<your_own_value> (source router.prefix-list.name)"
    


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
