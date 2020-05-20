:source: fortios_dlp_fp_doc_source.py

:orphan:

.. fortios_dlp_fp_doc_source:

fortios_dlp_fp_doc_source -- Create a DLP fingerprint database by allowing the FortiGate to access a file server containing files from which to create fingerprints in Fortinet's FortiOS and FortiGate.
++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++

.. versionadded:: 2.8

.. contents::
   :local:
   :depth: 1


Synopsis
--------
- This module is able to configure a FortiGate or FortiOS (FOS) device by allowing the user to set and modify dlp feature and fp_doc_source category. Examples include all parameters and values need to be adjusted to datasources before usage. Tested with FOS v6.0.0



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
    <li> <span class="li-head">state</span> - Indicates whether to create or remove the object. This attribute was present already in previous version in a deeper level. It has been moved out to this outer level. <span class="li-normal">type: str</span> <span class="li-required">required: False</span> <span class="li-normal">choices: present, absent</span></li>
    <li> <span class="li-head">dlp_fp_doc_source</span> - Create a DLP fingerprint database by allowing the FortiGate to access a file server containing files from which to create fingerprints. <span class="li-normal">type: dict</span></li>
        <ul class="ul-self">
        <li> <span class="li-head">state</span> - B(Deprecated) <span class="li-normal">type: str</span> <span class="li-required">required: False</span> <span class="li-normal">choices: present, absent</span></li>
        <li> <span class="li-head">date</span> - Day of the month on which to scan the server (1 - 31). <span class="li-normal">type: int</span></li>
        <li> <span class="li-head">file_path</span> - Path on the server to the fingerprint files (max 119 characters). <span class="li-normal">type: str</span></li>
        <li> <span class="li-head">file_pattern</span> - Files matching this pattern on the server are fingerprinted. Optionally use the * and ? wildcards. <span class="li-normal">type: str</span></li>
        <li> <span class="li-head">keep_modified</span> - Enable so that when a file is changed on the server the FortiGate keeps the old fingerprint and adds a new fingerprint to the database. <span class="li-normal">type: str</span> <span class="li-normal">choices: enable, disable</span></li>
        <li> <span class="li-head">name</span> - Name of the DLP fingerprint database. <span class="li-normal">type: str</span> <span class="li-required">required: True</span></li>
        <li> <span class="li-head">password</span> - Password required to log into the file server. <span class="li-normal">type: str</span></li>
        <li> <span class="li-head">period</span> - Frequency for which the FortiGate checks the server for new or changed files. <span class="li-normal">type: str</span> <span class="li-normal">choices: none, daily, weekly, monthly</span></li>
        <li> <span class="li-head">remove_deleted</span> - Enable to keep the fingerprint database up to date when a file is deleted from the server. <span class="li-normal">type: str</span> <span class="li-normal">choices: enable, disable</span></li>
        <li> <span class="li-head">scan_on_creation</span> - Enable to keep the fingerprint database up to date when a file is added or changed on the server. <span class="li-normal">type: str</span> <span class="li-normal">choices: enable, disable</span></li>
        <li> <span class="li-head">scan_subdirectories</span> - Enable/disable scanning subdirectories to find files to create fingerprints from. <span class="li-normal">type: str</span> <span class="li-normal">choices: enable, disable</span></li>
        <li> <span class="li-head">sensitivity</span> - Select a sensitivity or threat level for matches with this fingerprint database. Add sensitivities using fp-sensitivity. Source dlp .fp-sensitivity.name. <span class="li-normal">type: str</span></li>
        <li> <span class="li-head">server</span> - IPv4 or IPv6 address of the server. <span class="li-normal">type: str</span></li>
        <li> <span class="li-head">server_type</span> - Protocol used to communicate with the file server. Currently only Samba (SMB) servers are supported. <span class="li-normal">type: str</span> <span class="li-normal">choices: samba</span></li>
        <li> <span class="li-head">tod_hour</span> - Hour of the day on which to scan the server (0 - 23). <span class="li-normal">type: int</span></li>
        <li> <span class="li-head">tod_min</span> - Minute of the hour on which to scan the server (0 - 59). <span class="li-normal">type: int</span></li>
        <li> <span class="li-head">username</span> - User name required to log into the file server. <span class="li-normal">type: str</span></li>
        <li> <span class="li-head">vdom</span> - Select the VDOM that can communicate with the file server. <span class="li-normal">type: str</span> <span class="li-normal">choices: mgmt, current</span></li>
        <li> <span class="li-head">weekday</span> - Day of the week on which to scan the server. <span class="li-normal">type: str</span> <span class="li-normal">choices: sunday, monday, tuesday, wednesday, thursday, friday, saturday</span></li>
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
      - name: Create a DLP fingerprint database by allowing the FortiGate to access a file server containing files from which to create fingerprints.
        fortios_dlp_fp_doc_source:
          vdom:  "{{ vdom }}"
          state: "present"
          dlp_fp_doc_source:
            date: "3"
            file_path: "<your_own_value>"
            file_pattern: "<your_own_value>"
            keep_modified: "enable"
            name: "default_name_7"
            password: "<your_own_value>"
            period: "none"
            remove_deleted: "enable"
            scan_on_creation: "enable"
            scan_subdirectories: "enable"
            sensitivity: "<your_own_value> (source dlp.fp-sensitivity.name)"
            server: "192.168.100.40"
            server_type: "samba"
            tod_hour: "16"
            tod_min: "17"
            username: "<your_own_value>"
            vdom: "mgmt"
            weekday: "sunday"


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
