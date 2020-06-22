:source: fortios_ftp_proxy_explicit.py

:orphan:

.. fortios_ftp_proxy_explicit:

fortios_ftp_proxy_explicit -- Configure explicit FTP proxy settings in Fortinet's FortiOS and FortiGate.
++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++

.. versionadded:: 2.8

.. contents::
   :local:
   :depth: 1


Synopsis
--------
- This module is able to configure a FortiGate or FortiOS (FOS) device by allowing the user to set and modify ftp_proxy feature and explicit category. Examples include all parameters and values need to be adjusted to datasources before usage. Tested with FOS v6.4.0



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
    <li> <span class="li-head">ftp_proxy_explicit</span> - Configure explicit FTP proxy settings. <span class="li-normal">type: dict</span></li>
        <ul class="ul-self">
        <li> <span class="li-head">incoming_ip</span> - Accept incoming FTP requests from this IP address. An interface must have this IP address. <span class="li-normal">type: str</span></li>
        <li> <span class="li-head">incoming_port</span> - Accept incoming FTP requests on one or more ports. <span class="li-normal">type: str</span></li>
        <li> <span class="li-head">outgoing_ip</span> - Outgoing FTP requests will leave from this IP address. An interface must have this IP address. <span class="li-normal">type: str</span></li>
        <li> <span class="li-head">sec_default_action</span> - Accept or deny explicit FTP proxy sessions when no FTP proxy firewall policy exists. <span class="li-normal">type: str</span> <span class="li-normal">choices: accept, deny</span></li>
        <li> <span class="li-head">ssl</span> - Enable/disable the explicit FTPS proxy. <span class="li-normal">type: str</span> <span class="li-normal">choices: enable, disable</span></li>
        <li> <span class="li-head">ssl_algorithm</span> - Relative strength of encryption algorithms accepted in negotiation. <span class="li-normal">type: str</span> <span class="li-normal">choices: high, medium, low</span></li>
        <li> <span class="li-head">ssl_cert</span> - Name of certificate for SSL connections to this server . Source certificate.local.name. <span class="li-normal">type: str</span></li>
        <li> <span class="li-head">ssl_dh_bits</span> - Bit-size of Diffie-Hellman (DH) prime used in DHE-RSA negotiation . <span class="li-normal">type: str</span> <span class="li-normal">choices: 768, 1024, 1536, 2048</span></li>
        <li> <span class="li-head">status</span> - Enable/disable the explicit FTP proxy. <span class="li-normal">type: str</span> <span class="li-normal">choices: enable, disable</span></li>
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
      - name: Configure explicit FTP proxy settings.
        fortios_ftp_proxy_explicit:
          vdom:  "{{ vdom }}"
          ftp_proxy_explicit:
            incoming_ip: "<your_own_value>"
            incoming_port: "<your_own_value>"
            outgoing_ip: "<your_own_value>"
            sec_default_action: "accept"
            ssl: "enable"
            ssl_algorithm: "high"
            ssl_cert: "<your_own_value> (source certificate.local.name)"
            ssl_dh_bits: "768"
            status: "enable"


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
