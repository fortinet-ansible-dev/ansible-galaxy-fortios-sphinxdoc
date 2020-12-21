:source: fortios_emailfilter_profile.py

:orphan:

.. fortios_emailfilter_profile:

fortios_emailfilter_profile -- Configure Email Filter profiles in Fortinet's FortiOS and FortiGate.
+++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++

.. versionadded:: 2.9

.. contents::
   :local:
   :depth: 1


Synopsis
--------
- This module is able to configure a FortiGate or FortiOS (FOS) device by allowing the user to set and modify emailfilter feature and profile category. Examples include all parameters and values need to be adjusted to datasources before usage. Tested with FOS v6.4.0



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
    <li> <span class="li-head">state</span> - Indicates whether to create or remove the object. <span class="li-normal">type: str</span> <span class="li-required">required: True</span> <span class="li-normal">choices: present, absent</span></li>
    <li> <span class="li-head">emailfilter_profile</span> - Configure Email Filter profiles. <span class="li-normal">type: dict</span></li>
        <ul class="ul-self">
        <li> <span class="li-head">comment</span> - Comment. <span class="li-normal">type: str</span></li>
        <li> <span class="li-head">external</span> - Enable/disable external Email inspection. <span class="li-normal">type: str</span> <span class="li-normal">choices: enable, disable</span></li>
        <li> <span class="li-head">feature_set</span> - Flow/proxy feature set. <span class="li-normal">type: str</span> <span class="li-normal">choices: flow, proxy</span></li>
        <li> <span class="li-head">file_filter</span> - File filter. <span class="li-normal">type: dict</span></li>
            <ul class="ul-self">
            <li> <span class="li-head">entries</span> - File filter entries. <span class="li-normal">type: list</span></li>
                <ul class="ul-self">
                <li> <span class="li-head">action</span> - Action taken for matched file. <span class="li-normal">type: str</span> <span class="li-normal">choices: log, block</span></li>
                <li> <span class="li-head">comment</span> - Comment. <span class="li-normal">type: str</span></li>
                <li> <span class="li-head">file_type</span> - Select file type. <span class="li-normal">type: list</span></li>
                    <ul class="ul-self">
                    <li> <span class="li-head">name</span> - File type name. Source antivirus.filetype.name. <span class="li-normal">type: str</span> <span class="li-required">required: True</span></li>
                    </ul>
                <li> <span class="li-head">filter</span> - Add a file filter. <span class="li-normal">type: str</span> <span class="li-required">required: True</span></li>
                <li> <span class="li-head">password_protected</span> - Match password-protected files. <span class="li-normal">type: str</span> <span class="li-normal">choices: True, any</span></li>
                <li> <span class="li-head">protocol</span> - Protocols to apply with. <span class="li-normal">type: str</span> <span class="li-normal">choices: smtp, imap, pop3</span></li>
                </ul>
            <li> <span class="li-head">log</span> - Enable/disable file filter logging. <span class="li-normal">type: str</span> <span class="li-normal">choices: enable, disable</span></li>
            <li> <span class="li-head">scan_archive_contents</span> - Enable/disable file filter archive contents scan. <span class="li-normal">type: str</span> <span class="li-normal">choices: enable, disable</span></li>
            <li> <span class="li-head">status</span> - Enable/disable file filter. <span class="li-normal">type: str</span> <span class="li-normal">choices: enable, disable</span></li>
            </ul>
        <li> <span class="li-head">gmail</span> - Gmail. <span class="li-normal">type: dict</span></li>
            <ul class="ul-self">
            <li> <span class="li-head">log</span> - Enable/disable logging. <span class="li-normal">type: str</span> <span class="li-normal">choices: enable, disable</span></li>
            </ul>
        <li> <span class="li-head">imap</span> - IMAP. <span class="li-normal">type: dict</span></li>
            <ul class="ul-self">
            <li> <span class="li-head">action</span> - Action for spam email. <span class="li-normal">type: str</span> <span class="li-normal">choices: pass, tag</span></li>
            <li> <span class="li-head">log</span> - Enable/disable logging. <span class="li-normal">type: str</span> <span class="li-normal">choices: enable, disable</span></li>
            <li> <span class="li-head">tag_msg</span> - Subject text or header added to spam email. <span class="li-normal">type: str</span></li>
            <li> <span class="li-head">tag_type</span> - Tag subject or header for spam email. <span class="li-normal">type: str</span> <span class="li-normal">choices: subject, header, spaminfo</span></li>
            </ul>
        <li> <span class="li-head">mapi</span> - MAPI. <span class="li-normal">type: dict</span></li>
            <ul class="ul-self">
            <li> <span class="li-head">action</span> - Action for spam email. <span class="li-normal">type: str</span> <span class="li-normal">choices: pass, discard</span></li>
            <li> <span class="li-head">log</span> - Enable/disable logging. <span class="li-normal">type: str</span> <span class="li-normal">choices: enable, disable</span></li>
            </ul>
        <li> <span class="li-head">msn_hotmail</span> - MSN Hotmail. <span class="li-normal">type: dict</span></li>
            <ul class="ul-self">
            <li> <span class="li-head">log</span> - Enable/disable logging. <span class="li-normal">type: str</span> <span class="li-normal">choices: enable, disable</span></li>
            </ul>
        <li> <span class="li-head">name</span> - Profile name. <span class="li-normal">type: str</span> <span class="li-required">required: True</span></li>
        <li> <span class="li-head">options</span> - Options. <span class="li-normal">type: str</span> <span class="li-normal">choices: bannedword, spambwl, spamfsip, spamfssubmit, spamfschksum, spamfsurl, spamhelodns, spamraddrdns, spamrbl, spamhdrcheck, spamfsphish</span></li>
        <li> <span class="li-head">pop3</span> - POP3. <span class="li-normal">type: dict</span></li>
            <ul class="ul-self">
            <li> <span class="li-head">action</span> - Action for spam email. <span class="li-normal">type: str</span> <span class="li-normal">choices: pass, tag</span></li>
            <li> <span class="li-head">log</span> - Enable/disable logging. <span class="li-normal">type: str</span> <span class="li-normal">choices: enable, disable</span></li>
            <li> <span class="li-head">tag_msg</span> - Subject text or header added to spam email. <span class="li-normal">type: str</span></li>
            <li> <span class="li-head">tag_type</span> - Tag subject or header for spam email. <span class="li-normal">type: str</span> <span class="li-normal">choices: subject, header, spaminfo</span></li>
            </ul>
        <li> <span class="li-head">replacemsg_group</span> - Replacement message group. Source system.replacemsg-group.name. <span class="li-normal">type: str</span></li>
        <li> <span class="li-head">smtp</span> - SMTP. <span class="li-normal">type: dict</span></li>
            <ul class="ul-self">
            <li> <span class="li-head">action</span> - Action for spam email. <span class="li-normal">type: str</span> <span class="li-normal">choices: pass, tag, discard</span></li>
            <li> <span class="li-head">hdrip</span> - Enable/disable SMTP email header IP checks for spamfsip, spamrbl and spambwl filters. <span class="li-normal">type: str</span> <span class="li-normal">choices: disable, enable</span></li>
            <li> <span class="li-head">local_override</span> - Enable/disable local filter to override SMTP remote check result. <span class="li-normal">type: str</span> <span class="li-normal">choices: disable, enable</span></li>
            <li> <span class="li-head">log</span> - Enable/disable logging. <span class="li-normal">type: str</span> <span class="li-normal">choices: enable, disable</span></li>
            <li> <span class="li-head">tag_msg</span> - Subject text or header added to spam email. <span class="li-normal">type: str</span></li>
            <li> <span class="li-head">tag_type</span> - Tag subject or header for spam email. <span class="li-normal">type: str</span> <span class="li-normal">choices: subject, header, spaminfo</span></li>
            </ul>
        <li> <span class="li-head">spam_bwl_table</span> - Anti-spam black/white list table ID. Source emailfilter.bwl.id. <span class="li-normal">type: int</span></li>
        <li> <span class="li-head">spam_bword_table</span> - Anti-spam banned word table ID. Source emailfilter.bword.id. <span class="li-normal">type: int</span></li>
        <li> <span class="li-head">spam_bword_threshold</span> - Spam banned word threshold. <span class="li-normal">type: int</span></li>
        <li> <span class="li-head">spam_filtering</span> - Enable/disable spam filtering. <span class="li-normal">type: str</span> <span class="li-normal">choices: enable, disable</span></li>
        <li> <span class="li-head">spam_iptrust_table</span> - Anti-spam IP trust table ID. Source emailfilter.iptrust.id. <span class="li-normal">type: int</span></li>
        <li> <span class="li-head">spam_log</span> - Enable/disable spam logging for email filtering. <span class="li-normal">type: str</span> <span class="li-normal">choices: disable, enable</span></li>
        <li> <span class="li-head">spam_log_fortiguard_response</span> - Enable/disable logging FortiGuard spam response. <span class="li-normal">type: str</span> <span class="li-normal">choices: disable, enable</span></li>
        <li> <span class="li-head">spam_mheader_table</span> - Anti-spam MIME header table ID. Source emailfilter.mheader.id. <span class="li-normal">type: int</span></li>
        <li> <span class="li-head">spam_rbl_table</span> - Anti-spam DNSBL table ID. Source emailfilter.dnsbl.id. <span class="li-normal">type: int</span></li>
        <li> <span class="li-head">yahoo_mail</span> - Yahoo! Mail. <span class="li-normal">type: dict</span></li>
            <ul class="ul-self">
            <li> <span class="li-head">log</span> - Enable/disable logging. <span class="li-normal">type: str</span> <span class="li-normal">choices: enable, disable</span></li>
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
      - name: Configure Email Filter profiles.
        fortios_emailfilter_profile:
          vdom:  "{{ vdom }}"
          state: "present"
          access_token: "<your_own_value>"
          emailfilter_profile:
            comment: "Comment."
            external: "enable"
            feature_set: "flow"
            file_filter:
                entries:
                 -
                    action: "log"
                    comment: "Comment."
                    file_type:
                     -
                        name: "default_name_11 (source antivirus.filetype.name)"
                    filter: "<your_own_value>"
                    password_protected: "yes"
                    protocol: "smtp"
                log: "enable"
                scan_archive_contents: "enable"
                status: "enable"
            gmail:
                log: "enable"
            imap:
                action: "pass"
                log: "enable"
                tag_msg: "<your_own_value>"
                tag_type: "subject"
            mapi:
                action: "pass"
                log: "enable"
            msn_hotmail:
                log: "enable"
            name: "default_name_30"
            options: "bannedword"
            pop3:
                action: "pass"
                log: "enable"
                tag_msg: "<your_own_value>"
                tag_type: "subject"
            replacemsg_group: "<your_own_value> (source system.replacemsg-group.name)"
            smtp:
                action: "pass"
                hdrip: "disable"
                local_override: "disable"
                log: "enable"
                tag_msg: "<your_own_value>"
                tag_type: "subject"
            spam_bwl_table: "45 (source emailfilter.bwl.id)"
            spam_bword_table: "46 (source emailfilter.bword.id)"
            spam_bword_threshold: "47"
            spam_filtering: "enable"
            spam_iptrust_table: "49 (source emailfilter.iptrust.id)"
            spam_log: "disable"
            spam_log_fortiguard_response: "disable"
            spam_mheader_table: "52 (source emailfilter.mheader.id)"
            spam_rbl_table: "53 (source emailfilter.dnsbl.id)"
            yahoo_mail:
                log: "enable"
    


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