:source: fortios_system_cluster_sync.py

:orphan:

.. fortios_system_cluster_sync:

fortios_system_cluster_sync -- Configure FortiGate Session Life Support Protocol (FGSP) session synchronization in Fortinet's FortiOS and FortiGate.
++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++

.. versionadded:: 2.9

.. contents::
   :local:
   :depth: 1


Synopsis
--------
- This module is able to configure a FortiGate or FortiOS (FOS) device by allowing the user to set and modify system feature and cluster_sync category. Examples include all parameters and values need to be adjusted to datasources before usage. Tested with FOS v6.0.0



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
    <li> <span class="li-head">state</span> - Indicates whether to create or remove the object. <span class="li-normal">type: str</span> <span class="li-required">required: True</span> <span class="li-normal">choices: present, absent</span></li>
    <li> <span class="li-head">system_cluster_sync</span> - Configure FortiGate Session Life Support Protocol (FGSP) session synchronization. <span class="li-normal">type: dict</span></li>
        <ul class="ul-self">
        <li> <span class="li-head">down_intfs_before_sess_sync</span> - List of interfaces to be turned down before session synchronization is complete. <span class="li-normal">type: list</span></li>
            <ul class="ul-self">
            <li> <span class="li-head">name</span> - Interface name. Source system.interface.name. <span class="li-normal">type: str</span> <span class="li-required">required: True</span></li>
            </ul>
        <li> <span class="li-head">hb_interval</span> - Heartbeat interval (1 - 10 sec). <span class="li-normal">type: int</span></li>
        <li> <span class="li-head">hb_lost_threshold</span> - Lost heartbeat threshold (1 - 10). <span class="li-normal">type: int</span></li>
        <li> <span class="li-head">peerip</span> - IP address of the interface on the peer unit that is used for the session synchronization link. <span class="li-normal">type: str</span></li>
        <li> <span class="li-head">peervd</span> - VDOM that contains the session synchronization link interface on the peer unit. Usually both peers would have the same peervd. Source system.vdom.name. <span class="li-normal">type: str</span></li>
        <li> <span class="li-head">session_sync_filter</span> - Add one or more filters if you only want to synchronize some sessions. Use the filter to configure the types of sessions to synchronize. <span class="li-normal">type: dict</span></li>
            <ul class="ul-self">
            <li> <span class="li-head">custom_service</span> - Only sessions using these custom services are synchronized. Use source and destination port ranges to define these custome services. <span class="li-normal">type: list</span></li>
                <ul class="ul-self">
                <li> <span class="li-head">dst_port_range</span> - Custom service destination port range. <span class="li-normal">type: str</span></li>
                <li> <span class="li-head">id</span> - Custom service ID. <span class="li-normal">type: int</span> <span class="li-required">required: True</span></li>
                <li> <span class="li-head">src_port_range</span> - Custom service source port range. <span class="li-normal">type: str</span></li>
                </ul>
            <li> <span class="li-head">dstaddr</span> - Only sessions to this IPv4 address are synchronized. You can only enter one address. To synchronize sessions for multiple destination addresses, add multiple filters. <span class="li-normal">type: str</span></li>
            <li> <span class="li-head">dstaddr6</span> - Only sessions to this IPv6 address are synchronized. You can only enter one address. To synchronize sessions for multiple destination addresses, add multiple filters. <span class="li-normal">type: str</span></li>
            <li> <span class="li-head">dstintf</span> - Only sessions to this interface are synchronized. You can only enter one interface name. To synchronize sessions to multiple destination interfaces, add multiple filters. Source system.interface.name. <span class="li-normal">type: str</span></li>
            <li> <span class="li-head">srcaddr</span> - Only sessions from this IPv4 address are synchronized. You can only enter one address. To synchronize sessions from multiple source addresses, add multiple filters. <span class="li-normal">type: str</span></li>
            <li> <span class="li-head">srcaddr6</span> - Only sessions from this IPv6 address are synchronized. You can only enter one address. To synchronize sessions from multiple source addresses, add multiple filters. <span class="li-normal">type: str</span></li>
            <li> <span class="li-head">srcintf</span> - Only sessions from this interface are synchronized. You can only enter one interface name. To synchronize sessions for multiple source interfaces, add multiple filters. Source system.interface.name. <span class="li-normal">type: str</span></li>
            </ul>
        <li> <span class="li-head">slave_add_ike_routes</span> - Enable/disable IKE route announcement on the backup unit. <span class="li-normal">type: str</span> <span class="li-normal">choices: enable, disable</span></li>
        <li> <span class="li-head">sync_id</span> - Sync ID. <span class="li-normal">type: int</span></li>
        <li> <span class="li-head">syncvd</span> - Sessions from these VDOMs are synchronized using this session synchronization configuration. <span class="li-normal">type: list</span></li>
            <ul class="ul-self">
            <li> <span class="li-head">name</span> - VDOM name. Source system.vdom.name. <span class="li-normal">type: str</span> <span class="li-required">required: True</span></li>
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
      - name: Configure FortiGate Session Life Support Protocol (FGSP) session synchronization.
        fortios_system_cluster_sync:
          vdom:  "{{ vdom }}"
          state: "present"
          system_cluster_sync:
            down_intfs_before_sess_sync:
             -
                name: "default_name_4 (source system.interface.name)"
            hb_interval: "5"
            hb_lost_threshold: "6"
            peerip: "<your_own_value>"
            peervd: "<your_own_value> (source system.vdom.name)"
            session_sync_filter:
                custom_service:
                 -
                    dst_port_range: "<your_own_value>"
                    id:  "12"
                    src_port_range: "<your_own_value>"
                dstaddr: "<your_own_value>"
                dstaddr6: "<your_own_value>"
                dstintf: "<your_own_value> (source system.interface.name)"
                srcaddr: "<your_own_value>"
                srcaddr6: "<your_own_value>"
                srcintf: "<your_own_value> (source system.interface.name)"
            slave_add_ike_routes: "enable"
            sync_id: "21"
            syncvd:
             -
                name: "default_name_23 (source system.vdom.name)"


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
