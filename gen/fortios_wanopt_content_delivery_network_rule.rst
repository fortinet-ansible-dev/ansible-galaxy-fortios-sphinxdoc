:source: fortios_wanopt_content_delivery_network_rule.py

:orphan:

.. fortios_wanopt_content_delivery_network_rule:

fortios_wanopt_content_delivery_network_rule -- Configure WAN optimization content delivery network rules in Fortinet's FortiOS and FortiGate.
++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++

.. versionadded:: 2.9

.. contents::
   :local:
   :depth: 1


Synopsis
--------
- This module is able to configure a FortiGate or FortiOS (FOS) device by allowing the user to set and modify wanopt feature and content_delivery_network_rule category. Examples include all parameters and values need to be adjusted to datasources before usage. Tested with FOS v6.0.0



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
    <li> <span class="li-head">wanopt_content_delivery_network_rule</span> - Configure WAN optimization content delivery network rules. <span class="li-normal">type: dict</span></li>
        <ul class="ul-self">
        <li> <span class="li-head">category</span> - Content delivery network rule category. <span class="li-normal">type: str</span> <span class="li-normal">choices: vcache, youtube</span></li>
        <li> <span class="li-head">comment</span> - Comment about this CDN-rule. <span class="li-normal">type: str</span></li>
        <li> <span class="li-head">host_domain_name_suffix</span> - Suffix portion of the fully qualified domain name (eg. fortinet.com in "www.fortinet.com"). <span class="li-normal">type: list</span></li>
            <ul class="ul-self">
            <li> <span class="li-head">name</span> - Suffix portion of the fully qualified domain name. <span class="li-normal">type: str</span> <span class="li-required">required: True</span></li>
            </ul>
        <li> <span class="li-head">name</span> - Name of table. <span class="li-normal">type: str</span> <span class="li-required">required: True</span></li>
        <li> <span class="li-head">request_cache_control</span> - Enable/disable HTTP request cache control. <span class="li-normal">type: str</span> <span class="li-normal">choices: enable, disable</span></li>
        <li> <span class="li-head">response_cache_control</span> - Enable/disable HTTP response cache control. <span class="li-normal">type: str</span> <span class="li-normal">choices: enable, disable</span></li>
        <li> <span class="li-head">response_expires</span> - Enable/disable HTTP response cache expires. <span class="li-normal">type: str</span> <span class="li-normal">choices: enable, disable</span></li>
        <li> <span class="li-head">rules</span> - WAN optimization content delivery network rule entries. <span class="li-normal">type: list</span></li>
            <ul class="ul-self">
            <li> <span class="li-head">content_id</span> - Content ID settings. <span class="li-normal">type: dict</span></li>
                <ul class="ul-self">
                <li> <span class="li-head">end_direction</span> - Search direction from end-str match. <span class="li-normal">type: str</span> <span class="li-normal">choices: forward, backward</span></li>
                <li> <span class="li-head">end_skip</span> - Number of characters in URL to skip after end-str has been matched. <span class="li-normal">type: int</span></li>
                <li> <span class="li-head">end_str</span> - String from which to end search. <span class="li-normal">type: str</span></li>
                <li> <span class="li-head">range_str</span> - Name of content ID within the start string and end string. <span class="li-normal">type: str</span></li>
                <li> <span class="li-head">start_direction</span> - Search direction from start-str match. <span class="li-normal">type: str</span> <span class="li-normal">choices: forward, backward</span></li>
                <li> <span class="li-head">start_skip</span> - Number of characters in URL to skip after start-str has been matched. <span class="li-normal">type: int</span></li>
                <li> <span class="li-head">start_str</span> - String from which to start search. <span class="li-normal">type: str</span></li>
                <li> <span class="li-head">target</span> - Option in HTTP header or URL parameter to match. <span class="li-normal">type: str</span> <span class="li-normal">choices: path, parameter, referrer, youtube-map, youtube-id, youku-id, hls-manifest, dash-manifest, hls-fragment, dash-fragment</span></li>
                </ul>
            <li> <span class="li-head">match_entries</span> - List of entries to match. <span class="li-normal">type: list</span></li>
                <ul class="ul-self">
                <li> <span class="li-head">id</span> - Rule ID. <span class="li-normal">type: int</span> <span class="li-required">required: True</span></li>
                <li> <span class="li-head">pattern</span> - Pattern string for matching target (Referrer or URL pattern, eg. "a", "a*c", "*a*", "a*c*e", and "*"). <span class="li-normal">type: list</span></li>
                    <ul class="ul-self">
                    <li> <span class="li-head">string</span> - Pattern strings. <span class="li-normal">type: str</span> <span class="li-required">required: True</span></li>
                    </ul>
                <li> <span class="li-head">target</span> - Option in HTTP header or URL parameter to match. <span class="li-normal">type: str</span> <span class="li-normal">choices: path, parameter, referrer, youtube-map, youtube-id, youku-id</span></li>
                </ul>
            <li> <span class="li-head">match_mode</span> - Match criteria for collecting content ID. <span class="li-normal">type: str</span> <span class="li-normal">choices: all, any</span></li>
            <li> <span class="li-head">name</span> - WAN optimization content delivery network rule name. <span class="li-normal">type: str</span> <span class="li-required">required: True</span></li>
            <li> <span class="li-head">skip_entries</span> - List of entries to skip. <span class="li-normal">type: list</span></li>
                <ul class="ul-self">
                <li> <span class="li-head">id</span> - Rule ID. <span class="li-normal">type: int</span> <span class="li-required">required: True</span></li>
                <li> <span class="li-head">pattern</span> - Pattern string for matching target (Referrer or URL pattern, eg. "a", "a*c", "*a*", "a*c*e", and "*"). <span class="li-normal">type: list</span></li>
                    <ul class="ul-self">
                    <li> <span class="li-head">string</span> - Pattern strings. <span class="li-normal">type: str</span> <span class="li-required">required: True</span></li>
                    </ul>
                <li> <span class="li-head">target</span> - Option in HTTP header or URL parameter to match. <span class="li-normal">type: str</span> <span class="li-normal">choices: path, parameter, referrer, youtube-map, youtube-id, youku-id</span></li>
                </ul>
            <li> <span class="li-head">skip_rule_mode</span> - Skip mode when evaluating skip-rules. <span class="li-normal">type: str</span> <span class="li-normal">choices: all, any</span></li>
            </ul>
        <li> <span class="li-head">status</span> - Enable/disable WAN optimization content delivery network rules. <span class="li-normal">type: str</span> <span class="li-normal">choices: enable, disable</span></li>
        <li> <span class="li-head">text_response_vcache</span> - Enable/disable caching of text responses. <span class="li-normal">type: str</span> <span class="li-normal">choices: enable, disable</span></li>
        <li> <span class="li-head">updateserver</span> - Enable/disable update server. <span class="li-normal">type: str</span> <span class="li-normal">choices: enable, disable</span></li>
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
      - name: Configure WAN optimization content delivery network rules.
        fortios_wanopt_content_delivery_network_rule:
          vdom:  "{{ vdom }}"
          state: "present"
          wanopt_content_delivery_network_rule:
            category: "vcache"
            comment: "Comment about this CDN-rule."
            host_domain_name_suffix:
             -
                name: "default_name_6"
            name: "default_name_7"
            request_cache_control: "enable"
            response_cache_control: "enable"
            response_expires: "enable"
            rules:
             -
                content_id:
                    end_direction: "forward"
                    end_skip: "14"
                    end_str: "<your_own_value>"
                    range_str: "<your_own_value>"
                    start_direction: "forward"
                    start_skip: "18"
                    start_str: "<your_own_value>"
                    target: "path"
                match_entries:
                 -
                    id:  "22"
                    pattern:
                     -
                        string: "<your_own_value>"
                    target: "path"
                match_mode: "all"
                name: "default_name_27"
                skip_entries:
                 -
                    id:  "29"
                    pattern:
                     -
                        string: "<your_own_value>"
                    target: "path"
                skip_rule_mode: "all"
            status: "enable"
            text_response_vcache: "enable"
            updateserver: "enable"


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
