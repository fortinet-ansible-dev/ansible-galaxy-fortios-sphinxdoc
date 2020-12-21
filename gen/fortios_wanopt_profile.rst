:source: fortios_wanopt_profile.py

:orphan:

.. fortios_wanopt_profile:

fortios_wanopt_profile -- Configure WAN optimization profiles in Fortinet's FortiOS and FortiGate.
++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++

.. versionadded:: 2.8

.. contents::
   :local:
   :depth: 1


Synopsis
--------
- This module is able to configure a FortiGate or FortiOS (FOS) device by allowing the user to set and modify wanopt feature and profile category. Examples include all parameters and values need to be adjusted to datasources before usage. Tested with FOS v6.0.0



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
    <li> <span class="li-head">state</span> - Indicates whether to create or remove the object. This attribute was present already in previous version in a deeper level. It has been moved out to this outer level. <span class="li-normal">type: str</span> <span class="li-required">required: False</span> <span class="li-normal">choices: present, absent</span></li>
    <li> <span class="li-head">wanopt_profile</span> - Configure WAN optimization profiles. <span class="li-normal">type: dict</span></li>
        <ul class="ul-self">
        <li> <span class="li-head">state</span> - B(Deprecated) <span class="li-normal">type: str</span> <span class="li-required">required: False</span> <span class="li-normal">choices: present, absent</span></li>
        <li> <span class="li-head">auth_group</span> - Optionally add an authentication group to restrict access to the WAN Optimization tunnel to peers in the authentication group. Source wanopt.auth-group.name. <span class="li-normal">type: str</span></li>
        <li> <span class="li-head">cifs</span> - Enable/disable CIFS (Windows sharing) WAN Optimization and configure CIFS WAN Optimization features. <span class="li-normal">type: dict</span></li>
            <ul class="ul-self">
            <li> <span class="li-head">byte_caching</span> - Enable/disable byte-caching for HTTP. Byte caching reduces the amount of traffic by caching file data sent across the WAN and in future serving if from the cache. <span class="li-normal">type: str</span> <span class="li-normal">choices: enable, disable</span></li>
            <li> <span class="li-head">log_traffic</span> - Enable/disable logging. <span class="li-normal">type: str</span> <span class="li-normal">choices: enable, disable</span></li>
            <li> <span class="li-head">port</span> - Single port number or port number range for CIFS. Only packets with a destination port number that matches this port number or range are accepted by this profile. <span class="li-normal">type: int</span></li>
            <li> <span class="li-head">prefer_chunking</span> - Select dynamic or fixed-size data chunking for HTTP WAN Optimization. <span class="li-normal">type: str</span> <span class="li-normal">choices: dynamic, fix</span></li>
            <li> <span class="li-head">secure_tunnel</span> - Enable/disable securing the WAN Opt tunnel using SSL. Secure and non-secure tunnels use the same TCP port (7810). <span class="li-normal">type: str</span> <span class="li-normal">choices: enable, disable</span></li>
            <li> <span class="li-head">status</span> - Enable/disable HTTP WAN Optimization. <span class="li-normal">type: str</span> <span class="li-normal">choices: enable, disable</span></li>
            <li> <span class="li-head">tunnel_sharing</span> - Tunnel sharing mode for aggressive/non-aggressive and/or interactive/non-interactive protocols. <span class="li-normal">type: str</span> <span class="li-normal">choices: private, shared, express-shared</span></li>
            </ul>
        <li> <span class="li-head">comments</span> - Comment. <span class="li-normal">type: str</span></li>
        <li> <span class="li-head">ftp</span> - Enable/disable FTP WAN Optimization and configure FTP WAN Optimization features. <span class="li-normal">type: dict</span></li>
            <ul class="ul-self">
            <li> <span class="li-head">byte_caching</span> - Enable/disable byte-caching for HTTP. Byte caching reduces the amount of traffic by caching file data sent across the WAN and in future serving if from the cache. <span class="li-normal">type: str</span> <span class="li-normal">choices: enable, disable</span></li>
            <li> <span class="li-head">log_traffic</span> - Enable/disable logging. <span class="li-normal">type: str</span> <span class="li-normal">choices: enable, disable</span></li>
            <li> <span class="li-head">port</span> - Single port number or port number range for FTP. Only packets with a destination port number that matches this port number or range are accepted by this profile. <span class="li-normal">type: int</span></li>
            <li> <span class="li-head">prefer_chunking</span> - Select dynamic or fixed-size data chunking for HTTP WAN Optimization. <span class="li-normal">type: str</span> <span class="li-normal">choices: dynamic, fix</span></li>
            <li> <span class="li-head">secure_tunnel</span> - Enable/disable securing the WAN Opt tunnel using SSL. Secure and non-secure tunnels use the same TCP port (7810). <span class="li-normal">type: str</span> <span class="li-normal">choices: enable, disable</span></li>
            <li> <span class="li-head">status</span> - Enable/disable HTTP WAN Optimization. <span class="li-normal">type: str</span> <span class="li-normal">choices: enable, disable</span></li>
            <li> <span class="li-head">tunnel_sharing</span> - Tunnel sharing mode for aggressive/non-aggressive and/or interactive/non-interactive protocols. <span class="li-normal">type: str</span> <span class="li-normal">choices: private, shared, express-shared</span></li>
            </ul>
        <li> <span class="li-head">http</span> - Enable/disable HTTP WAN Optimization and configure HTTP WAN Optimization features. <span class="li-normal">type: dict</span></li>
            <ul class="ul-self">
            <li> <span class="li-head">byte_caching</span> - Enable/disable byte-caching for HTTP. Byte caching reduces the amount of traffic by caching file data sent across the WAN and in future serving if from the cache. <span class="li-normal">type: str</span> <span class="li-normal">choices: enable, disable</span></li>
            <li> <span class="li-head">log_traffic</span> - Enable/disable logging. <span class="li-normal">type: str</span> <span class="li-normal">choices: enable, disable</span></li>
            <li> <span class="li-head">port</span> - Single port number or port number range for HTTP. Only packets with a destination port number that matches this port number or range are accepted by this profile. <span class="li-normal">type: int</span></li>
            <li> <span class="li-head">prefer_chunking</span> - Select dynamic or fixed-size data chunking for HTTP WAN Optimization. <span class="li-normal">type: str</span> <span class="li-normal">choices: dynamic, fix</span></li>
            <li> <span class="li-head">secure_tunnel</span> - Enable/disable securing the WAN Opt tunnel using SSL. Secure and non-secure tunnels use the same TCP port (7810). <span class="li-normal">type: str</span> <span class="li-normal">choices: enable, disable</span></li>
            <li> <span class="li-head">ssl</span> - Enable/disable SSL/TLS offloading (hardware acceleration) for HTTPS traffic in this tunnel. <span class="li-normal">type: str</span> <span class="li-normal">choices: enable, disable</span></li>
            <li> <span class="li-head">ssl_port</span> - Port on which to expect HTTPS traffic for SSL/TLS offloading. <span class="li-normal">type: int</span></li>
            <li> <span class="li-head">status</span> - Enable/disable HTTP WAN Optimization. <span class="li-normal">type: str</span> <span class="li-normal">choices: enable, disable</span></li>
            <li> <span class="li-head">tunnel_non_http</span> - Configure how to process non-HTTP traffic when a profile configured for HTTP traffic accepts a non-HTTP session. Can occur if an application sends non-HTTP traffic using an HTTP destination port. <span class="li-normal">type: str</span> <span class="li-normal">choices: enable, disable</span></li>
            <li> <span class="li-head">tunnel_sharing</span> - Tunnel sharing mode for aggressive/non-aggressive and/or interactive/non-interactive protocols. <span class="li-normal">type: str</span> <span class="li-normal">choices: private, shared, express-shared</span></li>
            <li> <span class="li-head">unknown_http_version</span> - How to handle HTTP sessions that do not comply with HTTP 0.9, 1.0, or 1.1. <span class="li-normal">type: str</span> <span class="li-normal">choices: reject, tunnel, best-effort</span></li>
            </ul>
        <li> <span class="li-head">mapi</span> - Enable/disable MAPI email WAN Optimization and configure MAPI WAN Optimization features. <span class="li-normal">type: dict</span></li>
            <ul class="ul-self">
            <li> <span class="li-head">byte_caching</span> - Enable/disable byte-caching for HTTP. Byte caching reduces the amount of traffic by caching file data sent across the WAN and in future serving if from the cache. <span class="li-normal">type: str</span> <span class="li-normal">choices: enable, disable</span></li>
            <li> <span class="li-head">log_traffic</span> - Enable/disable logging. <span class="li-normal">type: str</span> <span class="li-normal">choices: enable, disable</span></li>
            <li> <span class="li-head">port</span> - Single port number or port number range for MAPI. Only packets with a destination port number that matches this port number or range are accepted by this profile. <span class="li-normal">type: int</span></li>
            <li> <span class="li-head">secure_tunnel</span> - Enable/disable securing the WAN Opt tunnel using SSL. Secure and non-secure tunnels use the same TCP port (7810). <span class="li-normal">type: str</span> <span class="li-normal">choices: enable, disable</span></li>
            <li> <span class="li-head">status</span> - Enable/disable HTTP WAN Optimization. <span class="li-normal">type: str</span> <span class="li-normal">choices: enable, disable</span></li>
            <li> <span class="li-head">tunnel_sharing</span> - Tunnel sharing mode for aggressive/non-aggressive and/or interactive/non-interactive protocols. <span class="li-normal">type: str</span> <span class="li-normal">choices: private, shared, express-shared</span></li>
            </ul>
        <li> <span class="li-head">name</span> - Profile name. <span class="li-normal">type: str</span> <span class="li-required">required: True</span></li>
        <li> <span class="li-head">tcp</span> - Enable/disable TCP WAN Optimization and configure TCP WAN Optimization features. <span class="li-normal">type: dict</span></li>
            <ul class="ul-self">
            <li> <span class="li-head">byte_caching</span> - Enable/disable byte-caching for HTTP. Byte caching reduces the amount of traffic by caching file data sent across the WAN and in future serving if from the cache. <span class="li-normal">type: str</span> <span class="li-normal">choices: enable, disable</span></li>
            <li> <span class="li-head">byte_caching_opt</span> - Select whether TCP byte-caching uses system memory only or both memory and disk space. <span class="li-normal">type: str</span> <span class="li-normal">choices: mem-only, mem-disk</span></li>
            <li> <span class="li-head">log_traffic</span> - Enable/disable logging. <span class="li-normal">type: str</span> <span class="li-normal">choices: enable, disable</span></li>
            <li> <span class="li-head">port</span> - Single port number or port number range for TCP. Only packets with a destination port number that matches this port number or range are accepted by this profile. <span class="li-normal">type: str</span></li>
            <li> <span class="li-head">secure_tunnel</span> - Enable/disable securing the WAN Opt tunnel using SSL. Secure and non-secure tunnels use the same TCP port (7810). <span class="li-normal">type: str</span> <span class="li-normal">choices: enable, disable</span></li>
            <li> <span class="li-head">ssl</span> - Enable/disable SSL/TLS offloading. <span class="li-normal">type: str</span> <span class="li-normal">choices: enable, disable</span></li>
            <li> <span class="li-head">ssl_port</span> - Port on which to expect HTTPS traffic for SSL/TLS offloading. <span class="li-normal">type: int</span></li>
            <li> <span class="li-head">status</span> - Enable/disable HTTP WAN Optimization. <span class="li-normal">type: str</span> <span class="li-normal">choices: enable, disable</span></li>
            <li> <span class="li-head">tunnel_sharing</span> - Tunnel sharing mode for aggressive/non-aggressive and/or interactive/non-interactive protocols. <span class="li-normal">type: str</span> <span class="li-normal">choices: private, shared, express-shared</span></li>
            </ul>
        <li> <span class="li-head">transparent</span> - Enable/disable transparent mode. <span class="li-normal">type: str</span> <span class="li-normal">choices: enable, disable</span></li>
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
      - name: Configure WAN optimization profiles.
        fortios_wanopt_profile:
          vdom:  "{{ vdom }}"
          state: "present"
          access_token: "<your_own_value>"
          wanopt_profile:
            auth_group: "<your_own_value> (source wanopt.auth-group.name)"
            cifs:
                byte_caching: "enable"
                log_traffic: "enable"
                port: "7"
                prefer_chunking: "dynamic"
                secure_tunnel: "enable"
                status: "enable"
                tunnel_sharing: "private"
            comments: "<your_own_value>"
            ftp:
                byte_caching: "enable"
                log_traffic: "enable"
                port: "16"
                prefer_chunking: "dynamic"
                secure_tunnel: "enable"
                status: "enable"
                tunnel_sharing: "private"
            http:
                byte_caching: "enable"
                log_traffic: "enable"
                port: "24"
                prefer_chunking: "dynamic"
                secure_tunnel: "enable"
                ssl: "enable"
                ssl_port: "28"
                status: "enable"
                tunnel_non_http: "enable"
                tunnel_sharing: "private"
                unknown_http_version: "reject"
            mapi:
                byte_caching: "enable"
                log_traffic: "enable"
                port: "36"
                secure_tunnel: "enable"
                status: "enable"
                tunnel_sharing: "private"
            name: "default_name_40"
            tcp:
                byte_caching: "enable"
                byte_caching_opt: "mem-only"
                log_traffic: "enable"
                port: "<your_own_value>"
                secure_tunnel: "enable"
                ssl: "enable"
                ssl_port: "48"
                status: "enable"
                tunnel_sharing: "private"
            transparent: "enable"
    


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
