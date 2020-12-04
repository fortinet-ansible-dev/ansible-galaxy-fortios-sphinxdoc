:source: fortios_dlp_sensor.py

:orphan:

.. fortios_dlp_sensor:

fortios_dlp_sensor -- Configure DLP sensors in Fortinet's FortiOS and FortiGate.
++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++

.. versionadded:: 2.8

.. contents::
   :local:
   :depth: 1


Synopsis
--------
- This module is able to configure a FortiGate or FortiOS (FOS) device by allowing the user to set and modify dlp feature and sensor category. Examples include all parameters and values need to be adjusted to datasources before usage. Tested with FOS v6.0.0



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
    <li> <span class="li-head">dlp_sensor</span> - Configure DLP sensors. <span class="li-normal">type: dict</span></li>
        <ul class="ul-self">
        <li> <span class="li-head">state</span> - B(Deprecated) <span class="li-normal">type: str</span> <span class="li-required">required: False</span> <span class="li-normal">choices: present, absent</span></li>
        <li> <span class="li-head">comment</span> - Comment. <span class="li-normal">type: str</span></li>
        <li> <span class="li-head">dlp_log</span> - Enable/disable DLP logging. <span class="li-normal">type: str</span> <span class="li-normal">choices: enable, disable</span></li>
        <li> <span class="li-head">extended_log</span> - Enable/disable extended logging for data leak prevention. <span class="li-normal">type: str</span> <span class="li-normal">choices: enable, disable</span></li>
        <li> <span class="li-head">filter</span> - Set up DLP filters for this sensor. <span class="li-normal">type: list</span></li>
            <ul class="ul-self">
            <li> <span class="li-head">action</span> - Action to take with content that this DLP sensor matches. <span class="li-normal">type: str</span> <span class="li-normal">choices: allow, log-only, block, quarantine-ip</span></li>
            <li> <span class="li-head">archive</span> - Enable/disable DLP archiving. <span class="li-normal">type: str</span> <span class="li-normal">choices: disable, enable</span></li>
            <li> <span class="li-head">company_identifier</span> - Enter a company identifier watermark to match. Only watermarks that your company has placed on the files are matched. <span class="li-normal">type: str</span></li>
            <li> <span class="li-head">expiry</span> - Quarantine duration in days, hours, minutes format (dddhhmm). <span class="li-normal">type: str</span></li>
            <li> <span class="li-head">file_size</span> - Match files this size or larger (0 - 4294967295 kbytes). <span class="li-normal">type: int</span></li>
            <li> <span class="li-head">file_type</span> - Select the number of a DLP file pattern table to match. Source dlp.filepattern.id. <span class="li-normal">type: int</span></li>
            <li> <span class="li-head">filter_by</span> - Select the type of content to match. <span class="li-normal">type: str</span> <span class="li-normal">choices: credit-card, ssn, regexp, file-type, file-size, fingerprint, watermark, encrypted</span></li>
            <li> <span class="li-head">fp_sensitivity</span> - Select a DLP file pattern sensitivity to match. <span class="li-normal">type: list</span></li>
                <ul class="ul-self">
                <li> <span class="li-head">name</span> - Select a DLP sensitivity. Source dlp.fp-sensitivity.name. <span class="li-normal">type: str</span> <span class="li-required">required: True</span></li>
                </ul>
            <li> <span class="li-head">id</span> - ID. <span class="li-normal">type: int</span> <span class="li-required">required: True</span></li>
            <li> <span class="li-head">match_percentage</span> - Percentage of fingerprints in the fingerprint databases designated with the selected fp-sensitivity to match. <span class="li-normal">type: int</span></li>
            <li> <span class="li-head">name</span> - Filter name. <span class="li-normal">type: str</span></li>
            <li> <span class="li-head">proto</span> - Check messages or files over one or more of these protocols. <span class="li-normal">type: str</span> <span class="li-normal">choices: smtp, pop3, imap, http-get, http-post, ftp, nntp, mapi, mm1, mm3, mm4, mm7</span></li>
            <li> <span class="li-head">regexp</span> - Enter a regular expression to match (max. 255 characters). <span class="li-normal">type: str</span></li>
            <li> <span class="li-head">severity</span> - Select the severity or threat level that matches this filter. <span class="li-normal">type: str</span> <span class="li-normal">choices: info, low, medium, high, critical</span></li>
            <li> <span class="li-head">type</span> - Select whether to check the content of messages (an email message) or files (downloaded files or email attachments). <span class="li-normal">type: str</span> <span class="li-normal">choices: file, message</span></li>
            </ul>
        <li> <span class="li-head">flow_based</span> - Enable/disable flow-based DLP. <span class="li-normal">type: str</span> <span class="li-normal">choices: enable, disable</span></li>
        <li> <span class="li-head">full_archive_proto</span> - Protocols to always content archive. <span class="li-normal">type: str</span> <span class="li-normal">choices: smtp, pop3, imap, http-get, http-post, ftp, nntp, mapi, mm1, mm3, mm4, mm7</span></li>
        <li> <span class="li-head">nac_quar_log</span> - Enable/disable NAC quarantine logging. <span class="li-normal">type: str</span> <span class="li-normal">choices: enable, disable</span></li>
        <li> <span class="li-head">name</span> - Name of the DLP sensor. <span class="li-normal">type: str</span> <span class="li-required">required: True</span></li>
        <li> <span class="li-head">options</span> - Configure DLP options. <span class="li-normal">type: str</span></li>
        <li> <span class="li-head">replacemsg_group</span> - Replacement message group used by this DLP sensor. Source system.replacemsg-group.name. <span class="li-normal">type: str</span></li>
        <li> <span class="li-head">summary_proto</span> - Protocols to always log summary. <span class="li-normal">type: str</span> <span class="li-normal">choices: smtp, pop3, imap, http-get, http-post, ftp, nntp, mapi, mm1, mm3, mm4, mm7</span></li>
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
      - name: Configure DLP sensors.
        fortios_dlp_sensor:
          vdom:  "{{ vdom }}"
          state: "present"
          access_token: "<your_own_value>"
          dlp_sensor:
            comment: "Comment."
            dlp_log: "enable"
            extended_log: "enable"
            filter:
             -
                action: "allow"
                archive: "disable"
                company_identifier:  "myId_9"
                expiry: "<your_own_value>"
                file_size: "11"
                file_type: "12 (source dlp.filepattern.id)"
                filter_by: "credit-card"
                fp_sensitivity:
                 -
                    name: "default_name_15 (source dlp.fp-sensitivity.name)"
                id:  "16"
                match_percentage: "17"
                name: "default_name_18"
                proto: "smtp"
                regexp: "<your_own_value>"
                severity: "info"
                type: "file"
            flow_based: "enable"
            full_archive_proto: "smtp"
            nac_quar_log: "enable"
            name: "default_name_26"
            options: "<your_own_value>"
            replacemsg_group: "<your_own_value> (source system.replacemsg-group.name)"
            summary_proto: "smtp"
    


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
