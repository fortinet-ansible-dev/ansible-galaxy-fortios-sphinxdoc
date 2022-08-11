
Release Notes
==============================

|

Release Galaxy 2.1.7
--------------------

Release Targets
^^^^^^^^^^^^^^^

FortiOS Galaxy 2.1.7 is based on 2.1.6

Features
^^^^^^^^^^^^^^^
- Support Fortios 7.2.0.
- Support Diff feature in check_mode.

Bug Fixes
^^^^^^^^^^^^^^^
- Fix typo in the documentation of ``Install FortiOS Galaxy Collection``.
- Fix the error message in the debugging log when using ``access_token``.
- Fix the Github Issue #187.
- Fix the Github Issue #188 and #189.
- Fix the Github Issue #190.
- Fix the Github Issue #191.
- Fix the issue when filtering out parameter with space in the module ``fortios_configuration_fact``.

Release Galaxy 2.1.6
--------------------

Release Targets
^^^^^^^^^^^^^^^

FortiOS Galaxy 2.1.6 is based on 2.1.5

Bug Fixes
^^^^^^^^^^^^^^^
- Fix import issues in sanity-test and improve unit tests.
- Fix parameter-list-no-elements error in sanity-test.
- Add defaut value for enable_log param.
- Relicense the FortiOS Collection under GPLv3+.
- Fix syntax issue in python2.7.
- Use collection version number in the doc.
- Update the logic in check_legacy_fortiosapi.
- Fix the syntax error in the three wireless_controller_hotspot20 modules.

Release Galaxy 2.1.5
--------------------

Release Targets
^^^^^^^^^^^^^^^

FortiOS Galaxy 2.1.5 is based on 2.1.4

Features
^^^^^^^^^^^^^^^
- Support FortiOS 7.0.2, 7.0.3, 7.0.4, 7.0.5.

Bug Fixes
^^^^^^^^^^^^^^^
- Fix status issue in fortios_json_generic().
- Fix issues in version mismatch logic.
- Fix the issue of inconsistent data types in different schemas.

Release Galaxy 2.1.4
--------------------

Release Targets
^^^^^^^^^^^^^^^

FortiOS Galaxy 2.1.4 is based on 2.1.3

Bug Fixes
^^^^^^^^^^^^^^^
- Fix bugs in the function of compare_ip_address on check_mode.
- Fix bugs when adding new members in some modules.

Release Galaxy 2.1.3
--------------------

Release Targets
^^^^^^^^^^^^^^^

FortiOS Galaxy 2.1.3 is based on 2.1.2

Features
^^^^^^^^^^^^^^^
- Collect the current configurations of the modules and convert them into playbooks.
- Support member operation (delete/add extra members) on an object that has a list of members in it.
- Add real-world use cases in the example section for some configuration modules.
- Support selectors feature in ``fortios_monitor_fact`` and ``fortios_log_fact``.
- Support FortiOS 7.0.1.

Bug Fixes
^^^^^^^^^^^^^^^
- Fix the filters error when fetching multiple facts with selectors for a configuration module (Github issue #138 ).
- Fix the corner cases that response does not have status in it.
- Fix Github issue #134

Release Galaxy 2.1.2
--------------------

Release Targets
^^^^^^^^^^^^^^^

FortiOS Galaxy 2.1.2 is based on 2.1.1

Bug Fixes
^^^^^^^^^^^^^^^
- Fix a regression bug caused by non-required attributes.
- Fix an intentional exception for listed options.

Release Galaxy 2.1.1
--------------------

Release Targets
^^^^^^^^^^^^^^^

FortiOS Galaxy 2.1.1 is based on 2.1.0

Bug Fixes
^^^^^^^^^^^^^^^
- Fix the KeyError caused by non-required multi-value attributes in an object.

Release Galaxy 2.1.0
--------------------

Release Targets
^^^^^^^^^^^^^^^

FortiOS Galaxy 2.1.0 is based on 2.0.2

Features
^^^^^^^^^^^^^^^
- Support Fortios 7.0.
- Support Log APIs.
- New module fortios_monitor_fact.

Bug Fixes
^^^^^^^^^^^^^^^
- Fix the unexpected warning caused by optinal params in ``fortios_monitor_fact`` and ``fortios_monitor``.
- Disable check_mode feature from all global objects of configuration modules due to 'state' issue.
- Fix a bug in IP_PREFIX.match().
- Fix the issue that the ``server_type`` is not updated in ``fortios_system_central_management``.

Release Galaxy 2.0.2
--------------------

Release Targets
^^^^^^^^^^^^^^^

FortiOS Galaxy 2.0.2 is based on 2.0.1

Features
^^^^^^^^^^^^^^^
- Support ``check_mode`` in all cofigurationAPI-based modules.
- Improve ``fortios_configuration_fact`` to use multiple selectors concurrently.
- Support moving policy in ``firewall_central_snat_map``.
- Support filtering for fact gathering modules ``fortios_configuration_fact`` and ``fortios_monitor_fact``.
- Unify schemas for monitor API.

Bug Fixes
^^^^^^^^^^^^^^^
- Fix the authorization fails at log in with username and password in FOS7.0.
- Github Issue #103
- Github Issue #105

Release Galaxy 2.0.1
--------------------

Release Targets
^^^^^^^^^^^^^^^
FortiOS Galaxy is based on ``2.0.0``.

Features
^^^^^^^^^^^^^^^^^^
 - fixed ``pylint`` minor errors.

Release Galaxy 2.0.0
--------------------

Release Targets
^^^^^^^^^^^^^^^

FortiOS Galaxy 2.0.0 is a major ansible release for all v6.x.x FOS virtual and hardware platforms.

Features
^^^^^^^^^^^^^^^^^^
- Full support for gathering facts of both configuration(``fortios_configuration_fact``) and monitor(``fortios_monitor_fact``) objects or runtime data.
- Support for requesting Monitor API via module ``fortios_monitor``.
- Ported FortiOS generic module: ``fortios_json_generic``.
- Unified collections for all 6.x FOS releases, Ansible detects versioning mismatch at runtime.
- Explicit logging option: ``enable_log``.
- Deprecated second-layer ``state`` module parameter.

Compatibility Notes
^^^^^^^^^^^^^^^^^^^^^^^^^^^^^
As a major release, it semantically breaks backward compability, some modules are removed as new full-fledged replacements come into being.

- For deprecated modules, please find the alternatives in **Deprecated Modules** section.
- Other existing modules are kepted compatible.


Deprecated Modules
^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^

- ``fortios_facts``: find full selectors in modules ``fortios_configuration_fact`` and ``fortios_monitor_fact``.
- ``fortios_registration_forticare``: replaced by module ``fortios_monitor``, see selector ``add-license.registration.forticare``.
- ``fortios_registration_vdom``: replaced by module ``fortios_monitor``, see selector ``add-license.registration.vdom``.
- ``fortios_system_vmlicense``: replaced by module ``fortios_monitor``, see selector ``upload.system.vmlicense``.
- ``fortios_system_config_backup_restore``: it was a complexed module.
   - To backup the FOS system, use module ``fortios_monitor_fact`` and its selector ``system_config_backup``.
   - To restore the configuration, use module ``fortios_monitor`` and its selector ``restore.system.config``.


--------------

Legacy Multiversions Note(Prior to 2.0.0)
------------------------------------------
The FortiOS Galaxy namespace: ``fortinet.fortios`` hosts Ansible modules
for multiple FortiOS major releases.

A mismatched Ansible collection version for a FortiOS device can cause a
warning:

::

    [WARNING]: Ansible has detected version mismatch between FortOS system and galaxy, see more details by specifying option -vvv

you can find more details with ``-vvv`` option when running a
playbook:

::

        ...
        "version_check_warning": {
            "ansible_collection_version": "v6.0.0 (galaxy: 1.0.13)",
            "matched": false,
            "message": "Please follow steps in FortiOS versioning notes: https://ansible-galaxy-fortios-docs.readthedocs.io/en/latest/version.html",
            "system_version": "v6.2.0"
        }
        ...

**Simply installing a matched FortiOS collection can prevent potential
compatibility issues.**

Release Galaxy 1.1.9
--------------------

Release Targets
^^^^^^^^^^^^^^^

- fos\_v6.0.0/galaxy\_1.1.9

Bug Fixes
^^^^^^^^^

- Fix legacy module ``fortios_system_config_backup_restore``


Release Galaxy 1.1.6 … 1.1.8
-----------------------------

Release Targets
^^^^^^^^^^^^^^^
There are multiple Galaxy releases dedicated to different FortiOS major releases.

- fos\_v6.2.0/galaxy\_1.1.6
- fos\_v6.4.0/galaxy\_1.1.7
- fos\_v6.0.0/galaxy\_1.1.8

Bug Fixes
^^^^^^^^^

- Fixed module construction for legacy module ``fortios_facts``.
- Sorted selector list of module ``fortios_configuration_fact``.


Release Galaxy 1.1.3 … 1.1.5
-----------------------------

Release Targets
^^^^^^^^^^^^^^^
There are multiple Galaxy releases dedicated to different FortiOS major releases.

- fos\_v6.2.0/galaxy\_1.1.3
- fos\_v6.4.0/galaxy\_1.1.4
- fos\_v6.0.0/galaxy\_1.1.5

Bug Fixes
^^^^^^^^^

- Fixed a fatal error: ``mkey`` not recognized in plugin due to wrong naming convention.



Release Galaxy 1.1.0 … 1.1.2
-----------------------------

|

Release Targets
^^^^^^^^^^^^^^^
There are multiple Galaxy releases dedicated to different FortiOS major releases.

- fos\_v6.2.0/galaxy\_1.1.0
- fos\_v6.4.0/galaxy\_1.1.1
- fos\_v6.0.0/galaxy\_1.1.2


Features
^^^^^^^^

- Support check mode for modules.
- Deprecate ``fortiosapi`` legacy connection mode.
- Support access token based authentication.
- Fully support fact gathering for all configuration API (``fortios_configuration_fact``).
- Suport Ansible 2.10 base framework.
- Support moving objects to different orders (``fortios_firewall_policy``).

Bug Fixes
^^^^^^^^^

- Github Issue #65

Release Galaxy 1.0.10 … 10.0.13
-------------------------------

|

Release Targets
^^^^^^^^^^^^^^^
There are multiple Galaxy releases dedicated to different FortiOS major releases.

-  fos\_v6.0.0/galaxy\_1.0.13
-  fos\_v6.0.5/galaxy\_1.0.12
-  fos\_v6.4.0/galaxy\_1.0.11
-  fos\_v6.2.0/galaxy\_1.0.10


New Modules
^^^^^^^^^^^

+-------+--------------------------------------------------------------+--------------+--------------+
| #     | Module Name                                                  | New in 6.2   | New in 6.4   |
+=======+==============================================================+==============+==============+
| 1     | ``fortios_cifs_domain_controller``                           | yes          | yes          |
+-------+--------------------------------------------------------------+--------------+--------------+
| 2     | ``fortios_cifs_profile``                                     | yes          | yes          |
+-------+--------------------------------------------------------------+--------------+--------------+
| 3     | ``fortios_dlp_sensitivity``                                  | yes          | yes          |
+-------+--------------------------------------------------------------+--------------+--------------+
| 4     | ``fortios_emailfilter_bwl``                                  | yes          | yes          |
+-------+--------------------------------------------------------------+--------------+--------------+
| 5     | ``fortios_emailfilter_bword``                                | yes          | yes          |
+-------+--------------------------------------------------------------+--------------+--------------+
| 6     | ``fortios_emailfilter_dnsbl``                                | yes          | yes          |
+-------+--------------------------------------------------------------+--------------+--------------+
| 7     | ``fortios_emailfilter_fortishield``                          | yes          | yes          |
+-------+--------------------------------------------------------------+--------------+--------------+
| 8     | ``fortios_emailfilter_iptrust``                              | yes          | yes          |
+-------+--------------------------------------------------------------+--------------+--------------+
| 9     | ``fortios_emailfilter_mheader``                              | yes          | yes          |
+-------+--------------------------------------------------------------+--------------+--------------+
| 10    | ``fortios_emailfilter_options``                              | yes          | yes          |
+-------+--------------------------------------------------------------+--------------+--------------+
| 11    | ``fortios_emailfilter_profile``                              | yes          | yes          |
+-------+--------------------------------------------------------------+--------------+--------------+
| 12    | ``fortios_endpoint_control_fctems``                          | yes          | yes          |
+-------+--------------------------------------------------------------+--------------+--------------+
| 13    | ``fortios_firewall_consolidated_policy``                     | yes          | yes          |
+-------+--------------------------------------------------------------+--------------+--------------+
| 14    | ``fortios_firewall_internet_service_addition``               | yes          | yes          |
+-------+--------------------------------------------------------------+--------------+--------------+
| 15    | ``fortios_firewall_internet_service_cat_definition``         | yes          | no           |
+-------+--------------------------------------------------------------+--------------+--------------+
| 16    | ``fortios_firewall_internet_service_definition``             | yes          | yes          |
+-------+--------------------------------------------------------------+--------------+--------------+
| 17    | ``fortios_firewall_internet_service_extension``              | yes          | yes          |
+-------+--------------------------------------------------------------+--------------+--------------+
| 18    | ``fortios_log_fortianalyzer2_override_filter``               | yes          | yes          |
+-------+--------------------------------------------------------------+--------------+--------------+
| 19    | ``fortios_log_fortianalyzer2_override_setting``              | yes          | yes          |
+-------+--------------------------------------------------------------+--------------+--------------+
| 20    | ``fortios_log_fortianalyzer3_override_filter``               | yes          | yes          |
+-------+--------------------------------------------------------------+--------------+--------------+
| 21    | ``fortios_log_fortianalyzer3_override_setting``              | yes          | yes          |
+-------+--------------------------------------------------------------+--------------+--------------+
| 22    | ``fortios_log_fortianalyzer_cloud_filter``                   | yes          | yes          |
+-------+--------------------------------------------------------------+--------------+--------------+
| 23    | ``fortios_log_fortianalyzer_cloud_override_filter``          | yes          | yes          |
+-------+--------------------------------------------------------------+--------------+--------------+
| 24    | ``fortios_log_fortianalyzer_cloud_override_setting``         | yes          | yes          |
+-------+--------------------------------------------------------------+--------------+--------------+
| 25    | ``fortios_log_fortianalyzer_cloud_setting``                  | yes          | yes          |
+-------+--------------------------------------------------------------+--------------+--------------+
| 26    | ``fortios_log_syslogd2_override_filter``                     | yes          | yes          |
+-------+--------------------------------------------------------------+--------------+--------------+
| 27    | ``fortios_log_syslogd2_override_setting``                    | yes          | yes          |
+-------+--------------------------------------------------------------+--------------+--------------+
| 28    | ``fortios_log_syslogd3_override_filter``                     | yes          | yes          |
+-------+--------------------------------------------------------------+--------------+--------------+
| 29    | ``fortios_log_syslogd3_override_setting``                    | yes          | yes          |
+-------+--------------------------------------------------------------+--------------+--------------+
| 30    | ``fortios_log_syslogd4_override_filter``                     | yes          | yes          |
+-------+--------------------------------------------------------------+--------------+--------------+
| 31    | ``fortios_log_syslogd4_override_setting``                    | yes          | yes          |
+-------+--------------------------------------------------------------+--------------+--------------+
| 32    | ``fortios_switch_controller_auto_config_custom``             | yes          | yes          |
+-------+--------------------------------------------------------------+--------------+--------------+
| 33    | ``fortios_switch_controller_auto_config_default``            | yes          | yes          |
+-------+--------------------------------------------------------------+--------------+--------------+
| 34    | ``fortios_switch_controller_auto_config_policy``             | yes          | yes          |
+-------+--------------------------------------------------------------+--------------+--------------+
| 35    | ``fortios_switch_controller_flow_tracking``                  | yes          | yes          |
+-------+--------------------------------------------------------------+--------------+--------------+
| 36    | ``fortios_switch_controller_location``                       | yes          | yes          |
+-------+--------------------------------------------------------------+--------------+--------------+
| 37    | ``fortios_switch_controller_security_policy_local_access``   | yes          | yes          |
+-------+--------------------------------------------------------------+--------------+--------------+
| 38    | ``fortios_switch_controller_storm_control_policy``           | yes          | yes          |
+-------+--------------------------------------------------------------+--------------+--------------+
| 39    | ``fortios_switch_controller_stp_instance``                   | yes          | yes          |
+-------+--------------------------------------------------------------+--------------+--------------+
| 40    | ``fortios_switch_controller_traffic_policy``                 | yes          | yes          |
+-------+--------------------------------------------------------------+--------------+--------------+
| 41    | ``fortios_switch_controller_traffic_sniffer``                | yes          | yes          |
+-------+--------------------------------------------------------------+--------------+--------------+
| 42    | ``fortios_system_ipsec_aggregate``                           | yes          | yes          |
+-------+--------------------------------------------------------------+--------------+--------------+
| 43    | ``fortios_system_lldp_network_policy``                       | yes          | yes          |
+-------+--------------------------------------------------------------+--------------+--------------+
| 44    | ``fortios_system_nd_proxy``                                  | yes          | yes          |
+-------+--------------------------------------------------------------+--------------+--------------+
| 45    | ``fortios_system_npu``                                       | yes          | yes          |
+-------+--------------------------------------------------------------+--------------+--------------+
| 46    | ``fortios_system_ptp``                                       | yes          | yes          |
+-------+--------------------------------------------------------------+--------------+--------------+
| 47    | ``fortios_system_saml``                                      | yes          | yes          |
+-------+--------------------------------------------------------------+--------------+--------------+
| 48    | ``fortios_system_speed_test_server``                         | yes          | yes          |
+-------+--------------------------------------------------------------+--------------+--------------+
| 49    | ``fortios_system_sso_admin``                                 | yes          | yes          |
+-------+--------------------------------------------------------------+--------------+--------------+
| 50    | ``fortios_user_exchange``                                    | yes          | yes          |
+-------+--------------------------------------------------------------+--------------+--------------+
| 51    | ``fortios_wireless_controller_address``                      | yes          | yes          |
+-------+--------------------------------------------------------------+--------------+--------------+
| 52    | ``fortios_wireless_controller_addrgrp``                      | yes          | yes          |
+-------+--------------------------------------------------------------+--------------+--------------+
| 53    | ``fortios_wireless_controller_log``                          | yes          | yes          |
+-------+--------------------------------------------------------------+--------------+--------------+
| 54    | ``fortios_wireless_controller_region``                       | yes          | yes          |
+-------+--------------------------------------------------------------+--------------+--------------+
| 55    | ``fortios_wireless_controller_snmp``                         | yes          | yes          |
+-------+--------------------------------------------------------------+--------------+--------------+
| 56    | ``fortios_certificate_remote``                               | no           | yes          |
+-------+--------------------------------------------------------------+--------------+--------------+
| 57    | ``fortios_credential_store_domain_controller``               | no           | yes          |
+-------+--------------------------------------------------------------+--------------+--------------+
| 58    | ``fortios_dpdk_cpus``                                        | no           | yes          |
+-------+--------------------------------------------------------------+--------------+--------------+
| 59    | ``fortios_dpdk_global``                                      | no           | yes          |
+-------+--------------------------------------------------------------+--------------+--------------+
| 60    | ``fortios_extender_modem_status``                            | no           | yes          |
+-------+--------------------------------------------------------------+--------------+--------------+
| 61    | ``fortios_extender_sys_info``                                | no           | yes          |
+-------+--------------------------------------------------------------+--------------+--------------+
| 62    | ``fortios_firewall_city``                                    | no           | yes          |
+-------+--------------------------------------------------------------+--------------+--------------+
| 63    | ``fortios_firewall_country``                                 | no           | yes          |
+-------+--------------------------------------------------------------+--------------+--------------+
| 64    | ``fortios_firewall_decrypted_traffic_mirror``                | no           | yes          |
+-------+--------------------------------------------------------------+--------------+--------------+
| 65    | ``fortios_firewall_internet_service_botnet``                 | no           | yes          |
+-------+--------------------------------------------------------------+--------------+--------------+
| 66    | ``fortios_firewall_internet_service_ipbl_reason``            | no           | yes          |
+-------+--------------------------------------------------------------+--------------+--------------+
| 67    | ``fortios_firewall_internet_service_ipbl_vendor``            | no           | yes          |
+-------+--------------------------------------------------------------+--------------+--------------+
| 68    | ``fortios_firewall_internet_service_list``                   | no           | yes          |
+-------+--------------------------------------------------------------+--------------+--------------+
| 69    | ``fortios_firewall_internet_service_name``                   | no           | yes          |
+-------+--------------------------------------------------------------+--------------+--------------+
| 70    | ``fortios_firewall_internet_service_owner``                  | no           | yes          |
+-------+--------------------------------------------------------------+--------------+--------------+
| 71    | ``fortios_firewall_internet_service_reputation``             | no           | yes          |
+-------+--------------------------------------------------------------+--------------+--------------+
| 72    | ``fortios_firewall_internet_service_sld``                    | no           | yes          |
+-------+--------------------------------------------------------------+--------------+--------------+
| 73    | ``fortios_firewall_iprope_list``                             | no           | yes          |
+-------+--------------------------------------------------------------+--------------+--------------+
| 74    | ``fortios_firewall_proute``                                  | no           | yes          |
+-------+--------------------------------------------------------------+--------------+--------------+
| 75    | ``fortios_firewall_region``                                  | no           | yes          |
+-------+--------------------------------------------------------------+--------------+--------------+
| 76    | ``fortios_firewall_security_policy``                         | no           | yes          |
+-------+--------------------------------------------------------------+--------------+--------------+
| 77    | ``fortios_firewall_traffic_class``                           | no           | yes          |
+-------+--------------------------------------------------------------+--------------+--------------+
| 78    | ``fortios_firewall_vendor_mac``                              | no           | yes          |
+-------+--------------------------------------------------------------+--------------+--------------+
| 79    | ``fortios_hardware_nic``                                     | no           | yes          |
+-------+--------------------------------------------------------------+--------------+--------------+
| 80    | ``fortios_ips_view_map``                                     | no           | yes          |
+-------+--------------------------------------------------------------+--------------+--------------+
| 81    | ``fortios_switch_controller_initial_config_template``        | no           | yes          |
+-------+--------------------------------------------------------------+--------------+--------------+
| 82    | ``fortios_switch_controller_initial_config_vlans``           | no           | yes          |
+-------+--------------------------------------------------------------+--------------+--------------+
| 83    | ``fortios_switch_controller_mac_policy``                     | no           | yes          |
+-------+--------------------------------------------------------------+--------------+--------------+
| 84    | ``fortios_switch_controller_nac_device``                     | no           | yes          |
+-------+--------------------------------------------------------------+--------------+--------------+
| 85    | ``fortios_switch_controller_nac_settings``                   | no           | yes          |
+-------+--------------------------------------------------------------+--------------+--------------+
| 86    | ``fortios_switch_controller_poe``                            | no           | yes          |
+-------+--------------------------------------------------------------+--------------+--------------+
| 87    | ``fortios_switch_controller_port_policy``                    | no           | yes          |
+-------+--------------------------------------------------------------+--------------+--------------+
| 88    | ``fortios_switch_controller_remote_log``                     | no           | yes          |
+-------+--------------------------------------------------------------+--------------+--------------+
| 89    | ``fortios_switch_controller_snmp_community``                 | no           | yes          |
+-------+--------------------------------------------------------------+--------------+--------------+
| 90    | ``fortios_switch_controller_snmp_sysinfo``                   | no           | yes          |
+-------+--------------------------------------------------------------+--------------+--------------+
| 91    | ``fortios_switch_controller_snmp_trap_threshold``            | no           | yes          |
+-------+--------------------------------------------------------------+--------------+--------------+
| 92    | ``fortios_switch_controller_snmp_user``                      | no           | yes          |
+-------+--------------------------------------------------------------+--------------+--------------+
| 93    | ``fortios_switch_controller_vlan_policy``                    | no           | yes          |
+-------+--------------------------------------------------------------+--------------+--------------+
| 94    | ``fortios_system_geneve``                                    | no           | yes          |
+-------+--------------------------------------------------------------+--------------+--------------+
| 95    | ``fortios_system_geoip_country``                             | no           | yes          |
+-------+--------------------------------------------------------------+--------------+--------------+
| 96    | ``fortios_system_performance_top``                           | no           | yes          |
+-------+--------------------------------------------------------------+--------------+--------------+
| 97    | ``fortios_system_standalone_cluster``                        | no           | yes          |
+-------+--------------------------------------------------------------+--------------+--------------+
| 98    | ``fortios_test_acd``                                         | no           | yes          |
+-------+--------------------------------------------------------------+--------------+--------------+
| 99    | ``fortios_test_acid``                                        | no           | yes          |
+-------+--------------------------------------------------------------+--------------+--------------+
| 100   | ``fortios_test_autod``                                       | no           | yes          |
+-------+--------------------------------------------------------------+--------------+--------------+
| 101   | ``fortios_test_awsd``                                        | no           | yes          |
+-------+--------------------------------------------------------------+--------------+--------------+
| 102   | ``fortios_test_azd``                                         | no           | yes          |
+-------+--------------------------------------------------------------+--------------+--------------+
| 103   | ``fortios_test_bfd``                                         | no           | yes          |
+-------+--------------------------------------------------------------+--------------+--------------+
| 104   | ``fortios_test_csfd``                                        | no           | yes          |
+-------+--------------------------------------------------------------+--------------+--------------+
| 105   | ``fortios_test_ddnscd``                                      | no           | yes          |
+-------+--------------------------------------------------------------+--------------+--------------+
| 106   | ``fortios_test_dhcp6c``                                      | no           | yes          |
+-------+--------------------------------------------------------------+--------------+--------------+
| 107   | ``fortios_test_dhcp6r``                                      | no           | yes          |
+-------+--------------------------------------------------------------+--------------+--------------+
| 108   | ``fortios_test_dhcprelay``                                   | no           | yes          |
+-------+--------------------------------------------------------------+--------------+--------------+
| 109   | ``fortios_test_dlpfingerprint``                              | no           | yes          |
+-------+--------------------------------------------------------------+--------------+--------------+
| 110   | ``fortios_test_dlpfpcache``                                  | no           | yes          |
+-------+--------------------------------------------------------------+--------------+--------------+
| 111   | ``fortios_test_dnsproxy``                                    | no           | yes          |
+-------+--------------------------------------------------------------+--------------+--------------+
| 112   | ``fortios_test_dsd``                                         | no           | yes          |
+-------+--------------------------------------------------------------+--------------+--------------+
| 113   | ``fortios_test_fas``                                         | no           | yes          |
+-------+--------------------------------------------------------------+--------------+--------------+
| 114   | ``fortios_test_fcnacd``                                      | no           | yes          |
+-------+--------------------------------------------------------------+--------------+--------------+
| 115   | ``fortios_test_fnbamd``                                      | no           | yes          |
+-------+--------------------------------------------------------------+--------------+--------------+
| 116   | ``fortios_test_forticldd``                                   | no           | yes          |
+-------+--------------------------------------------------------------+--------------+--------------+
| 117   | ``fortios_test_forticron``                                   | no           | yes          |
+-------+--------------------------------------------------------------+--------------+--------------+
| 118   | ``fortios_test_fsd``                                         | no           | yes          |
+-------+--------------------------------------------------------------+--------------+--------------+
| 119   | ``fortios_test_fsvrd``                                       | no           | yes          |
+-------+--------------------------------------------------------------+--------------+--------------+
| 120   | ``fortios_test_ftpd``                                        | no           | yes          |
+-------+--------------------------------------------------------------+--------------+--------------+
| 121   | ``fortios_test_gcpd``                                        | no           | yes          |
+-------+--------------------------------------------------------------+--------------+--------------+
| 122   | ``fortios_test_harelay``                                     | no           | yes          |
+-------+--------------------------------------------------------------+--------------+--------------+
| 123   | ``fortios_test_hasync``                                      | no           | yes          |
+-------+--------------------------------------------------------------+--------------+--------------+
| 124   | ``fortios_test_hatalk``                                      | no           | yes          |
+-------+--------------------------------------------------------------+--------------+--------------+
| 125   | ``fortios_test_imap``                                        | no           | yes          |
+-------+--------------------------------------------------------------+--------------+--------------+
| 126   | ``fortios_test_info_sslvpnd``                                | no           | yes          |
+-------+--------------------------------------------------------------+--------------+--------------+
| 127   | ``fortios_test_init``                                        | no           | yes          |
+-------+--------------------------------------------------------------+--------------+--------------+
| 128   | ``fortios_test_iotd``                                        | no           | yes          |
+-------+--------------------------------------------------------------+--------------+--------------+
| 129   | ``fortios_test_ipamd``                                       | no           | yes          |
+-------+--------------------------------------------------------------+--------------+--------------+
| 130   | ``fortios_test_ipldbd``                                      | no           | yes          |
+-------+--------------------------------------------------------------+--------------+--------------+
| 131   | ``fortios_test_ipsengine``                                   | no           | yes          |
+-------+--------------------------------------------------------------+--------------+--------------+
| 132   | ``fortios_test_ipsmonitor``                                  | no           | yes          |
+-------+--------------------------------------------------------------+--------------+--------------+
| 133   | ``fortios_test_ipsufd``                                      | no           | yes          |
+-------+--------------------------------------------------------------+--------------+--------------+
| 134   | ``fortios_test_kubed``                                       | no           | yes          |
+-------+--------------------------------------------------------------+--------------+--------------+
| 135   | ``fortios_test_l2tpcd``                                      | no           | yes          |
+-------+--------------------------------------------------------------+--------------+--------------+
| 136   | ``fortios_test_lnkmtd``                                      | no           | yes          |
+-------+--------------------------------------------------------------+--------------+--------------+
| 137   | ``fortios_test_lted``                                        | no           | yes          |
+-------+--------------------------------------------------------------+--------------+--------------+
| 138   | ``fortios_test_miglogd``                                     | no           | yes          |
+-------+--------------------------------------------------------------+--------------+--------------+
| 139   | ``fortios_test_mrd``                                         | no           | yes          |
+-------+--------------------------------------------------------------+--------------+--------------+
| 140   | ``fortios_test_netxd``                                       | no           | yes          |
+-------+--------------------------------------------------------------+--------------+--------------+
| 141   | ``fortios_test_nntp``                                        | no           | yes          |
+-------+--------------------------------------------------------------+--------------+--------------+
| 142   | ``fortios_test_ocid``                                        | no           | yes          |
+-------+--------------------------------------------------------------+--------------+--------------+
| 143   | ``fortios_test_openstackd``                                  | no           | yes          |
+-------+--------------------------------------------------------------+--------------+--------------+
| 144   | ``fortios_test_ovrd``                                        | no           | yes          |
+-------+--------------------------------------------------------------+--------------+--------------+
| 145   | ``fortios_test_pop3``                                        | no           | yes          |
+-------+--------------------------------------------------------------+--------------+--------------+
| 146   | ``fortios_test_pptpcd``                                      | no           | yes          |
+-------+--------------------------------------------------------------+--------------+--------------+
| 147   | ``fortios_test_quarantined``                                 | no           | yes          |
+-------+--------------------------------------------------------------+--------------+--------------+
| 148   | ``fortios_test_radius_das``                                  | no           | yes          |
+-------+--------------------------------------------------------------+--------------+--------------+
| 149   | ``fortios_test_radiusd``                                     | no           | yes          |
+-------+--------------------------------------------------------------+--------------+--------------+
| 150   | ``fortios_test_radvd``                                       | no           | yes          |
+-------+--------------------------------------------------------------+--------------+--------------+
| 151   | ``fortios_test_reportd``                                     | no           | yes          |
+-------+--------------------------------------------------------------+--------------+--------------+
| 152   | ``fortios_test_sdncd``                                       | no           | yes          |
+-------+--------------------------------------------------------------+--------------+--------------+
| 153   | ``fortios_test_sepmd``                                       | no           | yes          |
+-------+--------------------------------------------------------------+--------------+--------------+
| 154   | ``fortios_test_sessionsync``                                 | no           | yes          |
+-------+--------------------------------------------------------------+--------------+--------------+
| 155   | ``fortios_test_sflowd``                                      | no           | yes          |
+-------+--------------------------------------------------------------+--------------+--------------+
| 156   | ``fortios_test_smtp``                                        | no           | yes          |
+-------+--------------------------------------------------------------+--------------+--------------+
| 157   | ``fortios_test_snmpd``                                       | no           | yes          |
+-------+--------------------------------------------------------------+--------------+--------------+
| 158   | ``fortios_test_uploadd``                                     | no           | yes          |
+-------+--------------------------------------------------------------+--------------+--------------+
| 159   | ``fortios_test_urlfilter``                                   | no           | yes          |
+-------+--------------------------------------------------------------+--------------+--------------+
| 160   | ``fortios_test_vmwd``                                        | no           | yes          |
+-------+--------------------------------------------------------------+--------------+--------------+
| 161   | ``fortios_test_wad``                                         | no           | yes          |
+-------+--------------------------------------------------------------+--------------+--------------+
| 162   | ``fortios_test_wccpd``                                       | no           | yes          |
+-------+--------------------------------------------------------------+--------------+--------------+
| 163   | ``fortios_test_wf_monitor``                                  | no           | yes          |
+-------+--------------------------------------------------------------+--------------+--------------+
| 164   | ``fortios_test_zebos_launcher``                              | no           | yes          |
+-------+--------------------------------------------------------------+--------------+--------------+
| 165   | ``fortios_user_nac_policy``                                  | no           | yes          |
+-------+--------------------------------------------------------------+--------------+--------------+
| 166   | ``fortios_user_saml``                                        | no           | yes          |
+-------+--------------------------------------------------------------+--------------+--------------+
| 167   | ``fortios_vpn_ike_gateway``                                  | no           | yes          |
+-------+--------------------------------------------------------------+--------------+--------------+
| 168   | ``fortios_webfilter_status``                                 | no           | yes          |
+-------+--------------------------------------------------------------+--------------+--------------+
| 169   | ``fortios_wireless_controller_access_control_list``          | no           | yes          |
+-------+--------------------------------------------------------------+--------------+--------------+
| 170   | ``fortios_wireless_controller_apcfg_profile``                | no           | yes          |
+-------+--------------------------------------------------------------+--------------+--------------+
| 171   | ``fortios_wireless_controller_client_info``                  | no           | yes          |
+-------+--------------------------------------------------------------+--------------+--------------+
| 172   | ``fortios_wireless_controller_rf_analysis``                  | no           | yes          |
+-------+--------------------------------------------------------------+--------------+--------------+
| 173   | ``fortios_wireless_controller_spectral_info``                | no           | yes          |
+-------+--------------------------------------------------------------+--------------+--------------+
| 174   | ``fortios_wireless_controller_status``                       | no           | yes          |
+-------+--------------------------------------------------------------+--------------+--------------+
| 175   | ``fortios_wireless_controller_vap_status``                   | no           | yes          |
+-------+--------------------------------------------------------------+--------------+--------------+
| 176   | ``fortios_wireless_controller_wag_profile``                  | no           | yes          |
+-------+--------------------------------------------------------------+--------------+--------------+
| 177   | ``fortios_wireless_controller_wtp_status``                   | no           | yes          |
+-------+--------------------------------------------------------------+--------------+--------------+

Features
^^^^^^^^

-  Support special identifier validation and restoration in Ansible
   modules.
-  Support more valid identifiers: ``3gpp_plmn``, ``802_1X_settings``,
   ``802.1_tlvs`` and ``802.3_tlvs``.
-  Support ``revision_change`` in response since fortigate 6.2.3.
-  Support Underscore to hypen conversion.
-  Support licence modules: ``fortios_system_vmlicense``,
   ``fortios_registration_forticare`` and ``fortios_registration_vdom``.
-  Support raw json encoding for generic module.

Bug Fixes
^^^^^^^^^

-  Fix ``fgd_alert_subscription`` multiple choices problem for module
   ``fortios_system_global``.
-  Fix ``proposal`` exceptional multilist for module
   ``fortios_vpn_ipsec_phase2_interface``.
-  Fix issue #26 of ansible\_fgt\_modules.
-  Fix issue #24 of ansible\_fgt\_modules.
-  Fix ``events`` exceptional multilist for module
   ``fortios_system_snmp_community``.
-  Fix py2/py3 compability issue for httpapi plugin fortios.
-  Fix the mkey encoding in fortios api URL.
-  Fix ``banned_cipher`` exceptional multilist for module
   ``fortios_vpn_ssl_settings``.



