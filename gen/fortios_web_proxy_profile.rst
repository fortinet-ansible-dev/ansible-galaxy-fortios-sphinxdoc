:source: fortios_web_proxy_profile.py

:orphan:

.. _fortios_web_proxy_profile:

fortios_web_proxy_profile -- Configure web proxy profiles in Fortinet's FortiOS and FortiGate.
++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++

.. versionadded:: 2.8

.. contents::
   :local:
   :depth: 1


Synopsis
--------
- This module is able to configure a FortiGate or FortiOS (FOS) device by allowing the user to set and modify web_proxy feature and profile category. Examples include all parameters and values need to be adjusted to datasources before usage. Tested with FOS v6.0.5


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
    <li><span class="li-head">state</span> - Indicates whether to create or remove the object. This attribute was present already in previous version in a deeper level. It has been moved out to this outer level. <span class="li-normal">type: str</span> <span class="li-required">required: false</span> <span class="li-normal">choices: present,  absent</span></li>
    <li><span class="li-head">web_proxy_profile</span> - Configure web proxy profiles. <span class="li-normal">default: null</span> <span class="li-normal">type: dict</span></li>
            <ul class="ul-self">

            <li><span class="li-head">state</span> - B(Deprecated) Starting with Ansible 2.9 we recommend using the top-level 'state' parameter. HORIZONTALLINE Indicates whether to create or remove the object. <span class="li-normal">type: str</span> <span class="li-required">required: false</span> <span class="li-normal">choices: present,  absent</span></li>
            <li><span class="li-head">header_client_ip</span> - "Action to take on the HTTP client-IP header in forwarded requests: forwards (pass), adds, or removes the HTTP header." <span class="li-normal">type: str</span> <span class="li-normal">choices: pass,  add,  remove</span></li>
            <li><span class="li-head">header_front_end_https</span> - "Action to take on the HTTP front-end-HTTPS header in forwarded requests: forwards (pass), adds, or removes the HTTP header." <span class="li-normal">type: str</span> <span class="li-normal">choices: pass,  add,  remove</span></li>
            <li><span class="li-head">header_via_request</span> - "Action to take on the HTTP via header in forwarded requests: forwards (pass), adds, or removes the HTTP header." <span class="li-normal">type: str</span> <span class="li-normal">choices: pass,  add,  remove</span></li>
            <li><span class="li-head">header_via_response</span> - "Action to take on the HTTP via header in forwarded responses: forwards (pass), adds, or removes the HTTP header." <span class="li-normal">type: str</span> <span class="li-normal">choices: pass,  add,  remove</span></li>
            <li><span class="li-head">header_x_authenticated_groups</span> - "Action to take on the HTTP x-authenticated-groups header in forwarded requests: forwards (pass), adds, or removes the HTTP header." <span class="li-normal">type: str</span> <span class="li-normal">choices: pass,  add,  remove</span></li>
            <li><span class="li-head">header_x_authenticated_user</span> - "Action to take on the HTTP x-authenticated-user header in forwarded requests: forwards (pass), adds, or removes the HTTP header." <span class="li-normal">type: str</span> <span class="li-normal">choices: pass,  add,  remove</span></li>
            <li><span class="li-head">header_x_forwarded_for</span> - "Action to take on the HTTP x-forwarded-for header in forwarded requests: forwards (pass), adds, or removes the HTTP header." <span class="li-normal">type: str</span> <span class="li-normal">choices: pass,  add,  remove</span></li>
            <li><span class="li-head">headers</span> - Configure HTTP forwarded requests headers. <span class="li-normal">type: list</span></li>
                    <ul class="ul-self">

                    <li><span class="li-head">action</span> - Action when HTTP the header forwarded. <span class="li-normal">type: str</span> <span class="li-normal">choices: add-to-request,  add-to-response,  remove-from-request,  remove-from-response</span></li>
                    <li><span class="li-head">content</span> - HTTP header's content. <span class="li-normal">type: str</span></li>
                    <li><span class="li-head">id</span> - HTTP forwarded header id. <span class="li-required">required</span> <span class="li-normal">type: int</span></li>
                    <li><span class="li-head">name</span> - HTTP forwarded header name. <span class="li-normal">type: str</span>
                    </ul>

            <li><span class="li-head">log_header_change</span> - Enable/disable logging HTTP header changes. <span class="li-normal">type: str</span> <span class="li-normal">choices: enable,  disable</span></li>
            <li><span class="li-head">name</span> - Profile name. <span class="li-required">required</span> <span class="li-normal">type: str</span></li>
            <li><span class="li-head">strip_encoding</span> - Enable/disable stripping unsupported encoding from the request header. <span class="li-normal">type: str</span> <span class="li-normal">choices: enable,  disable</span>
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
      - name: Configure web proxy profiles.
        fortios_web_proxy_profile:
          host:  "{{ host }}"
          username: "{{ username }}"
          password: "{{ password }}"
          vdom:  "{{ vdom }}"
          https: "False"
          state: "present"
          web_proxy_profile:
            header_client_ip: "pass"
            header_front_end_https: "pass"
            header_via_request: "pass"
            header_via_response: "pass"
            header_x_authenticated_groups: "pass"
            header_x_authenticated_user: "pass"
            header_x_forwarded_for: "pass"
            headers:
             -
                action: "add-to-request"
                content: "<your_own_value>"
                id:  "13"
                name: "default_name_14"
            log_header_change: "enable"
            name: "default_name_16"
            strip_encoding: "enable"



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