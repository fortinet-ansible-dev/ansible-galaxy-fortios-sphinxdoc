:source: fortios_system_lldp_network_policy.py

:orphan:

.. fortios_system_lldp_network_policy:

fortios_system_lldp_network_policy -- Configure LLDP network policy in Fortinet's FortiOS and FortiGate.
++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++

.. versionadded:: 2.10

.. contents::
   :local:
   :depth: 1


Synopsis
--------
- This module is able to configure a FortiGate or FortiOS (FOS) device by allowing the user to set and modify system_lldp feature and network_policy category. Examples include all parameters and values need to be adjusted to datasources before usage. Tested with FOS v6.4.0



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
    <li> <span class="li-head">system_lldp_network_policy</span> - Configure LLDP network policy. <span class="li-normal">type: dict</span></li>
        <ul class="ul-self">
        <li> <span class="li-head">comment</span> - Comment. <span class="li-normal">type: str</span></li>
        <li> <span class="li-head">guest</span> - Guest. <span class="li-normal">type: dict</span></li>
            <ul class="ul-self">
            <li> <span class="li-head">dscp</span> - Differentiated Services Code Point (DSCP) value to advertise. <span class="li-normal">type: int</span></li>
            <li> <span class="li-head">priority</span> - 802.1P CoS/PCP to advertise (0 - 7; from lowest to highest priority). <span class="li-normal">type: int</span></li>
            <li> <span class="li-head">status</span> - Enable/disable advertising this policy. <span class="li-normal">type: str</span> <span class="li-normal">choices: disable, enable</span></li>
            <li> <span class="li-head">tag</span> - Advertise tagged or untagged traffic. <span class="li-normal">type: str</span> <span class="li-normal">choices: none, dot1q, dot1p</span></li>
            <li> <span class="li-head">vlan</span> - 802.1Q VLAN ID to advertise (1 - 4094). <span class="li-normal">type: int</span></li>
            </ul>
        <li> <span class="li-head">guest_voice_signaling</span> - Guest Voice Signaling. <span class="li-normal">type: dict</span></li>
            <ul class="ul-self">
            <li> <span class="li-head">dscp</span> - Differentiated Services Code Point (DSCP) value to advertise. <span class="li-normal">type: int</span></li>
            <li> <span class="li-head">priority</span> - 802.1P CoS/PCP to advertise (0 - 7; from lowest to highest priority). <span class="li-normal">type: int</span></li>
            <li> <span class="li-head">status</span> - Enable/disable advertising this policy. <span class="li-normal">type: str</span> <span class="li-normal">choices: disable, enable</span></li>
            <li> <span class="li-head">tag</span> - Advertise tagged or untagged traffic. <span class="li-normal">type: str</span> <span class="li-normal">choices: none, dot1q, dot1p</span></li>
            <li> <span class="li-head">vlan</span> - 802.1Q VLAN ID to advertise (1 - 4094). <span class="li-normal">type: int</span></li>
            </ul>
        <li> <span class="li-head">name</span> - LLDP network policy name. <span class="li-normal">type: str</span> <span class="li-required">required: True</span></li>
        <li> <span class="li-head">softphone</span> - Softphone. <span class="li-normal">type: dict</span></li>
            <ul class="ul-self">
            <li> <span class="li-head">dscp</span> - Differentiated Services Code Point (DSCP) value to advertise. <span class="li-normal">type: int</span></li>
            <li> <span class="li-head">priority</span> - 802.1P CoS/PCP to advertise (0 - 7; from lowest to highest priority). <span class="li-normal">type: int</span></li>
            <li> <span class="li-head">status</span> - Enable/disable advertising this policy. <span class="li-normal">type: str</span> <span class="li-normal">choices: disable, enable</span></li>
            <li> <span class="li-head">tag</span> - Advertise tagged or untagged traffic. <span class="li-normal">type: str</span> <span class="li-normal">choices: none, dot1q, dot1p</span></li>
            <li> <span class="li-head">vlan</span> - 802.1Q VLAN ID to advertise (1 - 4094). <span class="li-normal">type: int</span></li>
            </ul>
        <li> <span class="li-head">streaming_video</span> - Streaming Video. <span class="li-normal">type: dict</span></li>
            <ul class="ul-self">
            <li> <span class="li-head">dscp</span> - Differentiated Services Code Point (DSCP) value to advertise. <span class="li-normal">type: int</span></li>
            <li> <span class="li-head">priority</span> - 802.1P CoS/PCP to advertise (0 - 7; from lowest to highest priority). <span class="li-normal">type: int</span></li>
            <li> <span class="li-head">status</span> - Enable/disable advertising this policy. <span class="li-normal">type: str</span> <span class="li-normal">choices: disable, enable</span></li>
            <li> <span class="li-head">tag</span> - Advertise tagged or untagged traffic. <span class="li-normal">type: str</span> <span class="li-normal">choices: none, dot1q, dot1p</span></li>
            <li> <span class="li-head">vlan</span> - 802.1Q VLAN ID to advertise (1 - 4094). <span class="li-normal">type: int</span></li>
            </ul>
        <li> <span class="li-head">video_conferencing</span> - Video Conferencing. <span class="li-normal">type: dict</span></li>
            <ul class="ul-self">
            <li> <span class="li-head">dscp</span> - Differentiated Services Code Point (DSCP) value to advertise. <span class="li-normal">type: int</span></li>
            <li> <span class="li-head">priority</span> - 802.1P CoS/PCP to advertise (0 - 7; from lowest to highest priority). <span class="li-normal">type: int</span></li>
            <li> <span class="li-head">status</span> - Enable/disable advertising this policy. <span class="li-normal">type: str</span> <span class="li-normal">choices: disable, enable</span></li>
            <li> <span class="li-head">tag</span> - Advertise tagged or untagged traffic. <span class="li-normal">type: str</span> <span class="li-normal">choices: none, dot1q, dot1p</span></li>
            <li> <span class="li-head">vlan</span> - 802.1Q VLAN ID to advertise (1 - 4094). <span class="li-normal">type: int</span></li>
            </ul>
        <li> <span class="li-head">video_signaling</span> - Video Signaling. <span class="li-normal">type: dict</span></li>
            <ul class="ul-self">
            <li> <span class="li-head">dscp</span> - Differentiated Services Code Point (DSCP) value to advertise. <span class="li-normal">type: int</span></li>
            <li> <span class="li-head">priority</span> - 802.1P CoS/PCP to advertise (0 - 7; from lowest to highest priority). <span class="li-normal">type: int</span></li>
            <li> <span class="li-head">status</span> - Enable/disable advertising this policy. <span class="li-normal">type: str</span> <span class="li-normal">choices: disable, enable</span></li>
            <li> <span class="li-head">tag</span> - Advertise tagged or untagged traffic. <span class="li-normal">type: str</span> <span class="li-normal">choices: none, dot1q, dot1p</span></li>
            <li> <span class="li-head">vlan</span> - 802.1Q VLAN ID to advertise (1 - 4094). <span class="li-normal">type: int</span></li>
            </ul>
        <li> <span class="li-head">voice</span> - Voice. <span class="li-normal">type: dict</span></li>
            <ul class="ul-self">
            <li> <span class="li-head">dscp</span> - Differentiated Services Code Point (DSCP) value to advertise. <span class="li-normal">type: int</span></li>
            <li> <span class="li-head">priority</span> - 802.1P CoS/PCP to advertise (0 - 7; from lowest to highest priority). <span class="li-normal">type: int</span></li>
            <li> <span class="li-head">status</span> - Enable/disable advertising this policy. <span class="li-normal">type: str</span> <span class="li-normal">choices: disable, enable</span></li>
            <li> <span class="li-head">tag</span> - Advertise tagged or untagged traffic. <span class="li-normal">type: str</span> <span class="li-normal">choices: none, dot1q, dot1p</span></li>
            <li> <span class="li-head">vlan</span> - 802.1Q VLAN ID to advertise (1 - 4094). <span class="li-normal">type: int</span></li>
            </ul>
        <li> <span class="li-head">voice_signaling</span> - Voice signaling. <span class="li-normal">type: dict</span></li>
            <ul class="ul-self">
            <li> <span class="li-head">dscp</span> - Differentiated Services Code Point (DSCP) value to advertise. <span class="li-normal">type: int</span></li>
            <li> <span class="li-head">priority</span> - 802.1P CoS/PCP to advertise (0 - 7; from lowest to highest priority). <span class="li-normal">type: int</span></li>
            <li> <span class="li-head">status</span> - Enable/disable advertising this policy. <span class="li-normal">type: str</span> <span class="li-normal">choices: disable, enable</span></li>
            <li> <span class="li-head">tag</span> - Advertise tagged or untagged traffic. <span class="li-normal">type: str</span> <span class="li-normal">choices: none, dot1q, dot1p</span></li>
            <li> <span class="li-head">vlan</span> - 802.1Q VLAN ID to advertise (1 - 4094). <span class="li-normal">type: int</span></li>
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
      - name: Configure LLDP network policy.
        fortios_system_lldp_network_policy:
          vdom:  "{{ vdom }}"
          state: "present"
          system_lldp_network_policy:
            comment: "Comment."
            guest:
                dscp: "5"
                priority: "6"
                status: "disable"
                tag: "none"
                vlan: "9"
            guest_voice_signaling:
                dscp: "11"
                priority: "12"
                status: "disable"
                tag: "none"
                vlan: "15"
            name: "default_name_16"
            softphone:
                dscp: "18"
                priority: "19"
                status: "disable"
                tag: "none"
                vlan: "22"
            streaming_video:
                dscp: "24"
                priority: "25"
                status: "disable"
                tag: "none"
                vlan: "28"
            video_conferencing:
                dscp: "30"
                priority: "31"
                status: "disable"
                tag: "none"
                vlan: "34"
            video_signaling:
                dscp: "36"
                priority: "37"
                status: "disable"
                tag: "none"
                vlan: "40"
            voice:
                dscp: "42"
                priority: "43"
                status: "disable"
                tag: "none"
                vlan: "46"
            voice_signaling:
                dscp: "48"
                priority: "49"
                status: "disable"
                tag: "none"
                vlan: "52"


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
