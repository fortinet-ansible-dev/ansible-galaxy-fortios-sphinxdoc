:source: fortios_wanopt_webcache.py

:orphan:

.. fortios_wanopt_webcache:

fortios_wanopt_webcache -- Configure global Web cache settings in Fortinet's FortiOS and FortiGate.
+++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++

.. versionadded:: 2.9

.. contents::
   :local:
   :depth: 1


Synopsis
--------
- This module is able to configure a FortiGate or FortiOS (FOS) device by allowing the user to set and modify wanopt feature and webcache category. Examples include all parameters and values need to be adjusted to datasources before usage. Tested with FOS v6.4.0



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
    <li> <span class="li-head">wanopt_webcache</span> - Configure global Web cache settings. <span class="li-normal">type: dict</span></li>
        <ul class="ul-self">
        <li> <span class="li-head">always_revalidate</span> - Enable/disable revalidation of requested cached objects, which have content on the server, before serving it to the client. <span class="li-normal">type: str</span> <span class="li-normal">choices: enable, disable</span></li>
        <li> <span class="li-head">cache_by_default</span> - Enable/disable caching content that lacks explicit caching policies from the server. <span class="li-normal">type: str</span> <span class="li-normal">choices: enable, disable</span></li>
        <li> <span class="li-head">cache_cookie</span> - Enable/disable caching cookies. Since cookies contain information for or about individual users, they not usually cached. <span class="li-normal">type: str</span> <span class="li-normal">choices: enable, disable</span></li>
        <li> <span class="li-head">cache_expired</span> - Enable/disable caching type-1 objects that are already expired on arrival. <span class="li-normal">type: str</span> <span class="li-normal">choices: enable, disable</span></li>
        <li> <span class="li-head">default_ttl</span> - Default object expiry time . This only applies to those objects that do not have an expiry time set by the web server. <span class="li-normal">type: int</span></li>
        <li> <span class="li-head">external</span> - Enable/disable external Web caching. <span class="li-normal">type: str</span> <span class="li-normal">choices: enable, disable</span></li>
        <li> <span class="li-head">fresh_factor</span> - Frequency that the server is checked to see if any objects have expired (1 - 100). The higher the fresh factor, the less often the checks occur. <span class="li-normal">type: int</span></li>
        <li> <span class="li-head">host_validate</span> - Enable/disable validating "Host:" with original server IP. <span class="li-normal">type: str</span> <span class="li-normal">choices: enable, disable</span></li>
        <li> <span class="li-head">ignore_conditional</span> - Enable/disable controlling the behavior of cache-control HTTP 1.1 header values. <span class="li-normal">type: str</span> <span class="li-normal">choices: enable, disable</span></li>
        <li> <span class="li-head">ignore_ie_reload</span> - Enable/disable ignoring the PNC-interpretation of Internet Explorer"s Accept: / header. <span class="li-normal">type: str</span> <span class="li-normal">choices: enable, disable</span></li>
        <li> <span class="li-head">ignore_ims</span> - Enable/disable ignoring the if-modified-since (IMS) header. <span class="li-normal">type: str</span> <span class="li-normal">choices: enable, disable</span></li>
        <li> <span class="li-head">ignore_pnc</span> - Enable/disable ignoring the pragma no-cache (PNC) header. <span class="li-normal">type: str</span> <span class="li-normal">choices: enable, disable</span></li>
        <li> <span class="li-head">max_object_size</span> - Maximum cacheable object size in kB (1 - 2147483 kb (2GB). All objects that exceed this are delivered to the client but not stored in the web cache. <span class="li-normal">type: int</span></li>
        <li> <span class="li-head">max_ttl</span> - Maximum time an object can stay in the web cache without checking to see if it has expired on the server . <span class="li-normal">type: int</span></li>
        <li> <span class="li-head">min_ttl</span> - Minimum time an object can stay in the web cache without checking to see if it has expired on the server . <span class="li-normal">type: int</span></li>
        <li> <span class="li-head">neg_resp_time</span> - Time in minutes to cache negative responses or errors (0 - 4294967295). <span class="li-normal">type: int</span></li>
        <li> <span class="li-head">reval_pnc</span> - Enable/disable revalidation of pragma-no-cache (PNC) to address bandwidth concerns. <span class="li-normal">type: str</span> <span class="li-normal">choices: enable, disable</span></li>
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
      - name: Configure global Web cache settings.
        fortios_wanopt_webcache:
          vdom:  "{{ vdom }}"
          wanopt_webcache:
            always_revalidate: "enable"
            cache_by_default: "enable"
            cache_cookie: "enable"
            cache_expired: "enable"
            default_ttl: "7"
            external: "enable"
            fresh_factor: "9"
            host_validate: "enable"
            ignore_conditional: "enable"
            ignore_ie_reload: "enable"
            ignore_ims: "enable"
            ignore_pnc: "enable"
            max_object_size: "15"
            max_ttl: "16"
            min_ttl: "17"
            neg_resp_time: "18"
            reval_pnc: "enable"
    


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
