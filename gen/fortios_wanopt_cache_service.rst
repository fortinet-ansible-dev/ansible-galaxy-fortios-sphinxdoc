:source: fortios_wanopt_cache_service.py

:orphan:

.. fortios_wanopt_cache_service:

fortios_wanopt_cache_service -- Designate cache-service for wan-optimization and webcache in Fortinet's FortiOS and FortiGate.
++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++

.. versionadded:: 2.9

.. contents::
   :local:
   :depth: 1


Synopsis
--------
- This module is able to configure a FortiGate or FortiOS (FOS) device by allowing the user to set and modify wanopt feature and cache_service category. Examples include all parameters and values need to be adjusted to datasources before usage. Tested with FOS v6.0.5



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
    <li> <span class="li-head">wanopt_cache_service</span> - Designate cache-service for wan-optimization and webcache. <span class="li-normal">type: dict</span></li>
        <ul class="ul-self">
        <li> <span class="li-head">acceptable_connections</span> - Set strategy when accepting cache collaboration connection. <span class="li-normal">type: str</span> <span class="li-normal">choices: any, peers</span></li>
        <li> <span class="li-head">collaboration</span> - Enable/disable cache-collaboration between cache-service clusters. <span class="li-normal">type: str</span> <span class="li-normal">choices: enable, disable</span></li>
        <li> <span class="li-head">device_id</span> - Set identifier for this cache device. <span class="li-normal">type: str</span></li>
        <li> <span class="li-head">dst_peer</span> - Modify cache-service destination peer list. <span class="li-normal">type: list</span></li>
            <ul class="ul-self">
            <li> <span class="li-head">auth_type</span> - Set authentication type for this peer. <span class="li-normal">type: int</span></li>
            <li> <span class="li-head">device_id</span> - Device ID of this peer. <span class="li-normal">type: str</span></li>
            <li> <span class="li-head">encode_type</span> - Set encode type for this peer. <span class="li-normal">type: int</span></li>
            <li> <span class="li-head">ip</span> - Set cluster IP address of this peer. <span class="li-normal">type: str</span></li>
            <li> <span class="li-head">priority</span> - Set priority for this peer. <span class="li-normal">type: int</span></li>
            </ul>
        <li> <span class="li-head">prefer_scenario</span> - Set the preferred cache behavior towards the balance between latency and hit-ratio. <span class="li-normal">type: str</span> <span class="li-normal">choices: balance, prefer-speed, prefer-cache</span></li>
        <li> <span class="li-head">src_peer</span> - Modify cache-service source peer list. <span class="li-normal">type: list</span></li>
            <ul class="ul-self">
            <li> <span class="li-head">auth_type</span> - Set authentication type for this peer. <span class="li-normal">type: int</span></li>
            <li> <span class="li-head">device_id</span> - Device ID of this peer. <span class="li-normal">type: str</span></li>
            <li> <span class="li-head">encode_type</span> - Set encode type for this peer. <span class="li-normal">type: int</span></li>
            <li> <span class="li-head">ip</span> - Set cluster IP address of this peer. <span class="li-normal">type: str</span></li>
            <li> <span class="li-head">priority</span> - Set priority for this peer. <span class="li-normal">type: int</span></li>
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
      - name: Designate cache-service for wan-optimization and webcache.
        fortios_wanopt_cache_service:
          vdom:  "{{ vdom }}"
          wanopt_cache_service:
            acceptable_connections: "any"
            collaboration: "enable"
            device_id: "<your_own_value>"
            dst_peer:
             -
                auth_type: "7"
                device_id: "<your_own_value>"
                encode_type: "9"
                ip: "<your_own_value>"
                priority: "11"
            prefer_scenario: "balance"
            src_peer:
             -
                auth_type: "14"
                device_id: "<your_own_value>"
                encode_type: "16"
                ip: "<your_own_value>"
                priority: "18"


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
