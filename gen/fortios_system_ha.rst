:source: fortios_system_ha.py

:orphan:

.. fortios_system_ha:

fortios_system_ha -- Configure HA in Fortinet's FortiOS and FortiGate.
++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++

.. versionadded:: 2.9

.. contents::
   :local:
   :depth: 1


Synopsis
--------
- This module is able to configure a FortiGate or FortiOS (FOS) device by allowing the user to set and modify system feature and ha category. Examples include all parameters and values need to be adjusted to datasources before usage. Tested with FOS v6.0.5



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
    <li> <span class="li-head">system_ha</span> - Configure HA. <span class="li-normal">type: dict</span></li>
        <ul class="ul-self">
        <li> <span class="li-head">arps</span> - Number of gratuitous ARPs (1 - 60). Lower to reduce traffic. Higher to reduce failover time. <span class="li-normal">type: int</span></li>
        <li> <span class="li-head">arps_interval</span> - Time between gratuitous ARPs  (1 - 20 sec). Lower to reduce failover time. Higher to reduce traffic. <span class="li-normal">type: int</span></li>
        <li> <span class="li-head">authentication</span> - Enable/disable heartbeat message authentication. <span class="li-normal">type: str</span> <span class="li-normal">choices: enable, disable</span></li>
        <li> <span class="li-head">cpu_threshold</span> - Dynamic weighted load balancing CPU usage weight and high and low thresholds. <span class="li-normal">type: str</span></li>
        <li> <span class="li-head">encryption</span> - Enable/disable heartbeat message encryption. <span class="li-normal">type: str</span> <span class="li-normal">choices: enable, disable</span></li>
        <li> <span class="li-head">ftp_proxy_threshold</span> - Dynamic weighted load balancing weight and high and low number of FTP proxy sessions. <span class="li-normal">type: str</span></li>
        <li> <span class="li-head">gratuitous_arps</span> - Enable/disable gratuitous ARPs. Disable if link-failed-signal enabled. <span class="li-normal">type: str</span> <span class="li-normal">choices: enable, disable</span></li>
        <li> <span class="li-head">group_id</span> - Cluster group ID  (0 - 255). Must be the same for all members. <span class="li-normal">type: int</span></li>
        <li> <span class="li-head">group_name</span> - Cluster group name. Must be the same for all members. <span class="li-normal">type: str</span></li>
        <li> <span class="li-head">ha_direct</span> - Enable/disable using ha-mgmt interface for syslog, SNMP, remote authentication (RADIUS), FortiAnalyzer, and FortiSandbox. <span class="li-normal">type: str</span> <span class="li-normal">choices: enable, disable</span></li>
        <li> <span class="li-head">ha_eth_type</span> - HA heartbeat packet Ethertype (4-digit hex). <span class="li-normal">type: str</span></li>
        <li> <span class="li-head">ha_mgmt_interfaces</span> - Reserve interfaces to manage individual cluster units. <span class="li-normal">type: list</span></li>
            <ul class="ul-self">
            <li> <span class="li-head">dst</span> - Default route destination for reserved HA management interface. <span class="li-normal">type: str</span></li>
            <li> <span class="li-head">gateway</span> - Default route gateway for reserved HA management interface. <span class="li-normal">type: str</span></li>
            <li> <span class="li-head">gateway6</span> - Default IPv6 gateway for reserved HA management interface. <span class="li-normal">type: str</span></li>
            <li> <span class="li-head">id</span> - Table ID. <span class="li-normal">type: int</span> <span class="li-required">required: True</span></li>
            <li> <span class="li-head">interface</span> - Interface to reserve for HA management. Source system.interface.name. <span class="li-normal">type: str</span></li>
            </ul>
        <li> <span class="li-head">ha_mgmt_status</span> - Enable to reserve interfaces to manage individual cluster units. <span class="li-normal">type: str</span> <span class="li-normal">choices: enable, disable</span></li>
        <li> <span class="li-head">ha_uptime_diff_margin</span> - Normally you would only reduce this value for failover testing. <span class="li-normal">type: int</span></li>
        <li> <span class="li-head">hb_interval</span> - Time between sending heartbeat packets (1 - 20 (100*ms)). Increase to reduce false positives. <span class="li-normal">type: int</span></li>
        <li> <span class="li-head">hb_lost_threshold</span> - Number of lost heartbeats to signal a failure (1 - 60). Increase to reduce false positives. <span class="li-normal">type: int</span></li>
        <li> <span class="li-head">hbdev</span> - Heartbeat interfaces. Must be the same for all members. <span class="li-normal">type: str</span></li>
        <li> <span class="li-head">hc_eth_type</span> - Transparent mode HA heartbeat packet Ethertype (4-digit hex). <span class="li-normal">type: str</span></li>
        <li> <span class="li-head">hello_holddown</span> - Time to wait before changing from hello to work state (5 - 300 sec). <span class="li-normal">type: int</span></li>
        <li> <span class="li-head">http_proxy_threshold</span> - Dynamic weighted load balancing weight and high and low number of HTTP proxy sessions. <span class="li-normal">type: str</span></li>
        <li> <span class="li-head">imap_proxy_threshold</span> - Dynamic weighted load balancing weight and high and low number of IMAP proxy sessions. <span class="li-normal">type: str</span></li>
        <li> <span class="li-head">inter_cluster_session_sync</span> - Enable/disable synchronization of sessions among HA clusters. <span class="li-normal">type: str</span> <span class="li-normal">choices: enable, disable</span></li>
        <li> <span class="li-head">key</span> - key <span class="li-normal">type: str</span></li>
        <li> <span class="li-head">l2ep_eth_type</span> - Telnet session HA heartbeat packet Ethertype (4-digit hex). <span class="li-normal">type: str</span></li>
        <li> <span class="li-head">link_failed_signal</span> - Enable to shut down all interfaces for 1 sec after a failover. Use if gratuitous ARPs do not update network. <span class="li-normal">type: str</span> <span class="li-normal">choices: enable, disable</span></li>
        <li> <span class="li-head">load_balance_all</span> - Enable to load balance TCP sessions. Disable to load balance proxy sessions only. <span class="li-normal">type: str</span> <span class="li-normal">choices: enable, disable</span></li>
        <li> <span class="li-head">memory_compatible_mode</span> - Enable/disable memory compatible mode. <span class="li-normal">type: str</span> <span class="li-normal">choices: enable, disable</span></li>
        <li> <span class="li-head">memory_threshold</span> - Dynamic weighted load balancing memory usage weight and high and low thresholds. <span class="li-normal">type: str</span></li>
        <li> <span class="li-head">mode</span> - HA mode. Must be the same for all members. FGSP requires standalone. <span class="li-normal">type: str</span> <span class="li-normal">choices: standalone, a-a, a-p</span></li>
        <li> <span class="li-head">monitor</span> - Interfaces to check for port monitoring (or link failure). Source system.interface.name. <span class="li-normal">type: str</span></li>
        <li> <span class="li-head">multicast_ttl</span> - HA multicast TTL on master (5 - 3600 sec). <span class="li-normal">type: int</span></li>
        <li> <span class="li-head">nntp_proxy_threshold</span> - Dynamic weighted load balancing weight and high and low number of NNTP proxy sessions. <span class="li-normal">type: str</span></li>
        <li> <span class="li-head">override</span> - Enable and increase the priority of the unit that should always be primary (master). <span class="li-normal">type: str</span> <span class="li-normal">choices: enable, disable</span></li>
        <li> <span class="li-head">override_wait_time</span> - Delay negotiating if override is enabled (0 - 3600 sec). Reduces how often the cluster negotiates. <span class="li-normal">type: int</span></li>
        <li> <span class="li-head">password</span> - Cluster password. Must be the same for all members. <span class="li-normal">type: str</span></li>
        <li> <span class="li-head">pingserver_failover_threshold</span> - Remote IP monitoring failover threshold (0 - 50). <span class="li-normal">type: int</span></li>
        <li> <span class="li-head">pingserver_flip_timeout</span> - Time to wait in minutes before renegotiating after a remote IP monitoring failover. <span class="li-normal">type: int</span></li>
        <li> <span class="li-head">pingserver_monitor_interface</span> - Interfaces to check for remote IP monitoring. Source system.interface.name. <span class="li-normal">type: str</span></li>
        <li> <span class="li-head">pingserver_slave_force_reset</span> - Enable to force the cluster to negotiate after a remote IP monitoring failover. <span class="li-normal">type: str</span> <span class="li-normal">choices: enable, disable</span></li>
        <li> <span class="li-head">pop3_proxy_threshold</span> - Dynamic weighted load balancing weight and high and low number of POP3 proxy sessions. <span class="li-normal">type: str</span></li>
        <li> <span class="li-head">priority</span> - Increase the priority to select the primary unit (0 - 255). <span class="li-normal">type: int</span></li>
        <li> <span class="li-head">route_hold</span> - Time to wait between routing table updates to the cluster (0 - 3600 sec). <span class="li-normal">type: int</span></li>
        <li> <span class="li-head">route_ttl</span> - TTL for primary unit routes (5 - 3600 sec). Increase to maintain active routes during failover. <span class="li-normal">type: int</span></li>
        <li> <span class="li-head">route_wait</span> - Time to wait before sending new routes to the cluster (0 - 3600 sec). <span class="li-normal">type: int</span></li>
        <li> <span class="li-head">schedule</span> - Type of A-A load balancing. Use none if you have external load balancers. <span class="li-normal">type: str</span> <span class="li-normal">choices: none, hub, leastconnection, round-robin, weight-round-robin, random, ip, ipport</span></li>
        <li> <span class="li-head">secondary_vcluster</span> - Configure virtual cluster 2. <span class="li-normal">type: dict</span></li>
            <ul class="ul-self">
            <li> <span class="li-head">monitor</span> - Interfaces to check for port monitoring (or link failure). Source system.interface.name. <span class="li-normal">type: str</span></li>
            <li> <span class="li-head">override</span> - Enable and increase the priority of the unit that should always be primary (master). <span class="li-normal">type: str</span> <span class="li-normal">choices: enable, disable</span></li>
            <li> <span class="li-head">override_wait_time</span> - Delay negotiating if override is enabled (0 - 3600 sec). Reduces how often the cluster negotiates. <span class="li-normal">type: int</span></li>
            <li> <span class="li-head">pingserver_failover_threshold</span> - Remote IP monitoring failover threshold (0 - 50). <span class="li-normal">type: int</span></li>
            <li> <span class="li-head">pingserver_monitor_interface</span> - Interfaces to check for remote IP monitoring. Source system.interface.name. <span class="li-normal">type: str</span></li>
            <li> <span class="li-head">pingserver_slave_force_reset</span> - Enable to force the cluster to negotiate after a remote IP monitoring failover. <span class="li-normal">type: str</span> <span class="li-normal">choices: enable, disable</span></li>
            <li> <span class="li-head">priority</span> - Increase the priority to select the primary unit (0 - 255). <span class="li-normal">type: int</span></li>
            <li> <span class="li-head">vcluster_id</span> - Cluster ID. <span class="li-normal">type: int</span></li>
            <li> <span class="li-head">vdom</span> - VDOMs in virtual cluster 2. <span class="li-normal">type: str</span></li>
            </ul>
        <li> <span class="li-head">session_pickup</span> - Enable/disable session pickup. Enabling it can reduce session down time when fail over happens. <span class="li-normal">type: str</span> <span class="li-normal">choices: enable, disable</span></li>
        <li> <span class="li-head">session_pickup_connectionless</span> - Enable/disable UDP and ICMP session sync for FGSP. <span class="li-normal">type: str</span> <span class="li-normal">choices: enable, disable</span></li>
        <li> <span class="li-head">session_pickup_delay</span> - Enable to sync sessions longer than 30 sec. Only longer lived sessions need to be synced. <span class="li-normal">type: str</span> <span class="li-normal">choices: enable, disable</span></li>
        <li> <span class="li-head">session_pickup_expectation</span> - Enable/disable session helper expectation session sync for FGSP. <span class="li-normal">type: str</span> <span class="li-normal">choices: enable, disable</span></li>
        <li> <span class="li-head">session_pickup_nat</span> - Enable/disable NAT session sync for FGSP. <span class="li-normal">type: str</span> <span class="li-normal">choices: enable, disable</span></li>
        <li> <span class="li-head">session_sync_dev</span> - Offload session sync to one or more interfaces to distribute traffic and prevent delays if needed. Source system.interface.name. <span class="li-normal">type: str</span></li>
        <li> <span class="li-head">smtp_proxy_threshold</span> - Dynamic weighted load balancing weight and high and low number of SMTP proxy sessions. <span class="li-normal">type: str</span></li>
        <li> <span class="li-head">standalone_config_sync</span> - Enable/disable FGSP configuration synchronization. <span class="li-normal">type: str</span> <span class="li-normal">choices: enable, disable</span></li>
        <li> <span class="li-head">standalone_mgmt_vdom</span> - Enable/disable standalone management VDOM. <span class="li-normal">type: str</span> <span class="li-normal">choices: enable, disable</span></li>
        <li> <span class="li-head">sync_config</span> - Enable/disable configuration synchronization. <span class="li-normal">type: str</span> <span class="li-normal">choices: enable, disable</span></li>
        <li> <span class="li-head">sync_packet_balance</span> - Enable/disable HA packet distribution to multiple CPUs. <span class="li-normal">type: str</span> <span class="li-normal">choices: enable, disable</span></li>
        <li> <span class="li-head">unicast_hb</span> - Enable/disable unicast heartbeat. <span class="li-normal">type: str</span> <span class="li-normal">choices: enable, disable</span></li>
        <li> <span class="li-head">unicast_hb_netmask</span> - Unicast heartbeat netmask. <span class="li-normal">type: str</span></li>
        <li> <span class="li-head">unicast_hb_peerip</span> - Unicast heartbeat peer IP. <span class="li-normal">type: str</span></li>
        <li> <span class="li-head">uninterruptible_upgrade</span> - Enable to upgrade a cluster without blocking network traffic. <span class="li-normal">type: str</span> <span class="li-normal">choices: enable, disable</span></li>
        <li> <span class="li-head">vcluster_id</span> - Cluster ID. <span class="li-normal">type: int</span></li>
        <li> <span class="li-head">vcluster2</span> - Enable/disable virtual cluster 2 for virtual clustering. <span class="li-normal">type: str</span> <span class="li-normal">choices: enable, disable</span></li>
        <li> <span class="li-head">vdom</span> - VDOMs in virtual cluster 1. <span class="li-normal">type: str</span></li>
        <li> <span class="li-head">weight</span> - Weight-round-robin weight for each cluster unit. Syntax <priority> <weight>. <span class="li-normal">type: str</span></li>
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
      - name: Configure HA.
        fortios_system_ha:
          vdom:  "{{ vdom }}"
          system_ha:
            arps: "3"
            arps_interval: "4"
            authentication: "enable"
            cpu_threshold: "<your_own_value>"
            encryption: "enable"
            ftp_proxy_threshold: "<your_own_value>"
            gratuitous_arps: "enable"
            group_id: "10"
            group_name: "<your_own_value>"
            ha_direct: "enable"
            ha_eth_type: "<your_own_value>"
            ha_mgmt_interfaces:
             -
                dst: "<your_own_value>"
                gateway: "<your_own_value>"
                gateway6: "<your_own_value>"
                id:  "18"
                interface: "<your_own_value> (source system.interface.name)"
            ha_mgmt_status: "enable"
            ha_uptime_diff_margin: "21"
            hb_interval: "22"
            hb_lost_threshold: "23"
            hbdev: "<your_own_value>"
            hc_eth_type: "<your_own_value>"
            hello_holddown: "26"
            http_proxy_threshold: "<your_own_value>"
            imap_proxy_threshold: "<your_own_value>"
            inter_cluster_session_sync: "enable"
            key: "<your_own_value>"
            l2ep_eth_type: "<your_own_value>"
            link_failed_signal: "enable"
            load_balance_all: "enable"
            memory_compatible_mode: "enable"
            memory_threshold: "<your_own_value>"
            mode: "standalone"
            monitor: "<your_own_value> (source system.interface.name)"
            multicast_ttl: "38"
            nntp_proxy_threshold: "<your_own_value>"
            override: "enable"
            override_wait_time: "41"
            password: "<your_own_value>"
            pingserver_failover_threshold: "43"
            pingserver_flip_timeout: "44"
            pingserver_monitor_interface: "<your_own_value> (source system.interface.name)"
            pingserver_slave_force_reset: "enable"
            pop3_proxy_threshold: "<your_own_value>"
            priority: "48"
            route_hold: "49"
            route_ttl: "50"
            route_wait: "51"
            schedule: "none"
            secondary_vcluster:
                monitor: "<your_own_value> (source system.interface.name)"
                override: "enable"
                override_wait_time: "56"
                pingserver_failover_threshold: "57"
                pingserver_monitor_interface: "<your_own_value> (source system.interface.name)"
                pingserver_slave_force_reset: "enable"
                priority: "60"
                vcluster_id: "61"
                vdom: "<your_own_value>"
            session_pickup: "enable"
            session_pickup_connectionless: "enable"
            session_pickup_delay: "enable"
            session_pickup_expectation: "enable"
            session_pickup_nat: "enable"
            session_sync_dev: "<your_own_value> (source system.interface.name)"
            smtp_proxy_threshold: "<your_own_value>"
            standalone_config_sync: "enable"
            standalone_mgmt_vdom: "enable"
            sync_config: "enable"
            sync_packet_balance: "enable"
            unicast_hb: "enable"
            unicast_hb_netmask: "<your_own_value>"
            unicast_hb_peerip: "<your_own_value>"
            uninterruptible_upgrade: "enable"
            vcluster_id: "78"
            vcluster2: "enable"
            vdom: "<your_own_value>"
            weight: "<your_own_value>"


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
